# Comparing `tmp/autosubmit_api-4.0.0b7.tar.gz` & `tmp/autosubmit_api-4.0.0b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autosubmit_api-4.0.0b7.tar", last modified: Tue May 14 10:51:10 2024, max compression
+gzip compressed data, was "autosubmit_api-4.0.0b8.tar", last modified: Tue May 28 12:52:10 2024, max compression
```

## Comparing `autosubmit_api-4.0.0b7.tar` & `autosubmit_api-4.0.0b8.tar`

### file list

```diff
@@ -1,159 +1,159 @@
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.443341 autosubmit_api-4.0.0b7/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    35147 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b7/LICENSE
--rw-r--r--   0 ltenorio  (1001) ltenorio  (1001)     4875 2024-05-14 10:51:10.443341 autosubmit_api-4.0.0b7/PKG-INFO
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2504 2024-05-13 14:08:18.000000 autosubmit_api-4.0.0b7/README.md
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.427341 autosubmit_api-4.0.0b7/autosubmit_api/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      910 2024-05-14 10:48:56.000000 autosubmit_api-4.0.0b7/autosubmit_api/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2542 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/app.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.427341 autosubmit_api-4.0.0b7/autosubmit_api/auth/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2343 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b7/autosubmit_api/auth/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      293 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b7/autosubmit_api/auth/utils.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.427341 autosubmit_api-4.0.0b7/autosubmit_api/autosubmit_legacy/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b7/autosubmit_api/autosubmit_legacy/__init__.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.427341 autosubmit_api-4.0.0b7/autosubmit_api/autosubmit_legacy/job/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b7/autosubmit_api/autosubmit_legacy/job/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    43697 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/autosubmit_legacy/job/job_list.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    12421 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/autosubmit_legacy/job/job_utils.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.431341 autosubmit_api-4.0.0b7/autosubmit_api/bgtasks/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b7/autosubmit_api/bgtasks/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1632 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b7/autosubmit_api/bgtasks/bgtask.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1232 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b7/autosubmit_api/bgtasks/scheduler.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.431341 autosubmit_api-4.0.0b7/autosubmit_api/bgtasks/tasks/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b7/autosubmit_api/bgtasks/tasks/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     5243 2024-05-14 10:48:56.000000 autosubmit_api-4.0.0b7/autosubmit_api/bgtasks/tasks/status_updater.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.431341 autosubmit_api-4.0.0b7/autosubmit_api/blueprints/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b7/autosubmit_api/blueprints/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3008 2024-05-10 14:13:19.000000 autosubmit_api-4.0.0b7/autosubmit_api/blueprints/v3.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3381 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/blueprints/v4.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.431341 autosubmit_api-4.0.0b7/autosubmit_api/builders/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      468 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b7/autosubmit_api/builders/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      570 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b7/autosubmit_api/builders/basic_builder.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2652 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/builders/configuration_facade_builder.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3038 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/builders/experiment_builder.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3142 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/builders/experiment_history_builder.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2626 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/builders/joblist_helper_builder.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1521 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/builders/joblist_loader_builder.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2194 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/builders/pkl_organizer_builder.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3485 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b7/autosubmit_api/cli.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.431341 autosubmit_api-4.0.0b7/autosubmit_api/common/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b7/autosubmit_api/common/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     7779 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b7/autosubmit_api/common/utils.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      596 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b7/autosubmit_api/common/utils_for_testing.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.431341 autosubmit_api-4.0.0b7/autosubmit_api/components/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b7/autosubmit_api/components/__init__.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.431341 autosubmit_api-4.0.0b7/autosubmit_api/components/experiment/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b7/autosubmit_api/components/experiment/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    11007 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/components/experiment/configuration_facade.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     5840 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/components/experiment/pkl_organizer.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     4072 2024-05-03 14:10:04.000000 autosubmit_api-4.0.0b7/autosubmit_api/components/experiment/test.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.431341 autosubmit_api-4.0.0b7/autosubmit_api/components/jobs/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b7/autosubmit_api/components/jobs/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    12790 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/components/jobs/job_factory.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3127 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/components/jobs/job_support.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3902 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/components/jobs/joblist_helper.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     8695 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/components/jobs/joblist_loader.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     9703 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/components/jobs/utils.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.431341 autosubmit_api-4.0.0b7/autosubmit_api/components/representations/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b7/autosubmit_api/components/representations/__init__.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.431341 autosubmit_api-4.0.0b7/autosubmit_api/components/representations/graph/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b7/autosubmit_api/components/representations/graph/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1321 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/components/representations/graph/edge.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    17188 2024-05-13 14:08:18.000000 autosubmit_api-4.0.0b7/autosubmit_api/components/representations/graph/graph.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     6951 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/components/representations/graph/test.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.435341 autosubmit_api-4.0.0b7/autosubmit_api/components/representations/tree/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b7/autosubmit_api/components/representations/tree/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2688 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/components/representations/tree/test.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    13728 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/components/representations/tree/tree.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.435341 autosubmit_api-4.0.0b7/autosubmit_api/config/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    19521 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/config/IConfigStrategy.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1345 2024-03-18 14:29:27.000000 autosubmit_api-4.0.0b7/autosubmit_api/config/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3507 2024-05-13 14:08:18.000000 autosubmit_api-4.0.0b7/autosubmit_api/config/basicConfig.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    49166 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/config/confConfigStrategy.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    24148 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/config/config_common.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    14118 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b7/autosubmit_api/config/ymlConfigStrategy.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.435341 autosubmit_api-4.0.0b7/autosubmit_api/database/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      772 2024-05-13 14:08:18.000000 autosubmit_api-4.0.0b7/autosubmit_api/database/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2798 2024-05-14 10:48:56.000000 autosubmit_api-4.0.0b7/autosubmit_api/database/common.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    20480 2024-05-14 10:48:56.000000 autosubmit_api-4.0.0b7/autosubmit_api/database/db_common.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    45645 2024-05-13 14:08:18.000000 autosubmit_api-4.0.0b7/autosubmit_api/database/db_jobdata.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     9115 2024-04-11 13:47:25.000000 autosubmit_api-4.0.0b7/autosubmit_api/database/db_manager.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3627 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/database/db_structure.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1128 2024-03-18 14:29:27.000000 autosubmit_api-4.0.0b7/autosubmit_api/database/models.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2645 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/database/queries.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3491 2024-05-02 14:40:09.000000 autosubmit_api-4.0.0b7/autosubmit_api/database/tables.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      461 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b7/autosubmit_api/database/utils.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.435341 autosubmit_api-4.0.0b7/autosubmit_api/experiment/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b7/autosubmit_api/experiment/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     4016 2024-05-14 10:48:56.000000 autosubmit_api-4.0.0b7/autosubmit_api/experiment/common_db_requests.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    52845 2024-05-14 10:48:56.000000 autosubmit_api-4.0.0b7/autosubmit_api/experiment/common_requests.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      647 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b7/autosubmit_api/experiment/utils.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.435341 autosubmit_api-4.0.0b7/autosubmit_api/history/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b7/autosubmit_api/history/__init__.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.435341 autosubmit_api-4.0.0b7/autosubmit_api/history/data_classes/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b7/autosubmit_api/history/data_classes/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     7563 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/history/data_classes/experiment_run.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    11544 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/history/data_classes/job_data.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.435341 autosubmit_api-4.0.0b7/autosubmit_api/history/database_managers/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b7/autosubmit_api/history/database_managers/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     5829 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/history/database_managers/database_manager.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     5197 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b7/autosubmit_api/history/database_managers/database_models.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    23141 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/history/database_managers/experiment_history_db_manager.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     6124 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/history/experiment_history.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2041 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/history/internal_logging.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3090 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/history/utils.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1606 2024-04-25 14:05:26.000000 autosubmit_api-4.0.0b7/autosubmit_api/logger.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.435341 autosubmit_api-4.0.0b7/autosubmit_api/monitor/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b7/autosubmit_api/monitor/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     9896 2024-04-26 14:40:27.000000 autosubmit_api-4.0.0b7/autosubmit_api/monitor/monitor.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.439341 autosubmit_api-4.0.0b7/autosubmit_api/performance/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b7/autosubmit_api/performance/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     8010 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/performance/performance_metrics.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1081 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b7/autosubmit_api/performance/utils.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.439341 autosubmit_api-4.0.0b7/autosubmit_api/persistance/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b7/autosubmit_api/persistance/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1688 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b7/autosubmit_api/persistance/experiment.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3743 2024-04-19 11:53:24.000000 autosubmit_api-4.0.0b7/autosubmit_api/persistance/job_package_reader.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2287 2024-03-18 14:29:27.000000 autosubmit_api-4.0.0b7/autosubmit_api/persistance/pkl_reader.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.439341 autosubmit_api-4.0.0b7/autosubmit_api/statistics/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b7/autosubmit_api/statistics/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2791 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/statistics/job_stat.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     6956 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/statistics/statistics.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2565 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b7/autosubmit_api/statistics/stats_summary.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      177 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/statistics/utils.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.439341 autosubmit_api-4.0.0b7/autosubmit_api/views/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      476 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b7/autosubmit_api/views/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    13529 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/autosubmit_api/views/v3.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    15492 2024-04-19 11:53:24.000000 autosubmit_api-4.0.0b7/autosubmit_api/views/v4.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.439341 autosubmit_api-4.0.0b7/autosubmit_api/workers/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b7/autosubmit_api/workers/__init__.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.439341 autosubmit_api-4.0.0b7/autosubmit_api/workers/business/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b7/autosubmit_api/workers/business/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3010 2024-05-13 14:08:18.000000 autosubmit_api-4.0.0b7/autosubmit_api/workers/business/process_graph_drawings.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.439341 autosubmit_api-4.0.0b7/autosubmit_api/workers/populate_details/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b7/autosubmit_api/workers/populate_details/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     4279 2024-05-06 11:38:15.000000 autosubmit_api-4.0.0b7/autosubmit_api/workers/populate_details/populate.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      135 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b7/autosubmit_api/workers/populate_details_db.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      218 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b7/autosubmit_api/workers/populate_graph.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      269 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b7/autosubmit_api/workers/populate_running_experiments.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      158 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b7/autosubmit_api/workers/test_esarchive.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.439341 autosubmit_api-4.0.0b7/autosubmit_api.egg-info/
--rw-r--r--   0 ltenorio  (1001) ltenorio  (1001)     4875 2024-05-14 10:51:10.000000 autosubmit_api-4.0.0b7/autosubmit_api.egg-info/PKG-INFO
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     4991 2024-05-14 10:51:10.000000 autosubmit_api-4.0.0b7/autosubmit_api.egg-info/SOURCES.txt
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        1 2024-05-14 10:51:10.000000 autosubmit_api-4.0.0b7/autosubmit_api.egg-info/dependency_links.txt
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)       59 2024-05-14 10:51:10.000000 autosubmit_api-4.0.0b7/autosubmit_api.egg-info/entry_points.txt
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      665 2024-05-14 10:51:10.000000 autosubmit_api-4.0.0b7/autosubmit_api.egg-info/requires.txt
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)       21 2024-05-14 10:51:10.000000 autosubmit_api-4.0.0b7/autosubmit_api.egg-info/top_level.txt
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)       38 2024-05-14 10:51:10.443341 autosubmit_api-4.0.0b7/setup.cfg
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2142 2024-05-14 10:48:56.000000 autosubmit_api-4.0.0b7/setup.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-14 10:51:10.439341 autosubmit_api-4.0.0b7/tests/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b7/tests/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1337 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b7/tests/conftest.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      228 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b7/tests/custom_utils.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3377 2024-05-10 13:22:59.000000 autosubmit_api-4.0.0b7/tests/test_auth.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      714 2024-03-18 14:29:27.000000 autosubmit_api-4.0.0b7/tests/test_bg_tasks.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2871 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b7/tests/test_config.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      773 2024-05-14 10:48:56.000000 autosubmit_api-4.0.0b7/tests/test_database.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    20138 2024-05-13 15:01:30.000000 autosubmit_api-4.0.0b7/tests/test_endpoints_v3.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     6473 2024-04-19 11:53:24.000000 autosubmit_api-4.0.0b7/tests/test_endpoints_v4.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2504 2024-05-13 14:08:18.000000 autosubmit_api-4.0.0b7/tests/test_graph.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      531 2024-03-18 14:29:27.000000 autosubmit_api-4.0.0b7/tests/test_persistance.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-28 12:52:10.134307 autosubmit_api-4.0.0b8/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    35147 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b8/LICENSE
+-rw-r--r--   0 ltenorio  (1001) ltenorio  (1001)     4875 2024-05-28 12:52:10.134307 autosubmit_api-4.0.0b8/PKG-INFO
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2504 2024-05-16 12:30:28.000000 autosubmit_api-4.0.0b8/README.md
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-28 12:52:10.126307 autosubmit_api-4.0.0b8/autosubmit_api/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      910 2024-05-28 12:50:40.000000 autosubmit_api-4.0.0b8/autosubmit_api/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2542 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b8/autosubmit_api/app.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-28 12:52:10.126307 autosubmit_api-4.0.0b8/autosubmit_api/auth/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2343 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b8/autosubmit_api/auth/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      293 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b8/autosubmit_api/auth/utils.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-28 12:52:10.126307 autosubmit_api-4.0.0b8/autosubmit_api/autosubmit_legacy/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b8/autosubmit_api/autosubmit_legacy/__init__.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-28 12:52:10.126307 autosubmit_api-4.0.0b8/autosubmit_api/autosubmit_legacy/job/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b8/autosubmit_api/autosubmit_legacy/job/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    43809 2024-05-28 12:50:40.000000 autosubmit_api-4.0.0b8/autosubmit_api/autosubmit_legacy/job/job_list.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    12421 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b8/autosubmit_api/autosubmit_legacy/job/job_utils.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-28 12:52:10.126307 autosubmit_api-4.0.0b8/autosubmit_api/bgtasks/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b8/autosubmit_api/bgtasks/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1632 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b8/autosubmit_api/bgtasks/bgtask.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1232 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b8/autosubmit_api/bgtasks/scheduler.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-28 12:52:10.126307 autosubmit_api-4.0.0b8/autosubmit_api/bgtasks/tasks/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b8/autosubmit_api/bgtasks/tasks/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     5243 2024-05-28 12:49:24.000000 autosubmit_api-4.0.0b8/autosubmit_api/bgtasks/tasks/status_updater.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-28 12:52:10.130307 autosubmit_api-4.0.0b8/autosubmit_api/blueprints/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b8/autosubmit_api/blueprints/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3008 2024-05-15 12:29:37.000000 autosubmit_api-4.0.0b8/autosubmit_api/blueprints/v3.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3381 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b8/autosubmit_api/blueprints/v4.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-28 12:52:10.130307 autosubmit_api-4.0.0b8/autosubmit_api/builders/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      468 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b8/autosubmit_api/builders/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      570 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b8/autosubmit_api/builders/basic_builder.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2652 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b8/autosubmit_api/builders/configuration_facade_builder.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3038 2024-05-28 12:49:24.000000 autosubmit_api-4.0.0b8/autosubmit_api/builders/experiment_builder.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3282 2024-05-28 12:50:40.000000 autosubmit_api-4.0.0b8/autosubmit_api/builders/experiment_history_builder.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2626 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b8/autosubmit_api/builders/joblist_helper_builder.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1521 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b8/autosubmit_api/builders/joblist_loader_builder.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2194 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b8/autosubmit_api/builders/pkl_organizer_builder.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3485 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b8/autosubmit_api/cli.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-28 12:52:10.130307 autosubmit_api-4.0.0b8/autosubmit_api/common/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b8/autosubmit_api/common/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     7779 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b8/autosubmit_api/common/utils.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      596 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b8/autosubmit_api/common/utils_for_testing.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-28 12:52:10.130307 autosubmit_api-4.0.0b8/autosubmit_api/components/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b8/autosubmit_api/components/__init__.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-28 12:52:10.130307 autosubmit_api-4.0.0b8/autosubmit_api/components/experiment/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b8/autosubmit_api/components/experiment/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    11007 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b8/autosubmit_api/components/experiment/configuration_facade.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     5840 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b8/autosubmit_api/components/experiment/pkl_organizer.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     4072 2024-05-03 14:10:04.000000 autosubmit_api-4.0.0b8/autosubmit_api/components/experiment/test.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-28 12:52:10.130307 autosubmit_api-4.0.0b8/autosubmit_api/components/jobs/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b8/autosubmit_api/components/jobs/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    12790 2024-05-15 13:17:02.000000 autosubmit_api-4.0.0b8/autosubmit_api/components/jobs/job_factory.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3127 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b8/autosubmit_api/components/jobs/job_support.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3902 2024-05-28 12:49:24.000000 autosubmit_api-4.0.0b8/autosubmit_api/components/jobs/joblist_helper.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     8695 2024-05-28 12:49:24.000000 autosubmit_api-4.0.0b8/autosubmit_api/components/jobs/joblist_loader.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     9703 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b8/autosubmit_api/components/jobs/utils.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-28 12:52:10.130307 autosubmit_api-4.0.0b8/autosubmit_api/components/representations/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b8/autosubmit_api/components/representations/__init__.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-28 12:52:10.130307 autosubmit_api-4.0.0b8/autosubmit_api/components/representations/graph/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b8/autosubmit_api/components/representations/graph/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1321 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b8/autosubmit_api/components/representations/graph/edge.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    17188 2024-05-28 12:49:24.000000 autosubmit_api-4.0.0b8/autosubmit_api/components/representations/graph/graph.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     6951 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b8/autosubmit_api/components/representations/graph/test.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-28 12:52:10.130307 autosubmit_api-4.0.0b8/autosubmit_api/components/representations/tree/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b8/autosubmit_api/components/representations/tree/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2688 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b8/autosubmit_api/components/representations/tree/test.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    13728 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b8/autosubmit_api/components/representations/tree/tree.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-28 12:52:10.130307 autosubmit_api-4.0.0b8/autosubmit_api/config/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    19521 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b8/autosubmit_api/config/IConfigStrategy.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1345 2024-03-18 14:29:27.000000 autosubmit_api-4.0.0b8/autosubmit_api/config/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3507 2024-05-28 12:49:24.000000 autosubmit_api-4.0.0b8/autosubmit_api/config/basicConfig.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    49166 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b8/autosubmit_api/config/confConfigStrategy.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    24148 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b8/autosubmit_api/config/config_common.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    14118 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b8/autosubmit_api/config/ymlConfigStrategy.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-28 12:52:10.130307 autosubmit_api-4.0.0b8/autosubmit_api/database/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      772 2024-05-28 12:49:24.000000 autosubmit_api-4.0.0b8/autosubmit_api/database/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2798 2024-05-28 12:49:24.000000 autosubmit_api-4.0.0b8/autosubmit_api/database/common.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    20480 2024-05-28 12:49:24.000000 autosubmit_api-4.0.0b8/autosubmit_api/database/db_common.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    45680 2024-05-28 12:50:40.000000 autosubmit_api-4.0.0b8/autosubmit_api/database/db_jobdata.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     9115 2024-05-28 12:49:24.000000 autosubmit_api-4.0.0b8/autosubmit_api/database/db_manager.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3627 2024-05-28 12:49:24.000000 autosubmit_api-4.0.0b8/autosubmit_api/database/db_structure.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1128 2024-03-18 14:29:27.000000 autosubmit_api-4.0.0b8/autosubmit_api/database/models.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2645 2024-05-28 12:49:24.000000 autosubmit_api-4.0.0b8/autosubmit_api/database/queries.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3491 2024-05-28 12:49:24.000000 autosubmit_api-4.0.0b8/autosubmit_api/database/tables.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      461 2024-05-28 12:49:24.000000 autosubmit_api-4.0.0b8/autosubmit_api/database/utils.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-28 12:52:10.130307 autosubmit_api-4.0.0b8/autosubmit_api/experiment/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b8/autosubmit_api/experiment/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     4016 2024-05-28 12:49:24.000000 autosubmit_api-4.0.0b8/autosubmit_api/experiment/common_db_requests.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    53051 2024-05-28 12:50:40.000000 autosubmit_api-4.0.0b8/autosubmit_api/experiment/common_requests.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      647 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b8/autosubmit_api/experiment/utils.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-28 12:52:10.130307 autosubmit_api-4.0.0b8/autosubmit_api/history/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b8/autosubmit_api/history/__init__.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-28 12:52:10.130307 autosubmit_api-4.0.0b8/autosubmit_api/history/data_classes/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b8/autosubmit_api/history/data_classes/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     7563 2024-05-28 12:49:24.000000 autosubmit_api-4.0.0b8/autosubmit_api/history/data_classes/experiment_run.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    11544 2024-05-28 12:49:24.000000 autosubmit_api-4.0.0b8/autosubmit_api/history/data_classes/job_data.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-28 12:52:10.130307 autosubmit_api-4.0.0b8/autosubmit_api/history/database_managers/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b8/autosubmit_api/history/database_managers/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     5829 2024-05-28 12:49:24.000000 autosubmit_api-4.0.0b8/autosubmit_api/history/database_managers/database_manager.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     5197 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b8/autosubmit_api/history/database_managers/database_models.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    23141 2024-05-28 12:49:24.000000 autosubmit_api-4.0.0b8/autosubmit_api/history/database_managers/experiment_history_db_manager.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     6124 2024-05-28 12:49:24.000000 autosubmit_api-4.0.0b8/autosubmit_api/history/experiment_history.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2041 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b8/autosubmit_api/history/internal_logging.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3090 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b8/autosubmit_api/history/utils.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1606 2024-04-25 14:05:26.000000 autosubmit_api-4.0.0b8/autosubmit_api/logger.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-28 12:52:10.130307 autosubmit_api-4.0.0b8/autosubmit_api/monitor/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b8/autosubmit_api/monitor/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     9896 2024-04-26 14:40:27.000000 autosubmit_api-4.0.0b8/autosubmit_api/monitor/monitor.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-28 12:52:10.130307 autosubmit_api-4.0.0b8/autosubmit_api/performance/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b8/autosubmit_api/performance/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     8010 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b8/autosubmit_api/performance/performance_metrics.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1081 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b8/autosubmit_api/performance/utils.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-28 12:52:10.130307 autosubmit_api-4.0.0b8/autosubmit_api/persistance/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b8/autosubmit_api/persistance/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1688 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b8/autosubmit_api/persistance/experiment.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3743 2024-05-28 12:49:24.000000 autosubmit_api-4.0.0b8/autosubmit_api/persistance/job_package_reader.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2287 2024-03-18 14:29:27.000000 autosubmit_api-4.0.0b8/autosubmit_api/persistance/pkl_reader.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-28 12:52:10.130307 autosubmit_api-4.0.0b8/autosubmit_api/statistics/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b8/autosubmit_api/statistics/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2791 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b8/autosubmit_api/statistics/job_stat.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     6956 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b8/autosubmit_api/statistics/statistics.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2565 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b8/autosubmit_api/statistics/stats_summary.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      177 2024-05-13 13:39:21.000000 autosubmit_api-4.0.0b8/autosubmit_api/statistics/utils.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-28 12:52:10.130307 autosubmit_api-4.0.0b8/autosubmit_api/views/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      476 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b8/autosubmit_api/views/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    13529 2024-05-28 12:49:24.000000 autosubmit_api-4.0.0b8/autosubmit_api/views/v3.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    15492 2024-05-28 12:49:24.000000 autosubmit_api-4.0.0b8/autosubmit_api/views/v4.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-28 12:52:10.130307 autosubmit_api-4.0.0b8/autosubmit_api/workers/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b8/autosubmit_api/workers/__init__.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-28 12:52:10.130307 autosubmit_api-4.0.0b8/autosubmit_api/workers/business/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b8/autosubmit_api/workers/business/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3010 2024-05-28 12:49:24.000000 autosubmit_api-4.0.0b8/autosubmit_api/workers/business/process_graph_drawings.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-28 12:52:10.134307 autosubmit_api-4.0.0b8/autosubmit_api/workers/populate_details/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b8/autosubmit_api/workers/populate_details/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     4279 2024-05-28 12:49:24.000000 autosubmit_api-4.0.0b8/autosubmit_api/workers/populate_details/populate.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      135 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b8/autosubmit_api/workers/populate_details_db.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      218 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b8/autosubmit_api/workers/populate_graph.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      269 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b8/autosubmit_api/workers/populate_running_experiments.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      158 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b8/autosubmit_api/workers/test_esarchive.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-28 12:52:10.134307 autosubmit_api-4.0.0b8/autosubmit_api.egg-info/
+-rw-r--r--   0 ltenorio  (1001) ltenorio  (1001)     4875 2024-05-28 12:52:10.000000 autosubmit_api-4.0.0b8/autosubmit_api.egg-info/PKG-INFO
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     4991 2024-05-28 12:52:10.000000 autosubmit_api-4.0.0b8/autosubmit_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        1 2024-05-28 12:52:10.000000 autosubmit_api-4.0.0b8/autosubmit_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)       59 2024-05-28 12:52:10.000000 autosubmit_api-4.0.0b8/autosubmit_api.egg-info/entry_points.txt
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      665 2024-05-28 12:52:10.000000 autosubmit_api-4.0.0b8/autosubmit_api.egg-info/requires.txt
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)       21 2024-05-28 12:52:10.000000 autosubmit_api-4.0.0b8/autosubmit_api.egg-info/top_level.txt
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)       38 2024-05-28 12:52:10.134307 autosubmit_api-4.0.0b8/setup.cfg
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2142 2024-05-28 12:49:24.000000 autosubmit_api-4.0.0b8/setup.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-05-28 12:52:10.134307 autosubmit_api-4.0.0b8/tests/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b8/tests/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1337 2024-05-28 12:49:24.000000 autosubmit_api-4.0.0b8/tests/conftest.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      228 2024-05-28 12:49:24.000000 autosubmit_api-4.0.0b8/tests/custom_utils.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3377 2024-05-28 12:49:24.000000 autosubmit_api-4.0.0b8/tests/test_auth.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      714 2024-05-28 12:49:24.000000 autosubmit_api-4.0.0b8/tests/test_bg_tasks.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2871 2024-05-28 12:49:24.000000 autosubmit_api-4.0.0b8/tests/test_config.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      773 2024-05-28 12:49:24.000000 autosubmit_api-4.0.0b8/tests/test_database.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    20138 2024-05-28 12:49:24.000000 autosubmit_api-4.0.0b8/tests/test_endpoints_v3.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     6473 2024-05-28 12:49:24.000000 autosubmit_api-4.0.0b8/tests/test_endpoints_v4.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2504 2024-05-28 12:49:24.000000 autosubmit_api-4.0.0b8/tests/test_graph.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      531 2024-03-18 14:29:27.000000 autosubmit_api-4.0.0b8/tests/test_persistance.py
```

### Comparing `autosubmit_api-4.0.0b7/LICENSE` & `autosubmit_api-4.0.0b8/LICENSE`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/PKG-INFO` & `autosubmit_api-4.0.0b8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosubmit_api
-Version: 4.0.0b7
+Version: 4.0.0b8
 Summary: An extension to the Autosubmit package that serves its information as an API
 Home-page: https://earth.bsc.es/gitlab/es/autosubmit_api
 Author: Luiggi Tenorio, Bruno P. Kinoshita, Cristian Gutiérrez, Julian Berlin, Wilmer Uruchi
 Author-email: support-autosubmit@bsc.es
 License: GNU GPL
 Keywords: autosubmit,API
 Classifier: Development Status :: 4 - Beta
```

### Comparing `autosubmit_api-4.0.0b7/README.md` & `autosubmit_api-4.0.0b8/README.md`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/__init__.py` & `autosubmit_api-4.0.0b8/autosubmit_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,10 +13,10 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with Autosubmit.  If not, see <http://www.gnu.org/licenses/>.
 
-__version__ = "4.0.0b7"
+__version__ = "4.0.0b8"
 __author__ = "Luiggi Tenorio, Bruno P. Kinoshita, Cristian Gutiérrez, Julian Berlin, Wilmer Uruchi"
 __credits__ = "Barcelona Supercomputing Center"
```

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/app.py` & `autosubmit_api-4.0.0b8/autosubmit_api/app.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/auth/__init__.py` & `autosubmit_api-4.0.0b8/autosubmit_api/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/autosubmit_legacy/job/job_list.py` & `autosubmit_api-4.0.0b8/autosubmit_api/autosubmit_legacy/job/job_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -585,16 +585,20 @@
         """
         # Getting information
         path_local_root = basic_config.LOCAL_ROOT_DIR
         path_structure = basic_config.STRUCTURES_DIR
         db_file = os.path.join(path_local_root, basic_config.DB_FILE)
         # Job information from job historic data
         # print("Get current job data structure...")
-        experiment_history = ExperimentHistoryDirector(ExperimentHistoryBuilder(expid)).build_reader_experiment_history()
-        job_data = experiment_history.manager.get_all_last_job_data_dcs() if experiment_history.is_header_ready() else None
+        job_data = None
+        try:
+            experiment_history = ExperimentHistoryDirector(ExperimentHistoryBuilder(expid)).build_reader_experiment_history()
+            job_data = experiment_history.manager.get_all_last_job_data_dcs() if experiment_history.is_header_ready() else None
+        except Exception:
+            print(traceback.print_exc())
         # Result variables
         job_running_time_seconds = dict()
         job_running_to_runtext = dict()
         result = dict()
         current_table_structure = dict()
         job_name_to_job_info = dict()
         # Work variables
```

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/autosubmit_legacy/job/job_utils.py` & `autosubmit_api-4.0.0b8/autosubmit_api/autosubmit_legacy/job/job_utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/bgtasks/bgtask.py` & `autosubmit_api-4.0.0b8/autosubmit_api/bgtasks/bgtask.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/bgtasks/scheduler.py` & `autosubmit_api-4.0.0b8/autosubmit_api/bgtasks/scheduler.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/bgtasks/tasks/status_updater.py` & `autosubmit_api-4.0.0b8/autosubmit_api/bgtasks/tasks/status_updater.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/blueprints/v3.py` & `autosubmit_api-4.0.0b8/autosubmit_api/blueprints/v3.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/blueprints/v4.py` & `autosubmit_api-4.0.0b8/autosubmit_api/blueprints/v4.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/builders/basic_builder.py` & `autosubmit_api-4.0.0b8/autosubmit_api/builders/basic_builder.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/builders/configuration_facade_builder.py` & `autosubmit_api-4.0.0b8/autosubmit_api/builders/configuration_facade_builder.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/builders/experiment_builder.py` & `autosubmit_api-4.0.0b8/autosubmit_api/builders/experiment_builder.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/builders/experiment_history_builder.py` & `autosubmit_api-4.0.0b8/autosubmit_api/builders/experiment_history_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,17 @@
     self.logger = Logging(self.expid, self.basic_config)
 
   def make_experiment_history(self):
     # type: () -> ExperimentHistory
     self._validate_basic_config()
     if not self.experiment_history_db_manager:
       raise Exception("Experiment Database Manager is missing")
+    else:
+      if not self.experiment_history_db_manager.my_database_exists():
+        raise Exception("Job/Runs database does not exist")
     if not self.logger:
       raise Exception("Logging is missing.")
     return ExperimentHistory(self.expid, self.basic_config, self.experiment_history_db_manager, self.logger)
 
 class ExperimentHistoryDirector(object):
   def __init__(self, builder):
     # type: (Builder) -> None
```

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/builders/joblist_helper_builder.py` & `autosubmit_api-4.0.0b8/autosubmit_api/builders/joblist_helper_builder.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/builders/joblist_loader_builder.py` & `autosubmit_api-4.0.0b8/autosubmit_api/builders/joblist_loader_builder.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/builders/pkl_organizer_builder.py` & `autosubmit_api-4.0.0b8/autosubmit_api/builders/pkl_organizer_builder.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/cli.py` & `autosubmit_api-4.0.0b8/autosubmit_api/cli.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/common/utils.py` & `autosubmit_api-4.0.0b8/autosubmit_api/common/utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/common/utils_for_testing.py` & `autosubmit_api-4.0.0b8/autosubmit_api/common/utils_for_testing.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/components/experiment/configuration_facade.py` & `autosubmit_api-4.0.0b8/autosubmit_api/components/experiment/configuration_facade.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/components/experiment/pkl_organizer.py` & `autosubmit_api-4.0.0b8/autosubmit_api/components/experiment/pkl_organizer.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/components/experiment/test.py` & `autosubmit_api-4.0.0b8/autosubmit_api/components/experiment/test.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/components/jobs/job_factory.py` & `autosubmit_api-4.0.0b8/autosubmit_api/components/jobs/job_factory.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/components/jobs/job_support.py` & `autosubmit_api-4.0.0b8/autosubmit_api/components/jobs/job_support.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/components/jobs/joblist_helper.py` & `autosubmit_api-4.0.0b8/autosubmit_api/components/jobs/joblist_helper.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/components/jobs/joblist_loader.py` & `autosubmit_api-4.0.0b8/autosubmit_api/components/jobs/joblist_loader.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/components/jobs/utils.py` & `autosubmit_api-4.0.0b8/autosubmit_api/components/jobs/utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/components/representations/graph/edge.py` & `autosubmit_api-4.0.0b8/autosubmit_api/components/representations/graph/edge.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/components/representations/graph/graph.py` & `autosubmit_api-4.0.0b8/autosubmit_api/components/representations/graph/graph.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/components/representations/graph/test.py` & `autosubmit_api-4.0.0b8/autosubmit_api/components/representations/graph/test.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/components/representations/tree/test.py` & `autosubmit_api-4.0.0b8/autosubmit_api/components/representations/tree/test.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/components/representations/tree/tree.py` & `autosubmit_api-4.0.0b8/autosubmit_api/components/representations/tree/tree.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/config/IConfigStrategy.py` & `autosubmit_api-4.0.0b8/autosubmit_api/config/IConfigStrategy.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/config/__init__.py` & `autosubmit_api-4.0.0b8/autosubmit_api/config/__init__.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/config/basicConfig.py` & `autosubmit_api-4.0.0b8/autosubmit_api/config/basicConfig.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/config/confConfigStrategy.py` & `autosubmit_api-4.0.0b8/autosubmit_api/config/confConfigStrategy.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/config/config_common.py` & `autosubmit_api-4.0.0b8/autosubmit_api/config/config_common.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/config/ymlConfigStrategy.py` & `autosubmit_api-4.0.0b8/autosubmit_api/config/ymlConfigStrategy.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/database/__init__.py` & `autosubmit_api-4.0.0b8/autosubmit_api/database/__init__.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/database/common.py` & `autosubmit_api-4.0.0b8/autosubmit_api/database/common.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/database/db_common.py` & `autosubmit_api-4.0.0b8/autosubmit_api/database/db_common.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/database/db_jobdata.py` & `autosubmit_api-4.0.0b8/autosubmit_api/database/db_jobdata.py`

 * *Files 0% similar despite different names*

```diff
@@ -486,14 +486,15 @@
         :param create_table_sql: a CREATE TABLE statement
         :return:
         """
         try:
             if self.conn:
                 c = self.conn.cursor()
                 c.execute(self.create_table_query)
+                self.conn.commit()
             else:
                 raise IOError("Not a valid connection")
         except IOError as exp:
             Log.warning(exp)
             return None
         except sqlite3.Error as e:
             if _debug == True:
```

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/database/db_manager.py` & `autosubmit_api-4.0.0b8/autosubmit_api/database/db_manager.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/database/db_structure.py` & `autosubmit_api-4.0.0b8/autosubmit_api/database/db_structure.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/database/models.py` & `autosubmit_api-4.0.0b8/autosubmit_api/database/models.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/database/queries.py` & `autosubmit_api-4.0.0b8/autosubmit_api/database/queries.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/database/tables.py` & `autosubmit_api-4.0.0b8/autosubmit_api/database/tables.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/experiment/common_db_requests.py` & `autosubmit_api-4.0.0b8/autosubmit_api/experiment/common_db_requests.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/experiment/common_requests.py` & `autosubmit_api-4.0.0b8/autosubmit_api/experiment/common_requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,24 +168,28 @@
         result["model"] = autosubmit_config_facade.get_model()
         result["branch"] = autosubmit_config_facade.get_branch()
         result["hpc"] = autosubmit_config_facade.get_main_platform()
         result["updateTime"] = autosubmit_config_facade.get_safety_sleep_time()
         result["pkl_timestamp"] = autosubmit_config_facade.get_pkl_last_modified_timestamp()
         result["chunk_size"] = autosubmit_config_facade.chunk_size
         result["chunk_unit"] = autosubmit_config_facade.chunk_unit
-        experiment_history = ExperimentHistoryDirector(ExperimentHistoryBuilder(expid)).build_reader_experiment_history()
-        experiment_run = experiment_history.manager.get_experiment_run_dc_with_max_id()
-        if experiment_run and experiment_run.total > 0:
-            result["total_jobs"] = experiment_run.total
-            result["completed_jobs"] = experiment_run.completed
-            result["db_historic_version"] = experiment_history.manager.db_version
-        else:
-            result["total_jobs"] = 0
-            result["completed_jobs"] = 0
-            result["db_historic_version"] = "NA"
+
+        result["total_jobs"] = 0
+        result["completed_jobs"] = 0
+        result["db_historic_version"] = "NA"
+        try:
+            experiment_history = ExperimentHistoryDirector(ExperimentHistoryBuilder(expid)).build_reader_experiment_history()
+            experiment_run = experiment_history.manager.get_experiment_run_dc_with_max_id()
+            if experiment_run and experiment_run.total > 0:
+                result["total_jobs"] = experiment_run.total
+                result["completed_jobs"] = experiment_run.completed
+                result["db_historic_version"] = experiment_history.manager.db_version
+        except Exception as exc:
+            logger.warning((traceback.format_exc()))
+            logger.warning((f"Warning: Error in get_experiment_data while reading historical data: {exc}"))
 
     except Exception as exp:
         result["error"] = True
         result["error_message"] = str(exp)
         logger.error((traceback.format_exc()))
     return result
```

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/experiment/utils.py` & `autosubmit_api-4.0.0b8/autosubmit_api/experiment/utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/history/data_classes/experiment_run.py` & `autosubmit_api-4.0.0b8/autosubmit_api/history/data_classes/experiment_run.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/history/data_classes/job_data.py` & `autosubmit_api-4.0.0b8/autosubmit_api/history/data_classes/job_data.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/history/database_managers/database_manager.py` & `autosubmit_api-4.0.0b8/autosubmit_api/history/database_managers/database_manager.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/history/database_managers/database_models.py` & `autosubmit_api-4.0.0b8/autosubmit_api/history/database_managers/database_models.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/history/database_managers/experiment_history_db_manager.py` & `autosubmit_api-4.0.0b8/autosubmit_api/history/database_managers/experiment_history_db_manager.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/history/experiment_history.py` & `autosubmit_api-4.0.0b8/autosubmit_api/history/experiment_history.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/history/internal_logging.py` & `autosubmit_api-4.0.0b8/autosubmit_api/history/internal_logging.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/history/utils.py` & `autosubmit_api-4.0.0b8/autosubmit_api/history/utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/logger.py` & `autosubmit_api-4.0.0b8/autosubmit_api/logger.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/monitor/monitor.py` & `autosubmit_api-4.0.0b8/autosubmit_api/monitor/monitor.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/performance/performance_metrics.py` & `autosubmit_api-4.0.0b8/autosubmit_api/performance/performance_metrics.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/performance/utils.py` & `autosubmit_api-4.0.0b8/autosubmit_api/performance/utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/persistance/experiment.py` & `autosubmit_api-4.0.0b8/autosubmit_api/persistance/experiment.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/persistance/job_package_reader.py` & `autosubmit_api-4.0.0b8/autosubmit_api/persistance/job_package_reader.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/persistance/pkl_reader.py` & `autosubmit_api-4.0.0b8/autosubmit_api/persistance/pkl_reader.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/statistics/job_stat.py` & `autosubmit_api-4.0.0b8/autosubmit_api/statistics/job_stat.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/statistics/statistics.py` & `autosubmit_api-4.0.0b8/autosubmit_api/statistics/statistics.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/statistics/stats_summary.py` & `autosubmit_api-4.0.0b8/autosubmit_api/statistics/stats_summary.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/views/v3.py` & `autosubmit_api-4.0.0b8/autosubmit_api/views/v3.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/views/v4.py` & `autosubmit_api-4.0.0b8/autosubmit_api/views/v4.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/workers/business/process_graph_drawings.py` & `autosubmit_api-4.0.0b8/autosubmit_api/workers/business/process_graph_drawings.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api/workers/populate_details/populate.py` & `autosubmit_api-4.0.0b8/autosubmit_api/workers/populate_details/populate.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api.egg-info/PKG-INFO` & `autosubmit_api-4.0.0b8/autosubmit_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosubmit_api
-Version: 4.0.0b7
+Version: 4.0.0b8
 Summary: An extension to the Autosubmit package that serves its information as an API
 Home-page: https://earth.bsc.es/gitlab/es/autosubmit_api
 Author: Luiggi Tenorio, Bruno P. Kinoshita, Cristian Gutiérrez, Julian Berlin, Wilmer Uruchi
 Author-email: support-autosubmit@bsc.es
 License: GNU GPL
 Keywords: autosubmit,API
 Classifier: Development Status :: 4 - Beta
```

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api.egg-info/SOURCES.txt` & `autosubmit_api-4.0.0b8/autosubmit_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/autosubmit_api.egg-info/requires.txt` & `autosubmit_api-4.0.0b8/autosubmit_api.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/setup.py` & `autosubmit_api-4.0.0b8/setup.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/tests/conftest.py` & `autosubmit_api-4.0.0b8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/tests/test_auth.py` & `autosubmit_api-4.0.0b8/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/tests/test_bg_tasks.py` & `autosubmit_api-4.0.0b8/tests/test_bg_tasks.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/tests/test_config.py` & `autosubmit_api-4.0.0b8/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/tests/test_database.py` & `autosubmit_api-4.0.0b8/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/tests/test_endpoints_v3.py` & `autosubmit_api-4.0.0b8/tests/test_endpoints_v3.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/tests/test_endpoints_v4.py` & `autosubmit_api-4.0.0b8/tests/test_endpoints_v4.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/tests/test_graph.py` & `autosubmit_api-4.0.0b8/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b7/tests/test_persistance.py` & `autosubmit_api-4.0.0b8/tests/test_persistance.py`

 * *Files identical despite different names*

