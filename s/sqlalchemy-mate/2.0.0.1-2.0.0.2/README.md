# Comparing `tmp/sqlalchemy_mate-2.0.0.1.tar.gz` & `tmp/sqlalchemy_mate-2.0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_mate-2.0.0.1.tar", last modified: Fri May 17 06:10:33 2024, max compression
+gzip compressed data, was "sqlalchemy_mate-2.0.0.2.tar", last modified: Tue May 28 18:09:24 2024, max compression
```

## Comparing `sqlalchemy_mate-2.0.0.1.tar` & `sqlalchemy_mate-2.0.0.2.tar`

### file list

```diff
@@ -1,73 +1,82 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-17 06:10:33.674117 sqlalchemy_mate-2.0.0.1/
--rw-r--r--   0 sanhehu    (501) staff       (20)      670 2024-05-14 20:23:38.000000 sqlalchemy_mate-2.0.0.1/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1126 2024-05-14 20:23:38.000000 sqlalchemy_mate-2.0.0.1/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      356 2024-05-14 20:23:38.000000 sqlalchemy_mate-2.0.0.1/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)    11696 2024-05-17 06:10:33.673886 sqlalchemy_mate-2.0.0.1/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     9700 2024-05-17 05:49:58.000000 sqlalchemy_mate-2.0.0.1/README.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     8742 2024-05-17 06:07:09.000000 sqlalchemy_mate-2.0.0.1/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      102 2024-05-14 20:23:38.000000 sqlalchemy_mate-2.0.0.1/requirements-automation.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      390 2024-05-14 20:30:28.000000 sqlalchemy_mate-2.0.0.1/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      871 2024-05-14 20:26:57.000000 sqlalchemy_mate-2.0.0.1/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      128 2024-05-14 20:23:38.000000 sqlalchemy_mate-2.0.0.1/requirements-furo-sphinx-search.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      214 2024-05-14 20:27:06.000000 sqlalchemy_mate-2.0.0.1/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       51 2024-05-14 20:57:38.000000 sqlalchemy_mate-2.0.0.1/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2024-05-17 06:10:33.674164 sqlalchemy_mate-2.0.0.1/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7479 2024-05-15 05:55:50.000000 sqlalchemy_mate-2.0.0.1/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-17 06:10:33.663241 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/
--rw-r--r--   0 sanhehu    (501) staff       (20)      258 2024-05-16 13:04:55.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      100 2024-05-17 06:07:22.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      578 2024-05-17 04:57:05.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/api.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-17 06:10:33.666418 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/crud/
--rw-r--r--   0 sanhehu    (501) staff       (20)       85 2024-05-14 20:22:31.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/crud/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      343 2024-05-15 05:07:50.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/crud/deleting.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       58 2024-05-16 12:56:47.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/crud/deleting_api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3332 2024-05-15 04:37:22.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/crud/inserting.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       61 2024-05-16 12:57:04.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/crud/inserting_api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     6145 2024-05-15 05:01:17.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/crud/selecting.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      403 2024-05-16 12:57:55.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/crud/selecting_api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3686 2024-05-15 05:07:15.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/crud/updating.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       91 2024-05-16 12:57:34.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/crud/updating_api.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-17 06:10:33.666847 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2024-05-14 20:22:31.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    14141 2024-05-14 20:22:31.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/engine_creator.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2173 2024-05-14 21:20:06.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/io.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       80 2024-05-16 13:00:32.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/io_api.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-17 06:10:33.667611 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/orm/
--rw-r--r--   0 sanhehu    (501) staff       (20)       50 2024-05-14 20:22:31.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/orm/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       77 2024-05-16 12:59:27.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/orm/api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    20444 2024-05-15 05:18:28.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/orm/extended_declarative_base.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      642 2024-05-14 20:23:38.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/paths.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-17 06:10:33.668084 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/patterns/
--rw-r--r--   0 sanhehu    (501) staff       (20)        0 2024-05-15 18:33:49.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/patterns/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       75 2024-05-17 04:56:43.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/patterns/api.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-17 06:10:33.669360 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/patterns/status_tracker/
--rw-r--r--   0 sanhehu    (501) staff       (20)      357 2024-05-16 06:33:00.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/patterns/status_tracker/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      145 2024-05-16 14:11:16.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/patterns/status_tracker/api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    15137 2024-05-17 06:04:38.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/patterns/status_tracker/impl.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     5917 2024-05-15 04:01:42.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/pt.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      261 2024-05-16 13:21:05.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/pt_api.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-17 06:10:33.670457 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/types/
--rw-r--r--   0 sanhehu    (501) staff       (20)       24 2024-05-16 13:02:00.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/types/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      192 2024-05-16 13:02:02.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/types/api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1931 2024-05-14 20:22:31.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/types/compressed.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2565 2024-05-14 20:22:31.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/types/compressed_json.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2453 2024-05-14 20:22:31.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/types/json_serializable.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3487 2024-05-16 13:02:42.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/utils.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-17 06:10:33.670842 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/vendor/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2024-05-14 20:23:38.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/vendor/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2024-05-14 20:23:38.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/vendor/pytest_cov_helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-17 06:10:33.671242 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/vendor/timeout_decorator/
--rw-r--r--   0 sanhehu    (501) staff       (20)      162 2024-05-14 20:22:31.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/vendor/timeout_decorator/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     6411 2024-05-14 20:22:31.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/vendor/timeout_decorator/timeout_decorator.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-17 06:10:33.672763 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)    11696 2024-05-17 06:10:33.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     1825 2024-05-17 06:10:33.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2024-05-17 06:10:33.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      291 2024-05-17 06:10:33.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       16 2024-05-17 06:10:33.000000 sqlalchemy_mate-2.0.0.1/sqlalchemy_mate.egg-info/top_level.txt
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-17 06:10:33.672495 sqlalchemy_mate-2.0.0.1/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)     1276 2024-05-17 06:05:50.000000 sqlalchemy_mate-2.0.0.1/tests/test_api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3197 2024-05-16 12:45:12.000000 sqlalchemy_mate-2.0.0.1/tests/test_engine_creator.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1353 2024-05-16 12:45:55.000000 sqlalchemy_mate-2.0.0.1/tests/test_io.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     6071 2024-05-16 13:20:05.000000 sqlalchemy_mate-2.0.0.1/tests/test_pt.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1603 2024-05-16 13:20:23.000000 sqlalchemy_mate-2.0.0.1/tests/test_utils.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-28 18:09:24.681766 sqlalchemy_mate-2.0.0.2/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      670 2024-05-14 20:23:38.000000 sqlalchemy_mate-2.0.0.2/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1126 2024-05-14 20:23:38.000000 sqlalchemy_mate-2.0.0.2/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      356 2024-05-14 20:23:38.000000 sqlalchemy_mate-2.0.0.2/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)    11888 2024-05-28 18:09:24.681530 sqlalchemy_mate-2.0.0.2/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     9700 2024-05-17 05:49:58.000000 sqlalchemy_mate-2.0.0.2/README.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)    10485 2024-05-28 18:09:12.000000 sqlalchemy_mate-2.0.0.2/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      102 2024-05-14 20:23:38.000000 sqlalchemy_mate-2.0.0.2/requirements-automation.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      390 2024-05-14 20:30:28.000000 sqlalchemy_mate-2.0.0.2/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      871 2024-05-14 20:26:57.000000 sqlalchemy_mate-2.0.0.2/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      128 2024-05-14 20:23:38.000000 sqlalchemy_mate-2.0.0.2/requirements-furo-sphinx-search.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      307 2024-05-28 17:30:23.000000 sqlalchemy_mate-2.0.0.2/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       51 2024-05-14 20:57:38.000000 sqlalchemy_mate-2.0.0.2/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2024-05-28 18:09:24.681816 sqlalchemy_mate-2.0.0.2/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7479 2024-05-15 05:55:50.000000 sqlalchemy_mate-2.0.0.2/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-28 18:09:24.670893 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      258 2024-05-16 13:04:55.000000 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      100 2024-05-28 17:30:23.000000 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      578 2024-05-17 04:57:05.000000 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-28 18:09:24.673909 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/crud/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       85 2024-05-14 20:22:31.000000 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/crud/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      343 2024-05-15 05:07:50.000000 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/crud/deleting.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       58 2024-05-16 12:56:47.000000 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/crud/deleting_api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3332 2024-05-15 04:37:22.000000 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/crud/inserting.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       61 2024-05-16 12:57:04.000000 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/crud/inserting_api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     6139 2024-05-28 17:30:23.000000 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/crud/selecting.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      403 2024-05-16 12:57:55.000000 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/crud/selecting_api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3686 2024-05-15 05:07:15.000000 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/crud/updating.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       91 2024-05-16 12:57:34.000000 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/crud/updating_api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-28 18:09:24.674191 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2024-05-14 20:22:31.000000 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    14141 2024-05-14 20:22:31.000000 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/engine_creator.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2173 2024-05-14 21:20:06.000000 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/io.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       80 2024-05-16 13:00:32.000000 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/io_api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-28 18:09:24.675178 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/orm/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       50 2024-05-14 20:22:31.000000 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/orm/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       77 2024-05-16 12:59:27.000000 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/orm/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    20551 2024-05-28 17:30:23.000000 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/orm/extended_declarative_base.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      642 2024-05-14 20:23:38.000000 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/paths.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-28 18:09:24.675469 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/patterns/
+-rw-r--r--   0 sanhehu    (501) staff       (20)        0 2024-05-15 18:33:49.000000 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/patterns/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      135 2024-05-28 17:30:23.000000 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/patterns/api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-28 18:09:24.676381 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/patterns/large_binary_column/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      949 2024-05-28 17:30:23.000000 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/patterns/large_binary_column/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2024-05-28 17:30:23.000000 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/patterns/large_binary_column/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    12659 2024-05-28 17:30:23.000000 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/patterns/large_binary_column/aws_s3.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      350 2024-05-28 17:30:23.000000 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/patterns/large_binary_column/aws_s3_api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1793 2024-05-28 17:30:23.000000 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/patterns/large_binary_column/helpers.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5505 2024-05-28 17:30:23.000000 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/patterns/large_binary_column/local.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      350 2024-05-28 17:30:23.000000 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/patterns/large_binary_column/local_api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-28 18:09:24.676909 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/patterns/status_tracker/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      357 2024-05-16 06:33:00.000000 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/patterns/status_tracker/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      145 2024-05-16 14:11:16.000000 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/patterns/status_tracker/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    15137 2024-05-17 06:04:38.000000 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/patterns/status_tracker/impl.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5917 2024-05-15 04:01:42.000000 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/pt.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      261 2024-05-16 13:21:05.000000 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/pt_api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-28 18:09:24.677934 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/types/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       24 2024-05-16 13:02:00.000000 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/types/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      192 2024-05-16 13:02:02.000000 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/types/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1931 2024-05-14 20:22:31.000000 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/types/compressed.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2565 2024-05-14 20:22:31.000000 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/types/compressed_json.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2453 2024-05-14 20:22:31.000000 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/types/json_serializable.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3487 2024-05-16 13:02:42.000000 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/utils.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-28 18:09:24.678439 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2024-05-14 20:23:38.000000 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    13696 2024-05-28 17:30:23.000000 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/vendor/iterable.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2024-05-14 20:23:38.000000 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/vendor/pytest_cov_helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-28 18:09:24.678787 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/vendor/timeout_decorator/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      162 2024-05-14 20:22:31.000000 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/vendor/timeout_decorator/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     6411 2024-05-14 20:22:31.000000 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/vendor/timeout_decorator/timeout_decorator.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-28 18:09:24.680153 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)    11888 2024-05-28 18:09:24.000000 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2251 2024-05-28 18:09:24.000000 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2024-05-28 18:09:24.000000 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      384 2024-05-28 18:09:24.000000 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       16 2024-05-28 18:09:24.000000 sqlalchemy_mate-2.0.0.2/sqlalchemy_mate.egg-info/top_level.txt
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2024-05-28 18:09:24.679900 sqlalchemy_mate-2.0.0.2/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2444 2024-05-28 18:09:12.000000 sqlalchemy_mate-2.0.0.2/tests/test_api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3197 2024-05-16 12:45:12.000000 sqlalchemy_mate-2.0.0.2/tests/test_engine_creator.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1353 2024-05-16 12:45:55.000000 sqlalchemy_mate-2.0.0.2/tests/test_io.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     6071 2024-05-16 13:20:05.000000 sqlalchemy_mate-2.0.0.2/tests/test_pt.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1603 2024-05-16 13:20:23.000000 sqlalchemy_mate-2.0.0.2/tests/test_utils.py
```

### Comparing `sqlalchemy_mate-2.0.0.1/AUTHORS.rst` & `sqlalchemy_mate-2.0.0.2/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mate-2.0.0.1/LICENSE.txt` & `sqlalchemy_mate-2.0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mate-2.0.0.1/PKG-INFO` & `sqlalchemy_mate-2.0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: sqlalchemy_mate
-Version: 2.0.0.1
+Version: 2.0.0.2
 Summary: A library extend sqlalchemy module, makes CRUD easier.
 Home-page: https://github.com/MacHu-GWU/sqlalchemy_mate-project
-Download-URL: https://pypi.python.org/pypi/sqlalchemy_mate/2.0.0.1#downloads
+Download-URL: https://pypi.python.org/pypi/sqlalchemy_mate/2.0.0.2#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
@@ -32,15 +32,18 @@
 Requires-Dist: prettytable<4.0.0,>=3.0.0
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-cov; extra == "tests"
 Requires-Dist: pg8000; extra == "tests"
 Requires-Dist: attrs; extra == "tests"
 Requires-Dist: superjson; extra == "tests"
-Requires-Dist: pandas; extra == "tests"
+Requires-Dist: pandas<3.0.0,>=2.0.0; extra == "tests"
+Requires-Dist: moto<5.0.0,>=4.1.12; extra == "tests"
+Requires-Dist: boto_session_manager<2.0.0,>=1.7.2; extra == "tests"
+Requires-Dist: s3pathlib<3.0.0,>=2.1.2; extra == "tests"
 Provides-Extra: docs
 Requires-Dist: Sphinx==5.3.0; extra == "docs"
 Requires-Dist: sphinx-jinja==2.0.2; extra == "docs"
 Requires-Dist: sphinx-copybutton==0.5.1; extra == "docs"
 Requires-Dist: sphinx-design==0.5.0; extra == "docs"
 Requires-Dist: furo==2023.03.27; extra == "docs"
 Requires-Dist: nbsphinx==0.8.12; extra == "docs"
```

### Comparing `sqlalchemy_mate-2.0.0.1/README.rst` & `sqlalchemy_mate-2.0.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mate-2.0.0.1/release-history.rst` & `sqlalchemy_mate-2.0.0.2/release-history.rst`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,42 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+2.0.0.2 (2024-05-28)
+------------------------------------------------------------------------------
+**Features and Improvements**
+
+- Add "Large binary column" pattern, support local file and Amazon S3 backend.
+- Add the following public API
+    - ``sqlalchemy_mate.api.patterns.large_binary_column.aws_s3``
+    - ``sqlalchemy_mate.api.patterns.large_binary_column.aws_s3.PutS3BackedColumnResult``
+    - ``sqlalchemy_mate.api.patterns.large_binary_column.aws_s3.put_s3backed_column``
+    - ``sqlalchemy_mate.api.patterns.large_binary_column.aws_s3.clean_up_created_s3_object_when_create_or_update_row_failed``
+    - ``sqlalchemy_mate.api.patterns.large_binary_column.aws_s3.clean_up_old_s3_object_when_update_row_succeeded``
+    - ``sqlalchemy_mate.api.patterns.large_binary_column.aws_s3.PutS3ApiCall``
+    - ``sqlalchemy_mate.api.patterns.large_binary_column.aws_s3.PutS3Result``
+    - ``sqlalchemy_mate.api.patterns.large_binary_column.aws_s3.put_s3``
+    - ``sqlalchemy_mate.api.patterns.large_binary_column.local``
+    - ``sqlalchemy_mate.api.patterns.large_binary_column.local.WriteFileBackedColumnResult``
+    - ``sqlalchemy_mate.api.patterns.large_binary_column.local.write_file_backed_column``
+    - ``sqlalchemy_mate.api.patterns.large_binary_column.local.clean_up_new_file_when_create_or_update_row_failed``
+    - ``sqlalchemy_mate.api.patterns.large_binary_column.local.clean_up_old_file_when_update_row_succeeded``
+    - ``sqlalchemy_mate.api.patterns.large_binary_column.local.WriteFileApiCall``
+    - ``sqlalchemy_mate.api.patterns.large_binary_column.local.WriteFileResult``
+    - ``sqlalchemy_mate.api.patterns.large_binary_column.local.write_file``
+
+**Minor Improvements**
+
+- Use jupyter notebook to generate documentation.
+
+
 2.0.0.1 (2024-05-17)
 ------------------------------------------------------------------------------
 **💥Breaking Change**
 
 - Rework the public API import. Now you have to use ``import sqlalchemy_mate.api as sam`` to access the public API. ``from sqlalchemy_mate import ...`` is no longer working. Here's the full list of public API:
     - ``sqlalchemy_mate.api.selecting.count_row``
     - ``sqlalchemy_mate.api.selecting.by_pk``
```

### Comparing `sqlalchemy_mate-2.0.0.1/requirements-doc.txt` & `sqlalchemy_mate-2.0.0.2/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mate-2.0.0.1/setup.py` & `sqlalchemy_mate-2.0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/api.py` & `sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/api.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/crud/inserting.py` & `sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/crud/inserting.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/crud/selecting.py` & `sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/crud/selecting.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,17 +72,16 @@
             for column, value in zip(table.primary_key, id_):
                 where_args.append(column == value)
             stmt = sa.select(table).where(sa.and_(*where_args))
             return connection.execute(stmt).fetchone()
         else:
             if len(table.primary_key) != 1:
                 raise ValueError
-            return connection.execute(
-                sa.select(table).where(list(table.primary_key)[0] == id_)
-            ).fetchone()
+            stmt = sa.select(table).where(list(table.primary_key)[0] == id_)
+            return connection.execute(stmt).fetchone()
 
 
 def select_all(
     engine: sa.Engine,
     table: sa.Table,
 ) -> sa.Result:
     """
```

### Comparing `sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/crud/updating.py` & `sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/crud/updating.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/engine_creator.py` & `sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/engine_creator.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/io.py` & `sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/io.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/orm/extended_declarative_base.py` & `sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/orm/extended_declarative_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from typing import Union, List, Tuple, Dict, Any
 from collections import OrderedDict
 from copy import deepcopy
 
 from sqlalchemy import inspect, func, text, select, update, Column
 from sqlalchemy.sql.expression import TextClause
 from sqlalchemy.engine import Engine
-from sqlalchemy.orm import declarative_base, Session, InstrumentedAttribute
+from sqlalchemy.orm import declarative_base, Session, InstrumentedAttribute, MappedColumn
 from sqlalchemy.exc import IntegrityError
 from sqlalchemy.orm.exc import FlushError
 
 from ..utils import (
     ensure_exact_one_arg_is_not_none, ensure_list, grouper_list,
     ensure_session, clean_session,
 )
@@ -221,14 +221,16 @@
     @classmethod
     def _major_attrs(cls):
         if cls._cache_major_attrs is None:
             l = list()
             for item in cls._settings_major_attrs:
                 if isinstance(item, Column):
                     l.append(item.name)
+                elif isinstance(item, MappedColumn):
+                    l.append(item.name)
                 elif isinstance(item, str):
                     l.append(item)
                 else:  # pragma: no cover
                     raise TypeError
             if len(set(l)) != len(l):  # pragma: no cover
                 raise ValueError
             cls._cache_major_attrs = tuple(l)
```

### Comparing `sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/paths.py` & `sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/paths.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/patterns/status_tracker/impl.py` & `sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/patterns/status_tracker/impl.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/pt.py` & `sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/pt.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/types/compressed.py` & `sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/types/compressed.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/types/compressed_json.py` & `sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/types/compressed_json.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/types/json_serializable.py` & `sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/types/json_serializable.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/utils.py` & `sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/utils.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/vendor/pytest_cov_helper.py` & `sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/vendor/pytest_cov_helper.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mate-2.0.0.1/sqlalchemy_mate/vendor/timeout_decorator/timeout_decorator.py` & `sqlalchemy_mate-2.0.0.2/sqlalchemy_mate/vendor/timeout_decorator/timeout_decorator.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mate-2.0.0.1/sqlalchemy_mate.egg-info/PKG-INFO` & `sqlalchemy_mate-2.0.0.2/sqlalchemy_mate.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: sqlalchemy_mate
-Version: 2.0.0.1
+Version: 2.0.0.2
 Summary: A library extend sqlalchemy module, makes CRUD easier.
 Home-page: https://github.com/MacHu-GWU/sqlalchemy_mate-project
-Download-URL: https://pypi.python.org/pypi/sqlalchemy_mate/2.0.0.1#downloads
+Download-URL: https://pypi.python.org/pypi/sqlalchemy_mate/2.0.0.2#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
@@ -32,15 +32,18 @@
 Requires-Dist: prettytable<4.0.0,>=3.0.0
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-cov; extra == "tests"
 Requires-Dist: pg8000; extra == "tests"
 Requires-Dist: attrs; extra == "tests"
 Requires-Dist: superjson; extra == "tests"
-Requires-Dist: pandas; extra == "tests"
+Requires-Dist: pandas<3.0.0,>=2.0.0; extra == "tests"
+Requires-Dist: moto<5.0.0,>=4.1.12; extra == "tests"
+Requires-Dist: boto_session_manager<2.0.0,>=1.7.2; extra == "tests"
+Requires-Dist: s3pathlib<3.0.0,>=2.1.2; extra == "tests"
 Provides-Extra: docs
 Requires-Dist: Sphinx==5.3.0; extra == "docs"
 Requires-Dist: sphinx-jinja==2.0.2; extra == "docs"
 Requires-Dist: sphinx-copybutton==0.5.1; extra == "docs"
 Requires-Dist: sphinx-design==0.5.0; extra == "docs"
 Requires-Dist: furo==2023.03.27; extra == "docs"
 Requires-Dist: nbsphinx==0.8.12; extra == "docs"
```

### Comparing `sqlalchemy_mate-2.0.0.1/sqlalchemy_mate.egg-info/SOURCES.txt` & `sqlalchemy_mate-2.0.0.2/sqlalchemy_mate.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -36,23 +36,31 @@
 sqlalchemy_mate/crud/updating_api.py
 sqlalchemy_mate/docs/__init__.py
 sqlalchemy_mate/orm/__init__.py
 sqlalchemy_mate/orm/api.py
 sqlalchemy_mate/orm/extended_declarative_base.py
 sqlalchemy_mate/patterns/__init__.py
 sqlalchemy_mate/patterns/api.py
+sqlalchemy_mate/patterns/large_binary_column/__init__.py
+sqlalchemy_mate/patterns/large_binary_column/api.py
+sqlalchemy_mate/patterns/large_binary_column/aws_s3.py
+sqlalchemy_mate/patterns/large_binary_column/aws_s3_api.py
+sqlalchemy_mate/patterns/large_binary_column/helpers.py
+sqlalchemy_mate/patterns/large_binary_column/local.py
+sqlalchemy_mate/patterns/large_binary_column/local_api.py
 sqlalchemy_mate/patterns/status_tracker/__init__.py
 sqlalchemy_mate/patterns/status_tracker/api.py
 sqlalchemy_mate/patterns/status_tracker/impl.py
 sqlalchemy_mate/types/__init__.py
 sqlalchemy_mate/types/api.py
 sqlalchemy_mate/types/compressed.py
 sqlalchemy_mate/types/compressed_json.py
 sqlalchemy_mate/types/json_serializable.py
 sqlalchemy_mate/vendor/__init__.py
+sqlalchemy_mate/vendor/iterable.py
 sqlalchemy_mate/vendor/pytest_cov_helper.py
 sqlalchemy_mate/vendor/timeout_decorator/__init__.py
 sqlalchemy_mate/vendor/timeout_decorator/timeout_decorator.py
 tests/test_api.py
 tests/test_engine_creator.py
 tests/test_io.py
 tests/test_pt.py
```

### Comparing `sqlalchemy_mate-2.0.0.1/tests/test_engine_creator.py` & `sqlalchemy_mate-2.0.0.2/tests/test_engine_creator.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mate-2.0.0.1/tests/test_io.py` & `sqlalchemy_mate-2.0.0.2/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mate-2.0.0.1/tests/test_pt.py` & `sqlalchemy_mate-2.0.0.2/tests/test_pt.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mate-2.0.0.1/tests/test_utils.py` & `sqlalchemy_mate-2.0.0.2/tests/test_utils.py`

 * *Files identical despite different names*

