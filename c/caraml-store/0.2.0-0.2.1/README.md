# Comparing `tmp/caraml-store-0.2.0.tar.gz` & `tmp/caraml-store-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/caraml-store-0.2.0.tar", last modified: Fri May 17 07:22:07 2024, max compression
+gzip compressed data, was "dist/caraml-store-0.2.1.tar", last modified: Tue May 28 06:40:35 2024, max compression
```

## Comparing `caraml-store-0.2.0.tar` & `caraml-store-0.2.1.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:22:07.000000 caraml-store-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-17 07:22:07.000000 caraml-store-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 07:21:57.000000 caraml-store-0.2.0/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:22:07.000000 caraml-store-0.2.0/caraml_store.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-17 07:22:07.000000 caraml-store-0.2.0/caraml_store.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-05-17 07:22:07.000000 caraml-store-0.2.0/caraml_store.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 07:22:07.000000 caraml-store-0.2.0/caraml_store.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-17 07:22:07.000000 caraml-store-0.2.0/caraml_store.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-17 07:22:07.000000 caraml-store-0.2.0/caraml_store.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:22:07.000000 caraml-store-0.2.0/feast/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-17 07:21:57.000000 caraml-store-0.2.0/feast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15446 2024-05-17 07:21:57.000000 caraml-store-0.2.0/feast/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:22:07.000000 caraml-store-0.2.0/feast/core/
--rw-r--r--   0 runner    (1001) docker     (127)    12810 2024-05-17 07:21:57.000000 caraml-store-0.2.0/feast/core/CoreService_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    11452 2024-05-17 07:21:57.000000 caraml-store-0.2.0/feast/core/CoreService_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    30397 2024-05-17 07:21:57.000000 caraml-store-0.2.0/feast/core/CoreService_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-05-17 07:21:57.000000 caraml-store-0.2.0/feast/core/DataFormat_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-17 07:21:57.000000 caraml-store-0.2.0/feast/core/DataFormat_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-17 07:21:57.000000 caraml-store-0.2.0/feast/core/DataFormat_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-05-17 07:21:57.000000 caraml-store-0.2.0/feast/core/DataSource_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-17 07:21:57.000000 caraml-store-0.2.0/feast/core/DataSource_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-17 07:21:57.000000 caraml-store-0.2.0/feast/core/DataSource_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-17 07:21:57.000000 caraml-store-0.2.0/feast/core/Entity_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-05-17 07:21:57.000000 caraml-store-0.2.0/feast/core/Entity_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-17 07:21:57.000000 caraml-store-0.2.0/feast/core/Entity_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-05-17 07:21:57.000000 caraml-store-0.2.0/feast/core/FeatureTable_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-05-17 07:21:57.000000 caraml-store-0.2.0/feast/core/FeatureTable_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-17 07:21:57.000000 caraml-store-0.2.0/feast/core/FeatureTable_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-17 07:21:57.000000 caraml-store-0.2.0/feast/core/Feature_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-17 07:21:57.000000 caraml-store-0.2.0/feast/core/Feature_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-17 07:21:57.000000 caraml-store-0.2.0/feast/core/Feature_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-17 07:21:57.000000 caraml-store-0.2.0/feast/core/OnlineStore_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-17 07:21:57.000000 caraml-store-0.2.0/feast/core/OnlineStore_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-17 07:21:57.000000 caraml-store-0.2.0/feast/core/OnlineStore_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-17 07:21:57.000000 caraml-store-0.2.0/feast/core/SparkOverride_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-17 07:21:57.000000 caraml-store-0.2.0/feast/core/SparkOverride_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-17 07:21:57.000000 caraml-store-0.2.0/feast/core/SparkOverride_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 07:21:57.000000 caraml-store-0.2.0/feast/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-05-17 07:21:57.000000 caraml-store-0.2.0/feast/data_format.py
--rw-r--r--   0 runner    (1001) docker     (127)    10381 2024-05-17 07:21:57.000000 caraml-store-0.2.0/feast/data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     7745 2024-05-17 07:21:57.000000 caraml-store-0.2.0/feast/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-17 07:21:57.000000 caraml-store-0.2.0/feast/feature.py
--rw-r--r--   0 runner    (1001) docker     (127)    12703 2024-05-17 07:21:57.000000 caraml-store-0.2.0/feast/feature_table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:22:07.000000 caraml-store-0.2.0/feast/gcp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 07:21:57.000000 caraml-store-0.2.0/feast/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-17 07:21:57.000000 caraml-store-0.2.0/feast/gcp/staging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:22:07.000000 caraml-store-0.2.0/feast/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 07:21:57.000000 caraml-store-0.2.0/feast/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-17 07:21:57.000000 caraml-store-0.2.0/feast/loaders/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-05-17 07:21:57.000000 caraml-store-0.2.0/feast/online_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-05-17 07:21:57.000000 caraml-store-0.2.0/feast/online_store.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:22:07.000000 caraml-store-0.2.0/feast/serving/
--rw-r--r--   0 runner    (1001) docker     (127)     6618 2024-05-17 07:21:57.000000 caraml-store-0.2.0/feast/serving/ServingService_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-05-17 07:21:57.000000 caraml-store-0.2.0/feast/serving/ServingService_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6476 2024-05-17 07:21:57.000000 caraml-store-0.2.0/feast/serving/ServingService_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 07:21:57.000000 caraml-store-0.2.0/feast/serving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:22:07.000000 caraml-store-0.2.0/feast/types/
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-17 07:21:57.000000 caraml-store-0.2.0/feast/types/Field_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-17 07:21:57.000000 caraml-store-0.2.0/feast/types/Field_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-17 07:21:57.000000 caraml-store-0.2.0/feast/types/Field_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-05-17 07:21:57.000000 caraml-store-0.2.0/feast/types/Value_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-05-17 07:21:57.000000 caraml-store-0.2.0/feast/types/Value_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-17 07:21:57.000000 caraml-store-0.2.0/feast/types/Value_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 07:21:57.000000 caraml-store-0.2.0/feast/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-17 07:21:57.000000 caraml-store-0.2.0/feast/value_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:22:07.000000 caraml-store-0.2.0/feast_spark/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 07:21:57.000000 caraml-store-0.2.0/feast_spark/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:22:07.000000 caraml-store-0.2.0/feast_spark/api/
--rw-r--r--   0 runner    (1001) docker     (127)    10628 2024-05-17 07:21:57.000000 caraml-store-0.2.0/feast_spark/api/JobService_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    11210 2024-05-17 07:21:57.000000 caraml-store-0.2.0/feast_spark/api/JobService_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    19353 2024-05-17 07:21:57.000000 caraml-store-0.2.0/feast_spark/api/JobService_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 07:21:57.000000 caraml-store-0.2.0/feast_spark/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-17 07:21:57.000000 caraml-store-0.2.0/requirements-build.txt
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-17 07:21:57.000000 caraml-store-0.2.0/requirements-ci.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 07:22:07.000000 caraml-store-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-17 07:21:57.000000 caraml-store-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:22:07.000000 caraml-store-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 07:21:57.000000 caraml-store-0.2.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:22:07.000000 caraml-store-0.2.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-17 07:21:57.000000 caraml-store-0.2.0/tests/data/test_feature_table.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-05-17 07:21:57.000000 caraml-store-0.2.0/tests/test_model_protobuf_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:22:07.000000 caraml-store-0.2.0/utils/
--rwxr-xr-x   0 runner    (1001) docker     (127)      936 2024-05-17 07:21:57.000000 caraml-store-0.2.0/utils/compile_protos.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:35.000000 caraml-store-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-28 06:40:35.000000 caraml-store-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:26.000000 caraml-store-0.2.1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:35.000000 caraml-store-0.2.1/caraml_store.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-28 06:40:35.000000 caraml-store-0.2.1/caraml_store.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-05-28 06:40:35.000000 caraml-store-0.2.1/caraml_store.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 06:40:35.000000 caraml-store-0.2.1/caraml_store.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-28 06:40:35.000000 caraml-store-0.2.1/caraml_store.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-28 06:40:35.000000 caraml-store-0.2.1/caraml_store.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:35.000000 caraml-store-0.2.1/feast/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-28 06:40:26.000000 caraml-store-0.2.1/feast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15960 2024-05-28 06:40:26.000000 caraml-store-0.2.1/feast/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:35.000000 caraml-store-0.2.1/feast/core/
+-rw-r--r--   0 runner    (1001) docker     (127)    12810 2024-05-28 06:40:26.000000 caraml-store-0.2.1/feast/core/CoreService_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11452 2024-05-28 06:40:26.000000 caraml-store-0.2.1/feast/core/CoreService_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    30397 2024-05-28 06:40:26.000000 caraml-store-0.2.1/feast/core/CoreService_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-05-28 06:40:26.000000 caraml-store-0.2.1/feast/core/DataFormat_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-28 06:40:26.000000 caraml-store-0.2.1/feast/core/DataFormat_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-28 06:40:26.000000 caraml-store-0.2.1/feast/core/DataFormat_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-05-28 06:40:26.000000 caraml-store-0.2.1/feast/core/DataSource_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-28 06:40:26.000000 caraml-store-0.2.1/feast/core/DataSource_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-28 06:40:26.000000 caraml-store-0.2.1/feast/core/DataSource_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-28 06:40:26.000000 caraml-store-0.2.1/feast/core/Entity_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-05-28 06:40:26.000000 caraml-store-0.2.1/feast/core/Entity_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-28 06:40:26.000000 caraml-store-0.2.1/feast/core/Entity_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-05-28 06:40:26.000000 caraml-store-0.2.1/feast/core/FeatureTable_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-05-28 06:40:26.000000 caraml-store-0.2.1/feast/core/FeatureTable_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-28 06:40:26.000000 caraml-store-0.2.1/feast/core/FeatureTable_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-28 06:40:26.000000 caraml-store-0.2.1/feast/core/Feature_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-28 06:40:26.000000 caraml-store-0.2.1/feast/core/Feature_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-28 06:40:26.000000 caraml-store-0.2.1/feast/core/Feature_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-28 06:40:26.000000 caraml-store-0.2.1/feast/core/OnlineStore_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-28 06:40:26.000000 caraml-store-0.2.1/feast/core/OnlineStore_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-28 06:40:26.000000 caraml-store-0.2.1/feast/core/OnlineStore_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-28 06:40:26.000000 caraml-store-0.2.1/feast/core/SparkOverride_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-28 06:40:26.000000 caraml-store-0.2.1/feast/core/SparkOverride_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-28 06:40:26.000000 caraml-store-0.2.1/feast/core/SparkOverride_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:26.000000 caraml-store-0.2.1/feast/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-05-28 06:40:26.000000 caraml-store-0.2.1/feast/data_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10381 2024-05-28 06:40:26.000000 caraml-store-0.2.1/feast/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7745 2024-05-28 06:40:26.000000 caraml-store-0.2.1/feast/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-28 06:40:26.000000 caraml-store-0.2.1/feast/feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12703 2024-05-28 06:40:26.000000 caraml-store-0.2.1/feast/feature_table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:35.000000 caraml-store-0.2.1/feast/gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:26.000000 caraml-store-0.2.1/feast/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-28 06:40:26.000000 caraml-store-0.2.1/feast/gcp/staging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:35.000000 caraml-store-0.2.1/feast/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:26.000000 caraml-store-0.2.1/feast/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-28 06:40:26.000000 caraml-store-0.2.1/feast/loaders/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-05-28 06:40:26.000000 caraml-store-0.2.1/feast/online_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-05-28 06:40:26.000000 caraml-store-0.2.1/feast/online_store.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:35.000000 caraml-store-0.2.1/feast/serving/
+-rw-r--r--   0 runner    (1001) docker     (127)     6618 2024-05-28 06:40:26.000000 caraml-store-0.2.1/feast/serving/ServingService_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-05-28 06:40:26.000000 caraml-store-0.2.1/feast/serving/ServingService_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6476 2024-05-28 06:40:26.000000 caraml-store-0.2.1/feast/serving/ServingService_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:26.000000 caraml-store-0.2.1/feast/serving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:35.000000 caraml-store-0.2.1/feast/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-28 06:40:26.000000 caraml-store-0.2.1/feast/types/Field_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-28 06:40:26.000000 caraml-store-0.2.1/feast/types/Field_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-28 06:40:26.000000 caraml-store-0.2.1/feast/types/Field_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-05-28 06:40:26.000000 caraml-store-0.2.1/feast/types/Value_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-05-28 06:40:26.000000 caraml-store-0.2.1/feast/types/Value_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-28 06:40:26.000000 caraml-store-0.2.1/feast/types/Value_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:26.000000 caraml-store-0.2.1/feast/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-28 06:40:26.000000 caraml-store-0.2.1/feast/value_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:35.000000 caraml-store-0.2.1/feast_spark/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:26.000000 caraml-store-0.2.1/feast_spark/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:35.000000 caraml-store-0.2.1/feast_spark/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    11029 2024-05-28 06:40:26.000000 caraml-store-0.2.1/feast_spark/api/JobService_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11509 2024-05-28 06:40:26.000000 caraml-store-0.2.1/feast_spark/api/JobService_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    21062 2024-05-28 06:40:26.000000 caraml-store-0.2.1/feast_spark/api/JobService_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:26.000000 caraml-store-0.2.1/feast_spark/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-28 06:40:26.000000 caraml-store-0.2.1/requirements-build.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-28 06:40:26.000000 caraml-store-0.2.1/requirements-ci.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 06:40:35.000000 caraml-store-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-28 06:40:26.000000 caraml-store-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:35.000000 caraml-store-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:26.000000 caraml-store-0.2.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:35.000000 caraml-store-0.2.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-28 06:40:26.000000 caraml-store-0.2.1/tests/data/test_feature_table.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-05-28 06:40:26.000000 caraml-store-0.2.1/tests/test_model_protobuf_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:35.000000 caraml-store-0.2.1/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      936 2024-05-28 06:40:26.000000 caraml-store-0.2.1/utils/compile_protos.sh
```

### Comparing `caraml-store-0.2.0/caraml_store.egg-info/SOURCES.txt` & `caraml-store-0.2.1/caraml_store.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `caraml-store-0.2.0/feast/client.py` & `caraml-store-0.2.1/feast/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 from feast_spark.api.JobService_pb2 import (
     StartOfflineToOnlineIngestionJobRequest,
     StartOfflineToOnlineIngestionJobResponse,
     GetHistoricalFeaturesRequest,
     GetHistoricalFeaturesResponse,
     GetJobRequest,
     ListJobsRequest,
+    CancelJobRequest,
+    UnscheduleJobRequest,
     Job,
     ScheduleOfflineToOnlineIngestionJobRequest, ScheduledJob, ListScheduledJobsRequest, StartStreamIngestionJobResponse,
     StartStreamIngestionJobRequest, JobType, INVALID_JOB,
 )
 from feast_spark.api.JobService_pb2_grpc import JobServiceStub
 
 
@@ -423,7 +425,25 @@
         Delete Feature Table
         Args:
             feature_table: feature table name
             project: project name
         """
         request = DeleteFeatureTableRequest(name=feature_table, project=project)
         self._core_service.DeleteFeatureTable(request)
+
+    def cancel_job(self, job_id: str):
+        """
+        Cancel job
+        Args:
+            job_id: spark job id
+        """
+        request = CancelJobRequest(job_id=job_id)
+        self._job_service.CancelJob(request)
+
+    def unschedule_job(self, job_id: str):
+        """
+        Unschedule job
+        Args:
+            job_id: spark job id
+        """
+        request = UnscheduleJobRequest(job_id=job_id)
+        self._job_service.UnscheduleJob(request)
```

### Comparing `caraml-store-0.2.0/feast/core/CoreService_pb2.py` & `caraml-store-0.2.1/feast/core/CoreService_pb2.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.2.0/feast/core/CoreService_pb2.pyi` & `caraml-store-0.2.1/feast/core/CoreService_pb2.pyi`

 * *Files identical despite different names*

### Comparing `caraml-store-0.2.0/feast/core/CoreService_pb2_grpc.py` & `caraml-store-0.2.1/feast/core/CoreService_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.2.0/feast/core/DataFormat_pb2.py` & `caraml-store-0.2.1/feast/core/DataFormat_pb2.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.2.0/feast/core/DataFormat_pb2.pyi` & `caraml-store-0.2.1/feast/core/DataFormat_pb2.pyi`

 * *Files identical despite different names*

### Comparing `caraml-store-0.2.0/feast/core/DataSource_pb2.py` & `caraml-store-0.2.1/feast/core/DataSource_pb2.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.2.0/feast/core/DataSource_pb2.pyi` & `caraml-store-0.2.1/feast/core/DataSource_pb2.pyi`

 * *Files identical despite different names*

### Comparing `caraml-store-0.2.0/feast/core/Entity_pb2.py` & `caraml-store-0.2.1/feast/core/Entity_pb2.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.2.0/feast/core/Entity_pb2.pyi` & `caraml-store-0.2.1/feast/core/Entity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `caraml-store-0.2.0/feast/core/FeatureTable_pb2.py` & `caraml-store-0.2.1/feast/core/FeatureTable_pb2.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.2.0/feast/core/FeatureTable_pb2.pyi` & `caraml-store-0.2.1/feast/core/FeatureTable_pb2.pyi`

 * *Files identical despite different names*

### Comparing `caraml-store-0.2.0/feast/core/Feature_pb2.py` & `caraml-store-0.2.1/feast/core/Feature_pb2.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.2.0/feast/core/Feature_pb2.pyi` & `caraml-store-0.2.1/feast/core/Feature_pb2.pyi`

 * *Files identical despite different names*

### Comparing `caraml-store-0.2.0/feast/core/OnlineStore_pb2.py` & `caraml-store-0.2.1/feast/core/OnlineStore_pb2.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.2.0/feast/core/OnlineStore_pb2.pyi` & `caraml-store-0.2.1/feast/core/OnlineStore_pb2.pyi`

 * *Files identical despite different names*

### Comparing `caraml-store-0.2.0/feast/core/SparkOverride_pb2.py` & `caraml-store-0.2.1/feast/core/SparkOverride_pb2.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.2.0/feast/core/SparkOverride_pb2.pyi` & `caraml-store-0.2.1/feast/core/SparkOverride_pb2.pyi`

 * *Files identical despite different names*

### Comparing `caraml-store-0.2.0/feast/data_format.py` & `caraml-store-0.2.1/feast/data_format.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.2.0/feast/data_source.py` & `caraml-store-0.2.1/feast/data_source.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.2.0/feast/entity.py` & `caraml-store-0.2.1/feast/entity.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.2.0/feast/feature.py` & `caraml-store-0.2.1/feast/feature.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.2.0/feast/feature_table.py` & `caraml-store-0.2.1/feast/feature_table.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.2.0/feast/gcp/staging.py` & `caraml-store-0.2.1/feast/gcp/staging.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.2.0/feast/loaders/file.py` & `caraml-store-0.2.1/feast/loaders/file.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.2.0/feast/online_response.py` & `caraml-store-0.2.1/feast/online_response.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.2.0/feast/online_store.py` & `caraml-store-0.2.1/feast/online_store.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.2.0/feast/serving/ServingService_pb2.py` & `caraml-store-0.2.1/feast/serving/ServingService_pb2.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.2.0/feast/serving/ServingService_pb2.pyi` & `caraml-store-0.2.1/feast/serving/ServingService_pb2.pyi`

 * *Files identical despite different names*

### Comparing `caraml-store-0.2.0/feast/serving/ServingService_pb2_grpc.py` & `caraml-store-0.2.1/feast/serving/ServingService_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.2.0/feast/types/Field_pb2.py` & `caraml-store-0.2.1/feast/types/Field_pb2.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.2.0/feast/types/Field_pb2.pyi` & `caraml-store-0.2.1/feast/types/Field_pb2.pyi`

 * *Files identical despite different names*

### Comparing `caraml-store-0.2.0/feast/types/Value_pb2.py` & `caraml-store-0.2.1/feast/types/Value_pb2.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.2.0/feast/types/Value_pb2.pyi` & `caraml-store-0.2.1/feast/types/Value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `caraml-store-0.2.0/feast_spark/api/JobService_pb2.py` & `caraml-store-0.2.1/feast_spark/api/JobService_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,26 +11,26 @@
 _sym_db = _symbol_database.Default()
 
 
 from feast.core import DataSource_pb2 as feast_dot_core_dot_DataSource__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n feast_spark/api/JobService.proto\x12\x0f\x66\x65\x61st_spark.api\x1a\x1b\x66\x65\x61st/core/DataSource.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\xab\x01\n\x0cScheduledJob\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1d\n\ntable_name\x18\x02 \x01(\tR\ttableName\x12\x18\n\x07project\x18\x03 \x01(\tR\x07project\x12-\n\x12ingestion_timespan\x18\x04 \x01(\x05R\x11ingestionTimespan\x12#\n\rcron_schedule\x18\x05 \x01(\tR\x0c\x63ronSchedule\"\xc0\x05\n\x03Job\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12,\n\x04type\x18\x02 \x01(\x0e\x32\x18.feast_spark.api.JobTypeR\x04type\x12\x32\n\x06status\x18\x03 \x01(\x0e\x32\x1a.feast_spark.api.JobStatusR\x06status\x12\x12\n\x04hash\x18\x04 \x01(\tR\x04hash\x12\x39\n\nstart_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tstartTime\x12\x45\n\tretrieval\x18\x06 \x01(\x0b\x32%.feast_spark.api.Job.RetrievalJobMetaH\x00R\tretrieval\x12S\n\x0f\x62\x61tch_ingestion\x18\x07 \x01(\x0b\x32(.feast_spark.api.Job.OfflineToOnlineMetaH\x00R\x0e\x62\x61tchIngestion\x12T\n\x10stream_ingestion\x18\x08 \x01(\x0b\x32\'.feast_spark.api.Job.StreamToOnlineMetaH\x00R\x0fstreamIngestion\x12\x17\n\x07log_uri\x18\t \x01(\tR\x06logUri\x12#\n\rerror_message\x18\n \x01(\tR\x0c\x65rrorMessage\x12\x18\n\x07project\x18\x0b \x01(\tR\x07project\x1a;\n\x10RetrievalJobMeta\x12\'\n\x0foutput_location\x18\x01 \x01(\tR\x0eoutputLocation\x1a\x34\n\x13OfflineToOnlineMeta\x12\x1d\n\ntable_name\x18\x01 \x01(\tR\ttableName\x1a\x33\n\x12StreamToOnlineMeta\x12\x1d\n\ntable_name\x18\x01 \x01(\tR\ttableNameB\x06\n\x04meta\"\xfd\x01\n\'StartOfflineToOnlineIngestionJobRequest\x12\x18\n\x07project\x18\x01 \x01(\tR\x07project\x12\x1d\n\ntable_name\x18\x02 \x01(\tR\ttableName\x12\x39\n\nstart_date\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tstartDate\x12\x35\n\x08\x65nd_date\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x07\x65ndDate\x12\'\n\x0f\x64\x65lta_ingestion\x18\x05 \x01(\x08R\x0e\x64\x65ltaIngestion\"\xb4\x01\n(StartOfflineToOnlineIngestionJobResponse\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12@\n\x0ejob_start_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0cjobStartTime\x12\x1d\n\ntable_name\x18\x03 \x01(\tR\ttableName\x12\x17\n\x07log_uri\x18\x04 \x01(\tR\x06logUri\"Y\n\x1eStartStreamIngestionJobRequest\x12\x18\n\x07project\x18\x01 \x01(\tR\x07project\x12\x1d\n\ntable_name\x18\x02 \x01(\tR\ttableName\"1\n\x1fStartStreamIngestionJobResponse\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\"\xb9\x01\n*ScheduleOfflineToOnlineIngestionJobRequest\x12\x18\n\x07project\x18\x01 \x01(\tR\x07project\x12\x1d\n\ntable_name\x18\x02 \x01(\tR\ttableName\x12-\n\x12ingestion_timespan\x18\x03 \x01(\x05R\x11ingestionTimespan\x12#\n\rcron_schedule\x18\x04 \x01(\tR\x0c\x63ronSchedule\"-\n+ScheduleOfflineToOnlineIngestionJobResponse\"g\n,UnscheduleOfflineToOnlineIngestionJobRequest\x12\x18\n\x07project\x18\x01 \x01(\tR\x07project\x12\x1d\n\ntable_name\x18\x02 \x01(\tR\ttableName\"/\n-UnscheduleOfflineToOnlineIngestionJobResponse\"\xe6\x01\n\x1cGetHistoricalFeaturesRequest\x12!\n\x0c\x66\x65\x61ture_refs\x18\x01 \x03(\tR\x0b\x66\x65\x61tureRefs\x12;\n\rentity_source\x18\x02 \x01(\x0b\x32\x16.feast.core.DataSourceR\x0c\x65ntitySource\x12\x18\n\x07project\x18\x03 \x01(\tR\x07project\x12\'\n\x0foutput_location\x18\x04 \x01(\tR\x0eoutputLocation\x12#\n\routput_format\x18\x05 \x01(\tR\x0coutputFormat\"\xb2\x01\n\x1dGetHistoricalFeaturesResponse\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12&\n\x0foutput_file_uri\x18\x02 \x01(\tR\routputFileUri\x12@\n\x0ejob_start_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0cjobStartTime\x12\x17\n\x07log_uri\x18\x04 \x01(\tR\x06logUri\"\xa7\x01\n\x0fListJobsRequest\x12-\n\x12include_terminated\x18\x01 \x01(\x08R\x11includeTerminated\x12\x1d\n\ntable_name\x18\x02 \x01(\tR\ttableName\x12\x18\n\x07project\x18\x03 \x01(\tR\x07project\x12,\n\x04type\x18\x04 \x01(\x0e\x32\x18.feast_spark.api.JobTypeR\x04type\"S\n\x18ListScheduledJobsRequest\x12\x18\n\x07project\x18\x01 \x01(\tR\x07project\x12\x1d\n\ntable_name\x18\x02 \x01(\tR\ttableName\"<\n\x10ListJobsResponse\x12(\n\x04jobs\x18\x01 \x03(\x0b\x32\x14.feast_spark.api.JobR\x04jobs\"N\n\x19ListScheduledJobsResponse\x12\x31\n\x04jobs\x18\x01 \x03(\x0b\x32\x1d.feast_spark.api.ScheduledJobR\x04jobs\"&\n\rGetJobRequest\x12\x15\n\x06job_id\x18\x01 \x01(\tR\x05jobId\"8\n\x0eGetJobResponse\x12&\n\x03job\x18\x01 \x01(\x0b\x32\x14.feast_spark.api.JobR\x03job\")\n\x10\x43\x61ncelJobRequest\x12\x15\n\x06job_id\x18\x01 \x01(\tR\x05jobId\"\x13\n\x11\x43\x61ncelJobResponse\"T\n\x17GetHealthMetricsRequest\x12\x18\n\x07project\x18\x01 \x01(\tR\x07project\x12\x1f\n\x0btable_names\x18\x02 \x03(\tR\ntableNames\"J\n\x18GetHealthMetricsResponse\x12\x16\n\x06passed\x18\x01 \x03(\tR\x06passed\x12\x16\n\x06\x66\x61iled\x18\x02 \x03(\tR\x06\x66\x61iled*`\n\x07JobType\x12\x0f\n\x0bINVALID_JOB\x10\x00\x12\x17\n\x13\x42\x41TCH_INGESTION_JOB\x10\x01\x12\x18\n\x14STREAM_INGESTION_JOB\x10\x02\x12\x11\n\rRETRIEVAL_JOB\x10\x04*~\n\tJobStatus\x12\x16\n\x12JOB_STATUS_INVALID\x10\x00\x12\x16\n\x12JOB_STATUS_PENDING\x10\x01\x12\x16\n\x12JOB_STATUS_RUNNING\x10\x02\x12\x13\n\x0fJOB_STATUS_DONE\x10\x03\x12\x14\n\x10JOB_STATUS_ERROR\x10\x04\x32\xad\t\n\nJobService\x12\x97\x01\n StartOfflineToOnlineIngestionJob\x12\x38.feast_spark.api.StartOfflineToOnlineIngestionJobRequest\x1a\x39.feast_spark.api.StartOfflineToOnlineIngestionJobResponse\x12|\n\x17StartStreamIngestionJob\x12/.feast_spark.api.StartStreamIngestionJobRequest\x1a\x30.feast_spark.api.StartStreamIngestionJobResponse\x12\xa0\x01\n#ScheduleOfflineToOnlineIngestionJob\x12;.feast_spark.api.ScheduleOfflineToOnlineIngestionJobRequest\x1a<.feast_spark.api.ScheduleOfflineToOnlineIngestionJobResponse\x12\xa6\x01\n%UnscheduleOfflineToOnlineIngestionJob\x12=.feast_spark.api.UnscheduleOfflineToOnlineIngestionJobRequest\x1a>.feast_spark.api.UnscheduleOfflineToOnlineIngestionJobResponse\x12v\n\x15GetHistoricalFeatures\x12-.feast_spark.api.GetHistoricalFeaturesRequest\x1a..feast_spark.api.GetHistoricalFeaturesResponse\x12O\n\x08ListJobs\x12 .feast_spark.api.ListJobsRequest\x1a!.feast_spark.api.ListJobsResponse\x12j\n\x11ListScheduledJobs\x12).feast_spark.api.ListScheduledJobsRequest\x1a*.feast_spark.api.ListScheduledJobsResponse\x12R\n\tCancelJob\x12!.feast_spark.api.CancelJobRequest\x1a\".feast_spark.api.CancelJobResponse\x12I\n\x06GetJob\x12\x1e.feast_spark.api.GetJobRequest\x1a\x1f.feast_spark.api.GetJobResponse\x12g\n\x10GetHealthMetrics\x12(.feast_spark.api.GetHealthMetricsRequest\x1a).feast_spark.api.GetHealthMetricsResponseB\x86\x01\n$dev.caraml.store.protobuf.jobserviceB\x0fJobServiceProtoZMgithub.com/caraml-dev/caraml-store/caraml-store-sdk/go/protos/feast_spark/apib\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n feast_spark/api/JobService.proto\x12\x0f\x66\x65\x61st_spark.api\x1a\x1b\x66\x65\x61st/core/DataSource.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\xab\x01\n\x0cScheduledJob\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1d\n\ntable_name\x18\x02 \x01(\tR\ttableName\x12\x18\n\x07project\x18\x03 \x01(\tR\x07project\x12-\n\x12ingestion_timespan\x18\x04 \x01(\x05R\x11ingestionTimespan\x12#\n\rcron_schedule\x18\x05 \x01(\tR\x0c\x63ronSchedule\"\xc0\x05\n\x03Job\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12,\n\x04type\x18\x02 \x01(\x0e\x32\x18.feast_spark.api.JobTypeR\x04type\x12\x32\n\x06status\x18\x03 \x01(\x0e\x32\x1a.feast_spark.api.JobStatusR\x06status\x12\x12\n\x04hash\x18\x04 \x01(\tR\x04hash\x12\x39\n\nstart_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tstartTime\x12\x45\n\tretrieval\x18\x06 \x01(\x0b\x32%.feast_spark.api.Job.RetrievalJobMetaH\x00R\tretrieval\x12S\n\x0f\x62\x61tch_ingestion\x18\x07 \x01(\x0b\x32(.feast_spark.api.Job.OfflineToOnlineMetaH\x00R\x0e\x62\x61tchIngestion\x12T\n\x10stream_ingestion\x18\x08 \x01(\x0b\x32\'.feast_spark.api.Job.StreamToOnlineMetaH\x00R\x0fstreamIngestion\x12\x17\n\x07log_uri\x18\t \x01(\tR\x06logUri\x12#\n\rerror_message\x18\n \x01(\tR\x0c\x65rrorMessage\x12\x18\n\x07project\x18\x0b \x01(\tR\x07project\x1a;\n\x10RetrievalJobMeta\x12\'\n\x0foutput_location\x18\x01 \x01(\tR\x0eoutputLocation\x1a\x34\n\x13OfflineToOnlineMeta\x12\x1d\n\ntable_name\x18\x01 \x01(\tR\ttableName\x1a\x33\n\x12StreamToOnlineMeta\x12\x1d\n\ntable_name\x18\x01 \x01(\tR\ttableNameB\x06\n\x04meta\"\xfd\x01\n\'StartOfflineToOnlineIngestionJobRequest\x12\x18\n\x07project\x18\x01 \x01(\tR\x07project\x12\x1d\n\ntable_name\x18\x02 \x01(\tR\ttableName\x12\x39\n\nstart_date\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tstartDate\x12\x35\n\x08\x65nd_date\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x07\x65ndDate\x12\'\n\x0f\x64\x65lta_ingestion\x18\x05 \x01(\x08R\x0e\x64\x65ltaIngestion\"\xb4\x01\n(StartOfflineToOnlineIngestionJobResponse\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12@\n\x0ejob_start_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0cjobStartTime\x12\x1d\n\ntable_name\x18\x03 \x01(\tR\ttableName\x12\x17\n\x07log_uri\x18\x04 \x01(\tR\x06logUri\"Y\n\x1eStartStreamIngestionJobRequest\x12\x18\n\x07project\x18\x01 \x01(\tR\x07project\x12\x1d\n\ntable_name\x18\x02 \x01(\tR\ttableName\"1\n\x1fStartStreamIngestionJobResponse\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\"\xb9\x01\n*ScheduleOfflineToOnlineIngestionJobRequest\x12\x18\n\x07project\x18\x01 \x01(\tR\x07project\x12\x1d\n\ntable_name\x18\x02 \x01(\tR\ttableName\x12-\n\x12ingestion_timespan\x18\x03 \x01(\x05R\x11ingestionTimespan\x12#\n\rcron_schedule\x18\x04 \x01(\tR\x0c\x63ronSchedule\"-\n+ScheduleOfflineToOnlineIngestionJobResponse\"g\n,UnscheduleOfflineToOnlineIngestionJobRequest\x12\x18\n\x07project\x18\x01 \x01(\tR\x07project\x12\x1d\n\ntable_name\x18\x02 \x01(\tR\ttableName\"/\n-UnscheduleOfflineToOnlineIngestionJobResponse\"\xe6\x01\n\x1cGetHistoricalFeaturesRequest\x12!\n\x0c\x66\x65\x61ture_refs\x18\x01 \x03(\tR\x0b\x66\x65\x61tureRefs\x12;\n\rentity_source\x18\x02 \x01(\x0b\x32\x16.feast.core.DataSourceR\x0c\x65ntitySource\x12\x18\n\x07project\x18\x03 \x01(\tR\x07project\x12\'\n\x0foutput_location\x18\x04 \x01(\tR\x0eoutputLocation\x12#\n\routput_format\x18\x05 \x01(\tR\x0coutputFormat\"\xb2\x01\n\x1dGetHistoricalFeaturesResponse\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12&\n\x0foutput_file_uri\x18\x02 \x01(\tR\routputFileUri\x12@\n\x0ejob_start_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0cjobStartTime\x12\x17\n\x07log_uri\x18\x04 \x01(\tR\x06logUri\"\xa7\x01\n\x0fListJobsRequest\x12-\n\x12include_terminated\x18\x01 \x01(\x08R\x11includeTerminated\x12\x1d\n\ntable_name\x18\x02 \x01(\tR\ttableName\x12\x18\n\x07project\x18\x03 \x01(\tR\x07project\x12,\n\x04type\x18\x04 \x01(\x0e\x32\x18.feast_spark.api.JobTypeR\x04type\"S\n\x18ListScheduledJobsRequest\x12\x18\n\x07project\x18\x01 \x01(\tR\x07project\x12\x1d\n\ntable_name\x18\x02 \x01(\tR\ttableName\"<\n\x10ListJobsResponse\x12(\n\x04jobs\x18\x01 \x03(\x0b\x32\x14.feast_spark.api.JobR\x04jobs\"N\n\x19ListScheduledJobsResponse\x12\x31\n\x04jobs\x18\x01 \x03(\x0b\x32\x1d.feast_spark.api.ScheduledJobR\x04jobs\"&\n\rGetJobRequest\x12\x15\n\x06job_id\x18\x01 \x01(\tR\x05jobId\"8\n\x0eGetJobResponse\x12&\n\x03job\x18\x01 \x01(\x0b\x32\x14.feast_spark.api.JobR\x03job\")\n\x10\x43\x61ncelJobRequest\x12\x15\n\x06job_id\x18\x01 \x01(\tR\x05jobId\"\x13\n\x11\x43\x61ncelJobResponse\"-\n\x14UnscheduleJobRequest\x12\x15\n\x06job_id\x18\x01 \x01(\tR\x05jobId\"\x17\n\x15UnscheduleJobResponse\"T\n\x17GetHealthMetricsRequest\x12\x18\n\x07project\x18\x01 \x01(\tR\x07project\x12\x1f\n\x0btable_names\x18\x02 \x03(\tR\ntableNames\"J\n\x18GetHealthMetricsResponse\x12\x16\n\x06passed\x18\x01 \x03(\tR\x06passed\x12\x16\n\x06\x66\x61iled\x18\x02 \x03(\tR\x06\x66\x61iled*`\n\x07JobType\x12\x0f\n\x0bINVALID_JOB\x10\x00\x12\x17\n\x13\x42\x41TCH_INGESTION_JOB\x10\x01\x12\x18\n\x14STREAM_INGESTION_JOB\x10\x02\x12\x11\n\rRETRIEVAL_JOB\x10\x04*~\n\tJobStatus\x12\x16\n\x12JOB_STATUS_INVALID\x10\x00\x12\x16\n\x12JOB_STATUS_PENDING\x10\x01\x12\x16\n\x12JOB_STATUS_RUNNING\x10\x02\x12\x13\n\x0fJOB_STATUS_DONE\x10\x03\x12\x14\n\x10JOB_STATUS_ERROR\x10\x04\x32\x8d\n\n\nJobService\x12\x97\x01\n StartOfflineToOnlineIngestionJob\x12\x38.feast_spark.api.StartOfflineToOnlineIngestionJobRequest\x1a\x39.feast_spark.api.StartOfflineToOnlineIngestionJobResponse\x12|\n\x17StartStreamIngestionJob\x12/.feast_spark.api.StartStreamIngestionJobRequest\x1a\x30.feast_spark.api.StartStreamIngestionJobResponse\x12\xa0\x01\n#ScheduleOfflineToOnlineIngestionJob\x12;.feast_spark.api.ScheduleOfflineToOnlineIngestionJobRequest\x1a<.feast_spark.api.ScheduleOfflineToOnlineIngestionJobResponse\x12\xa6\x01\n%UnscheduleOfflineToOnlineIngestionJob\x12=.feast_spark.api.UnscheduleOfflineToOnlineIngestionJobRequest\x1a>.feast_spark.api.UnscheduleOfflineToOnlineIngestionJobResponse\x12v\n\x15GetHistoricalFeatures\x12-.feast_spark.api.GetHistoricalFeaturesRequest\x1a..feast_spark.api.GetHistoricalFeaturesResponse\x12O\n\x08ListJobs\x12 .feast_spark.api.ListJobsRequest\x1a!.feast_spark.api.ListJobsResponse\x12j\n\x11ListScheduledJobs\x12).feast_spark.api.ListScheduledJobsRequest\x1a*.feast_spark.api.ListScheduledJobsResponse\x12R\n\tCancelJob\x12!.feast_spark.api.CancelJobRequest\x1a\".feast_spark.api.CancelJobResponse\x12^\n\rUnscheduleJob\x12%.feast_spark.api.UnscheduleJobRequest\x1a&.feast_spark.api.UnscheduleJobResponse\x12I\n\x06GetJob\x12\x1e.feast_spark.api.GetJobRequest\x1a\x1f.feast_spark.api.GetJobResponse\x12g\n\x10GetHealthMetrics\x12(.feast_spark.api.GetHealthMetricsRequest\x1a).feast_spark.api.GetHealthMetricsResponseB\x86\x01\n$dev.caraml.store.protobuf.jobserviceB\x0fJobServiceProtoZMgithub.com/caraml-dev/caraml-store/caraml-store-sdk/go/protos/feast_spark/apib\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'feast_spark.api.JobService_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n$dev.caraml.store.protobuf.jobserviceB\017JobServiceProtoZMgithub.com/caraml-dev/caraml-store/caraml-store-sdk/go/protos/feast_spark/api'
-  _JOBTYPE._serialized_start=3101
-  _JOBTYPE._serialized_end=3197
-  _JOBSTATUS._serialized_start=3199
-  _JOBSTATUS._serialized_end=3325
+  _JOBTYPE._serialized_start=3173
+  _JOBTYPE._serialized_end=3269
+  _JOBSTATUS._serialized_start=3271
+  _JOBSTATUS._serialized_end=3397
   _SCHEDULEDJOB._serialized_start=116
   _SCHEDULEDJOB._serialized_end=287
   _JOB._serialized_start=290
   _JOB._serialized_end=994
   _JOB_RETRIEVALJOBMETA._serialized_start=820
   _JOB_RETRIEVALJOBMETA._serialized_end=879
   _JOB_OFFLINETOONLINEMETA._serialized_start=881
@@ -69,14 +69,18 @@
   _GETJOBREQUEST._serialized_end=2815
   _GETJOBRESPONSE._serialized_start=2817
   _GETJOBRESPONSE._serialized_end=2873
   _CANCELJOBREQUEST._serialized_start=2875
   _CANCELJOBREQUEST._serialized_end=2916
   _CANCELJOBRESPONSE._serialized_start=2918
   _CANCELJOBRESPONSE._serialized_end=2937
-  _GETHEALTHMETRICSREQUEST._serialized_start=2939
-  _GETHEALTHMETRICSREQUEST._serialized_end=3023
-  _GETHEALTHMETRICSRESPONSE._serialized_start=3025
-  _GETHEALTHMETRICSRESPONSE._serialized_end=3099
-  _JOBSERVICE._serialized_start=3328
-  _JOBSERVICE._serialized_end=4525
+  _UNSCHEDULEJOBREQUEST._serialized_start=2939
+  _UNSCHEDULEJOBREQUEST._serialized_end=2984
+  _UNSCHEDULEJOBRESPONSE._serialized_start=2986
+  _UNSCHEDULEJOBRESPONSE._serialized_end=3009
+  _GETHEALTHMETRICSREQUEST._serialized_start=3011
+  _GETHEALTHMETRICSREQUEST._serialized_end=3095
+  _GETHEALTHMETRICSRESPONSE._serialized_start=3097
+  _GETHEALTHMETRICSRESPONSE._serialized_end=3171
+  _JOBSERVICE._serialized_start=3400
+  _JOBSERVICE._serialized_end=4693
 # @@protoc_insertion_point(module_scope)
```

### Comparing `caraml-store-0.2.0/feast_spark/api/JobService_pb2.pyi` & `caraml-store-0.2.1/feast_spark/api/JobService_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -220,14 +220,24 @@
 
 class StartStreamIngestionJobResponse(_message.Message):
     __slots__ = ["id"]
     ID_FIELD_NUMBER: _ClassVar[int]
     id: str
     def __init__(self, id: _Optional[str] = ...) -> None: ...
 
+class UnscheduleJobRequest(_message.Message):
+    __slots__ = ["job_id"]
+    JOB_ID_FIELD_NUMBER: _ClassVar[int]
+    job_id: str
+    def __init__(self, job_id: _Optional[str] = ...) -> None: ...
+
+class UnscheduleJobResponse(_message.Message):
+    __slots__ = []
+    def __init__(self) -> None: ...
+
 class UnscheduleOfflineToOnlineIngestionJobRequest(_message.Message):
     __slots__ = ["project", "table_name"]
     PROJECT_FIELD_NUMBER: _ClassVar[int]
     TABLE_NAME_FIELD_NUMBER: _ClassVar[int]
     project: str
     table_name: str
     def __init__(self, project: _Optional[str] = ..., table_name: _Optional[str] = ...) -> None: ...
```

### Comparing `caraml-store-0.2.0/feast_spark/api/JobService_pb2_grpc.py` & `caraml-store-0.2.1/feast_spark/api/JobService_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,19 @@
                 response_deserializer=feast__spark_dot_api_dot_JobService__pb2.ListScheduledJobsResponse.FromString,
                 )
         self.CancelJob = channel.unary_unary(
                 '/feast_spark.api.JobService/CancelJob',
                 request_serializer=feast__spark_dot_api_dot_JobService__pb2.CancelJobRequest.SerializeToString,
                 response_deserializer=feast__spark_dot_api_dot_JobService__pb2.CancelJobResponse.FromString,
                 )
+        self.UnscheduleJob = channel.unary_unary(
+                '/feast_spark.api.JobService/UnscheduleJob',
+                request_serializer=feast__spark_dot_api_dot_JobService__pb2.UnscheduleJobRequest.SerializeToString,
+                response_deserializer=feast__spark_dot_api_dot_JobService__pb2.UnscheduleJobResponse.FromString,
+                )
         self.GetJob = channel.unary_unary(
                 '/feast_spark.api.JobService/GetJob',
                 request_serializer=feast__spark_dot_api_dot_JobService__pb2.GetJobRequest.SerializeToString,
                 response_deserializer=feast__spark_dot_api_dot_JobService__pb2.GetJobResponse.FromString,
                 )
         self.GetHealthMetrics = channel.unary_unary(
                 '/feast_spark.api.JobService/GetHealthMetrics',
@@ -121,14 +126,21 @@
     def CancelJob(self, request, context):
         """Cancel a single job
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def UnscheduleJob(self, request, context):
+        """Unschedule a job
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def GetJob(self, request, context):
         """Get details of a single job
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
@@ -178,14 +190,19 @@
                     response_serializer=feast__spark_dot_api_dot_JobService__pb2.ListScheduledJobsResponse.SerializeToString,
             ),
             'CancelJob': grpc.unary_unary_rpc_method_handler(
                     servicer.CancelJob,
                     request_deserializer=feast__spark_dot_api_dot_JobService__pb2.CancelJobRequest.FromString,
                     response_serializer=feast__spark_dot_api_dot_JobService__pb2.CancelJobResponse.SerializeToString,
             ),
+            'UnscheduleJob': grpc.unary_unary_rpc_method_handler(
+                    servicer.UnscheduleJob,
+                    request_deserializer=feast__spark_dot_api_dot_JobService__pb2.UnscheduleJobRequest.FromString,
+                    response_serializer=feast__spark_dot_api_dot_JobService__pb2.UnscheduleJobResponse.SerializeToString,
+            ),
             'GetJob': grpc.unary_unary_rpc_method_handler(
                     servicer.GetJob,
                     request_deserializer=feast__spark_dot_api_dot_JobService__pb2.GetJobRequest.FromString,
                     response_serializer=feast__spark_dot_api_dot_JobService__pb2.GetJobResponse.SerializeToString,
             ),
             'GetHealthMetrics': grpc.unary_unary_rpc_method_handler(
                     servicer.GetHealthMetrics,
@@ -335,14 +352,31 @@
         return grpc.experimental.unary_unary(request, target, '/feast_spark.api.JobService/CancelJob',
             feast__spark_dot_api_dot_JobService__pb2.CancelJobRequest.SerializeToString,
             feast__spark_dot_api_dot_JobService__pb2.CancelJobResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def UnscheduleJob(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/feast_spark.api.JobService/UnscheduleJob',
+            feast__spark_dot_api_dot_JobService__pb2.UnscheduleJobRequest.SerializeToString,
+            feast__spark_dot_api_dot_JobService__pb2.UnscheduleJobResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def GetJob(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
```

### Comparing `caraml-store-0.2.0/setup.py` & `caraml-store-0.2.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     name=NAME,
     author=AUTHOR,
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     python_requires=REQUIRES_PYTHON,
     url=URL,
     packages=find_packages(exclude=("tests",)),
+    include_package_data=True,
     install_requires=REQUIRED,
     extras_require=EXTRA_REQUIRED,
     use_scm_version={"root": "../..", "relative_to": __file__, "tag_regex": TAG_REGEX},
     setup_requires=["setuptools_scm"],
     # https://stackoverflow.com/questions/28509965/setuptools-development-requirements
     # Install dev requirements with: pip install -e .[dev]
     license="Apache",
```

### Comparing `caraml-store-0.2.0/tests/data/test_feature_table.yaml` & `caraml-store-0.2.1/tests/data/test_feature_table.yaml`

 * *Files identical despite different names*

### Comparing `caraml-store-0.2.0/tests/test_model_protobuf_conversion.py` & `caraml-store-0.2.1/tests/test_model_protobuf_conversion.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.2.0/utils/compile_protos.sh` & `caraml-store-0.2.1/utils/compile_protos.sh`

 * *Files identical despite different names*

