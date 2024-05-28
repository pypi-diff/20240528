# Comparing `tmp/datasphere-0.7.1.tar.gz` & `tmp/datasphere-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasphere-0.7.1.tar", last modified: Mon May 27 14:57:18 2024, max compression
+gzip compressed data, was "datasphere-0.7.2.tar", last modified: Tue May 28 13:24:52 2024, max compression
```

## Comparing `datasphere-0.7.1.tar` & `datasphere-0.7.2.tar`

### file list

```diff
@@ -1,1079 +1,1079 @@
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:18.744279 datasphere-0.7.1/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      771 2024-05-27 14:57:18.743174 datasphere-0.7.1/PKG-INFO
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4245 2024-05-03 11:43:05.000000 datasphere-0.7.1/README.md
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:17.742371 datasphere-0.7.1/datasphere/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)       21 2024-05-22 08:31:30.000000 datasphere-0.7.1/datasphere/__init__.py
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:17.750963 datasphere-0.7.1/datasphere/api/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2570 2024-05-03 11:43:05.000000 datasphere-0.7.1/datasphere/api/__init__.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5426 2024-05-22 08:31:30.000000 datasphere-0.7.1/datasphere/auth.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      853 2024-05-27 14:20:37.000000 datasphere-0.7.1/datasphere/changelog.md
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1950 2024-04-23 09:31:47.000000 datasphere-0.7.1/datasphere/channel.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13992 2024-05-27 14:20:37.000000 datasphere-0.7.1/datasphere/client.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    23742 2024-05-13 11:49:19.000000 datasphere-0.7.1/datasphere/config.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5620 2024-04-23 09:31:47.000000 datasphere-0.7.1/datasphere/files.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5410 2024-05-22 08:31:30.000000 datasphere-0.7.1/datasphere/fork.py
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:17.759499 datasphere-0.7.1/datasphere/logs/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)       22 2023-09-06 08:57:07.000000 datasphere-0.7.1/datasphere/logs/__init__.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1506 2024-04-26 10:14:56.000000 datasphere-0.7.1/datasphere/logs/config.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3252 2024-05-22 08:31:30.000000 datasphere-0.7.1/datasphere/logs/logging.yaml
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8705 2024-05-27 14:52:50.000000 datasphere-0.7.1/datasphere/main.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3423 2024-04-23 09:31:47.000000 datasphere-0.7.1/datasphere/output.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6504 2024-03-25 16:32:46.000000 datasphere-0.7.1/datasphere/pyenv.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8506 2024-05-27 14:20:37.000000 datasphere-0.7.1/datasphere/sdk.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8111 2024-04-23 09:31:47.000000 datasphere-0.7.1/datasphere/utils.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2894 2024-05-13 11:49:19.000000 datasphere-0.7.1/datasphere/validation.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)       18 2024-05-27 14:57:01.000000 datasphere-0.7.1/datasphere/version.py
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:18.741753 datasphere-0.7.1/datasphere.egg-info/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      771 2024-05-27 14:57:17.000000 datasphere-0.7.1/datasphere.egg-info/PKG-INFO
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    55007 2024-05-27 14:57:17.000000 datasphere-0.7.1/datasphere.egg-info/SOURCES.txt
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)        1 2024-05-27 14:57:17.000000 datasphere-0.7.1/datasphere.egg-info/dependency_links.txt
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)       52 2024-05-27 14:57:17.000000 datasphere-0.7.1/datasphere.egg-info/entry_points.txt
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)       91 2024-05-27 14:57:17.000000 datasphere-0.7.1/datasphere.egg-info/requires.txt
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)       18 2024-05-27 14:57:17.000000 datasphere-0.7.1/datasphere.egg-info/top_level.txt
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)       90 2023-09-06 08:57:07.000000 datasphere-0.7.1/pyproject.toml
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)       38 2024-05-27 14:57:18.744427 datasphere-0.7.1/setup.cfg
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1574 2024-04-23 09:31:47.000000 datasphere-0.7.1/setup.py
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:17.776190 datasphere-0.7.1/tests/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2745 2024-04-26 10:14:56.000000 datasphere-0.7.1/tests/test_auth.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    27131 2024-05-13 11:49:19.000000 datasphere-0.7.1/tests/test_config.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7009 2024-04-23 09:31:47.000000 datasphere-0.7.1/tests/test_files.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11483 2024-05-22 08:31:30.000000 datasphere-0.7.1/tests/test_fork.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    24569 2024-05-27 14:20:37.000000 datasphere-0.7.1/tests/test_main.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3325 2024-04-23 09:31:47.000000 datasphere-0.7.1/tests/test_output.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7625 2024-02-19 11:57:17.000000 datasphere-0.7.1/tests/test_pyenv.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5490 2024-05-06 11:33:30.000000 datasphere-0.7.1/tests/test_utils.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4120 2024-05-13 11:49:19.000000 datasphere-0.7.1/tests/test_validation.py
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:17.688230 datasphere-0.7.1/yandex/
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:17.781890 datasphere-0.7.1/yandex/cloud/
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:17.788187 datasphere-0.7.1/yandex/cloud/access/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7035 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/access/access_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11674 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/access/access_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/access/access_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/access/access_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:17.794099 datasphere-0.7.1/yandex/cloud/api/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1642 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/api/operation_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1547 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/api/operation_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/api/operation_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/api/operation_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:17.801356 datasphere-0.7.1/yandex/cloud/api/tools/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5058 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/api/tools/options_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10680 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/api/tools/options_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/api/tools/options_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/api/tools/options_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:17.690246 datasphere-0.7.1/yandex/cloud/datasphere/
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:17.845205 datasphere-0.7.1/yandex/cloud/datasphere/v1/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2127 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/datasphere/v1/app_token_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      697 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/datasphere/v1/app_token_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2843 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/datasphere/v1/app_token_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1756 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/datasphere/v1/app_token_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4363 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/datasphere/v1/folder_budget_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4359 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/datasphere/v1/folder_budget_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4843 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/datasphere/v1/folder_budget_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2933 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/datasphere/v1/folder_budget_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1475 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/datasphere/v1/node_execution_error_details_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1307 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/datasphere/v1/node_execution_error_details_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/datasphere/v1/node_execution_error_details_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/datasphere/v1/node_execution_error_details_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3397 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/datasphere/v1/node_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3598 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/datasphere/v1/node_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4708 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/datasphere/v1/node_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2731 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/datasphere/v1/node_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3622 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/datasphere/v1/project_data_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4327 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/datasphere/v1/project_data_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5007 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/datasphere/v1/project_data_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3101 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/datasphere/v1/project_data_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2853 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/datasphere/v1/project_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6747 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/datasphere/v1/project_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/datasphere/v1/project_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/datasphere/v1/project_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    21169 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/datasphere/v1/project_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    23777 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/datasphere/v1/project_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    23351 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/datasphere/v1/project_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11823 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/datasphere/v1/project_service_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:17.918427 datasphere-0.7.1/yandex/cloud/datasphere/v2/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2085 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/datasphere/v2/community_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2700 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/datasphere/v2/community_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/datasphere/v2/community_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/datasphere/v2/community_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    18039 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/datasphere/v2/community_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    14968 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/datasphere/v2/community_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    25433 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/datasphere/v2/community_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12673 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/datasphere/v2/community_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3222 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/datasphere/v2/dataset_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6003 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/datasphere/v2/dataset_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/datasphere/v2/dataset_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/datasphere/v2/dataset_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4262 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/datasphere/v2/dataset_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1431 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/datasphere/v2/dataset_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4727 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/datasphere/v2/dataset_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2718 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/datasphere/v2/dataset_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3085 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/datasphere/v2/docker_image_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      833 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/datasphere/v2/docker_image_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3000 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/datasphere/v2/docker_image_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1932 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/datasphere/v2/docker_image_service_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:17.929237 datasphere-0.7.1/yandex/cloud/datasphere/v2/jobs/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7499 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/datasphere/v2/jobs/jobs_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    19615 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/datasphere/v2/jobs/jobs_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/datasphere/v2/jobs/jobs_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/datasphere/v2/jobs/jobs_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    15121 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/datasphere/v2/jobs/project_job_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    24883 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/datasphere/v2/jobs/project_job_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    26393 2024-05-03 10:44:07.000000 datasphere-0.7.1/yandex/cloud/datasphere/v2/jobs/project_job_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13105 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/datasphere/v2/jobs/project_job_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4865 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/datasphere/v2/project_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13825 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/datasphere/v2/project_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/datasphere/v2/project_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/datasphere/v2/project_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    30712 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/datasphere/v2/project_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    32889 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/datasphere/v2/project_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    36560 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/datasphere/v2/project_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    18489 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/datasphere/v2/project_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1728 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/datasphere/v2/resource_types_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1808 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/datasphere/v2/resource_types_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/datasphere/v2/resource_types_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/datasphere/v2/resource_types_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2500 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/datasphere/v2/restrictions_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5074 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/datasphere/v2/restrictions_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/datasphere/v2/restrictions_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/datasphere/v2/restrictions_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4089 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/datasphere/v2/s3_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1351 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/datasphere/v2/s3_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4629 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/datasphere/v2/s3_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2625 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/datasphere/v2/s3_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2403 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/datasphere/v2/secret_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3671 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/datasphere/v2/secret_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/datasphere/v2/secret_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/datasphere/v2/secret_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1403 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/datasphere/v2/user_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1278 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/datasphere/v2/user_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/datasphere/v2/user_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/datasphere/v2/user_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:17.691263 datasphere-0.7.1/yandex/cloud/iam/
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:17.997799 datasphere-0.7.1/yandex/cloud/iam/v1/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1597 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/api_key_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1934 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/api_key_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/api_key_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/api_key_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9892 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/api_key_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10893 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/api_key_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11954 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/api_key_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6461 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/api_key_service_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:18.006576 datasphere-0.7.1/yandex/cloud/iam/v1/awscompatibility/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1790 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/awscompatibility/access_key_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2269 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/awscompatibility/access_key_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/awscompatibility/access_key_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/awscompatibility/access_key_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10875 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/awscompatibility/access_key_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11282 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/awscompatibility/access_key_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13154 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/awscompatibility/access_key_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7370 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/awscompatibility/access_key_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3737 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/iam_token_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3143 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/iam_token_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4843 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/iam_token_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2899 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/iam_token_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2010 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/key_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3961 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/key_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/key_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/key_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10266 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/key_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12175 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/key_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11657 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/key_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6206 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/key_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1793 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/resource_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      976 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/resource_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/resource_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/resource_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1255 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/role_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      925 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/role_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/role_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/role_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3767 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/role_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3291 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/role_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4554 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/role_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2781 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/role_service_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:18.024799 datasphere-0.7.1/yandex/cloud/iam/v1/saml/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2847 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/saml/certificate_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1777 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/saml/certificate_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/saml/certificate_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/saml/certificate_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12027 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/saml/certificate_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11859 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/saml/certificate_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12556 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/saml/certificate_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6877 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/saml/certificate_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4306 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/saml/federation_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6010 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/saml/federation_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/saml/federation_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/saml/federation_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    17989 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/saml/federation_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    22543 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/saml/federation_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    16385 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/saml/federation_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8728 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/saml/federation_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2036 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/service_account_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2749 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/service_account_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/service_account_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/service_account_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    15960 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/service_account_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13599 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/service_account_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    18212 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/service_account_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9932 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/service_account_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2152 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/service_control_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3714 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/service_control_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/service_control_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/service_control_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10684 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/service_control_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11460 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/service_control_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12220 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/service_control_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6823 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/service_control_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3432 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/user_account_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5187 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/user_account_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/user_account_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/user_account_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2488 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/user_account_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      760 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/user_account_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3160 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/user_account_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2128 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/user_account_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2614 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/yandex_passport_user_account_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      748 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/yandex_passport_user_account_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3259 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/yandex_passport_user_account_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2175 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/iam/v1/yandex_passport_user_account_service_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:18.033286 datasphere-0.7.1/yandex/cloud/operation/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2082 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/operation/operation_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3928 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/operation/operation_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/operation/operation_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/operation/operation_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3422 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/operation/operation_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1247 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/operation/operation_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4786 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/operation/operation_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3040 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/operation/operation_service_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:18.041807 datasphere-0.7.1/yandex/cloud/priv/
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:18.046252 datasphere-0.7.1/yandex/cloud/priv/access/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7436 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/access/access_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11207 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/access/access_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/access/access_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/access/access_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:17.693497 datasphere-0.7.1/yandex/cloud/priv/ai/
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:17.693891 datasphere-0.7.1/yandex/cloud/priv/ai/platform/
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:18.069943 datasphere-0.7.1/yandex/cloud/priv/ai/platform/v1/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5762 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/ai/platform/v1/project_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8938 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/ai/platform/v1/project_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/ai/platform/v1/project_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/ai/platform/v1/project_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    21479 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/ai/platform/v1/project_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    23490 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/ai/platform/v1/project_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    28428 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/ai/platform/v1/project_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11959 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/ai/platform/v1/project_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1957 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/ai/platform/v1/quota_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      166 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/ai/platform/v1/quota_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6379 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/ai/platform/v1/quota_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2764 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/ai/platform/v1/quota_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2479 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/ai/platform/v1/resource_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2109 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/ai/platform/v1/resource_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/ai/platform/v1/resource_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/ai/platform/v1/resource_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12394 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/ai/platform/v1/resource_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9656 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/ai/platform/v1/resource_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    16814 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/ai/platform/v1/resource_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7238 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/ai/platform/v1/resource_service_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:17.695113 datasphere-0.7.1/yandex/cloud/priv/console/
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:18.082996 datasphere-0.7.1/yandex/cloud/priv/console/v1/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3853 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/console/v1/access_binding_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4903 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/console/v1/access_binding_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/console/v1/access_binding_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/console/v1/access_binding_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5290 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/console/v1/form_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12845 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/console/v1/form_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/console/v1/form_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/console/v1/form_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3025 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/console/v1/resource_settings_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2765 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/console/v1/resource_settings_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/console/v1/resource_settings_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/console/v1/resource_settings_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:18.087523 datasphere-0.7.1/yandex/cloud/priv/console/v2/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6296 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/console/v2/form_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    16990 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/console/v2/form_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/console/v2/form_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/console/v2/form_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:17.696944 datasphere-0.7.1/yandex/cloud/priv/dataproc/
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:17.696399 datasphere-0.7.1/yandex/cloud/priv/dataproc/manager/
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:18.102395 datasphere-0.7.1/yandex/cloud/priv/dataproc/manager/v1/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8503 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/dataproc/manager/v1/job_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    27307 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/dataproc/manager/v1/job_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/dataproc/manager/v1/job_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/dataproc/manager/v1/job_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7819 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/dataproc/manager/v1/job_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9134 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/dataproc/manager/v1/job_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13216 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/dataproc/manager/v1/job_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6864 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/dataproc/manager/v1/job_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12676 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/dataproc/manager/v1/manager_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    31568 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/dataproc/manager/v1/manager_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13374 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/dataproc/manager/v1/manager_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7085 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/dataproc/manager/v1/manager_service_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:18.148273 datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5841 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/cluster_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    14555 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/cluster_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/cluster_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/cluster_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    24667 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/cluster_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    30846 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/cluster_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    21920 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/cluster_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11026 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/cluster_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1859 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/common_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2476 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/common_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/common_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/common_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:18.152373 datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/job_operation/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2187 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/job_operation/operation_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      738 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/job_operation/operation_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3212 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/job_operation/operation_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2039 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/job_operation/operation_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8327 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/job_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    27307 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/job_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/job_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/job_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    18092 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/job_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    16844 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/job_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    23743 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/job_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12016 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/job_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2522 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/operation_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      738 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/operation_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3080 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/operation_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1983 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/operation_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1402 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/resource_preset_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1536 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/resource_preset_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/resource_preset_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/resource_preset_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4317 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/resource_preset_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3414 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/resource_preset_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5289 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/resource_preset_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3454 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/resource_preset_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5320 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/subcluster_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8706 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/subcluster_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/subcluster_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/subcluster_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    14687 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/subcluster_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13191 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/subcluster_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12615 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/subcluster_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6472 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/subcluster_service_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:17.699069 datasphere-0.7.1/yandex/cloud/priv/datasphere/
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:18.173808 datasphere-0.7.1/yandex/cloud/priv/datasphere/v1/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2179 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v1/app_token_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      697 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v1/app_token_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2899 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v1/app_token_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1776 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v1/app_token_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5919 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v1/operation_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6258 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v1/operation_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8725 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v1/operation_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3967 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v1/operation_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3666 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v1/project_data_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3891 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v1/project_data_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5128 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v1/project_data_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2609 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v1/project_data_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4603 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v1/project_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10044 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v1/project_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v1/project_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v1/project_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    24541 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v1/project_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    23699 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v1/project_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    26233 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v1/project_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11102 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v1/project_service_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:18.325873 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2968 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/access_binding_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      838 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/access_binding_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3226 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/access_binding_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1707 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/access_binding_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2940 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/admin_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5151 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/admin_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/admin_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/admin_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1858 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/admin_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      698 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/admin_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3158 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/admin_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1659 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/admin_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1744 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/alpha_flag_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1995 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/alpha_flag_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/alpha_flag_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/alpha_flag_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3732 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/alpha_flag_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3342 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/alpha_flag_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8935 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/alpha_flag_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3996 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/alpha_flag_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4216 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/checkpoint_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8940 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/checkpoint_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/checkpoint_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/checkpoint_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    16670 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/checkpoint_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    22531 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/checkpoint_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    22907 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/checkpoint_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10053 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/checkpoint_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4388 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/community_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8562 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/community_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/community_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/community_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9325 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/community_quota_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    14063 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/community_quota_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    15703 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/community_quota_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7197 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/community_quota_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    41234 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/community_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    43622 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/community_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    74204 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/community_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    30906 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/community_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5533 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/data_proc_template_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11027 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/data_proc_template_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/data_proc_template_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/data_proc_template_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13301 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/data_proc_template_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12107 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/data_proc_template_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    19704 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/data_proc_template_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8849 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/data_proc_template_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3284 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/dataset_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5374 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/dataset_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/dataset_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/dataset_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    14406 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/dataset_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12655 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/dataset_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    36208 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/dataset_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    15498 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/dataset_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3054 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/docker_image_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5312 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/docker_image_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/docker_image_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/docker_image_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    20678 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/docker_image_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    19462 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/docker_image_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    28949 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/docker_image_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12489 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/docker_image_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4490 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/feature_property_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9583 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/feature_property_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/feature_property_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/feature_property_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5964 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/feature_property_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7982 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/feature_property_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11448 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/feature_property_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5081 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/feature_property_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4312 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/foundation_model_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8385 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/foundation_model_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/foundation_model_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/foundation_model_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11450 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/foundation_model_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    15499 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/foundation_model_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    19696 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/foundation_model_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9000 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/foundation_model_service_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:18.337973 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/internal/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3397 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/internal/community_info_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5236 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/internal/community_info_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/internal/community_info_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/internal/community_info_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7889 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/internal/project_info_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    17799 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/internal/project_info_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/internal/project_info_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/internal/project_info_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4091 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/internal/project_info_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1634 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/internal/project_info_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7526 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/internal/project_info_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3590 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/internal/project_info_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3422 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/internal_storage_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3962 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/internal_storage_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3328 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/internal_storage_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1874 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/internal_storage_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6797 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/invite_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6113 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/invite_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11164 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/invite_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5030 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/invite_service_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:18.344925 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/jobs/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9291 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/jobs/jobs_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    22514 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/jobs/jobs_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/jobs/jobs_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/jobs/jobs_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    19098 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/jobs/project_job_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    28824 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/jobs/project_job_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    35270 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/jobs/project_job_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    15679 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/jobs/project_job_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3386 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/model_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6482 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/model_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/model_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/model_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11037 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/model_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12352 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/model_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    14265 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/model_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6126 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/model_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8243 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/navigation_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12049 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/navigation_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12828 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/navigation_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5609 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/navigation_service_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:18.388078 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2546 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/billing_spec_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2126 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/billing_spec_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/billing_spec_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/billing_spec_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7543 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/docker_app_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11171 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/docker_app_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/docker_app_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/docker_app_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3489 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/healthcheck_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3942 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/healthcheck_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/healthcheck_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/healthcheck_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3638 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/instance_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4954 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/instance_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/instance_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/instance_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4197 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/instance_spec_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5151 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/instance_spec_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/instance_spec_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/instance_spec_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6231 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/node_alias_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7355 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/node_alias_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/node_alias_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/node_alias_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7247 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/node_alias_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7644 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/node_alias_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9379 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/node_alias_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4339 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/node_alias_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7987 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/node_deployer_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8549 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/node_deployer_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13689 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/node_deployer_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6285 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/node_deployer_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3423 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/node_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4115 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/node_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/node_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/node_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3322 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/node_spec_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2854 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/node_spec_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/node_spec_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/node_spec_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4276 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/policies_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4903 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/policies_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/policies_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/policies_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1588 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/runtime_options_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      652 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/runtime_options_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/runtime_options_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/runtime_options_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5122 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/servant_app_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7073 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/servant_app_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/servant_app_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/servant_app_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3635 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/triton_app_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7030 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/triton_app_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/triton_app_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/triton_app_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5664 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/project_ide_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5237 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/project_ide_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9310 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/project_ide_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4354 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/project_ide_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10444 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/project_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    22895 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/project_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/project_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/project_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    62074 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/project_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    76415 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/project_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    87993 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/project_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    37048 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/project_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11585 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/resource_actions_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    32305 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/resource_actions_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/resource_actions_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/resource_actions_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11654 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/resource_types_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    23421 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/resource_types_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/resource_types_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/resource_types_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2563 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/restrictions_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4668 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/restrictions_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/restrictions_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/restrictions_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2401 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/s3_keys_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1282 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/s3_keys_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2998 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/s3_keys_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1607 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/s3_keys_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3801 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/s3_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7191 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/s3_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/s3_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/s3_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    15821 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/s3_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    16907 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/s3_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    27459 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/s3_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11496 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/s3_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2785 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/secret_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4438 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/secret_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/secret_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/secret_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10294 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/secret_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7930 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/secret_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    16411 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/secret_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7233 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/secret_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7480 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/spark_connector_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8620 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/spark_connector_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/spark_connector_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/spark_connector_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10923 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/spark_connector_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11677 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/spark_connector_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    15539 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/spark_connector_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7009 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/spark_connector_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1446 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/user_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1092 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/user_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/user_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/user_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3899 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/user_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3052 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/user_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8621 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/user_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3770 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/user_service_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:18.391082 datasphere-0.7.1/yandex/cloud/priv/iam/
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:18.393858 datasphere-0.7.1/yandex/cloud/priv/iam/management/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1842 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/management/cache_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1299 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/management/cache_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3041 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/management/cache_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1968 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/management/cache_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6663 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/restriction_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9186 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/restriction_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/restriction_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/restriction_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:18.558498 datasphere-0.7.1/yandex/cloud/priv/iam/v1/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    20419 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/access_binding_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    27526 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/access_binding_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13351 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/access_binding_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5965 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/access_binding_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1687 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/api_key_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1945 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/api_key_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/api_key_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/api_key_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11072 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/api_key_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8448 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/api_key_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12365 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/api_key_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5310 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/api_key_service_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:18.570432 datasphere-0.7.1/yandex/cloud/priv/iam/v1/awscompatibility/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1766 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/awscompatibility/access_key_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1914 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/awscompatibility/access_key_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/awscompatibility/access_key_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/awscompatibility/access_key_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13006 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/awscompatibility/access_key_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9998 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/awscompatibility/access_key_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    15757 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/awscompatibility/access_key_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7186 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/awscompatibility/access_key_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3515 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/awscompatibility/delegation_key_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2046 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/awscompatibility/delegation_key_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3312 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/awscompatibility/delegation_key_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1915 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/awscompatibility/delegation_key_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4611 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/awscompatibility/temporary_access_key_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3491 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/awscompatibility/temporary_access_key_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3400 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/awscompatibility/temporary_access_key_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1947 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/awscompatibility/temporary_access_key_service_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:18.575810 datasphere-0.7.1/yandex/cloud/priv/iam/v1/backoffice/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7315 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/backoffice/access_binding_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9843 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/backoffice/access_binding_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5367 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/backoffice/access_binding_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2749 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/backoffice/access_binding_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4141 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/backoffice/permission_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4815 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/backoffice/permission_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3123 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/backoffice/permission_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1713 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/backoffice/permission_service_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:18.579245 datasphere-0.7.1/yandex/cloud/priv/iam/v1/compute/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10397 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/compute/os_login_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12623 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/compute/os_login_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8942 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/compute/os_login_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4284 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/compute/os_login_service_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:18.600286 datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4711 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/access_binding_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5177 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/access_binding_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5722 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/access_binding_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3554 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/access_binding_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3249 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/key_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1994 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/key_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2956 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/key_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1559 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/key_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3854 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/membership_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3267 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/membership_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3063 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/membership_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1820 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/membership_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2137 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/os_login_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1323 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/os_login_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3007 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/os_login_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1764 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/os_login_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3905 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/role_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4223 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/role_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4893 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/role_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2523 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/role_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7585 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/service_account_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5598 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/service_account_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7360 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/service_account_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3668 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/service_account_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2439 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/user_account_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      955 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/user_account_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3238 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/user_account_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1903 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/user_account_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4863 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/gizmo_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3148 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/gizmo_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5144 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/gizmo_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2479 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/gizmo_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6233 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/iam_cookie_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6400 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/iam_cookie_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8930 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/iam_cookie_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4143 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/iam_cookie_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2962 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/iam_credential_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1776 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/iam_credential_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3144 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/iam_credential_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1693 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/iam_credential_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4722 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/iam_session_token_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3041 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/iam_session_token_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3115 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/iam_session_token_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1937 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/iam_session_token_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    17389 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/iam_token_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    17269 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/iam_token_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    18896 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/iam_token_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9387 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/iam_token_service_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:18.606384 datasphere-0.7.1/yandex/cloud/priv/iam/v1/inner/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3215 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/inner/service_registry_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3953 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/inner/service_registry_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/inner/service_registry_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/inner/service_registry_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13970 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/inner/service_registry_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10870 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/inner/service_registry_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    14973 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/inner/service_registry_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6423 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/inner/service_registry_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2341 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/key_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3745 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/key_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/key_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/key_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13653 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/key_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11972 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/key_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    14022 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/key_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5878 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/key_service_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:18.609297 datasphere-0.7.1/yandex/cloud/priv/iam/v1/maintenance/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1785 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/maintenance/metadata_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1860 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/maintenance/metadata_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/maintenance/metadata_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/maintenance/metadata_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6828 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/membership_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6683 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/membership_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7267 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/membership_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4094 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/membership_service_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:18.618108 datasphere-0.7.1/yandex/cloud/priv/iam/v1/mfa/
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:18.621659 datasphere-0.7.1/yandex/cloud/priv/iam/v1/mfa/console/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4476 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/mfa/console/totp_profile_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4837 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/mfa/console/totp_profile_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5480 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/mfa/console/totp_profile_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3615 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/mfa/console/totp_profile_service_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:18.627659 datasphere-0.7.1/yandex/cloud/priv/iam/v1/mfa/hardware/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3216 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/mfa/hardware/totp_profile_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4660 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/mfa/hardware/totp_profile_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/mfa/hardware/totp_profile_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/mfa/hardware/totp_profile_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    24492 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/mfa/hardware/totp_profile_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    21229 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/mfa/hardware/totp_profile_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    23761 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/mfa/hardware/totp_profile_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12614 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/mfa/hardware/totp_profile_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2091 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/mfa/operation_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      687 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/mfa/operation_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3028 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/mfa/operation_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1586 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/mfa/operation_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3062 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/mfa/totp_profile_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5764 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/mfa/totp_profile_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/mfa/totp_profile_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/mfa/totp_profile_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9376 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/mfa/totp_profile_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9082 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/mfa/totp_profile_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    15464 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/mfa/totp_profile_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8966 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/mfa/totp_profile_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2066 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/oauth_client_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4656 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/oauth_client_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/oauth_client_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/oauth_client_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    15285 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/oauth_client_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13367 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/oauth_client_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12466 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/oauth_client_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5401 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/oauth_client_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1345 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/oauth_scope_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1228 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/oauth_scope_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/oauth_scope_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/oauth_scope_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7990 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/oauth_scope_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7215 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/oauth_scope_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10574 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/oauth_scope_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4625 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/oauth_scope_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2457 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/operation_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      687 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/operation_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2980 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/operation_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1570 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/operation_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1299 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/os_login_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      888 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/os_login_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/os_login_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/os_login_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5980 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/os_login_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4920 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/os_login_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6765 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/os_login_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3060 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/os_login_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1249 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/permission_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      725 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/permission_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/permission_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/permission_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6963 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/permission_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5725 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/permission_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10526 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/permission_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4600 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/permission_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3420 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/permission_stage_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4264 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/permission_stage_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/permission_stage_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/permission_stage_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6787 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/permission_stage_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5637 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/permission_stage_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8996 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/permission_stage_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4131 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/permission_stage_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2904 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/quota_limit_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      166 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/quota_limit_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8522 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/quota_limit_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3821 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/quota_limit_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1794 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/quota_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      166 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/quota_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6323 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/quota_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2764 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/quota_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4088 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/refresh_token_issue_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2806 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/refresh_token_issue_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3234 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/refresh_token_issue_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1816 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/refresh_token_issue_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8051 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/refresh_token_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9586 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/refresh_token_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5029 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/refresh_token_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2490 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/refresh_token_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2020 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/resource_boundary_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1022 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/resource_boundary_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/resource_boundary_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/resource_boundary_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1787 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/resource_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      820 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/resource_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/resource_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/resource_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1298 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/resource_type_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      876 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/resource_type_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/resource_type_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/resource_type_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10194 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/resource_type_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8808 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/resource_type_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    14808 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/resource_type_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6452 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/resource_type_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1817 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/restriction_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1626 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/restriction_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/restriction_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/restriction_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12853 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/restriction_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11981 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/restriction_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12870 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/restriction_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5695 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/restriction_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2432 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/restriction_type_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4629 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/restriction_type_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/restriction_type_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/restriction_type_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    16936 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/restriction_type_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    17238 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/restriction_type_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    17177 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/restriction_type_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7798 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/restriction_type_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1739 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/revoked_credential_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2197 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/revoked_credential_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/revoked_credential_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/revoked_credential_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1587 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/role_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2154 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/role_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/role_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/role_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    14082 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/role_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    14017 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/role_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    19538 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/role_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8002 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/role_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3993 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/root_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2470 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/root_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5121 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/root_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2461 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/root_service_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:18.640899 datasphere-0.7.1/yandex/cloud/priv/iam/v1/saml/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1803 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/saml/certificate_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2648 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/saml/certificate_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/saml/certificate_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/saml/certificate_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12270 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/saml/certificate_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8283 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/saml/certificate_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12943 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/saml/certificate_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5852 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/saml/certificate_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3070 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/saml/federation_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7156 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/saml/federation_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/saml/federation_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/saml/federation_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    19637 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/saml/federation_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    16002 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/saml/federation_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    19103 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/saml/federation_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8309 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/saml/federation_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2110 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/service_account_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2571 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/service_account_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/service_account_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/service_account_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    23376 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/service_account_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    14997 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/service_account_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    32314 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/service_account_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13727 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/service_account_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4541 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/service_control_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9023 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/service_control_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/service_control_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/service_control_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    35409 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/service_control_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    39042 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/service_control_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    42084 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/service_control_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    17665 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/service_control_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1800 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/ssh_key_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1494 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/ssh_key_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/ssh_key_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/ssh_key_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7460 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/ssh_key_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7777 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/ssh_key_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10494 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/ssh_key_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4549 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/ssh_key_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1688 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/subject_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2416 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/subject_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/subject_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/subject_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    19400 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/subject_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    26591 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/subject_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    16449 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/subject_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8715 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/subject_service_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:18.643618 datasphere-0.7.1/yandex/cloud/priv/iam/v1/token/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1767 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/token/iam_token_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1010 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/token/iam_token_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/token/iam_token_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/token/iam_token_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2200 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/token_agent_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1631 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/token_agent_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2788 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/token_agent_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1623 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/token_agent_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:18.673956 datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3651 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/agreement_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1284 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/agreement_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7376 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/agreement_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3706 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/agreement_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2710 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/auth_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1252 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/auth_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3014 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/auth_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1696 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/auth_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2833 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/health_check_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1957 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/health_check_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3179 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/health_check_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1734 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/health_check_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4164 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/passport_federation_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3230 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/passport_federation_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3334 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/passport_federation_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1776 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/passport_federation_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6081 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/policy_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5439 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/policy_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13083 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/policy_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5920 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/policy_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2418 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/roles_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1960 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/roles_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3020 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/roles_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1614 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/roles_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4268 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/service_account_access_key_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4220 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/service_account_access_key_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7626 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/service_account_access_key_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3720 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/service_account_access_key_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7133 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/user_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6911 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/user_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11106 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/user_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5022 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/user_service_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:18.678107 datasphere-0.7.1/yandex/cloud/priv/iam/v1/ts/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2581 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/ts/iam_token_service_subject_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2068 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/ts/iam_token_service_subject_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/ts/iam_token_service_subject_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/ts/iam_token_service_subject_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4652 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/user_account_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6814 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/user_account_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/user_account_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/user_account_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10219 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/user_account_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10216 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/user_account_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10807 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/user_account_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4754 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/user_account_service_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:18.686276 datasphere-0.7.1/yandex/cloud/priv/iam/v1/workload/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1681 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/workload/federated_credential_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1528 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/workload/federated_credential_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/workload/federated_credential_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/workload/federated_credential_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9085 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/workload/federated_credential_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6933 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/workload/federated_credential_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11852 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/workload/federated_credential_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5630 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/workload/federated_credential_service_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:18.693898 datasphere-0.7.1/yandex/cloud/priv/iam/v1/workload/oidc/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2211 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/workload/oidc/federation_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2863 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/workload/oidc/federation_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/workload/oidc/federation_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/workload/oidc/federation_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11277 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/workload/oidc/federation_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8949 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/workload/oidc/federation_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11214 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/workload/oidc/federation_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4950 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/workload/oidc/federation_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/yandex_passport_cookie_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1715 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/yandex_passport_cookie_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/yandex_passport_cookie_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/yandex_passport_cookie_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5811 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/yandex_passport_user_account_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3965 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/yandex_passport_user_account_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7412 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/yandex_passport_user_account_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3657 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/iam/v1/yandex_passport_user_account_service_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:18.698264 datasphere-0.7.1/yandex/cloud/priv/oauth/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8516 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/oauth/claims_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13189 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/oauth/claims_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/oauth/claims_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/oauth/claims_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:18.717546 datasphere-0.7.1/yandex/cloud/priv/oauth/v1/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3834 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/oauth/v1/claim_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5858 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/oauth/v1/claim_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2871 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/oauth/v1/claim_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1528 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/oauth/v1/claim_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2204 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/oauth/v1/cloud_user_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2418 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/oauth/v1/cloud_user_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/oauth/v1/cloud_user_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/oauth/v1/cloud_user_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4519 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/oauth/v1/login_history_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4058 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/oauth/v1/login_history_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5062 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/oauth/v1/login_history_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3288 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/oauth/v1/login_history_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1887 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/oauth/v1/oauth_request_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1192 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/oauth/v1/oauth_request_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/oauth/v1/oauth_request_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/oauth/v1/oauth_request_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12256 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/oauth/v1/session_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    16448 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/oauth/v1/session_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13682 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/oauth/v1/session_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9862 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/oauth/v1/session_service_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:18.720868 datasphere-0.7.1/yandex/cloud/priv/operation/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2057 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/operation/operation_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2678 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/operation/operation_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/operation/operation_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/operation/operation_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:18.727120 datasphere-0.7.1/yandex/cloud/priv/quota/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7135 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/quota/quota_limit_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9425 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/quota/quota_limit_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/quota/quota_limit_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/quota/quota_limit_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6853 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/quota/quota_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11292 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/quota/quota_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/quota/quota_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/quota/quota_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:18.731315 datasphere-0.7.1/yandex/cloud/priv/reference/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1762 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/reference/reference_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2597 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/reference/reference_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/reference/reference_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/reference/reference_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1953 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/sensitive_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2595 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/sensitive_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/sensitive_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/sensitive_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:17.713968 datasphere-0.7.1/yandex/cloud/priv/servicecontrol/
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-27 14:57:18.740385 datasphere-0.7.1/yandex/cloud/priv/servicecontrol/v1/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    17172 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/servicecontrol/v1/access_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    23231 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/servicecontrol/v1/access_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9486 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/servicecontrol/v1/access_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/servicecontrol/v1/access_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2246 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/servicecontrol/v1/resource_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1428 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/servicecontrol/v1/resource_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/servicecontrol/v1/resource_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/servicecontrol/v1/resource_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2111 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/validation_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2479 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/validation_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/validation_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/priv/validation_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2132 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/validation_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2479 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/validation_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/validation_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.1/yandex/cloud/validation_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:52.479396 datasphere-0.7.2/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      771 2024-05-28 13:24:52.478377 datasphere-0.7.2/PKG-INFO
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4245 2024-05-03 11:43:05.000000 datasphere-0.7.2/README.md
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:51.500989 datasphere-0.7.2/datasphere/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)       21 2024-05-22 08:31:30.000000 datasphere-0.7.2/datasphere/__init__.py
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:51.507056 datasphere-0.7.2/datasphere/api/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2570 2024-05-03 11:43:05.000000 datasphere-0.7.2/datasphere/api/__init__.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6455 2024-05-28 13:24:16.000000 datasphere-0.7.2/datasphere/auth.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      853 2024-05-27 14:20:37.000000 datasphere-0.7.2/datasphere/changelog.md
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1950 2024-04-23 09:31:47.000000 datasphere-0.7.2/datasphere/channel.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13992 2024-05-27 14:20:37.000000 datasphere-0.7.2/datasphere/client.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    23742 2024-05-13 11:49:19.000000 datasphere-0.7.2/datasphere/config.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5620 2024-04-23 09:31:47.000000 datasphere-0.7.2/datasphere/files.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5410 2024-05-22 08:31:30.000000 datasphere-0.7.2/datasphere/fork.py
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:51.511368 datasphere-0.7.2/datasphere/logs/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)       22 2023-09-06 08:57:07.000000 datasphere-0.7.2/datasphere/logs/__init__.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1506 2024-04-26 10:14:56.000000 datasphere-0.7.2/datasphere/logs/config.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3252 2024-05-22 08:31:30.000000 datasphere-0.7.2/datasphere/logs/logging.yaml
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8705 2024-05-27 14:52:50.000000 datasphere-0.7.2/datasphere/main.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3418 2024-05-28 12:04:44.000000 datasphere-0.7.2/datasphere/output.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6504 2024-03-25 16:32:46.000000 datasphere-0.7.2/datasphere/pyenv.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8506 2024-05-27 14:20:37.000000 datasphere-0.7.2/datasphere/sdk.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8111 2024-04-23 09:31:47.000000 datasphere-0.7.2/datasphere/utils.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2894 2024-05-13 11:49:19.000000 datasphere-0.7.2/datasphere/validation.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)       18 2024-05-28 13:24:16.000000 datasphere-0.7.2/datasphere/version.py
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:52.477041 datasphere-0.7.2/datasphere.egg-info/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      771 2024-05-28 13:24:51.000000 datasphere-0.7.2/datasphere.egg-info/PKG-INFO
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    55007 2024-05-28 13:24:51.000000 datasphere-0.7.2/datasphere.egg-info/SOURCES.txt
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)        1 2024-05-28 13:24:51.000000 datasphere-0.7.2/datasphere.egg-info/dependency_links.txt
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)       52 2024-05-28 13:24:51.000000 datasphere-0.7.2/datasphere.egg-info/entry_points.txt
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)       91 2024-05-28 13:24:51.000000 datasphere-0.7.2/datasphere.egg-info/requires.txt
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)       18 2024-05-28 13:24:51.000000 datasphere-0.7.2/datasphere.egg-info/top_level.txt
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)       90 2023-09-06 08:57:07.000000 datasphere-0.7.2/pyproject.toml
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)       38 2024-05-28 13:24:52.479546 datasphere-0.7.2/setup.cfg
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1574 2024-04-23 09:31:47.000000 datasphere-0.7.2/setup.py
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:51.525402 datasphere-0.7.2/tests/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4597 2024-05-28 13:24:16.000000 datasphere-0.7.2/tests/test_auth.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    27131 2024-05-13 11:49:19.000000 datasphere-0.7.2/tests/test_config.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7009 2024-04-23 09:31:47.000000 datasphere-0.7.2/tests/test_files.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11483 2024-05-22 08:31:30.000000 datasphere-0.7.2/tests/test_fork.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    24569 2024-05-27 14:20:37.000000 datasphere-0.7.2/tests/test_main.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3325 2024-04-23 09:31:47.000000 datasphere-0.7.2/tests/test_output.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7625 2024-02-19 11:57:17.000000 datasphere-0.7.2/tests/test_pyenv.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5490 2024-05-06 11:33:30.000000 datasphere-0.7.2/tests/test_utils.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4120 2024-05-13 11:49:19.000000 datasphere-0.7.2/tests/test_validation.py
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:51.457563 datasphere-0.7.2/yandex/
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:51.531721 datasphere-0.7.2/yandex/cloud/
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:51.539288 datasphere-0.7.2/yandex/cloud/access/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7035 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/access/access_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11674 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/access/access_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/access/access_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/access/access_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:51.547616 datasphere-0.7.2/yandex/cloud/api/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1642 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/api/operation_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1547 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/api/operation_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/api/operation_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/api/operation_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:51.557740 datasphere-0.7.2/yandex/cloud/api/tools/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5058 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/api/tools/options_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10680 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/api/tools/options_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/api/tools/options_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/api/tools/options_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:51.459172 datasphere-0.7.2/yandex/cloud/datasphere/
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:51.601857 datasphere-0.7.2/yandex/cloud/datasphere/v1/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2127 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/datasphere/v1/app_token_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      697 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/datasphere/v1/app_token_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2843 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/datasphere/v1/app_token_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1756 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/datasphere/v1/app_token_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4363 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/datasphere/v1/folder_budget_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4359 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/datasphere/v1/folder_budget_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4843 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/datasphere/v1/folder_budget_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2933 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/datasphere/v1/folder_budget_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1475 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/datasphere/v1/node_execution_error_details_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1307 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/datasphere/v1/node_execution_error_details_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/datasphere/v1/node_execution_error_details_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/datasphere/v1/node_execution_error_details_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3397 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/datasphere/v1/node_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3598 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/datasphere/v1/node_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4708 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/datasphere/v1/node_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2731 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/datasphere/v1/node_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3622 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/datasphere/v1/project_data_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4327 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/datasphere/v1/project_data_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5007 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/datasphere/v1/project_data_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3101 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/datasphere/v1/project_data_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2853 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/datasphere/v1/project_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6747 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/datasphere/v1/project_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/datasphere/v1/project_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/datasphere/v1/project_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    21169 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/datasphere/v1/project_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    23777 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/datasphere/v1/project_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    23351 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/datasphere/v1/project_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11823 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/datasphere/v1/project_service_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:51.661220 datasphere-0.7.2/yandex/cloud/datasphere/v2/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2085 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/datasphere/v2/community_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2700 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/datasphere/v2/community_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/datasphere/v2/community_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/datasphere/v2/community_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    18039 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/datasphere/v2/community_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    14968 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/datasphere/v2/community_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    25433 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/datasphere/v2/community_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12673 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/datasphere/v2/community_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3222 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/datasphere/v2/dataset_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6003 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/datasphere/v2/dataset_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/datasphere/v2/dataset_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/datasphere/v2/dataset_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4262 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/datasphere/v2/dataset_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1431 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/datasphere/v2/dataset_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4727 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/datasphere/v2/dataset_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2718 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/datasphere/v2/dataset_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3085 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/datasphere/v2/docker_image_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      833 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/datasphere/v2/docker_image_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3000 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/datasphere/v2/docker_image_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1932 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/datasphere/v2/docker_image_service_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:51.670545 datasphere-0.7.2/yandex/cloud/datasphere/v2/jobs/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7499 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/datasphere/v2/jobs/jobs_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    19615 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/datasphere/v2/jobs/jobs_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/datasphere/v2/jobs/jobs_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/datasphere/v2/jobs/jobs_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    15121 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/datasphere/v2/jobs/project_job_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    24883 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/datasphere/v2/jobs/project_job_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    26393 2024-05-03 10:44:07.000000 datasphere-0.7.2/yandex/cloud/datasphere/v2/jobs/project_job_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13105 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/datasphere/v2/jobs/project_job_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4865 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/datasphere/v2/project_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13825 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/datasphere/v2/project_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/datasphere/v2/project_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/datasphere/v2/project_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    30712 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/datasphere/v2/project_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    32889 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/datasphere/v2/project_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    36560 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/datasphere/v2/project_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    18489 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/datasphere/v2/project_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1728 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/datasphere/v2/resource_types_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1808 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/datasphere/v2/resource_types_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/datasphere/v2/resource_types_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/datasphere/v2/resource_types_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2500 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/datasphere/v2/restrictions_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5074 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/datasphere/v2/restrictions_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/datasphere/v2/restrictions_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/datasphere/v2/restrictions_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4089 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/datasphere/v2/s3_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1351 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/datasphere/v2/s3_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4629 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/datasphere/v2/s3_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2625 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/datasphere/v2/s3_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2403 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/datasphere/v2/secret_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3671 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/datasphere/v2/secret_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/datasphere/v2/secret_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/datasphere/v2/secret_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1403 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/datasphere/v2/user_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1278 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/datasphere/v2/user_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/datasphere/v2/user_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/datasphere/v2/user_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:51.460039 datasphere-0.7.2/yandex/cloud/iam/
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:51.736098 datasphere-0.7.2/yandex/cloud/iam/v1/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1597 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/api_key_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1934 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/api_key_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/api_key_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/api_key_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9892 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/api_key_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10893 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/api_key_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11954 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/api_key_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6461 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/api_key_service_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:51.744924 datasphere-0.7.2/yandex/cloud/iam/v1/awscompatibility/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1790 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/awscompatibility/access_key_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2269 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/awscompatibility/access_key_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/awscompatibility/access_key_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/awscompatibility/access_key_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10875 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/awscompatibility/access_key_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11282 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/awscompatibility/access_key_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13154 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/awscompatibility/access_key_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7370 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/awscompatibility/access_key_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3737 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/iam_token_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3143 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/iam_token_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4843 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/iam_token_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2899 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/iam_token_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2010 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/key_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3961 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/key_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/key_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/key_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10266 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/key_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12175 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/key_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11657 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/key_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6206 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/key_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1793 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/resource_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      976 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/resource_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/resource_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/resource_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1255 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/role_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      925 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/role_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/role_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/role_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3767 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/role_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3291 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/role_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4554 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/role_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2781 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/role_service_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:51.762097 datasphere-0.7.2/yandex/cloud/iam/v1/saml/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2847 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/saml/certificate_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1777 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/saml/certificate_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/saml/certificate_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/saml/certificate_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12027 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/saml/certificate_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11859 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/saml/certificate_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12556 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/saml/certificate_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6877 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/saml/certificate_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4306 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/saml/federation_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6010 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/saml/federation_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/saml/federation_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/saml/federation_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    17989 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/saml/federation_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    22543 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/saml/federation_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    16385 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/saml/federation_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8728 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/saml/federation_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2036 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/service_account_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2749 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/service_account_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/service_account_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/service_account_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    15960 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/service_account_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13599 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/service_account_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    18212 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/service_account_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9932 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/service_account_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2152 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/service_control_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3714 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/service_control_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/service_control_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/service_control_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10684 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/service_control_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11460 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/service_control_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12220 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/service_control_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6823 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/service_control_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3432 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/user_account_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5187 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/user_account_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/user_account_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/user_account_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2488 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/user_account_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      760 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/user_account_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3160 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/user_account_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2128 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/user_account_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2614 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/yandex_passport_user_account_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      748 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/yandex_passport_user_account_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3259 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/yandex_passport_user_account_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2175 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/iam/v1/yandex_passport_user_account_service_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:51.770038 datasphere-0.7.2/yandex/cloud/operation/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2082 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/operation/operation_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3928 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/operation/operation_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/operation/operation_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/operation/operation_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3422 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/operation/operation_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1247 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/operation/operation_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4786 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/operation/operation_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3040 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/operation/operation_service_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:51.775468 datasphere-0.7.2/yandex/cloud/priv/
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:51.778909 datasphere-0.7.2/yandex/cloud/priv/access/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7436 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/access/access_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11207 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/access/access_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/access/access_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/access/access_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:51.462715 datasphere-0.7.2/yandex/cloud/priv/ai/
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:51.463027 datasphere-0.7.2/yandex/cloud/priv/ai/platform/
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:51.793960 datasphere-0.7.2/yandex/cloud/priv/ai/platform/v1/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5762 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/ai/platform/v1/project_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8938 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/ai/platform/v1/project_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/ai/platform/v1/project_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/ai/platform/v1/project_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    21479 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/ai/platform/v1/project_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    23490 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/ai/platform/v1/project_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    28428 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/ai/platform/v1/project_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11959 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/ai/platform/v1/project_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1957 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/ai/platform/v1/quota_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      166 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/ai/platform/v1/quota_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6379 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/ai/platform/v1/quota_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2764 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/ai/platform/v1/quota_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2479 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/ai/platform/v1/resource_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2109 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/ai/platform/v1/resource_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/ai/platform/v1/resource_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/ai/platform/v1/resource_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12394 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/ai/platform/v1/resource_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9656 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/ai/platform/v1/resource_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    16814 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/ai/platform/v1/resource_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7238 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/ai/platform/v1/resource_service_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:51.464184 datasphere-0.7.2/yandex/cloud/priv/console/
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:51.803548 datasphere-0.7.2/yandex/cloud/priv/console/v1/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3853 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/console/v1/access_binding_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4903 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/console/v1/access_binding_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/console/v1/access_binding_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/console/v1/access_binding_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5290 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/console/v1/form_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12845 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/console/v1/form_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/console/v1/form_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/console/v1/form_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3025 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/console/v1/resource_settings_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2765 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/console/v1/resource_settings_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/console/v1/resource_settings_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/console/v1/resource_settings_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:51.806767 datasphere-0.7.2/yandex/cloud/priv/console/v2/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6296 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/console/v2/form_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    16990 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/console/v2/form_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/console/v2/form_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/console/v2/form_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:51.465649 datasphere-0.7.2/yandex/cloud/priv/dataproc/
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:51.465299 datasphere-0.7.2/yandex/cloud/priv/dataproc/manager/
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:51.817293 datasphere-0.7.2/yandex/cloud/priv/dataproc/manager/v1/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8503 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/dataproc/manager/v1/job_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    27307 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/dataproc/manager/v1/job_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/dataproc/manager/v1/job_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/dataproc/manager/v1/job_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7819 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/dataproc/manager/v1/job_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9134 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/dataproc/manager/v1/job_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13216 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/dataproc/manager/v1/job_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6864 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/dataproc/manager/v1/job_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12676 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/dataproc/manager/v1/manager_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    31568 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/dataproc/manager/v1/manager_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13374 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/dataproc/manager/v1/manager_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7085 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/dataproc/manager/v1/manager_service_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:51.846898 datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5841 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/cluster_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    14555 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/cluster_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/cluster_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/cluster_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    24667 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/cluster_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    30846 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/cluster_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    21920 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/cluster_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11026 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/cluster_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1859 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/common_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2476 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/common_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/common_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/common_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:51.849485 datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/job_operation/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2187 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/job_operation/operation_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      738 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/job_operation/operation_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3212 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/job_operation/operation_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2039 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/job_operation/operation_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8327 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/job_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    27307 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/job_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/job_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/job_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    18092 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/job_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    16844 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/job_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    23743 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/job_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12016 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/job_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2522 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/operation_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      738 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/operation_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3080 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/operation_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1983 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/operation_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1402 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/resource_preset_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1536 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/resource_preset_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/resource_preset_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/resource_preset_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4317 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/resource_preset_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3414 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/resource_preset_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5289 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/resource_preset_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3454 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/resource_preset_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5320 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/subcluster_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8706 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/subcluster_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/subcluster_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/subcluster_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    14687 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/subcluster_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13191 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/subcluster_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12615 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/subcluster_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6472 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/subcluster_service_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:51.467339 datasphere-0.7.2/yandex/cloud/priv/datasphere/
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:51.864971 datasphere-0.7.2/yandex/cloud/priv/datasphere/v1/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2179 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v1/app_token_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      697 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v1/app_token_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2899 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v1/app_token_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1776 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v1/app_token_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5919 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v1/operation_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6258 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v1/operation_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8725 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v1/operation_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3967 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v1/operation_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3666 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v1/project_data_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3891 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v1/project_data_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5128 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v1/project_data_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2609 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v1/project_data_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4603 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v1/project_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10044 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v1/project_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v1/project_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v1/project_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    24541 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v1/project_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    23699 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v1/project_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    26233 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v1/project_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11102 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v1/project_service_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:51.999184 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2968 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/access_binding_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      838 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/access_binding_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3226 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/access_binding_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1707 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/access_binding_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2940 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/admin_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5151 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/admin_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/admin_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/admin_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1858 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/admin_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      698 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/admin_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3158 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/admin_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1659 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/admin_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1744 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/alpha_flag_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1995 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/alpha_flag_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/alpha_flag_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/alpha_flag_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3732 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/alpha_flag_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3342 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/alpha_flag_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8935 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/alpha_flag_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3996 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/alpha_flag_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4216 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/checkpoint_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8940 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/checkpoint_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/checkpoint_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/checkpoint_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    16670 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/checkpoint_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    22531 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/checkpoint_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    22907 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/checkpoint_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10053 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/checkpoint_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4388 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/community_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8562 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/community_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/community_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/community_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9325 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/community_quota_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    14063 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/community_quota_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    15703 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/community_quota_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7197 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/community_quota_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    41234 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/community_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    43622 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/community_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    74204 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/community_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    30906 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/community_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5533 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/data_proc_template_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11027 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/data_proc_template_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/data_proc_template_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/data_proc_template_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13301 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/data_proc_template_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12107 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/data_proc_template_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    19704 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/data_proc_template_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8849 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/data_proc_template_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3284 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/dataset_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5374 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/dataset_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/dataset_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/dataset_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    14406 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/dataset_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12655 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/dataset_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    36208 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/dataset_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    15498 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/dataset_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3054 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/docker_image_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5312 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/docker_image_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/docker_image_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/docker_image_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    20678 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/docker_image_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    19462 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/docker_image_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    28949 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/docker_image_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12489 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/docker_image_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4490 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/feature_property_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9583 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/feature_property_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/feature_property_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/feature_property_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5964 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/feature_property_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7982 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/feature_property_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11448 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/feature_property_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5081 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/feature_property_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4312 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/foundation_model_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8385 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/foundation_model_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/foundation_model_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/foundation_model_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11450 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/foundation_model_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    15499 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/foundation_model_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    19696 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/foundation_model_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9000 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/foundation_model_service_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:52.008038 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/internal/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3397 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/internal/community_info_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5236 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/internal/community_info_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/internal/community_info_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/internal/community_info_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7889 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/internal/project_info_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    17799 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/internal/project_info_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/internal/project_info_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/internal/project_info_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4091 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/internal/project_info_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1634 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/internal/project_info_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7526 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/internal/project_info_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3590 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/internal/project_info_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3422 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/internal_storage_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3962 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/internal_storage_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3328 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/internal_storage_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1874 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/internal_storage_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6797 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/invite_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6113 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/invite_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11164 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/invite_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5030 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/invite_service_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:52.014017 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/jobs/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9291 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/jobs/jobs_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    22514 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/jobs/jobs_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/jobs/jobs_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/jobs/jobs_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    19098 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/jobs/project_job_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    28824 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/jobs/project_job_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    35270 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/jobs/project_job_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    15679 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/jobs/project_job_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3386 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/model_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6482 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/model_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/model_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/model_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11037 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/model_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12352 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/model_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    14265 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/model_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6126 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/model_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8243 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/navigation_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12049 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/navigation_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12828 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/navigation_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5609 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/navigation_service_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:52.054172 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2546 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/billing_spec_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2126 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/billing_spec_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/billing_spec_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/billing_spec_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7543 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/docker_app_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11171 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/docker_app_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/docker_app_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/docker_app_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3489 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/healthcheck_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3942 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/healthcheck_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/healthcheck_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/healthcheck_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3638 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/instance_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4954 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/instance_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/instance_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/instance_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4197 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/instance_spec_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5151 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/instance_spec_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/instance_spec_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/instance_spec_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6231 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/node_alias_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7355 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/node_alias_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/node_alias_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/node_alias_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7247 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/node_alias_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7644 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/node_alias_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9379 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/node_alias_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4339 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/node_alias_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7987 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/node_deployer_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8549 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/node_deployer_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13689 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/node_deployer_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6285 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/node_deployer_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3423 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/node_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4115 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/node_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/node_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/node_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3322 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/node_spec_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2854 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/node_spec_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/node_spec_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/node_spec_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4276 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/policies_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4903 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/policies_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/policies_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/policies_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1588 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/runtime_options_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      652 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/runtime_options_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/runtime_options_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/runtime_options_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5122 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/servant_app_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7073 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/servant_app_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/servant_app_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/servant_app_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3635 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/triton_app_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7030 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/triton_app_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/triton_app_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/triton_app_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5664 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/project_ide_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5237 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/project_ide_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9310 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/project_ide_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4354 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/project_ide_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10444 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/project_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    22895 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/project_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/project_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/project_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    62074 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/project_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    76415 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/project_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    87993 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/project_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    37048 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/project_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11585 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/resource_actions_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    32305 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/resource_actions_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/resource_actions_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/resource_actions_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11654 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/resource_types_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    23421 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/resource_types_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/resource_types_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/resource_types_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2563 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/restrictions_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4668 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/restrictions_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/restrictions_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/restrictions_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2401 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/s3_keys_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1282 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/s3_keys_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2998 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/s3_keys_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1607 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/s3_keys_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3801 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/s3_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7191 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/s3_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/s3_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/s3_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    15821 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/s3_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    16907 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/s3_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    27459 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/s3_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11496 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/s3_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2785 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/secret_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4438 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/secret_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/secret_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/secret_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10294 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/secret_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7930 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/secret_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    16411 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/secret_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7233 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/secret_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7480 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/spark_connector_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8620 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/spark_connector_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/spark_connector_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/spark_connector_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10923 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/spark_connector_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11677 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/spark_connector_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    15539 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/spark_connector_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7009 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/spark_connector_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1446 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/user_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1092 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/user_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/user_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/user_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3899 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/user_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3052 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/user_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8621 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/user_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3770 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/user_service_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:52.057223 datasphere-0.7.2/yandex/cloud/priv/iam/
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:52.060003 datasphere-0.7.2/yandex/cloud/priv/iam/management/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1842 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/management/cache_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1299 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/management/cache_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3041 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/management/cache_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1968 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/management/cache_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6663 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/restriction_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9186 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/restriction_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/restriction_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/restriction_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:52.262608 datasphere-0.7.2/yandex/cloud/priv/iam/v1/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    20419 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/access_binding_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    27526 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/access_binding_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13351 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/access_binding_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5965 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/access_binding_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1687 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/api_key_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1945 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/api_key_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/api_key_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/api_key_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11072 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/api_key_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8448 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/api_key_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12365 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/api_key_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5310 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/api_key_service_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:52.280904 datasphere-0.7.2/yandex/cloud/priv/iam/v1/awscompatibility/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1766 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/awscompatibility/access_key_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1914 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/awscompatibility/access_key_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/awscompatibility/access_key_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/awscompatibility/access_key_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13006 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/awscompatibility/access_key_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9998 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/awscompatibility/access_key_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    15757 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/awscompatibility/access_key_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7186 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/awscompatibility/access_key_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3515 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/awscompatibility/delegation_key_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2046 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/awscompatibility/delegation_key_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3312 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/awscompatibility/delegation_key_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1915 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/awscompatibility/delegation_key_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4611 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/awscompatibility/temporary_access_key_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3491 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/awscompatibility/temporary_access_key_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3400 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/awscompatibility/temporary_access_key_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1947 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/awscompatibility/temporary_access_key_service_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:52.290038 datasphere-0.7.2/yandex/cloud/priv/iam/v1/backoffice/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7315 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/backoffice/access_binding_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9843 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/backoffice/access_binding_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5367 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/backoffice/access_binding_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2749 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/backoffice/access_binding_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4141 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/backoffice/permission_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4815 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/backoffice/permission_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3123 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/backoffice/permission_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1713 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/backoffice/permission_service_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:52.294792 datasphere-0.7.2/yandex/cloud/priv/iam/v1/compute/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10397 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/compute/os_login_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12623 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/compute/os_login_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8942 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/compute/os_login_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4284 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/compute/os_login_service_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:52.321677 datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4711 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/access_binding_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5177 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/access_binding_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5722 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/access_binding_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3554 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/access_binding_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3249 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/key_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1994 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/key_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2956 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/key_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1559 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/key_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3854 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/membership_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3267 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/membership_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3063 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/membership_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1820 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/membership_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2137 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/os_login_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1323 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/os_login_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3007 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/os_login_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1764 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/os_login_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3905 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/role_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4223 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/role_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4893 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/role_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2523 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/role_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7585 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/service_account_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5598 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/service_account_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7360 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/service_account_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3668 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/service_account_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2439 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/user_account_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      955 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/user_account_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3238 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/user_account_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1903 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/user_account_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4863 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/gizmo_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3148 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/gizmo_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5144 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/gizmo_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2479 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/gizmo_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6233 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/iam_cookie_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6400 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/iam_cookie_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8930 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/iam_cookie_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4143 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/iam_cookie_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2962 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/iam_credential_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1776 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/iam_credential_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3144 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/iam_credential_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1693 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/iam_credential_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4722 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/iam_session_token_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3041 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/iam_session_token_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3115 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/iam_session_token_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1937 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/iam_session_token_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    17389 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/iam_token_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    17269 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/iam_token_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    18896 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/iam_token_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9387 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/iam_token_service_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:52.328446 datasphere-0.7.2/yandex/cloud/priv/iam/v1/inner/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3215 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/inner/service_registry_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3953 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/inner/service_registry_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/inner/service_registry_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/inner/service_registry_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13970 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/inner/service_registry_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10870 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/inner/service_registry_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    14973 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/inner/service_registry_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6423 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/inner/service_registry_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2341 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/key_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3745 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/key_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/key_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/key_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13653 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/key_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11972 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/key_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    14022 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/key_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5878 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/key_service_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:52.331429 datasphere-0.7.2/yandex/cloud/priv/iam/v1/maintenance/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1785 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/maintenance/metadata_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1860 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/maintenance/metadata_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/maintenance/metadata_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/maintenance/metadata_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6828 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/membership_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6683 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/membership_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7267 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/membership_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4094 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/membership_service_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:52.342717 datasphere-0.7.2/yandex/cloud/priv/iam/v1/mfa/
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:52.346425 datasphere-0.7.2/yandex/cloud/priv/iam/v1/mfa/console/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4476 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/mfa/console/totp_profile_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4837 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/mfa/console/totp_profile_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5480 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/mfa/console/totp_profile_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3615 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/mfa/console/totp_profile_service_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:52.353181 datasphere-0.7.2/yandex/cloud/priv/iam/v1/mfa/hardware/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3216 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/mfa/hardware/totp_profile_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4660 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/mfa/hardware/totp_profile_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/mfa/hardware/totp_profile_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/mfa/hardware/totp_profile_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    24492 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/mfa/hardware/totp_profile_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    21229 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/mfa/hardware/totp_profile_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    23761 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/mfa/hardware/totp_profile_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12614 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/mfa/hardware/totp_profile_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2091 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/mfa/operation_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      687 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/mfa/operation_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3028 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/mfa/operation_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1586 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/mfa/operation_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3062 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/mfa/totp_profile_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5764 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/mfa/totp_profile_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/mfa/totp_profile_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/mfa/totp_profile_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9376 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/mfa/totp_profile_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9082 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/mfa/totp_profile_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    15464 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/mfa/totp_profile_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8966 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/mfa/totp_profile_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2066 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/oauth_client_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4656 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/oauth_client_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/oauth_client_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/oauth_client_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    15285 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/oauth_client_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13367 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/oauth_client_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12466 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/oauth_client_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5401 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/oauth_client_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1345 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/oauth_scope_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1228 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/oauth_scope_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/oauth_scope_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/oauth_scope_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7990 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/oauth_scope_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7215 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/oauth_scope_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10574 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/oauth_scope_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4625 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/oauth_scope_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2457 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/operation_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      687 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/operation_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2980 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/operation_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1570 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/operation_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1299 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/os_login_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      888 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/os_login_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/os_login_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/os_login_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5980 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/os_login_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4920 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/os_login_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6765 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/os_login_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3060 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/os_login_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1249 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/permission_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      725 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/permission_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/permission_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/permission_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6963 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/permission_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5725 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/permission_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10526 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/permission_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4600 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/permission_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3420 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/permission_stage_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4264 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/permission_stage_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/permission_stage_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/permission_stage_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6787 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/permission_stage_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5637 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/permission_stage_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8996 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/permission_stage_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4131 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/permission_stage_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2904 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/quota_limit_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      166 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/quota_limit_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8522 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/quota_limit_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3821 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/quota_limit_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1794 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/quota_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      166 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/quota_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6323 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/quota_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2764 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/quota_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4088 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/refresh_token_issue_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2806 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/refresh_token_issue_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3234 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/refresh_token_issue_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1816 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/refresh_token_issue_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8051 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/refresh_token_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9586 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/refresh_token_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5029 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/refresh_token_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2490 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/refresh_token_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2020 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/resource_boundary_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1022 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/resource_boundary_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/resource_boundary_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/resource_boundary_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1787 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/resource_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      820 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/resource_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/resource_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/resource_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1298 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/resource_type_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      876 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/resource_type_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/resource_type_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/resource_type_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10194 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/resource_type_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8808 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/resource_type_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    14808 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/resource_type_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6452 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/resource_type_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1817 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/restriction_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1626 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/restriction_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/restriction_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/restriction_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12853 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/restriction_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11981 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/restriction_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12870 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/restriction_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5695 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/restriction_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2432 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/restriction_type_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4629 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/restriction_type_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/restriction_type_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/restriction_type_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    16936 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/restriction_type_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    17238 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/restriction_type_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    17177 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/restriction_type_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7798 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/restriction_type_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1739 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/revoked_credential_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2197 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/revoked_credential_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/revoked_credential_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/revoked_credential_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1587 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/role_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2154 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/role_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/role_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/role_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    14082 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/role_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    14017 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/role_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    19538 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/role_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8002 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/role_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3993 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/root_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2470 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/root_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5121 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/root_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2461 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/root_service_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:52.369262 datasphere-0.7.2/yandex/cloud/priv/iam/v1/saml/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1803 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/saml/certificate_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2648 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/saml/certificate_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/saml/certificate_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/saml/certificate_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12270 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/saml/certificate_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8283 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/saml/certificate_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12943 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/saml/certificate_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5852 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/saml/certificate_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3070 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/saml/federation_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7156 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/saml/federation_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/saml/federation_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/saml/federation_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    19637 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/saml/federation_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    16002 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/saml/federation_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    19103 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/saml/federation_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8309 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/saml/federation_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2110 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/service_account_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2571 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/service_account_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/service_account_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/service_account_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    23376 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/service_account_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    14997 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/service_account_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    32314 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/service_account_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13727 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/service_account_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4541 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/service_control_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9023 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/service_control_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/service_control_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/service_control_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    35409 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/service_control_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    39042 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/service_control_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    42084 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/service_control_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    17665 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/service_control_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1800 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/ssh_key_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1494 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/ssh_key_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/ssh_key_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/ssh_key_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7460 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/ssh_key_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7777 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/ssh_key_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10494 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/ssh_key_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4549 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/ssh_key_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1688 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/subject_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2416 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/subject_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/subject_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/subject_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    19400 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/subject_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    26591 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/subject_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    16449 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/subject_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8715 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/subject_service_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:52.373292 datasphere-0.7.2/yandex/cloud/priv/iam/v1/token/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1767 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/token/iam_token_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1010 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/token/iam_token_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/token/iam_token_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/token/iam_token_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2200 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/token_agent_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1631 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/token_agent_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2788 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/token_agent_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1623 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/token_agent_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:52.407311 datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3651 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/agreement_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1284 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/agreement_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7376 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/agreement_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3706 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/agreement_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2710 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/auth_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1252 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/auth_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3014 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/auth_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1696 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/auth_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2833 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/health_check_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1957 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/health_check_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3179 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/health_check_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1734 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/health_check_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4164 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/passport_federation_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3230 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/passport_federation_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3334 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/passport_federation_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1776 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/passport_federation_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6081 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/policy_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5439 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/policy_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13083 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/policy_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5920 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/policy_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2418 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/roles_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1960 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/roles_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3020 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/roles_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1614 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/roles_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4268 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/service_account_access_key_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4220 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/service_account_access_key_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7626 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/service_account_access_key_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3720 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/service_account_access_key_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7133 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/user_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6911 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/user_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11106 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/user_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5022 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/user_service_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:52.411466 datasphere-0.7.2/yandex/cloud/priv/iam/v1/ts/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2581 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/ts/iam_token_service_subject_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2068 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/ts/iam_token_service_subject_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/ts/iam_token_service_subject_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/ts/iam_token_service_subject_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4652 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/user_account_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6814 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/user_account_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/user_account_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/user_account_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10219 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/user_account_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10216 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/user_account_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10807 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/user_account_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4754 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/user_account_service_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:52.419760 datasphere-0.7.2/yandex/cloud/priv/iam/v1/workload/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1681 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/workload/federated_credential_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1528 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/workload/federated_credential_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/workload/federated_credential_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/workload/federated_credential_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9085 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/workload/federated_credential_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6933 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/workload/federated_credential_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11852 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/workload/federated_credential_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5630 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/workload/federated_credential_service_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:52.428455 datasphere-0.7.2/yandex/cloud/priv/iam/v1/workload/oidc/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2211 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/workload/oidc/federation_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2863 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/workload/oidc/federation_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/workload/oidc/federation_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/workload/oidc/federation_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11277 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/workload/oidc/federation_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8949 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/workload/oidc/federation_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11214 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/workload/oidc/federation_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4950 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/workload/oidc/federation_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/yandex_passport_cookie_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1715 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/yandex_passport_cookie_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/yandex_passport_cookie_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/yandex_passport_cookie_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5811 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/yandex_passport_user_account_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3965 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/yandex_passport_user_account_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7412 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/yandex_passport_user_account_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3657 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/iam/v1/yandex_passport_user_account_service_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:52.432851 datasphere-0.7.2/yandex/cloud/priv/oauth/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8516 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/oauth/claims_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13189 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/oauth/claims_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/oauth/claims_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/oauth/claims_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:52.453186 datasphere-0.7.2/yandex/cloud/priv/oauth/v1/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3834 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/oauth/v1/claim_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5858 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/oauth/v1/claim_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2871 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/oauth/v1/claim_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1528 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/oauth/v1/claim_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2204 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/oauth/v1/cloud_user_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2418 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/oauth/v1/cloud_user_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/oauth/v1/cloud_user_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/oauth/v1/cloud_user_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4519 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/oauth/v1/login_history_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4058 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/oauth/v1/login_history_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5062 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/oauth/v1/login_history_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3288 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/oauth/v1/login_history_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1887 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/oauth/v1/oauth_request_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1192 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/oauth/v1/oauth_request_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/oauth/v1/oauth_request_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/oauth/v1/oauth_request_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12256 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/oauth/v1/session_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    16448 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/oauth/v1/session_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13682 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/oauth/v1/session_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9862 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/oauth/v1/session_service_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:52.456519 datasphere-0.7.2/yandex/cloud/priv/operation/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2057 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/operation/operation_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2678 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/operation/operation_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/operation/operation_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/operation/operation_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:52.463628 datasphere-0.7.2/yandex/cloud/priv/quota/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7135 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/quota/quota_limit_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9425 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/quota/quota_limit_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/quota/quota_limit_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/quota/quota_limit_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6853 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/quota/quota_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11292 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/quota/quota_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/quota/quota_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/quota/quota_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:52.466955 datasphere-0.7.2/yandex/cloud/priv/reference/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1762 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/reference/reference_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2597 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/reference/reference_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/reference/reference_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/reference/reference_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1953 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/sensitive_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2595 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/sensitive_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/sensitive_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/sensitive_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:51.481820 datasphere-0.7.2/yandex/cloud/priv/servicecontrol/
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-05-28 13:24:52.475819 datasphere-0.7.2/yandex/cloud/priv/servicecontrol/v1/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    17172 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/servicecontrol/v1/access_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    23231 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/servicecontrol/v1/access_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9486 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/servicecontrol/v1/access_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/servicecontrol/v1/access_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2246 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/servicecontrol/v1/resource_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1428 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/servicecontrol/v1/resource_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/servicecontrol/v1/resource_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/servicecontrol/v1/resource_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2111 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/validation_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2479 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/validation_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/validation_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/priv/validation_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2132 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/validation_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2479 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/validation_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/validation_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      413 2024-05-03 10:44:08.000000 datasphere-0.7.2/yandex/cloud/validation_pb2_grpc.pyi
```

### Comparing `datasphere-0.7.1/PKG-INFO` & `datasphere-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasphere
-Version: 0.7.1
+Version: 0.7.2
 Summary: Yandex Cloud DataSphere
 Author: Yandex LLC
 Author-email: cloud@support.yandex.ru
 License: Apache-2.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `datasphere-0.7.1/README.md` & `datasphere-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/datasphere/api/__init__.py` & `datasphere-0.7.2/datasphere/api/__init__.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/datasphere/changelog.md` & `datasphere-0.7.2/datasphere/changelog.md`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/datasphere/channel.py` & `datasphere-0.7.2/datasphere/channel.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/datasphere/client.py` & `datasphere-0.7.2/datasphere/client.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/datasphere/config.py` & `datasphere-0.7.2/datasphere/config.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/datasphere/files.py` & `datasphere-0.7.2/datasphere/files.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/datasphere/fork.py` & `datasphere-0.7.2/datasphere/fork.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/datasphere/logs/config.py` & `datasphere-0.7.2/datasphere/logs/config.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/datasphere/logs/logging.yaml` & `datasphere-0.7.2/datasphere/logs/logging.yaml`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/datasphere/main.py` & `datasphere-0.7.2/datasphere/main.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/datasphere/output.py` & `datasphere-0.7.2/datasphere/output.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from dataclasses import dataclass
 from enum import Enum
 from typing import Callable, List, Optional, Union, TextIO
 
 from google.protobuf.timestamp_pb2 import Timestamp
 from tabulate import tabulate
 
-from datasphere.api import jobs_pb2, project_pb2, env, ServerEnv
+from datasphere.api import jobs_pb2, project_pb2, use_private_api
 
 
 class Format(Enum):
     TABLE = 'table'
     JSON = 'json'
 
 
@@ -31,15 +31,15 @@
         name: str  # for json/yaml/whatever output
         title: str  # for table output
 
     fields: List[Field]
 
 
 # TODO: delete after renaming `description` -> `desc` in private-api
-job_desc_attr = 'desc' if env == ServerEnv.PROD else 'description'
+job_desc_attr = 'description' if use_private_api else 'desc'
 
 
 job_spec = OutputEntitySpec(
     fields=[
         OutputEntitySpec.Field(lambda job: job.id, 'id', 'ID'),
         OutputEntitySpec.Field(lambda job: job.name, 'name', 'Name'),
         OutputEntitySpec.Field(lambda job: getattr(job, job_desc_attr), 'desc', 'Description'),
```

### Comparing `datasphere-0.7.1/datasphere/pyenv.py` & `datasphere-0.7.2/datasphere/pyenv.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/datasphere/sdk.py` & `datasphere-0.7.2/datasphere/sdk.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/datasphere/utils.py` & `datasphere-0.7.2/datasphere/utils.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/datasphere/validation.py` & `datasphere-0.7.2/datasphere/validation.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/datasphere.egg-info/PKG-INFO` & `datasphere-0.7.2/datasphere.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasphere
-Version: 0.7.1
+Version: 0.7.2
 Summary: Yandex Cloud DataSphere
 Author: Yandex LLC
 Author-email: cloud@support.yandex.ru
 License: Apache-2.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `datasphere-0.7.1/datasphere.egg-info/SOURCES.txt` & `datasphere-0.7.2/datasphere.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/setup.py` & `datasphere-0.7.2/setup.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/tests/test_config.py` & `datasphere-0.7.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/tests/test_files.py` & `datasphere-0.7.2/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/tests/test_fork.py` & `datasphere-0.7.2/tests/test_fork.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/tests/test_main.py` & `datasphere-0.7.2/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/tests/test_output.py` & `datasphere-0.7.2/tests/test_output.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/tests/test_pyenv.py` & `datasphere-0.7.2/tests/test_pyenv.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/tests/test_utils.py` & `datasphere-0.7.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/tests/test_validation.py` & `datasphere-0.7.2/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/access/access_pb2.py` & `datasphere-0.7.2/yandex/cloud/access/access_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/access/access_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/access/access_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/api/operation_pb2.py` & `datasphere-0.7.2/yandex/cloud/api/operation_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/api/operation_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/api/operation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/api/tools/options_pb2.py` & `datasphere-0.7.2/yandex/cloud/api/tools/options_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/api/tools/options_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/api/tools/options_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v1/app_token_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/datasphere/v1/app_token_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v1/app_token_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/datasphere/v1/app_token_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v1/app_token_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/datasphere/v1/app_token_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v1/app_token_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/datasphere/v1/app_token_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v1/folder_budget_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/datasphere/v1/folder_budget_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v1/folder_budget_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/datasphere/v1/folder_budget_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v1/folder_budget_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/datasphere/v1/folder_budget_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v1/folder_budget_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/datasphere/v1/folder_budget_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v1/node_execution_error_details_pb2.py` & `datasphere-0.7.2/yandex/cloud/datasphere/v1/node_execution_error_details_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v1/node_execution_error_details_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/datasphere/v1/node_execution_error_details_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v1/node_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/datasphere/v1/node_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v1/node_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/datasphere/v1/node_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v1/node_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/datasphere/v1/node_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v1/node_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/datasphere/v1/node_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v1/project_data_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/datasphere/v1/project_data_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v1/project_data_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/datasphere/v1/project_data_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v1/project_data_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/datasphere/v1/project_data_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v1/project_data_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/datasphere/v1/project_data_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v1/project_pb2.py` & `datasphere-0.7.2/yandex/cloud/datasphere/v1/project_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v1/project_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/datasphere/v1/project_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v1/project_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/datasphere/v1/project_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v1/project_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/datasphere/v1/project_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v1/project_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/datasphere/v1/project_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v1/project_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/datasphere/v1/project_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v2/community_pb2.py` & `datasphere-0.7.2/yandex/cloud/datasphere/v2/community_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v2/community_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/datasphere/v2/community_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v2/community_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/datasphere/v2/community_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v2/community_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/datasphere/v2/community_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v2/community_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/datasphere/v2/community_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v2/community_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/datasphere/v2/community_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v2/dataset_pb2.py` & `datasphere-0.7.2/yandex/cloud/datasphere/v2/dataset_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v2/dataset_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/datasphere/v2/dataset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v2/dataset_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/datasphere/v2/dataset_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v2/dataset_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/datasphere/v2/dataset_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v2/dataset_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/datasphere/v2/dataset_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v2/dataset_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/datasphere/v2/dataset_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v2/docker_image_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/datasphere/v2/docker_image_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v2/docker_image_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/datasphere/v2/docker_image_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v2/docker_image_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/datasphere/v2/docker_image_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v2/docker_image_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/datasphere/v2/docker_image_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v2/jobs/jobs_pb2.py` & `datasphere-0.7.2/yandex/cloud/datasphere/v2/jobs/jobs_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v2/jobs/jobs_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/datasphere/v2/jobs/jobs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v2/jobs/project_job_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/datasphere/v2/jobs/project_job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v2/jobs/project_job_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/datasphere/v2/jobs/project_job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v2/jobs/project_job_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/datasphere/v2/jobs/project_job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v2/jobs/project_job_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/datasphere/v2/jobs/project_job_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v2/project_pb2.py` & `datasphere-0.7.2/yandex/cloud/datasphere/v2/project_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v2/project_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/datasphere/v2/project_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v2/project_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/datasphere/v2/project_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v2/project_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/datasphere/v2/project_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v2/project_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/datasphere/v2/project_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v2/project_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/datasphere/v2/project_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v2/resource_types_pb2.py` & `datasphere-0.7.2/yandex/cloud/datasphere/v2/resource_types_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v2/resource_types_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/datasphere/v2/resource_types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v2/restrictions_pb2.py` & `datasphere-0.7.2/yandex/cloud/datasphere/v2/restrictions_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v2/restrictions_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/datasphere/v2/restrictions_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v2/s3_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/datasphere/v2/s3_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v2/s3_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/datasphere/v2/s3_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v2/s3_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/datasphere/v2/s3_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v2/s3_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/datasphere/v2/s3_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v2/secret_pb2.py` & `datasphere-0.7.2/yandex/cloud/datasphere/v2/secret_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v2/secret_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/datasphere/v2/secret_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v2/user_pb2.py` & `datasphere-0.7.2/yandex/cloud/datasphere/v2/user_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/datasphere/v2/user_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/datasphere/v2/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/api_key_pb2.py` & `datasphere-0.7.2/yandex/cloud/iam/v1/api_key_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/api_key_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/iam/v1/api_key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/api_key_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/iam/v1/api_key_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/api_key_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/iam/v1/api_key_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/api_key_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/iam/v1/api_key_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/api_key_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/iam/v1/api_key_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/awscompatibility/access_key_pb2.py` & `datasphere-0.7.2/yandex/cloud/iam/v1/awscompatibility/access_key_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/awscompatibility/access_key_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/iam/v1/awscompatibility/access_key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/awscompatibility/access_key_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/iam/v1/awscompatibility/access_key_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/awscompatibility/access_key_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/iam/v1/awscompatibility/access_key_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/awscompatibility/access_key_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/iam/v1/awscompatibility/access_key_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/awscompatibility/access_key_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/iam/v1/awscompatibility/access_key_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/iam_token_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/iam/v1/iam_token_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/iam_token_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/iam/v1/iam_token_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/iam_token_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/iam/v1/iam_token_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/iam_token_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/iam/v1/iam_token_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/key_pb2.py` & `datasphere-0.7.2/yandex/cloud/iam/v1/key_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/key_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/iam/v1/key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/key_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/iam/v1/key_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/key_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/iam/v1/key_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/key_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/iam/v1/key_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/key_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/iam/v1/key_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/resource_pb2.py` & `datasphere-0.7.2/yandex/cloud/iam/v1/resource_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/resource_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/iam/v1/resource_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/role_pb2.py` & `datasphere-0.7.2/yandex/cloud/iam/v1/role_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/role_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/iam/v1/role_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/role_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/iam/v1/role_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/role_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/iam/v1/role_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/role_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/iam/v1/role_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/role_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/iam/v1/role_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/saml/certificate_pb2.py` & `datasphere-0.7.2/yandex/cloud/iam/v1/saml/certificate_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/saml/certificate_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/iam/v1/saml/certificate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/saml/certificate_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/iam/v1/saml/certificate_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/saml/certificate_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/iam/v1/saml/certificate_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/saml/certificate_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/iam/v1/saml/certificate_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/saml/certificate_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/iam/v1/saml/certificate_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/saml/federation_pb2.py` & `datasphere-0.7.2/yandex/cloud/iam/v1/saml/federation_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/saml/federation_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/iam/v1/saml/federation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/saml/federation_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/iam/v1/saml/federation_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/saml/federation_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/iam/v1/saml/federation_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/saml/federation_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/iam/v1/saml/federation_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/saml/federation_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/iam/v1/saml/federation_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/service_account_pb2.py` & `datasphere-0.7.2/yandex/cloud/iam/v1/service_account_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/service_account_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/iam/v1/service_account_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/service_account_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/iam/v1/service_account_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/service_account_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/iam/v1/service_account_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/service_account_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/iam/v1/service_account_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/service_account_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/iam/v1/service_account_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/service_control_pb2.py` & `datasphere-0.7.2/yandex/cloud/iam/v1/service_control_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/service_control_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/iam/v1/service_control_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/service_control_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/iam/v1/service_control_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/service_control_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/iam/v1/service_control_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/service_control_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/iam/v1/service_control_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/service_control_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/iam/v1/service_control_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/user_account_pb2.py` & `datasphere-0.7.2/yandex/cloud/iam/v1/user_account_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/user_account_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/iam/v1/user_account_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/user_account_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/iam/v1/user_account_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/user_account_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/iam/v1/user_account_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/user_account_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/iam/v1/user_account_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/user_account_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/iam/v1/user_account_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/yandex_passport_user_account_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/iam/v1/yandex_passport_user_account_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/yandex_passport_user_account_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/iam/v1/yandex_passport_user_account_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/yandex_passport_user_account_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/iam/v1/yandex_passport_user_account_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/iam/v1/yandex_passport_user_account_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/iam/v1/yandex_passport_user_account_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/operation/operation_pb2.py` & `datasphere-0.7.2/yandex/cloud/operation/operation_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/operation/operation_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/operation/operation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/operation/operation_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/operation/operation_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/operation/operation_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/operation/operation_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/operation/operation_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/operation/operation_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/operation/operation_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/operation/operation_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/access/access_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/access/access_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/access/access_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/access/access_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/ai/platform/v1/project_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/ai/platform/v1/project_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/ai/platform/v1/project_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/ai/platform/v1/project_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/ai/platform/v1/project_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/ai/platform/v1/project_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/ai/platform/v1/project_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/ai/platform/v1/project_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/ai/platform/v1/project_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/ai/platform/v1/project_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/ai/platform/v1/project_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/ai/platform/v1/project_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/ai/platform/v1/quota_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/ai/platform/v1/quota_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/ai/platform/v1/quota_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/ai/platform/v1/quota_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/ai/platform/v1/quota_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/ai/platform/v1/quota_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/ai/platform/v1/resource_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/ai/platform/v1/resource_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/ai/platform/v1/resource_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/ai/platform/v1/resource_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/ai/platform/v1/resource_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/ai/platform/v1/resource_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/ai/platform/v1/resource_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/ai/platform/v1/resource_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/ai/platform/v1/resource_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/ai/platform/v1/resource_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/ai/platform/v1/resource_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/ai/platform/v1/resource_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/console/v1/access_binding_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/console/v1/access_binding_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/console/v1/access_binding_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/console/v1/access_binding_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/console/v1/form_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/console/v1/form_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/console/v1/form_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/console/v1/form_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/console/v1/resource_settings_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/console/v1/resource_settings_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/console/v1/resource_settings_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/console/v1/resource_settings_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/console/v2/form_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/console/v2/form_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/console/v2/form_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/console/v2/form_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/dataproc/manager/v1/job_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/dataproc/manager/v1/job_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/dataproc/manager/v1/job_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/dataproc/manager/v1/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/dataproc/manager/v1/job_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/dataproc/manager/v1/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/dataproc/manager/v1/job_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/dataproc/manager/v1/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/dataproc/manager/v1/job_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/dataproc/manager/v1/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/dataproc/manager/v1/job_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/dataproc/manager/v1/job_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/dataproc/manager/v1/manager_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/dataproc/manager/v1/manager_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/dataproc/manager/v1/manager_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/dataproc/manager/v1/manager_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/dataproc/manager/v1/manager_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/dataproc/manager/v1/manager_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/dataproc/manager/v1/manager_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/dataproc/manager/v1/manager_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/cluster_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/cluster_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/cluster_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/cluster_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/cluster_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/cluster_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/cluster_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/cluster_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/cluster_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/cluster_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/cluster_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/cluster_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/common_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/common_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/job_operation/operation_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/job_operation/operation_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/job_operation/operation_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/job_operation/operation_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/job_operation/operation_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/job_operation/operation_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/job_operation/operation_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/job_operation/operation_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/job_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/job_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/job_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/job_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/job_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/job_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/job_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/job_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/operation_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/operation_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/operation_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/operation_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/operation_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/operation_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/operation_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/operation_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/resource_preset_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/resource_preset_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/resource_preset_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/resource_preset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/resource_preset_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/resource_preset_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/resource_preset_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/resource_preset_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/resource_preset_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/resource_preset_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/resource_preset_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/resource_preset_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/subcluster_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/subcluster_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/subcluster_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/subcluster_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/subcluster_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/subcluster_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/subcluster_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/subcluster_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/subcluster_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/subcluster_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/dataproc/v1/subcluster_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/dataproc/v1/subcluster_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v1/app_token_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v1/app_token_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v1/app_token_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v1/app_token_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v1/app_token_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v1/app_token_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v1/app_token_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v1/app_token_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v1/operation_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v1/operation_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v1/operation_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v1/operation_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v1/operation_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v1/operation_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v1/operation_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v1/operation_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v1/project_data_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v1/project_data_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v1/project_data_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v1/project_data_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v1/project_data_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v1/project_data_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v1/project_data_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v1/project_data_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v1/project_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v1/project_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v1/project_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v1/project_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v1/project_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v1/project_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v1/project_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v1/project_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v1/project_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v1/project_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v1/project_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v1/project_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/access_binding_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/access_binding_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/access_binding_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/access_binding_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/access_binding_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/access_binding_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/access_binding_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/access_binding_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/admin_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/admin_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/admin_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/admin_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/admin_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/admin_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/admin_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/admin_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/admin_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/admin_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/admin_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/admin_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/alpha_flag_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/alpha_flag_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/alpha_flag_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/alpha_flag_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/alpha_flag_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/alpha_flag_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/alpha_flag_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/alpha_flag_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/alpha_flag_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/alpha_flag_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/alpha_flag_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/alpha_flag_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/checkpoint_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/checkpoint_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/checkpoint_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/checkpoint_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/checkpoint_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/checkpoint_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/checkpoint_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/checkpoint_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/checkpoint_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/checkpoint_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/checkpoint_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/checkpoint_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/community_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/community_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/community_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/community_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/community_quota_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/community_quota_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/community_quota_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/community_quota_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/community_quota_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/community_quota_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/community_quota_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/community_quota_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/community_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/community_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/community_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/community_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/community_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/community_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/community_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/community_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/data_proc_template_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/data_proc_template_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/data_proc_template_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/data_proc_template_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/data_proc_template_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/data_proc_template_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/data_proc_template_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/data_proc_template_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/data_proc_template_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/data_proc_template_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/data_proc_template_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/data_proc_template_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/dataset_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/dataset_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/dataset_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/dataset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/dataset_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/dataset_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/dataset_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/dataset_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/dataset_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/dataset_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/dataset_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/dataset_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/docker_image_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/docker_image_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/docker_image_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/docker_image_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/docker_image_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/docker_image_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/docker_image_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/docker_image_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/docker_image_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/docker_image_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/docker_image_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/docker_image_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/feature_property_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/feature_property_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/feature_property_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/feature_property_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/feature_property_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/feature_property_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/feature_property_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/feature_property_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/feature_property_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/feature_property_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/feature_property_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/feature_property_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/foundation_model_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/foundation_model_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/foundation_model_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/foundation_model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/foundation_model_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/foundation_model_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/foundation_model_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/foundation_model_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/foundation_model_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/foundation_model_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/foundation_model_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/foundation_model_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/internal/community_info_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/internal/community_info_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/internal/community_info_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/internal/community_info_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/internal/project_info_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/internal/project_info_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/internal/project_info_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/internal/project_info_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/internal/project_info_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/internal/project_info_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/internal/project_info_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/internal/project_info_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/internal/project_info_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/internal/project_info_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/internal/project_info_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/internal/project_info_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/internal_storage_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/internal_storage_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/internal_storage_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/internal_storage_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/internal_storage_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/internal_storage_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/internal_storage_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/internal_storage_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/invite_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/invite_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/invite_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/invite_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/invite_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/invite_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/invite_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/invite_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/jobs/jobs_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/jobs/jobs_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/jobs/jobs_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/jobs/jobs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/jobs/project_job_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/jobs/project_job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/jobs/project_job_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/jobs/project_job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/jobs/project_job_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/jobs/project_job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/jobs/project_job_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/jobs/project_job_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/model_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/model_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/model_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/model_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/model_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/model_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/model_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/model_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/model_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/model_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/model_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/navigation_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/navigation_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/navigation_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/navigation_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/navigation_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/navigation_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/navigation_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/navigation_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/billing_spec_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/billing_spec_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/billing_spec_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/billing_spec_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/docker_app_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/docker_app_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/docker_app_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/docker_app_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/healthcheck_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/healthcheck_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/healthcheck_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/healthcheck_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/instance_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/instance_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/instance_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/instance_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/instance_spec_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/instance_spec_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/instance_spec_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/instance_spec_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/node_alias_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/node_alias_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/node_alias_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/node_alias_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/node_alias_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/node_alias_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/node_alias_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/node_alias_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/node_alias_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/node_alias_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/node_alias_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/node_alias_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/node_deployer_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/node_deployer_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/node_deployer_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/node_deployer_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/node_deployer_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/node_deployer_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/node_deployer_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/node_deployer_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/node_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/node_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/node_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/node_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/node_spec_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/node_spec_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/node_spec_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/node_spec_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/policies_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/policies_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/policies_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/policies_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/runtime_options_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/runtime_options_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/runtime_options_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/runtime_options_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/servant_app_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/servant_app_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/servant_app_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/servant_app_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/triton_app_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/triton_app_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/nodedeployer/triton_app_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/nodedeployer/triton_app_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/project_ide_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/project_ide_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/project_ide_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/project_ide_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/project_ide_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/project_ide_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/project_ide_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/project_ide_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/project_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/project_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/project_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/project_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/project_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/project_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/project_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/project_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/project_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/project_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/project_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/project_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/resource_actions_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/resource_actions_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/resource_actions_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/resource_actions_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/resource_types_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/resource_types_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/resource_types_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/resource_types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/restrictions_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/restrictions_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/restrictions_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/restrictions_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/s3_keys_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/s3_keys_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/s3_keys_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/s3_keys_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/s3_keys_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/s3_keys_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/s3_keys_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/s3_keys_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/s3_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/s3_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/s3_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/s3_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/s3_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/s3_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/s3_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/s3_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/s3_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/s3_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/s3_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/s3_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/secret_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/secret_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/secret_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/secret_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/secret_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/secret_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/secret_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/secret_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/secret_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/secret_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/secret_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/secret_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/spark_connector_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/spark_connector_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/spark_connector_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/spark_connector_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/spark_connector_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/spark_connector_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/spark_connector_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/spark_connector_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/spark_connector_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/spark_connector_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/spark_connector_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/spark_connector_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/user_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/user_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/user_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/user_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/user_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/user_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/datasphere/v2/user_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/datasphere/v2/user_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/management/cache_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/management/cache_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/management/cache_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/management/cache_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/management/cache_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/management/cache_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/management/cache_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/management/cache_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/restriction_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/restriction_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/restriction_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/restriction_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/access_binding_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/access_binding_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/access_binding_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/access_binding_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/access_binding_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/access_binding_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/access_binding_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/access_binding_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/api_key_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/api_key_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/api_key_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/api_key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/api_key_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/api_key_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/api_key_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/api_key_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/api_key_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/api_key_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/api_key_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/api_key_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/awscompatibility/access_key_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/awscompatibility/access_key_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/awscompatibility/access_key_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/awscompatibility/access_key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/awscompatibility/access_key_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/awscompatibility/access_key_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/awscompatibility/access_key_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/awscompatibility/access_key_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/awscompatibility/access_key_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/awscompatibility/access_key_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/awscompatibility/access_key_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/awscompatibility/access_key_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/awscompatibility/delegation_key_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/awscompatibility/delegation_key_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/awscompatibility/delegation_key_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/awscompatibility/delegation_key_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/awscompatibility/delegation_key_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/awscompatibility/delegation_key_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/awscompatibility/delegation_key_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/awscompatibility/delegation_key_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/awscompatibility/temporary_access_key_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/awscompatibility/temporary_access_key_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/awscompatibility/temporary_access_key_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/awscompatibility/temporary_access_key_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/awscompatibility/temporary_access_key_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/awscompatibility/temporary_access_key_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/awscompatibility/temporary_access_key_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/awscompatibility/temporary_access_key_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/backoffice/access_binding_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/backoffice/access_binding_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/backoffice/access_binding_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/backoffice/access_binding_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/backoffice/access_binding_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/backoffice/access_binding_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/backoffice/access_binding_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/backoffice/access_binding_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/backoffice/permission_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/backoffice/permission_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/backoffice/permission_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/backoffice/permission_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/backoffice/permission_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/backoffice/permission_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/backoffice/permission_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/backoffice/permission_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/compute/os_login_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/compute/os_login_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/compute/os_login_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/compute/os_login_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/compute/os_login_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/compute/os_login_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/compute/os_login_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/compute/os_login_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/access_binding_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/access_binding_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/access_binding_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/access_binding_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/access_binding_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/access_binding_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/access_binding_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/access_binding_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/key_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/key_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/key_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/key_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/key_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/key_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/key_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/key_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/membership_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/membership_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/membership_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/membership_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/membership_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/membership_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/membership_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/membership_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/os_login_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/os_login_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/os_login_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/os_login_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/os_login_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/os_login_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/os_login_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/os_login_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/role_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/role_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/role_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/role_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/role_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/role_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/role_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/role_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/service_account_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/service_account_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/service_account_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/service_account_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/service_account_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/service_account_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/service_account_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/service_account_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/user_account_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/user_account_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/user_account_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/user_account_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/user_account_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/user_account_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/console/user_account_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/console/user_account_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/gizmo_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/gizmo_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/gizmo_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/gizmo_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/gizmo_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/gizmo_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/gizmo_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/gizmo_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/iam_cookie_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/iam_cookie_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/iam_cookie_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/iam_cookie_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/iam_cookie_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/iam_cookie_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/iam_cookie_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/iam_cookie_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/iam_credential_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/iam_credential_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/iam_credential_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/iam_credential_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/iam_credential_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/iam_credential_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/iam_credential_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/iam_credential_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/iam_session_token_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/iam_session_token_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/iam_session_token_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/iam_session_token_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/iam_session_token_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/iam_session_token_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/iam_session_token_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/iam_session_token_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/iam_token_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/iam_token_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/iam_token_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/iam_token_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/iam_token_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/iam_token_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/iam_token_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/iam_token_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/inner/service_registry_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/inner/service_registry_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/inner/service_registry_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/inner/service_registry_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/inner/service_registry_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/inner/service_registry_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/inner/service_registry_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/inner/service_registry_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/inner/service_registry_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/inner/service_registry_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/inner/service_registry_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/inner/service_registry_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/key_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/key_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/key_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/key_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/key_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/key_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/key_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/key_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/key_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/key_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/key_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/maintenance/metadata_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/maintenance/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/maintenance/metadata_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/maintenance/metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/membership_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/membership_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/membership_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/membership_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/membership_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/membership_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/membership_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/membership_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/mfa/console/totp_profile_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/mfa/console/totp_profile_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/mfa/console/totp_profile_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/mfa/console/totp_profile_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/mfa/console/totp_profile_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/mfa/console/totp_profile_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/mfa/console/totp_profile_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/mfa/console/totp_profile_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/mfa/hardware/totp_profile_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/mfa/hardware/totp_profile_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/mfa/hardware/totp_profile_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/mfa/hardware/totp_profile_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/mfa/hardware/totp_profile_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/mfa/hardware/totp_profile_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/mfa/hardware/totp_profile_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/mfa/hardware/totp_profile_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/mfa/hardware/totp_profile_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/mfa/hardware/totp_profile_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/mfa/hardware/totp_profile_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/mfa/hardware/totp_profile_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/mfa/operation_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/mfa/operation_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/mfa/operation_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/mfa/operation_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/mfa/operation_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/mfa/operation_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/mfa/operation_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/mfa/operation_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/mfa/totp_profile_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/mfa/totp_profile_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/mfa/totp_profile_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/mfa/totp_profile_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/mfa/totp_profile_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/mfa/totp_profile_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/mfa/totp_profile_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/mfa/totp_profile_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/mfa/totp_profile_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/mfa/totp_profile_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/mfa/totp_profile_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/mfa/totp_profile_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/oauth_client_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/oauth_client_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/oauth_client_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/oauth_client_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/oauth_client_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/oauth_client_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/oauth_client_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/oauth_client_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/oauth_client_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/oauth_client_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/oauth_client_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/oauth_client_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/oauth_scope_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/oauth_scope_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/oauth_scope_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/oauth_scope_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/oauth_scope_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/oauth_scope_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/oauth_scope_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/oauth_scope_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/oauth_scope_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/oauth_scope_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/oauth_scope_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/oauth_scope_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/operation_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/operation_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/operation_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/operation_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/operation_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/operation_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/operation_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/operation_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/os_login_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/os_login_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/os_login_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/os_login_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/os_login_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/os_login_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/os_login_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/os_login_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/os_login_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/os_login_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/os_login_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/os_login_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/permission_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/permission_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/permission_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/permission_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/permission_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/permission_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/permission_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/permission_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/permission_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/permission_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/permission_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/permission_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/permission_stage_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/permission_stage_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/permission_stage_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/permission_stage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/permission_stage_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/permission_stage_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/permission_stage_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/permission_stage_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/permission_stage_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/permission_stage_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/permission_stage_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/permission_stage_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/quota_limit_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/quota_limit_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/quota_limit_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/quota_limit_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/quota_limit_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/quota_limit_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/quota_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/quota_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/quota_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/quota_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/quota_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/quota_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/refresh_token_issue_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/refresh_token_issue_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/refresh_token_issue_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/refresh_token_issue_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/refresh_token_issue_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/refresh_token_issue_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/refresh_token_issue_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/refresh_token_issue_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/refresh_token_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/refresh_token_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/refresh_token_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/refresh_token_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/refresh_token_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/refresh_token_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/refresh_token_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/refresh_token_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/resource_boundary_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/resource_boundary_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/resource_boundary_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/resource_boundary_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/resource_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/resource_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/resource_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/resource_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/resource_type_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/resource_type_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/resource_type_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/resource_type_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/resource_type_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/resource_type_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/resource_type_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/resource_type_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/resource_type_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/resource_type_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/resource_type_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/resource_type_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/restriction_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/restriction_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/restriction_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/restriction_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/restriction_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/restriction_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/restriction_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/restriction_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/restriction_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/restriction_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/restriction_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/restriction_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/restriction_type_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/restriction_type_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/restriction_type_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/restriction_type_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/restriction_type_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/restriction_type_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/restriction_type_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/restriction_type_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/restriction_type_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/restriction_type_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/restriction_type_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/restriction_type_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/revoked_credential_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/revoked_credential_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/revoked_credential_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/revoked_credential_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/role_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/role_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/role_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/role_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/role_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/role_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/role_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/role_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/role_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/role_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/role_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/role_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/root_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/root_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/root_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/root_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/root_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/root_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/root_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/root_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/saml/certificate_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/saml/certificate_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/saml/certificate_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/saml/certificate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/saml/certificate_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/saml/certificate_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/saml/certificate_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/saml/certificate_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/saml/certificate_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/saml/certificate_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/saml/certificate_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/saml/certificate_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/saml/federation_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/saml/federation_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/saml/federation_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/saml/federation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/saml/federation_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/saml/federation_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/saml/federation_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/saml/federation_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/saml/federation_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/saml/federation_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/saml/federation_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/saml/federation_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/service_account_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/service_account_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/service_account_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/service_account_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/service_account_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/service_account_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/service_account_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/service_account_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/service_account_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/service_account_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/service_account_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/service_account_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/service_control_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/service_control_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/service_control_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/service_control_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/service_control_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/service_control_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/service_control_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/service_control_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/service_control_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/service_control_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/service_control_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/service_control_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/ssh_key_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/ssh_key_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/ssh_key_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/ssh_key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/ssh_key_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/ssh_key_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/ssh_key_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/ssh_key_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/ssh_key_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/ssh_key_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/ssh_key_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/ssh_key_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/subject_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/subject_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/subject_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/subject_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/subject_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/subject_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/subject_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/subject_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/subject_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/subject_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/subject_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/subject_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/token/iam_token_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/token/iam_token_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/token/iam_token_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/token/iam_token_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/token_agent_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/token_agent_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/token_agent_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/token_agent_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/token_agent_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/token_agent_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/token_agent_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/token_agent_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/agreement_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/agreement_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/agreement_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/agreement_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/agreement_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/agreement_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/agreement_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/agreement_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/auth_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/auth_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/auth_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/auth_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/auth_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/auth_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/auth_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/auth_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/health_check_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/health_check_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/health_check_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/health_check_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/health_check_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/health_check_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/health_check_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/health_check_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/passport_federation_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/passport_federation_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/passport_federation_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/passport_federation_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/passport_federation_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/passport_federation_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/passport_federation_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/passport_federation_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/policy_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/policy_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/policy_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/policy_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/policy_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/policy_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/policy_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/policy_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/roles_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/roles_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/roles_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/roles_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/roles_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/roles_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/roles_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/roles_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/service_account_access_key_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/service_account_access_key_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/service_account_access_key_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/service_account_access_key_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/service_account_access_key_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/service_account_access_key_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/service_account_access_key_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/service_account_access_key_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/user_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/user_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/user_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/transitional/user_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/transitional/user_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/ts/iam_token_service_subject_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/ts/iam_token_service_subject_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/ts/iam_token_service_subject_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/ts/iam_token_service_subject_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/user_account_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/user_account_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/user_account_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/user_account_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/user_account_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/user_account_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/user_account_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/user_account_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/user_account_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/user_account_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/user_account_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/user_account_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/workload/federated_credential_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/workload/federated_credential_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/workload/federated_credential_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/workload/federated_credential_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/workload/federated_credential_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/workload/federated_credential_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/workload/federated_credential_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/workload/federated_credential_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/workload/federated_credential_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/workload/federated_credential_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/workload/federated_credential_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/workload/federated_credential_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/workload/oidc/federation_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/workload/oidc/federation_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/workload/oidc/federation_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/workload/oidc/federation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/workload/oidc/federation_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/workload/oidc/federation_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/workload/oidc/federation_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/workload/oidc/federation_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/workload/oidc/federation_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/workload/oidc/federation_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/workload/oidc/federation_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/workload/oidc/federation_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/yandex_passport_cookie_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/yandex_passport_cookie_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/yandex_passport_cookie_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/yandex_passport_cookie_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/yandex_passport_user_account_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/yandex_passport_user_account_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/yandex_passport_user_account_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/yandex_passport_user_account_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/yandex_passport_user_account_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/yandex_passport_user_account_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/iam/v1/yandex_passport_user_account_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/iam/v1/yandex_passport_user_account_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/oauth/claims_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/oauth/claims_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/oauth/claims_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/oauth/claims_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/oauth/v1/claim_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/oauth/v1/claim_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/oauth/v1/claim_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/oauth/v1/claim_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/oauth/v1/claim_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/oauth/v1/claim_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/oauth/v1/claim_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/oauth/v1/claim_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/oauth/v1/cloud_user_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/oauth/v1/cloud_user_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/oauth/v1/cloud_user_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/oauth/v1/cloud_user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/oauth/v1/login_history_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/oauth/v1/login_history_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/oauth/v1/login_history_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/oauth/v1/login_history_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/oauth/v1/login_history_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/oauth/v1/login_history_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/oauth/v1/login_history_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/oauth/v1/login_history_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/oauth/v1/oauth_request_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/oauth/v1/oauth_request_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/oauth/v1/oauth_request_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/oauth/v1/oauth_request_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/oauth/v1/session_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/oauth/v1/session_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/oauth/v1/session_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/oauth/v1/session_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/oauth/v1/session_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/oauth/v1/session_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/oauth/v1/session_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/oauth/v1/session_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/operation/operation_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/operation/operation_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/operation/operation_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/operation/operation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/quota/quota_limit_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/quota/quota_limit_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/quota/quota_limit_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/quota/quota_limit_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/quota/quota_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/quota/quota_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/quota/quota_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/quota/quota_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/reference/reference_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/reference/reference_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/reference/reference_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/reference/reference_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/sensitive_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/sensitive_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/sensitive_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/sensitive_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/servicecontrol/v1/access_service_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/servicecontrol/v1/access_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/servicecontrol/v1/access_service_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/servicecontrol/v1/access_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/servicecontrol/v1/access_service_pb2_grpc.py` & `datasphere-0.7.2/yandex/cloud/priv/servicecontrol/v1/access_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/servicecontrol/v1/access_service_pb2_grpc.pyi` & `datasphere-0.7.2/yandex/cloud/priv/servicecontrol/v1/access_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/servicecontrol/v1/resource_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/servicecontrol/v1/resource_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/servicecontrol/v1/resource_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/servicecontrol/v1/resource_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/validation_pb2.py` & `datasphere-0.7.2/yandex/cloud/priv/validation_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/priv/validation_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/priv/validation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/validation_pb2.py` & `datasphere-0.7.2/yandex/cloud/validation_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.7.1/yandex/cloud/validation_pb2.pyi` & `datasphere-0.7.2/yandex/cloud/validation_pb2.pyi`

 * *Files identical despite different names*

