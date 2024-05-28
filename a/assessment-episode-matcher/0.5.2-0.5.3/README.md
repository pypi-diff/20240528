# Comparing `tmp/assessment_episode_matcher-0.5.2.tar.gz` & `tmp/assessment_episode_matcher-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assessment_episode_matcher-0.5.2.tar", last modified: Mon May 27 04:17:03 2024, max compression
+gzip compressed data, was "assessment_episode_matcher-0.5.3.tar", last modified: Tue May 28 08:10:43 2024, max compression
```

## Comparing `assessment_episode_matcher-0.5.2.tar` & `assessment_episode_matcher-0.5.3.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 04:17:03.412838 assessment_episode_matcher-0.5.2/
--rw-rw-rw-   0        0        0     1235 2024-05-17 18:46:24.000000 assessment_episode_matcher-0.5.2/LICENSE
--rw-rw-rw-   0        0        0       26 2024-05-23 22:46:12.000000 assessment_episode_matcher-0.5.2/MANIFEST.in
--rw-rw-rw-   0        0        0      523 2024-05-27 04:17:03.407787 assessment_episode_matcher-0.5.2/PKG-INFO
--rw-rw-rw-   0        0        0      889 2024-05-27 04:16:19.000000 assessment_episode_matcher-0.5.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 04:17:02.806818 assessment_episode_matcher-0.5.2/assessment_episode_matcher/
--rw-rw-rw-   0        0        0      275 2024-05-23 23:19:26.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/__init__.py
--rw-rw-rw-   0        0        0      267 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/audits.py
-drwxrwxrwx   0        0        0        0 2024-05-27 04:17:02.904542 assessment_episode_matcher-0.5.2/assessment_episode_matcher/azutil/
--rw-rw-rw-   0        0        0        0 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/azutil/__init__.py
--rw-rw-rw-   0        0        0     5165 2024-05-27 01:14:59.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/azutil/az_blob_query.py
--rw-rw-rw-   0        0        0     9458 2024-05-22 23:27:05.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/azutil/az_tables_query.py
--rw-rw-rw-   0        0        0     1594 2024-05-27 02:50:37.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/azutil/file_types.py
--rw-rw-rw-   0        0        0     3921 2024-05-18 20:57:07.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/azutil/helper.py
-drwxrwxrwx   0        0        0        0 2024-05-27 04:17:02.932368 assessment_episode_matcher-0.5.2/assessment_episode_matcher/configs/
--rw-rw-rw-   0        0        0        0 2024-05-24 21:35:01.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/configs/__init__.py
--rw-rw-rw-   0        0        0      972 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/configs/audit.py
--rw-rw-rw-   0        0        0      631 2024-05-26 21:44:37.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/configs/episodes.py
--rw-rw-rw-   0        0        0     8591 2024-05-17 22:40:20.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/data_config.py
--rw-rw-rw-   0        0        0     5899 2024-05-27 00:25:15.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/data_prep.py
-drwxrwxrwx   0        0        0        0 2024-05-27 04:17:02.953173 assessment_episode_matcher-0.5.2/assessment_episode_matcher/exporters/
--rw-rw-rw-   0        0        0     1848 2024-05-26 23:42:24.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/exporters/NADAbase.py
--rw-rw-rw-   0        0        0        0 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/exporters/__init__.py
--rw-rw-rw-   0        0        0     3850 2024-05-27 01:14:46.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/exporters/main.py
-drwxrwxrwx   0        0        0        0 2024-05-27 04:17:03.009614 assessment_episode_matcher-0.5.2/assessment_episode_matcher/importers/
--rw-rw-rw-   0        0        0        0 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/importers/__init__.py
--rw-rw-rw-   0        0        0    14368 2024-05-27 02:49:09.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/importers/aod.py
--rw-rw-rw-   0        0        0     8836 2024-05-26 22:49:07.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/importers/assessments.py
--rw-rw-rw-   0        0        0     6681 2024-05-26 21:50:05.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/importers/episodes.py
--rw-rw-rw-   0        0        0     3749 2024-05-27 00:19:22.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/importers/main.py
--rw-rw-rw-   0        0        0     1485 2024-05-26 23:26:37.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/importers/nada_indexed.py
-drwxrwxrwx   0        0        0        0 2024-05-27 04:17:03.101048 assessment_episode_matcher-0.5.2/assessment_episode_matcher/matching/
--rw-rw-rw-   0        0        0        0 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/matching/__init__.py
--rw-rw-rw-   0        0        0     4403 2024-05-18 20:54:57.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/matching/date_checks.py
--rw-rw-rw-   0        0        0     4510 2024-05-27 03:27:36.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/matching/errors.py
--rw-rw-rw-   0        0        0     5321 2024-05-18 20:55:18.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/matching/increasing_slack.py
--rw-rw-rw-   0        0        0    21314 2024-05-22 23:38:15.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/matching/main.py
--rw-rw-rw-   0        0        0     1004 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/matching/matching_stats.py
--rw-rw-rw-   0        0        0     2592 2024-05-27 02:55:23.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/mytypes.py
--rw-rw-rw-   0        0        0     3965 2024-05-27 03:29:54.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/nada.py
-drwxrwxrwx   0        0        0        0 2024-05-27 04:17:03.140411 assessment_episode_matcher-0.5.2/assessment_episode_matcher/setup/
--rw-rw-rw-   0        0        0        0 2024-05-19 22:35:00.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/setup/__init__.py
--rw-rw-rw-   0        0        0     4933 2024-05-26 00:16:34.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/setup/bootstrap.py
--rw-rw-rw-   0        0        0     2318 2024-05-19 22:34:48.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/setup/log_management.py
--rw-rw-rw-   0        0        0     8870 2024-05-27 03:01:01.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/test_surveytxt.py
--rw-rw-rw-   0        0        0     8366 2024-05-26 22:16:46.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/test_surveytxt_local.py
-drwxrwxrwx   0        0        0        0 2024-05-27 04:17:03.215437 assessment_episode_matcher-0.5.2/assessment_episode_matcher/tests/
--rw-rw-rw-   0        0        0       23 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/tests/__init__.py
--rw-rw-rw-   0        0        0     1377 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/tests/matching_test.py
-drwxrwxrwx   0        0        0        0 2024-05-27 04:17:03.371374 assessment_episode_matcher-0.5.2/assessment_episode_matcher/utils/
--rw-rw-rw-   0        0        0        0 2024-05-17 21:30:48.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/utils/__init__.py
--rw-rw-rw-   0        0        0     1270 2024-05-18 20:54:35.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/utils/base.py
--rw-rw-rw-   0        0        0     1693 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/utils/ccare_to_aztable.py
--rw-rw-rw-   0        0        0    13615 2024-05-19 23:11:34.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/utils/df_ops_base.py
--rw-rw-rw-   0        0        0     7323 2024-05-18 19:37:57.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/utils/dtypes.py
--rw-rw-rw-   0        0        0     1557 2024-05-22 23:17:51.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/utils/environment.py
--rw-rw-rw-   0        0        0     1972 2024-05-22 23:41:56.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/utils/fromstr.py
--rw-rw-rw-   0        0        0      748 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/utils/group_utils.py
--rw-rw-rw-   0        0        0    11458 2024-05-25 23:06:26.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/utils/io.py
--rw-rw-rw-   0        0        0       21 2024-05-27 04:15:38.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/version.py
-drwxrwxrwx   0        0        0        0 2024-05-27 04:17:03.383132 assessment_episode_matcher-0.5.2/assessment_episode_matcher.egg-info/
--rw-rw-rw-   0        0        0      523 2024-05-27 04:17:02.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2429 2024-05-27 04:17:02.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 04:17:02.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      105 2024-05-27 04:17:02.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2024-05-27 04:17:02.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      110 2024-05-17 19:08:24.000000 assessment_episode_matcher-0.5.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-27 04:17:03.416469 assessment_episode_matcher-0.5.2/setup.cfg
--rw-rw-rw-   0        0        0     1342 2024-05-24 03:53:56.000000 assessment_episode_matcher-0.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:10:43.469207 assessment_episode_matcher-0.5.3/
+-rw-rw-rw-   0        0        0     1235 2024-05-17 18:46:24.000000 assessment_episode_matcher-0.5.3/LICENSE
+-rw-rw-rw-   0        0        0       26 2024-05-23 22:46:12.000000 assessment_episode_matcher-0.5.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      523 2024-05-28 08:10:43.461449 assessment_episode_matcher-0.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0      935 2024-05-28 08:06:39.000000 assessment_episode_matcher-0.5.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 08:10:42.429201 assessment_episode_matcher-0.5.3/assessment_episode_matcher/
+-rw-rw-rw-   0        0        0      275 2024-05-23 23:19:26.000000 assessment_episode_matcher-0.5.3/assessment_episode_matcher/__init__.py
+-rw-rw-rw-   0        0        0      267 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.5.3/assessment_episode_matcher/audits.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:10:42.810421 assessment_episode_matcher-0.5.3/assessment_episode_matcher/azutil/
+-rw-rw-rw-   0        0        0        0 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.5.3/assessment_episode_matcher/azutil/__init__.py
+-rw-rw-rw-   0        0        0     5203 2024-05-27 23:08:56.000000 assessment_episode_matcher-0.5.3/assessment_episode_matcher/azutil/az_blob_query.py
+-rw-rw-rw-   0        0        0     9425 2024-05-27 23:09:54.000000 assessment_episode_matcher-0.5.3/assessment_episode_matcher/azutil/az_tables_query.py
+-rw-rw-rw-   0        0        0     1594 2024-05-27 02:50:37.000000 assessment_episode_matcher-0.5.3/assessment_episode_matcher/azutil/file_types.py
+-rw-rw-rw-   0        0        0     3921 2024-05-18 20:57:07.000000 assessment_episode_matcher-0.5.3/assessment_episode_matcher/azutil/helper.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:10:42.878128 assessment_episode_matcher-0.5.3/assessment_episode_matcher/configs/
+-rw-rw-rw-   0        0        0        0 2024-05-24 21:35:01.000000 assessment_episode_matcher-0.5.3/assessment_episode_matcher/configs/__init__.py
+-rw-rw-rw-   0        0        0     1331 2024-05-28 07:17:39.000000 assessment_episode_matcher-0.5.3/assessment_episode_matcher/configs/audit.py
+-rw-rw-rw-   0        0        0      631 2024-05-26 21:44:37.000000 assessment_episode_matcher-0.5.3/assessment_episode_matcher/configs/episodes.py
+-rw-rw-rw-   0        0        0     8591 2024-05-17 22:40:20.000000 assessment_episode_matcher-0.5.3/assessment_episode_matcher/data_config.py
+-rw-rw-rw-   0        0        0     5899 2024-05-27 00:25:15.000000 assessment_episode_matcher-0.5.3/assessment_episode_matcher/data_prep.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:10:42.922877 assessment_episode_matcher-0.5.3/assessment_episode_matcher/exporters/
+-rw-rw-rw-   0        0        0     1848 2024-05-26 23:42:24.000000 assessment_episode_matcher-0.5.3/assessment_episode_matcher/exporters/NADAbase.py
+-rw-rw-rw-   0        0        0        0 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.5.3/assessment_episode_matcher/exporters/__init__.py
+-rw-rw-rw-   0        0        0     3850 2024-05-27 01:14:46.000000 assessment_episode_matcher-0.5.3/assessment_episode_matcher/exporters/main.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:10:43.028776 assessment_episode_matcher-0.5.3/assessment_episode_matcher/importers/
+-rw-rw-rw-   0        0        0        0 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.5.3/assessment_episode_matcher/importers/__init__.py
+-rw-rw-rw-   0        0        0    14368 2024-05-27 02:49:09.000000 assessment_episode_matcher-0.5.3/assessment_episode_matcher/importers/aod.py
+-rw-rw-rw-   0        0        0     8836 2024-05-26 22:49:07.000000 assessment_episode_matcher-0.5.3/assessment_episode_matcher/importers/assessments.py
+-rw-rw-rw-   0        0        0     6681 2024-05-26 21:50:05.000000 assessment_episode_matcher-0.5.3/assessment_episode_matcher/importers/episodes.py
+-rw-rw-rw-   0        0        0     3749 2024-05-27 00:19:22.000000 assessment_episode_matcher-0.5.3/assessment_episode_matcher/importers/main.py
+-rw-rw-rw-   0        0        0     1485 2024-05-26 23:26:37.000000 assessment_episode_matcher-0.5.3/assessment_episode_matcher/importers/nada_indexed.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:10:43.105573 assessment_episode_matcher-0.5.3/assessment_episode_matcher/matching/
+-rw-rw-rw-   0        0        0        0 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.5.3/assessment_episode_matcher/matching/__init__.py
+-rw-rw-rw-   0        0        0     4474 2024-05-27 22:25:32.000000 assessment_episode_matcher-0.5.3/assessment_episode_matcher/matching/date_checks.py
+-rw-rw-rw-   0        0        0     4528 2024-05-28 07:17:12.000000 assessment_episode_matcher-0.5.3/assessment_episode_matcher/matching/errors.py
+-rw-rw-rw-   0        0        0     5321 2024-05-18 20:55:18.000000 assessment_episode_matcher-0.5.3/assessment_episode_matcher/matching/increasing_slack.py
+-rw-rw-rw-   0        0        0    22363 2024-05-28 07:22:56.000000 assessment_episode_matcher-0.5.3/assessment_episode_matcher/matching/main.py
+-rw-rw-rw-   0        0        0     1004 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.5.3/assessment_episode_matcher/matching/matching_stats.py
+-rw-rw-rw-   0        0        0     2506 2024-05-27 22:23:53.000000 assessment_episode_matcher-0.5.3/assessment_episode_matcher/mytypes.py
+-rw-rw-rw-   0        0        0     3965 2024-05-27 03:29:54.000000 assessment_episode_matcher-0.5.3/assessment_episode_matcher/nada.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:10:43.168717 assessment_episode_matcher-0.5.3/assessment_episode_matcher/setup/
+-rw-rw-rw-   0        0        0        0 2024-05-19 22:35:00.000000 assessment_episode_matcher-0.5.3/assessment_episode_matcher/setup/__init__.py
+-rw-rw-rw-   0        0        0     4933 2024-05-26 00:16:34.000000 assessment_episode_matcher-0.5.3/assessment_episode_matcher/setup/bootstrap.py
+-rw-rw-rw-   0        0        0     2318 2024-05-19 22:34:48.000000 assessment_episode_matcher-0.5.3/assessment_episode_matcher/setup/log_management.py
+-rw-rw-rw-   0        0        0     9278 2024-05-28 07:21:08.000000 assessment_episode_matcher-0.5.3/assessment_episode_matcher/test_surveytxt.py
+-rw-rw-rw-   0        0        0     8363 2024-05-27 22:54:01.000000 assessment_episode_matcher-0.5.3/assessment_episode_matcher/test_surveytxt_local.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:10:43.205006 assessment_episode_matcher-0.5.3/assessment_episode_matcher/tests/
+-rw-rw-rw-   0        0        0       23 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.5.3/assessment_episode_matcher/tests/__init__.py
+-rw-rw-rw-   0        0        0     1377 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.5.3/assessment_episode_matcher/tests/matching_test.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:10:43.402655 assessment_episode_matcher-0.5.3/assessment_episode_matcher/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-17 21:30:48.000000 assessment_episode_matcher-0.5.3/assessment_episode_matcher/utils/__init__.py
+-rw-rw-rw-   0        0        0     1270 2024-05-18 20:54:35.000000 assessment_episode_matcher-0.5.3/assessment_episode_matcher/utils/base.py
+-rw-rw-rw-   0        0        0     1693 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.5.3/assessment_episode_matcher/utils/ccare_to_aztable.py
+-rw-rw-rw-   0        0        0    13615 2024-05-19 23:11:34.000000 assessment_episode_matcher-0.5.3/assessment_episode_matcher/utils/df_ops_base.py
+-rw-rw-rw-   0        0        0     7323 2024-05-18 19:37:57.000000 assessment_episode_matcher-0.5.3/assessment_episode_matcher/utils/dtypes.py
+-rw-rw-rw-   0        0        0     1303 2024-05-27 04:43:32.000000 assessment_episode_matcher-0.5.3/assessment_episode_matcher/utils/environment.py
+-rw-rw-rw-   0        0        0     2247 2024-05-28 06:45:09.000000 assessment_episode_matcher-0.5.3/assessment_episode_matcher/utils/fromstr.py
+-rw-rw-rw-   0        0        0      748 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.5.3/assessment_episode_matcher/utils/group_utils.py
+-rw-rw-rw-   0        0        0    11458 2024-05-25 23:06:26.000000 assessment_episode_matcher-0.5.3/assessment_episode_matcher/utils/io.py
+-rw-rw-rw-   0        0        0       21 2024-05-28 08:05:58.000000 assessment_episode_matcher-0.5.3/assessment_episode_matcher/version.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:10:43.432545 assessment_episode_matcher-0.5.3/assessment_episode_matcher.egg-info/
+-rw-rw-rw-   0        0        0      523 2024-05-28 08:10:41.000000 assessment_episode_matcher-0.5.3/assessment_episode_matcher.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2429 2024-05-28 08:10:41.000000 assessment_episode_matcher-0.5.3/assessment_episode_matcher.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 08:10:41.000000 assessment_episode_matcher-0.5.3/assessment_episode_matcher.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      105 2024-05-28 08:10:41.000000 assessment_episode_matcher-0.5.3/assessment_episode_matcher.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2024-05-28 08:10:41.000000 assessment_episode_matcher-0.5.3/assessment_episode_matcher.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      110 2024-05-17 19:08:24.000000 assessment_episode_matcher-0.5.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 08:10:43.472586 assessment_episode_matcher-0.5.3/setup.cfg
+-rw-rw-rw-   0        0        0     1342 2024-05-24 03:53:56.000000 assessment_episode_matcher-0.5.3/setup.py
```

### Comparing `assessment_episode_matcher-0.5.2/LICENSE` & `assessment_episode_matcher-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.5.2/PKG-INFO` & `assessment_episode_matcher-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assessment_episode_matcher
-Version: 0.5.2
+Version: 0.5.3
 Author: Aftab Jalal
 Author-email: mj@auditlytics.nz
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `assessment_episode_matcher-0.5.2/README.md` & `assessment_episode_matcher-0.5.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -25,7 +25,8 @@
 
 0.3.1 - removing disk writes as read-only on cloud fs
 0.4.0 - remove all local writes and reads, refactor, fix errors_warning writes
 0.5.0 - write redindexed to csv (instead of parq).
          Survey.txt write to blob storage.
 0.5.1 - AOD warnings, rename reindexed file to match format prefix_date-range_suffix: prefix:forstxt_
 0.5.2 - Fixed Destination Paths (on blob storage)
+0.5.3 - Load Blob Config for drug Mapping, etc
```

### Comparing `assessment_episode_matcher-0.5.2/assessment_episode_matcher/azutil/az_blob_query.py` & `assessment_episode_matcher-0.5.3/assessment_episode_matcher/azutil/az_blob_query.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 
+import os
 import logging
 from typing import Any
 from io import BytesIO
 import pandas as pd
 from azure.storage.blob import BlobServiceClient #, BlobClient, ContainerClient
-
 from assessment_episode_matcher.mytypes import CSVTypeObject
-from assessment_episode_matcher.utils.environment import ConfigKeys, ConfigManager
-from assessment_episode_matcher.azutil.file_types import BlobCSVFilePrepper, BlobDataFrameCSVFilePrepper, BlobDataFrameParquetFilePrepper
+from assessment_episode_matcher.utils.environment import ConfigKeys
+import assessment_episode_matcher.azutil.file_types as AzUtilFtypes
 # import mylogging
 
 # logging = mylogging.get('azure.storage')
 
 
 class AzureBlobQuery(object):
-  def __init__(self):
-      config = ConfigManager().config
-    
-      # self.connection_string = str(config.get(ConfigKeys.AZURE_STORAGE_CONNECTION_STRING,"Help"))
-      self.connection_string = str(config.get(ConfigKeys.AZURE_BLOB_CONNECTION_STRING.value,"Help"))
-      
+  _instance = None
+
+  def __new__(cls):
+      if cls._instance is None:
+          cls._instance = super(AzureBlobQuery, cls).__new__(cls)
+          cls._instance.initialize()
+      return cls._instance
+
+  def initialize(self):
+      self.connection_string = str(os.environ.get(ConfigKeys.AZURE_BLOB_CONNECTION_STRING.value, "Help"))
       if self.connection_string == 'Help':
-        logging.error("Blob Connection string not found.")
-        self.connection_string = ""
-        # st.warning("An error occurred while loading the data. Please try again later.")
-        return None
-      self.blob_service_client =  BlobServiceClient.from_connection_string(self.connection_string)
+          logging.error("Blob Connection string not found.")
+          self.connection_string = ""
+          # st.warning("An error occurred while loading the data. Please try again later.")
+          return None
+      self.blob_service_client = BlobServiceClient.from_connection_string(self.connection_string)
 
 
   def list_files(self, container_name: str, folder_path:str , prefix: str, suffix: str) -> list[str]:
       # blob_service_client = BlobServiceClient.from_connection_string(self.connection_string)
       container_client = self.blob_service_client.get_container_client(container_name)
       if folder_path:
         final_prefix = folder_path + "/" + prefix
@@ -59,34 +63,34 @@
         # You may want to display a user-friendly message in the Streamlit app
         # st.warning("An error occurred while loading the data. Please try again later.")
         return None       
 
 
   def write_dataframe(self, container_name:str, blob_url:str
                  , data:pd.DataFrame) -> dict[str, Any]:
-
+    
     blob_client = self.blob_service_client.get_blob_client(container=container_name
                                                       , blob=blob_url)
     if blob_url[-3:] =='csv':
-      p = BlobDataFrameCSVFilePrepper()    
+      p = AzUtilFtypes.BlobDataFrameCSVFilePrepper()    
     else:
-      p = BlobDataFrameParquetFilePrepper()
+      p = AzUtilFtypes.BlobDataFrameParquetFilePrepper()
       
     file = p.get_file_for_blob(data)
        
     result_dict = blob_client.upload_blob(file, overwrite=True)
 
     return result_dict
   
 
 
   def write_csv(self, container_name:str, blob_url:str
                  , data:CSVTypeObject) -> dict[str, Any]:
     
-    csvprep = BlobCSVFilePrepper()
+    csvprep = AzUtilFtypes.BlobCSVFilePrepper()
     csv_data = csvprep.get_file_for_blob(data)
 
     # Upload the CSV data to Azure Blob Storage
     blob_client = self.blob_service_client \
                   .get_blob_client(container=container_name
                                   , blob=blob_url)
     result_dict = blob_client.upload_blob(csv_data, overwrite=True)
```

### Comparing `assessment_episode_matcher-0.5.2/assessment_episode_matcher/azutil/az_tables_query.py` & `assessment_episode_matcher-0.5.3/assessment_episode_matcher/azutil/az_tables_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 DESCRIPTION:
     These samples demonstrate the following: querying a table for entities.
 USAGE:
     python sample_query_table.py
     Set the environment variables with your own values before running the sample:
     1) AZURE_STORAGE_CONNECTION_STRING - the connection string to your storage account
 """
+import os
 import logging
 import pandas as pd
 from azure.data.tables import TableClient, TableEntity#, TableTransaction
 from azure.core.exceptions import HttpResponseError
-from assessment_episode_matcher.utils.environment import ConfigKeys, ConfigManager
+from assessment_episode_matcher.utils.environment import ConfigKeys
 # import mylogging
 
 # logging = mylogging.get(__name__)
 
 class SampleTablesQuery(object):
 
     def __init__(self, table_name:str):
-      config = ConfigManager().config
-    
-      self.connection_string = str(config.get(ConfigKeys.AZURE_STORAGE_CONNECTION_STRING.value,""))
+         
+      self.connection_string =  str(os.environ.get(ConfigKeys.AZURE_STORAGE_CONNECTION_STRING.value,""))
 
       self.table_name = table_name
       logging.info(f"SampleTablesQuery initialised with connection_string: {self.connection_string}")
 
         
     def query_table(self, select_fields:list[str], filter_template:str, query_params:dict|None):    
         """
```

### Comparing `assessment_episode_matcher-0.5.2/assessment_episode_matcher/azutil/file_types.py` & `assessment_episode_matcher-0.5.3/assessment_episode_matcher/azutil/file_types.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.5.2/assessment_episode_matcher/azutil/helper.py` & `assessment_episode_matcher-0.5.3/assessment_episode_matcher/azutil/helper.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.5.2/assessment_episode_matcher/configs/audit.py` & `assessment_episode_matcher-0.5.3/assessment_episode_matcher/configs/audit.py`

 * *Files 20% similar despite different names*

```diff
@@ -23,31 +23,39 @@
 "ESTABLISHMENT IDENTIFIER"
   , "PMSEpisodeID"
   , "PMSPersonID"
   , "CommencementDate"
   , "EndDate"
   , "SLK"
   , "Program"
-
 ]
 
 COLUMNS_AUDIT_EPKEY_CLIENTPROG = [ 
  *COLUMNS_AUDIT_EPKEY_CLIENT, "SLK_Program"
 ]
 
+COLUMNS_AUDIT_EPKEY_CLIENT = [ *COLUMNS_AUDIT_EPKEY_CLIENT
+                            , "closest_atom_SLK"]
+
+
 
-COLUMNS_AUDIT_ASMTKEY = [ 
+COLUMNS_AUDIT_ASMTKEY_CLIENT = [ 
    "SLK"
   , "RowKey"
 	, "AssessmentDate"
   , "Program"
 	, "Staff"
 	, "SurveyName"
-
 ]
 
+COLUMNS_AUDIT_ASMTKEY_CLIENTPROG = COLUMNS_AUDIT_ASMTKEY_CLIENT.copy()
 
+COLUMNS_AUDIT_ASMTKEY_CLIENT = [
+  *COLUMNS_AUDIT_ASMTKEY_CLIENTPROG 
+  , "closest_episode_SLK"]
 
 COLUMNS_AUDIT_DATES.extend(additional_fields)
 COLUMNS_AUDIT_EPKEY_CLIENT.extend(additional_fields)
 COLUMNS_AUDIT_EPKEY_CLIENTPROG.extend(additional_fields)
-COLUMNS_AUDIT_ASMTKEY.extend(additional_fields)
+
+COLUMNS_AUDIT_ASMTKEY_CLIENTPROG.extend(additional_fields)
+COLUMNS_AUDIT_ASMTKEY_CLIENT.extend(additional_fields)
```

### Comparing `assessment_episode_matcher-0.5.2/assessment_episode_matcher/configs/episodes.py` & `assessment_episode_matcher-0.5.3/assessment_episode_matcher/configs/episodes.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.5.2/assessment_episode_matcher/data_config.py` & `assessment_episode_matcher-0.5.3/assessment_episode_matcher/data_config.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.5.2/assessment_episode_matcher/data_prep.py` & `assessment_episode_matcher-0.5.3/assessment_episode_matcher/data_prep.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.5.2/assessment_episode_matcher/exporters/NADAbase.py` & `assessment_episode_matcher-0.5.3/assessment_episode_matcher/exporters/NADAbase.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.5.2/assessment_episode_matcher/exporters/main.py` & `assessment_episode_matcher-0.5.3/assessment_episode_matcher/exporters/main.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.5.2/assessment_episode_matcher/importers/aod.py` & `assessment_episode_matcher-0.5.3/assessment_episode_matcher/importers/aod.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.5.2/assessment_episode_matcher/importers/assessments.py` & `assessment_episode_matcher-0.5.3/assessment_episode_matcher/importers/assessments.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.5.2/assessment_episode_matcher/importers/episodes.py` & `assessment_episode_matcher-0.5.3/assessment_episode_matcher/importers/episodes.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.5.2/assessment_episode_matcher/importers/main.py` & `assessment_episode_matcher-0.5.3/assessment_episode_matcher/importers/main.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.5.2/assessment_episode_matcher/importers/nada_indexed.py` & `assessment_episode_matcher-0.5.3/assessment_episode_matcher/importers/nada_indexed.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.5.2/assessment_episode_matcher/matching/date_checks.py` & `assessment_episode_matcher-0.5.3/assessment_episode_matcher/matching/date_checks.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,16 +44,14 @@
     ValidationMaskIssueTuple(
        mask =  lambda df: (df['days_from_end'] > limit_days) ,
       validation_issue = ValidationError(      
                 msg =  f"Assessment date is after episode end date by more than {limit_days}.",
                 issue_type = IssueType.DATE_MISMATCH,
       )
     ),
-    
-   
   ]
 
 
 # Define matching functions
 def assessment_date_validator(gaps_df, mit_dict:ValidationMaskIssueTuple) ->\
                                 tuple[pd.DataFrame, pd.DataFrame]:
   # Check if assessment date falls between commencement and end dates
@@ -83,23 +81,28 @@
   merged_df = merged_df1.assign(
      days_from_start=(merged_df1[ad] - merged_df1[dk.episode_start_date.value]).apply(lambda x: x.days) 
     , days_from_end=( merged_df1[ad] - merged_df1[dk.episode_end_date.value]).apply(lambda x: x.days)
     )
   return merged_df
 
 
-def keep_nearest_mismatching_episode(unmatched_asmt:pd.DataFrame) -> pd.DataFrame:
+def keep_nearest_mismatching_episode(
+      unmatched_asmt:pd.DataFrame) -> pd.DataFrame:
    unm = unmatched_asmt.copy()
-   unm['min_days'] = np.minimum(np.abs(unm['days_from_start']), np.abs(unm['days_from_end']))
+   unm['min_days'] = np.minimum(
+                        np.abs(unm['days_from_start'])
+                        , np.abs(unm['days_from_end']))
    ew_df = unm.sort_values(['SLK_RowKey', 'min_days'])
    ew_df = ew_df.drop_duplicates('SLK_RowKey', keep='first')
    return ew_df
 
 
-def get_assessment_boundary_issues(dt_unmtch_asmt:pd.DataFrame, mask_isuetypes:list[ValidationMaskIssueTuple], ukey:str) \
+def get_assessment_boundary_issues(
+              dt_unmtch_asmt:pd.DataFrame
+              , mask_isuetypes:list[ValidationMaskIssueTuple]) \
                       -> pd.DataFrame:
     gaps_df = gap_asmtdate_epsd_boundaries(dt_unmtch_asmt)
     nearest_remaining_mismatch = keep_nearest_mismatching_episode(gaps_df)
     full_ew_df =  pd.DataFrame()
     for v in mask_isuetypes:
         nearest_remaining_mismatch, ew_df = assessment_date_validator(nearest_remaining_mismatch, v)        
         if ut.has_data(ew_df):
```

### Comparing `assessment_episode_matcher-0.5.2/assessment_episode_matcher/matching/errors.py` & `assessment_episode_matcher-0.5.3/assessment_episode_matcher/matching/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,16 +40,16 @@
                       ,a_dt,a_dt
                       ,period_start, period_end)
 
     # limit columns to write out
     final_dates_ew = final_dates_ew[audit_cfg.COLUMNS_AUDIT_DATES]
     slkonlyin_ep_error = slkonlyin_ep_error[audit_cfg.COLUMNS_AUDIT_EPKEY_CLIENT]
     slkprogonlyin_ep_warn = slkprogonlyin_ep_warn[audit_cfg.COLUMNS_AUDIT_EPKEY_CLIENTPROG]
-    slkonlyin_amst_error = slkonlyin_amst_error[audit_cfg.COLUMNS_AUDIT_ASMTKEY]
-    slkprogonlyin_amst_warn = slkprogonlyin_amst_warn[audit_cfg.COLUMNS_AUDIT_ASMTKEY]
+    slkonlyin_amst_error = slkonlyin_amst_error[audit_cfg.COLUMNS_AUDIT_ASMTKEY_CLIENT]
+    slkprogonlyin_amst_warn = slkprogonlyin_amst_warn[audit_cfg.COLUMNS_AUDIT_ASMTKEY_CLIENTPROG]
 
 
     ew2 = {
        'dates_ew':final_dates_ew,
        'asmt_key_errors': slkonlyin_amst_error,
        'ep_key_errors': slkonlyin_ep_error,
        'asmt_key_warn': slkprogonlyin_amst_warn,
```

### Comparing `assessment_episode_matcher-0.5.2/assessment_episode_matcher/matching/increasing_slack.py` & `assessment_episode_matcher-0.5.3/assessment_episode_matcher/matching/increasing_slack.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.5.2/assessment_episode_matcher/matching/main.py` & `assessment_episode_matcher-0.5.3/assessment_episode_matcher/matching/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import logging
 from datetime import date
+from typing import Optional
 import pandas as pd
 from assessment_episode_matcher.mytypes import DataKeys as dk, IssueLevel, IssueType, Purpose #, ValidationIssue
 # from utils.environment import MyEnvironmentConfig, ConfigKeys
 import assessment_episode_matcher.utils.df_ops_base as utdf
 from assessment_episode_matcher.utils import base as utbase
+from assessment_episode_matcher.utils import fromstr as utstr
 import assessment_episode_matcher.matching.date_checks as dtchk
 from assessment_episode_matcher.matching import increasing_slack as mis
-from assessment_episode_matcher.setup.bootstrap import Bootstrap
+# from assessment_episode_matcher.setup.bootstrap import Bootstrap
+SLK_MATCH_THRESHOLD = 0.75
 
 def get_data_for_matching2(episode_df, atom_df, start_date:date
                            , end_date:date, slack_for_matching) \
               -> tuple[pd.DataFrame, pd.DataFrame, pd.DataFrame, pd.DataFrame]:
   a_df, e_df,inperiod_atomslk_notin_ep, inperiod_epslk_notin_atom \
       = get_asmts_4_active_eps2(
                   episode_df, atom_df, start_date=start_date
@@ -202,15 +205,15 @@
     result_matched_df, dt_unmat_asmts, duplicate_rows_dfs = \
       mis.match_dates_increasing_slack (merged_df #,mergekeys_to_check
                                           , max_slack=slack_ndays)
 
     mask_isuetype_map = dtchk.date_boundary_validators(limit_days=slack_ndays)
     # validation_issues, matched_df, invalid_indices =
     ew_df = dtchk.get_assessment_boundary_issues(\
-       dt_unmat_asmts, mask_isuetype_map, match_key)
+       dt_unmat_asmts, mask_isuetype_map)
     
     if not utdf.has_data(duplicate_rows_dfs):
        return result_matched_df, ew_df
     # exclude from error reporting if it is in the results:
     duplicate_rows_dfs = duplicate_rows_dfs[~duplicate_rows_dfs.PMSEpisodeID_SLK_RowKey
                                             .isin(result_matched_df.PMSEpisodeID_SLK_RowKey)]
     # in the errors, show ALL the episodes the assessment matches to
@@ -356,15 +359,29 @@
           , slk_datematched['Program_y'].value_counts())
     
     slk_datematched['Program'] = slk_datematched['Program_y'] 
     
     return slk_datematched
 
 
-def match_and_get_issues(e_df, a_df, inperiod_atomslk_notin_ep, inperiod_epslk_notin_atom, slack_for_matching):
+def get_closest_slk_match (notmatched_slks:list[str]
+                           , slks:pd.Series
+                           , match_threshold=SLK_MATCH_THRESHOLD) -> pd.Series:
+  result = slks.apply(lambda x: utstr
+                      .find_closest_match(x
+                                          , notmatched_slks
+                                          , match_threshold))
+  return result
+
+   
+def match_and_get_issues(e_df, a_df
+                         , inperiod_atomslk_notin_ep
+                         , inperiod_epslk_notin_atom
+                         , slack_for_matching
+                         , config:Optional[dict]={}):
     """
       Perform Date Matching  - Assessment has to fall within Episode Start and End dates
       Steps: 
       1. Date-Match by SLK+Program combination
       2. For the unmatched set, date-match by SLK only (ignore if the program mismatches)
       3. Produce Errors and Warnings:
           a. Error: SLK not in Episodes list
@@ -409,14 +426,24 @@
 
     # TODO: explain why these are two different things (pre date-matching vs post date-matching errors)
     print("concating pre-match missing SLK errors of lengths :")
     print(f"\n\t only-in-ATOM: {len(inperiod_atomslk_notin_ep)}  ; only in Episode: {len(inperiod_epslk_notin_atom)} ")
     slk_onlyinass = pd.concat([slk_onlyinass, inperiod_atomslk_notin_ep])
     slk_onlyin_ep = pd.concat([slk_onlyin_ep, inperiod_epslk_notin_atom])
 
+    if config and config.get("get_nearest_slk",0) == 1:
+      slk_onlyin_ep['closest_atom_SLK'] = get_closest_slk_match(           
+              a_ineprogs.SLK.unique().tolist()
+              , slk_onlyin_ep.SLK
+              )
+      
+      slk_onlyinass['closest_episode_SLK'] = get_closest_slk_match(
+              e_df.SLK.unique().tolist()
+              , slk_onlyinass.SLK )
+
     ew = {
         'slk_onlyinass': slk_onlyinass,
         'slk_onlyin_ep': slk_onlyin_ep,
         'slk_prog_onlyinass': slk_prog_onlyinass,
         'slk_prog_onlyin_ep': slk_prog_onlyin_ep,
         'dates_ewdf': dates_ewdf,
         'dates_ewdf2': dates_ewdf2
```

### Comparing `assessment_episode_matcher-0.5.2/assessment_episode_matcher/matching/matching_stats.py` & `assessment_episode_matcher-0.5.3/assessment_episode_matcher/matching/matching_stats.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.5.2/assessment_episode_matcher/mytypes.py` & `assessment_episode_matcher-0.5.3/assessment_episode_matcher/mytypes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from enum import Enum, auto
 from dataclasses import dataclass, fields
 from typing import Any, Optional #, KW_ONLY
 from collections import namedtuple
 
 
-
 @dataclass
 class CSVTypeObject:
   header:list[str]
   rows:list
 
 @dataclass
 class AODWarning:
@@ -51,18 +50,14 @@
   episode_id = 'PMSEpisodeID'
   per_client_asmt_id = 'RowKey'
   assessment_id = f"{client_id}_{per_client_asmt_id}"  #'SLK_RowKey'
   assessment_date = 'AssessmentDate'
   episode_start_date = 'CommencementDate'
   episode_end_date = 'EndDate'
 
-class DatasetType(Enum):
-    ASSESSMENT = 'assessment'
-    EPISODE = 'episode'
-
 
 class IssueLevel(Enum):
   WARNING = auto()
   ERROR = auto()
 
 class IssueType(Enum):
   DATE_MISMATCH = auto()        #1
```

### Comparing `assessment_episode_matcher-0.5.2/assessment_episode_matcher/nada.py` & `assessment_episode_matcher-0.5.3/assessment_episode_matcher/nada.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.5.2/assessment_episode_matcher/setup/bootstrap.py` & `assessment_episode_matcher-0.5.3/assessment_episode_matcher/setup/bootstrap.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.5.2/assessment_episode_matcher/setup/log_management.py` & `assessment_episode_matcher-0.5.3/assessment_episode_matcher/setup/log_management.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.5.2/assessment_episode_matcher/test_surveytxt.py` & `assessment_episode_matcher-0.5.3/assessment_episode_matcher/test_surveytxt_local.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,22 @@
+import os
 import logging
 import json
-from datetime import datetime
-# from pathlib import Path
-# import pandas as pd
+
 from assessment_episode_matcher import project_directory
 from assessment_episode_matcher.importers.main import BlobFileSource, FileSource
 from assessment_episode_matcher.setup.bootstrap import Bootstrap
 from assessment_episode_matcher.utils.environment import ConfigKeys
 from assessment_episode_matcher.utils.fromstr import get_date_from_str
 from assessment_episode_matcher.matching import main as match_helper
 from assessment_episode_matcher.matching.errors import process_errors_warnings
 
-# from assessment_episode_matcher.data_prep import prep_dataframe_nada
-# from assessment_episode_matcher.exporters import NADAbase as out_exporter
-# from assessment_episode_matcher.importers import episodes as imptr_episodes
-# from assessment_episode_matcher.importers import assessments as imptr_atoms
 from assessment_episode_matcher.importers import episodes as EpisodesImporter
 from assessment_episode_matcher.importers import assessments as ATOMsImporter
-from assessment_episode_matcher.exporters.main import AzureBlobExporter #, CSVExporter as AuditExporter
+from assessment_episode_matcher.exporters import main as  ExporterTypes #import LocalFileExporter as DataExporter
 # from assessment_episode_matcher.exporters.main import AzureBlobExporter as AuditExporter
 import assessment_episode_matcher.utils.df_ops_base as utdf
 from assessment_episode_matcher.mytypes import DataKeys as dk, Purpose
 
 """
  TODO:
   A. Add to Matching:
@@ -44,22 +39,19 @@
         
 #     return st
     
 
 def main3():
     # TODO:
     # envinronemnt setup : Config setup, Expected Directories create, logging setup
-    bstrap = Bootstrap.setup(project_directory, env="prod")
+    # bstrap = Bootstrap.setup(project_directory, env="prod")
     container = "atom-matching"
     ep_folder, asmt_folder = "MDS", "ATOM"
     
-    cfg = bstrap.config #, bstrap.logger
-    # ConfigManager.setup('dev')
-    # cfg = ConfigManager().config
-    slack_for_matching = int(cfg.get(ConfigKeys.MATCHING_NDAYS_SLACK.value, 7))
+    slack_for_matching = 7 # int(cfg.get(ConfigKeys.MATCHING_NDAYS_SLACK.value, 7))
     
     reporting_start_str, reporting_end_str =  '20220101', '20240331'
 
     reporting_start, reporting_end = get_date_from_str (reporting_start_str,"%Y%m%d") \
                                       , get_date_from_str (reporting_end_str,"%Y%m%d")
 
     ep_file_source:FileSource = BlobFileSource(container_name=container
@@ -73,30 +65,30 @@
       logging.error("No episodes")
       return json.dumps({"result":"no episode data"})
     #TODO:
     if ep_cache_to_path:
       if ep_cache_to_path[-3:] =='csv':
          ep_cache_to_path = f"{ep_cache_to_path[:-3]}parquet"
          
-      exp = AzureBlobExporter(container_name=ep_file_source.container_name) #
+      exp = ExporterTypes.AzureBlobExporter(container_name=ep_file_source.container_name) #
       exp.export_dataframe(data_name=ep_cache_to_path, data=episode_df)   
                         # func.HttpResponse(body=json.dumps({"result":"no episode data"}),
                         #         mimetype="application/json", status_code=200)
 
     
     atom_file_source:FileSource = BlobFileSource(container_name=container
                                             , folder_path=asmt_folder)
     atoms_df, atom_cache_to_path = ATOMsImporter.import_data(
                             reporting_start_str, reporting_end_str
                             , atom_file_source
                             , prefix=asmt_folder, suffix="AllPrograms"
                             , purpose=Purpose.NADA, refresh=True)
     
     if atom_cache_to_path:
-      exp = AzureBlobExporter(container_name=atom_file_source.container_name) #
+      exp =  ExporterTypes.AzureBlobExporter(container_name=atom_file_source.container_name) #
       exp.export_dataframe(data_name=atom_cache_to_path, data=atoms_df)    
                             # , prefix="MDS", suffix="AllPrograms")
     if not utdf.has_data(atoms_df):
       logging.error("No ATOMs")
       return json.dumps({"result":"no ATOM data"})
 
     a_df, e_df, inperiod_atomslk_notin_ep, inperiod_epslk_notin_atom = \
@@ -108,45 +100,39 @@
    
     final_good, ew = match_helper.match_and_get_issues(e_df, a_df
                                           , inperiod_atomslk_notin_ep
                                           , inperiod_epslk_notin_atom, slack_for_matching)
 
     warning_asmt_ids  = final_good.SLK_RowKey.unique()
    
-    ae = AzureBlobExporter(container_name=atom_file_source.container_name
+    ae = ExporterTypes.AzureBlobExporter(container_name=atom_file_source.container_name
                            ,config={'location' : 'errors_warnings'})
 
     process_errors_warnings(ew, warning_asmt_ids, dk.client_id.value
                             , period_start=reporting_start
                             , period_end=reporting_end
                             , audit_exporter=ae)
   
 
     df_reindexed = final_good.reset_index(drop=True)
 
-    exp = AzureBlobExporter(container_name=atom_file_source.container_name) #
-    p_str = f"{reporting_start_str}-{reporting_end_str}"
-    exp.export_dataframe(data_name=f"NADA/{p_str}/forstxt_{p_str}_reindexed.parquet", data=df_reindexed)
+    exp = ExporterTypes.AzureBlobExporter(container_name=atom_file_source.container_name) #
+    exp.export_csv(data_name=f"NADA/{reporting_start_str}-{reporting_end_str}_reindexed.csv", data=df_reindexed)
     # exp.export_data(data_name=f"NADA/{reporting_start_str}-{reporting_end_str}_reindexed.parquet", data=df_reindexed)      
 
     #   # logging.info("Result object", json.dumps(result))
        
     # finally:
     return df_reindexed
     # nada_importfile:Path = Path("data/out") / \
     #                        f"{reporting_start}_{reporting_end}_surveytxt.csv"
     # nada = generate_nada_export(df_reindexed, outfile=nada_importfile)
 
     # return nada
-
-  
-       
-
 if __name__ == "__main__":
-  #  load_blob_config()
     res = main3()
 
 
 
 # def main2():
 #     # TODO:
 #     # envinronemnt setup : Config setup, Expected Directories create, logging setup
```

### Comparing `assessment_episode_matcher-0.5.2/assessment_episode_matcher/test_surveytxt_local.py` & `assessment_episode_matcher-0.5.3/assessment_episode_matcher/test_surveytxt.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 import logging
 import json
-
+from datetime import datetime
+# from pathlib import Path
+# import pandas as pd
 from assessment_episode_matcher import project_directory
 from assessment_episode_matcher.importers.main import BlobFileSource, FileSource
 from assessment_episode_matcher.setup.bootstrap import Bootstrap
 from assessment_episode_matcher.utils.environment import ConfigKeys
 from assessment_episode_matcher.utils.fromstr import get_date_from_str
 from assessment_episode_matcher.matching import main as match_helper
 from assessment_episode_matcher.matching.errors import process_errors_warnings
 
+# from assessment_episode_matcher.data_prep import prep_dataframe_nada
+# from assessment_episode_matcher.exporters import NADAbase as out_exporter
+# from assessment_episode_matcher.importers import episodes as imptr_episodes
+# from assessment_episode_matcher.importers import assessments as imptr_atoms
 from assessment_episode_matcher.importers import episodes as EpisodesImporter
 from assessment_episode_matcher.importers import assessments as ATOMsImporter
-from assessment_episode_matcher.exporters.main import LocalFileExporter as DataExporter
+from assessment_episode_matcher.exporters.main import AzureBlobExporter #, CSVExporter as AuditExporter
 # from assessment_episode_matcher.exporters.main import AzureBlobExporter as AuditExporter
 import assessment_episode_matcher.utils.df_ops_base as utdf
 from assessment_episode_matcher.mytypes import DataKeys as dk, Purpose
 
 """
  TODO:
   A. Add to Matching:
@@ -33,15 +39,21 @@
 #     res, warnings_aod = prep_dataframe_nada(matched_assessments)
 
 #     st = out_exporter.generate_finaloutput_df(res)
 #     # st.to_parquet('/data/out/surveytxt.parquet')
 #     st.to_csv(outfile, index=False)
         
 #     return st
-    
+
+def load_blob_config():
+  config_file_source = BlobFileSource(container_name="atom-matching"
+                                            , folder_path=".")
+  config = config_file_source.load_json_file(filename="configuration.json", dtype=str)
+  # print(config)
+  return config
 
 def main3():
     # TODO:
     # envinronemnt setup : Config setup, Expected Directories create, logging setup
     bstrap = Bootstrap.setup(project_directory, env="prod")
     container = "atom-matching"
     ep_folder, asmt_folder = "MDS", "ATOM"
@@ -68,45 +80,48 @@
       return json.dumps({"result":"no episode data"})
     #TODO:
     if ep_cache_to_path:
       if ep_cache_to_path[-3:] =='csv':
          ep_cache_to_path = f"{ep_cache_to_path[:-3]}parquet"
          
       exp = AzureBlobExporter(container_name=ep_file_source.container_name) #
-      exp.export_data(data_name=ep_cache_to_path, data=episode_df)   
+      exp.export_dataframe(data_name=ep_cache_to_path, data=episode_df)   
                         # func.HttpResponse(body=json.dumps({"result":"no episode data"}),
                         #         mimetype="application/json", status_code=200)
 
     
     atom_file_source:FileSource = BlobFileSource(container_name=container
                                             , folder_path=asmt_folder)
     atoms_df, atom_cache_to_path = ATOMsImporter.import_data(
                             reporting_start_str, reporting_end_str
                             , atom_file_source
                             , prefix=asmt_folder, suffix="AllPrograms"
                             , purpose=Purpose.NADA, refresh=True)
     
     if atom_cache_to_path:
       exp = AzureBlobExporter(container_name=atom_file_source.container_name) #
-      exp.export_data(data_name=atom_cache_to_path, data=atoms_df)    
+      exp.export_dataframe(data_name=atom_cache_to_path, data=atoms_df)    
                             # , prefix="MDS", suffix="AllPrograms")
     if not utdf.has_data(atoms_df):
       logging.error("No ATOMs")
       return json.dumps({"result":"no ATOM data"})
 
     a_df, e_df, inperiod_atomslk_notin_ep, inperiod_epslk_notin_atom = \
       match_helper.get_data_for_matching2(episode_df, atoms_df
                                         , reporting_start, reporting_end, slack_for_matching=7)    
     if not utdf.has_data(a_df) or not utdf.has_data(e_df):
         print("No data to match. Ending")
         return None    
    
+    config = load_blob_config()
     final_good, ew = match_helper.match_and_get_issues(e_df, a_df
                                           , inperiod_atomslk_notin_ep
-                                          , inperiod_epslk_notin_atom, slack_for_matching)
+                                          , inperiod_epslk_notin_atom
+                                          , slack_for_matching
+                                          , config)
 
     warning_asmt_ids  = final_good.SLK_RowKey.unique()
    
     ae = AzureBlobExporter(container_name=atom_file_source.container_name
                            ,config={'location' : 'errors_warnings'})
 
     process_errors_warnings(ew, warning_asmt_ids, dk.client_id.value
@@ -114,27 +129,33 @@
                             , period_end=reporting_end
                             , audit_exporter=ae)
   
 
     df_reindexed = final_good.reset_index(drop=True)
 
     exp = AzureBlobExporter(container_name=atom_file_source.container_name) #
-    exp.export_data(data_name=f"NADA/{reporting_start_str}-{reporting_end_str}_reindexed.csv", data=df_reindexed)
+    p_str = f"{reporting_start_str}-{reporting_end_str}"
+    exp.export_dataframe(data_name=f"NADA/{p_str}/forstxt_{p_str}_reindexed.parquet", data=df_reindexed)
     # exp.export_data(data_name=f"NADA/{reporting_start_str}-{reporting_end_str}_reindexed.parquet", data=df_reindexed)      
 
     #   # logging.info("Result object", json.dumps(result))
        
     # finally:
     return df_reindexed
     # nada_importfile:Path = Path("data/out") / \
     #                        f"{reporting_start}_{reporting_end}_surveytxt.csv"
     # nada = generate_nada_export(df_reindexed, outfile=nada_importfile)
 
     # return nada
+
+  
+       
+
 if __name__ == "__main__":
+  #  load_blob_config()
     res = main3()
 
 
 
 # def main2():
 #     # TODO:
 #     # envinronemnt setup : Config setup, Expected Directories create, logging setup
```

### Comparing `assessment_episode_matcher-0.5.2/assessment_episode_matcher/tests/matching_test.py` & `assessment_episode_matcher-0.5.3/assessment_episode_matcher/tests/matching_test.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.5.2/assessment_episode_matcher/utils/base.py` & `assessment_episode_matcher-0.5.3/assessment_episode_matcher/utils/base.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.5.2/assessment_episode_matcher/utils/ccare_to_aztable.py` & `assessment_episode_matcher-0.5.3/assessment_episode_matcher/utils/ccare_to_aztable.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.5.2/assessment_episode_matcher/utils/df_ops_base.py` & `assessment_episode_matcher-0.5.3/assessment_episode_matcher/utils/df_ops_base.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.5.2/assessment_episode_matcher/utils/dtypes.py` & `assessment_episode_matcher-0.5.3/assessment_episode_matcher/utils/dtypes.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.5.2/assessment_episode_matcher/utils/environment.py` & `assessment_episode_matcher-0.5.3/assessment_episode_matcher/utils/environment.py`

 * *Files 27% similar despite different names*

```diff
@@ -25,20 +25,16 @@
             # cls._instance.env = 'local'
         return cls._instance
   
     @classmethod
     def setup(cls, root, env:str):
         cls.env = env
         env_file = f'{root}/.env.{cls.env}'
-        if not os.path.isfile(env_file):
-            raise FileNotFoundError(f"Environment file {env_file} not found.")
-            
-        # load_dotenv: does not override existing environment variables by default.
-        # It only sets environment variables that are not already defined.
-        load_dotenv(env_file)
+        if  os.path.isfile(env_file):
+            load_dotenv(env_file)
 
         cls.env_config = {key: value for key, value in os.environ.items()}
         
     @property
     def config(self):
         return self.env_config        
     # @classmethod
```

### Comparing `assessment_episode_matcher-0.5.2/assessment_episode_matcher/utils/fromstr.py` & `assessment_episode_matcher-0.5.3/assessment_episode_matcher/utils/fromstr.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 import logging
 import json
 from datetime import datetime, date
+import difflib
+from typing import Optional
+
+
+def find_closest_match(slk: str, slks: list[str], pc_match: float) -> Optional[str]:
+    closest_match = difflib.get_close_matches(slk, slks, n=1, cutoff=pc_match)
+    return closest_match[0] if closest_match else None
+
+
 # import numpy as np
 
 # def convert_format_datestr(date_string:str, from_format:str, to_format:str) -> tuple[str, date]:
 #   date_dt = datetime.strptime(date_string, from_format)
 #   date1 = date_dt.strftime(to_format)
 #   return date1, date_dt.date()
```

### Comparing `assessment_episode_matcher-0.5.2/assessment_episode_matcher/utils/group_utils.py` & `assessment_episode_matcher-0.5.3/assessment_episode_matcher/utils/group_utils.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.5.2/assessment_episode_matcher/utils/io.py` & `assessment_episode_matcher-0.5.3/assessment_episode_matcher/utils/io.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.5.2/assessment_episode_matcher.egg-info/PKG-INFO` & `assessment_episode_matcher-0.5.3/assessment_episode_matcher.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assessment_episode_matcher
-Version: 0.5.2
+Version: 0.5.3
 Author: Aftab Jalal
 Author-email: mj@auditlytics.nz
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `assessment_episode_matcher-0.5.2/assessment_episode_matcher.egg-info/SOURCES.txt` & `assessment_episode_matcher-0.5.3/assessment_episode_matcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.5.2/setup.py` & `assessment_episode_matcher-0.5.3/setup.py`

 * *Files identical despite different names*

