# Comparing `tmp/jaqpotpy-1.1.2.tar.gz` & `tmp/jaqpotpy-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaqpotpy-1.1.2.tar", last modified: Mon May 27 14:07:45 2024, max compression
+gzip compressed data, was "jaqpotpy-1.2.0.tar", last modified: Tue May 28 14:17:38 2024, max compression
```

## Comparing `jaqpotpy-1.1.2.tar` & `jaqpotpy-1.2.0.tar`

### file list

```diff
@@ -1,197 +1,197 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:07:45.936234 jaqpotpy-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-05-27 14:07:45.936234 jaqpotpy-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:07:45.904233 jaqpotpy-1.1.2/jaqpotpy/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:07:45.908234 jaqpotpy-1.1.2/jaqpotpy/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/api/algorithms_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/api/chempot_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/api/dataset_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/api/doa_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/api/feature_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4213 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/api/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/api/models_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/api/task_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/base_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:07:45.908234 jaqpotpy-1.1.2/jaqpotpy/cfg/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/cfg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/cfg/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:07:45.908234 jaqpotpy-1.1.2/jaqpotpy/colorlog/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/colorlog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/colorlog/colorlog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/colorlog/escape_codes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/colorlog/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:07:45.912233 jaqpotpy-1.1.2/jaqpotpy/data/
--rw-r--r--   0 runner    (1001) docker     (127)  2077102 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/data/NP_score.pkl.gz
--rw-r--r--   0 runner    (1001) docker     (127)  3848394 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/data/SA_score.pkl.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:07:45.916233 jaqpotpy-1.1.2/jaqpotpy/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/datasets/dataset_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/datasets/image_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    14845 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/datasets/material_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    13972 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/datasets/molecular_datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:07:45.916233 jaqpotpy-1.1.2/jaqpotpy/descriptors/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/descriptors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25776 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/descriptors/base_classes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:07:45.916233 jaqpotpy-1.1.2/jaqpotpy/descriptors/graph/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/descriptors/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9731 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/descriptors/graph/graph_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    38001 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/descriptors/graph/graph_features.py
--rw-r--r--   0 runner    (1001) docker     (127)    14240 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/descriptors/graph/mol_graphs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:07:45.920234 jaqpotpy-1.1.2/jaqpotpy/descriptors/material/
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/descriptors/material/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7771 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/descriptors/material/cgcnn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:07:45.920234 jaqpotpy-1.1.2/jaqpotpy/descriptors/material/datafiles/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/descriptors/material/datafiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28409 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/descriptors/material/datafiles/atom_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/descriptors/material/element_property_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/descriptors/material/elemnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    10549 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/descriptors/material/geometrical.py
--rw-r--r--   0 runner    (1001) docker     (127)     6185 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/descriptors/material/graph_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5867 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/descriptors/material/sine_coulomb_matrix.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:07:45.920234 jaqpotpy-1.1.2/jaqpotpy/descriptors/molecular/
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/descriptors/molecular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9977 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/descriptors/molecular/coulomb_matrices.py
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/descriptors/molecular/maccs_keys_fingerprints.py
--rw-r--r--   0 runner    (1001) docker     (127)    36285 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/descriptors/molecular/molecule_graph_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)    12719 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/descriptors/molecular/molgan.py
--rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/descriptors/molecular/mordred.py
--rw-r--r--   0 runner    (1001) docker     (127)     5917 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/descriptors/molecular/one_hot_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/descriptors/molecular/pub_chem_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (127)     5770 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/descriptors/molecular/rdkit.py
--rw-r--r--   0 runner    (1001) docker     (127)     6830 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/descriptors/molecular/smiles_to_seq.py
--rw-r--r--   0 runner    (1001) docker     (127)    10885 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/descriptors/molecular/smles_to_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     7743 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/descriptors/molecular/topological_fingerprints.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:07:45.920234 jaqpotpy-1.1.2/jaqpotpy/doa/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/doa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10292 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/doa/doa.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:07:45.920234 jaqpotpy-1.1.2/jaqpotpy/docking/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/docking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4813 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/docking/binding_pocket.py
--rw-r--r--   0 runner    (1001) docker     (127)     5564 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/docking/docking.py
--rw-r--r--   0 runner    (1001) docker     (127)    18344 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/docking/pose_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/docking/pose_scoring.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:07:45.924234 jaqpotpy-1.1.2/jaqpotpy/docking/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/docking/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/docking/test/test_binding_pocket.py
--rw-r--r--   0 runner    (1001) docker     (127)    13794 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/docking/test/test_docking.py
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/docking/test/test_docking_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    34521 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/docking/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:07:45.924234 jaqpotpy-1.1.2/jaqpotpy/dto/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/dto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/dto/auth_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/dto/pretrained_requirements.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:07:45.924234 jaqpotpy-1.1.2/jaqpotpy/entities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8455 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/entities/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/entities/chemical_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/entities/dataentry.py
--rw-r--r--   0 runner    (1001) docker     (127)     9479 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/entities/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/entities/doa.py
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/entities/entryid.py
--rw-r--r--   0 runner    (1001) docker     (127)     7050 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/entities/error_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     7965 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/entities/feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     4146 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/entities/featureinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/entities/jaqpot_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/entities/material_models.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/entities/meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     7884 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/entities/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/entities/parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9108 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/entities/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:07:45.928234 jaqpotpy-1.1.2/jaqpotpy/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10729 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/helpers/builders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/helpers/dataset_deserializer.py
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/helpers/doa.py
--rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/helpers/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/helpers/jwt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/helpers/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/helpers/onnx_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:07:45.928234 jaqpotpy-1.1.2/jaqpotpy/helpers/periodic_table/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/helpers/periodic_table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/helpers/periodic_table/base_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/helpers/periodic_table/element.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/helpers/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/helpers/statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/jaqpot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:07:45.928234 jaqpotpy-1.1.2/jaqpotpy/jaqpotpy_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/jaqpotpy_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/jaqpotpy_tests/jaqpotpy_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:07:45.928234 jaqpotpy-1.1.2/jaqpotpy/mappers/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/mappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/mappers/decode.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:07:45.928234 jaqpotpy-1.1.2/jaqpotpy/models/
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19544 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/models/base_classes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:07:45.928234 jaqpotpy-1.1.2/jaqpotpy/models/evaluator/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/models/evaluator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/models/evaluator/evaluator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:07:45.928234 jaqpotpy-1.1.2/jaqpotpy/models/evaluator/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/models/evaluator/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16203 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/models/evaluator/test/test_evaluators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:07:45.932234 jaqpotpy-1.1.2/jaqpotpy/models/generative/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/models/generative/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:07:45.932234 jaqpotpy-1.1.2/jaqpotpy/models/generative/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/models/generative/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23444 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/models/generative/gan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:07:45.932234 jaqpotpy-1.1.2/jaqpotpy/models/generative/models/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/models/generative/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:07:45.932234 jaqpotpy-1.1.2/jaqpotpy/models/generative/models/layers/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/models/generative/models/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7356 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/models/generative/models/layers/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11056 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/models/generative/models/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    14246 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/models/generative/molecular_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/models/generative/vae.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/models/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:07:45.932234 jaqpotpy-1.1.2/jaqpotpy/models/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/models/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/models/preprocessing/preprocesses.py
--rw-r--r--   0 runner    (1001) docker     (127)    10840 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/models/sklearn.py
--rw-r--r--   0 runner    (1001) docker     (127)    19591 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/models/torch.py
--rw-r--r--   0 runner    (1001) docker     (127)    32270 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/models/torch_geometric.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:07:45.932234 jaqpotpy-1.1.2/jaqpotpy/models/torch_models/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/models/torch_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/models/torch_models/torch.py
--rw-r--r--   0 runner    (1001) docker     (127)    30056 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/models/torch_models/torch_geometric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/models/torch_models/torch_vision.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:07:45.932234 jaqpotpy-1.1.2/jaqpotpy/models/trainers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/models/trainers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:07:45.932234 jaqpotpy-1.1.2/jaqpotpy/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/parsers/base_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     9387 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/parsers/mol_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5406 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/parsers/pdb_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/parsers/xyz_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:07:45.932234 jaqpotpy-1.1.2/jaqpotpy/rl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22232 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/rl/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/rl/atom_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/rl/rl_envs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5370 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/rl/spaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:07:45.936234 jaqpotpy-1.1.2/jaqpotpy/simulation_kit/
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/simulation_kit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:07:45.936234 jaqpotpy-1.1.2/jaqpotpy/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12303 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/utils/fragment_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7752 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/utils/geometry_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    18655 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/utils/molecule_feature_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11685 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/utils/pdbqt_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/utils/pytorch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21146 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/utils/rdkit_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5514 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/utils/seeding.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/jaqpotpy/utils/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:07:45.904233 jaqpotpy-1.1.2/jaqpotpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-05-27 14:07:45.000000 jaqpotpy-1.1.2/jaqpotpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-05-27 14:07:45.000000 jaqpotpy-1.1.2/jaqpotpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 14:07:45.000000 jaqpotpy-1.1.2/jaqpotpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 14:07:45.000000 jaqpotpy-1.1.2/jaqpotpy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-27 14:07:45.000000 jaqpotpy-1.1.2/jaqpotpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-27 14:07:45.000000 jaqpotpy-1.1.2/jaqpotpy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:07:45.936234 jaqpotpy-1.1.2/run_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/run_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-27 14:07:40.000000 jaqpotpy-1.1.2/run_tests/run_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 14:07:45.936234 jaqpotpy-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-27 14:07:44.000000 jaqpotpy-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:17:38.512498 jaqpotpy-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-05-28 14:17:38.512498 jaqpotpy-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:17:38.484498 jaqpotpy-1.2.0/jaqpotpy/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:17:38.484498 jaqpotpy-1.2.0/jaqpotpy/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/api/algorithms_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/api/chempot_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/api/dataset_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/api/doa_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/api/feature_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4213 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/api/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/api/models_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/api/task_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/base_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:17:38.484498 jaqpotpy-1.2.0/jaqpotpy/cfg/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/cfg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/cfg/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:17:38.488498 jaqpotpy-1.2.0/jaqpotpy/colorlog/
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/colorlog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/colorlog/colorlog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/colorlog/escape_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/colorlog/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:17:38.488498 jaqpotpy-1.2.0/jaqpotpy/data/
+-rw-r--r--   0 runner    (1001) docker     (127)  2077102 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/data/NP_score.pkl.gz
+-rw-r--r--   0 runner    (1001) docker     (127)  3848394 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/data/SA_score.pkl.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:17:38.496498 jaqpotpy-1.2.0/jaqpotpy/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/datasets/dataset_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/datasets/image_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14845 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/datasets/material_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13972 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/datasets/molecular_datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:17:38.496498 jaqpotpy-1.2.0/jaqpotpy/descriptors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/descriptors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25776 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/descriptors/base_classes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:17:38.496498 jaqpotpy-1.2.0/jaqpotpy/descriptors/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/descriptors/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9731 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/descriptors/graph/graph_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38001 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/descriptors/graph/graph_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14240 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/descriptors/graph/mol_graphs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:17:38.496498 jaqpotpy-1.2.0/jaqpotpy/descriptors/material/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/descriptors/material/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7771 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/descriptors/material/cgcnn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:17:38.496498 jaqpotpy-1.2.0/jaqpotpy/descriptors/material/datafiles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/descriptors/material/datafiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28409 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/descriptors/material/datafiles/atom_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/descriptors/material/element_property_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/descriptors/material/elemnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10549 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/descriptors/material/geometrical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6185 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/descriptors/material/graph_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5867 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/descriptors/material/sine_coulomb_matrix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:17:38.500498 jaqpotpy-1.2.0/jaqpotpy/descriptors/molecular/
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/descriptors/molecular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9977 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/descriptors/molecular/coulomb_matrices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/descriptors/molecular/maccs_keys_fingerprints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36285 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/descriptors/molecular/molecule_graph_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12719 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/descriptors/molecular/molgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/descriptors/molecular/mordred.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5917 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/descriptors/molecular/one_hot_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/descriptors/molecular/pub_chem_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5770 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/descriptors/molecular/rdkit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6830 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/descriptors/molecular/smiles_to_seq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10885 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/descriptors/molecular/smles_to_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7743 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/descriptors/molecular/topological_fingerprints.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:17:38.500498 jaqpotpy-1.2.0/jaqpotpy/doa/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/doa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10292 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/doa/doa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:17:38.500498 jaqpotpy-1.2.0/jaqpotpy/docking/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/docking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4813 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/docking/binding_pocket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5564 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/docking/docking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18344 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/docking/pose_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/docking/pose_scoring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:17:38.500498 jaqpotpy-1.2.0/jaqpotpy/docking/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/docking/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/docking/test/test_binding_pocket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13794 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/docking/test/test_docking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/docking/test/test_docking_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34521 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/docking/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:17:38.500498 jaqpotpy-1.2.0/jaqpotpy/dto/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/dto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/dto/auth_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/dto/pretrained_requirements.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:17:38.504498 jaqpotpy-1.2.0/jaqpotpy/entities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8455 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/entities/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/entities/chemical_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/entities/dataentry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9479 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/entities/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/entities/doa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/entities/entryid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7050 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/entities/error_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7965 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/entities/feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4146 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/entities/featureinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/entities/jaqpot_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/entities/material_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/entities/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7884 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/entities/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/entities/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9108 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/entities/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:17:38.504498 jaqpotpy-1.2.0/jaqpotpy/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10729 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/helpers/builders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/helpers/dataset_deserializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/helpers/doa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/helpers/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/helpers/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/helpers/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/helpers/onnx_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:17:38.504498 jaqpotpy-1.2.0/jaqpotpy/helpers/periodic_table/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/helpers/periodic_table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/helpers/periodic_table/base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/helpers/periodic_table/element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/helpers/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/helpers/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/jaqpot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:17:38.504498 jaqpotpy-1.2.0/jaqpotpy/jaqpotpy_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/jaqpotpy_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/jaqpotpy_tests/jaqpotpy_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:17:38.504498 jaqpotpy-1.2.0/jaqpotpy/mappers/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/mappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/mappers/decode.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:17:38.504498 jaqpotpy-1.2.0/jaqpotpy/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19544 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/models/base_classes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:17:38.504498 jaqpotpy-1.2.0/jaqpotpy/models/evaluator/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/models/evaluator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/models/evaluator/evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:17:38.508498 jaqpotpy-1.2.0/jaqpotpy/models/evaluator/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/models/evaluator/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16203 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/models/evaluator/test/test_evaluators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:17:38.508498 jaqpotpy-1.2.0/jaqpotpy/models/generative/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/models/generative/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:17:38.508498 jaqpotpy-1.2.0/jaqpotpy/models/generative/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/models/generative/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23444 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/models/generative/gan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:17:38.508498 jaqpotpy-1.2.0/jaqpotpy/models/generative/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/models/generative/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:17:38.508498 jaqpotpy-1.2.0/jaqpotpy/models/generative/models/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/models/generative/models/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7356 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/models/generative/models/layers/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11056 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/models/generative/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14246 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/models/generative/molecular_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/models/generative/vae.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/models/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:17:38.508498 jaqpotpy-1.2.0/jaqpotpy/models/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/models/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/models/preprocessing/preprocesses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10840 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/models/sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19591 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/models/torch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32270 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/models/torch_geometric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:17:38.508498 jaqpotpy-1.2.0/jaqpotpy/models/torch_models/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/models/torch_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/models/torch_models/torch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30056 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/models/torch_models/torch_geometric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/models/torch_models/torch_vision.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:17:38.508498 jaqpotpy-1.2.0/jaqpotpy/models/trainers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/models/trainers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:17:38.508498 jaqpotpy-1.2.0/jaqpotpy/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/parsers/base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9387 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/parsers/mol_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5406 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/parsers/pdb_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/parsers/xyz_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:17:38.508498 jaqpotpy-1.2.0/jaqpotpy/rl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22232 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/rl/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/rl/atom_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/rl/rl_envs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5370 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/rl/spaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:17:38.508498 jaqpotpy-1.2.0/jaqpotpy/simulation_kit/
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/simulation_kit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:17:38.512498 jaqpotpy-1.2.0/jaqpotpy/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12303 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/utils/fragment_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7752 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/utils/geometry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18655 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/utils/molecule_feature_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11685 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/utils/pdbqt_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/utils/pytorch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21146 2024-05-28 14:17:31.000000 jaqpotpy-1.2.0/jaqpotpy/utils/rdkit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5514 2024-05-28 14:17:32.000000 jaqpotpy-1.2.0/jaqpotpy/utils/seeding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-28 14:17:32.000000 jaqpotpy-1.2.0/jaqpotpy/utils/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:17:38.484498 jaqpotpy-1.2.0/jaqpotpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-05-28 14:17:38.000000 jaqpotpy-1.2.0/jaqpotpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-05-28 14:17:38.000000 jaqpotpy-1.2.0/jaqpotpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 14:17:38.000000 jaqpotpy-1.2.0/jaqpotpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 14:17:38.000000 jaqpotpy-1.2.0/jaqpotpy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-28 14:17:38.000000 jaqpotpy-1.2.0/jaqpotpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-28 14:17:38.000000 jaqpotpy-1.2.0/jaqpotpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:17:38.512498 jaqpotpy-1.2.0/run_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 14:17:32.000000 jaqpotpy-1.2.0/run_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-28 14:17:32.000000 jaqpotpy-1.2.0/run_tests/run_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 14:17:38.512498 jaqpotpy-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-28 14:17:36.000000 jaqpotpy-1.2.0/setup.py
```

### Comparing `jaqpotpy-1.1.2/LICENSE` & `jaqpotpy-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/PKG-INFO` & `jaqpotpy-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaqpotpy
-Version: 1.1.2
+Version: 1.2.0
 Summary: Standardizing molecular modeling
 Home-page: https://github.com/ntua-unit-of-control-and-informatics/jaqpotpy
 Author: Unit of Process Control and Informatics | National Technical University of Athens
 Author-email: upci.ntua@gmail.com
 License: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `jaqpotpy-1.1.2/README.md` & `jaqpotpy-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/api/algorithms_api.py` & `jaqpotpy-1.2.0/jaqpotpy/api/algorithms_api.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/api/chempot_api.py` & `jaqpotpy-1.2.0/jaqpotpy/api/chempot_api.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/api/dataset_api.py` & `jaqpotpy-1.2.0/jaqpotpy/api/dataset_api.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/api/doa_api.py` & `jaqpotpy-1.2.0/jaqpotpy/api/doa_api.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/api/feature_api.py` & `jaqpotpy-1.2.0/jaqpotpy/api/feature_api.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/api/login.py` & `jaqpotpy-1.2.0/jaqpotpy/api/login.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/api/models_api.py` & `jaqpotpy-1.2.0/jaqpotpy/api/models_api.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/colorlog/__init__.py` & `jaqpotpy-1.2.0/jaqpotpy/colorlog/__init__.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/colorlog/colorlog.py` & `jaqpotpy-1.2.0/jaqpotpy/colorlog/colorlog.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/colorlog/escape_codes.py` & `jaqpotpy-1.2.0/jaqpotpy/colorlog/escape_codes.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/colorlog/logging.py` & `jaqpotpy-1.2.0/jaqpotpy/colorlog/logging.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/data/NP_score.pkl.gz` & `jaqpotpy-1.2.0/jaqpotpy/data/NP_score.pkl.gz`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/data/SA_score.pkl.gz` & `jaqpotpy-1.2.0/jaqpotpy/data/SA_score.pkl.gz`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/datasets/dataset_base.py` & `jaqpotpy-1.2.0/jaqpotpy/datasets/dataset_base.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/datasets/image_datasets.py` & `jaqpotpy-1.2.0/jaqpotpy/datasets/image_datasets.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/datasets/material_datasets.py` & `jaqpotpy-1.2.0/jaqpotpy/datasets/material_datasets.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/datasets/molecular_datasets.py` & `jaqpotpy-1.2.0/jaqpotpy/datasets/molecular_datasets.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/descriptors/__init__.py` & `jaqpotpy-1.2.0/jaqpotpy/descriptors/__init__.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/descriptors/base_classes.py` & `jaqpotpy-1.2.0/jaqpotpy/descriptors/base_classes.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/descriptors/graph/graph_data.py` & `jaqpotpy-1.2.0/jaqpotpy/descriptors/graph/graph_data.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/descriptors/graph/graph_features.py` & `jaqpotpy-1.2.0/jaqpotpy/descriptors/graph/graph_features.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/descriptors/graph/mol_graphs.py` & `jaqpotpy-1.2.0/jaqpotpy/descriptors/graph/mol_graphs.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/descriptors/material/__init__.py` & `jaqpotpy-1.2.0/jaqpotpy/descriptors/material/__init__.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/descriptors/material/cgcnn.py` & `jaqpotpy-1.2.0/jaqpotpy/descriptors/material/cgcnn.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/descriptors/material/datafiles/atom_init.py` & `jaqpotpy-1.2.0/jaqpotpy/descriptors/material/datafiles/atom_init.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/descriptors/material/element_property_fingerprint.py` & `jaqpotpy-1.2.0/jaqpotpy/descriptors/material/element_property_fingerprint.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/descriptors/material/elemnet.py` & `jaqpotpy-1.2.0/jaqpotpy/descriptors/material/elemnet.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/descriptors/material/geometrical.py` & `jaqpotpy-1.2.0/jaqpotpy/descriptors/material/geometrical.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/descriptors/material/graph_data.py` & `jaqpotpy-1.2.0/jaqpotpy/descriptors/material/graph_data.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/descriptors/material/sine_coulomb_matrix.py` & `jaqpotpy-1.2.0/jaqpotpy/descriptors/material/sine_coulomb_matrix.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/descriptors/molecular/__init__.py` & `jaqpotpy-1.2.0/jaqpotpy/descriptors/molecular/__init__.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/descriptors/molecular/coulomb_matrices.py` & `jaqpotpy-1.2.0/jaqpotpy/descriptors/molecular/coulomb_matrices.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/descriptors/molecular/maccs_keys_fingerprints.py` & `jaqpotpy-1.2.0/jaqpotpy/descriptors/molecular/maccs_keys_fingerprints.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/descriptors/molecular/molecule_graph_conv.py` & `jaqpotpy-1.2.0/jaqpotpy/descriptors/molecular/molecule_graph_conv.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/descriptors/molecular/molgan.py` & `jaqpotpy-1.2.0/jaqpotpy/descriptors/molecular/molgan.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/descriptors/molecular/mordred.py` & `jaqpotpy-1.2.0/jaqpotpy/descriptors/molecular/mordred.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/descriptors/molecular/one_hot_sequence.py` & `jaqpotpy-1.2.0/jaqpotpy/descriptors/molecular/one_hot_sequence.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/descriptors/molecular/pub_chem_fingerprint.py` & `jaqpotpy-1.2.0/jaqpotpy/descriptors/molecular/pub_chem_fingerprint.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/descriptors/molecular/rdkit.py` & `jaqpotpy-1.2.0/jaqpotpy/descriptors/molecular/rdkit.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/descriptors/molecular/smiles_to_seq.py` & `jaqpotpy-1.2.0/jaqpotpy/descriptors/molecular/smiles_to_seq.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/descriptors/molecular/smles_to_image.py` & `jaqpotpy-1.2.0/jaqpotpy/descriptors/molecular/smles_to_image.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/descriptors/molecular/topological_fingerprints.py` & `jaqpotpy-1.2.0/jaqpotpy/descriptors/molecular/topological_fingerprints.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/doa/doa.py` & `jaqpotpy-1.2.0/jaqpotpy/doa/doa.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/docking/binding_pocket.py` & `jaqpotpy-1.2.0/jaqpotpy/docking/binding_pocket.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/docking/docking.py` & `jaqpotpy-1.2.0/jaqpotpy/docking/docking.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/docking/pose_generation.py` & `jaqpotpy-1.2.0/jaqpotpy/docking/pose_generation.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/docking/pose_scoring.py` & `jaqpotpy-1.2.0/jaqpotpy/docking/pose_scoring.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/docking/test/test_binding_pocket.py` & `jaqpotpy-1.2.0/jaqpotpy/docking/test/test_binding_pocket.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/docking/test/test_docking.py` & `jaqpotpy-1.2.0/jaqpotpy/docking/test/test_docking.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/docking/test/test_docking_utils.py` & `jaqpotpy-1.2.0/jaqpotpy/docking/test/test_docking_utils.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/docking/utils.py` & `jaqpotpy-1.2.0/jaqpotpy/docking/utils.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/dto/auth_request.py` & `jaqpotpy-1.2.0/jaqpotpy/dto/auth_request.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/dto/pretrained_requirements.py` & `jaqpotpy-1.2.0/jaqpotpy/dto/pretrained_requirements.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/entities/algorithm.py` & `jaqpotpy-1.2.0/jaqpotpy/entities/algorithm.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/entities/chemical_models.py` & `jaqpotpy-1.2.0/jaqpotpy/entities/chemical_models.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/entities/dataentry.py` & `jaqpotpy-1.2.0/jaqpotpy/entities/dataentry.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/entities/dataset.py` & `jaqpotpy-1.2.0/jaqpotpy/entities/dataset.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/entities/entryid.py` & `jaqpotpy-1.2.0/jaqpotpy/entities/entryid.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/entities/error_report.py` & `jaqpotpy-1.2.0/jaqpotpy/entities/error_report.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/entities/feature.py` & `jaqpotpy-1.2.0/jaqpotpy/entities/feature.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/entities/featureinfo.py` & `jaqpotpy-1.2.0/jaqpotpy/entities/featureinfo.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/entities/material_models.py` & `jaqpotpy-1.2.0/jaqpotpy/entities/material_models.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/entities/model.py` & `jaqpotpy-1.2.0/jaqpotpy/entities/model.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/entities/parameter.py` & `jaqpotpy-1.2.0/jaqpotpy/entities/parameter.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/entities/task.py` & `jaqpotpy-1.2.0/jaqpotpy/entities/task.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/helpers/builders.py` & `jaqpotpy-1.2.0/jaqpotpy/helpers/builders.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/helpers/dataset_deserializer.py` & `jaqpotpy-1.2.0/jaqpotpy/helpers/dataset_deserializer.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/helpers/helpers.py` & `jaqpotpy-1.2.0/jaqpotpy/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/helpers/logging.py` & `jaqpotpy-1.2.0/jaqpotpy/helpers/logging.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/helpers/onnx_helpers.py` & `jaqpotpy-1.2.0/jaqpotpy/helpers/onnx_helpers.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/helpers/periodic_table/base_classes.py` & `jaqpotpy-1.2.0/jaqpotpy/helpers/periodic_table/base_classes.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/helpers/periodic_table/element.py` & `jaqpotpy-1.2.0/jaqpotpy/helpers/periodic_table/element.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/helpers/serializer.py` & `jaqpotpy-1.2.0/jaqpotpy/helpers/serializer.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/helpers/statistics.py` & `jaqpotpy-1.2.0/jaqpotpy/helpers/statistics.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/jaqpot.py` & `jaqpotpy-1.2.0/jaqpotpy/jaqpot.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/jaqpotpy_tests/jaqpotpy_test.py` & `jaqpotpy-1.2.0/jaqpotpy/jaqpotpy_tests/jaqpotpy_test.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/mappers/decode.py` & `jaqpotpy-1.2.0/jaqpotpy/mappers/decode.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/models/__init__.py` & `jaqpotpy-1.2.0/jaqpotpy/models/__init__.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/models/base_classes.py` & `jaqpotpy-1.2.0/jaqpotpy/models/base_classes.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/models/evaluator/evaluator.py` & `jaqpotpy-1.2.0/jaqpotpy/models/evaluator/evaluator.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/models/evaluator/test/test_evaluators.py` & `jaqpotpy-1.2.0/jaqpotpy/models/evaluator/test/test_evaluators.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/models/generative/gan.py` & `jaqpotpy-1.2.0/jaqpotpy/models/generative/gan.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/models/generative/models/layers/layers.py` & `jaqpotpy-1.2.0/jaqpotpy/models/generative/models/layers/layers.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/models/generative/models/models.py` & `jaqpotpy-1.2.0/jaqpotpy/models/generative/models/models.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/models/generative/molecular_metrics.py` & `jaqpotpy-1.2.0/jaqpotpy/models/generative/molecular_metrics.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/models/generative/vae.py` & `jaqpotpy-1.2.0/jaqpotpy/models/generative/vae.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/models/models.py` & `jaqpotpy-1.2.0/jaqpotpy/models/models.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/models/preprocessing/preprocesses.py` & `jaqpotpy-1.2.0/jaqpotpy/models/preprocessing/preprocesses.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/models/sklearn.py` & `jaqpotpy-1.2.0/jaqpotpy/models/sklearn.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/models/torch.py` & `jaqpotpy-1.2.0/jaqpotpy/models/torch.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/models/torch_geometric.py` & `jaqpotpy-1.2.0/jaqpotpy/models/torch_geometric.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/models/torch_models/torch.py` & `jaqpotpy-1.2.0/jaqpotpy/models/torch_models/torch.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/models/torch_models/torch_geometric.py` & `jaqpotpy-1.2.0/jaqpotpy/models/torch_models/torch_geometric.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/models/torch_models/torch_vision.py` & `jaqpotpy-1.2.0/jaqpotpy/models/torch_models/torch_vision.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/parsers/base_classes.py` & `jaqpotpy-1.2.0/jaqpotpy/parsers/base_classes.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/parsers/mol_parser.py` & `jaqpotpy-1.2.0/jaqpotpy/parsers/mol_parser.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/parsers/pdb_parser.py` & `jaqpotpy-1.2.0/jaqpotpy/parsers/pdb_parser.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/parsers/xyz_parser.py` & `jaqpotpy-1.2.0/jaqpotpy/parsers/xyz_parser.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/rl/abstract.py` & `jaqpotpy-1.2.0/jaqpotpy/rl/abstract.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/rl/atom_actions.py` & `jaqpotpy-1.2.0/jaqpotpy/rl/atom_actions.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/rl/spaces.py` & `jaqpotpy-1.2.0/jaqpotpy/rl/spaces.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/simulation_kit/__init__.py` & `jaqpotpy-1.2.0/jaqpotpy/simulation_kit/__init__.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/utils/data_utils.py` & `jaqpotpy-1.2.0/jaqpotpy/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/utils/fragment_utils.py` & `jaqpotpy-1.2.0/jaqpotpy/utils/fragment_utils.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/utils/geometry_utils.py` & `jaqpotpy-1.2.0/jaqpotpy/utils/geometry_utils.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/utils/molecule_feature_utils.py` & `jaqpotpy-1.2.0/jaqpotpy/utils/molecule_feature_utils.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/utils/pdbqt_utils.py` & `jaqpotpy-1.2.0/jaqpotpy/utils/pdbqt_utils.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/utils/pytorch_utils.py` & `jaqpotpy-1.2.0/jaqpotpy/utils/pytorch_utils.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/utils/rdkit_utils.py` & `jaqpotpy-1.2.0/jaqpotpy/utils/rdkit_utils.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/utils/seeding.py` & `jaqpotpy-1.2.0/jaqpotpy/utils/seeding.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy/utils/types.py` & `jaqpotpy-1.2.0/jaqpotpy/utils/types.py`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/jaqpotpy.egg-info/PKG-INFO` & `jaqpotpy-1.2.0/jaqpotpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaqpotpy
-Version: 1.1.2
+Version: 1.2.0
 Summary: Standardizing molecular modeling
 Home-page: https://github.com/ntua-unit-of-control-and-informatics/jaqpotpy
 Author: Unit of Process Control and Informatics | National Technical University of Athens
 Author-email: upci.ntua@gmail.com
 License: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `jaqpotpy-1.1.2/jaqpotpy.egg-info/SOURCES.txt` & `jaqpotpy-1.2.0/jaqpotpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jaqpotpy-1.1.2/run_tests/run_tests.py` & `jaqpotpy-1.2.0/run_tests/run_tests.py`

 * *Files identical despite different names*

