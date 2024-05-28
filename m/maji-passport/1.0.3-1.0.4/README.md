# Comparing `tmp/maji_passport-1.0.3.tar.gz` & `tmp/maji_passport-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maji_passport-1.0.3.tar", last modified: Wed May 22 13:06:34 2024, max compression
+gzip compressed data, was "maji_passport-1.0.4.tar", last modified: Tue May 28 11:38:43 2024, max compression
```

## Comparing `maji_passport-1.0.3.tar` & `maji_passport-1.0.4.tar`

### file list

```diff
@@ -1,52 +1,59 @@
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-22 13:06:34.986937 maji_passport-1.0.3/
--rw-rw-r--   0 teo       (1000) teo       (1000)     1073 2024-05-20 12:56:59.000000 maji_passport-1.0.3/LICENSE
--rw-r--r--   0 teo       (1000) teo       (1000)     3571 2024-05-22 13:06:34.986937 maji_passport-1.0.3/PKG-INFO
--rw-rw-r--   0 teo       (1000) teo       (1000)     2496 2024-05-21 13:19:25.000000 maji_passport-1.0.3/README.md
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-22 13:06:34.982937 maji_passport-1.0.3/maji_passport/
--rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-1.0.3/maji_passport/__init__.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)      406 2024-05-21 10:00:38.000000 maji_passport-1.0.3/maji_passport/admin.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)      246 2024-05-21 10:09:31.000000 maji_passport-1.0.3/maji_passport/apps.py
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-22 13:06:34.982937 maji_passport-1.0.3/maji_passport/authentication/
--rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-1.0.3/maji_passport/authentication/__init__.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     3046 2024-05-21 10:00:38.000000 maji_passport-1.0.3/maji_passport/authentication/backend.py
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-22 13:06:34.982937 maji_passport-1.0.3/maji_passport/migrations/
--rw-rw-r--   0 teo       (1000) teo       (1000)     2234 2024-05-21 10:45:54.000000 maji_passport-1.0.3/maji_passport/migrations/0001_initial.py
--rw-rw-r--   0 teo       (1000) teo       (1000)      526 2024-05-21 10:45:54.000000 maji_passport-1.0.3/maji_passport/migrations/0002_auto_20240418_1355.py
--rw-rw-r--   0 teo       (1000) teo       (1000)      471 2024-05-21 10:45:54.000000 maji_passport-1.0.3/maji_passport/migrations/0003_accesstoken_passport_ac_token_cccee9_hash.py
--rw-rw-r--   0 teo       (1000) teo       (1000)      536 2024-05-21 10:45:54.000000 maji_passport-1.0.3/maji_passport/migrations/0004_alter_accesstoken_passport_user.py
--rw-rw-r--   0 teo       (1000) teo       (1000)      615 2024-05-21 10:47:34.000000 maji_passport-1.0.3/maji_passport/migrations/0005_auto_20240521_1047.py
--rw-rw-r--   0 teo       (1000) teo       (1000)     2480 2024-05-21 12:23:56.000000 maji_passport-1.0.3/maji_passport/migrations/0006_auto_20240521_1118.py
--rw-rw-r--   0 teo       (1000) teo       (1000)      940 2024-05-22 13:04:11.000000 maji_passport-1.0.3/maji_passport/migrations/0007_auto_20240522_1304.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-1.0.3/maji_passport/migrations/__init__.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     2048 2024-05-22 13:03:07.000000 maji_passport-1.0.3/maji_passport/models.py
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-22 13:06:34.982937 maji_passport-1.0.3/maji_passport/serializers/
--rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-1.0.3/maji_passport/serializers/__init__.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     2397 2024-05-06 13:34:14.000000 maji_passport-1.0.3/maji_passport/serializers/exchange.py
--rw-rw-r--   0 teo       (1000) teo       (1000)     1866 2024-05-22 10:26:17.000000 maji_passport-1.0.3/maji_passport/serializers/kafka.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)      519 2024-05-17 08:38:42.000000 maji_passport-1.0.3/maji_passport/serializers/passport.py
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-22 13:06:34.986937 maji_passport-1.0.3/maji_passport/services/
--rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-1.0.3/maji_passport/services/__init__.py
--rw-rw-r--   0 teo       (1000) teo       (1000)     4612 2024-05-22 09:08:55.000000 maji_passport-1.0.3/maji_passport/services/auth.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     7023 2024-05-21 10:00:38.000000 maji_passport-1.0.3/maji_passport/services/exchange.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     2977 2024-05-21 09:04:04.000000 maji_passport-1.0.3/maji_passport/services/kafka.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)      305 2024-05-21 10:00:38.000000 maji_passport-1.0.3/maji_passport/services/passport.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     2880 2024-05-21 08:32:10.000000 maji_passport-1.0.3/maji_passport/services/passport_migrate.py
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-22 13:06:34.986937 maji_passport-1.0.3/maji_passport/tests/
--rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-1.0.3/maji_passport/tests/__init__.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     4010 2024-05-21 10:00:38.000000 maji_passport-1.0.3/maji_passport/tests/test_exchange.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     3026 2024-05-21 10:00:38.000000 maji_passport-1.0.3/maji_passport/tests/test_kafka.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)      940 2024-05-21 10:10:15.000000 maji_passport-1.0.3/maji_passport/urls.py
--rw-rw-r--   0 teo       (1000) teo       (1000)      207 2024-05-21 08:38:01.000000 maji_passport-1.0.3/maji_passport/utils.py
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-22 13:06:34.986937 maji_passport-1.0.3/maji_passport/views/
--rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-17 08:38:42.000000 maji_passport-1.0.3/maji_passport/views/__init__.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     4932 2024-05-22 09:07:59.000000 maji_passport-1.0.3/maji_passport/views/exchange.py
--rwxrwxr-x   0 teo       (1000) teo       (1000)     3753 2024-05-21 10:00:38.000000 maji_passport-1.0.3/maji_passport/views/passport.py
-drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-22 13:06:34.982937 maji_passport-1.0.3/maji_passport.egg-info/
--rw-r--r--   0 teo       (1000) teo       (1000)     3571 2024-05-22 13:06:34.000000 maji_passport-1.0.3/maji_passport.egg-info/PKG-INFO
--rw-rw-r--   0 teo       (1000) teo       (1000)     1441 2024-05-22 13:06:34.000000 maji_passport-1.0.3/maji_passport.egg-info/SOURCES.txt
--rw-rw-r--   0 teo       (1000) teo       (1000)        1 2024-05-22 13:06:34.000000 maji_passport-1.0.3/maji_passport.egg-info/dependency_links.txt
--rw-rw-r--   0 teo       (1000) teo       (1000)      207 2024-05-22 13:06:34.000000 maji_passport-1.0.3/maji_passport.egg-info/requires.txt
--rw-rw-r--   0 teo       (1000) teo       (1000)       14 2024-05-22 13:06:34.000000 maji_passport-1.0.3/maji_passport.egg-info/top_level.txt
--rw-rw-r--   0 teo       (1000) teo       (1000)      668 2024-05-22 13:06:34.000000 maji_passport-1.0.3/pyproject.toml
--rw-rw-r--   0 teo       (1000) teo       (1000)       38 2024-05-22 13:06:34.986937 maji_passport-1.0.3/setup.cfg
--rw-rw-r--   0 teo       (1000) teo       (1000)     1018 2024-05-22 13:06:34.000000 maji_passport-1.0.3/setup.py
+drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-28 11:38:43.812997 maji_passport-1.0.4/
+-rw-rw-r--   0 teo       (1000) teo       (1000)     1073 2024-05-20 12:56:59.000000 maji_passport-1.0.4/LICENSE
+-rw-r--r--   0 teo       (1000) teo       (1000)     3571 2024-05-28 11:38:43.812997 maji_passport-1.0.4/PKG-INFO
+-rw-rw-r--   0 teo       (1000) teo       (1000)     2496 2024-05-28 11:34:56.000000 maji_passport-1.0.4/README.md
+drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-28 11:38:43.808998 maji_passport-1.0.4/maji_passport/
+-rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-27 11:28:06.000000 maji_passport-1.0.4/maji_passport/__init__.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)      406 2024-05-27 11:28:06.000000 maji_passport-1.0.4/maji_passport/admin.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)      246 2024-05-27 11:28:06.000000 maji_passport-1.0.4/maji_passport/apps.py
+drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-28 11:38:43.808998 maji_passport-1.0.4/maji_passport/authentication/
+-rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-27 11:28:06.000000 maji_passport-1.0.4/maji_passport/authentication/__init__.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)     3046 2024-05-27 11:28:06.000000 maji_passport-1.0.4/maji_passport/authentication/backend.py
+drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-28 11:38:43.808998 maji_passport-1.0.4/maji_passport/management/
+-rw-rw-r--   0 teo       (1000) teo       (1000)        0 2024-05-22 13:36:51.000000 maji_passport-1.0.4/maji_passport/management/__init__.py
+drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-28 11:38:43.812997 maji_passport-1.0.4/maji_passport/management/commands/
+-rw-rw-r--   0 teo       (1000) teo       (1000)        0 2024-05-22 13:36:51.000000 maji_passport-1.0.4/maji_passport/management/commands/__init__.py
+-rw-rw-r--   0 teo       (1000) teo       (1000)      537 2024-05-22 13:36:51.000000 maji_passport-1.0.4/maji_passport/management/commands/kafka_consumer.py
+-rw-rw-r--   0 teo       (1000) teo       (1000)      861 2024-05-22 13:36:51.000000 maji_passport-1.0.4/maji_passport/management/commands/kafka_producer_test.py
+-rw-rw-r--   0 teo       (1000) teo       (1000)      236 2024-05-22 13:36:51.000000 maji_passport-1.0.4/maji_passport/management/commands/migrate_all_users_to_passport.py
+drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-28 11:38:43.812997 maji_passport-1.0.4/maji_passport/migrations/
+-rw-rw-r--   0 teo       (1000) teo       (1000)     2234 2024-05-27 11:28:06.000000 maji_passport-1.0.4/maji_passport/migrations/0001_initial.py
+-rw-rw-r--   0 teo       (1000) teo       (1000)      526 2024-05-27 11:28:06.000000 maji_passport-1.0.4/maji_passport/migrations/0002_auto_20240418_1355.py
+-rw-rw-r--   0 teo       (1000) teo       (1000)      471 2024-05-27 11:28:06.000000 maji_passport-1.0.4/maji_passport/migrations/0003_accesstoken_passport_ac_token_cccee9_hash.py
+-rw-rw-r--   0 teo       (1000) teo       (1000)      536 2024-05-27 11:28:06.000000 maji_passport-1.0.4/maji_passport/migrations/0004_alter_accesstoken_passport_user.py
+-rw-rw-r--   0 teo       (1000) teo       (1000)      615 2024-05-27 11:28:06.000000 maji_passport-1.0.4/maji_passport/migrations/0005_auto_20240521_1047.py
+-rw-rw-r--   0 teo       (1000) teo       (1000)     2480 2024-05-27 11:28:06.000000 maji_passport-1.0.4/maji_passport/migrations/0006_auto_20240521_1118.py
+-rw-rw-r--   0 teo       (1000) teo       (1000)      940 2024-05-27 11:28:06.000000 maji_passport-1.0.4/maji_passport/migrations/0007_auto_20240522_1304.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-27 11:28:06.000000 maji_passport-1.0.4/maji_passport/migrations/__init__.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)     2048 2024-05-27 11:28:06.000000 maji_passport-1.0.4/maji_passport/models.py
+drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-28 11:38:43.812997 maji_passport-1.0.4/maji_passport/serializers/
+-rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-27 11:28:06.000000 maji_passport-1.0.4/maji_passport/serializers/__init__.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)     2397 2024-05-27 11:28:06.000000 maji_passport-1.0.4/maji_passport/serializers/exchange.py
+-rw-rw-r--   0 teo       (1000) teo       (1000)     2105 2024-05-28 11:38:05.000000 maji_passport-1.0.4/maji_passport/serializers/kafka.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)      519 2024-05-27 11:28:06.000000 maji_passport-1.0.4/maji_passport/serializers/passport.py
+drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-28 11:38:43.812997 maji_passport-1.0.4/maji_passport/services/
+-rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-27 11:28:06.000000 maji_passport-1.0.4/maji_passport/services/__init__.py
+-rw-rw-r--   0 teo       (1000) teo       (1000)     4612 2024-05-27 11:28:06.000000 maji_passport-1.0.4/maji_passport/services/auth.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)     7023 2024-05-27 11:28:06.000000 maji_passport-1.0.4/maji_passport/services/exchange.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)     6051 2024-05-28 11:38:05.000000 maji_passport-1.0.4/maji_passport/services/kafka.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)      305 2024-05-27 11:28:06.000000 maji_passport-1.0.4/maji_passport/services/passport.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)     2880 2024-05-27 11:28:06.000000 maji_passport-1.0.4/maji_passport/services/passport_migrate.py
+drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-28 11:38:43.812997 maji_passport-1.0.4/maji_passport/tests/
+-rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-27 11:28:06.000000 maji_passport-1.0.4/maji_passport/tests/__init__.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)     4010 2024-05-27 11:28:06.000000 maji_passport-1.0.4/maji_passport/tests/test_exchange.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)     3026 2024-05-27 11:28:06.000000 maji_passport-1.0.4/maji_passport/tests/test_kafka.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)      940 2024-05-27 11:28:06.000000 maji_passport-1.0.4/maji_passport/urls.py
+-rw-rw-r--   0 teo       (1000) teo       (1000)     1504 2024-05-28 11:38:05.000000 maji_passport-1.0.4/maji_passport/utils.py
+drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-28 11:38:43.812997 maji_passport-1.0.4/maji_passport/views/
+-rwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-27 11:28:06.000000 maji_passport-1.0.4/maji_passport/views/__init__.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)     4932 2024-05-27 11:28:06.000000 maji_passport-1.0.4/maji_passport/views/exchange.py
+-rwxrwxr-x   0 teo       (1000) teo       (1000)     3753 2024-05-27 11:28:06.000000 maji_passport-1.0.4/maji_passport/views/passport.py
+drwxrwxr-x   0 teo       (1000) teo       (1000)        0 2024-05-28 11:38:43.808998 maji_passport-1.0.4/maji_passport.egg-info/
+-rw-r--r--   0 teo       (1000) teo       (1000)     3571 2024-05-28 11:38:43.000000 maji_passport-1.0.4/maji_passport.egg-info/PKG-INFO
+-rw-rw-r--   0 teo       (1000) teo       (1000)     1700 2024-05-28 11:38:43.000000 maji_passport-1.0.4/maji_passport.egg-info/SOURCES.txt
+-rw-rw-r--   0 teo       (1000) teo       (1000)        1 2024-05-28 11:38:43.000000 maji_passport-1.0.4/maji_passport.egg-info/dependency_links.txt
+-rw-rw-r--   0 teo       (1000) teo       (1000)      207 2024-05-28 11:38:43.000000 maji_passport-1.0.4/maji_passport.egg-info/requires.txt
+-rw-rw-r--   0 teo       (1000) teo       (1000)       14 2024-05-28 11:38:43.000000 maji_passport-1.0.4/maji_passport.egg-info/top_level.txt
+-rw-rw-r--   0 teo       (1000) teo       (1000)      668 2024-05-28 11:38:40.000000 maji_passport-1.0.4/pyproject.toml
+-rw-rw-r--   0 teo       (1000) teo       (1000)       38 2024-05-28 11:38:43.816997 maji_passport-1.0.4/setup.cfg
+-rw-rw-r--   0 teo       (1000) teo       (1000)     1018 2024-05-28 11:38:40.000000 maji_passport-1.0.4/setup.py
```

### Comparing `maji_passport-1.0.3/LICENSE` & `maji_passport-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.3/PKG-INFO` & `maji_passport-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maji_passport
-Version: 1.0.3
+Version: 1.0.4
 Summary: Maji Passport With custom authorisation
 Home-page: https://passport.maji.la/
 Author: ViktorTeodorih
 Author-email: Viktor Ivanov <viktorteodorihivanov@gmail.com>
 Project-URL: Homepage, https://gitlab.com/argo-media/argo-media-backend-ecosystem/maji-passport-library
 Project-URL: Issues, https://gitlab.com/argo-media/argo-media-backend-ecosystem/maji-passport-library/issues
 Keywords: maji passport python
```

### Comparing `maji_passport-1.0.3/README.md` & `maji_passport-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.3/maji_passport/authentication/backend.py` & `maji_passport-1.0.4/maji_passport/authentication/backend.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.3/maji_passport/migrations/0001_initial.py` & `maji_passport-1.0.4/maji_passport/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.3/maji_passport/migrations/0002_auto_20240418_1355.py` & `maji_passport-1.0.4/maji_passport/migrations/0002_auto_20240418_1355.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.3/maji_passport/migrations/0004_alter_accesstoken_passport_user.py` & `maji_passport-1.0.4/maji_passport/migrations/0004_alter_accesstoken_passport_user.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.3/maji_passport/migrations/0005_auto_20240521_1047.py` & `maji_passport-1.0.4/maji_passport/migrations/0005_auto_20240521_1047.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.3/maji_passport/migrations/0006_auto_20240521_1118.py` & `maji_passport-1.0.4/maji_passport/migrations/0006_auto_20240521_1118.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.3/maji_passport/migrations/0007_auto_20240522_1304.py` & `maji_passport-1.0.4/maji_passport/migrations/0007_auto_20240522_1304.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.3/maji_passport/models.py` & `maji_passport-1.0.4/maji_passport/models.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.3/maji_passport/serializers/exchange.py` & `maji_passport-1.0.4/maji_passport/serializers/exchange.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.3/maji_passport/serializers/kafka.py` & `maji_passport-1.0.4/maji_passport/serializers/kafka.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,44 +1,52 @@
-from django.conf import settings
-from django.contrib.auth import get_user_model
-from rest_framework.fields import BooleanField, CharField
-
+from rest_framework.fields import BooleanField, CharField, JSONField
 from rest_framework.serializers import Serializer
 
-from maji_passport.utils import clear_phone_number
+from maji_passport.utils import clear_phone_number, get_passport_user_serializer
+from maji_passport.models import PassportUser
+from django.contrib.auth import get_user_model
 
+CustomSerializer = get_passport_user_serializer()
 User = get_user_model()
 
-USER_DETAIL_SERIALIZER = settings.USER_DETAIL_SERIALIZER if getattr(settings, "USER_DETAIL_SERIALIZER") else Serializer
+
+class PassportUserDataSerializer(Serializer):
+    avatar_url = CharField(required=False, allow_blank=True, allow_null=True)
+    cover_url = CharField(required=False, allow_blank=True, allow_null=True)
+    display_name = CharField(required=False, allow_blank=True)
+    social_networks = JSONField(required=False)
 
 
-class KafkaUpdateUserSerializer(USER_DETAIL_SERIALIZER):
+class KafkaUpdateUserSerializer(CustomSerializer):
     """
     Serializer for kafka update user messages
 
     phone and is_phone_verified is read_only_fields in ArgoUserDetailsSerializer
     and here we must declare them read_only=False and required=False
     """
+
     phone = CharField(read_only=False, required=False, allow_blank=True)
     is_phone_verified = BooleanField(read_only=False, required=False)
 
+    user_data = PassportUserDataSerializer(required=False)
+
+    class Meta(CustomSerializer.Meta):
+        fields = CustomSerializer.Meta.fields + ("user_data",)
+
     def validate_phone(self, value):
         return clear_phone_number(value)
 
     def update(self, instance, validated_data):
         """
         If we get a phone number in data, this means that the user has changed phone
         in the passport and needs to update it for the current user
         and remove it from other users, who have that phone
         """
         if "phone" in validated_data and validated_data["phone"]:
             old_users = User.objects.filter(phone=validated_data["phone"])
             old_users.update(phone="", is_phone_verified=False)
-        # update avatar from kafka.
-        # otherwise rise errors:
-        # - ValueError: Cannot assign "3743": "User.avatar" must be a "Image" instance
-        # - Incorrect type. Expected pk value, received Image.
-        # if "avatar" in validated_data and validated_data["avatar"]:
-        #     avatar_id = validated_data.pop("avatar")
-        #     avatar = Image.objects.get(id=avatar_id)
-        #     instance.avatar = avatar
+        if "user_data" in validated_data:
+            # update PassportUser data for this user
+            PassportUser.objects.filter(argo_user=instance).update(
+                **validated_data["user_data"]
+            )
         return super().update(instance, validated_data)
```

### Comparing `maji_passport-1.0.3/maji_passport/serializers/passport.py` & `maji_passport-1.0.4/maji_passport/serializers/passport.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.3/maji_passport/services/auth.py` & `maji_passport-1.0.4/maji_passport/services/auth.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.3/maji_passport/services/exchange.py` & `maji_passport-1.0.4/maji_passport/services/exchange.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.3/maji_passport/services/passport_migrate.py` & `maji_passport-1.0.4/maji_passport/services/passport_migrate.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.3/maji_passport/tests/test_exchange.py` & `maji_passport-1.0.4/maji_passport/tests/test_exchange.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.3/maji_passport/tests/test_kafka.py` & `maji_passport-1.0.4/maji_passport/tests/test_kafka.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.3/maji_passport/urls.py` & `maji_passport-1.0.4/maji_passport/urls.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.3/maji_passport/views/exchange.py` & `maji_passport-1.0.4/maji_passport/views/exchange.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.3/maji_passport/views/passport.py` & `maji_passport-1.0.4/maji_passport/views/passport.py`

 * *Files identical despite different names*

### Comparing `maji_passport-1.0.3/maji_passport.egg-info/PKG-INFO` & `maji_passport-1.0.4/maji_passport.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maji-passport
-Version: 1.0.3
+Version: 1.0.4
 Summary: Maji Passport With custom authorisation
 Home-page: https://passport.maji.la/
 Author: ViktorTeodorih
 Author-email: Viktor Ivanov <viktorteodorihivanov@gmail.com>
 Project-URL: Homepage, https://gitlab.com/argo-media/argo-media-backend-ecosystem/maji-passport-library
 Project-URL: Issues, https://gitlab.com/argo-media/argo-media-backend-ecosystem/maji-passport-library/issues
 Keywords: maji passport python
```

### Comparing `maji_passport-1.0.3/maji_passport.egg-info/SOURCES.txt` & `maji_passport-1.0.4/maji_passport.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,19 @@
 maji_passport.egg-info/PKG-INFO
 maji_passport.egg-info/SOURCES.txt
 maji_passport.egg-info/dependency_links.txt
 maji_passport.egg-info/requires.txt
 maji_passport.egg-info/top_level.txt
 maji_passport/authentication/__init__.py
 maji_passport/authentication/backend.py
+maji_passport/management/__init__.py
+maji_passport/management/commands/__init__.py
+maji_passport/management/commands/kafka_consumer.py
+maji_passport/management/commands/kafka_producer_test.py
+maji_passport/management/commands/migrate_all_users_to_passport.py
 maji_passport/migrations/0001_initial.py
 maji_passport/migrations/0002_auto_20240418_1355.py
 maji_passport/migrations/0003_accesstoken_passport_ac_token_cccee9_hash.py
 maji_passport/migrations/0004_alter_accesstoken_passport_user.py
 maji_passport/migrations/0005_auto_20240521_1047.py
 maji_passport/migrations/0006_auto_20240521_1118.py
 maji_passport/migrations/0007_auto_20240522_1304.py
```

### Comparing `maji_passport-1.0.3/pyproject.toml` & `maji_passport-1.0.4/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "maji_passport"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="Viktor Ivanov", email="viktorteodorihivanov@gmail.com" },
 ]
 description = "Maji Passport With custom authorisation"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `maji_passport-1.0.3/setup.py` & `maji_passport-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 
 setup(
   name='maji_passport',
-  version='1.0.3',
+  version='1.0.4',
   author='ViktorTeodorih',
   author_email='viktorteodorihivanov@gmail.com',
   description='Maji Passport With custom authorisation',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://passport.maji.la/',
   packages=find_packages(),
```

