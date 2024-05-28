# Comparing `tmp/nsj_rest_lib-2.7.1.tar.gz` & `tmp/nsj_rest_lib-2.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsj_rest_lib-2.7.1.tar", last modified: Tue Apr 30 17:00:06 2024, max compression
+gzip compressed data, was "nsj_rest_lib-2.7.2.tar", last modified: Tue May 28 00:23:32 2024, max compression
```

## Comparing `nsj_rest_lib-2.7.1.tar` & `nsj_rest_lib-2.7.2.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-30 17:00:06.200817 nsj_rest_lib-2.7.1/
--rw-r--r--   0 sergio    (1000) sergio    (1000)     4938 2024-04-30 17:00:06.200817 nsj_rest_lib-2.7.1/PKG-INFO
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4082 2024-03-19 17:07:11.000000 nsj_rest_lib-2.7.1/README.md
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      103 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.1/pyproject.toml
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      914 2024-04-30 17:00:06.200817 nsj_rest_lib-2.7.1/setup.cfg
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-30 17:00:06.192817 nsj_rest_lib-2.7.1/src/
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-30 17:00:06.196817 nsj_rest_lib-2.7.1/src/nsj_rest_lib/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.1/src/nsj_rest_lib/__init__.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-30 17:00:06.196817 nsj_rest_lib-2.7.1/src/nsj_rest_lib/controller/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.1/src/nsj_rest_lib/controller/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       74 2023-07-22 20:03:52.000000 nsj_rest_lib-2.7.1/src/nsj_rest_lib/controller/constants.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       75 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.1/src/nsj_rest_lib/controller/controller_util.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     3298 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.1/src/nsj_rest_lib/controller/delete_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      944 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.1/src/nsj_rest_lib/controller/funtion_route_wrapper.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4408 2023-08-20 19:12:24.000000 nsj_rest_lib-2.7.1/src/nsj_rest_lib/controller/get_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     5436 2024-02-05 21:10:11.000000 nsj_rest_lib-2.7.1/src/nsj_rest_lib/controller/list_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4841 2023-09-27 21:20:22.000000 nsj_rest_lib-2.7.1/src/nsj_rest_lib/controller/patch_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4849 2024-03-04 22:24:04.000000 nsj_rest_lib-2.7.1/src/nsj_rest_lib/controller/post_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4902 2023-09-27 21:20:22.000000 nsj_rest_lib-2.7.1/src/nsj_rest_lib/controller/put_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4664 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.1/src/nsj_rest_lib/controller/route_base.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-30 17:00:06.196817 nsj_rest_lib-2.7.1/src/nsj_rest_lib/dao/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.1/src/nsj_rest_lib/dao/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)    35092 2024-03-04 17:45:18.000000 nsj_rest_lib-2.7.1/src/nsj_rest_lib/dao/dao_base.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1419 2023-10-05 17:46:49.000000 nsj_rest_lib-2.7.1/src/nsj_rest_lib/db_pool_config.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-30 17:00:06.196817 nsj_rest_lib-2.7.1/src/nsj_rest_lib/decorator/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.1/src/nsj_rest_lib/decorator/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)    13776 2024-04-24 19:50:59.000000 nsj_rest_lib-2.7.1/src/nsj_rest_lib/decorator/dto.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     2055 2023-08-26 23:46:06.000000 nsj_rest_lib-2.7.1/src/nsj_rest_lib/decorator/entity.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-30 17:00:06.196817 nsj_rest_lib-2.7.1/src/nsj_rest_lib/descriptor/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.1/src/nsj_rest_lib/descriptor/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      418 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.1/src/nsj_rest_lib/descriptor/conjunto_type.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)    10094 2024-02-05 19:44:51.000000 nsj_rest_lib-2.7.1/src/nsj_rest_lib/descriptor/dto_field.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     7563 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.1/src/nsj_rest_lib/descriptor/dto_field_validators.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4605 2024-03-04 22:21:11.000000 nsj_rest_lib-2.7.1/src/nsj_rest_lib/descriptor/dto_left_join_field.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     6071 2023-12-28 20:47:57.000000 nsj_rest_lib-2.7.1/src/nsj_rest_lib/descriptor/dto_list_field.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     3271 2024-04-30 16:59:49.000000 nsj_rest_lib-2.7.1/src/nsj_rest_lib/descriptor/dto_object_field.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     7331 2024-03-05 22:27:27.000000 nsj_rest_lib-2.7.1/src/nsj_rest_lib/descriptor/dto_sql_join_field.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      320 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.1/src/nsj_rest_lib/descriptor/filter_operator.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     2295 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.1/src/nsj_rest_lib/doc_route_generator.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-30 17:00:06.200817 nsj_rest_lib-2.7.1/src/nsj_rest_lib/dto/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.1/src/nsj_rest_lib/dto/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      144 2023-10-06 22:45:32.000000 nsj_rest_lib-2.7.1/src/nsj_rest_lib/dto/after_insert_update_data.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)    16734 2024-04-24 19:50:59.000000 nsj_rest_lib-2.7.1/src/nsj_rest_lib/dto/dto_base.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-30 17:00:06.200817 nsj_rest_lib-2.7.1/src/nsj_rest_lib/entity/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.1/src/nsj_rest_lib/entity/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1785 2023-08-26 23:46:06.000000 nsj_rest_lib-2.7.1/src/nsj_rest_lib/entity/entity_base.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      396 2024-02-29 18:49:26.000000 nsj_rest_lib-2.7.1/src/nsj_rest_lib/entity/filter.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      483 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.1/src/nsj_rest_lib/exception.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     2856 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.1/src/nsj_rest_lib/healthcheck_config.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      841 2023-09-15 22:16:41.000000 nsj_rest_lib-2.7.1/src/nsj_rest_lib/injector_factory_base.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-30 17:00:06.200817 nsj_rest_lib-2.7.1/src/nsj_rest_lib/service/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.1/src/nsj_rest_lib/service/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)    55848 2024-04-30 16:59:49.000000 nsj_rest_lib-2.7.1/src/nsj_rest_lib/service/service_base.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      845 2024-03-06 20:26:30.000000 nsj_rest_lib-2.7.1/src/nsj_rest_lib/settings.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-30 17:00:06.200817 nsj_rest_lib-2.7.1/src/nsj_rest_lib/util/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-10-23 23:15:21.000000 nsj_rest_lib-2.7.1/src/nsj_rest_lib/util/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      362 2024-02-29 18:49:26.000000 nsj_rest_lib-2.7.1/src/nsj_rest_lib/util/join_aux.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     6826 2023-12-13 16:07:49.000000 nsj_rest_lib-2.7.1/src/nsj_rest_lib/util/type_validator_util.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-30 17:00:06.200817 nsj_rest_lib-2.7.1/src/nsj_rest_lib/validator/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.1/src/nsj_rest_lib/validator/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4196 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.1/src/nsj_rest_lib/validator/cpf_cnpj.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      527 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.1/src/nsj_rest_lib/validator/validate_data.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      367 2023-12-28 20:47:57.000000 nsj_rest_lib-2.7.1/src/nsj_rest_lib/wsgi.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-30 17:00:06.200817 nsj_rest_lib-2.7.1/src/nsj_rest_lib.egg-info/
--rw-r--r--   0 sergio    (1000) sergio    (1000)     4938 2024-04-30 17:00:06.000000 nsj_rest_lib-2.7.1/src/nsj_rest_lib.egg-info/PKG-INFO
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     2111 2024-04-30 17:00:06.000000 nsj_rest_lib-2.7.1/src/nsj_rest_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        1 2024-04-30 17:00:06.000000 nsj_rest_lib-2.7.1/src/nsj_rest_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      138 2024-04-30 17:00:06.000000 nsj_rest_lib-2.7.1/src/nsj_rest_lib.egg-info/requires.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       13 2024-04-30 17:00:06.000000 nsj_rest_lib-2.7.1/src/nsj_rest_lib.egg-info/top_level.txt
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-05-28 00:23:32.803057 nsj_rest_lib-2.7.2/
+-rw-r--r--   0 sergio    (1000) sergio    (1000)     4938 2024-05-28 00:23:32.803057 nsj_rest_lib-2.7.2/PKG-INFO
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4082 2024-03-19 17:07:11.000000 nsj_rest_lib-2.7.2/README.md
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      103 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.2/pyproject.toml
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      914 2024-05-28 00:23:32.803057 nsj_rest_lib-2.7.2/setup.cfg
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-05-28 00:23:32.799057 nsj_rest_lib-2.7.2/src/
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-05-28 00:23:32.799057 nsj_rest_lib-2.7.2/src/nsj_rest_lib/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.2/src/nsj_rest_lib/__init__.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-05-28 00:23:32.803057 nsj_rest_lib-2.7.2/src/nsj_rest_lib/controller/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.2/src/nsj_rest_lib/controller/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       74 2023-07-22 20:03:52.000000 nsj_rest_lib-2.7.2/src/nsj_rest_lib/controller/constants.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       75 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.2/src/nsj_rest_lib/controller/controller_util.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     3298 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.2/src/nsj_rest_lib/controller/delete_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      944 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.2/src/nsj_rest_lib/controller/funtion_route_wrapper.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4408 2024-05-28 00:22:16.000000 nsj_rest_lib-2.7.2/src/nsj_rest_lib/controller/get_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     5436 2024-02-05 21:10:11.000000 nsj_rest_lib-2.7.2/src/nsj_rest_lib/controller/list_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4841 2023-09-27 21:20:22.000000 nsj_rest_lib-2.7.2/src/nsj_rest_lib/controller/patch_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4849 2024-03-04 22:24:04.000000 nsj_rest_lib-2.7.2/src/nsj_rest_lib/controller/post_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4902 2023-09-27 21:20:22.000000 nsj_rest_lib-2.7.2/src/nsj_rest_lib/controller/put_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4664 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.2/src/nsj_rest_lib/controller/route_base.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-05-28 00:23:32.803057 nsj_rest_lib-2.7.2/src/nsj_rest_lib/dao/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.2/src/nsj_rest_lib/dao/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    35092 2024-03-04 17:45:18.000000 nsj_rest_lib-2.7.2/src/nsj_rest_lib/dao/dao_base.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2174 2024-04-30 22:06:37.000000 nsj_rest_lib-2.7.2/src/nsj_rest_lib/db_pool_config.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-05-28 00:23:32.803057 nsj_rest_lib-2.7.2/src/nsj_rest_lib/decorator/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.2/src/nsj_rest_lib/decorator/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    13776 2024-04-24 19:50:59.000000 nsj_rest_lib-2.7.2/src/nsj_rest_lib/decorator/dto.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2055 2023-08-26 23:46:06.000000 nsj_rest_lib-2.7.2/src/nsj_rest_lib/decorator/entity.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-05-28 00:23:32.803057 nsj_rest_lib-2.7.2/src/nsj_rest_lib/descriptor/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.2/src/nsj_rest_lib/descriptor/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      418 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.2/src/nsj_rest_lib/descriptor/conjunto_type.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    10094 2024-02-05 19:44:51.000000 nsj_rest_lib-2.7.2/src/nsj_rest_lib/descriptor/dto_field.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     7563 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.2/src/nsj_rest_lib/descriptor/dto_field_validators.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4605 2024-03-04 22:21:11.000000 nsj_rest_lib-2.7.2/src/nsj_rest_lib/descriptor/dto_left_join_field.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     6071 2023-12-28 20:47:57.000000 nsj_rest_lib-2.7.2/src/nsj_rest_lib/descriptor/dto_list_field.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     3271 2024-04-30 16:59:49.000000 nsj_rest_lib-2.7.2/src/nsj_rest_lib/descriptor/dto_object_field.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     7331 2024-03-05 22:27:27.000000 nsj_rest_lib-2.7.2/src/nsj_rest_lib/descriptor/dto_sql_join_field.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      320 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.2/src/nsj_rest_lib/descriptor/filter_operator.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2295 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.2/src/nsj_rest_lib/doc_route_generator.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-05-28 00:23:32.803057 nsj_rest_lib-2.7.2/src/nsj_rest_lib/dto/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.2/src/nsj_rest_lib/dto/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      144 2023-10-06 22:45:32.000000 nsj_rest_lib-2.7.2/src/nsj_rest_lib/dto/after_insert_update_data.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    16734 2024-04-24 19:50:59.000000 nsj_rest_lib-2.7.2/src/nsj_rest_lib/dto/dto_base.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-05-28 00:23:32.803057 nsj_rest_lib-2.7.2/src/nsj_rest_lib/entity/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.2/src/nsj_rest_lib/entity/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1785 2023-08-26 23:46:06.000000 nsj_rest_lib-2.7.2/src/nsj_rest_lib/entity/entity_base.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      396 2024-02-29 18:49:26.000000 nsj_rest_lib-2.7.2/src/nsj_rest_lib/entity/filter.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      483 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.2/src/nsj_rest_lib/exception.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2856 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.2/src/nsj_rest_lib/healthcheck_config.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      841 2023-09-15 22:16:41.000000 nsj_rest_lib-2.7.2/src/nsj_rest_lib/injector_factory_base.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-05-28 00:23:32.803057 nsj_rest_lib-2.7.2/src/nsj_rest_lib/service/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.2/src/nsj_rest_lib/service/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    56112 2024-05-28 00:21:33.000000 nsj_rest_lib-2.7.2/src/nsj_rest_lib/service/service_base.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      845 2024-03-06 20:26:30.000000 nsj_rest_lib-2.7.2/src/nsj_rest_lib/settings.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-05-28 00:23:32.803057 nsj_rest_lib-2.7.2/src/nsj_rest_lib/util/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-10-23 23:15:21.000000 nsj_rest_lib-2.7.2/src/nsj_rest_lib/util/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      362 2024-02-29 18:49:26.000000 nsj_rest_lib-2.7.2/src/nsj_rest_lib/util/join_aux.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     6826 2023-12-13 16:07:49.000000 nsj_rest_lib-2.7.2/src/nsj_rest_lib/util/type_validator_util.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-05-28 00:23:32.803057 nsj_rest_lib-2.7.2/src/nsj_rest_lib/validator/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.2/src/nsj_rest_lib/validator/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4196 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.2/src/nsj_rest_lib/validator/cpf_cnpj.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      527 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.2/src/nsj_rest_lib/validator/validate_data.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      367 2023-12-28 20:47:57.000000 nsj_rest_lib-2.7.2/src/nsj_rest_lib/wsgi.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-05-28 00:23:32.803057 nsj_rest_lib-2.7.2/src/nsj_rest_lib.egg-info/
+-rw-r--r--   0 sergio    (1000) sergio    (1000)     4938 2024-05-28 00:23:32.000000 nsj_rest_lib-2.7.2/src/nsj_rest_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2111 2024-05-28 00:23:32.000000 nsj_rest_lib-2.7.2/src/nsj_rest_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        1 2024-05-28 00:23:32.000000 nsj_rest_lib-2.7.2/src/nsj_rest_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      138 2024-05-28 00:23:32.000000 nsj_rest_lib-2.7.2/src/nsj_rest_lib.egg-info/requires.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       13 2024-05-28 00:23:32.000000 nsj_rest_lib-2.7.2/src/nsj_rest_lib.egg-info/top_level.txt
```

### Comparing `nsj_rest_lib-2.7.1/PKG-INFO` & `nsj_rest_lib-2.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsj_rest_lib
-Version: 2.7.1
+Version: 2.7.2
 Summary: Biblioteca para construção de APIs Rest Python, de acordo com o guidelines interno, e com paradigma declarativo.
 Home-page: https://github.com/Nasajon/nsj_rest_lib
 Author: Nasajon Sistemas
 Author-email: contact.dev@nasajon.com.br
 Project-URL: Source, https://github.com/Nasajon/nsj_rest_lib
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `nsj_rest_lib-2.7.1/README.md` & `nsj_rest_lib-2.7.2/README.md`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.7.1/setup.cfg` & `nsj_rest_lib-2.7.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nsj_rest_lib
-version = 2.7.1
+version = 2.7.2
 author = Nasajon Sistemas
 author_email = contact.dev@nasajon.com.br
 description = Biblioteca para construção de APIs Rest Python, de acordo com o guidelines interno, e com paradigma declarativo.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Nasajon/nsj_rest_lib
 project_urls =
```

### Comparing `nsj_rest_lib-2.7.1/src/nsj_rest_lib/controller/delete_route.py` & `nsj_rest_lib-2.7.2/src/nsj_rest_lib/controller/delete_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.7.1/src/nsj_rest_lib/controller/funtion_route_wrapper.py` & `nsj_rest_lib-2.7.2/src/nsj_rest_lib/controller/funtion_route_wrapper.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.7.1/src/nsj_rest_lib/controller/get_route.py` & `nsj_rest_lib-2.7.2/src/nsj_rest_lib/controller/get_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.7.1/src/nsj_rest_lib/controller/list_route.py` & `nsj_rest_lib-2.7.2/src/nsj_rest_lib/controller/list_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.7.1/src/nsj_rest_lib/controller/patch_route.py` & `nsj_rest_lib-2.7.2/src/nsj_rest_lib/controller/patch_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.7.1/src/nsj_rest_lib/controller/post_route.py` & `nsj_rest_lib-2.7.2/src/nsj_rest_lib/controller/post_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.7.1/src/nsj_rest_lib/controller/put_route.py` & `nsj_rest_lib-2.7.2/src/nsj_rest_lib/controller/put_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.7.1/src/nsj_rest_lib/controller/route_base.py` & `nsj_rest_lib-2.7.2/src/nsj_rest_lib/controller/route_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.7.1/src/nsj_rest_lib/dao/dao_base.py` & `nsj_rest_lib-2.7.2/src/nsj_rest_lib/dao/dao_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.7.1/src/nsj_rest_lib/db_pool_config.py` & `nsj_rest_lib-2.7.2/src/nsj_rest_lib/db_pool_config.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,34 +7,69 @@
 from nsj_rest_lib.settings import CLOUD_SQL_CONN_NAME
 from nsj_rest_lib.settings import ENV
 from nsj_rest_lib.settings import DB_POOL_SIZE
 
 import sqlalchemy
 
 
+def create_url(
+    username: str,
+    password: str,
+    host: str,
+    port: str,
+    database: str,
+    db_dialect: str = "postgresql+pg8000",
+):
+    return str(
+        sqlalchemy.engine.URL.create(
+            db_dialect,
+            username=username,
+            password=password,
+            host=host,
+            port=port,
+            database=database,
+        )
+    )
+
+
 def create_pool(database_conn_url):
     # Creating database connection pool
     db_pool = sqlalchemy.create_engine(
         database_conn_url,
         # pool_size=DB_POOL_SIZE,
         # max_overflow=2,
         # pool_timeout=30,
         # pool_recycle=1800,
         poolclass=sqlalchemy.pool.NullPool,
     )
     return db_pool
 
 
 if DATABASE_DRIVER.upper() in ["SINGLE_STORE", "MYSQL"]:
-    database_conn_url = f"mysql+pymysql://{DATABASE_USER}:{DATABASE_PASS}@{DATABASE_HOST}:{DATABASE_PORT}/{DATABASE_NAME}"
+    database_conn_url = create_url(
+        DATABASE_USER,
+        DATABASE_PASS,
+        DATABASE_HOST,
+        DATABASE_PORT,
+        DATABASE_NAME,
+        "mysql+pymysql",
+    )
+    # database_conn_url = f"mysql+pymysql://{DATABASE_USER}:{DATABASE_PASS}@{DATABASE_HOST}:{DATABASE_PORT}/{DATABASE_NAME}"
 else:
     if ENV.upper() == "GCP":
         database_conn_url = f"postgresql+pg8000://{DATABASE_USER}:{DATABASE_PASS}@/{DATABASE_NAME}?unix_sock=/cloudsql/{CLOUD_SQL_CONN_NAME}/.s.PGSQL.{DATABASE_PORT}"
     else:
-        database_conn_url = f"postgresql+pg8000://{DATABASE_USER}:{DATABASE_PASS}@{DATABASE_HOST}:{DATABASE_PORT}/{DATABASE_NAME}"
+        database_conn_url = create_url(
+            DATABASE_USER,
+            DATABASE_PASS,
+            DATABASE_HOST,
+            DATABASE_PORT,
+            DATABASE_NAME,
+        )
+        # database_conn_url = f"postgresql+pg8000://{DATABASE_USER}:{DATABASE_PASS}@{DATABASE_HOST}:{DATABASE_PORT}/{DATABASE_NAME}"
 
 
 def default_create_pool():
     return create_pool(database_conn_url)
 
 
 # db_pool = create_pool(database_conn_url)
```

### Comparing `nsj_rest_lib-2.7.1/src/nsj_rest_lib/decorator/dto.py` & `nsj_rest_lib-2.7.2/src/nsj_rest_lib/decorator/dto.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.7.1/src/nsj_rest_lib/decorator/entity.py` & `nsj_rest_lib-2.7.2/src/nsj_rest_lib/decorator/entity.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.7.1/src/nsj_rest_lib/descriptor/dto_field.py` & `nsj_rest_lib-2.7.2/src/nsj_rest_lib/descriptor/dto_field.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.7.1/src/nsj_rest_lib/descriptor/dto_field_validators.py` & `nsj_rest_lib-2.7.2/src/nsj_rest_lib/descriptor/dto_field_validators.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.7.1/src/nsj_rest_lib/descriptor/dto_left_join_field.py` & `nsj_rest_lib-2.7.2/src/nsj_rest_lib/descriptor/dto_left_join_field.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.7.1/src/nsj_rest_lib/descriptor/dto_list_field.py` & `nsj_rest_lib-2.7.2/src/nsj_rest_lib/descriptor/dto_list_field.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.7.1/src/nsj_rest_lib/descriptor/dto_object_field.py` & `nsj_rest_lib-2.7.2/src/nsj_rest_lib/descriptor/dto_object_field.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.7.1/src/nsj_rest_lib/descriptor/dto_sql_join_field.py` & `nsj_rest_lib-2.7.2/src/nsj_rest_lib/descriptor/dto_sql_join_field.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.7.1/src/nsj_rest_lib/doc_route_generator.py` & `nsj_rest_lib-2.7.2/src/nsj_rest_lib/doc_route_generator.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.7.1/src/nsj_rest_lib/dto/dto_base.py` & `nsj_rest_lib-2.7.2/src/nsj_rest_lib/dto/dto_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.7.1/src/nsj_rest_lib/entity/entity_base.py` & `nsj_rest_lib-2.7.2/src/nsj_rest_lib/entity/entity_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.7.1/src/nsj_rest_lib/healthcheck_config.py` & `nsj_rest_lib-2.7.2/src/nsj_rest_lib/healthcheck_config.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.7.1/src/nsj_rest_lib/injector_factory_base.py` & `nsj_rest_lib-2.7.2/src/nsj_rest_lib/injector_factory_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.7.1/src/nsj_rest_lib/service/service_base.py` & `nsj_rest_lib-2.7.2/src/nsj_rest_lib/service/service_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -685,20 +685,23 @@
                         )
 
                     # Resolvendo a chave do relacionamento
                     relation_key_field = self._dto_class.pk_field
                     if list_field.relation_key_field is not None:
                         relation_key_field = list_field.relation_key_field
 
+                    # Getting value to filter related list
+                    relation_filter_value = getattr(dto, relation_key_field)
+                    if relation_filter_value is None:
+                        # If None, there is no related objects. So, set empty list and return.
+                        setattr(dto, master_dto_attr, [])
+                        return
+
                     # Making filter to relation
-                    filters = {
-                        list_field.related_entity_field: getattr(
-                            dto, relation_key_field
-                        )
-                    }
+                    filters = {list_field.related_entity_field: relation_filter_value}
 
                     # Tratando campos de particionamento
                     for field in self._dto_class.partition_fields:
                         if field in list_field.dto_type.partition_fields:
                             filters[field] = getattr(dto, field)
 
                     # Resolvendo os fields da entidade aninhada
```

### Comparing `nsj_rest_lib-2.7.1/src/nsj_rest_lib/settings.py` & `nsj_rest_lib-2.7.2/src/nsj_rest_lib/settings.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.7.1/src/nsj_rest_lib/util/type_validator_util.py` & `nsj_rest_lib-2.7.2/src/nsj_rest_lib/util/type_validator_util.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.7.1/src/nsj_rest_lib/validator/cpf_cnpj.py` & `nsj_rest_lib-2.7.2/src/nsj_rest_lib/validator/cpf_cnpj.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.7.1/src/nsj_rest_lib/validator/validate_data.py` & `nsj_rest_lib-2.7.2/src/nsj_rest_lib/validator/validate_data.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.7.1/src/nsj_rest_lib.egg-info/PKG-INFO` & `nsj_rest_lib-2.7.2/src/nsj_rest_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsj_rest_lib
-Version: 2.7.1
+Version: 2.7.2
 Summary: Biblioteca para construção de APIs Rest Python, de acordo com o guidelines interno, e com paradigma declarativo.
 Home-page: https://github.com/Nasajon/nsj_rest_lib
 Author: Nasajon Sistemas
 Author-email: contact.dev@nasajon.com.br
 Project-URL: Source, https://github.com/Nasajon/nsj_rest_lib
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `nsj_rest_lib-2.7.1/src/nsj_rest_lib.egg-info/SOURCES.txt` & `nsj_rest_lib-2.7.2/src/nsj_rest_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

