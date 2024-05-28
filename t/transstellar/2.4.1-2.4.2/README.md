# Comparing `tmp/transstellar-2.4.1.tar.gz` & `tmp/transstellar-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transstellar-2.4.1.tar", max compression
+gzip compressed data, was "transstellar-2.4.2.tar", max compression
```

## Comparing `transstellar-2.4.1.tar` & `transstellar-2.4.2.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0      396 2024-05-27 06:50:03.398828 transstellar-2.4.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-25 07:21:52.372907 transstellar-2.4.1/src/transstellar/__init__.py
--rw-r--r--   0        0        0      333 2024-05-23 08:08:58.028344 transstellar-2.4.1/src/transstellar/api_client/__init__.py
--rw-r--r--   0        0        0      474 2024-05-23 08:50:22.393777 transstellar-2.4.1/src/transstellar/api_client/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     6405 2024-05-23 08:50:22.393777 transstellar-2.4.1/src/transstellar/api_client/__pycache__/api_client.cpython-312.pyc
--rw-r--r--   0        0        0     3392 2024-05-27 03:39:07.570292 transstellar-2.4.1/src/transstellar/api_client/__pycache__/api_resource.cpython-312.pyc
--rw-r--r--   0        0        0     4656 2024-05-23 08:08:58.024343 transstellar-2.4.1/src/transstellar/api_client/api_client.py
--rw-r--r--   0        0        0     2436 2024-05-23 10:30:29.487092 transstellar-2.4.1/src/transstellar/api_client/api_resource.py
--rw-r--r--   0        0        0      189 2024-03-25 07:21:52.372907 transstellar-2.4.1/src/transstellar/api_client/errors/__init__.py
--rw-r--r--   0        0        0      352 2024-03-25 08:02:28.073753 transstellar-2.4.1/src/transstellar/api_client/errors/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0      383 2024-03-07 09:16:29.850062 transstellar-2.4.1/src/transstellar/api_client/errors/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      400 2024-03-25 08:02:28.073753 transstellar-2.4.1/src/transstellar/api_client/errors/__pycache__/client_error.cpython-312.pyc
--rw-r--r--   0        0        0      355 2024-03-07 09:16:29.850062 transstellar-2.4.1/src/transstellar/api_client/errors/__pycache__/client_error.cpython-38.pyc
--rw-r--r--   0        0        0      400 2024-03-25 08:02:28.073753 transstellar-2.4.1/src/transstellar/api_client/errors/__pycache__/server_error.cpython-312.pyc
--rw-r--r--   0        0        0      355 2024-03-07 09:16:29.854062 transstellar-2.4.1/src/transstellar/api_client/errors/__pycache__/server_error.cpython-38.pyc
--rw-r--r--   0        0        0      412 2024-03-25 08:02:28.073753 transstellar-2.4.1/src/transstellar/api_client/errors/__pycache__/unauthorized_error.cpython-312.pyc
--rw-r--r--   0        0        0      367 2024-03-07 09:16:29.854062 transstellar-2.4.1/src/transstellar/api_client/errors/__pycache__/unauthorized_error.cpython-38.pyc
--rw-r--r--   0        0        0       96 2024-03-25 07:21:52.372907 transstellar-2.4.1/src/transstellar/api_client/errors/client_error.py
--rw-r--r--   0        0        0       96 2024-03-25 07:21:52.372907 transstellar-2.4.1/src/transstellar/api_client/errors/server_error.py
--rw-r--r--   0        0        0      102 2024-03-25 07:21:52.372907 transstellar-2.4.1/src/transstellar/api_client/errors/unauthorized_error.py
--rw-r--r--   0        0        0      831 2024-05-06 07:57:56.408911 transstellar-2.4.1/src/transstellar/framework/__init__.py
--rw-r--r--   0        0        0      925 2024-05-14 08:42:29.711243 transstellar-2.4.1/src/transstellar/framework/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     5740 2024-05-22 08:04:44.985764 transstellar-2.4.1/src/transstellar/framework/__pycache__/application.cpython-312.pyc
--rw-r--r--   0        0        0      832 2024-05-06 07:03:19.734569 transstellar-2.4.1/src/transstellar/framework/__pycache__/application_bootstrapper.cpython-312.pyc
--rw-r--r--   0        0        0      856 2024-03-20 08:12:14.536313 transstellar-2.4.1/src/transstellar/framework/__pycache__/base_api_test.cpython-312-pytest-8.0.2.pyc
--rw-r--r--   0        0        0      595 2024-03-25 08:02:27.945759 transstellar-2.4.1/src/transstellar/framework/__pycache__/base_api_test.cpython-312-pytest-8.1.1.pyc
--rw-r--r--   0        0        0      595 2024-05-03 10:38:32.725071 transstellar-2.4.1/src/transstellar/framework/__pycache__/base_api_test.cpython-312-pytest-8.2.0.pyc
--rw-r--r--   0        0        0     1553 2024-05-15 07:21:51.348116 transstellar-2.4.1/src/transstellar/framework/__pycache__/base_page.cpython-312.pyc
--rw-r--r--   0        0        0     1012 2024-03-20 09:47:02.256105 transstellar-2.4.1/src/transstellar/framework/__pycache__/base_test.cpython-312-pytest-8.0.2.pyc
--rw-r--r--   0        0        0     1012 2024-03-25 08:02:27.945759 transstellar-2.4.1/src/transstellar/framework/__pycache__/base_test.cpython-312-pytest-8.1.1.pyc
--rw-r--r--   0        0        0     1012 2024-05-03 10:38:32.725071 transstellar-2.4.1/src/transstellar/framework/__pycache__/base_test.cpython-312-pytest-8.2.0.pyc
--rw-r--r--   0        0        0     3237 2024-03-21 03:52:22.082583 transstellar-2.4.1/src/transstellar/framework/__pycache__/base_ui_test.cpython-312-pytest-8.0.2.pyc
--rw-r--r--   0        0        0     3237 2024-04-30 08:38:09.180119 transstellar-2.4.1/src/transstellar/framework/__pycache__/base_ui_test.cpython-312-pytest-8.1.1.pyc
--rw-r--r--   0        0        0     3237 2024-05-03 10:38:32.737071 transstellar-2.4.1/src/transstellar/framework/__pycache__/base_ui_test.cpython-312-pytest-8.2.0.pyc
--rw-r--r--   0        0        0     1210 2024-03-25 08:02:27.957759 transstellar-2.4.1/src/transstellar/framework/__pycache__/config_service.cpython-312.pyc
--rw-r--r--   0        0        0    11927 2024-05-27 03:39:07.082291 transstellar-2.4.1/src/transstellar/framework/__pycache__/element.cpython-312.pyc
--rw-r--r--   0        0        0      212 2024-03-25 08:02:28.005756 transstellar-2.4.1/src/transstellar/framework/__pycache__/handle_error.cpython-312.pyc
--rw-r--r--   0        0        0     1882 2024-03-25 08:02:28.005756 transstellar-2.4.1/src/transstellar/framework/__pycache__/handle_ui_error.cpython-312.pyc
--rw-r--r--   0        0        0      646 2024-03-25 08:02:27.941759 transstellar-2.4.1/src/transstellar/framework/__pycache__/loggable.cpython-312.pyc
--rw-r--r--   0        0        0     2428 2024-03-25 08:02:27.945759 transstellar-2.4.1/src/transstellar/framework/__pycache__/logger.cpython-312.pyc
--rw-r--r--   0        0        0     1010 2024-03-25 08:02:28.005756 transstellar-2.4.1/src/transstellar/framework/__pycache__/main_config.cpython-312.pyc
--rw-r--r--   0        0        0      892 2024-03-25 08:02:27.941759 transstellar-2.4.1/src/transstellar/framework/__pycache__/module.cpython-312.pyc
--rw-r--r--   0        0        0     1232 2024-05-14 08:42:29.807242 transstellar-2.4.1/src/transstellar/framework/__pycache__/router.cpython-312.pyc
--rw-r--r--   0        0        0     2467 2024-05-23 06:46:43.216136 transstellar-2.4.1/src/transstellar/framework/__pycache__/utils.cpython-312.pyc
--rw-r--r--   0        0        0     3177 2024-05-21 10:39:38.120518 transstellar-2.4.1/src/transstellar/framework/application.py
--rw-r--r--   0        0        0      273 2024-05-06 06:58:08.437282 transstellar-2.4.1/src/transstellar/framework/application_bootstrapper.py
--rw-r--r--   0        0        0      104 2024-03-25 07:21:52.372907 transstellar-2.4.1/src/transstellar/framework/base_api_test.py
--rw-r--r--   0        0        0      545 2024-05-15 07:02:34.774249 transstellar-2.4.1/src/transstellar/framework/base_page.py
--rw-r--r--   0        0        0      305 2024-03-25 07:22:27.425371 transstellar-2.4.1/src/transstellar/framework/base_test.py
--rw-r--r--   0        0        0     1426 2024-04-30 08:37:17.948017 transstellar-2.4.1/src/transstellar/framework/base_ui_test.py
--rw-r--r--   0        0        0      410 2024-03-25 07:21:52.372907 transstellar-2.4.1/src/transstellar/framework/config_service.py
--rw-r--r--   0        0        0     7511 2024-05-24 10:56:09.398120 transstellar-2.4.1/src/transstellar/framework/element.py
--rw-r--r--   0        0        0       77 2024-03-25 07:22:27.421371 transstellar-2.4.1/src/transstellar/framework/handle_error.py
--rw-r--r--   0        0        0     1194 2024-03-25 07:22:27.421371 transstellar-2.4.1/src/transstellar/framework/handle_ui_error.py
--rw-r--r--   0        0        0      151 2024-03-25 07:21:52.372907 transstellar-2.4.1/src/transstellar/framework/loggable.py
--rw-r--r--   0        0        0     1087 2024-03-25 07:22:27.437371 transstellar-2.4.1/src/transstellar/framework/logger.py
--rw-r--r--   0        0        0      348 2024-03-25 07:21:52.372907 transstellar-2.4.1/src/transstellar/framework/main_config.py
--rw-r--r--   0        0        0      288 2024-03-25 07:22:27.429371 transstellar-2.4.1/src/transstellar/framework/module.py
--rw-r--r--   0        0        0      520 2024-05-06 07:57:56.408911 transstellar-2.4.1/src/transstellar/framework/router.py
--rw-r--r--   0        0        0     1374 2024-05-23 06:42:34.553784 transstellar-2.4.1/src/transstellar/framework/utils.py
--rw-r--r--   0        0        0      516 1970-01-01 00:00:00.000000 transstellar-2.4.1/PKG-INFO
+-rw-r--r--   0        0        0      396 2024-05-28 03:32:59.930310 transstellar-2.4.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-25 07:21:52.372907 transstellar-2.4.2/src/transstellar/__init__.py
+-rw-r--r--   0        0        0      333 2024-05-23 08:08:58.028344 transstellar-2.4.2/src/transstellar/api_client/__init__.py
+-rw-r--r--   0        0        0      474 2024-05-23 08:50:22.393777 transstellar-2.4.2/src/transstellar/api_client/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     6405 2024-05-23 08:50:22.393777 transstellar-2.4.2/src/transstellar/api_client/__pycache__/api_client.cpython-312.pyc
+-rw-r--r--   0        0        0     3392 2024-05-27 03:39:07.570292 transstellar-2.4.2/src/transstellar/api_client/__pycache__/api_resource.cpython-312.pyc
+-rw-r--r--   0        0        0     4656 2024-05-23 08:08:58.024343 transstellar-2.4.2/src/transstellar/api_client/api_client.py
+-rw-r--r--   0        0        0     2436 2024-05-23 10:30:29.487092 transstellar-2.4.2/src/transstellar/api_client/api_resource.py
+-rw-r--r--   0        0        0      189 2024-03-25 07:21:52.372907 transstellar-2.4.2/src/transstellar/api_client/errors/__init__.py
+-rw-r--r--   0        0        0      352 2024-03-25 08:02:28.073753 transstellar-2.4.2/src/transstellar/api_client/errors/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0      383 2024-03-07 09:16:29.850062 transstellar-2.4.2/src/transstellar/api_client/errors/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      400 2024-03-25 08:02:28.073753 transstellar-2.4.2/src/transstellar/api_client/errors/__pycache__/client_error.cpython-312.pyc
+-rw-r--r--   0        0        0      355 2024-03-07 09:16:29.850062 transstellar-2.4.2/src/transstellar/api_client/errors/__pycache__/client_error.cpython-38.pyc
+-rw-r--r--   0        0        0      400 2024-03-25 08:02:28.073753 transstellar-2.4.2/src/transstellar/api_client/errors/__pycache__/server_error.cpython-312.pyc
+-rw-r--r--   0        0        0      355 2024-03-07 09:16:29.854062 transstellar-2.4.2/src/transstellar/api_client/errors/__pycache__/server_error.cpython-38.pyc
+-rw-r--r--   0        0        0      412 2024-03-25 08:02:28.073753 transstellar-2.4.2/src/transstellar/api_client/errors/__pycache__/unauthorized_error.cpython-312.pyc
+-rw-r--r--   0        0        0      367 2024-03-07 09:16:29.854062 transstellar-2.4.2/src/transstellar/api_client/errors/__pycache__/unauthorized_error.cpython-38.pyc
+-rw-r--r--   0        0        0       96 2024-03-25 07:21:52.372907 transstellar-2.4.2/src/transstellar/api_client/errors/client_error.py
+-rw-r--r--   0        0        0       96 2024-03-25 07:21:52.372907 transstellar-2.4.2/src/transstellar/api_client/errors/server_error.py
+-rw-r--r--   0        0        0      102 2024-03-25 07:21:52.372907 transstellar-2.4.2/src/transstellar/api_client/errors/unauthorized_error.py
+-rw-r--r--   0        0        0      831 2024-05-06 07:57:56.408911 transstellar-2.4.2/src/transstellar/framework/__init__.py
+-rw-r--r--   0        0        0      925 2024-05-14 08:42:29.711243 transstellar-2.4.2/src/transstellar/framework/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     5740 2024-05-22 08:04:44.985764 transstellar-2.4.2/src/transstellar/framework/__pycache__/application.cpython-312.pyc
+-rw-r--r--   0        0        0      832 2024-05-06 07:03:19.734569 transstellar-2.4.2/src/transstellar/framework/__pycache__/application_bootstrapper.cpython-312.pyc
+-rw-r--r--   0        0        0      856 2024-03-20 08:12:14.536313 transstellar-2.4.2/src/transstellar/framework/__pycache__/base_api_test.cpython-312-pytest-8.0.2.pyc
+-rw-r--r--   0        0        0      595 2024-03-25 08:02:27.945759 transstellar-2.4.2/src/transstellar/framework/__pycache__/base_api_test.cpython-312-pytest-8.1.1.pyc
+-rw-r--r--   0        0        0      595 2024-05-03 10:38:32.725071 transstellar-2.4.2/src/transstellar/framework/__pycache__/base_api_test.cpython-312-pytest-8.2.0.pyc
+-rw-r--r--   0        0        0     1553 2024-05-15 07:21:51.348116 transstellar-2.4.2/src/transstellar/framework/__pycache__/base_page.cpython-312.pyc
+-rw-r--r--   0        0        0     1012 2024-03-20 09:47:02.256105 transstellar-2.4.2/src/transstellar/framework/__pycache__/base_test.cpython-312-pytest-8.0.2.pyc
+-rw-r--r--   0        0        0     1012 2024-03-25 08:02:27.945759 transstellar-2.4.2/src/transstellar/framework/__pycache__/base_test.cpython-312-pytest-8.1.1.pyc
+-rw-r--r--   0        0        0     1012 2024-05-03 10:38:32.725071 transstellar-2.4.2/src/transstellar/framework/__pycache__/base_test.cpython-312-pytest-8.2.0.pyc
+-rw-r--r--   0        0        0     3237 2024-03-21 03:52:22.082583 transstellar-2.4.2/src/transstellar/framework/__pycache__/base_ui_test.cpython-312-pytest-8.0.2.pyc
+-rw-r--r--   0        0        0     3237 2024-04-30 08:38:09.180119 transstellar-2.4.2/src/transstellar/framework/__pycache__/base_ui_test.cpython-312-pytest-8.1.1.pyc
+-rw-r--r--   0        0        0     3237 2024-05-03 10:38:32.737071 transstellar-2.4.2/src/transstellar/framework/__pycache__/base_ui_test.cpython-312-pytest-8.2.0.pyc
+-rw-r--r--   0        0        0     1210 2024-03-25 08:02:27.957759 transstellar-2.4.2/src/transstellar/framework/__pycache__/config_service.cpython-312.pyc
+-rw-r--r--   0        0        0    11927 2024-05-28 03:31:12.501774 transstellar-2.4.2/src/transstellar/framework/__pycache__/element.cpython-312.pyc
+-rw-r--r--   0        0        0      212 2024-03-25 08:02:28.005756 transstellar-2.4.2/src/transstellar/framework/__pycache__/handle_error.cpython-312.pyc
+-rw-r--r--   0        0        0     1882 2024-03-25 08:02:28.005756 transstellar-2.4.2/src/transstellar/framework/__pycache__/handle_ui_error.cpython-312.pyc
+-rw-r--r--   0        0        0      646 2024-03-25 08:02:27.941759 transstellar-2.4.2/src/transstellar/framework/__pycache__/loggable.cpython-312.pyc
+-rw-r--r--   0        0        0     2428 2024-03-25 08:02:27.945759 transstellar-2.4.2/src/transstellar/framework/__pycache__/logger.cpython-312.pyc
+-rw-r--r--   0        0        0     1010 2024-03-25 08:02:28.005756 transstellar-2.4.2/src/transstellar/framework/__pycache__/main_config.cpython-312.pyc
+-rw-r--r--   0        0        0      892 2024-03-25 08:02:27.941759 transstellar-2.4.2/src/transstellar/framework/__pycache__/module.cpython-312.pyc
+-rw-r--r--   0        0        0     1232 2024-05-14 08:42:29.807242 transstellar-2.4.2/src/transstellar/framework/__pycache__/router.cpython-312.pyc
+-rw-r--r--   0        0        0     2467 2024-05-23 06:46:43.216136 transstellar-2.4.2/src/transstellar/framework/__pycache__/utils.cpython-312.pyc
+-rw-r--r--   0        0        0     3177 2024-05-21 10:39:38.120518 transstellar-2.4.2/src/transstellar/framework/application.py
+-rw-r--r--   0        0        0      273 2024-05-06 06:58:08.437282 transstellar-2.4.2/src/transstellar/framework/application_bootstrapper.py
+-rw-r--r--   0        0        0      104 2024-03-25 07:21:52.372907 transstellar-2.4.2/src/transstellar/framework/base_api_test.py
+-rw-r--r--   0        0        0      545 2024-05-15 07:02:34.774249 transstellar-2.4.2/src/transstellar/framework/base_page.py
+-rw-r--r--   0        0        0      305 2024-03-25 07:22:27.425371 transstellar-2.4.2/src/transstellar/framework/base_test.py
+-rw-r--r--   0        0        0     1426 2024-04-30 08:37:17.948017 transstellar-2.4.2/src/transstellar/framework/base_ui_test.py
+-rw-r--r--   0        0        0      410 2024-03-25 07:21:52.372907 transstellar-2.4.2/src/transstellar/framework/config_service.py
+-rw-r--r--   0        0        0     7511 2024-05-28 03:31:10.333764 transstellar-2.4.2/src/transstellar/framework/element.py
+-rw-r--r--   0        0        0       77 2024-03-25 07:22:27.421371 transstellar-2.4.2/src/transstellar/framework/handle_error.py
+-rw-r--r--   0        0        0     1194 2024-03-25 07:22:27.421371 transstellar-2.4.2/src/transstellar/framework/handle_ui_error.py
+-rw-r--r--   0        0        0      151 2024-03-25 07:21:52.372907 transstellar-2.4.2/src/transstellar/framework/loggable.py
+-rw-r--r--   0        0        0     1087 2024-03-25 07:22:27.437371 transstellar-2.4.2/src/transstellar/framework/logger.py
+-rw-r--r--   0        0        0      348 2024-03-25 07:21:52.372907 transstellar-2.4.2/src/transstellar/framework/main_config.py
+-rw-r--r--   0        0        0      288 2024-03-25 07:22:27.429371 transstellar-2.4.2/src/transstellar/framework/module.py
+-rw-r--r--   0        0        0      520 2024-05-06 07:57:56.408911 transstellar-2.4.2/src/transstellar/framework/router.py
+-rw-r--r--   0        0        0     1374 2024-05-23 06:42:34.553784 transstellar-2.4.2/src/transstellar/framework/utils.py
+-rw-r--r--   0        0        0      516 1970-01-01 00:00:00.000000 transstellar-2.4.2/PKG-INFO
```

### Comparing `transstellar-2.4.1/src/transstellar/api_client/__pycache__/api_client.cpython-312.pyc` & `transstellar-2.4.2/src/transstellar/api_client/__pycache__/api_client.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.4.1/src/transstellar/api_client/__pycache__/api_resource.cpython-312.pyc` & `transstellar-2.4.2/src/transstellar/api_client/__pycache__/api_resource.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.4.1/src/transstellar/api_client/api_client.py` & `transstellar-2.4.2/src/transstellar/api_client/api_client.py`

 * *Files identical despite different names*

### Comparing `transstellar-2.4.1/src/transstellar/api_client/api_resource.py` & `transstellar-2.4.2/src/transstellar/api_client/api_resource.py`

 * *Files identical despite different names*

### Comparing `transstellar-2.4.1/src/transstellar/framework/__init__.py` & `transstellar-2.4.2/src/transstellar/framework/__init__.py`

 * *Files identical despite different names*

### Comparing `transstellar-2.4.1/src/transstellar/framework/__pycache__/__init__.cpython-312.pyc` & `transstellar-2.4.2/src/transstellar/framework/__pycache__/__init__.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.4.1/src/transstellar/framework/__pycache__/application.cpython-312.pyc` & `transstellar-2.4.2/src/transstellar/framework/__pycache__/application.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.4.1/src/transstellar/framework/__pycache__/application_bootstrapper.cpython-312.pyc` & `transstellar-2.4.2/src/transstellar/framework/__pycache__/application_bootstrapper.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.4.1/src/transstellar/framework/__pycache__/base_api_test.cpython-312-pytest-8.0.2.pyc` & `transstellar-2.4.2/src/transstellar/framework/__pycache__/base_api_test.cpython-312-pytest-8.0.2.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.4.1/src/transstellar/framework/__pycache__/base_api_test.cpython-312-pytest-8.1.1.pyc` & `transstellar-2.4.2/src/transstellar/framework/__pycache__/base_api_test.cpython-312-pytest-8.1.1.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.4.1/src/transstellar/framework/__pycache__/base_api_test.cpython-312-pytest-8.2.0.pyc` & `transstellar-2.4.2/src/transstellar/framework/__pycache__/base_api_test.cpython-312-pytest-8.2.0.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.4.1/src/transstellar/framework/__pycache__/base_page.cpython-312.pyc` & `transstellar-2.4.2/src/transstellar/framework/__pycache__/base_page.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.4.1/src/transstellar/framework/__pycache__/base_test.cpython-312-pytest-8.0.2.pyc` & `transstellar-2.4.2/src/transstellar/framework/__pycache__/base_test.cpython-312-pytest-8.0.2.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.4.1/src/transstellar/framework/__pycache__/base_test.cpython-312-pytest-8.1.1.pyc` & `transstellar-2.4.2/src/transstellar/framework/__pycache__/base_test.cpython-312-pytest-8.1.1.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.4.1/src/transstellar/framework/__pycache__/base_test.cpython-312-pytest-8.2.0.pyc` & `transstellar-2.4.2/src/transstellar/framework/__pycache__/base_test.cpython-312-pytest-8.2.0.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.4.1/src/transstellar/framework/__pycache__/base_ui_test.cpython-312-pytest-8.0.2.pyc` & `transstellar-2.4.2/src/transstellar/framework/__pycache__/base_ui_test.cpython-312-pytest-8.0.2.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.4.1/src/transstellar/framework/__pycache__/base_ui_test.cpython-312-pytest-8.1.1.pyc` & `transstellar-2.4.2/src/transstellar/framework/__pycache__/base_ui_test.cpython-312-pytest-8.1.1.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.4.1/src/transstellar/framework/__pycache__/base_ui_test.cpython-312-pytest-8.2.0.pyc` & `transstellar-2.4.2/src/transstellar/framework/__pycache__/base_ui_test.cpython-312-pytest-8.2.0.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.4.1/src/transstellar/framework/__pycache__/config_service.cpython-312.pyc` & `transstellar-2.4.2/src/transstellar/framework/__pycache__/config_service.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.4.1/src/transstellar/framework/__pycache__/element.cpython-312.pyc` & `transstellar-2.4.2/src/transstellar/framework/__pycache__/element.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Fri May 24 10:56:09 2024 UTC, .py size: 7511 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 4972 5066 571d 0000  ........IrPfW...
+00000000: cb0d 0d0a 0000 0000 fe4f 5566 571d 0000  .........OUfW...
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 00f3 9e00 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 5a00 6400 6401 6c01 5a01 6400 6402  l.Z.d.d.l.Z.d.d.
 00000040: 6c02 6d03 5a03 6d04 5a04 0100 6400 6403  l.m.Z.m.Z...d.d.
 00000050: 6c05 6d06 5a06 0100 6400 6404 6c07 6d08  l.m.Z...d.d.l.m.
 00000060: 5a08 0100 6400 6405 6c09 6d0a 5a0a 0100  Z...d.d.l.m.Z...
 00000070: 6400 6406 6c0b 6d0c 5a0c 0100 6407 6408  d.d.l.m.Z...d.d.
@@ -399,15 +399,15 @@
 000018e0: 0000 0000 00ab 0000 0000 0000 006a 0300  .............j..
 000018f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001900: 0064 01ab 0100 0000 0000 007d 017c 006a  .d.........}.|.j
 00001910: 0400 0000 0000 0000 0000 0000 0000 0000  ................
 00001920: 0000 006a 0700 0000 0000 0000 0000 0000  ...j............
 00001930: 0000 0000 0000 0064 027c 019b 009d 02ab  .......d.|......
 00001940: 0100 0000 0000 0001 007c 0153 0029 034e  .........|.S.).N
-00001950: da09 696e 6e65 7248 544d 4c7a 0e63 7572  ..innerHTMLz.cur
+00001950: da09 6f75 7465 7248 544d 4c7a 0e63 7572  ..outerHTMLz.cur
 00001960: 7265 6e74 2048 544d 4c3a 2029 0472 3c00  rent HTML: ).r<.
 00001970: 0000 da0d 6765 745f 6174 7472 6962 7574  ....get_attribut
 00001980: 6572 3300 0000 7234 0000 0029 0272 1e00  er3...r4...).r..
 00001990: 0000 da04 6874 6d6c 7302 0000 0020 2072  ....htmls....  r
 000019a0: 2000 0000 da10 6765 745f 6375 7272 656e   .....get_curren
 000019b0: 745f 6874 6d6c 7a18 456c 656d 656e 742e  t_htmlz.Element.
 000019c0: 6765 745f 6375 7272 656e 745f 6874 6d6c  get_current_html
```

### Comparing `transstellar-2.4.1/src/transstellar/framework/__pycache__/handle_ui_error.cpython-312.pyc` & `transstellar-2.4.2/src/transstellar/framework/__pycache__/handle_ui_error.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.4.1/src/transstellar/framework/__pycache__/loggable.cpython-312.pyc` & `transstellar-2.4.2/src/transstellar/framework/__pycache__/loggable.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.4.1/src/transstellar/framework/__pycache__/logger.cpython-312.pyc` & `transstellar-2.4.2/src/transstellar/framework/__pycache__/logger.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.4.1/src/transstellar/framework/__pycache__/main_config.cpython-312.pyc` & `transstellar-2.4.2/src/transstellar/framework/__pycache__/main_config.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.4.1/src/transstellar/framework/__pycache__/module.cpython-312.pyc` & `transstellar-2.4.2/src/transstellar/framework/__pycache__/module.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.4.1/src/transstellar/framework/__pycache__/router.cpython-312.pyc` & `transstellar-2.4.2/src/transstellar/framework/__pycache__/router.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.4.1/src/transstellar/framework/__pycache__/utils.cpython-312.pyc` & `transstellar-2.4.2/src/transstellar/framework/__pycache__/utils.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar-2.4.1/src/transstellar/framework/application.py` & `transstellar-2.4.2/src/transstellar/framework/application.py`

 * *Files identical despite different names*

### Comparing `transstellar-2.4.1/src/transstellar/framework/base_page.py` & `transstellar-2.4.2/src/transstellar/framework/base_page.py`

 * *Files identical despite different names*

### Comparing `transstellar-2.4.1/src/transstellar/framework/base_ui_test.py` & `transstellar-2.4.2/src/transstellar/framework/base_ui_test.py`

 * *Files identical despite different names*

### Comparing `transstellar-2.4.1/src/transstellar/framework/element.py` & `transstellar-2.4.2/src/transstellar/framework/element.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,15 +145,15 @@
         dom_element = self.find_global_dom_element_by_xpath(xpath)
 
         self.set_current_dom_element(dom_element)
 
         return self.dom_element
 
     def get_current_html(self):
-        html = self.get_current_dom_element().get_attribute("innerHTML")
+        html = self.get_current_dom_element().get_attribute("outerHTML")
 
         self.logger.debug(f"current HTML: {html}")
 
         return html
 
     def find_global_dom_element_by_xpath(self, xpath: str):
         self.logger.debug(f"finding global dom element by xpath: {xpath}")
```

### Comparing `transstellar-2.4.1/src/transstellar/framework/handle_ui_error.py` & `transstellar-2.4.2/src/transstellar/framework/handle_ui_error.py`

 * *Files identical despite different names*

### Comparing `transstellar-2.4.1/src/transstellar/framework/logger.py` & `transstellar-2.4.2/src/transstellar/framework/logger.py`

 * *Files identical despite different names*

### Comparing `transstellar-2.4.1/src/transstellar/framework/router.py` & `transstellar-2.4.2/src/transstellar/framework/router.py`

 * *Files identical despite different names*

### Comparing `transstellar-2.4.1/src/transstellar/framework/utils.py` & `transstellar-2.4.2/src/transstellar/framework/utils.py`

 * *Files identical despite different names*

### Comparing `transstellar-2.4.1/PKG-INFO` & `transstellar-2.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transstellar
-Version: 2.4.1
+Version: 2.4.2
 Summary: A pytest framework
 Author: Onramplab Dev
 Author-email: dev@onramplab.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: injector (>=0.21.0,<0.22.0)
```

