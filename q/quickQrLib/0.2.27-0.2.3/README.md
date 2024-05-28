# Comparing `tmp/quickQrLib-0.2.27.tar.gz` & `tmp/quickQrLib-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickQrLib-0.2.27.tar", last modified: Tue May 28 13:30:44 2024, max compression
+gzip compressed data, was "quickQrLib-0.2.3.tar", last modified: Mon May 27 16:06:03 2024, max compression
```

## Comparing `quickQrLib-0.2.27.tar` & `quickQrLib-0.2.3.tar`

### file list

```diff
@@ -1,32 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 13:30:44.119470 quickQrLib-0.2.27/
--rw-rw-rw-   0        0        0     1092 2024-05-27 14:41:13.000000 quickQrLib-0.2.27/LICENSE
--rw-rw-rw-   0        0        0       81 2024-05-28 13:30:44.113534 quickQrLib-0.2.27/PKG-INFO
--rw-rw-rw-   0        0        0      183 2024-05-27 15:15:15.000000 quickQrLib-0.2.27/README.md
-drwxrwxrwx   0        0        0        0 2024-05-28 13:30:43.922856 quickQrLib-0.2.27/quickQrLib/
--rw-rw-rw-   0        0        0        0 2024-05-27 14:37:12.000000 quickQrLib-0.2.27/quickQrLib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-28 13:30:44.042423 quickQrLib-0.2.27/quickQrLib/auth_util/
--rw-rw-rw-   0        0        0        0 2024-05-27 14:37:12.000000 quickQrLib-0.2.27/quickQrLib/auth_util/__init__.py
--rw-rw-rw-   0        0        0      893 2024-05-27 15:27:15.000000 quickQrLib-0.2.27/quickQrLib/auth_util/authenticate_jwt.py
-drwxrwxrwx   0        0        0        0 2024-05-28 13:30:44.047146 quickQrLib-0.2.27/quickQrLib/permissions_util/
--rw-rw-rw-   0        0        0        0 2024-05-27 14:37:12.000000 quickQrLib-0.2.27/quickQrLib/permissions_util/__init__.py
--rw-rw-rw-   0        0        0     4264 2024-05-27 17:09:11.000000 quickQrLib-0.2.27/quickQrLib/permissions_util/permissions_helper.py
-drwxrwxrwx   0        0        0        0 2024-05-28 13:30:44.053278 quickQrLib-0.2.27/quickQrLib/s3_util/
--rw-rw-rw-   0        0        0        0 2024-05-27 14:37:12.000000 quickQrLib-0.2.27/quickQrLib/s3_util/__init__.py
--rw-rw-rw-   0        0        0     2770 2024-05-27 20:06:17.000000 quickQrLib-0.2.27/quickQrLib/s3_util/s3_storage_util.py
-drwxrwxrwx   0        0        0        0 2024-05-28 13:30:44.074233 quickQrLib-0.2.27/quickQrLib/signature_util/
--rw-rw-rw-   0        0        0        0 2024-05-28 13:30:33.000000 quickQrLib-0.2.27/quickQrLib/signature_util/__init__.py
--rw-rw-rw-   0        0        0     3260 2024-05-27 20:44:59.000000 quickQrLib-0.2.27/quickQrLib/signature_util/signatures.py
-drwxrwxrwx   0        0        0        0 2024-05-28 13:30:44.077242 quickQrLib-0.2.27/quickQrLib/test_folder_util/
--rw-rw-rw-   0        0        0        0 2024-05-27 14:37:12.000000 quickQrLib-0.2.27/quickQrLib/test_folder_util/__init__.py
--rw-rw-rw-   0        0        0       33 2024-05-27 16:01:30.000000 quickQrLib-0.2.27/quickQrLib/test_folder_util/test.py
-drwxrwxrwx   0        0        0        0 2024-05-28 13:30:44.110025 quickQrLib-0.2.27/quickQrLib/time_util/
--rw-rw-rw-   0        0        0        0 2024-05-27 14:37:12.000000 quickQrLib-0.2.27/quickQrLib/time_util/__init__.py
--rw-rw-rw-   0        0        0     1239 2024-05-27 20:41:49.000000 quickQrLib-0.2.27/quickQrLib/time_util/date_time_helpers.py
-drwxrwxrwx   0        0        0        0 2024-05-28 13:30:44.013164 quickQrLib-0.2.27/quickQrLib.egg-info/
--rw-rw-rw-   0        0        0       81 2024-05-28 13:30:43.000000 quickQrLib-0.2.27/quickQrLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      680 2024-05-28 13:30:43.000000 quickQrLib-0.2.27/quickQrLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 13:30:43.000000 quickQrLib-0.2.27/quickQrLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       97 2024-05-28 13:30:43.000000 quickQrLib-0.2.27/quickQrLib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-28 13:30:43.000000 quickQrLib-0.2.27/quickQrLib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-28 13:30:44.120966 quickQrLib-0.2.27/setup.cfg
--rw-rw-rw-   0        0        0      348 2024-05-28 13:30:40.000000 quickQrLib-0.2.27/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 16:06:03.153874 quickQrLib-0.2.3/
+-rw-rw-rw-   0        0        0     1092 2024-05-27 14:41:13.000000 quickQrLib-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0       80 2024-05-27 16:06:03.150865 quickQrLib-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0      183 2024-05-27 15:15:15.000000 quickQrLib-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 16:06:02.894496 quickQrLib-0.2.3/quickQrLib/
+-rw-rw-rw-   0        0        0        0 2024-05-27 14:37:12.000000 quickQrLib-0.2.3/quickQrLib/__init__.py
+-rw-rw-rw-   0        0        0      893 2024-05-27 15:54:12.000000 quickQrLib-0.2.3/quickQrLib/qr_auth_util.py
+-rw-rw-rw-   0        0        0      104 2024-05-27 16:01:43.000000 quickQrLib-0.2.3/quickQrLib/test_util.py
+-rw-rw-rw-   0        0        0        0 2024-05-27 15:54:26.000000 quickQrLib-0.2.3/quickQrLib/time_util.py
+drwxrwxrwx   0        0        0        0 2024-05-27 16:06:03.144201 quickQrLib-0.2.3/quickQrLib.egg-info/
+-rw-rw-rw-   0        0        0       80 2024-05-27 16:06:02.000000 quickQrLib-0.2.3/quickQrLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2024-05-27 16:06:02.000000 quickQrLib-0.2.3/quickQrLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 16:06:02.000000 quickQrLib-0.2.3/quickQrLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2024-05-27 16:06:02.000000 quickQrLib-0.2.3/quickQrLib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-27 16:06:02.000000 quickQrLib-0.2.3/quickQrLib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 16:06:03.154828 quickQrLib-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      272 2024-05-27 16:05:56.000000 quickQrLib-0.2.3/setup.py
```

### Comparing `quickQrLib-0.2.27/LICENSE` & `quickQrLib-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `quickQrLib-0.2.27/quickQrLib/auth_util/authenticate_jwt.py` & `quickQrLib-0.2.3/quickQrLib/qr_auth_util.py`

 * *Files identical despite different names*

