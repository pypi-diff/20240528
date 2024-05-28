# Comparing `tmp/smsapi-client-2.9.4.tar.gz` & `tmp/smsapi-client-2.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smsapi-client-2.9.4.tar", last modified: Mon Oct  9 11:52:22 2023, max compression
+gzip compressed data, was "smsapi-client-2.9.5.tar", last modified: Tue Oct 10 15:43:15 2023, max compression
```

## Comparing `smsapi-client-2.9.4.tar` & `smsapi-client-2.9.5.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxr-x   0 ash       (1000) ash       (1000)        0 2023-10-09 11:52:22.498038 smsapi-client-2.9.4/
--rw-rw-r--   0 ash       (1000) ash       (1000)      542 2021-03-10 08:56:24.000000 smsapi-client-2.9.4/LICENSE
--rw-rw-r--   0 ash       (1000) ash       (1000)       46 2021-03-10 08:56:24.000000 smsapi-client-2.9.4/MANIFEST.in
--rw-rw-r--   0 ash       (1000) ash       (1000)     3234 2023-10-09 11:52:22.498038 smsapi-client-2.9.4/PKG-INFO
--rw-rw-r--   0 ash       (1000) ash       (1000)     1734 2021-03-10 08:56:24.000000 smsapi-client-2.9.4/README.md
--rw-rw-r--   0 ash       (1000) ash       (1000)       67 2023-10-09 11:52:22.498038 smsapi-client-2.9.4/setup.cfg
--rw-rw-r--   0 ash       (1000) ash       (1000)     1116 2021-03-10 08:56:24.000000 smsapi-client-2.9.4/setup.py
-drwxrwxr-x   0 ash       (1000) ash       (1000)        0 2023-10-09 11:52:22.498038 smsapi-client-2.9.4/smsapi/
--rw-rw-r--   0 ash       (1000) ash       (1000)       79 2023-10-09 11:51:33.000000 smsapi-client-2.9.4/smsapi/__init__.py
-drwxrwxr-x   0 ash       (1000) ash       (1000)        0 2023-10-09 11:52:22.498038 smsapi-client-2.9.4/smsapi/account/
--rw-rw-r--   0 ash       (1000) ash       (1000)        0 2021-03-10 08:56:24.000000 smsapi-client-2.9.4/smsapi/account/__init__.py
--rw-rw-r--   0 ash       (1000) ash       (1000)     2365 2023-10-09 10:59:04.000000 smsapi-client-2.9.4/smsapi/account/api.py
--rw-rw-r--   0 ash       (1000) ash       (1000)     1321 2021-03-10 08:56:24.000000 smsapi-client-2.9.4/smsapi/account/models.py
--rw-rw-r--   0 ash       (1000) ash       (1000)      152 2021-03-10 08:56:24.000000 smsapi-client-2.9.4/smsapi/api.py
--rw-rw-r--   0 ash       (1000) ash       (1000)      450 2021-03-10 08:56:24.000000 smsapi-client-2.9.4/smsapi/auth.py
-drwxrwxr-x   0 ash       (1000) ash       (1000)        0 2023-10-09 11:52:22.498038 smsapi-client-2.9.4/smsapi/blacklist/
--rw-rw-r--   0 ash       (1000) ash       (1000)        0 2021-03-10 08:56:24.000000 smsapi-client-2.9.4/smsapi/blacklist/__init__.py
--rw-rw-r--   0 ash       (1000) ash       (1000)     1166 2021-03-10 08:56:24.000000 smsapi-client-2.9.4/smsapi/blacklist/api.py
--rw-rw-r--   0 ash       (1000) ash       (1000)      618 2021-03-10 08:56:24.000000 smsapi-client-2.9.4/smsapi/blacklist/models.py
--rw-rw-r--   0 ash       (1000) ash       (1000)     1904 2023-10-09 11:51:33.000000 smsapi-client-2.9.4/smsapi/client.py
--rw-rw-r--   0 ash       (1000) ash       (1000)      254 2021-03-10 08:56:24.000000 smsapi-client-2.9.4/smsapi/compat.py
-drwxrwxr-x   0 ash       (1000) ash       (1000)        0 2023-10-09 11:52:22.498038 smsapi-client-2.9.4/smsapi/contacts/
--rw-rw-r--   0 ash       (1000) ash       (1000)        0 2021-03-10 08:56:24.000000 smsapi-client-2.9.4/smsapi/contacts/__init__.py
--rw-rw-r--   0 ash       (1000) ash       (1000)     6938 2023-09-20 12:18:34.000000 smsapi-client-2.9.4/smsapi/contacts/api.py
--rw-rw-r--   0 ash       (1000) ash       (1000)      676 2021-03-10 08:56:24.000000 smsapi-client-2.9.4/smsapi/contacts/exceptions.py
--rw-rw-r--   0 ash       (1000) ash       (1000)     2585 2021-03-10 08:56:24.000000 smsapi-client-2.9.4/smsapi/contacts/models.py
--rw-rw-r--   0 ash       (1000) ash       (1000)     3997 2023-01-24 09:29:24.000000 smsapi-client-2.9.4/smsapi/endpoint.py
--rw-rw-r--   0 ash       (1000) ash       (1000)     1720 2021-03-11 08:35:01.000000 smsapi-client-2.9.4/smsapi/exception.py
-drwxrwxr-x   0 ash       (1000) ash       (1000)        0 2023-10-09 11:52:22.498038 smsapi-client-2.9.4/smsapi/hlr/
--rw-rw-r--   0 ash       (1000) ash       (1000)        0 2021-03-10 08:56:24.000000 smsapi-client-2.9.4/smsapi/hlr/__init__.py
--rw-rw-r--   0 ash       (1000) ash       (1000)      933 2023-10-09 10:25:18.000000 smsapi-client-2.9.4/smsapi/hlr/api.py
-drwxrwxr-x   0 ash       (1000) ash       (1000)        0 2023-10-09 11:52:22.498038 smsapi-client-2.9.4/smsapi/mfa/
--rw-rw-r--   0 ash       (1000) ash       (1000)        0 2023-09-18 11:14:24.000000 smsapi-client-2.9.4/smsapi/mfa/__init__.py
--rw-rw-r--   0 ash       (1000) ash       (1000)     1279 2023-09-18 11:14:24.000000 smsapi-client-2.9.4/smsapi/mfa/api.py
--rw-rw-r--   0 ash       (1000) ash       (1000)      997 2023-09-18 11:14:24.000000 smsapi-client-2.9.4/smsapi/mfa/model.py
-drwxrwxr-x   0 ash       (1000) ash       (1000)        0 2023-10-09 11:52:22.498038 smsapi-client-2.9.4/smsapi/mms/
--rw-rw-r--   0 ash       (1000) ash       (1000)        0 2021-03-10 08:56:24.000000 smsapi-client-2.9.4/smsapi/mms/__init__.py
--rw-rw-r--   0 ash       (1000) ash       (1000)     1775 2023-10-09 10:26:24.000000 smsapi-client-2.9.4/smsapi/mms/api.py
--rw-rw-r--   0 ash       (1000) ash       (1000)     3864 2021-03-10 08:56:24.000000 smsapi-client-2.9.4/smsapi/models.py
-drwxrwxr-x   0 ash       (1000) ash       (1000)        0 2023-10-09 11:52:22.498038 smsapi-client-2.9.4/smsapi/sender/
--rw-rw-r--   0 ash       (1000) ash       (1000)        0 2021-03-10 08:56:24.000000 smsapi-client-2.9.4/smsapi/sender/__init__.py
--rw-rw-r--   0 ash       (1000) ash       (1000)     2098 2023-10-09 10:37:53.000000 smsapi-client-2.9.4/smsapi/sender/api.py
--rw-rw-r--   0 ash       (1000) ash       (1000)      487 2021-03-10 08:56:24.000000 smsapi-client-2.9.4/smsapi/sender/models.py
-drwxrwxr-x   0 ash       (1000) ash       (1000)        0 2023-10-09 11:52:22.498038 smsapi-client-2.9.4/smsapi/short_url/
--rw-rw-r--   0 ash       (1000) ash       (1000)        0 2021-03-10 08:56:24.000000 smsapi-client-2.9.4/smsapi/short_url/__init__.py
--rw-rw-r--   0 ash       (1000) ash       (1000)     2727 2023-01-24 09:27:41.000000 smsapi-client-2.9.4/smsapi/short_url/api.py
--rw-rw-r--   0 ash       (1000) ash       (1000)     2249 2021-03-10 08:56:24.000000 smsapi-client-2.9.4/smsapi/short_url/models.py
-drwxrwxr-x   0 ash       (1000) ash       (1000)        0 2023-10-09 11:52:22.498038 smsapi-client-2.9.4/smsapi/sms/
--rw-rw-r--   0 ash       (1000) ash       (1000)      104 2021-03-10 08:56:24.000000 smsapi-client-2.9.4/smsapi/sms/__init__.py
--rw-rw-r--   0 ash       (1000) ash       (1000)     3053 2023-10-09 10:17:33.000000 smsapi-client-2.9.4/smsapi/sms/api.py
--rw-rw-r--   0 ash       (1000) ash       (1000)      809 2023-09-18 11:14:24.000000 smsapi-client-2.9.4/smsapi/sms/model.py
--rw-rw-r--   0 ash       (1000) ash       (1000)     2262 2021-03-10 08:56:24.000000 smsapi-client-2.9.4/smsapi/utils.py
-drwxrwxr-x   0 ash       (1000) ash       (1000)        0 2023-10-09 11:52:22.498038 smsapi-client-2.9.4/smsapi/vms/
--rw-rw-r--   0 ash       (1000) ash       (1000)        0 2021-03-10 08:56:24.000000 smsapi-client-2.9.4/smsapi/vms/__init__.py
--rw-rw-r--   0 ash       (1000) ash       (1000)     2088 2023-10-09 10:36:16.000000 smsapi-client-2.9.4/smsapi/vms/api.py
-drwxrwxr-x   0 ash       (1000) ash       (1000)        0 2023-10-09 11:52:22.498038 smsapi-client-2.9.4/smsapi_client.egg-info/
--rw-rw-r--   0 ash       (1000) ash       (1000)     3234 2023-10-09 11:52:22.000000 smsapi-client-2.9.4/smsapi_client.egg-info/PKG-INFO
--rw-rw-r--   0 ash       (1000) ash       (1000)     1043 2023-10-09 11:52:22.000000 smsapi-client-2.9.4/smsapi_client.egg-info/SOURCES.txt
--rw-rw-r--   0 ash       (1000) ash       (1000)        1 2023-10-09 11:52:22.000000 smsapi-client-2.9.4/smsapi_client.egg-info/dependency_links.txt
--rw-rw-r--   0 ash       (1000) ash       (1000)        9 2023-10-09 11:52:22.000000 smsapi-client-2.9.4/smsapi_client.egg-info/requires.txt
--rw-rw-r--   0 ash       (1000) ash       (1000)        7 2023-10-09 11:52:22.000000 smsapi-client-2.9.4/smsapi_client.egg-info/top_level.txt
+drwxrwxr-x   0 ash       (1000) ash       (1000)        0 2023-10-10 15:43:15.546187 smsapi-client-2.9.5/
+-rw-rw-r--   0 ash       (1000) ash       (1000)      542 2021-03-10 08:56:24.000000 smsapi-client-2.9.5/LICENSE
+-rw-rw-r--   0 ash       (1000) ash       (1000)       46 2021-03-10 08:56:24.000000 smsapi-client-2.9.5/MANIFEST.in
+-rw-rw-r--   0 ash       (1000) ash       (1000)     3234 2023-10-10 15:43:15.546187 smsapi-client-2.9.5/PKG-INFO
+-rw-rw-r--   0 ash       (1000) ash       (1000)     1734 2021-03-10 08:56:24.000000 smsapi-client-2.9.5/README.md
+-rw-rw-r--   0 ash       (1000) ash       (1000)       67 2023-10-10 15:43:15.550187 smsapi-client-2.9.5/setup.cfg
+-rw-rw-r--   0 ash       (1000) ash       (1000)     1116 2021-03-10 08:56:24.000000 smsapi-client-2.9.5/setup.py
+drwxrwxr-x   0 ash       (1000) ash       (1000)        0 2023-10-10 15:43:15.542188 smsapi-client-2.9.5/smsapi/
+-rw-rw-r--   0 ash       (1000) ash       (1000)       79 2023-10-10 15:31:04.000000 smsapi-client-2.9.5/smsapi/__init__.py
+drwxrwxr-x   0 ash       (1000) ash       (1000)        0 2023-10-10 15:43:15.542188 smsapi-client-2.9.5/smsapi/account/
+-rw-rw-r--   0 ash       (1000) ash       (1000)        0 2021-03-10 08:56:24.000000 smsapi-client-2.9.5/smsapi/account/__init__.py
+-rw-rw-r--   0 ash       (1000) ash       (1000)     2383 2023-10-10 15:25:42.000000 smsapi-client-2.9.5/smsapi/account/api.py
+-rw-rw-r--   0 ash       (1000) ash       (1000)     1321 2021-03-10 08:56:24.000000 smsapi-client-2.9.5/smsapi/account/models.py
+-rw-rw-r--   0 ash       (1000) ash       (1000)      152 2021-03-10 08:56:24.000000 smsapi-client-2.9.5/smsapi/api.py
+-rw-rw-r--   0 ash       (1000) ash       (1000)      450 2021-03-10 08:56:24.000000 smsapi-client-2.9.5/smsapi/auth.py
+drwxrwxr-x   0 ash       (1000) ash       (1000)        0 2023-10-10 15:43:15.542188 smsapi-client-2.9.5/smsapi/blacklist/
+-rw-rw-r--   0 ash       (1000) ash       (1000)        0 2021-03-10 08:56:24.000000 smsapi-client-2.9.5/smsapi/blacklist/__init__.py
+-rw-rw-r--   0 ash       (1000) ash       (1000)     1166 2021-03-10 08:56:24.000000 smsapi-client-2.9.5/smsapi/blacklist/api.py
+-rw-rw-r--   0 ash       (1000) ash       (1000)      618 2021-03-10 08:56:24.000000 smsapi-client-2.9.5/smsapi/blacklist/models.py
+-rw-rw-r--   0 ash       (1000) ash       (1000)     1904 2023-10-10 15:38:46.000000 smsapi-client-2.9.5/smsapi/client.py
+-rw-rw-r--   0 ash       (1000) ash       (1000)      254 2021-03-10 08:56:24.000000 smsapi-client-2.9.5/smsapi/compat.py
+drwxrwxr-x   0 ash       (1000) ash       (1000)        0 2023-10-10 15:43:15.546187 smsapi-client-2.9.5/smsapi/contacts/
+-rw-rw-r--   0 ash       (1000) ash       (1000)        0 2021-03-10 08:56:24.000000 smsapi-client-2.9.5/smsapi/contacts/__init__.py
+-rw-rw-r--   0 ash       (1000) ash       (1000)     6938 2023-09-20 12:18:34.000000 smsapi-client-2.9.5/smsapi/contacts/api.py
+-rw-rw-r--   0 ash       (1000) ash       (1000)      676 2021-03-10 08:56:24.000000 smsapi-client-2.9.5/smsapi/contacts/exceptions.py
+-rw-rw-r--   0 ash       (1000) ash       (1000)     2585 2021-03-10 08:56:24.000000 smsapi-client-2.9.5/smsapi/contacts/models.py
+-rw-rw-r--   0 ash       (1000) ash       (1000)     3997 2023-01-24 09:29:24.000000 smsapi-client-2.9.5/smsapi/endpoint.py
+-rw-rw-r--   0 ash       (1000) ash       (1000)     1720 2021-03-11 08:35:01.000000 smsapi-client-2.9.5/smsapi/exception.py
+drwxrwxr-x   0 ash       (1000) ash       (1000)        0 2023-10-10 15:43:15.546187 smsapi-client-2.9.5/smsapi/hlr/
+-rw-rw-r--   0 ash       (1000) ash       (1000)        0 2021-03-10 08:56:24.000000 smsapi-client-2.9.5/smsapi/hlr/__init__.py
+-rw-rw-r--   0 ash       (1000) ash       (1000)      933 2023-10-09 10:25:18.000000 smsapi-client-2.9.5/smsapi/hlr/api.py
+drwxrwxr-x   0 ash       (1000) ash       (1000)        0 2023-10-10 15:43:15.546187 smsapi-client-2.9.5/smsapi/mfa/
+-rw-rw-r--   0 ash       (1000) ash       (1000)        0 2023-09-18 11:14:24.000000 smsapi-client-2.9.5/smsapi/mfa/__init__.py
+-rw-rw-r--   0 ash       (1000) ash       (1000)     1279 2023-09-18 11:14:24.000000 smsapi-client-2.9.5/smsapi/mfa/api.py
+-rw-rw-r--   0 ash       (1000) ash       (1000)      997 2023-09-18 11:14:24.000000 smsapi-client-2.9.5/smsapi/mfa/model.py
+drwxrwxr-x   0 ash       (1000) ash       (1000)        0 2023-10-10 15:43:15.546187 smsapi-client-2.9.5/smsapi/mms/
+-rw-rw-r--   0 ash       (1000) ash       (1000)        0 2021-03-10 08:56:24.000000 smsapi-client-2.9.5/smsapi/mms/__init__.py
+-rw-rw-r--   0 ash       (1000) ash       (1000)     1775 2023-10-09 10:26:24.000000 smsapi-client-2.9.5/smsapi/mms/api.py
+-rw-rw-r--   0 ash       (1000) ash       (1000)     3864 2021-03-10 08:56:24.000000 smsapi-client-2.9.5/smsapi/models.py
+drwxrwxr-x   0 ash       (1000) ash       (1000)        0 2023-10-10 15:43:15.546187 smsapi-client-2.9.5/smsapi/sender/
+-rw-rw-r--   0 ash       (1000) ash       (1000)        0 2021-03-10 08:56:24.000000 smsapi-client-2.9.5/smsapi/sender/__init__.py
+-rw-rw-r--   0 ash       (1000) ash       (1000)     2073 2023-10-10 13:20:43.000000 smsapi-client-2.9.5/smsapi/sender/api.py
+-rw-rw-r--   0 ash       (1000) ash       (1000)      487 2021-03-10 08:56:24.000000 smsapi-client-2.9.5/smsapi/sender/models.py
+drwxrwxr-x   0 ash       (1000) ash       (1000)        0 2023-10-10 15:43:15.546187 smsapi-client-2.9.5/smsapi/short_url/
+-rw-rw-r--   0 ash       (1000) ash       (1000)        0 2021-03-10 08:56:24.000000 smsapi-client-2.9.5/smsapi/short_url/__init__.py
+-rw-rw-r--   0 ash       (1000) ash       (1000)     2727 2023-01-24 09:27:41.000000 smsapi-client-2.9.5/smsapi/short_url/api.py
+-rw-rw-r--   0 ash       (1000) ash       (1000)     2249 2021-03-10 08:56:24.000000 smsapi-client-2.9.5/smsapi/short_url/models.py
+drwxrwxr-x   0 ash       (1000) ash       (1000)        0 2023-10-10 15:43:15.546187 smsapi-client-2.9.5/smsapi/sms/
+-rw-rw-r--   0 ash       (1000) ash       (1000)      104 2021-03-10 08:56:24.000000 smsapi-client-2.9.5/smsapi/sms/__init__.py
+-rw-rw-r--   0 ash       (1000) ash       (1000)     3053 2023-10-09 10:17:33.000000 smsapi-client-2.9.5/smsapi/sms/api.py
+-rw-rw-r--   0 ash       (1000) ash       (1000)      809 2023-09-18 11:14:24.000000 smsapi-client-2.9.5/smsapi/sms/model.py
+-rw-rw-r--   0 ash       (1000) ash       (1000)     2262 2021-03-10 08:56:24.000000 smsapi-client-2.9.5/smsapi/utils.py
+drwxrwxr-x   0 ash       (1000) ash       (1000)        0 2023-10-10 15:43:15.546187 smsapi-client-2.9.5/smsapi/vms/
+-rw-rw-r--   0 ash       (1000) ash       (1000)        0 2021-03-10 08:56:24.000000 smsapi-client-2.9.5/smsapi/vms/__init__.py
+-rw-rw-r--   0 ash       (1000) ash       (1000)     2088 2023-10-09 10:36:16.000000 smsapi-client-2.9.5/smsapi/vms/api.py
+drwxrwxr-x   0 ash       (1000) ash       (1000)        0 2023-10-10 15:43:15.546187 smsapi-client-2.9.5/smsapi_client.egg-info/
+-rw-rw-r--   0 ash       (1000) ash       (1000)     3234 2023-10-10 15:43:15.000000 smsapi-client-2.9.5/smsapi_client.egg-info/PKG-INFO
+-rw-rw-r--   0 ash       (1000) ash       (1000)     1043 2023-10-10 15:43:15.000000 smsapi-client-2.9.5/smsapi_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 ash       (1000) ash       (1000)        1 2023-10-10 15:43:15.000000 smsapi-client-2.9.5/smsapi_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 ash       (1000) ash       (1000)        9 2023-10-10 15:43:15.000000 smsapi-client-2.9.5/smsapi_client.egg-info/requires.txt
+-rw-rw-r--   0 ash       (1000) ash       (1000)        7 2023-10-10 15:43:15.000000 smsapi-client-2.9.5/smsapi_client.egg-info/top_level.txt
```

### Comparing `smsapi-client-2.9.4/LICENSE` & `smsapi-client-2.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `smsapi-client-2.9.4/PKG-INFO` & `smsapi-client-2.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smsapi-client
-Version: 2.9.4
+Version: 2.9.5
 Summary: SmsAPI client
 Home-page: https://github.com/smsapi/smsapi-python-client
 Author: SMSAPI
 Author-email: bok@smsapi.pl
 License: UNKNOWN
 Description: ﻿# smsapi-python
```

### Comparing `smsapi-client-2.9.4/README.md` & `smsapi-client-2.9.5/README.md`

 * *Files identical despite different names*

### Comparing `smsapi-client-2.9.4/setup.py` & `smsapi-client-2.9.5/setup.py`

 * *Files identical despite different names*

### Comparing `smsapi-client-2.9.4/smsapi/account/api.py` & `smsapi-client-2.9.5/smsapi/account/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         exception_class=EndpointException
     )
 
     user = bind_api_endpoint(
         method='GET',
         path=path,
         mapping=UserResult,
-        accept_parameters=['name'],
+        accept_parameters=['without_prefix', 'name'],
         force_parameters=response_format_param,
         exception_class=EndpointException,
         parameters_transformer=parameters_transformer({'name': 'get_user'})
     )
 
     create_user = bind_api_endpoint(
         method='POST',
```

### Comparing `smsapi-client-2.9.4/smsapi/account/models.py` & `smsapi-client-2.9.5/smsapi/account/models.py`

 * *Files identical despite different names*

### Comparing `smsapi-client-2.9.4/smsapi/blacklist/api.py` & `smsapi-client-2.9.5/smsapi/blacklist/api.py`

 * *Files identical despite different names*

### Comparing `smsapi-client-2.9.4/smsapi/blacklist/models.py` & `smsapi-client-2.9.5/smsapi/blacklist/models.py`

 * *Files identical despite different names*

### Comparing `smsapi-client-2.9.4/smsapi/client.py` & `smsapi-client-2.9.5/smsapi/client.py`

 * *Files identical despite different names*

### Comparing `smsapi-client-2.9.4/smsapi/contacts/api.py` & `smsapi-client-2.9.5/smsapi/contacts/api.py`

 * *Files identical despite different names*

### Comparing `smsapi-client-2.9.4/smsapi/contacts/exceptions.py` & `smsapi-client-2.9.5/smsapi/contacts/exceptions.py`

 * *Files identical despite different names*

### Comparing `smsapi-client-2.9.4/smsapi/contacts/models.py` & `smsapi-client-2.9.5/smsapi/contacts/models.py`

 * *Files identical despite different names*

### Comparing `smsapi-client-2.9.4/smsapi/endpoint.py` & `smsapi-client-2.9.5/smsapi/endpoint.py`

 * *Files identical despite different names*

### Comparing `smsapi-client-2.9.4/smsapi/exception.py` & `smsapi-client-2.9.5/smsapi/exception.py`

 * *Files identical despite different names*

### Comparing `smsapi-client-2.9.4/smsapi/hlr/api.py` & `smsapi-client-2.9.5/smsapi/hlr/api.py`

 * *Files identical despite different names*

### Comparing `smsapi-client-2.9.4/smsapi/mfa/api.py` & `smsapi-client-2.9.5/smsapi/mfa/api.py`

 * *Files identical despite different names*

### Comparing `smsapi-client-2.9.4/smsapi/mfa/model.py` & `smsapi-client-2.9.5/smsapi/mfa/model.py`

 * *Files identical despite different names*

### Comparing `smsapi-client-2.9.4/smsapi/mms/api.py` & `smsapi-client-2.9.5/smsapi/mms/api.py`

 * *Files identical despite different names*

### Comparing `smsapi-client-2.9.4/smsapi/models.py` & `smsapi-client-2.9.5/smsapi/models.py`

 * *Files identical despite different names*

### Comparing `smsapi-client-2.9.4/smsapi/sender/api.py` & `smsapi-client-2.9.5/smsapi/sender/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 from smsapi.api import Api
 from smsapi.endpoint import bind_api_endpoint
 from smsapi.exception import EndpointException
 from smsapi.models import ResultCollection
 from smsapi.sms import response_format_param
 from smsapi.utils import update_dict
 from smsapi.sender.models import SenderNameResult, SenderNameSuccessResult
```

### Comparing `smsapi-client-2.9.4/smsapi/short_url/api.py` & `smsapi-client-2.9.5/smsapi/short_url/api.py`

 * *Files identical despite different names*

### Comparing `smsapi-client-2.9.4/smsapi/short_url/models.py` & `smsapi-client-2.9.5/smsapi/short_url/models.py`

 * *Files identical despite different names*

### Comparing `smsapi-client-2.9.4/smsapi/sms/api.py` & `smsapi-client-2.9.5/smsapi/sms/api.py`

 * *Files identical despite different names*

### Comparing `smsapi-client-2.9.4/smsapi/sms/model.py` & `smsapi-client-2.9.5/smsapi/sms/model.py`

 * *Files identical despite different names*

### Comparing `smsapi-client-2.9.4/smsapi/utils.py` & `smsapi-client-2.9.5/smsapi/utils.py`

 * *Files identical despite different names*

### Comparing `smsapi-client-2.9.4/smsapi/vms/api.py` & `smsapi-client-2.9.5/smsapi/vms/api.py`

 * *Files identical despite different names*

### Comparing `smsapi-client-2.9.4/smsapi_client.egg-info/PKG-INFO` & `smsapi-client-2.9.5/smsapi_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smsapi-client
-Version: 2.9.4
+Version: 2.9.5
 Summary: SmsAPI client
 Home-page: https://github.com/smsapi/smsapi-python-client
 Author: SMSAPI
 Author-email: bok@smsapi.pl
 License: UNKNOWN
 Description: ﻿# smsapi-python
```

### Comparing `smsapi-client-2.9.4/smsapi_client.egg-info/SOURCES.txt` & `smsapi-client-2.9.5/smsapi_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

