# Comparing `tmp/dbt_athena_community-1.8.1.tar.gz` & `tmp/dbt_athena_community-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_athena_community-1.8.1.tar", last modified: Mon May 13 10:49:12 2024, max compression
+gzip compressed data, was "dbt_athena_community-1.8.2.tar", last modified: Tue May 28 18:18:55 2024, max compression
```

## Comparing `dbt_athena_community-1.8.1.tar` & `dbt_athena_community-1.8.2.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:49:12.955687 dbt_athena_community-1.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)    10702 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    34898 2024-05-13 10:49:12.955687 dbt_athena_community-1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    33725 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:49:12.943687 dbt_athena_community-1.8.1/dbt/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:49:12.943687 dbt_athena_community-1.8.1/dbt/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:49:12.943687 dbt_athena_community-1.8.1/dbt/adapters/athena/
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/adapters/athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/adapters/athena/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/adapters/athena/column.py
--rw-r--r--   0 runner    (1001) docker     (127)     6043 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/adapters/athena/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    13273 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/adapters/athena/connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/adapters/athena/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/adapters/athena/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    58912 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/adapters/athena/impl.py
--rw-r--r--   0 runner    (1001) docker     (127)    12859 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/adapters/athena/lakeformation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10857 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/adapters/athena/python_submissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/adapters/athena/query_headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/adapters/athena/relation.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/adapters/athena/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)    10079 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/adapters/athena/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/adapters/athena/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:49:12.939687 dbt_athena_community-1.8.1/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:49:12.947687 dbt_athena_community-1.8.1/dbt/include/athena/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:49:12.939687 dbt_athena_community-1.8.1/dbt/include/athena/macros/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:49:12.947687 dbt_athena_community-1.8.1/dbt/include/athena/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/adapters/columns.sql
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/adapters/metadata.sql
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/adapters/persist_docs.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/adapters/python_submissions.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/adapters/relation.sql
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/adapters/schema.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:49:12.947687 dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/hooks.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:49:12.939687 dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:49:12.947687 dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/models/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)     4676 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/models/helpers/get_partition_batches.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/models/helpers/process_bucket_column.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:49:12.947687 dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/models/incremental/
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/models/incremental/column_helpers.sql
--rw-r--r--   0 runner    (1001) docker     (127)     4755 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/models/incremental/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/models/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (127)     6707 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/models/incremental/merge.sql
--rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/models/incremental/on_schema_change.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:49:12.947687 dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/models/table/
--rw-r--r--   0 runner    (1001) docker     (127)     9632 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/models/table/create_table_as.sql
--rw-r--r--   0 runner    (1001) docker     (127)     7956 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/models/table/table.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:49:12.951687 dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/models/view/
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/models/view/create_or_replace_view.sql
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/models/view/create_view_as.sql
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/models/view/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:49:12.951687 dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/seeds/
--rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/seeds/helpers.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:49:12.951687 dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/snapshots/
--rw-r--r--   0 runner    (1001) docker     (127)     9052 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/snapshots/snapshot.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:49:12.951687 dbt_athena_community-1.8.1/dbt/include/athena/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/utils/any_value.sql
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/utils/array_append.sql
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/utils/array_concat.sql
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/utils/bool_or.sql
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/utils/datatypes.sql
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/utils/date_trunc.sql
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/utils/ddl_dml_data_type.sql
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/utils/hash.sql
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/utils/right.sql
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/utils/safe_cast.sql
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/macros/utils/timestamps.sql
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/profile_template.yml
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/dbt/include/athena/sample_profiles.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:49:12.955687 dbt_athena_community-1.8.1/dbt_athena_community.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    34898 2024-05-13 10:49:12.000000 dbt_athena_community-1.8.1/dbt_athena_community.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-05-13 10:49:12.000000 dbt_athena_community-1.8.1/dbt_athena_community.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 10:49:12.000000 dbt_athena_community-1.8.1/dbt_athena_community.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-13 10:49:12.000000 dbt_athena_community-1.8.1/dbt_athena_community.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-13 10:49:12.000000 dbt_athena_community-1.8.1/dbt_athena_community.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 10:49:12.955687 dbt_athena_community-1.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-05-13 10:49:05.000000 dbt_athena_community-1.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:18:55.618924 dbt_athena_community-1.8.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    10702 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    35760 2024-05-28 18:18:55.618924 dbt_athena_community-1.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    34587 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:18:55.610924 dbt_athena_community-1.8.2/dbt/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:18:55.610924 dbt_athena_community-1.8.2/dbt/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:18:55.610924 dbt_athena_community-1.8.2/dbt/adapters/athena/
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/adapters/athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/adapters/athena/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/adapters/athena/column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6043 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/adapters/athena/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14240 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/adapters/athena/connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/adapters/athena/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/adapters/athena/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    59369 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/adapters/athena/impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12859 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/adapters/athena/lakeformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10857 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/adapters/athena/python_submissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/adapters/athena/query_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/adapters/athena/relation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/adapters/athena/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10079 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/adapters/athena/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/adapters/athena/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:18:55.606924 dbt_athena_community-1.8.2/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:18:55.610924 dbt_athena_community-1.8.2/dbt/include/athena/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/include/athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/include/athena/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:18:55.606924 dbt_athena_community-1.8.2/dbt/include/athena/macros/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:18:55.614924 dbt_athena_community-1.8.2/dbt/include/athena/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/include/athena/macros/adapters/columns.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/include/athena/macros/adapters/metadata.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/include/athena/macros/adapters/persist_docs.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/include/athena/macros/adapters/python_submissions.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/include/athena/macros/adapters/relation.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/include/athena/macros/adapters/schema.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:18:55.614924 dbt_athena_community-1.8.2/dbt/include/athena/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/include/athena/macros/materializations/hooks.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:18:55.606924 dbt_athena_community-1.8.2/dbt/include/athena/macros/materializations/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:18:55.614924 dbt_athena_community-1.8.2/dbt/include/athena/macros/materializations/models/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)     4676 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/include/athena/macros/materializations/models/helpers/get_partition_batches.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/include/athena/macros/materializations/models/helpers/process_bucket_column.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:18:55.614924 dbt_athena_community-1.8.2/dbt/include/athena/macros/materializations/models/incremental/
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/include/athena/macros/materializations/models/incremental/column_helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     4755 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/include/athena/macros/materializations/models/incremental/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/include/athena/macros/materializations/models/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     6707 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/include/athena/macros/materializations/models/incremental/merge.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/include/athena/macros/materializations/models/incremental/on_schema_change.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:18:55.614924 dbt_athena_community-1.8.2/dbt/include/athena/macros/materializations/models/table/
+-rw-r--r--   0 runner    (1001) docker     (127)     9632 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/include/athena/macros/materializations/models/table/create_table_as.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     7956 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/include/athena/macros/materializations/models/table/table.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:18:55.614924 dbt_athena_community-1.8.2/dbt/include/athena/macros/materializations/models/view/
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/include/athena/macros/materializations/models/view/create_or_replace_view.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/include/athena/macros/materializations/models/view/create_view_as.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/include/athena/macros/materializations/models/view/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:18:55.614924 dbt_athena_community-1.8.2/dbt/include/athena/macros/materializations/seeds/
+-rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/include/athena/macros/materializations/seeds/helpers.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:18:55.614924 dbt_athena_community-1.8.2/dbt/include/athena/macros/materializations/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (127)     9052 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/include/athena/macros/materializations/snapshots/snapshot.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:18:55.618924 dbt_athena_community-1.8.2/dbt/include/athena/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/include/athena/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/include/athena/macros/utils/array_append.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/include/athena/macros/utils/array_concat.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/include/athena/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/include/athena/macros/utils/bool_or.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/include/athena/macros/utils/datatypes.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/include/athena/macros/utils/date_trunc.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/include/athena/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/include/athena/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/include/athena/macros/utils/ddl_dml_data_type.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/include/athena/macros/utils/hash.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/include/athena/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/include/athena/macros/utils/right.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/include/athena/macros/utils/safe_cast.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/include/athena/macros/utils/timestamps.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/include/athena/profile_template.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/dbt/include/athena/sample_profiles.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:18:55.618924 dbt_athena_community-1.8.2/dbt_athena_community.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    35760 2024-05-28 18:18:55.000000 dbt_athena_community-1.8.2/dbt_athena_community.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-05-28 18:18:55.000000 dbt_athena_community-1.8.2/dbt_athena_community.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 18:18:55.000000 dbt_athena_community-1.8.2/dbt_athena_community.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-28 18:18:55.000000 dbt_athena_community-1.8.2/dbt_athena_community.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-28 18:18:55.000000 dbt_athena_community-1.8.2/dbt_athena_community.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 18:18:55.618924 dbt_athena_community-1.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-05-28 18:18:47.000000 dbt_athena_community-1.8.2/setup.py
```

### Comparing `dbt_athena_community-1.8.1/LICENSE.txt` & `dbt_athena_community-1.8.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.1/PKG-INFO` & `dbt_athena_community-1.8.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-athena-community
-Version: 1.8.1
+Version: 1.8.2
 Summary: The athena adapter plugin for dbt (data build tool)
 Home-page: https://github.com/dbt-athena/dbt-athena
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
@@ -45,57 +45,57 @@
     <a href="https://pepy.tech/project/dbt-athena-community">
       <img src="https://static.pepy.tech/badge/dbt-athena-community/month" />
     </a>
 </p>
 <!-- TOC -->
 
 - [Features](#features)
-  - [Quick Start](#quick-start)
+  - [Quick start](#quick-start)
     - [Installation](#installation)
     - [Prerequisites](#prerequisites)
     - [Credentials](#credentials)
     - [Configuring your profile](#configuring-your-profile)
     - [Additional information](#additional-information)
   - [Models](#models)
-    - [Table Configuration](#table-configuration)
+    - [Table configuration](#table-configuration)
     - [Table location](#table-location)
     - [Incremental models](#incremental-models)
     - [On schema change](#on-schema-change)
     - [Iceberg](#iceberg)
     - [Highly available table (HA)](#highly-available-table-ha)
-      - [HA Known issues](#ha-known-issues)
+      - [HA known issues](#ha-known-issues)
     - [Update glue data catalog](#update-glue-data-catalog)
   - [Snapshots](#snapshots)
     - [Timestamp strategy](#timestamp-strategy)
     - [Check strategy](#check-strategy)
     - [Hard-deletes](#hard-deletes)
     - [Working example](#working-example)
-    - [Snapshots Known issues](#snapshots-known-issues)
-  - [AWS Lakeformation integration](#aws-lakeformation-integration)
-  - [Python Models](#python-models)
+    - [Snapshots known issues](#snapshots-known-issues)
+  - [AWS Lake Formation integration](#aws-lake-formation-integration)
+  - [Python models](#python-models)
   - [Contracts](#contracts)
   - [Contributing](#contributing)
   - [Contributors ✨](#contributors-)
 <!-- TOC -->
 
 # Features
 
 - Supports dbt version `1.7.*`
 - Support for Python
 - Supports [seeds][seeds]
 - Correctly detects views and their columns
 - Supports [table materialization][table]
   - [Iceberg tables][athena-iceberg] are supported **only with Athena Engine v3** and **a unique table location**
     (see table location section below)
-  - Hive tables are supported by both Athena engines.
+  - Hive tables are supported by both Athena engines
 - Supports [incremental models][incremental]
-  - On Iceberg tables :
+  - On Iceberg tables:
     - Supports the use of `unique_key` only with the `merge` strategy
     - Supports the `append` strategy
-  - On Hive tables :
+  - On Hive tables:
     - Supports two incremental update strategies: `insert_overwrite` and `append`
     - Does **not** support the use of `unique_key`
 - Supports [snapshots][snapshots]
 - Supports [Python models][python-models]
 
 [seeds]: https://docs.getdbt.com/docs/building-a-dbt-project/seeds
 
@@ -105,15 +105,15 @@
 
 [python-models]: https://docs.getdbt.com/docs/build/python-models#configuring-python-models
 
 [athena-iceberg]: https://docs.aws.amazon.com/athena/latest/ug/querying-iceberg.html
 
 [snapshots]: https://docs.getdbt.com/docs/build/snapshots
 
-## Quick Start
+## Quick start
 
 ### Installation
 
 - `pip install dbt-athena-community`
 - Or `pip install git+https://github.com/dbt-athena/dbt-athena.git`
 
 ### Prerequisites
@@ -136,40 +136,41 @@
 ### Credentials
 
 Credentials can be passed directly to the adapter, or they can
 be [determined automatically](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/credentials.html) based
 on `aws cli`/`boto3` conventions.
 You can either:
 
-- configure `aws_access_key_id` and `aws_secret_access_key`
-- configure `aws_profile_name` to match a profile defined in your AWS credentials file
+- Configure `aws_access_key_id` and `aws_secret_access_key`
+- Configure `aws_profile_name` to match a profile defined in your AWS credentials file.
   Checkout dbt profile configuration below for details.
 
 ### Configuring your profile
 
 A dbt profile can be configured to run against AWS Athena using the following configuration:
 
 | Option                | Description                                                                              | Required? | Example                                    |
-| --------------------- | ---------------------------------------------------------------------------------------- | --------- | ------------------------------------------ |
+|-----------------------|------------------------------------------------------------------------------------------|-----------|--------------------------------------------|
 | s3_staging_dir        | S3 location to store Athena query results and metadata                                   | Required  | `s3://bucket/dbt/`                         |
 | s3_data_dir           | Prefix for storing tables, if different from the connection's `s3_staging_dir`           | Optional  | `s3://bucket2/dbt/`                        |
 | s3_data_naming        | How to generate table paths in `s3_data_dir`                                             | Optional  | `schema_table_unique`                      |
 | s3_tmp_table_dir      | Prefix for storing temporary tables, if different from the connection's `s3_data_dir`    | Optional  | `s3://bucket3/dbt/`                        |
 | region_name           | AWS region of your Athena instance                                                       | Required  | `eu-west-1`                                |
 | schema                | Specify the schema (Athena database) to build models into (lowercase **only**)           | Required  | `dbt`                                      |
 | database              | Specify the database (Data catalog) to build models into (lowercase **only**)            | Required  | `awsdatacatalog`                           |
 | poll_interval         | Interval in seconds to use for polling the status of query results in Athena             | Optional  | `5`                                        |
 | debug_query_state     | Flag if debug message with Athena query state is needed                                  | Optional  | `false`                                    |
-| aws_access_key_id     | Access key ID of the user performing requests.                                           | Optional  | `AKIAIOSFODNN7EXAMPLE`                     |
+| aws_access_key_id     | Access key ID of the user performing requests                                            | Optional  | `AKIAIOSFODNN7EXAMPLE`                     |
 | aws_secret_access_key | Secret access key of the user performing requests                                        | Optional  | `wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY` |
-| aws_profile_name      | Profile to use from your AWS shared credentials file.                                    | Optional  | `my-profile`                               |
+| aws_profile_name      | Profile to use from your AWS shared credentials file                                     | Optional  | `my-profile`                               |
 | work_group            | Identifier of Athena workgroup                                                           | Optional  | `my-custom-workgroup`                      |
 | num_retries           | Number of times to retry a failing query                                                 | Optional  | `3`                                        |
-| spark_work_group      | Identifier of Athena Spark workgroup                                           | Optional  | `my-spark-workgroup`                       |
 | num_boto3_retries     | Number of times to retry boto3 requests (e.g. deleting S3 files for materialized tables) | Optional  | `5`                                        |
+| num_iceberg_retries   | Number of times to retry iceberg commit queries to fix ICEBERG_COMMIT_ERROR              | Optional  | `0`                                        |
+| spark_work_group      | Identifier of Athena Spark workgroup for running Python models                           | Optional  | `my-spark-workgroup`                       |
 | seed_s3_upload_args   | Dictionary containing boto3 ExtraArgs when uploading to S3                               | Optional  | `{"ACL": "bucket-owner-full-control"}`     |
 | lf_tags_database      | Default LF tags for new database if it's created by dbt                                  | Optional  | `tag_key: tag_value`                       |
 
 **Example profiles.yml entry:**
 
 ```yaml
 athena:
@@ -195,20 +196,20 @@
 ### Additional information
 
 - `threads` is supported
 - `database` and `catalog` can be used interchangeably
 
 ## Models
 
-### Table Configuration
+### Table configuration
 
 - `external_location` (`default=none`)
-  - If set, the full S3 path in which the table will be saved.
-  - It works only with incremental models.
-  - Does not work with Hive table with `ha` set to true.
+  - If set, the full S3 path to which the table will be saved
+  - Works only with incremental models
+  - Does not work with Hive table with `ha` set to true
 - `partitioned_by` (`default=none`)
   - An array list of columns by which the table will be partitioned
   - Limited to creation of 100 partitions (*currently*)
 - `bucketed_by` (`default=none`)
   - An array list of columns to bucket data, ignored if using Iceberg
 - `bucket_count` (`default=none`)
   - The number of buckets for bucketing your data, ignored if using Iceberg
@@ -228,23 +229,31 @@
   - Custom field delimiter, for when format is set to `TEXTFILE`
 - `table_properties`: table properties to add to the table, valid for Iceberg only
 - `native_drop`: Relation drop operations will be performed with SQL, not direct Glue API calls. No S3 calls will be
   made to manage data in S3. Data in S3 will only be cleared up for Iceberg
   tables [see AWS docs](https://docs.aws.amazon.com/athena/latest/ug/querying-iceberg-managing-tables.html). Note that
   Iceberg DROP TABLE operations may timeout if they take longer than 60 seconds.
 - `seed_by_insert` (`default=false`)
-  - default behaviour uploads seed data to S3. This flag will create seeds using an SQL insert statement
-  - large seed files cannot use `seed_by_insert`, as the SQL insert statement would
+  - Default behaviour uploads seed data to S3. This flag will create seeds using an SQL insert statement
+  - Large seed files cannot use `seed_by_insert`, as the SQL insert statement would
     exceed [the Athena limit of 262144 bytes](https://docs.aws.amazon.com/athena/latest/ug/service-limits.html)
 - `force_batch` (`default=false`)
-  - Skip creating the table as ctas and run the operation directly in batch insert mode.
+  - Skip creating the table as CTAS and run the operation directly in batch insert mode
   - This is particularly useful when the standard table creation process fails due to partition limitations,
-  allowing you to work with temporary tables and persist the dataset more efficiently.
+  allowing you to work with temporary tables and persist the dataset more efficiently
+- `unique_tmp_table_suffix` (`default=false`)
+  - For incremental models using insert overwrite strategy on hive table
+  - Replace the __dbt_tmp suffix used as temporary table name suffix by a unique uuid
+  - Useful if you are looking to run multiple dbt build inserting in the same table in parallel
+- `temp_schema` (`default=none`)
+  - For incremental models, it allows to define a schema to hold temporary create statements
+  used in incremental model runs
+  - Schema will be created in the model target database if does not exist
 - `lf_tags_config` (`default=none`)
-  - [AWS lakeformation](#aws-lakeformation-integration) tags to associate with the table and columns
+  - [AWS Lake Formation](#aws-lake-formation-integration) tags to associate with the table and columns
   - `enabled` (`default=False`) whether LF tags management is enabled for a model
   - `tags` dictionary with tags and their values to assign for the model
   - `tags_columns` dictionary with a tag key, value and list of columns they must be assigned to
   - `lf_inherited_tags` (`default=none`)
     - List of Lake Formation tag keys that are intended to be inherited from the database level and thus shouldn't be
       removed during association of those defined in `lf_tags_config`
       - i.e., the default behavior of `lf_tags_config` is to be exhaustive and first remove any pre-existing tags from
@@ -273,31 +282,31 @@
           },
           'inherited_tags': ['tag1', 'tag2']
     }
   )
 }}
 ```
 
-- format for `dbt_project.yml`:
+- Format for `dbt_project.yml`:
 
 ```yaml
   +lf_tags_config:
     enabled: true
     tags:
       tag1: value1
       tag2: value2
     tags_columns:
       tag1:
         value1: [ column1, column2 ]
     inherited_tags: [ tag1, tag2 ]
 ```
 
 - `lf_grants` (`default=none`)
-  - lakeformation grants config for data_cell filters
-  - format:
+  - Lake Formation grants config for data_cell filters
+  - Format:
 
   ```python
   lf_grants={
           'data_cell_filters': {
               'enabled': True | False,
               'filters': {
                   'filter_name': {
@@ -328,17 +337,17 @@
       where the inherited value is configured nor in the DBT project where the override previously existed but now is
       gone)
 
 [create-table-as]: https://docs.aws.amazon.com/athena/latest/ug/create-table-as.html#ctas-table-properties
 
 ### Table location
 
-The location in which a table is saved is determined by:
+The location a table is saved to is determined by:
 
-1. If `external_location` is defined, that value is used.
+1. If `external_location` is defined, that value is used
 2. If `s3_data_dir` is defined, the path is determined by that and `s3_data_naming`
 3. If `s3_data_dir` is not defined, data is stored under `s3_staging_dir/tables/`
 
 Here all the options available for `s3_data_naming`:
 
 - `unique`: `{s3_data_dir}/{uuid4()}/`
 - `table`: `{s3_data_dir}/{table}/`
@@ -498,19 +507,20 @@
     , (2, 1)
 ) as t (id, status)
 
 ```
 
 ### Highly available table (HA)
 
-The current implementation of the table materialization can lead to downtime, as target table is dropped and re-created.
-To have the less destructive behavior it's possible to use the `ha` config on your `table` materialized models.
-It leverages the table versions feature of glue catalog, creating a tmp table and swapping the target table to the
-location of the tmp table. This materialization is only available for `table_type=hive` and requires using unique
-locations. For iceberg, high availability is by default.
+The current implementation of the table materialization can lead to downtime, as the target table is
+dropped and re-created. To have the less destructive behavior it's possible to use the `ha` config on
+your `table` materialized models. It leverages the table versions feature of glue catalog, creating
+a temp table and swapping the target table to the location of the temp table. This materialization
+is only available for `table_type=hive` and requires using unique locations. For iceberg, high
+availability is the default.
 
 ```sql
 {{ config(
     materialized='table',
     ha=true,
     format='parquet',
     table_type='hive',
@@ -525,21 +535,21 @@
 select 'b'        as user_id,
        'sh'       as user_name,
        'disabled' as status
 ```
 
 By default, the materialization keeps the last 4 table versions, you can change it by setting `versions_to_keep`.
 
-#### HA Known issues
+#### HA known issues
 
 - When swapping from a table with partitions to a table without (and the other way around), there could be a little
   downtime.
-  In case high performances are needed consider bucketing instead of partitions
+  If high performances is needed consider bucketing instead of partitions
 - By default, Glue "duplicates" the versions internally, so the last two versions of a table point to the same location
-- It's recommended to have `versions_to_keep` >= 4, as this will avoid having the older location removed
+- It's recommended to set `versions_to_keep` >= 4, as this will avoid having the older location removed
 
 ### Update glue data catalog
 
 Optionally persist resource descriptions as column and relation comments to the glue data catalog, and meta as
 [glue table properties](https://docs.aws.amazon.com/glue/latest/dg/tables-described.html#table-properties)
 and [column parameters](https://docs.aws.amazon.com/glue/latest/webapi/API_Column.html).
 By default, documentation persistence is disabled, but it can be enabled for specific resources or
@@ -672,74 +682,75 @@
         check_cols=['series_reference','data_value']
     )
 }}
 select *
 from {{ ref('model') }} {% endsnapshot %}
 ```
 
-### Snapshots Known issues
+### Snapshots known issues
 
-- Incremental Iceberg models - Sync all columns on schema change can't remove columns used as partitioning.
+- Incremental Iceberg models - Sync all columns on schema change can't remove columns used for partitioning.
   The only way, from a dbt perspective, is to do a full-refresh of the incremental model.
 
-- Tables, schemas and database should only be lowercase
+- Tables, schemas and database names should only be lowercase
 
 - In order to avoid potential conflicts, make sure [`dbt-athena-adapter`](https://github.com/Tomme/dbt-athena) is not
   installed in the target environment.
   See <https://github.com/dbt-athena/dbt-athena/issues/103> for more details.
 
 - Snapshot does not support dropping columns from the source table. If you drop a column make sure to drop the column
   from the snapshot as well. Another workaround is to NULL the column in the snapshot definition to preserve history
 
-## AWS Lakeformation integration
+## AWS Lake Formation integration
 
-The adapter implements AWS Lakeformation tags management in the following way:
+The adapter implements AWS Lake Formation tags management in the following way:
 
-- you can enable or disable lf-tags management via [config](#table-configuration) (disabled by default)
-- once you enable the feature, lf-tags will be updated on every dbt run
-- first, all lf-tags for columns are removed to avoid inheritance issues
-- then all redundant lf-tags are removed from table and actual tags from config are applied
-- finally, lf-tags for columns are applied
+- You can enable or disable lf-tags management via [config](#table-configuration) (disabled by default)
+- Once you enable the feature, lf-tags will be updated on every dbt run
+- First, all lf-tags for columns are removed to avoid inheritance issues
+- Then, all redundant lf-tags are removed from tables and actual tags from table configs are applied
+- Finally, lf-tags for columns are applied
 
 It's important to understand the following points:
 
-- dbt does not manage lf-tags for database
-- dbt does not manage lakeformation permissions
+- dbt does not manage lf-tags for databases
+- dbt does not manage Lake Formation permissions
 
-That's why you should handle this by yourself manually or using some automation tools like terraform, AWS CDK etc.
+That's why you should handle this by yourself manually or using an automation tool like terraform, AWS CDK etc.
 You may find the following links useful to manage that:
 
 <!-- markdownlint-disable -->
 * [terraform aws_lakeformation_permissions](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lakeformation_permissions)
 * [terraform aws_lakeformation_resource_lf_tags](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lakeformation_resource_lf_tags)
 <!-- markdownlint-restore -->
 
-## Python Models
+## Python models
 
-The adapter supports python models using [`spark`](https://docs.aws.amazon.com/athena/latest/ug/notebooks-spark.html).
+The adapter supports Python models using [`spark`](https://docs.aws.amazon.com/athena/latest/ug/notebooks-spark.html).
 
 ### Setup
 
 - A Spark-enabled workgroup created in Athena
 - Spark execution role granted access to Athena, Glue and S3
-- The Spark workgroup is added to the `~/.dbt/profiles.yml` file and the profile
- is referenced in `dbt_project.yml` that will be created. It is recommended to keep this same as threads.
+- The Spark workgroup is added to the `~/.dbt/profiles.yml` file and the profile to be used
+  is referenced in `dbt_project.yml`
 
 ### Spark-specific table configuration
 
 - `timeout` (`default=43200`)
   - Time out in seconds for each Python model execution. Defaults to 12 hours/43200 seconds.
 - `spark_encryption` (`default=false`)
   - If this flag is set to true, encrypts data in transit between Spark nodes and also encrypts data at rest stored
    locally by Spark.
 - `spark_cross_account_catalog` (`default=false`)
-  - In Spark, you can query the external account catalog and for that the consumer account has to be configured to
-   access the producer catalog.
-  - If this flag is set to true, "/" can be used as the glue catalog separator.
-   Ex: 999999999999/mydatabase.cloudfront_logs (*where *999999999999* is the external catalog ID*)
+  - When using the Spark Athena workgroup, queries can only be made against catalogs located on the same
+    AWS account by default. However, sometimes you want to query another catalog located on an external AWS
+    account. Setting this additional Spark properties parameter to true will enable querying external catalogs.
+    You can use the syntax `external_catalog_id/database.table` to access the external table on the external
+    catalog (ex: `999999999999/mydatabase.cloudfront_logs` where 999999999999 is the external catalog ID)
 - `spark_requester_pays` (`default=false`)
   - When an Amazon S3 bucket is configured as requester pays, the account of the user running the query is charged for
    data access and data transfer fees associated with the query.
   - If this flag is set to true, requester pays S3 buckets are enabled in Athena for Spark.
 
 ### Spark notes
 
@@ -852,36 +863,36 @@
     return df.withColumn("udf_test_col", udf_with_import(col("alpha")))
 ```
 
 ### Known issues in Python models
 
 - Python models cannot
  [reference Athena SQL views](https://docs.aws.amazon.com/athena/latest/ug/notebooks-spark.html).
-- Third-party Python libraries can be used, but they must be [included in the pre-installed list]([pre-installed list])
- or [imported manually]([imported manually]).
+- Third-party Python libraries can be used, but they must be [included in the pre-installed list][pre-installed list]
+ or [imported manually][imported manually].
 - Python models can only reference or write to tables with names meeting the
  regular expression: `^[0-9a-zA-Z_]+$`. Dashes and special characters are not
  supported by Spark, even though Athena supports them.
 - Incremental models do not fully utilize Spark capabilities. They depend partially on existing SQL-based logic which
  runs on Trino.
 - Snapshot materializations are not supported.
 - Spark can only reference tables within the same catalog.
 
 [pre-installed list]: https://docs.aws.amazon.com/athena/latest/ug/notebooks-spark-preinstalled-python-libraries.html
 [imported manually]: https://docs.aws.amazon.com/athena/latest/ug/notebooks-import-files-libraries.html
 
 ## Contracts
 
-The adapter partly supports contract definition.
+The adapter partly supports contract definitions:
 
-- Concerning the `data_type`, it is supported but needs to be adjusted for complex types. They must be specified
+- `data_type` is supported but needs to be adjusted for complex types. Types must be specified
   entirely (for instance `array<int>`) even though they won't be checked. Indeed, as dbt recommends, we only compare
   the broader type (array, map, int, varchar). The complete definition is used in order to check that the data types
-  defined in athena are ok (pre-flight check).
-- the adapter does not support the constraints since no constraints don't exist in Athena.
+  defined in Athena are ok (pre-flight check).
+- The adapter does not support the constraints since there is no constraint concept in Athena.
 
 ## Contributing
 
 See [CONTRIBUTING](CONTRIBUTING.md) for more information on how to contribute to this project.
 
 ## Contributors ✨
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-athena-community Version: 1.8.1 Summary: The
+Metadata-Version: 2.1 Name: dbt-athena-community Version: 1.8.2 Summary: The
 athena adapter plugin for dbt (data build tool) Home-page: https://github.com/
 dbt-athena/dbt-athena License: Apache License 2.0 Platform: any Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
@@ -17,100 +17,102 @@
  [https://raw.githubusercontent.com/dbt-athena/dbt-athena/main/static/images/
 dbt-athena-long.png]_[_h_t_t_p_s_:_/_/_b_a_d_g_e_._f_u_r_y_._i_o_/_p_y_/_d_b_t_-_a_t_h_e_n_a_-_c_o_m_m_u_n_i_t_y_._s_v_g_]_[_h_t_t_p_s_:_/
  _/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_d_b_t_-_a_t_h_e_n_a_-_c_o_m_m_u_n_i_t_y_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
     _b_a_d_g_e_/_%_2_0_i_m_p_o_r_t_s_-_i_s_o_r_t_-_%_2_3_1_6_7_4_b_1_?_s_t_y_l_e_=_f_l_a_t_&_l_a_b_e_l_C_o_l_o_r_=_e_f_8_3_3_6_]_[_h_t_t_p_s_:_/_/
 _i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_c_o_d_e_%_2_0_s_t_y_l_e_-_b_l_a_c_k_-_0_0_0_0_0_0_._s_v_g_]_[_h_t_t_p_s_:_/_/_w_w_w_._m_y_p_y_-_l_a_n_g_._o_r_g_/
   _s_t_a_t_i_c_/_m_y_p_y___b_a_d_g_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_s_t_a_t_i_c_._p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/_d_b_t_-_a_t_h_e_n_a_-_c_o_m_m_u_n_i_t_y_/
                                     _m_o_n_t_h_]
-- [Features](#features) - [Quick Start](#quick-start) - [Installation]
+- [Features](#features) - [Quick start](#quick-start) - [Installation]
 (#installation) - [Prerequisites](#prerequisites) - [Credentials](#credentials)
 - [Configuring your profile](#configuring-your-profile) - [Additional
 information](#additional-information) - [Models](#models) - [Table
-Configuration](#table-configuration) - [Table location](#table-location) -
+configuration](#table-configuration) - [Table location](#table-location) -
 [Incremental models](#incremental-models) - [On schema change](#on-schema-
 change) - [Iceberg](#iceberg) - [Highly available table (HA)](#highly-
-available-table-ha) - [HA Known issues](#ha-known-issues) - [Update glue data
+available-table-ha) - [HA known issues](#ha-known-issues) - [Update glue data
 catalog](#update-glue-data-catalog) - [Snapshots](#snapshots) - [Timestamp
 strategy](#timestamp-strategy) - [Check strategy](#check-strategy) - [Hard-
 deletes](#hard-deletes) - [Working example](#working-example) - [Snapshots
-Known issues](#snapshots-known-issues) - [AWS Lakeformation integration](#aws-
-lakeformation-integration) - [Python Models](#python-models) - [Contracts]
+known issues](#snapshots-known-issues) - [AWS Lake Formation integration](#aws-
+lake-formation-integration) - [Python models](#python-models) - [Contracts]
 (#contracts) - [Contributing](#contributing) - [Contributors â¨]
 (#contributors-) # Features - Supports dbt version `1.7.*` - Support for Python
 - Supports [seeds][seeds] - Correctly detects views and their columns -
 Supports [table materialization][table] - [Iceberg tables][athena-iceberg] are
 supported **only with Athena Engine v3** and **a unique table location** (see
 table location section below) - Hive tables are supported by both Athena
-engines. - Supports [incremental models][incremental] - On Iceberg tables : -
+engines - Supports [incremental models][incremental] - On Iceberg tables: -
 Supports the use of `unique_key` only with the `merge` strategy - Supports the
-`append` strategy - On Hive tables : - Supports two incremental update
+`append` strategy - On Hive tables: - Supports two incremental update
 strategies: `insert_overwrite` and `append` - Does **not** support the use of
 `unique_key` - Supports [snapshots][snapshots] - Supports [Python models]
 [python-models] [seeds]: https://docs.getdbt.com/docs/building-a-dbt-project/
 seeds [incremental]: https://docs.getdbt.com/docs/build/incremental-models
 [table]: https://docs.getdbt.com/docs/build/materializations#table [python-
 models]: https://docs.getdbt.com/docs/build/python-models#configuring-python-
 models [athena-iceberg]: https://docs.aws.amazon.com/athena/latest/ug/querying-
 iceberg.html [snapshots]: https://docs.getdbt.com/docs/build/snapshots ## Quick
-Start ### Installation - `pip install dbt-athena-community` - Or `pip install
+start ### Installation - `pip install dbt-athena-community` - Or `pip install
 git+https://github.com/dbt-athena/dbt-athena.git` ### Prerequisites To start,
 you will need an S3 bucket, for instance `my-bucket` and an Athena database:
 ```sql CREATE DATABASE IF NOT EXISTS analytics_dev COMMENT 'Analytics models
 generated by dbt (development)' LOCATION 's3://my-bucket/' WITH DBPROPERTIES
 ('creator'='Foo Bar', 'email'='foo@bar.com'); ``` Notes: - Take note of your
 AWS region code (e.g. `us-west-2` or `eu-west-2`, etc.). - You can also use
 [AWS Glue](https://docs.aws.amazon.com/athena/latest/ug/glue-athena.html) to
 create and manage Athena databases. ### Credentials Credentials can be passed
 directly to the adapter, or they can be [determined automatically](https://
 boto3.amazonaws.com/v1/documentation/api/latest/guide/credentials.html) based
-on `aws cli`/`boto3` conventions. You can either: - configure
-`aws_access_key_id` and `aws_secret_access_key` - configure `aws_profile_name`
-to match a profile defined in your AWS credentials file Checkout dbt profile
+on `aws cli`/`boto3` conventions. You can either: - Configure
+`aws_access_key_id` and `aws_secret_access_key` - Configure `aws_profile_name`
+to match a profile defined in your AWS credentials file. Checkout dbt profile
 configuration below for details. ### Configuring your profile A dbt profile can
 be configured to run against AWS Athena using the following configuration: |
-Option | Description | Required? | Example | | --------------------- | --------
+Option | Description | Required? | Example | |-----------------------|---------
 -------------------------------------------------------------------------------
-- | --------- | ------------------------------------------ | | s3_staging_dir |
+--|-----------|--------------------------------------------| | s3_staging_dir |
 S3 location to store Athena query results and metadata | Required | `s3://
 bucket/dbt/` | | s3_data_dir | Prefix for storing tables, if different from the
 connection's `s3_staging_dir` | Optional | `s3://bucket2/dbt/` | |
 s3_data_naming | How to generate table paths in `s3_data_dir` | Optional |
 `schema_table_unique` | | s3_tmp_table_dir | Prefix for storing temporary
 tables, if different from the connection's `s3_data_dir` | Optional | `s3://
 bucket3/dbt/` | | region_name | AWS region of your Athena instance | Required |
 `eu-west-1` | | schema | Specify the schema (Athena database) to build models
 into (lowercase **only**) | Required | `dbt` | | database | Specify the
 database (Data catalog) to build models into (lowercase **only**) | Required |
 `awsdatacatalog` | | poll_interval | Interval in seconds to use for polling the
 status of query results in Athena | Optional | `5` | | debug_query_state | Flag
 if debug message with Athena query state is needed | Optional | `false` | |
-aws_access_key_id | Access key ID of the user performing requests. | Optional |
+aws_access_key_id | Access key ID of the user performing requests | Optional |
 `AKIAIOSFODNN7EXAMPLE` | | aws_secret_access_key | Secret access key of the
 user performing requests | Optional | `wJalrXUtnFEMI/K7MDENG/
 bPxRfiCYEXAMPLEKEY` | | aws_profile_name | Profile to use from your AWS shared
-credentials file. | Optional | `my-profile` | | work_group | Identifier of
+credentials file | Optional | `my-profile` | | work_group | Identifier of
 Athena workgroup | Optional | `my-custom-workgroup` | | num_retries | Number of
-times to retry a failing query | Optional | `3` | | spark_work_group |
-Identifier of Athena Spark workgroup | Optional | `my-spark-workgroup` | |
-num_boto3_retries | Number of times to retry boto3 requests (e.g. deleting S3
-files for materialized tables) | Optional | `5` | | seed_s3_upload_args |
-Dictionary containing boto3 ExtraArgs when uploading to S3 | Optional | `
-{"ACL": "bucket-owner-full-control"}` | | lf_tags_database | Default LF tags
-for new database if it's created by dbt | Optional | `tag_key: tag_value` |
-**Example profiles.yml entry:** ```yaml athena: target: dev outputs: dev: type:
-athena s3_staging_dir: s3://athena-query-results/dbt/ s3_data_dir: s3://
+times to retry a failing query | Optional | `3` | | num_boto3_retries | Number
+of times to retry boto3 requests (e.g. deleting S3 files for materialized
+tables) | Optional | `5` | | num_iceberg_retries | Number of times to retry
+iceberg commit queries to fix ICEBERG_COMMIT_ERROR | Optional | `0` | |
+spark_work_group | Identifier of Athena Spark workgroup for running Python
+models | Optional | `my-spark-workgroup` | | seed_s3_upload_args | Dictionary
+containing boto3 ExtraArgs when uploading to S3 | Optional | `{"ACL": "bucket-
+owner-full-control"}` | | lf_tags_database | Default LF tags for new database
+if it's created by dbt | Optional | `tag_key: tag_value` | **Example
+profiles.yml entry:** ```yaml athena: target: dev outputs: dev: type: athena
+s3_staging_dir: s3://athena-query-results/dbt/ s3_data_dir: s3://
 your_s3_bucket/dbt/ s3_data_naming: schema_table s3_tmp_table_dir: s3://
 your_s3_bucket/temp/ region_name: eu-west-1 schema: dbt database:
 awsdatacatalog threads: 4 aws_profile_name: my-profile work_group: my-workgroup
 spark_work_group: my-spark-workgroup seed_s3_upload_args: ACL: bucket-owner-
 full-control ``` ### Additional information - `threads` is supported -
 `database` and `catalog` can be used interchangeably ## Models ### Table
-Configuration - `external_location` (`default=none`) - If set, the full S3 path
-in which the table will be saved. - It works only with incremental models. -
-Does not work with Hive table with `ha` set to true. - `partitioned_by`
+configuration - `external_location` (`default=none`) - If set, the full S3 path
+to which the table will be saved - Works only with incremental models - Does
+not work with Hive table with `ha` set to true - `partitioned_by`
 (`default=none`) - An array list of columns by which the table will be
 partitioned - Limited to creation of 100 partitions (*currently*) -
 `bucketed_by` (`default=none`) - An array list of columns to bucket data,
 ignored if using Iceberg - `bucket_count` (`default=none`) - The number of
 buckets for bucketing your data, ignored if using Iceberg - `table_type`
 (`default='hive'`) - The type of table - Supports `hive` or `iceberg` - `ha`
 (`default=false`) - If the table should be built using the high-availability
@@ -124,24 +126,31 @@
 Custom field delimiter, for when format is set to `TEXTFILE` -
 `table_properties`: table properties to add to the table, valid for Iceberg
 only - `native_drop`: Relation drop operations will be performed with SQL, not
 direct Glue API calls. No S3 calls will be made to manage data in S3. Data in
 S3 will only be cleared up for Iceberg tables [see AWS docs](https://
 docs.aws.amazon.com/athena/latest/ug/querying-iceberg-managing-tables.html).
 Note that Iceberg DROP TABLE operations may timeout if they take longer than 60
-seconds. - `seed_by_insert` (`default=false`) - default behaviour uploads seed
-data to S3. This flag will create seeds using an SQL insert statement - large
+seconds. - `seed_by_insert` (`default=false`) - Default behaviour uploads seed
+data to S3. This flag will create seeds using an SQL insert statement - Large
 seed files cannot use `seed_by_insert`, as the SQL insert statement would
 exceed [the Athena limit of 262144 bytes](https://docs.aws.amazon.com/athena/
 latest/ug/service-limits.html) - `force_batch` (`default=false`) - Skip
-creating the table as ctas and run the operation directly in batch insert mode.
+creating the table as CTAS and run the operation directly in batch insert mode
 - This is particularly useful when the standard table creation process fails
 due to partition limitations, allowing you to work with temporary tables and
-persist the dataset more efficiently. - `lf_tags_config` (`default=none`) -
-[AWS lakeformation](#aws-lakeformation-integration) tags to associate with the
+persist the dataset more efficiently - `unique_tmp_table_suffix`
+(`default=false`) - For incremental models using insert overwrite strategy on
+hive table - Replace the __dbt_tmp suffix used as temporary table name suffix
+by a unique uuid - Useful if you are looking to run multiple dbt build
+inserting in the same table in parallel - `temp_schema` (`default=none`) - For
+incremental models, it allows to define a schema to hold temporary create
+statements used in incremental model runs - Schema will be created in the model
+target database if does not exist - `lf_tags_config` (`default=none`) - [AWS
+Lake Formation](#aws-lake-formation-integration) tags to associate with the
 table and columns - `enabled` (`default=False`) whether LF tags management is
 enabled for a model - `tags` dictionary with tags and their values to assign
 for the model - `tags_columns` dictionary with a tag key, value and list of
 columns they must be assigned to - `lf_inherited_tags` (`default=none`) - List
 of Lake Formation tag keys that are intended to be inherited from the database
 level and thus shouldn't be removed during association of those defined in
 `lf_tags_config` - i.e., the default behavior of `lf_tags_config` is to be
@@ -149,19 +158,19 @@
 before associating the ones currently defined for a given model - This breaks
 tag inheritance as inherited tags appear on tables and columns like those
 associated directly ```sql {{ config( materialized='incremental',
 incremental_strategy='append', on_schema_change='append_new_columns',
 table_type='iceberg', schema='test_schema', lf_tags_config={ 'enabled': true,
 'tags': { 'tag1': 'value1', 'tag2': 'value2' }, 'tags_columns': { 'tag1':
 { 'value1': ['column1', 'column2'], 'value2': ['column3', 'column4'] } },
-'inherited_tags': ['tag1', 'tag2'] } ) }} ``` - format for `dbt_project.yml`:
+'inherited_tags': ['tag1', 'tag2'] } ) }} ``` - Format for `dbt_project.yml`:
 ```yaml +lf_tags_config: enabled: true tags: tag1: value1 tag2: value2
 tags_columns: tag1: value1: [ column1, column2 ] inherited_tags: [ tag1, tag2 ]
-``` - `lf_grants` (`default=none`) - lakeformation grants config for data_cell
-filters - format: ```python lf_grants={ 'data_cell_filters': { 'enabled': True
+``` - `lf_grants` (`default=none`) - Lake Formation grants config for data_cell
+filters - Format: ```python lf_grants={ 'data_cell_filters': { 'enabled': True
 | False, 'filters': { 'filter_name': { 'row_filter': '', 'principals':
 ['principal_arn1', 'principal_arn2'] } } } } ``` > Notes: > > - `lf_tags` and
 `lf_tags_columns` configs support only attaching lf tags to corresponding
 resources. > We recommend managing LF Tags permissions somewhere outside dbt.
 For example, you may use > [terraform](https://registry.terraform.io/providers/
 hashicorp/aws/latest/docs/resources/lakeformation_permissions) or > [aws cdk]
 (https://docs.aws.amazon.com/cdk/api/v1/docs/aws-lakeformation-readme.html) for
@@ -176,17 +185,17 @@
 not differentiate between an inherited tag association and an override of same
 it made > previously > - e.g. If an inherited tag is overridden by an
 `lf_tags_config` value in one DBT run, and that override is removed prior to a
 subsequent run, the prior override will linger and no longer be encoded
 anywhere (in e.g. Terraform where the inherited value is configured nor in the
 DBT project where the override previously existed but now is gone) [create-
 table-as]: https://docs.aws.amazon.com/athena/latest/ug/create-table-
-as.html#ctas-table-properties ### Table location The location in which a table
-is saved is determined by: 1. If `external_location` is defined, that value is
-used. 2. If `s3_data_dir` is defined, the path is determined by that and
+as.html#ctas-table-properties ### Table location The location a table is saved
+to is determined by: 1. If `external_location` is defined, that value is used
+2. If `s3_data_dir` is defined, the path is determined by that and
 `s3_data_naming` 3. If `s3_data_dir` is not defined, data is stored under
 `s3_staging_dir/tables/` Here all the options available for `s3_data_naming`: -
 `unique`: `{s3_data_dir}/{uuid4()}/` - `table`: `{s3_data_dir}/{table}/` -
 `table_unique`: `{s3_data_dir}/{table}/{uuid4()}/` - `schema_table`: `
 {s3_data_dir}/{schema}/{table}/` - `s3_data_naming=schema_table_unique`: `
 {s3_data_dir}/{schema}/{table}/{uuid4()}/` It's possible to set the
 `s3_data_naming` globally in the target profile, or overwrite the value in the
@@ -246,34 +255,34 @@
 %} select * from ( values (1, 'v1-updated') , (2, 'v2-updated') ) as t (id,
 value) {% else %} select * from ( values (-1, 'v-1') , (0, 'v0') , (1, 'v1') ,
 (2, 'v2') ) as t (id, value) {% endif %} ``` `insert_condition` example: ```sql
 {{ config( materialized='incremental', incremental_strategy='merge',
 unique_key=['id'], insert_condition='target.status != 0', schema='sandbox' ) }}
 select * from ( values (1, 0) , (2, 1) ) as t (id, status) ``` ### Highly
 available table (HA) The current implementation of the table materialization
-can lead to downtime, as target table is dropped and re-created. To have the
-less destructive behavior it's possible to use the `ha` config on your `table`
-materialized models. It leverages the table versions feature of glue catalog,
-creating a tmp table and swapping the target table to the location of the tmp
-table. This materialization is only available for `table_type=hive` and
-requires using unique locations. For iceberg, high availability is by default.
-```sql {{ config( materialized='table', ha=true, format='parquet',
+can lead to downtime, as the target table is dropped and re-created. To have
+the less destructive behavior it's possible to use the `ha` config on your
+`table` materialized models. It leverages the table versions feature of glue
+catalog, creating a temp table and swapping the target table to the location of
+the temp table. This materialization is only available for `table_type=hive`
+and requires using unique locations. For iceberg, high availability is the
+default. ```sql {{ config( materialized='table', ha=true, format='parquet',
 table_type='hive', partitioned_by=['status'], s3_data_naming='table_unique' )
 }} select 'a' as user_id, 'pi' as user_name, 'active' as status union all
 select 'b' as user_id, 'sh' as user_name, 'disabled' as status ``` By default,
 the materialization keeps the last 4 table versions, you can change it by
-setting `versions_to_keep`. #### HA Known issues - When swapping from a table
+setting `versions_to_keep`. #### HA known issues - When swapping from a table
 with partitions to a table without (and the other way around), there could be a
-little downtime. In case high performances are needed consider bucketing
-instead of partitions - By default, Glue "duplicates" the versions internally,
-so the last two versions of a table point to the same location - It's
-recommended to have `versions_to_keep` >= 4, as this will avoid having the
-older location removed ### Update glue data catalog Optionally persist resource
-descriptions as column and relation comments to the glue data catalog, and meta
-as [glue table properties](https://docs.aws.amazon.com/glue/latest/dg/tables-
+little downtime. If high performances is needed consider bucketing instead of
+partitions - By default, Glue "duplicates" the versions internally, so the last
+two versions of a table point to the same location - It's recommended to set
+`versions_to_keep` >= 4, as this will avoid having the older location removed
+### Update glue data catalog Optionally persist resource descriptions as column
+and relation comments to the glue data catalog, and meta as [glue table
+properties](https://docs.aws.amazon.com/glue/latest/dg/tables-
 described.html#table-properties) and [column parameters](https://
 docs.aws.amazon.com/glue/latest/webapi/API_Column.html). By default,
 documentation persistence is disabled, but it can be enabled for specific
 resources or groups of resources as needed. For example: ```yaml models: -
 name: test_deduplicate description: another value config: persist_docs:
 relation: true columns: true meta: test: value columns: - name: id meta:
 primary_key: true ``` See [persist docs](https://docs.getdbt.com/reference/
@@ -304,54 +313,58 @@
 ('model') }} {% endsnapshot %} ``` invalidate hard deletes - model_snapshot_2
 ```sql {% snapshot model_snapshot_2 %} {{ config ( unique_key='id',
 strategy='timestamp', updated_at='refresh_timestamp',
 invalidate_hard_deletes=True, ) }} select * from {{ ref('model') }} {%
 endsnapshot %} ``` check strategy - model_snapshot_3 ```sql {% snapshot
 model_snapshot_3 %} {{ config ( unique_key='id', strategy='check', check_cols=
 ['series_reference','data_value'] ) }} select * from {{ ref('model') }} {%
-endsnapshot %} ``` ### Snapshots Known issues - Incremental Iceberg models -
-Sync all columns on schema change can't remove columns used as partitioning.
+endsnapshot %} ``` ### Snapshots known issues - Incremental Iceberg models -
+Sync all columns on schema change can't remove columns used for partitioning.
 The only way, from a dbt perspective, is to do a full-refresh of the
-incremental model. - Tables, schemas and database should only be lowercase - In
-order to avoid potential conflicts, make sure [`dbt-athena-adapter`](https://
-github.com/Tomme/dbt-athena) is not installed in the target environment. See
+incremental model. - Tables, schemas and database names should only be
+lowercase - In order to avoid potential conflicts, make sure [`dbt-athena-
+adapter`](https://github.com/Tomme/dbt-athena) is not installed in the target
+environment. See
 github.com/dbt-athena/dbt-athena/issues/103> for more details. - Snapshot does
 not support dropping columns from the source table. If you drop a column make
 sure to drop the column from the snapshot as well. Another workaround is to
-NULL the column in the snapshot definition to preserve history ## AWS
-Lakeformation integration The adapter implements AWS Lakeformation tags
-management in the following way: - you can enable or disable lf-tags management
-via [config](#table-configuration) (disabled by default) - once you enable the
-feature, lf-tags will be updated on every dbt run - first, all lf-tags for
-columns are removed to avoid inheritance issues - then all redundant lf-tags
-are removed from table and actual tags from config are applied - finally, lf-
-tags for columns are applied It's important to understand the following points:
-- dbt does not manage lf-tags for database - dbt does not manage lakeformation
-permissions That's why you should handle this by yourself manually or using
-some automation tools like terraform, AWS CDK etc. You may find the following
-links useful to manage that: * [terraform aws_lakeformation_permissions](https:
-//registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/
-lakeformation_permissions) * [terraform aws_lakeformation_resource_lf_tags]
-(https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/
-lakeformation_resource_lf_tags) ## Python Models The adapter supports python
-models using [`spark`](https://docs.aws.amazon.com/athena/latest/ug/notebooks-
-spark.html). ### Setup - A Spark-enabled workgroup created in Athena - Spark
-execution role granted access to Athena, Glue and S3 - The Spark workgroup is
-added to the `~/.dbt/profiles.yml` file and the profile is referenced in
-`dbt_project.yml` that will be created. It is recommended to keep this same as
-threads. ### Spark-specific table configuration - `timeout` (`default=43200`) -
-Time out in seconds for each Python model execution. Defaults to 12 hours/43200
-seconds. - `spark_encryption` (`default=false`) - If this flag is set to true,
-encrypts data in transit between Spark nodes and also encrypts data at rest
-stored locally by Spark. - `spark_cross_account_catalog` (`default=false`) - In
-Spark, you can query the external account catalog and for that the consumer
-account has to be configured to access the producer catalog. - If this flag is
-set to true, "/" can be used as the glue catalog separator. Ex: 999999999999/
-mydatabase.cloudfront_logs (*where *999999999999* is the external catalog ID*)
-- `spark_requester_pays` (`default=false`) - When an Amazon S3 bucket is
+NULL the column in the snapshot definition to preserve history ## AWS Lake
+Formation integration The adapter implements AWS Lake Formation tags management
+in the following way: - You can enable or disable lf-tags management via
+[config](#table-configuration) (disabled by default) - Once you enable the
+feature, lf-tags will be updated on every dbt run - First, all lf-tags for
+columns are removed to avoid inheritance issues - Then, all redundant lf-tags
+are removed from tables and actual tags from table configs are applied -
+Finally, lf-tags for columns are applied It's important to understand the
+following points: - dbt does not manage lf-tags for databases - dbt does not
+manage Lake Formation permissions That's why you should handle this by yourself
+manually or using an automation tool like terraform, AWS CDK etc. You may find
+the following links useful to manage that: * [terraform
+aws_lakeformation_permissions](https://registry.terraform.io/providers/
+hashicorp/aws/latest/docs/resources/lakeformation_permissions) * [terraform
+aws_lakeformation_resource_lf_tags](https://registry.terraform.io/providers/
+hashicorp/aws/latest/docs/resources/lakeformation_resource_lf_tags) ## Python
+models The adapter supports Python models using [`spark`](https://
+docs.aws.amazon.com/athena/latest/ug/notebooks-spark.html). ### Setup - A
+Spark-enabled workgroup created in Athena - Spark execution role granted access
+to Athena, Glue and S3 - The Spark workgroup is added to the `~/.dbt/
+profiles.yml` file and the profile to be used is referenced in
+`dbt_project.yml` ### Spark-specific table configuration - `timeout`
+(`default=43200`) - Time out in seconds for each Python model execution.
+Defaults to 12 hours/43200 seconds. - `spark_encryption` (`default=false`) - If
+this flag is set to true, encrypts data in transit between Spark nodes and also
+encrypts data at rest stored locally by Spark. - `spark_cross_account_catalog`
+(`default=false`) - When using the Spark Athena workgroup, queries can only be
+made against catalogs located on the same AWS account by default. However,
+sometimes you want to query another catalog located on an external AWS account.
+Setting this additional Spark properties parameter to true will enable querying
+external catalogs. You can use the syntax `external_catalog_id/database.table`
+to access the external table on the external catalog (ex: `999999999999/
+mydatabase.cloudfront_logs` where 999999999999 is the external catalog ID) -
+`spark_requester_pays` (`default=false`) - When an Amazon S3 bucket is
 configured as requester pays, the account of the user running the query is
 charged for data access and data transfer fees associated with the query. - If
 this flag is set to true, requester pays S3 buckets are enabled in Athena for
 Spark. ### Spark notes - A session is created for each unique engine
 configuration defined in the models that are part of the invocation. - A
 session's idle timeout is set to 10 minutes. Within the timeout period, if
 there is a new calculation (Spark Python model) ready for execution and the
@@ -386,29 +399,28 @@
 pyspark.sql.functions import udf from pyspark.sql.functions import col
 udf_with_import = udf(func) data = [(1, "a"), (2, "b"), (3, "c")] cols =
 ["num", "alpha"] df = spark_session.createDataFrame(data, cols) return
 df.withColumn("udf_test_col", udf_with_import(col("alpha"))) ``` ### Known
 issues in Python models - Python models cannot [reference Athena SQL views]
 (https://docs.aws.amazon.com/athena/latest/ug/notebooks-spark.html). - Third-
 party Python libraries can be used, but they must be [included in the pre-
-installed list]([pre-installed list]) or [imported manually]([imported
-manually]). - Python models can only reference or write to tables with names
-meeting the regular expression: `^[0-9a-zA-Z_]+$`. Dashes and special
-characters are not supported by Spark, even though Athena supports them. -
-Incremental models do not fully utilize Spark capabilities. They depend
-partially on existing SQL-based logic which runs on Trino. - Snapshot
-materializations are not supported. - Spark can only reference tables within
-the same catalog. [pre-installed list]: https://docs.aws.amazon.com/athena/
-latest/ug/notebooks-spark-preinstalled-python-libraries.html [imported
-manually]: https://docs.aws.amazon.com/athena/latest/ug/notebooks-import-files-
-libraries.html ## Contracts The adapter partly supports contract definition. -
-Concerning the `data_type`, it is supported but needs to be adjusted for
-complex types. They must be specified entirely (for instance `array`) even
-though they won't be checked. Indeed, as dbt recommends, we only compare the
-broader type (array, map, int, varchar). The complete definition is used in
-order to check that the data types defined in athena are ok (pre-flight check).
-- the adapter does not support the constraints since no constraints don't exist
-in Athena. ## Contributing See [CONTRIBUTING](CONTRIBUTING.md) for more
-information on how to contribute to this project. ## Contributors â¨ Thanks
-goes to these wonderful people ([emoji key](https://allcontributors.org/docs/
-en/emoji-key)): _[_h_t_t_p_s_:_/_/_c_o_n_t_r_i_b_._r_o_c_k_s_/_i_m_a_g_e_?_r_e_p_o_=_d_b_t_-_a_t_h_e_n_a_/_d_b_t_-
-_a_t_h_e_n_a_]Contributions of any kind welcome!
+installed list][pre-installed list] or [imported manually][imported manually].
+- Python models can only reference or write to tables with names meeting the
+regular expression: `^[0-9a-zA-Z_]+$`. Dashes and special characters are not
+supported by Spark, even though Athena supports them. - Incremental models do
+not fully utilize Spark capabilities. They depend partially on existing SQL-
+based logic which runs on Trino. - Snapshot materializations are not supported.
+- Spark can only reference tables within the same catalog. [pre-installed
+list]: https://docs.aws.amazon.com/athena/latest/ug/notebooks-spark-
+preinstalled-python-libraries.html [imported manually]: https://
+docs.aws.amazon.com/athena/latest/ug/notebooks-import-files-libraries.html ##
+Contracts The adapter partly supports contract definitions: - `data_type` is
+supported but needs to be adjusted for complex types. Types must be specified
+entirely (for instance `array`) even though they won't be checked. Indeed, as
+dbt recommends, we only compare the broader type (array, map, int, varchar).
+The complete definition is used in order to check that the data types defined
+in Athena are ok (pre-flight check). - The adapter does not support the
+constraints since there is no constraint concept in Athena. ## Contributing See
+[CONTRIBUTING](CONTRIBUTING.md) for more information on how to contribute to
+this project. ## Contributors â¨ Thanks goes to these wonderful people ([emoji
+key](https://allcontributors.org/docs/en/emoji-key)): _[_h_t_t_p_s_:_/_/_c_o_n_t_r_i_b_._r_o_c_k_s_/
+_i_m_a_g_e_?_r_e_p_o_=_d_b_t_-_a_t_h_e_n_a_/_d_b_t_-_a_t_h_e_n_a_]Contributions of any kind welcome!
```

### Comparing `dbt_athena_community-1.8.1/README.md` & `dbt_athena_community-1.8.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,57 +15,57 @@
     <a href="https://pepy.tech/project/dbt-athena-community">
       <img src="https://static.pepy.tech/badge/dbt-athena-community/month" />
     </a>
 </p>
 <!-- TOC -->
 
 - [Features](#features)
-  - [Quick Start](#quick-start)
+  - [Quick start](#quick-start)
     - [Installation](#installation)
     - [Prerequisites](#prerequisites)
     - [Credentials](#credentials)
     - [Configuring your profile](#configuring-your-profile)
     - [Additional information](#additional-information)
   - [Models](#models)
-    - [Table Configuration](#table-configuration)
+    - [Table configuration](#table-configuration)
     - [Table location](#table-location)
     - [Incremental models](#incremental-models)
     - [On schema change](#on-schema-change)
     - [Iceberg](#iceberg)
     - [Highly available table (HA)](#highly-available-table-ha)
-      - [HA Known issues](#ha-known-issues)
+      - [HA known issues](#ha-known-issues)
     - [Update glue data catalog](#update-glue-data-catalog)
   - [Snapshots](#snapshots)
     - [Timestamp strategy](#timestamp-strategy)
     - [Check strategy](#check-strategy)
     - [Hard-deletes](#hard-deletes)
     - [Working example](#working-example)
-    - [Snapshots Known issues](#snapshots-known-issues)
-  - [AWS Lakeformation integration](#aws-lakeformation-integration)
-  - [Python Models](#python-models)
+    - [Snapshots known issues](#snapshots-known-issues)
+  - [AWS Lake Formation integration](#aws-lake-formation-integration)
+  - [Python models](#python-models)
   - [Contracts](#contracts)
   - [Contributing](#contributing)
   - [Contributors ✨](#contributors-)
 <!-- TOC -->
 
 # Features
 
 - Supports dbt version `1.7.*`
 - Support for Python
 - Supports [seeds][seeds]
 - Correctly detects views and their columns
 - Supports [table materialization][table]
   - [Iceberg tables][athena-iceberg] are supported **only with Athena Engine v3** and **a unique table location**
     (see table location section below)
-  - Hive tables are supported by both Athena engines.
+  - Hive tables are supported by both Athena engines
 - Supports [incremental models][incremental]
-  - On Iceberg tables :
+  - On Iceberg tables:
     - Supports the use of `unique_key` only with the `merge` strategy
     - Supports the `append` strategy
-  - On Hive tables :
+  - On Hive tables:
     - Supports two incremental update strategies: `insert_overwrite` and `append`
     - Does **not** support the use of `unique_key`
 - Supports [snapshots][snapshots]
 - Supports [Python models][python-models]
 
 [seeds]: https://docs.getdbt.com/docs/building-a-dbt-project/seeds
 
@@ -75,15 +75,15 @@
 
 [python-models]: https://docs.getdbt.com/docs/build/python-models#configuring-python-models
 
 [athena-iceberg]: https://docs.aws.amazon.com/athena/latest/ug/querying-iceberg.html
 
 [snapshots]: https://docs.getdbt.com/docs/build/snapshots
 
-## Quick Start
+## Quick start
 
 ### Installation
 
 - `pip install dbt-athena-community`
 - Or `pip install git+https://github.com/dbt-athena/dbt-athena.git`
 
 ### Prerequisites
@@ -106,40 +106,41 @@
 ### Credentials
 
 Credentials can be passed directly to the adapter, or they can
 be [determined automatically](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/credentials.html) based
 on `aws cli`/`boto3` conventions.
 You can either:
 
-- configure `aws_access_key_id` and `aws_secret_access_key`
-- configure `aws_profile_name` to match a profile defined in your AWS credentials file
+- Configure `aws_access_key_id` and `aws_secret_access_key`
+- Configure `aws_profile_name` to match a profile defined in your AWS credentials file.
   Checkout dbt profile configuration below for details.
 
 ### Configuring your profile
 
 A dbt profile can be configured to run against AWS Athena using the following configuration:
 
 | Option                | Description                                                                              | Required? | Example                                    |
-| --------------------- | ---------------------------------------------------------------------------------------- | --------- | ------------------------------------------ |
+|-----------------------|------------------------------------------------------------------------------------------|-----------|--------------------------------------------|
 | s3_staging_dir        | S3 location to store Athena query results and metadata                                   | Required  | `s3://bucket/dbt/`                         |
 | s3_data_dir           | Prefix for storing tables, if different from the connection's `s3_staging_dir`           | Optional  | `s3://bucket2/dbt/`                        |
 | s3_data_naming        | How to generate table paths in `s3_data_dir`                                             | Optional  | `schema_table_unique`                      |
 | s3_tmp_table_dir      | Prefix for storing temporary tables, if different from the connection's `s3_data_dir`    | Optional  | `s3://bucket3/dbt/`                        |
 | region_name           | AWS region of your Athena instance                                                       | Required  | `eu-west-1`                                |
 | schema                | Specify the schema (Athena database) to build models into (lowercase **only**)           | Required  | `dbt`                                      |
 | database              | Specify the database (Data catalog) to build models into (lowercase **only**)            | Required  | `awsdatacatalog`                           |
 | poll_interval         | Interval in seconds to use for polling the status of query results in Athena             | Optional  | `5`                                        |
 | debug_query_state     | Flag if debug message with Athena query state is needed                                  | Optional  | `false`                                    |
-| aws_access_key_id     | Access key ID of the user performing requests.                                           | Optional  | `AKIAIOSFODNN7EXAMPLE`                     |
+| aws_access_key_id     | Access key ID of the user performing requests                                            | Optional  | `AKIAIOSFODNN7EXAMPLE`                     |
 | aws_secret_access_key | Secret access key of the user performing requests                                        | Optional  | `wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY` |
-| aws_profile_name      | Profile to use from your AWS shared credentials file.                                    | Optional  | `my-profile`                               |
+| aws_profile_name      | Profile to use from your AWS shared credentials file                                     | Optional  | `my-profile`                               |
 | work_group            | Identifier of Athena workgroup                                                           | Optional  | `my-custom-workgroup`                      |
 | num_retries           | Number of times to retry a failing query                                                 | Optional  | `3`                                        |
-| spark_work_group      | Identifier of Athena Spark workgroup                                           | Optional  | `my-spark-workgroup`                       |
 | num_boto3_retries     | Number of times to retry boto3 requests (e.g. deleting S3 files for materialized tables) | Optional  | `5`                                        |
+| num_iceberg_retries   | Number of times to retry iceberg commit queries to fix ICEBERG_COMMIT_ERROR              | Optional  | `0`                                        |
+| spark_work_group      | Identifier of Athena Spark workgroup for running Python models                           | Optional  | `my-spark-workgroup`                       |
 | seed_s3_upload_args   | Dictionary containing boto3 ExtraArgs when uploading to S3                               | Optional  | `{"ACL": "bucket-owner-full-control"}`     |
 | lf_tags_database      | Default LF tags for new database if it's created by dbt                                  | Optional  | `tag_key: tag_value`                       |
 
 **Example profiles.yml entry:**
 
 ```yaml
 athena:
@@ -165,20 +166,20 @@
 ### Additional information
 
 - `threads` is supported
 - `database` and `catalog` can be used interchangeably
 
 ## Models
 
-### Table Configuration
+### Table configuration
 
 - `external_location` (`default=none`)
-  - If set, the full S3 path in which the table will be saved.
-  - It works only with incremental models.
-  - Does not work with Hive table with `ha` set to true.
+  - If set, the full S3 path to which the table will be saved
+  - Works only with incremental models
+  - Does not work with Hive table with `ha` set to true
 - `partitioned_by` (`default=none`)
   - An array list of columns by which the table will be partitioned
   - Limited to creation of 100 partitions (*currently*)
 - `bucketed_by` (`default=none`)
   - An array list of columns to bucket data, ignored if using Iceberg
 - `bucket_count` (`default=none`)
   - The number of buckets for bucketing your data, ignored if using Iceberg
@@ -198,23 +199,31 @@
   - Custom field delimiter, for when format is set to `TEXTFILE`
 - `table_properties`: table properties to add to the table, valid for Iceberg only
 - `native_drop`: Relation drop operations will be performed with SQL, not direct Glue API calls. No S3 calls will be
   made to manage data in S3. Data in S3 will only be cleared up for Iceberg
   tables [see AWS docs](https://docs.aws.amazon.com/athena/latest/ug/querying-iceberg-managing-tables.html). Note that
   Iceberg DROP TABLE operations may timeout if they take longer than 60 seconds.
 - `seed_by_insert` (`default=false`)
-  - default behaviour uploads seed data to S3. This flag will create seeds using an SQL insert statement
-  - large seed files cannot use `seed_by_insert`, as the SQL insert statement would
+  - Default behaviour uploads seed data to S3. This flag will create seeds using an SQL insert statement
+  - Large seed files cannot use `seed_by_insert`, as the SQL insert statement would
     exceed [the Athena limit of 262144 bytes](https://docs.aws.amazon.com/athena/latest/ug/service-limits.html)
 - `force_batch` (`default=false`)
-  - Skip creating the table as ctas and run the operation directly in batch insert mode.
+  - Skip creating the table as CTAS and run the operation directly in batch insert mode
   - This is particularly useful when the standard table creation process fails due to partition limitations,
-  allowing you to work with temporary tables and persist the dataset more efficiently.
+  allowing you to work with temporary tables and persist the dataset more efficiently
+- `unique_tmp_table_suffix` (`default=false`)
+  - For incremental models using insert overwrite strategy on hive table
+  - Replace the __dbt_tmp suffix used as temporary table name suffix by a unique uuid
+  - Useful if you are looking to run multiple dbt build inserting in the same table in parallel
+- `temp_schema` (`default=none`)
+  - For incremental models, it allows to define a schema to hold temporary create statements
+  used in incremental model runs
+  - Schema will be created in the model target database if does not exist
 - `lf_tags_config` (`default=none`)
-  - [AWS lakeformation](#aws-lakeformation-integration) tags to associate with the table and columns
+  - [AWS Lake Formation](#aws-lake-formation-integration) tags to associate with the table and columns
   - `enabled` (`default=False`) whether LF tags management is enabled for a model
   - `tags` dictionary with tags and their values to assign for the model
   - `tags_columns` dictionary with a tag key, value and list of columns they must be assigned to
   - `lf_inherited_tags` (`default=none`)
     - List of Lake Formation tag keys that are intended to be inherited from the database level and thus shouldn't be
       removed during association of those defined in `lf_tags_config`
       - i.e., the default behavior of `lf_tags_config` is to be exhaustive and first remove any pre-existing tags from
@@ -243,31 +252,31 @@
           },
           'inherited_tags': ['tag1', 'tag2']
     }
   )
 }}
 ```
 
-- format for `dbt_project.yml`:
+- Format for `dbt_project.yml`:
 
 ```yaml
   +lf_tags_config:
     enabled: true
     tags:
       tag1: value1
       tag2: value2
     tags_columns:
       tag1:
         value1: [ column1, column2 ]
     inherited_tags: [ tag1, tag2 ]
 ```
 
 - `lf_grants` (`default=none`)
-  - lakeformation grants config for data_cell filters
-  - format:
+  - Lake Formation grants config for data_cell filters
+  - Format:
 
   ```python
   lf_grants={
           'data_cell_filters': {
               'enabled': True | False,
               'filters': {
                   'filter_name': {
@@ -298,17 +307,17 @@
       where the inherited value is configured nor in the DBT project where the override previously existed but now is
       gone)
 
 [create-table-as]: https://docs.aws.amazon.com/athena/latest/ug/create-table-as.html#ctas-table-properties
 
 ### Table location
 
-The location in which a table is saved is determined by:
+The location a table is saved to is determined by:
 
-1. If `external_location` is defined, that value is used.
+1. If `external_location` is defined, that value is used
 2. If `s3_data_dir` is defined, the path is determined by that and `s3_data_naming`
 3. If `s3_data_dir` is not defined, data is stored under `s3_staging_dir/tables/`
 
 Here all the options available for `s3_data_naming`:
 
 - `unique`: `{s3_data_dir}/{uuid4()}/`
 - `table`: `{s3_data_dir}/{table}/`
@@ -468,19 +477,20 @@
     , (2, 1)
 ) as t (id, status)
 
 ```
 
 ### Highly available table (HA)
 
-The current implementation of the table materialization can lead to downtime, as target table is dropped and re-created.
-To have the less destructive behavior it's possible to use the `ha` config on your `table` materialized models.
-It leverages the table versions feature of glue catalog, creating a tmp table and swapping the target table to the
-location of the tmp table. This materialization is only available for `table_type=hive` and requires using unique
-locations. For iceberg, high availability is by default.
+The current implementation of the table materialization can lead to downtime, as the target table is
+dropped and re-created. To have the less destructive behavior it's possible to use the `ha` config on
+your `table` materialized models. It leverages the table versions feature of glue catalog, creating
+a temp table and swapping the target table to the location of the temp table. This materialization
+is only available for `table_type=hive` and requires using unique locations. For iceberg, high
+availability is the default.
 
 ```sql
 {{ config(
     materialized='table',
     ha=true,
     format='parquet',
     table_type='hive',
@@ -495,21 +505,21 @@
 select 'b'        as user_id,
        'sh'       as user_name,
        'disabled' as status
 ```
 
 By default, the materialization keeps the last 4 table versions, you can change it by setting `versions_to_keep`.
 
-#### HA Known issues
+#### HA known issues
 
 - When swapping from a table with partitions to a table without (and the other way around), there could be a little
   downtime.
-  In case high performances are needed consider bucketing instead of partitions
+  If high performances is needed consider bucketing instead of partitions
 - By default, Glue "duplicates" the versions internally, so the last two versions of a table point to the same location
-- It's recommended to have `versions_to_keep` >= 4, as this will avoid having the older location removed
+- It's recommended to set `versions_to_keep` >= 4, as this will avoid having the older location removed
 
 ### Update glue data catalog
 
 Optionally persist resource descriptions as column and relation comments to the glue data catalog, and meta as
 [glue table properties](https://docs.aws.amazon.com/glue/latest/dg/tables-described.html#table-properties)
 and [column parameters](https://docs.aws.amazon.com/glue/latest/webapi/API_Column.html).
 By default, documentation persistence is disabled, but it can be enabled for specific resources or
@@ -642,74 +652,75 @@
         check_cols=['series_reference','data_value']
     )
 }}
 select *
 from {{ ref('model') }} {% endsnapshot %}
 ```
 
-### Snapshots Known issues
+### Snapshots known issues
 
-- Incremental Iceberg models - Sync all columns on schema change can't remove columns used as partitioning.
+- Incremental Iceberg models - Sync all columns on schema change can't remove columns used for partitioning.
   The only way, from a dbt perspective, is to do a full-refresh of the incremental model.
 
-- Tables, schemas and database should only be lowercase
+- Tables, schemas and database names should only be lowercase
 
 - In order to avoid potential conflicts, make sure [`dbt-athena-adapter`](https://github.com/Tomme/dbt-athena) is not
   installed in the target environment.
   See <https://github.com/dbt-athena/dbt-athena/issues/103> for more details.
 
 - Snapshot does not support dropping columns from the source table. If you drop a column make sure to drop the column
   from the snapshot as well. Another workaround is to NULL the column in the snapshot definition to preserve history
 
-## AWS Lakeformation integration
+## AWS Lake Formation integration
 
-The adapter implements AWS Lakeformation tags management in the following way:
+The adapter implements AWS Lake Formation tags management in the following way:
 
-- you can enable or disable lf-tags management via [config](#table-configuration) (disabled by default)
-- once you enable the feature, lf-tags will be updated on every dbt run
-- first, all lf-tags for columns are removed to avoid inheritance issues
-- then all redundant lf-tags are removed from table and actual tags from config are applied
-- finally, lf-tags for columns are applied
+- You can enable or disable lf-tags management via [config](#table-configuration) (disabled by default)
+- Once you enable the feature, lf-tags will be updated on every dbt run
+- First, all lf-tags for columns are removed to avoid inheritance issues
+- Then, all redundant lf-tags are removed from tables and actual tags from table configs are applied
+- Finally, lf-tags for columns are applied
 
 It's important to understand the following points:
 
-- dbt does not manage lf-tags for database
-- dbt does not manage lakeformation permissions
+- dbt does not manage lf-tags for databases
+- dbt does not manage Lake Formation permissions
 
-That's why you should handle this by yourself manually or using some automation tools like terraform, AWS CDK etc.
+That's why you should handle this by yourself manually or using an automation tool like terraform, AWS CDK etc.
 You may find the following links useful to manage that:
 
 <!-- markdownlint-disable -->
 * [terraform aws_lakeformation_permissions](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lakeformation_permissions)
 * [terraform aws_lakeformation_resource_lf_tags](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lakeformation_resource_lf_tags)
 <!-- markdownlint-restore -->
 
-## Python Models
+## Python models
 
-The adapter supports python models using [`spark`](https://docs.aws.amazon.com/athena/latest/ug/notebooks-spark.html).
+The adapter supports Python models using [`spark`](https://docs.aws.amazon.com/athena/latest/ug/notebooks-spark.html).
 
 ### Setup
 
 - A Spark-enabled workgroup created in Athena
 - Spark execution role granted access to Athena, Glue and S3
-- The Spark workgroup is added to the `~/.dbt/profiles.yml` file and the profile
- is referenced in `dbt_project.yml` that will be created. It is recommended to keep this same as threads.
+- The Spark workgroup is added to the `~/.dbt/profiles.yml` file and the profile to be used
+  is referenced in `dbt_project.yml`
 
 ### Spark-specific table configuration
 
 - `timeout` (`default=43200`)
   - Time out in seconds for each Python model execution. Defaults to 12 hours/43200 seconds.
 - `spark_encryption` (`default=false`)
   - If this flag is set to true, encrypts data in transit between Spark nodes and also encrypts data at rest stored
    locally by Spark.
 - `spark_cross_account_catalog` (`default=false`)
-  - In Spark, you can query the external account catalog and for that the consumer account has to be configured to
-   access the producer catalog.
-  - If this flag is set to true, "/" can be used as the glue catalog separator.
-   Ex: 999999999999/mydatabase.cloudfront_logs (*where *999999999999* is the external catalog ID*)
+  - When using the Spark Athena workgroup, queries can only be made against catalogs located on the same
+    AWS account by default. However, sometimes you want to query another catalog located on an external AWS
+    account. Setting this additional Spark properties parameter to true will enable querying external catalogs.
+    You can use the syntax `external_catalog_id/database.table` to access the external table on the external
+    catalog (ex: `999999999999/mydatabase.cloudfront_logs` where 999999999999 is the external catalog ID)
 - `spark_requester_pays` (`default=false`)
   - When an Amazon S3 bucket is configured as requester pays, the account of the user running the query is charged for
    data access and data transfer fees associated with the query.
   - If this flag is set to true, requester pays S3 buckets are enabled in Athena for Spark.
 
 ### Spark notes
 
@@ -822,36 +833,36 @@
     return df.withColumn("udf_test_col", udf_with_import(col("alpha")))
 ```
 
 ### Known issues in Python models
 
 - Python models cannot
  [reference Athena SQL views](https://docs.aws.amazon.com/athena/latest/ug/notebooks-spark.html).
-- Third-party Python libraries can be used, but they must be [included in the pre-installed list]([pre-installed list])
- or [imported manually]([imported manually]).
+- Third-party Python libraries can be used, but they must be [included in the pre-installed list][pre-installed list]
+ or [imported manually][imported manually].
 - Python models can only reference or write to tables with names meeting the
  regular expression: `^[0-9a-zA-Z_]+$`. Dashes and special characters are not
  supported by Spark, even though Athena supports them.
 - Incremental models do not fully utilize Spark capabilities. They depend partially on existing SQL-based logic which
  runs on Trino.
 - Snapshot materializations are not supported.
 - Spark can only reference tables within the same catalog.
 
 [pre-installed list]: https://docs.aws.amazon.com/athena/latest/ug/notebooks-spark-preinstalled-python-libraries.html
 [imported manually]: https://docs.aws.amazon.com/athena/latest/ug/notebooks-import-files-libraries.html
 
 ## Contracts
 
-The adapter partly supports contract definition.
+The adapter partly supports contract definitions:
 
-- Concerning the `data_type`, it is supported but needs to be adjusted for complex types. They must be specified
+- `data_type` is supported but needs to be adjusted for complex types. Types must be specified
   entirely (for instance `array<int>`) even though they won't be checked. Indeed, as dbt recommends, we only compare
   the broader type (array, map, int, varchar). The complete definition is used in order to check that the data types
-  defined in athena are ok (pre-flight check).
-- the adapter does not support the constraints since no constraints don't exist in Athena.
+  defined in Athena are ok (pre-flight check).
+- The adapter does not support the constraints since there is no constraint concept in Athena.
 
 ## Contributing
 
 See [CONTRIBUTING](CONTRIBUTING.md) for more information on how to contribute to this project.
 
 ## Contributors ✨
```

#### html2text {}

```diff
@@ -1,100 +1,102 @@
  [https://raw.githubusercontent.com/dbt-athena/dbt-athena/main/static/images/
 dbt-athena-long.png]_[_h_t_t_p_s_:_/_/_b_a_d_g_e_._f_u_r_y_._i_o_/_p_y_/_d_b_t_-_a_t_h_e_n_a_-_c_o_m_m_u_n_i_t_y_._s_v_g_]_[_h_t_t_p_s_:_/
  _/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_d_b_t_-_a_t_h_e_n_a_-_c_o_m_m_u_n_i_t_y_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
     _b_a_d_g_e_/_%_2_0_i_m_p_o_r_t_s_-_i_s_o_r_t_-_%_2_3_1_6_7_4_b_1_?_s_t_y_l_e_=_f_l_a_t_&_l_a_b_e_l_C_o_l_o_r_=_e_f_8_3_3_6_]_[_h_t_t_p_s_:_/_/
 _i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_c_o_d_e_%_2_0_s_t_y_l_e_-_b_l_a_c_k_-_0_0_0_0_0_0_._s_v_g_]_[_h_t_t_p_s_:_/_/_w_w_w_._m_y_p_y_-_l_a_n_g_._o_r_g_/
   _s_t_a_t_i_c_/_m_y_p_y___b_a_d_g_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_s_t_a_t_i_c_._p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/_d_b_t_-_a_t_h_e_n_a_-_c_o_m_m_u_n_i_t_y_/
                                     _m_o_n_t_h_]
-- [Features](#features) - [Quick Start](#quick-start) - [Installation]
+- [Features](#features) - [Quick start](#quick-start) - [Installation]
 (#installation) - [Prerequisites](#prerequisites) - [Credentials](#credentials)
 - [Configuring your profile](#configuring-your-profile) - [Additional
 information](#additional-information) - [Models](#models) - [Table
-Configuration](#table-configuration) - [Table location](#table-location) -
+configuration](#table-configuration) - [Table location](#table-location) -
 [Incremental models](#incremental-models) - [On schema change](#on-schema-
 change) - [Iceberg](#iceberg) - [Highly available table (HA)](#highly-
-available-table-ha) - [HA Known issues](#ha-known-issues) - [Update glue data
+available-table-ha) - [HA known issues](#ha-known-issues) - [Update glue data
 catalog](#update-glue-data-catalog) - [Snapshots](#snapshots) - [Timestamp
 strategy](#timestamp-strategy) - [Check strategy](#check-strategy) - [Hard-
 deletes](#hard-deletes) - [Working example](#working-example) - [Snapshots
-Known issues](#snapshots-known-issues) - [AWS Lakeformation integration](#aws-
-lakeformation-integration) - [Python Models](#python-models) - [Contracts]
+known issues](#snapshots-known-issues) - [AWS Lake Formation integration](#aws-
+lake-formation-integration) - [Python models](#python-models) - [Contracts]
 (#contracts) - [Contributing](#contributing) - [Contributors â¨]
 (#contributors-) # Features - Supports dbt version `1.7.*` - Support for Python
 - Supports [seeds][seeds] - Correctly detects views and their columns -
 Supports [table materialization][table] - [Iceberg tables][athena-iceberg] are
 supported **only with Athena Engine v3** and **a unique table location** (see
 table location section below) - Hive tables are supported by both Athena
-engines. - Supports [incremental models][incremental] - On Iceberg tables : -
+engines - Supports [incremental models][incremental] - On Iceberg tables: -
 Supports the use of `unique_key` only with the `merge` strategy - Supports the
-`append` strategy - On Hive tables : - Supports two incremental update
+`append` strategy - On Hive tables: - Supports two incremental update
 strategies: `insert_overwrite` and `append` - Does **not** support the use of
 `unique_key` - Supports [snapshots][snapshots] - Supports [Python models]
 [python-models] [seeds]: https://docs.getdbt.com/docs/building-a-dbt-project/
 seeds [incremental]: https://docs.getdbt.com/docs/build/incremental-models
 [table]: https://docs.getdbt.com/docs/build/materializations#table [python-
 models]: https://docs.getdbt.com/docs/build/python-models#configuring-python-
 models [athena-iceberg]: https://docs.aws.amazon.com/athena/latest/ug/querying-
 iceberg.html [snapshots]: https://docs.getdbt.com/docs/build/snapshots ## Quick
-Start ### Installation - `pip install dbt-athena-community` - Or `pip install
+start ### Installation - `pip install dbt-athena-community` - Or `pip install
 git+https://github.com/dbt-athena/dbt-athena.git` ### Prerequisites To start,
 you will need an S3 bucket, for instance `my-bucket` and an Athena database:
 ```sql CREATE DATABASE IF NOT EXISTS analytics_dev COMMENT 'Analytics models
 generated by dbt (development)' LOCATION 's3://my-bucket/' WITH DBPROPERTIES
 ('creator'='Foo Bar', 'email'='foo@bar.com'); ``` Notes: - Take note of your
 AWS region code (e.g. `us-west-2` or `eu-west-2`, etc.). - You can also use
 [AWS Glue](https://docs.aws.amazon.com/athena/latest/ug/glue-athena.html) to
 create and manage Athena databases. ### Credentials Credentials can be passed
 directly to the adapter, or they can be [determined automatically](https://
 boto3.amazonaws.com/v1/documentation/api/latest/guide/credentials.html) based
-on `aws cli`/`boto3` conventions. You can either: - configure
-`aws_access_key_id` and `aws_secret_access_key` - configure `aws_profile_name`
-to match a profile defined in your AWS credentials file Checkout dbt profile
+on `aws cli`/`boto3` conventions. You can either: - Configure
+`aws_access_key_id` and `aws_secret_access_key` - Configure `aws_profile_name`
+to match a profile defined in your AWS credentials file. Checkout dbt profile
 configuration below for details. ### Configuring your profile A dbt profile can
 be configured to run against AWS Athena using the following configuration: |
-Option | Description | Required? | Example | | --------------------- | --------
+Option | Description | Required? | Example | |-----------------------|---------
 -------------------------------------------------------------------------------
-- | --------- | ------------------------------------------ | | s3_staging_dir |
+--|-----------|--------------------------------------------| | s3_staging_dir |
 S3 location to store Athena query results and metadata | Required | `s3://
 bucket/dbt/` | | s3_data_dir | Prefix for storing tables, if different from the
 connection's `s3_staging_dir` | Optional | `s3://bucket2/dbt/` | |
 s3_data_naming | How to generate table paths in `s3_data_dir` | Optional |
 `schema_table_unique` | | s3_tmp_table_dir | Prefix for storing temporary
 tables, if different from the connection's `s3_data_dir` | Optional | `s3://
 bucket3/dbt/` | | region_name | AWS region of your Athena instance | Required |
 `eu-west-1` | | schema | Specify the schema (Athena database) to build models
 into (lowercase **only**) | Required | `dbt` | | database | Specify the
 database (Data catalog) to build models into (lowercase **only**) | Required |
 `awsdatacatalog` | | poll_interval | Interval in seconds to use for polling the
 status of query results in Athena | Optional | `5` | | debug_query_state | Flag
 if debug message with Athena query state is needed | Optional | `false` | |
-aws_access_key_id | Access key ID of the user performing requests. | Optional |
+aws_access_key_id | Access key ID of the user performing requests | Optional |
 `AKIAIOSFODNN7EXAMPLE` | | aws_secret_access_key | Secret access key of the
 user performing requests | Optional | `wJalrXUtnFEMI/K7MDENG/
 bPxRfiCYEXAMPLEKEY` | | aws_profile_name | Profile to use from your AWS shared
-credentials file. | Optional | `my-profile` | | work_group | Identifier of
+credentials file | Optional | `my-profile` | | work_group | Identifier of
 Athena workgroup | Optional | `my-custom-workgroup` | | num_retries | Number of
-times to retry a failing query | Optional | `3` | | spark_work_group |
-Identifier of Athena Spark workgroup | Optional | `my-spark-workgroup` | |
-num_boto3_retries | Number of times to retry boto3 requests (e.g. deleting S3
-files for materialized tables) | Optional | `5` | | seed_s3_upload_args |
-Dictionary containing boto3 ExtraArgs when uploading to S3 | Optional | `
-{"ACL": "bucket-owner-full-control"}` | | lf_tags_database | Default LF tags
-for new database if it's created by dbt | Optional | `tag_key: tag_value` |
-**Example profiles.yml entry:** ```yaml athena: target: dev outputs: dev: type:
-athena s3_staging_dir: s3://athena-query-results/dbt/ s3_data_dir: s3://
+times to retry a failing query | Optional | `3` | | num_boto3_retries | Number
+of times to retry boto3 requests (e.g. deleting S3 files for materialized
+tables) | Optional | `5` | | num_iceberg_retries | Number of times to retry
+iceberg commit queries to fix ICEBERG_COMMIT_ERROR | Optional | `0` | |
+spark_work_group | Identifier of Athena Spark workgroup for running Python
+models | Optional | `my-spark-workgroup` | | seed_s3_upload_args | Dictionary
+containing boto3 ExtraArgs when uploading to S3 | Optional | `{"ACL": "bucket-
+owner-full-control"}` | | lf_tags_database | Default LF tags for new database
+if it's created by dbt | Optional | `tag_key: tag_value` | **Example
+profiles.yml entry:** ```yaml athena: target: dev outputs: dev: type: athena
+s3_staging_dir: s3://athena-query-results/dbt/ s3_data_dir: s3://
 your_s3_bucket/dbt/ s3_data_naming: schema_table s3_tmp_table_dir: s3://
 your_s3_bucket/temp/ region_name: eu-west-1 schema: dbt database:
 awsdatacatalog threads: 4 aws_profile_name: my-profile work_group: my-workgroup
 spark_work_group: my-spark-workgroup seed_s3_upload_args: ACL: bucket-owner-
 full-control ``` ### Additional information - `threads` is supported -
 `database` and `catalog` can be used interchangeably ## Models ### Table
-Configuration - `external_location` (`default=none`) - If set, the full S3 path
-in which the table will be saved. - It works only with incremental models. -
-Does not work with Hive table with `ha` set to true. - `partitioned_by`
+configuration - `external_location` (`default=none`) - If set, the full S3 path
+to which the table will be saved - Works only with incremental models - Does
+not work with Hive table with `ha` set to true - `partitioned_by`
 (`default=none`) - An array list of columns by which the table will be
 partitioned - Limited to creation of 100 partitions (*currently*) -
 `bucketed_by` (`default=none`) - An array list of columns to bucket data,
 ignored if using Iceberg - `bucket_count` (`default=none`) - The number of
 buckets for bucketing your data, ignored if using Iceberg - `table_type`
 (`default='hive'`) - The type of table - Supports `hive` or `iceberg` - `ha`
 (`default=false`) - If the table should be built using the high-availability
@@ -108,24 +110,31 @@
 Custom field delimiter, for when format is set to `TEXTFILE` -
 `table_properties`: table properties to add to the table, valid for Iceberg
 only - `native_drop`: Relation drop operations will be performed with SQL, not
 direct Glue API calls. No S3 calls will be made to manage data in S3. Data in
 S3 will only be cleared up for Iceberg tables [see AWS docs](https://
 docs.aws.amazon.com/athena/latest/ug/querying-iceberg-managing-tables.html).
 Note that Iceberg DROP TABLE operations may timeout if they take longer than 60
-seconds. - `seed_by_insert` (`default=false`) - default behaviour uploads seed
-data to S3. This flag will create seeds using an SQL insert statement - large
+seconds. - `seed_by_insert` (`default=false`) - Default behaviour uploads seed
+data to S3. This flag will create seeds using an SQL insert statement - Large
 seed files cannot use `seed_by_insert`, as the SQL insert statement would
 exceed [the Athena limit of 262144 bytes](https://docs.aws.amazon.com/athena/
 latest/ug/service-limits.html) - `force_batch` (`default=false`) - Skip
-creating the table as ctas and run the operation directly in batch insert mode.
+creating the table as CTAS and run the operation directly in batch insert mode
 - This is particularly useful when the standard table creation process fails
 due to partition limitations, allowing you to work with temporary tables and
-persist the dataset more efficiently. - `lf_tags_config` (`default=none`) -
-[AWS lakeformation](#aws-lakeformation-integration) tags to associate with the
+persist the dataset more efficiently - `unique_tmp_table_suffix`
+(`default=false`) - For incremental models using insert overwrite strategy on
+hive table - Replace the __dbt_tmp suffix used as temporary table name suffix
+by a unique uuid - Useful if you are looking to run multiple dbt build
+inserting in the same table in parallel - `temp_schema` (`default=none`) - For
+incremental models, it allows to define a schema to hold temporary create
+statements used in incremental model runs - Schema will be created in the model
+target database if does not exist - `lf_tags_config` (`default=none`) - [AWS
+Lake Formation](#aws-lake-formation-integration) tags to associate with the
 table and columns - `enabled` (`default=False`) whether LF tags management is
 enabled for a model - `tags` dictionary with tags and their values to assign
 for the model - `tags_columns` dictionary with a tag key, value and list of
 columns they must be assigned to - `lf_inherited_tags` (`default=none`) - List
 of Lake Formation tag keys that are intended to be inherited from the database
 level and thus shouldn't be removed during association of those defined in
 `lf_tags_config` - i.e., the default behavior of `lf_tags_config` is to be
@@ -133,19 +142,19 @@
 before associating the ones currently defined for a given model - This breaks
 tag inheritance as inherited tags appear on tables and columns like those
 associated directly ```sql {{ config( materialized='incremental',
 incremental_strategy='append', on_schema_change='append_new_columns',
 table_type='iceberg', schema='test_schema', lf_tags_config={ 'enabled': true,
 'tags': { 'tag1': 'value1', 'tag2': 'value2' }, 'tags_columns': { 'tag1':
 { 'value1': ['column1', 'column2'], 'value2': ['column3', 'column4'] } },
-'inherited_tags': ['tag1', 'tag2'] } ) }} ``` - format for `dbt_project.yml`:
+'inherited_tags': ['tag1', 'tag2'] } ) }} ``` - Format for `dbt_project.yml`:
 ```yaml +lf_tags_config: enabled: true tags: tag1: value1 tag2: value2
 tags_columns: tag1: value1: [ column1, column2 ] inherited_tags: [ tag1, tag2 ]
-``` - `lf_grants` (`default=none`) - lakeformation grants config for data_cell
-filters - format: ```python lf_grants={ 'data_cell_filters': { 'enabled': True
+``` - `lf_grants` (`default=none`) - Lake Formation grants config for data_cell
+filters - Format: ```python lf_grants={ 'data_cell_filters': { 'enabled': True
 | False, 'filters': { 'filter_name': { 'row_filter': '', 'principals':
 ['principal_arn1', 'principal_arn2'] } } } } ``` > Notes: > > - `lf_tags` and
 `lf_tags_columns` configs support only attaching lf tags to corresponding
 resources. > We recommend managing LF Tags permissions somewhere outside dbt.
 For example, you may use > [terraform](https://registry.terraform.io/providers/
 hashicorp/aws/latest/docs/resources/lakeformation_permissions) or > [aws cdk]
 (https://docs.aws.amazon.com/cdk/api/v1/docs/aws-lakeformation-readme.html) for
@@ -160,17 +169,17 @@
 not differentiate between an inherited tag association and an override of same
 it made > previously > - e.g. If an inherited tag is overridden by an
 `lf_tags_config` value in one DBT run, and that override is removed prior to a
 subsequent run, the prior override will linger and no longer be encoded
 anywhere (in e.g. Terraform where the inherited value is configured nor in the
 DBT project where the override previously existed but now is gone) [create-
 table-as]: https://docs.aws.amazon.com/athena/latest/ug/create-table-
-as.html#ctas-table-properties ### Table location The location in which a table
-is saved is determined by: 1. If `external_location` is defined, that value is
-used. 2. If `s3_data_dir` is defined, the path is determined by that and
+as.html#ctas-table-properties ### Table location The location a table is saved
+to is determined by: 1. If `external_location` is defined, that value is used
+2. If `s3_data_dir` is defined, the path is determined by that and
 `s3_data_naming` 3. If `s3_data_dir` is not defined, data is stored under
 `s3_staging_dir/tables/` Here all the options available for `s3_data_naming`: -
 `unique`: `{s3_data_dir}/{uuid4()}/` - `table`: `{s3_data_dir}/{table}/` -
 `table_unique`: `{s3_data_dir}/{table}/{uuid4()}/` - `schema_table`: `
 {s3_data_dir}/{schema}/{table}/` - `s3_data_naming=schema_table_unique`: `
 {s3_data_dir}/{schema}/{table}/{uuid4()}/` It's possible to set the
 `s3_data_naming` globally in the target profile, or overwrite the value in the
@@ -230,34 +239,34 @@
 %} select * from ( values (1, 'v1-updated') , (2, 'v2-updated') ) as t (id,
 value) {% else %} select * from ( values (-1, 'v-1') , (0, 'v0') , (1, 'v1') ,
 (2, 'v2') ) as t (id, value) {% endif %} ``` `insert_condition` example: ```sql
 {{ config( materialized='incremental', incremental_strategy='merge',
 unique_key=['id'], insert_condition='target.status != 0', schema='sandbox' ) }}
 select * from ( values (1, 0) , (2, 1) ) as t (id, status) ``` ### Highly
 available table (HA) The current implementation of the table materialization
-can lead to downtime, as target table is dropped and re-created. To have the
-less destructive behavior it's possible to use the `ha` config on your `table`
-materialized models. It leverages the table versions feature of glue catalog,
-creating a tmp table and swapping the target table to the location of the tmp
-table. This materialization is only available for `table_type=hive` and
-requires using unique locations. For iceberg, high availability is by default.
-```sql {{ config( materialized='table', ha=true, format='parquet',
+can lead to downtime, as the target table is dropped and re-created. To have
+the less destructive behavior it's possible to use the `ha` config on your
+`table` materialized models. It leverages the table versions feature of glue
+catalog, creating a temp table and swapping the target table to the location of
+the temp table. This materialization is only available for `table_type=hive`
+and requires using unique locations. For iceberg, high availability is the
+default. ```sql {{ config( materialized='table', ha=true, format='parquet',
 table_type='hive', partitioned_by=['status'], s3_data_naming='table_unique' )
 }} select 'a' as user_id, 'pi' as user_name, 'active' as status union all
 select 'b' as user_id, 'sh' as user_name, 'disabled' as status ``` By default,
 the materialization keeps the last 4 table versions, you can change it by
-setting `versions_to_keep`. #### HA Known issues - When swapping from a table
+setting `versions_to_keep`. #### HA known issues - When swapping from a table
 with partitions to a table without (and the other way around), there could be a
-little downtime. In case high performances are needed consider bucketing
-instead of partitions - By default, Glue "duplicates" the versions internally,
-so the last two versions of a table point to the same location - It's
-recommended to have `versions_to_keep` >= 4, as this will avoid having the
-older location removed ### Update glue data catalog Optionally persist resource
-descriptions as column and relation comments to the glue data catalog, and meta
-as [glue table properties](https://docs.aws.amazon.com/glue/latest/dg/tables-
+little downtime. If high performances is needed consider bucketing instead of
+partitions - By default, Glue "duplicates" the versions internally, so the last
+two versions of a table point to the same location - It's recommended to set
+`versions_to_keep` >= 4, as this will avoid having the older location removed
+### Update glue data catalog Optionally persist resource descriptions as column
+and relation comments to the glue data catalog, and meta as [glue table
+properties](https://docs.aws.amazon.com/glue/latest/dg/tables-
 described.html#table-properties) and [column parameters](https://
 docs.aws.amazon.com/glue/latest/webapi/API_Column.html). By default,
 documentation persistence is disabled, but it can be enabled for specific
 resources or groups of resources as needed. For example: ```yaml models: -
 name: test_deduplicate description: another value config: persist_docs:
 relation: true columns: true meta: test: value columns: - name: id meta:
 primary_key: true ``` See [persist docs](https://docs.getdbt.com/reference/
@@ -288,54 +297,58 @@
 ('model') }} {% endsnapshot %} ``` invalidate hard deletes - model_snapshot_2
 ```sql {% snapshot model_snapshot_2 %} {{ config ( unique_key='id',
 strategy='timestamp', updated_at='refresh_timestamp',
 invalidate_hard_deletes=True, ) }} select * from {{ ref('model') }} {%
 endsnapshot %} ``` check strategy - model_snapshot_3 ```sql {% snapshot
 model_snapshot_3 %} {{ config ( unique_key='id', strategy='check', check_cols=
 ['series_reference','data_value'] ) }} select * from {{ ref('model') }} {%
-endsnapshot %} ``` ### Snapshots Known issues - Incremental Iceberg models -
-Sync all columns on schema change can't remove columns used as partitioning.
+endsnapshot %} ``` ### Snapshots known issues - Incremental Iceberg models -
+Sync all columns on schema change can't remove columns used for partitioning.
 The only way, from a dbt perspective, is to do a full-refresh of the
-incremental model. - Tables, schemas and database should only be lowercase - In
-order to avoid potential conflicts, make sure [`dbt-athena-adapter`](https://
-github.com/Tomme/dbt-athena) is not installed in the target environment. See
+incremental model. - Tables, schemas and database names should only be
+lowercase - In order to avoid potential conflicts, make sure [`dbt-athena-
+adapter`](https://github.com/Tomme/dbt-athena) is not installed in the target
+environment. See
 github.com/dbt-athena/dbt-athena/issues/103> for more details. - Snapshot does
 not support dropping columns from the source table. If you drop a column make
 sure to drop the column from the snapshot as well. Another workaround is to
-NULL the column in the snapshot definition to preserve history ## AWS
-Lakeformation integration The adapter implements AWS Lakeformation tags
-management in the following way: - you can enable or disable lf-tags management
-via [config](#table-configuration) (disabled by default) - once you enable the
-feature, lf-tags will be updated on every dbt run - first, all lf-tags for
-columns are removed to avoid inheritance issues - then all redundant lf-tags
-are removed from table and actual tags from config are applied - finally, lf-
-tags for columns are applied It's important to understand the following points:
-- dbt does not manage lf-tags for database - dbt does not manage lakeformation
-permissions That's why you should handle this by yourself manually or using
-some automation tools like terraform, AWS CDK etc. You may find the following
-links useful to manage that: * [terraform aws_lakeformation_permissions](https:
-//registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/
-lakeformation_permissions) * [terraform aws_lakeformation_resource_lf_tags]
-(https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/
-lakeformation_resource_lf_tags) ## Python Models The adapter supports python
-models using [`spark`](https://docs.aws.amazon.com/athena/latest/ug/notebooks-
-spark.html). ### Setup - A Spark-enabled workgroup created in Athena - Spark
-execution role granted access to Athena, Glue and S3 - The Spark workgroup is
-added to the `~/.dbt/profiles.yml` file and the profile is referenced in
-`dbt_project.yml` that will be created. It is recommended to keep this same as
-threads. ### Spark-specific table configuration - `timeout` (`default=43200`) -
-Time out in seconds for each Python model execution. Defaults to 12 hours/43200
-seconds. - `spark_encryption` (`default=false`) - If this flag is set to true,
-encrypts data in transit between Spark nodes and also encrypts data at rest
-stored locally by Spark. - `spark_cross_account_catalog` (`default=false`) - In
-Spark, you can query the external account catalog and for that the consumer
-account has to be configured to access the producer catalog. - If this flag is
-set to true, "/" can be used as the glue catalog separator. Ex: 999999999999/
-mydatabase.cloudfront_logs (*where *999999999999* is the external catalog ID*)
-- `spark_requester_pays` (`default=false`) - When an Amazon S3 bucket is
+NULL the column in the snapshot definition to preserve history ## AWS Lake
+Formation integration The adapter implements AWS Lake Formation tags management
+in the following way: - You can enable or disable lf-tags management via
+[config](#table-configuration) (disabled by default) - Once you enable the
+feature, lf-tags will be updated on every dbt run - First, all lf-tags for
+columns are removed to avoid inheritance issues - Then, all redundant lf-tags
+are removed from tables and actual tags from table configs are applied -
+Finally, lf-tags for columns are applied It's important to understand the
+following points: - dbt does not manage lf-tags for databases - dbt does not
+manage Lake Formation permissions That's why you should handle this by yourself
+manually or using an automation tool like terraform, AWS CDK etc. You may find
+the following links useful to manage that: * [terraform
+aws_lakeformation_permissions](https://registry.terraform.io/providers/
+hashicorp/aws/latest/docs/resources/lakeformation_permissions) * [terraform
+aws_lakeformation_resource_lf_tags](https://registry.terraform.io/providers/
+hashicorp/aws/latest/docs/resources/lakeformation_resource_lf_tags) ## Python
+models The adapter supports Python models using [`spark`](https://
+docs.aws.amazon.com/athena/latest/ug/notebooks-spark.html). ### Setup - A
+Spark-enabled workgroup created in Athena - Spark execution role granted access
+to Athena, Glue and S3 - The Spark workgroup is added to the `~/.dbt/
+profiles.yml` file and the profile to be used is referenced in
+`dbt_project.yml` ### Spark-specific table configuration - `timeout`
+(`default=43200`) - Time out in seconds for each Python model execution.
+Defaults to 12 hours/43200 seconds. - `spark_encryption` (`default=false`) - If
+this flag is set to true, encrypts data in transit between Spark nodes and also
+encrypts data at rest stored locally by Spark. - `spark_cross_account_catalog`
+(`default=false`) - When using the Spark Athena workgroup, queries can only be
+made against catalogs located on the same AWS account by default. However,
+sometimes you want to query another catalog located on an external AWS account.
+Setting this additional Spark properties parameter to true will enable querying
+external catalogs. You can use the syntax `external_catalog_id/database.table`
+to access the external table on the external catalog (ex: `999999999999/
+mydatabase.cloudfront_logs` where 999999999999 is the external catalog ID) -
+`spark_requester_pays` (`default=false`) - When an Amazon S3 bucket is
 configured as requester pays, the account of the user running the query is
 charged for data access and data transfer fees associated with the query. - If
 this flag is set to true, requester pays S3 buckets are enabled in Athena for
 Spark. ### Spark notes - A session is created for each unique engine
 configuration defined in the models that are part of the invocation. - A
 session's idle timeout is set to 10 minutes. Within the timeout period, if
 there is a new calculation (Spark Python model) ready for execution and the
@@ -370,29 +383,28 @@
 pyspark.sql.functions import udf from pyspark.sql.functions import col
 udf_with_import = udf(func) data = [(1, "a"), (2, "b"), (3, "c")] cols =
 ["num", "alpha"] df = spark_session.createDataFrame(data, cols) return
 df.withColumn("udf_test_col", udf_with_import(col("alpha"))) ``` ### Known
 issues in Python models - Python models cannot [reference Athena SQL views]
 (https://docs.aws.amazon.com/athena/latest/ug/notebooks-spark.html). - Third-
 party Python libraries can be used, but they must be [included in the pre-
-installed list]([pre-installed list]) or [imported manually]([imported
-manually]). - Python models can only reference or write to tables with names
-meeting the regular expression: `^[0-9a-zA-Z_]+$`. Dashes and special
-characters are not supported by Spark, even though Athena supports them. -
-Incremental models do not fully utilize Spark capabilities. They depend
-partially on existing SQL-based logic which runs on Trino. - Snapshot
-materializations are not supported. - Spark can only reference tables within
-the same catalog. [pre-installed list]: https://docs.aws.amazon.com/athena/
-latest/ug/notebooks-spark-preinstalled-python-libraries.html [imported
-manually]: https://docs.aws.amazon.com/athena/latest/ug/notebooks-import-files-
-libraries.html ## Contracts The adapter partly supports contract definition. -
-Concerning the `data_type`, it is supported but needs to be adjusted for
-complex types. They must be specified entirely (for instance `array`) even
-though they won't be checked. Indeed, as dbt recommends, we only compare the
-broader type (array, map, int, varchar). The complete definition is used in
-order to check that the data types defined in athena are ok (pre-flight check).
-- the adapter does not support the constraints since no constraints don't exist
-in Athena. ## Contributing See [CONTRIBUTING](CONTRIBUTING.md) for more
-information on how to contribute to this project. ## Contributors â¨ Thanks
-goes to these wonderful people ([emoji key](https://allcontributors.org/docs/
-en/emoji-key)): _[_h_t_t_p_s_:_/_/_c_o_n_t_r_i_b_._r_o_c_k_s_/_i_m_a_g_e_?_r_e_p_o_=_d_b_t_-_a_t_h_e_n_a_/_d_b_t_-
-_a_t_h_e_n_a_]Contributions of any kind welcome!
+installed list][pre-installed list] or [imported manually][imported manually].
+- Python models can only reference or write to tables with names meeting the
+regular expression: `^[0-9a-zA-Z_]+$`. Dashes and special characters are not
+supported by Spark, even though Athena supports them. - Incremental models do
+not fully utilize Spark capabilities. They depend partially on existing SQL-
+based logic which runs on Trino. - Snapshot materializations are not supported.
+- Spark can only reference tables within the same catalog. [pre-installed
+list]: https://docs.aws.amazon.com/athena/latest/ug/notebooks-spark-
+preinstalled-python-libraries.html [imported manually]: https://
+docs.aws.amazon.com/athena/latest/ug/notebooks-import-files-libraries.html ##
+Contracts The adapter partly supports contract definitions: - `data_type` is
+supported but needs to be adjusted for complex types. Types must be specified
+entirely (for instance `array`) even though they won't be checked. Indeed, as
+dbt recommends, we only compare the broader type (array, map, int, varchar).
+The complete definition is used in order to check that the data types defined
+in Athena are ok (pre-flight check). - The adapter does not support the
+constraints since there is no constraint concept in Athena. ## Contributing See
+[CONTRIBUTING](CONTRIBUTING.md) for more information on how to contribute to
+this project. ## Contributors â¨ Thanks goes to these wonderful people ([emoji
+key](https://allcontributors.org/docs/en/emoji-key)): _[_h_t_t_p_s_:_/_/_c_o_n_t_r_i_b_._r_o_c_k_s_/
+_i_m_a_g_e_?_r_e_p_o_=_d_b_t_-_a_t_h_e_n_a_/_d_b_t_-_a_t_h_e_n_a_]Contributions of any kind welcome!
```

### Comparing `dbt_athena_community-1.8.1/dbt/adapters/athena/column.py` & `dbt_athena_community-1.8.2/dbt/adapters/athena/column.py`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.1/dbt/adapters/athena/config.py` & `dbt_athena_community-1.8.2/dbt/adapters/athena/config.py`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.1/dbt/adapters/athena/connections.py` & `dbt_athena_community-1.8.2/dbt/adapters/athena/connections.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from concurrent.futures.thread import ThreadPoolExecutor
 from contextlib import contextmanager
 from copy import deepcopy
 from dataclasses import dataclass
 from decimal import Decimal
 from typing import Any, ContextManager, Dict, List, Optional, Tuple
 
-import tenacity
 from dbt_common.exceptions import ConnectionError, DbtRuntimeError
 from dbt_common.utils import md5
 from pyathena.connection import Connection as AthenaConnection
 from pyathena.cursor import Cursor
 from pyathena.error import OperationalError, ProgrammingError
 
 # noinspection PyProtectedMember
@@ -21,17 +20,21 @@
     Formatter,
     _escape_hive,
     _escape_presto,
 )
 from pyathena.model import AthenaQueryExecution
 from pyathena.result_set import AthenaResultSet
 from pyathena.util import RetryConfig
-from tenacity.retry import retry_if_exception
-from tenacity.stop import stop_after_attempt
-from tenacity.wait import wait_exponential
+from tenacity import (
+    retry,
+    retry_if_exception,
+    stop_after_attempt,
+    wait_random_exponential,
+)
+from typing_extensions import Self
 
 from dbt.adapters.athena.config import get_boto3_config
 from dbt.adapters.athena.constants import LOGGER
 from dbt.adapters.athena.query_headers import AthenaMacroQueryStringSetter
 from dbt.adapters.athena.session import get_boto3_session
 from dbt.adapters.contracts.connection import (
     AdapterResponse,
@@ -58,16 +61,17 @@
     aws_secret_access_key: Optional[str] = None
     aws_session_token: Optional[str] = None
     poll_interval: float = 1.0
     debug_query_state: bool = False
     _ALIASES = {"catalog": "database"}
     num_retries: int = 5
     num_boto3_retries: Optional[int] = None
+    num_iceberg_retries: int = 3
     s3_data_dir: Optional[str] = None
-    s3_data_naming: Optional[str] = "schema_table_unique"
+    s3_data_naming: str = "schema_table_unique"
     spark_work_group: Optional[str] = None
     s3_tmp_table_dir: Optional[str] = None
     # Unfortunately we can not just use dict, must be Dict because we'll get the following error:
     # Credentials in profile "athena", target "athena" invalid: Unable to create schema for 'dict'
     seed_s3_upload_args: Optional[Dict[str, Any]] = None
     lf_tags_database: Optional[Dict[str, str]] = None
 
@@ -141,68 +145,82 @@
             ]:
                 return query_execution
 
             if self.connection.cursor_kwargs.get("debug_query_state", False):
                 LOGGER.debug(f"Query state is: {query_execution.state}. Sleeping for {self._poll_interval}...")
             time.sleep(self._poll_interval)
 
-    def execute(  # type: ignore
+    def execute(
         self,
         operation: str,
         parameters: Optional[Dict[str, Any]] = None,
         work_group: Optional[str] = None,
         s3_staging_dir: Optional[str] = None,
         endpoint_url: Optional[str] = None,
         cache_size: int = 0,
         cache_expiration_time: int = 0,
         catch_partitions_limit: bool = False,
-        **kwargs,
-    ):
-        def inner() -> AthenaCursor:
-            query_id = self._execute(
-                operation,
-                parameters=parameters,
-                work_group=work_group,
-                s3_staging_dir=s3_staging_dir,
-                cache_size=cache_size,
-                cache_expiration_time=cache_expiration_time,
-            )
-
-            LOGGER.debug(f"Athena query ID {query_id}")
-
-            query_execution = self._executor.submit(self._collect_result_set, query_id).result()
-            if query_execution.state == AthenaQueryExecution.STATE_SUCCEEDED:
-                self.result_set = self._result_set_class(
-                    self._connection,
-                    self._converter,
-                    query_execution,
-                    self.arraysize,
-                    self._retry_config,
-                )
-
-            else:
-                raise OperationalError(query_execution.state_change_reason)
-            return self
-
-        retry = tenacity.Retrying(
+        **kwargs: Dict[str, Any],
+    ) -> Self:
+        @retry(
             # No need to retry if TOO_MANY_OPEN_PARTITIONS occurs.
             # Otherwise, Athena throws ICEBERG_FILESYSTEM_ERROR after retry,
             # because not all files are removed immediately after first try to create table
             retry=retry_if_exception(
                 lambda e: False if catch_partitions_limit and "TOO_MANY_OPEN_PARTITIONS" in str(e) else True
             ),
             stop=stop_after_attempt(self._retry_config.attempt),
-            wait=wait_exponential(
+            wait=wait_random_exponential(
                 multiplier=self._retry_config.attempt,
                 max=self._retry_config.max_delay,
                 exp_base=self._retry_config.exponential_base,
             ),
             reraise=True,
         )
-        return retry(inner)
+        def inner() -> AthenaCursor:
+            num_iceberg_retries = self.connection.cursor_kwargs.get("num_iceberg_retries") + 1
+
+            @retry(
+                # Nested retry is needed to handle ICEBERG_COMMIT_ERROR for parallel inserts
+                retry=retry_if_exception(lambda e: "ICEBERG_COMMIT_ERROR" in str(e)),
+                stop=stop_after_attempt(num_iceberg_retries),
+                wait=wait_random_exponential(
+                    multiplier=num_iceberg_retries,
+                    max=self._retry_config.max_delay,
+                    exp_base=self._retry_config.exponential_base,
+                ),
+                reraise=True,
+            )
+            def execute_with_iceberg_retries() -> AthenaCursor:
+                query_id = self._execute(
+                    operation,
+                    parameters=parameters,
+                    work_group=work_group,
+                    s3_staging_dir=s3_staging_dir,
+                    cache_size=cache_size,
+                    cache_expiration_time=cache_expiration_time,
+                )
+
+                LOGGER.debug(f"Athena query ID {query_id}")
+
+                query_execution = self._executor.submit(self._collect_result_set, query_id).result()
+                if query_execution.state == AthenaQueryExecution.STATE_SUCCEEDED:
+                    self.result_set = self._result_set_class(
+                        self._connection,
+                        self._converter,
+                        query_execution,
+                        self.arraysize,
+                        self._retry_config,
+                    )
+                    return self
+                raise OperationalError(query_execution.state_change_reason)
+
+            return execute_with_iceberg_retries()  # type: ignore
+
+        return inner()  # type: ignore
 
 
 class AthenaConnectionManager(SQLConnectionManager):
     TYPE = "athena"
 
     def set_query_header(self, query_header_context: Dict[str, Any]) -> None:
         self.query_header = AthenaMacroQueryStringSetter(self.profile, query_header_context)
@@ -237,15 +255,18 @@
             handle = AthenaConnection(
                 s3_staging_dir=creds.s3_staging_dir,
                 endpoint_url=creds.endpoint_url,
                 catalog_name=creds.database,
                 schema_name=creds.schema,
                 work_group=creds.work_group,
                 cursor_class=AthenaCursor,
-                cursor_kwargs={"debug_query_state": creds.debug_query_state},
+                cursor_kwargs={
+                    "debug_query_state": creds.debug_query_state,
+                    "num_iceberg_retries": creds.num_iceberg_retries,
+                },
                 formatter=AthenaParameterFormatter(),
                 poll_interval=creds.poll_interval,
                 session=get_boto3_session(connection),
                 retry_config=RetryConfig(
                     attempt=creds.num_retries + 1,
                     exceptions=("ThrottlingException", "TooManyRequestsException", "InternalServerException"),
                 ),
```

### Comparing `dbt_athena_community-1.8.1/dbt/adapters/athena/constants.py` & `dbt_athena_community-1.8.2/dbt/adapters/athena/constants.py`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.1/dbt/adapters/athena/impl.py` & `dbt_athena_community-1.8.2/dbt/adapters/athena/impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,14 @@
     LfGrantsConfig,
     LfPermissions,
     LfTagsConfig,
     LfTagsManager,
 )
 from dbt.adapters.athena.python_submissions import AthenaPythonJobHelper
 from dbt.adapters.athena.relation import (
-    RELATION_TYPE_MAP,
     AthenaRelation,
     AthenaSchemaSearchMap,
     TableType,
     get_table_type,
 )
 from dbt.adapters.athena.s3 import S3DataNaming
 from dbt.adapters.athena.utils import (
@@ -95,14 +94,16 @@
         table_properties : Table properties to add to the table, valid for Iceberg only.
         native_drop:  Relation drop operations will be performed with SQL, not direct Glue API calls.
         seed_by_insert: default behaviour uploads seed data to S3.
         lf_tags_config: AWS lakeformation tags to associate with the table and columns.
         seed_s3_upload_args: Dictionary containing boto3 ExtraArgs when uploading to S3.
         partitions_limit: Maximum numbers of partitions when batching.
         force_batch: Skip creating the table as ctas and run the operation directly in batch insert mode.
+        unique_tmp_table_suffix: Enforce the use of a unique id as tmp table suffix instead of __dbt_tmp.
+        temp_schema: Define in which schema to create temporary tables used in incremental runs.
     """
 
     work_group: Optional[str] = None
     s3_staging_dir: Optional[str] = None
     external_location: Optional[str] = None
     partitioned_by: Optional[str] = None
     bucketed_by: Optional[str] = None
@@ -115,14 +116,16 @@
     table_properties: Optional[str] = None
     native_drop: Optional[str] = None
     seed_by_insert: bool = False
     lf_tags_config: Optional[Dict[str, Any]] = None
     seed_s3_upload_args: Optional[Dict[str, Any]] = None
     partitions_limit: Optional[int] = None
     force_batch: bool = False
+    unique_tmp_table_suffix: bool = False
+    temp_schema: Optional[str] = None
 
 
 class AthenaAdapter(SQLAdapter):
     BATCH_CREATE_PARTITION_API_LIMIT = 100
     BATCH_DELETE_PARTITION_API_LIMIT = 25
     INTEGER_MAX_VALUE_32_BIT_SIGNED = 0x7FFFFFFF
 
@@ -415,14 +418,18 @@
     @available
     def clean_up_table(self, relation: AthenaRelation) -> None:
         # this check avoids issues for when the table location is an empty string
         # or when the table does not exist and table location is None
         if table_location := self.get_glue_table_location(relation):
             self.delete_from_s3(table_location)
 
+    @available
+    def generate_unique_temporary_table_suffix(self, suffix_initial: str = "__dbt_tmp") -> str:
+        return f"{suffix_initial}_{str(uuid4())}"
+
     def quote(self, identifier: str) -> str:
         return f"{self.quote_character}{identifier}{self.quote_character}"
 
     @available
     def quote_seed_column(
         self, column: str, quote_config: Optional[bool], quote_character: Optional[str] = None
     ) -> str:
@@ -532,20 +539,21 @@
                 "s3",
                 region_name=client.region_name,
                 config=get_boto3_config(num_retries=creds.effective_num_retries),
             )
         response = s3_client.list_objects_v2(Bucket=s3_bucket, Prefix=s3_prefix)
         return True if "Contents" in response else False
 
-    def _get_one_table_for_catalog(self, table: TableTypeDef, database: str) -> List[Dict[str, Any]]:
+    @staticmethod
+    def _get_one_table_for_catalog(table: TableTypeDef, database: str) -> List[Dict[str, Any]]:
         table_catalog = {
             "table_database": database,
             "table_schema": table["DatabaseName"],
             "table_name": table["Name"],
-            "table_type": RELATION_TYPE_MAP[table.get("TableType", "EXTERNAL_TABLE")].value,
+            "table_type": get_table_type(table).value,
             "table_comment": table.get("Parameters", {}).get("comment", table.get("Description", "")),
         }
         return [
             {
                 **table_catalog,
                 **{
                     "column_name": col["Name"],
@@ -553,34 +561,34 @@
                     "column_type": col["Type"],
                     "column_comment": col.get("Comment", ""),
                 },
             }
             for idx, col in enumerate(table["StorageDescriptor"]["Columns"] + table.get("PartitionKeys", []))
         ]
 
-    def _get_one_table_for_non_glue_catalog(
-        self, table: TableTypeDef, schema: str, database: str
-    ) -> List[Dict[str, Any]]:
+    @staticmethod
+    def _get_one_table_for_non_glue_catalog(table: TableTypeDef, schema: str, database: str) -> List[Dict[str, Any]]:
         table_catalog = {
             "table_database": database,
             "table_schema": schema,
             "table_name": table["Name"],
-            "table_type": RELATION_TYPE_MAP[table.get("TableType", "EXTERNAL_TABLE")].value,
+            "table_type": get_table_type(table).value,
             "table_comment": table.get("Parameters", {}).get("comment", ""),
         }
         return [
             {
                 **table_catalog,
                 **{
                     "column_name": col["Name"],
                     "column_index": idx,
                     "column_type": col["Type"],
                     "column_comment": col.get("Comment", ""),
                 },
             }
+            # TODO: review this code part as TableTypeDef class does not contain "Columns" attribute
             for idx, col in enumerate(table["Columns"] + table.get("PartitionKeys", []))
         ]
 
     def _get_one_catalog(
         self,
         information_schema: InformationSchema,
         schemas: Set[str],
```

### Comparing `dbt_athena_community-1.8.1/dbt/adapters/athena/lakeformation.py` & `dbt_athena_community-1.8.2/dbt/adapters/athena/lakeformation.py`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.1/dbt/adapters/athena/python_submissions.py` & `dbt_athena_community-1.8.2/dbt/adapters/athena/python_submissions.py`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.1/dbt/adapters/athena/query_headers.py` & `dbt_athena_community-1.8.2/dbt/adapters/athena/query_headers.py`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.1/dbt/adapters/athena/relation.py` & `dbt_athena_community-1.8.2/dbt/adapters/athena/relation.py`

 * *Files 20% similar despite different names*

```diff
@@ -77,30 +77,35 @@
                 self[key][schema] = set()
             self[key][schema].add(relation_name)
 
 
 RELATION_TYPE_MAP = {
     "EXTERNAL_TABLE": TableType.TABLE,
     "EXTERNAL": TableType.TABLE,  # type returned by federated query tables
+    "GOVERNED": TableType.TABLE,
     "MANAGED_TABLE": TableType.TABLE,
     "VIRTUAL_VIEW": TableType.VIEW,
     "table": TableType.TABLE,
     "view": TableType.VIEW,
     "cte": TableType.CTE,
     "materializedview": TableType.MATERIALIZED_VIEW,
 }
 
 
 def get_table_type(table: TableTypeDef) -> TableType:
-    _type = RELATION_TYPE_MAP.get(table.get("TableType"))
-    _specific_type = table.get("Parameters", {}).get("table_type", "")
+    table_full_name = ".".join(filter(None, [table.get("CatalogId"), table.get("DatabaseName"), table["Name"]]))
 
-    if _specific_type.lower() == "iceberg":
-        _type = TableType.ICEBERG
+    input_table_type = table.get("TableType")
+    if input_table_type and input_table_type not in RELATION_TYPE_MAP:
+        raise ValueError(f"Table type {table['TableType']} is not supported for table {table_full_name}")
 
-    if _type is None:
-        raise ValueError("Table type cannot be None")
+    if table.get("Parameters", {}).get("table_type", "").lower() == "iceberg":
+        _type = TableType.ICEBERG
+    elif not input_table_type:
+        raise ValueError(f"Table type cannot be None for table {table_full_name}")
+    else:
+        _type = RELATION_TYPE_MAP[input_table_type]
 
-    LOGGER.debug(f"table_name : {table.get('Name')}")
+    LOGGER.debug(f"table_name : {table_full_name}")
     LOGGER.debug(f"table type : {_type}")
 
     return _type
```

### Comparing `dbt_athena_community-1.8.1/dbt/adapters/athena/session.py` & `dbt_athena_community-1.8.2/dbt/adapters/athena/session.py`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.1/dbt/adapters/athena/utils.py` & `dbt_athena_community-1.8.2/dbt/adapters/athena/utils.py`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.1/dbt/include/athena/macros/adapters/columns.sql` & `dbt_athena_community-1.8.2/dbt/include/athena/macros/adapters/columns.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.1/dbt/include/athena/macros/adapters/metadata.sql` & `dbt_athena_community-1.8.2/dbt/include/athena/macros/adapters/metadata.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.1/dbt/include/athena/macros/adapters/persist_docs.sql` & `dbt_athena_community-1.8.2/dbt/include/athena/macros/adapters/persist_docs.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.1/dbt/include/athena/macros/adapters/python_submissions.sql` & `dbt_athena_community-1.8.2/dbt/include/athena/macros/adapters/python_submissions.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.1/dbt/include/athena/macros/adapters/relation.sql` & `dbt_athena_community-1.8.2/dbt/include/athena/macros/adapters/relation.sql`

 * *Files 8% similar despite different names*

```diff
@@ -32,12 +32,27 @@
 {% macro set_table_classification(relation) -%}
   {%- set format = config.get('format', default='parquet') -%}
   {% call statement('set_table_classification', auto_begin=False) -%}
     alter table {{ relation.render_hive() }} set tblproperties ('classification' = '{{ format }}')
   {%- endcall %}
 {%- endmacro %}
 
+{% macro make_temp_relation(base_relation, suffix='__dbt_tmp', temp_schema=none) %}
+  {%- set temp_identifier = base_relation.identifier ~ suffix -%}
+  {%- set temp_relation = base_relation.incorporate(path={"identifier": temp_identifier}) -%}
+
+  {%- if temp_schema is not none -%}
+    {%- set temp_relation = temp_relation.incorporate(path={
+      "identifier": temp_identifier,
+      "schema": temp_schema
+      }) -%}
+      {%- do create_schema(temp_relation) -%}
+  {% endif %}
+
+  {{ return(temp_relation) }}
+{% endmacro %}
+
 {% macro athena__rename_relation(from_relation, to_relation) %}
   {% call statement('rename_relation') -%}
     alter table {{ from_relation.render_hive() }} rename to `{{ to_relation.schema }}`.`{{ to_relation.identifier }}`
   {%- endcall %}
 {%- endmacro %}
```

### Comparing `dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/hooks.sql` & `dbt_athena_community-1.8.2/dbt/include/athena/macros/materializations/hooks.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/models/helpers/get_partition_batches.sql` & `dbt_athena_community-1.8.2/dbt/include/athena/macros/materializations/models/helpers/get_partition_batches.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/models/helpers/process_bucket_column.sql` & `dbt_athena_community-1.8.2/dbt/include/athena/macros/materializations/models/helpers/process_bucket_column.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/models/incremental/column_helpers.sql` & `dbt_athena_community-1.8.2/dbt/include/athena/macros/materializations/models/incremental/column_helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/models/incremental/helpers.sql` & `dbt_athena_community-1.8.2/dbt/include/athena/macros/materializations/models/incremental/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/models/incremental/incremental.sql` & `dbt_athena_community-1.8.2/dbt/include/athena/macros/materializations/models/incremental/incremental.sql`

 * *Files 6% similar despite different names*

```diff
@@ -5,20 +5,29 @@
   {% set strategy = validate_get_incremental_strategy(raw_strategy, table_type) %}
   {% set on_schema_change = incremental_validate_on_schema_change(config.get('on_schema_change'), default='ignore') %}
   {% set versions_to_keep = config.get('versions_to_keep', 1) | as_number %}
   {% set lf_tags_config = config.get('lf_tags_config') %}
   {% set lf_grants = config.get('lf_grants') %}
   {% set partitioned_by = config.get('partitioned_by') %}
   {% set force_batch = config.get('force_batch', False) | as_bool -%}
+  {% set unique_tmp_table_suffix = config.get('unique_tmp_table_suffix', False) | as_bool -%}
+  {% set temp_schema = config.get('temp_schema') %}
   {% set target_relation = this.incorporate(type='table') %}
   {% set existing_relation = load_relation(this) %}
-  {% set old_tmp_relation = adapter.get_relation(identifier=target_relation.identifier ~ '__dbt_tmp',
+  -- If using insert_overwrite on Hive table, allow to set a unique tmp table suffix
+  {% if unique_tmp_table_suffix == True and strategy == 'insert_overwrite' and table_type == 'hive' %}
+    {% set tmp_table_suffix = adapter.generate_unique_temporary_table_suffix() %}
+  {% else %}
+    {% set tmp_table_suffix = '__dbt_tmp' %}
+  {% endif %}
+
+  {% set old_tmp_relation = adapter.get_relation(identifier=target_relation.identifier ~ tmp_table_suffix,
                                              schema=schema,
                                              database=database) %}
-  {% set tmp_relation = make_temp_relation(target_relation, '__dbt_tmp') %}
+  {% set tmp_relation = make_temp_relation(target_relation, suffix=tmp_table_suffix, temp_schema=temp_schema) %}
 
   -- If no partitions are used with insert_overwrite, we fall back to append mode.
   {% if partitioned_by is none and strategy == 'insert_overwrite' %}
     {% set strategy = 'append' %}
   {% endif %}
 
   {{ run_hooks(pre_hooks, inside_transaction=False) }}
```

### Comparing `dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/models/incremental/merge.sql` & `dbt_athena_community-1.8.2/dbt/include/athena/macros/materializations/models/incremental/merge.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/models/incremental/on_schema_change.sql` & `dbt_athena_community-1.8.2/dbt/include/athena/macros/materializations/models/incremental/on_schema_change.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/models/table/create_table_as.sql` & `dbt_athena_community-1.8.2/dbt/include/athena/macros/materializations/models/table/create_table_as.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/models/table/table.sql` & `dbt_athena_community-1.8.2/dbt/include/athena/macros/materializations/models/table/table.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/models/view/create_or_replace_view.sql` & `dbt_athena_community-1.8.2/dbt/include/athena/macros/materializations/models/view/create_or_replace_view.sql`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
   -- for Snowflake and BigQuery, so multiple dispatch is used.
   {%- if old_relation is not none and old_relation.is_table -%}
     {{ handle_existing_table(should_full_refresh(), old_relation) }}
   {%- endif -%}
 
   -- build model
   {% call statement('main') -%}
-    {{ create_view_as(target_relation, sql) }}
+    {{ create_view_as(target_relation, compiled_code) }}
   {%- endcall %}
 
   {% if lf_tags_config is not none %}
     {{ adapter.add_lf_tags(target_relation, lf_tags_config) }}
   {% endif %}
 
   {% if lf_grants is not none %}
```

### Comparing `dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/models/view/view.sql` & `dbt_athena_community-1.8.2/dbt/include/athena/macros/materializations/models/view/view.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/seeds/helpers.sql` & `dbt_athena_community-1.8.2/dbt/include/athena/macros/materializations/seeds/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.1/dbt/include/athena/macros/materializations/snapshots/snapshot.sql` & `dbt_athena_community-1.8.2/dbt/include/athena/macros/materializations/snapshots/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.1/dbt/include/athena/macros/utils/datediff.sql` & `dbt_athena_community-1.8.2/dbt/include/athena/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.1/dbt/include/athena/macros/utils/ddl_dml_data_type.sql` & `dbt_athena_community-1.8.2/dbt/include/athena/macros/utils/ddl_dml_data_type.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.1/dbt/include/athena/macros/utils/timestamps.sql` & `dbt_athena_community-1.8.2/dbt/include/athena/macros/utils/timestamps.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.1/dbt/include/athena/profile_template.yml` & `dbt_athena_community-1.8.2/dbt/include/athena/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.1/dbt_athena_community.egg-info/PKG-INFO` & `dbt_athena_community-1.8.2/dbt_athena_community.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-athena-community
-Version: 1.8.1
+Version: 1.8.2
 Summary: The athena adapter plugin for dbt (data build tool)
 Home-page: https://github.com/dbt-athena/dbt-athena
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
@@ -45,57 +45,57 @@
     <a href="https://pepy.tech/project/dbt-athena-community">
       <img src="https://static.pepy.tech/badge/dbt-athena-community/month" />
     </a>
 </p>
 <!-- TOC -->
 
 - [Features](#features)
-  - [Quick Start](#quick-start)
+  - [Quick start](#quick-start)
     - [Installation](#installation)
     - [Prerequisites](#prerequisites)
     - [Credentials](#credentials)
     - [Configuring your profile](#configuring-your-profile)
     - [Additional information](#additional-information)
   - [Models](#models)
-    - [Table Configuration](#table-configuration)
+    - [Table configuration](#table-configuration)
     - [Table location](#table-location)
     - [Incremental models](#incremental-models)
     - [On schema change](#on-schema-change)
     - [Iceberg](#iceberg)
     - [Highly available table (HA)](#highly-available-table-ha)
-      - [HA Known issues](#ha-known-issues)
+      - [HA known issues](#ha-known-issues)
     - [Update glue data catalog](#update-glue-data-catalog)
   - [Snapshots](#snapshots)
     - [Timestamp strategy](#timestamp-strategy)
     - [Check strategy](#check-strategy)
     - [Hard-deletes](#hard-deletes)
     - [Working example](#working-example)
-    - [Snapshots Known issues](#snapshots-known-issues)
-  - [AWS Lakeformation integration](#aws-lakeformation-integration)
-  - [Python Models](#python-models)
+    - [Snapshots known issues](#snapshots-known-issues)
+  - [AWS Lake Formation integration](#aws-lake-formation-integration)
+  - [Python models](#python-models)
   - [Contracts](#contracts)
   - [Contributing](#contributing)
   - [Contributors ✨](#contributors-)
 <!-- TOC -->
 
 # Features
 
 - Supports dbt version `1.7.*`
 - Support for Python
 - Supports [seeds][seeds]
 - Correctly detects views and their columns
 - Supports [table materialization][table]
   - [Iceberg tables][athena-iceberg] are supported **only with Athena Engine v3** and **a unique table location**
     (see table location section below)
-  - Hive tables are supported by both Athena engines.
+  - Hive tables are supported by both Athena engines
 - Supports [incremental models][incremental]
-  - On Iceberg tables :
+  - On Iceberg tables:
     - Supports the use of `unique_key` only with the `merge` strategy
     - Supports the `append` strategy
-  - On Hive tables :
+  - On Hive tables:
     - Supports two incremental update strategies: `insert_overwrite` and `append`
     - Does **not** support the use of `unique_key`
 - Supports [snapshots][snapshots]
 - Supports [Python models][python-models]
 
 [seeds]: https://docs.getdbt.com/docs/building-a-dbt-project/seeds
 
@@ -105,15 +105,15 @@
 
 [python-models]: https://docs.getdbt.com/docs/build/python-models#configuring-python-models
 
 [athena-iceberg]: https://docs.aws.amazon.com/athena/latest/ug/querying-iceberg.html
 
 [snapshots]: https://docs.getdbt.com/docs/build/snapshots
 
-## Quick Start
+## Quick start
 
 ### Installation
 
 - `pip install dbt-athena-community`
 - Or `pip install git+https://github.com/dbt-athena/dbt-athena.git`
 
 ### Prerequisites
@@ -136,40 +136,41 @@
 ### Credentials
 
 Credentials can be passed directly to the adapter, or they can
 be [determined automatically](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/credentials.html) based
 on `aws cli`/`boto3` conventions.
 You can either:
 
-- configure `aws_access_key_id` and `aws_secret_access_key`
-- configure `aws_profile_name` to match a profile defined in your AWS credentials file
+- Configure `aws_access_key_id` and `aws_secret_access_key`
+- Configure `aws_profile_name` to match a profile defined in your AWS credentials file.
   Checkout dbt profile configuration below for details.
 
 ### Configuring your profile
 
 A dbt profile can be configured to run against AWS Athena using the following configuration:
 
 | Option                | Description                                                                              | Required? | Example                                    |
-| --------------------- | ---------------------------------------------------------------------------------------- | --------- | ------------------------------------------ |
+|-----------------------|------------------------------------------------------------------------------------------|-----------|--------------------------------------------|
 | s3_staging_dir        | S3 location to store Athena query results and metadata                                   | Required  | `s3://bucket/dbt/`                         |
 | s3_data_dir           | Prefix for storing tables, if different from the connection's `s3_staging_dir`           | Optional  | `s3://bucket2/dbt/`                        |
 | s3_data_naming        | How to generate table paths in `s3_data_dir`                                             | Optional  | `schema_table_unique`                      |
 | s3_tmp_table_dir      | Prefix for storing temporary tables, if different from the connection's `s3_data_dir`    | Optional  | `s3://bucket3/dbt/`                        |
 | region_name           | AWS region of your Athena instance                                                       | Required  | `eu-west-1`                                |
 | schema                | Specify the schema (Athena database) to build models into (lowercase **only**)           | Required  | `dbt`                                      |
 | database              | Specify the database (Data catalog) to build models into (lowercase **only**)            | Required  | `awsdatacatalog`                           |
 | poll_interval         | Interval in seconds to use for polling the status of query results in Athena             | Optional  | `5`                                        |
 | debug_query_state     | Flag if debug message with Athena query state is needed                                  | Optional  | `false`                                    |
-| aws_access_key_id     | Access key ID of the user performing requests.                                           | Optional  | `AKIAIOSFODNN7EXAMPLE`                     |
+| aws_access_key_id     | Access key ID of the user performing requests                                            | Optional  | `AKIAIOSFODNN7EXAMPLE`                     |
 | aws_secret_access_key | Secret access key of the user performing requests                                        | Optional  | `wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY` |
-| aws_profile_name      | Profile to use from your AWS shared credentials file.                                    | Optional  | `my-profile`                               |
+| aws_profile_name      | Profile to use from your AWS shared credentials file                                     | Optional  | `my-profile`                               |
 | work_group            | Identifier of Athena workgroup                                                           | Optional  | `my-custom-workgroup`                      |
 | num_retries           | Number of times to retry a failing query                                                 | Optional  | `3`                                        |
-| spark_work_group      | Identifier of Athena Spark workgroup                                           | Optional  | `my-spark-workgroup`                       |
 | num_boto3_retries     | Number of times to retry boto3 requests (e.g. deleting S3 files for materialized tables) | Optional  | `5`                                        |
+| num_iceberg_retries   | Number of times to retry iceberg commit queries to fix ICEBERG_COMMIT_ERROR              | Optional  | `0`                                        |
+| spark_work_group      | Identifier of Athena Spark workgroup for running Python models                           | Optional  | `my-spark-workgroup`                       |
 | seed_s3_upload_args   | Dictionary containing boto3 ExtraArgs when uploading to S3                               | Optional  | `{"ACL": "bucket-owner-full-control"}`     |
 | lf_tags_database      | Default LF tags for new database if it's created by dbt                                  | Optional  | `tag_key: tag_value`                       |
 
 **Example profiles.yml entry:**
 
 ```yaml
 athena:
@@ -195,20 +196,20 @@
 ### Additional information
 
 - `threads` is supported
 - `database` and `catalog` can be used interchangeably
 
 ## Models
 
-### Table Configuration
+### Table configuration
 
 - `external_location` (`default=none`)
-  - If set, the full S3 path in which the table will be saved.
-  - It works only with incremental models.
-  - Does not work with Hive table with `ha` set to true.
+  - If set, the full S3 path to which the table will be saved
+  - Works only with incremental models
+  - Does not work with Hive table with `ha` set to true
 - `partitioned_by` (`default=none`)
   - An array list of columns by which the table will be partitioned
   - Limited to creation of 100 partitions (*currently*)
 - `bucketed_by` (`default=none`)
   - An array list of columns to bucket data, ignored if using Iceberg
 - `bucket_count` (`default=none`)
   - The number of buckets for bucketing your data, ignored if using Iceberg
@@ -228,23 +229,31 @@
   - Custom field delimiter, for when format is set to `TEXTFILE`
 - `table_properties`: table properties to add to the table, valid for Iceberg only
 - `native_drop`: Relation drop operations will be performed with SQL, not direct Glue API calls. No S3 calls will be
   made to manage data in S3. Data in S3 will only be cleared up for Iceberg
   tables [see AWS docs](https://docs.aws.amazon.com/athena/latest/ug/querying-iceberg-managing-tables.html). Note that
   Iceberg DROP TABLE operations may timeout if they take longer than 60 seconds.
 - `seed_by_insert` (`default=false`)
-  - default behaviour uploads seed data to S3. This flag will create seeds using an SQL insert statement
-  - large seed files cannot use `seed_by_insert`, as the SQL insert statement would
+  - Default behaviour uploads seed data to S3. This flag will create seeds using an SQL insert statement
+  - Large seed files cannot use `seed_by_insert`, as the SQL insert statement would
     exceed [the Athena limit of 262144 bytes](https://docs.aws.amazon.com/athena/latest/ug/service-limits.html)
 - `force_batch` (`default=false`)
-  - Skip creating the table as ctas and run the operation directly in batch insert mode.
+  - Skip creating the table as CTAS and run the operation directly in batch insert mode
   - This is particularly useful when the standard table creation process fails due to partition limitations,
-  allowing you to work with temporary tables and persist the dataset more efficiently.
+  allowing you to work with temporary tables and persist the dataset more efficiently
+- `unique_tmp_table_suffix` (`default=false`)
+  - For incremental models using insert overwrite strategy on hive table
+  - Replace the __dbt_tmp suffix used as temporary table name suffix by a unique uuid
+  - Useful if you are looking to run multiple dbt build inserting in the same table in parallel
+- `temp_schema` (`default=none`)
+  - For incremental models, it allows to define a schema to hold temporary create statements
+  used in incremental model runs
+  - Schema will be created in the model target database if does not exist
 - `lf_tags_config` (`default=none`)
-  - [AWS lakeformation](#aws-lakeformation-integration) tags to associate with the table and columns
+  - [AWS Lake Formation](#aws-lake-formation-integration) tags to associate with the table and columns
   - `enabled` (`default=False`) whether LF tags management is enabled for a model
   - `tags` dictionary with tags and their values to assign for the model
   - `tags_columns` dictionary with a tag key, value and list of columns they must be assigned to
   - `lf_inherited_tags` (`default=none`)
     - List of Lake Formation tag keys that are intended to be inherited from the database level and thus shouldn't be
       removed during association of those defined in `lf_tags_config`
       - i.e., the default behavior of `lf_tags_config` is to be exhaustive and first remove any pre-existing tags from
@@ -273,31 +282,31 @@
           },
           'inherited_tags': ['tag1', 'tag2']
     }
   )
 }}
 ```
 
-- format for `dbt_project.yml`:
+- Format for `dbt_project.yml`:
 
 ```yaml
   +lf_tags_config:
     enabled: true
     tags:
       tag1: value1
       tag2: value2
     tags_columns:
       tag1:
         value1: [ column1, column2 ]
     inherited_tags: [ tag1, tag2 ]
 ```
 
 - `lf_grants` (`default=none`)
-  - lakeformation grants config for data_cell filters
-  - format:
+  - Lake Formation grants config for data_cell filters
+  - Format:
 
   ```python
   lf_grants={
           'data_cell_filters': {
               'enabled': True | False,
               'filters': {
                   'filter_name': {
@@ -328,17 +337,17 @@
       where the inherited value is configured nor in the DBT project where the override previously existed but now is
       gone)
 
 [create-table-as]: https://docs.aws.amazon.com/athena/latest/ug/create-table-as.html#ctas-table-properties
 
 ### Table location
 
-The location in which a table is saved is determined by:
+The location a table is saved to is determined by:
 
-1. If `external_location` is defined, that value is used.
+1. If `external_location` is defined, that value is used
 2. If `s3_data_dir` is defined, the path is determined by that and `s3_data_naming`
 3. If `s3_data_dir` is not defined, data is stored under `s3_staging_dir/tables/`
 
 Here all the options available for `s3_data_naming`:
 
 - `unique`: `{s3_data_dir}/{uuid4()}/`
 - `table`: `{s3_data_dir}/{table}/`
@@ -498,19 +507,20 @@
     , (2, 1)
 ) as t (id, status)
 
 ```
 
 ### Highly available table (HA)
 
-The current implementation of the table materialization can lead to downtime, as target table is dropped and re-created.
-To have the less destructive behavior it's possible to use the `ha` config on your `table` materialized models.
-It leverages the table versions feature of glue catalog, creating a tmp table and swapping the target table to the
-location of the tmp table. This materialization is only available for `table_type=hive` and requires using unique
-locations. For iceberg, high availability is by default.
+The current implementation of the table materialization can lead to downtime, as the target table is
+dropped and re-created. To have the less destructive behavior it's possible to use the `ha` config on
+your `table` materialized models. It leverages the table versions feature of glue catalog, creating
+a temp table and swapping the target table to the location of the temp table. This materialization
+is only available for `table_type=hive` and requires using unique locations. For iceberg, high
+availability is the default.
 
 ```sql
 {{ config(
     materialized='table',
     ha=true,
     format='parquet',
     table_type='hive',
@@ -525,21 +535,21 @@
 select 'b'        as user_id,
        'sh'       as user_name,
        'disabled' as status
 ```
 
 By default, the materialization keeps the last 4 table versions, you can change it by setting `versions_to_keep`.
 
-#### HA Known issues
+#### HA known issues
 
 - When swapping from a table with partitions to a table without (and the other way around), there could be a little
   downtime.
-  In case high performances are needed consider bucketing instead of partitions
+  If high performances is needed consider bucketing instead of partitions
 - By default, Glue "duplicates" the versions internally, so the last two versions of a table point to the same location
-- It's recommended to have `versions_to_keep` >= 4, as this will avoid having the older location removed
+- It's recommended to set `versions_to_keep` >= 4, as this will avoid having the older location removed
 
 ### Update glue data catalog
 
 Optionally persist resource descriptions as column and relation comments to the glue data catalog, and meta as
 [glue table properties](https://docs.aws.amazon.com/glue/latest/dg/tables-described.html#table-properties)
 and [column parameters](https://docs.aws.amazon.com/glue/latest/webapi/API_Column.html).
 By default, documentation persistence is disabled, but it can be enabled for specific resources or
@@ -672,74 +682,75 @@
         check_cols=['series_reference','data_value']
     )
 }}
 select *
 from {{ ref('model') }} {% endsnapshot %}
 ```
 
-### Snapshots Known issues
+### Snapshots known issues
 
-- Incremental Iceberg models - Sync all columns on schema change can't remove columns used as partitioning.
+- Incremental Iceberg models - Sync all columns on schema change can't remove columns used for partitioning.
   The only way, from a dbt perspective, is to do a full-refresh of the incremental model.
 
-- Tables, schemas and database should only be lowercase
+- Tables, schemas and database names should only be lowercase
 
 - In order to avoid potential conflicts, make sure [`dbt-athena-adapter`](https://github.com/Tomme/dbt-athena) is not
   installed in the target environment.
   See <https://github.com/dbt-athena/dbt-athena/issues/103> for more details.
 
 - Snapshot does not support dropping columns from the source table. If you drop a column make sure to drop the column
   from the snapshot as well. Another workaround is to NULL the column in the snapshot definition to preserve history
 
-## AWS Lakeformation integration
+## AWS Lake Formation integration
 
-The adapter implements AWS Lakeformation tags management in the following way:
+The adapter implements AWS Lake Formation tags management in the following way:
 
-- you can enable or disable lf-tags management via [config](#table-configuration) (disabled by default)
-- once you enable the feature, lf-tags will be updated on every dbt run
-- first, all lf-tags for columns are removed to avoid inheritance issues
-- then all redundant lf-tags are removed from table and actual tags from config are applied
-- finally, lf-tags for columns are applied
+- You can enable or disable lf-tags management via [config](#table-configuration) (disabled by default)
+- Once you enable the feature, lf-tags will be updated on every dbt run
+- First, all lf-tags for columns are removed to avoid inheritance issues
+- Then, all redundant lf-tags are removed from tables and actual tags from table configs are applied
+- Finally, lf-tags for columns are applied
 
 It's important to understand the following points:
 
-- dbt does not manage lf-tags for database
-- dbt does not manage lakeformation permissions
+- dbt does not manage lf-tags for databases
+- dbt does not manage Lake Formation permissions
 
-That's why you should handle this by yourself manually or using some automation tools like terraform, AWS CDK etc.
+That's why you should handle this by yourself manually or using an automation tool like terraform, AWS CDK etc.
 You may find the following links useful to manage that:
 
 <!-- markdownlint-disable -->
 * [terraform aws_lakeformation_permissions](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lakeformation_permissions)
 * [terraform aws_lakeformation_resource_lf_tags](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lakeformation_resource_lf_tags)
 <!-- markdownlint-restore -->
 
-## Python Models
+## Python models
 
-The adapter supports python models using [`spark`](https://docs.aws.amazon.com/athena/latest/ug/notebooks-spark.html).
+The adapter supports Python models using [`spark`](https://docs.aws.amazon.com/athena/latest/ug/notebooks-spark.html).
 
 ### Setup
 
 - A Spark-enabled workgroup created in Athena
 - Spark execution role granted access to Athena, Glue and S3
-- The Spark workgroup is added to the `~/.dbt/profiles.yml` file and the profile
- is referenced in `dbt_project.yml` that will be created. It is recommended to keep this same as threads.
+- The Spark workgroup is added to the `~/.dbt/profiles.yml` file and the profile to be used
+  is referenced in `dbt_project.yml`
 
 ### Spark-specific table configuration
 
 - `timeout` (`default=43200`)
   - Time out in seconds for each Python model execution. Defaults to 12 hours/43200 seconds.
 - `spark_encryption` (`default=false`)
   - If this flag is set to true, encrypts data in transit between Spark nodes and also encrypts data at rest stored
    locally by Spark.
 - `spark_cross_account_catalog` (`default=false`)
-  - In Spark, you can query the external account catalog and for that the consumer account has to be configured to
-   access the producer catalog.
-  - If this flag is set to true, "/" can be used as the glue catalog separator.
-   Ex: 999999999999/mydatabase.cloudfront_logs (*where *999999999999* is the external catalog ID*)
+  - When using the Spark Athena workgroup, queries can only be made against catalogs located on the same
+    AWS account by default. However, sometimes you want to query another catalog located on an external AWS
+    account. Setting this additional Spark properties parameter to true will enable querying external catalogs.
+    You can use the syntax `external_catalog_id/database.table` to access the external table on the external
+    catalog (ex: `999999999999/mydatabase.cloudfront_logs` where 999999999999 is the external catalog ID)
 - `spark_requester_pays` (`default=false`)
   - When an Amazon S3 bucket is configured as requester pays, the account of the user running the query is charged for
    data access and data transfer fees associated with the query.
   - If this flag is set to true, requester pays S3 buckets are enabled in Athena for Spark.
 
 ### Spark notes
 
@@ -852,36 +863,36 @@
     return df.withColumn("udf_test_col", udf_with_import(col("alpha")))
 ```
 
 ### Known issues in Python models
 
 - Python models cannot
  [reference Athena SQL views](https://docs.aws.amazon.com/athena/latest/ug/notebooks-spark.html).
-- Third-party Python libraries can be used, but they must be [included in the pre-installed list]([pre-installed list])
- or [imported manually]([imported manually]).
+- Third-party Python libraries can be used, but they must be [included in the pre-installed list][pre-installed list]
+ or [imported manually][imported manually].
 - Python models can only reference or write to tables with names meeting the
  regular expression: `^[0-9a-zA-Z_]+$`. Dashes and special characters are not
  supported by Spark, even though Athena supports them.
 - Incremental models do not fully utilize Spark capabilities. They depend partially on existing SQL-based logic which
  runs on Trino.
 - Snapshot materializations are not supported.
 - Spark can only reference tables within the same catalog.
 
 [pre-installed list]: https://docs.aws.amazon.com/athena/latest/ug/notebooks-spark-preinstalled-python-libraries.html
 [imported manually]: https://docs.aws.amazon.com/athena/latest/ug/notebooks-import-files-libraries.html
 
 ## Contracts
 
-The adapter partly supports contract definition.
+The adapter partly supports contract definitions:
 
-- Concerning the `data_type`, it is supported but needs to be adjusted for complex types. They must be specified
+- `data_type` is supported but needs to be adjusted for complex types. Types must be specified
   entirely (for instance `array<int>`) even though they won't be checked. Indeed, as dbt recommends, we only compare
   the broader type (array, map, int, varchar). The complete definition is used in order to check that the data types
-  defined in athena are ok (pre-flight check).
-- the adapter does not support the constraints since no constraints don't exist in Athena.
+  defined in Athena are ok (pre-flight check).
+- The adapter does not support the constraints since there is no constraint concept in Athena.
 
 ## Contributing
 
 See [CONTRIBUTING](CONTRIBUTING.md) for more information on how to contribute to this project.
 
 ## Contributors ✨
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-athena-community Version: 1.8.1 Summary: The
+Metadata-Version: 2.1 Name: dbt-athena-community Version: 1.8.2 Summary: The
 athena adapter plugin for dbt (data build tool) Home-page: https://github.com/
 dbt-athena/dbt-athena License: Apache License 2.0 Platform: any Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
@@ -17,100 +17,102 @@
  [https://raw.githubusercontent.com/dbt-athena/dbt-athena/main/static/images/
 dbt-athena-long.png]_[_h_t_t_p_s_:_/_/_b_a_d_g_e_._f_u_r_y_._i_o_/_p_y_/_d_b_t_-_a_t_h_e_n_a_-_c_o_m_m_u_n_i_t_y_._s_v_g_]_[_h_t_t_p_s_:_/
  _/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_d_b_t_-_a_t_h_e_n_a_-_c_o_m_m_u_n_i_t_y_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
     _b_a_d_g_e_/_%_2_0_i_m_p_o_r_t_s_-_i_s_o_r_t_-_%_2_3_1_6_7_4_b_1_?_s_t_y_l_e_=_f_l_a_t_&_l_a_b_e_l_C_o_l_o_r_=_e_f_8_3_3_6_]_[_h_t_t_p_s_:_/_/
 _i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_c_o_d_e_%_2_0_s_t_y_l_e_-_b_l_a_c_k_-_0_0_0_0_0_0_._s_v_g_]_[_h_t_t_p_s_:_/_/_w_w_w_._m_y_p_y_-_l_a_n_g_._o_r_g_/
   _s_t_a_t_i_c_/_m_y_p_y___b_a_d_g_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_s_t_a_t_i_c_._p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/_d_b_t_-_a_t_h_e_n_a_-_c_o_m_m_u_n_i_t_y_/
                                     _m_o_n_t_h_]
-- [Features](#features) - [Quick Start](#quick-start) - [Installation]
+- [Features](#features) - [Quick start](#quick-start) - [Installation]
 (#installation) - [Prerequisites](#prerequisites) - [Credentials](#credentials)
 - [Configuring your profile](#configuring-your-profile) - [Additional
 information](#additional-information) - [Models](#models) - [Table
-Configuration](#table-configuration) - [Table location](#table-location) -
+configuration](#table-configuration) - [Table location](#table-location) -
 [Incremental models](#incremental-models) - [On schema change](#on-schema-
 change) - [Iceberg](#iceberg) - [Highly available table (HA)](#highly-
-available-table-ha) - [HA Known issues](#ha-known-issues) - [Update glue data
+available-table-ha) - [HA known issues](#ha-known-issues) - [Update glue data
 catalog](#update-glue-data-catalog) - [Snapshots](#snapshots) - [Timestamp
 strategy](#timestamp-strategy) - [Check strategy](#check-strategy) - [Hard-
 deletes](#hard-deletes) - [Working example](#working-example) - [Snapshots
-Known issues](#snapshots-known-issues) - [AWS Lakeformation integration](#aws-
-lakeformation-integration) - [Python Models](#python-models) - [Contracts]
+known issues](#snapshots-known-issues) - [AWS Lake Formation integration](#aws-
+lake-formation-integration) - [Python models](#python-models) - [Contracts]
 (#contracts) - [Contributing](#contributing) - [Contributors â¨]
 (#contributors-) # Features - Supports dbt version `1.7.*` - Support for Python
 - Supports [seeds][seeds] - Correctly detects views and their columns -
 Supports [table materialization][table] - [Iceberg tables][athena-iceberg] are
 supported **only with Athena Engine v3** and **a unique table location** (see
 table location section below) - Hive tables are supported by both Athena
-engines. - Supports [incremental models][incremental] - On Iceberg tables : -
+engines - Supports [incremental models][incremental] - On Iceberg tables: -
 Supports the use of `unique_key` only with the `merge` strategy - Supports the
-`append` strategy - On Hive tables : - Supports two incremental update
+`append` strategy - On Hive tables: - Supports two incremental update
 strategies: `insert_overwrite` and `append` - Does **not** support the use of
 `unique_key` - Supports [snapshots][snapshots] - Supports [Python models]
 [python-models] [seeds]: https://docs.getdbt.com/docs/building-a-dbt-project/
 seeds [incremental]: https://docs.getdbt.com/docs/build/incremental-models
 [table]: https://docs.getdbt.com/docs/build/materializations#table [python-
 models]: https://docs.getdbt.com/docs/build/python-models#configuring-python-
 models [athena-iceberg]: https://docs.aws.amazon.com/athena/latest/ug/querying-
 iceberg.html [snapshots]: https://docs.getdbt.com/docs/build/snapshots ## Quick
-Start ### Installation - `pip install dbt-athena-community` - Or `pip install
+start ### Installation - `pip install dbt-athena-community` - Or `pip install
 git+https://github.com/dbt-athena/dbt-athena.git` ### Prerequisites To start,
 you will need an S3 bucket, for instance `my-bucket` and an Athena database:
 ```sql CREATE DATABASE IF NOT EXISTS analytics_dev COMMENT 'Analytics models
 generated by dbt (development)' LOCATION 's3://my-bucket/' WITH DBPROPERTIES
 ('creator'='Foo Bar', 'email'='foo@bar.com'); ``` Notes: - Take note of your
 AWS region code (e.g. `us-west-2` or `eu-west-2`, etc.). - You can also use
 [AWS Glue](https://docs.aws.amazon.com/athena/latest/ug/glue-athena.html) to
 create and manage Athena databases. ### Credentials Credentials can be passed
 directly to the adapter, or they can be [determined automatically](https://
 boto3.amazonaws.com/v1/documentation/api/latest/guide/credentials.html) based
-on `aws cli`/`boto3` conventions. You can either: - configure
-`aws_access_key_id` and `aws_secret_access_key` - configure `aws_profile_name`
-to match a profile defined in your AWS credentials file Checkout dbt profile
+on `aws cli`/`boto3` conventions. You can either: - Configure
+`aws_access_key_id` and `aws_secret_access_key` - Configure `aws_profile_name`
+to match a profile defined in your AWS credentials file. Checkout dbt profile
 configuration below for details. ### Configuring your profile A dbt profile can
 be configured to run against AWS Athena using the following configuration: |
-Option | Description | Required? | Example | | --------------------- | --------
+Option | Description | Required? | Example | |-----------------------|---------
 -------------------------------------------------------------------------------
-- | --------- | ------------------------------------------ | | s3_staging_dir |
+--|-----------|--------------------------------------------| | s3_staging_dir |
 S3 location to store Athena query results and metadata | Required | `s3://
 bucket/dbt/` | | s3_data_dir | Prefix for storing tables, if different from the
 connection's `s3_staging_dir` | Optional | `s3://bucket2/dbt/` | |
 s3_data_naming | How to generate table paths in `s3_data_dir` | Optional |
 `schema_table_unique` | | s3_tmp_table_dir | Prefix for storing temporary
 tables, if different from the connection's `s3_data_dir` | Optional | `s3://
 bucket3/dbt/` | | region_name | AWS region of your Athena instance | Required |
 `eu-west-1` | | schema | Specify the schema (Athena database) to build models
 into (lowercase **only**) | Required | `dbt` | | database | Specify the
 database (Data catalog) to build models into (lowercase **only**) | Required |
 `awsdatacatalog` | | poll_interval | Interval in seconds to use for polling the
 status of query results in Athena | Optional | `5` | | debug_query_state | Flag
 if debug message with Athena query state is needed | Optional | `false` | |
-aws_access_key_id | Access key ID of the user performing requests. | Optional |
+aws_access_key_id | Access key ID of the user performing requests | Optional |
 `AKIAIOSFODNN7EXAMPLE` | | aws_secret_access_key | Secret access key of the
 user performing requests | Optional | `wJalrXUtnFEMI/K7MDENG/
 bPxRfiCYEXAMPLEKEY` | | aws_profile_name | Profile to use from your AWS shared
-credentials file. | Optional | `my-profile` | | work_group | Identifier of
+credentials file | Optional | `my-profile` | | work_group | Identifier of
 Athena workgroup | Optional | `my-custom-workgroup` | | num_retries | Number of
-times to retry a failing query | Optional | `3` | | spark_work_group |
-Identifier of Athena Spark workgroup | Optional | `my-spark-workgroup` | |
-num_boto3_retries | Number of times to retry boto3 requests (e.g. deleting S3
-files for materialized tables) | Optional | `5` | | seed_s3_upload_args |
-Dictionary containing boto3 ExtraArgs when uploading to S3 | Optional | `
-{"ACL": "bucket-owner-full-control"}` | | lf_tags_database | Default LF tags
-for new database if it's created by dbt | Optional | `tag_key: tag_value` |
-**Example profiles.yml entry:** ```yaml athena: target: dev outputs: dev: type:
-athena s3_staging_dir: s3://athena-query-results/dbt/ s3_data_dir: s3://
+times to retry a failing query | Optional | `3` | | num_boto3_retries | Number
+of times to retry boto3 requests (e.g. deleting S3 files for materialized
+tables) | Optional | `5` | | num_iceberg_retries | Number of times to retry
+iceberg commit queries to fix ICEBERG_COMMIT_ERROR | Optional | `0` | |
+spark_work_group | Identifier of Athena Spark workgroup for running Python
+models | Optional | `my-spark-workgroup` | | seed_s3_upload_args | Dictionary
+containing boto3 ExtraArgs when uploading to S3 | Optional | `{"ACL": "bucket-
+owner-full-control"}` | | lf_tags_database | Default LF tags for new database
+if it's created by dbt | Optional | `tag_key: tag_value` | **Example
+profiles.yml entry:** ```yaml athena: target: dev outputs: dev: type: athena
+s3_staging_dir: s3://athena-query-results/dbt/ s3_data_dir: s3://
 your_s3_bucket/dbt/ s3_data_naming: schema_table s3_tmp_table_dir: s3://
 your_s3_bucket/temp/ region_name: eu-west-1 schema: dbt database:
 awsdatacatalog threads: 4 aws_profile_name: my-profile work_group: my-workgroup
 spark_work_group: my-spark-workgroup seed_s3_upload_args: ACL: bucket-owner-
 full-control ``` ### Additional information - `threads` is supported -
 `database` and `catalog` can be used interchangeably ## Models ### Table
-Configuration - `external_location` (`default=none`) - If set, the full S3 path
-in which the table will be saved. - It works only with incremental models. -
-Does not work with Hive table with `ha` set to true. - `partitioned_by`
+configuration - `external_location` (`default=none`) - If set, the full S3 path
+to which the table will be saved - Works only with incremental models - Does
+not work with Hive table with `ha` set to true - `partitioned_by`
 (`default=none`) - An array list of columns by which the table will be
 partitioned - Limited to creation of 100 partitions (*currently*) -
 `bucketed_by` (`default=none`) - An array list of columns to bucket data,
 ignored if using Iceberg - `bucket_count` (`default=none`) - The number of
 buckets for bucketing your data, ignored if using Iceberg - `table_type`
 (`default='hive'`) - The type of table - Supports `hive` or `iceberg` - `ha`
 (`default=false`) - If the table should be built using the high-availability
@@ -124,24 +126,31 @@
 Custom field delimiter, for when format is set to `TEXTFILE` -
 `table_properties`: table properties to add to the table, valid for Iceberg
 only - `native_drop`: Relation drop operations will be performed with SQL, not
 direct Glue API calls. No S3 calls will be made to manage data in S3. Data in
 S3 will only be cleared up for Iceberg tables [see AWS docs](https://
 docs.aws.amazon.com/athena/latest/ug/querying-iceberg-managing-tables.html).
 Note that Iceberg DROP TABLE operations may timeout if they take longer than 60
-seconds. - `seed_by_insert` (`default=false`) - default behaviour uploads seed
-data to S3. This flag will create seeds using an SQL insert statement - large
+seconds. - `seed_by_insert` (`default=false`) - Default behaviour uploads seed
+data to S3. This flag will create seeds using an SQL insert statement - Large
 seed files cannot use `seed_by_insert`, as the SQL insert statement would
 exceed [the Athena limit of 262144 bytes](https://docs.aws.amazon.com/athena/
 latest/ug/service-limits.html) - `force_batch` (`default=false`) - Skip
-creating the table as ctas and run the operation directly in batch insert mode.
+creating the table as CTAS and run the operation directly in batch insert mode
 - This is particularly useful when the standard table creation process fails
 due to partition limitations, allowing you to work with temporary tables and
-persist the dataset more efficiently. - `lf_tags_config` (`default=none`) -
-[AWS lakeformation](#aws-lakeformation-integration) tags to associate with the
+persist the dataset more efficiently - `unique_tmp_table_suffix`
+(`default=false`) - For incremental models using insert overwrite strategy on
+hive table - Replace the __dbt_tmp suffix used as temporary table name suffix
+by a unique uuid - Useful if you are looking to run multiple dbt build
+inserting in the same table in parallel - `temp_schema` (`default=none`) - For
+incremental models, it allows to define a schema to hold temporary create
+statements used in incremental model runs - Schema will be created in the model
+target database if does not exist - `lf_tags_config` (`default=none`) - [AWS
+Lake Formation](#aws-lake-formation-integration) tags to associate with the
 table and columns - `enabled` (`default=False`) whether LF tags management is
 enabled for a model - `tags` dictionary with tags and their values to assign
 for the model - `tags_columns` dictionary with a tag key, value and list of
 columns they must be assigned to - `lf_inherited_tags` (`default=none`) - List
 of Lake Formation tag keys that are intended to be inherited from the database
 level and thus shouldn't be removed during association of those defined in
 `lf_tags_config` - i.e., the default behavior of `lf_tags_config` is to be
@@ -149,19 +158,19 @@
 before associating the ones currently defined for a given model - This breaks
 tag inheritance as inherited tags appear on tables and columns like those
 associated directly ```sql {{ config( materialized='incremental',
 incremental_strategy='append', on_schema_change='append_new_columns',
 table_type='iceberg', schema='test_schema', lf_tags_config={ 'enabled': true,
 'tags': { 'tag1': 'value1', 'tag2': 'value2' }, 'tags_columns': { 'tag1':
 { 'value1': ['column1', 'column2'], 'value2': ['column3', 'column4'] } },
-'inherited_tags': ['tag1', 'tag2'] } ) }} ``` - format for `dbt_project.yml`:
+'inherited_tags': ['tag1', 'tag2'] } ) }} ``` - Format for `dbt_project.yml`:
 ```yaml +lf_tags_config: enabled: true tags: tag1: value1 tag2: value2
 tags_columns: tag1: value1: [ column1, column2 ] inherited_tags: [ tag1, tag2 ]
-``` - `lf_grants` (`default=none`) - lakeformation grants config for data_cell
-filters - format: ```python lf_grants={ 'data_cell_filters': { 'enabled': True
+``` - `lf_grants` (`default=none`) - Lake Formation grants config for data_cell
+filters - Format: ```python lf_grants={ 'data_cell_filters': { 'enabled': True
 | False, 'filters': { 'filter_name': { 'row_filter': '', 'principals':
 ['principal_arn1', 'principal_arn2'] } } } } ``` > Notes: > > - `lf_tags` and
 `lf_tags_columns` configs support only attaching lf tags to corresponding
 resources. > We recommend managing LF Tags permissions somewhere outside dbt.
 For example, you may use > [terraform](https://registry.terraform.io/providers/
 hashicorp/aws/latest/docs/resources/lakeformation_permissions) or > [aws cdk]
 (https://docs.aws.amazon.com/cdk/api/v1/docs/aws-lakeformation-readme.html) for
@@ -176,17 +185,17 @@
 not differentiate between an inherited tag association and an override of same
 it made > previously > - e.g. If an inherited tag is overridden by an
 `lf_tags_config` value in one DBT run, and that override is removed prior to a
 subsequent run, the prior override will linger and no longer be encoded
 anywhere (in e.g. Terraform where the inherited value is configured nor in the
 DBT project where the override previously existed but now is gone) [create-
 table-as]: https://docs.aws.amazon.com/athena/latest/ug/create-table-
-as.html#ctas-table-properties ### Table location The location in which a table
-is saved is determined by: 1. If `external_location` is defined, that value is
-used. 2. If `s3_data_dir` is defined, the path is determined by that and
+as.html#ctas-table-properties ### Table location The location a table is saved
+to is determined by: 1. If `external_location` is defined, that value is used
+2. If `s3_data_dir` is defined, the path is determined by that and
 `s3_data_naming` 3. If `s3_data_dir` is not defined, data is stored under
 `s3_staging_dir/tables/` Here all the options available for `s3_data_naming`: -
 `unique`: `{s3_data_dir}/{uuid4()}/` - `table`: `{s3_data_dir}/{table}/` -
 `table_unique`: `{s3_data_dir}/{table}/{uuid4()}/` - `schema_table`: `
 {s3_data_dir}/{schema}/{table}/` - `s3_data_naming=schema_table_unique`: `
 {s3_data_dir}/{schema}/{table}/{uuid4()}/` It's possible to set the
 `s3_data_naming` globally in the target profile, or overwrite the value in the
@@ -246,34 +255,34 @@
 %} select * from ( values (1, 'v1-updated') , (2, 'v2-updated') ) as t (id,
 value) {% else %} select * from ( values (-1, 'v-1') , (0, 'v0') , (1, 'v1') ,
 (2, 'v2') ) as t (id, value) {% endif %} ``` `insert_condition` example: ```sql
 {{ config( materialized='incremental', incremental_strategy='merge',
 unique_key=['id'], insert_condition='target.status != 0', schema='sandbox' ) }}
 select * from ( values (1, 0) , (2, 1) ) as t (id, status) ``` ### Highly
 available table (HA) The current implementation of the table materialization
-can lead to downtime, as target table is dropped and re-created. To have the
-less destructive behavior it's possible to use the `ha` config on your `table`
-materialized models. It leverages the table versions feature of glue catalog,
-creating a tmp table and swapping the target table to the location of the tmp
-table. This materialization is only available for `table_type=hive` and
-requires using unique locations. For iceberg, high availability is by default.
-```sql {{ config( materialized='table', ha=true, format='parquet',
+can lead to downtime, as the target table is dropped and re-created. To have
+the less destructive behavior it's possible to use the `ha` config on your
+`table` materialized models. It leverages the table versions feature of glue
+catalog, creating a temp table and swapping the target table to the location of
+the temp table. This materialization is only available for `table_type=hive`
+and requires using unique locations. For iceberg, high availability is the
+default. ```sql {{ config( materialized='table', ha=true, format='parquet',
 table_type='hive', partitioned_by=['status'], s3_data_naming='table_unique' )
 }} select 'a' as user_id, 'pi' as user_name, 'active' as status union all
 select 'b' as user_id, 'sh' as user_name, 'disabled' as status ``` By default,
 the materialization keeps the last 4 table versions, you can change it by
-setting `versions_to_keep`. #### HA Known issues - When swapping from a table
+setting `versions_to_keep`. #### HA known issues - When swapping from a table
 with partitions to a table without (and the other way around), there could be a
-little downtime. In case high performances are needed consider bucketing
-instead of partitions - By default, Glue "duplicates" the versions internally,
-so the last two versions of a table point to the same location - It's
-recommended to have `versions_to_keep` >= 4, as this will avoid having the
-older location removed ### Update glue data catalog Optionally persist resource
-descriptions as column and relation comments to the glue data catalog, and meta
-as [glue table properties](https://docs.aws.amazon.com/glue/latest/dg/tables-
+little downtime. If high performances is needed consider bucketing instead of
+partitions - By default, Glue "duplicates" the versions internally, so the last
+two versions of a table point to the same location - It's recommended to set
+`versions_to_keep` >= 4, as this will avoid having the older location removed
+### Update glue data catalog Optionally persist resource descriptions as column
+and relation comments to the glue data catalog, and meta as [glue table
+properties](https://docs.aws.amazon.com/glue/latest/dg/tables-
 described.html#table-properties) and [column parameters](https://
 docs.aws.amazon.com/glue/latest/webapi/API_Column.html). By default,
 documentation persistence is disabled, but it can be enabled for specific
 resources or groups of resources as needed. For example: ```yaml models: -
 name: test_deduplicate description: another value config: persist_docs:
 relation: true columns: true meta: test: value columns: - name: id meta:
 primary_key: true ``` See [persist docs](https://docs.getdbt.com/reference/
@@ -304,54 +313,58 @@
 ('model') }} {% endsnapshot %} ``` invalidate hard deletes - model_snapshot_2
 ```sql {% snapshot model_snapshot_2 %} {{ config ( unique_key='id',
 strategy='timestamp', updated_at='refresh_timestamp',
 invalidate_hard_deletes=True, ) }} select * from {{ ref('model') }} {%
 endsnapshot %} ``` check strategy - model_snapshot_3 ```sql {% snapshot
 model_snapshot_3 %} {{ config ( unique_key='id', strategy='check', check_cols=
 ['series_reference','data_value'] ) }} select * from {{ ref('model') }} {%
-endsnapshot %} ``` ### Snapshots Known issues - Incremental Iceberg models -
-Sync all columns on schema change can't remove columns used as partitioning.
+endsnapshot %} ``` ### Snapshots known issues - Incremental Iceberg models -
+Sync all columns on schema change can't remove columns used for partitioning.
 The only way, from a dbt perspective, is to do a full-refresh of the
-incremental model. - Tables, schemas and database should only be lowercase - In
-order to avoid potential conflicts, make sure [`dbt-athena-adapter`](https://
-github.com/Tomme/dbt-athena) is not installed in the target environment. See
+incremental model. - Tables, schemas and database names should only be
+lowercase - In order to avoid potential conflicts, make sure [`dbt-athena-
+adapter`](https://github.com/Tomme/dbt-athena) is not installed in the target
+environment. See
 github.com/dbt-athena/dbt-athena/issues/103> for more details. - Snapshot does
 not support dropping columns from the source table. If you drop a column make
 sure to drop the column from the snapshot as well. Another workaround is to
-NULL the column in the snapshot definition to preserve history ## AWS
-Lakeformation integration The adapter implements AWS Lakeformation tags
-management in the following way: - you can enable or disable lf-tags management
-via [config](#table-configuration) (disabled by default) - once you enable the
-feature, lf-tags will be updated on every dbt run - first, all lf-tags for
-columns are removed to avoid inheritance issues - then all redundant lf-tags
-are removed from table and actual tags from config are applied - finally, lf-
-tags for columns are applied It's important to understand the following points:
-- dbt does not manage lf-tags for database - dbt does not manage lakeformation
-permissions That's why you should handle this by yourself manually or using
-some automation tools like terraform, AWS CDK etc. You may find the following
-links useful to manage that: * [terraform aws_lakeformation_permissions](https:
-//registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/
-lakeformation_permissions) * [terraform aws_lakeformation_resource_lf_tags]
-(https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/
-lakeformation_resource_lf_tags) ## Python Models The adapter supports python
-models using [`spark`](https://docs.aws.amazon.com/athena/latest/ug/notebooks-
-spark.html). ### Setup - A Spark-enabled workgroup created in Athena - Spark
-execution role granted access to Athena, Glue and S3 - The Spark workgroup is
-added to the `~/.dbt/profiles.yml` file and the profile is referenced in
-`dbt_project.yml` that will be created. It is recommended to keep this same as
-threads. ### Spark-specific table configuration - `timeout` (`default=43200`) -
-Time out in seconds for each Python model execution. Defaults to 12 hours/43200
-seconds. - `spark_encryption` (`default=false`) - If this flag is set to true,
-encrypts data in transit between Spark nodes and also encrypts data at rest
-stored locally by Spark. - `spark_cross_account_catalog` (`default=false`) - In
-Spark, you can query the external account catalog and for that the consumer
-account has to be configured to access the producer catalog. - If this flag is
-set to true, "/" can be used as the glue catalog separator. Ex: 999999999999/
-mydatabase.cloudfront_logs (*where *999999999999* is the external catalog ID*)
-- `spark_requester_pays` (`default=false`) - When an Amazon S3 bucket is
+NULL the column in the snapshot definition to preserve history ## AWS Lake
+Formation integration The adapter implements AWS Lake Formation tags management
+in the following way: - You can enable or disable lf-tags management via
+[config](#table-configuration) (disabled by default) - Once you enable the
+feature, lf-tags will be updated on every dbt run - First, all lf-tags for
+columns are removed to avoid inheritance issues - Then, all redundant lf-tags
+are removed from tables and actual tags from table configs are applied -
+Finally, lf-tags for columns are applied It's important to understand the
+following points: - dbt does not manage lf-tags for databases - dbt does not
+manage Lake Formation permissions That's why you should handle this by yourself
+manually or using an automation tool like terraform, AWS CDK etc. You may find
+the following links useful to manage that: * [terraform
+aws_lakeformation_permissions](https://registry.terraform.io/providers/
+hashicorp/aws/latest/docs/resources/lakeformation_permissions) * [terraform
+aws_lakeformation_resource_lf_tags](https://registry.terraform.io/providers/
+hashicorp/aws/latest/docs/resources/lakeformation_resource_lf_tags) ## Python
+models The adapter supports Python models using [`spark`](https://
+docs.aws.amazon.com/athena/latest/ug/notebooks-spark.html). ### Setup - A
+Spark-enabled workgroup created in Athena - Spark execution role granted access
+to Athena, Glue and S3 - The Spark workgroup is added to the `~/.dbt/
+profiles.yml` file and the profile to be used is referenced in
+`dbt_project.yml` ### Spark-specific table configuration - `timeout`
+(`default=43200`) - Time out in seconds for each Python model execution.
+Defaults to 12 hours/43200 seconds. - `spark_encryption` (`default=false`) - If
+this flag is set to true, encrypts data in transit between Spark nodes and also
+encrypts data at rest stored locally by Spark. - `spark_cross_account_catalog`
+(`default=false`) - When using the Spark Athena workgroup, queries can only be
+made against catalogs located on the same AWS account by default. However,
+sometimes you want to query another catalog located on an external AWS account.
+Setting this additional Spark properties parameter to true will enable querying
+external catalogs. You can use the syntax `external_catalog_id/database.table`
+to access the external table on the external catalog (ex: `999999999999/
+mydatabase.cloudfront_logs` where 999999999999 is the external catalog ID) -
+`spark_requester_pays` (`default=false`) - When an Amazon S3 bucket is
 configured as requester pays, the account of the user running the query is
 charged for data access and data transfer fees associated with the query. - If
 this flag is set to true, requester pays S3 buckets are enabled in Athena for
 Spark. ### Spark notes - A session is created for each unique engine
 configuration defined in the models that are part of the invocation. - A
 session's idle timeout is set to 10 minutes. Within the timeout period, if
 there is a new calculation (Spark Python model) ready for execution and the
@@ -386,29 +399,28 @@
 pyspark.sql.functions import udf from pyspark.sql.functions import col
 udf_with_import = udf(func) data = [(1, "a"), (2, "b"), (3, "c")] cols =
 ["num", "alpha"] df = spark_session.createDataFrame(data, cols) return
 df.withColumn("udf_test_col", udf_with_import(col("alpha"))) ``` ### Known
 issues in Python models - Python models cannot [reference Athena SQL views]
 (https://docs.aws.amazon.com/athena/latest/ug/notebooks-spark.html). - Third-
 party Python libraries can be used, but they must be [included in the pre-
-installed list]([pre-installed list]) or [imported manually]([imported
-manually]). - Python models can only reference or write to tables with names
-meeting the regular expression: `^[0-9a-zA-Z_]+$`. Dashes and special
-characters are not supported by Spark, even though Athena supports them. -
-Incremental models do not fully utilize Spark capabilities. They depend
-partially on existing SQL-based logic which runs on Trino. - Snapshot
-materializations are not supported. - Spark can only reference tables within
-the same catalog. [pre-installed list]: https://docs.aws.amazon.com/athena/
-latest/ug/notebooks-spark-preinstalled-python-libraries.html [imported
-manually]: https://docs.aws.amazon.com/athena/latest/ug/notebooks-import-files-
-libraries.html ## Contracts The adapter partly supports contract definition. -
-Concerning the `data_type`, it is supported but needs to be adjusted for
-complex types. They must be specified entirely (for instance `array`) even
-though they won't be checked. Indeed, as dbt recommends, we only compare the
-broader type (array, map, int, varchar). The complete definition is used in
-order to check that the data types defined in athena are ok (pre-flight check).
-- the adapter does not support the constraints since no constraints don't exist
-in Athena. ## Contributing See [CONTRIBUTING](CONTRIBUTING.md) for more
-information on how to contribute to this project. ## Contributors â¨ Thanks
-goes to these wonderful people ([emoji key](https://allcontributors.org/docs/
-en/emoji-key)): _[_h_t_t_p_s_:_/_/_c_o_n_t_r_i_b_._r_o_c_k_s_/_i_m_a_g_e_?_r_e_p_o_=_d_b_t_-_a_t_h_e_n_a_/_d_b_t_-
-_a_t_h_e_n_a_]Contributions of any kind welcome!
+installed list][pre-installed list] or [imported manually][imported manually].
+- Python models can only reference or write to tables with names meeting the
+regular expression: `^[0-9a-zA-Z_]+$`. Dashes and special characters are not
+supported by Spark, even though Athena supports them. - Incremental models do
+not fully utilize Spark capabilities. They depend partially on existing SQL-
+based logic which runs on Trino. - Snapshot materializations are not supported.
+- Spark can only reference tables within the same catalog. [pre-installed
+list]: https://docs.aws.amazon.com/athena/latest/ug/notebooks-spark-
+preinstalled-python-libraries.html [imported manually]: https://
+docs.aws.amazon.com/athena/latest/ug/notebooks-import-files-libraries.html ##
+Contracts The adapter partly supports contract definitions: - `data_type` is
+supported but needs to be adjusted for complex types. Types must be specified
+entirely (for instance `array`) even though they won't be checked. Indeed, as
+dbt recommends, we only compare the broader type (array, map, int, varchar).
+The complete definition is used in order to check that the data types defined
+in Athena are ok (pre-flight check). - The adapter does not support the
+constraints since there is no constraint concept in Athena. ## Contributing See
+[CONTRIBUTING](CONTRIBUTING.md) for more information on how to contribute to
+this project. ## Contributors â¨ Thanks goes to these wonderful people ([emoji
+key](https://allcontributors.org/docs/en/emoji-key)): _[_h_t_t_p_s_:_/_/_c_o_n_t_r_i_b_._r_o_c_k_s_/
+_i_m_a_g_e_?_r_e_p_o_=_d_b_t_-_a_t_h_e_n_a_/_d_b_t_-_a_t_h_e_n_a_]Contributions of any kind welcome!
```

### Comparing `dbt_athena_community-1.8.1/dbt_athena_community.egg-info/SOURCES.txt` & `dbt_athena_community-1.8.2/dbt_athena_community.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.1/pyproject.toml` & `dbt_athena_community-1.8.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.1/setup.py` & `dbt_athena_community-1.8.2/setup.py`

 * *Files identical despite different names*

