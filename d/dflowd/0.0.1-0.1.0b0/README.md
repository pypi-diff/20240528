# Comparing `tmp/dflowd-0.0.1.tar.gz` & `tmp/dflowd-0.1.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dflowd-0.0.1.tar", last modified: Mon May 27 16:44:46 2024, max compression
+gzip compressed data, was "dflowd-0.1.0b0.tar", max compression
```

## Comparing `dflowd-0.0.1.tar` & `dflowd-0.1.0b0.tar`

### file list

```diff
@@ -1,11 +1,63 @@
-drwxrwxr-x   0 kudep     (1000) kudep     (1000)        0 2024-05-27 16:44:46.269400 dflowd-0.0.1/
--rw-r--r--   0 kudep     (1000) kudep     (1000)      164 2024-05-27 16:44:46.269400 dflowd-0.0.1/PKG-INFO
-drwxrwxr-x   0 kudep     (1000) kudep     (1000)        0 2024-05-27 16:44:46.265400 dflowd-0.0.1/dflowd/
--rw-rw-r--   0 kudep     (1000) kudep     (1000)        0 2024-05-27 16:44:11.000000 dflowd-0.0.1/dflowd/main.py
-drwxrwxr-x   0 kudep     (1000) kudep     (1000)        0 2024-05-27 16:44:46.269400 dflowd-0.0.1/dflowd.egg-info/
--rw-r--r--   0 kudep     (1000) kudep     (1000)      164 2024-05-27 16:44:46.000000 dflowd-0.0.1/dflowd.egg-info/PKG-INFO
--rw-rw-r--   0 kudep     (1000) kudep     (1000)      149 2024-05-27 16:44:46.000000 dflowd-0.0.1/dflowd.egg-info/SOURCES.txt
--rw-rw-r--   0 kudep     (1000) kudep     (1000)        1 2024-05-27 16:44:46.000000 dflowd-0.0.1/dflowd.egg-info/dependency_links.txt
--rw-rw-r--   0 kudep     (1000) kudep     (1000)        7 2024-05-27 16:44:46.000000 dflowd-0.0.1/dflowd.egg-info/top_level.txt
--rw-rw-r--   0 kudep     (1000) kudep     (1000)      188 2024-05-27 16:43:52.000000 dflowd-0.0.1/pyproject.toml
--rw-rw-r--   0 kudep     (1000) kudep     (1000)       38 2024-05-27 16:44:46.269400 dflowd-0.0.1/setup.cfg
+-rw-r--r--   0        0        0        0 2024-05-24 06:59:31.740535 dflowd-0.1.0b0/README.md
+-rw-r--r--   0        0        0        0 2024-05-24 06:59:31.740535 dflowd-0.1.0b0/app/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 06:59:31.740535 dflowd-0.1.0b0/app/api/__init_.py
+-rw-r--r--   0        0        0        0 2024-05-24 06:59:31.740535 dflowd-0.1.0b0/app/api/api_v1/__init__.py
+-rw-r--r--   0        0        0      479 2024-05-24 06:59:31.740535 dflowd-0.1.0b0/app/api/api_v1/api.py
+-rw-r--r--   0        0        0        0 2024-05-24 06:59:31.740535 dflowd-0.1.0b0/app/api/api_v1/endpoints/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 06:59:31.740535 dflowd-0.1.0b0/app/api/api_v1/endpoints/auth.py
+-rw-r--r--   0        0        0     6726 2024-05-28 09:06:59.747403 dflowd-0.1.0b0/app/api/api_v1/endpoints/bot.py
+-rw-r--r--   0        0        0      584 2024-05-24 06:59:31.740535 dflowd-0.1.0b0/app/api/api_v1/endpoints/dff_services.py
+-rw-r--r--   0        0        0      625 2024-05-24 06:59:31.740535 dflowd-0.1.0b0/app/api/api_v1/endpoints/flows.py
+-rw-r--r--   0        0        0      538 2024-05-24 06:59:31.740535 dflowd-0.1.0b0/app/api/deps.py
+-rw-r--r--   0        0        0     4782 2024-05-28 09:06:59.747403 dflowd-0.1.0b0/app/cli.py
+-rw-r--r--   0        0        0        0 2024-05-24 06:59:31.740535 dflowd-0.1.0b0/app/clients/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 06:59:31.740535 dflowd-0.1.0b0/app/clients/dff.py
+-rw-r--r--   0        0        0        0 2024-05-24 06:59:31.740535 dflowd-0.1.0b0/app/core/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 06:59:31.740535 dflowd-0.1.0b0/app/core/auth.py
+-rw-r--r--   0        0        0     1270 2024-05-28 10:56:26.956622 dflowd-0.1.0b0/app/core/config.py
+-rw-r--r--   0        0        0     1896 2024-05-28 09:06:59.747403 dflowd-0.1.0b0/app/core/logger_config.py
+-rw-r--r--   0        0        0        0 2024-05-24 06:59:31.740535 dflowd-0.1.0b0/app/core/security.py
+-rw-r--r--   0        0        0        0 2024-05-24 06:59:31.740535 dflowd-0.1.0b0/app/db/__init__.py
+-rw-r--r--   0        0        0      845 2024-05-24 06:59:31.740535 dflowd-0.1.0b0/app/db/base.py
+-rw-r--r--   0        0        0        0 2024-05-24 06:59:31.740535 dflowd-0.1.0b0/app/db/base_class.py
+-rw-r--r--   0        0        0        0 2024-05-24 06:59:31.740535 dflowd-0.1.0b0/app/db/crud/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 06:59:31.740535 dflowd-0.1.0b0/app/db/crud/base.py
+-rw-r--r--   0        0        0        0 2024-05-24 06:59:31.740535 dflowd-0.1.0b0/app/db/crud/crud_bot.py
+-rw-r--r--   0        0        0        0 2024-05-24 06:59:31.740535 dflowd-0.1.0b0/app/db/init_db.py
+-rw-r--r--   0        0        0        0 2024-05-24 06:59:31.740535 dflowd-0.1.0b0/app/db/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 06:59:31.740535 dflowd-0.1.0b0/app/db/models/bot.py
+-rw-r--r--   0        0        0        0 2024-05-24 06:59:31.740535 dflowd-0.1.0b0/app/db/session.py
+-rw-r--r--   0        0        0        0 2024-05-24 06:59:31.740535 dflowd-0.1.0b0/app/initial_data.py
+-rw-r--r--   0        0        0     1360 2024-05-28 11:24:55.296418 dflowd-0.1.0b0/app/main.py
+-rw-r--r--   0        0        0        0 2024-05-24 06:59:31.740535 dflowd-0.1.0b0/app/schemas/__init__.py
+-rw-r--r--   0        0        0      229 2024-05-24 06:59:31.740535 dflowd-0.1.0b0/app/schemas/pagination.py
+-rw-r--r--   0        0        0      161 2024-05-24 06:59:31.740535 dflowd-0.1.0b0/app/schemas/preset.py
+-rw-r--r--   0        0        0      250 2024-05-28 09:06:59.747403 dflowd-0.1.0b0/app/schemas/process_status.py
+-rw-r--r--   0        0        0        0 2024-05-24 06:59:31.740535 dflowd-0.1.0b0/app/services/__init__.py
+-rw-r--r--   0        0        0     3698 2024-05-28 09:06:59.747403 dflowd-0.1.0b0/app/services/index.py
+-rw-r--r--   0        0        0     7041 2024-05-28 09:06:59.757403 dflowd-0.1.0b0/app/services/json_translator.py
+-rw-r--r--   0        0        0     8699 2024-05-28 09:06:59.757403 dflowd-0.1.0b0/app/services/process.py
+-rw-r--r--   0        0        0     5081 2024-05-28 09:06:59.757403 dflowd-0.1.0b0/app/services/process_manager.py
+-rw-r--r--   0        0        0     2419 2024-05-28 09:06:59.757403 dflowd-0.1.0b0/app/services/websocket_manager.py
+-rw-r--r--   0        0        0        0 2024-05-24 06:59:31.740535 dflowd-0.1.0b0/app/static/.gitkeep
+-rw-r--r--   0        0        0   803384 2024-05-27 06:19:30.960003 dflowd-0.1.0b0/app/static/Inter-VariableFont_slnt,wght.ttf
+-rw-r--r--   0        0        0    52946 2024-05-27 06:19:30.840003 dflowd-0.1.0b0/app/static/favicon.ico
+-rw-r--r--   0        0        0   181859 2024-05-27 06:19:30.870003 dflowd-0.1.0b0/app/static/index-C6QGfX62.css
+-rw-r--r--   0        0        0  1551312 2024-05-27 06:19:30.910003 dflowd-0.1.0b0/app/static/index-C9yCL8f6.js
+-rw-r--r--   0        0        0      448 2024-05-27 06:19:30.930003 dflowd-0.1.0b0/app/static/index.html
+-rw-r--r--   0        0        0        0 2024-05-24 06:59:31.750535 dflowd-0.1.0b0/app/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 06:59:31.750535 dflowd-0.1.0b0/app/tests/api/__init__.py
+-rw-r--r--   0        0        0     6250 2024-05-28 09:06:59.757403 dflowd-0.1.0b0/app/tests/api/test_bot.py
+-rw-r--r--   0        0        0      651 2024-05-28 09:06:59.757403 dflowd-0.1.0b0/app/tests/api/test_flows.py
+-rw-r--r--   0        0        0        0 2024-05-24 13:54:11.107938 dflowd-0.1.0b0/app/tests/confest.py
+-rw-r--r--   0        0        0     1892 2024-05-24 06:59:31.750535 dflowd-0.1.0b0/app/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-05-24 06:59:31.750535 dflowd-0.1.0b0/app/tests/e2e/__init__.py
+-rw-r--r--   0        0        0     2332 2024-05-28 09:06:59.757403 dflowd-0.1.0b0/app/tests/e2e/test_e2e.py
+-rw-r--r--   0        0        0        0 2024-05-24 06:59:31.750535 dflowd-0.1.0b0/app/tests/integration/__init__.py
+-rw-r--r--   0        0        0     6163 2024-05-28 09:06:59.757403 dflowd-0.1.0b0/app/tests/integration/test_api_integration.py
+-rw-r--r--   0        0        0        0 2024-05-24 06:59:31.750535 dflowd-0.1.0b0/app/tests/services/__init__.py
+-rw-r--r--   0        0        0     1759 2024-05-28 09:06:59.757403 dflowd-0.1.0b0/app/tests/services/test_process.py
+-rw-r--r--   0        0        0     3328 2024-05-28 09:06:59.767403 dflowd-0.1.0b0/app/tests/services/test_process_manager.py
+-rw-r--r--   0        0        0     2542 2024-05-24 06:59:31.750535 dflowd-0.1.0b0/app/tests/services/test_websocket_manager.py
+-rw-r--r--   0        0        0      877 2024-05-28 11:47:44.536268 dflowd-0.1.0b0/pyproject.toml
+-rw-r--r--   0        0        0     1105 1970-01-01 00:00:00.000000 dflowd-0.1.0b0/PKG-INFO
```

