# Comparing `tmp/philologic-4.7.4.4.tar.gz` & `tmp/philologic-4.7.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "philologic-4.7.4.4.tar", last modified: Wed Sep 20 15:31:00 2023, max compression
+gzip compressed data, was "philologic-4.7.5.0.tar", last modified: Tue May 28 16:27:16 2024, max compression
```

## Comparing `philologic-4.7.4.4.tar` & `philologic-4.7.5.0.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 clovis    (1000) artfl     (1003)        0 2023-09-20 15:31:00.759910 philologic-4.7.4.4/
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)    35141 2022-11-22 20:47:37.000000 philologic-4.7.4.4/LICENSE
--rw-r--r--   0 clovis    (1000) artfl     (1003)      746 2023-09-20 15:31:00.759910 philologic-4.7.4.4/PKG-INFO
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)      428 2022-11-22 16:01:26.000000 philologic-4.7.4.4/README
-drwxr-xr-x   0 clovis    (1000) artfl     (1003)        0 2023-09-20 15:31:00.755910 philologic-4.7.4.4/philologic/
--rw-r--r--   0 clovis    (1000) artfl     (1003)    36981 2022-12-05 22:36:45.000000 philologic-4.7.4.4/philologic/Config.py
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)     4469 2022-11-22 16:35:28.000000 philologic-4.7.4.4/philologic/TagCensus.py
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)      101 2022-11-22 20:47:37.000000 philologic-4.7.4.4/philologic/__init__.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)      181 2022-11-22 21:05:10.000000 philologic-4.7.4.4/philologic/_version.py
-drwxr-xr-x   0 clovis    (1000) artfl     (1003)        0 2023-09-20 15:31:00.759910 philologic-4.7.4.4/philologic/loadtime/
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)    17188 2023-09-14 14:45:36.000000 philologic-4.7.4.4/philologic/loadtime/LoadFilters.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)    10528 2022-11-24 20:03:41.000000 philologic-4.7.4.4/philologic/loadtime/LoadOptions.py
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)    42131 2023-09-14 15:27:20.000000 philologic-4.7.4.4/philologic/loadtime/Loader.py
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)    13824 2023-09-20 15:10:43.000000 philologic-4.7.4.4/philologic/loadtime/OHCOVector.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)    72616 2023-09-20 15:28:46.000000 philologic-4.7.4.4/philologic/loadtime/Parser.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     8083 2023-02-07 19:21:34.000000 philologic-4.7.4.4/philologic/loadtime/PlainTextParser.py
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)    10370 2023-03-04 17:27:17.000000 philologic-4.7.4.4/philologic/loadtime/PostFilters.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)       49 2022-11-22 16:35:28.000000 philologic-4.7.4.4/philologic/loadtime/__init__.py
-drwxr-xr-x   0 clovis    (1000) artfl     (1003)        0 2023-09-20 15:31:00.759910 philologic-4.7.4.4/philologic/runtime/
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)     9410 2022-11-22 16:35:28.000000 philologic-4.7.4.4/philologic/runtime/DB.py
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)     3776 2022-11-22 16:35:28.000000 philologic-4.7.4.4/philologic/runtime/FragmentParser.py
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)     9822 2022-11-22 16:35:28.000000 philologic-4.7.4.4/philologic/runtime/HitList.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     6768 2022-11-22 16:35:28.000000 philologic-4.7.4.4/philologic/runtime/HitWrapper.py
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)    12990 2022-11-22 16:35:28.000000 philologic-4.7.4.4/philologic/runtime/MetadataQuery.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)    31760 2023-06-20 16:50:25.000000 philologic-4.7.4.4/philologic/runtime/ObjectFormatter.py
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)     9792 2022-11-22 16:35:28.000000 philologic-4.7.4.4/philologic/runtime/Query.py
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)     3493 2022-11-22 16:35:28.000000 philologic-4.7.4.4/philologic/runtime/QuerySyntax.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     7458 2022-12-19 19:58:22.000000 philologic-4.7.4.4/philologic/runtime/WSGIHandler.py
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)      951 2022-11-22 16:35:28.000000 philologic-4.7.4.4/philologic/runtime/__init__.py
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)     6071 2022-11-22 16:35:28.000000 philologic-4.7.4.4/philologic/runtime/access_control.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     5693 2022-11-22 16:35:28.000000 philologic-4.7.4.4/philologic/runtime/citations.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)      511 2022-11-22 16:35:28.000000 philologic-4.7.4.4/philologic/runtime/collocation_scores.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     2412 2022-11-22 16:35:28.000000 philologic-4.7.4.4/philologic/runtime/find_similar_words.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     4044 2023-06-20 14:24:18.000000 philologic-4.7.4.4/philologic/runtime/get_text.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     2956 2022-12-09 02:32:30.000000 philologic-4.7.4.4/philologic/runtime/link.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)      413 2022-11-22 16:35:28.000000 philologic-4.7.4.4/philologic/runtime/pages.py
-drwxr-xr-x   0 clovis    (1000) artfl     (1003)        0 2023-09-20 15:31:00.759910 philologic-4.7.4.4/philologic/runtime/reports/
--rw-r--r--   0 clovis    (1000) artfl     (1003)      977 2022-11-22 16:35:28.000000 philologic-4.7.4.4/philologic/runtime/reports/__init__.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     7673 2022-11-22 16:35:28.000000 philologic-4.7.4.4/philologic/runtime/reports/aggregation.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     3242 2022-12-19 22:17:21.000000 philologic-4.7.4.4/philologic/runtime/reports/bibliography.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     5332 2022-12-05 22:33:58.000000 philologic-4.7.4.4/philologic/runtime/reports/collocation.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     2712 2022-11-22 16:35:28.000000 philologic-4.7.4.4/philologic/runtime/reports/concordance.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     2627 2022-11-22 16:35:28.000000 philologic-4.7.4.4/philologic/runtime/reports/filter_word_by_property.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     7830 2022-11-22 16:35:28.000000 philologic-4.7.4.4/philologic/runtime/reports/frequency.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     2507 2022-11-22 16:35:28.000000 philologic-4.7.4.4/philologic/runtime/reports/generate_word_frequency.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     3349 2022-11-22 16:35:28.000000 philologic-4.7.4.4/philologic/runtime/reports/kwic.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     7425 2022-11-22 16:35:28.000000 philologic-4.7.4.4/philologic/runtime/reports/landing_page.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     3074 2022-11-22 16:35:28.000000 philologic-4.7.4.4/philologic/runtime/reports/navigation.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     3870 2022-11-22 16:35:28.000000 philologic-4.7.4.4/philologic/runtime/reports/table_of_contents.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     4925 2022-11-22 16:35:28.000000 philologic-4.7.4.4/philologic/runtime/reports/time_series.py
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)      894 2022-11-22 16:35:28.000000 philologic-4.7.4.4/philologic/runtime/web_config.py
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)     6167 2022-11-22 16:35:28.000000 philologic-4.7.4.4/philologic/shlax.py
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)     8793 2022-11-22 16:35:28.000000 philologic-4.7.4.4/philologic/shlaxtree.py
-drwxr-xr-x   0 clovis    (1000) artfl     (1003)        0 2023-09-20 15:31:00.759910 philologic-4.7.4.4/philologic/utils/
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)      221 2022-11-22 16:35:28.000000 philologic-4.7.4.4/philologic/utils/__init__.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)      762 2022-11-22 16:35:28.000000 philologic-4.7.4.4/philologic/utils/convert_entities.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)      430 2022-11-22 16:35:28.000000 philologic-4.7.4.4/philologic/utils/load_module.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     1929 2022-11-22 16:35:28.000000 philologic-4.7.4.4/philologic/utils/metadata_type_handler.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)     1113 2022-11-22 16:35:28.000000 philologic-4.7.4.4/philologic/utils/pretty_print.py
--rw-r--r--   0 clovis    (1000) artfl     (1003)      581 2022-11-22 16:35:28.000000 philologic-4.7.4.4/philologic/utils/sort.py
-drwxr-xr-x   0 clovis    (1000) artfl     (1003)        0 2023-09-20 15:31:00.755910 philologic-4.7.4.4/philologic.egg-info/
--rw-r--r--   0 clovis    (1000) artfl     (1003)      746 2023-09-20 15:31:00.000000 philologic-4.7.4.4/philologic.egg-info/PKG-INFO
--rw-r--r--   0 clovis    (1000) artfl     (1003)     1975 2023-09-20 15:31:00.000000 philologic-4.7.4.4/philologic.egg-info/SOURCES.txt
--rw-r--r--   0 clovis    (1000) artfl     (1003)        1 2023-09-20 15:31:00.000000 philologic-4.7.4.4/philologic.egg-info/dependency_links.txt
--rw-r--r--   0 clovis    (1000) artfl     (1003)       91 2023-09-20 15:31:00.000000 philologic-4.7.4.4/philologic.egg-info/requires.txt
--rw-r--r--   0 clovis    (1000) artfl     (1003)       11 2023-09-20 15:31:00.000000 philologic-4.7.4.4/philologic.egg-info/top_level.txt
-drwxr-xr-x   0 clovis    (1000) artfl     (1003)        0 2023-09-20 15:31:00.759910 philologic-4.7.4.4/scripts/
--rwxr-xr-x   0 clovis    (1000) artfl     (1003)     1361 2022-11-22 17:21:51.000000 philologic-4.7.4.4/scripts/philoload4
--rw-r--r--   0 clovis    (1000) artfl     (1003)       38 2023-09-20 15:31:00.759910 philologic-4.7.4.4/setup.cfg
--rw-r--r--   0 clovis    (1000) artfl     (1003)     1137 2022-11-30 18:18:41.000000 philologic-4.7.4.4/setup.py
+drwxr-xr-x   0 clovis    (1000) artfl     (1003)        0 2024-05-28 16:27:16.185078 philologic-4.7.5.0/
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)    35141 2022-11-22 20:47:37.000000 philologic-4.7.5.0/LICENSE
+-rw-r--r--   0 clovis    (1000) artfl     (1003)    41516 2024-05-28 16:27:16.185078 philologic-4.7.5.0/PKG-INFO
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)      428 2022-11-22 16:01:26.000000 philologic-4.7.5.0/README
+drwxr-xr-x   0 clovis    (1000) artfl     (1003)        0 2024-05-28 16:27:16.177078 philologic-4.7.5.0/philologic/
+-rw-r--r--   0 clovis    (1000) artfl     (1003)    36981 2022-12-05 22:36:45.000000 philologic-4.7.5.0/philologic/Config.py
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)     4469 2022-11-22 16:35:28.000000 philologic-4.7.5.0/philologic/TagCensus.py
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)      101 2022-11-22 20:47:37.000000 philologic-4.7.5.0/philologic/__init__.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)      181 2022-11-22 21:05:10.000000 philologic-4.7.5.0/philologic/_version.py
+drwxr-xr-x   0 clovis    (1000) artfl     (1003)        0 2024-05-28 16:27:16.181078 philologic-4.7.5.0/philologic/loadtime/
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)    17188 2023-09-14 14:45:36.000000 philologic-4.7.5.0/philologic/loadtime/LoadFilters.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)    10528 2022-11-24 20:03:41.000000 philologic-4.7.5.0/philologic/loadtime/LoadOptions.py
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)    42180 2024-05-28 16:24:37.000000 philologic-4.7.5.0/philologic/loadtime/Loader.py
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)    13824 2023-09-20 15:10:43.000000 philologic-4.7.5.0/philologic/loadtime/OHCOVector.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)    72616 2023-09-20 15:28:46.000000 philologic-4.7.5.0/philologic/loadtime/Parser.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     1351 2024-04-17 13:47:53.000000 philologic-4.7.5.0/philologic/loadtime/PhiloLoad.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     8083 2023-02-07 19:21:34.000000 philologic-4.7.5.0/philologic/loadtime/PlainTextParser.py
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)    10370 2023-03-04 17:27:17.000000 philologic-4.7.5.0/philologic/loadtime/PostFilters.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)      101 2024-04-17 13:37:09.000000 philologic-4.7.5.0/philologic/loadtime/__init__.py
+drwxr-xr-x   0 clovis    (1000) artfl     (1003)        0 2024-05-28 16:27:16.181078 philologic-4.7.5.0/philologic/runtime/
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)     9410 2023-11-13 19:06:30.000000 philologic-4.7.5.0/philologic/runtime/DB.py
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)     3776 2024-04-19 14:58:16.000000 philologic-4.7.5.0/philologic/runtime/FragmentParser.py
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)     9822 2023-11-13 19:06:30.000000 philologic-4.7.5.0/philologic/runtime/HitList.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     6768 2024-04-17 13:42:41.000000 philologic-4.7.5.0/philologic/runtime/HitWrapper.py
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)    12990 2022-11-22 16:35:28.000000 philologic-4.7.5.0/philologic/runtime/MetadataQuery.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)    31760 2023-06-20 16:50:25.000000 philologic-4.7.5.0/philologic/runtime/ObjectFormatter.py
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)     9792 2024-04-17 13:42:23.000000 philologic-4.7.5.0/philologic/runtime/Query.py
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)     3493 2023-11-13 19:06:30.000000 philologic-4.7.5.0/philologic/runtime/QuerySyntax.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     7458 2023-11-13 18:45:12.000000 philologic-4.7.5.0/philologic/runtime/WSGIHandler.py
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)      951 2022-11-22 16:35:28.000000 philologic-4.7.5.0/philologic/runtime/__init__.py
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)     6071 2022-11-22 16:35:28.000000 philologic-4.7.5.0/philologic/runtime/access_control.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     5693 2022-11-22 16:35:28.000000 philologic-4.7.5.0/philologic/runtime/citations.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)      511 2022-11-22 16:35:28.000000 philologic-4.7.5.0/philologic/runtime/collocation_scores.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     2412 2022-11-22 16:35:28.000000 philologic-4.7.5.0/philologic/runtime/find_similar_words.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     4044 2023-06-20 14:24:18.000000 philologic-4.7.5.0/philologic/runtime/get_text.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     2956 2022-12-09 02:32:30.000000 philologic-4.7.5.0/philologic/runtime/link.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)      413 2022-11-22 16:35:28.000000 philologic-4.7.5.0/philologic/runtime/pages.py
+drwxr-xr-x   0 clovis    (1000) artfl     (1003)        0 2024-05-28 16:27:16.185078 philologic-4.7.5.0/philologic/runtime/reports/
+-rw-r--r--   0 clovis    (1000) artfl     (1003)      977 2022-11-22 16:35:28.000000 philologic-4.7.5.0/philologic/runtime/reports/__init__.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     7673 2022-11-22 16:35:28.000000 philologic-4.7.5.0/philologic/runtime/reports/aggregation.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     3242 2022-12-19 22:17:21.000000 philologic-4.7.5.0/philologic/runtime/reports/bibliography.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     5332 2023-11-13 19:06:30.000000 philologic-4.7.5.0/philologic/runtime/reports/collocation.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     2712 2023-11-13 18:46:16.000000 philologic-4.7.5.0/philologic/runtime/reports/concordance.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     2627 2022-11-22 16:35:28.000000 philologic-4.7.5.0/philologic/runtime/reports/filter_word_by_property.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     7830 2022-11-22 16:35:28.000000 philologic-4.7.5.0/philologic/runtime/reports/frequency.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     2507 2022-11-22 16:35:28.000000 philologic-4.7.5.0/philologic/runtime/reports/generate_word_frequency.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     3349 2022-11-22 16:35:28.000000 philologic-4.7.5.0/philologic/runtime/reports/kwic.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     7425 2022-11-22 16:35:28.000000 philologic-4.7.5.0/philologic/runtime/reports/landing_page.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     3074 2022-11-22 16:35:28.000000 philologic-4.7.5.0/philologic/runtime/reports/navigation.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     3870 2022-11-22 16:35:28.000000 philologic-4.7.5.0/philologic/runtime/reports/table_of_contents.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     4925 2022-11-22 16:35:28.000000 philologic-4.7.5.0/philologic/runtime/reports/time_series.py
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)      894 2022-11-22 16:35:28.000000 philologic-4.7.5.0/philologic/runtime/web_config.py
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)     6167 2022-11-22 16:35:28.000000 philologic-4.7.5.0/philologic/shlax.py
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)     8793 2022-11-22 16:35:28.000000 philologic-4.7.5.0/philologic/shlaxtree.py
+drwxr-xr-x   0 clovis    (1000) artfl     (1003)        0 2024-05-28 16:27:16.185078 philologic-4.7.5.0/philologic/utils/
+-rwxr-xr-x   0 clovis    (1000) artfl     (1003)      221 2022-11-22 16:35:28.000000 philologic-4.7.5.0/philologic/utils/__init__.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)      762 2022-11-22 16:35:28.000000 philologic-4.7.5.0/philologic/utils/convert_entities.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)      430 2022-11-22 16:35:28.000000 philologic-4.7.5.0/philologic/utils/load_module.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     1929 2022-11-22 16:35:28.000000 philologic-4.7.5.0/philologic/utils/metadata_type_handler.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     1113 2022-11-22 16:35:28.000000 philologic-4.7.5.0/philologic/utils/pretty_print.py
+-rw-r--r--   0 clovis    (1000) artfl     (1003)      581 2022-11-22 16:35:28.000000 philologic-4.7.5.0/philologic/utils/sort.py
+drwxr-xr-x   0 clovis    (1000) artfl     (1003)        0 2024-05-28 16:27:16.185078 philologic-4.7.5.0/philologic.egg-info/
+-rw-r--r--   0 clovis    (1000) artfl     (1003)    41516 2024-05-28 16:27:16.000000 philologic-4.7.5.0/philologic.egg-info/PKG-INFO
+-rw-r--r--   0 clovis    (1000) artfl     (1003)     2032 2024-05-28 16:27:16.000000 philologic-4.7.5.0/philologic.egg-info/SOURCES.txt
+-rw-r--r--   0 clovis    (1000) artfl     (1003)        1 2024-05-28 16:27:16.000000 philologic-4.7.5.0/philologic.egg-info/dependency_links.txt
+-rw-r--r--   0 clovis    (1000) artfl     (1003)       61 2024-05-28 16:27:16.000000 philologic-4.7.5.0/philologic.egg-info/entry_points.txt
+-rw-r--r--   0 clovis    (1000) artfl     (1003)       91 2024-05-28 16:27:16.000000 philologic-4.7.5.0/philologic.egg-info/requires.txt
+-rw-r--r--   0 clovis    (1000) artfl     (1003)       11 2024-05-28 16:27:16.000000 philologic-4.7.5.0/philologic.egg-info/top_level.txt
+-rw-r--r--   0 clovis    (1000) artfl     (1003)      869 2024-04-22 20:21:48.000000 philologic-4.7.5.0/pyproject.toml
+-rw-r--r--   0 clovis    (1000) artfl     (1003)       38 2024-05-28 16:27:16.185078 philologic-4.7.5.0/setup.cfg
```

### Comparing `philologic-4.7.4.4/LICENSE` & `philologic-4.7.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.4/philologic/Config.py` & `philologic-4.7.5.0/philologic/Config.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.4/philologic/TagCensus.py` & `philologic-4.7.5.0/philologic/TagCensus.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.4/philologic/loadtime/LoadFilters.py` & `philologic-4.7.5.0/philologic/loadtime/LoadFilters.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.4/philologic/loadtime/LoadOptions.py` & `philologic-4.7.5.0/philologic/loadtime/LoadOptions.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.4/philologic/loadtime/Loader.py` & `philologic-4.7.5.0/philologic/loadtime/Loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 #!/usr/bin/env python3
 """Standard PhiloLogic4 loader.
 Calls all parsing functions and stores data in index"""
 
 import collections
+import csv
 import datetime
 import math
 import os
 import pickle
 import shutil
 import sqlite3
 import sys
 import time
 from glob import iglob
 from json import dump
-import csv
 
 import lxml.etree
 import regex as re
 from black import FileMode, format_str
 from multiprocess import Pool
 from philologic.Config import MakeDBConfig, MakeWebConfig
 from philologic.loadtime.PostFilters import make_sentences_table, make_sql_table
@@ -923,16 +923,16 @@
 
 def setup_db_dir(db_destination, web_app_dir, force_delete=False):
     """Setup database directory"""
     try:
         os.mkdir(db_destination)
     except OSError:
         if force_delete is True:  # useful to run db loads with nohup
-            os.system("rm -rf %s" % db_destination)
-            os.mkdir(db_destination)
+            shutil.rmtree(db_destination)
+            os.makedirs(db_destination, exist_ok=True)  # in the event it does not get deleted.
         else:
             print("The database folder could not be created at %s" % db_destination)
             print("Do you want to delete this database? Yes/No")
             choice = input().lower()
             if choice.startswith("y"):
                 os.system("rm -rf %s" % db_destination)
                 os.mkdir(db_destination)
```

### Comparing `philologic-4.7.4.4/philologic/loadtime/OHCOVector.py` & `philologic-4.7.5.0/philologic/loadtime/OHCOVector.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.4/philologic/loadtime/Parser.py` & `philologic-4.7.5.0/philologic/loadtime/Parser.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.4/philologic/loadtime/PlainTextParser.py` & `philologic-4.7.5.0/philologic/loadtime/PlainTextParser.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.4/philologic/loadtime/PostFilters.py` & `philologic-4.7.5.0/philologic/loadtime/PostFilters.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.4/philologic/runtime/DB.py` & `philologic-4.7.5.0/philologic/runtime/DB.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.4/philologic/runtime/FragmentParser.py` & `philologic-4.7.5.0/philologic/runtime/FragmentParser.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.4/philologic/runtime/HitList.py` & `philologic-4.7.5.0/philologic/runtime/HitList.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.4/philologic/runtime/HitWrapper.py` & `philologic-4.7.5.0/philologic/runtime/HitWrapper.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.4/philologic/runtime/MetadataQuery.py` & `philologic-4.7.5.0/philologic/runtime/MetadataQuery.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.4/philologic/runtime/ObjectFormatter.py` & `philologic-4.7.5.0/philologic/runtime/ObjectFormatter.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.4/philologic/runtime/Query.py` & `philologic-4.7.5.0/philologic/runtime/Query.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.4/philologic/runtime/QuerySyntax.py` & `philologic-4.7.5.0/philologic/runtime/QuerySyntax.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.4/philologic/runtime/WSGIHandler.py` & `philologic-4.7.5.0/philologic/runtime/WSGIHandler.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.4/philologic/runtime/__init__.py` & `philologic-4.7.5.0/philologic/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.4/philologic/runtime/access_control.py` & `philologic-4.7.5.0/philologic/runtime/access_control.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.4/philologic/runtime/citations.py` & `philologic-4.7.5.0/philologic/runtime/citations.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.4/philologic/runtime/find_similar_words.py` & `philologic-4.7.5.0/philologic/runtime/find_similar_words.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.4/philologic/runtime/get_text.py` & `philologic-4.7.5.0/philologic/runtime/get_text.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.4/philologic/runtime/link.py` & `philologic-4.7.5.0/philologic/runtime/link.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.4/philologic/runtime/reports/__init__.py` & `philologic-4.7.5.0/philologic/runtime/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.4/philologic/runtime/reports/aggregation.py` & `philologic-4.7.5.0/philologic/runtime/reports/aggregation.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.4/philologic/runtime/reports/bibliography.py` & `philologic-4.7.5.0/philologic/runtime/reports/bibliography.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.4/philologic/runtime/reports/collocation.py` & `philologic-4.7.5.0/philologic/runtime/reports/collocation.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.4/philologic/runtime/reports/concordance.py` & `philologic-4.7.5.0/philologic/runtime/reports/concordance.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.4/philologic/runtime/reports/filter_word_by_property.py` & `philologic-4.7.5.0/philologic/runtime/reports/filter_word_by_property.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.4/philologic/runtime/reports/frequency.py` & `philologic-4.7.5.0/philologic/runtime/reports/frequency.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.4/philologic/runtime/reports/generate_word_frequency.py` & `philologic-4.7.5.0/philologic/runtime/reports/generate_word_frequency.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.4/philologic/runtime/reports/kwic.py` & `philologic-4.7.5.0/philologic/runtime/reports/kwic.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.4/philologic/runtime/reports/landing_page.py` & `philologic-4.7.5.0/philologic/runtime/reports/landing_page.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.4/philologic/runtime/reports/navigation.py` & `philologic-4.7.5.0/philologic/runtime/reports/navigation.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.4/philologic/runtime/reports/table_of_contents.py` & `philologic-4.7.5.0/philologic/runtime/reports/table_of_contents.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.4/philologic/runtime/reports/time_series.py` & `philologic-4.7.5.0/philologic/runtime/reports/time_series.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.4/philologic/runtime/web_config.py` & `philologic-4.7.5.0/philologic/runtime/web_config.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.4/philologic/shlax.py` & `philologic-4.7.5.0/philologic/shlax.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.4/philologic/shlaxtree.py` & `philologic-4.7.5.0/philologic/shlaxtree.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.4/philologic/utils/convert_entities.py` & `philologic-4.7.5.0/philologic/utils/convert_entities.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.4/philologic/utils/metadata_type_handler.py` & `philologic-4.7.5.0/philologic/utils/metadata_type_handler.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.4/philologic/utils/pretty_print.py` & `philologic-4.7.5.0/philologic/utils/pretty_print.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.4/philologic/utils/sort.py` & `philologic-4.7.5.0/philologic/utils/sort.py`

 * *Files identical despite different names*

### Comparing `philologic-4.7.4.4/philologic.egg-info/SOURCES.txt` & `philologic-4.7.5.0/philologic.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 LICENSE
 README
-setup.py
+pyproject.toml
 philologic/Config.py
 philologic/TagCensus.py
 philologic/__init__.py
 philologic/_version.py
 philologic/shlax.py
 philologic/shlaxtree.py
 philologic.egg-info/PKG-INFO
 philologic.egg-info/SOURCES.txt
 philologic.egg-info/dependency_links.txt
+philologic.egg-info/entry_points.txt
 philologic.egg-info/requires.txt
 philologic.egg-info/top_level.txt
 philologic/loadtime/LoadFilters.py
 philologic/loadtime/LoadOptions.py
 philologic/loadtime/Loader.py
 philologic/loadtime/OHCOVector.py
 philologic/loadtime/Parser.py
+philologic/loadtime/PhiloLoad.py
 philologic/loadtime/PlainTextParser.py
 philologic/loadtime/PostFilters.py
 philologic/loadtime/__init__.py
 philologic/runtime/DB.py
 philologic/runtime/FragmentParser.py
 philologic/runtime/HitList.py
 philologic/runtime/HitWrapper.py
@@ -52,9 +54,8 @@
 philologic/runtime/reports/table_of_contents.py
 philologic/runtime/reports/time_series.py
 philologic/utils/__init__.py
 philologic/utils/convert_entities.py
 philologic/utils/load_module.py
 philologic/utils/metadata_type_handler.py
 philologic/utils/pretty_print.py
-philologic/utils/sort.py
-scripts/philoload4
+philologic/utils/sort.py
```

### Comparing `philologic-4.7.4.4/scripts/philoload4` & `philologic-4.7.5.0/philologic/loadtime/PhiloLoad.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #!/usr/bin/env python3
 
 import os
 import sys
 
-from philologic.loadtime.LoadOptions import LoadOptions, CONFIG_FILE
 from philologic.loadtime.Loader import Loader, setup_db_dir
+from philologic.loadtime.LoadOptions import CONFIG_FILE, LoadOptions
 
 os.environ["LC_ALL"] = "C"  # Exceedingly important to get uniform sort order.
 os.environ["PYTHONIOENCODING"] = "utf-8"
 
 
-if __name__ == "__main__":
+def philoload():
     load_options = LoadOptions()
     load_options.parse(sys.argv)
     setup_db_dir(load_options["db_destination"], load_options["web_app_dir"], force_delete=load_options.force_delete)
 
     # Database load
     l = Loader.set_class_attributes(load_options.values)
     l.add_files(load_options.files)
```

### Comparing `philologic-4.7.4.4/setup.py` & `philologic-4.7.5.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,43 @@
-"""Install script for PhiloLogic Python library"""
-from setuptools import setup
 
-with open("README", encoding="utf8") as input_file:
-    long_description = input_file.read()
+[build-system]
+requires = ["setuptools>=61.0", "wheel", "build"]
+build-backend = "setuptools.build_meta"
 
+[project]
+name = "philologic"
+version = "4.7.5.0"
+authors = [
+    { name = "Clovis Gladstone", email = "clovisgladstone@artfl.uchicago.edu" },
+]
+license = { file = "LICENSE" }
+description = "A concordance search engine for TEI-XML"
+readme = "README"
+urls = { Homepage = "https://github.com/ARTFL-Project/PhiloLogic4" }
 
-setup(
-    name="philologic",
-    author="Clovis Gladstone",
-    author_email="clovisgladstone@artfl.uchicago.edu",
-    description="A concordance search engine for TEI-XML",
-    long_description=long_description,
-    url="https://github.com/ARTFL-Project/PhiloLogic4",
-    packages=[
-        "philologic",
-        "philologic.runtime",
-        "philologic.utils",
-        "philologic.runtime.reports",
-        "philologic.loadtime",
-    ],
-    scripts=["scripts/philoload4"],
-    install_requires=[
-        "regex",
-        "lxml",
-        "python-levenshtein",
-        "natsort",
-        "multiprocess",
-        "tqdm",
-        "orjson",
-        "black",
-        "msgpack",
-        "unidecode",
-        "lz4",
-    ],
-    python_requires=">=3.8",
-    use_scm_version={
-        "root": "..",
-        "relative_to": __file__,
-        "local_scheme": "no-local-version",
-        "version_scheme": "guess-next-dev",
-    },
-    setup_requires=["setuptools_scm"],
-)
+requires-python = ">=3.10"
+dependencies = [
+    "regex",
+    "lxml",
+    "python-levenshtein",
+    "natsort",
+    "multiprocess",
+    "tqdm",
+    "orjson",
+    "black",
+    "msgpack",
+    "unidecode",
+    "lz4",
+]
+
+[project.scripts]
+philoload4 = "philologic.loadtime:philoload"
+
+
+[tool.setuptools]
+packages = [
+    "philologic",
+    "philologic.runtime",
+    "philologic.utils",
+    "philologic.runtime.reports",
+    "philologic.loadtime",
+]
```

