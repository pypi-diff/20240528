# Comparing `tmp/mscore-1.0.0.tar.gz` & `tmp/mscore-24.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mscore-1.0.0.tar", last modified: Fri Feb  9 19:00:45 2024, max compression
+gzip compressed data, was "mscore-24.1.1.tar", last modified: Thu Apr 18 15:35:15 2024, max compression
```

## Comparing `mscore-1.0.0.tar` & `mscore-24.1.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxr-x   0 nitromav  (1000) nitromav  (1000)        0 2024-02-09 19:00:45.734709 mscore-1.0.0/
--rw-r--r--   0 nitromav  (1000) nitromav  (1000)     8677 2024-02-09 19:00:45.734709 mscore-1.0.0/PKG-INFO
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     7917 2024-02-06 18:29:06.000000 mscore-1.0.0/README.md
-drwxrwxr-x   0 nitromav  (1000) nitromav  (1000)        0 2024-02-09 19:00:45.654709 mscore-1.0.0/mscore/
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     1188 2024-02-09 19:00:37.000000 mscore-1.0.0/mscore/__init__.pye
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)       84 2023-12-22 13:38:45.000000 mscore-1.0.0/mscore/__main__.py
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     2319 2024-02-09 19:00:38.000000 mscore-1.0.0/mscore/activate.pye
-drwxrwxr-x   0 nitromav  (1000) nitromav  (1000)        0 2024-02-09 19:00:45.658709 mscore-1.0.0/mscore/data_variables/
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)      149 2024-02-09 19:00:40.000000 mscore-1.0.0/mscore/data_variables/__init__.pye
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)    20525 2024-02-09 19:00:40.000000 mscore-1.0.0/mscore/data_variables/hcc_descriptors.pye
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     8457 2024-02-09 19:00:41.000000 mscore-1.0.0/mscore/data_variables/hierarchies.pye
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)    22040 2024-02-09 19:00:40.000000 mscore-1.0.0/mscore/data_variables/variable_dict.pye
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)    15341 2024-02-09 19:00:38.000000 mscore-1.0.0/mscore/demography_builder.pye
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     7883 2024-02-09 19:00:39.000000 mscore-1.0.0/mscore/demography_vars_applicator.pye
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)    14910 2024-02-09 19:00:38.000000 mscore-1.0.0/mscore/file_handler.pye
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     8814 2024-02-09 19:00:37.000000 mscore-1.0.0/mscore/hcc_handler.pye
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     9755 2024-02-09 19:00:39.000000 mscore-1.0.0/mscore/ram_models.pye
-drwxrwxr-x   0 nitromav  (1000) nitromav  (1000)        0 2024-02-09 19:00:45.650709 mscore-1.0.0/mscore/reference_data/
-drwxrwxr-x   0 nitromav  (1000) nitromav  (1000)        0 2024-02-09 19:00:45.670709 mscore-1.0.0/mscore/reference_data/Crosswalks/
--rwxrwxr-x   0 nitromav  (1000) nitromav  (1000)   110293 2023-06-23 19:57:48.000000 mscore-1.0.0/mscore/reference_data/Crosswalks/F2221CW.TXT
--rwxrwxr-x   0 nitromav  (1000) nitromav  (1000)   110523 2023-06-23 19:57:48.000000 mscore-1.0.0/mscore/reference_data/Crosswalks/F2222CW.TXT
--rwxrwxr-x   0 nitromav  (1000) nitromav  (1000)   121889 2023-06-23 19:57:48.000000 mscore-1.0.0/mscore/reference_data/Crosswalks/F2223CW.TXT
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)   112065 2023-11-03 17:05:55.000000 mscore-1.0.0/mscore/reference_data/Crosswalks/F2224CW.TXT
--rwxrwxr-x   0 nitromav  (1000) nitromav  (1000)   111973 2023-06-23 19:57:48.000000 mscore-1.0.0/mscore/reference_data/Crosswalks/F2421CW.TXT
--rwxrwxr-x   0 nitromav  (1000) nitromav  (1000)   112169 2023-06-23 19:57:48.000000 mscore-1.0.0/mscore/reference_data/Crosswalks/F2422CW.TXT
--rwxrwxr-x   0 nitromav  (1000) nitromav  (1000)   124500 2023-06-23 19:57:48.000000 mscore-1.0.0/mscore/reference_data/Crosswalks/F2423CW.TXT
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)   114449 2023-11-03 17:05:55.000000 mscore-1.0.0/mscore/reference_data/Crosswalks/F2424CW.TXT
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)   100259 2023-06-23 19:57:48.000000 mscore-1.0.0/mscore/reference_data/Crosswalks/F2824CW.TXT
-drwxrwxr-x   0 nitromav  (1000) nitromav  (1000)        0 2024-02-09 19:00:45.686709 mscore-1.0.0/mscore/reference_data/Model_Coefficients/
--rwxrwxr-x   0 nitromav  (1000) nitromav  (1000)    19597 2023-06-23 19:57:48.000000 mscore-1.0.0/mscore/reference_data/Model_Coefficients/2021_CMS-HCC_V22.csv
--rwxrwxr-x   0 nitromav  (1000) nitromav  (1000)    19597 2023-06-23 19:57:48.000000 mscore-1.0.0/mscore/reference_data/Model_Coefficients/2021_CMS-HCC_V222179O1.csv
--rwxrwxr-x   0 nitromav  (1000) nitromav  (1000)    20948 2023-06-23 19:57:48.000000 mscore-1.0.0/mscore/reference_data/Model_Coefficients/2021_CMS-HCC_V24.csv
--rwxrwxr-x   0 nitromav  (1000) nitromav  (1000)    20948 2023-06-23 19:57:48.000000 mscore-1.0.0/mscore/reference_data/Model_Coefficients/2021_CMS-HCC_V242186P1.csv
--rwxrwxr-x   0 nitromav  (1000) nitromav  (1000)    19597 2023-06-23 19:57:48.000000 mscore-1.0.0/mscore/reference_data/Model_Coefficients/2022_CMS-HCC_V22.csv
--rwxrwxr-x   0 nitromav  (1000) nitromav  (1000)    19597 2023-06-23 19:57:48.000000 mscore-1.0.0/mscore/reference_data/Model_Coefficients/2022_CMS-HCC_V222279O1.csv
--rwxrwxr-x   0 nitromav  (1000) nitromav  (1000)    20948 2023-06-23 19:57:48.000000 mscore-1.0.0/mscore/reference_data/Model_Coefficients/2022_CMS-HCC_V24.csv
--rwxrwxr-x   0 nitromav  (1000) nitromav  (1000)    20948 2023-06-23 19:57:48.000000 mscore-1.0.0/mscore/reference_data/Model_Coefficients/2022_CMS-HCC_V242286P1.csv
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)    19597 2023-06-23 19:57:48.000000 mscore-1.0.0/mscore/reference_data/Model_Coefficients/2023_CMS-HCC_V22.csv
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)    20948 2023-06-23 19:57:48.000000 mscore-1.0.0/mscore/reference_data/Model_Coefficients/2023_CMS-HCC_V24.csv
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)    19597 2023-11-03 17:05:55.000000 mscore-1.0.0/mscore/reference_data/Model_Coefficients/2024_CMS-HCC_V22.csv
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)    20948 2023-11-03 17:05:55.000000 mscore-1.0.0/mscore/reference_data/Model_Coefficients/2024_CMS-HCC_V24.csv
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)    24329 2023-06-23 19:57:48.000000 mscore-1.0.0/mscore/reference_data/Model_Coefficients/2024_CMS-HCC_V28.csv
-drwxrwxr-x   0 nitromav  (1000) nitromav  (1000)        0 2024-02-09 19:00:45.710709 mscore-1.0.0/mscore/reference_data/application_tables/
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)  3530400 2023-11-03 17:05:55.000000 mscore-1.0.0/mscore/reference_data/application_tables/application_format_fact.parquet
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)   149779 2023-11-03 17:05:55.000000 mscore-1.0.0/mscore/reference_data/application_tables/application_model_coefficient.parquet
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     4113 2023-11-03 17:05:55.000000 mscore-1.0.0/mscore/reference_data/application_tables/application_model_dimension.parquet
-drwxrwxr-x   0 nitromav  (1000) nitromav  (1000)        0 2024-02-09 19:00:45.722709 mscore-1.0.0/mscore/reference_data/model_formats_all_columns/
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)   663610 2023-06-23 19:57:48.000000 mscore-1.0.0/mscore/reference_data/model_formats_all_columns/2023_CMS-HCC_V222379O1_format.csv
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)   680986 2023-06-23 19:57:48.000000 mscore-1.0.0/mscore/reference_data/model_formats_all_columns/2023_CMS-HCC_V242386P1_format.csv
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)  1088405 2023-06-23 19:57:48.000000 mscore-1.0.0/mscore/reference_data/model_formats_all_columns/2024_CMS-HCC_V28_format.csv
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)    15680 2024-02-09 19:00:38.000000 mscore-1.0.0/mscore/scoring_handler.pye
-drwxrwxr-x   0 nitromav  (1000) nitromav  (1000)        0 2024-02-09 19:00:45.730709 mscore-1.0.0/mscore/utilities/
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)      935 2024-02-09 19:00:42.000000 mscore-1.0.0/mscore/utilities/__init__.pye
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)    10793 2024-02-09 19:00:43.000000 mscore-1.0.0/mscore/utilities/authentication.pye
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     6639 2024-02-09 19:00:39.000000 mscore-1.0.0/mscore/utilities/cli.pye
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     4159 2024-02-09 19:00:44.000000 mscore-1.0.0/mscore/utilities/context.pye
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     2010 2024-02-09 19:00:43.000000 mscore-1.0.0/mscore/utilities/data_models.pye
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)    11082 2024-02-09 19:00:43.000000 mscore-1.0.0/mscore/utilities/data_validation.pye
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     1964 2024-02-09 19:00:39.000000 mscore-1.0.0/mscore/utilities/file_organizer.pye
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     8354 2024-02-09 19:00:39.000000 mscore-1.0.0/mscore/utilities/licensing.pye
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     2247 2024-02-09 19:00:43.000000 mscore-1.0.0/mscore/utilities/log_handler.pye
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     2093 2024-02-09 19:00:42.000000 mscore-1.0.0/mscore/utilities/user_models.pye
-drwxrwxr-x   0 nitromav  (1000) nitromav  (1000)        0 2024-02-09 19:00:45.730709 mscore-1.0.0/mscore.egg-info/
--rw-r--r--   0 nitromav  (1000) nitromav  (1000)     8677 2024-02-09 19:00:45.000000 mscore-1.0.0/mscore.egg-info/PKG-INFO
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     2611 2024-02-09 19:00:45.000000 mscore-1.0.0/mscore.egg-info/SOURCES.txt
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)        1 2024-02-09 19:00:45.000000 mscore-1.0.0/mscore.egg-info/dependency_links.txt
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)       52 2024-02-09 19:00:45.000000 mscore-1.0.0/mscore.egg-info/entry_points.txt
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)       81 2024-02-09 19:00:45.000000 mscore-1.0.0/mscore.egg-info/requires.txt
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)        7 2024-02-09 19:00:45.000000 mscore-1.0.0/mscore.egg-info/top_level.txt
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     1191 2024-02-09 18:40:38.000000 mscore-1.0.0/pyproject.toml
--rw-rw-r--   0 nitromav  (1000) nitromav  (1000)       38 2024-02-09 19:00:45.734709 mscore-1.0.0/setup.cfg
+drwxrwxr-x   0 nitromav  (1000) nitromav  (1000)        0 2024-04-18 15:35:15.478664 mscore-24.1.1/
+-rw-r--r--   0 nitromav  (1000) nitromav  (1000)     8678 2024-04-18 15:35:15.478664 mscore-24.1.1/PKG-INFO
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     7917 2024-03-11 14:02:27.000000 mscore-24.1.1/README.md
+drwxrwxr-x   0 nitromav  (1000) nitromav  (1000)        0 2024-04-18 15:35:15.462657 mscore-24.1.1/mscore/
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     1239 2024-04-18 15:32:27.000000 mscore-24.1.1/mscore/__init__.pye
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)       84 2024-03-11 14:02:27.000000 mscore-24.1.1/mscore/__main__.py
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     2319 2024-04-18 15:32:48.000000 mscore-24.1.1/mscore/activate.pye
+drwxrwxr-x   0 nitromav  (1000) nitromav  (1000)        0 2024-04-18 15:35:15.466658 mscore-24.1.1/mscore/data_variables/
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)      149 2024-04-18 15:33:20.000000 mscore-24.1.1/mscore/data_variables/__init__.pye
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)    20525 2024-04-18 15:33:28.000000 mscore-24.1.1/mscore/data_variables/hcc_descriptors.pye
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     8457 2024-04-18 15:33:49.000000 mscore-24.1.1/mscore/data_variables/hierarchies.pye
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)    22040 2024-04-18 15:33:32.000000 mscore-24.1.1/mscore/data_variables/variable_dict.pye
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)    16374 2024-04-18 15:32:40.000000 mscore-24.1.1/mscore/demography_builder.pye
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     7883 2024-04-18 15:33:15.000000 mscore-24.1.1/mscore/demography_vars_applicator.pye
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)    14910 2024-04-18 15:32:52.000000 mscore-24.1.1/mscore/file_handler.pye
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     8814 2024-04-18 15:32:32.000000 mscore-24.1.1/mscore/hcc_handler.pye
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     9755 2024-04-18 15:32:56.000000 mscore-24.1.1/mscore/ram_models.pye
+drwxrwxr-x   0 nitromav  (1000) nitromav  (1000)        0 2024-04-18 15:35:15.462657 mscore-24.1.1/mscore/reference_data/
+drwxrwxr-x   0 nitromav  (1000) nitromav  (1000)        0 2024-04-18 15:35:15.466658 mscore-24.1.1/mscore/reference_data/Crosswalks/
+-rwxrwxr-x   0 nitromav  (1000) nitromav  (1000)   110293 2023-06-23 19:57:48.000000 mscore-24.1.1/mscore/reference_data/Crosswalks/F2221CW.TXT
+-rwxrwxr-x   0 nitromav  (1000) nitromav  (1000)   110523 2023-06-23 19:57:48.000000 mscore-24.1.1/mscore/reference_data/Crosswalks/F2222CW.TXT
+-rwxrwxr-x   0 nitromav  (1000) nitromav  (1000)   121889 2023-06-23 19:57:48.000000 mscore-24.1.1/mscore/reference_data/Crosswalks/F2223CW.TXT
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)   112657 2024-03-11 13:53:36.000000 mscore-24.1.1/mscore/reference_data/Crosswalks/F2224CW.TXT
+-rwxrwxr-x   0 nitromav  (1000) nitromav  (1000)   111973 2023-06-23 19:57:48.000000 mscore-24.1.1/mscore/reference_data/Crosswalks/F2421CW.TXT
+-rwxrwxr-x   0 nitromav  (1000) nitromav  (1000)   112169 2023-06-23 19:57:48.000000 mscore-24.1.1/mscore/reference_data/Crosswalks/F2422CW.TXT
+-rwxrwxr-x   0 nitromav  (1000) nitromav  (1000)   124500 2023-06-23 19:57:48.000000 mscore-24.1.1/mscore/reference_data/Crosswalks/F2423CW.TXT
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)   115090 2024-03-11 13:53:36.000000 mscore-24.1.1/mscore/reference_data/Crosswalks/F2424CW.TXT
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)   100809 2024-03-11 13:53:36.000000 mscore-24.1.1/mscore/reference_data/Crosswalks/F2824CW.TXT
+drwxrwxr-x   0 nitromav  (1000) nitromav  (1000)        0 2024-04-18 15:35:15.470661 mscore-24.1.1/mscore/reference_data/Model_Coefficients/
+-rwxrwxr-x   0 nitromav  (1000) nitromav  (1000)    19597 2023-06-23 19:57:48.000000 mscore-24.1.1/mscore/reference_data/Model_Coefficients/2021_CMS-HCC_V22.csv
+-rwxrwxr-x   0 nitromav  (1000) nitromav  (1000)    19597 2023-06-23 19:57:48.000000 mscore-24.1.1/mscore/reference_data/Model_Coefficients/2021_CMS-HCC_V222179O1.csv
+-rwxrwxr-x   0 nitromav  (1000) nitromav  (1000)    20948 2023-06-23 19:57:48.000000 mscore-24.1.1/mscore/reference_data/Model_Coefficients/2021_CMS-HCC_V24.csv
+-rwxrwxr-x   0 nitromav  (1000) nitromav  (1000)    20948 2023-06-23 19:57:48.000000 mscore-24.1.1/mscore/reference_data/Model_Coefficients/2021_CMS-HCC_V242186P1.csv
+-rwxrwxr-x   0 nitromav  (1000) nitromav  (1000)    19597 2023-06-23 19:57:48.000000 mscore-24.1.1/mscore/reference_data/Model_Coefficients/2022_CMS-HCC_V22.csv
+-rwxrwxr-x   0 nitromav  (1000) nitromav  (1000)    19597 2023-06-23 19:57:48.000000 mscore-24.1.1/mscore/reference_data/Model_Coefficients/2022_CMS-HCC_V222279O1.csv
+-rwxrwxr-x   0 nitromav  (1000) nitromav  (1000)    20948 2023-06-23 19:57:48.000000 mscore-24.1.1/mscore/reference_data/Model_Coefficients/2022_CMS-HCC_V24.csv
+-rwxrwxr-x   0 nitromav  (1000) nitromav  (1000)    20948 2023-06-23 19:57:48.000000 mscore-24.1.1/mscore/reference_data/Model_Coefficients/2022_CMS-HCC_V242286P1.csv
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)    19597 2023-06-23 19:57:48.000000 mscore-24.1.1/mscore/reference_data/Model_Coefficients/2023_CMS-HCC_V22.csv
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)    20948 2023-06-23 19:57:48.000000 mscore-24.1.1/mscore/reference_data/Model_Coefficients/2023_CMS-HCC_V24.csv
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)    19597 2023-11-03 17:05:55.000000 mscore-24.1.1/mscore/reference_data/Model_Coefficients/2024_CMS-HCC_V22.csv
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)    20948 2023-11-03 17:05:55.000000 mscore-24.1.1/mscore/reference_data/Model_Coefficients/2024_CMS-HCC_V24.csv
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)    24329 2023-06-23 19:57:48.000000 mscore-24.1.1/mscore/reference_data/Model_Coefficients/2024_CMS-HCC_V28.csv
+drwxrwxr-x   0 nitromav  (1000) nitromav  (1000)        0 2024-04-18 15:35:15.470661 mscore-24.1.1/mscore/reference_data/application_tables/
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)  1572021 2024-03-11 13:53:36.000000 mscore-24.1.1/mscore/reference_data/application_tables/application_format_fact.parquet
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)    68902 2024-03-11 13:53:36.000000 mscore-24.1.1/mscore/reference_data/application_tables/application_model_coefficient.parquet
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     3585 2024-03-11 13:53:36.000000 mscore-24.1.1/mscore/reference_data/application_tables/application_model_dimension.parquet
+drwxrwxr-x   0 nitromav  (1000) nitromav  (1000)        0 2024-04-18 15:35:15.470661 mscore-24.1.1/mscore/reference_data/model_formats_all_columns/
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)   663610 2023-06-23 19:57:48.000000 mscore-24.1.1/mscore/reference_data/model_formats_all_columns/2023_CMS-HCC_V222379O1_format.csv
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)   680986 2023-06-23 19:57:48.000000 mscore-24.1.1/mscore/reference_data/model_formats_all_columns/2023_CMS-HCC_V242386P1_format.csv
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)  1088405 2023-06-23 19:57:48.000000 mscore-24.1.1/mscore/reference_data/model_formats_all_columns/2024_CMS-HCC_V28_format.csv
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)    15680 2024-04-18 15:32:35.000000 mscore-24.1.1/mscore/scoring_handler.pye
+drwxrwxr-x   0 nitromav  (1000) nitromav  (1000)        0 2024-04-18 15:35:15.478664 mscore-24.1.1/mscore/utilities/
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)      935 2024-04-18 15:34:06.000000 mscore-24.1.1/mscore/utilities/__init__.pye
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)    10793 2024-04-18 15:34:29.000000 mscore-24.1.1/mscore/utilities/authentication.pye
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     6659 2024-04-18 15:33:06.000000 mscore-24.1.1/mscore/utilities/cli.pye
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     4159 2024-04-18 15:35:02.000000 mscore-24.1.1/mscore/utilities/context.pye
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     2010 2024-04-18 15:34:34.000000 mscore-24.1.1/mscore/utilities/data_models.pye
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)    11082 2024-04-18 15:34:45.000000 mscore-24.1.1/mscore/utilities/data_validation.pye
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     1964 2024-04-18 15:33:06.000000 mscore-24.1.1/mscore/utilities/file_organizer.pye
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     8354 2024-04-18 15:33:06.000000 mscore-24.1.1/mscore/utilities/licensing.pye
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     2247 2024-04-18 15:34:24.000000 mscore-24.1.1/mscore/utilities/log_handler.pye
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     2093 2024-04-18 15:34:19.000000 mscore-24.1.1/mscore/utilities/user_models.pye
+drwxrwxr-x   0 nitromav  (1000) nitromav  (1000)        0 2024-04-18 15:35:15.478664 mscore-24.1.1/mscore.egg-info/
+-rw-r--r--   0 nitromav  (1000) nitromav  (1000)     8678 2024-04-18 15:35:15.000000 mscore-24.1.1/mscore.egg-info/PKG-INFO
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     2611 2024-04-18 15:35:15.000000 mscore-24.1.1/mscore.egg-info/SOURCES.txt
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)        1 2024-04-18 15:35:15.000000 mscore-24.1.1/mscore.egg-info/dependency_links.txt
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)       52 2024-04-18 15:35:15.000000 mscore-24.1.1/mscore.egg-info/entry_points.txt
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)       81 2024-04-18 15:35:15.000000 mscore-24.1.1/mscore.egg-info/requires.txt
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)        7 2024-04-18 15:35:15.000000 mscore-24.1.1/mscore.egg-info/top_level.txt
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)     1192 2024-04-18 15:23:53.000000 mscore-24.1.1/pyproject.toml
+-rw-rw-r--   0 nitromav  (1000) nitromav  (1000)       38 2024-04-18 15:35:15.478664 mscore-24.1.1/setup.cfg
```

### Comparing `mscore-1.0.0/PKG-INFO` & `mscore-24.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mscore
-Version: 1.0.0
+Version: 24.1.1
 Summary: MScore: Risk Scores Made Easy
 Home-page: https://github.com/elevendatacorp/mscore.git
 Author: RAM Development Team
 Author-email: RAM Development Team <dev@riskadjustmentmodel.com>
 Project-URL: Homepage, https://riskadjustmentmodel.com/mscore-product
 Project-URL: Bug Tracker, https://github.com/elevendatacorp/mscore/issues
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mscore Version: 1.0.0 Summary: MScore: Risk Scores
+Metadata-Version: 2.1 Name: mscore Version: 24.1.1 Summary: MScore: Risk Scores
 Made Easy Home-page: https://github.com/elevendatacorp/mscore.git Author: RAM
 Development Team Author-email: RAM Development Team
 riskadjustmentmodel.com> Project-URL: Homepage, https://
 riskadjustmentmodel.com/mscore-product Project-URL: Bug Tracker, https://
 github.com/elevendatacorp/mscore/issues Classifier: Programming Language ::
 Python :: 3 Classifier: Operating System :: OS Independent Requires-Python:
 >=3.10 Description-Content-Type: text/markdown Requires-Dist: pandas Requires-
```

### Comparing `mscore-1.0.0/README.md` & `mscore-24.1.1/README.md`

 * *Files identical despite different names*

### Comparing `mscore-1.0.0/mscore/activate.pye` & `mscore-24.1.1/mscore/activate.pye`

 * *Files identical despite different names*

### Comparing `mscore-1.0.0/mscore/data_variables/hcc_descriptors.pye` & `mscore-24.1.1/mscore/data_variables/hcc_descriptors.pye`

 * *Files identical despite different names*

### Comparing `mscore-1.0.0/mscore/data_variables/hierarchies.pye` & `mscore-24.1.1/mscore/data_variables/hierarchies.pye`

 * *Files identical despite different names*

### Comparing `mscore-1.0.0/mscore/data_variables/variable_dict.pye` & `mscore-24.1.1/mscore/data_variables/variable_dict.pye`

 * *Files identical despite different names*

### Comparing `mscore-1.0.0/mscore/demography_vars_applicator.pye` & `mscore-24.1.1/mscore/demography_vars_applicator.pye`

 * *Files identical despite different names*

### Comparing `mscore-1.0.0/mscore/file_handler.pye` & `mscore-24.1.1/mscore/file_handler.pye`

 * *Files identical despite different names*

### Comparing `mscore-1.0.0/mscore/hcc_handler.pye` & `mscore-24.1.1/mscore/hcc_handler.pye`

 * *Files identical despite different names*

### Comparing `mscore-1.0.0/mscore/ram_models.pye` & `mscore-24.1.1/mscore/ram_models.pye`

 * *Files identical despite different names*

### Comparing `mscore-1.0.0/mscore/reference_data/Crosswalks/F2221CW.TXT` & `mscore-24.1.1/mscore/reference_data/Crosswalks/F2221CW.TXT`

 * *Files identical despite different names*

### Comparing `mscore-1.0.0/mscore/reference_data/Crosswalks/F2222CW.TXT` & `mscore-24.1.1/mscore/reference_data/Crosswalks/F2222CW.TXT`

 * *Files identical despite different names*

### Comparing `mscore-1.0.0/mscore/reference_data/Crosswalks/F2223CW.TXT` & `mscore-24.1.1/mscore/reference_data/Crosswalks/F2223CW.TXT`

 * *Files identical despite different names*

### Comparing `mscore-1.0.0/mscore/reference_data/Crosswalks/F2224CW.TXT` & `mscore-24.1.1/mscore/reference_data/Crosswalks/F2224CW.TXT`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 A412	2	
 A413	2	
 A414	2	
 A4150	2	
 A4151	2	
 A4152	2	
 A4153	2	
+A4154	2	
 A4159	2	
 A4181	2	
 A4189	2	
 A419	2	
 A420	115	
 A427	2	
 A430	115	
@@ -1271,74 +1272,80 @@
 D564	48	
 D565	48	
 D568	48	
 D5700	46	
 D5701	46	
 D5702	46	
 D5703	46	
+D5704	46	
 D5709	46	
 D571	46	
 D5720	46	
 D57211	46	
 D57212	46	
 D57213	46	
+D57214	46	
 D57218	46	
 D57219	46	
 D573	48	
 D5740	46	
 D57411	46	
 D57412	46	
 D57413	46	
+D57414	46	
 D57418	46	
 D57419	46	
 D5742	46	
 D57431	46	
 D57432	46	
 D57433	46	
+D57434	46	
 D57438	46	
 D57439	46	
 D5744	46	
 D57451	46	
 D57452	46	
 D57453	46	
+D57454	46	
 D57458	46	
 D57459	46	
 D5780	46	
 D57811	46	
 D57812	46	
 D57813	46	
+D57814	46	
 D57818	46	
 D57819	46	
 D580	48	
 D581	48	
 D582	48	
 D588	48	
 D589	48	
 D590	46	
 D5910	46	
 D5911	46	
 D5912	46	
 D5913	46	
 D5919	46	
 D592	46	
-D593	46	
 D5930	46	
 D5931	46	
 D5932	46	
 D5939	46	
 D594	46	
 D595	46	
 D596	46	
 D598	46	
 D599	46	
 D600	46	
 D601	46	
 D608	46	
 D609	46	
 D6101	46	
+D6102	46	
 D6109	46	
 D611	46	
 D612	46	
 D613	46	
 D61810	47	
 D61811	47	
 D61818	47	
@@ -1348,15 +1355,14 @@
 D640	48	
 D641	48	
 D642	48	
 D643	48	
 D65	48	
 D66	46	
 D67	46	
-D680	48	
 D6800	48	
 D6801	48	
 D68020	48	
 D68021	48	
 D68022	48	
 D68023	48	
 D68029	48	
@@ -1394,15 +1400,14 @@
 D703	47	
 D704	47	
 D708	47	
 D709	47	
 D71	47	
 D720	47	
 D7581	46	
-D7582	48	
 D75821	48	
 D75822	48	
 D75828	48	
 D75829	48	
 D7584	48	
 D761	47	
 D762	47	
@@ -1462,14 +1467,15 @@
 D8944	47	
 D8949	47	
 D89810	47	
 D89811	47	
 D89812	47	
 D89813	47	
 D8982	47	
+D8984	47	
 D8989	47	
 D899	47	
 E035	23	
 E0800	17	
 E0801	17	
 E0810	17	
 E0811	17	
@@ -2036,14 +2042,20 @@
 E1365	18	
 E1369	18	
 E138	18	
 E139	19	
 E15	23	
 E200	23	
 E208	23	
+E20810	23	
+E20811	23	
+E20812	23	
+E20818	23	
+E20819	23	
+E2089	23	
 E209	23	
 E210	23	
 E211	23	
 E212	23	
 E213	23	
 E214	23	
 E215	23	
@@ -2198,14 +2210,15 @@
 E7289	23	
 E729	23	
 E7400	23	
 E7401	23	
 E7402	23	
 E7403	23	
 E7404	23	
+E7405	23	
 E7409	23	
 E7420	23	
 E7421	23	
 E7429	23	
 E744	23	
 E74810	23	
 E74818	23	
@@ -2237,14 +2250,17 @@
 E770	23	
 E771	23	
 E778	23	
 E779	23	
 E791	23	
 E792	23	
 E798	23	
+E7981	23	
+E7982	23	
+E7989	23	
 E799	23	
 E800	23	
 E801	23	
 E8020	23	
 E8021	23	
 E8029	23	
 E803	23	
@@ -2263,16 +2279,18 @@
 E8582	23	
 E8589	23	
 E859	23	
 E8801	23	
 E8840	23	
 E8841	23	
 E8842	23	
+E8843	23	
 E8849	23	
 E8889	23	
+E88A	21	
 E892	23	
 E893	23	
 E896	23	
 F10120	55	
 F10121	55	
 F10129	55	
 F10130	55	
@@ -2753,14 +2771,16 @@
 G110	72	
 G1110	72	
 G1111	72	
 G1119	72	
 G112	72	
 G113	72	
 G114	72	
+G115	72	
+G116	72	
 G118	72	
 G119	72	
 G120	72	
 G121	72	
 G1220	73	
 G1221	73	
 G1222	73	
@@ -2769,24 +2789,30 @@
 G1225	73	
 G1229	73	
 G128	72	
 G129	72	
 G130	75	
 G131	75	
 G20	78	
+G20A1	78	
+G20A2	78	
+G20B1	78	
+G20B2	78	
+G20C	78	
 G2111	78	
 G2119	78	
 G212	78	
 G213	78	
 G214	78	
 G218	78	
 G219	78	
 G230	78	
 G231	78	
 G232	78	
+G233	78	
 G238	78	
 G239	78	
 G320	72	
 G3281	72	
 G35	77	
 G360	77	
 G361	77	
@@ -2795,14 +2821,16 @@
 G370	77	
 G371	77	
 G372	77	
 G373	72	
 G374	72	
 G375	77	
 G378	77	
+G3781	77	
+G3789	77	
 G379	77	
 G40001	79	
 G40009	79	
 G40011	79	
 G40019	79	
 G40101	79	
 G40109	79	
@@ -2846,14 +2874,18 @@
 G40A09	79	
 G40A11	79	
 G40A19	79	
 G40B01	79	
 G40B09	79	
 G40B11	79	
 G40B19	79	
+G40C01	79	
+G40C09	79	
+G40C11	79	
+G40C19	79	
 G546	189	
 G547	189	
 G610	75	
 G611	75	
 G6181	75	
 G6182	75	
 G6189	75	
@@ -2977,14 +3009,26 @@
 H353231	124	
 H353232	124	
 H353233	124	
 H353290	124	
 H353291	124	
 H353292	124	
 H353293	124	
+H36811	46	
+H36812	46	
+H36813	46	
+H36819	46	
+H36821	46	
+H36821	122	D
+H36822	46	
+H36822	122	D
+H36823	46	
+H36823	122	D
+H36829	46	
+H36829	122	D
 H4310	122	
 H4311	122	
 H4312	122	
 H4313	122	
 H49811	23	
 H49812	23	
 H49813	23	
@@ -2996,27 +3040,30 @@
 I1311	136	
 I132	85	
 I132	136	D
 I200	87	
 I201	88	
 I202	88	
 I208	88	
+I2081	88	
+I2089	88	
 I209	88	
 I2101	86	
 I2102	86	
 I2109	86	
 I2111	86	
 I2119	86	
 I2121	86	
 I2129	86	
 I213	86	
 I214	86	
 I219	86	
 I21A1	86	
 I21A9	86	
+I21B	86	
 I220	86	
 I221	86	
 I222	86	
 I228	86	
 I229	86	
 I230	87	
 I231	87	
@@ -3026,14 +3073,16 @@
 I235	86	
 I236	87	
 I237	87	
 I238	87	
 I240	87	
 I241	87	
 I248	87	
+I2481	87	
+I2489	87	
 I249	87	
 I25110	87	
 I25111	88	
 I25112	88	
 I25118	88	
 I25119	88	
 I25700	87	
@@ -3112,15 +3161,17 @@
 I43	85	
 I442	96	
 I462	84	
 I468	84	
 I469	84	
 I470	96	
 I471	96	
-I472	96	
+I4710	96	
+I4711	96	
+I4719	96	
 I4720	96	
 I4721	96	
 I4729	96	
 I479	96	
 I480	96	
 I4811	96	
 I4819	96	
@@ -3742,46 +3793,39 @@
 I70791	108	
 I70792	108	
 I70793	108	
 I70798	108	
 I70799	108	
 I7092	108	
 I7100	107	
-I7101	107	
 I71010	107	
 I71011	107	
 I71012	107	
 I71019	107	
 I7102	107	
 I7103	107	
-I711	107	
 I7110	107	
 I7111	107	
 I7112	107	
 I7113	107	
-I712	108	
 I7120	108	
 I7121	108	
 I7122	108	
 I7123	108	
-I713	107	
 I7130	107	
 I7131	107	
 I7132	107	
 I7133	107	
-I714	108	
 I7140	108	
 I7141	108	
 I7142	108	
 I7143	108	
-I715	107	
 I7150	107	
 I7151	107	
 I7152	107	
-I716	108	
 I7160	108	
 I7161	108	
 I7162	108	
 I718	107	
 I719	108	
 I720	108	
 I721	108	
@@ -4073,31 +4117,38 @@
 J15211	114	
 J15212	114	
 J1529	114	
 J153	115	
 J154	115	
 J155	114	
 J156	114	
+J1561	114	
+J1569	114	
 J158	114	
 J181	115	
 J410	111	
 J411	111	
 J418	111	
 J42	111	
 J430	111	
 J431	111	
 J432	111	
 J438	111	
 J439	111	
 J440	111	
 J441	111	
+J4481	111	
+J4489	111	
 J449	111	
 J470	112	
 J471	112	
 J479	112	
+J4A0	186	
+J4A8	186	
+J4A9	186	
 J60	112	
 J61	112	
 J620	112	
 J628	112	
 J630	112	
 J631	112	
 J632	112	
@@ -6140,15 +6191,14 @@
 Q079	72	
 Q8500	12	
 Q8501	12	
 Q8502	12	
 Q8503	12	
 Q8509	12	
 Q851	12	
-Q858	12	
 Q8581	12	
 Q8582	12	
 Q8583	12	
 Q8589	12	
 Q859	12	
 R092	83	
 R4020	80	
@@ -6193,14 +6243,15 @@
 R402433	80	
 R402434	80	
 R402440	80	
 R402441	80	
 R402442	80	
 R402443	80	
 R402444	80	
+R402A	80	
 R403	80	
 R4588	58	
 R532	70	
 R5600	79	
 R5601	79	
 R561	79	
 R569	79	
@@ -9010,14 +9061,16 @@
 T565X2S	58	
 T566X2A	58	
 T566X2S	58	
 T567X2A	58	
 T567X2S	58	
 T56812A	58	
 T56812S	58	
+T56822A	58	
+T56822S	58	
 T56892A	58	
 T56892S	58	
 T5692XA	58	
 T5692XS	58	
 T570X2A	58	
 T570X2S	58	
 T571X2A	58	
@@ -9819,14 +9872,16 @@
 Z89611	189	
 Z89612	189	
 Z89619	189	
 Z9115	134	
 Z91151	134	
 Z91158	134	
 Z91A5	134	
+Z91A51	134	
+Z91A58	134	
 Z930	82	
 Z931	188	
 Z932	188	
 Z933	188	
 Z934	188	
 Z9350	188	
 Z9351	188
```

### Comparing `mscore-1.0.0/mscore/reference_data/Crosswalks/F2421CW.TXT` & `mscore-24.1.1/mscore/reference_data/Crosswalks/F2421CW.TXT`

 * *Files identical despite different names*

### Comparing `mscore-1.0.0/mscore/reference_data/Crosswalks/F2422CW.TXT` & `mscore-24.1.1/mscore/reference_data/Crosswalks/F2422CW.TXT`

 * *Files identical despite different names*

### Comparing `mscore-1.0.0/mscore/reference_data/Crosswalks/F2423CW.TXT` & `mscore-24.1.1/mscore/reference_data/Crosswalks/F2423CW.TXT`

 * *Files identical despite different names*

### Comparing `mscore-1.0.0/mscore/reference_data/Crosswalks/F2424CW.TXT` & `mscore-24.1.1/mscore/reference_data/Crosswalks/F2424CW.TXT`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 A412	2	
 A413	2	
 A414	2	
 A4150	2	
 A4151	2	
 A4152	2	
 A4153	2	
+A4154	2	
 A4159	2	
 A4181	2	
 A4189	2	
 A419	2	
 A420	115	
 A427	2	
 A430	115	
@@ -1281,74 +1282,80 @@
 D564	48	
 D565	48	
 D568	48	
 D5700	46	
 D5701	46	
 D5702	46	
 D5703	46	
+D5704	46	
 D5709	46	
 D571	46	
 D5720	46	
 D57211	46	
 D57212	46	
 D57213	46	
+D57214	46	
 D57218	46	
 D57219	46	
 D573	48	
 D5740	46	
 D57411	46	
 D57412	46	
 D57413	46	
+D57414	46	
 D57418	46	
 D57419	46	
 D5742	46	
 D57431	46	
 D57432	46	
 D57433	46	
+D57434	46	
 D57438	46	
 D57439	46	
 D5744	46	
 D57451	46	
 D57452	46	
 D57453	46	
+D57454	46	
 D57458	46	
 D57459	46	
 D5780	46	
 D57811	46	
 D57812	46	
 D57813	46	
+D57814	46	
 D57818	46	
 D57819	46	
 D580	48	
 D581	48	
 D582	48	
 D588	48	
 D589	48	
 D590	46	
 D5910	46	
 D5911	46	
 D5912	46	
 D5913	46	
 D5919	46	
 D592	46	
-D593	46	
 D5930	46	
 D5931	46	
 D5932	46	
 D5939	46	
 D594	46	
 D595	46	
 D596	46	
 D598	46	
 D599	46	
 D600	46	
 D601	46	
 D608	46	
 D609	46	
 D6101	46	
+D6102	46	
 D6109	46	
 D611	46	
 D612	46	
 D613	46	
 D61810	47	
 D61811	47	
 D61818	47	
@@ -1358,15 +1365,14 @@
 D640	48	
 D641	48	
 D642	48	
 D643	48	
 D65	48	
 D66	46	
 D67	46	
-D680	48	
 D6800	48	
 D6801	48	
 D68020	48	
 D68021	48	
 D68022	48	
 D68023	48	
 D68029	48	
@@ -1404,15 +1410,14 @@
 D703	47	
 D704	47	
 D708	47	
 D709	47	
 D71	47	
 D720	47	
 D7581	46	
-D7582	48	
 D75821	48	
 D75822	48	
 D75828	48	
 D75829	48	
 D7584	48	
 D761	47	
 D762	47	
@@ -1472,14 +1477,15 @@
 D8944	47	
 D8949	47	
 D89810	47	
 D89811	47	
 D89812	47	
 D89813	47	
 D8982	47	
+D8984	47	
 D8989	47	
 D899	47	
 E035	23	
 E0800	17	
 E0801	17	
 E0810	17	
 E0811	17	
@@ -2046,14 +2052,20 @@
 E1365	18	
 E1369	18	
 E138	18	
 E139	19	
 E15	23	
 E200	23	
 E208	23	
+E20810	23	
+E20811	23	
+E20812	23	
+E20818	23	
+E20819	23	
+E2089	23	
 E209	23	
 E210	23	
 E211	23	
 E212	23	
 E213	23	
 E214	23	
 E215	23	
@@ -2208,14 +2220,15 @@
 E7289	23	
 E729	23	
 E7400	23	
 E7401	23	
 E7402	23	
 E7403	23	
 E7404	23	
+E7405	23	
 E7409	23	
 E7420	23	
 E7421	23	
 E7429	23	
 E744	23	
 E74810	23	
 E74818	23	
@@ -2237,14 +2250,16 @@
 E75242	23	
 E75243	23	
 E75244	23	
 E75248	23	
 E75249	23	
 E7525	52	
 E7526	52	
+E7527	52	
+E7528	52	
 E7529	52	
 E753	23	
 E754	52	
 E7601	23	
 E7602	23	
 E7603	23	
 E761	23	
@@ -2259,14 +2274,17 @@
 E770	23	
 E771	23	
 E778	23	
 E779	23	
 E791	23	
 E792	23	
 E798	23	
+E7981	23	
+E7982	23	
+E7989	23	
 E799	23	
 E800	23	
 E801	23	
 E8020	23	
 E8021	23	
 E8029	23	
 E803	23	
@@ -2285,21 +2303,22 @@
 E8582	23	
 E8589	23	
 E859	23	
 E8801	23	
 E8840	23	
 E8841	23	
 E8842	23	
+E8843	23	
 E8849	23	
 E8889	23	
+E88A	21	
 E892	23	
 E893	23	
 E896	23	
 F0150	52	
-F0151	51	
 F01511	51	
 F01518	51	
 F0152	51	
 F0153	51	
 F0154	51	
 F01A0	52	
 F01A11	51	
@@ -2316,15 +2335,14 @@
 F01C0	52	
 F01C11	51	
 F01C18	51	
 F01C2	51	
 F01C3	51	
 F01C4	51	
 F0280	52	
-F0281	51	
 F02811	51	
 F02818	51	
 F0282	51	
 F0283	51	
 F0284	51	
 F02A0	52	
 F02A11	51	
@@ -2341,15 +2359,14 @@
 F02C0	52	
 F02C11	51	
 F02C18	51	
 F02C2	51	
 F02C3	51	
 F02C4	51	
 F0390	52	
-F0391	51	
 F03911	51	
 F03918	51	
 F0392	51	
 F0393	51	
 F0394	51	
 F03A0	52	
 F03A11	51	
@@ -2885,14 +2902,16 @@
 G110	72	
 G1110	72	
 G1111	72	
 G1119	72	
 G112	72	
 G113	72	
 G114	72	
+G115	72	
+G116	72	
 G118	72	
 G119	72	
 G120	72	
 G121	72	
 G1220	73	
 G1221	73	
 G1222	73	
@@ -2903,38 +2922,46 @@
 G128	72	
 G129	72	
 G130	75	
 G131	75	
 G132	52	
 G138	52	
 G20	78	
+G20A1	78	
+G20A2	78	
+G20B1	78	
+G20B2	78	
+G20C	78	
 G2111	78	
 G2119	78	
 G212	78	
 G213	78	
 G214	78	
 G218	78	
 G219	78	
 G230	78	
 G231	78	
 G232	78	
+G233	78	
 G238	78	
 G239	78	
 G300	52	
 G301	52	
 G308	52	
 G309	52	
 G3101	52	
 G3109	52	
 G311	52	
 G312	52	
+G3180	52	
 G3181	52	
 G3182	52	
 G3183	52	
 G3185	52	
+G3186	52	
 G3189	52	
 G319	52	
 G320	72	
 G3281	72	
 G35	77	
 G360	77	
 G361	77	
@@ -2943,14 +2970,16 @@
 G370	77	
 G371	77	
 G372	77	
 G373	72	
 G374	72	
 G375	77	
 G378	77	
+G3781	77	
+G3789	77	
 G379	77	
 G40001	79	
 G40009	79	
 G40011	79	
 G40019	79	
 G40101	79	
 G40109	79	
@@ -2994,14 +3023,18 @@
 G40A09	79	
 G40A11	79	
 G40A19	79	
 G40B01	79	
 G40B09	79	
 G40B11	79	
 G40B19	79	
+G40C01	79	
+G40C09	79	
+G40C11	79	
+G40C19	79	
 G546	189	
 G547	189	
 G610	75	
 G611	75	
 G6181	75	
 G6182	75	
 G6189	75	
@@ -3097,22 +3130,26 @@
 G8382	104	
 G8383	104	
 G8384	104	
 G8389	104	
 G839	104	
 G901	72	
 G903	78	
+G90B	52	
 G910	51	
 G911	51	
 G912	51	
 G913	51	
 G914	51	
 G918	51	
 G919	51	
 G931	80	
+G9342	52	
+G9343	52	
+G9344	52	
 G935	80	
 G936	80	
 G937	52	
 G950	72	
 G9511	72	
 G9519	72	
 G9520	72	
@@ -3133,14 +3170,26 @@
 H353231	124	
 H353232	124	
 H353233	124	
 H353290	124	
 H353291	124	
 H353292	124	
 H353293	124	
+H36811	46	
+H36812	46	
+H36813	46	
+H36819	46	
+H36821	46	
+H36821	122	D
+H36822	46	
+H36822	122	D
+H36823	46	
+H36823	122	D
+H36829	46	
+H36829	122	D
 H4310	122	
 H4311	122	
 H4312	122	
 H4313	122	
 H49811	23	
 H49812	23	
 H49813	23	
@@ -3152,27 +3201,30 @@
 I1311	136	
 I132	85	
 I132	136	D
 I200	87	
 I201	88	
 I202	88	
 I208	88	
+I2081	88	
+I2089	88	
 I209	88	
 I2101	86	
 I2102	86	
 I2109	86	
 I2111	86	
 I2119	86	
 I2121	86	
 I2129	86	
 I213	86	
 I214	86	
 I219	86	
 I21A1	86	
 I21A9	86	
+I21B	86	
 I220	86	
 I221	86	
 I222	86	
 I228	86	
 I229	86	
 I230	87	
 I231	87	
@@ -3182,14 +3234,16 @@
 I235	86	
 I236	87	
 I237	87	
 I238	87	
 I240	87	
 I241	87	
 I248	87	
+I2481	87	
+I2489	87	
 I249	87	
 I25110	87	
 I25111	88	
 I25112	88	
 I25118	88	
 I25119	88	
 I25700	87	
@@ -3268,15 +3322,17 @@
 I43	85	
 I442	96	
 I462	84	
 I468	84	
 I469	84	
 I470	96	
 I471	96	
-I472	96	
+I4710	96	
+I4711	96	
+I4719	96	
 I4720	96	
 I4721	96	
 I4729	96	
 I479	96	
 I480	96	
 I4811	96	
 I4819	96	
@@ -3899,46 +3955,39 @@
 I70791	108	
 I70792	108	
 I70793	108	
 I70798	108	
 I70799	108	
 I7092	108	
 I7100	107	
-I7101	107	
 I71010	107	
 I71011	107	
 I71012	107	
 I71019	107	
 I7102	107	
 I7103	107	
-I711	107	
 I7110	107	
 I7111	107	
 I7112	107	
 I7113	107	
-I712	108	
 I7120	108	
 I7121	108	
 I7122	108	
 I7123	108	
-I713	107	
 I7130	107	
 I7131	107	
 I7132	107	
 I7133	107	
-I714	108	
 I7140	108	
 I7141	108	
 I7142	108	
 I7143	108	
-I715	107	
 I7150	107	
 I7151	107	
 I7152	107	
-I716	108	
 I7160	108	
 I7161	108	
 I7162	108	
 I718	107	
 I719	108	
 I720	108	
 I721	108	
@@ -4230,31 +4279,38 @@
 J15211	114	
 J15212	114	
 J1529	114	
 J153	115	
 J154	115	
 J155	114	
 J156	114	
+J1561	114	
+J1569	114	
 J158	114	
 J181	115	
 J410	111	
 J411	111	
 J418	111	
 J42	111	
 J430	111	
 J431	111	
 J432	111	
 J438	111	
 J439	111	
 J440	111	
 J441	111	
+J4481	111	
+J4489	111	
 J449	111	
 J470	112	
 J471	112	
 J479	112	
+J4A0	186	
+J4A8	186	
+J4A9	186	
 J60	112	
 J61	112	
 J620	112	
 J628	112	
 J630	112	
 J631	112	
 J632	112	
@@ -6325,15 +6381,14 @@
 Q079	72	
 Q8500	12	
 Q8501	12	
 Q8502	12	
 Q8503	12	
 Q8509	12	
 Q851	12	
-Q858	12	
 Q8581	12	
 Q8582	12	
 Q8583	12	
 Q8589	12	
 Q859	12	
 R092	83	
 R4020	80	
@@ -6378,14 +6433,15 @@
 R402433	80	
 R402434	80	
 R402440	80	
 R402441	80	
 R402442	80	
 R402443	80	
 R402444	80	
+R402A	80	
 R403	80	
 R4588	59	
 R532	70	
 R5600	79	
 R5601	79	
 R561	79	
 R569	79	
@@ -9237,14 +9293,16 @@
 T565X2S	59	
 T566X2A	59	
 T566X2S	59	
 T567X2A	59	
 T567X2S	59	
 T56812A	59	
 T56812S	59	
+T56822A	59	
+T56822S	59	
 T56892A	59	
 T56892S	59	
 T5692XA	59	
 T5692XS	59	
 T570X2A	59	
 T570X2S	59	
 T571X2A	59	
@@ -10046,14 +10104,16 @@
 Z89611	189	
 Z89612	189	
 Z89619	189	
 Z9115	134	
 Z91151	134	
 Z91158	134	
 Z91A5	134	
+Z91A51	134	
+Z91A58	134	
 Z930	82	
 Z931	188	
 Z932	188	
 Z933	188	
 Z934	188	
 Z9350	188	
 Z9351	188
```

### Comparing `mscore-1.0.0/mscore/reference_data/Crosswalks/F2824CW.TXT` & `mscore-24.1.1/mscore/reference_data/Crosswalks/F2824CW.TXT`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 A412	2	
 A413	2	
 A414	2	
 A4150	2	
 A4151	2	
 A4152	2	
 A4153	2	
+A4154	2	
 A4159	2	
 A4181	2	
 A4189	2	
 A419	2	
 A427	2	
 A480	263	
 A481	282	
@@ -1272,78 +1273,83 @@
 D561	108	
 D562	108	
 D565	108	
 D5700	107	
 D5701	107	
 D5702	107	
 D5703	107	
+D5704	107	
 D5709	107	
 D571	107	
 D5720	108	
 D57211	108	
 D57212	108	
 D57213	108	
+D57214	108	
 D57218	108	
 D57219	108	
 D5740	108	
 D57411	108	
 D57412	108	
 D57413	108	
+D57414	108	
 D57418	108	
 D57419	108	
 D5742	107	
 D57431	107	
 D57432	107	
 D57433	107	
+D57434	107	
 D57438	107	
 D57439	107	
 D5744	108	
 D57451	108	
 D57452	108	
 D57453	108	
+D57454	108	
 D57458	108	
 D57459	108	
 D5780	108	
 D57811	108	
 D57812	108	
 D57813	108	
+D57814	108	
 D57818	108	
 D57819	108	
 D5910	109	
 D5911	109	
 D5912	109	
 D5913	109	
 D5919	109	
-D593	109	
 D5930	109	
 D5931	109	
 D5932	109	
 D5939	109	
 D594	109	
 D595	109	
 D596	109	
 D598	109	
 D599	109	
 D600	109	
 D608	109	
 D609	109	
 D6101	109	
+D6102	109	
 D6109	109	
 D612	109	
 D613	109	
 D61818	109	
 D6182	109	
 D6189	109	
 D640	109	
 D641	109	
 D643	109	
 D644	109	
 D66	111	
 D67	111	
-D680	112	
 D6800	112	
 D6801	112	
 D68020	112	
 D68021	112	
 D68022	112	
 D68023	112	
 D68029	112	
@@ -1396,14 +1402,15 @@
 D863	387	
 D8686	93	
 D8687	93	
 D89810	454	
 D89811	454	
 D89812	454	
 D89813	454	
+D8984	115	
 E035	202	
 E0800	36	
 E0801	36	
 E0810	36	
 E0811	36	
 E0821	37	
 E0822	37	
@@ -1919,14 +1926,15 @@
 E662	48	
 E7253	50	
 E7400	50	
 E7401	50	
 E7402	49	
 E7403	50	
 E7404	50	
+E7405	50	
 E7409	50	
 E7521	49	
 E7522	49	
 E7601	49	
 E7602	49	
 E7603	49	
 E761	49	
@@ -1960,15 +1968,14 @@
 E8581	50	
 E8582	50	
 E8589	50	
 E859	50	
 E8801	50	
 E8889	50	
 F0150	127	
-F0151	127	
 F01511	127	
 F01518	127	
 F0152	127	
 F0153	127	
 F0154	127	
 F01A0	127	
 F01A11	127	
@@ -1985,15 +1992,14 @@
 F01C0	125	
 F01C11	125	
 F01C18	125	
 F01C2	125	
 F01C3	125	
 F01C4	125	
 F0280	127	
-F0281	127	
 F02811	127	
 F02818	127	
 F0282	127	
 F0283	127	
 F0284	127	
 F02A0	127	
 F02A11	127	
@@ -2010,15 +2016,14 @@
 F02C0	125	
 F02C11	125	
 F02C18	125	
 F02C2	125	
 F02C3	125	
 F02C4	125	
 F0390	127	
-F0391	127	
 F03911	127	
 F03918	127	
 F0392	127	
 F0393	127	
 F0394	127	
 F03A0	127	
 F03A11	127	
@@ -2520,14 +2525,16 @@
 G110	200	
 G1110	200	
 G1111	200	
 G1119	200	
 G112	200	
 G113	200	
 G114	200	
+G115	200	
+G116	200	
 G118	200	
 G119	200	
 G120	190	
 G121	190	
 G1220	190	
 G1221	190	
 G1222	190	
@@ -2535,46 +2542,56 @@
 G1224	190	
 G1225	190	
 G1229	190	
 G128	190	
 G129	190	
 G14	182	
 G20	199	
+G20A1	199	
+G20A2	199	
+G20B1	199	
+G20B2	199	
+G20C	199	
 G213	199	
 G214	199	
 G218	199	
 G219	199	
 G230	199	
 G231	199	
 G232	199	
+G233	199	
 G238	199	
 G239	199	
 G300	127	
 G301	127	
 G308	127	
 G309	127	
 G3101	127	
 G3109	127	
+G3180	200	
 G3181	127	
 G3182	127	
 G3183	127	
+G3186	127	
 G320	182	
 G3281	182	
 G35	198	
 G360	198	
 G361	198	
 G368	198	
 G369	198	
 G370	198	
 G371	198	
 G372	198	
 G373	182	
 G374	182	
 G375	198	
 G378	198	
+G3781	198	
+G3789	198	
 G379	198	
 G40001	201	
 G40009	201	
 G40011	201	
 G40019	201	
 G40101	201	
 G40109	201	
@@ -2618,14 +2635,18 @@
 G40A09	201	
 G40A11	201	
 G40A19	201	
 G40B01	201	
 G40B09	201	
 G40B11	201	
 G40B19	201	
+G40C01	201	
+G40C09	201	
+G40C11	201	
+G40C19	201	
 G546	409	
 G547	409	
 G6181	193	
 G6182	193	
 G7000	196	
 G7001	195	
 G701	196	
@@ -2709,22 +2730,26 @@
 G8382	254	
 G8383	254	
 G8384	254	
 G8389	254	
 G839	254	
 G901	182	
 G903	199	
+G90B	200	
 G910	127	
 G911	127	
 G912	127	
 G913	127	
 G914	127	
 G918	127	
 G919	127	
 G931	202	
+G9342	200	
+G9343	200	
+G9344	200	
 G935	202	
 G936	202	
 G937	127	
 G950	182	
 G9511	182	
 G9519	182	
 G9520	182	
@@ -2769,14 +2794,26 @@
 H353231	300	
 H353232	300	
 H353233	300	
 H353290	300	
 H353291	300	
 H353292	300	
 H353293	300	
+H36811	108	
+H36812	108	
+H36813	108	
+H36819	108	
+H36821	108	
+H36821	298	D
+H36822	108	
+H36822	298	D
+H36823	108	
+H36823	298	D
+H36829	108	
+H36829	298	D
 H4310	298	
 H4311	298	
 H4312	298	
 H4313	298	
 I0981	226	
 I110	226	
 I120	326	
@@ -2793,14 +2830,15 @@
 I2121	228	
 I2129	228	
 I213	228	
 I214	228	
 I219	228	
 I21A1	228	
 I21A9	228	
+I21B	228	
 I220	228	
 I221	228	
 I222	228	
 I228	228	
 I229	228	
 I230	229	
 I231	229	
@@ -2810,14 +2848,16 @@
 I235	229	
 I236	229	
 I237	229	
 I238	229	
 I240	229	
 I241	229	
 I248	229	
+I2481	229	
+I2489	229	
 I249	229	
 I25110	229	
 I25700	229	
 I25710	229	
 I25720	229	
 I25730	229	
 I25750	229	
@@ -2860,15 +2900,14 @@
 I429	227	
 I43	227	
 I442	238	
 I462	213	
 I468	213	
 I469	213	
 I470	238	
-I472	238	
 I4720	238	
 I4721	238	
 I4729	238	
 I479	238	
 I480	238	
 I4811	238	
 I4819	238	
@@ -3397,32 +3436,28 @@
 I7075	383	D
 I70761	263	
 I70762	263	
 I70763	263	
 I70768	263	
 I70769	263	
 I7100	264	
-I7101	264	
 I71010	264	
 I71011	264	
 I71012	264	
 I71019	264	
 I7102	264	
 I7103	264	
-I711	264	
 I7110	264	
 I7111	264	
 I7112	264	
 I7113	264	
-I713	264	
 I7130	264	
 I7131	264	
 I7132	264	
 I7133	264	
-I715	264	
 I7150	264	
 I7151	264	
 I7152	264	
 I718	264	
 I7301	263	
 I7401	264	
 I7409	264	
@@ -3666,33 +3701,40 @@
 J151	282	
 J1520	282	
 J15211	282	
 J15212	282	
 J1529	282	
 J155	282	
 J156	282	
+J1561	282	
+J1569	282	
 J158	282	
 J410	280	
 J411	280	
 J418	280	
 J42	280	
 J430	280	
 J431	280	
 J432	280	
 J438	280	
 J439	280	
 J440	280	
 J441	280	
+J4481	280	
+J4489	280	
 J449	280	
 J4550	279	
 J4551	279	
 J4552	279	
 J470	280	
 J471	280	
 J479	280	
+J4A0	276	
+J4A8	276	
+J4A9	276	
 J60	280	
 J61	280	
 J620	280	
 J628	280	
 J630	280	
 J631	280	
 J632	280	
@@ -5662,21 +5704,21 @@
 Q428	78	
 Q429	78	
 Q431	78	
 Q432	78	
 Q433	78	
 Q442	68	
 Q443	68	
+Q4471	68	
 Q8500	23	
 Q8501	23	
 Q8502	23	
 Q8503	23	
 Q8509	23	
 Q851	23	
-Q858	23	
 Q8581	23	
 Q8582	23	
 Q8583	23	
 Q8589	23	
 Q859	23	
 R092	212	
 R180	17	
@@ -5717,14 +5759,15 @@
 R402433	202	
 R402434	202	
 R402440	202	
 R402441	202	
 R402442	202	
 R402443	202	
 R402444	202	
+R402A	202	
 R403	202	
 R4588	155	
 R532	180	
 R5600	201	
 R5601	201	
 R561	201	
 R569	201	
@@ -7754,14 +7797,15 @@
 T562X2A	155	
 T563X2A	155	
 T564X2A	155	
 T565X2A	155	
 T566X2A	155	
 T567X2A	155	
 T56812A	155	
+T56822A	155	
 T56892A	155	
 T5692XA	155	
 T570X2A	155	
 T571X2A	155	
 T572X2A	155	
 T573X2A	155	
 T578X2A	155
```

### Comparing `mscore-1.0.0/mscore/reference_data/Model_Coefficients/2021_CMS-HCC_V22.csv` & `mscore-24.1.1/mscore/reference_data/Model_Coefficients/2021_CMS-HCC_V22.csv`

 * *Files identical despite different names*

### Comparing `mscore-1.0.0/mscore/reference_data/Model_Coefficients/2021_CMS-HCC_V222179O1.csv` & `mscore-24.1.1/mscore/reference_data/Model_Coefficients/2021_CMS-HCC_V222179O1.csv`

 * *Files identical despite different names*

### Comparing `mscore-1.0.0/mscore/reference_data/Model_Coefficients/2021_CMS-HCC_V24.csv` & `mscore-24.1.1/mscore/reference_data/Model_Coefficients/2021_CMS-HCC_V24.csv`

 * *Files identical despite different names*

### Comparing `mscore-1.0.0/mscore/reference_data/Model_Coefficients/2021_CMS-HCC_V242186P1.csv` & `mscore-24.1.1/mscore/reference_data/Model_Coefficients/2021_CMS-HCC_V242186P1.csv`

 * *Files identical despite different names*

### Comparing `mscore-1.0.0/mscore/reference_data/Model_Coefficients/2022_CMS-HCC_V22.csv` & `mscore-24.1.1/mscore/reference_data/Model_Coefficients/2022_CMS-HCC_V22.csv`

 * *Files identical despite different names*

### Comparing `mscore-1.0.0/mscore/reference_data/Model_Coefficients/2022_CMS-HCC_V222279O1.csv` & `mscore-24.1.1/mscore/reference_data/Model_Coefficients/2022_CMS-HCC_V222279O1.csv`

 * *Files identical despite different names*

### Comparing `mscore-1.0.0/mscore/reference_data/Model_Coefficients/2022_CMS-HCC_V24.csv` & `mscore-24.1.1/mscore/reference_data/Model_Coefficients/2022_CMS-HCC_V24.csv`

 * *Files identical despite different names*

### Comparing `mscore-1.0.0/mscore/reference_data/Model_Coefficients/2022_CMS-HCC_V242286P1.csv` & `mscore-24.1.1/mscore/reference_data/Model_Coefficients/2022_CMS-HCC_V242286P1.csv`

 * *Files identical despite different names*

### Comparing `mscore-1.0.0/mscore/reference_data/Model_Coefficients/2023_CMS-HCC_V22.csv` & `mscore-24.1.1/mscore/reference_data/Model_Coefficients/2023_CMS-HCC_V22.csv`

 * *Files identical despite different names*

### Comparing `mscore-1.0.0/mscore/reference_data/Model_Coefficients/2023_CMS-HCC_V24.csv` & `mscore-24.1.1/mscore/reference_data/Model_Coefficients/2023_CMS-HCC_V24.csv`

 * *Files identical despite different names*

### Comparing `mscore-1.0.0/mscore/reference_data/Model_Coefficients/2024_CMS-HCC_V22.csv` & `mscore-24.1.1/mscore/reference_data/Model_Coefficients/2024_CMS-HCC_V22.csv`

 * *Files identical despite different names*

### Comparing `mscore-1.0.0/mscore/reference_data/Model_Coefficients/2024_CMS-HCC_V24.csv` & `mscore-24.1.1/mscore/reference_data/Model_Coefficients/2024_CMS-HCC_V24.csv`

 * *Files identical despite different names*

### Comparing `mscore-1.0.0/mscore/reference_data/Model_Coefficients/2024_CMS-HCC_V28.csv` & `mscore-24.1.1/mscore/reference_data/Model_Coefficients/2024_CMS-HCC_V28.csv`

 * *Files identical despite different names*

### Comparing `mscore-1.0.0/mscore/reference_data/application_tables/application_model_dimension.parquet` & `mscore-24.1.1/mscore/reference_data/application_tables/application_model_dimension.parquet`

 * *Files 18% similar despite different names*

```diff
@@ -1,258 +1,225 @@
-00000000: 5041 5231 1504 1580 0815 9e04 4c15 8001  PAR1........L...
-00000010: 1500 1200 0080 0404 0100 0901 0002 0907  ................
-00000020: 0400 030d 0800 040d 0800 050d 0800 060d  ................
-00000030: 0800 070d 0800 080d 0800 090d 0800 0a0d  ................
-00000040: 0800 0b0d 0800 0c0d 0800 0d0d 0800 0e0d  ................
-00000050: 0800 0f0d 0800 100d 0800 110d 0800 120d  ................
-00000060: 0800 130d 0800 140d 0800 150d 0800 160d  ................
-00000070: 0800 170d 0800 180d 0800 190d 0800 1a0d  ................
-00000080: 0800 1b0d 0800 1c0d 0800 1d0d 0800 1e0d  ................
-00000090: 0800 1f0d 0800 200d 0800 210d 0800 220d  ...... ...!...".
-000000a0: 0800 230d 0800 240d 0800 250d 0800 260d  ..#...$...%...&.
-000000b0: 0800 270d 0800 280d 0800 290d 0800 2a0d  ..'...(...)...*.
-000000c0: 0800 2b0d 0800 2c0d 0800 2d0d 0800 2e0d  ..+...,...-.....
-000000d0: 0800 2f0d 0800 300d 0800 310d 0800 320d  ../...0...1...2.
-000000e0: 0800 330d 0800 340d 0800 350d 0800 360d  ..3...4...5...6.
-000000f0: 0800 370d 0800 380d 0800 390d 0804 3a00  ..7...8...9...:.
-00000100: 0901 003b 0907 0400 3c0d 0800 3d0d 0800  ...;....<...=...
-00000110: 3e0d 083c 3f00 0000 0000 0000 4000 0000  >..<?.......@...
-00000120: 0000 0000 1500 1572 1576 2c15 8001 1510  .......r.v,.....
-00000130: 1506 1506 1c18 0840 0000 0000 0000 0018  .......@........
-00000140: 0801 0000 0000 0000 0016 0028 0840 0000  ...........(.@..
-00000150: 0000 0000 0018 0801 0000 0000 0000 0000  ................
-00000160: 0000 39e0 0300 0000 8001 0106 1140 200c  ..9..........@ .
-00000170: 4461 1c48 a22c 4ce3 3c50 244d 5465 5d58  Da.H.,L.<P$MTe]X
-00000180: a66d 5ce7 7d60 288e 6469 9e68 aaae 6ceb  .m\.}`(.di.h..l.
-00000190: be70 2ccf 746d df78 aeef 7cef ff26 ba06  .p,.tm.x..|..&..
-000001a0: 1c15 0419 3500 0610 1918 084d 6f64 656c  ....5......Model
-000001b0: 5f49 4415 0216 8001 1690 0a16 b206 26c8  _ID...........&.
-000001c0: 0426 081c 1808 4000 0000 0000 0000 1808  .&....@.........
-000001d0: 0100 0000 0000 0000 1600 2808 4000 0000  ..........(.@...
-000001e0: 0000 0000 1808 0100 0000 0000 0000 0019  ................
-000001f0: 2c15 0415 0015 0200 1500 1510 1502 0000  ,...............
-00000200: 0015 0415 d001 1580 014c 151a 1500 1200  .........L......
-00000210: 0068 08dc 0700 0501 00dd 0d08 00de 0d08  .h..............
-00000220: 00df 0d08 00e0 0d08 00e1 0d08 00e2 0d08  ................
-00000230: 00e3 0d08 00e4 0d08 00e5 0d08 00e6 0d08  ................
-00000240: 3ce7 0700 0000 0000 00e8 0700 0000 0000  <...............
-00000250: 0015 0015 5215 562c 1580 0115 1015 0615  ....R.V,........
-00000260: 061c 1808 e807 0000 0000 0000 1808 dc07  ................
-00000270: 0000 0000 0000 1600 2808 e807 0000 0000  ........(.......
-00000280: 0000 1808 dc07 0000 0000 0000 0000 0029  ...............)
-00000290: a003 0000 0080 0101 0411 0000 1111 2222  ..............""
-000002a0: 3233 3344 4455 5566 6677 7787 8888 9999  233DDUUffww.....
-000002b0: a9aa aaba bbbb cbcc cccc 26f4 0a1c 1504  ..........&.....
-000002c0: 1935 0006 1019 180c 5061 796d 656e 745f  .5......Payment_
-000002d0: 5965 6172 1502 1680 0116 be03 16f2 0226  Year...........&
-000002e0: a209 2682 081c 1808 e807 0000 0000 0000  ..&.............
-000002f0: 1808 dc07 0000 0000 0000 1600 2808 e807  ............(...
-00000300: 0000 0000 0000 1808 dc07 0000 0000 0000  ................
-00000310: 0019 2c15 0415 0015 0200 1500 1510 1502  ..,.............
-00000320: 0000 0015 0415 3815 3c4c 1506 1500 1200  ......8.<L......
-00000330: 001c 6c07 0000 0043 4d53 2d48 4343 0400  ..l....CMS-HCC..
-00000340: 0000 4553 5244 0500 0000 5278 4843 4315  ..ESRD....RxHCC.
-00000350: 0015 3215 362c 1580 0115 1015 0615 061c  ..2.6,..........
-00000360: 3600 2805 5278 4843 4318 0743 4d53 2d48  6.(.RxHCC..CMS-H
-00000370: 4343 0000 0019 6003 0000 0080 0101 0211  CC....`.........
-00000380: 9090 4002 0909 0909 2494 5042 2994 02a5  ..@.....$.PB)...
-00000390: 26a0 0e1c 150c 1935 0006 1019 180a 4d6f  &......5......Mo
-000003a0: 6465 6c5f 5479 7065 1502 1680 0116 d201  del_Type........
-000003b0: 16da 0126 9e0d 26c6 0c1c 3600 2805 5278  ...&..&...6.(.Rx
-000003c0: 4843 4318 0743 4d53 2d48 4343 0019 2c15  HCC..CMS-HCC..,.
-000003d0: 0415 0015 0200 1500 1510 1502 0000 0015  ................
-000003e0: 0415 f00a 15f4 054c 156c 1500 1200 00b8  .......L.l......
-000003f0: 057c 0700 0000 4d41 2043 6f73 7404 0000  .|....MA Cost...
-00000400: 0050 4143 4509 0000 0056 3132 3133 3730  .PACE....V121370
-00000410: 4a31 050d 1832 3131 3338 3748 050d 0045  J1...211387H...E
-00000420: 2e0d 0018 5230 3331 3337 3811 2701 3408  ....R031378.'.4.
-00000430: 394c 3201 340d 1a00 4c05 3401 4100 3611  9L2.4...L.4.A.6.
-00000440: 4118 5632 3231 3637 3909 1a01 4e15 1a1c  A.V221679...N...
-00000450: 5230 3531 3637 364e 0541 0134 0037 2e34  R051676N.A.4.7.4
-00000460: 000c 3737 394f 054e 0134 151a 0134 0837  ..779O.N.4...4.7
-00000470: 3736 091a 0134 0038 2e34 0000 382e 3400  76...4.8.4..8.4.
-00000480: 151a 0134 0c38 3736 5005 4e01 3400 392e  ...4.876P.N.4.9.
-00000490: 3400 0039 1134 1856 3233 3139 3833 0927  4..9.4.V231983.'
-000004a0: 0175 0839 3837 090d 0141 0039 1941 0832  .u.987...A.9.A.2
-000004b0: 3230 1934 0c34 3230 380d 5b10 4532 3132  20.4.4208.[.E212
-000004c0: 3011 3411 0d05 dd10 5230 3532 302e 4100  0.4.....R0520.A.
-000004d0: 0031 2e41 0000 312e 4100 0031 2e41 0001  .1.A..1.A..1.A..
-000004e0: 0d15 4100 312e 4100 0032 2e41 0000 322e  ..A.1.A..2.A..2.
-000004f0: 4100 0032 2e41 0001 0d15 4100 3211 4101  A..2.A....A.2.A.
-00000500: 8f0c 3237 3653 2d11 0832 3233 2e4e 0000  ..276S-..223.N..
-00000510: 332e 4e00 0033 194e 0034 011a 0054 0534  3.N..3.N.4...T.4
-00000520: 0141 0033 194e 1038 3233 3834 091a 0056  .A.3.N.82384...V
-00000530: 0d4e 0575 0056 0934 0850 320a 4163 2032  .N.u.V.4.P2.Ac 2
-00000540: 3832 3331 3135 5433 4130 211f 015c 0528  823115T3A0!..\.(
-00000550: 0045 0928 0054 050d 115c 3432 0900 0000  .E.(.T...\42....
-00000560: 5230 3832 3338 3454 3215 0015 7415 782c  R082384T2...t.x,
-00000570: 1580 0115 1015 0615 061c 3604 280a 5632  ..........6.(.V2
-00000580: 3832 3331 3135 5433 1809 4532 3131 3338  823115T3..E21138
-00000590: 3748 3100 0000 3ae4 0400 0000 03f3 7001  7H1...:.......p.
-000005a0: 0611 4020 0c44 210c 0671 0883 411c 48a2  ..@ .D!..q..A.H.
-000005b0: 2c4c e33c 5024 4d54 655d 58a6 6d5c e77d  ,L.<P$MTe]X.m\.}
-000005c0: 6028 8e64 699e 68aa ae6c ebbe 702c cf74  `(.di.h..l..p,.t
-000005d0: 0d00 26a4 171c 150c 1935 0006 1019 1811  ..&......5......
-000005e0: 5341 535f 4d6f 6465 6c5f 5665 7273 696f  SAS_Model_Versio
-000005f0: 6e15 0216 8001 16de 0c16 e607 26d2 1526  n...........&..&
-00000600: be0f 1c36 0428 0a56 3238 3233 3131 3554  ...6.(.V2823115T
-00000610: 3318 0945 3231 3133 3837 4831 0019 2c15  3..E211387H1..,.
-00000620: 0415 0015 0200 1500 1510 1502 0000 0015  ................
-00000630: 0419 5c35 0018 0673 6368 656d 6115 0800  ..\5...schema...
-00000640: 1504 2502 1808 4d6f 6465 6c5f 4944 0015  ..%...Model_ID..
-00000650: 0425 0218 0c50 6179 6d65 6e74 5f59 6561  .%...Payment_Yea
-00000660: 7200 150c 2502 180a 4d6f 6465 6c5f 5479  r...%...Model_Ty
-00000670: 7065 2500 4c1c 0000 0015 0c25 0218 1153  pe%.L......%...S
-00000680: 4153 5f4d 6f64 656c 5f56 6572 7369 6f6e  AS_Model_Version
-00000690: 2500 4c1c 0000 0016 8001 191c 194c 26ba  %.L..........L&.
-000006a0: 061c 1504 1935 0006 1019 1808 4d6f 6465  .....5......Mode
-000006b0: 6c5f 4944 1502 1680 0116 900a 16b2 0626  l_ID...........&
-000006c0: c804 2608 1c18 0840 0000 0000 0000 0018  ..&....@........
-000006d0: 0801 0000 0000 0000 0016 0028 0840 0000  ...........(.@..
-000006e0: 0000 0000 0018 0801 0000 0000 0000 0000  ................
-000006f0: 192c 1504 1500 1502 0015 0015 1015 0200  .,..............
-00000700: 0000 26f4 0a1c 1504 1935 0006 1019 180c  ..&......5......
-00000710: 5061 796d 656e 745f 5965 6172 1502 1680  Payment_Year....
-00000720: 0116 be03 16f2 0226 a209 2682 081c 1808  .......&..&.....
-00000730: e807 0000 0000 0000 1808 dc07 0000 0000  ................
-00000740: 0000 1600 2808 e807 0000 0000 0000 1808  ....(...........
-00000750: dc07 0000 0000 0000 0019 2c15 0415 0015  ..........,.....
-00000760: 0200 1500 1510 1502 0000 0026 a00e 1c15  ...........&....
-00000770: 0c19 3500 0610 1918 0a4d 6f64 656c 5f54  ..5......Model_T
-00000780: 7970 6515 0216 8001 16d2 0116 da01 269e  ype...........&.
-00000790: 0d26 c60c 1c36 0028 0552 7848 4343 1807  .&...6.(.RxHCC..
-000007a0: 434d 532d 4843 4300 192c 1504 1500 1502  CMS-HCC..,......
-000007b0: 0015 0015 1015 0200 0000 26a4 171c 150c  ..........&.....
-000007c0: 1935 0006 1019 1811 5341 535f 4d6f 6465  .5......SAS_Mode
-000007d0: 6c5f 5665 7273 696f 6e15 0216 8001 16de  l_Version.......
-000007e0: 0c16 e607 26d2 1526 be0f 1c36 0428 0a56  ....&..&...6.(.V
-000007f0: 3238 3233 3131 3554 3318 0945 3231 3133  2823115T3..E2113
-00000800: 3837 4831 0019 2c15 0415 0015 0200 1500  87H1..,.........
-00000810: 1510 1502 0000 0016 fe1b 1680 0126 0816  .............&..
-00000820: e412 1400 0019 2c18 0670 616e 6461 7318  ......,..pandas.
-00000830: f304 7b22 696e 6465 785f 636f 6c75 6d6e  ..{"index_column
-00000840: 7322 3a20 5b5d 2c20 2263 6f6c 756d 6e5f  s": [], "column_
-00000850: 696e 6465 7865 7322 3a20 5b5d 2c20 2263  indexes": [], "c
-00000860: 6f6c 756d 6e73 223a 205b 7b22 6e61 6d65  olumns": [{"name
-00000870: 223a 2022 4d6f 6465 6c5f 4944 222c 2022  ": "Model_ID", "
-00000880: 6669 656c 645f 6e61 6d65 223a 2022 4d6f  field_name": "Mo
-00000890: 6465 6c5f 4944 222c 2022 7061 6e64 6173  del_ID", "pandas
-000008a0: 5f74 7970 6522 3a20 2269 6e74 3634 222c  _type": "int64",
-000008b0: 2022 6e75 6d70 795f 7479 7065 223a 2022   "numpy_type": "
-000008c0: 696e 7436 3422 2c20 226d 6574 6164 6174  int64", "metadat
-000008d0: 6122 3a20 6e75 6c6c 7d2c 207b 226e 616d  a": null}, {"nam
-000008e0: 6522 3a20 2250 6179 6d65 6e74 5f59 6561  e": "Payment_Yea
-000008f0: 7222 2c20 2266 6965 6c64 5f6e 616d 6522  r", "field_name"
-00000900: 3a20 2250 6179 6d65 6e74 5f59 6561 7222  : "Payment_Year"
-00000910: 2c20 2270 616e 6461 735f 7479 7065 223a  , "pandas_type":
-00000920: 2022 696e 7436 3422 2c20 226e 756d 7079   "int64", "numpy
-00000930: 5f74 7970 6522 3a20 2269 6e74 3634 222c  _type": "int64",
-00000940: 2022 6d65 7461 6461 7461 223a 206e 756c   "metadata": nul
-00000950: 6c7d 2c20 7b22 6e61 6d65 223a 2022 4d6f  l}, {"name": "Mo
-00000960: 6465 6c5f 5479 7065 222c 2022 6669 656c  del_Type", "fiel
-00000970: 645f 6e61 6d65 223a 2022 4d6f 6465 6c5f  d_name": "Model_
-00000980: 5479 7065 222c 2022 7061 6e64 6173 5f74  Type", "pandas_t
-00000990: 7970 6522 3a20 2275 6e69 636f 6465 222c  ype": "unicode",
-000009a0: 2022 6e75 6d70 795f 7479 7065 223a 2022   "numpy_type": "
-000009b0: 6f62 6a65 6374 222c 2022 6d65 7461 6461  object", "metada
-000009c0: 7461 223a 206e 756c 6c7d 2c20 7b22 6e61  ta": null}, {"na
-000009d0: 6d65 223a 2022 5341 535f 4d6f 6465 6c5f  me": "SAS_Model_
-000009e0: 5665 7273 696f 6e22 2c20 2266 6965 6c64  Version", "field
-000009f0: 5f6e 616d 6522 3a20 2253 4153 5f4d 6f64  _name": "SAS_Mod
-00000a00: 656c 5f56 6572 7369 6f6e 222c 2022 7061  el_Version", "pa
-00000a10: 6e64 6173 5f74 7970 6522 3a20 2275 6e69  ndas_type": "uni
-00000a20: 636f 6465 222c 2022 6e75 6d70 795f 7479  code", "numpy_ty
-00000a30: 7065 223a 2022 6f62 6a65 6374 222c 2022  pe": "object", "
-00000a40: 6d65 7461 6461 7461 223a 206e 756c 6c7d  metadata": null}
-00000a50: 5d2c 2022 6372 6561 746f 7222 3a20 7b22  ], "creator": {"
-00000a60: 6c69 6272 6172 7922 3a20 2270 7961 7272  library": "pyarr
-00000a70: 6f77 222c 2022 7665 7273 696f 6e22 3a20  ow", "version": 
-00000a80: 2231 332e 302e 3022 7d2c 2022 7061 6e64  "13.0.0"}, "pand
-00000a90: 6173 5f76 6572 7369 6f6e 223a 2022 322e  as_version": "2.
-00000aa0: 302e 3222 7d00 180c 4152 524f 573a 7363  0.2"}...ARROW:sc
-00000ab0: 6865 6d61 18a0 0a2f 2f2f 2f2f 3941 4441  hema.../////9ADA
-00000ac0: 4141 5141 4141 4141 4141 4b41 4134 4142  AAQAAAAAAAKAA4AB
-00000ad0: 6741 4641 4167 4143 6741 4141 4141 4242  gAFAAgACgAAAAABB
-00000ae0: 4141 5141 4141 4141 4141 4b41 4177 4141  AAQAAAAAAAKAAwAA
-00000af0: 4141 4541 4167 4143 6741 4141 4b67 4341  AAEAAgACgAAAKgCA
-00000b00: 4141 4541 4141 4141 5141 4141 4177 4141  AAEAAAAAQAAAAwAA
-00000b10: 4141 4941 4177 4142 4141 4941 4167 4141  AAIAAwABAAIAAgAA
-00000b20: 4141 4941 4141 4145 4141 4141 4159 4141  AAIAAAAEAAAAAYAA
-00000b30: 4142 7759 5735 6b59 584d 4141 484d 4341  ABwYW5kYXMAAHMCA
-00000b40: 4142 3749 6d6c 755a 4756 3458 324e 7662  AB7ImluZGV4X2Nvb
-00000b50: 4856 7462 6e4d 694f 6942 6258 5377 6749  HVtbnMiOiBbXSwgI
-00000b60: 6d4e 7662 4856 7462 6c39 7062 6d52 6c65  mNvbHVtbl9pbmRle
-00000b70: 4756 7a49 6a6f 6757 3130 7349 434a 6a62  GVzIjogW10sICJjb
-00000b80: 3278 3162 5735 7a49 6a6f 6757 3373 6962  2x1bW5zIjogW3sib
-00000b90: 6d46 745a 5349 3649 434a 4e62 3252 6c62  mFtZSI6ICJNb2Rlb
-00000ba0: 4639 4a52 4349 7349 434a 6d61 5756 735a  F9JRCIsICJmaWVsZ
-00000bb0: 4639 7559 5731 6c49 6a6f 6749 6b31 765a  F9uYW1lIjogIk1vZ
-00000bc0: 4756 7358 306c 4549 6977 6749 6e42 6862  GVsX0lEIiwgInBhb
-00000bd0: 6d52 6863 3139 3065 5842 6c49 6a6f 6749  mRhc190eXBlIjogI
-00000be0: 6d6c 7564 4459 3049 6977 6749 6d35 3162  mludDY0IiwgIm51b
-00000bf0: 5842 3558 3352 3563 4755 694f 6941 6961  XB5X3R5cGUiOiAia
-00000c00: 5735 304e 6a51 694c 4341 6962 5756 3059  W50NjQiLCAibWV0Y
-00000c10: 5752 6864 4745 694f 6942 7564 5778 7366  WRhdGEiOiBudWxsf
-00000c20: 5377 6765 794a 7559 5731 6c49 6a6f 6749  SwgeyJuYW1lIjogI
-00000c30: 6c42 6865 5731 6c62 6e52 6657 5756 6863  lBheW1lbnRfWWVhc
-00000c40: 6949 7349 434a 6d61 5756 735a 4639 7559  iIsICJmaWVsZF9uY
-00000c50: 5731 6c49 6a6f 6749 6c42 6865 5731 6c62  W1lIjogIlBheW1lb
-00000c60: 6e52 6657 5756 6863 6949 7349 434a 7759  nRfWWVhciIsICJwY
-00000c70: 5735 6b59 584e 6664 486c 775a 5349 3649  W5kYXNfdHlwZSI6I
-00000c80: 434a 7062 6e51 324e 4349 7349 434a 7564  CJpbnQ2NCIsICJud
-00000c90: 5731 7765 5639 3065 5842 6c49 6a6f 6749  W1weV90eXBlIjogI
-00000ca0: 6d6c 7564 4459 3049 6977 6749 6d31 6c64  mludDY0IiwgIm1ld
-00000cb0: 4746 6b59 5852 6849 6a6f 6762 6e56 7362  GFkYXRhIjogbnVsb
-00000cc0: 4830 7349 4873 6962 6d46 745a 5349 3649  H0sIHsibmFtZSI6I
-00000cd0: 434a 4e62 3252 6c62 4639 5565 5842 6c49  CJNb2RlbF9UeXBlI
-00000ce0: 6977 6749 6d5a 705a 5778 6b58 3235 6862  iwgImZpZWxkX25hb
-00000cf0: 5755 694f 6941 6954 5739 6b5a 5778 6656  WUiOiAiTW9kZWxfV
-00000d00: 486c 775a 5349 7349 434a 7759 5735 6b59  HlwZSIsICJwYW5kY
-00000d10: 584e 6664 486c 775a 5349 3649 434a 3162  XNfdHlwZSI6ICJ1b
-00000d20: 6d6c 6a62 3252 6c49 6977 6749 6d35 3162  mljb2RlIiwgIm51b
-00000d30: 5842 3558 3352 3563 4755 694f 6941 6962  XB5X3R5cGUiOiAib
-00000d40: 324a 715a 574e 3049 6977 6749 6d31 6c64  2JqZWN0IiwgIm1ld
-00000d50: 4746 6b59 5852 6849 6a6f 6762 6e56 7362  GFkYXRhIjogbnVsb
-00000d60: 4830 7349 4873 6962 6d46 745a 5349 3649  H0sIHsibmFtZSI6I
-00000d70: 434a 5451 564e 6654 5739 6b5a 5778 6656  CJTQVNfTW9kZWxfV
-00000d80: 6d56 7963 326c 7662 6949 7349 434a 6d61  mVyc2lvbiIsICJma
-00000d90: 5756 735a 4639 7559 5731 6c49 6a6f 6749  WVsZF9uYW1lIjogI
-00000da0: 6c4e 4255 3139 4e62 3252 6c62 4639 575a  lNBU19Nb2RlbF9WZ
-00000db0: 584a 7a61 5739 7549 6977 6749 6e42 6862  XJzaW9uIiwgInBhb
-00000dc0: 6d52 6863 3139 3065 5842 6c49 6a6f 6749  mRhc190eXBlIjogI
-00000dd0: 6e56 7561 574e 765a 4755 694c 4341 6962  nVuaWNvZGUiLCAib
-00000de0: 6e56 7463 486c 6664 486c 775a 5349 3649  nVtcHlfdHlwZSI6I
-00000df0: 434a 7659 6d70 6c59 3351 694c 4341 6962  CJvYmplY3QiLCAib
-00000e00: 5756 3059 5752 6864 4745 694f 6942 7564  WV0YWRhdGEiOiBud
-00000e10: 5778 7366 5630 7349 434a 6a63 6d56 6864  WxsfV0sICJjcmVhd
-00000e20: 4739 7949 6a6f 6765 794a 7361 574a 7959  G9yIjogeyJsaWJyY
-00000e30: 584a 3549 6a6f 6749 6e42 3559 584a 7962  XJ5IjogInB5YXJyb
-00000e40: 3363 694c 4341 6964 6d56 7963 326c 7662  3ciLCAidmVyc2lvb
-00000e50: 6949 3649 4349 784d 7934 774c 6a41 6966  iI6ICIxMy4wLjAif
-00000e60: 5377 6749 6e42 6862 6d52 6863 3139 325a  SwgInBhbmRhc192Z
-00000e70: 584a 7a61 5739 7549 6a6f 6749 6a49 754d  XJzaW9uIjogIjIuM
-00000e80: 4334 7949 6e30 4142 4141 4141 4c77 4141  C4yIn0ABAAAALwAA
-00000e90: 4142 7741 4141 4150 4141 4141 4151 4141  ABwAAAAPAAAAAQAA
-00000ea0: 4142 6b2f 2f2f 2f41 4141 4242 5241 4141  ABk////AAABBRAAA
-00000eb0: 4141 6b41 4141 4142 4141 4141 4141 4141  AAkAAAABAAAAAAAA
-00000ec0: 4141 5241 4141 4155 3046 5458 3031 765a  AARAAAAU0FTX01vZ
-00000ed0: 4756 7358 315a 6c63 6e4e 7062 3234 4141  GVsX1ZlcnNpb24AA
-00000ee0: 4144 552f 2f2f 2f6d 502f 2f2f 7741 4141  ADU////mP///wAAA
-00000ef0: 5155 5141 4141 4149 4141 4141 4151 4141  QUQAAAAIAAAAAQAA
-00000f00: 4141 4141 4141 4143 6741 4141 4531 765a  AAAAAAACgAAAE1vZ
-00000f10: 4756 7358 3152 3563 4755 4141 4151 4142  GVsX1R5cGUAAAQAB
-00000f20: 4141 4541 4141 4179 502f 2f2f 7741 4141  AAEAAAAyP///wAAA
-00000f30: 5149 5141 4141 4149 4141 4141 4151 4141  QIQAAAAIAAAAAQAA
-00000f40: 4141 4141 4141 4144 4141 4141 4642 6865  AAAAAAADAAAAFBhe
-00000f50: 5731 6c62 6e52 6657 5756 6863 6741 4141  W1lbnRfWWVhcgAAA
-00000f60: 4143 382f 2f2f 2f41 4141 4141 5541 4141  AC8////AAAAAUAAA
-00000f70: 4141 5141 4251 4143 4141 4741 4163 4144  AAQABQACAAGAAcAD
-00000f80: 4141 4141 4241 4145 4141 4141 4141 4141  AAAABAAEAAAAAAAA
-00000f90: 5149 5141 4141 414a 4141 4141 4151 4141  QIQAAAAJAAAAAQAA
-00000fa0: 4141 4141 4141 4143 4141 4141 4531 765a  AAAAAAACAAAAE1vZ
-00000fb0: 4756 7358 306c 4541 4141 4141 4167 4144  GVsX0lEAAAAAAgAD
-00000fc0: 4141 4941 4163 4143 4141 4141 4141 4141  AAIAAcACAAAAAAAA
-00000fd0: 4146 4141 4141 4100 1820 7061 7271 7565  AFAAAAA.. parque
-00000fe0: 742d 6370 702d 6172 726f 7720 7665 7273  t-cpp-arrow vers
-00000ff0: 696f 6e20 3133 2e30 2e30 194c 1c00 001c  ion 13.0.0.L....
-00001000: 0000 1c00 001c 0000 00da 0900 0050 4152  .............PAR
-00001010: 31                                       1
+00000000: 5041 5231 1504 1580 0315 da01 4c15 3015  PAR1........L.0.
+00000010: 0012 0000 c001 0401 0009 0100 0209 0704  ................
+00000020: 0003 0d08 0004 0d08 0005 0d08 0006 0d08  ................
+00000030: 0007 0d08 0008 0d08 0009 0d08 000a 0d08  ................
+00000040: 000b 0d08 000c 0d08 000d 0d08 000e 0d08  ................
+00000050: 000f 0d08 0010 0d08 0011 0d08 0012 0d08  ................
+00000060: 0013 0d08 0014 0d08 0015 0d08 0016 0d08  ................
+00000070: 3c17 0000 0000 0000 0018 0000 0000 0000  <...............
+00000080: 0015 0015 2e15 322c 1530 1510 1506 1506  ......2,.0......
+00000090: 1c18 0818 0000 0000 0000 0018 0801 0000  ................
+000000a0: 0000 0000 0016 0028 0818 0000 0000 0000  .......(........
+000000b0: 0018 0801 0000 0000 0000 0000 0000 1758  ...............X
+000000c0: 0200 0000 3001 0507 2088 418a 3928 a9c5  ....0... .A.9(..
+000000d0: 9a7b 30ca 49ab bd26 ae03 1c15 0419 3500  .{0.I..&......5.
+000000e0: 0610 1918 084d 6f64 656c 5f49 4415 0216  .....Model_ID...
+000000f0: 3016 c804 16a6 0326 8202 2608 1c18 0818  0......&..&.....
+00000100: 0000 0000 0000 0018 0801 0000 0000 0000  ................
+00000110: 0016 0028 0818 0000 0000 0000 0018 0801  ...(............
+00000120: 0000 0000 0000 0000 192c 1504 1500 1502  .........,......
+00000130: 0015 0015 1015 0200 0000 1504 1540 1538  .............@.8
+00000140: 4c15 0815 0012 0000 2008 e507 0005 0100  L....... .......
+00000150: e60d 083c e707 0000 0000 0000 e807 0000  ...<............
+00000160: 0000 0000 1500 151c 1520 2c15 3015 1015  ......... ,.0...
+00000170: 0615 061c 1808 e807 0000 0000 0000 1808  ................
+00000180: e507 0000 0000 0000 1600 2808 e807 0000  ..........(.....
+00000190: 0000 0000 1808 e507 0000 0000 0000 0000  ................
+000001a0: 000e 3402 0000 0030 0102 0700 5495 aafe  ..4....0....T...
+000001b0: ff26 e206 1c15 0419 3500 0610 1918 0c50  .&......5......P
+000001c0: 6179 6d65 6e74 5f59 6561 7215 0216 3016  ayment_Year...0.
+000001d0: f201 16ee 0126 c805 26f4 041c 1808 e807  .....&..&.......
+000001e0: 0000 0000 0000 1808 e507 0000 0000 0000  ................
+000001f0: 1600 2808 e807 0000 0000 0000 1808 e507  ..(.............
+00000200: 0000 0000 0000 0019 2c15 0415 0015 0200  ........,.......
+00000210: 1500 1510 1502 0000 0015 0415 3815 3c4c  ............8.<L
+00000220: 1506 1500 1200 001c 6c07 0000 0043 4d53  ........l....CMS
+00000230: 2d48 4343 0400 0000 4553 5244 0500 0000  -HCC....ESRD....
+00000240: 5278 4843 4315 0015 1c15 202c 1530 1510  RxHCC..... ,.0..
+00000250: 1506 1506 1c36 0028 0552 7848 4343 1807  .....6.(.RxHCC..
+00000260: 434d 532d 4843 4300 0000 0e34 0200 0000  CMS-HCC....4....
+00000270: 3001 0207 5042 2994 02a5 26f4 091c 150c  0...PB)...&.....
+00000280: 1935 0006 1019 180a 4d6f 6465 6c5f 5479  .5......Model_Ty
+00000290: 7065 1502 1630 16ba 0116 c201 268a 0926  pe...0......&..&
+000002a0: b208 1c36 0028 0552 7848 4343 1807 434d  ...6.(.RxHCC..CM
+000002b0: 532d 4843 4300 192c 1504 1500 1502 0015  S-HCC..,........
+000002c0: 0015 1015 0200 0000 1504 15f2 0415 d802  ................
+000002d0: 4c15 3015 0012 0000 b902 3009 0000 0056  L.0.......0....V
+000002e0: 3232 3231 3739 4f31 090d 1434 3231 3836  222179O1...42186
+000002f0: 5005 0d18 4532 3132 3138 3736 0d00 0032  P...E2121876...2
+00000300: 0127 1452 3035 3231 370d 2710 5632 3232  .'.R05217.'.V222
+00000310: 322e 4100 0032 2e41 0000 322e 4100 010d  2.A..2.A..2.A...
+00000320: 1541 0032 1141 014e 0c32 3736 5305 7501  .A.2.A.N.276S.u.
+00000330: 4e00 332e 4e00 0033 2e4e 0000 3319 4e00  N.3.N..3.N..3.N.
+00000340: 3401 1a00 5405 3401 4100 3319 4e10 3832  4...T.4.A.3.N.82
+00000350: 3338 3409 1a01 4e00 342e 4e00 0034 014e  384...N.4.N..4.N
+00000360: 000a 05f7 1438 3234 3131 3509 2801 eb00  .....824115.(...
+00000370: 342e 5c00 0434 381d 5c00 342e 5c00 1034  4.\..48.\.4.\..4
+00000380: 3834 5431 1500 152e 1532 2c15 3015 1015  84T1.....2,.0...
+00000390: 0615 061c 3600 280a 5632 3832 3431 3135  ....6.(.V2824115
+000003a0: 5431 1809 4532 3132 3138 3750 3100 0000  T1..E212187P1...
+000003b0: 1758 0200 0000 3001 0507 2088 418a 3928  .X....0... .A.9(
+000003c0: a9c5 9a7b 30ca 49ab bd26 920f 1c15 0c19  ...{0.I..&......
+000003d0: 3500 0610 1918 1153 4153 5f4d 6f64 656c  5......SAS_Model
+000003e0: 5f56 6572 7369 6f6e 1502 1630 1698 0616  _Version...0....
+000003f0: 8204 2688 0e26 900b 1c36 0028 0a56 3238  ..&..&...6.(.V28
+00000400: 3234 3131 3554 3118 0945 3231 3231 3837  24115T1..E212187
+00000410: 5031 0019 2c15 0415 0015 0200 1500 1510  P1..,...........
+00000420: 1502 0000 0015 0419 5c35 0018 0673 6368  ........\5...sch
+00000430: 656d 6115 0800 1504 2502 1808 4d6f 6465  ema.....%...Mode
+00000440: 6c5f 4944 0015 0425 0218 0c50 6179 6d65  l_ID...%...Payme
+00000450: 6e74 5f59 6561 7200 150c 2502 180a 4d6f  nt_Year...%...Mo
+00000460: 6465 6c5f 5479 7065 2500 4c1c 0000 0015  del_Type%.L.....
+00000470: 0c25 0218 1153 4153 5f4d 6f64 656c 5f56  .%...SAS_Model_V
+00000480: 6572 7369 6f6e 2500 4c1c 0000 0016 3019  ersion%.L.....0.
+00000490: 1c19 4c26 ae03 1c15 0419 3500 0610 1918  ..L&......5.....
+000004a0: 084d 6f64 656c 5f49 4415 0216 3016 c804  .Model_ID...0...
+000004b0: 16a6 0326 8202 2608 1c18 0818 0000 0000  ...&..&.........
+000004c0: 0000 0018 0801 0000 0000 0000 0016 0028  ...............(
+000004d0: 0818 0000 0000 0000 0018 0801 0000 0000  ................
+000004e0: 0000 0000 192c 1504 1500 1502 0015 0015  .....,..........
+000004f0: 1015 0200 0000 26e2 061c 1504 1935 0006  ......&......5..
+00000500: 1019 180c 5061 796d 656e 745f 5965 6172  ....Payment_Year
+00000510: 1502 1630 16f2 0116 ee01 26c8 0526 f404  ...0......&..&..
+00000520: 1c18 08e8 0700 0000 0000 0018 08e5 0700  ................
+00000530: 0000 0000 0016 0028 08e8 0700 0000 0000  .......(........
+00000540: 0018 08e5 0700 0000 0000 0000 192c 1504  .............,..
+00000550: 1500 1502 0015 0015 1015 0200 0000 26f4  ..............&.
+00000560: 091c 150c 1935 0006 1019 180a 4d6f 6465  .....5......Mode
+00000570: 6c5f 5479 7065 1502 1630 16ba 0116 c201  l_Type...0......
+00000580: 268a 0926 b208 1c36 0028 0552 7848 4343  &..&...6.(.RxHCC
+00000590: 1807 434d 532d 4843 4300 192c 1504 1500  ..CMS-HCC..,....
+000005a0: 1502 0015 0015 1015 0200 0000 2692 0f1c  ............&...
+000005b0: 150c 1935 0006 1019 1811 5341 535f 4d6f  ...5......SAS_Mo
+000005c0: 6465 6c5f 5665 7273 696f 6e15 0216 3016  del_Version...0.
+000005d0: 9806 1682 0426 880e 2690 0b1c 3600 280a  .....&..&...6.(.
+000005e0: 5632 3832 3431 3135 5431 1809 4532 3132  V2824115T1..E212
+000005f0: 3138 3750 3100 192c 1504 1500 1502 0015  187P1..,........
+00000600: 0015 1015 0200 0000 168c 0e16 3026 0816  ............0&..
+00000610: d80a 1400 0019 2c18 0670 616e 6461 7318  ......,..pandas.
+00000620: f304 7b22 696e 6465 785f 636f 6c75 6d6e  ..{"index_column
+00000630: 7322 3a20 5b5d 2c20 2263 6f6c 756d 6e5f  s": [], "column_
+00000640: 696e 6465 7865 7322 3a20 5b5d 2c20 2263  indexes": [], "c
+00000650: 6f6c 756d 6e73 223a 205b 7b22 6e61 6d65  olumns": [{"name
+00000660: 223a 2022 4d6f 6465 6c5f 4944 222c 2022  ": "Model_ID", "
+00000670: 6669 656c 645f 6e61 6d65 223a 2022 4d6f  field_name": "Mo
+00000680: 6465 6c5f 4944 222c 2022 7061 6e64 6173  del_ID", "pandas
+00000690: 5f74 7970 6522 3a20 2269 6e74 3634 222c  _type": "int64",
+000006a0: 2022 6e75 6d70 795f 7479 7065 223a 2022   "numpy_type": "
+000006b0: 696e 7436 3422 2c20 226d 6574 6164 6174  int64", "metadat
+000006c0: 6122 3a20 6e75 6c6c 7d2c 207b 226e 616d  a": null}, {"nam
+000006d0: 6522 3a20 2250 6179 6d65 6e74 5f59 6561  e": "Payment_Yea
+000006e0: 7222 2c20 2266 6965 6c64 5f6e 616d 6522  r", "field_name"
+000006f0: 3a20 2250 6179 6d65 6e74 5f59 6561 7222  : "Payment_Year"
+00000700: 2c20 2270 616e 6461 735f 7479 7065 223a  , "pandas_type":
+00000710: 2022 696e 7436 3422 2c20 226e 756d 7079   "int64", "numpy
+00000720: 5f74 7970 6522 3a20 2269 6e74 3634 222c  _type": "int64",
+00000730: 2022 6d65 7461 6461 7461 223a 206e 756c   "metadata": nul
+00000740: 6c7d 2c20 7b22 6e61 6d65 223a 2022 4d6f  l}, {"name": "Mo
+00000750: 6465 6c5f 5479 7065 222c 2022 6669 656c  del_Type", "fiel
+00000760: 645f 6e61 6d65 223a 2022 4d6f 6465 6c5f  d_name": "Model_
+00000770: 5479 7065 222c 2022 7061 6e64 6173 5f74  Type", "pandas_t
+00000780: 7970 6522 3a20 2275 6e69 636f 6465 222c  ype": "unicode",
+00000790: 2022 6e75 6d70 795f 7479 7065 223a 2022   "numpy_type": "
+000007a0: 6f62 6a65 6374 222c 2022 6d65 7461 6461  object", "metada
+000007b0: 7461 223a 206e 756c 6c7d 2c20 7b22 6e61  ta": null}, {"na
+000007c0: 6d65 223a 2022 5341 535f 4d6f 6465 6c5f  me": "SAS_Model_
+000007d0: 5665 7273 696f 6e22 2c20 2266 6965 6c64  Version", "field
+000007e0: 5f6e 616d 6522 3a20 2253 4153 5f4d 6f64  _name": "SAS_Mod
+000007f0: 656c 5f56 6572 7369 6f6e 222c 2022 7061  el_Version", "pa
+00000800: 6e64 6173 5f74 7970 6522 3a20 2275 6e69  ndas_type": "uni
+00000810: 636f 6465 222c 2022 6e75 6d70 795f 7479  code", "numpy_ty
+00000820: 7065 223a 2022 6f62 6a65 6374 222c 2022  pe": "object", "
+00000830: 6d65 7461 6461 7461 223a 206e 756c 6c7d  metadata": null}
+00000840: 5d2c 2022 6372 6561 746f 7222 3a20 7b22  ], "creator": {"
+00000850: 6c69 6272 6172 7922 3a20 2270 7961 7272  library": "pyarr
+00000860: 6f77 222c 2022 7665 7273 696f 6e22 3a20  ow", "version": 
+00000870: 2231 352e 302e 3022 7d2c 2022 7061 6e64  "15.0.0"}, "pand
+00000880: 6173 5f76 6572 7369 6f6e 223a 2022 322e  as_version": "2.
+00000890: 322e 3022 7d00 180c 4152 524f 573a 7363  2.0"}...ARROW:sc
+000008a0: 6865 6d61 18a0 0a2f 2f2f 2f2f 3941 4441  hema.../////9ADA
+000008b0: 4141 5141 4141 4141 4141 4b41 4134 4142  AAQAAAAAAAKAA4AB
+000008c0: 6741 4641 4167 4143 6741 4141 4141 4242  gAFAAgACgAAAAABB
+000008d0: 4141 5141 4141 4141 4141 4b41 4177 4141  AAQAAAAAAAKAAwAA
+000008e0: 4141 4541 4167 4143 6741 4141 4b67 4341  AAEAAgACgAAAKgCA
+000008f0: 4141 4541 4141 4141 5141 4141 4177 4141  AAEAAAAAQAAAAwAA
+00000900: 4141 4941 4177 4142 4141 4941 4167 4141  AAIAAwABAAIAAgAA
+00000910: 4141 4941 4141 4145 4141 4141 4159 4141  AAIAAAAEAAAAAYAA
+00000920: 4142 7759 5735 6b59 584d 4141 484d 4341  ABwYW5kYXMAAHMCA
+00000930: 4142 3749 6d6c 755a 4756 3458 324e 7662  AB7ImluZGV4X2Nvb
+00000940: 4856 7462 6e4d 694f 6942 6258 5377 6749  HVtbnMiOiBbXSwgI
+00000950: 6d4e 7662 4856 7462 6c39 7062 6d52 6c65  mNvbHVtbl9pbmRle
+00000960: 4756 7a49 6a6f 6757 3130 7349 434a 6a62  GVzIjogW10sICJjb
+00000970: 3278 3162 5735 7a49 6a6f 6757 3373 6962  2x1bW5zIjogW3sib
+00000980: 6d46 745a 5349 3649 434a 4e62 3252 6c62  mFtZSI6ICJNb2Rlb
+00000990: 4639 4a52 4349 7349 434a 6d61 5756 735a  F9JRCIsICJmaWVsZ
+000009a0: 4639 7559 5731 6c49 6a6f 6749 6b31 765a  F9uYW1lIjogIk1vZ
+000009b0: 4756 7358 306c 4549 6977 6749 6e42 6862  GVsX0lEIiwgInBhb
+000009c0: 6d52 6863 3139 3065 5842 6c49 6a6f 6749  mRhc190eXBlIjogI
+000009d0: 6d6c 7564 4459 3049 6977 6749 6d35 3162  mludDY0IiwgIm51b
+000009e0: 5842 3558 3352 3563 4755 694f 6941 6961  XB5X3R5cGUiOiAia
+000009f0: 5735 304e 6a51 694c 4341 6962 5756 3059  W50NjQiLCAibWV0Y
+00000a00: 5752 6864 4745 694f 6942 7564 5778 7366  WRhdGEiOiBudWxsf
+00000a10: 5377 6765 794a 7559 5731 6c49 6a6f 6749  SwgeyJuYW1lIjogI
+00000a20: 6c42 6865 5731 6c62 6e52 6657 5756 6863  lBheW1lbnRfWWVhc
+00000a30: 6949 7349 434a 6d61 5756 735a 4639 7559  iIsICJmaWVsZF9uY
+00000a40: 5731 6c49 6a6f 6749 6c42 6865 5731 6c62  W1lIjogIlBheW1lb
+00000a50: 6e52 6657 5756 6863 6949 7349 434a 7759  nRfWWVhciIsICJwY
+00000a60: 5735 6b59 584e 6664 486c 775a 5349 3649  W5kYXNfdHlwZSI6I
+00000a70: 434a 7062 6e51 324e 4349 7349 434a 7564  CJpbnQ2NCIsICJud
+00000a80: 5731 7765 5639 3065 5842 6c49 6a6f 6749  W1weV90eXBlIjogI
+00000a90: 6d6c 7564 4459 3049 6977 6749 6d31 6c64  mludDY0IiwgIm1ld
+00000aa0: 4746 6b59 5852 6849 6a6f 6762 6e56 7362  GFkYXRhIjogbnVsb
+00000ab0: 4830 7349 4873 6962 6d46 745a 5349 3649  H0sIHsibmFtZSI6I
+00000ac0: 434a 4e62 3252 6c62 4639 5565 5842 6c49  CJNb2RlbF9UeXBlI
+00000ad0: 6977 6749 6d5a 705a 5778 6b58 3235 6862  iwgImZpZWxkX25hb
+00000ae0: 5755 694f 6941 6954 5739 6b5a 5778 6656  WUiOiAiTW9kZWxfV
+00000af0: 486c 775a 5349 7349 434a 7759 5735 6b59  HlwZSIsICJwYW5kY
+00000b00: 584e 6664 486c 775a 5349 3649 434a 3162  XNfdHlwZSI6ICJ1b
+00000b10: 6d6c 6a62 3252 6c49 6977 6749 6d35 3162  mljb2RlIiwgIm51b
+00000b20: 5842 3558 3352 3563 4755 694f 6941 6962  XB5X3R5cGUiOiAib
+00000b30: 324a 715a 574e 3049 6977 6749 6d31 6c64  2JqZWN0IiwgIm1ld
+00000b40: 4746 6b59 5852 6849 6a6f 6762 6e56 7362  GFkYXRhIjogbnVsb
+00000b50: 4830 7349 4873 6962 6d46 745a 5349 3649  H0sIHsibmFtZSI6I
+00000b60: 434a 5451 564e 6654 5739 6b5a 5778 6656  CJTQVNfTW9kZWxfV
+00000b70: 6d56 7963 326c 7662 6949 7349 434a 6d61  mVyc2lvbiIsICJma
+00000b80: 5756 735a 4639 7559 5731 6c49 6a6f 6749  WVsZF9uYW1lIjogI
+00000b90: 6c4e 4255 3139 4e62 3252 6c62 4639 575a  lNBU19Nb2RlbF9WZ
+00000ba0: 584a 7a61 5739 7549 6977 6749 6e42 6862  XJzaW9uIiwgInBhb
+00000bb0: 6d52 6863 3139 3065 5842 6c49 6a6f 6749  mRhc190eXBlIjogI
+00000bc0: 6e56 7561 574e 765a 4755 694c 4341 6962  nVuaWNvZGUiLCAib
+00000bd0: 6e56 7463 486c 6664 486c 775a 5349 3649  nVtcHlfdHlwZSI6I
+00000be0: 434a 7659 6d70 6c59 3351 694c 4341 6962  CJvYmplY3QiLCAib
+00000bf0: 5756 3059 5752 6864 4745 694f 6942 7564  WV0YWRhdGEiOiBud
+00000c00: 5778 7366 5630 7349 434a 6a63 6d56 6864  WxsfV0sICJjcmVhd
+00000c10: 4739 7949 6a6f 6765 794a 7361 574a 7959  G9yIjogeyJsaWJyY
+00000c20: 584a 3549 6a6f 6749 6e42 3559 584a 7962  XJ5IjogInB5YXJyb
+00000c30: 3363 694c 4341 6964 6d56 7963 326c 7662  3ciLCAidmVyc2lvb
+00000c40: 6949 3649 4349 784e 5334 774c 6a41 6966  iI6ICIxNS4wLjAif
+00000c50: 5377 6749 6e42 6862 6d52 6863 3139 325a  SwgInBhbmRhc192Z
+00000c60: 584a 7a61 5739 7549 6a6f 6749 6a49 754d  XJzaW9uIjogIjIuM
+00000c70: 6934 7749 6e30 4142 4141 4141 4c77 4141  i4wIn0ABAAAALwAA
+00000c80: 4142 7741 4141 4150 4141 4141 4151 4141  ABwAAAAPAAAAAQAA
+00000c90: 4142 6b2f 2f2f 2f41 4141 4242 5241 4141  ABk////AAABBRAAA
+00000ca0: 4141 6b41 4141 4142 4141 4141 4141 4141  AAkAAAABAAAAAAAA
+00000cb0: 4141 5241 4141 4155 3046 5458 3031 765a  AARAAAAU0FTX01vZ
+00000cc0: 4756 7358 315a 6c63 6e4e 7062 3234 4141  GVsX1ZlcnNpb24AA
+00000cd0: 4144 552f 2f2f 2f6d 502f 2f2f 7741 4141  ADU////mP///wAAA
+00000ce0: 5155 5141 4141 4149 4141 4141 4151 4141  QUQAAAAIAAAAAQAA
+00000cf0: 4141 4141 4141 4143 6741 4141 4531 765a  AAAAAAACgAAAE1vZ
+00000d00: 4756 7358 3152 3563 4755 4141 4151 4142  GVsX1R5cGUAAAQAB
+00000d10: 4141 4541 4141 4179 502f 2f2f 7741 4141  AAEAAAAyP///wAAA
+00000d20: 5149 5141 4141 4149 4141 4141 4151 4141  QIQAAAAIAAAAAQAA
+00000d30: 4141 4141 4141 4144 4141 4141 4642 6865  AAAAAAADAAAAFBhe
+00000d40: 5731 6c62 6e52 6657 5756 6863 6741 4141  W1lbnRfWWVhcgAAA
+00000d50: 4143 382f 2f2f 2f41 4141 4141 5541 4141  AC8////AAAAAUAAA
+00000d60: 4141 5141 4251 4143 4141 4741 4163 4144  AAQABQACAAGAAcAD
+00000d70: 4141 4141 4241 4145 4141 4141 4141 4141  AAAABAAEAAAAAAAA
+00000d80: 5149 5141 4141 414a 4141 4141 4151 4141  QIQAAAAJAAAAAQAA
+00000d90: 4141 4141 4141 4143 4141 4141 4531 765a  AAAAAAACAAAAE1vZ
+00000da0: 4756 7358 306c 4541 4141 4141 4167 4144  GVsX0lEAAAAAAgAD
+00000db0: 4141 4941 4163 4143 4141 4141 4141 4141  AAIAAcACAAAAAAAA
+00000dc0: 4146 4141 4141 4100 1820 7061 7271 7565  AFAAAAA.. parque
+00000dd0: 742d 6370 702d 6172 726f 7720 7665 7273  t-cpp-arrow vers
+00000de0: 696f 6e20 3135 2e30 2e30 194c 1c00 001c  ion 15.0.0.L....
+00000df0: 0000 1c00 001c 0000 00d4 0900 0050 4152  .............PAR
+00000e00: 31                                       1
```

### Comparing `mscore-1.0.0/mscore/reference_data/model_formats_all_columns/2023_CMS-HCC_V222379O1_format.csv` & `mscore-24.1.1/mscore/reference_data/model_formats_all_columns/2023_CMS-HCC_V222379O1_format.csv`

 * *Files identical despite different names*

### Comparing `mscore-1.0.0/mscore/reference_data/model_formats_all_columns/2023_CMS-HCC_V242386P1_format.csv` & `mscore-24.1.1/mscore/reference_data/model_formats_all_columns/2023_CMS-HCC_V242386P1_format.csv`

 * *Files identical despite different names*

### Comparing `mscore-1.0.0/mscore/reference_data/model_formats_all_columns/2024_CMS-HCC_V28_format.csv` & `mscore-24.1.1/mscore/reference_data/model_formats_all_columns/2024_CMS-HCC_V28_format.csv`

 * *Files identical despite different names*

### Comparing `mscore-1.0.0/mscore/scoring_handler.pye` & `mscore-24.1.1/mscore/scoring_handler.pye`

 * *Files identical despite different names*

### Comparing `mscore-1.0.0/mscore/utilities/__init__.pye` & `mscore-24.1.1/mscore/utilities/__init__.pye`

 * *Files identical despite different names*

### Comparing `mscore-1.0.0/mscore/utilities/authentication.pye` & `mscore-24.1.1/mscore/utilities/authentication.pye`

 * *Files identical despite different names*

### Comparing `mscore-1.0.0/mscore/utilities/context.pye` & `mscore-24.1.1/mscore/utilities/context.pye`

 * *Files identical despite different names*

### Comparing `mscore-1.0.0/mscore/utilities/data_models.pye` & `mscore-24.1.1/mscore/utilities/data_models.pye`

 * *Files identical despite different names*

### Comparing `mscore-1.0.0/mscore/utilities/data_validation.pye` & `mscore-24.1.1/mscore/utilities/data_validation.pye`

 * *Files identical despite different names*

### Comparing `mscore-1.0.0/mscore/utilities/file_organizer.pye` & `mscore-24.1.1/mscore/utilities/file_organizer.pye`

 * *Files identical despite different names*

### Comparing `mscore-1.0.0/mscore/utilities/licensing.pye` & `mscore-24.1.1/mscore/utilities/licensing.pye`

 * *Files identical despite different names*

### Comparing `mscore-1.0.0/mscore/utilities/log_handler.pye` & `mscore-24.1.1/mscore/utilities/log_handler.pye`

 * *Files identical despite different names*

### Comparing `mscore-1.0.0/mscore/utilities/user_models.pye` & `mscore-24.1.1/mscore/utilities/user_models.pye`

 * *Files identical despite different names*

### Comparing `mscore-1.0.0/mscore.egg-info/PKG-INFO` & `mscore-24.1.1/mscore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mscore
-Version: 1.0.0
+Version: 24.1.1
 Summary: MScore: Risk Scores Made Easy
 Home-page: https://github.com/elevendatacorp/mscore.git
 Author: RAM Development Team
 Author-email: RAM Development Team <dev@riskadjustmentmodel.com>
 Project-URL: Homepage, https://riskadjustmentmodel.com/mscore-product
 Project-URL: Bug Tracker, https://github.com/elevendatacorp/mscore/issues
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mscore Version: 1.0.0 Summary: MScore: Risk Scores
+Metadata-Version: 2.1 Name: mscore Version: 24.1.1 Summary: MScore: Risk Scores
 Made Easy Home-page: https://github.com/elevendatacorp/mscore.git Author: RAM
 Development Team Author-email: RAM Development Team
 riskadjustmentmodel.com> Project-URL: Homepage, https://
 riskadjustmentmodel.com/mscore-product Project-URL: Bug Tracker, https://
 github.com/elevendatacorp/mscore/issues Classifier: Programming Language ::
 Python :: 3 Classifier: Operating System :: OS Independent Requires-Python:
 >=3.10 Description-Content-Type: text/markdown Requires-Dist: pandas Requires-
```

### Comparing `mscore-1.0.0/mscore.egg-info/SOURCES.txt` & `mscore-24.1.1/mscore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mscore-1.0.0/pyproject.toml` & `mscore-24.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mscore"
-version = "1.0.0"
+version = "24.1.1"
 dependencies = [
   "pandas",
   "pyarrow",
   "numpy",
   "requests",
   "getmac",
   "cython",
```

