# Comparing `tmp/viggocore-1.2.9.tar.gz` & `tmp/viggocore-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viggocore-1.2.9.tar", last modified: Fri Jan 26 13:46:51 2024, max compression
+gzip compressed data, was "viggocore-1.3.0.tar", last modified: Tue May 28 17:30:05 2024, max compression
```

## Comparing `viggocore-1.2.9.tar` & `viggocore-1.3.0.tar`

### file list

```diff
@@ -1,176 +1,176 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.174111 viggocore-1.2.9/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-01-26 13:46:15.000000 viggocore-1.2.9/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-26 13:46:15.000000 viggocore-1.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-01-26 13:46:51.174111 viggocore-1.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-01-26 13:46:15.000000 viggocore-1.2.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-26 13:46:51.174111 viggocore-1.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-01-26 13:46:15.000000 viggocore-1.2.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.158111 viggocore-1.2.9/viggocore/
--rw-r--r--   0 runner    (1001) docker     (127)     4917 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.158111 viggocore-1.2.9/viggocore/bootstrap/
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/bootstrap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.162111 viggocore-1.2.9/viggocore/bootstrap/default/
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/bootstrap/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/bootstrap/default/application.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/bootstrap/default/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/bootstrap/default/policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/bootstrap/default/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/bootstrap/roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/bootstrap/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/celery.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.162111 viggocore-1.2.9/viggocore/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/common/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/common/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/common/input.py
--rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/common/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/common/operation_after_post.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.162111 viggocore-1.2.9/viggocore/common/subsystem/
--rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/common/subsystem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/common/subsystem/apihandler.py
--rw-r--r--   0 runner    (1001) docker     (127)    11474 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/common/subsystem/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     7069 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/common/subsystem/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/common/subsystem/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/common/subsystem/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/common/subsystem/operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/common/subsystem/pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/common/subsystem/router.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/common/subsystem/transaction_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.162111 viggocore-1.2.9/viggocore/subsystem/
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.162111 viggocore-1.2.9/viggocore/subsystem/application/
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/application/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    10433 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/application/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/application/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/application/router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.162111 viggocore-1.2.9/viggocore/subsystem/capability/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/capability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/capability/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/capability/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.166111 viggocore-1.2.9/viggocore/subsystem/constant_for_calculation/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/constant_for_calculation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/constant_for_calculation/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/constant_for_calculation/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/constant_for_calculation/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/constant_for_calculation/router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.166111 viggocore-1.2.9/viggocore/subsystem/domain/
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12501 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/domain/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.166111 viggocore-1.2.9/viggocore/subsystem/domain/files/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/domain/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/domain/files/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    25868 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/domain/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/domain/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/domain/router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.166111 viggocore-1.2.9/viggocore/subsystem/domain/sql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/domain/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/domain/sql/disk_space_totals_by_db.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/domain/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.166111 viggocore-1.2.9/viggocore/subsystem/domain_and_table_sequence/
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/domain_and_table_sequence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/domain_and_table_sequence/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/domain_and_table_sequence/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/domain_and_table_sequence/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/domain_and_table_sequence/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/domain_and_table_sequence/router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.166111 viggocore-1.2.9/viggocore/subsystem/domain_sequence/
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/domain_sequence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/domain_sequence/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/domain_sequence/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/domain_sequence/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/domain_sequence/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/domain_sequence/router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.166111 viggocore-1.2.9/viggocore/subsystem/file/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/file/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/file/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/file/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.166111 viggocore-1.2.9/viggocore/subsystem/file_sync/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/file_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/file_sync/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.166111 viggocore-1.2.9/viggocore/subsystem/grant/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/grant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/grant/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.170112 viggocore-1.2.9/viggocore/subsystem/image/
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/image/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/image/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/image/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/image/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/image/router.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/image/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.170112 viggocore-1.2.9/viggocore/subsystem/notification/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/notification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/notification/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.170112 viggocore-1.2.9/viggocore/subsystem/policy/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/policy/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.170112 viggocore-1.2.9/viggocore/subsystem/project_cost/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/project_cost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/project_cost/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/project_cost/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.170112 viggocore-1.2.9/viggocore/subsystem/registration/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/registration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/registration/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/registration/router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.170112 viggocore-1.2.9/viggocore/subsystem/role/
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/role/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/role/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/role/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/role/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/role/router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.170112 viggocore-1.2.9/viggocore/subsystem/route/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/route/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/route/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/route/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.170112 viggocore-1.2.9/viggocore/subsystem/tag/
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/tag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/tag/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/tag/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/tag/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/tag/router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.170112 viggocore-1.2.9/viggocore/subsystem/timeline_event/
--rwxr-xr-x   0 runner    (1001) docker     (127)      312 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/timeline_event/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1696 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/timeline_event/controller.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2767 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/timeline_event/manager.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2798 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/timeline_event/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.170112 viggocore-1.2.9/viggocore/subsystem/token/
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/token/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/token/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/token/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/token/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/token/router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.174111 viggocore-1.2.9/viggocore/subsystem/user/
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9627 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/user/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     5493 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/user/email.py
--rw-r--r--   0 runner    (1001) docker     (127)    10413 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/user/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/user/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/user/router.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/system.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.174111 viggocore-1.2.9/viggocore/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.174111 viggocore-1.2.9/viggocore/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/tests/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/tests/functional/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/tests/functional/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/tests/functional/test_domains.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/tests/functional/test_grants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/tests/functional/test_grants_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/tests/functional/test_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/tests/functional/test_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/tests/functional/test_users.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.158111 viggocore-1.2.9/viggocore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-01-26 13:46:51.000000 viggocore-1.2.9/viggocore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5488 2024-01-26 13:46:51.000000 viggocore-1.2.9/viggocore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-26 13:46:51.000000 viggocore-1.2.9/viggocore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-01-26 13:46:51.000000 viggocore-1.2.9/viggocore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-01-26 13:46:51.000000 viggocore-1.2.9/viggocore.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:30:05.383789 viggocore-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-28 17:29:38.000000 viggocore-1.3.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-28 17:29:38.000000 viggocore-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-28 17:30:05.383789 viggocore-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-28 17:29:38.000000 viggocore-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 17:30:05.383789 viggocore-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-28 17:29:38.000000 viggocore-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:30:05.359789 viggocore-1.3.0/viggocore/
+-rw-r--r--   0 runner    (1001) docker     (127)     4917 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:30:05.363788 viggocore-1.3.0/viggocore/bootstrap/
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/bootstrap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:30:05.363788 viggocore-1.3.0/viggocore/bootstrap/default/
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/bootstrap/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/bootstrap/default/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/bootstrap/default/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/bootstrap/default/policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/bootstrap/default/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/bootstrap/roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/bootstrap/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/celery.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:30:05.363788 viggocore-1.3.0/viggocore/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/common/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/common/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/common/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/common/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/common/operation_after_post.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:30:05.367789 viggocore-1.3.0/viggocore/common/subsystem/
+-rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/common/subsystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/common/subsystem/apihandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11474 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/common/subsystem/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7069 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/common/subsystem/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/common/subsystem/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/common/subsystem/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/common/subsystem/operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/common/subsystem/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/common/subsystem/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/common/subsystem/transaction_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:30:05.367789 viggocore-1.3.0/viggocore/subsystem/
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:30:05.367789 viggocore-1.3.0/viggocore/subsystem/application/
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/application/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10433 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/application/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/application/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/application/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:30:05.367789 viggocore-1.3.0/viggocore/subsystem/capability/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/capability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/capability/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/capability/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:30:05.367789 viggocore-1.3.0/viggocore/subsystem/constant_for_calculation/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/constant_for_calculation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/constant_for_calculation/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/constant_for_calculation/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/constant_for_calculation/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/constant_for_calculation/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:30:05.371789 viggocore-1.3.0/viggocore/subsystem/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12996 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/domain/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:30:05.371789 viggocore-1.3.0/viggocore/subsystem/domain/files/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/domain/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/domain/files/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26854 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/domain/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/domain/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/domain/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:30:05.371789 viggocore-1.3.0/viggocore/subsystem/domain/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/domain/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/domain/sql/disk_space_totals_by_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/domain/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:30:05.371789 viggocore-1.3.0/viggocore/subsystem/domain_and_table_sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/domain_and_table_sequence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/domain_and_table_sequence/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/domain_and_table_sequence/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/domain_and_table_sequence/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/domain_and_table_sequence/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/domain_and_table_sequence/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:30:05.371789 viggocore-1.3.0/viggocore/subsystem/domain_sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/domain_sequence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/domain_sequence/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/domain_sequence/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/domain_sequence/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/domain_sequence/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/domain_sequence/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:30:05.371789 viggocore-1.3.0/viggocore/subsystem/file/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/file/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/file/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/file/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:30:05.371789 viggocore-1.3.0/viggocore/subsystem/file_sync/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/file_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/file_sync/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:30:05.375789 viggocore-1.3.0/viggocore/subsystem/grant/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/grant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/grant/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:30:05.375789 viggocore-1.3.0/viggocore/subsystem/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/image/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/image/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/image/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/image/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/image/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/image/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:30:05.375789 viggocore-1.3.0/viggocore/subsystem/notification/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/notification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/notification/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:30:05.375789 viggocore-1.3.0/viggocore/subsystem/policy/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/policy/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:30:05.375789 viggocore-1.3.0/viggocore/subsystem/project_cost/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/project_cost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/project_cost/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/project_cost/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:30:05.375789 viggocore-1.3.0/viggocore/subsystem/registration/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/registration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/registration/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/registration/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:30:05.375789 viggocore-1.3.0/viggocore/subsystem/role/
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/role/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/role/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/role/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/role/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/role/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:30:05.375789 viggocore-1.3.0/viggocore/subsystem/route/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/route/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/route/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/route/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:30:05.379789 viggocore-1.3.0/viggocore/subsystem/tag/
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/tag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/tag/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/tag/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/tag/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/tag/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:30:05.379789 viggocore-1.3.0/viggocore/subsystem/timeline_event/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      312 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/timeline_event/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1696 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/timeline_event/controller.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2767 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/timeline_event/manager.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2798 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/timeline_event/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:30:05.379789 viggocore-1.3.0/viggocore/subsystem/token/
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/token/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/token/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/token/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/token/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/token/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:30:05.379789 viggocore-1.3.0/viggocore/subsystem/user/
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9627 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/user/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5493 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/user/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10413 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/user/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/user/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/subsystem/user/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:30:05.379789 viggocore-1.3.0/viggocore/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:30:05.379789 viggocore-1.3.0/viggocore/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/tests/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/tests/functional/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/tests/functional/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/tests/functional/test_domains.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/tests/functional/test_grants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/tests/functional/test_grants_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/tests/functional/test_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/tests/functional/test_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-28 17:29:38.000000 viggocore-1.3.0/viggocore/tests/functional/test_users.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:30:05.363788 viggocore-1.3.0/viggocore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-28 17:30:05.000000 viggocore-1.3.0/viggocore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5488 2024-05-28 17:30:05.000000 viggocore-1.3.0/viggocore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 17:30:05.000000 viggocore-1.3.0/viggocore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-28 17:30:05.000000 viggocore-1.3.0/viggocore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-28 17:30:05.000000 viggocore-1.3.0/viggocore.egg-info/top_level.txt
```

### Comparing `viggocore-1.2.9/LICENSE` & `viggocore-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/README.md` & `viggocore-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/setup.py` & `viggocore-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/__init__.py` & `viggocore-1.3.0/viggocore/__init__.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/bootstrap/__init__.py` & `viggocore-1.3.0/viggocore/bootstrap/__init__.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/bootstrap/default/__init__.py` & `viggocore-1.3.0/viggocore/bootstrap/default/__init__.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/bootstrap/default/application.py` & `viggocore-1.3.0/viggocore/bootstrap/default/application.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/bootstrap/default/domain.py` & `viggocore-1.3.0/viggocore/bootstrap/default/domain.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/bootstrap/default/policies.py` & `viggocore-1.3.0/viggocore/bootstrap/default/policies.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/bootstrap/default/user.py` & `viggocore-1.3.0/viggocore/bootstrap/default/user.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/bootstrap/roles.py` & `viggocore-1.3.0/viggocore/bootstrap/roles.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/bootstrap/routes.py` & `viggocore-1.3.0/viggocore/bootstrap/routes.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/celery.py` & `viggocore-1.3.0/viggocore/celery.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/common/controller.py` & `viggocore-1.3.0/viggocore/common/controller.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/common/exception.py` & `viggocore-1.3.0/viggocore/common/exception.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/common/input.py` & `viggocore-1.3.0/viggocore/common/input.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/common/manager.py` & `viggocore-1.3.0/viggocore/common/manager.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/common/operation_after_post.py` & `viggocore-1.3.0/viggocore/common/operation_after_post.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/common/subsystem/__init__.py` & `viggocore-1.3.0/viggocore/common/subsystem/__init__.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/common/subsystem/apihandler.py` & `viggocore-1.3.0/viggocore/common/subsystem/apihandler.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/common/subsystem/controller.py` & `viggocore-1.3.0/viggocore/common/subsystem/controller.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/common/subsystem/driver.py` & `viggocore-1.3.0/viggocore/common/subsystem/driver.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/common/subsystem/entity.py` & `viggocore-1.3.0/viggocore/common/subsystem/entity.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/common/subsystem/manager.py` & `viggocore-1.3.0/viggocore/common/subsystem/manager.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/common/subsystem/operation.py` & `viggocore-1.3.0/viggocore/common/subsystem/operation.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/common/subsystem/pagination.py` & `viggocore-1.3.0/viggocore/common/subsystem/pagination.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/common/subsystem/router.py` & `viggocore-1.3.0/viggocore/common/subsystem/router.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/common/utils.py` & `viggocore-1.3.0/viggocore/common/utils.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/queue.py` & `viggocore-1.3.0/viggocore/queue.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/request.py` & `viggocore-1.3.0/viggocore/request.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/resources.py` & `viggocore-1.3.0/viggocore/resources.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/scheduler.py` & `viggocore-1.3.0/viggocore/scheduler.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/subsystem/application/controller.py` & `viggocore-1.3.0/viggocore/subsystem/application/controller.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/subsystem/application/manager.py` & `viggocore-1.3.0/viggocore/subsystem/application/manager.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/subsystem/application/resource.py` & `viggocore-1.3.0/viggocore/subsystem/application/resource.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/subsystem/application/router.py` & `viggocore-1.3.0/viggocore/subsystem/application/router.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/subsystem/capability/manager.py` & `viggocore-1.3.0/viggocore/subsystem/capability/manager.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/subsystem/capability/resource.py` & `viggocore-1.3.0/viggocore/subsystem/capability/resource.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/subsystem/constant_for_calculation/controller.py` & `viggocore-1.3.0/viggocore/subsystem/constant_for_calculation/controller.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/subsystem/constant_for_calculation/manager.py` & `viggocore-1.3.0/viggocore/subsystem/constant_for_calculation/manager.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/subsystem/constant_for_calculation/resource.py` & `viggocore-1.3.0/viggocore/subsystem/constant_for_calculation/resource.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/subsystem/constant_for_calculation/router.py` & `viggocore-1.3.0/viggocore/subsystem/constant_for_calculation/router.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/subsystem/domain/controller.py` & `viggocore-1.3.0/viggocore/subsystem/domain/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -321,7 +321,20 @@
                                             'total': total}})
         else:
             response = {self.collection_wrap: entities, 'totals': totals}
 
         return flask.Response(response=utils.to_json(response),
                               status=200,
                               mimetype="application/json")
+
+    def get_roles(self, id: str):
+        try:
+            roles = self.manager.get_roles(id=id)
+            response = {"roles": [role.to_dict() for role in roles]}
+
+        except exception.ViggoCoreException as exc:
+            return flask.Response(response=exc.message,
+                                  status=exc.status)
+
+        return flask.Response(response=utils.to_json(response),
+                              status=200,
+                              mimetype="application/json")
```

### Comparing `viggocore-1.2.9/viggocore/subsystem/domain/manager.py` & `viggocore-1.3.0/viggocore/subsystem/domain/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,19 @@
+from sqlalchemy import and_
 from viggocore.common import exception
+from viggocore.subsystem.application.resource import Application
+from viggocore.subsystem.capability.resource import Capability
 from viggocore.subsystem.domain import tasks
-from viggocore.common.subsystem import operation, manager
+from viggocore.common.subsystem import operation
+from viggocore.common import manager
 from viggocore.subsystem.image.resource import QualityImage
 from viggocore.subsystem.domain.files import utils
 from viggocore.common.utils import round_abnt
+from viggocore.subsystem.policy.resource import Policy
+from viggocore.subsystem.role.resource import Role
 
 
 class DomainByName(operation.Operation):
 
     def pre(self, session, domain_name, **kwargs):
         self.domain_name = domain_name
         return True
@@ -267,15 +273,15 @@
 
 class GetFilesSize(operation.Get):
 
     def pre(self, session, id, **kwargs):
         return super().pre(session, id=id)
 
     def do(self, session, **kwargs):
-        response_dict = utils.get_size(domain_id=self.id)
+        response_dict = utils.get_size(domain_id=self.id, **kwargs)
         return response_dict
 
 
 class GetUsageInfoByDomain(operation.List):
 
     PRECISION = 2
 
@@ -433,15 +439,15 @@
                 dc['total_space_disc_bank'] += total_space_disc_bank
                 dc['total_process'] += total_process
                 dc['total_acess_db'] += total_acess_db
 
             # calcula o espaço ocupado por arquivos no servidor para este
             # domínio
             dc['total_space_disc_file'] = self.manager.get_files_size(
-                id=dc['domain_id']).get('BYTES', 0)
+                id=dc['domain_id'], de=self.de, ate=self.ate).get('BYTES', 0)
 
             # faz a somatória total de todos os campos
             grand_totals_dict['total_entities'] += dc['total_entities']
             grand_totals_dict['total_space_disc_bank'] += \
                 dc['total_space_disc_bank']
             grand_totals_dict['total_process'] += dc['total_process']
             grand_totals_dict['total_acess_db'] += dc['total_acess_db']
@@ -533,14 +539,16 @@
 
     def fill_in_percentages(self, response, grand_totals_dict):
         total_entities = grand_totals_dict['total_entities']
         total_space_disc_bank = grand_totals_dict['total_space_disc_bank']
         total_process = grand_totals_dict['total_process']
         total_acess_db = grand_totals_dict['total_acess_db']
         total_space_disc_file = grand_totals_dict['total_space_disc_file']
+        if total_space_disc_file == 0:
+            total_space_disc_file = 1
 
         for i in range(0, len(response)):
             response[i]['percent_total_entities'] = (
                 response[i]['total_entities'] / total_entities)
             response[i]['percent_total_space_disc_bank'] = (
                 response[i]['total_space_disc_bank'] / total_space_disc_bank)
             response[i]['percent_total_process'] = (
@@ -597,16 +605,16 @@
             self.cost_servidor = 0
         if self.cost_operacional is None:
             self.cost_operacional = 0
         if self.cost_administrativo is None:
             self.cost_administrativo = 0
 
     def pre(self, **kwargs):
-        self.de = kwargs.get('de', '2020-01-01')
-        self.ate = kwargs.get('ate', '9020-01-01')
+        self.de = kwargs.get('de', '2020-01-01-0300')
+        self.ate = kwargs.get('ate', '9020-01-01-0300')
         self.domain_name = kwargs.get('domain_name', None)
 
         session = kwargs.get('session', None)
 
         self.p_storage_bank = float(kwargs.get('p_storage_bank', 0.1))
         self.p_storage_file = float(kwargs.get('p_storage_file', 0.1))
         self.p_process = float(kwargs.get('p_process', 0.3))
@@ -645,15 +653,32 @@
         grand_totals_dict['p_process'] = self.p_process
         grand_totals_dict['p_access_db'] = self.p_access_db
         grand_totals_dict = self._normalize_values_grand_totals_dict(
             grand_totals_dict)
         return (response, grand_totals_dict)
 
 
-class Manager(manager.Manager):
+class GetRoles(operation.Operation):
+
+    def pre(self, session, id, **kwargs):
+        self.entity = self.driver.get(id, session=session)
+        return self.entity is not None
+
+    def do(self, session, **kwargs):
+        roles = session.query(Role). \
+            join(Policy). \
+            join(Capability). \
+            join(Application). \
+            filter(and_(Capability.application_id == self.entity.application_id,
+                        Role.name != Role.USER)). \
+            distinct()
+        return roles
+
+
+class Manager(manager.CommonManager):
 
     def __init__(self, driver):
         super(Manager, self).__init__(driver)
         self.domain_by_name = DomainByName(self)
         self.domain_logo_by_name = DomainLogoByName(self)
         self.upload_logo = UploadLogo(self)
         self.remove_logo = RemoveLogo(self)
@@ -661,7 +686,8 @@
         self.activate = Activate(self)
         self.update_settings = UpdateSettings(self)
         self.remove_settings = RemoveSettings(self)
         self.get_domain_settings_by_keys = GetDomainSettingsByKeys(self)
         self.send_email_activate_account = SendEmailActivateAccount(self)
         self.get_files_size = GetFilesSize(self)
         self.get_usage_info_by_domain = GetUsageInfoByDomain(self)
+        self.get_roles = GetRoles(self)
```

### Comparing `viggocore-1.2.9/viggocore/subsystem/domain/resource.py` & `viggocore-1.3.0/viggocore/subsystem/domain/resource.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/subsystem/domain/router.py` & `viggocore-1.3.0/viggocore/subsystem/domain/router.py`

 * *Files 6% similar despite different names*

```diff
@@ -93,9 +93,15 @@
                 'callback': 'get_files_size'
             },
             {
                 'action': 'Get usage infos by Domain',
                 'method': 'GET',
                 'url': self.collection_url + '/get_usage_info_by_domain',
                 'callback': 'get_usage_info_by_domain'
+            },
+            {
+                'action': 'Lista papéis pesquisando por domínio',
+                'method': 'GET',
+                'url': self.resource_url + '/roles',
+                'callback': 'get_roles'
             }
         ]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `viggocore-1.2.9/viggocore/subsystem/domain/tasks.py` & `viggocore-1.3.0/viggocore/subsystem/domain/tasks.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/subsystem/domain_and_table_sequence/controller.py` & `viggocore-1.3.0/viggocore/subsystem/domain_and_table_sequence/controller.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/subsystem/domain_and_table_sequence/manager.py` & `viggocore-1.3.0/viggocore/subsystem/domain_and_table_sequence/manager.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/subsystem/domain_and_table_sequence/resource.py` & `viggocore-1.3.0/viggocore/subsystem/domain_sequence/resource.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,46 +1,41 @@
 from sqlalchemy import UniqueConstraint
 
 from viggocore.database import db
 from viggocore.common.subsystem import entity
 
 
-class DomainAndTableSequence(entity.Entity, db.Model):
+class DomainSequence(entity.Entity, db.Model):
 
-    attributes = ['domain_id', 'table_id', 'name', 'value']
+    attributes = ['domain_id', 'name', 'value']
     attributes += entity.Entity.attributes
 
     domain_id = db.Column(
         db.CHAR(32), db.ForeignKey('domain.id'), nullable=False)
-    table_id = db.Column(db.CHAR(32), nullable=False)
     name = db.Column(db.String(100), nullable=False)
     value = db.Column(db.Numeric(10), default=0, nullable=False)
 
     __table_args__ = (
         UniqueConstraint(
             'name',
-            'table_id',
             'domain_id',
-            name='domain_and_table_sequence_name_table_id_domain_id_uk'),)
+            name='domain_sequence_name_domain_id_uk'),)
 
-    def __init__(self, id, domain_id, table_id, name, value,
+    def __init__(self, id, domain_id, name, value,
                  active=True, created_at=None, created_by=None,
                  updated_at=None, updated_by=None, tag=None):
         super().__init__(id, active, created_at, created_by,
                          updated_at, updated_by, tag)
         self.domain_id = domain_id
-        self.table_id = table_id
         self.name = name
         self.value = value
 
     @classmethod
     def individual(cls):
-        return 'domain_and_table_sequence'
+        return 'domain_sequence'
 
     def is_stable(self):
         domain_id_stable = self.domain_id is not None
-        table_id_stable = self.table_id is not None
         name_stable = self.name is not None
         value_stable = self.value is not None and self.value >= 0
 
-        return domain_id_stable and table_id_stable \
-            and name_stable and value_stable
+        return domain_id_stable and name_stable and value_stable
```

### Comparing `viggocore-1.2.9/viggocore/subsystem/domain_and_table_sequence/router.py` & `viggocore-1.3.0/viggocore/subsystem/domain_and_table_sequence/router.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/subsystem/domain_sequence/controller.py` & `viggocore-1.3.0/viggocore/subsystem/domain_sequence/controller.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/subsystem/domain_sequence/manager.py` & `viggocore-1.3.0/viggocore/subsystem/domain_sequence/manager.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/subsystem/domain_sequence/resource.py` & `viggocore-1.3.0/viggocore/subsystem/domain_and_table_sequence/resource.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,46 @@
 from sqlalchemy import UniqueConstraint
 
 from viggocore.database import db
 from viggocore.common.subsystem import entity
 
 
-class DomainSequence(entity.Entity, db.Model):
+class DomainAndTableSequence(entity.Entity, db.Model):
 
-    attributes = ['domain_id', 'name', 'value']
+    attributes = ['domain_id', 'table_id', 'name', 'value']
     attributes += entity.Entity.attributes
 
     domain_id = db.Column(
         db.CHAR(32), db.ForeignKey('domain.id'), nullable=False)
+    table_id = db.Column(db.String(100), nullable=False)
     name = db.Column(db.String(100), nullable=False)
     value = db.Column(db.Numeric(10), default=0, nullable=False)
 
     __table_args__ = (
         UniqueConstraint(
             'name',
+            'table_id',
             'domain_id',
-            name='domain_sequence_name_domain_id_uk'),)
+            name='domain_and_table_sequence_name_table_id_domain_id_uk'),)
 
-    def __init__(self, id, domain_id, name, value,
+    def __init__(self, id, domain_id, table_id, name, value,
                  active=True, created_at=None, created_by=None,
                  updated_at=None, updated_by=None, tag=None):
         super().__init__(id, active, created_at, created_by,
                          updated_at, updated_by, tag)
         self.domain_id = domain_id
+        self.table_id = table_id
         self.name = name
         self.value = value
 
     @classmethod
     def individual(cls):
-        return 'domain_sequence'
+        return 'domain_and_table_sequence'
 
     def is_stable(self):
         domain_id_stable = self.domain_id is not None
+        table_id_stable = self.table_id is not None
         name_stable = self.name is not None
         value_stable = self.value is not None and self.value >= 0
 
-        return domain_id_stable and name_stable and value_stable
+        return domain_id_stable and table_id_stable \
+            and name_stable and value_stable
```

### Comparing `viggocore-1.2.9/viggocore/subsystem/domain_sequence/router.py` & `viggocore-1.3.0/viggocore/subsystem/domain_sequence/router.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/subsystem/file/controller.py` & `viggocore-1.3.0/viggocore/subsystem/file/controller.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/subsystem/file/manager.py` & `viggocore-1.3.0/viggocore/subsystem/file/manager.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/subsystem/file/resource.py` & `viggocore-1.3.0/viggocore/subsystem/file/resource.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/subsystem/file_sync/resource.py` & `viggocore-1.3.0/viggocore/subsystem/file_sync/resource.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/subsystem/grant/resource.py` & `viggocore-1.3.0/viggocore/subsystem/grant/resource.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/subsystem/image/controller.py` & `viggocore-1.3.0/viggocore/subsystem/image/controller.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/subsystem/image/handler.py` & `viggocore-1.3.0/viggocore/subsystem/image/handler.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/subsystem/image/manager.py` & `viggocore-1.3.0/viggocore/subsystem/image/manager.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/subsystem/image/resource.py` & `viggocore-1.3.0/viggocore/subsystem/image/resource.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/subsystem/image/router.py` & `viggocore-1.3.0/viggocore/subsystem/image/router.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/subsystem/notification/resource.py` & `viggocore-1.3.0/viggocore/subsystem/notification/resource.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/subsystem/policy/resource.py` & `viggocore-1.3.0/viggocore/subsystem/policy/resource.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/subsystem/project_cost/manager.py` & `viggocore-1.3.0/viggocore/subsystem/project_cost/manager.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/subsystem/project_cost/resource.py` & `viggocore-1.3.0/viggocore/subsystem/project_cost/resource.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/subsystem/registration/controller.py` & `viggocore-1.3.0/viggocore/subsystem/registration/controller.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/subsystem/registration/router.py` & `viggocore-1.3.0/viggocore/subsystem/registration/router.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/subsystem/role/controller.py` & `viggocore-1.3.0/viggocore/subsystem/role/controller.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/subsystem/role/manager.py` & `viggocore-1.3.0/viggocore/subsystem/role/manager.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/subsystem/role/resource.py` & `viggocore-1.3.0/viggocore/subsystem/role/resource.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/subsystem/route/manager.py` & `viggocore-1.3.0/viggocore/subsystem/route/manager.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/subsystem/route/resource.py` & `viggocore-1.3.0/viggocore/subsystem/route/resource.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 from viggocore.database import db
 from sqlalchemy import UniqueConstraint
 from viggocore.common.subsystem import entity
 
 
 class Route(entity.Entity, db.Model):
 
-    attributes = ['name', 'url', 'method', 'sysadmin', 'bypass']
+    attributes = ['name', 'url', 'method', 'sysadmin', 'bypass', 'projeto']
     attributes += entity.Entity.attributes
 
     name = db.Column(db.String(100), nullable=False)
     url = db.Column(db.String(80), nullable=False)
     method = db.Column(db.String(10), nullable=False)
     bypass = db.Column(db.Boolean(), nullable=False)
     sysadmin = db.Column(db.Boolean(), nullable=False)
+    projeto = db.Column(db.Boolean(), nullable=False, server_default='True')
 
     __table_args__ = (UniqueConstraint('url', 'method', name='route_uk'),)
 
     def __init__(self, id, name, url, method, bypass=False, sysadmin=False,
+                 projeto=True,
                  active=True, created_at=None, created_by=None,
                  updated_at=None, updated_by=None, tag=None):
         super().__init__(id, active, created_at, created_by,
                          updated_at, updated_by, tag)
         self.name = name
         self.url = url
         self.method = method
         self.bypass = bypass
         self.sysadmin = sysadmin
+        self.projeto = projeto
```

### Comparing `viggocore-1.2.9/viggocore/subsystem/tag/controller.py` & `viggocore-1.3.0/viggocore/subsystem/tag/controller.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/subsystem/tag/manager.py` & `viggocore-1.3.0/viggocore/subsystem/tag/manager.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/subsystem/tag/resource.py` & `viggocore-1.3.0/viggocore/subsystem/tag/resource.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/subsystem/tag/router.py` & `viggocore-1.3.0/viggocore/subsystem/tag/router.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/subsystem/timeline_event/controller.py` & `viggocore-1.3.0/viggocore/subsystem/timeline_event/controller.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/subsystem/timeline_event/manager.py` & `viggocore-1.3.0/viggocore/subsystem/timeline_event/manager.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/subsystem/timeline_event/resource.py` & `viggocore-1.3.0/viggocore/subsystem/timeline_event/resource.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/subsystem/token/controller.py` & `viggocore-1.3.0/viggocore/subsystem/token/controller.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/subsystem/token/manager.py` & `viggocore-1.3.0/viggocore/subsystem/token/manager.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/subsystem/token/resource.py` & `viggocore-1.3.0/viggocore/subsystem/token/resource.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/subsystem/token/router.py` & `viggocore-1.3.0/viggocore/subsystem/token/router.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/subsystem/user/controller.py` & `viggocore-1.3.0/viggocore/subsystem/user/controller.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/subsystem/user/email.py` & `viggocore-1.3.0/viggocore/subsystem/user/email.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/subsystem/user/manager.py` & `viggocore-1.3.0/viggocore/subsystem/user/manager.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/subsystem/user/resource.py` & `viggocore-1.3.0/viggocore/subsystem/user/resource.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/subsystem/user/router.py` & `viggocore-1.3.0/viggocore/subsystem/user/router.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/system.py` & `viggocore-1.3.0/viggocore/system.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/tests/functional/fixtures.py` & `viggocore-1.3.0/viggocore/tests/functional/fixtures.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/tests/functional/test_base.py` & `viggocore-1.3.0/viggocore/tests/functional/test_base.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/tests/functional/test_domains.py` & `viggocore-1.3.0/viggocore/tests/functional/test_domains.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/tests/functional/test_grants.py` & `viggocore-1.3.0/viggocore/tests/functional/test_grants.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/tests/functional/test_grants_policies.py` & `viggocore-1.3.0/viggocore/tests/functional/test_grants_policies.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/tests/functional/test_policies.py` & `viggocore-1.3.0/viggocore/tests/functional/test_policies.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/tests/functional/test_roles.py` & `viggocore-1.3.0/viggocore/tests/functional/test_roles.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore/tests/functional/test_users.py` & `viggocore-1.3.0/viggocore/tests/functional/test_users.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore.egg-info/SOURCES.txt` & `viggocore-1.3.0/viggocore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.9/viggocore.egg-info/requires.txt` & `viggocore-1.3.0/viggocore.egg-info/requires.txt`

 * *Files identical despite different names*

