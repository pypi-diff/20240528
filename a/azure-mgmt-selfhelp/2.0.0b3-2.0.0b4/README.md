# Comparing `tmp/azure-mgmt-selfhelp-2.0.0b3.tar.gz` & `tmp/azure-mgmt-selfhelp-2.0.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure-mgmt-selfhelp-2.0.0b3.tar", last modified: Wed Apr 24 04:40:26 2024, max compression
+gzip compressed data, was "azure-mgmt-selfhelp-2.0.0b4.tar", last modified: Tue May 28 02:18:55 2024, max compression
```

## Comparing `azure-mgmt-selfhelp-2.0.0b3.tar` & `azure-mgmt-selfhelp-2.0.0b4.tar`

### file list

```diff
@@ -1,68 +1,66 @@
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-24 04:40:26.545424 azure-mgmt-selfhelp-2.0.0b3/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2803 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/CHANGELOG.md
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1074 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/LICENSE
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      214 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/MANIFEST.in
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5696 2024-04-24 04:40:26.545424 azure-mgmt-selfhelp-2.0.0b3/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2001 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/README.md
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      618 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/_meta.json
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-24 04:40:26.533424 azure-mgmt-selfhelp-2.0.0b3/azure/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-24 04:40:26.533424 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-24 04:40:26.537424 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      895 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3461 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8294 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/_self_help_mgmt_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    78873 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/_serialization.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      778 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/_vendor.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      488 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/_version.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-24 04:40:26.537424 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      842 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3509 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8490 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/_self_help_mgmt_client.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-24 04:40:26.541424 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1795 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8376 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/operations/_check_name_availability_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    15277 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/operations/_diagnostics_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7368 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/operations/_discovery_solution_nlp_subscription_scope_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7241 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/operations/_discovery_solution_nlp_tenant_scope_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7283 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/operations/_discovery_solution_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5546 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/operations/_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/operations/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    16587 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/operations/_simplified_solutions_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    32962 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/operations/_solution_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4709 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/operations/_solution_self_help_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    26887 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/operations/_troubleshooters_operations.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-24 04:40:26.541424 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/models/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5742 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/models/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    98429 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/models/_models_py3.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/models/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6275 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/models/_self_help_mgmt_client_enums.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-24 04:40:26.541424 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1795 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9518 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/operations/_check_name_availability_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    17826 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/operations/_diagnostics_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8533 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/operations/_discovery_solution_nlp_subscription_scope_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8167 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/operations/_discovery_solution_nlp_tenant_scope_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8260 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/operations/_discovery_solution_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6250 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/operations/_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/operations/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    19296 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/operations/_simplified_solutions_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    38193 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/operations/_solution_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5674 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/operations/_solution_self_help_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    33377 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/operations/_troubleshooters_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       26 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/py.typed
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-24 04:40:26.545424 azure-mgmt-selfhelp-2.0.0b3/azure_mgmt_selfhelp.egg-info/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5696 2024-04-24 04:40:26.000000 azure-mgmt-selfhelp-2.0.0b3/azure_mgmt_selfhelp.egg-info/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2556 2024-04-24 04:40:26.000000 azure-mgmt-selfhelp-2.0.0b3/azure_mgmt_selfhelp.egg-info/SOURCES.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-04-24 04:40:26.000000 azure-mgmt-selfhelp-2.0.0b3/azure_mgmt_selfhelp.egg-info/dependency_links.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-04-24 04:40:26.000000 azure-mgmt-selfhelp-2.0.0b3/azure_mgmt_selfhelp.egg-info/not-zip-safe
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       56 2024-04-24 04:40:26.000000 azure-mgmt-selfhelp-2.0.0b3/azure_mgmt_selfhelp.egg-info/requires.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        6 2024-04-24 04:40:26.000000 azure-mgmt-selfhelp-2.0.0b3/azure_mgmt_selfhelp.egg-info/top_level.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2024-04-24 04:40:26.545424 azure-mgmt-selfhelp-2.0.0b3/setup.cfg
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2769 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/setup.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-24 04:40:26.545424 azure-mgmt-selfhelp-2.0.0b3/tests/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2616 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/tests/conftest.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      741 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/tests/test_cli_mgmt_selfhelp.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-28 02:18:55.929283 azure-mgmt-selfhelp-2.0.0b4/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3205 2024-05-28 02:17:38.000000 azure-mgmt-selfhelp-2.0.0b4/CHANGELOG.md
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1074 2024-05-28 02:17:38.000000 azure-mgmt-selfhelp-2.0.0b4/LICENSE
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      214 2024-05-28 02:17:38.000000 azure-mgmt-selfhelp-2.0.0b4/MANIFEST.in
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6098 2024-05-28 02:18:55.929283 azure-mgmt-selfhelp-2.0.0b4/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2001 2024-05-28 02:17:38.000000 azure-mgmt-selfhelp-2.0.0b4/README.md
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      622 2024-05-28 02:17:38.000000 azure-mgmt-selfhelp-2.0.0b4/_meta.json
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-28 02:18:55.921284 azure-mgmt-selfhelp-2.0.0b4/azure/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-05-28 02:17:38.000000 azure-mgmt-selfhelp-2.0.0b4/azure/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-28 02:18:55.921284 azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-05-28 02:17:38.000000 azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-28 02:18:55.921284 azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      895 2024-05-28 02:17:38.000000 azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3147 2024-05-28 02:17:38.000000 azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-28 02:17:38.000000 azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7487 2024-05-28 02:17:38.000000 azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/_self_help_mgmt_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    78873 2024-05-28 02:17:38.000000 azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/_serialization.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      778 2024-05-28 02:17:38.000000 azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/_vendor.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      488 2024-05-28 02:17:38.000000 azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/_version.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-28 02:18:55.921284 azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/aio/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      842 2024-05-28 02:17:38.000000 azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/aio/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3195 2024-05-28 02:17:38.000000 azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/aio/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-28 02:17:38.000000 azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/aio/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7684 2024-05-28 02:17:38.000000 azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/aio/_self_help_mgmt_client.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-28 02:18:55.925284 azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/aio/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1590 2024-05-28 02:17:38.000000 azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/aio/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8684 2024-05-28 02:17:38.000000 azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/aio/operations/_check_name_availability_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    15561 2024-05-28 02:17:38.000000 azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/aio/operations/_diagnostics_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    13226 2024-05-28 02:17:38.000000 azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/aio/operations/_discovery_solution_nlp_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7523 2024-05-28 02:17:38.000000 azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/aio/operations/_discovery_solution_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5784 2024-05-28 02:17:38.000000 azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/aio/operations/_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-28 02:17:38.000000 azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/aio/operations/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    16871 2024-05-28 02:17:38.000000 azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/aio/operations/_simplified_solutions_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    33338 2024-05-28 02:17:38.000000 azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/aio/operations/_solution_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4947 2024-05-28 02:17:38.000000 azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/aio/operations/_solution_self_help_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    27309 2024-05-28 02:17:38.000000 azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/aio/operations/_troubleshooters_operations.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-28 02:18:55.925284 azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/models/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5742 2024-05-28 02:17:38.000000 azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/models/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    98569 2024-05-28 02:17:38.000000 azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/models/_models_py3.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-28 02:17:38.000000 azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/models/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6275 2024-05-28 02:17:38.000000 azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/models/_self_help_mgmt_client_enums.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-28 02:18:55.929283 azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1590 2024-05-28 02:17:38.000000 azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9826 2024-05-28 02:17:38.000000 azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/operations/_check_name_availability_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    18110 2024-05-28 02:17:38.000000 azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/operations/_diagnostics_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    15377 2024-05-28 02:17:38.000000 azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/operations/_discovery_solution_nlp_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8500 2024-05-28 02:17:38.000000 azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/operations/_discovery_solution_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6488 2024-05-28 02:17:38.000000 azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/operations/_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-28 02:17:38.000000 azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/operations/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    19580 2024-05-28 02:17:38.000000 azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/operations/_simplified_solutions_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    38569 2024-05-28 02:17:38.000000 azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/operations/_solution_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5912 2024-05-28 02:17:38.000000 azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/operations/_solution_self_help_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    33799 2024-05-28 02:17:38.000000 azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/operations/_troubleshooters_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       26 2024-05-28 02:17:38.000000 azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/py.typed
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-28 02:18:55.929283 azure-mgmt-selfhelp-2.0.0b4/azure_mgmt_selfhelp.egg-info/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6098 2024-05-28 02:18:55.000000 azure-mgmt-selfhelp-2.0.0b4/azure_mgmt_selfhelp.egg-info/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2350 2024-05-28 02:18:55.000000 azure-mgmt-selfhelp-2.0.0b4/azure_mgmt_selfhelp.egg-info/SOURCES.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-05-28 02:18:55.000000 azure-mgmt-selfhelp-2.0.0b4/azure_mgmt_selfhelp.egg-info/dependency_links.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-05-28 02:18:55.000000 azure-mgmt-selfhelp-2.0.0b4/azure_mgmt_selfhelp.egg-info/not-zip-safe
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       56 2024-05-28 02:18:55.000000 azure-mgmt-selfhelp-2.0.0b4/azure_mgmt_selfhelp.egg-info/requires.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        6 2024-05-28 02:18:55.000000 azure-mgmt-selfhelp-2.0.0b4/azure_mgmt_selfhelp.egg-info/top_level.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2024-05-28 02:18:55.929283 azure-mgmt-selfhelp-2.0.0b4/setup.cfg
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2769 2024-05-28 02:17:38.000000 azure-mgmt-selfhelp-2.0.0b4/setup.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-28 02:18:55.929283 azure-mgmt-selfhelp-2.0.0b4/tests/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2616 2024-05-28 02:17:38.000000 azure-mgmt-selfhelp-2.0.0b4/tests/conftest.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      741 2024-05-28 02:17:38.000000 azure-mgmt-selfhelp-2.0.0b4/tests/test_cli_mgmt_selfhelp.py
```

### Comparing `azure-mgmt-selfhelp-2.0.0b3/CHANGELOG.md` & `azure-mgmt-selfhelp-2.0.0b4/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,22 @@
 # Release History
 
+## 2.0.0b4 (2024-05-27)
+
+### Features Added
+
+  - Added operation CheckNameAvailabilityOperations.check_availability
+  - Added operation group DiscoverySolutionNLPOperations
+
+### Breaking Changes
+
+  - Removed operation CheckNameAvailabilityOperations.post
+  - Removed operation group DiscoverySolutionNLPSubscriptionScopeOperations
+  - Removed operation group DiscoverySolutionNLPTenantScopeOperations
+
 ## 2.0.0b3 (2024-04-22)
 
 ### Features Added
 
   - Added operation SolutionOperations.warm_up
   - Added operation group DiscoverySolutionNLPSubscriptionScopeOperations
   - Added operation group DiscoverySolutionNLPTenantScopeOperations
```

### Comparing `azure-mgmt-selfhelp-2.0.0b3/LICENSE` & `azure-mgmt-selfhelp-2.0.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `azure-mgmt-selfhelp-2.0.0b3/PKG-INFO` & `azure-mgmt-selfhelp-2.0.0b4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-selfhelp
-Version: 2.0.0b3
+Version: 2.0.0b4
 Summary: Microsoft Azure Selfhelp Management Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
 Classifier: Development Status :: 4 - Beta
@@ -82,14 +82,27 @@
 If you encounter any bugs or have suggestions, please file an issue in the
 [Issues](https://github.com/Azure/azure-sdk-for-python/issues)
 section of the project. 
 
 
 # Release History
 
+## 2.0.0b4 (2024-05-27)
+
+### Features Added
+
+  - Added operation CheckNameAvailabilityOperations.check_availability
+  - Added operation group DiscoverySolutionNLPOperations
+
+### Breaking Changes
+
+  - Removed operation CheckNameAvailabilityOperations.post
+  - Removed operation group DiscoverySolutionNLPSubscriptionScopeOperations
+  - Removed operation group DiscoverySolutionNLPTenantScopeOperations
+
 ## 2.0.0b3 (2024-04-22)
 
 ### Features Added
 
   - Added operation SolutionOperations.warm_up
   - Added operation group DiscoverySolutionNLPSubscriptionScopeOperations
   - Added operation group DiscoverySolutionNLPTenantScopeOperations
```

### Comparing `azure-mgmt-selfhelp-2.0.0b3/README.md` & `azure-mgmt-selfhelp-2.0.0b4/README.md`

 * *Files identical despite different names*

### Comparing `azure-mgmt-selfhelp-2.0.0b3/_meta.json` & `azure-mgmt-selfhelp-2.0.0b4/_meta.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6944444444444443%*

 * *Differences: {"'autorest'": "'3.10.2'",*

 * * "'autorest_command'": "'autorest specification/help/resource-manager/readme.md "*

 * *                       '--generate-sample=True --include-x-ms-examples-original-file=True --python '*

 * *                       '--python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk '*

 * *                       '--use=@autorest/python@6.13.16 --use=@autorest/modelerfour@4.27.0 '*

 * *                       "--version=3.10.2 --version-tolerant=False'",*

 * * "'commit'": "'c3cc9abe085093ba880ee3eeb792edb4fa78 […]*

```diff
@@ -1,11 +1,11 @@
 {
-    "autorest": "3.9.7",
-    "autorest_command": "autorest specification/help/resource-manager/readme.md --generate-sample=True --include-x-ms-examples-original-file=True --python --python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk --use=@autorest/python@6.13.7 --use=@autorest/modelerfour@4.27.0 --version=3.9.7 --version-tolerant=False",
-    "commit": "835b124ff8160d23823c0e770b4989ca79e7418c",
+    "autorest": "3.10.2",
+    "autorest_command": "autorest specification/help/resource-manager/readme.md --generate-sample=True --include-x-ms-examples-original-file=True --python --python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk --use=@autorest/python@6.13.16 --use=@autorest/modelerfour@4.27.0 --version=3.10.2 --version-tolerant=False",
+    "commit": "c3cc9abe085093ba880ee3eeb792edb4fa789553",
     "readme": "specification/help/resource-manager/readme.md",
     "repository_url": "https://github.com/Azure/azure-rest-api-specs",
     "use": [
-        "@autorest/python@6.13.7",
+        "@autorest/python@6.13.16",
         "@autorest/modelerfour@4.27.0"
     ]
 }
```

### Comparing `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/__init__.py` & `azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/_configuration.py` & `azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/aio/_configuration.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,61 +5,56 @@
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from typing import Any, TYPE_CHECKING
 
 from azure.core.pipeline import policies
-from azure.mgmt.core.policies import ARMChallengeAuthenticationPolicy, ARMHttpLoggingPolicy
+from azure.mgmt.core.policies import ARMHttpLoggingPolicy, AsyncARMChallengeAuthenticationPolicy
 
-from ._version import VERSION
+from .._version import VERSION
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
-    from azure.core.credentials import TokenCredential
+    from azure.core.credentials_async import AsyncTokenCredential
 
 
 class SelfHelpMgmtClientConfiguration:  # pylint: disable=too-many-instance-attributes,name-too-long
     """Configuration for SelfHelpMgmtClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure. Required.
-    :type credential: ~azure.core.credentials.TokenCredential
-    :param subscription_id: The ID of the target subscription. The value must be an UUID. Required.
-    :type subscription_id: str
+    :type credential: ~azure.core.credentials_async.AsyncTokenCredential
     :keyword api_version: Api Version. Default value is "2024-03-01-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
-    def __init__(self, credential: "TokenCredential", subscription_id: str, **kwargs: Any) -> None:
+    def __init__(self, credential: "AsyncTokenCredential", **kwargs: Any) -> None:
         api_version: str = kwargs.pop("api_version", "2024-03-01-preview")
 
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
-        if subscription_id is None:
-            raise ValueError("Parameter 'subscription_id' must not be None.")
 
         self.credential = credential
-        self.subscription_id = subscription_id
         self.api_version = api_version
         self.credential_scopes = kwargs.pop("credential_scopes", ["https://management.azure.com/.default"])
         kwargs.setdefault("sdk_moniker", "mgmt-selfhelp/{}".format(VERSION))
         self.polling_interval = kwargs.get("polling_interval", 30)
         self._configure(**kwargs)
 
     def _configure(self, **kwargs: Any) -> None:
         self.user_agent_policy = kwargs.get("user_agent_policy") or policies.UserAgentPolicy(**kwargs)
         self.headers_policy = kwargs.get("headers_policy") or policies.HeadersPolicy(**kwargs)
         self.proxy_policy = kwargs.get("proxy_policy") or policies.ProxyPolicy(**kwargs)
         self.logging_policy = kwargs.get("logging_policy") or policies.NetworkTraceLoggingPolicy(**kwargs)
         self.http_logging_policy = kwargs.get("http_logging_policy") or ARMHttpLoggingPolicy(**kwargs)
         self.custom_hook_policy = kwargs.get("custom_hook_policy") or policies.CustomHookPolicy(**kwargs)
-        self.redirect_policy = kwargs.get("redirect_policy") or policies.RedirectPolicy(**kwargs)
-        self.retry_policy = kwargs.get("retry_policy") or policies.RetryPolicy(**kwargs)
+        self.redirect_policy = kwargs.get("redirect_policy") or policies.AsyncRedirectPolicy(**kwargs)
+        self.retry_policy = kwargs.get("retry_policy") or policies.AsyncRetryPolicy(**kwargs)
         self.authentication_policy = kwargs.get("authentication_policy")
         if self.credential and not self.authentication_policy:
-            self.authentication_policy = ARMChallengeAuthenticationPolicy(
+            self.authentication_policy = AsyncARMChallengeAuthenticationPolicy(
                 self.credential, *self.credential_scopes, **kwargs
             )
```

### Comparing `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/_patch.py` & `azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/_self_help_mgmt_client.py` & `azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/_self_help_mgmt_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,16 +16,15 @@
 
 from . import models as _models
 from ._configuration import SelfHelpMgmtClientConfiguration
 from ._serialization import Deserializer, Serializer
 from .operations import (
     CheckNameAvailabilityOperations,
     DiagnosticsOperations,
-    DiscoverySolutionNLPSubscriptionScopeOperations,
-    DiscoverySolutionNLPTenantScopeOperations,
+    DiscoverySolutionNLPOperations,
     DiscoverySolutionOperations,
     Operations,
     SimplifiedSolutionsOperations,
     SolutionOperations,
     SolutionSelfHelpOperations,
     TroubleshootersOperations,
 )
@@ -51,42 +50,31 @@
     :vartype solution: azure.mgmt.selfhelp.operations.SolutionOperations
     :ivar simplified_solutions: SimplifiedSolutionsOperations operations
     :vartype simplified_solutions: azure.mgmt.selfhelp.operations.SimplifiedSolutionsOperations
     :ivar troubleshooters: TroubleshootersOperations operations
     :vartype troubleshooters: azure.mgmt.selfhelp.operations.TroubleshootersOperations
     :ivar solution_self_help: SolutionSelfHelpOperations operations
     :vartype solution_self_help: azure.mgmt.selfhelp.operations.SolutionSelfHelpOperations
-    :ivar discovery_solution_nlp_tenant_scope: DiscoverySolutionNLPTenantScopeOperations operations
-    :vartype discovery_solution_nlp_tenant_scope:
-     azure.mgmt.selfhelp.operations.DiscoverySolutionNLPTenantScopeOperations
-    :ivar discovery_solution_nlp_subscription_scope:
-     DiscoverySolutionNLPSubscriptionScopeOperations operations
-    :vartype discovery_solution_nlp_subscription_scope:
-     azure.mgmt.selfhelp.operations.DiscoverySolutionNLPSubscriptionScopeOperations
+    :ivar discovery_solution_nlp: DiscoverySolutionNLPOperations operations
+    :vartype discovery_solution_nlp: azure.mgmt.selfhelp.operations.DiscoverySolutionNLPOperations
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials.TokenCredential
-    :param subscription_id: The ID of the target subscription. The value must be an UUID. Required.
-    :type subscription_id: str
     :param base_url: Service URL. Default value is "https://management.azure.com".
     :type base_url: str
     :keyword api_version: Api Version. Default value is "2024-03-01-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
      Retry-After header is present.
     """
 
     def __init__(
-        self,
-        credential: "TokenCredential",
-        subscription_id: str,
-        base_url: str = "https://management.azure.com",
-        **kwargs: Any
+        self, credential: "TokenCredential", base_url: str = "https://management.azure.com", **kwargs: Any
     ) -> None:
-        self._config = SelfHelpMgmtClientConfiguration(credential=credential, subscription_id=subscription_id, **kwargs)
+        self._config = SelfHelpMgmtClientConfiguration(credential=credential, **kwargs)
         _policies = kwargs.pop("policies", None)
         if _policies is None:
             _policies = [
                 policies.RequestIdPolicy(**kwargs),
                 self._config.headers_policy,
                 self._config.user_agent_policy,
                 self._config.proxy_policy,
@@ -119,18 +107,15 @@
         self.simplified_solutions = SimplifiedSolutionsOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.troubleshooters = TroubleshootersOperations(self._client, self._config, self._serialize, self._deserialize)
         self.solution_self_help = SolutionSelfHelpOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
-        self.discovery_solution_nlp_tenant_scope = DiscoverySolutionNLPTenantScopeOperations(
-            self._client, self._config, self._serialize, self._deserialize
-        )
-        self.discovery_solution_nlp_subscription_scope = DiscoverySolutionNLPSubscriptionScopeOperations(
+        self.discovery_solution_nlp = DiscoverySolutionNLPOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
 
     def _send_request(self, request: HttpRequest, *, stream: bool = False, **kwargs: Any) -> HttpResponse:
         """Runs the network request through the client's chained policies.
 
         >>> from azure.core.rest import HttpRequest
```

### Comparing `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/_serialization.py` & `azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/_serialization.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/_vendor.py` & `azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/_vendor.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/__init__.py` & `azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/_configuration.py` & `azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/_configuration.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,61 +5,56 @@
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from typing import Any, TYPE_CHECKING
 
 from azure.core.pipeline import policies
-from azure.mgmt.core.policies import ARMHttpLoggingPolicy, AsyncARMChallengeAuthenticationPolicy
+from azure.mgmt.core.policies import ARMChallengeAuthenticationPolicy, ARMHttpLoggingPolicy
 
-from .._version import VERSION
+from ._version import VERSION
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
-    from azure.core.credentials_async import AsyncTokenCredential
+    from azure.core.credentials import TokenCredential
 
 
 class SelfHelpMgmtClientConfiguration:  # pylint: disable=too-many-instance-attributes,name-too-long
     """Configuration for SelfHelpMgmtClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure. Required.
-    :type credential: ~azure.core.credentials_async.AsyncTokenCredential
-    :param subscription_id: The ID of the target subscription. The value must be an UUID. Required.
-    :type subscription_id: str
+    :type credential: ~azure.core.credentials.TokenCredential
     :keyword api_version: Api Version. Default value is "2024-03-01-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
-    def __init__(self, credential: "AsyncTokenCredential", subscription_id: str, **kwargs: Any) -> None:
+    def __init__(self, credential: "TokenCredential", **kwargs: Any) -> None:
         api_version: str = kwargs.pop("api_version", "2024-03-01-preview")
 
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
-        if subscription_id is None:
-            raise ValueError("Parameter 'subscription_id' must not be None.")
 
         self.credential = credential
-        self.subscription_id = subscription_id
         self.api_version = api_version
         self.credential_scopes = kwargs.pop("credential_scopes", ["https://management.azure.com/.default"])
         kwargs.setdefault("sdk_moniker", "mgmt-selfhelp/{}".format(VERSION))
         self.polling_interval = kwargs.get("polling_interval", 30)
         self._configure(**kwargs)
 
     def _configure(self, **kwargs: Any) -> None:
         self.user_agent_policy = kwargs.get("user_agent_policy") or policies.UserAgentPolicy(**kwargs)
         self.headers_policy = kwargs.get("headers_policy") or policies.HeadersPolicy(**kwargs)
         self.proxy_policy = kwargs.get("proxy_policy") or policies.ProxyPolicy(**kwargs)
         self.logging_policy = kwargs.get("logging_policy") or policies.NetworkTraceLoggingPolicy(**kwargs)
         self.http_logging_policy = kwargs.get("http_logging_policy") or ARMHttpLoggingPolicy(**kwargs)
         self.custom_hook_policy = kwargs.get("custom_hook_policy") or policies.CustomHookPolicy(**kwargs)
-        self.redirect_policy = kwargs.get("redirect_policy") or policies.AsyncRedirectPolicy(**kwargs)
-        self.retry_policy = kwargs.get("retry_policy") or policies.AsyncRetryPolicy(**kwargs)
+        self.redirect_policy = kwargs.get("redirect_policy") or policies.RedirectPolicy(**kwargs)
+        self.retry_policy = kwargs.get("retry_policy") or policies.RetryPolicy(**kwargs)
         self.authentication_policy = kwargs.get("authentication_policy")
         if self.credential and not self.authentication_policy:
-            self.authentication_policy = AsyncARMChallengeAuthenticationPolicy(
+            self.authentication_policy = ARMChallengeAuthenticationPolicy(
                 self.credential, *self.credential_scopes, **kwargs
             )
```

### Comparing `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/_patch.py` & `azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/_self_help_mgmt_client.py` & `azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/aio/_self_help_mgmt_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,16 +16,15 @@
 
 from .. import models as _models
 from .._serialization import Deserializer, Serializer
 from ._configuration import SelfHelpMgmtClientConfiguration
 from .operations import (
     CheckNameAvailabilityOperations,
     DiagnosticsOperations,
-    DiscoverySolutionNLPSubscriptionScopeOperations,
-    DiscoverySolutionNLPTenantScopeOperations,
+    DiscoverySolutionNLPOperations,
     DiscoverySolutionOperations,
     Operations,
     SimplifiedSolutionsOperations,
     SolutionOperations,
     SolutionSelfHelpOperations,
     TroubleshootersOperations,
 )
@@ -51,42 +50,32 @@
     :vartype solution: azure.mgmt.selfhelp.aio.operations.SolutionOperations
     :ivar simplified_solutions: SimplifiedSolutionsOperations operations
     :vartype simplified_solutions: azure.mgmt.selfhelp.aio.operations.SimplifiedSolutionsOperations
     :ivar troubleshooters: TroubleshootersOperations operations
     :vartype troubleshooters: azure.mgmt.selfhelp.aio.operations.TroubleshootersOperations
     :ivar solution_self_help: SolutionSelfHelpOperations operations
     :vartype solution_self_help: azure.mgmt.selfhelp.aio.operations.SolutionSelfHelpOperations
-    :ivar discovery_solution_nlp_tenant_scope: DiscoverySolutionNLPTenantScopeOperations operations
-    :vartype discovery_solution_nlp_tenant_scope:
-     azure.mgmt.selfhelp.aio.operations.DiscoverySolutionNLPTenantScopeOperations
-    :ivar discovery_solution_nlp_subscription_scope:
-     DiscoverySolutionNLPSubscriptionScopeOperations operations
-    :vartype discovery_solution_nlp_subscription_scope:
-     azure.mgmt.selfhelp.aio.operations.DiscoverySolutionNLPSubscriptionScopeOperations
+    :ivar discovery_solution_nlp: DiscoverySolutionNLPOperations operations
+    :vartype discovery_solution_nlp:
+     azure.mgmt.selfhelp.aio.operations.DiscoverySolutionNLPOperations
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials_async.AsyncTokenCredential
-    :param subscription_id: The ID of the target subscription. The value must be an UUID. Required.
-    :type subscription_id: str
     :param base_url: Service URL. Default value is "https://management.azure.com".
     :type base_url: str
     :keyword api_version: Api Version. Default value is "2024-03-01-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
      Retry-After header is present.
     """
 
     def __init__(
-        self,
-        credential: "AsyncTokenCredential",
-        subscription_id: str,
-        base_url: str = "https://management.azure.com",
-        **kwargs: Any
+        self, credential: "AsyncTokenCredential", base_url: str = "https://management.azure.com", **kwargs: Any
     ) -> None:
-        self._config = SelfHelpMgmtClientConfiguration(credential=credential, subscription_id=subscription_id, **kwargs)
+        self._config = SelfHelpMgmtClientConfiguration(credential=credential, **kwargs)
         _policies = kwargs.pop("policies", None)
         if _policies is None:
             _policies = [
                 policies.RequestIdPolicy(**kwargs),
                 self._config.headers_policy,
                 self._config.user_agent_policy,
                 self._config.proxy_policy,
@@ -119,18 +108,15 @@
         self.simplified_solutions = SimplifiedSolutionsOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.troubleshooters = TroubleshootersOperations(self._client, self._config, self._serialize, self._deserialize)
         self.solution_self_help = SolutionSelfHelpOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
-        self.discovery_solution_nlp_tenant_scope = DiscoverySolutionNLPTenantScopeOperations(
-            self._client, self._config, self._serialize, self._deserialize
-        )
-        self.discovery_solution_nlp_subscription_scope = DiscoverySolutionNLPSubscriptionScopeOperations(
+        self.discovery_solution_nlp = DiscoverySolutionNLPOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
 
     def _send_request(
         self, request: HttpRequest, *, stream: bool = False, **kwargs: Any
     ) -> Awaitable[AsyncHttpResponse]:
         """Runs the network request through the client's chained policies.
```

### Comparing `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/operations/__init__.py` & `azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/aio/operations/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,28 +10,26 @@
 from ._check_name_availability_operations import CheckNameAvailabilityOperations
 from ._diagnostics_operations import DiagnosticsOperations
 from ._discovery_solution_operations import DiscoverySolutionOperations
 from ._solution_operations import SolutionOperations
 from ._simplified_solutions_operations import SimplifiedSolutionsOperations
 from ._troubleshooters_operations import TroubleshootersOperations
 from ._solution_self_help_operations import SolutionSelfHelpOperations
-from ._discovery_solution_nlp_tenant_scope_operations import DiscoverySolutionNLPTenantScopeOperations
-from ._discovery_solution_nlp_subscription_scope_operations import DiscoverySolutionNLPSubscriptionScopeOperations
+from ._discovery_solution_nlp_operations import DiscoverySolutionNLPOperations
 
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "Operations",
     "CheckNameAvailabilityOperations",
     "DiagnosticsOperations",
     "DiscoverySolutionOperations",
     "SolutionOperations",
     "SimplifiedSolutionsOperations",
     "TroubleshootersOperations",
     "SolutionSelfHelpOperations",
-    "DiscoverySolutionNLPTenantScopeOperations",
-    "DiscoverySolutionNLPSubscriptionScopeOperations",
+    "DiscoverySolutionNLPOperations",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 _patch_sdk()
```

### Comparing `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/operations/_check_name_availability_operations.py` & `azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/aio/operations/_check_name_availability_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
-from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, overload
+import sys
+from typing import Any, Callable, Dict, IO, Optional, Type, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
@@ -22,16 +23,20 @@
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator_async import distributed_trace_async
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
-from ...operations._check_name_availability_operations import build_post_request
+from ...operations._check_name_availability_operations import build_check_availability_request
 
+if sys.version_info >= (3, 9):
+    from collections.abc import MutableMapping
+else:
+    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class CheckNameAvailabilityOperations:
     """
     .. warning::
@@ -48,15 +53,15 @@
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @overload
-    async def post(
+    async def check_availability(
         self,
         scope: str,
         check_name_availability_request: Optional[_models.CheckNameAvailabilityRequest] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.CheckNameAvailabilityResponse:
@@ -75,15 +80,15 @@
         :paramtype content_type: str
         :return: CheckNameAvailabilityResponse or the result of cls(response)
         :rtype: ~azure.mgmt.selfhelp.models.CheckNameAvailabilityResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
-    async def post(
+    async def check_availability(
         self,
         scope: str,
         check_name_availability_request: Optional[IO[bytes]] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.CheckNameAvailabilityResponse:
@@ -102,15 +107,15 @@
         :paramtype content_type: str
         :return: CheckNameAvailabilityResponse or the result of cls(response)
         :rtype: ~azure.mgmt.selfhelp.models.CheckNameAvailabilityResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
-    async def post(
+    async def check_availability(
         self,
         scope: str,
         check_name_availability_request: Optional[Union[_models.CheckNameAvailabilityRequest, IO[bytes]]] = None,
         **kwargs: Any
     ) -> _models.CheckNameAvailabilityResponse:
         """This API is used to check the uniqueness of a resource name used for a diagnostic,
         troubleshooter or solutions.
@@ -123,15 +128,15 @@
          either a CheckNameAvailabilityRequest type or a IO[bytes] type. Default value is None.
         :type check_name_availability_request: ~azure.mgmt.selfhelp.models.CheckNameAvailabilityRequest
          or IO[bytes]
         :return: CheckNameAvailabilityResponse or the result of cls(response)
         :rtype: ~azure.mgmt.selfhelp.models.CheckNameAvailabilityResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -149,15 +154,15 @@
             _content = check_name_availability_request
         else:
             if check_name_availability_request is not None:
                 _json = self._serialize.body(check_name_availability_request, "CheckNameAvailabilityRequest")
             else:
                 _json = None
 
-        _request = build_post_request(
+        _request = build_check_availability_request(
             scope=scope,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
             headers=_headers,
             params=_params,
```

### Comparing `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/operations/_diagnostics_operations.py` & `azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/aio/operations/_diagnostics_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
-from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
+import sys
+from typing import Any, Callable, Dict, IO, Optional, Type, TypeVar, Union, cast, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
@@ -26,14 +27,18 @@
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.async_arm_polling import AsyncARMPolling
 
 from ... import models as _models
 from ..._vendor import _convert_request
 from ...operations._diagnostics_operations import build_create_request, build_get_request
 
+if sys.version_info >= (3, 9):
+    from collections.abc import MutableMapping
+else:
+    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class DiagnosticsOperations:
     """
     .. warning::
@@ -56,15 +61,15 @@
     async def _create_initial(
         self,
         scope: str,
         diagnostics_resource_name: str,
         diagnostic_resource_request: Optional[Union[_models.DiagnosticResource, IO[bytes]]] = None,
         **kwargs: Any
     ) -> _models.DiagnosticResource:
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -275,15 +280,15 @@
         :type scope: str
         :param diagnostics_resource_name: Unique resource name for insight resources. Required.
         :type diagnostics_resource_name: str
         :return: DiagnosticResource or the result of cls(response)
         :rtype: ~azure.mgmt.selfhelp.models.DiagnosticResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
```

### Comparing `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/operations/_discovery_solution_nlp_subscription_scope_operations.py` & `azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/operations/_operations.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,166 +2,155 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-from io import IOBase
-from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, overload
+import sys
+from typing import Any, Callable, Dict, Iterable, Optional, Type, TypeVar
+import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
     map_error,
 )
+from azure.core.paging import ItemPaged
 from azure.core.pipeline import PipelineResponse
-from azure.core.pipeline.transport import AsyncHttpResponse
+from azure.core.pipeline.transport import HttpResponse
 from azure.core.rest import HttpRequest
-from azure.core.tracing.decorator_async import distributed_trace_async
+from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
-from ... import models as _models
-from ..._vendor import _convert_request
-from ...operations._discovery_solution_nlp_subscription_scope_operations import build_post_request
-
+from .. import models as _models
+from .._serialization import Serializer
+from .._vendor import _convert_request
+
+if sys.version_info >= (3, 9):
+    from collections.abc import MutableMapping
+else:
+    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
-ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
+ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
+
+_SERIALIZER = Serializer()
+_SERIALIZER.client_side_validation = False
+
+
+def build_list_request(**kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-preview"))
+    accept = _headers.pop("Accept", "application/json")
 
+    # Construct URL
+    _url = kwargs.pop("template_url", "/providers/Microsoft.Help/operations")
 
-class DiscoverySolutionNLPSubscriptionScopeOperations:  # pylint: disable=name-too-long
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
+
+
+class Operations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.selfhelp.aio.SelfHelpMgmtClient`'s
-        :attr:`discovery_solution_nlp_subscription_scope` attribute.
+        :class:`~azure.mgmt.selfhelp.SelfHelpMgmtClient`'s
+        :attr:`operations` attribute.
     """
 
     models = _models
 
-    def __init__(self, *args, **kwargs) -> None:
+    def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
-    @overload
-    async def post(
-        self,
-        discover_solution_request: Optional[_models.DiscoveryNlpRequest] = None,
-        *,
-        content_type: str = "application/json",
-        **kwargs: Any
-    ) -> _models.DiscoveryNlpResponse:
-        """Search for relevant Azure Diagnostics, Solutions and Troubleshooters using a natural language
-        issue summary and subscription.
-
-        :param discover_solution_request: Request body for discovering solutions using NLP. Default
-         value is None.
-        :type discover_solution_request: ~azure.mgmt.selfhelp.models.DiscoveryNlpRequest
-        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
-         Default value is "application/json".
-        :paramtype content_type: str
-        :return: DiscoveryNlpResponse or the result of cls(response)
-        :rtype: ~azure.mgmt.selfhelp.models.DiscoveryNlpResponse
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
+    @distributed_trace
+    def list(self, **kwargs: Any) -> Iterable["_models.Operation"]:
+        """Returns list of operations.
 
-    @overload
-    async def post(
-        self,
-        discover_solution_request: Optional[IO[bytes]] = None,
-        *,
-        content_type: str = "application/json",
-        **kwargs: Any
-    ) -> _models.DiscoveryNlpResponse:
-        """Search for relevant Azure Diagnostics, Solutions and Troubleshooters using a natural language
-        issue summary and subscription.
-
-        :param discover_solution_request: Request body for discovering solutions using NLP. Default
-         value is None.
-        :type discover_solution_request: IO[bytes]
-        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
-         Default value is "application/json".
-        :paramtype content_type: str
-        :return: DiscoveryNlpResponse or the result of cls(response)
-        :rtype: ~azure.mgmt.selfhelp.models.DiscoveryNlpResponse
+        :return: An iterator like instance of either Operation or the result of cls(response)
+        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.selfhelp.models.Operation]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    @distributed_trace_async
-    async def post(
-        self, discover_solution_request: Optional[Union[_models.DiscoveryNlpRequest, IO[bytes]]] = None, **kwargs: Any
-    ) -> _models.DiscoveryNlpResponse:
-        """Search for relevant Azure Diagnostics, Solutions and Troubleshooters using a natural language
-        issue summary and subscription.
-
-        :param discover_solution_request: Request body for discovering solutions using NLP. Is either a
-         DiscoveryNlpRequest type or a IO[bytes] type. Default value is None.
-        :type discover_solution_request: ~azure.mgmt.selfhelp.models.DiscoveryNlpRequest or IO[bytes]
-        :return: DiscoveryNlpResponse or the result of cls(response)
-        :rtype: ~azure.mgmt.selfhelp.models.DiscoveryNlpResponse
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
-        error_map = {
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.OperationListResult] = kwargs.pop("cls", None)
+
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
-        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+        def prepare_request(next_link=None):
+            if not next_link:
 
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[_models.DiscoveryNlpResponse] = kwargs.pop("cls", None)
+                _request = build_list_request(
+                    api_version=api_version,
+                    headers=_headers,
+                    params=_params,
+                )
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
-        content_type = content_type or "application/json"
-        _json = None
-        _content = None
-        if isinstance(discover_solution_request, (IOBase, bytes)):
-            _content = discover_solution_request
-        else:
-            if discover_solution_request is not None:
-                _json = self._serialize.body(discover_solution_request, "DiscoveryNlpRequest")
             else:
-                _json = None
-
-        _request = build_post_request(
-            subscription_id=self._config.subscription_id,
-            api_version=api_version,
-            content_type=content_type,
-            json=_json,
-            content=_content,
-            headers=_headers,
-            params=_params,
-        )
-        _request = _convert_request(_request)
-        _request.url = self._client.format_url(_request.url)
-
-        _stream = False
-        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            _request, stream=_stream, **kwargs
-        )
-
-        response = pipeline_response.http_response
-
-        if response.status_code not in [200]:
-            map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
-            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
-
-        deserialized = self._deserialize("DiscoveryNlpResponse", pipeline_response)
+                # make call to next link with the client's api-version
+                _parsed_next_link = urllib.parse.urlparse(next_link)
+                _next_request_params = case_insensitive_dict(
+                    {
+                        key: [urllib.parse.quote(v) for v in value]
+                        for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
+                    }
+                )
+                _next_request_params["api-version"] = self._config.api_version
+                _request = HttpRequest(
+                    "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
+                )
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
+
+        def extract_data(pipeline_response):
+            deserialized = self._deserialize("OperationListResult", pipeline_response)
+            list_of_elem = deserialized.value
+            if cls:
+                list_of_elem = cls(list_of_elem)  # type: ignore
+            return deserialized.next_link or None, iter(list_of_elem)
+
+        def get_next(next_link=None):
+            _request = prepare_request(next_link)
+
+            _stream = False
+            pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+            response = pipeline_response.http_response
+
+            if response.status_code not in [200]:
+                map_error(status_code=response.status_code, response=response, error_map=error_map)
+                error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
+                raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        if cls:
-            return cls(pipeline_response, deserialized, {})  # type: ignore
+            return pipeline_response
 
-        return deserialized  # type: ignore
+        return ItemPaged(get_next, extract_data)
```

### Comparing `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/operations/_discovery_solution_nlp_tenant_scope_operations.py` & `azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/aio/operations/_operations.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,165 +2,133 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-from io import IOBase
-from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, overload
+import sys
+from typing import Any, AsyncIterable, Callable, Dict, Optional, Type, TypeVar
+import urllib.parse
 
+from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
     map_error,
 )
 from azure.core.pipeline import PipelineResponse
 from azure.core.pipeline.transport import AsyncHttpResponse
 from azure.core.rest import HttpRequest
-from azure.core.tracing.decorator_async import distributed_trace_async
+from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
-from ...operations._discovery_solution_nlp_tenant_scope_operations import build_post_request
+from ...operations._operations import build_list_request
 
+if sys.version_info >= (3, 9):
+    from collections.abc import MutableMapping
+else:
+    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
-class DiscoverySolutionNLPTenantScopeOperations:  # pylint: disable=name-too-long
+class Operations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.selfhelp.aio.SelfHelpMgmtClient`'s
-        :attr:`discovery_solution_nlp_tenant_scope` attribute.
+        :attr:`operations` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
-    @overload
-    async def post(
-        self,
-        discover_solution_request: Optional[_models.DiscoveryNlpRequest] = None,
-        *,
-        content_type: str = "application/json",
-        **kwargs: Any
-    ) -> _models.DiscoveryNlpResponse:
-        """Search for relevant Azure Diagnostics, Solutions and Troubleshooters using a natural language
-        issue summary.
-
-        :param discover_solution_request: Request body for discovering solutions using NLP. Default
-         value is None.
-        :type discover_solution_request: ~azure.mgmt.selfhelp.models.DiscoveryNlpRequest
-        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
-         Default value is "application/json".
-        :paramtype content_type: str
-        :return: DiscoveryNlpResponse or the result of cls(response)
-        :rtype: ~azure.mgmt.selfhelp.models.DiscoveryNlpResponse
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
+    @distributed_trace
+    def list(self, **kwargs: Any) -> AsyncIterable["_models.Operation"]:
+        """Returns list of operations.
 
-    @overload
-    async def post(
-        self,
-        discover_solution_request: Optional[IO[bytes]] = None,
-        *,
-        content_type: str = "application/json",
-        **kwargs: Any
-    ) -> _models.DiscoveryNlpResponse:
-        """Search for relevant Azure Diagnostics, Solutions and Troubleshooters using a natural language
-        issue summary.
-
-        :param discover_solution_request: Request body for discovering solutions using NLP. Default
-         value is None.
-        :type discover_solution_request: IO[bytes]
-        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
-         Default value is "application/json".
-        :paramtype content_type: str
-        :return: DiscoveryNlpResponse or the result of cls(response)
-        :rtype: ~azure.mgmt.selfhelp.models.DiscoveryNlpResponse
+        :return: An iterator like instance of either Operation or the result of cls(response)
+        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.selfhelp.models.Operation]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    @distributed_trace_async
-    async def post(
-        self, discover_solution_request: Optional[Union[_models.DiscoveryNlpRequest, IO[bytes]]] = None, **kwargs: Any
-    ) -> _models.DiscoveryNlpResponse:
-        """Search for relevant Azure Diagnostics, Solutions and Troubleshooters using a natural language
-        issue summary.
-
-        :param discover_solution_request: Request body for discovering solutions using NLP. Is either a
-         DiscoveryNlpRequest type or a IO[bytes] type. Default value is None.
-        :type discover_solution_request: ~azure.mgmt.selfhelp.models.DiscoveryNlpRequest or IO[bytes]
-        :return: DiscoveryNlpResponse or the result of cls(response)
-        :rtype: ~azure.mgmt.selfhelp.models.DiscoveryNlpResponse
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
-        error_map = {
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.OperationListResult] = kwargs.pop("cls", None)
+
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
-        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+        def prepare_request(next_link=None):
+            if not next_link:
 
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[_models.DiscoveryNlpResponse] = kwargs.pop("cls", None)
+                _request = build_list_request(
+                    api_version=api_version,
+                    headers=_headers,
+                    params=_params,
+                )
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
-        content_type = content_type or "application/json"
-        _json = None
-        _content = None
-        if isinstance(discover_solution_request, (IOBase, bytes)):
-            _content = discover_solution_request
-        else:
-            if discover_solution_request is not None:
-                _json = self._serialize.body(discover_solution_request, "DiscoveryNlpRequest")
             else:
-                _json = None
-
-        _request = build_post_request(
-            api_version=api_version,
-            content_type=content_type,
-            json=_json,
-            content=_content,
-            headers=_headers,
-            params=_params,
-        )
-        _request = _convert_request(_request)
-        _request.url = self._client.format_url(_request.url)
-
-        _stream = False
-        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            _request, stream=_stream, **kwargs
-        )
-
-        response = pipeline_response.http_response
-
-        if response.status_code not in [200]:
-            map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
-            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
-
-        deserialized = self._deserialize("DiscoveryNlpResponse", pipeline_response)
+                # make call to next link with the client's api-version
+                _parsed_next_link = urllib.parse.urlparse(next_link)
+                _next_request_params = case_insensitive_dict(
+                    {
+                        key: [urllib.parse.quote(v) for v in value]
+                        for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
+                    }
+                )
+                _next_request_params["api-version"] = self._config.api_version
+                _request = HttpRequest(
+                    "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
+                )
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
+
+        async def extract_data(pipeline_response):
+            deserialized = self._deserialize("OperationListResult", pipeline_response)
+            list_of_elem = deserialized.value
+            if cls:
+                list_of_elem = cls(list_of_elem)  # type: ignore
+            return deserialized.next_link or None, AsyncList(list_of_elem)
+
+        async def get_next(next_link=None):
+            _request = prepare_request(next_link)
+
+            _stream = False
+            pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+            response = pipeline_response.http_response
+
+            if response.status_code not in [200]:
+                map_error(status_code=response.status_code, response=response, error_map=error_map)
+                error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
+                raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        if cls:
-            return cls(pipeline_response, deserialized, {})  # type: ignore
+            return pipeline_response
 
-        return deserialized  # type: ignore
+        return AsyncItemPaged(get_next, extract_data)
```

### Comparing `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/operations/_discovery_solution_operations.py` & `azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/aio/operations/_discovery_solution_operations.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-from typing import Any, AsyncIterable, Callable, Dict, Optional, TypeVar
+import sys
+from typing import Any, AsyncIterable, Callable, Dict, Optional, Type, TypeVar
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -25,14 +26,18 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
 from ...operations._discovery_solution_operations import build_list_request
 
+if sys.version_info >= (3, 9):
+    from collections.abc import MutableMapping
+else:
+    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class DiscoverySolutionOperations:
     """
     .. warning::
@@ -54,19 +59,19 @@
 
     @distributed_trace
     def list(
         self, filter: Optional[str] = None, skiptoken: Optional[str] = None, **kwargs: Any
     ) -> AsyncIterable["_models.SolutionMetadataResource"]:
         """Lists the relevant Azure Diagnostics, Solutions and Troubleshooters using
         `problemClassification API
-        <https://learn.microsoft.com/rest/api/support/problem-classifications/list?tabs=HTTP>`_\ ) AND
+        <https://learn.microsoft.com/rest/api/support/problem-classifications/list?tabs=HTTP>`_\\ ) AND
         resourceUri or resourceType.:code:`<br/>` Discovery Solutions is the initial entry point within
         Help API, which identifies relevant Azure diagnostics and solutions. :code:`<br/>`:code:`<br/>`
         Required Input :  problemClassificationId (Use the `problemClassification API
-        <https://learn.microsoft.com/rest/api/support/problem-classifications/list?tabs=HTTP>`_\ )
+        <https://learn.microsoft.com/rest/api/support/problem-classifications/list?tabs=HTTP>`_\\ )
         :code:`<br/>`Optional input: resourceUri OR resource Type :code:`<br/>`:code:`<br/>`
         :code:`<b>Note: </b>`  ‘requiredInputs’ from Discovery solutions response must be passed via
         ‘additionalParameters’ as an input to Diagnostics and Solutions API.
 
         :param filter: 'ProblemClassificationId' is a mandatory filter to get solutions ids. It also
          supports optional 'ResourceType' and 'SolutionType' filters. The `$filter
          <https://learn.microsoft.com/en-us/odata/webapi/first-odata-api#filter>`_ supports only 'and',
@@ -84,15 +89,15 @@
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.DiscoveryResponse] = kwargs.pop("cls", None)
 
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
```

### Comparing `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/operations/_operations.py` & `azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/aio/operations/_solution_self_help_operations.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,128 +2,112 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-from typing import Any, AsyncIterable, Callable, Dict, Optional, TypeVar
-import urllib.parse
+import sys
+from typing import Any, Callable, Dict, Optional, Type, TypeVar
 
-from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
     map_error,
 )
 from azure.core.pipeline import PipelineResponse
 from azure.core.pipeline.transport import AsyncHttpResponse
 from azure.core.rest import HttpRequest
-from azure.core.tracing.decorator import distributed_trace
+from azure.core.tracing.decorator_async import distributed_trace_async
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
-from ...operations._operations import build_list_request
+from ...operations._solution_self_help_operations import build_get_request
 
+if sys.version_info >= (3, 9):
+    from collections.abc import MutableMapping
+else:
+    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
-class Operations:
+class SolutionSelfHelpOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.selfhelp.aio.SelfHelpMgmtClient`'s
-        :attr:`operations` attribute.
+        :attr:`solution_self_help` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
-    @distributed_trace
-    def list(self, **kwargs: Any) -> AsyncIterable["_models.Operation"]:
-        """Returns list of operations.
-
-        :return: An iterator like instance of either Operation or the result of cls(response)
-        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.selfhelp.models.Operation]
+    @distributed_trace_async
+    async def get(self, solution_id: str, **kwargs: Any) -> _models.SolutionResourceSelfHelp:
+        """Gets Self Help Solutions for a given solutionId. Self Help Solutions consist of rich
+        instructional video tutorials, links and guides to public documentation related to a specific
+        problem that enables users to troubleshoot Azure issues.
+
+        :param solution_id: SolutionId is a unique id to identify a solution. You can retrieve the
+         solution id using the Discovery api -
+         https://learn.microsoft.com/en-us/rest/api/help/discovery-solution/list?view=rest-help-2023-09-01-preview&tabs=HTTP.
+         Required.
+        :type solution_id: str
+        :return: SolutionResourceSelfHelp or the result of cls(response)
+        :rtype: ~azure.mgmt.selfhelp.models.SolutionResourceSelfHelp
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        _headers = kwargs.pop("headers", {}) or {}
-        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        cls: ClsType[_models.OperationListResult] = kwargs.pop("cls", None)
-
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
-        def prepare_request(next_link=None):
-            if not next_link:
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.SolutionResourceSelfHelp] = kwargs.pop("cls", None)
+
+        _request = build_get_request(
+            solution_id=solution_id,
+            api_version=api_version,
+            headers=_headers,
+            params=_params,
+        )
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
+            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-                _request = build_list_request(
-                    api_version=api_version,
-                    headers=_headers,
-                    params=_params,
-                )
-                _request = _convert_request(_request)
-                _request.url = self._client.format_url(_request.url)
-
-            else:
-                # make call to next link with the client's api-version
-                _parsed_next_link = urllib.parse.urlparse(next_link)
-                _next_request_params = case_insensitive_dict(
-                    {
-                        key: [urllib.parse.quote(v) for v in value]
-                        for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
-                    }
-                )
-                _next_request_params["api-version"] = self._config.api_version
-                _request = HttpRequest(
-                    "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
-                )
-                _request = _convert_request(_request)
-                _request.url = self._client.format_url(_request.url)
-                _request.method = "GET"
-            return _request
-
-        async def extract_data(pipeline_response):
-            deserialized = self._deserialize("OperationListResult", pipeline_response)
-            list_of_elem = deserialized.value
-            if cls:
-                list_of_elem = cls(list_of_elem)  # type: ignore
-            return deserialized.next_link or None, AsyncList(list_of_elem)
-
-        async def get_next(next_link=None):
-            _request = prepare_request(next_link)
-
-            _stream = False
-            pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                _request, stream=_stream, **kwargs
-            )
-            response = pipeline_response.http_response
-
-            if response.status_code not in [200]:
-                map_error(status_code=response.status_code, response=response, error_map=error_map)
-                error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
-                raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
+        deserialized = self._deserialize("SolutionResourceSelfHelp", pipeline_response)
 
-            return pipeline_response
+        if cls:
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-        return AsyncItemPaged(get_next, extract_data)
+        return deserialized  # type: ignore
```

### Comparing `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/operations/_patch.py` & `azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/operations/_simplified_solutions_operations.py` & `azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/aio/operations/_simplified_solutions_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
-from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
+import sys
+from typing import Any, Callable, Dict, IO, Optional, Type, TypeVar, Union, cast, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
@@ -26,14 +27,18 @@
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.async_arm_polling import AsyncARMPolling
 
 from ... import models as _models
 from ..._vendor import _convert_request
 from ...operations._simplified_solutions_operations import build_create_request, build_get_request
 
+if sys.version_info >= (3, 9):
+    from collections.abc import MutableMapping
+else:
+    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class SimplifiedSolutionsOperations:
     """
     .. warning::
@@ -56,15 +61,15 @@
     async def _create_initial(
         self,
         scope: str,
         simplified_solutions_resource_name: str,
         simplified_solutions_request_body: Optional[Union[_models.SimplifiedSolutionsResource, IO[bytes]]] = None,
         **kwargs: Any
     ) -> _models.SimplifiedSolutionsResource:
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -289,15 +294,15 @@
         :type scope: str
         :param simplified_solutions_resource_name: Simplified Solutions Resource Name. Required.
         :type simplified_solutions_resource_name: str
         :return: SimplifiedSolutionsResource or the result of cls(response)
         :rtype: ~azure.mgmt.selfhelp.models.SimplifiedSolutionsResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
```

### Comparing `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/operations/_solution_operations.py` & `azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/aio/operations/_solution_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
-from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
+import sys
+from typing import Any, Callable, Dict, IO, Optional, Type, TypeVar, Union, cast, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
@@ -31,14 +32,18 @@
 from ...operations._solution_operations import (
     build_create_request,
     build_get_request,
     build_update_request,
     build_warm_up_request,
 )
 
+if sys.version_info >= (3, 9):
+    from collections.abc import MutableMapping
+else:
+    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class SolutionOperations:
     """
     .. warning::
@@ -61,15 +66,15 @@
     async def _create_initial(
         self,
         scope: str,
         solution_resource_name: str,
         solution_request_body: Optional[Union[_models.SolutionResource, IO[bytes]]] = None,
         **kwargs: Any
     ) -> _models.SolutionResource:
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -294,15 +299,15 @@
         :type scope: str
         :param solution_resource_name: Solution resource Name. Required.
         :type solution_resource_name: str
         :return: SolutionResource or the result of cls(response)
         :rtype: ~azure.mgmt.selfhelp.models.SolutionResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -344,15 +349,15 @@
     async def _update_initial(
         self,
         scope: str,
         solution_resource_name: str,
         solution_patch_request_body: Optional[Union[_models.SolutionPatchRequestBody, IO[bytes]]] = None,
         **kwargs: Any
     ) -> _models.SolutionResource:
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -632,15 +637,15 @@
          None.
         :type solution_warm_up_request_body: ~azure.mgmt.selfhelp.models.SolutionWarmUpRequestBody or
          IO[bytes]
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
```

### Comparing `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/operations/_solution_self_help_operations.py` & `azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/operations/_solution_self_help_operations.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,74 +2,106 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-from typing import Any, Callable, Dict, Optional, TypeVar
+import sys
+from typing import Any, Callable, Dict, Optional, Type, TypeVar
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
     map_error,
 )
 from azure.core.pipeline import PipelineResponse
-from azure.core.pipeline.transport import AsyncHttpResponse
+from azure.core.pipeline.transport import HttpResponse
 from azure.core.rest import HttpRequest
-from azure.core.tracing.decorator_async import distributed_trace_async
+from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
-from ... import models as _models
-from ..._vendor import _convert_request
-from ...operations._solution_self_help_operations import build_get_request
-
+from .. import models as _models
+from .._serialization import Serializer
+from .._vendor import _convert_request
+
+if sys.version_info >= (3, 9):
+    from collections.abc import MutableMapping
+else:
+    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
-ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
+ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
+
+_SERIALIZER = Serializer()
+_SERIALIZER.client_side_validation = False
+
+
+def build_get_request(solution_id: str, **kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-preview"))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop("template_url", "/providers/Microsoft.Help/selfHelp/{solutionId}")
+    path_format_arguments = {
+        "solutionId": _SERIALIZER.url("solution_id", solution_id, "str", max_length=100, min_length=1),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 class SolutionSelfHelpOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.selfhelp.aio.SelfHelpMgmtClient`'s
+        :class:`~azure.mgmt.selfhelp.SelfHelpMgmtClient`'s
         :attr:`solution_self_help` attribute.
     """
 
     models = _models
 
-    def __init__(self, *args, **kwargs) -> None:
+    def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
-    @distributed_trace_async
-    async def get(self, solution_id: str, **kwargs: Any) -> _models.SolutionResourceSelfHelp:
+    @distributed_trace
+    def get(self, solution_id: str, **kwargs: Any) -> _models.SolutionResourceSelfHelp:
         """Gets Self Help Solutions for a given solutionId. Self Help Solutions consist of rich
         instructional video tutorials, links and guides to public documentation related to a specific
         problem that enables users to troubleshoot Azure issues.
 
         :param solution_id: SolutionId is a unique id to identify a solution. You can retrieve the
          solution id using the Discovery api -
          https://learn.microsoft.com/en-us/rest/api/help/discovery-solution/list?view=rest-help-2023-09-01-preview&tabs=HTTP.
          Required.
         :type solution_id: str
         :return: SolutionResourceSelfHelp or the result of cls(response)
         :rtype: ~azure.mgmt.selfhelp.models.SolutionResourceSelfHelp
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -85,15 +117,15 @@
             headers=_headers,
             params=_params,
         )
         _request = _convert_request(_request)
         _request.url = self._client.format_url(_request.url)
 
         _stream = False
-        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
             _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
```

### Comparing `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/operations/_troubleshooters_operations.py` & `azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/aio/operations/_troubleshooters_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
-from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, overload
+import sys
+from typing import Any, Callable, Dict, IO, Optional, Type, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
@@ -30,14 +31,18 @@
     build_continue_method_request,
     build_create_request,
     build_end_request,
     build_get_request,
     build_restart_request,
 )
 
+if sys.version_info >= (3, 9):
+    from collections.abc import MutableMapping
+else:
+    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class TroubleshootersOperations:
     """
     .. warning::
@@ -160,15 +165,15 @@
          is None.
         :type create_troubleshooter_request_body: ~azure.mgmt.selfhelp.models.TroubleshooterResource or
          IO[bytes]
         :return: TroubleshooterResource or the result of cls(response)
         :rtype: ~azure.mgmt.selfhelp.models.TroubleshooterResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -240,15 +245,15 @@
         :type scope: str
         :param troubleshooter_name: Troubleshooter resource Name. Required.
         :type troubleshooter_name: str
         :return: TroubleshooterResource or the result of cls(response)
         :rtype: ~azure.mgmt.selfhelp.models.TroubleshooterResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -374,15 +379,15 @@
          Troubleshooter resource. Is either a ContinueRequestBody type or a IO[bytes] type. Default
          value is None.
         :type continue_request_body: ~azure.mgmt.selfhelp.models.ContinueRequestBody or IO[bytes]
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -447,15 +452,15 @@
         :type scope: str
         :param troubleshooter_name: Troubleshooter resource Name. Required.
         :type troubleshooter_name: str
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -507,15 +512,15 @@
         :type scope: str
         :param troubleshooter_name: Troubleshooter resource Name. Required.
         :type troubleshooter_name: str
         :return: RestartTroubleshooterResponse or the result of cls(response)
         :rtype: ~azure.mgmt.selfhelp.models.RestartTroubleshooterResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
```

### Comparing `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/models/__init__.py` & `azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/models/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/models/_models_py3.py` & `azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/models/_models_py3.py`

 * *Files 0% similar despite different names*

```diff
@@ -418,15 +418,16 @@
 class DiscoveryNlpRequest(_serialization.Model):
     """Discover NLP request.
 
     All required parameters must be populated in order to send to server.
 
     :ivar issue_summary: Natural language description of the issue. Required.
     :vartype issue_summary: str
-    :ivar resource_id: ARM resource Id of the resource that is having the issue.
+    :ivar resource_id: ARM resource Id of the resource that is having the issue. Only applicable
+     for Discovery Solution NLP Subscription Scope.
     :vartype resource_id: str
     :ivar service_id: ARM service Id of the service that is having the issue. For more information
      on service Id see https://learn.microsoft.com/rest/api/support/services/list?tabs=HTTP.
     :vartype service_id: str
     :ivar additional_context: Additional information in the form of a string.
     :vartype additional_context: str
     """
@@ -450,15 +451,16 @@
         service_id: Optional[str] = None,
         additional_context: Optional[str] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword issue_summary: Natural language description of the issue. Required.
         :paramtype issue_summary: str
-        :keyword resource_id: ARM resource Id of the resource that is having the issue.
+        :keyword resource_id: ARM resource Id of the resource that is having the issue. Only applicable
+         for Discovery Solution NLP Subscription Scope.
         :paramtype resource_id: str
         :keyword service_id: ARM service Id of the service that is having the issue. For more
          information on service Id see
          https://learn.microsoft.com/rest/api/support/services/list?tabs=HTTP.
         :paramtype service_id: str
         :keyword additional_context: Additional information in the form of a string.
         :paramtype additional_context: str
```

### Comparing `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/models/_patch.py` & `azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/models/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/models/_self_help_mgmt_client_enums.py` & `azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/models/_self_help_mgmt_client_enums.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/operations/__init__.py` & `azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/operations/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,28 +10,26 @@
 from ._check_name_availability_operations import CheckNameAvailabilityOperations
 from ._diagnostics_operations import DiagnosticsOperations
 from ._discovery_solution_operations import DiscoverySolutionOperations
 from ._solution_operations import SolutionOperations
 from ._simplified_solutions_operations import SimplifiedSolutionsOperations
 from ._troubleshooters_operations import TroubleshootersOperations
 from ._solution_self_help_operations import SolutionSelfHelpOperations
-from ._discovery_solution_nlp_tenant_scope_operations import DiscoverySolutionNLPTenantScopeOperations
-from ._discovery_solution_nlp_subscription_scope_operations import DiscoverySolutionNLPSubscriptionScopeOperations
+from ._discovery_solution_nlp_operations import DiscoverySolutionNLPOperations
 
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "Operations",
     "CheckNameAvailabilityOperations",
     "DiagnosticsOperations",
     "DiscoverySolutionOperations",
     "SolutionOperations",
     "SimplifiedSolutionsOperations",
     "TroubleshootersOperations",
     "SolutionSelfHelpOperations",
-    "DiscoverySolutionNLPTenantScopeOperations",
-    "DiscoverySolutionNLPSubscriptionScopeOperations",
+    "DiscoverySolutionNLPOperations",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 _patch_sdk()
```

### Comparing `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/operations/_check_name_availability_operations.py` & `azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/operations/_check_name_availability_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
-from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, overload
+import sys
+from typing import Any, Callable, Dict, IO, Optional, Type, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
@@ -24,22 +25,26 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request
 
+if sys.version_info >= (3, 9):
+    from collections.abc import MutableMapping
+else:
+    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
-def build_post_request(scope: str, **kwargs: Any) -> HttpRequest:
+def build_check_availability_request(scope: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
@@ -78,15 +83,15 @@
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @overload
-    def post(
+    def check_availability(
         self,
         scope: str,
         check_name_availability_request: Optional[_models.CheckNameAvailabilityRequest] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.CheckNameAvailabilityResponse:
@@ -105,15 +110,15 @@
         :paramtype content_type: str
         :return: CheckNameAvailabilityResponse or the result of cls(response)
         :rtype: ~azure.mgmt.selfhelp.models.CheckNameAvailabilityResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
-    def post(
+    def check_availability(
         self,
         scope: str,
         check_name_availability_request: Optional[IO[bytes]] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.CheckNameAvailabilityResponse:
@@ -132,15 +137,15 @@
         :paramtype content_type: str
         :return: CheckNameAvailabilityResponse or the result of cls(response)
         :rtype: ~azure.mgmt.selfhelp.models.CheckNameAvailabilityResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
-    def post(
+    def check_availability(
         self,
         scope: str,
         check_name_availability_request: Optional[Union[_models.CheckNameAvailabilityRequest, IO[bytes]]] = None,
         **kwargs: Any
     ) -> _models.CheckNameAvailabilityResponse:
         """This API is used to check the uniqueness of a resource name used for a diagnostic,
         troubleshooter or solutions.
@@ -153,15 +158,15 @@
          either a CheckNameAvailabilityRequest type or a IO[bytes] type. Default value is None.
         :type check_name_availability_request: ~azure.mgmt.selfhelp.models.CheckNameAvailabilityRequest
          or IO[bytes]
         :return: CheckNameAvailabilityResponse or the result of cls(response)
         :rtype: ~azure.mgmt.selfhelp.models.CheckNameAvailabilityResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -179,15 +184,15 @@
             _content = check_name_availability_request
         else:
             if check_name_availability_request is not None:
                 _json = self._serialize.body(check_name_availability_request, "CheckNameAvailabilityRequest")
             else:
                 _json = None
 
-        _request = build_post_request(
+        _request = build_check_availability_request(
             scope=scope,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
             headers=_headers,
             params=_params,
```

### Comparing `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/operations/_diagnostics_operations.py` & `azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/operations/_diagnostics_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
-from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
+import sys
+from typing import Any, Callable, Dict, IO, Optional, Type, TypeVar, Union, cast, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
@@ -26,14 +27,18 @@
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.arm_polling import ARMPolling
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request
 
+if sys.version_info >= (3, 9):
+    from collections.abc import MutableMapping
+else:
+    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
@@ -126,15 +131,15 @@
     def _create_initial(
         self,
         scope: str,
         diagnostics_resource_name: str,
         diagnostic_resource_request: Optional[Union[_models.DiagnosticResource, IO[bytes]]] = None,
         **kwargs: Any
     ) -> _models.DiagnosticResource:
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -344,15 +349,15 @@
         :type scope: str
         :param diagnostics_resource_name: Unique resource name for insight resources. Required.
         :type diagnostics_resource_name: str
         :return: DiagnosticResource or the result of cls(response)
         :rtype: ~azure.mgmt.selfhelp.models.DiagnosticResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
```

### Comparing `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/operations/_discovery_solution_nlp_subscription_scope_operations.py` & `azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/operations/_discovery_solution_nlp_operations.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
-from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, overload
+import sys
+from typing import Any, Callable, Dict, IO, Optional, Type, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
@@ -24,33 +25,61 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request
 
+if sys.version_info >= (3, 9):
+    from collections.abc import MutableMapping
+else:
+    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
-def build_post_request(subscription_id: str, **kwargs: Any) -> HttpRequest:
+def build_discover_solutions_request(**kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-preview"))
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop("template_url", "/providers/Microsoft.Help/discoverSolutions")
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
+
+
+def build_discover_solutions_by_subscription_request(  # pylint: disable=name-too-long
+    subscription_id: str, **kwargs: Any
+) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.Help/discoverSolutions")
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", skip_quote=True),
     }
 
     _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -58,92 +87,217 @@
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-class DiscoverySolutionNLPSubscriptionScopeOperations:  # pylint: disable=name-too-long
+class DiscoverySolutionNLPOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.selfhelp.SelfHelpMgmtClient`'s
-        :attr:`discovery_solution_nlp_subscription_scope` attribute.
+        :attr:`discovery_solution_nlp` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @overload
-    def post(
+    def discover_solutions(
         self,
         discover_solution_request: Optional[_models.DiscoveryNlpRequest] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.DiscoveryNlpResponse:
         """Search for relevant Azure Diagnostics, Solutions and Troubleshooters using a natural language
+        issue summary.
+
+        :param discover_solution_request: Request body for discovering solutions using NLP. Default
+         value is None.
+        :type discover_solution_request: ~azure.mgmt.selfhelp.models.DiscoveryNlpRequest
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: DiscoveryNlpResponse or the result of cls(response)
+        :rtype: ~azure.mgmt.selfhelp.models.DiscoveryNlpResponse
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    def discover_solutions(
+        self,
+        discover_solution_request: Optional[IO[bytes]] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> _models.DiscoveryNlpResponse:
+        """Search for relevant Azure Diagnostics, Solutions and Troubleshooters using a natural language
+        issue summary.
+
+        :param discover_solution_request: Request body for discovering solutions using NLP. Default
+         value is None.
+        :type discover_solution_request: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: DiscoveryNlpResponse or the result of cls(response)
+        :rtype: ~azure.mgmt.selfhelp.models.DiscoveryNlpResponse
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace
+    def discover_solutions(
+        self, discover_solution_request: Optional[Union[_models.DiscoveryNlpRequest, IO[bytes]]] = None, **kwargs: Any
+    ) -> _models.DiscoveryNlpResponse:
+        """Search for relevant Azure Diagnostics, Solutions and Troubleshooters using a natural language
+        issue summary.
+
+        :param discover_solution_request: Request body for discovering solutions using NLP. Is either a
+         DiscoveryNlpRequest type or a IO[bytes] type. Default value is None.
+        :type discover_solution_request: ~azure.mgmt.selfhelp.models.DiscoveryNlpRequest or IO[bytes]
+        :return: DiscoveryNlpResponse or the result of cls(response)
+        :rtype: ~azure.mgmt.selfhelp.models.DiscoveryNlpResponse
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.DiscoveryNlpResponse] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(discover_solution_request, (IOBase, bytes)):
+            _content = discover_solution_request
+        else:
+            if discover_solution_request is not None:
+                _json = self._serialize.body(discover_solution_request, "DiscoveryNlpRequest")
+            else:
+                _json = None
+
+        _request = build_discover_solutions_request(
+            api_version=api_version,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
+            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
+
+        deserialized = self._deserialize("DiscoveryNlpResponse", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})  # type: ignore
+
+        return deserialized  # type: ignore
+
+    @overload
+    def discover_solutions_by_subscription(
+        self,
+        subscription_id: str,
+        discover_solution_request: Optional[_models.DiscoveryNlpRequest] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> _models.DiscoveryNlpResponse:
+        """Search for relevant Azure Diagnostics, Solutions and Troubleshooters using a natural language
         issue summary and subscription.
 
+        :param subscription_id: The Azure subscription ID. Required.
+        :type subscription_id: str
         :param discover_solution_request: Request body for discovering solutions using NLP. Default
          value is None.
         :type discover_solution_request: ~azure.mgmt.selfhelp.models.DiscoveryNlpRequest
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :return: DiscoveryNlpResponse or the result of cls(response)
         :rtype: ~azure.mgmt.selfhelp.models.DiscoveryNlpResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
-    def post(
+    def discover_solutions_by_subscription(
         self,
+        subscription_id: str,
         discover_solution_request: Optional[IO[bytes]] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.DiscoveryNlpResponse:
         """Search for relevant Azure Diagnostics, Solutions and Troubleshooters using a natural language
         issue summary and subscription.
 
+        :param subscription_id: The Azure subscription ID. Required.
+        :type subscription_id: str
         :param discover_solution_request: Request body for discovering solutions using NLP. Default
          value is None.
         :type discover_solution_request: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :return: DiscoveryNlpResponse or the result of cls(response)
         :rtype: ~azure.mgmt.selfhelp.models.DiscoveryNlpResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
-    def post(
-        self, discover_solution_request: Optional[Union[_models.DiscoveryNlpRequest, IO[bytes]]] = None, **kwargs: Any
+    def discover_solutions_by_subscription(
+        self,
+        subscription_id: str,
+        discover_solution_request: Optional[Union[_models.DiscoveryNlpRequest, IO[bytes]]] = None,
+        **kwargs: Any
     ) -> _models.DiscoveryNlpResponse:
         """Search for relevant Azure Diagnostics, Solutions and Troubleshooters using a natural language
         issue summary and subscription.
 
+        :param subscription_id: The Azure subscription ID. Required.
+        :type subscription_id: str
         :param discover_solution_request: Request body for discovering solutions using NLP. Is either a
          DiscoveryNlpRequest type or a IO[bytes] type. Default value is None.
         :type discover_solution_request: ~azure.mgmt.selfhelp.models.DiscoveryNlpRequest or IO[bytes]
         :return: DiscoveryNlpResponse or the result of cls(response)
         :rtype: ~azure.mgmt.selfhelp.models.DiscoveryNlpResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -161,16 +315,16 @@
             _content = discover_solution_request
         else:
             if discover_solution_request is not None:
                 _json = self._serialize.body(discover_solution_request, "DiscoveryNlpRequest")
             else:
                 _json = None
 
-        _request = build_post_request(
-            subscription_id=self._config.subscription_id,
+        _request = build_discover_solutions_by_subscription_request(
+            subscription_id=subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
             headers=_headers,
             params=_params,
         )
```

### Comparing `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/operations/_discovery_solution_operations.py` & `azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/operations/_discovery_solution_operations.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-from typing import Any, Callable, Dict, Iterable, Optional, TypeVar
+import sys
+from typing import Any, Callable, Dict, Iterable, Optional, Type, TypeVar
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -25,14 +26,18 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request
 
+if sys.version_info >= (3, 9):
+    from collections.abc import MutableMapping
+else:
+    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
@@ -80,19 +85,19 @@
 
     @distributed_trace
     def list(
         self, filter: Optional[str] = None, skiptoken: Optional[str] = None, **kwargs: Any
     ) -> Iterable["_models.SolutionMetadataResource"]:
         """Lists the relevant Azure Diagnostics, Solutions and Troubleshooters using
         `problemClassification API
-        <https://learn.microsoft.com/rest/api/support/problem-classifications/list?tabs=HTTP>`_\ ) AND
+        <https://learn.microsoft.com/rest/api/support/problem-classifications/list?tabs=HTTP>`_\\ ) AND
         resourceUri or resourceType.:code:`<br/>` Discovery Solutions is the initial entry point within
         Help API, which identifies relevant Azure diagnostics and solutions. :code:`<br/>`:code:`<br/>`
         Required Input :  problemClassificationId (Use the `problemClassification API
-        <https://learn.microsoft.com/rest/api/support/problem-classifications/list?tabs=HTTP>`_\ )
+        <https://learn.microsoft.com/rest/api/support/problem-classifications/list?tabs=HTTP>`_\\ )
         :code:`<br/>`Optional input: resourceUri OR resource Type :code:`<br/>`:code:`<br/>`
         :code:`<b>Note: </b>`  ‘requiredInputs’ from Discovery solutions response must be passed via
         ‘additionalParameters’ as an input to Diagnostics and Solutions API.
 
         :param filter: 'ProblemClassificationId' is a mandatory filter to get solutions ids. It also
          supports optional 'ResourceType' and 'SolutionType' filters. The `$filter
          <https://learn.microsoft.com/en-us/odata/webapi/first-odata-api#filter>`_ supports only 'and',
@@ -109,15 +114,15 @@
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.DiscoveryResponse] = kwargs.pop("cls", None)
 
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
```

### Comparing `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/operations/_patch.py` & `azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/operations/_simplified_solutions_operations.py` & `azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/operations/_simplified_solutions_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
-from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
+import sys
+from typing import Any, Callable, Dict, IO, Optional, Type, TypeVar, Union, cast, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
@@ -26,14 +27,18 @@
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.arm_polling import ARMPolling
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request
 
+if sys.version_info >= (3, 9):
+    from collections.abc import MutableMapping
+else:
+    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
@@ -130,15 +135,15 @@
     def _create_initial(
         self,
         scope: str,
         simplified_solutions_resource_name: str,
         simplified_solutions_request_body: Optional[Union[_models.SimplifiedSolutionsResource, IO[bytes]]] = None,
         **kwargs: Any
     ) -> _models.SimplifiedSolutionsResource:
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -359,15 +364,15 @@
         :type scope: str
         :param simplified_solutions_resource_name: Simplified Solutions Resource Name. Required.
         :type simplified_solutions_resource_name: str
         :return: SimplifiedSolutionsResource or the result of cls(response)
         :rtype: ~azure.mgmt.selfhelp.models.SimplifiedSolutionsResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
```

### Comparing `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/operations/_solution_operations.py` & `azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/operations/_solution_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
-from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
+import sys
+from typing import Any, Callable, Dict, IO, Optional, Type, TypeVar, Union, cast, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
@@ -26,14 +27,18 @@
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.arm_polling import ARMPolling
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request
 
+if sys.version_info >= (3, 9):
+    from collections.abc import MutableMapping
+else:
+    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
@@ -196,15 +201,15 @@
     def _create_initial(
         self,
         scope: str,
         solution_resource_name: str,
         solution_request_body: Optional[Union[_models.SolutionResource, IO[bytes]]] = None,
         **kwargs: Any
     ) -> _models.SolutionResource:
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -428,15 +433,15 @@
         :type scope: str
         :param solution_resource_name: Solution resource Name. Required.
         :type solution_resource_name: str
         :return: SolutionResource or the result of cls(response)
         :rtype: ~azure.mgmt.selfhelp.models.SolutionResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -478,15 +483,15 @@
     def _update_initial(
         self,
         scope: str,
         solution_resource_name: str,
         solution_patch_request_body: Optional[Union[_models.SolutionPatchRequestBody, IO[bytes]]] = None,
         **kwargs: Any
     ) -> _models.SolutionResource:
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -765,15 +770,15 @@
          None.
         :type solution_warm_up_request_body: ~azure.mgmt.selfhelp.models.SolutionWarmUpRequestBody or
          IO[bytes]
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
```

### Comparing `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/operations/_troubleshooters_operations.py` & `azure-mgmt-selfhelp-2.0.0b4/azure/mgmt/selfhelp/operations/_troubleshooters_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
-from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, overload
+import sys
+from typing import Any, Callable, Dict, IO, Optional, Type, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
@@ -24,14 +25,18 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import _convert_request
 
+if sys.version_info >= (3, 9):
+    from collections.abc import MutableMapping
+else:
+    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
@@ -323,15 +328,15 @@
          is None.
         :type create_troubleshooter_request_body: ~azure.mgmt.selfhelp.models.TroubleshooterResource or
          IO[bytes]
         :return: TroubleshooterResource or the result of cls(response)
         :rtype: ~azure.mgmt.selfhelp.models.TroubleshooterResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -403,15 +408,15 @@
         :type scope: str
         :param troubleshooter_name: Troubleshooter resource Name. Required.
         :type troubleshooter_name: str
         :return: TroubleshooterResource or the result of cls(response)
         :rtype: ~azure.mgmt.selfhelp.models.TroubleshooterResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -537,15 +542,15 @@
          Troubleshooter resource. Is either a ContinueRequestBody type or a IO[bytes] type. Default
          value is None.
         :type continue_request_body: ~azure.mgmt.selfhelp.models.ContinueRequestBody or IO[bytes]
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -610,15 +615,15 @@
         :type scope: str
         :param troubleshooter_name: Troubleshooter resource Name. Required.
         :type troubleshooter_name: str
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -668,15 +673,15 @@
         :type scope: str
         :param troubleshooter_name: Troubleshooter resource Name. Required.
         :type troubleshooter_name: str
         :return: RestartTroubleshooterResponse or the result of cls(response)
         :rtype: ~azure.mgmt.selfhelp.models.RestartTroubleshooterResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
```

### Comparing `azure-mgmt-selfhelp-2.0.0b3/azure_mgmt_selfhelp.egg-info/PKG-INFO` & `azure-mgmt-selfhelp-2.0.0b4/azure_mgmt_selfhelp.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-selfhelp
-Version: 2.0.0b3
+Version: 2.0.0b4
 Summary: Microsoft Azure Selfhelp Management Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
 Classifier: Development Status :: 4 - Beta
@@ -82,14 +82,27 @@
 If you encounter any bugs or have suggestions, please file an issue in the
 [Issues](https://github.com/Azure/azure-sdk-for-python/issues)
 section of the project. 
 
 
 # Release History
 
+## 2.0.0b4 (2024-05-27)
+
+### Features Added
+
+  - Added operation CheckNameAvailabilityOperations.check_availability
+  - Added operation group DiscoverySolutionNLPOperations
+
+### Breaking Changes
+
+  - Removed operation CheckNameAvailabilityOperations.post
+  - Removed operation group DiscoverySolutionNLPSubscriptionScopeOperations
+  - Removed operation group DiscoverySolutionNLPTenantScopeOperations
+
 ## 2.0.0b3 (2024-04-22)
 
 ### Features Added
 
   - Added operation SolutionOperations.warm_up
   - Added operation group DiscoverySolutionNLPSubscriptionScopeOperations
   - Added operation group DiscoverySolutionNLPTenantScopeOperations
```

### Comparing `azure-mgmt-selfhelp-2.0.0b3/azure_mgmt_selfhelp.egg-info/SOURCES.txt` & `azure-mgmt-selfhelp-2.0.0b4/azure_mgmt_selfhelp.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -17,32 +17,30 @@
 azure/mgmt/selfhelp/aio/__init__.py
 azure/mgmt/selfhelp/aio/_configuration.py
 azure/mgmt/selfhelp/aio/_patch.py
 azure/mgmt/selfhelp/aio/_self_help_mgmt_client.py
 azure/mgmt/selfhelp/aio/operations/__init__.py
 azure/mgmt/selfhelp/aio/operations/_check_name_availability_operations.py
 azure/mgmt/selfhelp/aio/operations/_diagnostics_operations.py
-azure/mgmt/selfhelp/aio/operations/_discovery_solution_nlp_subscription_scope_operations.py
-azure/mgmt/selfhelp/aio/operations/_discovery_solution_nlp_tenant_scope_operations.py
+azure/mgmt/selfhelp/aio/operations/_discovery_solution_nlp_operations.py
 azure/mgmt/selfhelp/aio/operations/_discovery_solution_operations.py
 azure/mgmt/selfhelp/aio/operations/_operations.py
 azure/mgmt/selfhelp/aio/operations/_patch.py
 azure/mgmt/selfhelp/aio/operations/_simplified_solutions_operations.py
 azure/mgmt/selfhelp/aio/operations/_solution_operations.py
 azure/mgmt/selfhelp/aio/operations/_solution_self_help_operations.py
 azure/mgmt/selfhelp/aio/operations/_troubleshooters_operations.py
 azure/mgmt/selfhelp/models/__init__.py
 azure/mgmt/selfhelp/models/_models_py3.py
 azure/mgmt/selfhelp/models/_patch.py
 azure/mgmt/selfhelp/models/_self_help_mgmt_client_enums.py
 azure/mgmt/selfhelp/operations/__init__.py
 azure/mgmt/selfhelp/operations/_check_name_availability_operations.py
 azure/mgmt/selfhelp/operations/_diagnostics_operations.py
-azure/mgmt/selfhelp/operations/_discovery_solution_nlp_subscription_scope_operations.py
-azure/mgmt/selfhelp/operations/_discovery_solution_nlp_tenant_scope_operations.py
+azure/mgmt/selfhelp/operations/_discovery_solution_nlp_operations.py
 azure/mgmt/selfhelp/operations/_discovery_solution_operations.py
 azure/mgmt/selfhelp/operations/_operations.py
 azure/mgmt/selfhelp/operations/_patch.py
 azure/mgmt/selfhelp/operations/_simplified_solutions_operations.py
 azure/mgmt/selfhelp/operations/_solution_operations.py
 azure/mgmt/selfhelp/operations/_solution_self_help_operations.py
 azure/mgmt/selfhelp/operations/_troubleshooters_operations.py
```

### Comparing `azure-mgmt-selfhelp-2.0.0b3/setup.py` & `azure-mgmt-selfhelp-2.0.0b4/setup.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-selfhelp-2.0.0b3/tests/conftest.py` & `azure-mgmt-selfhelp-2.0.0b4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-selfhelp-2.0.0b3/tests/test_cli_mgmt_selfhelp.py` & `azure-mgmt-selfhelp-2.0.0b4/tests/test_cli_mgmt_selfhelp.py`

 * *Files identical despite different names*

