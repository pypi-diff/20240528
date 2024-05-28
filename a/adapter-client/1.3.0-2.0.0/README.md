# Comparing `tmp/adapter-client-1.3.0.tar.gz` & `tmp/adapter-client-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adapter-client-1.3.0.tar", last modified: Thu Jul 13 05:51:55 2023, max compression
+gzip compressed data, was "adapter-client-2.0.0.tar", last modified: Tue May 28 11:34:55 2024, max compression
```

## Comparing `adapter-client-1.3.0.tar` & `adapter-client-2.0.0.tar`

### file list

```diff
@@ -1,59 +1,60 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 05:51:55.915982 adapter-client-1.3.0/
--rw-r--r--   0 root         (0) root         (0)      290 2022-07-22 09:13:24.000000 adapter-client-1.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4353 2023-07-13 05:51:55.914982 adapter-client-1.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3243 2022-07-22 09:13:24.000000 adapter-client-1.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 05:51:55.890982 adapter-client-1.3.0/requirements/
--rw-r--r--   0 root         (0) root         (0)      217 2023-07-06 12:44:32.000000 adapter-client-1.3.0/requirements/base.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-07-22 09:13:24.000000 adapter-client-1.3.0/requirements/prod.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-13 05:51:55.915982 adapter-client-1.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2710 2023-07-06 12:44:32.000000 adapter-client-1.3.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 05:51:55.887982 adapter-client-1.3.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 05:51:55.894982 adapter-client-1.3.0/src/adapter_client/
--rw-r--r--   0 root         (0) root         (0)       70 2022-07-22 09:13:24.000000 adapter-client-1.3.0/src/adapter_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 05:51:55.898982 adapter-client-1.3.0/src/adapter_client/adapters/
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 09:13:24.000000 adapter-client-1.3.0/src/adapter_client/adapters/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2478 2023-07-06 12:44:32.000000 adapter-client-1.3.0/src/adapter_client/adapters/base.py
--rw-r--r--   0 root         (0) root         (0)     9914 2022-07-22 09:13:24.000000 adapter-client-1.3.0/src/adapter_client/adapters/db.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 05:51:55.899982 adapter-client-1.3.0/src/adapter_client/adapters/smev/
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 09:13:24.000000 adapter-client-1.3.0/src/adapter_client/adapters/smev/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8563 2023-04-17 05:18:46.000000 adapter-client-1.3.0/src/adapter_client/adapters/smev/adapter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 05:51:55.902982 adapter-client-1.3.0/src/adapter_client/adapters/smev/interfaces/
--rw-r--r--   0 root         (0) root         (0)       95 2022-07-22 09:13:24.000000 adapter-client-1.3.0/src/adapter_client/adapters/smev/interfaces/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1622 2023-07-06 12:44:32.000000 adapter-client-1.3.0/src/adapter_client/adapters/smev/interfaces/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 05:51:55.903982 adapter-client-1.3.0/src/adapter_client/adapters/smev/interfaces/soap/
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 09:13:24.000000 adapter-client-1.3.0/src/adapter_client/adapters/smev/interfaces/soap/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12745 2023-07-13 05:51:43.000000 adapter-client-1.3.0/src/adapter_client/adapters/smev/interfaces/soap/interface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 05:51:55.906982 adapter-client-1.3.0/src/adapter_client/adapters/smev/interfaces/soap/schema/
--rw-r--r--   0 root         (0) root         (0)     8513 2022-07-22 09:13:24.000000 adapter-client-1.3.0/src/adapter_client/adapters/smev/interfaces/soap/schema/adapter.wsdl
--rw-r--r--   0 root         (0) root         (0)     4627 2022-07-22 09:13:24.000000 adapter-client-1.3.0/src/adapter_client/adapters/smev/interfaces/soap/schema/smev-service-adapter-faults.xsd
--rw-r--r--   0 root         (0) root         (0)    56967 2022-07-22 09:13:24.000000 adapter-client-1.3.0/src/adapter_client/adapters/smev/interfaces/soap/schema/smev-service-adapter-types.xsd
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 05:51:55.908982 adapter-client-1.3.0/src/adapter_client/adapters/smev/logging/
--rw-r--r--   0 root         (0) root         (0)     1714 2023-07-06 12:44:32.000000 adapter-client-1.3.0/src/adapter_client/adapters/smev/logging/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3613 2023-07-06 12:44:32.000000 adapter-client-1.3.0/src/adapter_client/adapters/smev/logging/opensearch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 05:51:55.909982 adapter-client-1.3.0/src/adapter_client/adapters/smev/services/
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 09:13:24.000000 adapter-client-1.3.0/src/adapter_client/adapters/smev/services/__init__.py
--rw-r--r--   0 root         (0) root         (0)      301 2022-07-22 09:13:24.000000 adapter-client-1.3.0/src/adapter_client/adapters/smev/services/base.py
--rw-r--r--   0 root         (0) root         (0)     1501 2022-07-22 09:13:24.000000 adapter-client-1.3.0/src/adapter_client/adapters/smev/services/registry.py
--rw-r--r--   0 root         (0) root         (0)     3624 2023-07-06 12:44:32.000000 adapter-client-1.3.0/src/adapter_client/apps.py
--rw-r--r--   0 root         (0) root         (0)      961 2022-07-22 09:13:24.000000 adapter-client-1.3.0/src/adapter_client/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 05:51:55.911982 adapter-client-1.3.0/src/adapter_client/core/
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 09:13:24.000000 adapter-client-1.3.0/src/adapter_client/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 05:51:55.912982 adapter-client-1.3.0/src/adapter_client/core/domain/
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 09:13:24.000000 adapter-client-1.3.0/src/adapter_client/core/domain/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9137 2023-07-13 05:51:43.000000 adapter-client-1.3.0/src/adapter_client/core/domain/model.py
--rw-r--r--   0 root         (0) root         (0)      286 2022-07-22 09:13:24.000000 adapter-client-1.3.0/src/adapter_client/core/services.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 05:51:55.914982 adapter-client-1.3.0/src/adapter_client/migrations/
--rw-r--r--   0 root         (0) root         (0)     7165 2022-07-22 09:13:24.000000 adapter-client-1.3.0/src/adapter_client/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)     3282 2023-07-06 12:44:32.000000 adapter-client-1.3.0/src/adapter_client/migrations/0002_alter_journalentry_options_config_adapter_interface_and_more.py
--rw-r--r--   0 root         (0) root         (0)      613 2023-07-13 05:51:43.000000 adapter-client-1.3.0/src/adapter_client/migrations/0003_message_transaction_code_alter_config_journal_config_and_more.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 09:13:24.000000 adapter-client-1.3.0/src/adapter_client/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8019 2023-07-13 05:51:43.000000 adapter-client-1.3.0/src/adapter_client/models.py
--rw-r--r--   0 root         (0) root         (0)     5004 2023-07-06 12:44:32.000000 adapter-client-1.3.0/src/adapter_client/tasks.py
--rw-r--r--   0 root         (0) root         (0)      574 2023-04-17 05:18:46.000000 adapter-client-1.3.0/src/adapter_client/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 05:51:55.896982 adapter-client-1.3.0/src/adapter_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4353 2023-07-13 05:51:55.000000 adapter-client-1.3.0/src/adapter_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1850 2023-07-13 05:51:55.000000 adapter-client-1.3.0/src/adapter_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-07-13 05:51:55.000000 adapter-client-1.3.0/src/adapter_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      219 2023-07-13 05:51:55.000000 adapter-client-1.3.0/src/adapter_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-13 05:51:55.000000 adapter-client-1.3.0/src/adapter_client.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      450 2023-07-13 05:51:55.000000 adapter-client-1.3.0/version.conf
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-28 11:34:55.941395 adapter-client-2.0.0/
+-rw-r--r--   0 toor      (1000) toor      (1000)      290 2022-07-22 09:13:24.000000 adapter-client-2.0.0/MANIFEST.in
+-rw-r--r--   0 toor      (1000) toor      (1000)     4874 2024-05-28 11:34:55.940394 adapter-client-2.0.0/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)     3243 2022-07-22 09:13:24.000000 adapter-client-2.0.0/README.md
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-28 11:34:55.901395 adapter-client-2.0.0/requirements/
+-rw-r--r--   0 toor      (1000) toor      (1000)      334 2024-05-28 11:34:51.000000 adapter-client-2.0.0/requirements/base.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       12 2022-07-22 09:13:24.000000 adapter-client-2.0.0/requirements/prod.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       38 2024-05-28 11:34:55.941395 adapter-client-2.0.0/setup.cfg
+-rw-r--r--   0 toor      (1000) toor      (1000)     2798 2024-05-28 11:34:51.000000 adapter-client-2.0.0/setup.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-28 11:34:55.896395 adapter-client-2.0.0/src/
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-28 11:34:55.912395 adapter-client-2.0.0/src/adapter_client/
+-rw-r--r--   0 toor      (1000) toor      (1000)       70 2022-07-22 09:13:24.000000 adapter-client-2.0.0/src/adapter_client/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-28 11:34:55.916395 adapter-client-2.0.0/src/adapter_client/adapters/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-07-22 09:13:24.000000 adapter-client-2.0.0/src/adapter_client/adapters/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2478 2023-07-06 12:44:32.000000 adapter-client-2.0.0/src/adapter_client/adapters/base.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     9967 2024-05-28 11:34:51.000000 adapter-client-2.0.0/src/adapter_client/adapters/db.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-28 11:34:55.917394 adapter-client-2.0.0/src/adapter_client/adapters/smev/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-07-22 09:13:24.000000 adapter-client-2.0.0/src/adapter_client/adapters/smev/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     9291 2024-05-28 11:34:51.000000 adapter-client-2.0.0/src/adapter_client/adapters/smev/adapter.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-28 11:34:55.918395 adapter-client-2.0.0/src/adapter_client/adapters/smev/interfaces/
+-rw-r--r--   0 toor      (1000) toor      (1000)       95 2022-07-22 09:13:24.000000 adapter-client-2.0.0/src/adapter_client/adapters/smev/interfaces/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1622 2023-07-06 12:44:32.000000 adapter-client-2.0.0/src/adapter_client/adapters/smev/interfaces/base.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-28 11:34:55.919395 adapter-client-2.0.0/src/adapter_client/adapters/smev/interfaces/soap/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-07-22 09:13:24.000000 adapter-client-2.0.0/src/adapter_client/adapters/smev/interfaces/soap/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    12745 2023-07-13 05:51:43.000000 adapter-client-2.0.0/src/adapter_client/adapters/smev/interfaces/soap/interface.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-28 11:34:55.923395 adapter-client-2.0.0/src/adapter_client/adapters/smev/interfaces/soap/schema/
+-rw-r--r--   0 toor      (1000) toor      (1000)     8513 2022-07-22 09:13:24.000000 adapter-client-2.0.0/src/adapter_client/adapters/smev/interfaces/soap/schema/adapter.wsdl
+-rw-r--r--   0 toor      (1000) toor      (1000)     4627 2022-07-22 09:13:24.000000 adapter-client-2.0.0/src/adapter_client/adapters/smev/interfaces/soap/schema/smev-service-adapter-faults.xsd
+-rw-r--r--   0 toor      (1000) toor      (1000)    56967 2022-07-22 09:13:24.000000 adapter-client-2.0.0/src/adapter_client/adapters/smev/interfaces/soap/schema/smev-service-adapter-types.xsd
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-28 11:34:55.929395 adapter-client-2.0.0/src/adapter_client/adapters/smev/logging/
+-rw-r--r--   0 toor      (1000) toor      (1000)     1714 2023-07-06 12:44:32.000000 adapter-client-2.0.0/src/adapter_client/adapters/smev/logging/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3945 2024-05-28 11:34:51.000000 adapter-client-2.0.0/src/adapter_client/adapters/smev/logging/opensearch.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-28 11:34:55.931395 adapter-client-2.0.0/src/adapter_client/adapters/smev/services/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-07-22 09:13:24.000000 adapter-client-2.0.0/src/adapter_client/adapters/smev/services/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      301 2022-07-22 09:13:24.000000 adapter-client-2.0.0/src/adapter_client/adapters/smev/services/base.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1501 2022-07-22 09:13:24.000000 adapter-client-2.0.0/src/adapter_client/adapters/smev/services/registry.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3624 2023-07-06 12:44:32.000000 adapter-client-2.0.0/src/adapter_client/apps.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      961 2022-07-22 09:13:24.000000 adapter-client-2.0.0/src/adapter_client/config.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-28 11:34:55.933395 adapter-client-2.0.0/src/adapter_client/core/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-07-22 09:13:24.000000 adapter-client-2.0.0/src/adapter_client/core/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-28 11:34:55.934395 adapter-client-2.0.0/src/adapter_client/core/domain/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-07-22 09:13:24.000000 adapter-client-2.0.0/src/adapter_client/core/domain/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     9137 2023-07-13 05:51:43.000000 adapter-client-2.0.0/src/adapter_client/core/domain/model.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      286 2022-07-22 09:13:24.000000 adapter-client-2.0.0/src/adapter_client/core/services.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-28 11:34:55.938395 adapter-client-2.0.0/src/adapter_client/migrations/
+-rw-r--r--   0 toor      (1000) toor      (1000)     7165 2022-07-22 09:13:24.000000 adapter-client-2.0.0/src/adapter_client/migrations/0001_initial.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3282 2023-07-06 12:44:32.000000 adapter-client-2.0.0/src/adapter_client/migrations/0002_alter_journalentry_options_config_adapter_interface_and_more.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      613 2023-07-13 05:51:43.000000 adapter-client-2.0.0/src/adapter_client/migrations/0003_message_transaction_code_alter_config_journal_config_and_more.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1366 2024-05-28 11:34:51.000000 adapter-client-2.0.0/src/adapter_client/migrations/0004_alter_incomingmessage_id.py
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-07-22 09:13:24.000000 adapter-client-2.0.0/src/adapter_client/migrations/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     8022 2024-05-28 11:34:51.000000 adapter-client-2.0.0/src/adapter_client/models.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     5004 2023-07-06 12:44:32.000000 adapter-client-2.0.0/src/adapter_client/tasks.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      574 2023-04-17 05:18:46.000000 adapter-client-2.0.0/src/adapter_client/utils.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-28 11:34:55.939395 adapter-client-2.0.0/src/adapter_client.egg-info/
+-rw-r--r--   0 toor      (1000) toor      (1000)     4874 2024-05-28 11:34:55.000000 adapter-client-2.0.0/src/adapter_client.egg-info/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)     1913 2024-05-28 11:34:55.000000 adapter-client-2.0.0/src/adapter_client.egg-info/SOURCES.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       44 2024-05-28 11:34:55.000000 adapter-client-2.0.0/src/adapter_client.egg-info/dependency_links.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)      244 2024-05-28 11:34:55.000000 adapter-client-2.0.0/src/adapter_client.egg-info/requires.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       15 2024-05-28 11:34:55.000000 adapter-client-2.0.0/src/adapter_client.egg-info/top_level.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)      450 2024-05-28 11:34:55.000000 adapter-client-2.0.0/version.conf
```

### Comparing `adapter-client-1.3.0/PKG-INFO` & `adapter-client-2.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,45 @@
 Metadata-Version: 2.1
 Name: adapter-client
-Version: 1.3.0
+Version: 2.0.0
 Summary: Клиент для взаимодействия со СМЭВ3 посредством Адаптера
 Author: BARS Group
 Author-email: education_dev@bars-open.ru
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Web Environment
 Classifier: Natural Language :: Russian
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Description-Content-Type: text/markdown
+Requires-Dist: pydantic<1.10.0,>=1.9.0
+Requires-Dist: zeep<4.2.0,>=4.1.0
+Requires-Dist: django
+Requires-Dist: celery<5.3.0; python_version == "3.7"
+Requires-Dist: celery; python_version > "3.7"
+Requires-Dist: django_celery_beat<2.6.0; python_version == "3.7"
+Requires-Dist: django_celery_beat; python_version > "3.7"
+Requires-Dist: django-postgres-partitioning==1.1.0
 Provides-Extra: opensearch
+Requires-Dist: opensearch-logger==1.2.2; extra == "opensearch"
 
 # Клиент для взаимодействия со СМЭВ3 посредством Адаптера
 ## Подключение
 settings:
 
     INSTALLED_APPS = [
         'adapter_client'
```

### Comparing `adapter-client-1.3.0/README.md` & `adapter-client-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `adapter-client-1.3.0/setup.py` & `adapter-client-2.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,22 +57,24 @@
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'Development Status :: 5 - Production/Stable',
         'Framework :: Django :: 2.2',
         'Framework :: Django :: 3.0',
         'Framework :: Django :: 3.1',
         'Framework :: Django :: 3.2',
         'Framework :: Django :: 4.0',
         'Framework :: Django :: 4.1',
         'Framework :: Django :: 4.2',
+        'Framework :: Django :: 5.0',
     ],
     extras_require={
         'opensearch': (
             'opensearch-logger==1.2.2',
         ),
     },
     dependency_links=(
```

### Comparing `adapter-client-1.3.0/src/adapter_client/adapters/base.py` & `adapter-client-2.0.0/src/adapter_client/adapters/base.py`

 * *Files identical despite different names*

### Comparing `adapter-client-1.3.0/src/adapter_client/adapters/db.py` & `adapter-client-2.0.0/src/adapter_client/adapters/db.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,34 +40,35 @@
 config_repository = ConfigRepository()
 
 
 class RelatedToMessageMixin:
 
     """Примесь для хранилищ данных связанных с сообщением."""
 
-    db_model_cls: DjangoModel
+    db_model_cls: Type[DjangoModel]
 
     @property
     def _qs(self):
         return self.db_model_cls.objects.select_related('message__reply_to')
 
     def _message_to_db(self, message: model.Message) -> model.Message:
         defaults = asdict(
             message,
-            dict_factory=lambda x: {k: v for (k, v) in x if k != 'reply_to'}
+            dict_factory=lambda x: {k: v for (k, v) in x if k not in ('id', 'reply_to', 'client_id')}
         )
 
         if message.reply_to is not None:
             assert message.reply_to.id is not None
             defaults.update(
                 reply_to_id=message.reply_to.id,
             )
 
         dbinstance, _ = db.Message.objects.update_or_create(
-            pk=message.id, defaults=defaults
+            client_id=message.client_id,
+            defaults=defaults
         )
 
         message.id = dbinstance.id
         return message
 
     def _message_from_db(self, dbinstance: db.Message) -> model.Message:
 
@@ -123,22 +124,21 @@
             message_metadata.message = self._message_to_db(
                 message_metadata.message
             )
 
         defaults = {
             **asdict(
                 message_metadata,
-                dict_factory=lambda x: {k: v for (k, v) in x if k != 'message'}
+                dict_factory=lambda x: {k: v for (k, v) in x if k not in ('message', 'id')}
             ),
-            **{'status': message_metadata.status.id},
-            **{'message_id': message_metadata.message.id},
+            'status': message_metadata.status.id
         }
 
         dbinstance, _ = self.db_model_cls.objects.update_or_create(
-            pk=message_metadata.id, defaults=defaults
+            message_id=message_metadata.message.id, defaults=defaults
         )
 
         message_metadata.id = dbinstance.id
         return message_metadata
 
     def _from_db(self, dbinstance: 'db_model_cls') -> 'data_model_cls':
         def get_status(dbinstance: 'db_model_cls'):
@@ -162,22 +162,23 @@
     """Хранилище исходящих сообщений."""
 
     statuses_enum = model.OutgoingStatus
     db_model_cls = db.OutgoingMessage
     data_model_cls = model.OutgoingMessage
 
     def get_unreplied_messages(self) -> Generator[model.OutgoingMessage, None, None]:
-        # id сообщений на которые уже получен ответ
+
+        # id сообщений, являющихся ответами на другие сообщения
         reply_ids = db.Message.objects.filter(
             reply_to_id__isnull=False
         ).values('reply_to')
         # перебираем исходящие сообщения на которые еще не был получен ответ
         for reply in db.OutgoingMessage.objects.filter(
             status=model.OutgoingStatus.sent.id,
-        ).exclude(id__in=reply_ids).iterator():
+        ).exclude(message_id__in=reply_ids).iterator():
             yield self._from_db(reply)
 
     def get_pending_messages(self) -> Generator[model.OutgoingMessage, None, None]:
         for reply in db.OutgoingMessage.objects.filter(
             attempts__lt=self._config.send_request_retry_count,
             status__in=(model.OutgoingStatus.new.id, model.OutgoingStatus.retry.id),
         ).iterator():
```

### Comparing `adapter-client-1.3.0/src/adapter_client/adapters/smev/adapter.py` & `adapter-client-2.0.0/src/adapter_client/adapters/smev/adapter.py`

 * *Files 7% similar despite different names*

```diff
@@ -70,15 +70,17 @@
 
     @abstractmethod
     def get_pending(self) -> ExchangeResult:
         self._reload_config()
 
     @abstractmethod
     def find_pending(self) -> Generator[ExchangeResult, None, None]:
-        """Получение ответов на сообщения переданные в адаптер СМЭВ."""
+        """
+        Получение ответов на исходящие сообщения, переданные в адаптер СМЭВ.
+        """
         self._reload_config()
 
     def _reload_config(self) -> None:
         config = config_repository.load_config()
         self._interface = import_string(config.adapter_interface)(config)
         self._outgoing_message_repository = import_string(
             config.outgoing_message_repository
@@ -121,14 +123,19 @@
             else:
                 incoming_message.status = model.IncomingStatus.processed
                 logger.info(
                     'Processing complete for message: %s' % message.client_id)
         return incoming_message
 
     def process_pending(self) -> Generator[model.IncomingMessage, None, None]:
+        """Передача сообщений на обработку в РИС.
+
+        Передаёт на обработку в РИС сообщения которые
+        ранее не удалось успешно обработать.
+        """
         logger.info('Processing pending messages...')
         super().process_pending()
         incoming_messages = (
             self._incoming_message_repository.get_pending_messages()
         )
         with ThreadPoolExecutor() as executor:
             for incoming_message in executor.map(
@@ -182,14 +189,15 @@
         self,
         incoming_message: model.IncomingMessage
     ) -> model.IncomingMessage:
         assert incoming_message.id is not None
         return self._incoming_message_repository.update(incoming_message)
 
     def send_pending(self) -> Generator[ExchangeResult, None, None]:
+        """Передача сообщений из очереди ИС в Адаптер СМЭВ."""
         logger.info('Sending pending messages...')
 
         super().send_pending()
 
         for exchange_result in self._interface.send(
             *self._outgoing_message_repository.get_pending_messages()
         ):
@@ -203,21 +211,29 @@
             )
             self._journal.log_exchange_result(exchange_result)
             yield exchange_result
 
         logger.info('Pending messages sent')
 
     def get_pending(self) -> ExchangeResult:
+        """
+        Получение одного сообщения из очереди Адаптера СМЭВ и обработка в РИС.
+        """
+
         logger.info('Receiving ...')
         super().get_pending()
         exchange_result = self._process_exchange_result(self._interface.get())
         self._journal.log_exchange_result(exchange_result)
         return exchange_result
 
     def find_pending(self) -> Generator[ExchangeResult, None, None]:
+        """
+        Получение ответов на исходящие сообщения, переданные в адаптер СМЭВ.
+        """
+
         logger.info('Receiving pending replies...')
 
         super().find_pending()
 
         with ThreadPoolExecutor() as executor:
             for exchange_result in executor.map(
                 self._process_exchange_result,
```

### Comparing `adapter-client-1.3.0/src/adapter_client/adapters/smev/interfaces/base.py` & `adapter-client-2.0.0/src/adapter_client/adapters/smev/interfaces/base.py`

 * *Files identical despite different names*

### Comparing `adapter-client-1.3.0/src/adapter_client/adapters/smev/interfaces/soap/interface.py` & `adapter-client-2.0.0/src/adapter_client/adapters/smev/interfaces/soap/interface.py`

 * *Files identical despite different names*

### Comparing `adapter-client-1.3.0/src/adapter_client/adapters/smev/interfaces/soap/schema/adapter.wsdl` & `adapter-client-2.0.0/src/adapter_client/adapters/smev/interfaces/soap/schema/adapter.wsdl`

 * *Files identical despite different names*

### Comparing `adapter-client-1.3.0/src/adapter_client/adapters/smev/interfaces/soap/schema/smev-service-adapter-faults.xsd` & `adapter-client-2.0.0/src/adapter_client/adapters/smev/interfaces/soap/schema/smev-service-adapter-faults.xsd`

 * *Files identical despite different names*

### Comparing `adapter-client-1.3.0/src/adapter_client/adapters/smev/interfaces/soap/schema/smev-service-adapter-types.xsd` & `adapter-client-2.0.0/src/adapter_client/adapters/smev/interfaces/soap/schema/smev-service-adapter-types.xsd`

 * *Files identical despite different names*

### Comparing `adapter-client-1.3.0/src/adapter_client/adapters/smev/logging/__init__.py` & `adapter-client-2.0.0/src/adapter_client/adapters/smev/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `adapter-client-1.3.0/src/adapter_client/adapters/smev/logging/opensearch.py` & `adapter-client-2.0.0/src/adapter_client/adapters/smev/logging/opensearch.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 from datetime import datetime
-from opensearch_logger import OpenSearchHandler
-from pydantic.json import pydantic_encoder
+from functools import partial
 from typing import Dict
-from zeep.helpers import serialize_object
-from zeep.xsd.valueobjects import CompoundValue
+import base64
 import json
 import logging
 
+from lxml import etree
+from opensearch_logger import OpenSearchHandler
+from pydantic.json import custom_pydantic_encoder
+from zeep.helpers import serialize_object
+from zeep.xsd.valueobjects import CompoundValue
+
 from adapter_client.adapters.smev.interfaces.base import ExchangeResult
 from adapter_client.adapters.smev.logging import AbstractWriteOnlyJournal
 from adapter_client.core.domain import model
 
 
 LEVEL = logging.INFO
 
@@ -51,18 +55,24 @@
 
     def log_exchange_result(self, exchange_result: ExchangeResult) -> model.JournalEntry:
         log = self._get_log_from_result(exchange_result)
         self.logger.log(LEVEL, f'Запрос {datetime.now().astimezone()}', extra=log)
         return self._get_entry_from_result(exchange_result)
 
     def _get_log_from_result(self, exchange_result: ExchangeResult) -> Dict[str, dict]:
-        if isinstance(exchange_result.result, CompoundValue):
-            exchange_result.result = dict(serialize_object(exchange_result.result))
+        _json_encoders = {
+            CompoundValue: serialize_object,
+            etree._Element: partial(etree.tostring, encoding='unicode'),
+            # для обратного преобразования байтов PKCS7 подписи в base64
+            bytes: lambda o: base64.b64encode(o).decode('ascii'),
+        }
+
+        json_encoder = partial(custom_pydantic_encoder, _json_encoders)
 
-        log = json.loads(json.dumps(exchange_result, default=pydantic_encoder))
+        log = json.loads(json.dumps(exchange_result, default=json_encoder))
 
         # Нельзя сохранить список из разных типов: [1, 'Send'], преобразуем в словарь
         log['request_type'] = log.get('request_type') or {}
         if log['request_type']:
             log['request_type'] = {
                 'id': log['request_type'][0],
                 'name': log['request_type'][1],
```

### Comparing `adapter-client-1.3.0/src/adapter_client/adapters/smev/services/registry.py` & `adapter-client-2.0.0/src/adapter_client/adapters/smev/services/registry.py`

 * *Files identical despite different names*

### Comparing `adapter-client-1.3.0/src/adapter_client/apps.py` & `adapter-client-2.0.0/src/adapter_client/apps.py`

 * *Files identical despite different names*

### Comparing `adapter-client-1.3.0/src/adapter_client/config.py` & `adapter-client-2.0.0/src/adapter_client/config.py`

 * *Files identical despite different names*

### Comparing `adapter-client-1.3.0/src/adapter_client/core/domain/model.py` & `adapter-client-2.0.0/src/adapter_client/core/domain/model.py`

 * *Files identical despite different names*

### Comparing `adapter-client-1.3.0/src/adapter_client/migrations/0001_initial.py` & `adapter-client-2.0.0/src/adapter_client/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `adapter-client-1.3.0/src/adapter_client/migrations/0002_alter_journalentry_options_config_adapter_interface_and_more.py` & `adapter-client-2.0.0/src/adapter_client/migrations/0002_alter_journalentry_options_config_adapter_interface_and_more.py`

 * *Files identical despite different names*

### Comparing `adapter-client-1.3.0/src/adapter_client/migrations/0003_message_transaction_code_alter_config_journal_config_and_more.py` & `adapter-client-2.0.0/src/adapter_client/migrations/0003_message_transaction_code_alter_config_journal_config_and_more.py`

 * *Files identical despite different names*

### Comparing `adapter-client-1.3.0/src/adapter_client/models.py` & `adapter-client-2.0.0/src/adapter_client/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,15 +183,15 @@
 
 class IncomingMessage(models.Model):
     """Входящее сообщение.
 
     Может быть как ответом на Find так и ответом на Get запрос.
     Это сообщение требуется обработать сервисом.
     """
-    message = models.ForeignKey(Message, on_delete=models.PROTECT)
+    message = models.OneToOneField(Message, on_delete=models.PROTECT)
     status = models.IntegerField(
         verbose_name=model.IncomingMessage.status.title,
         default=model.IncomingStatus.received.id,
         choices=[
             (item.id, item.verbose) for item in model.IncomingStatus
         ]
     )
```

### Comparing `adapter-client-1.3.0/src/adapter_client/tasks.py` & `adapter-client-2.0.0/src/adapter_client/tasks.py`

 * *Files identical despite different names*

### Comparing `adapter-client-1.3.0/src/adapter_client/utils.py` & `adapter-client-2.0.0/src/adapter_client/utils.py`

 * *Files identical despite different names*

### Comparing `adapter-client-1.3.0/src/adapter_client.egg-info/PKG-INFO` & `adapter-client-2.0.0/src/adapter_client.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,45 @@
 Metadata-Version: 2.1
 Name: adapter-client
-Version: 1.3.0
+Version: 2.0.0
 Summary: Клиент для взаимодействия со СМЭВ3 посредством Адаптера
 Author: BARS Group
 Author-email: education_dev@bars-open.ru
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Web Environment
 Classifier: Natural Language :: Russian
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Description-Content-Type: text/markdown
+Requires-Dist: pydantic<1.10.0,>=1.9.0
+Requires-Dist: zeep<4.2.0,>=4.1.0
+Requires-Dist: django
+Requires-Dist: celery<5.3.0; python_version == "3.7"
+Requires-Dist: celery; python_version > "3.7"
+Requires-Dist: django_celery_beat<2.6.0; python_version == "3.7"
+Requires-Dist: django_celery_beat; python_version > "3.7"
+Requires-Dist: django-postgres-partitioning==1.1.0
 Provides-Extra: opensearch
+Requires-Dist: opensearch-logger==1.2.2; extra == "opensearch"
 
 # Клиент для взаимодействия со СМЭВ3 посредством Адаптера
 ## Подключение
 settings:
 
     INSTALLED_APPS = [
         'adapter_client'
```

### Comparing `adapter-client-1.3.0/src/adapter_client.egg-info/SOURCES.txt` & `adapter-client-2.0.0/src/adapter_client.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -35,8 +35,9 @@
 src/adapter_client/core/__init__.py
 src/adapter_client/core/services.py
 src/adapter_client/core/domain/__init__.py
 src/adapter_client/core/domain/model.py
 src/adapter_client/migrations/0001_initial.py
 src/adapter_client/migrations/0002_alter_journalentry_options_config_adapter_interface_and_more.py
 src/adapter_client/migrations/0003_message_transaction_code_alter_config_journal_config_and_more.py
+src/adapter_client/migrations/0004_alter_incomingmessage_id.py
 src/adapter_client/migrations/__init__.py
```

