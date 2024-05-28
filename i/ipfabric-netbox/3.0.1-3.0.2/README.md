# Comparing `tmp/ipfabric_netbox-3.0.1.tar.gz` & `tmp/ipfabric_netbox-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipfabric_netbox-3.0.1.tar", last modified: Thu May 23 09:54:45 2024, max compression
+gzip compressed data, was "ipfabric_netbox-3.0.2.tar", last modified: Tue May 28 13:59:40 2024, max compression
```

## Comparing `ipfabric_netbox-3.0.1.tar` & `ipfabric_netbox-3.0.2.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 09:54:45.429791 ipfabric_netbox-3.0.1/
--rw-r--r--   0 root         (0) root         (0)       46 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1823 2024-05-23 09:54:45.429791 ipfabric_netbox-3.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1214 2024-05-23 09:54:40.000000 ipfabric_netbox-3.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 09:54:45.417791 ipfabric_netbox-3.0.1/ipfabric_netbox/
--rw-r--r--   0 root         (0) root         (0)     1468 2024-05-23 09:54:40.000000 ipfabric_netbox-3.0.1/ipfabric_netbox/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 09:54:45.417791 ipfabric_netbox-3.0.1/ipfabric_netbox/api/
--rw-r--r--   0 root         (0) root         (0)      101 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.1/ipfabric_netbox/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2684 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.1/ipfabric_netbox/api/nested_serializers.py
--rw-r--r--   0 root         (0) root         (0)     4307 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.1/ipfabric_netbox/api/serializers.py
--rw-r--r--   0 root         (0) root         (0)      948 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.1/ipfabric_netbox/api/urls.py
--rw-r--r--   0 root         (0) root         (0)     4429 2024-05-23 09:35:50.000000 ipfabric_netbox-3.0.1/ipfabric_netbox/api/views.py
--rw-r--r--   0 root         (0) root         (0)     4848 2024-04-23 10:08:08.000000 ipfabric_netbox-3.0.1/ipfabric_netbox/choices.py
--rw-r--r--   0 root         (0) root         (0)     3877 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.1/ipfabric_netbox/filtersets.py
--rw-r--r--   0 root         (0) root         (0)    43205 2024-05-23 09:35:50.000000 ipfabric_netbox-3.0.1/ipfabric_netbox/forms.py
--rw-r--r--   0 root         (0) root         (0)     2398 2024-05-23 09:35:50.000000 ipfabric_netbox-3.0.1/ipfabric_netbox/jobs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 09:54:45.421791 ipfabric_netbox-3.0.1/ipfabric_netbox/migrations/
--rw-r--r--   0 root         (0) root         (0)    13813 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.1/ipfabric_netbox/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)      431 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.1/ipfabric_netbox/migrations/0002_ipfabricsnapshot_status.py
--rw-r--r--   0 root         (0) root         (0)     1579 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.1/ipfabric_netbox/migrations/0003_ipfabricsource_type_and_more.py
--rw-r--r--   0 root         (0) root         (0)      435 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.1/ipfabric_netbox/migrations/0004_ipfabricsync_auto_merge.py
--rw-r--r--   0 root         (0) root         (0)     2802 2024-05-23 09:35:50.000000 ipfabric_netbox-3.0.1/ipfabric_netbox/migrations/0005_alter_ipfabricrelationshipfield_source_model_and_more.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.1/ipfabric_netbox/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29555 2024-05-23 09:35:50.000000 ipfabric_netbox-3.0.1/ipfabric_netbox/models.py
--rw-r--r--   0 root         (0) root         (0)     1735 2024-05-23 09:35:50.000000 ipfabric_netbox-3.0.1/ipfabric_netbox/navigation.py
--rw-r--r--   0 root         (0) root         (0)     2588 2024-05-23 09:35:50.000000 ipfabric_netbox-3.0.1/ipfabric_netbox/signals.py
--rw-r--r--   0 root         (0) root         (0)     6613 2024-05-23 09:35:50.000000 ipfabric_netbox-3.0.1/ipfabric_netbox/tables.py
--rw-r--r--   0 root         (0) root         (0)      315 2024-03-08 10:45:55.000000 ipfabric_netbox-3.0.1/ipfabric_netbox/template_content.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 09:54:45.409791 ipfabric_netbox-3.0.1/ipfabric_netbox/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 09:54:45.421791 ipfabric_netbox-3.0.1/ipfabric_netbox/templates/ipfabric_netbox/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 09:54:45.425791 ipfabric_netbox-3.0.1/ipfabric_netbox/templates/ipfabric_netbox/inc/
--rw-r--r--   0 root         (0) root         (0)     3229 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.1/ipfabric_netbox/templates/ipfabric_netbox/inc/diff.html
--rw-r--r--   0 root         (0) root         (0)      569 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.1/ipfabric_netbox/templates/ipfabric_netbox/inc/json.html
--rw-r--r--   0 root         (0) root         (0)      295 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.1/ipfabric_netbox/templates/ipfabric_netbox/inc/logs_pending.html
--rw-r--r--   0 root         (0) root         (0)      710 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.1/ipfabric_netbox/templates/ipfabric_netbox/inc/merge_form.html
--rw-r--r--   0 root         (0) root         (0)     2674 2024-03-18 10:24:22.000000 ipfabric_netbox-3.0.1/ipfabric_netbox/templates/ipfabric_netbox/inc/site_topology_button.html
--rw-r--r--   0 root         (0) root         (0)     2124 2024-05-23 09:35:50.000000 ipfabric_netbox-3.0.1/ipfabric_netbox/templates/ipfabric_netbox/inc/site_topology_modal.html
--rw-r--r--   0 root         (0) root         (0)     2885 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.1/ipfabric_netbox/templates/ipfabric_netbox/inc/snapshotdata.html
--rw-r--r--   0 root         (0) root         (0)      717 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.1/ipfabric_netbox/templates/ipfabric_netbox/inc/sync_delete.html
--rw-r--r--   0 root         (0) root         (0)      500 2024-05-23 09:35:50.000000 ipfabric_netbox-3.0.1/ipfabric_netbox/templates/ipfabric_netbox/inc/transform_map_field_map.html
--rw-r--r--   0 root         (0) root         (0)      504 2024-05-23 09:35:50.000000 ipfabric_netbox-3.0.1/ipfabric_netbox/templates/ipfabric_netbox/inc/transform_map_relationship_map.html
--rw-r--r--   0 root         (0) root         (0)     1631 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.1/ipfabric_netbox/templates/ipfabric_netbox/ipfabric_table.html
--rw-r--r--   0 root         (0) root         (0)     4694 2024-05-23 09:35:50.000000 ipfabric_netbox-3.0.1/ipfabric_netbox/templates/ipfabric_netbox/ipfabricbranch.html
--rw-r--r--   0 root         (0) root         (0)     3482 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.1/ipfabric_netbox/templates/ipfabric_netbox/ipfabricsnapshot.html
--rw-r--r--   0 root         (0) root         (0)     3845 2024-05-23 09:35:50.000000 ipfabric_netbox-3.0.1/ipfabric_netbox/templates/ipfabric_netbox/ipfabricsource.html
--rw-r--r--   0 root         (0) root         (0)     3725 2024-05-23 09:54:40.000000 ipfabric_netbox-3.0.1/ipfabric_netbox/templates/ipfabric_netbox/ipfabricsync.html
--rw-r--r--   0 root         (0) root         (0)     1100 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.1/ipfabric_netbox/templates/ipfabric_netbox/ipfabrictransformmap.html
--rw-r--r--   0 root         (0) root         (0)      452 2024-05-23 09:35:50.000000 ipfabric_netbox-3.0.1/ipfabric_netbox/templates/ipfabric_netbox/ipfabrictransformmap_list.html
--rw-r--r--   0 root         (0) root         (0)     2562 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.1/ipfabric_netbox/templates/ipfabric_netbox/ipfabrictransformmap_restore.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 09:54:45.425791 ipfabric_netbox-3.0.1/ipfabric_netbox/templates/ipfabric_netbox/partials/
--rw-r--r--   0 root         (0) root         (0)      368 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.1/ipfabric_netbox/templates/ipfabric_netbox/partials/branch_all.html
--rw-r--r--   0 root         (0) root         (0)      590 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.1/ipfabric_netbox/templates/ipfabric_netbox/partials/branch_progress.html
--rw-r--r--   0 root         (0) root         (0)       81 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.1/ipfabric_netbox/templates/ipfabric_netbox/partials/branch_status.html
--rw-r--r--   0 root         (0) root         (0)     1622 2024-05-23 09:35:50.000000 ipfabric_netbox-3.0.1/ipfabric_netbox/templates/ipfabric_netbox/partials/job_logs.html
--rw-r--r--   0 root         (0) root         (0)      167 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.1/ipfabric_netbox/templates/ipfabric_netbox/partials/sync_last_branch.html
--rw-r--r--   0 root         (0) root         (0)     5587 2024-05-23 09:35:50.000000 ipfabric_netbox-3.0.1/ipfabric_netbox/templates/ipfabric_netbox/sync_list.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 09:54:45.409791 ipfabric_netbox-3.0.1/ipfabric_netbox/templates/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 09:54:45.409791 ipfabric_netbox-3.0.1/ipfabric_netbox/templates/static/ipfabric_netbox/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 09:54:45.425791 ipfabric_netbox-3.0.1/ipfabric_netbox/templates/static/ipfabric_netbox/css/
--rw-r--r--   0 root         (0) root         (0)      118 2024-03-11 10:17:28.000000 ipfabric_netbox-3.0.1/ipfabric_netbox/templates/static/ipfabric_netbox/css/rack.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 09:54:45.425791 ipfabric_netbox-3.0.1/ipfabric_netbox/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.1/ipfabric_netbox/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45898 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.1/ipfabric_netbox/tests/test_models.py
--rw-r--r--   0 root         (0) root         (0)     4430 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.1/ipfabric_netbox/urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 09:54:45.429791 ipfabric_netbox-3.0.1/ipfabric_netbox/utilities/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.1/ipfabric_netbox/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20437 2024-05-23 09:35:50.000000 ipfabric_netbox-3.0.1/ipfabric_netbox/utilities/ipfutils.py
--rw-r--r--   0 root         (0) root         (0)     3221 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.1/ipfabric_netbox/utilities/logging.py
--rw-r--r--   0 root         (0) root         (0)     3117 2024-05-23 09:35:50.000000 ipfabric_netbox-3.0.1/ipfabric_netbox/utilities/nbutils.py
--rw-r--r--   0 root         (0) root         (0)     1256 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.1/ipfabric_netbox/utilities/transform_map.py
--rw-r--r--   0 root         (0) root         (0)    28452 2024-05-23 09:35:50.000000 ipfabric_netbox-3.0.1/ipfabric_netbox/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 09:54:45.429791 ipfabric_netbox-3.0.1/ipfabric_netbox.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1823 2024-05-23 09:54:45.000000 ipfabric_netbox-3.0.1/ipfabric_netbox.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3031 2024-05-23 09:54:45.000000 ipfabric_netbox-3.0.1/ipfabric_netbox.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 09:54:45.000000 ipfabric_netbox-3.0.1/ipfabric_netbox.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-20 17:00:30.000000 ipfabric_netbox-3.0.1/ipfabric_netbox.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       25 2024-05-23 09:54:45.000000 ipfabric_netbox-3.0.1/ipfabric_netbox.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-05-23 09:54:45.000000 ipfabric_netbox-3.0.1/ipfabric_netbox.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-23 09:54:45.429791 ipfabric_netbox-3.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      961 2024-05-23 09:54:40.000000 ipfabric_netbox-3.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 13:59:40.056939 ipfabric_netbox-3.0.2/
+-rw-r--r--   0 root         (0) root         (0)       46 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1823 2024-05-28 13:59:40.056939 ipfabric_netbox-3.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1214 2024-05-23 09:54:40.000000 ipfabric_netbox-3.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 13:59:40.024939 ipfabric_netbox-3.0.2/ipfabric_netbox/
+-rw-r--r--   0 root         (0) root         (0)     1468 2024-05-28 13:59:33.000000 ipfabric_netbox-3.0.2/ipfabric_netbox/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 13:59:40.032939 ipfabric_netbox-3.0.2/ipfabric_netbox/api/
+-rw-r--r--   0 root         (0) root         (0)      101 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.2/ipfabric_netbox/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2684 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.2/ipfabric_netbox/api/nested_serializers.py
+-rw-r--r--   0 root         (0) root         (0)     4307 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.2/ipfabric_netbox/api/serializers.py
+-rw-r--r--   0 root         (0) root         (0)      948 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.2/ipfabric_netbox/api/urls.py
+-rw-r--r--   0 root         (0) root         (0)     4429 2024-05-23 09:35:50.000000 ipfabric_netbox-3.0.2/ipfabric_netbox/api/views.py
+-rw-r--r--   0 root         (0) root         (0)     4848 2024-04-23 10:08:08.000000 ipfabric_netbox-3.0.2/ipfabric_netbox/choices.py
+-rw-r--r--   0 root         (0) root         (0)     3877 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.2/ipfabric_netbox/filtersets.py
+-rw-r--r--   0 root         (0) root         (0)    43205 2024-05-23 09:35:50.000000 ipfabric_netbox-3.0.2/ipfabric_netbox/forms.py
+-rw-r--r--   0 root         (0) root         (0)     2862 2024-05-28 13:59:33.000000 ipfabric_netbox-3.0.2/ipfabric_netbox/jobs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 13:59:40.036939 ipfabric_netbox-3.0.2/ipfabric_netbox/migrations/
+-rw-r--r--   0 root         (0) root         (0)    13813 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.2/ipfabric_netbox/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)      431 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.2/ipfabric_netbox/migrations/0002_ipfabricsnapshot_status.py
+-rw-r--r--   0 root         (0) root         (0)     1579 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.2/ipfabric_netbox/migrations/0003_ipfabricsource_type_and_more.py
+-rw-r--r--   0 root         (0) root         (0)      435 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.2/ipfabric_netbox/migrations/0004_ipfabricsync_auto_merge.py
+-rw-r--r--   0 root         (0) root         (0)     2802 2024-05-23 09:35:50.000000 ipfabric_netbox-3.0.2/ipfabric_netbox/migrations/0005_alter_ipfabricrelationshipfield_source_model_and_more.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.2/ipfabric_netbox/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30058 2024-05-28 13:59:33.000000 ipfabric_netbox-3.0.2/ipfabric_netbox/models.py
+-rw-r--r--   0 root         (0) root         (0)     1735 2024-05-23 09:35:50.000000 ipfabric_netbox-3.0.2/ipfabric_netbox/navigation.py
+-rw-r--r--   0 root         (0) root         (0)     2588 2024-05-23 09:35:50.000000 ipfabric_netbox-3.0.2/ipfabric_netbox/signals.py
+-rw-r--r--   0 root         (0) root         (0)     6613 2024-05-23 09:35:50.000000 ipfabric_netbox-3.0.2/ipfabric_netbox/tables.py
+-rw-r--r--   0 root         (0) root         (0)      315 2024-03-08 10:45:55.000000 ipfabric_netbox-3.0.2/ipfabric_netbox/template_content.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 13:59:40.016939 ipfabric_netbox-3.0.2/ipfabric_netbox/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 13:59:40.040939 ipfabric_netbox-3.0.2/ipfabric_netbox/templates/ipfabric_netbox/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 13:59:40.048939 ipfabric_netbox-3.0.2/ipfabric_netbox/templates/ipfabric_netbox/inc/
+-rw-r--r--   0 root         (0) root         (0)     3229 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.2/ipfabric_netbox/templates/ipfabric_netbox/inc/diff.html
+-rw-r--r--   0 root         (0) root         (0)      569 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.2/ipfabric_netbox/templates/ipfabric_netbox/inc/json.html
+-rw-r--r--   0 root         (0) root         (0)      295 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.2/ipfabric_netbox/templates/ipfabric_netbox/inc/logs_pending.html
+-rw-r--r--   0 root         (0) root         (0)      710 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.2/ipfabric_netbox/templates/ipfabric_netbox/inc/merge_form.html
+-rw-r--r--   0 root         (0) root         (0)     2674 2024-03-18 10:24:22.000000 ipfabric_netbox-3.0.2/ipfabric_netbox/templates/ipfabric_netbox/inc/site_topology_button.html
+-rw-r--r--   0 root         (0) root         (0)     2124 2024-05-23 09:35:50.000000 ipfabric_netbox-3.0.2/ipfabric_netbox/templates/ipfabric_netbox/inc/site_topology_modal.html
+-rw-r--r--   0 root         (0) root         (0)     2885 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.2/ipfabric_netbox/templates/ipfabric_netbox/inc/snapshotdata.html
+-rw-r--r--   0 root         (0) root         (0)      717 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.2/ipfabric_netbox/templates/ipfabric_netbox/inc/sync_delete.html
+-rw-r--r--   0 root         (0) root         (0)      500 2024-05-23 09:35:50.000000 ipfabric_netbox-3.0.2/ipfabric_netbox/templates/ipfabric_netbox/inc/transform_map_field_map.html
+-rw-r--r--   0 root         (0) root         (0)      504 2024-05-23 09:35:50.000000 ipfabric_netbox-3.0.2/ipfabric_netbox/templates/ipfabric_netbox/inc/transform_map_relationship_map.html
+-rw-r--r--   0 root         (0) root         (0)     1631 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.2/ipfabric_netbox/templates/ipfabric_netbox/ipfabric_table.html
+-rw-r--r--   0 root         (0) root         (0)     4694 2024-05-23 09:35:50.000000 ipfabric_netbox-3.0.2/ipfabric_netbox/templates/ipfabric_netbox/ipfabricbranch.html
+-rw-r--r--   0 root         (0) root         (0)     3482 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.2/ipfabric_netbox/templates/ipfabric_netbox/ipfabricsnapshot.html
+-rw-r--r--   0 root         (0) root         (0)     3845 2024-05-23 09:35:50.000000 ipfabric_netbox-3.0.2/ipfabric_netbox/templates/ipfabric_netbox/ipfabricsource.html
+-rw-r--r--   0 root         (0) root         (0)     3725 2024-05-23 09:54:40.000000 ipfabric_netbox-3.0.2/ipfabric_netbox/templates/ipfabric_netbox/ipfabricsync.html
+-rw-r--r--   0 root         (0) root         (0)     1100 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.2/ipfabric_netbox/templates/ipfabric_netbox/ipfabrictransformmap.html
+-rw-r--r--   0 root         (0) root         (0)      452 2024-05-23 09:35:50.000000 ipfabric_netbox-3.0.2/ipfabric_netbox/templates/ipfabric_netbox/ipfabrictransformmap_list.html
+-rw-r--r--   0 root         (0) root         (0)     2562 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.2/ipfabric_netbox/templates/ipfabric_netbox/ipfabrictransformmap_restore.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 13:59:40.048939 ipfabric_netbox-3.0.2/ipfabric_netbox/templates/ipfabric_netbox/partials/
+-rw-r--r--   0 root         (0) root         (0)      368 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.2/ipfabric_netbox/templates/ipfabric_netbox/partials/branch_all.html
+-rw-r--r--   0 root         (0) root         (0)      590 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.2/ipfabric_netbox/templates/ipfabric_netbox/partials/branch_progress.html
+-rw-r--r--   0 root         (0) root         (0)       81 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.2/ipfabric_netbox/templates/ipfabric_netbox/partials/branch_status.html
+-rw-r--r--   0 root         (0) root         (0)     1622 2024-05-23 09:35:50.000000 ipfabric_netbox-3.0.2/ipfabric_netbox/templates/ipfabric_netbox/partials/job_logs.html
+-rw-r--r--   0 root         (0) root         (0)      167 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.2/ipfabric_netbox/templates/ipfabric_netbox/partials/sync_last_branch.html
+-rw-r--r--   0 root         (0) root         (0)     5587 2024-05-23 09:35:50.000000 ipfabric_netbox-3.0.2/ipfabric_netbox/templates/ipfabric_netbox/sync_list.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 13:59:40.016939 ipfabric_netbox-3.0.2/ipfabric_netbox/templates/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 13:59:40.016939 ipfabric_netbox-3.0.2/ipfabric_netbox/templates/static/ipfabric_netbox/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 13:59:40.048939 ipfabric_netbox-3.0.2/ipfabric_netbox/templates/static/ipfabric_netbox/css/
+-rw-r--r--   0 root         (0) root         (0)      118 2024-03-11 10:17:28.000000 ipfabric_netbox-3.0.2/ipfabric_netbox/templates/static/ipfabric_netbox/css/rack.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 13:59:40.052939 ipfabric_netbox-3.0.2/ipfabric_netbox/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.2/ipfabric_netbox/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45898 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.2/ipfabric_netbox/tests/test_models.py
+-rw-r--r--   0 root         (0) root         (0)     4430 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.2/ipfabric_netbox/urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 13:59:40.056939 ipfabric_netbox-3.0.2/ipfabric_netbox/utilities/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.2/ipfabric_netbox/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20437 2024-05-23 09:35:50.000000 ipfabric_netbox-3.0.2/ipfabric_netbox/utilities/ipfutils.py
+-rw-r--r--   0 root         (0) root         (0)     3221 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.2/ipfabric_netbox/utilities/logging.py
+-rw-r--r--   0 root         (0) root         (0)     3117 2024-05-23 09:35:50.000000 ipfabric_netbox-3.0.2/ipfabric_netbox/utilities/nbutils.py
+-rw-r--r--   0 root         (0) root         (0)     1256 2024-02-20 16:51:44.000000 ipfabric_netbox-3.0.2/ipfabric_netbox/utilities/transform_map.py
+-rw-r--r--   0 root         (0) root         (0)    28452 2024-05-23 10:10:35.000000 ipfabric_netbox-3.0.2/ipfabric_netbox/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 13:59:40.056939 ipfabric_netbox-3.0.2/ipfabric_netbox.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1823 2024-05-28 13:59:39.000000 ipfabric_netbox-3.0.2/ipfabric_netbox.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3031 2024-05-28 13:59:40.000000 ipfabric_netbox-3.0.2/ipfabric_netbox.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 13:59:39.000000 ipfabric_netbox-3.0.2/ipfabric_netbox.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-02-20 17:00:30.000000 ipfabric_netbox-3.0.2/ipfabric_netbox.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       25 2024-05-28 13:59:39.000000 ipfabric_netbox-3.0.2/ipfabric_netbox.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-05-28 13:59:39.000000 ipfabric_netbox-3.0.2/ipfabric_netbox.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 13:59:40.056939 ipfabric_netbox-3.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      961 2024-05-28 13:59:33.000000 ipfabric_netbox-3.0.2/setup.py
```

### Comparing `ipfabric_netbox-3.0.1/PKG-INFO` & `ipfabric_netbox-3.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipfabric_netbox
-Version: 3.0.1
+Version: 3.0.2
 Summary: NetBox plugin to sync IP Fabric data into NetBox
 Home-page: https://gitlab.com/ip-fabric/integrations/ipfabric-netbox-sync
 Author: Solution Architecture
 Author-email: solution.architecture@ipfabric.io
 Project-URL: Bug Tracker, https://gitlab.com/ip-fabric/integrations/ipfabric-netbox-sync/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ipfabric_netbox-3.0.1/README.md` & `ipfabric_netbox-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-3.0.1/ipfabric_netbox/__init__.py` & `ipfabric_netbox-3.0.2/ipfabric_netbox/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from netbox.plugins import PluginConfig
 
 
 class NetboxIPFabricConfig(PluginConfig):
     name = "ipfabric_netbox"
     verbose_name = "NetBox IP Fabric SoT Plugin"
     description = "Sync IP Fabric into NetBox"
-    version = "3.0.1"
+    version = "3.0.2"
     base_url = "ipfabric"
 
     def ready(self):
         super().ready()
         try:
             from ipfabric_netbox.signals import ipfabric_netbox_init
```

### Comparing `ipfabric_netbox-3.0.1/ipfabric_netbox/api/nested_serializers.py` & `ipfabric_netbox-3.0.2/ipfabric_netbox/api/nested_serializers.py`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-3.0.1/ipfabric_netbox/api/serializers.py` & `ipfabric_netbox-3.0.2/ipfabric_netbox/api/serializers.py`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-3.0.1/ipfabric_netbox/api/urls.py` & `ipfabric_netbox-3.0.2/ipfabric_netbox/api/urls.py`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-3.0.1/ipfabric_netbox/api/views.py` & `ipfabric_netbox-3.0.2/ipfabric_netbox/api/views.py`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-3.0.1/ipfabric_netbox/choices.py` & `ipfabric_netbox-3.0.2/ipfabric_netbox/choices.py`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-3.0.1/ipfabric_netbox/filtersets.py` & `ipfabric_netbox-3.0.2/ipfabric_netbox/filtersets.py`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-3.0.1/ipfabric_netbox/forms.py` & `ipfabric_netbox-3.0.2/ipfabric_netbox/forms.py`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-3.0.1/ipfabric_netbox/migrations/0001_initial.py` & `ipfabric_netbox-3.0.2/ipfabric_netbox/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-3.0.1/ipfabric_netbox/migrations/0003_ipfabricsource_type_and_more.py` & `ipfabric_netbox-3.0.2/ipfabric_netbox/migrations/0003_ipfabricsource_type_and_more.py`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-3.0.1/ipfabric_netbox/migrations/0005_alter_ipfabricrelationshipfield_source_model_and_more.py` & `ipfabric_netbox-3.0.2/ipfabric_netbox/migrations/0005_alter_ipfabricrelationshipfield_source_model_and_more.py`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-3.0.1/ipfabric_netbox/models.py` & `ipfabric_netbox-3.0.2/ipfabric_netbox/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,21 +13,24 @@
 from dcim.signals import assign_virtualchassis_master
 from django.apps import apps
 from django.conf import settings
 from django.contrib.contenttypes.models import ContentType
 from django.core.cache import cache
 from django.core.validators import MinValueValidator
 from django.db import models
+from django.db import transaction
 from django.db.models import Q
 from django.db.models import signals
 from django.urls import reverse
 from django.utils import timezone
 from django.utils.module_loading import import_string
 from django.utils.translation import gettext as _
 from extras.models import Branch
+from extras.models import StagedChange
+from extras.signals import handle_deleted_object
 from netbox.models import ChangeLoggedModel
 from netbox.models import NetBoxModel
 from netbox.models import PrimaryModel
 from netbox.models.features import JobsMixin
 from netbox.models.features import TagsMixin
 from netbox.registry import registry
 from netbox.staging import checkout
@@ -801,14 +804,23 @@
             for model, stats in job_results["statistics"].items():
                 if stats["total"] > 0:
                     statistics[model] = stats["current"] / stats["total"] * 100
                 else:
                     statistics[model] = stats["current"] / 1 * 100
         return {"job_results": job_results, "statistics": statistics}
 
+    def merge(self):
+        logger.info(f"Merging changes in branch {self}")
+        with transaction.atomic():
+            for change in self.staged_changes.all():
+                change.apply()
+        signals.pre_delete.disconnect(handle_deleted_object)
+        self.staged_changes.all().delete()
+        signals.pre_delete.connect(handle_deleted_object, sender=StagedChange)
+
     def sync_merge(self):
         ipfabricsync = self.sync
         if ipfabricsync.status == DataSourceStatusChoices.SYNCING:
             raise SyncError("Cannot initiate merge; merge already in progress.")
 
         pre_sync.send(sender=self.__class__, instance=self)
```

### Comparing `ipfabric_netbox-3.0.1/ipfabric_netbox/navigation.py` & `ipfabric_netbox-3.0.2/ipfabric_netbox/navigation.py`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-3.0.1/ipfabric_netbox/signals.py` & `ipfabric_netbox-3.0.2/ipfabric_netbox/signals.py`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-3.0.1/ipfabric_netbox/tables.py` & `ipfabric_netbox-3.0.2/ipfabric_netbox/tables.py`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-3.0.1/ipfabric_netbox/templates/ipfabric_netbox/inc/diff.html` & `ipfabric_netbox-3.0.2/ipfabric_netbox/templates/ipfabric_netbox/inc/diff.html`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-3.0.1/ipfabric_netbox/templates/ipfabric_netbox/inc/json.html` & `ipfabric_netbox-3.0.2/ipfabric_netbox/templates/ipfabric_netbox/inc/json.html`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-3.0.1/ipfabric_netbox/templates/ipfabric_netbox/inc/merge_form.html` & `ipfabric_netbox-3.0.2/ipfabric_netbox/templates/ipfabric_netbox/inc/merge_form.html`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-3.0.1/ipfabric_netbox/templates/ipfabric_netbox/inc/site_topology_button.html` & `ipfabric_netbox-3.0.2/ipfabric_netbox/templates/ipfabric_netbox/inc/site_topology_button.html`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-3.0.1/ipfabric_netbox/templates/ipfabric_netbox/inc/site_topology_modal.html` & `ipfabric_netbox-3.0.2/ipfabric_netbox/templates/ipfabric_netbox/inc/site_topology_modal.html`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-3.0.1/ipfabric_netbox/templates/ipfabric_netbox/inc/snapshotdata.html` & `ipfabric_netbox-3.0.2/ipfabric_netbox/templates/ipfabric_netbox/inc/snapshotdata.html`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-3.0.1/ipfabric_netbox/templates/ipfabric_netbox/inc/sync_delete.html` & `ipfabric_netbox-3.0.2/ipfabric_netbox/templates/ipfabric_netbox/inc/sync_delete.html`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-3.0.1/ipfabric_netbox/templates/ipfabric_netbox/ipfabric_table.html` & `ipfabric_netbox-3.0.2/ipfabric_netbox/templates/ipfabric_netbox/ipfabric_table.html`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-3.0.1/ipfabric_netbox/templates/ipfabric_netbox/ipfabricbranch.html` & `ipfabric_netbox-3.0.2/ipfabric_netbox/templates/ipfabric_netbox/ipfabricbranch.html`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-3.0.1/ipfabric_netbox/templates/ipfabric_netbox/ipfabricsnapshot.html` & `ipfabric_netbox-3.0.2/ipfabric_netbox/templates/ipfabric_netbox/ipfabricsnapshot.html`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-3.0.1/ipfabric_netbox/templates/ipfabric_netbox/ipfabricsource.html` & `ipfabric_netbox-3.0.2/ipfabric_netbox/templates/ipfabric_netbox/ipfabricsource.html`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-3.0.1/ipfabric_netbox/templates/ipfabric_netbox/ipfabricsync.html` & `ipfabric_netbox-3.0.2/ipfabric_netbox/templates/ipfabric_netbox/ipfabricsync.html`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-3.0.1/ipfabric_netbox/templates/ipfabric_netbox/ipfabrictransformmap.html` & `ipfabric_netbox-3.0.2/ipfabric_netbox/templates/ipfabric_netbox/ipfabrictransformmap.html`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-3.0.1/ipfabric_netbox/templates/ipfabric_netbox/ipfabrictransformmap_restore.html` & `ipfabric_netbox-3.0.2/ipfabric_netbox/templates/ipfabric_netbox/ipfabrictransformmap_restore.html`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-3.0.1/ipfabric_netbox/templates/ipfabric_netbox/partials/branch_progress.html` & `ipfabric_netbox-3.0.2/ipfabric_netbox/templates/ipfabric_netbox/partials/branch_progress.html`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-3.0.1/ipfabric_netbox/templates/ipfabric_netbox/partials/job_logs.html` & `ipfabric_netbox-3.0.2/ipfabric_netbox/templates/ipfabric_netbox/partials/job_logs.html`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-3.0.1/ipfabric_netbox/templates/ipfabric_netbox/sync_list.html` & `ipfabric_netbox-3.0.2/ipfabric_netbox/templates/ipfabric_netbox/sync_list.html`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-3.0.1/ipfabric_netbox/tests/test_models.py` & `ipfabric_netbox-3.0.2/ipfabric_netbox/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-3.0.1/ipfabric_netbox/urls.py` & `ipfabric_netbox-3.0.2/ipfabric_netbox/urls.py`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-3.0.1/ipfabric_netbox/utilities/ipfutils.py` & `ipfabric_netbox-3.0.2/ipfabric_netbox/utilities/ipfutils.py`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-3.0.1/ipfabric_netbox/utilities/logging.py` & `ipfabric_netbox-3.0.2/ipfabric_netbox/utilities/logging.py`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-3.0.1/ipfabric_netbox/utilities/nbutils.py` & `ipfabric_netbox-3.0.2/ipfabric_netbox/utilities/nbutils.py`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-3.0.1/ipfabric_netbox/utilities/transform_map.py` & `ipfabric_netbox-3.0.2/ipfabric_netbox/utilities/transform_map.py`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-3.0.1/ipfabric_netbox/views.py` & `ipfabric_netbox-3.0.2/ipfabric_netbox/views.py`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-3.0.1/ipfabric_netbox.egg-info/PKG-INFO` & `ipfabric_netbox-3.0.2/ipfabric_netbox.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipfabric_netbox
-Version: 3.0.1
+Version: 3.0.2
 Summary: NetBox plugin to sync IP Fabric data into NetBox
 Home-page: https://gitlab.com/ip-fabric/integrations/ipfabric-netbox-sync
 Author: Solution Architecture
 Author-email: solution.architecture@ipfabric.io
 Project-URL: Bug Tracker, https://gitlab.com/ip-fabric/integrations/ipfabric-netbox-sync/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ipfabric_netbox-3.0.1/ipfabric_netbox.egg-info/SOURCES.txt` & `ipfabric_netbox-3.0.2/ipfabric_netbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-3.0.1/setup.py` & `ipfabric_netbox-3.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="ipfabric_netbox",
-    version="3.0.1",
+    version="3.0.2",
     author="Solution Architecture",
     author_email="solution.architecture@ipfabric.io",
     description="NetBox plugin to sync IP Fabric data into NetBox",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=["ipfabric>=6.6.4", "netutils"],
     url="https://gitlab.com/ip-fabric/integrations/ipfabric-netbox-sync",
```

