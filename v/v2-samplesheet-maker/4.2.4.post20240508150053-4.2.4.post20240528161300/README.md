# Comparing `tmp/v2_samplesheet_maker-4.2.4.post20240508150053.tar.gz` & `tmp/v2_samplesheet_maker-4.2.4.post20240528161300.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "v2_samplesheet_maker-4.2.4.post20240508150053.tar", last modified: Wed May  8 05:02:27 2024, max compression
+gzip compressed data, was "v2_samplesheet_maker-4.2.4.post20240528161300.tar", last modified: Tue May 28 06:14:40 2024, max compression
```

## Comparing `v2_samplesheet_maker-4.2.4.post20240508150053.tar` & `v2_samplesheet_maker-4.2.4.post20240528161300.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 05:02:27.127716 v2_samplesheet_maker-4.2.4.post20240508150053/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-08 05:02:04.000000 v2_samplesheet_maker-4.2.4.post20240508150053/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    22433 2024-05-08 05:02:27.123716 v2_samplesheet_maker-4.2.4.post20240508150053/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21412 2024-05-08 05:02:04.000000 v2_samplesheet_maker-4.2.4.post20240508150053/Readme.md
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-08 05:02:04.000000 v2_samplesheet_maker-4.2.4.post20240508150053/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 05:02:27.115716 v2_samplesheet_maker-4.2.4.post20240508150053/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)     8257 2024-05-08 05:02:04.000000 v2_samplesheet_maker-4.2.4.post20240508150053/scripts/build-samplesheet-and-validate-with-bcl-convert.sh
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 05:02:27.127716 v2_samplesheet_maker-4.2.4.post20240508150053/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 05:02:27.115716 v2_samplesheet_maker-4.2.4.post20240508150053/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 05:02:27.115716 v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 05:02:04.000000 v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 05:02:27.119716 v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/classes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 05:02:04.000000 v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16492 2024-05-08 05:02:04.000000 v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/classes/samplesheet.py
--rw-r--r--   0 runner    (1001) docker     (127)    10267 2024-05-08 05:02:04.000000 v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/classes/super_sections.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-08 05:02:04.000000 v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 05:02:27.119716 v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/functions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 05:02:04.000000 v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-08 05:02:04.000000 v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/functions/run_info_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6069 2024-05-08 05:02:04.000000 v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/functions/run_info_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-08 05:02:04.000000 v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/functions/v2_samplesheet_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-05-08 05:02:04.000000 v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/functions/v2_samplesheet_to_run_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-08 05:02:04.000000 v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/functions/v2_samplesheet_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-08 05:02:04.000000 v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 05:02:27.119716 v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 05:02:04.000000 v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7483 2024-05-08 05:02:04.000000 v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/models/bcl_convert_sections.py
--rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-05-08 05:02:04.000000 v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/models/cloud_section.py
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-08 05:02:04.000000 v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/models/run_info_sections.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-08 05:02:04.000000 v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/models/samplesheet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4888 2024-05-08 05:02:04.000000 v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/models/tso500l_sections.py
--rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-05-08 05:02:04.000000 v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/models/tso500s_sections.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 05:02:27.123716 v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/run/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 05:02:04.000000 v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-08 05:02:04.000000 v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/run/run_info_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-08 05:02:04.000000 v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/run/run_info_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-08 05:02:04.000000 v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/run/v2_samplesheet_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-08 05:02:04.000000 v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/run/v2_samplesheet_to_run_info_xml.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-08 05:02:04.000000 v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/run/v2_samplesheet_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 05:02:27.123716 v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/section_classes/
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-08 05:02:04.000000 v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/section_classes/bcl_convert_sections.py
--rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-05-08 05:02:04.000000 v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/section_classes/cloud_sections.py
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-08 05:02:04.000000 v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/section_classes/run_info_sections.py
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-08 05:02:04.000000 v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/section_classes/tso500l_sections.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-08 05:02:04.000000 v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/section_classes/tso500s_sections.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 05:02:27.123716 v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-05-08 05:02:04.000000 v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8848 2024-05-08 05:02:04.000000 v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6353 2024-05-08 05:02:04.000000 v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/utils/docopt_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-08 05:02:04.000000 v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-08 05:02:04.000000 v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/utils/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 05:02:27.123716 v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22433 2024-05-08 05:02:27.000000 v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-05-08 05:02:27.000000 v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 05:02:27.000000 v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-08 05:02:27.000000 v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-08 05:02:27.000000 v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-08 05:02:27.000000 v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:14:40.029294 v2_samplesheet_maker-4.2.4.post20240528161300/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-28 06:14:15.000000 v2_samplesheet_maker-4.2.4.post20240528161300/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    22433 2024-05-28 06:14:40.025294 v2_samplesheet_maker-4.2.4.post20240528161300/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21412 2024-05-28 06:14:15.000000 v2_samplesheet_maker-4.2.4.post20240528161300/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-28 06:14:15.000000 v2_samplesheet_maker-4.2.4.post20240528161300/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:14:40.017294 v2_samplesheet_maker-4.2.4.post20240528161300/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8257 2024-05-28 06:14:15.000000 v2_samplesheet_maker-4.2.4.post20240528161300/scripts/build-samplesheet-and-validate-with-bcl-convert.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 06:14:40.029294 v2_samplesheet_maker-4.2.4.post20240528161300/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:14:40.017294 v2_samplesheet_maker-4.2.4.post20240528161300/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:14:40.017294 v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 06:14:15.000000 v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:14:40.021294 v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 06:14:15.000000 v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16492 2024-05-28 06:14:15.000000 v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/classes/samplesheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10267 2024-05-28 06:14:15.000000 v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/classes/super_sections.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-28 06:14:15.000000 v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:14:40.021294 v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 06:14:15.000000 v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-28 06:14:15.000000 v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/functions/run_info_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6069 2024-05-28 06:14:15.000000 v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/functions/run_info_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-28 06:14:15.000000 v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/functions/v2_samplesheet_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-05-28 06:14:15.000000 v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/functions/v2_samplesheet_to_run_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-28 06:14:15.000000 v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/functions/v2_samplesheet_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-28 06:14:15.000000 v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:14:40.021294 v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 06:14:15.000000 v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7483 2024-05-28 06:14:15.000000 v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/models/bcl_convert_sections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-05-28 06:14:15.000000 v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/models/cloud_section.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-28 06:14:15.000000 v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/models/run_info_sections.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-28 06:14:15.000000 v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/models/samplesheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4888 2024-05-28 06:14:15.000000 v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/models/tso500l_sections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-05-28 06:14:15.000000 v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/models/tso500s_sections.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:14:40.025294 v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/run/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 06:14:15.000000 v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-28 06:14:15.000000 v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/run/run_info_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-28 06:14:15.000000 v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/run/run_info_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-28 06:14:15.000000 v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/run/v2_samplesheet_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-28 06:14:15.000000 v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/run/v2_samplesheet_to_run_info_xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-28 06:14:15.000000 v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/run/v2_samplesheet_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:14:40.025294 v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/section_classes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-28 06:14:15.000000 v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/section_classes/bcl_convert_sections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-05-28 06:14:15.000000 v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/section_classes/cloud_sections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-28 06:14:15.000000 v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/section_classes/run_info_sections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-28 06:14:15.000000 v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/section_classes/tso500l_sections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-28 06:14:15.000000 v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/section_classes/tso500s_sections.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:14:40.025294 v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-05-28 06:14:15.000000 v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8848 2024-05-28 06:14:15.000000 v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6353 2024-05-28 06:14:15.000000 v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/utils/docopt_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-28 06:14:15.000000 v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-28 06:14:15.000000 v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/utils/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:14:40.025294 v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22433 2024-05-28 06:14:40.000000 v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-05-28 06:14:40.000000 v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 06:14:40.000000 v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-28 06:14:40.000000 v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-28 06:14:40.000000 v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-28 06:14:40.000000 v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker.egg-info/top_level.txt
```

### Comparing `v2_samplesheet_maker-4.2.4.post20240508150053/LICENSE` & `v2_samplesheet_maker-4.2.4.post20240528161300/LICENSE`

 * *Files identical despite different names*

### Comparing `v2_samplesheet_maker-4.2.4.post20240508150053/PKG-INFO` & `v2_samplesheet_maker-4.2.4.post20240528161300/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: v2_samplesheet_maker
-Version: 4.2.4.post20240508150053
+Version: 4.2.4.post20240528161300
 Summary: v2 SampleSheet maker
 Author-email: Alexis Lucattini <alexis.lucattini@umccr.org>
 Project-URL: Homepage, https://github.com/umccr/v2-samplesheet-maker
 Project-URL: Bug Tracker, https://github.com/umccr/v2-samplesheet-maker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `v2_samplesheet_maker-4.2.4.post20240508150053/Readme.md` & `v2_samplesheet_maker-4.2.4.post20240528161300/Readme.md`

 * *Files identical despite different names*

### Comparing `v2_samplesheet_maker-4.2.4.post20240508150053/pyproject.toml` & `v2_samplesheet_maker-4.2.4.post20240528161300/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "setuptools>=61.0",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "v2_samplesheet_maker"
-version = "4.2.4.post20240508150053"
+version = "4.2.4.post20240528161300"
 description = "v2 SampleSheet maker"
 readme = "Readme.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `v2_samplesheet_maker-4.2.4.post20240508150053/scripts/build-samplesheet-and-validate-with-bcl-convert.sh` & `v2_samplesheet_maker-4.2.4.post20240528161300/scripts/build-samplesheet-and-validate-with-bcl-convert.sh`

 * *Files identical despite different names*

### Comparing `v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/classes/samplesheet.py` & `v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/classes/samplesheet.py`

 * *Files identical despite different names*

### Comparing `v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/classes/super_sections.py` & `v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/classes/super_sections.py`

 * *Files identical despite different names*

### Comparing `v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/functions/run_info_reader.py` & `v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/functions/run_info_reader.py`

 * *Files identical despite different names*

### Comparing `v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/functions/run_info_writer.py` & `v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/functions/run_info_writer.py`

 * *Files identical despite different names*

### Comparing `v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/functions/v2_samplesheet_reader.py` & `v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/functions/v2_samplesheet_reader.py`

 * *Files identical despite different names*

### Comparing `v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/functions/v2_samplesheet_to_run_info.py` & `v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/functions/v2_samplesheet_to_run_info.py`

 * *Files identical despite different names*

### Comparing `v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/functions/v2_samplesheet_writer.py` & `v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/functions/v2_samplesheet_writer.py`

 * *Files identical despite different names*

### Comparing `v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/models/bcl_convert_sections.py` & `v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/models/bcl_convert_sections.py`

 * *Files identical despite different names*

### Comparing `v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/models/cloud_section.py` & `v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/models/cloud_section.py`

 * *Files identical despite different names*

### Comparing `v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/models/run_info_sections.py` & `v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/models/run_info_sections.py`

 * *Files identical despite different names*

### Comparing `v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/models/samplesheet.py` & `v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/models/samplesheet.py`

 * *Files identical despite different names*

### Comparing `v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/models/tso500l_sections.py` & `v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/models/tso500l_sections.py`

 * *Files identical despite different names*

### Comparing `v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/models/tso500s_sections.py` & `v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/models/tso500s_sections.py`

 * *Files identical despite different names*

### Comparing `v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/run/run_info_reader.py` & `v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/run/run_info_reader.py`

 * *Files identical despite different names*

### Comparing `v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/run/run_info_writer.py` & `v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/run/run_info_writer.py`

 * *Files identical despite different names*

### Comparing `v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/run/v2_samplesheet_reader.py` & `v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/run/v2_samplesheet_reader.py`

 * *Files identical despite different names*

### Comparing `v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/run/v2_samplesheet_to_run_info_xml.py` & `v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/run/v2_samplesheet_to_run_info_xml.py`

 * *Files identical despite different names*

### Comparing `v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/run/v2_samplesheet_writer.py` & `v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/run/v2_samplesheet_writer.py`

 * *Files identical despite different names*

### Comparing `v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/section_classes/bcl_convert_sections.py` & `v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/section_classes/bcl_convert_sections.py`

 * *Files identical despite different names*

### Comparing `v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/section_classes/cloud_sections.py` & `v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/section_classes/cloud_sections.py`

 * *Files identical despite different names*

### Comparing `v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/section_classes/run_info_sections.py` & `v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/section_classes/run_info_sections.py`

 * *Files identical despite different names*

### Comparing `v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/section_classes/tso500l_sections.py` & `v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/section_classes/tso500l_sections.py`

 * *Files identical despite different names*

### Comparing `v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/section_classes/tso500s_sections.py` & `v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/section_classes/tso500s_sections.py`

 * *Files identical despite different names*

### Comparing `v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/utils/__init__.py` & `v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/utils/cli.py` & `v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/utils/cli.py`

 * *Files identical despite different names*

### Comparing `v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/utils/docopt_docs.py` & `v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/utils/docopt_docs.py`

 * *Files identical despite different names*

### Comparing `v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/utils/logger.py` & `v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/utils/logger.py`

 * *Files identical despite different names*

### Comparing `v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker/utils/xml.py` & `v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker/utils/xml.py`

 * *Files identical despite different names*

### Comparing `v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker.egg-info/PKG-INFO` & `v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: v2_samplesheet_maker
-Version: 4.2.4.post20240508150053
+Version: 4.2.4.post20240528161300
 Summary: v2 SampleSheet maker
 Author-email: Alexis Lucattini <alexis.lucattini@umccr.org>
 Project-URL: Homepage, https://github.com/umccr/v2-samplesheet-maker
 Project-URL: Bug Tracker, https://github.com/umccr/v2-samplesheet-maker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `v2_samplesheet_maker-4.2.4.post20240508150053/src/v2_samplesheet_maker.egg-info/SOURCES.txt` & `v2_samplesheet_maker-4.2.4.post20240528161300/src/v2_samplesheet_maker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

