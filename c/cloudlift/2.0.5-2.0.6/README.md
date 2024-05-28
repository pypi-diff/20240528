# Comparing `tmp/cloudlift-2.0.5.tar.gz` & `tmp/cloudlift-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudlift-2.0.5.tar", last modified: Mon Apr 15 15:46:14 2024, max compression
+gzip compressed data, was "cloudlift-2.0.6.tar", last modified: Tue May 28 13:59:21 2024, max compression
```

## Comparing `cloudlift-2.0.5.tar` & `cloudlift-2.0.6.tar`

### file list

```diff
@@ -1,64 +1,62 @@
-drwxr-xr-x   0 shoan     (1000) shoan     (1000)        0 2024-04-15 15:46:14.363932 cloudlift-2.0.5/
--rw-rw-rw-   0 shoan     (1000) shoan     (1000)     1062 2020-04-14 13:38:03.000000 cloudlift-2.0.5/LICENSE
--rwx------   0 shoan     (1000) shoan     (1000)       40 2020-02-21 06:48:18.000000 cloudlift-2.0.5/MANIFEST.in
--rw-r--r--   0 shoan     (1000) shoan     (1000)    13573 2024-04-15 15:46:14.360011 cloudlift-2.0.5/PKG-INFO
--rw-r--r--   0 shoan     (1000) shoan     (1000)    13309 2023-12-04 09:29:06.000000 cloudlift-2.0.5/README.md
-drwxr-xr-x   0 shoan     (1000) shoan     (1000)        0 2024-04-15 15:46:13.543328 cloudlift-2.0.5/cloudlift/
--rw-r--r--   0 shoan     (1000) shoan     (1000)     6400 2023-04-26 12:53:28.000000 cloudlift-2.0.5/cloudlift/__init__.py
-drwxr-xr-x   0 shoan     (1000) shoan     (1000)        0 2024-04-15 15:46:13.920612 cloudlift-2.0.5/cloudlift/config/
--rw-r--r--   0 shoan     (1000) shoan     (1000)      266 2022-12-15 11:12:05.000000 cloudlift-2.0.5/cloudlift/config/__init__.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)      669 2024-03-14 07:26:45.000000 cloudlift-2.0.5/cloudlift/config/account.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)      448 2023-02-02 08:10:32.000000 cloudlift-2.0.5/cloudlift/config/banner.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)      621 2022-12-15 11:12:05.000000 cloudlift-2.0.5/cloudlift/config/decimal_encoder.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)     2408 2022-12-15 11:12:05.000000 cloudlift-2.0.5/cloudlift/config/diff.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)     1844 2022-12-15 11:12:05.000000 cloudlift-2.0.5/cloudlift/config/dynamodb_configuration.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)    22093 2023-12-04 09:29:06.000000 cloudlift-2.0.5/cloudlift/config/environment_configuration.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)      546 2022-12-15 11:12:05.000000 cloudlift-2.0.5/cloudlift/config/logging.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)     2129 2024-04-15 12:48:19.000000 cloudlift-2.0.5/cloudlift/config/mfa.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)     4387 2023-01-25 11:43:34.000000 cloudlift-2.0.5/cloudlift/config/parameter_store.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)     2568 2023-04-26 12:53:28.000000 cloudlift-2.0.5/cloudlift/config/pre_flight.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)     3516 2022-12-15 11:12:05.000000 cloudlift-2.0.5/cloudlift/config/region.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)    20176 2023-12-04 09:29:06.000000 cloudlift-2.0.5/cloudlift/config/service_configuration.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)      161 2022-12-15 11:12:05.000000 cloudlift-2.0.5/cloudlift/config/stack.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)     7127 2023-12-04 09:29:06.000000 cloudlift-2.0.5/cloudlift/config/utils.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)      217 2023-12-04 09:29:06.000000 cloudlift-2.0.5/cloudlift/constants.py
-drwxr-xr-x   0 shoan     (1000) shoan     (1000)        0 2024-04-15 15:46:14.219932 cloudlift-2.0.5/cloudlift/deployment/
--rw-r--r--   0 shoan     (1000) shoan     (1000)      373 2022-12-15 11:12:05.000000 cloudlift-2.0.5/cloudlift/deployment/__init__.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)     3154 2022-12-15 11:12:05.000000 cloudlift-2.0.5/cloudlift/deployment/changesets.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)    41735 2024-01-23 15:20:25.000000 cloudlift-2.0.5/cloudlift/deployment/cluster_template_generator.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)      267 2022-12-15 11:12:05.000000 cloudlift-2.0.5/cloudlift/deployment/configs.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)     6391 2023-07-18 05:11:33.000000 cloudlift-2.0.5/cloudlift/deployment/deployer.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)     7658 2024-04-15 15:41:57.000000 cloudlift-2.0.5/cloudlift/deployment/ecr_client.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)    18003 2024-04-15 12:48:19.000000 cloudlift-2.0.5/cloudlift/deployment/ecs.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)      996 2022-12-15 11:12:05.000000 cloudlift-2.0.5/cloudlift/deployment/editor.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)     8032 2023-12-04 18:19:19.000000 cloudlift-2.0.5/cloudlift/deployment/environment_creator.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)      896 2022-12-15 11:12:05.000000 cloudlift-2.0.5/cloudlift/deployment/progress.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)     6646 2022-12-15 11:12:05.000000 cloudlift-2.0.5/cloudlift/deployment/service_creator.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)     7056 2023-12-04 09:29:06.000000 cloudlift-2.0.5/cloudlift/deployment/service_information_fetcher.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)    46514 2023-12-04 09:29:06.000000 cloudlift-2.0.5/cloudlift/deployment/service_template_generator.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)     4397 2023-02-02 08:10:32.000000 cloudlift-2.0.5/cloudlift/deployment/service_updater.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)     6527 2023-04-26 12:53:28.000000 cloudlift-2.0.5/cloudlift/deployment/task_definition_creator.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)     1257 2022-12-15 11:12:05.000000 cloudlift-2.0.5/cloudlift/deployment/template_generator.py
-drwxr-xr-x   0 shoan     (1000) shoan     (1000)        0 2024-04-15 15:46:14.253934 cloudlift-2.0.5/cloudlift/exceptions/
--rw-r--r--   0 shoan     (1000) shoan     (1000)       46 2022-12-15 11:12:05.000000 cloudlift-2.0.5/cloudlift/exceptions/__init__.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)      154 2022-12-15 11:12:05.000000 cloudlift-2.0.5/cloudlift/exceptions/exceptions.py
-drwxr-xr-x   0 shoan     (1000) shoan     (1000)        0 2024-04-15 15:46:14.292934 cloudlift-2.0.5/cloudlift/session/
--rw-r--r--   0 shoan     (1000) shoan     (1000)       30 2022-12-15 11:12:05.000000 cloudlift-2.0.5/cloudlift/session/__init__.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)     1874 2022-12-15 11:12:05.000000 cloudlift-2.0.5/cloudlift/session/session_creator.py
-drwxr-xr-x   0 shoan     (1000) shoan     (1000)        0 2024-04-15 15:46:14.310968 cloudlift-2.0.5/cloudlift/version/
--rw-r--r--   0 shoan     (1000) shoan     (1000)       18 2024-04-15 15:41:57.000000 cloudlift-2.0.5/cloudlift/version/__init__.py
-drwxr-xr-x   0 shoan     (1000) shoan     (1000)        0 2024-04-15 15:46:13.643926 cloudlift-2.0.5/cloudlift.egg-info/
--rw-r--r--   0 shoan     (1000) shoan     (1000)    13573 2024-04-15 15:46:13.000000 cloudlift-2.0.5/cloudlift.egg-info/PKG-INFO
--rw-rw-rw-   0 shoan     (1000) shoan     (1000)     1665 2024-04-15 15:46:13.000000 cloudlift-2.0.5/cloudlift.egg-info/SOURCES.txt
--rw-rw-rw-   0 shoan     (1000) shoan     (1000)        1 2024-04-15 15:46:13.000000 cloudlift-2.0.5/cloudlift.egg-info/dependency_links.txt
--rw-rw-rw-   0 shoan     (1000) shoan     (1000)       44 2024-04-15 15:46:13.000000 cloudlift-2.0.5/cloudlift.egg-info/entry_points.txt
--rw-rw-rw-   0 shoan     (1000) shoan     (1000)      384 2024-04-15 15:46:13.000000 cloudlift-2.0.5/cloudlift.egg-info/requires.txt
--rw-rw-rw-   0 shoan     (1000) shoan     (1000)       10 2024-04-15 15:46:13.000000 cloudlift-2.0.5/cloudlift.egg-info/top_level.txt
--rw-rw-rw-   0 shoan     (1000) shoan     (1000)        1 2020-01-19 03:14:24.000000 cloudlift-2.0.5/cloudlift.egg-info/zip-safe
--rw-r--r--   0 shoan     (1000) shoan     (1000)      100 2021-03-16 11:07:35.000000 cloudlift-2.0.5/pyproject.toml
--rw-r--r--   0 shoan     (1000) shoan     (1000)      383 2024-04-15 12:48:19.000000 cloudlift-2.0.5/requirements.txt
--rw-r--r--   0 shoan     (1000) shoan     (1000)       38 2024-04-15 15:46:14.364932 cloudlift-2.0.5/setup.cfg
--rw-r--r--   0 shoan     (1000) shoan     (1000)      774 2023-12-04 09:29:06.000000 cloudlift-2.0.5/setup.py
-drwxr-xr-x   0 shoan     (1000) shoan     (1000)        0 2024-04-15 15:46:14.340963 cloudlift-2.0.5/test/
--rw-r--r--   0 shoan     (1000) shoan     (1000)     5303 2023-12-04 09:29:06.000000 cloudlift-2.0.5/test/test_cloudlift.py
--rwx------   0 shoan     (1000) shoan     (1000)     2787 2023-08-13 02:51:34.000000 cloudlift-2.0.5/test/test_cloudlift_cluster.py
+drwxr-xr-x   0 shoan     (1000) shoan     (1000)        0 2024-05-28 13:59:21.676849 cloudlift-2.0.6/
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     1062 2024-05-20 12:04:27.000000 cloudlift-2.0.6/LICENSE
+-rw-r--r--   0 shoan     (1000) shoan     (1000)       40 2024-05-20 12:04:27.000000 cloudlift-2.0.6/MANIFEST.in
+-rw-r--r--   0 shoan     (1000) shoan     (1000)    14323 2024-05-28 13:59:21.676849 cloudlift-2.0.6/PKG-INFO
+-rw-r--r--   0 shoan     (1000) shoan     (1000)    13309 2024-05-20 12:04:27.000000 cloudlift-2.0.6/README.md
+drwxr-xr-x   0 shoan     (1000) shoan     (1000)        0 2024-05-28 13:59:21.666849 cloudlift-2.0.6/cloudlift/
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     6400 2024-05-20 12:04:27.000000 cloudlift-2.0.6/cloudlift/__init__.py
+drwxr-xr-x   0 shoan     (1000) shoan     (1000)        0 2024-05-28 13:59:21.666849 cloudlift-2.0.6/cloudlift/config/
+-rw-r--r--   0 shoan     (1000) shoan     (1000)      266 2024-05-20 12:04:27.000000 cloudlift-2.0.6/cloudlift/config/__init__.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)      669 2024-05-20 12:04:27.000000 cloudlift-2.0.6/cloudlift/config/account.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)      448 2024-05-20 12:04:27.000000 cloudlift-2.0.6/cloudlift/config/banner.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)      621 2024-05-20 12:04:27.000000 cloudlift-2.0.6/cloudlift/config/decimal_encoder.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     2408 2024-05-20 12:04:27.000000 cloudlift-2.0.6/cloudlift/config/diff.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     1844 2024-05-20 12:04:27.000000 cloudlift-2.0.6/cloudlift/config/dynamodb_configuration.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)    22232 2024-05-28 10:02:39.000000 cloudlift-2.0.6/cloudlift/config/environment_configuration.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)      546 2024-05-20 12:04:27.000000 cloudlift-2.0.6/cloudlift/config/logging.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     2129 2024-05-20 12:04:27.000000 cloudlift-2.0.6/cloudlift/config/mfa.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     4387 2024-05-20 12:04:27.000000 cloudlift-2.0.6/cloudlift/config/parameter_store.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     2568 2024-05-20 12:04:27.000000 cloudlift-2.0.6/cloudlift/config/pre_flight.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     3516 2024-05-20 12:04:27.000000 cloudlift-2.0.6/cloudlift/config/region.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)    20176 2024-05-20 12:04:27.000000 cloudlift-2.0.6/cloudlift/config/service_configuration.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)      161 2024-05-20 12:04:27.000000 cloudlift-2.0.6/cloudlift/config/stack.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     7127 2024-05-20 12:04:27.000000 cloudlift-2.0.6/cloudlift/config/utils.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)      217 2024-05-20 12:04:27.000000 cloudlift-2.0.6/cloudlift/constants.py
+drwxr-xr-x   0 shoan     (1000) shoan     (1000)        0 2024-05-28 13:59:21.666849 cloudlift-2.0.6/cloudlift/deployment/
+-rw-r--r--   0 shoan     (1000) shoan     (1000)      373 2024-05-20 12:04:27.000000 cloudlift-2.0.6/cloudlift/deployment/__init__.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     3154 2024-05-20 12:04:27.000000 cloudlift-2.0.6/cloudlift/deployment/changesets.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)    42301 2024-05-28 10:02:39.000000 cloudlift-2.0.6/cloudlift/deployment/cluster_template_generator.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)      267 2024-05-20 12:04:27.000000 cloudlift-2.0.6/cloudlift/deployment/configs.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     6391 2024-05-20 12:04:27.000000 cloudlift-2.0.6/cloudlift/deployment/deployer.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     7658 2024-05-24 07:27:39.000000 cloudlift-2.0.6/cloudlift/deployment/ecr_client.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)    18003 2024-05-20 12:04:27.000000 cloudlift-2.0.6/cloudlift/deployment/ecs.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)      996 2024-05-20 12:04:27.000000 cloudlift-2.0.6/cloudlift/deployment/editor.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     8032 2024-05-20 12:04:27.000000 cloudlift-2.0.6/cloudlift/deployment/environment_creator.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)      896 2024-05-20 12:04:27.000000 cloudlift-2.0.6/cloudlift/deployment/progress.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     6646 2024-05-20 12:04:27.000000 cloudlift-2.0.6/cloudlift/deployment/service_creator.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     7056 2024-05-20 12:04:27.000000 cloudlift-2.0.6/cloudlift/deployment/service_information_fetcher.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)    46491 2024-05-28 10:02:39.000000 cloudlift-2.0.6/cloudlift/deployment/service_template_generator.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     4397 2024-05-20 12:04:27.000000 cloudlift-2.0.6/cloudlift/deployment/service_updater.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     6527 2024-05-20 12:04:27.000000 cloudlift-2.0.6/cloudlift/deployment/task_definition_creator.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     1257 2024-05-20 12:04:27.000000 cloudlift-2.0.6/cloudlift/deployment/template_generator.py
+drwxr-xr-x   0 shoan     (1000) shoan     (1000)        0 2024-05-28 13:59:21.676849 cloudlift-2.0.6/cloudlift/exceptions/
+-rw-r--r--   0 shoan     (1000) shoan     (1000)       46 2024-05-20 12:04:27.000000 cloudlift-2.0.6/cloudlift/exceptions/__init__.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)      154 2024-05-20 12:04:27.000000 cloudlift-2.0.6/cloudlift/exceptions/exceptions.py
+drwxr-xr-x   0 shoan     (1000) shoan     (1000)        0 2024-05-28 13:59:21.676849 cloudlift-2.0.6/cloudlift/session/
+-rw-r--r--   0 shoan     (1000) shoan     (1000)       30 2024-05-20 12:04:27.000000 cloudlift-2.0.6/cloudlift/session/__init__.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     1874 2024-05-20 12:04:27.000000 cloudlift-2.0.6/cloudlift/session/session_creator.py
+drwxr-xr-x   0 shoan     (1000) shoan     (1000)        0 2024-05-28 13:59:21.676849 cloudlift-2.0.6/cloudlift/version/
+-rw-r--r--   0 shoan     (1000) shoan     (1000)       18 2024-05-28 10:02:39.000000 cloudlift-2.0.6/cloudlift/version/__init__.py
+drwxr-xr-x   0 shoan     (1000) shoan     (1000)        0 2024-05-28 13:59:21.676849 cloudlift-2.0.6/cloudlift.egg-info/
+-rw-r--r--   0 shoan     (1000) shoan     (1000)    14323 2024-05-28 13:59:21.000000 cloudlift-2.0.6/cloudlift.egg-info/PKG-INFO
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     1619 2024-05-28 13:59:21.000000 cloudlift-2.0.6/cloudlift.egg-info/SOURCES.txt
+-rw-r--r--   0 shoan     (1000) shoan     (1000)        1 2024-05-28 13:59:21.000000 cloudlift-2.0.6/cloudlift.egg-info/dependency_links.txt
+-rw-r--r--   0 shoan     (1000) shoan     (1000)       44 2024-05-28 13:59:21.000000 cloudlift-2.0.6/cloudlift.egg-info/entry_points.txt
+-rw-r--r--   0 shoan     (1000) shoan     (1000)      390 2024-05-28 13:59:21.000000 cloudlift-2.0.6/cloudlift.egg-info/requires.txt
+-rw-r--r--   0 shoan     (1000) shoan     (1000)       10 2024-05-28 13:59:21.000000 cloudlift-2.0.6/cloudlift.egg-info/top_level.txt
+-rw-r--r--   0 shoan     (1000) shoan     (1000)        1 2024-05-21 06:39:07.000000 cloudlift-2.0.6/cloudlift.egg-info/zip-safe
+-rw-r--r--   0 shoan     (1000) shoan     (1000)      396 2024-05-28 10:02:39.000000 cloudlift-2.0.6/requirements.txt
+-rw-r--r--   0 shoan     (1000) shoan     (1000)       38 2024-05-28 13:59:21.676849 cloudlift-2.0.6/setup.cfg
+-rw-r--r--   0 shoan     (1000) shoan     (1000)      774 2024-05-20 12:04:27.000000 cloudlift-2.0.6/setup.py
+drwxr-xr-x   0 shoan     (1000) shoan     (1000)        0 2024-05-28 13:59:21.676849 cloudlift-2.0.6/test/
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     5303 2024-05-20 12:04:27.000000 cloudlift-2.0.6/test/test_cloudlift.py
```

### Comparing `cloudlift-2.0.5/LICENSE` & `cloudlift-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.5/PKG-INFO` & `cloudlift-2.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: cloudlift
-Version: 2.0.5
-Summary: Cloudlift makes it easier to launch dockerized services in AWS ECS
-Home-page: https://github.com/GetSimpl/cloudlift
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Cloudlift
 
 Cloudlift is built by Simpl developers to make it easier to launch dockerized
 services in AWS ECS.
 
 Cloudlift is a command-line tool for dockerized services to be deployed in AWS
 ECS. It's very simple to use. That's possible because this is heavily
```

### Comparing `cloudlift-2.0.5/README.md` & `cloudlift-2.0.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,40 @@
+Metadata-Version: 2.1
+Name: cloudlift
+Version: 2.0.6
+Summary: Cloudlift makes it easier to launch dockerized services in AWS ECS
+Home-page: https://github.com/GetSimpl/cloudlift
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: boto3==1.34.111
+Requires-Dist: awscli==1.32.111
+Requires-Dist: certifi==2017.7.27.1
+Requires-Dist: cfn-flip==1.0.3
+Requires-Dist: chardet==3.0.4
+Requires-Dist: click==6.7
+Requires-Dist: colorclass==2.2.2
+Requires-Dist: dictdiffer==0.7.0
+Requires-Dist: docutils==0.14
+Requires-Dist: future==0.16.0
+Requires-Dist: futures==3.1.1
+Requires-Dist: idna==2.6
+Requires-Dist: jmespath==0.9.3
+Requires-Dist: jsonschema==2.6.0
+Requires-Dist: moto==1.3.7
+Requires-Dist: pytest==4.0.0
+Requires-Dist: python-dateutil==2.8.2
+Requires-Dist: requests>=2.20.0
+Requires-Dist: six==1.10.0
+Requires-Dist: stringcase==1.0.6
+Requires-Dist: terminaltables==3.1.0
+Requires-Dist: troposphere==4.5.2
+Requires-Dist: awacs==2.4.0
+Requires-Dist: botocore==1.34.111
+
 # Cloudlift
 
 Cloudlift is built by Simpl developers to make it easier to launch dockerized
 services in AWS ECS.
 
 Cloudlift is a command-line tool for dockerized services to be deployed in AWS
 ECS. It's very simple to use. That's possible because this is heavily
```

### Comparing `cloudlift-2.0.5/cloudlift/__init__.py` & `cloudlift-2.0.6/cloudlift/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.5/cloudlift/config/account.py` & `cloudlift-2.0.6/cloudlift/config/account.py`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.5/cloudlift/config/decimal_encoder.py` & `cloudlift-2.0.6/cloudlift/config/decimal_encoder.py`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.5/cloudlift/config/diff.py` & `cloudlift-2.0.6/cloudlift/config/diff.py`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.5/cloudlift/config/dynamodb_configuration.py` & `cloudlift-2.0.6/cloudlift/config/dynamodb_configuration.py`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.5/cloudlift/config/environment_configuration.py` & `cloudlift-2.0.6/cloudlift/config/environment_configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -298,15 +298,18 @@
                                 "max_instances": {"type": "integer"},
                                 "spot_min_instances": {"type": "integer"},
                                 "spot_max_instances": {"type": "integer"},
                                 "instance_type": {"type": "string"},
                                 "key_name": {"type": "string"},
                                 "allocation_strategy": {"type": "string"},
                                 "spot_instance_pools": {"type": "integer"},
-                                "ecs_instance_default_lifecycle_type": {"type": "string"}
+                                "ecs_instance_default_lifecycle_type":  {
+                                    "type": "string",
+                                    "pattern": "^(spot|ondemand)$"
+                                }
                             },
                             "required": [
                                 "min_instances",
                                 "max_instances",
                                 "instance_type",
                                 "key_name"
                             ]
```

### Comparing `cloudlift-2.0.5/cloudlift/config/logging.py` & `cloudlift-2.0.6/cloudlift/config/logging.py`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.5/cloudlift/config/mfa.py` & `cloudlift-2.0.6/cloudlift/config/mfa.py`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.5/cloudlift/config/parameter_store.py` & `cloudlift-2.0.6/cloudlift/config/parameter_store.py`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.5/cloudlift/config/pre_flight.py` & `cloudlift-2.0.6/cloudlift/config/pre_flight.py`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.5/cloudlift/config/region.py` & `cloudlift-2.0.6/cloudlift/config/region.py`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.5/cloudlift/config/service_configuration.py` & `cloudlift-2.0.6/cloudlift/config/service_configuration.py`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.5/cloudlift/config/utils.py` & `cloudlift-2.0.6/cloudlift/config/utils.py`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.5/cloudlift/deployment/changesets.py` & `cloudlift-2.0.6/cloudlift/deployment/changesets.py`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.5/cloudlift/deployment/cluster_template_generator.py` & `cloudlift-2.0.6/cloudlift/deployment/cluster_template_generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import json
 import re
+import textwrap
 
 from cfn_flip import to_yaml
 from stringcase import camelcase, pascalcase
 from troposphere import (Base64, FindInMap, Output, Parameter, Ref, Sub,
                          cloudformation, Export, GetAtt, Tags)
 from troposphere.autoscaling import (AutoScalingGroup, LaunchTemplateSpecification, NotificationConfigurations,
                                      ScalingPolicy, MixedInstancesPolicy, LaunchTemplateOverrides, InstancesDistribution )
 from troposphere.autoscaling import LaunchTemplate as ASGLaunchTemplate
 from troposphere.cloudwatch import Alarm, MetricDimension
 from troposphere.ec2 import (VPC, InternetGateway, NatGateway, Route,
                              RouteTable, SecurityGroup, Subnet,
                              SubnetRouteTableAssociation, VPCGatewayAttachment,SecurityGroupIngress,
-                             LaunchTemplateData, LaunchTemplate, IamInstanceProfile, LaunchTemplateBlockDeviceMapping, EBSBlockDevice)
+                             LaunchTemplateData, LaunchTemplate, IamInstanceProfile, LaunchTemplateBlockDeviceMapping,
+                             EBSBlockDevice, MetadataOptions)
 from troposphere.ecs import Cluster
 from troposphere.elasticache import SubnetGroup as ElastiCacheSubnetGroup
 from troposphere.iam import InstanceProfile, Role
 from troposphere.logs import LogGroup
 from troposphere.policies import (AutoScalingRollingUpdate, CreationPolicy,
                                   ResourceSignal)
 from troposphere.rds import DBSubnetGroup
@@ -489,23 +491,23 @@
                                 ])
                             ),
                         ),
                     "/etc/dnsmasq.conf": cloudformation.InitFile(
                         content=Sub(
                             '\n'.join([
                                 '# Server Configuration',
-                                'listen-address=127.0.0.1',
+                                'listen-address=::1,127.0.0.1',
                                 'port=53',
                                 'bind-interfaces',
+                                'interface=lo',
                                 'user=dnsmasq',
                                 'group=dnsmasq',
                                 'pid-file=/var/run/dnsmasq.pid',
-                                '# Name resolution options',
                                 'resolv-file=/etc/resolv.dnsmasq',
-                                'cache-size=500',
+                                'cache-size=1000',
                                 'neg-ttl=60',
                                 'domain-needed',
                                 'bogus-priv',
                             ])
                         ),
                     )
                 }),
@@ -528,47 +530,67 @@
                                 'echo ECS_AVAILABLE_LOGGING_DRIVERS=\'["awslogs","fluentd"]\' >> /etc/ecs/ecs.config',
                                 'echo ECS_INSTANCE_ATTRIBUTES=\'{"deployment_type": "'+ deployment_type.lower() + '"}\' >> /etc/ecs/ecs.config',
                                 lc_metadata_override,
                                 ]).strip()
                             )
                         },
                         '02_set_nameserver': {
-                            'command': "INTERFACE=$(curl --silent http://169.254.169.254/latest/meta-data/network/interfaces/macs/ | head -n1); IS_IT_CLASSIC=$(curl --write-out %{http_code} --silent --output /dev/null http://169.254.169.254/latest/meta-data/network/interfaces/macs/${INTERFACE}/vpc-id); if [[ $IS_IT_CLASSIC == '404' ]]; then bash -c \"echo 'supersede domain-name-servers 127.0.0.1, 172.16.0.23;' >> /etc/dhcp/dhclient.conf && echo 'nameserver 172.16.0.23' > /etc/resolv.dnsmasq\"; else  bash -c \"echo 'supersede domain-name-servers 127.0.0.1, 169.254.169.253;' >> /etc/dhcp/dhclient.conf && echo 'nameserver 169.254.169.253' > /etc/resolv.dnsmasq\"; fi"
+                            'command': 'echo "nameserver 169.254.169.253" > /etc/resolv.dnsmasq'
                         },
                         '03_install_dnsmasq_package': {
                             'command': 'yum install -y dnsmasq bind-utils'
                         },
                         '04_create_group': {
-                            'command': 'groupadd -r dnsmasq'
+                            'command': 'groupadd -r -f dnsmasq'
                         },
                         '05_create_user': {
-                            'command': 'useradd -r -g dnsmasq dnsmasq'
+                            'command': 'id -u dnsmasq &>/dev/null && (id -nG dnsmasq | grep -qw dnsmasq || usermod -a -G dnsmasq dnsmasq) || useradd -r -g dnsmasq dnsmasq'
                         },
-                        '06_add_locahost_nameserver': {
-                            'command': "sed -i '/search ap-south-1.compute.internal/a nameserver 127.0.0.1' /etc/resolv.conf"
+                        '06_disable_systemd_resolved_stub_resolver': {
+                            'command': textwrap.dedent("""
+                                        mkdir -pv /etc/systemd/resolved.conf.d
+
+                                        cat <<'EOF' | tee /etc/systemd/resolved.conf.d/00-override.conf
+                                        [Resolve]
+                                        DNSStubListener=no
+                                        MulticastDNS=no
+                                        LLMNR=no
+
+                                        EOF
+
+                                        systemctl daemon-reload
+                                        systemctl restart systemd-resolved""")
                         },
-                        '07_enable_dnsmasq_service': {
-                            'command': 'pidof systemd && systemctl restart dnsmasq.service || service dnsmasq restart'
+                        '07_add_localhost_nameserver': {
+                            'command': textwrap.dedent(f"""
+                                        unlink /etc/resolv.conf
+                                        cat <<'EOF' | tee /etc/resolv.conf
+                                        nameserver 127.0.0.1
+                                        search {self.region}.compute.internal
+
+                                        EOF
+                                        """)
+                        },
+                        '08_enable_dnsmasq_service': {
+                            'command': 'pidof systemd && systemctl enable dnsmasq.service || chkconfig dnsmasq on'
                         },
-                        '08_start_dnsmasq_service': {
-                            'command': 'pidof systemd && systemctl enable  dnsmasq.service || chkconfig dnsmasq on'
+                        '09_start_dnsmasq_service': {
+                            'command': 'pidof systemd && systemctl restart dnsmasq.service || service dnsmasq restart'
                         },
-                        '09_configure_dhclient': {
-                            'command': 'bash -c "dhclient"'
-                        }
             })})
             launch_template_data = LaunchTemplateData(
                 'LaunchTemplateData',
                 UserData=user_data,
                 IamInstanceProfile=IamInstanceProfile(
                     Arn=GetAtt(instance_profile, 'Arn')
                 ),
                 SecurityGroupIds=[GetAtt(self.sg_hosts, 'GroupId')],
                 ImageId=FindInMap("AWSRegionToAMI", Ref("AWS::Region"), "AMI"),
                 KeyName=Ref(self.key_pair),
+                MetadataOptions=MetadataOptions(HttpTokens="required"),
                 BlockDeviceMappings=[
                     LaunchTemplateBlockDeviceMapping(
                         DeviceName="/dev/xvda",
                         Ebs=EBSBlockDevice(
                             VolumeType="gp3"
                         )
                     )
@@ -729,15 +751,15 @@
         # Pick from https://docs.aws.amazon.com/AmazonECS/latest/developerguide/al2ami.html
         ami_id_ssm = self.configuration.get('cluster', {}).get('ami_id', None)
         if ami_id_ssm == 'None':
             ami_id_ssm = None
         ssm_client = get_client_for('ssm', self.env)
         if ami_id_ssm == None:
             ami_response = ssm_client.get_parameter(
-                Name='/aws/service/ecs/optimized-ami/amazon-linux-2/recommended')
+                Name='/aws/service/ecs/optimized-ami/amazon-linux-2023/recommended')
         else:
             ami_response = ssm_client.get_parameter(
                 Name= str(ami_id_ssm))
         ami_id = json.loads(ami_response['Parameter']['Value'])['image_id']
         region = get_region_for_environment(self.env)
         self.template.add_mapping('AWSRegionToAMI', {
             region: {"AMI": ami_id}
```

### Comparing `cloudlift-2.0.5/cloudlift/deployment/deployer.py` & `cloudlift-2.0.6/cloudlift/deployment/deployer.py`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.5/cloudlift/deployment/ecr_client.py` & `cloudlift-2.0.6/cloudlift/deployment/ecr_client.py`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.5/cloudlift/deployment/ecs.py` & `cloudlift-2.0.6/cloudlift/deployment/ecs.py`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.5/cloudlift/deployment/editor.py` & `cloudlift-2.0.6/cloudlift/deployment/editor.py`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.5/cloudlift/deployment/environment_creator.py` & `cloudlift-2.0.6/cloudlift/deployment/environment_creator.py`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.5/cloudlift/deployment/progress.py` & `cloudlift-2.0.6/cloudlift/deployment/progress.py`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.5/cloudlift/deployment/service_creator.py` & `cloudlift-2.0.6/cloudlift/deployment/service_creator.py`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.5/cloudlift/deployment/service_information_fetcher.py` & `cloudlift-2.0.6/cloudlift/deployment/service_information_fetcher.py`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.5/cloudlift/deployment/service_template_generator.py` & `cloudlift-2.0.6/cloudlift/deployment/service_template_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -230,15 +230,16 @@
             "Essential": 'true',
             "Cpu": 0
         }
         placement_constraint = {}
         if 'fargate' not in config:
             for key in self.environment_stack["Outputs"]:
                 if key["OutputKey"] == 'ECSClusterDefaultInstanceLifecycle':
-                    spot_deployment = False if ImportValue("{self.env}ECSClusterDefaultInstanceLifecycle".format(**locals())) == 'ondemand' else True
+                    instance_lifecycle = key["OutputValue"]
+                    spot_deployment = instance_lifecycle == 'spot'
                     placement_constraint = {
                         "PlacementConstraints": [PlacementConstraint(
                             Type='memberOf',
                             Expression='attribute:deployment_type == spot' if spot_deployment else 'attribute:deployment_type == ondemand'
                         )],
                     }
             if 'spot_deployment' in config:
```

### Comparing `cloudlift-2.0.5/cloudlift/deployment/service_updater.py` & `cloudlift-2.0.6/cloudlift/deployment/service_updater.py`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.5/cloudlift/deployment/task_definition_creator.py` & `cloudlift-2.0.6/cloudlift/deployment/task_definition_creator.py`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.5/cloudlift/deployment/template_generator.py` & `cloudlift-2.0.6/cloudlift/deployment/template_generator.py`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.5/cloudlift/session/session_creator.py` & `cloudlift-2.0.6/cloudlift/session/session_creator.py`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.5/cloudlift.egg-info/PKG-INFO` & `cloudlift-2.0.6/cloudlift.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,39 @@
 Metadata-Version: 2.1
 Name: cloudlift
-Version: 2.0.5
+Version: 2.0.6
 Summary: Cloudlift makes it easier to launch dockerized services in AWS ECS
 Home-page: https://github.com/GetSimpl/cloudlift
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: boto3==1.34.111
+Requires-Dist: awscli==1.32.111
+Requires-Dist: certifi==2017.7.27.1
+Requires-Dist: cfn-flip==1.0.3
+Requires-Dist: chardet==3.0.4
+Requires-Dist: click==6.7
+Requires-Dist: colorclass==2.2.2
+Requires-Dist: dictdiffer==0.7.0
+Requires-Dist: docutils==0.14
+Requires-Dist: future==0.16.0
+Requires-Dist: futures==3.1.1
+Requires-Dist: idna==2.6
+Requires-Dist: jmespath==0.9.3
+Requires-Dist: jsonschema==2.6.0
+Requires-Dist: moto==1.3.7
+Requires-Dist: pytest==4.0.0
+Requires-Dist: python-dateutil==2.8.2
+Requires-Dist: requests>=2.20.0
+Requires-Dist: six==1.10.0
+Requires-Dist: stringcase==1.0.6
+Requires-Dist: terminaltables==3.1.0
+Requires-Dist: troposphere==4.5.2
+Requires-Dist: awacs==2.4.0
+Requires-Dist: botocore==1.34.111
 
 # Cloudlift
 
 Cloudlift is built by Simpl developers to make it easier to launch dockerized
 services in AWS ECS.
 
 Cloudlift is a command-line tool for dockerized services to be deployed in AWS
```

### Comparing `cloudlift-2.0.5/cloudlift.egg-info/SOURCES.txt` & `cloudlift-2.0.6/cloudlift.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
 MANIFEST.in
 README.md
-pyproject.toml
 requirements.txt
 setup.py
 cloudlift/__init__.py
 cloudlift/constants.py
 cloudlift.egg-info/PKG-INFO
 cloudlift.egg-info/SOURCES.txt
 cloudlift.egg-info/dependency_links.txt
@@ -45,9 +44,8 @@
 cloudlift/deployment/task_definition_creator.py
 cloudlift/deployment/template_generator.py
 cloudlift/exceptions/__init__.py
 cloudlift/exceptions/exceptions.py
 cloudlift/session/__init__.py
 cloudlift/session/session_creator.py
 cloudlift/version/__init__.py
-test/test_cloudlift.py
-test/test_cloudlift_cluster.py
+test/test_cloudlift.py
```

### Comparing `cloudlift-2.0.5/setup.py` & `cloudlift-2.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.5/test/test_cloudlift.py` & `cloudlift-2.0.6/test/test_cloudlift.py`

 * *Files identical despite different names*

