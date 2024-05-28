# Comparing `tmp/google-shopping-merchant-lfp-0.1.0.tar.gz` & `tmp/google-shopping-merchant-lfp-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-shopping-merchant-lfp-0.1.0.tar", last modified: Wed Apr 17 14:53:11 2024, max compression
+gzip compressed data, was "google-shopping-merchant-lfp-0.1.1.tar", last modified: Tue May 28 08:24:15 2024, max compression
```

## Comparing `google-shopping-merchant-lfp-0.1.0.tar` & `google-shopping-merchant-lfp-0.1.1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-17 14:53:11.271025 google-shopping-merchant-lfp-0.1.0/
--rw-rw-r--   0 root         (0)     1003    11358 2024-04-17 14:49:31.000000 google-shopping-merchant-lfp-0.1.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2024-04-17 14:49:31.000000 google-shopping-merchant-lfp-0.1.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     5195 2024-04-17 14:53:11.271025 google-shopping-merchant-lfp-0.1.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3754 2024-04-17 14:49:31.000000 google-shopping-merchant-lfp-0.1.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-17 14:53:11.251025 google-shopping-merchant-lfp-0.1.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-17 14:53:11.251025 google-shopping-merchant-lfp-0.1.0/google/shopping/
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-17 14:53:11.255025 google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp/
--rw-rw-r--   0 root         (0)     1003     2342 2024-04-17 14:49:31.000000 google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2024-04-17 14:49:31.000000 google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2024-04-17 14:49:31.000000 google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-17 14:53:11.255025 google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/
--rw-rw-r--   0 root         (0)     1003     1800 2024-04-17 14:49:31.000000 google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/__init__.py
--rw-rw-r--   0 root         (0)     1003     3750 2024-04-17 14:49:31.000000 google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2024-04-17 14:49:31.000000 google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2024-04-17 14:49:31.000000 google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-17 14:53:11.255025 google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/
--rw-rw-r--   0 root         (0)     1003      600 2024-04-17 14:49:31.000000 google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-17 14:53:11.259025 google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/lfp_inventory_service/
--rw-rw-r--   0 root         (0)     1003      789 2024-04-17 14:49:31.000000 google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/lfp_inventory_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    15261 2024-04-17 14:49:31.000000 google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/lfp_inventory_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    31936 2024-04-17 14:49:31.000000 google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/lfp_inventory_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-17 14:53:11.259025 google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/lfp_inventory_service/transports/
--rw-rw-r--   0 root         (0)     1003     1478 2024-04-17 14:49:31.000000 google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/lfp_inventory_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6166 2024-04-17 14:49:31.000000 google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/lfp_inventory_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    12103 2024-04-17 14:49:31.000000 google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/lfp_inventory_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    12327 2024-04-17 14:49:31.000000 google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/lfp_inventory_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    12505 2024-04-17 14:49:31.000000 google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/lfp_inventory_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-17 14:53:11.259025 google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/lfp_sale_service/
--rw-rw-r--   0 root         (0)     1003      769 2024-04-17 14:49:31.000000 google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/lfp_sale_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    14769 2024-04-17 14:49:31.000000 google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/lfp_sale_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    31199 2024-04-17 14:49:31.000000 google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/lfp_sale_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-17 14:53:11.259025 google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/lfp_sale_service/transports/
--rw-rw-r--   0 root         (0)     1003     1400 2024-04-17 14:49:31.000000 google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/lfp_sale_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6101 2024-04-17 14:49:31.000000 google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/lfp_sale_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    11832 2024-04-17 14:49:31.000000 google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/lfp_sale_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    12037 2024-04-17 14:49:31.000000 google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/lfp_sale_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    12124 2024-04-17 14:49:31.000000 google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/lfp_sale_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-17 14:53:11.263025 google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/lfp_store_service/
--rw-rw-r--   0 root         (0)     1003      773 2024-04-17 14:49:31.000000 google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/lfp_store_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    29226 2024-04-17 14:49:31.000000 google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/lfp_store_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    46252 2024-04-17 14:49:31.000000 google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/lfp_store_service/client.py
--rw-rw-r--   0 root         (0)     1003     5831 2024-04-17 14:49:31.000000 google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/lfp_store_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-17 14:53:11.263025 google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/lfp_store_service/transports/
--rw-rw-r--   0 root         (0)     1003     1414 2024-04-17 14:49:31.000000 google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/lfp_store_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7456 2024-04-17 14:49:31.000000 google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/lfp_store_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    15356 2024-04-17 14:49:31.000000 google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/lfp_store_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    15642 2024-04-17 14:49:31.000000 google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/lfp_store_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    26446 2024-04-17 14:49:31.000000 google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/lfp_store_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-17 14:53:11.263025 google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/types/
--rw-rw-r--   0 root         (0)     1003     1156 2024-04-17 14:49:31.000000 google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     6590 2024-04-17 14:49:31.000000 google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/types/lfpinventory.py
--rw-rw-r--   0 root         (0)     1003     4966 2024-04-17 14:49:31.000000 google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/types/lfpsale.py
--rw-rw-r--   0 root         (0)     1003    10364 2024-04-17 14:49:31.000000 google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/types/lfpstore.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-17 14:53:11.267025 google-shopping-merchant-lfp-0.1.0/google_shopping_merchant_lfp.egg-info/
--rw-r--r--   0 root         (0)     1003     5195 2024-04-17 14:53:11.000000 google-shopping-merchant-lfp-0.1.0/google_shopping_merchant_lfp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     3307 2024-04-17 14:53:11.000000 google-shopping-merchant-lfp-0.1.0/google_shopping_merchant_lfp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2024-04-17 14:53:11.000000 google-shopping-merchant-lfp-0.1.0/google_shopping_merchant_lfp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003        1 2024-04-17 14:53:11.000000 google-shopping-merchant-lfp-0.1.0/google_shopping_merchant_lfp.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      343 2024-04-17 14:53:11.000000 google-shopping-merchant-lfp-0.1.0/google_shopping_merchant_lfp.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2024-04-17 14:53:11.000000 google-shopping-merchant-lfp-0.1.0/google_shopping_merchant_lfp.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2024-04-17 14:53:11.271025 google-shopping-merchant-lfp-0.1.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3249 2024-04-17 14:49:31.000000 google-shopping-merchant-lfp-0.1.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-17 14:53:11.267025 google-shopping-merchant-lfp-0.1.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2024-04-17 14:49:31.000000 google-shopping-merchant-lfp-0.1.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-17 14:53:11.267025 google-shopping-merchant-lfp-0.1.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2024-04-17 14:49:31.000000 google-shopping-merchant-lfp-0.1.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-17 14:53:11.267025 google-shopping-merchant-lfp-0.1.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2024-04-17 14:49:31.000000 google-shopping-merchant-lfp-0.1.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-17 14:53:11.267025 google-shopping-merchant-lfp-0.1.0/tests/unit/gapic/merchant_lfp_v1beta/
--rw-rw-r--   0 root         (0)     1003      600 2024-04-17 14:49:31.000000 google-shopping-merchant-lfp-0.1.0/tests/unit/gapic/merchant_lfp_v1beta/__init__.py
--rw-rw-r--   0 root         (0)     1003    95174 2024-04-17 14:49:31.000000 google-shopping-merchant-lfp-0.1.0/tests/unit/gapic/merchant_lfp_v1beta/test_lfp_inventory_service.py
--rw-rw-r--   0 root         (0)     1003    91140 2024-04-17 14:49:31.000000 google-shopping-merchant-lfp-0.1.0/tests/unit/gapic/merchant_lfp_v1beta/test_lfp_sale_service.py
--rw-rw-r--   0 root         (0)     1003   169660 2024-04-17 14:49:31.000000 google-shopping-merchant-lfp-0.1.0/tests/unit/gapic/merchant_lfp_v1beta/test_lfp_store_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:15.785914 google-shopping-merchant-lfp-0.1.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2024-05-28 08:20:21.000000 google-shopping-merchant-lfp-0.1.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2024-05-28 08:20:21.000000 google-shopping-merchant-lfp-0.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     5195 2024-05-28 08:24:15.785914 google-shopping-merchant-lfp-0.1.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3754 2024-05-28 08:20:21.000000 google-shopping-merchant-lfp-0.1.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:15.765910 google-shopping-merchant-lfp-0.1.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:15.765910 google-shopping-merchant-lfp-0.1.1/google/shopping/
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:15.769911 google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp/
+-rw-rw-r--   0 root         (0)     1003     2342 2024-05-28 08:20:21.000000 google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2024-05-28 08:20:21.000000 google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2024-05-28 08:20:21.000000 google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:15.773912 google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/
+-rw-rw-r--   0 root         (0)     1003     1800 2024-05-28 08:20:21.000000 google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3750 2024-05-28 08:20:21.000000 google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2024-05-28 08:20:21.000000 google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2024-05-28 08:20:21.000000 google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:15.773912 google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-28 08:20:21.000000 google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:15.773912 google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/lfp_inventory_service/
+-rw-rw-r--   0 root         (0)     1003      789 2024-05-28 08:20:21.000000 google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/lfp_inventory_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    15865 2024-05-28 08:20:21.000000 google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/lfp_inventory_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    32666 2024-05-28 08:20:21.000000 google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/lfp_inventory_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:15.773912 google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/lfp_inventory_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1478 2024-05-28 08:20:21.000000 google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/lfp_inventory_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6166 2024-05-28 08:20:21.000000 google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/lfp_inventory_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    12650 2024-05-28 08:20:21.000000 google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/lfp_inventory_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13309 2024-05-28 08:20:21.000000 google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/lfp_inventory_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    12505 2024-05-28 08:20:21.000000 google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/lfp_inventory_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:15.773912 google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/lfp_sale_service/
+-rw-rw-r--   0 root         (0)     1003      769 2024-05-28 08:20:21.000000 google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/lfp_sale_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    15285 2024-05-28 08:20:21.000000 google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/lfp_sale_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    31829 2024-05-28 08:20:21.000000 google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/lfp_sale_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:15.777913 google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/lfp_sale_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1400 2024-05-28 08:20:21.000000 google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/lfp_sale_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6101 2024-05-28 08:20:21.000000 google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/lfp_sale_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    12379 2024-05-28 08:20:21.000000 google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/lfp_sale_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13009 2024-05-28 08:20:21.000000 google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/lfp_sale_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    12124 2024-05-28 08:20:21.000000 google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/lfp_sale_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:15.777913 google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/lfp_store_service/
+-rw-rw-r--   0 root         (0)     1003      773 2024-05-28 08:20:21.000000 google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/lfp_store_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    30275 2024-05-28 08:20:21.000000 google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/lfp_store_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    46723 2024-05-28 08:20:21.000000 google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/lfp_store_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5831 2024-05-28 08:20:21.000000 google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/lfp_store_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:15.777913 google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/lfp_store_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1414 2024-05-28 08:20:21.000000 google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/lfp_store_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7456 2024-05-28 08:20:21.000000 google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/lfp_store_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    15903 2024-05-28 08:20:21.000000 google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/lfp_store_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    17217 2024-05-28 08:20:21.000000 google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/lfp_store_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    26488 2024-05-28 08:20:21.000000 google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/lfp_store_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:15.781913 google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/types/
+-rw-rw-r--   0 root         (0)     1003     1156 2024-05-28 08:20:21.000000 google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6590 2024-05-28 08:20:21.000000 google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/types/lfpinventory.py
+-rw-rw-r--   0 root         (0)     1003     4966 2024-05-28 08:20:21.000000 google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/types/lfpsale.py
+-rw-rw-r--   0 root         (0)     1003    10345 2024-05-28 08:20:21.000000 google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/types/lfpstore.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:15.781913 google-shopping-merchant-lfp-0.1.1/google_shopping_merchant_lfp.egg-info/
+-rw-r--r--   0 root         (0)     1003     5195 2024-05-28 08:24:15.000000 google-shopping-merchant-lfp-0.1.1/google_shopping_merchant_lfp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     3307 2024-05-28 08:24:15.000000 google-shopping-merchant-lfp-0.1.1/google_shopping_merchant_lfp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-05-28 08:24:15.000000 google-shopping-merchant-lfp-0.1.1/google_shopping_merchant_lfp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-05-28 08:24:15.000000 google-shopping-merchant-lfp-0.1.1/google_shopping_merchant_lfp.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      343 2024-05-28 08:24:15.000000 google-shopping-merchant-lfp-0.1.1/google_shopping_merchant_lfp.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2024-05-28 08:24:15.000000 google-shopping-merchant-lfp-0.1.1/google_shopping_merchant_lfp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2024-05-28 08:24:15.785914 google-shopping-merchant-lfp-0.1.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3249 2024-05-28 08:20:21.000000 google-shopping-merchant-lfp-0.1.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:15.781913 google-shopping-merchant-lfp-0.1.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-28 08:20:21.000000 google-shopping-merchant-lfp-0.1.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:15.781913 google-shopping-merchant-lfp-0.1.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-28 08:20:21.000000 google-shopping-merchant-lfp-0.1.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:15.781913 google-shopping-merchant-lfp-0.1.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-28 08:20:21.000000 google-shopping-merchant-lfp-0.1.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-28 08:24:15.785914 google-shopping-merchant-lfp-0.1.1/tests/unit/gapic/merchant_lfp_v1beta/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-28 08:20:21.000000 google-shopping-merchant-lfp-0.1.1/tests/unit/gapic/merchant_lfp_v1beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003    99833 2024-05-28 08:20:21.000000 google-shopping-merchant-lfp-0.1.1/tests/unit/gapic/merchant_lfp_v1beta/test_lfp_inventory_service.py
+-rw-rw-r--   0 root         (0)     1003    95617 2024-05-28 08:20:21.000000 google-shopping-merchant-lfp-0.1.1/tests/unit/gapic/merchant_lfp_v1beta/test_lfp_sale_service.py
+-rw-rw-r--   0 root         (0)     1003   187668 2024-05-28 08:20:21.000000 google-shopping-merchant-lfp-0.1.1/tests/unit/gapic/merchant_lfp_v1beta/test_lfp_store_service.py
```

### Comparing `google-shopping-merchant-lfp-0.1.0/LICENSE` & `google-shopping-merchant-lfp-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-lfp-0.1.0/MANIFEST.in` & `google-shopping-merchant-lfp-0.1.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-lfp-0.1.0/PKG-INFO` & `google-shopping-merchant-lfp-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-shopping-merchant-lfp
-Version: 0.1.0
+Version: 0.1.1
 Summary: Google Shopping Merchant Lfp API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-shopping-merchant-lfp
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-shopping-merchant-lfp-0.1.0/README.rst` & `google-shopping-merchant-lfp-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp/__init__.py` & `google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp/__init__.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp/gapic_version.py` & `google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.1.1"  # {x-release-please-version}
```

### Comparing `google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/__init__.py` & `google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/__init__.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/gapic_metadata.json` & `google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/gapic_version.py` & `google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.1.1"  # {x-release-please-version}
```

### Comparing `google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/__init__.py` & `google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/lfp_inventory_service/__init__.py` & `google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/lfp_inventory_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/lfp_inventory_service/async_client.py` & `google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/lfp_inventory_service/async_client.py`

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
@@ -198,29 +199,37 @@
         type(LfpInventoryServiceClient),
     )
 
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
-        transport: Union[str, LfpInventoryServiceTransport] = "grpc_asyncio",
+        transport: Optional[
+            Union[
+                str,
+                LfpInventoryServiceTransport,
+                Callable[..., LfpInventoryServiceTransport],
+            ]
+        ] = "grpc_asyncio",
         client_options: Optional[ClientOptions] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the lfp inventory service async client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
-            transport (Union[str, ~.LfpInventoryServiceTransport]): The
-                transport to use. If set to None, a transport is chosen
-                automatically.
+            transport (Optional[Union[str,LfpInventoryServiceTransport,Callable[..., LfpInventoryServiceTransport]]]):
+                The transport to use, or a Callable that constructs and returns a new transport to use.
+                If a Callable is given, it will be called with the same set of initialization
+                arguments as used in the LfpInventoryServiceTransport constructor.
+                If set to None, a transport is chosen automatically.
             client_options (Optional[Union[google.api_core.client_options.ClientOptions, dict]]):
                 Custom options for the client.
 
                 1. The ``api_endpoint`` property can be used to override the
                 default endpoint provided by the client when ``transport`` is
                 not explicitly provided. Only if this property is not set and
                 ``transport`` was not explicitly provided, the endpoint is
@@ -317,23 +326,24 @@
                 sent along with the request as metadata.
 
         Returns:
             google.shopping.merchant_lfp_v1beta.types.LfpInventory:
                 Local Inventory for the merchant.
         """
         # Create or coerce a protobuf request object.
-        request = lfpinventory.InsertLfpInventoryRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, lfpinventory.InsertLfpInventoryRequest):
+            request = lfpinventory.InsertLfpInventoryRequest(request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.insert_lfp_inventory,
-            default_timeout=None,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.insert_lfp_inventory
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
         )
```

### Comparing `google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/lfp_inventory_service/client.py` & `google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/lfp_inventory_service/client.py`

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
-        transport: Optional[Union[str, LfpInventoryServiceTransport]] = None,
+        transport: Optional[
+            Union[
+                str,
+                LfpInventoryServiceTransport,
+                Callable[..., LfpInventoryServiceTransport],
+            ]
+        ] = None,
         client_options: Optional[Union[client_options_lib.ClientOptions, dict]] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the lfp inventory service client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
-            transport (Union[str, LfpInventoryServiceTransport]): The
-                transport to use. If set to None, a transport is chosen
-                automatically.
+            transport (Optional[Union[str,LfpInventoryServiceTransport,Callable[..., LfpInventoryServiceTransport]]]):
+                The transport to use, or a Callable that constructs and returns a new transport.
+                If a Callable is given, it will be called with the same set of initialization
+                arguments as used in the LfpInventoryServiceTransport constructor.
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
+                Type[LfpInventoryServiceTransport],
+                Callable[..., LfpInventoryServiceTransport],
+            ] = (
+                type(self).get_transport_class(transport)
+                if isinstance(transport, str) or transport is None
+                else cast(Callable[..., LfpInventoryServiceTransport], transport)
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
@@ -729,18 +746,16 @@
                 sent along with the request as metadata.
 
         Returns:
             google.shopping.merchant_lfp_v1beta.types.LfpInventory:
                 Local Inventory for the merchant.
         """
         # Create or coerce a protobuf request object.
-        # Minor optimization to avoid making a copy if the user passes
-        # in a lfpinventory.InsertLfpInventoryRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, lfpinventory.InsertLfpInventoryRequest):
             request = lfpinventory.InsertLfpInventoryRequest(request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
         rpc = self._transport._wrapped_methods[self._transport.insert_lfp_inventory]
```

### Comparing `google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/lfp_inventory_service/transports/__init__.py` & `google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/lfp_inventory_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/lfp_inventory_service/transports/base.py` & `google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/lfp_inventory_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/lfp_inventory_service/transports/grpc.py` & `google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/lfp_inventory_service/transports/grpc.py`

 * *Files 3% similar despite different names*

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

### Comparing `google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/lfp_inventory_service/transports/grpc_asyncio.py` & `google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/lfp_inventory_service/transports/grpc_asyncio.py`

 * *Files 5% similar despite different names*

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
 import grpc  # type: ignore
 from grpc.experimental import aio  # type: ignore
 
 from google.shopping.merchant_lfp_v1beta.types import lfpinventory
 
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
@@ -259,12 +265,22 @@
             self._stubs["insert_lfp_inventory"] = self.grpc_channel.unary_unary(
                 "/google.shopping.merchant.lfp.v1beta.LfpInventoryService/InsertLfpInventory",
                 request_serializer=lfpinventory.InsertLfpInventoryRequest.serialize,
                 response_deserializer=lfpinventory.LfpInventory.deserialize,
             )
         return self._stubs["insert_lfp_inventory"]
 
+    def _prep_wrapped_messages(self, client_info):
+        """Precompute the wrapped methods, overriding the base class method to use async wrappers."""
+        self._wrapped_methods = {
+            self.insert_lfp_inventory: gapic_v1.method_async.wrap_method(
+                self.insert_lfp_inventory,
+                default_timeout=None,
+                client_info=client_info,
+            ),
+        }
+
     def close(self):
         return self.grpc_channel.close()
 
 
 __all__ = ("LfpInventoryServiceGrpcAsyncIOTransport",)
```

### Comparing `google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/lfp_inventory_service/transports/rest.py` & `google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/lfp_inventory_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/lfp_sale_service/__init__.py` & `google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/lfp_sale_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/lfp_sale_service/async_client.py` & `google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/lfp_sale_service/async_client.py`

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
@@ -195,29 +196,33 @@
         type(LfpSaleServiceClient).get_transport_class, type(LfpSaleServiceClient)
     )
 
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
-        transport: Union[str, LfpSaleServiceTransport] = "grpc_asyncio",
+        transport: Optional[
+            Union[str, LfpSaleServiceTransport, Callable[..., LfpSaleServiceTransport]]
+        ] = "grpc_asyncio",
         client_options: Optional[ClientOptions] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the lfp sale service async client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
-            transport (Union[str, ~.LfpSaleServiceTransport]): The
-                transport to use. If set to None, a transport is chosen
-                automatically.
+            transport (Optional[Union[str,LfpSaleServiceTransport,Callable[..., LfpSaleServiceTransport]]]):
+                The transport to use, or a Callable that constructs and returns a new transport to use.
+                If a Callable is given, it will be called with the same set of initialization
+                arguments as used in the LfpSaleServiceTransport constructor.
+                If set to None, a transport is chosen automatically.
             client_options (Optional[Union[google.api_core.client_options.ClientOptions, dict]]):
                 Custom options for the client.
 
                 1. The ``api_endpoint`` property can be used to override the
                 default endpoint provided by the client when ``transport`` is
                 not explicitly provided. Only if this property is not set and
                 ``transport`` was not explicitly provided, the endpoint is
@@ -314,23 +319,24 @@
                 sent along with the request as metadata.
 
         Returns:
             google.shopping.merchant_lfp_v1beta.types.LfpSale:
                 A sale for the merchant.
         """
         # Create or coerce a protobuf request object.
-        request = lfpsale.InsertLfpSaleRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, lfpsale.InsertLfpSaleRequest):
+            request = lfpsale.InsertLfpSaleRequest(request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.insert_lfp_sale,
-            default_timeout=None,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.insert_lfp_sale
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
         )
```

### Comparing `google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/lfp_sale_service/client.py` & `google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/lfp_sale_service/client.py`

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
@@ -525,29 +526,33 @@
         """
         return self._universe_domain
 
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
-        transport: Optional[Union[str, LfpSaleServiceTransport]] = None,
+        transport: Optional[
+            Union[str, LfpSaleServiceTransport, Callable[..., LfpSaleServiceTransport]]
+        ] = None,
         client_options: Optional[Union[client_options_lib.ClientOptions, dict]] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the lfp sale service client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
-            transport (Union[str, LfpSaleServiceTransport]): The
-                transport to use. If set to None, a transport is chosen
-                automatically.
+            transport (Optional[Union[str,LfpSaleServiceTransport,Callable[..., LfpSaleServiceTransport]]]):
+                The transport to use, or a Callable that constructs and returns a new transport.
+                If a Callable is given, it will be called with the same set of initialization
+                arguments as used in the LfpSaleServiceTransport constructor.
+                If set to None, a transport is chosen automatically.
             client_options (Optional[Union[google.api_core.client_options.ClientOptions, dict]]):
                 Custom options for the client.
 
                 1. The ``api_endpoint`` property can be used to override the
                 default endpoint provided by the client when ``transport`` is
                 not explicitly provided. Only if this property is not set and
                 ``transport`` was not explicitly provided, the endpoint is
@@ -648,16 +653,23 @@
             if api_key_value and hasattr(
                 google.auth._default, "get_api_key_credentials"
             ):
                 credentials = google.auth._default.get_api_key_credentials(
                     api_key_value
                 )
 
-            Transport = type(self).get_transport_class(cast(str, transport))
-            self._transport = Transport(
+            transport_init: Union[
+                Type[LfpSaleServiceTransport], Callable[..., LfpSaleServiceTransport]
+            ] = (
+                type(self).get_transport_class(transport)
+                if isinstance(transport, str) or transport is None
+                else cast(Callable[..., LfpSaleServiceTransport], transport)
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
@@ -722,18 +734,16 @@
                 sent along with the request as metadata.
 
         Returns:
             google.shopping.merchant_lfp_v1beta.types.LfpSale:
                 A sale for the merchant.
         """
         # Create or coerce a protobuf request object.
-        # Minor optimization to avoid making a copy if the user passes
-        # in a lfpsale.InsertLfpSaleRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, lfpsale.InsertLfpSaleRequest):
             request = lfpsale.InsertLfpSaleRequest(request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
         rpc = self._transport._wrapped_methods[self._transport.insert_lfp_sale]
```

### Comparing `google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/lfp_sale_service/transports/__init__.py` & `google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/lfp_sale_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/lfp_sale_service/transports/base.py` & `google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/lfp_sale_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/lfp_sale_service/transports/grpc.py` & `google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/lfp_sale_service/transports/grpc.py`

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

### Comparing `google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/lfp_sale_service/transports/grpc_asyncio.py` & `google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/lfp_sale_service/transports/grpc_asyncio.py`

 * *Files 4% similar despite different names*

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
 import grpc  # type: ignore
 from grpc.experimental import aio  # type: ignore
 
 from google.shopping.merchant_lfp_v1beta.types import lfpsale
 
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
@@ -255,12 +261,22 @@
             self._stubs["insert_lfp_sale"] = self.grpc_channel.unary_unary(
                 "/google.shopping.merchant.lfp.v1beta.LfpSaleService/InsertLfpSale",
                 request_serializer=lfpsale.InsertLfpSaleRequest.serialize,
                 response_deserializer=lfpsale.LfpSale.deserialize,
             )
         return self._stubs["insert_lfp_sale"]
 
+    def _prep_wrapped_messages(self, client_info):
+        """Precompute the wrapped methods, overriding the base class method to use async wrappers."""
+        self._wrapped_methods = {
+            self.insert_lfp_sale: gapic_v1.method_async.wrap_method(
+                self.insert_lfp_sale,
+                default_timeout=None,
+                client_info=client_info,
+            ),
+        }
+
     def close(self):
         return self.grpc_channel.close()
 
 
 __all__ = ("LfpSaleServiceGrpcAsyncIOTransport",)
```

### Comparing `google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/lfp_sale_service/transports/rest.py` & `google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/lfp_sale_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/lfp_store_service/__init__.py` & `google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/lfp_store_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/lfp_store_service/async_client.py` & `google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/lfp_store_service/async_client.py`

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
@@ -193,29 +194,35 @@
         type(LfpStoreServiceClient).get_transport_class, type(LfpStoreServiceClient)
     )
 
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
-        transport: Union[str, LfpStoreServiceTransport] = "grpc_asyncio",
+        transport: Optional[
+            Union[
+                str, LfpStoreServiceTransport, Callable[..., LfpStoreServiceTransport]
+            ]
+        ] = "grpc_asyncio",
         client_options: Optional[ClientOptions] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the lfp store service async client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
-            transport (Union[str, ~.LfpStoreServiceTransport]): The
-                transport to use. If set to None, a transport is chosen
-                automatically.
+            transport (Optional[Union[str,LfpStoreServiceTransport,Callable[..., LfpStoreServiceTransport]]]):
+                The transport to use, or a Callable that constructs and returns a new transport to use.
+                If a Callable is given, it will be called with the same set of initialization
+                arguments as used in the LfpStoreServiceTransport constructor.
+                If set to None, a transport is chosen automatically.
             client_options (Optional[Union[google.api_core.client_options.ClientOptions, dict]]):
                 Custom options for the client.
 
                 1. The ``api_endpoint`` property can be used to override the
                 default endpoint provided by the client when ``transport`` is
                 not explicitly provided. Only if this property is not set and
                 ``transport`` was not explicitly provided, the endpoint is
@@ -307,45 +314,47 @@
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.shopping.merchant_lfp_v1beta.types.LfpStore:
                 A store for the merchant. This will
-                be used to match to a Google Business
-                Profile listing for the target merchant.
-                If a matching listing can't be found,
-                the inventories or sales submitted with
-                the store code will not be used.
+                be used to match to a store under the
+                Google Business Profile of the target
+                merchant. If a matching store can't be
+                found, the inventories or sales
+                submitted with the store code will not
+                be used.
 
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
 
-        request = lfpstore.GetLfpStoreRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, lfpstore.GetLfpStoreRequest):
+            request = lfpstore.GetLfpStoreRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if name is not None:
             request.name = name
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.get_lfp_store,
-            default_timeout=None,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.get_lfp_store
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
@@ -430,47 +439,49 @@
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.shopping.merchant_lfp_v1beta.types.LfpStore:
                 A store for the merchant. This will
-                be used to match to a Google Business
-                Profile listing for the target merchant.
-                If a matching listing can't be found,
-                the inventories or sales submitted with
-                the store code will not be used.
+                be used to match to a store under the
+                Google Business Profile of the target
+                merchant. If a matching store can't be
+                found, the inventories or sales
+                submitted with the store code will not
+                be used.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, lfp_store])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = lfpstore.InsertLfpStoreRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, lfpstore.InsertLfpStoreRequest):
+            request = lfpstore.InsertLfpStoreRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if parent is not None:
             request.parent = parent
         if lfp_store is not None:
             request.lfp_store = lfp_store
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.insert_lfp_store,
-            default_timeout=None,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.insert_lfp_store
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
         )
 
@@ -537,37 +548,38 @@
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
 
-        request = lfpstore.DeleteLfpStoreRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, lfpstore.DeleteLfpStoreRequest):
+            request = lfpstore.DeleteLfpStoreRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if name is not None:
             request.name = name
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.delete_lfp_store,
-            default_timeout=None,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.delete_lfp_store
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
@@ -645,37 +657,38 @@
                 ListLfpStores method.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
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
 
-        request = lfpstore.ListLfpStoresRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, lfpstore.ListLfpStoresRequest):
+            request = lfpstore.ListLfpStoresRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if parent is not None:
             request.parent = parent
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.list_lfp_stores,
-            default_timeout=None,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.list_lfp_stores
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
         )
```

### Comparing `google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/lfp_store_service/client.py` & `google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/lfp_store_service/client.py`

 * *Files 7% similar despite different names*

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
@@ -528,29 +529,35 @@
         """
         return self._universe_domain
 
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
-        transport: Optional[Union[str, LfpStoreServiceTransport]] = None,
+        transport: Optional[
+            Union[
+                str, LfpStoreServiceTransport, Callable[..., LfpStoreServiceTransport]
+            ]
+        ] = None,
         client_options: Optional[Union[client_options_lib.ClientOptions, dict]] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the lfp store service client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
-            transport (Union[str, LfpStoreServiceTransport]): The
-                transport to use. If set to None, a transport is chosen
-                automatically.
+            transport (Optional[Union[str,LfpStoreServiceTransport,Callable[..., LfpStoreServiceTransport]]]):
+                The transport to use, or a Callable that constructs and returns a new transport.
+                If a Callable is given, it will be called with the same set of initialization
+                arguments as used in the LfpStoreServiceTransport constructor.
+                If set to None, a transport is chosen automatically.
             client_options (Optional[Union[google.api_core.client_options.ClientOptions, dict]]):
                 Custom options for the client.
 
                 1. The ``api_endpoint`` property can be used to override the
                 default endpoint provided by the client when ``transport`` is
                 not explicitly provided. Only if this property is not set and
                 ``transport`` was not explicitly provided, the endpoint is
@@ -651,16 +658,23 @@
             if api_key_value and hasattr(
                 google.auth._default, "get_api_key_credentials"
             ):
                 credentials = google.auth._default.get_api_key_credentials(
                     api_key_value
                 )
 
-            Transport = type(self).get_transport_class(cast(str, transport))
-            self._transport = Transport(
+            transport_init: Union[
+                Type[LfpStoreServiceTransport], Callable[..., LfpStoreServiceTransport]
+            ] = (
+                type(self).get_transport_class(transport)
+                if isinstance(transport, str) or transport is None
+                else cast(Callable[..., LfpStoreServiceTransport], transport)
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
@@ -720,35 +734,34 @@
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.shopping.merchant_lfp_v1beta.types.LfpStore:
                 A store for the merchant. This will
-                be used to match to a Google Business
-                Profile listing for the target merchant.
-                If a matching listing can't be found,
-                the inventories or sales submitted with
-                the store code will not be used.
+                be used to match to a store under the
+                Google Business Profile of the target
+                merchant. If a matching store can't be
+                found, the inventories or sales
+                submitted with the store code will not
+                be used.
 
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
-        # in a lfpstore.GetLfpStoreRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, lfpstore.GetLfpStoreRequest):
             request = lfpstore.GetLfpStoreRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if name is not None:
                 request.name = name
 
@@ -843,35 +856,34 @@
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.shopping.merchant_lfp_v1beta.types.LfpStore:
                 A store for the merchant. This will
-                be used to match to a Google Business
-                Profile listing for the target merchant.
-                If a matching listing can't be found,
-                the inventories or sales submitted with
-                the store code will not be used.
+                be used to match to a store under the
+                Google Business Profile of the target
+                merchant. If a matching store can't be
+                found, the inventories or sales
+                submitted with the store code will not
+                be used.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, lfp_store])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a lfpstore.InsertLfpStoreRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, lfpstore.InsertLfpStoreRequest):
             request = lfpstore.InsertLfpStoreRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if parent is not None:
                 request.parent = parent
             if lfp_store is not None:
@@ -950,27 +962,25 @@
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
-        # in a lfpstore.DeleteLfpStoreRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, lfpstore.DeleteLfpStoreRequest):
             request = lfpstore.DeleteLfpStoreRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if name is not None:
                 request.name = name
 
@@ -1058,27 +1068,25 @@
                 ListLfpStores method.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
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
-        # in a lfpstore.ListLfpStoresRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, lfpstore.ListLfpStoresRequest):
             request = lfpstore.ListLfpStoresRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if parent is not None:
                 request.parent = parent
```

### Comparing `google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/lfp_store_service/pagers.py` & `google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/lfp_store_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/lfp_store_service/transports/__init__.py` & `google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/lfp_store_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/lfp_store_service/transports/base.py` & `google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/lfp_store_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/lfp_store_service/transports/grpc.py` & `google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/lfp_store_service/transports/grpc.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,15 +48,15 @@
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
@@ -68,36 +68,39 @@
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
@@ -115,15 +118,15 @@
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
@@ -156,15 +159,17 @@
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

### Comparing `google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/lfp_store_service/transports/grpc_asyncio.py` & `google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/lfp_store_service/transports/grpc_asyncio.py`

 * *Files 4% similar despite different names*

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
 
 from google.shopping.merchant_lfp_v1beta.types import lfpstore
@@ -63,15 +65,14 @@
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
@@ -93,15 +94,15 @@
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
@@ -113,37 +114,40 @@
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
@@ -161,15 +165,15 @@
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
@@ -201,15 +205,17 @@
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
@@ -339,12 +345,37 @@
             self._stubs["list_lfp_stores"] = self.grpc_channel.unary_unary(
                 "/google.shopping.merchant.lfp.v1beta.LfpStoreService/ListLfpStores",
                 request_serializer=lfpstore.ListLfpStoresRequest.serialize,
                 response_deserializer=lfpstore.ListLfpStoresResponse.deserialize,
             )
         return self._stubs["list_lfp_stores"]
 
+    def _prep_wrapped_messages(self, client_info):
+        """Precompute the wrapped methods, overriding the base class method to use async wrappers."""
+        self._wrapped_methods = {
+            self.get_lfp_store: gapic_v1.method_async.wrap_method(
+                self.get_lfp_store,
+                default_timeout=None,
+                client_info=client_info,
+            ),
+            self.insert_lfp_store: gapic_v1.method_async.wrap_method(
+                self.insert_lfp_store,
+                default_timeout=None,
+                client_info=client_info,
+            ),
+            self.delete_lfp_store: gapic_v1.method_async.wrap_method(
+                self.delete_lfp_store,
+                default_timeout=None,
+                client_info=client_info,
+            ),
+            self.list_lfp_stores: gapic_v1.method_async.wrap_method(
+                self.list_lfp_stores,
+                default_timeout=None,
+                client_info=client_info,
+            ),
+        }
+
     def close(self):
         return self.grpc_channel.close()
 
 
 __all__ = ("LfpStoreServiceGrpcAsyncIOTransport",)
```

### Comparing `google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/services/lfp_store_service/transports/rest.py` & `google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/services/lfp_store_service/transports/rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -381,19 +381,20 @@
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
                 ~.lfpstore.LfpStore:
                     A store for the merchant. This will
-                be used to match to a Google Business
-                Profile listing for the target merchant.
-                If a matching listing can't be found,
-                the inventories or sales submitted with
-                the store code will not be used.
+                be used to match to a store under the
+                Google Business Profile of the target
+                merchant. If a matching store can't be
+                found, the inventories or sales
+                submitted with the store code will not
+                be used.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "get",
                     "uri": "/lfp/v1beta/{name=accounts/*/lfpStores/*}",
@@ -473,19 +474,20 @@
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
                 ~.lfpstore.LfpStore:
                     A store for the merchant. This will
-                be used to match to a Google Business
-                Profile listing for the target merchant.
-                If a matching listing can't be found,
-                the inventories or sales submitted with
-                the store code will not be used.
+                be used to match to a store under the
+                Google Business Profile of the target
+                merchant. If a matching store can't be
+                found, the inventories or sales
+                submitted with the store code will not
+                be used.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "post",
                     "uri": "/lfp/v1beta/{parent=accounts/*}/lfpStores:insert",
```

### Comparing `google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/types/__init__.py` & `google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/types/lfpinventory.py` & `google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/types/lfpinventory.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
             This field is a member of `oneof`_ ``_gtin``.
         price (google.shopping.type.types.Price):
             Optional. The current price of the product.
         availability (str):
             Required. Availability of the product at this store. For
             accepted attribute values, see the `local product inventory
-            feed
+            data
             specification <https://support.google.com/merchants/answer/3061342>`__
         quantity (int):
             Optional. Quantity of the product available
             at this store. Must be greater than or equal to
             zero.
 
             This field is a member of `oneof`_ ``_quantity``.
@@ -83,23 +83,23 @@
             Optional. The time when the inventory is
             collected. If not set, it will be set to the
             time when the inventory is submitted.
         pickup_method (str):
             Optional. Supported pickup method for this offer. Unless the
             value is "not supported", this field must be submitted
             together with ``pickupSla``. For accepted attribute values,
-            see the `local product inventory feed
+            see the `local product inventory data
             specification <https://support.google.com/merchants/answer/3061342>`__.
 
             This field is a member of `oneof`_ ``_pickup_method``.
         pickup_sla (str):
             Optional. Expected date that an order will be ready for
             pickup relative to the order date. Must be submitted
             together with ``pickupMethod``. For accepted attribute
-            values, see the `local product inventory feed
+            values, see the `local product inventory data
             specification <https://support.google.com/merchants/answer/3061342>`__.
 
             This field is a member of `oneof`_ ``_pickup_sla``.
         feed_label (str):
             Optional. The `feed
             label <https://developers.google.com/shopping-content/guides/products/feed-labels>`__
             for the product. If this is not set, it will default to
```

### Comparing `google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/types/lfpsale.py` & `google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/types/lfpsale.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-lfp-0.1.0/google/shopping/merchant_lfp_v1beta/types/lfpstore.py` & `google-shopping-merchant-lfp-0.1.1/google/shopping/merchant_lfp_v1beta/types/lfpstore.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,16 +30,16 @@
         "ListLfpStoresResponse",
     },
 )
 
 
 class LfpStore(proto.Message):
     r"""A store for the merchant. This will be used to match to a
-    Google Business Profile listing for the target merchant. If a
-    matching listing can't be found, the inventories or sales
+    store under the Google Business Profile of the target merchant.
+    If a matching store can't be found, the inventories or sales
     submitted with the store code will not be used.
 
 
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
     Attributes:
         name (str):
@@ -78,15 +78,15 @@
             Optional. The `Google Place
             Id <https://developers.google.com/maps/documentation/places/web-service/place-id#id-overview>`__
             of the store location.
 
             This field is a member of `oneof`_ ``_place_id``.
         matching_state (google.shopping.merchant_lfp_v1beta.types.LfpStore.StoreMatchingState):
             Optional. Output only. The state of matching to a Google
-            Business Profile listing. See
+            Business Profile. See
             [matchingStateHint][google.shopping.merchant.lfp.v1beta.LfpStore.matching_state_hint]
             for further details if no match is found.
         matching_state_hint (str):
             Optional. Output only. The hint of why the matching has
             failed. This is only set when
             [matchingState][google.shopping.merchant.lfp.v1beta.LfpStore.matching_state]=``STORE_MATCHING_STATE_FAILED``.
 
@@ -108,16 +108,15 @@
                Profile store is unverified. Go through the Google
                Business Profile verification process to match correctly.
 
             This field is a member of `oneof`_ ``_matching_state_hint``.
     """
 
     class StoreMatchingState(proto.Enum):
-        r"""The state of matching ``LfpStore`` to a Google Business Profile
-        listing.
+        r"""The state of matching ``LfpStore`` to a Google Business Profile.
 
         Values:
             STORE_MATCHING_STATE_UNSPECIFIED (0):
                 Store matching state unspecified.
             STORE_MATCHING_STATE_MATCHED (1):
                 The ``LfpStore`` is successfully matched with a Google
                 Business Profile store.
```

### Comparing `google-shopping-merchant-lfp-0.1.0/google_shopping_merchant_lfp.egg-info/PKG-INFO` & `google-shopping-merchant-lfp-0.1.1/google_shopping_merchant_lfp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-shopping-merchant-lfp
-Version: 0.1.0
+Version: 0.1.1
 Summary: Google Shopping Merchant Lfp API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-shopping-merchant-lfp
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-shopping-merchant-lfp-0.1.0/google_shopping_merchant_lfp.egg-info/SOURCES.txt` & `google-shopping-merchant-lfp-0.1.1/google_shopping_merchant_lfp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-lfp-0.1.0/setup.py` & `google-shopping-merchant-lfp-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-lfp-0.1.0/tests/__init__.py` & `google-shopping-merchant-lfp-0.1.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-lfp-0.1.0/tests/unit/__init__.py` & `google-shopping-merchant-lfp-0.1.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-lfp-0.1.0/tests/unit/gapic/__init__.py` & `google-shopping-merchant-lfp-0.1.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-lfp-0.1.0/tests/unit/gapic/merchant_lfp_v1beta/__init__.py` & `google-shopping-merchant-lfp-0.1.1/tests/unit/gapic/merchant_lfp_v1beta/__init__.py`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-lfp-0.1.0/tests/unit/gapic/merchant_lfp_v1beta/test_lfp_inventory_service.py` & `google-shopping-merchant-lfp-0.1.1/tests/unit/gapic/merchant_lfp_v1beta/test_lfp_inventory_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1253,14 +1253,17 @@
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.insert_lfp_inventory), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.insert_lfp_inventory()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == lfpinventory.InsertLfpInventoryRequest()
 
 
 def test_insert_lfp_inventory_non_empty_request_with_auto_populated_field():
@@ -1278,22 +1281,64 @@
         parent="parent_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.insert_lfp_inventory), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.insert_lfp_inventory(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == lfpinventory.InsertLfpInventoryRequest(
             parent="parent_value",
         )
 
 
+def test_insert_lfp_inventory_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = LfpInventoryServiceClient(
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
+            client._transport.insert_lfp_inventory in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.insert_lfp_inventory
+        ] = mock_rpc
+        request = {}
+        client.insert_lfp_inventory(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.insert_lfp_inventory(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_insert_lfp_inventory_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = LfpInventoryServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -1323,14 +1368,60 @@
         response = await client.insert_lfp_inventory()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == lfpinventory.InsertLfpInventoryRequest()
 
 
 @pytest.mark.asyncio
+async def test_insert_lfp_inventory_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = LfpInventoryServiceAsyncClient(
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
+            client._client._transport.insert_lfp_inventory
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
+            client._client._transport.insert_lfp_inventory
+        ] = mock_object
+
+        request = {}
+        await client.insert_lfp_inventory(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.insert_lfp_inventory(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_insert_lfp_inventory_async(
     transport: str = "grpc_asyncio", request_type=lfpinventory.InsertLfpInventoryRequest
 ):
     client = LfpInventoryServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
@@ -1595,14 +1686,54 @@
     assert response.availability == "availability_value"
     assert response.quantity == 895
     assert response.pickup_method == "pickup_method_value"
     assert response.pickup_sla == "pickup_sla_value"
     assert response.feed_label == "feed_label_value"
 
 
+def test_insert_lfp_inventory_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = LfpInventoryServiceClient(
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
+            client._transport.insert_lfp_inventory in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.insert_lfp_inventory
+        ] = mock_rpc
+
+        request = {}
+        client.insert_lfp_inventory(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.insert_lfp_inventory(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_insert_lfp_inventory_rest_required_fields(
     request_type=lfpinventory.InsertLfpInventoryRequest,
 ):
     transport_class = transports.LfpInventoryServiceRestTransport
 
     request_init = {}
     request_init["parent"] = ""
```

### Comparing `google-shopping-merchant-lfp-0.1.0/tests/unit/gapic/merchant_lfp_v1beta/test_lfp_sale_service.py` & `google-shopping-merchant-lfp-0.1.1/tests/unit/gapic/merchant_lfp_v1beta/test_lfp_sale_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1181,14 +1181,17 @@
     client = LfpSaleServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.insert_lfp_sale), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.insert_lfp_sale()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == lfpsale.InsertLfpSaleRequest()
 
 
 def test_insert_lfp_sale_non_empty_request_with_auto_populated_field():
@@ -1204,22 +1207,60 @@
     # if they meet the requirements of AIP 4235.
     request = lfpsale.InsertLfpSaleRequest(
         parent="parent_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.insert_lfp_sale), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.insert_lfp_sale(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == lfpsale.InsertLfpSaleRequest(
             parent="parent_value",
         )
 
 
+def test_insert_lfp_sale_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = LfpSaleServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.insert_lfp_sale in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.insert_lfp_sale] = mock_rpc
+        request = {}
+        client.insert_lfp_sale(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.insert_lfp_sale(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_insert_lfp_sale_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = LfpSaleServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -1245,14 +1286,60 @@
         response = await client.insert_lfp_sale()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == lfpsale.InsertLfpSaleRequest()
 
 
 @pytest.mark.asyncio
+async def test_insert_lfp_sale_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = LfpSaleServiceAsyncClient(
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
+            client._client._transport.insert_lfp_sale
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
+            client._client._transport.insert_lfp_sale
+        ] = mock_object
+
+        request = {}
+        await client.insert_lfp_sale(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.insert_lfp_sale(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_insert_lfp_sale_async(
     transport: str = "grpc_asyncio", request_type=lfpsale.InsertLfpSaleRequest
 ):
     client = LfpSaleServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
@@ -1499,14 +1586,50 @@
     assert response.content_language == "content_language_value"
     assert response.gtin == "gtin_value"
     assert response.quantity == 895
     assert response.uid == "uid_value"
     assert response.feed_label == "feed_label_value"
 
 
+def test_insert_lfp_sale_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = LfpSaleServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.insert_lfp_sale in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.insert_lfp_sale] = mock_rpc
+
+        request = {}
+        client.insert_lfp_sale(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.insert_lfp_sale(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_insert_lfp_sale_rest_required_fields(
     request_type=lfpsale.InsertLfpSaleRequest,
 ):
     transport_class = transports.LfpSaleServiceRestTransport
 
     request_init = {}
     request_init["parent"] = ""
```

### Comparing `google-shopping-merchant-lfp-0.1.0/tests/unit/gapic/merchant_lfp_v1beta/test_lfp_store_service.py` & `google-shopping-merchant-lfp-0.1.1/tests/unit/gapic/merchant_lfp_v1beta/test_lfp_store_service.py`

 * *Files 7% similar despite different names*

```diff
@@ -1205,14 +1205,17 @@
     client = LfpStoreServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_lfp_store), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.get_lfp_store()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == lfpstore.GetLfpStoreRequest()
 
 
 def test_get_lfp_store_non_empty_request_with_auto_populated_field():
@@ -1228,22 +1231,60 @@
     # if they meet the requirements of AIP 4235.
     request = lfpstore.GetLfpStoreRequest(
         name="name_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_lfp_store), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.get_lfp_store(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == lfpstore.GetLfpStoreRequest(
             name="name_value",
         )
 
 
+def test_get_lfp_store_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = LfpStoreServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.get_lfp_store in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.get_lfp_store] = mock_rpc
+        request = {}
+        client.get_lfp_store(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.get_lfp_store(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_get_lfp_store_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = LfpStoreServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -1270,14 +1311,60 @@
         response = await client.get_lfp_store()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == lfpstore.GetLfpStoreRequest()
 
 
 @pytest.mark.asyncio
+async def test_get_lfp_store_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = LfpStoreServiceAsyncClient(
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
+            client._client._transport.get_lfp_store
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
+            client._client._transport.get_lfp_store
+        ] = mock_object
+
+        request = {}
+        await client.get_lfp_store(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.get_lfp_store(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_get_lfp_store_async(
     transport: str = "grpc_asyncio", request_type=lfpstore.GetLfpStoreRequest
 ):
     client = LfpStoreServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
@@ -1539,14 +1626,17 @@
     client = LfpStoreServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.insert_lfp_store), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.insert_lfp_store()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == lfpstore.InsertLfpStoreRequest()
 
 
 def test_insert_lfp_store_non_empty_request_with_auto_populated_field():
@@ -1562,22 +1652,62 @@
     # if they meet the requirements of AIP 4235.
     request = lfpstore.InsertLfpStoreRequest(
         parent="parent_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.insert_lfp_store), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.insert_lfp_store(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == lfpstore.InsertLfpStoreRequest(
             parent="parent_value",
         )
 
 
+def test_insert_lfp_store_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = LfpStoreServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.insert_lfp_store in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.insert_lfp_store
+        ] = mock_rpc
+        request = {}
+        client.insert_lfp_store(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.insert_lfp_store(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_insert_lfp_store_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = LfpStoreServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -1604,14 +1734,60 @@
         response = await client.insert_lfp_store()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == lfpstore.InsertLfpStoreRequest()
 
 
 @pytest.mark.asyncio
+async def test_insert_lfp_store_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = LfpStoreServiceAsyncClient(
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
+            client._client._transport.insert_lfp_store
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
+            client._client._transport.insert_lfp_store
+        ] = mock_object
+
+        request = {}
+        await client.insert_lfp_store(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.insert_lfp_store(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_insert_lfp_store_async(
     transport: str = "grpc_asyncio", request_type=lfpstore.InsertLfpStoreRequest
 ):
     client = LfpStoreServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
@@ -1857,14 +2033,17 @@
     client = LfpStoreServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.delete_lfp_store), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.delete_lfp_store()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == lfpstore.DeleteLfpStoreRequest()
 
 
 def test_delete_lfp_store_non_empty_request_with_auto_populated_field():
@@ -1880,22 +2059,62 @@
     # if they meet the requirements of AIP 4235.
     request = lfpstore.DeleteLfpStoreRequest(
         name="name_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.delete_lfp_store), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.delete_lfp_store(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == lfpstore.DeleteLfpStoreRequest(
             name="name_value",
         )
 
 
+def test_delete_lfp_store_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = LfpStoreServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.delete_lfp_store in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.delete_lfp_store
+        ] = mock_rpc
+        request = {}
+        client.delete_lfp_store(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.delete_lfp_store(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_delete_lfp_store_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = LfpStoreServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -1908,14 +2127,60 @@
         response = await client.delete_lfp_store()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == lfpstore.DeleteLfpStoreRequest()
 
 
 @pytest.mark.asyncio
+async def test_delete_lfp_store_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = LfpStoreServiceAsyncClient(
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
+            client._client._transport.delete_lfp_store
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
+            client._client._transport.delete_lfp_store
+        ] = mock_object
+
+        request = {}
+        await client.delete_lfp_store(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.delete_lfp_store(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_delete_lfp_store_async(
     transport: str = "grpc_asyncio", request_type=lfpstore.DeleteLfpStoreRequest
 ):
     client = LfpStoreServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
@@ -2126,14 +2391,17 @@
     client = LfpStoreServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.list_lfp_stores), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.list_lfp_stores()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == lfpstore.ListLfpStoresRequest()
 
 
 def test_list_lfp_stores_non_empty_request_with_auto_populated_field():
@@ -2150,23 +2418,61 @@
     request = lfpstore.ListLfpStoresRequest(
         parent="parent_value",
         page_token="page_token_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.list_lfp_stores), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.list_lfp_stores(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == lfpstore.ListLfpStoresRequest(
             parent="parent_value",
             page_token="page_token_value",
         )
 
 
+def test_list_lfp_stores_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = LfpStoreServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.list_lfp_stores in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.list_lfp_stores] = mock_rpc
+        request = {}
+        client.list_lfp_stores(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.list_lfp_stores(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_list_lfp_stores_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = LfpStoreServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -2183,14 +2489,60 @@
         response = await client.list_lfp_stores()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == lfpstore.ListLfpStoresRequest()
 
 
 @pytest.mark.asyncio
+async def test_list_lfp_stores_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = LfpStoreServiceAsyncClient(
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
+            client._client._transport.list_lfp_stores
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
+            client._client._transport.list_lfp_stores
+        ] = mock_object
+
+        request = {}
+        await client.list_lfp_stores(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.list_lfp_stores(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_list_lfp_stores_async(
     transport: str = "grpc_asyncio", request_type=lfpstore.ListLfpStoresRequest
 ):
     client = LfpStoreServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
@@ -2617,14 +2969,50 @@
     assert (
         response.matching_state
         == lfpstore.LfpStore.StoreMatchingState.STORE_MATCHING_STATE_MATCHED
     )
     assert response.matching_state_hint == "matching_state_hint_value"
 
 
+def test_get_lfp_store_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = LfpStoreServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.get_lfp_store in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.get_lfp_store] = mock_rpc
+
+        request = {}
+        client.get_lfp_store(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.get_lfp_store(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_get_lfp_store_rest_required_fields(request_type=lfpstore.GetLfpStoreRequest):
     transport_class = transports.LfpStoreServiceRestTransport
 
     request_init = {}
     request_init["name"] = ""
     request = request_type(**request_init)
     pb_request = request_type.pb(request)
@@ -2980,14 +3368,52 @@
     assert (
         response.matching_state
         == lfpstore.LfpStore.StoreMatchingState.STORE_MATCHING_STATE_MATCHED
     )
     assert response.matching_state_hint == "matching_state_hint_value"
 
 
+def test_insert_lfp_store_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = LfpStoreServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.insert_lfp_store in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.insert_lfp_store
+        ] = mock_rpc
+
+        request = {}
+        client.insert_lfp_store(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.insert_lfp_store(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_insert_lfp_store_rest_required_fields(
     request_type=lfpstore.InsertLfpStoreRequest,
 ):
     transport_class = transports.LfpStoreServiceRestTransport
 
     request_init = {}
     request_init["parent"] = ""
@@ -3249,14 +3675,52 @@
         req.return_value = response_value
         response = client.delete_lfp_store(request)
 
     # Establish that the response is the type that we expect.
     assert response is None
 
 
+def test_delete_lfp_store_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = LfpStoreServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.delete_lfp_store in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.delete_lfp_store
+        ] = mock_rpc
+
+        request = {}
+        client.delete_lfp_store(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.delete_lfp_store(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_delete_lfp_store_rest_required_fields(
     request_type=lfpstore.DeleteLfpStoreRequest,
 ):
     transport_class = transports.LfpStoreServiceRestTransport
 
     request_init = {}
     request_init["name"] = ""
@@ -3500,14 +3964,50 @@
         response = client.list_lfp_stores(request)
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.ListLfpStoresPager)
     assert response.next_page_token == "next_page_token_value"
 
 
+def test_list_lfp_stores_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = LfpStoreServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.list_lfp_stores in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.list_lfp_stores] = mock_rpc
+
+        request = {}
+        client.list_lfp_stores(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.list_lfp_stores(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_list_lfp_stores_rest_required_fields(
     request_type=lfpstore.ListLfpStoresRequest,
 ):
     transport_class = transports.LfpStoreServiceRestTransport
 
     request_init = {}
     request_init["parent"] = ""
```

