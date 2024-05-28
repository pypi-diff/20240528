# Comparing `tmp/google-cloud-gke-backup-0.5.8.tar.gz` & `tmp/google-cloud-gke-backup-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-gke-backup-0.5.8.tar", last modified: Tue Mar 26 15:43:56 2024, max compression
+gzip compressed data, was "google-cloud-gke-backup-0.5.9.tar", last modified: Tue May 28 08:23:46 2024, max compression
```

## Comparing `google-cloud-gke-backup-0.5.8.tar` & `google-cloud-gke-backup-0.5.9.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-26 15:43:56.719729 google-cloud-gke-backup-0.5.8/
--rw-rw-r--   0 root         (0)     1003    11358 2024-03-26 15:41:08.000000 google-cloud-gke-backup-0.5.8/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2024-03-26 15:41:08.000000 google-cloud-gke-backup-0.5.8/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     5363 2024-03-26 15:43:56.719729 google-cloud-gke-backup-0.5.8/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3938 2024-03-26 15:41:08.000000 google-cloud-gke-backup-0.5.8/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-26 15:43:56.703731 google-cloud-gke-backup-0.5.8/google/
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-26 15:43:56.703731 google-cloud-gke-backup-0.5.8/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-26 15:43:56.707731 google-cloud-gke-backup-0.5.8/google/cloud/gke_backup/
--rw-rw-r--   0 root         (0)     1003     3741 2024-03-26 15:41:08.000000 google-cloud-gke-backup-0.5.8/google/cloud/gke_backup/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2024-03-26 15:41:08.000000 google-cloud-gke-backup-0.5.8/google/cloud/gke_backup/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       84 2024-03-26 15:41:08.000000 google-cloud-gke-backup-0.5.8/google/cloud/gke_backup/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-26 15:43:56.707731 google-cloud-gke-backup-0.5.8/google/cloud/gke_backup_v1/
--rw-rw-r--   0 root         (0)     1003     3407 2024-03-26 15:41:08.000000 google-cloud-gke-backup-0.5.8/google/cloud/gke_backup_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    10094 2024-03-26 15:41:08.000000 google-cloud-gke-backup-0.5.8/google/cloud/gke_backup_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2024-03-26 15:41:08.000000 google-cloud-gke-backup-0.5.8/google/cloud/gke_backup_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       84 2024-03-26 15:41:08.000000 google-cloud-gke-backup-0.5.8/google/cloud/gke_backup_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-26 15:43:56.707731 google-cloud-gke-backup-0.5.8/google/cloud/gke_backup_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-26 15:41:08.000000 google-cloud-gke-backup-0.5.8/google/cloud/gke_backup_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-26 15:43:56.711730 google-cloud-gke-backup-0.5.8/google/cloud/gke_backup_v1/services/backup_for_gke/
--rw-rw-r--   0 root         (0)     1003      761 2024-03-26 15:41:08.000000 google-cloud-gke-backup-0.5.8/google/cloud/gke_backup_v1/services/backup_for_gke/__init__.py
--rw-rw-r--   0 root         (0)     1003   169562 2024-03-26 15:41:08.000000 google-cloud-gke-backup-0.5.8/google/cloud/gke_backup_v1/services/backup_for_gke/async_client.py
--rw-rw-r--   0 root         (0)     1003   189452 2024-03-26 15:41:08.000000 google-cloud-gke-backup-0.5.8/google/cloud/gke_backup_v1/services/backup_for_gke/client.py
--rw-rw-r--   0 root         (0)     1003    31038 2024-03-26 15:41:08.000000 google-cloud-gke-backup-0.5.8/google/cloud/gke_backup_v1/services/backup_for_gke/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-26 15:43:56.711730 google-cloud-gke-backup-0.5.8/google/cloud/gke_backup_v1/services/backup_for_gke/transports/
--rw-rw-r--   0 root         (0)     1003     1372 2024-03-26 15:41:08.000000 google-cloud-gke-backup-0.5.8/google/cloud/gke_backup_v1/services/backup_for_gke/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    23950 2024-03-26 15:41:08.000000 google-cloud-gke-backup-0.5.8/google/cloud/gke_backup_v1/services/backup_for_gke/transports/base.py
--rw-rw-r--   0 root         (0)     1003    48348 2024-03-26 15:41:08.000000 google-cloud-gke-backup-0.5.8/google/cloud/gke_backup_v1/services/backup_for_gke/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    49349 2024-03-26 15:41:08.000000 google-cloud-gke-backup-0.5.8/google/cloud/gke_backup_v1/services/backup_for_gke/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   170171 2024-03-26 15:41:08.000000 google-cloud-gke-backup-0.5.8/google/cloud/gke_backup_v1/services/backup_for_gke/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-26 15:43:56.715730 google-cloud-gke-backup-0.5.8/google/cloud/gke_backup_v1/types/
--rw-rw-r--   0 root         (0)     1003     3110 2024-03-26 15:41:08.000000 google-cloud-gke-backup-0.5.8/google/cloud/gke_backup_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    14320 2024-03-26 15:41:08.000000 google-cloud-gke-backup-0.5.8/google/cloud/gke_backup_v1/types/backup.py
--rw-rw-r--   0 root         (0)     1003    20891 2024-03-26 15:41:08.000000 google-cloud-gke-backup-0.5.8/google/cloud/gke_backup_v1/types/backup_plan.py
--rw-rw-r--   0 root         (0)     1003     2606 2024-03-26 15:41:08.000000 google-cloud-gke-backup-0.5.8/google/cloud/gke_backup_v1/types/common.py
--rw-rw-r--   0 root         (0)     1003    37714 2024-03-26 15:41:08.000000 google-cloud-gke-backup-0.5.8/google/cloud/gke_backup_v1/types/gkebackup.py
--rw-rw-r--   0 root         (0)     1003    33489 2024-03-26 15:41:08.000000 google-cloud-gke-backup-0.5.8/google/cloud/gke_backup_v1/types/restore.py
--rw-rw-r--   0 root         (0)     1003     5912 2024-03-26 15:41:08.000000 google-cloud-gke-backup-0.5.8/google/cloud/gke_backup_v1/types/restore_plan.py
--rw-rw-r--   0 root         (0)     1003    12208 2024-03-26 15:41:08.000000 google-cloud-gke-backup-0.5.8/google/cloud/gke_backup_v1/types/volume.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-26 15:43:56.715730 google-cloud-gke-backup-0.5.8/google_cloud_gke_backup.egg-info/
--rw-r--r--   0 root         (0)     1003     5363 2024-03-26 15:43:56.000000 google-cloud-gke-backup-0.5.8/google_cloud_gke_backup.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1795 2024-03-26 15:43:56.000000 google-cloud-gke-backup-0.5.8/google_cloud_gke_backup.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2024-03-26 15:43:56.000000 google-cloud-gke-backup-0.5.8/google_cloud_gke_backup.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003        1 2024-03-26 15:43:56.000000 google-cloud-gke-backup-0.5.8/google_cloud_gke_backup.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      342 2024-03-26 15:43:56.000000 google-cloud-gke-backup-0.5.8/google_cloud_gke_backup.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2024-03-26 15:43:56.000000 google-cloud-gke-backup-0.5.8/google_cloud_gke_backup.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2024-03-26 15:43:56.719729 google-cloud-gke-backup-0.5.8/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3222 2024-03-26 15:41:08.000000 google-cloud-gke-backup-0.5.8/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-26 15:43:56.715730 google-cloud-gke-backup-0.5.8/tests/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-26 15:41:08.000000 google-cloud-gke-backup-0.5.8/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-26 15:43:56.715730 google-cloud-gke-backup-0.5.8/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-26 15:41:08.000000 google-cloud-gke-backup-0.5.8/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-26 15:43:56.715730 google-cloud-gke-backup-0.5.8/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-26 15:41:08.000000 google-cloud-gke-backup-0.5.8/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-26 15:43:56.715730 google-cloud-gke-backup-0.5.8/tests/unit/gapic/gke_backup_v1/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-26 15:41:08.000000 google-cloud-gke-backup-0.5.8/tests/unit/gapic/gke_backup_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   777593 2024-03-26 15:41:08.000000 google-cloud-gke-backup-0.5.8/tests/unit/gapic/gke_backup_v1/test_backup_for_gke.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:23:46.724068 google-cloud-gke-backup-0.5.9/
+-rw-rw-r--   0 root         (0)     1003    11358 2024-05-28 08:20:19.000000 google-cloud-gke-backup-0.5.9/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2024-05-28 08:20:19.000000 google-cloud-gke-backup-0.5.9/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     5363 2024-05-28 08:23:46.724068 google-cloud-gke-backup-0.5.9/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3938 2024-05-28 08:20:19.000000 google-cloud-gke-backup-0.5.9/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:23:46.708065 google-cloud-gke-backup-0.5.9/google/
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:23:46.708065 google-cloud-gke-backup-0.5.9/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:23:46.712066 google-cloud-gke-backup-0.5.9/google/cloud/gke_backup/
+-rw-rw-r--   0 root         (0)     1003     3918 2024-05-28 08:20:19.000000 google-cloud-gke-backup-0.5.9/google/cloud/gke_backup/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2024-05-28 08:20:19.000000 google-cloud-gke-backup-0.5.9/google/cloud/gke_backup/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       84 2024-05-28 08:20:19.000000 google-cloud-gke-backup-0.5.9/google/cloud/gke_backup/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:23:46.712066 google-cloud-gke-backup-0.5.9/google/cloud/gke_backup_v1/
+-rw-rw-r--   0 root         (0)     1003     3605 2024-05-28 08:20:19.000000 google-cloud-gke-backup-0.5.9/google/cloud/gke_backup_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10094 2024-05-28 08:20:19.000000 google-cloud-gke-backup-0.5.9/google/cloud/gke_backup_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2024-05-28 08:20:19.000000 google-cloud-gke-backup-0.5.9/google/cloud/gke_backup_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       84 2024-05-28 08:20:19.000000 google-cloud-gke-backup-0.5.9/google/cloud/gke_backup_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:23:46.712066 google-cloud-gke-backup-0.5.9/google/cloud/gke_backup_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-28 08:20:19.000000 google-cloud-gke-backup-0.5.9/google/cloud/gke_backup_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:23:46.716067 google-cloud-gke-backup-0.5.9/google/cloud/gke_backup_v1/services/backup_for_gke/
+-rw-rw-r--   0 root         (0)     1003      761 2024-05-28 08:20:19.000000 google-cloud-gke-backup-0.5.9/google/cloud/gke_backup_v1/services/backup_for_gke/__init__.py
+-rw-rw-r--   0 root         (0)     1003   169718 2024-05-28 08:20:19.000000 google-cloud-gke-backup-0.5.9/google/cloud/gke_backup_v1/services/backup_for_gke/async_client.py
+-rw-rw-r--   0 root         (0)     1003   188088 2024-05-28 08:20:19.000000 google-cloud-gke-backup-0.5.9/google/cloud/gke_backup_v1/services/backup_for_gke/client.py
+-rw-rw-r--   0 root         (0)     1003    31038 2024-05-28 08:20:19.000000 google-cloud-gke-backup-0.5.9/google/cloud/gke_backup_v1/services/backup_for_gke/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:23:46.716067 google-cloud-gke-backup-0.5.9/google/cloud/gke_backup_v1/services/backup_for_gke/transports/
+-rw-rw-r--   0 root         (0)     1003     1372 2024-05-28 08:20:19.000000 google-cloud-gke-backup-0.5.9/google/cloud/gke_backup_v1/services/backup_for_gke/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    23950 2024-05-28 08:20:19.000000 google-cloud-gke-backup-0.5.9/google/cloud/gke_backup_v1/services/backup_for_gke/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    48895 2024-05-28 08:20:19.000000 google-cloud-gke-backup-0.5.9/google/cloud/gke_backup_v1/services/backup_for_gke/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    59725 2024-05-28 08:20:19.000000 google-cloud-gke-backup-0.5.9/google/cloud/gke_backup_v1/services/backup_for_gke/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   170171 2024-05-28 08:20:19.000000 google-cloud-gke-backup-0.5.9/google/cloud/gke_backup_v1/services/backup_for_gke/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:23:46.720068 google-cloud-gke-backup-0.5.9/google/cloud/gke_backup_v1/types/
+-rw-rw-r--   0 root         (0)     1003     3308 2024-05-28 08:20:19.000000 google-cloud-gke-backup-0.5.9/google/cloud/gke_backup_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    14797 2024-05-28 08:20:19.000000 google-cloud-gke-backup-0.5.9/google/cloud/gke_backup_v1/types/backup.py
+-rw-rw-r--   0 root         (0)     1003    21350 2024-05-28 08:20:19.000000 google-cloud-gke-backup-0.5.9/google/cloud/gke_backup_v1/types/backup_plan.py
+-rw-rw-r--   0 root         (0)     1003     3046 2024-05-28 08:20:19.000000 google-cloud-gke-backup-0.5.9/google/cloud/gke_backup_v1/types/common.py
+-rw-rw-r--   0 root         (0)     1003    37714 2024-05-28 08:20:19.000000 google-cloud-gke-backup-0.5.9/google/cloud/gke_backup_v1/types/gkebackup.py
+-rw-rw-r--   0 root         (0)     1003    46247 2024-05-28 08:20:19.000000 google-cloud-gke-backup-0.5.9/google/cloud/gke_backup_v1/types/restore.py
+-rw-rw-r--   0 root         (0)     1003     5912 2024-05-28 08:20:19.000000 google-cloud-gke-backup-0.5.9/google/cloud/gke_backup_v1/types/restore_plan.py
+-rw-rw-r--   0 root         (0)     1003    12208 2024-05-28 08:20:19.000000 google-cloud-gke-backup-0.5.9/google/cloud/gke_backup_v1/types/volume.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:23:46.720068 google-cloud-gke-backup-0.5.9/google_cloud_gke_backup.egg-info/
+-rw-r--r--   0 root         (0)     1003     5363 2024-05-28 08:23:46.000000 google-cloud-gke-backup-0.5.9/google_cloud_gke_backup.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1795 2024-05-28 08:23:46.000000 google-cloud-gke-backup-0.5.9/google_cloud_gke_backup.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-05-28 08:23:46.000000 google-cloud-gke-backup-0.5.9/google_cloud_gke_backup.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-05-28 08:23:46.000000 google-cloud-gke-backup-0.5.9/google_cloud_gke_backup.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      342 2024-05-28 08:23:46.000000 google-cloud-gke-backup-0.5.9/google_cloud_gke_backup.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2024-05-28 08:23:46.000000 google-cloud-gke-backup-0.5.9/google_cloud_gke_backup.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2024-05-28 08:23:46.724068 google-cloud-gke-backup-0.5.9/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3222 2024-05-28 08:20:19.000000 google-cloud-gke-backup-0.5.9/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:23:46.720068 google-cloud-gke-backup-0.5.9/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-28 08:20:19.000000 google-cloud-gke-backup-0.5.9/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:23:46.720068 google-cloud-gke-backup-0.5.9/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-28 08:20:19.000000 google-cloud-gke-backup-0.5.9/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:23:46.720068 google-cloud-gke-backup-0.5.9/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-28 08:20:19.000000 google-cloud-gke-backup-0.5.9/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:23:46.720068 google-cloud-gke-backup-0.5.9/tests/unit/gapic/gke_backup_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-28 08:20:19.000000 google-cloud-gke-backup-0.5.9/tests/unit/gapic/gke_backup_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   898813 2024-05-28 08:20:19.000000 google-cloud-gke-backup-0.5.9/tests/unit/gapic/gke_backup_v1/test_backup_for_gke.py
```

### Comparing `google-cloud-gke-backup-0.5.8/LICENSE` & `google-cloud-gke-backup-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.5.8/MANIFEST.in` & `google-cloud-gke-backup-0.5.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.5.8/PKG-INFO` & `google-cloud-gke-backup-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-gke-backup
-Version: 0.5.8
+Version: 0.5.9
 Summary: Google Cloud Gke Backup API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-gke-backup
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-gke-backup-0.5.8/README.rst` & `google-cloud-gke-backup-0.5.9/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.5.8/google/cloud/gke_backup/__init__.py` & `google-cloud-gke-backup-0.5.9/google/cloud/gke_backup/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     RpoConfig,
 )
 from google.cloud.gke_backup_v1.types.common import (
     EncryptionKey,
     NamespacedName,
     NamespacedNames,
     Namespaces,
+    VolumeTypeEnum,
 )
 from google.cloud.gke_backup_v1.types.gkebackup import (
     CreateBackupPlanRequest,
     CreateBackupRequest,
     CreateRestorePlanRequest,
     CreateRestoreRequest,
     DeleteBackupPlanRequest,
@@ -65,29 +66,35 @@
     ListVolumeRestoresResponse,
     OperationMetadata,
     UpdateBackupPlanRequest,
     UpdateBackupRequest,
     UpdateRestorePlanRequest,
     UpdateRestoreRequest,
 )
-from google.cloud.gke_backup_v1.types.restore import Restore, RestoreConfig
+from google.cloud.gke_backup_v1.types.restore import (
+    ResourceSelector,
+    Restore,
+    RestoreConfig,
+    VolumeDataRestorePolicyOverride,
+)
 from google.cloud.gke_backup_v1.types.restore_plan import RestorePlan
 from google.cloud.gke_backup_v1.types.volume import VolumeBackup, VolumeRestore
 
 __all__ = (
     "BackupForGKEClient",
     "BackupForGKEAsyncClient",
     "Backup",
     "BackupPlan",
     "ExclusionWindow",
     "RpoConfig",
     "EncryptionKey",
     "NamespacedName",
     "NamespacedNames",
     "Namespaces",
+    "VolumeTypeEnum",
     "CreateBackupPlanRequest",
     "CreateBackupRequest",
     "CreateRestorePlanRequest",
     "CreateRestoreRequest",
     "DeleteBackupPlanRequest",
     "DeleteBackupRequest",
     "DeleteRestorePlanRequest",
@@ -113,13 +120,15 @@
     "ListVolumeRestoresRequest",
     "ListVolumeRestoresResponse",
     "OperationMetadata",
     "UpdateBackupPlanRequest",
     "UpdateBackupRequest",
     "UpdateRestorePlanRequest",
     "UpdateRestoreRequest",
+    "ResourceSelector",
     "Restore",
     "RestoreConfig",
+    "VolumeDataRestorePolicyOverride",
     "RestorePlan",
     "VolumeBackup",
     "VolumeRestore",
 )
```

### Comparing `google-cloud-gke-backup-0.5.8/google/cloud/gke_backup/gapic_version.py` & `google-cloud-gke-backup-0.5.9/google/cloud/gke_backup/gapic_version.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.5.8"  # {x-release-please-version}
+__version__ = "0.5.9"  # {x-release-please-version}
```

### Comparing `google-cloud-gke-backup-0.5.8/google/cloud/gke_backup_v1/__init__.py` & `google-cloud-gke-backup-0.5.9/google/cloud/gke_backup_v1/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,21 @@
 
 __version__ = package_version.__version__
 
 
 from .services.backup_for_gke import BackupForGKEAsyncClient, BackupForGKEClient
 from .types.backup import Backup
 from .types.backup_plan import BackupPlan, ExclusionWindow, RpoConfig
-from .types.common import EncryptionKey, NamespacedName, NamespacedNames, Namespaces
+from .types.common import (
+    EncryptionKey,
+    NamespacedName,
+    NamespacedNames,
+    Namespaces,
+    VolumeTypeEnum,
+)
 from .types.gkebackup import (
     CreateBackupPlanRequest,
     CreateBackupRequest,
     CreateRestorePlanRequest,
     CreateRestoreRequest,
     DeleteBackupPlanRequest,
     DeleteBackupRequest,
@@ -53,15 +59,20 @@
     ListVolumeRestoresResponse,
     OperationMetadata,
     UpdateBackupPlanRequest,
     UpdateBackupRequest,
     UpdateRestorePlanRequest,
     UpdateRestoreRequest,
 )
-from .types.restore import Restore, RestoreConfig
+from .types.restore import (
+    ResourceSelector,
+    Restore,
+    RestoreConfig,
+    VolumeDataRestorePolicyOverride,
+)
 from .types.restore_plan import RestorePlan
 from .types.volume import VolumeBackup, VolumeRestore
 
 __all__ = (
     "BackupForGKEAsyncClient",
     "Backup",
     "BackupForGKEClient",
@@ -96,18 +107,21 @@
     "ListVolumeBackupsResponse",
     "ListVolumeRestoresRequest",
     "ListVolumeRestoresResponse",
     "NamespacedName",
     "NamespacedNames",
     "Namespaces",
     "OperationMetadata",
+    "ResourceSelector",
     "Restore",
     "RestoreConfig",
     "RestorePlan",
     "RpoConfig",
     "UpdateBackupPlanRequest",
     "UpdateBackupRequest",
     "UpdateRestorePlanRequest",
     "UpdateRestoreRequest",
     "VolumeBackup",
+    "VolumeDataRestorePolicyOverride",
     "VolumeRestore",
+    "VolumeTypeEnum",
 )
```

### Comparing `google-cloud-gke-backup-0.5.8/google/cloud/gke_backup_v1/gapic_metadata.json` & `google-cloud-gke-backup-0.5.9/google/cloud/gke_backup_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.5.8/google/cloud/gke_backup_v1/gapic_version.py` & `google-cloud-gke-backup-0.5.9/google/cloud/gke_backup_v1/gapic_version.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.5.8"  # {x-release-please-version}
+__version__ = "0.5.9"  # {x-release-please-version}
```

### Comparing `google-cloud-gke-backup-0.5.8/google/cloud/gke_backup_v1/services/__init__.py` & `google-cloud-gke-backup-0.5.9/google/cloud/gke_backup_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.5.8/google/cloud/gke_backup_v1/services/backup_for_gke/__init__.py` & `google-cloud-gke-backup-0.5.9/google/cloud/gke_backup_v1/services/backup_for_gke/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.5.8/google/cloud/gke_backup_v1/services/backup_for_gke/async_client.py` & `google-cloud-gke-backup-0.5.9/google/cloud/gke_backup_v1/services/backup_for_gke/async_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import functools
 import re
 from typing import (
+    Callable,
     Dict,
     Mapping,
     MutableMapping,
     MutableSequence,
     Optional,
     Sequence,
     Tuple,
@@ -224,29 +225,33 @@
         type(BackupForGKEClient).get_transport_class, type(BackupForGKEClient)
     )
 
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
-        transport: Union[str, BackupForGKETransport] = "grpc_asyncio",
+        transport: Optional[
+            Union[str, BackupForGKETransport, Callable[..., BackupForGKETransport]]
+        ] = "grpc_asyncio",
         client_options: Optional[ClientOptions] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the backup for gke async client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
-            transport (Union[str, ~.BackupForGKETransport]): The
-                transport to use. If set to None, a transport is chosen
-                automatically.
+            transport (Optional[Union[str,BackupForGKETransport,Callable[..., BackupForGKETransport]]]):
+                The transport to use, or a Callable that constructs and returns a new transport to use.
+                If a Callable is given, it will be called with the same set of initialization
+                arguments as used in the BackupForGKETransport constructor.
+                If set to None, a transport is chosen automatically.
             client_options (Optional[Union[google.api_core.client_options.ClientOptions, dict]]):
                 Custom options for the client.
 
                 1. The ``api_endpoint`` property can be used to override the
                 default endpoint provided by the client when ``transport`` is
                 not explicitly provided. Only if this property is not set and
                 ``transport`` was not explicitly provided, the endpoint is
@@ -381,41 +386,42 @@
                 The result type for the operation will be
                 :class:`google.cloud.gke_backup_v1.types.BackupPlan`
                 Defines the configuration and scheduling for a "line" of
                 Backups.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, backup_plan, backup_plan_id])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = gkebackup.CreateBackupPlanRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, gkebackup.CreateBackupPlanRequest):
+            request = gkebackup.CreateBackupPlanRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if parent is not None:
             request.parent = parent
         if backup_plan is not None:
             request.backup_plan = backup_plan
         if backup_plan_id is not None:
             request.backup_plan_id = backup_plan_id
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.create_backup_plan,
-            default_timeout=300.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.create_backup_plan
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
         )
 
@@ -501,46 +507,38 @@
 
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = gkebackup.ListBackupPlansRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, gkebackup.ListBackupPlansRequest):
+            request = gkebackup.ListBackupPlansRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if parent is not None:
             request.parent = parent
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.list_backup_plans,
-            default_retry=retries.AsyncRetry(
-                initial=1.0,
-                maximum=60.0,
-                multiplier=1.3,
-                predicate=retries.if_exception_type(
-                    core_exceptions.ServiceUnavailable,
-                ),
-                deadline=60.0,
-            ),
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.list_backup_plans
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
         )
 
@@ -623,46 +621,38 @@
         Returns:
             google.cloud.gke_backup_v1.types.BackupPlan:
                 Defines the configuration and
                 scheduling for a "line" of Backups.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = gkebackup.GetBackupPlanRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, gkebackup.GetBackupPlanRequest):
+            request = gkebackup.GetBackupPlanRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if name is not None:
             request.name = name
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.get_backup_plan,
-            default_retry=retries.AsyncRetry(
-                initial=1.0,
-                maximum=60.0,
-                multiplier=1.3,
-                predicate=retries.if_exception_type(
-                    core_exceptions.ServiceUnavailable,
-                ),
-                deadline=60.0,
-            ),
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.get_backup_plan
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
@@ -766,39 +756,40 @@
                 The result type for the operation will be
                 :class:`google.cloud.gke_backup_v1.types.BackupPlan`
                 Defines the configuration and scheduling for a "line" of
                 Backups.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([backup_plan, update_mask])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = gkebackup.UpdateBackupPlanRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, gkebackup.UpdateBackupPlanRequest):
+            request = gkebackup.UpdateBackupPlanRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if backup_plan is not None:
             request.backup_plan = backup_plan
         if update_mask is not None:
             request.update_mask = update_mask
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.update_backup_plan,
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.update_backup_plan
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata(
                 (("backup_plan.name", request.backup_plan.name),)
             ),
@@ -896,37 +887,38 @@
                          rpc Bar(google.protobuf.Empty) returns
                          (google.protobuf.Empty);
 
                       }
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = gkebackup.DeleteBackupPlanRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, gkebackup.DeleteBackupPlanRequest):
+            request = gkebackup.DeleteBackupPlanRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if name is not None:
             request.name = name
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.delete_backup_plan,
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.delete_backup_plan
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
@@ -1043,41 +1035,42 @@
                    some portion of the state of a GKE cluster, the
                    record of the backup operation itself, and an anchor
                    for the underlying artifacts that comprise the Backup
                    (the config backup and VolumeBackups).
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, backup, backup_id])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = gkebackup.CreateBackupRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, gkebackup.CreateBackupRequest):
+            request = gkebackup.CreateBackupRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if parent is not None:
             request.parent = parent
         if backup is not None:
             request.backup = backup
         if backup_id is not None:
             request.backup_id = backup_id
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.create_backup,
-            default_timeout=120.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.create_backup
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
         )
 
@@ -1163,46 +1156,38 @@
 
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = gkebackup.ListBackupsRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, gkebackup.ListBackupsRequest):
+            request = gkebackup.ListBackupsRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if parent is not None:
             request.parent = parent
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.list_backups,
-            default_retry=retries.AsyncRetry(
-                initial=1.0,
-                maximum=60.0,
-                multiplier=1.3,
-                predicate=retries.if_exception_type(
-                    core_exceptions.ServiceUnavailable,
-                ),
-                deadline=60.0,
-            ),
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.list_backups
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
         )
 
@@ -1290,46 +1275,38 @@
                 the record of the backup operation
                 itself, and an anchor for the underlying
                 artifacts that comprise the Backup (the
                 config backup and VolumeBackups).
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = gkebackup.GetBackupRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, gkebackup.GetBackupRequest):
+            request = gkebackup.GetBackupRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if name is not None:
             request.name = name
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.get_backup,
-            default_retry=retries.AsyncRetry(
-                initial=1.0,
-                maximum=60.0,
-                multiplier=1.3,
-                predicate=retries.if_exception_type(
-                    core_exceptions.ServiceUnavailable,
-                ),
-                deadline=60.0,
-            ),
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.get_backup
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
@@ -1431,39 +1408,40 @@
                    some portion of the state of a GKE cluster, the
                    record of the backup operation itself, and an anchor
                    for the underlying artifacts that comprise the Backup
                    (the config backup and VolumeBackups).
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([backup, update_mask])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = gkebackup.UpdateBackupRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, gkebackup.UpdateBackupRequest):
+            request = gkebackup.UpdateBackupRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if backup is not None:
             request.backup = backup
         if update_mask is not None:
             request.update_mask = update_mask
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.update_backup,
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.update_backup
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata(
                 (("backup.name", request.backup.name),)
             ),
@@ -1561,37 +1539,38 @@
                          rpc Bar(google.protobuf.Empty) returns
                          (google.protobuf.Empty);
 
                       }
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = gkebackup.DeleteBackupRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, gkebackup.DeleteBackupRequest):
+            request = gkebackup.DeleteBackupRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if name is not None:
             request.name = name
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.delete_backup,
-            default_timeout=300.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.delete_backup
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
@@ -1679,46 +1658,38 @@
                 ListVolumeBackups.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = gkebackup.ListVolumeBackupsRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, gkebackup.ListVolumeBackupsRequest):
+            request = gkebackup.ListVolumeBackupsRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if parent is not None:
             request.parent = parent
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.list_volume_backups,
-            default_retry=retries.AsyncRetry(
-                initial=1.0,
-                maximum=60.0,
-                multiplier=1.3,
-                predicate=retries.if_exception_type(
-                    core_exceptions.ServiceUnavailable,
-                ),
-                deadline=60.0,
-            ),
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.list_volume_backups
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
         )
 
@@ -1805,46 +1776,38 @@
                 persistent volume as a component of a
                 Backup - both the record of the
                 operation and a pointer to the
                 underlying storage-specific artifacts.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = gkebackup.GetVolumeBackupRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, gkebackup.GetVolumeBackupRequest):
+            request = gkebackup.GetVolumeBackupRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if name is not None:
             request.name = name
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.get_volume_backup,
-            default_retry=retries.AsyncRetry(
-                initial=1.0,
-                maximum=60.0,
-                multiplier=1.3,
-                predicate=retries.if_exception_type(
-                    core_exceptions.ServiceUnavailable,
-                ),
-                deadline=60.0,
-            ),
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.get_volume_backup
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
@@ -1958,41 +1921,42 @@
                 An object representing a long-running operation.
 
                 The result type for the operation will be :class:`google.cloud.gke_backup_v1.types.RestorePlan` The configuration of a potential series of Restore operations to be performed
                    against Backups belong to a particular BackupPlan.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, restore_plan, restore_plan_id])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = gkebackup.CreateRestorePlanRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, gkebackup.CreateRestorePlanRequest):
+            request = gkebackup.CreateRestorePlanRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if parent is not None:
             request.parent = parent
         if restore_plan is not None:
             request.restore_plan = restore_plan
         if restore_plan_id is not None:
             request.restore_plan_id = restore_plan_id
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.create_restore_plan,
-            default_timeout=120.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.create_restore_plan
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
         )
 
@@ -2078,46 +2042,38 @@
                 ListRestorePlans.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = gkebackup.ListRestorePlansRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, gkebackup.ListRestorePlansRequest):
+            request = gkebackup.ListRestorePlansRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if parent is not None:
             request.parent = parent
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.list_restore_plans,
-            default_retry=retries.AsyncRetry(
-                initial=1.0,
-                maximum=60.0,
-                multiplier=1.3,
-                predicate=retries.if_exception_type(
-                    core_exceptions.ServiceUnavailable,
-                ),
-                deadline=60.0,
-            ),
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.list_restore_plans
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
         )
 
@@ -2202,46 +2158,38 @@
                 The configuration of a potential
                 series of Restore operations to be
                 performed against Backups belong to a
                 particular BackupPlan.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = gkebackup.GetRestorePlanRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, gkebackup.GetRestorePlanRequest):
+            request = gkebackup.GetRestorePlanRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if name is not None:
             request.name = name
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.get_restore_plan,
-            default_retry=retries.AsyncRetry(
-                initial=1.0,
-                maximum=60.0,
-                multiplier=1.3,
-                predicate=retries.if_exception_type(
-                    core_exceptions.ServiceUnavailable,
-                ),
-                deadline=60.0,
-            ),
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.get_restore_plan
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
@@ -2344,39 +2292,40 @@
                 An object representing a long-running operation.
 
                 The result type for the operation will be :class:`google.cloud.gke_backup_v1.types.RestorePlan` The configuration of a potential series of Restore operations to be performed
                    against Backups belong to a particular BackupPlan.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([restore_plan, update_mask])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = gkebackup.UpdateRestorePlanRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, gkebackup.UpdateRestorePlanRequest):
+            request = gkebackup.UpdateRestorePlanRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if restore_plan is not None:
             request.restore_plan = restore_plan
         if update_mask is not None:
             request.update_mask = update_mask
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.update_restore_plan,
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.update_restore_plan
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata(
                 (("restore_plan.name", request.restore_plan.name),)
             ),
@@ -2475,37 +2424,38 @@
                          rpc Bar(google.protobuf.Empty) returns
                          (google.protobuf.Empty);
 
                       }
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = gkebackup.DeleteRestorePlanRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, gkebackup.DeleteRestorePlanRequest):
+            request = gkebackup.DeleteRestorePlanRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if name is not None:
             request.name = name
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.delete_restore_plan,
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.delete_restore_plan
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
@@ -2626,41 +2576,42 @@
 
                 The result type for the operation will be :class:`google.cloud.gke_backup_v1.types.Restore` Represents both a request to Restore some portion of a Backup into
                    a target GKE cluster and a record of the restore
                    operation itself.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, restore, restore_id])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = gkebackup.CreateRestoreRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, gkebackup.CreateRestoreRequest):
+            request = gkebackup.CreateRestoreRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if parent is not None:
             request.parent = parent
         if restore is not None:
             request.restore = restore
         if restore_id is not None:
             request.restore_id = restore_id
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.create_restore,
-            default_timeout=120.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.create_restore
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
         )
 
@@ -2746,46 +2697,38 @@
 
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = gkebackup.ListRestoresRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, gkebackup.ListRestoresRequest):
+            request = gkebackup.ListRestoresRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if parent is not None:
             request.parent = parent
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.list_restores,
-            default_retry=retries.AsyncRetry(
-                initial=1.0,
-                maximum=60.0,
-                multiplier=1.3,
-                predicate=retries.if_exception_type(
-                    core_exceptions.ServiceUnavailable,
-                ),
-                deadline=60.0,
-            ),
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.list_restores
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
         )
 
@@ -2870,46 +2813,38 @@
                 Represents both a request to Restore
                 some portion of a Backup into a target
                 GKE cluster and a record of the restore
                 operation itself.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = gkebackup.GetRestoreRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, gkebackup.GetRestoreRequest):
+            request = gkebackup.GetRestoreRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if name is not None:
             request.name = name
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.get_restore,
-            default_retry=retries.AsyncRetry(
-                initial=1.0,
-                maximum=60.0,
-                multiplier=1.3,
-                predicate=retries.if_exception_type(
-                    core_exceptions.ServiceUnavailable,
-                ),
-                deadline=60.0,
-            ),
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.get_restore
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
@@ -3009,39 +2944,40 @@
 
                 The result type for the operation will be :class:`google.cloud.gke_backup_v1.types.Restore` Represents both a request to Restore some portion of a Backup into
                    a target GKE cluster and a record of the restore
                    operation itself.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([restore, update_mask])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = gkebackup.UpdateRestoreRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, gkebackup.UpdateRestoreRequest):
+            request = gkebackup.UpdateRestoreRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if restore is not None:
             request.restore = restore
         if update_mask is not None:
             request.update_mask = update_mask
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.update_restore,
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.update_restore
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata(
                 (("restore.name", request.restore.name),)
             ),
@@ -3139,37 +3075,38 @@
                          rpc Bar(google.protobuf.Empty) returns
                          (google.protobuf.Empty);
 
                       }
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = gkebackup.DeleteRestoreRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, gkebackup.DeleteRestoreRequest):
+            request = gkebackup.DeleteRestoreRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if name is not None:
             request.name = name
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.delete_restore,
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.delete_restore
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
@@ -3257,46 +3194,38 @@
                 ListVolumeRestores.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = gkebackup.ListVolumeRestoresRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, gkebackup.ListVolumeRestoresRequest):
+            request = gkebackup.ListVolumeRestoresRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if parent is not None:
             request.parent = parent
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.list_volume_restores,
-            default_retry=retries.AsyncRetry(
-                initial=1.0,
-                maximum=60.0,
-                multiplier=1.3,
-                predicate=retries.if_exception_type(
-                    core_exceptions.ServiceUnavailable,
-                ),
-                deadline=60.0,
-            ),
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.list_volume_restores
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
         )
 
@@ -3380,46 +3309,38 @@
         Returns:
             google.cloud.gke_backup_v1.types.VolumeRestore:
                 Represents the operation of restoring
                 a volume from a VolumeBackup.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = gkebackup.GetVolumeRestoreRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, gkebackup.GetVolumeRestoreRequest):
+            request = gkebackup.GetVolumeRestoreRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if name is not None:
             request.name = name
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.get_volume_restore,
-            default_retry=retries.AsyncRetry(
-                initial=1.0,
-                maximum=60.0,
-                multiplier=1.3,
-                predicate=retries.if_exception_type(
-                    core_exceptions.ServiceUnavailable,
-                ),
-                deadline=60.0,
-            ),
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.get_volume_restore
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
@@ -3496,46 +3417,38 @@
         Returns:
             google.cloud.gke_backup_v1.types.GetBackupIndexDownloadUrlResponse:
                 Response message for
                 GetBackupIndexDownloadUrl.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([backup])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = gkebackup.GetBackupIndexDownloadUrlRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, gkebackup.GetBackupIndexDownloadUrlRequest):
+            request = gkebackup.GetBackupIndexDownloadUrlRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if backup is not None:
             request.backup = backup
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.get_backup_index_download_url,
-            default_retry=retries.AsyncRetry(
-                initial=1.0,
-                maximum=60.0,
-                multiplier=1.3,
-                predicate=retries.if_exception_type(
-                    core_exceptions.ServiceUnavailable,
-                ),
-                deadline=60.0,
-            ),
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.get_backup_index_download_url
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("backup", request.backup),)),
         )
```

### Comparing `google-cloud-gke-backup-0.5.8/google/cloud/gke_backup_v1/services/backup_for_gke/client.py` & `google-cloud-gke-backup-0.5.9/google/cloud/gke_backup_v1/services/backup_for_gke/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import os
 import re
 from typing import (
+    Callable,
     Dict,
     Mapping,
     MutableMapping,
     MutableSequence,
     Optional,
     Sequence,
     Tuple,
@@ -715,29 +716,33 @@
         """
         return self._universe_domain
 
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
-        transport: Optional[Union[str, BackupForGKETransport]] = None,
+        transport: Optional[
+            Union[str, BackupForGKETransport, Callable[..., BackupForGKETransport]]
+        ] = None,
         client_options: Optional[Union[client_options_lib.ClientOptions, dict]] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the backup for gke client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
-            transport (Union[str, BackupForGKETransport]): The
-                transport to use. If set to None, a transport is chosen
-                automatically.
+            transport (Optional[Union[str,BackupForGKETransport,Callable[..., BackupForGKETransport]]]):
+                The transport to use, or a Callable that constructs and returns a new transport.
+                If a Callable is given, it will be called with the same set of initialization
+                arguments as used in the BackupForGKETransport constructor.
+                If set to None, a transport is chosen automatically.
             client_options (Optional[Union[google.api_core.client_options.ClientOptions, dict]]):
                 Custom options for the client.
 
                 1. The ``api_endpoint`` property can be used to override the
                 default endpoint provided by the client when ``transport`` is
                 not explicitly provided. Only if this property is not set and
                 ``transport`` was not explicitly provided, the endpoint is
@@ -835,16 +840,23 @@
             if api_key_value and hasattr(
                 google.auth._default, "get_api_key_credentials"
             ):
                 credentials = google.auth._default.get_api_key_credentials(
                     api_key_value
                 )
 
-            Transport = type(self).get_transport_class(cast(str, transport))
-            self._transport = Transport(
+            transport_init: Union[
+                Type[BackupForGKETransport], Callable[..., BackupForGKETransport]
+            ] = (
+                type(self).get_transport_class(transport)
+                if isinstance(transport, str) or transport is None
+                else cast(Callable[..., BackupForGKETransport], transport)
+            )
+            # initialize with the provided callable or the passed in class
+            self._transport = transport_init(
                 credentials=credentials,
                 credentials_file=self._client_options.credentials_file,
                 host=self._api_endpoint,
                 scopes=self._client_options.scopes,
                 client_cert_source_for_mtls=self._client_cert_source,
                 quota_project_id=self._client_options.quota_project_id,
                 client_info=client_info,
@@ -947,27 +959,25 @@
                 The result type for the operation will be
                 :class:`google.cloud.gke_backup_v1.types.BackupPlan`
                 Defines the configuration and scheduling for a "line" of
                 Backups.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, backup_plan, backup_plan_id])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a gkebackup.CreateBackupPlanRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, gkebackup.CreateBackupPlanRequest):
             request = gkebackup.CreateBackupPlanRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if parent is not None:
                 request.parent = parent
             if backup_plan is not None:
@@ -1067,27 +1077,25 @@
 
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a gkebackup.ListBackupPlansRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, gkebackup.ListBackupPlansRequest):
             request = gkebackup.ListBackupPlansRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if parent is not None:
                 request.parent = parent
 
@@ -1180,27 +1188,25 @@
         Returns:
             google.cloud.gke_backup_v1.types.BackupPlan:
                 Defines the configuration and
                 scheduling for a "line" of Backups.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a gkebackup.GetBackupPlanRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, gkebackup.GetBackupPlanRequest):
             request = gkebackup.GetBackupPlanRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if name is not None:
                 request.name = name
 
@@ -1314,27 +1320,25 @@
                 The result type for the operation will be
                 :class:`google.cloud.gke_backup_v1.types.BackupPlan`
                 Defines the configuration and scheduling for a "line" of
                 Backups.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([backup_plan, update_mask])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a gkebackup.UpdateBackupPlanRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, gkebackup.UpdateBackupPlanRequest):
             request = gkebackup.UpdateBackupPlanRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if backup_plan is not None:
                 request.backup_plan = backup_plan
             if update_mask is not None:
@@ -1444,27 +1448,25 @@
                          rpc Bar(google.protobuf.Empty) returns
                          (google.protobuf.Empty);
 
                       }
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a gkebackup.DeleteBackupPlanRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, gkebackup.DeleteBackupPlanRequest):
             request = gkebackup.DeleteBackupPlanRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if name is not None:
                 request.name = name
 
@@ -1591,27 +1593,25 @@
                    some portion of the state of a GKE cluster, the
                    record of the backup operation itself, and an anchor
                    for the underlying artifacts that comprise the Backup
                    (the config backup and VolumeBackups).
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, backup, backup_id])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a gkebackup.CreateBackupRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, gkebackup.CreateBackupRequest):
             request = gkebackup.CreateBackupRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if parent is not None:
                 request.parent = parent
             if backup is not None:
@@ -1711,27 +1711,25 @@
 
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a gkebackup.ListBackupsRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, gkebackup.ListBackupsRequest):
             request = gkebackup.ListBackupsRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if parent is not None:
                 request.parent = parent
 
@@ -1829,27 +1827,25 @@
                 the record of the backup operation
                 itself, and an anchor for the underlying
                 artifacts that comprise the Backup (the
                 config backup and VolumeBackups).
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a gkebackup.GetBackupRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, gkebackup.GetBackupRequest):
             request = gkebackup.GetBackupRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if name is not None:
                 request.name = name
 
@@ -1961,27 +1957,25 @@
                    some portion of the state of a GKE cluster, the
                    record of the backup operation itself, and an anchor
                    for the underlying artifacts that comprise the Backup
                    (the config backup and VolumeBackups).
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([backup, update_mask])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a gkebackup.UpdateBackupRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, gkebackup.UpdateBackupRequest):
             request = gkebackup.UpdateBackupRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if backup is not None:
                 request.backup = backup
             if update_mask is not None:
@@ -2091,27 +2085,25 @@
                          rpc Bar(google.protobuf.Empty) returns
                          (google.protobuf.Empty);
 
                       }
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a gkebackup.DeleteBackupRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, gkebackup.DeleteBackupRequest):
             request = gkebackup.DeleteBackupRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if name is not None:
                 request.name = name
 
@@ -2209,27 +2201,25 @@
                 ListVolumeBackups.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a gkebackup.ListVolumeBackupsRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, gkebackup.ListVolumeBackupsRequest):
             request = gkebackup.ListVolumeBackupsRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if parent is not None:
                 request.parent = parent
 
@@ -2326,27 +2316,25 @@
                 persistent volume as a component of a
                 Backup - both the record of the
                 operation and a pointer to the
                 underlying storage-specific artifacts.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a gkebackup.GetVolumeBackupRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, gkebackup.GetVolumeBackupRequest):
             request = gkebackup.GetVolumeBackupRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if name is not None:
                 request.name = name
 
@@ -2470,27 +2458,25 @@
                 An object representing a long-running operation.
 
                 The result type for the operation will be :class:`google.cloud.gke_backup_v1.types.RestorePlan` The configuration of a potential series of Restore operations to be performed
                    against Backups belong to a particular BackupPlan.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, restore_plan, restore_plan_id])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a gkebackup.CreateRestorePlanRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, gkebackup.CreateRestorePlanRequest):
             request = gkebackup.CreateRestorePlanRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if parent is not None:
                 request.parent = parent
             if restore_plan is not None:
@@ -2590,27 +2576,25 @@
                 ListRestorePlans.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a gkebackup.ListRestorePlansRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, gkebackup.ListRestorePlansRequest):
             request = gkebackup.ListRestorePlansRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if parent is not None:
                 request.parent = parent
 
@@ -2705,27 +2689,25 @@
                 The configuration of a potential
                 series of Restore operations to be
                 performed against Backups belong to a
                 particular BackupPlan.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a gkebackup.GetRestorePlanRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, gkebackup.GetRestorePlanRequest):
             request = gkebackup.GetRestorePlanRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if name is not None:
                 request.name = name
 
@@ -2838,27 +2820,25 @@
                 An object representing a long-running operation.
 
                 The result type for the operation will be :class:`google.cloud.gke_backup_v1.types.RestorePlan` The configuration of a potential series of Restore operations to be performed
                    against Backups belong to a particular BackupPlan.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([restore_plan, update_mask])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a gkebackup.UpdateRestorePlanRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, gkebackup.UpdateRestorePlanRequest):
             request = gkebackup.UpdateRestorePlanRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if restore_plan is not None:
                 request.restore_plan = restore_plan
             if update_mask is not None:
@@ -2969,27 +2949,25 @@
                          rpc Bar(google.protobuf.Empty) returns
                          (google.protobuf.Empty);
 
                       }
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a gkebackup.DeleteRestorePlanRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, gkebackup.DeleteRestorePlanRequest):
             request = gkebackup.DeleteRestorePlanRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if name is not None:
                 request.name = name
 
@@ -3120,27 +3098,25 @@
 
                 The result type for the operation will be :class:`google.cloud.gke_backup_v1.types.Restore` Represents both a request to Restore some portion of a Backup into
                    a target GKE cluster and a record of the restore
                    operation itself.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, restore, restore_id])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a gkebackup.CreateRestoreRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, gkebackup.CreateRestoreRequest):
             request = gkebackup.CreateRestoreRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if parent is not None:
                 request.parent = parent
             if restore is not None:
@@ -3240,27 +3216,25 @@
 
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a gkebackup.ListRestoresRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, gkebackup.ListRestoresRequest):
             request = gkebackup.ListRestoresRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if parent is not None:
                 request.parent = parent
 
@@ -3355,27 +3329,25 @@
                 Represents both a request to Restore
                 some portion of a Backup into a target
                 GKE cluster and a record of the restore
                 operation itself.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a gkebackup.GetRestoreRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, gkebackup.GetRestoreRequest):
             request = gkebackup.GetRestoreRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if name is not None:
                 request.name = name
 
@@ -3485,27 +3457,25 @@
 
                 The result type for the operation will be :class:`google.cloud.gke_backup_v1.types.Restore` Represents both a request to Restore some portion of a Backup into
                    a target GKE cluster and a record of the restore
                    operation itself.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([restore, update_mask])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a gkebackup.UpdateRestoreRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, gkebackup.UpdateRestoreRequest):
             request = gkebackup.UpdateRestoreRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if restore is not None:
                 request.restore = restore
             if update_mask is not None:
@@ -3615,27 +3585,25 @@
                          rpc Bar(google.protobuf.Empty) returns
                          (google.protobuf.Empty);
 
                       }
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a gkebackup.DeleteRestoreRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, gkebackup.DeleteRestoreRequest):
             request = gkebackup.DeleteRestoreRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if name is not None:
                 request.name = name
 
@@ -3733,27 +3701,25 @@
                 ListVolumeRestores.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a gkebackup.ListVolumeRestoresRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, gkebackup.ListVolumeRestoresRequest):
             request = gkebackup.ListVolumeRestoresRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if parent is not None:
                 request.parent = parent
 
@@ -3847,27 +3813,25 @@
         Returns:
             google.cloud.gke_backup_v1.types.VolumeRestore:
                 Represents the operation of restoring
                 a volume from a VolumeBackup.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a gkebackup.GetVolumeRestoreRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, gkebackup.GetVolumeRestoreRequest):
             request = gkebackup.GetVolumeRestoreRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if name is not None:
                 request.name = name
 
@@ -3954,27 +3918,25 @@
         Returns:
             google.cloud.gke_backup_v1.types.GetBackupIndexDownloadUrlResponse:
                 Response message for
                 GetBackupIndexDownloadUrl.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([backup])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a gkebackup.GetBackupIndexDownloadUrlRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, gkebackup.GetBackupIndexDownloadUrlRequest):
             request = gkebackup.GetBackupIndexDownloadUrlRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if backup is not None:
                 request.backup = backup
```

### Comparing `google-cloud-gke-backup-0.5.8/google/cloud/gke_backup_v1/services/backup_for_gke/pagers.py` & `google-cloud-gke-backup-0.5.9/google/cloud/gke_backup_v1/services/backup_for_gke/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.5.8/google/cloud/gke_backup_v1/services/backup_for_gke/transports/__init__.py` & `google-cloud-gke-backup-0.5.9/google/cloud/gke_backup_v1/services/backup_for_gke/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.5.8/google/cloud/gke_backup_v1/services/backup_for_gke/transports/base.py` & `google-cloud-gke-backup-0.5.9/google/cloud/gke_backup_v1/services/backup_for_gke/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.5.8/google/cloud/gke_backup_v1/services/backup_for_gke/transports/grpc.py` & `google-cloud-gke-backup-0.5.9/google/cloud/gke_backup_v1/services/backup_for_gke/transports/grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     def __init__(
         self,
         *,
         host: str = "gkebackup.googleapis.com",
         credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
-        channel: Optional[grpc.Channel] = None,
+        channel: Optional[Union[grpc.Channel, Callable[..., grpc.Channel]]] = None,
         api_mtls_endpoint: Optional[str] = None,
         client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
         client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
@@ -78,36 +78,39 @@
             host (Optional[str]):
                  The hostname to connect to (default: 'gkebackup.googleapis.com').
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
-                This argument is ignored if ``channel`` is provided.
+                This argument is ignored if a ``channel`` instance is provided.
             credentials_file (Optional[str]): A file with credentials that can
                 be loaded with :func:`google.auth.load_credentials_from_file`.
-                This argument is ignored if ``channel`` is provided.
+                This argument is ignored if a ``channel`` instance is provided.
             scopes (Optional(Sequence[str])): A list of scopes. This argument is
-                ignored if ``channel`` is provided.
-            channel (Optional[grpc.Channel]): A ``Channel`` instance through
-                which to make calls.
+                ignored if a ``channel`` instance is provided.
+            channel (Optional[Union[grpc.Channel, Callable[..., grpc.Channel]]]):
+                A ``Channel`` instance through which to make calls, or a Callable
+                that constructs and returns one. If set to None, ``self.create_channel``
+                is used to create the channel. If a Callable is given, it will be called
+                with the same arguments as used in ``self.create_channel``.
             api_mtls_endpoint (Optional[str]): Deprecated. The mutual TLS endpoint.
                 If provided, it overrides the ``host`` argument and tries to create
                 a mutual TLS channel with client SSL credentials from
                 ``client_cert_source`` or application default SSL credentials.
             client_cert_source (Optional[Callable[[], Tuple[bytes, bytes]]]):
                 Deprecated. A callback to provide client SSL certificate bytes and
                 private key bytes, both in PEM format. It is ignored if
                 ``api_mtls_endpoint`` is None.
             ssl_channel_credentials (grpc.ChannelCredentials): SSL credentials
-                for the grpc channel. It is ignored if ``channel`` is provided.
+                for the grpc channel. It is ignored if a ``channel`` instance is provided.
             client_cert_source_for_mtls (Optional[Callable[[], Tuple[bytes, bytes]]]):
                 A callback to provide client certificate bytes and private key bytes,
                 both in PEM format. It is used to configure a mutual TLS channel. It is
-                ignored if ``channel`` or ``ssl_channel_credentials`` is provided.
+                ignored if a ``channel`` instance or ``ssl_channel_credentials`` is provided.
             quota_project_id (Optional[str]): An optional project to use for billing
                 and quota.
             client_info (google.api_core.gapic_v1.client_info.ClientInfo):
                 The client info used to send a user-agent string along with
                 API requests. If ``None``, then default info will be used.
                 Generally, you only need to set this if you're developing
                 your own client library.
@@ -126,15 +129,15 @@
         self._operations_client: Optional[operations_v1.OperationsClient] = None
 
         if api_mtls_endpoint:
             warnings.warn("api_mtls_endpoint is deprecated", DeprecationWarning)
         if client_cert_source:
             warnings.warn("client_cert_source is deprecated", DeprecationWarning)
 
-        if channel:
+        if isinstance(channel, grpc.Channel):
             # Ignore credentials if a channel was passed.
             credentials = False
             # If a channel was explicitly provided, set it.
             self._grpc_channel = channel
             self._ssl_channel_credentials = None
 
         else:
@@ -167,15 +170,17 @@
             quota_project_id=quota_project_id,
             client_info=client_info,
             always_use_jwt_access=always_use_jwt_access,
             api_audience=api_audience,
         )
 
         if not self._grpc_channel:
-            self._grpc_channel = type(self).create_channel(
+            # initialize with the provided callable or the default channel
+            channel_init = channel or type(self).create_channel
+            self._grpc_channel = channel_init(
                 self._host,
                 # use the credentials which are saved
                 credentials=self._credentials,
                 # Set ``credentials_file`` to ``None`` here as
                 # the credentials that we saved earlier should be used.
                 credentials_file=None,
                 scopes=self._scopes,
```

### Comparing `google-cloud-gke-backup-0.5.8/google/cloud/gke_backup_v1/services/backup_for_gke/transports/grpc_asyncio.py` & `google-cloud-gke-backup-0.5.9/google/cloud/gke_backup_v1/services/backup_for_gke/transports/grpc_asyncio.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from typing import Awaitable, Callable, Dict, Optional, Sequence, Tuple, Union
 import warnings
 
+from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1, grpc_helpers_async, operations_v1
+from google.api_core import retry_async as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 from google.cloud.location import locations_pb2  # type: ignore
 from google.iam.v1 import iam_policy_pb2  # type: ignore
 from google.iam.v1 import policy_pb2  # type: ignore
 from google.longrunning import operations_pb2  # type: ignore
 import grpc  # type: ignore
@@ -73,15 +75,14 @@
             credentials (Optional[~.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify this application to the service. If
                 none are specified, the client will attempt to ascertain
                 the credentials from the environment.
             credentials_file (Optional[str]): A file with credentials that can
                 be loaded with :func:`google.auth.load_credentials_from_file`.
-                This argument is ignored if ``channel`` is provided.
             scopes (Optional[Sequence[str]]): A optional list of scopes needed for this
                 service. These are only used when credentials are not specified and
                 are passed to :func:`google.auth.default`.
             quota_project_id (Optional[str]): An optional project to use for billing
                 and quota.
             kwargs (Optional[dict]): Keyword arguments, which are passed to the
                 channel creation.
@@ -103,15 +104,15 @@
     def __init__(
         self,
         *,
         host: str = "gkebackup.googleapis.com",
         credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
-        channel: Optional[aio.Channel] = None,
+        channel: Optional[Union[aio.Channel, Callable[..., aio.Channel]]] = None,
         api_mtls_endpoint: Optional[str] = None,
         client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
         client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
@@ -123,37 +124,40 @@
             host (Optional[str]):
                  The hostname to connect to (default: 'gkebackup.googleapis.com').
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
-                This argument is ignored if ``channel`` is provided.
+                This argument is ignored if a ``channel`` instance is provided.
             credentials_file (Optional[str]): A file with credentials that can
                 be loaded with :func:`google.auth.load_credentials_from_file`.
-                This argument is ignored if ``channel`` is provided.
+                This argument is ignored if a ``channel`` instance is provided.
             scopes (Optional[Sequence[str]]): A optional list of scopes needed for this
                 service. These are only used when credentials are not specified and
                 are passed to :func:`google.auth.default`.
-            channel (Optional[aio.Channel]): A ``Channel`` instance through
-                which to make calls.
+            channel (Optional[Union[aio.Channel, Callable[..., aio.Channel]]]):
+                A ``Channel`` instance through which to make calls, or a Callable
+                that constructs and returns one. If set to None, ``self.create_channel``
+                is used to create the channel. If a Callable is given, it will be called
+                with the same arguments as used in ``self.create_channel``.
             api_mtls_endpoint (Optional[str]): Deprecated. The mutual TLS endpoint.
                 If provided, it overrides the ``host`` argument and tries to create
                 a mutual TLS channel with client SSL credentials from
                 ``client_cert_source`` or application default SSL credentials.
             client_cert_source (Optional[Callable[[], Tuple[bytes, bytes]]]):
                 Deprecated. A callback to provide client SSL certificate bytes and
                 private key bytes, both in PEM format. It is ignored if
                 ``api_mtls_endpoint`` is None.
             ssl_channel_credentials (grpc.ChannelCredentials): SSL credentials
-                for the grpc channel. It is ignored if ``channel`` is provided.
+                for the grpc channel. It is ignored if a ``channel`` instance is provided.
             client_cert_source_for_mtls (Optional[Callable[[], Tuple[bytes, bytes]]]):
                 A callback to provide client certificate bytes and private key bytes,
                 both in PEM format. It is used to configure a mutual TLS channel. It is
-                ignored if ``channel`` or ``ssl_channel_credentials`` is provided.
+                ignored if a ``channel`` instance or ``ssl_channel_credentials`` is provided.
             quota_project_id (Optional[str]): An optional project to use for billing
                 and quota.
             client_info (google.api_core.gapic_v1.client_info.ClientInfo):
                 The client info used to send a user-agent string along with
                 API requests. If ``None``, then default info will be used.
                 Generally, you only need to set this if you're developing
                 your own client library.
@@ -172,15 +176,15 @@
         self._operations_client: Optional[operations_v1.OperationsAsyncClient] = None
 
         if api_mtls_endpoint:
             warnings.warn("api_mtls_endpoint is deprecated", DeprecationWarning)
         if client_cert_source:
             warnings.warn("client_cert_source is deprecated", DeprecationWarning)
 
-        if channel:
+        if isinstance(channel, aio.Channel):
             # Ignore credentials if a channel was passed.
             credentials = False
             # If a channel was explicitly provided, set it.
             self._grpc_channel = channel
             self._ssl_channel_credentials = None
         else:
             if api_mtls_endpoint:
@@ -212,15 +216,17 @@
             quota_project_id=quota_project_id,
             client_info=client_info,
             always_use_jwt_access=always_use_jwt_access,
             api_audience=api_audience,
         )
 
         if not self._grpc_channel:
-            self._grpc_channel = type(self).create_channel(
+            # initialize with the provided callable or the default channel
+            channel_init = channel or type(self).create_channel
+            self._grpc_channel = channel_init(
                 self._host,
                 # use the credentials which are saved
                 credentials=self._credentials,
                 # Set ``credentials_file`` to ``None`` here as
                 # the credentials that we saved earlier should be used.
                 credentials_file=None,
                 scopes=self._scopes,
@@ -947,14 +953,261 @@
             ] = self.grpc_channel.unary_unary(
                 "/google.cloud.gkebackup.v1.BackupForGKE/GetBackupIndexDownloadUrl",
                 request_serializer=gkebackup.GetBackupIndexDownloadUrlRequest.serialize,
                 response_deserializer=gkebackup.GetBackupIndexDownloadUrlResponse.deserialize,
             )
         return self._stubs["get_backup_index_download_url"]
 
+    def _prep_wrapped_messages(self, client_info):
+        """Precompute the wrapped methods, overriding the base class method to use async wrappers."""
+        self._wrapped_methods = {
+            self.create_backup_plan: gapic_v1.method_async.wrap_method(
+                self.create_backup_plan,
+                default_timeout=300.0,
+                client_info=client_info,
+            ),
+            self.list_backup_plans: gapic_v1.method_async.wrap_method(
+                self.list_backup_plans,
+                default_retry=retries.AsyncRetry(
+                    initial=1.0,
+                    maximum=60.0,
+                    multiplier=1.3,
+                    predicate=retries.if_exception_type(
+                        core_exceptions.ServiceUnavailable,
+                    ),
+                    deadline=60.0,
+                ),
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
+            self.get_backup_plan: gapic_v1.method_async.wrap_method(
+                self.get_backup_plan,
+                default_retry=retries.AsyncRetry(
+                    initial=1.0,
+                    maximum=60.0,
+                    multiplier=1.3,
+                    predicate=retries.if_exception_type(
+                        core_exceptions.ServiceUnavailable,
+                    ),
+                    deadline=60.0,
+                ),
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
+            self.update_backup_plan: gapic_v1.method_async.wrap_method(
+                self.update_backup_plan,
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
+            self.delete_backup_plan: gapic_v1.method_async.wrap_method(
+                self.delete_backup_plan,
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
+            self.create_backup: gapic_v1.method_async.wrap_method(
+                self.create_backup,
+                default_timeout=120.0,
+                client_info=client_info,
+            ),
+            self.list_backups: gapic_v1.method_async.wrap_method(
+                self.list_backups,
+                default_retry=retries.AsyncRetry(
+                    initial=1.0,
+                    maximum=60.0,
+                    multiplier=1.3,
+                    predicate=retries.if_exception_type(
+                        core_exceptions.ServiceUnavailable,
+                    ),
+                    deadline=60.0,
+                ),
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
+            self.get_backup: gapic_v1.method_async.wrap_method(
+                self.get_backup,
+                default_retry=retries.AsyncRetry(
+                    initial=1.0,
+                    maximum=60.0,
+                    multiplier=1.3,
+                    predicate=retries.if_exception_type(
+                        core_exceptions.ServiceUnavailable,
+                    ),
+                    deadline=60.0,
+                ),
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
+            self.update_backup: gapic_v1.method_async.wrap_method(
+                self.update_backup,
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
+            self.delete_backup: gapic_v1.method_async.wrap_method(
+                self.delete_backup,
+                default_timeout=300.0,
+                client_info=client_info,
+            ),
+            self.list_volume_backups: gapic_v1.method_async.wrap_method(
+                self.list_volume_backups,
+                default_retry=retries.AsyncRetry(
+                    initial=1.0,
+                    maximum=60.0,
+                    multiplier=1.3,
+                    predicate=retries.if_exception_type(
+                        core_exceptions.ServiceUnavailable,
+                    ),
+                    deadline=60.0,
+                ),
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
+            self.get_volume_backup: gapic_v1.method_async.wrap_method(
+                self.get_volume_backup,
+                default_retry=retries.AsyncRetry(
+                    initial=1.0,
+                    maximum=60.0,
+                    multiplier=1.3,
+                    predicate=retries.if_exception_type(
+                        core_exceptions.ServiceUnavailable,
+                    ),
+                    deadline=60.0,
+                ),
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
+            self.create_restore_plan: gapic_v1.method_async.wrap_method(
+                self.create_restore_plan,
+                default_timeout=120.0,
+                client_info=client_info,
+            ),
+            self.list_restore_plans: gapic_v1.method_async.wrap_method(
+                self.list_restore_plans,
+                default_retry=retries.AsyncRetry(
+                    initial=1.0,
+                    maximum=60.0,
+                    multiplier=1.3,
+                    predicate=retries.if_exception_type(
+                        core_exceptions.ServiceUnavailable,
+                    ),
+                    deadline=60.0,
+                ),
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
+            self.get_restore_plan: gapic_v1.method_async.wrap_method(
+                self.get_restore_plan,
+                default_retry=retries.AsyncRetry(
+                    initial=1.0,
+                    maximum=60.0,
+                    multiplier=1.3,
+                    predicate=retries.if_exception_type(
+                        core_exceptions.ServiceUnavailable,
+                    ),
+                    deadline=60.0,
+                ),
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
+            self.update_restore_plan: gapic_v1.method_async.wrap_method(
+                self.update_restore_plan,
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
+            self.delete_restore_plan: gapic_v1.method_async.wrap_method(
+                self.delete_restore_plan,
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
+            self.create_restore: gapic_v1.method_async.wrap_method(
+                self.create_restore,
+                default_timeout=120.0,
+                client_info=client_info,
+            ),
+            self.list_restores: gapic_v1.method_async.wrap_method(
+                self.list_restores,
+                default_retry=retries.AsyncRetry(
+                    initial=1.0,
+                    maximum=60.0,
+                    multiplier=1.3,
+                    predicate=retries.if_exception_type(
+                        core_exceptions.ServiceUnavailable,
+                    ),
+                    deadline=60.0,
+                ),
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
+            self.get_restore: gapic_v1.method_async.wrap_method(
+                self.get_restore,
+                default_retry=retries.AsyncRetry(
+                    initial=1.0,
+                    maximum=60.0,
+                    multiplier=1.3,
+                    predicate=retries.if_exception_type(
+                        core_exceptions.ServiceUnavailable,
+                    ),
+                    deadline=60.0,
+                ),
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
+            self.update_restore: gapic_v1.method_async.wrap_method(
+                self.update_restore,
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
+            self.delete_restore: gapic_v1.method_async.wrap_method(
+                self.delete_restore,
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
+            self.list_volume_restores: gapic_v1.method_async.wrap_method(
+                self.list_volume_restores,
+                default_retry=retries.AsyncRetry(
+                    initial=1.0,
+                    maximum=60.0,
+                    multiplier=1.3,
+                    predicate=retries.if_exception_type(
+                        core_exceptions.ServiceUnavailable,
+                    ),
+                    deadline=60.0,
+                ),
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
+            self.get_volume_restore: gapic_v1.method_async.wrap_method(
+                self.get_volume_restore,
+                default_retry=retries.AsyncRetry(
+                    initial=1.0,
+                    maximum=60.0,
+                    multiplier=1.3,
+                    predicate=retries.if_exception_type(
+                        core_exceptions.ServiceUnavailable,
+                    ),
+                    deadline=60.0,
+                ),
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
+            self.get_backup_index_download_url: gapic_v1.method_async.wrap_method(
+                self.get_backup_index_download_url,
+                default_retry=retries.AsyncRetry(
+                    initial=1.0,
+                    maximum=60.0,
+                    multiplier=1.3,
+                    predicate=retries.if_exception_type(
+                        core_exceptions.ServiceUnavailable,
+                    ),
+                    deadline=60.0,
+                ),
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
+        }
+
     def close(self):
         return self.grpc_channel.close()
 
     @property
     def delete_operation(
         self,
     ) -> Callable[[operations_pb2.DeleteOperationRequest], None]:
```

### Comparing `google-cloud-gke-backup-0.5.8/google/cloud/gke_backup_v1/services/backup_for_gke/transports/rest.py` & `google-cloud-gke-backup-0.5.9/google/cloud/gke_backup_v1/services/backup_for_gke/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.5.8/google/cloud/gke_backup_v1/types/__init__.py` & `google-cloud-gke-backup-0.5.9/google/cloud/gke_backup_v1/types/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,21 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from .backup import Backup
 from .backup_plan import BackupPlan, ExclusionWindow, RpoConfig
-from .common import EncryptionKey, NamespacedName, NamespacedNames, Namespaces
+from .common import (
+    EncryptionKey,
+    NamespacedName,
+    NamespacedNames,
+    Namespaces,
+    VolumeTypeEnum,
+)
 from .gkebackup import (
     CreateBackupPlanRequest,
     CreateBackupRequest,
     CreateRestorePlanRequest,
     CreateRestoreRequest,
     DeleteBackupPlanRequest,
     DeleteBackupRequest,
@@ -47,27 +53,33 @@
     ListVolumeRestoresResponse,
     OperationMetadata,
     UpdateBackupPlanRequest,
     UpdateBackupRequest,
     UpdateRestorePlanRequest,
     UpdateRestoreRequest,
 )
-from .restore import Restore, RestoreConfig
+from .restore import (
+    ResourceSelector,
+    Restore,
+    RestoreConfig,
+    VolumeDataRestorePolicyOverride,
+)
 from .restore_plan import RestorePlan
 from .volume import VolumeBackup, VolumeRestore
 
 __all__ = (
     "Backup",
     "BackupPlan",
     "ExclusionWindow",
     "RpoConfig",
     "EncryptionKey",
     "NamespacedName",
     "NamespacedNames",
     "Namespaces",
+    "VolumeTypeEnum",
     "CreateBackupPlanRequest",
     "CreateBackupRequest",
     "CreateRestorePlanRequest",
     "CreateRestoreRequest",
     "DeleteBackupPlanRequest",
     "DeleteBackupRequest",
     "DeleteRestorePlanRequest",
@@ -93,13 +105,15 @@
     "ListVolumeRestoresRequest",
     "ListVolumeRestoresResponse",
     "OperationMetadata",
     "UpdateBackupPlanRequest",
     "UpdateBackupRequest",
     "UpdateRestorePlanRequest",
     "UpdateRestoreRequest",
+    "ResourceSelector",
     "Restore",
     "RestoreConfig",
+    "VolumeDataRestorePolicyOverride",
     "RestorePlan",
     "VolumeBackup",
     "VolumeRestore",
 )
```

### Comparing `google-cloud-gke-backup-0.5.8/google/cloud/gke_backup_v1/types/backup.py` & `google-cloud-gke-backup-0.5.9/google/cloud/gke_backup_v1/types/backup.py`

 * *Files 5% similar despite different names*

```diff
@@ -167,14 +167,22 @@
             for this Backup.
         pod_count (int):
             Output only. The total number of Kubernetes
             Pods contained in the Backup.
         config_backup_size_bytes (int):
             Output only. The size of the config backup in
             bytes.
+        permissive_mode (bool):
+            Output only. If false, Backup will fail when Backup for GKE
+            detects Kubernetes configuration that is non-standard or
+            requires additional setup to restore.
+
+            Inherited from the parent BackupPlan's
+            [permissive_mode][google.cloud.gkebackup.v1.BackupPlan.BackupConfig.permissive_mode]
+            value.
     """
 
     class State(proto.Enum):
         r"""State
 
         Values:
             STATE_UNSPECIFIED (0):
@@ -383,10 +391,14 @@
         proto.INT32,
         number=26,
     )
     config_backup_size_bytes: int = proto.Field(
         proto.INT64,
         number=27,
     )
+    permissive_mode: bool = proto.Field(
+        proto.BOOL,
+        number=28,
+    )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-gke-backup-0.5.8/google/cloud/gke_backup_v1/types/backup_plan.py` & `google-cloud-gke-backup-0.5.9/google/cloud/gke_backup_v1/types/backup_plan.py`

 * *Files 2% similar despite different names*

```diff
@@ -309,14 +309,21 @@
                 Optional. This defines a customer managed
                 encryption key that will be used to encrypt the
                 "config" portion (the Kubernetes resources) of
                 Backups created via this plan.
 
                 Default (empty): Config backup artifacts will
                 not be encrypted.
+            permissive_mode (bool):
+                Optional. If false, Backups will fail when
+                Backup for GKE detects Kubernetes configuration
+                that is non-standard or requires additional
+                setup to restore.
+
+                Default: False
         """
 
         all_namespaces: bool = proto.Field(
             proto.BOOL,
             number=1,
             oneof="backup_scope",
         )
@@ -341,14 +348,18 @@
             number=5,
         )
         encryption_key: common.EncryptionKey = proto.Field(
             proto.MESSAGE,
             number=6,
             message=common.EncryptionKey,
         )
+        permissive_mode: bool = proto.Field(
+            proto.BOOL,
+            number=7,
+        )
 
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
     uid: str = proto.Field(
         proto.STRING,
@@ -470,17 +481,18 @@
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
     Attributes:
         start_time (google.type.timeofday_pb2.TimeOfDay):
             Required. Specifies the start time of the
             window using time of the day in UTC.
         duration (google.protobuf.duration_pb2.Duration):
-            Required. Specifies duration of the window. Restrictions for
-            duration based on the recurrence type to allow some time for
-            backup to happen:
+            Required. Specifies duration of the window. Duration must be
+            >= 5 minutes and < (target RPO - 20 minutes). Additional
+            restrictions based on the recurrence type to allow some time
+            for backup to happen:
 
             -  single_occurrence_date: no restriction, but UI may warn
                about this when duration >= target RPO
             -  daily window: duration < 24 hours
             -  weekly window:
 
                -  days of week includes all seven days of a week:
```

### Comparing `google-cloud-gke-backup-0.5.8/google/cloud/gke_backup_v1/types/gkebackup.py` & `google-cloud-gke-backup-0.5.9/google/cloud/gke_backup_v1/types/gkebackup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.5.8/google/cloud/gke_backup_v1/types/restore.py` & `google-cloud-gke-backup-0.5.9/google/cloud/gke_backup_v1/types/restore.py`

 * *Files 19% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 from google.cloud.gke_backup_v1.types import common
 
 __protobuf__ = proto.module(
     package="google.cloud.gkebackup.v1",
     manifest={
         "Restore",
         "RestoreConfig",
+        "ResourceSelector",
+        "VolumeDataRestorePolicyOverride",
     },
 )
 
 
 class Restore(proto.Message):
     r"""Represents both a request to Restore some portion of a Backup
     into a target GKE cluster and a record of the restore operation
@@ -104,14 +106,30 @@
             suggested that systems make use of the ``etag`` in the
             read-modify-write cycle to perform restore updates in order
             to avoid race conditions: An ``etag`` is returned in the
             response to ``GetRestore``, and systems are expected to put
             that etag in the request to ``UpdateRestore`` or
             ``DeleteRestore`` to ensure that their change will be
             applied to the same version of the resource.
+        filter (google.cloud.gke_backup_v1.types.Restore.Filter):
+            Optional. Immutable. Filters resources for ``Restore``. If
+            not specified, the scope of the restore will remain the same
+            as defined in the ``RestorePlan``. If this is specified, and
+            no resources are matched by the ``inclusion_filters`` or
+            everyting is excluded by the ``exclusion_filters``, nothing
+            will be restored. This filter can only be specified if the
+            value of
+            [namespaced_resource_restore_mode][google.cloud.gkebackup.v1.RestoreConfig.namespaced_resource_restore_mode]
+            is set to ``MERGE_SKIP_ON_CONFLICT``,
+            ``MERGE_REPLACE_VOLUME_ON_CONFLICT`` or
+            ``MERGE_REPLACE_ON_CONFLICT``.
+        volume_data_restore_policy_overrides (MutableSequence[google.cloud.gke_backup_v1.types.VolumeDataRestorePolicyOverride]):
+            Optional. Immutable. Overrides the volume
+            data restore policies selected in the Restore
+            Config for override-scoped resources.
     """
 
     class State(proto.Enum):
         r"""Possible values for state of the Restore.
 
         Values:
             STATE_UNSPECIFIED (0):
@@ -137,14 +155,46 @@
         STATE_UNSPECIFIED = 0
         CREATING = 1
         IN_PROGRESS = 2
         SUCCEEDED = 3
         FAILED = 4
         DELETING = 5
 
+    class Filter(proto.Message):
+        r"""Defines the filter for ``Restore``. This filter can be used to
+        further refine the resource selection of the ``Restore`` beyond the
+        coarse-grained scope defined in the ``RestorePlan``.
+        ``exclusion_filters`` take precedence over ``inclusion_filters``. If
+        a resource matches both ``inclusion_filters`` and
+        ``exclusion_filters``, it will not be restored.
+
+        Attributes:
+            inclusion_filters (MutableSequence[google.cloud.gke_backup_v1.types.ResourceSelector]):
+                Optional. Selects resources for restoration. If specified,
+                only resources which match ``inclusion_filters`` will be
+                selected for restoration. A resource will be selected if it
+                matches any ``ResourceSelector`` of the
+                ``inclusion_filters``.
+            exclusion_filters (MutableSequence[google.cloud.gke_backup_v1.types.ResourceSelector]):
+                Optional. Excludes resources from restoration. If specified,
+                a resource will not be restored if it matches any
+                ``ResourceSelector`` of the ``exclusion_filters``.
+        """
+
+        inclusion_filters: MutableSequence["ResourceSelector"] = proto.RepeatedField(
+            proto.MESSAGE,
+            number=1,
+            message="ResourceSelector",
+        )
+        exclusion_filters: MutableSequence["ResourceSelector"] = proto.RepeatedField(
+            proto.MESSAGE,
+            number=2,
+            message="ResourceSelector",
+        )
+
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
     uid: str = proto.Field(
         proto.STRING,
         number=2,
@@ -211,14 +261,26 @@
         proto.INT32,
         number=16,
     )
     etag: str = proto.Field(
         proto.STRING,
         number=17,
     )
+    filter: Filter = proto.Field(
+        proto.MESSAGE,
+        number=18,
+        message=Filter,
+    )
+    volume_data_restore_policy_overrides: MutableSequence[
+        "VolumeDataRestorePolicyOverride"
+    ] = proto.RepeatedField(
+        proto.MESSAGE,
+        number=19,
+        message="VolumeDataRestorePolicyOverride",
+    )
 
 
 class RestoreConfig(proto.Message):
     r"""Configuration of a restore.
 
     This message has `oneof`_ fields (mutually exclusive fields).
     For each oneof, at most one member field can be set at the same time.
@@ -292,14 +354,22 @@
             Optional. A list of transformation rules to
             be applied against Kubernetes resources as they
             are selected for restoration from a Backup.
             Rules are executed in order defined - this order
             matters, as changes made by a rule may impact
             the filtering logic of subsequent rules. An
             empty list means no transformation will occur.
+        volume_data_restore_policy_bindings (MutableSequence[google.cloud.gke_backup_v1.types.RestoreConfig.VolumeDataRestorePolicyBinding]):
+            Optional. A table that binds volumes by their scope to a
+            restore policy. Bindings must have a unique scope. Any
+            volumes not scoped in the bindings are subject to the policy
+            defined in volume_data_restore_policy.
+        restore_order (google.cloud.gke_backup_v1.types.RestoreConfig.RestoreOrder):
+            Optional. RestoreOrder contains custom
+            ordering to use on a Restore.
     """
 
     class VolumeDataRestorePolicy(proto.Enum):
         r"""Defines how volume data should be restored.
 
         Values:
             VOLUME_DATA_RESTORE_POLICY_UNSPECIFIED (0):
@@ -376,18 +446,59 @@
                 Namespaces or ProtectedApplications, depending
                 upon the scope) are encountered at the beginning
                 of a restore process, the Restore will fail.  If
                 a conflict occurs during the restore process
                 itself (e.g., because an out of band process
                 creates conflicting resources), a conflict will
                 be reported.
+            MERGE_SKIP_ON_CONFLICT (3):
+                This mode merges the backup and the target
+                cluster and skips the conflicting resources. If
+                a single resource to restore exists in the
+                cluster before restoration, the resource will be
+                skipped, otherwise it will be restored.
+            MERGE_REPLACE_VOLUME_ON_CONFLICT (4):
+                This mode merges the backup and the target cluster and skips
+                the conflicting resources except volume data. If a PVC to
+                restore already exists, this mode will restore/reconnect the
+                volume without overwriting the PVC. It is similar to
+                MERGE_SKIP_ON_CONFLICT except that it will apply the volume
+                data policy for the conflicting PVCs:
+
+                -  RESTORE_VOLUME_DATA_FROM_BACKUP: restore data only and
+                   respect the reclaim policy of the original PV;
+                -  REUSE_VOLUME_HANDLE_FROM_BACKUP: reconnect and respect
+                   the reclaim policy of the original PV;
+                -  NO_VOLUME_DATA_RESTORATION: new provision and respect the
+                   reclaim policy of the original PV. Note that this mode
+                   could cause data loss as the original PV can be retained
+                   or deleted depending on its reclaim policy.
+            MERGE_REPLACE_ON_CONFLICT (5):
+                This mode merges the backup and the target
+                cluster and replaces the conflicting resources
+                with the ones in the backup. If a single
+                resource to restore exists in the cluster before
+                restoration, the resource will be replaced with
+                the one from the backup. To replace an existing
+                resource, the first attempt is to update the
+                resource to match the one from the backup; if
+                the update fails, the second attempt is to
+                delete the resource and restore it from the
+                backup.
+                Note that this mode could cause data loss as it
+                replaces the existing resources in the target
+                cluster, and the original PV can be retained or
+                deleted depending on its reclaim policy.
         """
         NAMESPACED_RESOURCE_RESTORE_MODE_UNSPECIFIED = 0
         DELETE_AND_RESTORE = 1
         FAIL_ON_CONFLICT = 2
+        MERGE_SKIP_ON_CONFLICT = 3
+        MERGE_REPLACE_VOLUME_ON_CONFLICT = 4
+        MERGE_REPLACE_ON_CONFLICT = 5
 
     class GroupKind(proto.Message):
         r"""This is a direct map to the Kubernetes GroupKind type
         `GroupKind <https://godoc.org/k8s.io/apimachinery/pkg/runtime/schema#GroupKind>`__
         and is used for identifying specific "types" of resources to
         restore.
 
@@ -740,14 +851,89 @@
             message="RestoreConfig.ResourceFilter",
         )
         description: str = proto.Field(
             proto.STRING,
             number=3,
         )
 
+    class VolumeDataRestorePolicyBinding(proto.Message):
+        r"""Binds resources in the scope to the given
+        VolumeDataRestorePolicy.
+
+
+        .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
+
+        Attributes:
+            policy (google.cloud.gke_backup_v1.types.RestoreConfig.VolumeDataRestorePolicy):
+                Required. The VolumeDataRestorePolicy to
+                apply when restoring volumes in scope.
+            volume_type (google.cloud.gke_backup_v1.types.VolumeTypeEnum.VolumeType):
+                The volume type, as determined by the PVC's
+                bound PV, to apply the policy to.
+
+                This field is a member of `oneof`_ ``scope``.
+        """
+
+        policy: "RestoreConfig.VolumeDataRestorePolicy" = proto.Field(
+            proto.ENUM,
+            number=1,
+            enum="RestoreConfig.VolumeDataRestorePolicy",
+        )
+        volume_type: common.VolumeTypeEnum.VolumeType = proto.Field(
+            proto.ENUM,
+            number=2,
+            oneof="scope",
+            enum=common.VolumeTypeEnum.VolumeType,
+        )
+
+    class RestoreOrder(proto.Message):
+        r"""Allows customers to specify dependencies between resources
+        that Backup for GKE can use to compute a resasonable restore
+        order.
+
+        Attributes:
+            group_kind_dependencies (MutableSequence[google.cloud.gke_backup_v1.types.RestoreConfig.RestoreOrder.GroupKindDependency]):
+                Optional. Contains a list of group kind
+                dependency pairs provided by the customer, that
+                is used by Backup for GKE to generate a group
+                kind restore order.
+        """
+
+        class GroupKindDependency(proto.Message):
+            r"""Defines a dependency between two group kinds.
+
+            Attributes:
+                satisfying (google.cloud.gke_backup_v1.types.RestoreConfig.GroupKind):
+                    Required. The satisfying group kind must be
+                    restored first in order to satisfy the
+                    dependency.
+                requiring (google.cloud.gke_backup_v1.types.RestoreConfig.GroupKind):
+                    Required. The requiring group kind requires
+                    that the other group kind be restored first.
+            """
+
+            satisfying: "RestoreConfig.GroupKind" = proto.Field(
+                proto.MESSAGE,
+                number=1,
+                message="RestoreConfig.GroupKind",
+            )
+            requiring: "RestoreConfig.GroupKind" = proto.Field(
+                proto.MESSAGE,
+                number=2,
+                message="RestoreConfig.GroupKind",
+            )
+
+        group_kind_dependencies: MutableSequence[
+            "RestoreConfig.RestoreOrder.GroupKindDependency"
+        ] = proto.RepeatedField(
+            proto.MESSAGE,
+            number=1,
+            message="RestoreConfig.RestoreOrder.GroupKindDependency",
+        )
+
     volume_data_restore_policy: VolumeDataRestorePolicy = proto.Field(
         proto.ENUM,
         number=1,
         enum=VolumeDataRestorePolicy,
     )
     cluster_resource_conflict_policy: ClusterResourceConflictPolicy = proto.Field(
         proto.ENUM,
@@ -798,10 +984,111 @@
         message=SubstitutionRule,
     )
     transformation_rules: MutableSequence[TransformationRule] = proto.RepeatedField(
         proto.MESSAGE,
         number=11,
         message=TransformationRule,
     )
+    volume_data_restore_policy_bindings: MutableSequence[
+        VolumeDataRestorePolicyBinding
+    ] = proto.RepeatedField(
+        proto.MESSAGE,
+        number=12,
+        message=VolumeDataRestorePolicyBinding,
+    )
+    restore_order: RestoreOrder = proto.Field(
+        proto.MESSAGE,
+        number=13,
+        message=RestoreOrder,
+    )
+
+
+class ResourceSelector(proto.Message):
+    r"""Defines a selector to identify a single or a group of
+    resources. Conditions in the selector are optional, but at least
+    one field should be set to a non-empty value. If a condition is
+    not specified, no restrictions will be applied on that
+    dimension.
+    If more than one condition is specified, a resource will be
+    selected if and only if all conditions are met.
+
+    Attributes:
+        group_kind (google.cloud.gke_backup_v1.types.RestoreConfig.GroupKind):
+            Optional. Selects resources using their
+            Kubernetes GroupKinds. If specified, only
+            resources of provided GroupKind will be
+            selected.
+        name (str):
+            Optional. Selects resources using their
+            resource names. If specified, only resources
+            with the provided name will be selected.
+        namespace (str):
+            Optional. Selects resources using their namespaces. This
+            only applies to namespace scoped resources and cannot be
+            used for selecting cluster scoped resources. If specified,
+            only resources in the provided namespace will be selected.
+            If not specified, the filter will apply to both cluster
+            scoped and namespace scoped resources (e.g. name or label).
+            The
+            `Namespace <https://pkg.go.dev/k8s.io/api/core/v1#Namespace>`__
+            resource itself will be restored if and only if any
+            resources within the namespace are restored.
+        labels (MutableMapping[str, str]):
+            Optional. Selects resources using Kubernetes
+            `labels <https://kubernetes.io/docs/concepts/overview/working-with-objects/labels/>`__.
+            If specified, a resource will be selected if and only if the
+            resource has all of the provided labels and all the label
+            values match.
+    """
+
+    group_kind: "RestoreConfig.GroupKind" = proto.Field(
+        proto.MESSAGE,
+        number=1,
+        message="RestoreConfig.GroupKind",
+    )
+    name: str = proto.Field(
+        proto.STRING,
+        number=2,
+    )
+    namespace: str = proto.Field(
+        proto.STRING,
+        number=3,
+    )
+    labels: MutableMapping[str, str] = proto.MapField(
+        proto.STRING,
+        proto.STRING,
+        number=4,
+    )
+
+
+class VolumeDataRestorePolicyOverride(proto.Message):
+    r"""Defines an override to apply a VolumeDataRestorePolicy for
+    scoped resources.
+
+
+    .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
+
+    Attributes:
+        policy (google.cloud.gke_backup_v1.types.RestoreConfig.VolumeDataRestorePolicy):
+            Required. The VolumeDataRestorePolicy to
+            apply when restoring volumes in scope.
+        selected_pvcs (google.cloud.gke_backup_v1.types.NamespacedNames):
+            A list of PVCs to apply the policy override
+            to.
+
+            This field is a member of `oneof`_ ``scope``.
+    """
+
+    policy: "RestoreConfig.VolumeDataRestorePolicy" = proto.Field(
+        proto.ENUM,
+        number=1,
+        enum="RestoreConfig.VolumeDataRestorePolicy",
+    )
+    selected_pvcs: common.NamespacedNames = proto.Field(
+        proto.MESSAGE,
+        number=2,
+        oneof="scope",
+        message=common.NamespacedNames,
+    )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-gke-backup-0.5.8/google/cloud/gke_backup_v1/types/restore_plan.py` & `google-cloud-gke-backup-0.5.9/google/cloud/gke_backup_v1/types/restore_plan.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.5.8/google/cloud/gke_backup_v1/types/volume.py` & `google-cloud-gke-backup-0.5.9/google/cloud/gke_backup_v1/types/volume.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.5.8/google_cloud_gke_backup.egg-info/PKG-INFO` & `google-cloud-gke-backup-0.5.9/google_cloud_gke_backup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-gke-backup
-Version: 0.5.8
+Version: 0.5.9
 Summary: Google Cloud Gke Backup API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-gke-backup
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-gke-backup-0.5.8/google_cloud_gke_backup.egg-info/SOURCES.txt` & `google-cloud-gke-backup-0.5.9/google_cloud_gke_backup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.5.8/setup.py` & `google-cloud-gke-backup-0.5.9/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.5.8/tests/__init__.py` & `google-cloud-gke-backup-0.5.9/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.5.8/tests/unit/__init__.py` & `google-cloud-gke-backup-0.5.9/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.5.8/tests/unit/gapic/__init__.py` & `google-cloud-gke-backup-0.5.9/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.5.8/tests/unit/gapic/gke_backup_v1/__init__.py` & `google-cloud-gke-backup-0.5.9/tests/unit/gapic/gke_backup_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.5.8/tests/unit/gapic/gke_backup_v1/test_backup_for_gke.py` & `google-cloud-gke-backup-0.5.9/tests/unit/gapic/gke_backup_v1/test_backup_for_gke.py`

 * *Files 13% similar despite different names*

```diff
@@ -1166,14 +1166,17 @@
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.create_backup_plan), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.create_backup_plan()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.CreateBackupPlanRequest()
 
 
 def test_create_backup_plan_non_empty_request_with_auto_populated_field():
@@ -1192,23 +1195,69 @@
         backup_plan_id="backup_plan_id_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.create_backup_plan), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.create_backup_plan(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.CreateBackupPlanRequest(
             parent="parent_value",
             backup_plan_id="backup_plan_id_value",
         )
 
 
+def test_create_backup_plan_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = BackupForGKEClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.create_backup_plan in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.create_backup_plan
+        ] = mock_rpc
+        request = {}
+        client.create_backup_plan(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        # Operation methods build a cached wrapper on first rpc call
+        # subsequent calls should use the cached wrapper
+        wrapper_fn.reset_mock()
+
+        client.create_backup_plan(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_create_backup_plan_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = BackupForGKEAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -1225,14 +1274,64 @@
         response = await client.create_backup_plan()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.CreateBackupPlanRequest()
 
 
 @pytest.mark.asyncio
+async def test_create_backup_plan_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = BackupForGKEAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.create_backup_plan
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.create_backup_plan
+        ] = mock_object
+
+        request = {}
+        await client.create_backup_plan(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        # Operation methods build a cached wrapper on first rpc call
+        # subsequent calls should use the cached wrapper
+        wrapper_fn.reset_mock()
+
+        await client.create_backup_plan(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_create_backup_plan_async(
     transport: str = "grpc_asyncio", request_type=gkebackup.CreateBackupPlanRequest
 ):
     client = BackupForGKEAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
@@ -1485,14 +1584,17 @@
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_backup_plans), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.list_backup_plans()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.ListBackupPlansRequest()
 
 
 def test_list_backup_plans_non_empty_request_with_auto_populated_field():
@@ -1513,25 +1615,65 @@
         order_by="order_by_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_backup_plans), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.list_backup_plans(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.ListBackupPlansRequest(
             parent="parent_value",
             page_token="page_token_value",
             filter="filter_value",
             order_by="order_by_value",
         )
 
 
+def test_list_backup_plans_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = BackupForGKEClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.list_backup_plans in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.list_backup_plans
+        ] = mock_rpc
+        request = {}
+        client.list_backup_plans(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.list_backup_plans(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_list_backup_plans_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = BackupForGKEAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -1551,14 +1693,60 @@
         response = await client.list_backup_plans()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.ListBackupPlansRequest()
 
 
 @pytest.mark.asyncio
+async def test_list_backup_plans_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = BackupForGKEAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.list_backup_plans
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.list_backup_plans
+        ] = mock_object
+
+        request = {}
+        await client.list_backup_plans(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.list_backup_plans(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_list_backup_plans_async(
     transport: str = "grpc_asyncio", request_type=gkebackup.ListBackupPlansRequest
 ):
     client = BackupForGKEAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
@@ -2008,14 +2196,17 @@
     client = BackupForGKEClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_backup_plan), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.get_backup_plan()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.GetBackupPlanRequest()
 
 
 def test_get_backup_plan_non_empty_request_with_auto_populated_field():
@@ -2031,22 +2222,60 @@
     # if they meet the requirements of AIP 4235.
     request = gkebackup.GetBackupPlanRequest(
         name="name_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_backup_plan), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.get_backup_plan(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.GetBackupPlanRequest(
             name="name_value",
         )
 
 
+def test_get_backup_plan_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = BackupForGKEClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.get_backup_plan in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.get_backup_plan] = mock_rpc
+        request = {}
+        client.get_backup_plan(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.get_backup_plan(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_get_backup_plan_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = BackupForGKEAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -2073,14 +2302,60 @@
         response = await client.get_backup_plan()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.GetBackupPlanRequest()
 
 
 @pytest.mark.asyncio
+async def test_get_backup_plan_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = BackupForGKEAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.get_backup_plan
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.get_backup_plan
+        ] = mock_object
+
+        request = {}
+        await client.get_backup_plan(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.get_backup_plan(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_get_backup_plan_async(
     transport: str = "grpc_asyncio", request_type=gkebackup.GetBackupPlanRequest
 ):
     client = BackupForGKEAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
@@ -2321,14 +2596,17 @@
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.update_backup_plan), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.update_backup_plan()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.UpdateBackupPlanRequest()
 
 
 def test_update_backup_plan_non_empty_request_with_auto_populated_field():
@@ -2344,20 +2622,66 @@
     # if they meet the requirements of AIP 4235.
     request = gkebackup.UpdateBackupPlanRequest()
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.update_backup_plan), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.update_backup_plan(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.UpdateBackupPlanRequest()
 
 
+def test_update_backup_plan_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = BackupForGKEClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.update_backup_plan in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.update_backup_plan
+        ] = mock_rpc
+        request = {}
+        client.update_backup_plan(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        # Operation methods build a cached wrapper on first rpc call
+        # subsequent calls should use the cached wrapper
+        wrapper_fn.reset_mock()
+
+        client.update_backup_plan(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_update_backup_plan_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = BackupForGKEAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -2374,14 +2698,64 @@
         response = await client.update_backup_plan()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.UpdateBackupPlanRequest()
 
 
 @pytest.mark.asyncio
+async def test_update_backup_plan_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = BackupForGKEAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.update_backup_plan
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.update_backup_plan
+        ] = mock_object
+
+        request = {}
+        await client.update_backup_plan(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        # Operation methods build a cached wrapper on first rpc call
+        # subsequent calls should use the cached wrapper
+        wrapper_fn.reset_mock()
+
+        await client.update_backup_plan(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_update_backup_plan_async(
     transport: str = "grpc_asyncio", request_type=gkebackup.UpdateBackupPlanRequest
 ):
     client = BackupForGKEAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
@@ -2619,14 +2993,17 @@
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.delete_backup_plan), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.delete_backup_plan()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.DeleteBackupPlanRequest()
 
 
 def test_delete_backup_plan_non_empty_request_with_auto_populated_field():
@@ -2645,23 +3022,69 @@
         etag="etag_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.delete_backup_plan), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.delete_backup_plan(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.DeleteBackupPlanRequest(
             name="name_value",
             etag="etag_value",
         )
 
 
+def test_delete_backup_plan_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = BackupForGKEClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.delete_backup_plan in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.delete_backup_plan
+        ] = mock_rpc
+        request = {}
+        client.delete_backup_plan(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        # Operation methods build a cached wrapper on first rpc call
+        # subsequent calls should use the cached wrapper
+        wrapper_fn.reset_mock()
+
+        client.delete_backup_plan(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_delete_backup_plan_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = BackupForGKEAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -2678,14 +3101,64 @@
         response = await client.delete_backup_plan()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.DeleteBackupPlanRequest()
 
 
 @pytest.mark.asyncio
+async def test_delete_backup_plan_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = BackupForGKEAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.delete_backup_plan
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.delete_backup_plan
+        ] = mock_object
+
+        request = {}
+        await client.delete_backup_plan(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        # Operation methods build a cached wrapper on first rpc call
+        # subsequent calls should use the cached wrapper
+        wrapper_fn.reset_mock()
+
+        await client.delete_backup_plan(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_delete_backup_plan_async(
     transport: str = "grpc_asyncio", request_type=gkebackup.DeleteBackupPlanRequest
 ):
     client = BackupForGKEAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
@@ -2909,14 +3382,17 @@
     client = BackupForGKEClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.create_backup), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.create_backup()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.CreateBackupRequest()
 
 
 def test_create_backup_non_empty_request_with_auto_populated_field():
@@ -2933,23 +3409,65 @@
     request = gkebackup.CreateBackupRequest(
         parent="parent_value",
         backup_id="backup_id_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.create_backup), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.create_backup(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.CreateBackupRequest(
             parent="parent_value",
             backup_id="backup_id_value",
         )
 
 
+def test_create_backup_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = BackupForGKEClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.create_backup in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.create_backup] = mock_rpc
+        request = {}
+        client.create_backup(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        # Operation methods build a cached wrapper on first rpc call
+        # subsequent calls should use the cached wrapper
+        wrapper_fn.reset_mock()
+
+        client.create_backup(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_create_backup_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = BackupForGKEAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -2964,14 +3482,64 @@
         response = await client.create_backup()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.CreateBackupRequest()
 
 
 @pytest.mark.asyncio
+async def test_create_backup_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = BackupForGKEAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.create_backup
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.create_backup
+        ] = mock_object
+
+        request = {}
+        await client.create_backup(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        # Operation methods build a cached wrapper on first rpc call
+        # subsequent calls should use the cached wrapper
+        wrapper_fn.reset_mock()
+
+        await client.create_backup(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_create_backup_async(
     transport: str = "grpc_asyncio", request_type=gkebackup.CreateBackupRequest
 ):
     client = BackupForGKEAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
@@ -3208,14 +3776,17 @@
     client = BackupForGKEClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.list_backups), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.list_backups()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.ListBackupsRequest()
 
 
 def test_list_backups_non_empty_request_with_auto_populated_field():
@@ -3234,25 +3805,63 @@
         page_token="page_token_value",
         filter="filter_value",
         order_by="order_by_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.list_backups), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.list_backups(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.ListBackupsRequest(
             parent="parent_value",
             page_token="page_token_value",
             filter="filter_value",
             order_by="order_by_value",
         )
 
 
+def test_list_backups_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = BackupForGKEClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.list_backups in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.list_backups] = mock_rpc
+        request = {}
+        client.list_backups(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.list_backups(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_list_backups_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = BackupForGKEAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -3269,14 +3878,60 @@
         response = await client.list_backups()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.ListBackupsRequest()
 
 
 @pytest.mark.asyncio
+async def test_list_backups_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = BackupForGKEAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.list_backups
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.list_backups
+        ] = mock_object
+
+        request = {}
+        await client.list_backups(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.list_backups(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_list_backups_async(
     transport: str = "grpc_asyncio", request_type=gkebackup.ListBackupsRequest
 ):
     client = BackupForGKEAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
@@ -3677,14 +4332,15 @@
             resource_count=1520,
             volume_count=1312,
             size_bytes=1089,
             etag="etag_value",
             description="description_value",
             pod_count=971,
             config_backup_size_bytes=2539,
+            permissive_mode=True,
             all_namespaces=True,
         )
         response = client.get_backup(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
@@ -3705,26 +4361,30 @@
     assert response.resource_count == 1520
     assert response.volume_count == 1312
     assert response.size_bytes == 1089
     assert response.etag == "etag_value"
     assert response.description == "description_value"
     assert response.pod_count == 971
     assert response.config_backup_size_bytes == 2539
+    assert response.permissive_mode is True
 
 
 def test_get_backup_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = BackupForGKEClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_backup), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.get_backup()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.GetBackupRequest()
 
 
 def test_get_backup_non_empty_request_with_auto_populated_field():
@@ -3740,22 +4400,60 @@
     # if they meet the requirements of AIP 4235.
     request = gkebackup.GetBackupRequest(
         name="name_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_backup), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.get_backup(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.GetBackupRequest(
             name="name_value",
         )
 
 
+def test_get_backup_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = BackupForGKEClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.get_backup in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.get_backup] = mock_rpc
+        request = {}
+        client.get_backup(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.get_backup(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_get_backup_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = BackupForGKEAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -3778,23 +4476,68 @@
                 resource_count=1520,
                 volume_count=1312,
                 size_bytes=1089,
                 etag="etag_value",
                 description="description_value",
                 pod_count=971,
                 config_backup_size_bytes=2539,
+                permissive_mode=True,
             )
         )
         response = await client.get_backup()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.GetBackupRequest()
 
 
 @pytest.mark.asyncio
+async def test_get_backup_async_use_cached_wrapped_rpc(transport: str = "grpc_asyncio"):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = BackupForGKEAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.get_backup
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.get_backup
+        ] = mock_object
+
+        request = {}
+        await client.get_backup(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.get_backup(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_get_backup_async(
     transport: str = "grpc_asyncio", request_type=gkebackup.GetBackupRequest
 ):
     client = BackupForGKEAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
@@ -3820,14 +4563,15 @@
                 resource_count=1520,
                 volume_count=1312,
                 size_bytes=1089,
                 etag="etag_value",
                 description="description_value",
                 pod_count=971,
                 config_backup_size_bytes=2539,
+                permissive_mode=True,
             )
         )
         response = await client.get_backup(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
@@ -3848,14 +4592,15 @@
     assert response.resource_count == 1520
     assert response.volume_count == 1312
     assert response.size_bytes == 1089
     assert response.etag == "etag_value"
     assert response.description == "description_value"
     assert response.pod_count == 971
     assert response.config_backup_size_bytes == 2539
+    assert response.permissive_mode is True
 
 
 @pytest.mark.asyncio
 async def test_get_backup_async_from_dict():
     await test_get_backup_async(request_type=dict)
 
 
@@ -4037,14 +4782,17 @@
     client = BackupForGKEClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.update_backup), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.update_backup()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.UpdateBackupRequest()
 
 
 def test_update_backup_non_empty_request_with_auto_populated_field():
@@ -4058,20 +4806,62 @@
     # Populate all string fields in the request which are not UUID4
     # since we want to check that UUID4 are populated automatically
     # if they meet the requirements of AIP 4235.
     request = gkebackup.UpdateBackupRequest()
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.update_backup), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.update_backup(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.UpdateBackupRequest()
 
 
+def test_update_backup_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = BackupForGKEClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.update_backup in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.update_backup] = mock_rpc
+        request = {}
+        client.update_backup(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        # Operation methods build a cached wrapper on first rpc call
+        # subsequent calls should use the cached wrapper
+        wrapper_fn.reset_mock()
+
+        client.update_backup(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_update_backup_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = BackupForGKEAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -4086,14 +4876,64 @@
         response = await client.update_backup()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.UpdateBackupRequest()
 
 
 @pytest.mark.asyncio
+async def test_update_backup_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = BackupForGKEAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.update_backup
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.update_backup
+        ] = mock_object
+
+        request = {}
+        await client.update_backup(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        # Operation methods build a cached wrapper on first rpc call
+        # subsequent calls should use the cached wrapper
+        wrapper_fn.reset_mock()
+
+        await client.update_backup(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_update_backup_async(
     transport: str = "grpc_asyncio", request_type=gkebackup.UpdateBackupRequest
 ):
     client = BackupForGKEAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
@@ -4317,14 +5157,17 @@
     client = BackupForGKEClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.delete_backup), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.delete_backup()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.DeleteBackupRequest()
 
 
 def test_delete_backup_non_empty_request_with_auto_populated_field():
@@ -4341,23 +5184,65 @@
     request = gkebackup.DeleteBackupRequest(
         name="name_value",
         etag="etag_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.delete_backup), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.delete_backup(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.DeleteBackupRequest(
             name="name_value",
             etag="etag_value",
         )
 
 
+def test_delete_backup_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = BackupForGKEClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.delete_backup in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.delete_backup] = mock_rpc
+        request = {}
+        client.delete_backup(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        # Operation methods build a cached wrapper on first rpc call
+        # subsequent calls should use the cached wrapper
+        wrapper_fn.reset_mock()
+
+        client.delete_backup(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_delete_backup_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = BackupForGKEAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -4372,14 +5257,64 @@
         response = await client.delete_backup()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.DeleteBackupRequest()
 
 
 @pytest.mark.asyncio
+async def test_delete_backup_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = BackupForGKEAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.delete_backup
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.delete_backup
+        ] = mock_object
+
+        request = {}
+        await client.delete_backup(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        # Operation methods build a cached wrapper on first rpc call
+        # subsequent calls should use the cached wrapper
+        wrapper_fn.reset_mock()
+
+        await client.delete_backup(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_delete_backup_async(
     transport: str = "grpc_asyncio", request_type=gkebackup.DeleteBackupRequest
 ):
     client = BackupForGKEAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
@@ -4600,14 +5535,17 @@
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_volume_backups), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.list_volume_backups()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.ListVolumeBackupsRequest()
 
 
 def test_list_volume_backups_non_empty_request_with_auto_populated_field():
@@ -4628,25 +5566,67 @@
         order_by="order_by_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_volume_backups), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.list_volume_backups(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.ListVolumeBackupsRequest(
             parent="parent_value",
             page_token="page_token_value",
             filter="filter_value",
             order_by="order_by_value",
         )
 
 
+def test_list_volume_backups_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = BackupForGKEClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.list_volume_backups in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.list_volume_backups
+        ] = mock_rpc
+        request = {}
+        client.list_volume_backups(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.list_volume_backups(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_list_volume_backups_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = BackupForGKEAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -4665,14 +5645,60 @@
         response = await client.list_volume_backups()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.ListVolumeBackupsRequest()
 
 
 @pytest.mark.asyncio
+async def test_list_volume_backups_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = BackupForGKEAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.list_volume_backups
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.list_volume_backups
+        ] = mock_object
+
+        request = {}
+        await client.list_volume_backups(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.list_volume_backups(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_list_volume_backups_async(
     transport: str = "grpc_asyncio", request_type=gkebackup.ListVolumeBackupsRequest
 ):
     client = BackupForGKEAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
@@ -5122,14 +6148,17 @@
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.get_volume_backup), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.get_volume_backup()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.GetVolumeBackupRequest()
 
 
 def test_get_volume_backup_non_empty_request_with_auto_populated_field():
@@ -5147,22 +6176,62 @@
         name="name_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.get_volume_backup), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.get_volume_backup(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.GetVolumeBackupRequest(
             name="name_value",
         )
 
 
+def test_get_volume_backup_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = BackupForGKEClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.get_volume_backup in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.get_volume_backup
+        ] = mock_rpc
+        request = {}
+        client.get_volume_backup(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.get_volume_backup(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_get_volume_backup_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = BackupForGKEAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -5189,14 +6258,60 @@
         response = await client.get_volume_backup()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.GetVolumeBackupRequest()
 
 
 @pytest.mark.asyncio
+async def test_get_volume_backup_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = BackupForGKEAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.get_volume_backup
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.get_volume_backup
+        ] = mock_object
+
+        request = {}
+        await client.get_volume_backup(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.get_volume_backup(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_get_volume_backup_async(
     transport: str = "grpc_asyncio", request_type=gkebackup.GetVolumeBackupRequest
 ):
     client = BackupForGKEAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
@@ -5441,14 +6556,17 @@
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.create_restore_plan), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.create_restore_plan()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.CreateRestorePlanRequest()
 
 
 def test_create_restore_plan_non_empty_request_with_auto_populated_field():
@@ -5467,23 +6585,69 @@
         restore_plan_id="restore_plan_id_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.create_restore_plan), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.create_restore_plan(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.CreateRestorePlanRequest(
             parent="parent_value",
             restore_plan_id="restore_plan_id_value",
         )
 
 
+def test_create_restore_plan_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = BackupForGKEClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.create_restore_plan in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.create_restore_plan
+        ] = mock_rpc
+        request = {}
+        client.create_restore_plan(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        # Operation methods build a cached wrapper on first rpc call
+        # subsequent calls should use the cached wrapper
+        wrapper_fn.reset_mock()
+
+        client.create_restore_plan(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_create_restore_plan_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = BackupForGKEAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -5500,14 +6664,64 @@
         response = await client.create_restore_plan()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.CreateRestorePlanRequest()
 
 
 @pytest.mark.asyncio
+async def test_create_restore_plan_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = BackupForGKEAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.create_restore_plan
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.create_restore_plan
+        ] = mock_object
+
+        request = {}
+        await client.create_restore_plan(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        # Operation methods build a cached wrapper on first rpc call
+        # subsequent calls should use the cached wrapper
+        wrapper_fn.reset_mock()
+
+        await client.create_restore_plan(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_create_restore_plan_async(
     transport: str = "grpc_asyncio", request_type=gkebackup.CreateRestorePlanRequest
 ):
     client = BackupForGKEAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
@@ -5760,14 +6974,17 @@
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_restore_plans), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.list_restore_plans()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.ListRestorePlansRequest()
 
 
 def test_list_restore_plans_non_empty_request_with_auto_populated_field():
@@ -5788,25 +7005,67 @@
         order_by="order_by_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_restore_plans), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.list_restore_plans(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.ListRestorePlansRequest(
             parent="parent_value",
             page_token="page_token_value",
             filter="filter_value",
             order_by="order_by_value",
         )
 
 
+def test_list_restore_plans_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = BackupForGKEClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.list_restore_plans in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.list_restore_plans
+        ] = mock_rpc
+        request = {}
+        client.list_restore_plans(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.list_restore_plans(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_list_restore_plans_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = BackupForGKEAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -5826,14 +7085,60 @@
         response = await client.list_restore_plans()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.ListRestorePlansRequest()
 
 
 @pytest.mark.asyncio
+async def test_list_restore_plans_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = BackupForGKEAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.list_restore_plans
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.list_restore_plans
+        ] = mock_object
+
+        request = {}
+        await client.list_restore_plans(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.list_restore_plans(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_list_restore_plans_async(
     transport: str = "grpc_asyncio", request_type=gkebackup.ListRestorePlansRequest
 ):
     client = BackupForGKEAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
@@ -6277,14 +7582,17 @@
     client = BackupForGKEClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_restore_plan), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.get_restore_plan()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.GetRestorePlanRequest()
 
 
 def test_get_restore_plan_non_empty_request_with_auto_populated_field():
@@ -6300,22 +7608,62 @@
     # if they meet the requirements of AIP 4235.
     request = gkebackup.GetRestorePlanRequest(
         name="name_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_restore_plan), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.get_restore_plan(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.GetRestorePlanRequest(
             name="name_value",
         )
 
 
+def test_get_restore_plan_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = BackupForGKEClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.get_restore_plan in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.get_restore_plan
+        ] = mock_rpc
+        request = {}
+        client.get_restore_plan(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.get_restore_plan(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_get_restore_plan_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = BackupForGKEAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -6339,14 +7687,60 @@
         response = await client.get_restore_plan()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.GetRestorePlanRequest()
 
 
 @pytest.mark.asyncio
+async def test_get_restore_plan_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = BackupForGKEAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.get_restore_plan
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.get_restore_plan
+        ] = mock_object
+
+        request = {}
+        await client.get_restore_plan(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.get_restore_plan(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_get_restore_plan_async(
     transport: str = "grpc_asyncio", request_type=gkebackup.GetRestorePlanRequest
 ):
     client = BackupForGKEAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
@@ -6581,14 +7975,17 @@
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.update_restore_plan), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.update_restore_plan()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.UpdateRestorePlanRequest()
 
 
 def test_update_restore_plan_non_empty_request_with_auto_populated_field():
@@ -6604,20 +8001,66 @@
     # if they meet the requirements of AIP 4235.
     request = gkebackup.UpdateRestorePlanRequest()
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.update_restore_plan), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.update_restore_plan(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.UpdateRestorePlanRequest()
 
 
+def test_update_restore_plan_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = BackupForGKEClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.update_restore_plan in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.update_restore_plan
+        ] = mock_rpc
+        request = {}
+        client.update_restore_plan(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        # Operation methods build a cached wrapper on first rpc call
+        # subsequent calls should use the cached wrapper
+        wrapper_fn.reset_mock()
+
+        client.update_restore_plan(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_update_restore_plan_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = BackupForGKEAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -6634,14 +8077,64 @@
         response = await client.update_restore_plan()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.UpdateRestorePlanRequest()
 
 
 @pytest.mark.asyncio
+async def test_update_restore_plan_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = BackupForGKEAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.update_restore_plan
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.update_restore_plan
+        ] = mock_object
+
+        request = {}
+        await client.update_restore_plan(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        # Operation methods build a cached wrapper on first rpc call
+        # subsequent calls should use the cached wrapper
+        wrapper_fn.reset_mock()
+
+        await client.update_restore_plan(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_update_restore_plan_async(
     transport: str = "grpc_asyncio", request_type=gkebackup.UpdateRestorePlanRequest
 ):
     client = BackupForGKEAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
@@ -6879,14 +8372,17 @@
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.delete_restore_plan), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.delete_restore_plan()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.DeleteRestorePlanRequest()
 
 
 def test_delete_restore_plan_non_empty_request_with_auto_populated_field():
@@ -6905,23 +8401,69 @@
         etag="etag_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.delete_restore_plan), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.delete_restore_plan(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.DeleteRestorePlanRequest(
             name="name_value",
             etag="etag_value",
         )
 
 
+def test_delete_restore_plan_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = BackupForGKEClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.delete_restore_plan in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.delete_restore_plan
+        ] = mock_rpc
+        request = {}
+        client.delete_restore_plan(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        # Operation methods build a cached wrapper on first rpc call
+        # subsequent calls should use the cached wrapper
+        wrapper_fn.reset_mock()
+
+        client.delete_restore_plan(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_delete_restore_plan_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = BackupForGKEAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -6938,14 +8480,64 @@
         response = await client.delete_restore_plan()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.DeleteRestorePlanRequest()
 
 
 @pytest.mark.asyncio
+async def test_delete_restore_plan_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = BackupForGKEAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.delete_restore_plan
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.delete_restore_plan
+        ] = mock_object
+
+        request = {}
+        await client.delete_restore_plan(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        # Operation methods build a cached wrapper on first rpc call
+        # subsequent calls should use the cached wrapper
+        wrapper_fn.reset_mock()
+
+        await client.delete_restore_plan(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_delete_restore_plan_async(
     transport: str = "grpc_asyncio", request_type=gkebackup.DeleteRestorePlanRequest
 ):
     client = BackupForGKEAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
@@ -7169,14 +8761,17 @@
     client = BackupForGKEClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.create_restore), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.create_restore()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.CreateRestoreRequest()
 
 
 def test_create_restore_non_empty_request_with_auto_populated_field():
@@ -7193,23 +8788,65 @@
     request = gkebackup.CreateRestoreRequest(
         parent="parent_value",
         restore_id="restore_id_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.create_restore), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.create_restore(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.CreateRestoreRequest(
             parent="parent_value",
             restore_id="restore_id_value",
         )
 
 
+def test_create_restore_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = BackupForGKEClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.create_restore in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.create_restore] = mock_rpc
+        request = {}
+        client.create_restore(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        # Operation methods build a cached wrapper on first rpc call
+        # subsequent calls should use the cached wrapper
+        wrapper_fn.reset_mock()
+
+        client.create_restore(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_create_restore_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = BackupForGKEAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -7224,14 +8861,64 @@
         response = await client.create_restore()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.CreateRestoreRequest()
 
 
 @pytest.mark.asyncio
+async def test_create_restore_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = BackupForGKEAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.create_restore
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.create_restore
+        ] = mock_object
+
+        request = {}
+        await client.create_restore(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        # Operation methods build a cached wrapper on first rpc call
+        # subsequent calls should use the cached wrapper
+        wrapper_fn.reset_mock()
+
+        await client.create_restore(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_create_restore_async(
     transport: str = "grpc_asyncio", request_type=gkebackup.CreateRestoreRequest
 ):
     client = BackupForGKEAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
@@ -7470,14 +9157,17 @@
     client = BackupForGKEClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.list_restores), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.list_restores()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.ListRestoresRequest()
 
 
 def test_list_restores_non_empty_request_with_auto_populated_field():
@@ -7496,25 +9186,63 @@
         page_token="page_token_value",
         filter="filter_value",
         order_by="order_by_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.list_restores), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.list_restores(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.ListRestoresRequest(
             parent="parent_value",
             page_token="page_token_value",
             filter="filter_value",
             order_by="order_by_value",
         )
 
 
+def test_list_restores_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = BackupForGKEClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.list_restores in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.list_restores] = mock_rpc
+        request = {}
+        client.list_restores(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.list_restores(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_list_restores_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = BackupForGKEAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -7532,14 +9260,60 @@
         response = await client.list_restores()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.ListRestoresRequest()
 
 
 @pytest.mark.asyncio
+async def test_list_restores_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = BackupForGKEAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.list_restores
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.list_restores
+        ] = mock_object
+
+        request = {}
+        await client.list_restores(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.list_restores(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_list_restores_async(
     transport: str = "grpc_asyncio", request_type=gkebackup.ListRestoresRequest
 ):
     client = BackupForGKEAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
@@ -7973,14 +9747,17 @@
     client = BackupForGKEClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_restore), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.get_restore()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.GetRestoreRequest()
 
 
 def test_get_restore_non_empty_request_with_auto_populated_field():
@@ -7996,22 +9773,60 @@
     # if they meet the requirements of AIP 4235.
     request = gkebackup.GetRestoreRequest(
         name="name_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_restore), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.get_restore(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.GetRestoreRequest(
             name="name_value",
         )
 
 
+def test_get_restore_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = BackupForGKEClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.get_restore in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.get_restore] = mock_rpc
+        request = {}
+        client.get_restore(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.get_restore(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_get_restore_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = BackupForGKEAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -8039,14 +9854,60 @@
         response = await client.get_restore()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.GetRestoreRequest()
 
 
 @pytest.mark.asyncio
+async def test_get_restore_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = BackupForGKEAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.get_restore
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.get_restore
+        ] = mock_object
+
+        request = {}
+        await client.get_restore(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.get_restore(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_get_restore_async(
     transport: str = "grpc_asyncio", request_type=gkebackup.GetRestoreRequest
 ):
     client = BackupForGKEAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
@@ -8281,14 +10142,17 @@
     client = BackupForGKEClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.update_restore), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.update_restore()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.UpdateRestoreRequest()
 
 
 def test_update_restore_non_empty_request_with_auto_populated_field():
@@ -8302,20 +10166,62 @@
     # Populate all string fields in the request which are not UUID4
     # since we want to check that UUID4 are populated automatically
     # if they meet the requirements of AIP 4235.
     request = gkebackup.UpdateRestoreRequest()
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.update_restore), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.update_restore(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.UpdateRestoreRequest()
 
 
+def test_update_restore_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = BackupForGKEClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.update_restore in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.update_restore] = mock_rpc
+        request = {}
+        client.update_restore(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        # Operation methods build a cached wrapper on first rpc call
+        # subsequent calls should use the cached wrapper
+        wrapper_fn.reset_mock()
+
+        client.update_restore(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_update_restore_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = BackupForGKEAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -8330,14 +10236,64 @@
         response = await client.update_restore()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.UpdateRestoreRequest()
 
 
 @pytest.mark.asyncio
+async def test_update_restore_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = BackupForGKEAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.update_restore
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.update_restore
+        ] = mock_object
+
+        request = {}
+        await client.update_restore(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        # Operation methods build a cached wrapper on first rpc call
+        # subsequent calls should use the cached wrapper
+        wrapper_fn.reset_mock()
+
+        await client.update_restore(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_update_restore_async(
     transport: str = "grpc_asyncio", request_type=gkebackup.UpdateRestoreRequest
 ):
     client = BackupForGKEAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
@@ -8561,14 +10517,17 @@
     client = BackupForGKEClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.delete_restore), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.delete_restore()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.DeleteRestoreRequest()
 
 
 def test_delete_restore_non_empty_request_with_auto_populated_field():
@@ -8585,23 +10544,65 @@
     request = gkebackup.DeleteRestoreRequest(
         name="name_value",
         etag="etag_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.delete_restore), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.delete_restore(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.DeleteRestoreRequest(
             name="name_value",
             etag="etag_value",
         )
 
 
+def test_delete_restore_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = BackupForGKEClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.delete_restore in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.delete_restore] = mock_rpc
+        request = {}
+        client.delete_restore(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        # Operation methods build a cached wrapper on first rpc call
+        # subsequent calls should use the cached wrapper
+        wrapper_fn.reset_mock()
+
+        client.delete_restore(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_delete_restore_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = BackupForGKEAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -8616,14 +10617,64 @@
         response = await client.delete_restore()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.DeleteRestoreRequest()
 
 
 @pytest.mark.asyncio
+async def test_delete_restore_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = BackupForGKEAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.delete_restore
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.delete_restore
+        ] = mock_object
+
+        request = {}
+        await client.delete_restore(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        # Operation methods build a cached wrapper on first rpc call
+        # subsequent calls should use the cached wrapper
+        wrapper_fn.reset_mock()
+
+        await client.delete_restore(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_delete_restore_async(
     transport: str = "grpc_asyncio", request_type=gkebackup.DeleteRestoreRequest
 ):
     client = BackupForGKEAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
@@ -8844,14 +10895,17 @@
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_volume_restores), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.list_volume_restores()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.ListVolumeRestoresRequest()
 
 
 def test_list_volume_restores_non_empty_request_with_auto_populated_field():
@@ -8872,25 +10926,67 @@
         order_by="order_by_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_volume_restores), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.list_volume_restores(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.ListVolumeRestoresRequest(
             parent="parent_value",
             page_token="page_token_value",
             filter="filter_value",
             order_by="order_by_value",
         )
 
 
+def test_list_volume_restores_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = BackupForGKEClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.list_volume_restores in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.list_volume_restores
+        ] = mock_rpc
+        request = {}
+        client.list_volume_restores(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.list_volume_restores(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_list_volume_restores_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = BackupForGKEAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -8909,14 +11005,60 @@
         response = await client.list_volume_restores()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.ListVolumeRestoresRequest()
 
 
 @pytest.mark.asyncio
+async def test_list_volume_restores_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = BackupForGKEAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.list_volume_restores
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.list_volume_restores
+        ] = mock_object
+
+        request = {}
+        await client.list_volume_restores(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.list_volume_restores(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_list_volume_restores_async(
     transport: str = "grpc_asyncio", request_type=gkebackup.ListVolumeRestoresRequest
 ):
     client = BackupForGKEAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
@@ -9362,14 +11504,17 @@
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.get_volume_restore), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.get_volume_restore()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.GetVolumeRestoreRequest()
 
 
 def test_get_volume_restore_non_empty_request_with_auto_populated_field():
@@ -9387,22 +11532,64 @@
         name="name_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.get_volume_restore), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.get_volume_restore(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.GetVolumeRestoreRequest(
             name="name_value",
         )
 
 
+def test_get_volume_restore_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = BackupForGKEClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.get_volume_restore in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.get_volume_restore
+        ] = mock_rpc
+        request = {}
+        client.get_volume_restore(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.get_volume_restore(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_get_volume_restore_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = BackupForGKEAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -9428,14 +11615,60 @@
         response = await client.get_volume_restore()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.GetVolumeRestoreRequest()
 
 
 @pytest.mark.asyncio
+async def test_get_volume_restore_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = BackupForGKEAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.get_volume_restore
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.get_volume_restore
+        ] = mock_object
+
+        request = {}
+        await client.get_volume_restore(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.get_volume_restore(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_get_volume_restore_async(
     transport: str = "grpc_asyncio", request_type=gkebackup.GetVolumeRestoreRequest
 ):
     client = BackupForGKEAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
@@ -9683,14 +11916,17 @@
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.get_backup_index_download_url), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.get_backup_index_download_url()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.GetBackupIndexDownloadUrlRequest()
 
 
 def test_get_backup_index_download_url_non_empty_request_with_auto_populated_field():
@@ -9708,22 +11944,65 @@
         backup="backup_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.get_backup_index_download_url), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.get_backup_index_download_url(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.GetBackupIndexDownloadUrlRequest(
             backup="backup_value",
         )
 
 
+def test_get_backup_index_download_url_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = BackupForGKEClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.get_backup_index_download_url
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.get_backup_index_download_url
+        ] = mock_rpc
+        request = {}
+        client.get_backup_index_download_url(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.get_backup_index_download_url(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_get_backup_index_download_url_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = BackupForGKEAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -9742,14 +12021,60 @@
         response = await client.get_backup_index_download_url()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == gkebackup.GetBackupIndexDownloadUrlRequest()
 
 
 @pytest.mark.asyncio
+async def test_get_backup_index_download_url_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = BackupForGKEAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.get_backup_index_download_url
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.get_backup_index_download_url
+        ] = mock_object
+
+        request = {}
+        await client.get_backup_index_download_url(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.get_backup_index_download_url(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_get_backup_index_download_url_async(
     transport: str = "grpc_asyncio",
     request_type=gkebackup.GetBackupIndexDownloadUrlRequest,
 ):
     client = BackupForGKEAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -10005,14 +12330,15 @@
                 ]
             },
             "include_volume_data": True,
             "include_secrets": True,
             "encryption_key": {
                 "gcp_kms_encryption_key": "gcp_kms_encryption_key_value"
             },
+            "permissive_mode": True,
         },
         "protected_pod_count": 2036,
         "state": 1,
         "state_reason": "state_reason_value",
         "rpo_risk_level": 1504,
         "rpo_risk_reason": "rpo_risk_reason_value",
     }
@@ -10099,14 +12425,58 @@
         req.return_value = response_value
         response = client.create_backup_plan(request)
 
     # Establish that the response is the type that we expect.
     assert response.operation.name == "operations/spam"
 
 
+def test_create_backup_plan_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = BackupForGKEClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.create_backup_plan in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.create_backup_plan
+        ] = mock_rpc
+
+        request = {}
+        client.create_backup_plan(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        # Operation methods build a cached wrapper on first rpc call
+        # subsequent calls should use the cached wrapper
+        wrapper_fn.reset_mock()
+
+        client.create_backup_plan(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_create_backup_plan_rest_required_fields(
     request_type=gkebackup.CreateBackupPlanRequest,
 ):
     transport_class = transports.BackupForGKERestTransport
 
     request_init = {}
     request_init["parent"] = ""
@@ -10394,14 +12764,52 @@
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.ListBackupPlansPager)
     assert response.next_page_token == "next_page_token_value"
     assert response.unreachable == ["unreachable_value"]
 
 
+def test_list_backup_plans_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = BackupForGKEClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.list_backup_plans in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.list_backup_plans
+        ] = mock_rpc
+
+        request = {}
+        client.list_backup_plans(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.list_backup_plans(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_list_backup_plans_rest_required_fields(
     request_type=gkebackup.ListBackupPlansRequest,
 ):
     transport_class = transports.BackupForGKERestTransport
 
     request_init = {}
     request_init["parent"] = ""
@@ -10755,14 +13163,50 @@
     assert response.protected_pod_count == 2036
     assert response.state == backup_plan.BackupPlan.State.CLUSTER_PENDING
     assert response.state_reason == "state_reason_value"
     assert response.rpo_risk_level == 1504
     assert response.rpo_risk_reason == "rpo_risk_reason_value"
 
 
+def test_get_backup_plan_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = BackupForGKEClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.get_backup_plan in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.get_backup_plan] = mock_rpc
+
+        request = {}
+        client.get_backup_plan(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.get_backup_plan(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_get_backup_plan_rest_required_fields(
     request_type=gkebackup.GetBackupPlanRequest,
 ):
     transport_class = transports.BackupForGKERestTransport
 
     request_init = {}
     request_init["name"] = ""
@@ -11057,14 +13501,15 @@
                 ]
             },
             "include_volume_data": True,
             "include_secrets": True,
             "encryption_key": {
                 "gcp_kms_encryption_key": "gcp_kms_encryption_key_value"
             },
+            "permissive_mode": True,
         },
         "protected_pod_count": 2036,
         "state": 1,
         "state_reason": "state_reason_value",
         "rpo_risk_level": 1504,
         "rpo_risk_reason": "rpo_risk_reason_value",
     }
@@ -11151,14 +13596,58 @@
         req.return_value = response_value
         response = client.update_backup_plan(request)
 
     # Establish that the response is the type that we expect.
     assert response.operation.name == "operations/spam"
 
 
+def test_update_backup_plan_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = BackupForGKEClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.update_backup_plan in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.update_backup_plan
+        ] = mock_rpc
+
+        request = {}
+        client.update_backup_plan(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        # Operation methods build a cached wrapper on first rpc call
+        # subsequent calls should use the cached wrapper
+        wrapper_fn.reset_mock()
+
+        client.update_backup_plan(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_update_backup_plan_rest_required_fields(
     request_type=gkebackup.UpdateBackupPlanRequest,
 ):
     transport_class = transports.BackupForGKERestTransport
 
     request_init = {}
     request = request_type(**request_init)
@@ -11418,14 +13907,58 @@
         req.return_value = response_value
         response = client.delete_backup_plan(request)
 
     # Establish that the response is the type that we expect.
     assert response.operation.name == "operations/spam"
 
 
+def test_delete_backup_plan_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = BackupForGKEClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.delete_backup_plan in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.delete_backup_plan
+        ] = mock_rpc
+
+        request = {}
+        client.delete_backup_plan(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        # Operation methods build a cached wrapper on first rpc call
+        # subsequent calls should use the cached wrapper
+        wrapper_fn.reset_mock()
+
+        client.delete_backup_plan(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_delete_backup_plan_rest_required_fields(
     request_type=gkebackup.DeleteBackupPlanRequest,
 ):
     transport_class = transports.BackupForGKERestTransport
 
     request_init = {}
     request_init["name"] = ""
@@ -11699,14 +14232,15 @@
         "resource_count": 1520,
         "volume_count": 1312,
         "size_bytes": 1089,
         "etag": "etag_value",
         "description": "description_value",
         "pod_count": 971,
         "config_backup_size_bytes": 2539,
+        "permissive_mode": True,
     }
     # The version of a generated dependency at test runtime may differ from the version used during generation.
     # Delete any fields which are not present in the current runtime dependency
     # See https://github.com/googleapis/gapic-generator-python/issues/1748
 
     # Determine if the message type is proto-plus or protobuf
     test_field = gkebackup.CreateBackupRequest.meta.fields["backup"]
@@ -11787,14 +14321,54 @@
         req.return_value = response_value
         response = client.create_backup(request)
 
     # Establish that the response is the type that we expect.
     assert response.operation.name == "operations/spam"
 
 
+def test_create_backup_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = BackupForGKEClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.create_backup in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.create_backup] = mock_rpc
+
+        request = {}
+        client.create_backup(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        # Operation methods build a cached wrapper on first rpc call
+        # subsequent calls should use the cached wrapper
+        wrapper_fn.reset_mock()
+
+        client.create_backup(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_create_backup_rest_required_fields(request_type=gkebackup.CreateBackupRequest):
     transport_class = transports.BackupForGKERestTransport
 
     request_init = {}
     request_init["parent"] = ""
     request = request_type(**request_init)
     pb_request = request_type.pb(request)
@@ -12056,14 +14630,50 @@
         response = client.list_backups(request)
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.ListBackupsPager)
     assert response.next_page_token == "next_page_token_value"
 
 
+def test_list_backups_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = BackupForGKEClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.list_backups in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.list_backups] = mock_rpc
+
+        request = {}
+        client.list_backups(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.list_backups(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_list_backups_rest_required_fields(request_type=gkebackup.ListBackupsRequest):
     transport_class = transports.BackupForGKERestTransport
 
     request_init = {}
     request_init["parent"] = ""
     request = request_type(**request_init)
     pb_request = request_type.pb(request)
@@ -12396,14 +15006,15 @@
             resource_count=1520,
             volume_count=1312,
             size_bytes=1089,
             etag="etag_value",
             description="description_value",
             pod_count=971,
             config_backup_size_bytes=2539,
+            permissive_mode=True,
             all_namespaces=True,
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         # Convert return value to protobuf type
@@ -12428,14 +15039,51 @@
     assert response.resource_count == 1520
     assert response.volume_count == 1312
     assert response.size_bytes == 1089
     assert response.etag == "etag_value"
     assert response.description == "description_value"
     assert response.pod_count == 971
     assert response.config_backup_size_bytes == 2539
+    assert response.permissive_mode is True
+
+
+def test_get_backup_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = BackupForGKEClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.get_backup in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.get_backup] = mock_rpc
+
+        request = {}
+        client.get_backup(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.get_backup(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
 
 
 def test_get_backup_rest_required_fields(request_type=gkebackup.GetBackupRequest):
     transport_class = transports.BackupForGKERestTransport
 
     request_init = {}
     request_init["name"] = ""
@@ -12712,14 +15360,15 @@
         "resource_count": 1520,
         "volume_count": 1312,
         "size_bytes": 1089,
         "etag": "etag_value",
         "description": "description_value",
         "pod_count": 971,
         "config_backup_size_bytes": 2539,
+        "permissive_mode": True,
     }
     # The version of a generated dependency at test runtime may differ from the version used during generation.
     # Delete any fields which are not present in the current runtime dependency
     # See https://github.com/googleapis/gapic-generator-python/issues/1748
 
     # Determine if the message type is proto-plus or protobuf
     test_field = gkebackup.UpdateBackupRequest.meta.fields["backup"]
@@ -12800,14 +15449,54 @@
         req.return_value = response_value
         response = client.update_backup(request)
 
     # Establish that the response is the type that we expect.
     assert response.operation.name == "operations/spam"
 
 
+def test_update_backup_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = BackupForGKEClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.update_backup in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.update_backup] = mock_rpc
+
+        request = {}
+        client.update_backup(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        # Operation methods build a cached wrapper on first rpc call
+        # subsequent calls should use the cached wrapper
+        wrapper_fn.reset_mock()
+
+        client.update_backup(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_update_backup_rest_required_fields(request_type=gkebackup.UpdateBackupRequest):
     transport_class = transports.BackupForGKERestTransport
 
     request_init = {}
     request = request_type(**request_init)
     pb_request = request_type.pb(request)
     jsonified_request = json.loads(
@@ -13065,14 +15754,54 @@
         req.return_value = response_value
         response = client.delete_backup(request)
 
     # Establish that the response is the type that we expect.
     assert response.operation.name == "operations/spam"
 
 
+def test_delete_backup_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = BackupForGKEClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.delete_backup in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.delete_backup] = mock_rpc
+
+        request = {}
+        client.delete_backup(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        # Operation methods build a cached wrapper on first rpc call
+        # subsequent calls should use the cached wrapper
+        wrapper_fn.reset_mock()
+
+        client.delete_backup(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_delete_backup_rest_required_fields(request_type=gkebackup.DeleteBackupRequest):
     transport_class = transports.BackupForGKERestTransport
 
     request_init = {}
     request_init["name"] = ""
     request = request_type(**request_init)
     pb_request = request_type.pb(request)
@@ -13346,14 +16075,54 @@
         response = client.list_volume_backups(request)
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.ListVolumeBackupsPager)
     assert response.next_page_token == "next_page_token_value"
 
 
+def test_list_volume_backups_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = BackupForGKEClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.list_volume_backups in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.list_volume_backups
+        ] = mock_rpc
+
+        request = {}
+        client.list_volume_backups(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.list_volume_backups(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_list_volume_backups_rest_required_fields(
     request_type=gkebackup.ListVolumeBackupsRequest,
 ):
     transport_class = transports.BackupForGKERestTransport
 
     request_init = {}
     request_init["parent"] = ""
@@ -13715,14 +16484,52 @@
     assert response.storage_bytes == 1403
     assert response.disk_size_bytes == 1611
     assert response.state == volume.VolumeBackup.State.CREATING
     assert response.state_message == "state_message_value"
     assert response.etag == "etag_value"
 
 
+def test_get_volume_backup_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = BackupForGKEClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.get_volume_backup in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.get_volume_backup
+        ] = mock_rpc
+
+        request = {}
+        client.get_volume_backup(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.get_volume_backup(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_get_volume_backup_rest_required_fields(
     request_type=gkebackup.GetVolumeBackupRequest,
 ):
     transport_class = transports.BackupForGKERestTransport
 
     request_init = {}
     request_init["name"] = ""
@@ -14023,14 +16830,18 @@
                         "namespaces": ["namespaces_value1", "namespaces_value2"],
                         "group_kinds": {},
                         "json_path": "json_path_value",
                     },
                     "description": "description_value",
                 }
             ],
+            "volume_data_restore_policy_bindings": [{"policy": 1, "volume_type": 1}],
+            "restore_order": {
+                "group_kind_dependencies": [{"satisfying": {}, "requiring": {}}]
+            },
         },
         "labels": {},
         "etag": "etag_value",
         "state": 1,
         "state_reason": "state_reason_value",
     }
     # The version of a generated dependency at test runtime may differ from the version used during generation.
@@ -14116,14 +16927,58 @@
         req.return_value = response_value
         response = client.create_restore_plan(request)
 
     # Establish that the response is the type that we expect.
     assert response.operation.name == "operations/spam"
 
 
+def test_create_restore_plan_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = BackupForGKEClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.create_restore_plan in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.create_restore_plan
+        ] = mock_rpc
+
+        request = {}
+        client.create_restore_plan(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        # Operation methods build a cached wrapper on first rpc call
+        # subsequent calls should use the cached wrapper
+        wrapper_fn.reset_mock()
+
+        client.create_restore_plan(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_create_restore_plan_rest_required_fields(
     request_type=gkebackup.CreateRestorePlanRequest,
 ):
     transport_class = transports.BackupForGKERestTransport
 
     request_init = {}
     request_init["parent"] = ""
@@ -14411,14 +17266,54 @@
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.ListRestorePlansPager)
     assert response.next_page_token == "next_page_token_value"
     assert response.unreachable == ["unreachable_value"]
 
 
+def test_list_restore_plans_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = BackupForGKEClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.list_restore_plans in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.list_restore_plans
+        ] = mock_rpc
+
+        request = {}
+        client.list_restore_plans(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.list_restore_plans(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_list_restore_plans_rest_required_fields(
     request_type=gkebackup.ListRestorePlansRequest,
 ):
     transport_class = transports.BackupForGKERestTransport
 
     request_init = {}
     request_init["parent"] = ""
@@ -14768,14 +17663,52 @@
     assert response.backup_plan == "backup_plan_value"
     assert response.cluster == "cluster_value"
     assert response.etag == "etag_value"
     assert response.state == restore_plan.RestorePlan.State.CLUSTER_PENDING
     assert response.state_reason == "state_reason_value"
 
 
+def test_get_restore_plan_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = BackupForGKEClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.get_restore_plan in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.get_restore_plan
+        ] = mock_rpc
+
+        request = {}
+        client.get_restore_plan(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.get_restore_plan(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_get_restore_plan_rest_required_fields(
     request_type=gkebackup.GetRestorePlanRequest,
 ):
     transport_class = transports.BackupForGKERestTransport
 
     request_init = {}
     request_init["name"] = ""
@@ -15080,14 +18013,18 @@
                         "namespaces": ["namespaces_value1", "namespaces_value2"],
                         "group_kinds": {},
                         "json_path": "json_path_value",
                     },
                     "description": "description_value",
                 }
             ],
+            "volume_data_restore_policy_bindings": [{"policy": 1, "volume_type": 1}],
+            "restore_order": {
+                "group_kind_dependencies": [{"satisfying": {}, "requiring": {}}]
+            },
         },
         "labels": {},
         "etag": "etag_value",
         "state": 1,
         "state_reason": "state_reason_value",
     }
     # The version of a generated dependency at test runtime may differ from the version used during generation.
@@ -15173,14 +18110,58 @@
         req.return_value = response_value
         response = client.update_restore_plan(request)
 
     # Establish that the response is the type that we expect.
     assert response.operation.name == "operations/spam"
 
 
+def test_update_restore_plan_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = BackupForGKEClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.update_restore_plan in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.update_restore_plan
+        ] = mock_rpc
+
+        request = {}
+        client.update_restore_plan(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        # Operation methods build a cached wrapper on first rpc call
+        # subsequent calls should use the cached wrapper
+        wrapper_fn.reset_mock()
+
+        client.update_restore_plan(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_update_restore_plan_rest_required_fields(
     request_type=gkebackup.UpdateRestorePlanRequest,
 ):
     transport_class = transports.BackupForGKERestTransport
 
     request_init = {}
     request = request_type(**request_init)
@@ -15440,14 +18421,58 @@
         req.return_value = response_value
         response = client.delete_restore_plan(request)
 
     # Establish that the response is the type that we expect.
     assert response.operation.name == "operations/spam"
 
 
+def test_delete_restore_plan_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = BackupForGKEClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.delete_restore_plan in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.delete_restore_plan
+        ] = mock_rpc
+
+        request = {}
+        client.delete_restore_plan(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        # Operation methods build a cached wrapper on first rpc call
+        # subsequent calls should use the cached wrapper
+        wrapper_fn.reset_mock()
+
+        client.delete_restore_plan(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_delete_restore_plan_rest_required_fields(
     request_type=gkebackup.DeleteRestorePlanRequest,
 ):
     transport_class = transports.BackupForGKERestTransport
 
     request_init = {}
     request_init["name"] = ""
@@ -15760,24 +18785,40 @@
                         "namespaces": ["namespaces_value1", "namespaces_value2"],
                         "group_kinds": {},
                         "json_path": "json_path_value",
                     },
                     "description": "description_value",
                 }
             ],
+            "volume_data_restore_policy_bindings": [{"policy": 1, "volume_type": 1}],
+            "restore_order": {
+                "group_kind_dependencies": [{"satisfying": {}, "requiring": {}}]
+            },
         },
         "labels": {},
         "state": 1,
         "state_reason": "state_reason_value",
         "complete_time": {},
         "resources_restored_count": 2602,
         "resources_excluded_count": 2576,
         "resources_failed_count": 2343,
         "volumes_restored_count": 2394,
         "etag": "etag_value",
+        "filter": {
+            "inclusion_filters": [
+                {
+                    "group_kind": {},
+                    "name": "name_value",
+                    "namespace": "namespace_value",
+                    "labels": {},
+                }
+            ],
+            "exclusion_filters": {},
+        },
+        "volume_data_restore_policy_overrides": [{"policy": 1, "selected_pvcs": {}}],
     }
     # The version of a generated dependency at test runtime may differ from the version used during generation.
     # Delete any fields which are not present in the current runtime dependency
     # See https://github.com/googleapis/gapic-generator-python/issues/1748
 
     # Determine if the message type is proto-plus or protobuf
     test_field = gkebackup.CreateRestoreRequest.meta.fields["restore"]
@@ -15858,14 +18899,54 @@
         req.return_value = response_value
         response = client.create_restore(request)
 
     # Establish that the response is the type that we expect.
     assert response.operation.name == "operations/spam"
 
 
+def test_create_restore_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = BackupForGKEClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.create_restore in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.create_restore] = mock_rpc
+
+        request = {}
+        client.create_restore(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        # Operation methods build a cached wrapper on first rpc call
+        # subsequent calls should use the cached wrapper
+        wrapper_fn.reset_mock()
+
+        client.create_restore(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_create_restore_rest_required_fields(
     request_type=gkebackup.CreateRestoreRequest,
 ):
     transport_class = transports.BackupForGKERestTransport
 
     request_init = {}
     request_init["parent"] = ""
@@ -16153,14 +19234,50 @@
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.ListRestoresPager)
     assert response.next_page_token == "next_page_token_value"
     assert response.unreachable == ["unreachable_value"]
 
 
+def test_list_restores_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = BackupForGKEClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.list_restores in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.list_restores] = mock_rpc
+
+        request = {}
+        client.list_restores(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.list_restores(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_list_restores_rest_required_fields(request_type=gkebackup.ListRestoresRequest):
     transport_class = transports.BackupForGKERestTransport
 
     request_init = {}
     request_init["parent"] = ""
     request = request_type(**request_init)
     pb_request = request_type.pb(request)
@@ -16518,14 +19635,50 @@
     assert response.resources_restored_count == 2602
     assert response.resources_excluded_count == 2576
     assert response.resources_failed_count == 2343
     assert response.volumes_restored_count == 2394
     assert response.etag == "etag_value"
 
 
+def test_get_restore_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = BackupForGKEClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.get_restore in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.get_restore] = mock_rpc
+
+        request = {}
+        client.get_restore(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.get_restore(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_get_restore_rest_required_fields(request_type=gkebackup.GetRestoreRequest):
     transport_class = transports.BackupForGKERestTransport
 
     request_init = {}
     request_init["name"] = ""
     request = request_type(**request_init)
     pb_request = request_type.pb(request)
@@ -16826,24 +19979,40 @@
                         "namespaces": ["namespaces_value1", "namespaces_value2"],
                         "group_kinds": {},
                         "json_path": "json_path_value",
                     },
                     "description": "description_value",
                 }
             ],
+            "volume_data_restore_policy_bindings": [{"policy": 1, "volume_type": 1}],
+            "restore_order": {
+                "group_kind_dependencies": [{"satisfying": {}, "requiring": {}}]
+            },
         },
         "labels": {},
         "state": 1,
         "state_reason": "state_reason_value",
         "complete_time": {},
         "resources_restored_count": 2602,
         "resources_excluded_count": 2576,
         "resources_failed_count": 2343,
         "volumes_restored_count": 2394,
         "etag": "etag_value",
+        "filter": {
+            "inclusion_filters": [
+                {
+                    "group_kind": {},
+                    "name": "name_value",
+                    "namespace": "namespace_value",
+                    "labels": {},
+                }
+            ],
+            "exclusion_filters": {},
+        },
+        "volume_data_restore_policy_overrides": [{"policy": 1, "selected_pvcs": {}}],
     }
     # The version of a generated dependency at test runtime may differ from the version used during generation.
     # Delete any fields which are not present in the current runtime dependency
     # See https://github.com/googleapis/gapic-generator-python/issues/1748
 
     # Determine if the message type is proto-plus or protobuf
     test_field = gkebackup.UpdateRestoreRequest.meta.fields["restore"]
@@ -16924,14 +20093,54 @@
         req.return_value = response_value
         response = client.update_restore(request)
 
     # Establish that the response is the type that we expect.
     assert response.operation.name == "operations/spam"
 
 
+def test_update_restore_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = BackupForGKEClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.update_restore in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.update_restore] = mock_rpc
+
+        request = {}
+        client.update_restore(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        # Operation methods build a cached wrapper on first rpc call
+        # subsequent calls should use the cached wrapper
+        wrapper_fn.reset_mock()
+
+        client.update_restore(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_update_restore_rest_required_fields(
     request_type=gkebackup.UpdateRestoreRequest,
 ):
     transport_class = transports.BackupForGKERestTransport
 
     request_init = {}
     request = request_type(**request_init)
@@ -17191,14 +20400,54 @@
         req.return_value = response_value
         response = client.delete_restore(request)
 
     # Establish that the response is the type that we expect.
     assert response.operation.name == "operations/spam"
 
 
+def test_delete_restore_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = BackupForGKEClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.delete_restore in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.delete_restore] = mock_rpc
+
+        request = {}
+        client.delete_restore(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        # Operation methods build a cached wrapper on first rpc call
+        # subsequent calls should use the cached wrapper
+        wrapper_fn.reset_mock()
+
+        client.delete_restore(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_delete_restore_rest_required_fields(
     request_type=gkebackup.DeleteRestoreRequest,
 ):
     transport_class = transports.BackupForGKERestTransport
 
     request_init = {}
     request_init["name"] = ""
@@ -17474,14 +20723,54 @@
         response = client.list_volume_restores(request)
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.ListVolumeRestoresPager)
     assert response.next_page_token == "next_page_token_value"
 
 
+def test_list_volume_restores_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = BackupForGKEClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.list_volume_restores in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.list_volume_restores
+        ] = mock_rpc
+
+        request = {}
+        client.list_volume_restores(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.list_volume_restores(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_list_volume_restores_rest_required_fields(
     request_type=gkebackup.ListVolumeRestoresRequest,
 ):
     transport_class = transports.BackupForGKERestTransport
 
     request_init = {}
     request_init["parent"] = ""
@@ -17839,14 +21128,54 @@
     assert response.volume_handle == "volume_handle_value"
     assert response.volume_type == volume.VolumeRestore.VolumeType.GCE_PERSISTENT_DISK
     assert response.state == volume.VolumeRestore.State.CREATING
     assert response.state_message == "state_message_value"
     assert response.etag == "etag_value"
 
 
+def test_get_volume_restore_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = BackupForGKEClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.get_volume_restore in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.get_volume_restore
+        ] = mock_rpc
+
+        request = {}
+        client.get_volume_restore(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.get_volume_restore(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_get_volume_restore_rest_required_fields(
     request_type=gkebackup.GetVolumeRestoreRequest,
 ):
     transport_class = transports.BackupForGKERestTransport
 
     request_init = {}
     request_init["name"] = ""
@@ -18110,14 +21439,55 @@
         response = client.get_backup_index_download_url(request)
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, gkebackup.GetBackupIndexDownloadUrlResponse)
     assert response.signed_url == "signed_url_value"
 
 
+def test_get_backup_index_download_url_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = BackupForGKEClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.get_backup_index_download_url
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.get_backup_index_download_url
+        ] = mock_rpc
+
+        request = {}
+        client.get_backup_index_download_url(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.get_backup_index_download_url(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_get_backup_index_download_url_rest_required_fields(
     request_type=gkebackup.GetBackupIndexDownloadUrlRequest,
 ):
     transport_class = transports.BackupForGKERestTransport
 
     request_init = {}
     request_init["backup"] = ""
```

