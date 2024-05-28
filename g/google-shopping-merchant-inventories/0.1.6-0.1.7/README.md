# Comparing `tmp/google-shopping-merchant-inventories-0.1.6.tar.gz` & `tmp/google-shopping-merchant-inventories-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-shopping-merchant-inventories-0.1.6.tar", last modified: Mon Apr 15 13:58:58 2024, max compression
+gzip compressed data, was "google-shopping-merchant-inventories-0.1.7.tar", last modified: Tue May 28 08:24:09 2024, max compression
```

## Comparing `google-shopping-merchant-inventories-0.1.6.tar` & `google-shopping-merchant-inventories-0.1.7.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:58.088363 google-shopping-merchant-inventories-0.1.6/
--rw-rw-r--   0 root         (0)     1003    11358 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     5391 2024-04-15 13:58:58.088363 google-shopping-merchant-inventories-0.1.6/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3926 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:58.076362 google-shopping-merchant-inventories-0.1.6/google/
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:58.076362 google-shopping-merchant-inventories-0.1.6/google/shopping/
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:58.080362 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories/
--rw-rw-r--   0 root         (0)     1003     2291 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       97 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:58.080362 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/
--rw-rw-r--   0 root         (0)     1003     1897 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/__init__.py
--rw-rw-r--   0 root         (0)     1003     3685 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       97 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:58.080362 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/
--rw-rw-r--   0 root         (0)     1003      600 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:58.080362 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/
--rw-rw-r--   0 root         (0)     1003      797 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    25264 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    42185 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/client.py
--rw-rw-r--   0 root         (0)     1003     6203 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:58.080362 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/transports/
--rw-rw-r--   0 root         (0)     1003     1519 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7245 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    15447 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    15726 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    22430 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:58.084363 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/
--rw-rw-r--   0 root         (0)     1003      809 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    25770 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    42812 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/client.py
--rw-rw-r--   0 root         (0)     1003     6375 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:58.084363 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/transports/
--rw-rw-r--   0 root         (0)     1003     1561 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7361 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    15724 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    15997 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    23034 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:58.084363 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/types/
--rw-rw-r--   0 root         (0)     1003     1344 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     9899 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/types/localinventory.py
--rw-rw-r--   0 root         (0)     1003     8279 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/types/regionalinventory.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:58.088363 google-shopping-merchant-inventories-0.1.6/google_shopping_merchant_inventories.egg-info/
--rw-r--r--   0 root         (0)     1003     5391 2024-04-15 13:58:58.000000 google-shopping-merchant-inventories-0.1.6/google_shopping_merchant_inventories.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     3053 2024-04-15 13:58:58.000000 google-shopping-merchant-inventories-0.1.6/google_shopping_merchant_inventories.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2024-04-15 13:58:58.000000 google-shopping-merchant-inventories-0.1.6/google_shopping_merchant_inventories.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003        1 2024-04-15 13:58:58.000000 google-shopping-merchant-inventories-0.1.6/google_shopping_merchant_inventories.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      343 2024-04-15 13:58:58.000000 google-shopping-merchant-inventories-0.1.6/google_shopping_merchant_inventories.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2024-04-15 13:58:58.000000 google-shopping-merchant-inventories-0.1.6/google_shopping_merchant_inventories.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2024-04-15 13:58:58.088363 google-shopping-merchant-inventories-0.1.6/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3281 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:58.088363 google-shopping-merchant-inventories-0.1.6/tests/
--rw-rw-r--   0 root         (0)     1003      600 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:58.088363 google-shopping-merchant-inventories-0.1.6/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:58.088363 google-shopping-merchant-inventories-0.1.6/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:58.088363 google-shopping-merchant-inventories-0.1.6/tests/unit/gapic/merchant_inventories_v1beta/
--rw-rw-r--   0 root         (0)     1003      600 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/tests/unit/gapic/merchant_inventories_v1beta/__init__.py
--rw-rw-r--   0 root         (0)     1003   145402 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/tests/unit/gapic/merchant_inventories_v1beta/test_local_inventory_service.py
--rw-rw-r--   0 root         (0)     1003   146307 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/tests/unit/gapic/merchant_inventories_v1beta/test_regional_inventory_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:09.480640 google-shopping-merchant-inventories-0.1.7/
+-rw-rw-r--   0 root         (0)     1003    11358 2024-05-28 08:20:21.000000 google-shopping-merchant-inventories-0.1.7/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2024-05-28 08:20:21.000000 google-shopping-merchant-inventories-0.1.7/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     5391 2024-05-28 08:24:09.480640 google-shopping-merchant-inventories-0.1.7/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3926 2024-05-28 08:20:21.000000 google-shopping-merchant-inventories-0.1.7/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:09.464637 google-shopping-merchant-inventories-0.1.7/google/
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:09.464637 google-shopping-merchant-inventories-0.1.7/google/shopping/
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:09.468638 google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories/
+-rw-rw-r--   0 root         (0)     1003     2291 2024-05-28 08:20:21.000000 google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2024-05-28 08:20:21.000000 google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       97 2024-05-28 08:20:21.000000 google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:09.468638 google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/
+-rw-rw-r--   0 root         (0)     1003     1897 2024-05-28 08:20:21.000000 google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3685 2024-05-28 08:20:21.000000 google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2024-05-28 08:20:21.000000 google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       97 2024-05-28 08:20:21.000000 google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:09.468638 google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/services/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-28 08:20:21.000000 google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:09.472639 google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/
+-rw-rw-r--   0 root         (0)     1003      797 2024-05-28 08:20:21.000000 google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    26206 2024-05-28 08:20:21.000000 google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    42737 2024-05-28 08:20:21.000000 google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/client.py
+-rw-rw-r--   0 root         (0)     1003     6203 2024-05-28 08:20:21.000000 google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:09.472639 google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1519 2024-05-28 08:20:21.000000 google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7245 2024-05-28 08:20:21.000000 google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    15994 2024-05-28 08:20:21.000000 google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    17142 2024-05-28 08:20:21.000000 google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    22430 2024-05-28 08:20:21.000000 google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:09.472639 google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/
+-rw-rw-r--   0 root         (0)     1003      809 2024-05-28 08:20:21.000000 google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    26739 2024-05-28 08:20:21.000000 google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    43364 2024-05-28 08:20:21.000000 google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/client.py
+-rw-rw-r--   0 root         (0)     1003     6375 2024-05-28 08:20:21.000000 google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:09.476640 google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1561 2024-05-28 08:20:21.000000 google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7361 2024-05-28 08:20:21.000000 google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    16271 2024-05-28 08:20:21.000000 google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    17431 2024-05-28 08:20:21.000000 google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    23034 2024-05-28 08:20:21.000000 google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:09.476640 google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/types/
+-rw-rw-r--   0 root         (0)     1003     1344 2024-05-28 08:20:21.000000 google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9899 2024-05-28 08:20:21.000000 google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/types/localinventory.py
+-rw-rw-r--   0 root         (0)     1003     8279 2024-05-28 08:20:21.000000 google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/types/regionalinventory.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:09.476640 google-shopping-merchant-inventories-0.1.7/google_shopping_merchant_inventories.egg-info/
+-rw-r--r--   0 root         (0)     1003     5391 2024-05-28 08:24:09.000000 google-shopping-merchant-inventories-0.1.7/google_shopping_merchant_inventories.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     3053 2024-05-28 08:24:09.000000 google-shopping-merchant-inventories-0.1.7/google_shopping_merchant_inventories.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-05-28 08:24:09.000000 google-shopping-merchant-inventories-0.1.7/google_shopping_merchant_inventories.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-05-28 08:24:09.000000 google-shopping-merchant-inventories-0.1.7/google_shopping_merchant_inventories.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      343 2024-05-28 08:24:09.000000 google-shopping-merchant-inventories-0.1.7/google_shopping_merchant_inventories.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2024-05-28 08:24:09.000000 google-shopping-merchant-inventories-0.1.7/google_shopping_merchant_inventories.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2024-05-28 08:24:09.480640 google-shopping-merchant-inventories-0.1.7/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3281 2024-05-28 08:20:21.000000 google-shopping-merchant-inventories-0.1.7/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:09.476640 google-shopping-merchant-inventories-0.1.7/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-28 08:20:21.000000 google-shopping-merchant-inventories-0.1.7/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:09.476640 google-shopping-merchant-inventories-0.1.7/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-28 08:20:21.000000 google-shopping-merchant-inventories-0.1.7/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:09.480640 google-shopping-merchant-inventories-0.1.7/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-28 08:20:21.000000 google-shopping-merchant-inventories-0.1.7/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:09.480640 google-shopping-merchant-inventories-0.1.7/tests/unit/gapic/merchant_inventories_v1beta/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-28 08:20:21.000000 google-shopping-merchant-inventories-0.1.7/tests/unit/gapic/merchant_inventories_v1beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003   159559 2024-05-28 08:20:21.000000 google-shopping-merchant-inventories-0.1.7/tests/unit/gapic/merchant_inventories_v1beta/test_local_inventory_service.py
+-rw-rw-r--   0 root         (0)     1003   160626 2024-05-28 08:20:21.000000 google-shopping-merchant-inventories-0.1.7/tests/unit/gapic/merchant_inventories_v1beta/test_regional_inventory_service.py
```

### Comparing `google-shopping-merchant-inventories-0.1.6/LICENSE` & `google-shopping-merchant-inventories-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-inventories-0.1.6/MANIFEST.in` & `google-shopping-merchant-inventories-0.1.7/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-inventories-0.1.6/PKG-INFO` & `google-shopping-merchant-inventories-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-shopping-merchant-inventories
-Version: 0.1.6
+Version: 0.1.7
 Summary: Google Shopping Merchant Inventories API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-shopping-merchant-inventories
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-shopping-merchant-inventories-0.1.6/README.rst` & `google-shopping-merchant-inventories-0.1.7/README.rst`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories/__init__.py` & `google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories/__init__.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories/gapic_version.py` & `google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.6"  # {x-release-please-version}
+__version__ = "0.1.7"  # {x-release-please-version}
```

### Comparing `google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/__init__.py` & `google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/__init__.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/gapic_metadata.json` & `google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/gapic_version.py` & `google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.6"  # {x-release-please-version}
+__version__ = "0.1.7"  # {x-release-please-version}
```

### Comparing `google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/__init__.py` & `google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/__init__.py` & `google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/async_client.py` & `google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/async_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import functools
 import re
 from typing import (
+    Callable,
     Dict,
     Mapping,
     MutableMapping,
     MutableSequence,
     Optional,
     Sequence,
     Tuple,
@@ -202,29 +203,37 @@
         type(LocalInventoryServiceClient),
     )
 
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
-        transport: Union[str, LocalInventoryServiceTransport] = "grpc_asyncio",
+        transport: Optional[
+            Union[
+                str,
+                LocalInventoryServiceTransport,
+                Callable[..., LocalInventoryServiceTransport],
+            ]
+        ] = "grpc_asyncio",
         client_options: Optional[ClientOptions] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the local inventory service async client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
-            transport (Union[str, ~.LocalInventoryServiceTransport]): The
-                transport to use. If set to None, a transport is chosen
-                automatically.
+            transport (Optional[Union[str,LocalInventoryServiceTransport,Callable[..., LocalInventoryServiceTransport]]]):
+                The transport to use, or a Callable that constructs and returns a new transport to use.
+                If a Callable is given, it will be called with the same set of initialization
+                arguments as used in the LocalInventoryServiceTransport constructor.
+                If set to None, a transport is chosen automatically.
             client_options (Optional[Union[google.api_core.client_options.ClientOptions, dict]]):
                 Custom options for the client.
 
                 1. The ``api_endpoint`` property can be used to override the
                 default endpoint provided by the client when ``transport`` is
                 not explicitly provided. Only if this property is not set and
                 ``transport`` was not explicitly provided, the endpoint is
@@ -332,37 +341,38 @@
                 Response message for the ListLocalInventories method.
 
                 Iterating over this object will yield results and
                 resolve additional pages automatically.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = localinventory.ListLocalInventoriesRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, localinventory.ListLocalInventoriesRequest):
+            request = localinventory.ListLocalInventoriesRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if parent is not None:
             request.parent = parent
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.list_local_inventories,
-            default_timeout=None,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.list_local_inventories
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
         )
 
@@ -451,28 +461,29 @@
 
         Returns:
             google.shopping.merchant_inventories_v1beta.types.LocalInventory:
                 Local inventory information for the product. Represents in-store information
                    for a specific product at the store specified by
                    [storeCode][google.shopping.merchant.inventories.v1beta.LocalInventory.store_code].
                    For a list of all accepted attribute values, see the
-                   [local product inventory feed
+                   [local product inventory data
                    specification](\ https://support.google.com/merchants/answer/3061342).
 
         """
         # Create or coerce a protobuf request object.
-        request = localinventory.InsertLocalInventoryRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, localinventory.InsertLocalInventoryRequest):
+            request = localinventory.InsertLocalInventoryRequest(request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.insert_local_inventory,
-            default_timeout=None,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.insert_local_inventory
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
         )
 
@@ -544,37 +555,38 @@
             retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = localinventory.DeleteLocalInventoryRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, localinventory.DeleteLocalInventoryRequest):
+            request = localinventory.DeleteLocalInventoryRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if name is not None:
             request.name = name
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.delete_local_inventory,
-            default_timeout=None,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.delete_local_inventory
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
```

### Comparing `google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/client.py` & `google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import os
 import re
 from typing import (
+    Callable,
     Dict,
     Mapping,
     MutableMapping,
     MutableSequence,
     Optional,
     Sequence,
     Tuple,
@@ -532,29 +533,37 @@
         """
         return self._universe_domain
 
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
-        transport: Optional[Union[str, LocalInventoryServiceTransport]] = None,
+        transport: Optional[
+            Union[
+                str,
+                LocalInventoryServiceTransport,
+                Callable[..., LocalInventoryServiceTransport],
+            ]
+        ] = None,
         client_options: Optional[Union[client_options_lib.ClientOptions, dict]] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the local inventory service client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
-            transport (Union[str, LocalInventoryServiceTransport]): The
-                transport to use. If set to None, a transport is chosen
-                automatically.
+            transport (Optional[Union[str,LocalInventoryServiceTransport,Callable[..., LocalInventoryServiceTransport]]]):
+                The transport to use, or a Callable that constructs and returns a new transport.
+                If a Callable is given, it will be called with the same set of initialization
+                arguments as used in the LocalInventoryServiceTransport constructor.
+                If set to None, a transport is chosen automatically.
             client_options (Optional[Union[google.api_core.client_options.ClientOptions, dict]]):
                 Custom options for the client.
 
                 1. The ``api_endpoint`` property can be used to override the
                 default endpoint provided by the client when ``transport`` is
                 not explicitly provided. Only if this property is not set and
                 ``transport`` was not explicitly provided, the endpoint is
@@ -655,16 +664,24 @@
             if api_key_value and hasattr(
                 google.auth._default, "get_api_key_credentials"
             ):
                 credentials = google.auth._default.get_api_key_credentials(
                     api_key_value
                 )
 
-            Transport = type(self).get_transport_class(cast(str, transport))
-            self._transport = Transport(
+            transport_init: Union[
+                Type[LocalInventoryServiceTransport],
+                Callable[..., LocalInventoryServiceTransport],
+            ] = (
+                type(self).get_transport_class(transport)
+                if isinstance(transport, str) or transport is None
+                else cast(Callable[..., LocalInventoryServiceTransport], transport)
+            )
+            # initialize with the provided callable or the passed in class
+            self._transport = transport_init(
                 credentials=credentials,
                 credentials_file=self._client_options.credentials_file,
                 host=self._api_endpoint,
                 scopes=self._client_options.scopes,
                 client_cert_source_for_mtls=self._client_cert_source,
                 quota_project_id=self._client_options.quota_project_id,
                 client_info=client_info,
@@ -740,27 +757,25 @@
                 Response message for the ListLocalInventories method.
 
                 Iterating over this object will yield results and
                 resolve additional pages automatically.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a localinventory.ListLocalInventoriesRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, localinventory.ListLocalInventoriesRequest):
             request = localinventory.ListLocalInventoriesRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if parent is not None:
                 request.parent = parent
 
@@ -859,23 +874,21 @@
 
         Returns:
             google.shopping.merchant_inventories_v1beta.types.LocalInventory:
                 Local inventory information for the product. Represents in-store information
                    for a specific product at the store specified by
                    [storeCode][google.shopping.merchant.inventories.v1beta.LocalInventory.store_code].
                    For a list of all accepted attribute values, see the
-                   [local product inventory feed
+                   [local product inventory data
                    specification](\ https://support.google.com/merchants/answer/3061342).
 
         """
         # Create or coerce a protobuf request object.
-        # Minor optimization to avoid making a copy if the user passes
-        # in a localinventory.InsertLocalInventoryRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, localinventory.InsertLocalInventoryRequest):
             request = localinventory.InsertLocalInventoryRequest(request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
         rpc = self._transport._wrapped_methods[self._transport.insert_local_inventory]
 
@@ -953,27 +966,25 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a localinventory.DeleteLocalInventoryRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, localinventory.DeleteLocalInventoryRequest):
             request = localinventory.DeleteLocalInventoryRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if name is not None:
                 request.name = name
```

### Comparing `google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/pagers.py` & `google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/transports/__init__.py` & `google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/transports/base.py` & `google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/transports/grpc.py` & `google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/transports/grpc.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     def __init__(
         self,
         *,
         host: str = "merchantapi.googleapis.com",
         credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
-        channel: Optional[grpc.Channel] = None,
+        channel: Optional[Union[grpc.Channel, Callable[..., grpc.Channel]]] = None,
         api_mtls_endpoint: Optional[str] = None,
         client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
         client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
@@ -66,36 +66,39 @@
             host (Optional[str]):
                  The hostname to connect to (default: 'merchantapi.googleapis.com').
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
-                This argument is ignored if ``channel`` is provided.
+                This argument is ignored if a ``channel`` instance is provided.
             credentials_file (Optional[str]): A file with credentials that can
                 be loaded with :func:`google.auth.load_credentials_from_file`.
-                This argument is ignored if ``channel`` is provided.
+                This argument is ignored if a ``channel`` instance is provided.
             scopes (Optional(Sequence[str])): A list of scopes. This argument is
-                ignored if ``channel`` is provided.
-            channel (Optional[grpc.Channel]): A ``Channel`` instance through
-                which to make calls.
+                ignored if a ``channel`` instance is provided.
+            channel (Optional[Union[grpc.Channel, Callable[..., grpc.Channel]]]):
+                A ``Channel`` instance through which to make calls, or a Callable
+                that constructs and returns one. If set to None, ``self.create_channel``
+                is used to create the channel. If a Callable is given, it will be called
+                with the same arguments as used in ``self.create_channel``.
             api_mtls_endpoint (Optional[str]): Deprecated. The mutual TLS endpoint.
                 If provided, it overrides the ``host`` argument and tries to create
                 a mutual TLS channel with client SSL credentials from
                 ``client_cert_source`` or application default SSL credentials.
             client_cert_source (Optional[Callable[[], Tuple[bytes, bytes]]]):
                 Deprecated. A callback to provide client SSL certificate bytes and
                 private key bytes, both in PEM format. It is ignored if
                 ``api_mtls_endpoint`` is None.
             ssl_channel_credentials (grpc.ChannelCredentials): SSL credentials
-                for the grpc channel. It is ignored if ``channel`` is provided.
+                for the grpc channel. It is ignored if a ``channel`` instance is provided.
             client_cert_source_for_mtls (Optional[Callable[[], Tuple[bytes, bytes]]]):
                 A callback to provide client certificate bytes and private key bytes,
                 both in PEM format. It is used to configure a mutual TLS channel. It is
-                ignored if ``channel`` or ``ssl_channel_credentials`` is provided.
+                ignored if a ``channel`` instance or ``ssl_channel_credentials`` is provided.
             quota_project_id (Optional[str]): An optional project to use for billing
                 and quota.
             client_info (google.api_core.gapic_v1.client_info.ClientInfo):
                 The client info used to send a user-agent string along with
                 API requests. If ``None``, then default info will be used.
                 Generally, you only need to set this if you're developing
                 your own client library.
@@ -113,15 +116,15 @@
         self._stubs: Dict[str, Callable] = {}
 
         if api_mtls_endpoint:
             warnings.warn("api_mtls_endpoint is deprecated", DeprecationWarning)
         if client_cert_source:
             warnings.warn("client_cert_source is deprecated", DeprecationWarning)
 
-        if channel:
+        if isinstance(channel, grpc.Channel):
             # Ignore credentials if a channel was passed.
             credentials = False
             # If a channel was explicitly provided, set it.
             self._grpc_channel = channel
             self._ssl_channel_credentials = None
 
         else:
@@ -154,15 +157,17 @@
             quota_project_id=quota_project_id,
             client_info=client_info,
             always_use_jwt_access=always_use_jwt_access,
             api_audience=api_audience,
         )
 
         if not self._grpc_channel:
-            self._grpc_channel = type(self).create_channel(
+            # initialize with the provided callable or the default channel
+            channel_init = channel or type(self).create_channel
+            self._grpc_channel = channel_init(
                 self._host,
                 # use the credentials which are saved
                 credentials=self._credentials,
                 # Set ``credentials_file`` to ``None`` here as
                 # the credentials that we saved earlier should be used.
                 credentials_file=None,
                 scopes=self._scopes,
```

### Comparing `google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/transports/grpc_asyncio.py` & `google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/transports/grpc_asyncio.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from typing import Awaitable, Callable, Dict, Optional, Sequence, Tuple, Union
 import warnings
 
+from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1, grpc_helpers_async
+from google.api_core import retry_async as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 from google.protobuf import empty_pb2  # type: ignore
 import grpc  # type: ignore
 from grpc.experimental import aio  # type: ignore
 
 from google.shopping.merchant_inventories_v1beta.types import localinventory
@@ -61,15 +63,14 @@
             credentials (Optional[~.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify this application to the service. If
                 none are specified, the client will attempt to ascertain
                 the credentials from the environment.
             credentials_file (Optional[str]): A file with credentials that can
                 be loaded with :func:`google.auth.load_credentials_from_file`.
-                This argument is ignored if ``channel`` is provided.
             scopes (Optional[Sequence[str]]): A optional list of scopes needed for this
                 service. These are only used when credentials are not specified and
                 are passed to :func:`google.auth.default`.
             quota_project_id (Optional[str]): An optional project to use for billing
                 and quota.
             kwargs (Optional[dict]): Keyword arguments, which are passed to the
                 channel creation.
@@ -91,15 +92,15 @@
     def __init__(
         self,
         *,
         host: str = "merchantapi.googleapis.com",
         credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
-        channel: Optional[aio.Channel] = None,
+        channel: Optional[Union[aio.Channel, Callable[..., aio.Channel]]] = None,
         api_mtls_endpoint: Optional[str] = None,
         client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
         client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
@@ -111,37 +112,40 @@
             host (Optional[str]):
                  The hostname to connect to (default: 'merchantapi.googleapis.com').
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
-                This argument is ignored if ``channel`` is provided.
+                This argument is ignored if a ``channel`` instance is provided.
             credentials_file (Optional[str]): A file with credentials that can
                 be loaded with :func:`google.auth.load_credentials_from_file`.
-                This argument is ignored if ``channel`` is provided.
+                This argument is ignored if a ``channel`` instance is provided.
             scopes (Optional[Sequence[str]]): A optional list of scopes needed for this
                 service. These are only used when credentials are not specified and
                 are passed to :func:`google.auth.default`.
-            channel (Optional[aio.Channel]): A ``Channel`` instance through
-                which to make calls.
+            channel (Optional[Union[aio.Channel, Callable[..., aio.Channel]]]):
+                A ``Channel`` instance through which to make calls, or a Callable
+                that constructs and returns one. If set to None, ``self.create_channel``
+                is used to create the channel. If a Callable is given, it will be called
+                with the same arguments as used in ``self.create_channel``.
             api_mtls_endpoint (Optional[str]): Deprecated. The mutual TLS endpoint.
                 If provided, it overrides the ``host`` argument and tries to create
                 a mutual TLS channel with client SSL credentials from
                 ``client_cert_source`` or application default SSL credentials.
             client_cert_source (Optional[Callable[[], Tuple[bytes, bytes]]]):
                 Deprecated. A callback to provide client SSL certificate bytes and
                 private key bytes, both in PEM format. It is ignored if
                 ``api_mtls_endpoint`` is None.
             ssl_channel_credentials (grpc.ChannelCredentials): SSL credentials
-                for the grpc channel. It is ignored if ``channel`` is provided.
+                for the grpc channel. It is ignored if a ``channel`` instance is provided.
             client_cert_source_for_mtls (Optional[Callable[[], Tuple[bytes, bytes]]]):
                 A callback to provide client certificate bytes and private key bytes,
                 both in PEM format. It is used to configure a mutual TLS channel. It is
-                ignored if ``channel`` or ``ssl_channel_credentials`` is provided.
+                ignored if a ``channel`` instance or ``ssl_channel_credentials`` is provided.
             quota_project_id (Optional[str]): An optional project to use for billing
                 and quota.
             client_info (google.api_core.gapic_v1.client_info.ClientInfo):
                 The client info used to send a user-agent string along with
                 API requests. If ``None``, then default info will be used.
                 Generally, you only need to set this if you're developing
                 your own client library.
@@ -159,15 +163,15 @@
         self._stubs: Dict[str, Callable] = {}
 
         if api_mtls_endpoint:
             warnings.warn("api_mtls_endpoint is deprecated", DeprecationWarning)
         if client_cert_source:
             warnings.warn("client_cert_source is deprecated", DeprecationWarning)
 
-        if channel:
+        if isinstance(channel, aio.Channel):
             # Ignore credentials if a channel was passed.
             credentials = False
             # If a channel was explicitly provided, set it.
             self._grpc_channel = channel
             self._ssl_channel_credentials = None
         else:
             if api_mtls_endpoint:
@@ -199,15 +203,17 @@
             quota_project_id=quota_project_id,
             client_info=client_info,
             always_use_jwt_access=always_use_jwt_access,
             api_audience=api_audience,
         )
 
         if not self._grpc_channel:
-            self._grpc_channel = type(self).create_channel(
+            # initialize with the provided callable or the default channel
+            channel_init = channel or type(self).create_channel
+            self._grpc_channel = channel_init(
                 self._host,
                 # use the credentials which are saved
                 credentials=self._credentials,
                 # Set ``credentials_file`` to ``None`` here as
                 # the credentials that we saved earlier should be used.
                 credentials_file=None,
                 scopes=self._scopes,
@@ -333,12 +339,32 @@
             self._stubs["delete_local_inventory"] = self.grpc_channel.unary_unary(
                 "/google.shopping.merchant.inventories.v1beta.LocalInventoryService/DeleteLocalInventory",
                 request_serializer=localinventory.DeleteLocalInventoryRequest.serialize,
                 response_deserializer=empty_pb2.Empty.FromString,
             )
         return self._stubs["delete_local_inventory"]
 
+    def _prep_wrapped_messages(self, client_info):
+        """Precompute the wrapped methods, overriding the base class method to use async wrappers."""
+        self._wrapped_methods = {
+            self.list_local_inventories: gapic_v1.method_async.wrap_method(
+                self.list_local_inventories,
+                default_timeout=None,
+                client_info=client_info,
+            ),
+            self.insert_local_inventory: gapic_v1.method_async.wrap_method(
+                self.insert_local_inventory,
+                default_timeout=None,
+                client_info=client_info,
+            ),
+            self.delete_local_inventory: gapic_v1.method_async.wrap_method(
+                self.delete_local_inventory,
+                default_timeout=None,
+                client_info=client_info,
+            ),
+        }
+
     def close(self):
         return self.grpc_channel.close()
 
 
 __all__ = ("LocalInventoryServiceGrpcAsyncIOTransport",)
```

### Comparing `google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/transports/rest.py` & `google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -357,15 +357,15 @@
             Returns:
                 ~.localinventory.LocalInventory:
                     Local inventory information for the product. Represents
                 in-store information for a specific product at the store
                 specified by
                 [``storeCode``][google.shopping.merchant.inventories.v1beta.LocalInventory.store_code].
                 For a list of all accepted attribute values, see the
-                `local product inventory feed
+                `local product inventory data
                 specification <https://support.google.com/merchants/answer/3061342>`__.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "post",
```

### Comparing `google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/__init__.py` & `google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/async_client.py` & `google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/async_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import functools
 import re
 from typing import (
+    Callable,
     Dict,
     Mapping,
     MutableMapping,
     MutableSequence,
     Optional,
     Sequence,
     Tuple,
@@ -208,29 +209,37 @@
         type(RegionalInventoryServiceClient),
     )
 
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
-        transport: Union[str, RegionalInventoryServiceTransport] = "grpc_asyncio",
+        transport: Optional[
+            Union[
+                str,
+                RegionalInventoryServiceTransport,
+                Callable[..., RegionalInventoryServiceTransport],
+            ]
+        ] = "grpc_asyncio",
         client_options: Optional[ClientOptions] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the regional inventory service async client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
-            transport (Union[str, ~.RegionalInventoryServiceTransport]): The
-                transport to use. If set to None, a transport is chosen
-                automatically.
+            transport (Optional[Union[str,RegionalInventoryServiceTransport,Callable[..., RegionalInventoryServiceTransport]]]):
+                The transport to use, or a Callable that constructs and returns a new transport to use.
+                If a Callable is given, it will be called with the same set of initialization
+                arguments as used in the RegionalInventoryServiceTransport constructor.
+                If set to None, a transport is chosen automatically.
             client_options (Optional[Union[google.api_core.client_options.ClientOptions, dict]]):
                 Custom options for the client.
 
                 1. The ``api_endpoint`` property can be used to override the
                 default endpoint provided by the client when ``transport`` is
                 not explicitly provided. Only if this property is not set and
                 ``transport`` was not explicitly provided, the endpoint is
@@ -339,37 +348,38 @@
                 Response message for the ListRegionalInventories method.
 
                 Iterating over this object will yield results and
                 resolve additional pages automatically.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = regionalinventory.ListRegionalInventoriesRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, regionalinventory.ListRegionalInventoriesRequest):
+            request = regionalinventory.ListRegionalInventoriesRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if parent is not None:
             request.parent = parent
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.list_regional_inventories,
-            default_timeout=None,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.list_regional_inventories
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
         )
 
@@ -460,28 +470,29 @@
         Returns:
             google.shopping.merchant_inventories_v1beta.types.RegionalInventory:
                 Regional inventory information for the product. Represents specific
                    information like price and availability for a given
                    product in a specific
                    [region][google.shopping.merchant.inventories.v1beta.RegionalInventory.region].
                    For a list of all accepted attribute values, see the
-                   [regional product inventory feed
+                   [regional product inventory data
                    specification](\ https://support.google.com/merchants/answer/9698880).
 
         """
         # Create or coerce a protobuf request object.
-        request = regionalinventory.InsertRegionalInventoryRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, regionalinventory.InsertRegionalInventoryRequest):
+            request = regionalinventory.InsertRegionalInventoryRequest(request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.insert_regional_inventory,
-            default_timeout=None,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.insert_regional_inventory
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
         )
 
@@ -554,37 +565,38 @@
             retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = regionalinventory.DeleteRegionalInventoryRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, regionalinventory.DeleteRegionalInventoryRequest):
+            request = regionalinventory.DeleteRegionalInventoryRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if name is not None:
             request.name = name
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.delete_regional_inventory,
-            default_timeout=None,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.delete_regional_inventory
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
```

### Comparing `google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/client.py` & `google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import os
 import re
 from typing import (
+    Callable,
     Dict,
     Mapping,
     MutableMapping,
     MutableSequence,
     Optional,
     Sequence,
     Tuple,
@@ -536,29 +537,37 @@
         """
         return self._universe_domain
 
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
-        transport: Optional[Union[str, RegionalInventoryServiceTransport]] = None,
+        transport: Optional[
+            Union[
+                str,
+                RegionalInventoryServiceTransport,
+                Callable[..., RegionalInventoryServiceTransport],
+            ]
+        ] = None,
         client_options: Optional[Union[client_options_lib.ClientOptions, dict]] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the regional inventory service client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
-            transport (Union[str, RegionalInventoryServiceTransport]): The
-                transport to use. If set to None, a transport is chosen
-                automatically.
+            transport (Optional[Union[str,RegionalInventoryServiceTransport,Callable[..., RegionalInventoryServiceTransport]]]):
+                The transport to use, or a Callable that constructs and returns a new transport.
+                If a Callable is given, it will be called with the same set of initialization
+                arguments as used in the RegionalInventoryServiceTransport constructor.
+                If set to None, a transport is chosen automatically.
             client_options (Optional[Union[google.api_core.client_options.ClientOptions, dict]]):
                 Custom options for the client.
 
                 1. The ``api_endpoint`` property can be used to override the
                 default endpoint provided by the client when ``transport`` is
                 not explicitly provided. Only if this property is not set and
                 ``transport`` was not explicitly provided, the endpoint is
@@ -661,16 +670,24 @@
             if api_key_value and hasattr(
                 google.auth._default, "get_api_key_credentials"
             ):
                 credentials = google.auth._default.get_api_key_credentials(
                     api_key_value
                 )
 
-            Transport = type(self).get_transport_class(cast(str, transport))
-            self._transport = Transport(
+            transport_init: Union[
+                Type[RegionalInventoryServiceTransport],
+                Callable[..., RegionalInventoryServiceTransport],
+            ] = (
+                type(self).get_transport_class(transport)
+                if isinstance(transport, str) or transport is None
+                else cast(Callable[..., RegionalInventoryServiceTransport], transport)
+            )
+            # initialize with the provided callable or the passed in class
+            self._transport = transport_init(
                 credentials=credentials,
                 credentials_file=self._client_options.credentials_file,
                 host=self._api_endpoint,
                 scopes=self._client_options.scopes,
                 client_cert_source_for_mtls=self._client_cert_source,
                 quota_project_id=self._client_options.quota_project_id,
                 client_info=client_info,
@@ -747,27 +764,25 @@
                 Response message for the ListRegionalInventories method.
 
                 Iterating over this object will yield results and
                 resolve additional pages automatically.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a regionalinventory.ListRegionalInventoriesRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, regionalinventory.ListRegionalInventoriesRequest):
             request = regionalinventory.ListRegionalInventoriesRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if parent is not None:
                 request.parent = parent
 
@@ -870,23 +885,21 @@
         Returns:
             google.shopping.merchant_inventories_v1beta.types.RegionalInventory:
                 Regional inventory information for the product. Represents specific
                    information like price and availability for a given
                    product in a specific
                    [region][google.shopping.merchant.inventories.v1beta.RegionalInventory.region].
                    For a list of all accepted attribute values, see the
-                   [regional product inventory feed
+                   [regional product inventory data
                    specification](\ https://support.google.com/merchants/answer/9698880).
 
         """
         # Create or coerce a protobuf request object.
-        # Minor optimization to avoid making a copy if the user passes
-        # in a regionalinventory.InsertRegionalInventoryRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, regionalinventory.InsertRegionalInventoryRequest):
             request = regionalinventory.InsertRegionalInventoryRequest(request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
         rpc = self._transport._wrapped_methods[
             self._transport.insert_regional_inventory
@@ -967,27 +980,25 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a regionalinventory.DeleteRegionalInventoryRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, regionalinventory.DeleteRegionalInventoryRequest):
             request = regionalinventory.DeleteRegionalInventoryRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if name is not None:
                 request.name = name
```

### Comparing `google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/pagers.py` & `google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/transports/__init__.py` & `google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/transports/base.py` & `google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/transports/grpc.py` & `google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/transports/grpc.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     def __init__(
         self,
         *,
         host: str = "merchantapi.googleapis.com",
         credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
-        channel: Optional[grpc.Channel] = None,
+        channel: Optional[Union[grpc.Channel, Callable[..., grpc.Channel]]] = None,
         api_mtls_endpoint: Optional[str] = None,
         client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
         client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
@@ -67,36 +67,39 @@
             host (Optional[str]):
                  The hostname to connect to (default: 'merchantapi.googleapis.com').
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
-                This argument is ignored if ``channel`` is provided.
+                This argument is ignored if a ``channel`` instance is provided.
             credentials_file (Optional[str]): A file with credentials that can
                 be loaded with :func:`google.auth.load_credentials_from_file`.
-                This argument is ignored if ``channel`` is provided.
+                This argument is ignored if a ``channel`` instance is provided.
             scopes (Optional(Sequence[str])): A list of scopes. This argument is
-                ignored if ``channel`` is provided.
-            channel (Optional[grpc.Channel]): A ``Channel`` instance through
-                which to make calls.
+                ignored if a ``channel`` instance is provided.
+            channel (Optional[Union[grpc.Channel, Callable[..., grpc.Channel]]]):
+                A ``Channel`` instance through which to make calls, or a Callable
+                that constructs and returns one. If set to None, ``self.create_channel``
+                is used to create the channel. If a Callable is given, it will be called
+                with the same arguments as used in ``self.create_channel``.
             api_mtls_endpoint (Optional[str]): Deprecated. The mutual TLS endpoint.
                 If provided, it overrides the ``host`` argument and tries to create
                 a mutual TLS channel with client SSL credentials from
                 ``client_cert_source`` or application default SSL credentials.
             client_cert_source (Optional[Callable[[], Tuple[bytes, bytes]]]):
                 Deprecated. A callback to provide client SSL certificate bytes and
                 private key bytes, both in PEM format. It is ignored if
                 ``api_mtls_endpoint`` is None.
             ssl_channel_credentials (grpc.ChannelCredentials): SSL credentials
-                for the grpc channel. It is ignored if ``channel`` is provided.
+                for the grpc channel. It is ignored if a ``channel`` instance is provided.
             client_cert_source_for_mtls (Optional[Callable[[], Tuple[bytes, bytes]]]):
                 A callback to provide client certificate bytes and private key bytes,
                 both in PEM format. It is used to configure a mutual TLS channel. It is
-                ignored if ``channel`` or ``ssl_channel_credentials`` is provided.
+                ignored if a ``channel`` instance or ``ssl_channel_credentials`` is provided.
             quota_project_id (Optional[str]): An optional project to use for billing
                 and quota.
             client_info (google.api_core.gapic_v1.client_info.ClientInfo):
                 The client info used to send a user-agent string along with
                 API requests. If ``None``, then default info will be used.
                 Generally, you only need to set this if you're developing
                 your own client library.
@@ -114,15 +117,15 @@
         self._stubs: Dict[str, Callable] = {}
 
         if api_mtls_endpoint:
             warnings.warn("api_mtls_endpoint is deprecated", DeprecationWarning)
         if client_cert_source:
             warnings.warn("client_cert_source is deprecated", DeprecationWarning)
 
-        if channel:
+        if isinstance(channel, grpc.Channel):
             # Ignore credentials if a channel was passed.
             credentials = False
             # If a channel was explicitly provided, set it.
             self._grpc_channel = channel
             self._ssl_channel_credentials = None
 
         else:
@@ -155,15 +158,17 @@
             quota_project_id=quota_project_id,
             client_info=client_info,
             always_use_jwt_access=always_use_jwt_access,
             api_audience=api_audience,
         )
 
         if not self._grpc_channel:
-            self._grpc_channel = type(self).create_channel(
+            # initialize with the provided callable or the default channel
+            channel_init = channel or type(self).create_channel
+            self._grpc_channel = channel_init(
                 self._host,
                 # use the credentials which are saved
                 credentials=self._credentials,
                 # Set ``credentials_file`` to ``None`` here as
                 # the credentials that we saved earlier should be used.
                 credentials_file=None,
                 scopes=self._scopes,
```

### Comparing `google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/transports/grpc_asyncio.py` & `google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/transports/grpc_asyncio.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from typing import Awaitable, Callable, Dict, Optional, Sequence, Tuple, Union
 import warnings
 
+from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1, grpc_helpers_async
+from google.api_core import retry_async as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 from google.protobuf import empty_pb2  # type: ignore
 import grpc  # type: ignore
 from grpc.experimental import aio  # type: ignore
 
 from google.shopping.merchant_inventories_v1beta.types import regionalinventory
@@ -62,15 +64,14 @@
             credentials (Optional[~.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify this application to the service. If
                 none are specified, the client will attempt to ascertain
                 the credentials from the environment.
             credentials_file (Optional[str]): A file with credentials that can
                 be loaded with :func:`google.auth.load_credentials_from_file`.
-                This argument is ignored if ``channel`` is provided.
             scopes (Optional[Sequence[str]]): A optional list of scopes needed for this
                 service. These are only used when credentials are not specified and
                 are passed to :func:`google.auth.default`.
             quota_project_id (Optional[str]): An optional project to use for billing
                 and quota.
             kwargs (Optional[dict]): Keyword arguments, which are passed to the
                 channel creation.
@@ -92,15 +93,15 @@
     def __init__(
         self,
         *,
         host: str = "merchantapi.googleapis.com",
         credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
-        channel: Optional[aio.Channel] = None,
+        channel: Optional[Union[aio.Channel, Callable[..., aio.Channel]]] = None,
         api_mtls_endpoint: Optional[str] = None,
         client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
         client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
@@ -112,37 +113,40 @@
             host (Optional[str]):
                  The hostname to connect to (default: 'merchantapi.googleapis.com').
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
-                This argument is ignored if ``channel`` is provided.
+                This argument is ignored if a ``channel`` instance is provided.
             credentials_file (Optional[str]): A file with credentials that can
                 be loaded with :func:`google.auth.load_credentials_from_file`.
-                This argument is ignored if ``channel`` is provided.
+                This argument is ignored if a ``channel`` instance is provided.
             scopes (Optional[Sequence[str]]): A optional list of scopes needed for this
                 service. These are only used when credentials are not specified and
                 are passed to :func:`google.auth.default`.
-            channel (Optional[aio.Channel]): A ``Channel`` instance through
-                which to make calls.
+            channel (Optional[Union[aio.Channel, Callable[..., aio.Channel]]]):
+                A ``Channel`` instance through which to make calls, or a Callable
+                that constructs and returns one. If set to None, ``self.create_channel``
+                is used to create the channel. If a Callable is given, it will be called
+                with the same arguments as used in ``self.create_channel``.
             api_mtls_endpoint (Optional[str]): Deprecated. The mutual TLS endpoint.
                 If provided, it overrides the ``host`` argument and tries to create
                 a mutual TLS channel with client SSL credentials from
                 ``client_cert_source`` or application default SSL credentials.
             client_cert_source (Optional[Callable[[], Tuple[bytes, bytes]]]):
                 Deprecated. A callback to provide client SSL certificate bytes and
                 private key bytes, both in PEM format. It is ignored if
                 ``api_mtls_endpoint`` is None.
             ssl_channel_credentials (grpc.ChannelCredentials): SSL credentials
-                for the grpc channel. It is ignored if ``channel`` is provided.
+                for the grpc channel. It is ignored if a ``channel`` instance is provided.
             client_cert_source_for_mtls (Optional[Callable[[], Tuple[bytes, bytes]]]):
                 A callback to provide client certificate bytes and private key bytes,
                 both in PEM format. It is used to configure a mutual TLS channel. It is
-                ignored if ``channel`` or ``ssl_channel_credentials`` is provided.
+                ignored if a ``channel`` instance or ``ssl_channel_credentials`` is provided.
             quota_project_id (Optional[str]): An optional project to use for billing
                 and quota.
             client_info (google.api_core.gapic_v1.client_info.ClientInfo):
                 The client info used to send a user-agent string along with
                 API requests. If ``None``, then default info will be used.
                 Generally, you only need to set this if you're developing
                 your own client library.
@@ -160,15 +164,15 @@
         self._stubs: Dict[str, Callable] = {}
 
         if api_mtls_endpoint:
             warnings.warn("api_mtls_endpoint is deprecated", DeprecationWarning)
         if client_cert_source:
             warnings.warn("client_cert_source is deprecated", DeprecationWarning)
 
-        if channel:
+        if isinstance(channel, aio.Channel):
             # Ignore credentials if a channel was passed.
             credentials = False
             # If a channel was explicitly provided, set it.
             self._grpc_channel = channel
             self._ssl_channel_credentials = None
         else:
             if api_mtls_endpoint:
@@ -200,15 +204,17 @@
             quota_project_id=quota_project_id,
             client_info=client_info,
             always_use_jwt_access=always_use_jwt_access,
             api_audience=api_audience,
         )
 
         if not self._grpc_channel:
-            self._grpc_channel = type(self).create_channel(
+            # initialize with the provided callable or the default channel
+            channel_init = channel or type(self).create_channel
+            self._grpc_channel = channel_init(
                 self._host,
                 # use the credentials which are saved
                 credentials=self._credentials,
                 # Set ``credentials_file`` to ``None`` here as
                 # the credentials that we saved earlier should be used.
                 credentials_file=None,
                 scopes=self._scopes,
@@ -334,12 +340,32 @@
             self._stubs["delete_regional_inventory"] = self.grpc_channel.unary_unary(
                 "/google.shopping.merchant.inventories.v1beta.RegionalInventoryService/DeleteRegionalInventory",
                 request_serializer=regionalinventory.DeleteRegionalInventoryRequest.serialize,
                 response_deserializer=empty_pb2.Empty.FromString,
             )
         return self._stubs["delete_regional_inventory"]
 
+    def _prep_wrapped_messages(self, client_info):
+        """Precompute the wrapped methods, overriding the base class method to use async wrappers."""
+        self._wrapped_methods = {
+            self.list_regional_inventories: gapic_v1.method_async.wrap_method(
+                self.list_regional_inventories,
+                default_timeout=None,
+                client_info=client_info,
+            ),
+            self.insert_regional_inventory: gapic_v1.method_async.wrap_method(
+                self.insert_regional_inventory,
+                default_timeout=None,
+                client_info=client_info,
+            ),
+            self.delete_regional_inventory: gapic_v1.method_async.wrap_method(
+                self.delete_regional_inventory,
+                default_timeout=None,
+                client_info=client_info,
+            ),
+        }
+
     def close(self):
         return self.grpc_channel.close()
 
 
 __all__ = ("RegionalInventoryServiceGrpcAsyncIOTransport",)
```

### Comparing `google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/transports/rest.py` & `google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -366,15 +366,15 @@
             Returns:
                 ~.regionalinventory.RegionalInventory:
                     Regional inventory information for the product.
                 Represents specific information like price and
                 availability for a given product in a specific
                 [``region``][google.shopping.merchant.inventories.v1beta.RegionalInventory.region].
                 For a list of all accepted attribute values, see the
-                `regional product inventory feed
+                `regional product inventory data
                 specification <https://support.google.com/merchants/answer/9698880>`__.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "post",
```

### Comparing `google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/types/__init__.py` & `google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/types/localinventory.py` & `google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/types/localinventory.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 
 class LocalInventory(proto.Message):
     r"""Local inventory information for the product. Represents in-store
     information for a specific product at the store specified by
     [``storeCode``][google.shopping.merchant.inventories.v1beta.LocalInventory.store_code].
     For a list of all accepted attribute values, see the `local product
-    inventory feed
+    inventory data
     specification <https://support.google.com/merchants/answer/3061342>`__.
 
 
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
     Attributes:
         name (str):
@@ -52,61 +52,61 @@
         account (int):
             Output only. The account that owns the
             product. This field will be ignored if set by
             the client.
         store_code (str):
             Required. Immutable. Store code (the store ID from your
             Business Profile) of the physical store the product is sold
-            in. See the `Local product inventory feed
+            in. See the `Local product inventory data
             specification <https://support.google.com/merchants/answer/3061342>`__
             for more information.
         price (google.shopping.type.types.Price):
             Price of the product at this store.
         sale_price (google.shopping.type.types.Price):
             Sale price of the product at this store. Mandatory if
             [``salePriceEffectiveDate``][google.shopping.merchant.inventories.v1beta.LocalInventory.sale_price_effective_date]
             is defined.
         sale_price_effective_date (google.type.interval_pb2.Interval):
             The ``TimePeriod`` of the sale at this store.
         availability (str):
             Availability of the product at this store. For accepted
-            attribute values, see the `local product inventory feed
+            attribute values, see the `local product inventory data
             specification <https://support.google.com/merchants/answer/3061342>`__
 
             This field is a member of `oneof`_ ``_availability``.
         quantity (int):
             Quantity of the product available at this
             store. Must be greater than or equal to zero.
 
             This field is a member of `oneof`_ ``_quantity``.
         pickup_method (str):
             Supported pickup method for this product. Unless the value
             is ``"not supported"``, this field must be submitted
             together with ``pickupSla``. For accepted attribute values,
-            see the `local product inventory feed
+            see the `local product inventory data
             specification <https://support.google.com/merchants/answer/3061342>`__
 
             This field is a member of `oneof`_ ``_pickup_method``.
         pickup_sla (str):
             Relative time period from the order date for an order for
             this product, from this store, to be ready for pickup. Must
             be submitted with ``pickupMethod``. For accepted attribute
-            values, see the `local product inventory feed
+            values, see the `local product inventory data
             specification <https://support.google.com/merchants/answer/3061342>`__
 
             This field is a member of `oneof`_ ``_pickup_sla``.
         instore_product_location (str):
             Location of the product inside the store.
             Maximum length is 20 bytes.
 
             This field is a member of `oneof`_ ``_instore_product_location``.
         custom_attributes (MutableSequence[google.shopping.type.types.CustomAttribute]):
             A list of custom (merchant-provided) attributes. You can
             also use ``CustomAttribute`` to submit any attribute of the
-            feed specification in its generic form.
+            data specification in its generic form.
     """
 
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
     account: int = proto.Field(
```

### Comparing `google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/types/regionalinventory.py` & `google-shopping-merchant-inventories-0.1.7/google/shopping/merchant_inventories_v1beta/types/regionalinventory.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 class RegionalInventory(proto.Message):
     r"""Regional inventory information for the product. Represents specific
     information like price and availability for a given product in a
     specific
     [``region``][google.shopping.merchant.inventories.v1beta.RegionalInventory.region].
     For a list of all accepted attribute values, see the `regional
-    product inventory feed
+    product inventory data
     specification <https://support.google.com/merchants/answer/9698880>`__.
 
 
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
     Attributes:
         name (str):
@@ -66,22 +66,22 @@
             Sale price of the product in this region. Mandatory if
             [``salePriceEffectiveDate``][google.shopping.merchant.inventories.v1beta.RegionalInventory.sale_price_effective_date]
             is defined.
         sale_price_effective_date (google.type.interval_pb2.Interval):
             The ``TimePeriod`` of the sale price in this region.
         availability (str):
             Availability of the product in this region. For accepted
-            attribute values, see the `regional product inventory feed
+            attribute values, see the `regional product inventory data
             specification <https://support.google.com/merchants/answer/3061342>`__
 
             This field is a member of `oneof`_ ``_availability``.
         custom_attributes (MutableSequence[google.shopping.type.types.CustomAttribute]):
             A list of custom (merchant-provided) attributes. You can
             also use ``CustomAttribute`` to submit any attribute of the
-            feed specification in its generic form.
+            data specification in its generic form.
     """
 
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
     account: int = proto.Field(
```

### Comparing `google-shopping-merchant-inventories-0.1.6/google_shopping_merchant_inventories.egg-info/PKG-INFO` & `google-shopping-merchant-inventories-0.1.7/google_shopping_merchant_inventories.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-shopping-merchant-inventories
-Version: 0.1.6
+Version: 0.1.7
 Summary: Google Shopping Merchant Inventories API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-shopping-merchant-inventories
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-shopping-merchant-inventories-0.1.6/google_shopping_merchant_inventories.egg-info/SOURCES.txt` & `google-shopping-merchant-inventories-0.1.7/google_shopping_merchant_inventories.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-inventories-0.1.6/setup.py` & `google-shopping-merchant-inventories-0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-inventories-0.1.6/tests/__init__.py` & `google-shopping-merchant-inventories-0.1.7/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-inventories-0.1.6/tests/unit/__init__.py` & `google-shopping-merchant-inventories-0.1.7/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-inventories-0.1.6/tests/unit/gapic/__init__.py` & `google-shopping-merchant-inventories-0.1.7/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-inventories-0.1.6/tests/unit/gapic/merchant_inventories_v1beta/__init__.py` & `google-shopping-merchant-inventories-0.1.7/tests/unit/gapic/merchant_inventories_v1beta/__init__.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-inventories-0.1.6/tests/unit/gapic/merchant_inventories_v1beta/test_local_inventory_service.py` & `google-shopping-merchant-inventories-0.1.7/tests/unit/gapic/merchant_inventories_v1beta/test_local_inventory_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -1235,14 +1235,17 @@
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_local_inventories), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.list_local_inventories()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == localinventory.ListLocalInventoriesRequest()
 
 
 def test_list_local_inventories_non_empty_request_with_auto_populated_field():
@@ -1261,23 +1264,66 @@
         page_token="page_token_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_local_inventories), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.list_local_inventories(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == localinventory.ListLocalInventoriesRequest(
             parent="parent_value",
             page_token="page_token_value",
         )
 
 
+def test_list_local_inventories_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = LocalInventoryServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.list_local_inventories
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.list_local_inventories
+        ] = mock_rpc
+        request = {}
+        client.list_local_inventories(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.list_local_inventories(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_list_local_inventories_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = LocalInventoryServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -1296,14 +1342,60 @@
         response = await client.list_local_inventories()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == localinventory.ListLocalInventoriesRequest()
 
 
 @pytest.mark.asyncio
+async def test_list_local_inventories_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = LocalInventoryServiceAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.list_local_inventories
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.list_local_inventories
+        ] = mock_object
+
+        request = {}
+        await client.list_local_inventories(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.list_local_inventories(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_list_local_inventories_async(
     transport: str = "grpc_asyncio",
     request_type=localinventory.ListLocalInventoriesRequest,
 ):
     client = LocalInventoryServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -1750,14 +1842,17 @@
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.insert_local_inventory), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.insert_local_inventory()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == localinventory.InsertLocalInventoryRequest()
 
 
 def test_insert_local_inventory_non_empty_request_with_auto_populated_field():
@@ -1775,22 +1870,65 @@
         parent="parent_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.insert_local_inventory), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.insert_local_inventory(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == localinventory.InsertLocalInventoryRequest(
             parent="parent_value",
         )
 
 
+def test_insert_local_inventory_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = LocalInventoryServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.insert_local_inventory
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.insert_local_inventory
+        ] = mock_rpc
+        request = {}
+        client.insert_local_inventory(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.insert_local_inventory(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_insert_local_inventory_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = LocalInventoryServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -1816,14 +1954,60 @@
         response = await client.insert_local_inventory()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == localinventory.InsertLocalInventoryRequest()
 
 
 @pytest.mark.asyncio
+async def test_insert_local_inventory_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = LocalInventoryServiceAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.insert_local_inventory
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.insert_local_inventory
+        ] = mock_object
+
+        request = {}
+        await client.insert_local_inventory(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.insert_local_inventory(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_insert_local_inventory_async(
     transport: str = "grpc_asyncio",
     request_type=localinventory.InsertLocalInventoryRequest,
 ):
     client = LocalInventoryServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -1983,14 +2167,17 @@
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.delete_local_inventory), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.delete_local_inventory()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == localinventory.DeleteLocalInventoryRequest()
 
 
 def test_delete_local_inventory_non_empty_request_with_auto_populated_field():
@@ -2008,22 +2195,65 @@
         name="name_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.delete_local_inventory), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.delete_local_inventory(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == localinventory.DeleteLocalInventoryRequest(
             name="name_value",
         )
 
 
+def test_delete_local_inventory_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = LocalInventoryServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.delete_local_inventory
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.delete_local_inventory
+        ] = mock_rpc
+        request = {}
+        client.delete_local_inventory(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.delete_local_inventory(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_delete_local_inventory_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = LocalInventoryServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -2038,14 +2268,60 @@
         response = await client.delete_local_inventory()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == localinventory.DeleteLocalInventoryRequest()
 
 
 @pytest.mark.asyncio
+async def test_delete_local_inventory_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = LocalInventoryServiceAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.delete_local_inventory
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.delete_local_inventory
+        ] = mock_object
+
+        request = {}
+        await client.delete_local_inventory(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.delete_local_inventory(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_delete_local_inventory_async(
     transport: str = "grpc_asyncio",
     request_type=localinventory.DeleteLocalInventoryRequest,
 ):
     client = LocalInventoryServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -2261,14 +2537,55 @@
         response = client.list_local_inventories(request)
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.ListLocalInventoriesPager)
     assert response.next_page_token == "next_page_token_value"
 
 
+def test_list_local_inventories_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = LocalInventoryServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.list_local_inventories
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.list_local_inventories
+        ] = mock_rpc
+
+        request = {}
+        client.list_local_inventories(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.list_local_inventories(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_list_local_inventories_rest_required_fields(
     request_type=localinventory.ListLocalInventoriesRequest,
 ):
     transport_class = transports.LocalInventoryServiceRestTransport
 
     request_init = {}
     request_init["parent"] = ""
@@ -2702,14 +3019,55 @@
     assert response.availability == "availability_value"
     assert response.quantity == 895
     assert response.pickup_method == "pickup_method_value"
     assert response.pickup_sla == "pickup_sla_value"
     assert response.instore_product_location == "instore_product_location_value"
 
 
+def test_insert_local_inventory_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = LocalInventoryServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.insert_local_inventory
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.insert_local_inventory
+        ] = mock_rpc
+
+        request = {}
+        client.insert_local_inventory(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.insert_local_inventory(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_insert_local_inventory_rest_required_fields(
     request_type=localinventory.InsertLocalInventoryRequest,
 ):
     transport_class = transports.LocalInventoryServiceRestTransport
 
     request_init = {}
     request_init["parent"] = ""
@@ -2918,14 +3276,55 @@
         req.return_value = response_value
         response = client.delete_local_inventory(request)
 
     # Establish that the response is the type that we expect.
     assert response is None
 
 
+def test_delete_local_inventory_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = LocalInventoryServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.delete_local_inventory
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.delete_local_inventory
+        ] = mock_rpc
+
+        request = {}
+        client.delete_local_inventory(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.delete_local_inventory(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_delete_local_inventory_rest_required_fields(
     request_type=localinventory.DeleteLocalInventoryRequest,
 ):
     transport_class = transports.LocalInventoryServiceRestTransport
 
     request_init = {}
     request_init["name"] = ""
```

### Comparing `google-shopping-merchant-inventories-0.1.6/tests/unit/gapic/merchant_inventories_v1beta/test_regional_inventory_service.py` & `google-shopping-merchant-inventories-0.1.7/tests/unit/gapic/merchant_inventories_v1beta/test_regional_inventory_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -1243,14 +1243,17 @@
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_regional_inventories), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.list_regional_inventories()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == regionalinventory.ListRegionalInventoriesRequest()
 
 
 def test_list_regional_inventories_non_empty_request_with_auto_populated_field():
@@ -1269,23 +1272,66 @@
         page_token="page_token_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_regional_inventories), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.list_regional_inventories(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == regionalinventory.ListRegionalInventoriesRequest(
             parent="parent_value",
             page_token="page_token_value",
         )
 
 
+def test_list_regional_inventories_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = RegionalInventoryServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.list_regional_inventories
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.list_regional_inventories
+        ] = mock_rpc
+        request = {}
+        client.list_regional_inventories(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.list_regional_inventories(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_list_regional_inventories_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = RegionalInventoryServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -1304,14 +1350,60 @@
         response = await client.list_regional_inventories()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == regionalinventory.ListRegionalInventoriesRequest()
 
 
 @pytest.mark.asyncio
+async def test_list_regional_inventories_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = RegionalInventoryServiceAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.list_regional_inventories
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.list_regional_inventories
+        ] = mock_object
+
+        request = {}
+        await client.list_regional_inventories(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.list_regional_inventories(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_list_regional_inventories_async(
     transport: str = "grpc_asyncio",
     request_type=regionalinventory.ListRegionalInventoriesRequest,
 ):
     client = RegionalInventoryServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -1752,14 +1844,17 @@
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.insert_regional_inventory), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.insert_regional_inventory()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == regionalinventory.InsertRegionalInventoryRequest()
 
 
 def test_insert_regional_inventory_non_empty_request_with_auto_populated_field():
@@ -1777,22 +1872,65 @@
         parent="parent_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.insert_regional_inventory), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.insert_regional_inventory(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == regionalinventory.InsertRegionalInventoryRequest(
             parent="parent_value",
         )
 
 
+def test_insert_regional_inventory_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = RegionalInventoryServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.insert_regional_inventory
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.insert_regional_inventory
+        ] = mock_rpc
+        request = {}
+        client.insert_regional_inventory(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.insert_regional_inventory(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_insert_regional_inventory_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = RegionalInventoryServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -1814,14 +1952,60 @@
         response = await client.insert_regional_inventory()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == regionalinventory.InsertRegionalInventoryRequest()
 
 
 @pytest.mark.asyncio
+async def test_insert_regional_inventory_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = RegionalInventoryServiceAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.insert_regional_inventory
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.insert_regional_inventory
+        ] = mock_object
+
+        request = {}
+        await client.insert_regional_inventory(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.insert_regional_inventory(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_insert_regional_inventory_async(
     transport: str = "grpc_asyncio",
     request_type=regionalinventory.InsertRegionalInventoryRequest,
 ):
     client = RegionalInventoryServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -1973,14 +2157,17 @@
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.delete_regional_inventory), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.delete_regional_inventory()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == regionalinventory.DeleteRegionalInventoryRequest()
 
 
 def test_delete_regional_inventory_non_empty_request_with_auto_populated_field():
@@ -1998,22 +2185,65 @@
         name="name_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.delete_regional_inventory), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.delete_regional_inventory(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == regionalinventory.DeleteRegionalInventoryRequest(
             name="name_value",
         )
 
 
+def test_delete_regional_inventory_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = RegionalInventoryServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.delete_regional_inventory
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.delete_regional_inventory
+        ] = mock_rpc
+        request = {}
+        client.delete_regional_inventory(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.delete_regional_inventory(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_delete_regional_inventory_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = RegionalInventoryServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -2028,14 +2258,60 @@
         response = await client.delete_regional_inventory()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == regionalinventory.DeleteRegionalInventoryRequest()
 
 
 @pytest.mark.asyncio
+async def test_delete_regional_inventory_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = RegionalInventoryServiceAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.delete_regional_inventory
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.delete_regional_inventory
+        ] = mock_object
+
+        request = {}
+        await client.delete_regional_inventory(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.delete_regional_inventory(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_delete_regional_inventory_async(
     transport: str = "grpc_asyncio",
     request_type=regionalinventory.DeleteRegionalInventoryRequest,
 ):
     client = RegionalInventoryServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -2253,14 +2529,55 @@
         response = client.list_regional_inventories(request)
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.ListRegionalInventoriesPager)
     assert response.next_page_token == "next_page_token_value"
 
 
+def test_list_regional_inventories_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = RegionalInventoryServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.list_regional_inventories
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.list_regional_inventories
+        ] = mock_rpc
+
+        request = {}
+        client.list_regional_inventories(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.list_regional_inventories(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_list_regional_inventories_rest_required_fields(
     request_type=regionalinventory.ListRegionalInventoriesRequest,
 ):
     transport_class = transports.RegionalInventoryServiceRestTransport
 
     request_init = {}
     request_init["parent"] = ""
@@ -2692,14 +3009,55 @@
     assert isinstance(response, regionalinventory.RegionalInventory)
     assert response.name == "name_value"
     assert response.account == 749
     assert response.region == "region_value"
     assert response.availability == "availability_value"
 
 
+def test_insert_regional_inventory_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = RegionalInventoryServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.insert_regional_inventory
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.insert_regional_inventory
+        ] = mock_rpc
+
+        request = {}
+        client.insert_regional_inventory(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.insert_regional_inventory(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_insert_regional_inventory_rest_required_fields(
     request_type=regionalinventory.InsertRegionalInventoryRequest,
 ):
     transport_class = transports.RegionalInventoryServiceRestTransport
 
     request_init = {}
     request_init["parent"] = ""
@@ -2911,14 +3269,55 @@
         req.return_value = response_value
         response = client.delete_regional_inventory(request)
 
     # Establish that the response is the type that we expect.
     assert response is None
 
 
+def test_delete_regional_inventory_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = RegionalInventoryServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.delete_regional_inventory
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.delete_regional_inventory
+        ] = mock_rpc
+
+        request = {}
+        client.delete_regional_inventory(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.delete_regional_inventory(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_delete_regional_inventory_rest_required_fields(
     request_type=regionalinventory.DeleteRegionalInventoryRequest,
 ):
     transport_class = transports.RegionalInventoryServiceRestTransport
 
     request_init = {}
     request_init["name"] = ""
```

