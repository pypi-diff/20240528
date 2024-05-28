# Comparing `tmp/ec_tools-0.9.tar.gz` & `tmp/ec_tools-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ec_tools-0.9.tar", last modified: Wed Nov 25 11:30:24 2020, max compression
+gzip compressed data, was "ec_tools-1.0.tar", last modified: Tue May 28 05:26:34 2024, max compression
```

## Comparing `ec_tools-0.9.tar` & `ec_tools-1.0.tar`

### file list

```diff
@@ -1,28 +1,38 @@
-drwxr-xr-x   0 indestinee   (501) staff       (20)        0 2020-11-25 11:30:24.460495 ec_tools-0.9/
--rw-r--r--   0 indestinee   (501) staff       (20)      367 2020-11-25 11:30:24.460009 ec_tools-0.9/PKG-INFO
--rw-r--r--   0 indestinee   (501) staff       (20)       11 2020-10-20 12:04:11.000000 ec_tools-0.9/README.md
-drwxr-xr-x   0 indestinee   (501) staff       (20)        0 2020-11-25 11:30:24.451479 ec_tools-0.9/ec_tools.egg-info/
--rw-r--r--   0 indestinee   (501) staff       (20)      367 2020-11-25 11:30:24.000000 ec_tools-0.9/ec_tools.egg-info/PKG-INFO
--rw-r--r--   0 indestinee   (501) staff       (20)      577 2020-11-25 11:30:24.000000 ec_tools-0.9/ec_tools.egg-info/SOURCES.txt
--rw-r--r--   0 indestinee   (501) staff       (20)        1 2020-11-25 11:30:24.000000 ec_tools-0.9/ec_tools.egg-info/dependency_links.txt
--rw-r--r--   0 indestinee   (501) staff       (20)        9 2020-11-25 11:30:24.000000 ec_tools-0.9/ec_tools.egg-info/top_level.txt
--rw-r--r--   0 indestinee   (501) staff       (20)       38 2020-11-25 11:30:24.460641 ec_tools-0.9/setup.cfg
--rw-r--r--   0 indestinee   (501) staff       (20)      792 2020-11-25 11:29:06.000000 ec_tools-0.9/setup.py
-drwxr-xr-x   0 indestinee   (501) staff       (20)        0 2020-11-25 11:30:24.447673 ec_tools-0.9/src/
-drwxr-xr-x   0 indestinee   (501) staff       (20)        0 2020-11-25 11:30:24.451967 ec_tools-0.9/src/ec_tools/
--rw-r--r--   0 indestinee   (501) staff       (20)      360 2020-10-20 12:17:05.000000 ec_tools-0.9/src/ec_tools/__init__.py
-drwxr-xr-x   0 indestinee   (501) staff       (20)        0 2020-11-25 11:30:24.454930 ec_tools-0.9/src/ec_tools/basic_tools/
--rw-r--r--   0 indestinee   (501) staff       (20)      549 2020-10-20 12:06:17.000000 ec_tools-0.9/src/ec_tools/basic_tools/__init__.py
--rw-r--r--   0 indestinee   (501) staff       (20)     2389 2020-10-28 14:29:22.000000 ec_tools-0.9/src/ec_tools/basic_tools/colorful_log.py
--rw-r--r--   0 indestinee   (501) staff       (20)     1676 2020-10-20 12:17:05.000000 ec_tools-0.9/src/ec_tools/basic_tools/colorful_str.py
--rw-r--r--   0 indestinee   (501) staff       (20)      757 2020-10-20 12:17:05.000000 ec_tools-0.9/src/ec_tools/basic_tools/procedure.py
--rw-r--r--   0 indestinee   (501) staff       (20)      540 2020-10-20 12:04:59.000000 ec_tools-0.9/src/ec_tools/basic_tools/replace_dict.py
-drwxr-xr-x   0 indestinee   (501) staff       (20)        0 2020-11-25 11:30:24.457908 ec_tools-0.9/src/ec_tools/database/
--rw-r--r--   0 indestinee   (501) staff       (20)       50 2020-10-28 14:29:22.000000 ec_tools-0.9/src/ec_tools/database/__init__.py
--rw-r--r--   0 indestinee   (501) staff       (20)      267 2020-10-28 14:17:45.000000 ec_tools-0.9/src/ec_tools/database/database_client.py
--rw-r--r--   0 indestinee   (501) staff       (20)     2253 2020-11-25 11:28:52.000000 ec_tools-0.9/src/ec_tools/database/sqlite_client.py
--rw-r--r--   0 indestinee   (501) staff       (20)      804 2020-10-28 14:29:22.000000 ec_tools-0.9/src/ec_tools/database/utils.py
-drwxr-xr-x   0 indestinee   (501) staff       (20)        0 2020-11-25 11:30:24.458455 ec_tools-0.9/src/ec_tools/image/
--rw-r--r--   0 indestinee   (501) staff       (20)      289 2020-10-20 12:17:05.000000 ec_tools-0.9/src/ec_tools/image/__init__.py
-drwxr-xr-x   0 indestinee   (501) staff       (20)        0 2020-11-25 11:30:24.459059 ec_tools-0.9/src/ec_tools/spider/
--rw-r--r--   0 indestinee   (501) staff       (20)      242 2020-10-20 12:17:05.000000 ec_tools-0.9/src/ec_tools/spider/__init__.py
+drwxr-xr-x   0 yaolin_chen   (501) staff       (20)        0 2024-05-28 05:26:34.615160 ec_tools-1.0/
+-rw-r--r--   0 yaolin_chen   (501) staff       (20)      190 2024-05-28 05:26:34.615014 ec_tools-1.0/PKG-INFO
+-rw-r--r--   0 yaolin_chen   (501) staff       (20)       11 2024-05-28 02:16:50.000000 ec_tools-1.0/README.md
+drwxr-xr-x   0 yaolin_chen   (501) staff       (20)        0 2024-05-28 05:26:34.600948 ec_tools-1.0/ec_tools/
+-rw-r--r--   0 yaolin_chen   (501) staff       (20)        0 2024-05-28 02:52:24.000000 ec_tools-1.0/ec_tools/__init__.py
+drwxr-xr-x   0 yaolin_chen   (501) staff       (20)        0 2024-05-28 05:26:34.602329 ec_tools-1.0/ec_tools/database/
+-rwxr-xr-x   0 yaolin_chen   (501) staff       (20)      663 2024-05-28 02:25:28.000000 ec_tools-1.0/ec_tools/database/__init__.py
+drwxr-xr-x   0 yaolin_chen   (501) staff       (20)        0 2024-05-28 05:26:34.603493 ec_tools-1.0/ec_tools/database/kv_dao/
+-rwxr-xr-x   0 yaolin_chen   (501) staff       (20)        0 2023-10-07 05:06:22.000000 ec_tools-1.0/ec_tools/database/kv_dao/__init__.py
+-rwxr-xr-x   0 yaolin_chen   (501) staff       (20)      939 2024-05-28 05:07:00.000000 ec_tools-1.0/ec_tools/database/kv_dao/kv_dao.py
+-rwxr-xr-x   0 yaolin_chen   (501) staff       (20)      430 2024-05-28 03:11:49.000000 ec_tools-1.0/ec_tools/database/kv_dao/kv_data.py
+-rwxr-xr-x   0 yaolin_chen   (501) staff       (20)     1376 2024-05-28 04:01:35.000000 ec_tools-1.0/ec_tools/database/kv_dao/sqlite_kv_dao.py
+drwxr-xr-x   0 yaolin_chen   (501) staff       (20)        0 2024-05-28 05:26:34.607726 ec_tools-1.0/ec_tools/database/sqlite_client/
+-rwxr-xr-x   0 yaolin_chen   (501) staff       (20)        0 2023-10-07 05:06:22.000000 ec_tools-1.0/ec_tools/database/sqlite_client/__init__.py
+-rwxr-xr-x   0 yaolin_chen   (501) staff       (20)     1683 2024-05-28 03:08:07.000000 ec_tools-1.0/ec_tools/database/sqlite_client/sqlite_client.py
+-rwxr-xr-x   0 yaolin_chen   (501) staff       (20)      535 2023-10-07 05:06:22.000000 ec_tools-1.0/ec_tools/database/sqlite_client/sqlite_query.py
+drwxr-xr-x   0 yaolin_chen   (501) staff       (20)        0 2024-05-28 05:26:34.611723 ec_tools-1.0/ec_tools/database/sqlite_dao/
+-rwxr-xr-x   0 yaolin_chen   (501) staff       (20)        0 2023-10-07 05:06:22.000000 ec_tools-1.0/ec_tools/database/sqlite_dao/__init__.py
+-rwxr-xr-x   0 yaolin_chen   (501) staff       (20)     3107 2024-05-28 04:03:22.000000 ec_tools-1.0/ec_tools/database/sqlite_dao/sqlite_dao.py
+-rwxr-xr-x   0 yaolin_chen   (501) staff       (20)     2767 2024-05-28 05:07:00.000000 ec_tools-1.0/ec_tools/database/sqlite_dao/sqlite_data_object.py
+-rwxr-xr-x   0 yaolin_chen   (501) staff       (20)     5248 2024-05-28 03:09:18.000000 ec_tools-1.0/ec_tools/database/sqlite_dao/sqlite_query_generator.py
+drwxr-xr-x   0 yaolin_chen   (501) staff       (20)        0 2024-05-28 05:26:34.612518 ec_tools-1.0/ec_tools/database/utils/
+-rw-r--r--   0 yaolin_chen   (501) staff       (20)        0 2023-10-07 05:06:22.000000 ec_tools-1.0/ec_tools/database/utils/__init__.py
+-rw-r--r--   0 yaolin_chen   (501) staff       (20)      943 2024-05-28 03:09:18.000000 ec_tools-1.0/ec_tools/database/utils/dataclass_utils.py
+drwxr-xr-x   0 yaolin_chen   (501) staff       (20)        0 2024-05-28 05:26:34.614688 ec_tools-1.0/ec_tools/utils/
+-rw-r--r--   0 yaolin_chen   (501) staff       (20)       85 2024-05-28 02:52:24.000000 ec_tools-1.0/ec_tools/utils/__init__.py
+-rw-r--r--   0 yaolin_chen   (501) staff       (20)      593 2024-05-28 04:03:22.000000 ec_tools-1.0/ec_tools/utils/io_utils.py
+-rw-r--r--   0 yaolin_chen   (501) staff       (20)     1054 2024-05-28 03:07:26.000000 ec_tools-1.0/ec_tools/utils/misc.py
+-rw-r--r--   0 yaolin_chen   (501) staff       (20)      471 2024-05-28 02:31:52.000000 ec_tools-1.0/ec_tools/utils/os_utils.py
+-rw-r--r--   0 yaolin_chen   (501) staff       (20)     1507 2024-05-28 03:07:26.000000 ec_tools-1.0/ec_tools/utils/thread_pool.py
+drwxr-xr-x   0 yaolin_chen   (501) staff       (20)        0 2024-05-28 05:26:34.602140 ec_tools-1.0/ec_tools.egg-info/
+-rw-r--r--   0 yaolin_chen   (501) staff       (20)      190 2024-05-28 05:26:34.000000 ec_tools-1.0/ec_tools.egg-info/PKG-INFO
+-rw-r--r--   0 yaolin_chen   (501) staff       (20)      922 2024-05-28 05:26:34.000000 ec_tools-1.0/ec_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 yaolin_chen   (501) staff       (20)        1 2024-05-28 05:26:34.000000 ec_tools-1.0/ec_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 yaolin_chen   (501) staff       (20)       19 2024-05-28 05:26:34.000000 ec_tools-1.0/ec_tools.egg-info/requires.txt
+-rw-r--r--   0 yaolin_chen   (501) staff       (20)        9 2024-05-28 05:26:34.000000 ec_tools-1.0/ec_tools.egg-info/top_level.txt
+-rw-r--r--   0 yaolin_chen   (501) staff       (20)       38 2024-05-28 05:26:34.615216 ec_tools-1.0/setup.cfg
+-rw-r--r--   0 yaolin_chen   (501) staff       (20)      375 2024-05-28 05:18:17.000000 ec_tools-1.0/setup.py
```

