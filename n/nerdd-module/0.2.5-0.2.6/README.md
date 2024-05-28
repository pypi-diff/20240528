# Comparing `tmp/nerdd-module-0.2.5.tar.gz` & `tmp/nerdd_module-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nerdd-module-0.2.5.tar", last modified: Mon Apr  8 07:23:46 2024, max compression
+gzip compressed data, was "nerdd_module-0.2.6.tar", last modified: Tue May 28 10:41:38 2024, max compression
```

## Comparing `nerdd-module-0.2.5.tar` & `nerdd_module-0.2.6.tar`

### file list

```diff
@@ -1,85 +1,89 @@
-drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2024-04-08 07:23:46.356554 nerdd-module-0.2.5/
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     1554 2023-12-18 12:01:47.000000 nerdd-module-0.2.5/LICENSE
--rw-r--r--   0 hirte     (1000) hirte     (1000)     2460 2024-04-08 07:23:46.356554 nerdd-module-0.2.5/PKG-INFO
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      419 2024-01-24 10:52:08.000000 nerdd-module-0.2.5/README.md
-drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2024-04-08 07:23:45.600563 nerdd-module-0.2.5/nerdd_module/
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      243 2024-03-24 11:31:46.000000 nerdd-module-0.2.5/nerdd_module/__init__.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)    10022 2024-04-07 08:38:06.000000 nerdd-module-0.2.5/nerdd_module/abstract_model.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     4012 2024-03-22 18:30:38.000000 nerdd-module-0.2.5/nerdd_module/cli.py
-drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2024-04-08 07:23:45.604563 nerdd-module-0.2.5/nerdd_module/config/
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      241 2023-12-10 19:26:28.000000 nerdd-module-0.2.5/nerdd_module/config/__init__.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     2335 2023-12-10 17:11:45.000000 nerdd-module-0.2.5/nerdd_module/config/auto_configuration.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     1523 2023-12-06 23:18:58.000000 nerdd-module-0.2.5/nerdd_module/config/configuration.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      394 2024-01-24 09:35:05.000000 nerdd-module-0.2.5/nerdd_module/config/default_configuration.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      258 2023-12-06 23:18:58.000000 nerdd-module-0.2.5/nerdd_module/config/dict_configuration.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      337 2023-12-06 23:18:58.000000 nerdd-module-0.2.5/nerdd_module/config/merged_configuration.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      929 2024-03-24 21:07:43.000000 nerdd-module-0.2.5/nerdd_module/config/package_configuration.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     1744 2023-12-10 17:08:25.000000 nerdd-module-0.2.5/nerdd_module/config/yaml_configuration.py
-drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2024-04-08 07:23:46.168556 nerdd-module-0.2.5/nerdd_module/io/
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      465 2024-03-22 12:42:07.000000 nerdd-module-0.2.5/nerdd_module/io/__init__.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      889 2024-04-07 14:23:44.000000 nerdd-module-0.2.5/nerdd_module/io/csv_writer.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     3664 2024-03-27 06:58:24.000000 nerdd-module-0.2.5/nerdd_module/io/depth_first_explorer.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      264 2024-03-20 10:24:14.000000 nerdd-module-0.2.5/nerdd_module/io/explorer.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     1583 2024-04-07 08:55:03.000000 nerdd-module-0.2.5/nerdd_module/io/file_reader.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      855 2024-03-20 10:13:39.000000 nerdd-module-0.2.5/nerdd_module/io/gzip_reader.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     1628 2024-03-22 11:10:20.000000 nerdd-module-0.2.5/nerdd_module/io/inchi_reader.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      729 2024-03-20 10:17:29.000000 nerdd-module-0.2.5/nerdd_module/io/list_reader.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      599 2024-03-22 12:43:39.000000 nerdd-module-0.2.5/nerdd_module/io/mol_reader.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      531 2024-03-22 10:49:27.000000 nerdd-module-0.2.5/nerdd_module/io/reader.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     2021 2024-04-07 20:57:32.000000 nerdd-module-0.2.5/nerdd_module/io/reader_registry.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     2887 2024-03-22 10:49:14.000000 nerdd-module-0.2.5/nerdd_module/io/sdf_reader.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     1058 2023-12-11 19:46:27.000000 nerdd-module-0.2.5/nerdd_module/io/sdf_writer.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     1965 2024-03-22 10:49:43.000000 nerdd-module-0.2.5/nerdd_module/io/smiles_reader.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      530 2024-03-20 10:15:58.000000 nerdd-module-0.2.5/nerdd_module/io/string_reader.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      904 2024-03-20 10:14:38.000000 nerdd-module-0.2.5/nerdd_module/io/tar_reader.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     1224 2023-12-11 19:45:43.000000 nerdd-module-0.2.5/nerdd_module/io/writer.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      983 2023-12-06 23:18:58.000000 nerdd-module-0.2.5/nerdd_module/io/writer_registry.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      974 2024-03-20 10:15:18.000000 nerdd-module-0.2.5/nerdd_module/io/zip_reader.py
-drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2024-04-08 07:23:46.356554 nerdd-module-0.2.5/nerdd_module/polyfills/
--rw-rw-r--   0 hirte     (1000) hirte     (1000)       53 2024-03-24 20:59:23.000000 nerdd-module-0.2.5/nerdd_module/polyfills/__init__.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      153 2024-03-24 21:05:05.000000 nerdd-module-0.2.5/nerdd_module/polyfills/files.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      511 2024-03-27 09:45:43.000000 nerdd-module-0.2.5/nerdd_module/polyfills/get_entry_points.py
-drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2024-04-08 07:23:46.356554 nerdd-module-0.2.5/nerdd_module/preprocessing/
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      262 2024-02-27 15:00:52.000000 nerdd-module-0.2.5/nerdd_module/preprocessing/__init__.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      685 2024-02-27 15:00:52.000000 nerdd-module-0.2.5/nerdd_module/preprocessing/check_valid_smiles.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     3624 2024-04-01 17:51:23.000000 nerdd-module-0.2.5/nerdd_module/preprocessing/chembl_structure_pipeline.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      177 2023-12-06 23:18:58.000000 nerdd-module-0.2.5/nerdd_module/preprocessing/empty_pipeline.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     1240 2024-02-27 15:00:52.000000 nerdd-module-0.2.5/nerdd_module/preprocessing/filter_by_element.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     1065 2024-02-27 15:00:52.000000 nerdd-module-0.2.5/nerdd_module/preprocessing/filter_by_weight.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     1578 2024-03-22 10:50:00.000000 nerdd-module-0.2.5/nerdd_module/preprocessing/pipeline.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      435 2023-12-06 23:18:58.000000 nerdd-module-0.2.5/nerdd_module/preprocessing/registry.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      584 2024-02-27 15:00:52.000000 nerdd-module-0.2.5/nerdd_module/preprocessing/remove_stereochemistry.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      506 2024-02-27 15:00:52.000000 nerdd-module-0.2.5/nerdd_module/preprocessing/step.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      113 2024-03-22 10:41:14.000000 nerdd-module-0.2.5/nerdd_module/problem.py
-drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2024-04-08 07:23:46.356554 nerdd-module-0.2.5/nerdd_module/tests/
--rw-rw-r--   0 hirte     (1000) hirte     (1000)       80 2024-04-01 21:15:07.000000 nerdd-module-0.2.5/nerdd_module/tests/__init__.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     5531 2024-04-08 07:01:05.000000 nerdd-module-0.2.5/nerdd_module/tests/checks.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      693 2024-03-30 13:02:15.000000 nerdd-module-0.2.5/nerdd_module/tests/predictions.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     1998 2024-04-06 12:35:46.000000 nerdd-module-0.2.5/nerdd_module/tests/representations.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      198 2024-01-08 13:34:40.000000 nerdd-module-0.2.5/nerdd_module/version.py
-drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2024-04-08 07:23:46.356554 nerdd-module-0.2.5/nerdd_module.egg-info/
--rw-r--r--   0 hirte     (1000) hirte     (1000)     2460 2024-04-08 07:23:45.000000 nerdd-module-0.2.5/nerdd_module.egg-info/PKG-INFO
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     2400 2024-04-08 07:23:45.000000 nerdd-module-0.2.5/nerdd_module.egg-info/SOURCES.txt
--rw-rw-r--   0 hirte     (1000) hirte     (1000)        1 2024-04-08 07:23:45.000000 nerdd-module-0.2.5/nerdd_module.egg-info/dependency_links.txt
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      388 2024-04-08 07:23:45.000000 nerdd-module-0.2.5/nerdd_module.egg-info/requires.txt
--rw-rw-r--   0 hirte     (1000) hirte     (1000)       19 2024-04-08 07:23:45.000000 nerdd-module-0.2.5/nerdd_module.egg-info/top_level.txt
--rw-rw-r--   0 hirte     (1000) hirte     (1000)       38 2024-04-08 07:23:46.356554 nerdd-module-0.2.5/setup.cfg
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     2654 2024-04-08 06:53:55.000000 nerdd-module-0.2.5/setup.py
-drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2024-04-08 07:23:46.356554 nerdd-module-0.2.5/tests/
--rw-rw-r--   0 hirte     (1000) hirte     (1000)        0 2023-12-06 23:18:58.000000 nerdd-module-0.2.5/tests/__init__.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      281 2024-04-06 12:32:55.000000 nerdd-module-0.2.5/tests/conftest.py
-drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2024-04-08 07:23:46.356554 nerdd-module-0.2.5/tests/models/
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      928 2023-12-06 23:18:58.000000 nerdd-module-0.2.5/tests/models/AtomicMassModel.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      796 2024-03-22 18:15:00.000000 nerdd-module-0.2.5/tests/models/MolWeightModel.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      921 2024-03-22 18:21:41.000000 nerdd-module-0.2.5/tests/models/MolWeightModelWithExplicitMolIds.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      876 2024-03-22 18:21:50.000000 nerdd-module-0.2.5/tests/models/MolWeightModelWithExplicitMols.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      155 2023-12-06 23:18:58.000000 nerdd-module-0.2.5/tests/models/__init__.py
-drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2024-04-08 07:23:46.356554 nerdd-module-0.2.5/tests/steps/
--rw-rw-r--   0 hirte     (1000) hirte     (1000)       77 2024-04-06 12:33:52.000000 nerdd-module-0.2.5/tests/steps/__init__.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     1596 2024-03-22 18:21:18.000000 nerdd-module-0.2.5/tests/steps/checks.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     1449 2023-12-06 23:18:58.000000 nerdd-module-0.2.5/tests/steps/predictors.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      278 2023-12-06 23:18:58.000000 nerdd-module-0.2.5/tests/steps/preprocessing.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     2248 2023-12-06 23:18:58.000000 nerdd-module-0.2.5/tests/test_atom_property_prediction.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     2036 2024-03-22 18:20:19.000000 nerdd-module-0.2.5/tests/test_molecule_property_prediction.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      360 2023-12-06 23:18:58.000000 nerdd-module-0.2.5/tests/test_preprocessing.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     4681 2024-03-22 18:24:13.000000 nerdd-module-0.2.5/tests/test_reading_formats.py
+drwxr-xr-x   0 hirte     (1000) hirte     (1000)        0 2024-05-28 10:41:38.353666 nerdd_module-0.2.6/
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     1554 2023-12-18 12:01:47.000000 nerdd_module-0.2.6/LICENSE
+-rw-r--r--   0 hirte     (1000) hirte     (1000)     2566 2024-05-28 10:41:38.353666 nerdd_module-0.2.6/PKG-INFO
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      419 2024-01-24 10:52:08.000000 nerdd_module-0.2.6/README.md
+drwxr-xr-x   0 hirte     (1000) hirte     (1000)        0 2024-05-28 10:41:38.349666 nerdd_module-0.2.6/nerdd_module/
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      243 2024-03-24 11:31:46.000000 nerdd_module-0.2.6/nerdd_module/__init__.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)    10112 2024-05-28 09:32:51.000000 nerdd_module-0.2.6/nerdd_module/abstract_model.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     4016 2024-05-15 07:36:59.000000 nerdd_module-0.2.6/nerdd_module/cli.py
+drwxr-xr-x   0 hirte     (1000) hirte     (1000)        0 2024-05-28 10:41:38.349666 nerdd_module-0.2.6/nerdd_module/config/
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      241 2023-12-10 19:26:28.000000 nerdd_module-0.2.6/nerdd_module/config/__init__.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     2335 2023-12-10 17:11:45.000000 nerdd_module-0.2.6/nerdd_module/config/auto_configuration.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     1523 2023-12-06 23:18:58.000000 nerdd_module-0.2.6/nerdd_module/config/configuration.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     1175 2024-05-28 09:51:53.000000 nerdd_module-0.2.6/nerdd_module/config/default_configuration.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      258 2023-12-06 23:18:58.000000 nerdd_module-0.2.6/nerdd_module/config/dict_configuration.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      458 2024-05-27 14:11:38.000000 nerdd_module-0.2.6/nerdd_module/config/merged_configuration.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      929 2024-05-27 14:10:20.000000 nerdd_module-0.2.6/nerdd_module/config/package_configuration.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     1744 2023-12-10 17:08:25.000000 nerdd_module-0.2.6/nerdd_module/config/yaml_configuration.py
+drwxr-xr-x   0 hirte     (1000) hirte     (1000)        0 2024-05-28 10:41:38.349666 nerdd_module-0.2.6/nerdd_module/input/
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      360 2024-05-27 14:42:34.000000 nerdd_module-0.2.6/nerdd_module/input/__init__.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     3664 2024-03-27 06:58:24.000000 nerdd_module-0.2.6/nerdd_module/input/depth_first_explorer.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      264 2024-03-20 10:24:14.000000 nerdd_module-0.2.6/nerdd_module/input/explorer.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     1613 2024-05-27 15:27:58.000000 nerdd_module-0.2.6/nerdd_module/input/file_reader.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      855 2024-03-20 10:13:39.000000 nerdd_module-0.2.6/nerdd_module/input/gzip_reader.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     1628 2024-03-22 11:10:20.000000 nerdd_module-0.2.6/nerdd_module/input/inchi_reader.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      729 2024-03-20 10:17:29.000000 nerdd_module-0.2.6/nerdd_module/input/list_reader.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      599 2024-03-22 12:43:39.000000 nerdd_module-0.2.6/nerdd_module/input/mol_reader.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      531 2024-03-22 10:49:27.000000 nerdd_module-0.2.6/nerdd_module/input/reader.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     2064 2024-05-27 15:28:56.000000 nerdd_module-0.2.6/nerdd_module/input/reader_registry.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     2887 2024-03-22 10:49:14.000000 nerdd_module-0.2.6/nerdd_module/input/sdf_reader.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     1965 2024-03-22 10:49:43.000000 nerdd_module-0.2.6/nerdd_module/input/smiles_reader.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      530 2024-03-20 10:15:58.000000 nerdd_module-0.2.6/nerdd_module/input/string_reader.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      904 2024-03-20 10:14:38.000000 nerdd_module-0.2.6/nerdd_module/input/tar_reader.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      974 2024-03-20 10:15:18.000000 nerdd_module-0.2.6/nerdd_module/input/zip_reader.py
+drwxr-xr-x   0 hirte     (1000) hirte     (1000)        0 2024-05-28 10:41:38.349666 nerdd_module-0.2.6/nerdd_module/output/
+-rw-r--r--   0 hirte     (1000) hirte     (1000)       31 2024-05-27 14:44:47.000000 nerdd_module-0.2.6/nerdd_module/output/__init__.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      889 2024-04-07 14:23:44.000000 nerdd_module-0.2.6/nerdd_module/output/csv_writer.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     1058 2023-12-11 19:46:27.000000 nerdd_module-0.2.6/nerdd_module/output/sdf_writer.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     1224 2023-12-11 19:45:43.000000 nerdd_module-0.2.6/nerdd_module/output/writer.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      983 2023-12-06 23:18:58.000000 nerdd_module-0.2.6/nerdd_module/output/writer_registry.py
+drwxr-xr-x   0 hirte     (1000) hirte     (1000)        0 2024-05-28 10:41:38.349666 nerdd_module-0.2.6/nerdd_module/polyfills/
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)       76 2024-05-14 17:19:24.000000 nerdd_module-0.2.6/nerdd_module/polyfills/__init__.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      153 2024-03-24 21:05:05.000000 nerdd_module-0.2.6/nerdd_module/polyfills/files.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      511 2024-03-27 09:45:43.000000 nerdd_module-0.2.6/nerdd_module/polyfills/get_entry_points.py
+-rw-r--r--   0 hirte     (1000) hirte     (1000)      158 2024-05-14 17:19:33.000000 nerdd_module-0.2.6/nerdd_module/polyfills/version.py
+drwxr-xr-x   0 hirte     (1000) hirte     (1000)        0 2024-05-28 10:41:38.349666 nerdd_module-0.2.6/nerdd_module/preprocessing/
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      300 2024-05-28 08:58:08.000000 nerdd_module-0.2.6/nerdd_module/preprocessing/__init__.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      643 2024-05-26 14:13:49.000000 nerdd_module-0.2.6/nerdd_module/preprocessing/check_valid_smiles.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     3654 2024-05-26 14:15:33.000000 nerdd_module-0.2.6/nerdd_module/preprocessing/chembl_structure_pipeline.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      177 2023-12-06 23:18:58.000000 nerdd_module-0.2.6/nerdd_module/preprocessing/empty_pipeline.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     1260 2024-05-26 14:22:56.000000 nerdd_module-0.2.6/nerdd_module/preprocessing/filter_by_element.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     1150 2024-05-27 17:17:07.000000 nerdd_module-0.2.6/nerdd_module/preprocessing/filter_by_weight.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     1578 2024-03-22 10:50:00.000000 nerdd_module-0.2.6/nerdd_module/preprocessing/pipeline.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      435 2023-12-06 23:18:58.000000 nerdd_module-0.2.6/nerdd_module/preprocessing/registry.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      584 2024-02-27 15:00:52.000000 nerdd_module-0.2.6/nerdd_module/preprocessing/remove_stereochemistry.py
+-rw-r--r--   0 hirte     (1000) hirte     (1000)      286 2024-05-28 09:25:54.000000 nerdd_module-0.2.6/nerdd_module/preprocessing/sanitize.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      536 2024-05-26 14:13:12.000000 nerdd_module-0.2.6/nerdd_module/preprocessing/step.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      322 2024-05-28 09:39:10.000000 nerdd_module-0.2.6/nerdd_module/problem.py
+drwxr-xr-x   0 hirte     (1000) hirte     (1000)        0 2024-05-28 10:41:38.349666 nerdd_module-0.2.6/nerdd_module/tests/
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)       80 2024-04-01 21:15:07.000000 nerdd_module-0.2.6/nerdd_module/tests/__init__.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     5581 2024-05-27 15:31:22.000000 nerdd_module-0.2.6/nerdd_module/tests/checks.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      693 2024-03-30 13:02:15.000000 nerdd_module-0.2.6/nerdd_module/tests/predictions.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     1998 2024-04-06 12:35:46.000000 nerdd_module-0.2.6/nerdd_module/tests/representations.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)       94 2024-05-14 17:30:35.000000 nerdd_module-0.2.6/nerdd_module/version.py
+drwxr-xr-x   0 hirte     (1000) hirte     (1000)        0 2024-05-28 10:41:38.353666 nerdd_module-0.2.6/nerdd_module.egg-info/
+-rw-r--r--   0 hirte     (1000) hirte     (1000)     2566 2024-05-28 10:41:38.000000 nerdd_module-0.2.6/nerdd_module.egg-info/PKG-INFO
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     2566 2024-05-28 10:41:38.000000 nerdd_module-0.2.6/nerdd_module.egg-info/SOURCES.txt
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)        1 2024-05-28 10:41:38.000000 nerdd_module-0.2.6/nerdd_module.egg-info/dependency_links.txt
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      407 2024-05-28 10:41:38.000000 nerdd_module-0.2.6/nerdd_module.egg-info/requires.txt
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)       19 2024-05-28 10:41:38.000000 nerdd_module-0.2.6/nerdd_module.egg-info/top_level.txt
+-rw-r--r--   0 hirte     (1000) hirte     (1000)       38 2024-05-28 10:41:38.353666 nerdd_module-0.2.6/setup.cfg
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     2873 2024-05-27 15:40:10.000000 nerdd_module-0.2.6/setup.py
+drwxr-xr-x   0 hirte     (1000) hirte     (1000)        0 2024-05-28 10:41:38.353666 nerdd_module-0.2.6/tests/
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)        0 2023-12-06 23:18:58.000000 nerdd_module-0.2.6/tests/__init__.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      281 2024-04-06 12:32:55.000000 nerdd_module-0.2.6/tests/conftest.py
+drwxr-xr-x   0 hirte     (1000) hirte     (1000)        0 2024-05-28 10:41:38.353666 nerdd_module-0.2.6/tests/models/
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      928 2023-12-06 23:18:58.000000 nerdd_module-0.2.6/tests/models/AtomicMassModel.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      776 2024-05-28 08:57:52.000000 nerdd_module-0.2.6/tests/models/MolWeightModel.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      954 2024-05-28 09:32:42.000000 nerdd_module-0.2.6/tests/models/MolWeightModelWithExplicitMolIds.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      862 2024-05-28 09:03:31.000000 nerdd_module-0.2.6/tests/models/MolWeightModelWithExplicitMols.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      155 2023-12-06 23:18:58.000000 nerdd_module-0.2.6/tests/models/__init__.py
+drwxr-xr-x   0 hirte     (1000) hirte     (1000)        0 2024-05-28 10:41:38.353666 nerdd_module-0.2.6/tests/steps/
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)       77 2024-04-06 12:33:52.000000 nerdd_module-0.2.6/tests/steps/__init__.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     1596 2024-03-22 18:21:18.000000 nerdd_module-0.2.6/tests/steps/checks.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     1449 2024-05-27 16:12:52.000000 nerdd_module-0.2.6/tests/steps/predictors.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      278 2023-12-06 23:18:58.000000 nerdd_module-0.2.6/tests/steps/preprocessing.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     2248 2023-12-06 23:18:58.000000 nerdd_module-0.2.6/tests/test_atom_property_prediction.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     2036 2024-03-22 18:20:19.000000 nerdd_module-0.2.6/tests/test_molecule_property_prediction.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      360 2023-12-06 23:18:58.000000 nerdd_module-0.2.6/tests/test_preprocessing.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     4681 2024-03-22 18:24:13.000000 nerdd_module-0.2.6/tests/test_reading_formats.py
```

### Comparing `nerdd-module-0.2.5/LICENSE` & `nerdd_module-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.5/PKG-INFO` & `nerdd_module-0.2.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: nerdd-module
-Version: 0.2.5
+Version: 0.2.6
 Summary: Base package to create NERDD modules
-Home-page: https://github.com/molinfo-vienna/nerdd-module.git
+Home-page: https://github.com/molinfo-vienna/nerdd-module
 Maintainer: Steffen Hirte
 Maintainer-email: steffen.hirte@univie.ac.at
 License: BSD 3-Clause License
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: C
@@ -29,16 +29,19 @@
 Requires-Dist: pyyaml>=6.0
 Requires-Dist: filetype~=1.2.0
 Requires-Dist: rich-click>=1.7.1
 Requires-Dist: stringcase>=1.2.0
 Requires-Dist: decorator>=5.1.1
 Requires-Dist: importlib-resources>=5; python_version < "3.10"
 Requires-Dist: importlib-metadata>=4.6; python_version < "3.10"
-Requires-Dist: chembl_structure_pipeline>=1.0.0
 Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+Requires-Dist: isort; extra == "dev"
+Provides-Extra: csp
+Requires-Dist: chembl_structure_pipeline>=1.0.0; extra == "csp"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-sugar; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-asyncio; extra == "test"
 Requires-Dist: pytest-bdd; extra == "test"
 Requires-Dist: pytest-mock; extra == "test"
```

### Comparing `nerdd-module-0.2.5/nerdd_module/abstract_model.py` & `nerdd_module-0.2.6/nerdd_module/abstract_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from abc import ABC, abstractmethod
-from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple, Union
+from typing import Callable, Iterable, List, Tuple, Union
 
 import pandas as pd
-from rdkit.Chem import Mol, MolToSmiles
+from rdkit.Chem import Mol
 
 from .config import AutoConfiguration, Configuration
-from .io import DepthFirstExplorer, MoleculeEntry
+from .input import DepthFirstExplorer, MoleculeEntry
 from .preprocessing import Pipeline, Step, registry
-from .problem import Problem
+from .problem import Problem, UnknownProblem
 
 __all__ = ["AbstractModel"]
 
 
 class CustomPreprocessingStep(Step):
     def __init__(self, fn: Callable[[Mol], Tuple[Mol, List[Problem]]]):
         super().__init__()
@@ -152,25 +152,28 @@
         # 1. df_prediction contains a column "mol_id" that contains the molecule ids
         # 2. df_prediction contains a column "mol" that contains the molecules, which
         #    have the id as their name so that we can match them to the original
         # 3. df_prediction has the same length as the number of valid molecules
         #    (and we assume that the order of the molecules is the same)
         if "mol_id" in df_predictions.columns:
             # check that mol_id contains only valid ids
-            assert set(df_predictions.mol_id).issubset(
-                set(df_valid_subset.mol_id)
-            ), f"The mol_id column contains invalid ids: {set(df_predictions.mol_id).difference(set(df_valid_subset.mol_id))}."
+            assert set(df_predictions.mol_id).issubset(set(df_valid_subset.mol_id)), (
+                f"The mol_id column contains invalid ids: "
+                f"{set(df_predictions.mol_id).difference(set(df_valid_subset.mol_id))}."
+            )
+
             # use mol_id as index
             df_predictions.set_index("mol_id", drop=True, inplace=True)
         elif "mol" in df_predictions.columns:
             # check that molecule names contain only valid ids
             names = df_predictions.mol.apply(lambda mol: int(mol.GetProp("_Name")))
-            assert set(names).issubset(
-                set(df_preprocess.mol_id)
-            ), f"The mol_id column contains invalid ids: {set(df_predictions.mol_id).difference(set(df_valid_subset.mol_id))}."
+            assert set(names).issubset(set(df_preprocess.mol_id)), (
+                f"The mol_id column contains invalid ids: "
+                f"{set(df_predictions.mol_id).difference(set(df_valid_subset.mol_id))}."
+            )
 
             # use mol_id as index
             df_predictions.set_index(
                 names,
                 inplace=True,
             )
             df_predictions.drop(columns="mol", inplace=True)
@@ -180,14 +183,16 @@
                 "valid input molecules."
             )
             # use index from input series (type cast if series was empty)
             df_predictions.set_index(
                 df_valid_subset.index.astype("int64"), inplace=True
             )
 
+        # TODO: check derivative_id or atom_id
+
         # add column that indicates whether a molecule was missing
         missing_mol_ids = set(df_preprocess.mol_id).difference(df_predictions.index)
         df_preprocess["missing"] = df_preprocess.mol_id.isin(missing_mol_ids)
 
         # merge the preprocessed molecules with the predictions
         df_result = df_preprocess.merge(
             df_predictions, left_on="mol_id", right_index=True, how="left"
@@ -208,15 +213,15 @@
             df_result["errors"] = (
                 df_result.preprocessing_errors + df_result.prediction_errors
             )
             df_result.drop(columns=["prediction_errors"], inplace=True)
         else:
             df_result["errors"] = df_result.preprocessing_errors
         df_result["errors"] = df_result.errors + df_result.missing.map(
-            lambda x: ["!1"] if x else []
+            lambda x: [UnknownProblem()] if x else []
         )
         df_result.drop(columns=["missing", "preprocessing_errors"], inplace=True)
 
         # convert errors to string
         if "errors" not in df_result.columns:
             df_result["errors"] = []
```

### Comparing `nerdd-module-0.2.5/nerdd_module/cli.py` & `nerdd_module-0.2.6/nerdd_module/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import os
 import sys
 
 import rich_click as click
 from decorator import decorator
-from nerdd_module.io import WriterRegistry
+from nerdd_module.output import WriterRegistry
 from stringcase import spinalcase
 
 __all__ = ["auto_cli"]
 
 input_description = """{description}
 
 INPUT molecules are provided as file paths or strings. The following formats are
```

### Comparing `nerdd-module-0.2.5/nerdd_module/config/auto_configuration.py` & `nerdd_module-0.2.6/nerdd_module/config/auto_configuration.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.5/nerdd_module/config/configuration.py` & `nerdd_module-0.2.6/nerdd_module/config/configuration.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.5/nerdd_module/config/package_configuration.py` & `nerdd_module-0.2.6/nerdd_module/config/package_configuration.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.5/nerdd_module/config/yaml_configuration.py` & `nerdd_module-0.2.6/nerdd_module/config/yaml_configuration.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.5/nerdd_module/io/csv_writer.py` & `nerdd_module-0.2.6/nerdd_module/output/csv_writer.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.5/nerdd_module/io/depth_first_explorer.py` & `nerdd_module-0.2.6/nerdd_module/input/depth_first_explorer.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.5/nerdd_module/io/file_reader.py` & `nerdd_module-0.2.6/nerdd_module/input/file_reader.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-import os
 from pathlib import Path
-from typing import Generator
+from typing import Generator, Tuple
 
 from .reader import MoleculeEntry, Reader
 from .reader_registry import register_reader
 
 __all__ = ["FileReader"]
 
 
@@ -20,31 +19,33 @@
         assert isinstance(filename, str), "input must be a string"
 
         # convert filename to path
         try:
             path = Path(filename)
         except:
             raise ValueError("input must be a valid path")
-        
+
         # convert to absolute path
         if not path.is_absolute():
             if self.data_dir is not None:
                 path = self.data_dir / path
             else:
                 path = Path(".") / path
 
         # check that the file is within the data_dir
-        assert self.data_dir is None or self.data_dir in path.parents, "input must be a relative path"
+        assert (
+            self.data_dir is None or self.data_dir in path.parents
+        ), "input must be a relative path"
 
         # check that the file exists
         assert path.exists(), "input must be a valid file"
 
         with open(path, "rb") as f:
             for entry in explore(f):
                 if len(entry.source) == 1 and entry.source[0] == "raw_input":
-                    source = tuple()
+                    source: Tuple[str, ...] = tuple()
                 else:
                     source = entry.source
                 yield entry._replace(source=tuple([filename, *source]))
 
     def __repr__(self):
         return f"FileReader()"
```

### Comparing `nerdd-module-0.2.5/nerdd_module/io/gzip_reader.py` & `nerdd_module-0.2.6/nerdd_module/input/gzip_reader.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.5/nerdd_module/io/inchi_reader.py` & `nerdd_module-0.2.6/nerdd_module/input/inchi_reader.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.5/nerdd_module/io/list_reader.py` & `nerdd_module-0.2.6/nerdd_module/input/list_reader.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.5/nerdd_module/io/mol_reader.py` & `nerdd_module-0.2.6/nerdd_module/input/mol_reader.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.5/nerdd_module/io/reader.py` & `nerdd_module-0.2.6/nerdd_module/input/reader.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.5/nerdd_module/io/reader_registry.py` & `nerdd_module-0.2.6/nerdd_module/input/reader_registry.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,29 +6,33 @@
 __all__ = ["ReaderRegistry", "register_reader"]
 
 
 # lru_cache makes the registry a singleton
 @lru_cache(maxsize=1)
 class ReaderRegistry:
     def __init__(self):
-        self._factories : List[Tuple[Type[Reader], Tuple[str, ...], Dict[str, str]]] = []
+        self._factories: List[Tuple[Type[Reader], Tuple[str, ...], Dict[str, str]]] = []
         self._config = {}
 
     def _create_reader(self, ReaderClass: Type[Reader], *args, **kwargs) -> Reader:
         # translate all args
-        args = [self._config.get(arg, None) for arg in args]
+        args = tuple(self._config.get(arg, None) for arg in args)
         # translate all kwargs
-        kwargs = {k: self._config.get(v, None) for k, v in kwargs.items() if v in self._config}
+        kwargs = {
+            k: self._config.get(v, None) for k, v in kwargs.items() if v in self._config
+        }
 
         return ReaderClass(*args, **kwargs)
 
-    def register(self, ReaderClass: Type[Reader], *args :str , **kwargs:str):
+    def register(self, ReaderClass: Type[Reader], *args: str, **kwargs: str):
         assert issubclass(ReaderClass, Reader)
         assert all([isinstance(arg, str) for arg in args])
-        assert all([isinstance(k, str) and isinstance(v, str) for k, v in kwargs.items()])
+        assert all(
+            [isinstance(k, str) and isinstance(v, str) for k, v in kwargs.items()]
+        )
         self._factories.append((ReaderClass, args, kwargs))
 
     def readers(self) -> Generator[Reader, None, None]:
         for reader, args, kwargs in self._factories:
             yield self._create_reader(reader, *args, **kwargs)
 
     def __iter__(self):
@@ -36,24 +40,25 @@
 
 
 def register_reader(*args, **kwargs):
     def wrapper(cls, *args, **kwargs):
         ReaderRegistry().register(cls, *args, **kwargs)
         return cls
 
-    # Case 1: first argument is a class 
-    # --> decorator is used without arguments 
+    # Case 1: first argument is a class
+    # --> decorator is used without arguments
     # @register_reader
     # class F:
     #     ...
     if len(args) > 0 and isinstance(args[0], type):
         return wrapper(args[0], *args[1:], **kwargs)
-    
+
     # Case 2: first argument is a not a class
     # --> decorator is used with arguments
     # @register_reader("blah")
     # class F:
     #     ...
     def inner(cls):
         assert isinstance(cls, type), "Decorator must be used with a class"
         return wrapper(cls, *args, **kwargs)
+
     return inner
```

### Comparing `nerdd-module-0.2.5/nerdd_module/io/sdf_reader.py` & `nerdd_module-0.2.6/nerdd_module/input/sdf_reader.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.5/nerdd_module/io/sdf_writer.py` & `nerdd_module-0.2.6/nerdd_module/output/sdf_writer.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.5/nerdd_module/io/smiles_reader.py` & `nerdd_module-0.2.6/nerdd_module/input/smiles_reader.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.5/nerdd_module/io/string_reader.py` & `nerdd_module-0.2.6/nerdd_module/input/string_reader.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.5/nerdd_module/io/tar_reader.py` & `nerdd_module-0.2.6/nerdd_module/input/tar_reader.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.5/nerdd_module/io/writer.py` & `nerdd_module-0.2.6/nerdd_module/output/writer.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.5/nerdd_module/io/writer_registry.py` & `nerdd_module-0.2.6/nerdd_module/output/writer_registry.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.5/nerdd_module/io/zip_reader.py` & `nerdd_module-0.2.6/nerdd_module/input/zip_reader.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.5/nerdd_module/preprocessing/check_valid_smiles.py` & `nerdd_module-0.2.6/nerdd_module/preprocessing/remove_stereochemistry.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 from typing import List, Tuple
 
-from rdkit.Chem import Mol, MolFromSmiles, MolToSmiles
+from rdkit.Chem import Mol
+from rdkit.Chem import RemoveStereochemistry as remove_stereochemistry
 
 from ..problem import Problem
 from .step import Step
 
-__all__ = ["CheckValidSmiles"]
-
-
-class CheckValidSmiles(Step):
-    """Checks if the molecule can be converted to SMILES and back."""
 
+class RemoveStereochemistry(Step):
     def __init__(self):
         super().__init__()
 
     def _run(self, mol: Mol) -> Tuple[Mol, List[Problem]]:
         errors = []
 
-        smi = MolToSmiles(mol, True)
-        check_mol = MolFromSmiles(smi)
-        if check_mol is None:
+        try:
+            remove_stereochemistry(mol)
+        except Exception:
             errors.append(
-                Problem("invalid_smiles", "Cannot convert molecule to SMILES")
+                Problem("remove_stereochemistry", "Cannot remove stereochemistry")
             )
-            mol = None
 
         return mol, errors
```

### Comparing `nerdd-module-0.2.5/nerdd_module/preprocessing/chembl_structure_pipeline.py` & `nerdd_module-0.2.6/nerdd_module/preprocessing/chembl_structure_pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import warnings
-from typing import List, Tuple
+from typing import List, Optional, Tuple
 
 from rdkit.Chem import Mol
 from rdkit.rdBase import BlockLogs
 
 from ..problem import Problem
 from .check_valid_smiles import CheckValidSmiles
 from .filter_by_element import FilterByElement
@@ -37,15 +37,15 @@
 class StandardizeWithCsp(Step):
     def __init__(self):
         super().__init__()
 
         if import_error is not None:
             raise import_error
 
-    def _run(self, mol: Mol) -> Tuple[Mol, List[Problem]]:
+    def _run(self, mol: Mol) -> Tuple[Optional[Mol], List[Problem]]:
         errors = []
 
         # chembl structure pipeline cannot handle molecules with 3D coordinates
         # --> delete conformers
         mol.RemoveAllConformers()
 
         # standardization via chembl structure pipeline
@@ -61,15 +61,15 @@
 class GetParentMol(Step):
     def __init__(self):
         super().__init__()
 
         if import_error is not None:
             raise import_error
 
-    def _run(self, mol: Mol) -> Tuple[Mol, List[Problem]]:
+    def _run(self, mol: Mol) -> Tuple[Optional[Mol], List[Problem]]:
         errors = []
 
         # chembl structure pipeline cannot handle molecules with 3D coordinates
         # --> delete conformers
         mol.RemoveAllConformers()
 
         # get parent molecule via chembl structure pipeline
```

### Comparing `nerdd-module-0.2.5/nerdd_module/preprocessing/filter_by_element.py` & `nerdd_module-0.2.6/nerdd_module/preprocessing/filter_by_element.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Iterable, List, Tuple
+from typing import Iterable, List, Optional, Tuple
 
 from rdkit.Chem import Mol
 
 from ..problem import Problem
 from .step import Step
 
 
@@ -10,15 +10,15 @@
     def __init__(
         self, allowed_elements: Iterable[str], remove_invalid_molecules: bool = False
     ):
         super().__init__()
         self.allowed_elements = set(allowed_elements)
         self.remove_invalid_molecules = remove_invalid_molecules
 
-    def _run(self, mol: Mol) -> Tuple[Mol, List[Problem]]:
+    def _run(self, mol: Mol) -> Tuple[Optional[Mol], List[Problem]]:
         errors = []
         result_mol = mol
 
         elements = set(atom.GetSymbol() for atom in mol.GetAtoms())
         invalid_elements = elements - self.allowed_elements
         if len(elements - self.allowed_elements) > 0:
             if self.remove_invalid_molecules:
```

### Comparing `nerdd-module-0.2.5/nerdd_module/preprocessing/filter_by_weight.py` & `nerdd_module-0.2.6/nerdd_module/preprocessing/filter_by_weight.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Tuple
+from typing import List, Optional, Tuple
 
 from rdkit.Chem import Mol
 from rdkit.Chem.Descriptors import MolWt
 
 from ..problem import Problem
 from .step import Step
 
@@ -10,27 +10,29 @@
 class FilterByWeight(Step):
     def __init__(self, min_weight, max_weight, remove_invalid_molecules=False):
         super().__init__()
         self.min_weight = min_weight
         self.max_weight = max_weight
         self.remove_invalid_molecules = remove_invalid_molecules
 
-    def _run(self, mol: Mol) -> Tuple[Mol, List[Problem]]:
+    def _run(self, mol: Mol) -> Tuple[Optional[Mol], List[Problem]]:
         errors = []
 
         weight = MolWt(mol)
         if weight < self.min_weight or weight > self.max_weight:
             if self.remove_invalid_molecules:
                 result_mol = None
             else:
                 result_mol = mol
             errors.append(
                 Problem(
-                    "invalid_weight",
-                    f"Molecular weight {weight:.2f} out of range "
-                    f"[{self.min_weight}, {self.max_weight}]",
+                    type="invalid_weight",
+                    message=(
+                        f"Molecular weight {weight:.2f} out of range "
+                        f"[{self.min_weight}, {self.max_weight}]"
+                    ),
                 )
             )
         else:
             result_mol = mol
 
         return result_mol, errors
```

### Comparing `nerdd-module-0.2.5/nerdd_module/preprocessing/pipeline.py` & `nerdd_module-0.2.6/nerdd_module/preprocessing/pipeline.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.5/nerdd_module/tests/checks.py` & `nerdd_module-0.2.6/nerdd_module/tests/checks.py`

 * *Files 8% similar despite different names*

```diff
@@ -134,17 +134,23 @@
 def check_column_length(subset, column_name, length):
     length = int(length)
     assert (
         subset[column_name].map(lambda x: len(x) > length)
     ).all(), f"Column {column_name} has unexpected length"
 
 
-@then(parsers.parse("when '{condition_column_name}' is '{condition_value}' " 
-                    "the value in column '{column_name}' should be '{expected_value}'"))
-def check_conditional_column_value(subset, condition_column_name, condition_value, column_name, expected_value):
+@then(
+    parsers.parse(
+        "when '{condition_column_name}' is '{condition_value}' "
+        "the value in column '{column_name}' should be '{expected_value}'"
+    )
+)
+def check_conditional_column_value(
+    subset, condition_column_name, condition_value, column_name, expected_value
+):
     # expected value is always provided as string
     # try to convert to float if possible
     try:
         expected_value = literal_eval(expected_value)
     except:
         pass
 
@@ -157,18 +163,22 @@
     # condition value can be (none) to indicate None
     if condition_value == "(none)":
         subset = subset[pd.isnull(subset[condition_column_name])]
     else:
         subset = subset[subset[condition_column_name] == condition_value]
 
     value = subset[column_name]
-    assert len(value) > 0, f"No rows found for condition {condition_column_name} == {condition_value}"
+    assert (
+        len(value) > 0
+    ), f"No rows found for condition {condition_column_name} == {condition_value}"
 
     # expected value can be (none) to indicate None
     if expected_value == "(none)":
         # if expected_value is the magic string "(none)", we expect None
-        assert pd.isnull(value).all(), f"Column {column_name} is assigned to {value} != None"
+        assert pd.isnull(
+            value
+        ).all(), f"Column {column_name} is assigned to {value} != None"
     else:
         # otherwise, we expect the value to be equal to the expected value
         assert (
-            (value == expected_value).all()
-        ), f"Column {column_name} is assigned to {value} != {expected_value}"
+            value == expected_value
+        ).all(), f"Column {column_name} is assigned to {value} != {expected_value}"
```

### Comparing `nerdd-module-0.2.5/nerdd_module/tests/predictions.py` & `nerdd_module-0.2.6/nerdd_module/tests/predictions.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.5/nerdd_module/tests/representations.py` & `nerdd_module-0.2.6/nerdd_module/tests/representations.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.5/nerdd_module.egg-info/PKG-INFO` & `nerdd_module-0.2.6/nerdd_module.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: nerdd-module
-Version: 0.2.5
+Version: 0.2.6
 Summary: Base package to create NERDD modules
-Home-page: https://github.com/molinfo-vienna/nerdd-module.git
+Home-page: https://github.com/molinfo-vienna/nerdd-module
 Maintainer: Steffen Hirte
 Maintainer-email: steffen.hirte@univie.ac.at
 License: BSD 3-Clause License
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: C
@@ -29,16 +29,19 @@
 Requires-Dist: pyyaml>=6.0
 Requires-Dist: filetype~=1.2.0
 Requires-Dist: rich-click>=1.7.1
 Requires-Dist: stringcase>=1.2.0
 Requires-Dist: decorator>=5.1.1
 Requires-Dist: importlib-resources>=5; python_version < "3.10"
 Requires-Dist: importlib-metadata>=4.6; python_version < "3.10"
-Requires-Dist: chembl_structure_pipeline>=1.0.0
 Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+Requires-Dist: isort; extra == "dev"
+Provides-Extra: csp
+Requires-Dist: chembl_structure_pipeline>=1.0.0; extra == "csp"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-sugar; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-asyncio; extra == "test"
 Requires-Dist: pytest-bdd; extra == "test"
 Requires-Dist: pytest-mock; extra == "test"
```

### Comparing `nerdd-module-0.2.5/nerdd_module.egg-info/SOURCES.txt` & `nerdd_module-0.2.6/nerdd_module.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -15,45 +15,48 @@
 nerdd_module/config/auto_configuration.py
 nerdd_module/config/configuration.py
 nerdd_module/config/default_configuration.py
 nerdd_module/config/dict_configuration.py
 nerdd_module/config/merged_configuration.py
 nerdd_module/config/package_configuration.py
 nerdd_module/config/yaml_configuration.py
-nerdd_module/io/__init__.py
-nerdd_module/io/csv_writer.py
-nerdd_module/io/depth_first_explorer.py
-nerdd_module/io/explorer.py
-nerdd_module/io/file_reader.py
-nerdd_module/io/gzip_reader.py
-nerdd_module/io/inchi_reader.py
-nerdd_module/io/list_reader.py
-nerdd_module/io/mol_reader.py
-nerdd_module/io/reader.py
-nerdd_module/io/reader_registry.py
-nerdd_module/io/sdf_reader.py
-nerdd_module/io/sdf_writer.py
-nerdd_module/io/smiles_reader.py
-nerdd_module/io/string_reader.py
-nerdd_module/io/tar_reader.py
-nerdd_module/io/writer.py
-nerdd_module/io/writer_registry.py
-nerdd_module/io/zip_reader.py
+nerdd_module/input/__init__.py
+nerdd_module/input/depth_first_explorer.py
+nerdd_module/input/explorer.py
+nerdd_module/input/file_reader.py
+nerdd_module/input/gzip_reader.py
+nerdd_module/input/inchi_reader.py
+nerdd_module/input/list_reader.py
+nerdd_module/input/mol_reader.py
+nerdd_module/input/reader.py
+nerdd_module/input/reader_registry.py
+nerdd_module/input/sdf_reader.py
+nerdd_module/input/smiles_reader.py
+nerdd_module/input/string_reader.py
+nerdd_module/input/tar_reader.py
+nerdd_module/input/zip_reader.py
+nerdd_module/output/__init__.py
+nerdd_module/output/csv_writer.py
+nerdd_module/output/sdf_writer.py
+nerdd_module/output/writer.py
+nerdd_module/output/writer_registry.py
 nerdd_module/polyfills/__init__.py
 nerdd_module/polyfills/files.py
 nerdd_module/polyfills/get_entry_points.py
+nerdd_module/polyfills/version.py
 nerdd_module/preprocessing/__init__.py
 nerdd_module/preprocessing/check_valid_smiles.py
 nerdd_module/preprocessing/chembl_structure_pipeline.py
 nerdd_module/preprocessing/empty_pipeline.py
 nerdd_module/preprocessing/filter_by_element.py
 nerdd_module/preprocessing/filter_by_weight.py
 nerdd_module/preprocessing/pipeline.py
 nerdd_module/preprocessing/registry.py
 nerdd_module/preprocessing/remove_stereochemistry.py
+nerdd_module/preprocessing/sanitize.py
 nerdd_module/preprocessing/step.py
 nerdd_module/tests/__init__.py
 nerdd_module/tests/checks.py
 nerdd_module/tests/predictions.py
 nerdd_module/tests/representations.py
 tests/__init__.py
 tests/conftest.py
```

### Comparing `nerdd-module-0.2.5/setup.py` & `nerdd_module-0.2.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,19 +12,19 @@
     pass
 
 # rdkit 2022.3.3 is the oldest (reasonable) version
 rdkit_requirement = ["rdkit>=2022.3.3"] if not rdkit_installed else []
 
 setup(
     name="nerdd-module",
-    version="0.2.5",
+    version="0.2.6",
     maintainer="Steffen Hirte",
     maintainer_email="steffen.hirte@univie.ac.at",
     packages=find_packages(),
-    url="https://github.com/molinfo-vienna/nerdd-module.git",
+    url="https://github.com/molinfo-vienna/nerdd-module",
     description="Base package to create NERDD modules",
     license="BSD 3-Clause License",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     install_requires=rdkit_requirement
     + [
         "pandas>=1.2.1",
@@ -32,20 +32,27 @@
         "filetype~=1.2.0",
         "rich-click>=1.7.1",
         "stringcase>=1.2.0",
         "decorator>=5.1.1",
         # install importlib-resources and importlib-metadata for old Python versions
         "importlib-resources>=5; python_version<'3.10'",
         "importlib-metadata>=4.6; python_version<'3.10'",
-        # note: version 1.0.0 of chembl_structure_pipeline is not available on pypi,
-        # but it could potentially be installed from github
-        "chembl_structure_pipeline>=1.0.0",
     ],
     extras_require={
-        "dev": [],
+        "dev": [
+            "black",
+            "isort",
+        ],
+        "csp": [
+            # note: version 1.0.0 of chembl_structure_pipeline is not available on pypi
+            # BUT: maybe it was already installed in the current environment manually
+            # other note: chembl_structure_pipeline *always* installs a recent version
+            #   of rdkit
+            "chembl_structure_pipeline>=1.0.0"
+        ],
         "test": [
             "pytest",
             "pytest-sugar",
             "pytest-cov",
             "pytest-asyncio",
             "pytest-bdd",
             "pytest-mock",
```

### Comparing `nerdd-module-0.2.5/tests/models/AtomicMassModel.py` & `nerdd_module-0.2.6/tests/models/AtomicMassModel.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.5/tests/models/MolWeightModel.py` & `nerdd_module-0.2.6/tests/models/MolWeightModelWithExplicitMols.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 import pandas as pd
 from nerdd_module import AbstractModel
+from nerdd_module.preprocessing import Sanitize
 from rdkit.Chem.Descriptors import MolWt
 
-__all__ = ["MolWeightModel"]
+__all__ = ["MolWeightModelWithExplicitMols"]
 
 
-class MolWeightModel(AbstractModel):
-    def __init__(self, preprocessing_pipeline="chembl_structure_pipeline", **kwargs):
+class MolWeightModelWithExplicitMols(AbstractModel):
+    def __init__(self, preprocessing_pipeline=[Sanitize()], **kwargs):
         super().__init__(preprocessing_pipeline, **kwargs)
 
     def _predict_mols(self, mols, multiplier):
         return pd.DataFrame(
-            {
-                "weight": [MolWt(m) * multiplier for m in mols],
-            }
+            {"mol": mols, "weight": [MolWt(m) * multiplier for m in mols]}
         )
 
     def _get_config(self):
         return {
-            "name": "mol_weight_model",
+            "name": "mol_weight_model_with_explicit_mols",
             "job_parameters": [
                 {"name": "multiplier", "type": "float"},
             ],
             "result_properties": [
                 {"name": "weight", "type": "float"},
             ],
         }
```

### Comparing `nerdd-module-0.2.5/tests/models/MolWeightModelWithExplicitMolIds.py` & `nerdd_module-0.2.6/tests/models/MolWeightModelWithExplicitMolIds.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import pandas as pd
 from nerdd_module import AbstractModel
+from nerdd_module.preprocessing import Sanitize
 from rdkit.Chem.Descriptors import MolWt
 
 __all__ = ["MolWeightModelWithExplicitMolIds"]
 
 
 class MolWeightModelWithExplicitMolIds(AbstractModel):
-    def __init__(self, preprocessing_pipeline="chembl_structure_pipeline", **kwargs):
+    def __init__(self, preprocessing_pipeline=[Sanitize()], **kwargs):
         super().__init__(preprocessing_pipeline, **kwargs)
 
     def _predict_mols(self, mols, multiplier):
         return pd.DataFrame(
             {
                 "mol_id": [int(m.GetProp("_Name")) for m in mols],
                 "weight": [MolWt(m) * multiplier for m in mols],
```

### Comparing `nerdd-module-0.2.5/tests/steps/checks.py` & `nerdd_module-0.2.6/tests/steps/checks.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.5/tests/steps/predictors.py` & `nerdd_module-0.2.6/tests/steps/predictors.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.5/tests/test_atom_property_prediction.py` & `nerdd_module-0.2.6/tests/test_atom_property_prediction.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.5/tests/test_molecule_property_prediction.py` & `nerdd_module-0.2.6/tests/test_molecule_property_prediction.py`

 * *Files identical despite different names*

### Comparing `nerdd-module-0.2.5/tests/test_reading_formats.py` & `nerdd_module-0.2.6/tests/test_reading_formats.py`

 * *Files identical despite different names*

