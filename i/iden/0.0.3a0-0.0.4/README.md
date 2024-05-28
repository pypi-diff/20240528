# Comparing `tmp/iden-0.0.3a0.tar.gz` & `tmp/iden-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iden-0.0.3a0.tar", max compression
+gzip compressed data, was "iden-0.0.4.tar", max compression
```

## Comparing `iden-0.0.3a0.tar` & `iden-0.0.4.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0     1501 2024-03-17 23:02:36.019436 iden-0.0.3a0/LICENSE
--rw-r--r--   0        0        0     5643 2024-03-17 23:02:36.019436 iden-0.0.3a0/README.md
--rw-r--r--   0        0        0     6445 2024-03-17 23:02:36.023435 iden-0.0.3a0/pyproject.toml
--rw-r--r--   0        0        0       21 2024-03-17 23:02:36.023435 iden-0.0.3a0/src/iden/__init__.py
--rw-r--r--   0        0        0      196 2024-03-17 23:02:36.023435 iden-0.0.3a0/src/iden/constants.py
--rw-r--r--   0        0        0       38 2024-03-17 23:02:36.023435 iden-0.0.3a0/src/iden/data/__init__.py
--rw-r--r--   0        0        0      379 2024-03-17 23:02:36.023435 iden-0.0.3a0/src/iden/data/generator/__init__.py
--rw-r--r--   0        0        0     3002 2024-03-17 23:02:36.023435 iden-0.0.3a0/src/iden/data/generator/base.py
--rw-r--r--   0        0        0     1077 2024-03-17 23:02:36.023435 iden-0.0.3a0/src/iden/data/generator/vanilla.py
--rw-r--r--   0        0        0      326 2024-03-17 23:02:36.023435 iden-0.0.3a0/src/iden/dataset/__init__.py
--rw-r--r--   0        0        0    20422 2024-03-17 23:02:36.023435 iden-0.0.3a0/src/iden/dataset/base.py
--rw-r--r--   0        0        0      482 2024-03-17 23:02:36.023435 iden-0.0.3a0/src/iden/dataset/exceptions.py
--rw-r--r--   0        0        0      426 2024-03-17 23:02:36.023435 iden-0.0.3a0/src/iden/dataset/generator/__init__.py
--rw-r--r--   0        0        0     6365 2024-03-17 23:02:36.023435 iden-0.0.3a0/src/iden/dataset/generator/base.py
--rw-r--r--   0        0        0     3548 2024-03-17 23:02:36.023435 iden-0.0.3a0/src/iden/dataset/generator/vanilla.py
--rw-r--r--   0        0        0      393 2024-03-17 23:02:36.023435 iden-0.0.3a0/src/iden/dataset/loader/__init__.py
--rw-r--r--   0        0        0     5806 2024-03-17 23:02:36.023435 iden-0.0.3a0/src/iden/dataset/loader/base.py
--rw-r--r--   0        0        0     3054 2024-03-17 23:02:36.023435 iden-0.0.3a0/src/iden/dataset/loader/vanilla.py
--rw-r--r--   0        0        0     3333 2024-03-17 23:02:36.023435 iden-0.0.3a0/src/iden/dataset/loading.py
--rw-r--r--   0        0        0    15717 2024-03-17 23:02:36.023435 iden-0.0.3a0/src/iden/dataset/vanilla.py
--rw-r--r--   0        0        0     1218 2024-03-17 23:02:36.023435 iden-0.0.3a0/src/iden/io/__init__.py
--rw-r--r--   0        0        0     4200 2024-03-17 23:02:36.023435 iden-0.0.3a0/src/iden/io/auto.py
--rw-r--r--   0        0        0     9319 2024-03-17 23:02:36.023435 iden-0.0.3a0/src/iden/io/base.py
--rw-r--r--   0        0        0     4216 2024-03-17 23:02:36.023435 iden-0.0.3a0/src/iden/io/json.py
--rw-r--r--   0        0        0     4713 2024-03-17 23:02:36.023435 iden-0.0.3a0/src/iden/io/pickle.py
--rw-r--r--   0        0        0      850 2024-03-17 23:02:36.023435 iden-0.0.3a0/src/iden/io/safetensors/__init__.py
--rw-r--r--   0        0        0     1969 2024-03-17 23:02:36.023435 iden-0.0.3a0/src/iden/io/safetensors/loaders.py
--rw-r--r--   0        0        0     1993 2024-03-17 23:02:36.023435 iden-0.0.3a0/src/iden/io/safetensors/savers.py
--rw-r--r--   0        0        0     4227 2024-03-17 23:02:36.023435 iden-0.0.3a0/src/iden/io/text.py
--rw-r--r--   0        0        0     4455 2024-03-17 23:02:36.023435 iden-0.0.3a0/src/iden/io/torch.py
--rw-r--r--   0        0        0     1811 2024-03-17 23:02:36.023435 iden-0.0.3a0/src/iden/io/utils.py
--rw-r--r--   0        0        0     4609 2024-03-17 23:02:36.023435 iden-0.0.3a0/src/iden/io/yaml.py
--rw-r--r--   0        0        0     1428 2024-03-17 23:02:36.023435 iden-0.0.3a0/src/iden/shard/__init__.py
--rw-r--r--   0        0        0     5429 2024-03-17 23:02:36.023435 iden-0.0.3a0/src/iden/shard/base.py
--rw-r--r--   0        0        0     1438 2024-03-17 23:02:36.023435 iden-0.0.3a0/src/iden/shard/comparators.py
--rw-r--r--   0        0        0    10853 2024-03-17 23:02:36.023435 iden-0.0.3a0/src/iden/shard/dict.py
--rw-r--r--   0        0        0      350 2024-03-17 23:02:36.023435 iden-0.0.3a0/src/iden/shard/exceptions.py
--rw-r--r--   0        0        0     4424 2024-03-17 23:02:36.023435 iden-0.0.3a0/src/iden/shard/file.py
--rw-r--r--   0        0        0     1019 2024-03-17 23:02:36.023435 iden-0.0.3a0/src/iden/shard/generator/__init__.py
--rw-r--r--   0        0        0     4659 2024-03-17 23:02:36.023435 iden-0.0.3a0/src/iden/shard/generator/base.py
--rw-r--r--   0        0        0     2999 2024-03-17 23:02:36.023435 iden-0.0.3a0/src/iden/shard/generator/dict.py
--rw-r--r--   0        0        0     2812 2024-03-17 23:02:36.023435 iden-0.0.3a0/src/iden/shard/generator/file.py
--rw-r--r--   0        0        0     1604 2024-03-17 23:02:36.023435 iden-0.0.3a0/src/iden/shard/generator/json.py
--rw-r--r--   0        0        0     1627 2024-03-17 23:02:36.023435 iden-0.0.3a0/src/iden/shard/generator/pickle.py
--rw-r--r--   0        0        0     4559 2024-03-17 23:02:36.023435 iden-0.0.3a0/src/iden/shard/generator/safetensors.py
--rw-r--r--   0        0        0     1979 2024-03-17 23:02:36.023435 iden-0.0.3a0/src/iden/shard/generator/torch.py
--rw-r--r--   0        0        0     3010 2024-03-17 23:02:36.023435 iden-0.0.3a0/src/iden/shard/generator/tuple.py
--rw-r--r--   0        0        0     1965 2024-03-17 23:02:36.023435 iden-0.0.3a0/src/iden/shard/generator/yaml.py
--rw-r--r--   0        0        0     1177 2024-03-17 23:02:36.023435 iden-0.0.3a0/src/iden/shard/in_memory.py
--rw-r--r--   0        0        0     3451 2024-03-17 23:02:36.023435 iden-0.0.3a0/src/iden/shard/json.py
--rw-r--r--   0        0        0     1000 2024-03-17 23:02:36.023435 iden-0.0.3a0/src/iden/shard/loader/__init__.py
--rw-r--r--   0        0        0     3786 2024-03-17 23:02:36.023435 iden-0.0.3a0/src/iden/shard/loader/base.py
--rw-r--r--   0        0        0     1503 2024-03-17 23:02:36.027435 iden-0.0.3a0/src/iden/shard/loader/dict.py
--rw-r--r--   0        0        0     1039 2024-03-17 23:02:36.027435 iden-0.0.3a0/src/iden/shard/loader/file.py
--rw-r--r--   0        0        0     1027 2024-03-17 23:02:36.027435 iden-0.0.3a0/src/iden/shard/loader/json.py
--rw-r--r--   0        0        0     1053 2024-03-17 23:02:36.027435 iden-0.0.3a0/src/iden/shard/loader/pickle.py
--rw-r--r--   0        0        0     3004 2024-03-17 23:02:36.027435 iden-0.0.3a0/src/iden/shard/loader/safetensors.py
--rw-r--r--   0        0        0     1175 2024-03-17 23:02:36.027435 iden-0.0.3a0/src/iden/shard/loader/torch.py
--rw-r--r--   0        0        0     1456 2024-03-17 23:02:36.027435 iden-0.0.3a0/src/iden/shard/loader/tuple.py
--rw-r--r--   0        0        0     1123 2024-03-17 23:02:36.027435 iden-0.0.3a0/src/iden/shard/loader/yaml.py
--rw-r--r--   0        0        0     1363 2024-03-17 23:02:36.027435 iden-0.0.3a0/src/iden/shard/loading.py
--rw-r--r--   0        0        0     3522 2024-03-17 23:02:36.027435 iden-0.0.3a0/src/iden/shard/pickle.py
--rw-r--r--   0        0        0     8617 2024-03-17 23:02:36.027435 iden-0.0.3a0/src/iden/shard/safetensors.py
--rw-r--r--   0        0        0     4118 2024-03-17 23:02:36.027435 iden-0.0.3a0/src/iden/shard/torch.py
--rw-r--r--   0        0        0     8848 2024-03-17 23:02:36.027435 iden-0.0.3a0/src/iden/shard/tuple.py
--rw-r--r--   0        0        0     4486 2024-03-17 23:02:36.027435 iden-0.0.3a0/src/iden/shard/utils.py
--rw-r--r--   0        0        0     3462 2024-03-17 23:02:36.027435 iden-0.0.3a0/src/iden/shard/yaml.py
--rw-r--r--   0        0        0      214 2024-03-17 23:02:36.027435 iden-0.0.3a0/src/iden/testing/__init__.py
--rw-r--r--   0        0        0      414 2024-03-17 23:02:36.027435 iden-0.0.3a0/src/iden/testing/fixtures.py
--rw-r--r--   0        0        0       38 2024-03-17 23:02:36.027435 iden-0.0.3a0/src/iden/utils/__init__.py
--rw-r--r--   0        0        0      794 2024-03-17 23:02:36.027435 iden-0.0.3a0/src/iden/utils/format.py
--rw-r--r--   0        0        0     3757 2024-03-17 23:02:36.027435 iden-0.0.3a0/src/iden/utils/imports.py
--rw-r--r--   0        0        0      937 2024-03-17 23:02:36.027435 iden-0.0.3a0/src/iden/utils/path.py
--rw-r--r--   0        0        0     1996 2024-03-17 23:02:36.027435 iden-0.0.3a0/src/iden/utils/time.py
--rw-r--r--   0        0        0     7082 1970-01-01 00:00:00.000000 iden-0.0.3a0/PKG-INFO
+-rw-r--r--   0        0        0     1501 2024-05-28 14:16:08.135299 iden-0.0.4/LICENSE
+-rw-r--r--   0        0        0     5796 2024-05-28 14:16:08.135299 iden-0.0.4/README.md
+-rw-r--r--   0        0        0     6569 2024-05-28 14:16:08.135299 iden-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0       21 2024-05-28 14:16:08.135299 iden-0.0.4/src/iden/__init__.py
+-rw-r--r--   0        0        0      196 2024-05-28 14:16:08.135299 iden-0.0.4/src/iden/constants.py
+-rw-r--r--   0        0        0       38 2024-05-28 14:16:08.135299 iden-0.0.4/src/iden/data/__init__.py
+-rw-r--r--   0        0        0      379 2024-05-28 14:16:08.135299 iden-0.0.4/src/iden/data/generator/__init__.py
+-rw-r--r--   0        0        0     3002 2024-05-28 14:16:08.135299 iden-0.0.4/src/iden/data/generator/base.py
+-rw-r--r--   0        0        0     1077 2024-05-28 14:16:08.135299 iden-0.0.4/src/iden/data/generator/vanilla.py
+-rw-r--r--   0        0        0      326 2024-05-28 14:16:08.135299 iden-0.0.4/src/iden/dataset/__init__.py
+-rw-r--r--   0        0        0    20422 2024-05-28 14:16:08.135299 iden-0.0.4/src/iden/dataset/base.py
+-rw-r--r--   0        0        0      482 2024-05-28 14:16:08.135299 iden-0.0.4/src/iden/dataset/exceptions.py
+-rw-r--r--   0        0        0      426 2024-05-28 14:16:08.135299 iden-0.0.4/src/iden/dataset/generator/__init__.py
+-rw-r--r--   0        0        0     6365 2024-05-28 14:16:08.135299 iden-0.0.4/src/iden/dataset/generator/base.py
+-rw-r--r--   0        0        0     3548 2024-05-28 14:16:08.135299 iden-0.0.4/src/iden/dataset/generator/vanilla.py
+-rw-r--r--   0        0        0      393 2024-05-28 14:16:08.135299 iden-0.0.4/src/iden/dataset/loader/__init__.py
+-rw-r--r--   0        0        0     5806 2024-05-28 14:16:08.135299 iden-0.0.4/src/iden/dataset/loader/base.py
+-rw-r--r--   0        0        0     3054 2024-05-28 14:16:08.135299 iden-0.0.4/src/iden/dataset/loader/vanilla.py
+-rw-r--r--   0        0        0     3333 2024-05-28 14:16:08.135299 iden-0.0.4/src/iden/dataset/loading.py
+-rw-r--r--   0        0        0    15717 2024-05-28 14:16:08.135299 iden-0.0.4/src/iden/dataset/vanilla.py
+-rw-r--r--   0        0        0     1218 2024-05-28 14:16:08.135299 iden-0.0.4/src/iden/io/__init__.py
+-rw-r--r--   0        0        0     4200 2024-05-28 14:16:08.135299 iden-0.0.4/src/iden/io/auto.py
+-rw-r--r--   0        0        0     9319 2024-05-28 14:16:08.135299 iden-0.0.4/src/iden/io/base.py
+-rw-r--r--   0        0        0     4216 2024-05-28 14:16:08.135299 iden-0.0.4/src/iden/io/json.py
+-rw-r--r--   0        0        0     4713 2024-05-28 14:16:08.135299 iden-0.0.4/src/iden/io/pickle.py
+-rw-r--r--   0        0        0      850 2024-05-28 14:16:08.139299 iden-0.0.4/src/iden/io/safetensors/__init__.py
+-rw-r--r--   0        0        0     1969 2024-05-28 14:16:08.139299 iden-0.0.4/src/iden/io/safetensors/loaders.py
+-rw-r--r--   0        0        0     1993 2024-05-28 14:16:08.139299 iden-0.0.4/src/iden/io/safetensors/savers.py
+-rw-r--r--   0        0        0     4227 2024-05-28 14:16:08.139299 iden-0.0.4/src/iden/io/text.py
+-rw-r--r--   0        0        0     4455 2024-05-28 14:16:08.139299 iden-0.0.4/src/iden/io/torch.py
+-rw-r--r--   0        0        0     1811 2024-05-28 14:16:08.139299 iden-0.0.4/src/iden/io/utils.py
+-rw-r--r--   0        0        0     4609 2024-05-28 14:16:08.139299 iden-0.0.4/src/iden/io/yaml.py
+-rw-r--r--   0        0        0     1428 2024-05-28 14:16:08.139299 iden-0.0.4/src/iden/shard/__init__.py
+-rw-r--r--   0        0        0     5429 2024-05-28 14:16:08.139299 iden-0.0.4/src/iden/shard/base.py
+-rw-r--r--   0        0        0     1438 2024-05-28 14:16:08.139299 iden-0.0.4/src/iden/shard/comparators.py
+-rw-r--r--   0        0        0    10853 2024-05-28 14:16:08.139299 iden-0.0.4/src/iden/shard/dict.py
+-rw-r--r--   0        0        0      350 2024-05-28 14:16:08.139299 iden-0.0.4/src/iden/shard/exceptions.py
+-rw-r--r--   0        0        0     4424 2024-05-28 14:16:08.139299 iden-0.0.4/src/iden/shard/file.py
+-rw-r--r--   0        0        0     1019 2024-05-28 14:16:08.139299 iden-0.0.4/src/iden/shard/generator/__init__.py
+-rw-r--r--   0        0        0     4659 2024-05-28 14:16:08.139299 iden-0.0.4/src/iden/shard/generator/base.py
+-rw-r--r--   0        0        0     2999 2024-05-28 14:16:08.139299 iden-0.0.4/src/iden/shard/generator/dict.py
+-rw-r--r--   0        0        0     2812 2024-05-28 14:16:08.139299 iden-0.0.4/src/iden/shard/generator/file.py
+-rw-r--r--   0        0        0     1604 2024-05-28 14:16:08.139299 iden-0.0.4/src/iden/shard/generator/json.py
+-rw-r--r--   0        0        0     1627 2024-05-28 14:16:08.139299 iden-0.0.4/src/iden/shard/generator/pickle.py
+-rw-r--r--   0        0        0     4559 2024-05-28 14:16:08.139299 iden-0.0.4/src/iden/shard/generator/safetensors.py
+-rw-r--r--   0        0        0     1979 2024-05-28 14:16:08.139299 iden-0.0.4/src/iden/shard/generator/torch.py
+-rw-r--r--   0        0        0     3010 2024-05-28 14:16:08.139299 iden-0.0.4/src/iden/shard/generator/tuple.py
+-rw-r--r--   0        0        0     1965 2024-05-28 14:16:08.139299 iden-0.0.4/src/iden/shard/generator/yaml.py
+-rw-r--r--   0        0        0     1177 2024-05-28 14:16:08.139299 iden-0.0.4/src/iden/shard/in_memory.py
+-rw-r--r--   0        0        0     3451 2024-05-28 14:16:08.139299 iden-0.0.4/src/iden/shard/json.py
+-rw-r--r--   0        0        0     1000 2024-05-28 14:16:08.139299 iden-0.0.4/src/iden/shard/loader/__init__.py
+-rw-r--r--   0        0        0     3786 2024-05-28 14:16:08.139299 iden-0.0.4/src/iden/shard/loader/base.py
+-rw-r--r--   0        0        0     1503 2024-05-28 14:16:08.139299 iden-0.0.4/src/iden/shard/loader/dict.py
+-rw-r--r--   0        0        0     1039 2024-05-28 14:16:08.139299 iden-0.0.4/src/iden/shard/loader/file.py
+-rw-r--r--   0        0        0     1027 2024-05-28 14:16:08.139299 iden-0.0.4/src/iden/shard/loader/json.py
+-rw-r--r--   0        0        0     1053 2024-05-28 14:16:08.139299 iden-0.0.4/src/iden/shard/loader/pickle.py
+-rw-r--r--   0        0        0     3004 2024-05-28 14:16:08.139299 iden-0.0.4/src/iden/shard/loader/safetensors.py
+-rw-r--r--   0        0        0     1175 2024-05-28 14:16:08.139299 iden-0.0.4/src/iden/shard/loader/torch.py
+-rw-r--r--   0        0        0     1456 2024-05-28 14:16:08.139299 iden-0.0.4/src/iden/shard/loader/tuple.py
+-rw-r--r--   0        0        0     1123 2024-05-28 14:16:08.139299 iden-0.0.4/src/iden/shard/loader/yaml.py
+-rw-r--r--   0        0        0     1363 2024-05-28 14:16:08.139299 iden-0.0.4/src/iden/shard/loading.py
+-rw-r--r--   0        0        0     3522 2024-05-28 14:16:08.139299 iden-0.0.4/src/iden/shard/pickle.py
+-rw-r--r--   0        0        0     8617 2024-05-28 14:16:08.139299 iden-0.0.4/src/iden/shard/safetensors.py
+-rw-r--r--   0        0        0     4118 2024-05-28 14:16:08.139299 iden-0.0.4/src/iden/shard/torch.py
+-rw-r--r--   0        0        0     8848 2024-05-28 14:16:08.139299 iden-0.0.4/src/iden/shard/tuple.py
+-rw-r--r--   0        0        0     4486 2024-05-28 14:16:08.139299 iden-0.0.4/src/iden/shard/utils.py
+-rw-r--r--   0        0        0     3462 2024-05-28 14:16:08.139299 iden-0.0.4/src/iden/shard/yaml.py
+-rw-r--r--   0        0        0      215 2024-05-28 14:16:08.139299 iden-0.0.4/src/iden/testing/__init__.py
+-rw-r--r--   0        0        0      414 2024-05-28 14:16:08.139299 iden-0.0.4/src/iden/testing/fixtures.py
+-rw-r--r--   0        0        0       38 2024-05-28 14:16:08.139299 iden-0.0.4/src/iden/utils/__init__.py
+-rw-r--r--   0        0        0      794 2024-05-28 14:16:08.139299 iden-0.0.4/src/iden/utils/format.py
+-rw-r--r--   0        0        0     3757 2024-05-28 14:16:08.139299 iden-0.0.4/src/iden/utils/imports.py
+-rw-r--r--   0        0        0      937 2024-05-28 14:16:08.139299 iden-0.0.4/src/iden/utils/path.py
+-rw-r--r--   0        0        0     1996 2024-05-28 14:16:08.139299 iden-0.0.4/src/iden/utils/time.py
+-rw-r--r--   0        0        0     7350 1970-01-01 00:00:00.000000 iden-0.0.4/PKG-INFO
```

### Comparing `iden-0.0.3a0/LICENSE` & `iden-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/README.md` & `iden-0.0.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -89,14 +89,15 @@
 Please check the [get started page](https://durandtibo.github.io/iden/get_started) to see how to
 install only some specific dependencies or other alternatives to install the library.
 The following is the corresponding `iden` versions and tested dependencies.
 
 | `iden`  | `coola`      | `objectory`  | `numpy`<sup>*</sup> | `pyyaml`<sup>*</sup> | `safetensors`<sup>*</sup> | `torch`<sup>*</sup> | `python`      |
 |---------|--------------|--------------|---------------------|----------------------|---------------------------|---------------------|---------------|
 | `main`  | `>=0.3,<1.0` | `>=0.1,<1.0` | `>=1.22,<2.0`       | `>=6.0,<7.0`         | `>=0.4,<1.0`              | `>=2.0,<3.0`        | `>=3.9,<3.12` |
+| `0.0.3` | `>=0.3,<1.0` | `>=0.1,<1.0` | `>=1.22,<2.0`       | `>=6.0,<7.0`         | `>=0.4,<1.0`              | `>=2.0,<3.0`        | `>=3.9,<3.12` |
 | `0.0.2` | `>=0.4,<1.0` | `>=0.1,<1.0` | `>=1.22,<2.0`       | `>=6.0,<7.0`         | `>=0.4,<1.0`              | `>=2.0,<2.1`        | `>=3.9,<3.12` |
 | `0.0.1` | `>=0.4,<1.0` | `>=0.1,<1.0` | `>=1.22,<2.0`       | `>=6.0,<7.0`         | `>=0.4,<1.0`              | `>=2.0,<2.1`        | `>=3.9,<3.12` |
 
 <sup>*</sup> indicates an optional dependency
 
 ## Contributing
```

#### html2text {}

```diff
@@ -21,22 +21,24 @@
 see how to install only some specific dependencies or other alternatives to
 install the library. The following is the corresponding `iden` versions and
 tested dependencies. | `iden` | `coola` | `objectory` | `numpy`* | `pyyaml`* |
 `safetensors`* | `torch`* | `python` | |---------|--------------|--------------
 |---------------------|----------------------|---------------------------|-----
 ----------------|---------------| | `main` | `>=0.3,<1.0` | `>=0.1,<1.0` |
 `>=1.22,<2.0` | `>=6.0,<7.0` | `>=0.4,<1.0` | `>=2.0,<3.0` | `>=3.9,<3.12` | |
-`0.0.2` | `>=0.4,<1.0` | `>=0.1,<1.0` | `>=1.22,<2.0` | `>=6.0,<7.0` |
-`>=0.4,<1.0` | `>=2.0,<2.1` | `>=3.9,<3.12` | | `0.0.1` | `>=0.4,<1.0` |
+`0.0.3` | `>=0.3,<1.0` | `>=0.1,<1.0` | `>=1.22,<2.0` | `>=6.0,<7.0` |
+`>=0.4,<1.0` | `>=2.0,<3.0` | `>=3.9,<3.12` | | `0.0.2` | `>=0.4,<1.0` |
 `>=0.1,<1.0` | `>=1.22,<2.0` | `>=6.0,<7.0` | `>=0.4,<1.0` | `>=2.0,<2.1` |
-`>=3.9,<3.12` | * indicates an optional dependency ## Contributing Please check
-the instructions in [CONTRIBUTING.md](.github/CONTRIBUTING.md). ## Suggestions
-and Communication Everyone is welcome to contribute to the community. If you
-have any questions or suggestions, you can submit [Github Issues](https://
-github.com/durandtibo/iden/issues). We will reply to you as soon as possible.
-Thank you very much. ## API stability :warning: While `iden` is in development
-stage, no API is guaranteed to be stable from one release to the next. In fact,
-it is very likely that the API will change multiple times before a stable 1.0.0
-release. In practice, this means that upgrading `iden` to a new version will
-possibly break any code that was using the old version of `iden`. ## License
-`iden` is licensed under BSD 3-Clause "New" or "Revised" license available in
-[LICENSE](LICENSE) file.
+`>=3.9,<3.12` | | `0.0.1` | `>=0.4,<1.0` | `>=0.1,<1.0` | `>=1.22,<2.0` |
+`>=6.0,<7.0` | `>=0.4,<1.0` | `>=2.0,<2.1` | `>=3.9,<3.12` | * indicates an
+optional dependency ## Contributing Please check the instructions in
+[CONTRIBUTING.md](.github/CONTRIBUTING.md). ## Suggestions and Communication
+Everyone is welcome to contribute to the community. If you have any questions
+or suggestions, you can submit [Github Issues](https://github.com/durandtibo/
+iden/issues). We will reply to you as soon as possible. Thank you very much. ##
+API stability :warning: While `iden` is in development stage, no API is
+guaranteed to be stable from one release to the next. In fact, it is very
+likely that the API will change multiple times before a stable 1.0.0 release.
+In practice, this means that upgrading `iden` to a new version will possibly
+break any code that was using the old version of `iden`. ## License `iden` is
+licensed under BSD 3-Clause "New" or "Revised" license available in [LICENSE]
+(LICENSE) file.
```

### Comparing `iden-0.0.3a0/pyproject.toml` & `iden-0.0.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iden"
-version = "0.0.3a0"
+version = "0.0.4"
 description = "simple library to manage a dataset of shards to train machine learning models"
 readme = "README.md"
 authors = ["Thibaut Durand <durand.tibo+gh@gmail.com>"]
 homepage = "https://github.com/durandtibo/iden"
 repository = "https://github.com/durandtibo/iden"
 keywords = ["dataset", "shard"]
 license = "BSD-3-Clause"
@@ -35,37 +35,40 @@
 objectory = ">=0.1,<1.0"
 python = ">=3.9,<3.13"
 
 # Optional dependencies
 numpy = { version = ">=1.22,<2.0", optional = true }
 pyyaml = { version = ">=6.0,<7.0", optional = true }
 safetensors = { version = ">=0.4,<1.0", optional = true }
-torch = { version = ">=1.11,<3.0", optional = true }
+torch = [
+    { version = ">=1.11,<2.3", optional = true, markers="sys_platform == 'darwin' and platform_machine != 'arm64'" },
+    { version = ">=1.11,<3.0", optional = true }
+]
 
 [tool.poetry.extras]
 all = ["numpy", "pyyaml", "safetensors", "torch"]
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
-mike = "^2.0"
+mike = "^2.1"
 mkdocs-material = "^9.5"
-mkdocstrings = { extras = ["python"], version = "^0.24" }
+mkdocstrings = { extras = ["python"], version = "^0.25" }
 
 [tool.poetry.group.dev.dependencies]
-black = ">=24.3"
-coverage = { extras = ["toml"], version = "^7.4" }
+black = ">=24.4"
+coverage = { extras = ["toml"], version = "^7.5" }
 docformatter = { extras = ["tomli"], version = "^1.7" }
-pre-commit = "^3.6"
-pygments = "^2.17"
-pytest = "^8.0"
-pytest-cov = "^4.1"
-pytest-timeout = "^2.2"
-ruff = ">=0.3.0,<1.0"
+pre-commit = "^3.7"
+pygments = "^2.18"
+pytest = "^8.2"
+pytest-cov = "^5.0"
+pytest-timeout = "^2.3"
+ruff = ">=0.4.0,<1.0"
 xdoctest = "^1.1"
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `iden-0.0.3a0/src/iden/data/generator/base.py` & `iden-0.0.4/src/iden/data/generator/base.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/data/generator/vanilla.py` & `iden-0.0.4/src/iden/data/generator/vanilla.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/dataset/base.py` & `iden-0.0.4/src/iden/dataset/base.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/dataset/generator/base.py` & `iden-0.0.4/src/iden/dataset/generator/base.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/dataset/generator/vanilla.py` & `iden-0.0.4/src/iden/dataset/generator/vanilla.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/dataset/loader/base.py` & `iden-0.0.4/src/iden/dataset/loader/base.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/dataset/loader/vanilla.py` & `iden-0.0.4/src/iden/dataset/loader/vanilla.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/dataset/loading.py` & `iden-0.0.4/src/iden/dataset/loading.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/dataset/vanilla.py` & `iden-0.0.4/src/iden/dataset/vanilla.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/io/__init__.py` & `iden-0.0.4/src/iden/io/__init__.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/io/auto.py` & `iden-0.0.4/src/iden/io/auto.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/io/base.py` & `iden-0.0.4/src/iden/io/base.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/io/json.py` & `iden-0.0.4/src/iden/io/json.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/io/pickle.py` & `iden-0.0.4/src/iden/io/pickle.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/io/safetensors/__init__.py` & `iden-0.0.4/src/iden/io/safetensors/__init__.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/io/safetensors/loaders.py` & `iden-0.0.4/src/iden/io/safetensors/loaders.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/io/safetensors/savers.py` & `iden-0.0.4/src/iden/io/safetensors/savers.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/io/text.py` & `iden-0.0.4/src/iden/io/text.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/io/torch.py` & `iden-0.0.4/src/iden/io/torch.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/io/utils.py` & `iden-0.0.4/src/iden/io/utils.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/io/yaml.py` & `iden-0.0.4/src/iden/io/yaml.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/shard/__init__.py` & `iden-0.0.4/src/iden/shard/__init__.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/shard/base.py` & `iden-0.0.4/src/iden/shard/base.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/shard/comparators.py` & `iden-0.0.4/src/iden/shard/comparators.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/shard/dict.py` & `iden-0.0.4/src/iden/shard/dict.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/shard/file.py` & `iden-0.0.4/src/iden/shard/file.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/shard/generator/__init__.py` & `iden-0.0.4/src/iden/shard/generator/__init__.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/shard/generator/base.py` & `iden-0.0.4/src/iden/shard/generator/base.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/shard/generator/dict.py` & `iden-0.0.4/src/iden/shard/generator/dict.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/shard/generator/file.py` & `iden-0.0.4/src/iden/shard/generator/file.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/shard/generator/json.py` & `iden-0.0.4/src/iden/shard/generator/json.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/shard/generator/pickle.py` & `iden-0.0.4/src/iden/shard/generator/pickle.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/shard/generator/safetensors.py` & `iden-0.0.4/src/iden/shard/generator/safetensors.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/shard/generator/torch.py` & `iden-0.0.4/src/iden/shard/generator/torch.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/shard/generator/tuple.py` & `iden-0.0.4/src/iden/shard/generator/tuple.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/shard/generator/yaml.py` & `iden-0.0.4/src/iden/shard/generator/yaml.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/shard/in_memory.py` & `iden-0.0.4/src/iden/shard/in_memory.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/shard/json.py` & `iden-0.0.4/src/iden/shard/json.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/shard/loader/__init__.py` & `iden-0.0.4/src/iden/shard/loader/__init__.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/shard/loader/base.py` & `iden-0.0.4/src/iden/shard/loader/base.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/shard/loader/dict.py` & `iden-0.0.4/src/iden/shard/loader/dict.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/shard/loader/file.py` & `iden-0.0.4/src/iden/shard/loader/file.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/shard/loader/json.py` & `iden-0.0.4/src/iden/shard/loader/json.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/shard/loader/pickle.py` & `iden-0.0.4/src/iden/shard/loader/pickle.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/shard/loader/safetensors.py` & `iden-0.0.4/src/iden/shard/loader/safetensors.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/shard/loader/torch.py` & `iden-0.0.4/src/iden/shard/loader/torch.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/shard/loader/tuple.py` & `iden-0.0.4/src/iden/shard/loader/tuple.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/shard/loader/yaml.py` & `iden-0.0.4/src/iden/shard/loader/yaml.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/shard/loading.py` & `iden-0.0.4/src/iden/shard/loading.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/shard/pickle.py` & `iden-0.0.4/src/iden/shard/pickle.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/shard/safetensors.py` & `iden-0.0.4/src/iden/shard/safetensors.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/shard/torch.py` & `iden-0.0.4/src/iden/shard/torch.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/shard/tuple.py` & `iden-0.0.4/src/iden/shard/tuple.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/shard/utils.py` & `iden-0.0.4/src/iden/shard/utils.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/shard/yaml.py` & `iden-0.0.4/src/iden/shard/yaml.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/utils/format.py` & `iden-0.0.4/src/iden/utils/format.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/utils/imports.py` & `iden-0.0.4/src/iden/utils/imports.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/utils/path.py` & `iden-0.0.4/src/iden/utils/path.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/src/iden/utils/time.py` & `iden-0.0.4/src/iden/utils/time.py`

 * *Files identical despite different names*

### Comparing `iden-0.0.3a0/PKG-INFO` & `iden-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iden
-Version: 0.0.3a0
+Version: 0.0.4
 Summary: simple library to manage a dataset of shards to train machine learning models
 Home-page: https://github.com/durandtibo/iden
 License: BSD-3-Clause
 Keywords: dataset,shard
 Author: Thibaut Durand
 Author-email: durand.tibo+gh@gmail.com
 Requires-Python: >=3.9,<3.13
@@ -24,14 +24,15 @@
 Classifier: Topic :: Software Development :: Libraries
 Provides-Extra: all
 Requires-Dist: coola (>=0.3,<1.0)
 Requires-Dist: numpy (>=1.22,<2.0) ; extra == "all"
 Requires-Dist: objectory (>=0.1,<1.0)
 Requires-Dist: pyyaml (>=6.0,<7.0) ; extra == "all"
 Requires-Dist: safetensors (>=0.4,<1.0) ; extra == "all"
+Requires-Dist: torch (>=1.11,<2.3) ; (sys_platform == "darwin" and platform_machine != "arm64") and (extra == "all")
 Requires-Dist: torch (>=1.11,<3.0) ; extra == "all"
 Project-URL: Repository, https://github.com/durandtibo/iden
 Description-Content-Type: text/markdown
 
 # iden
 
 <p align="center">
@@ -123,14 +124,15 @@
 Please check the [get started page](https://durandtibo.github.io/iden/get_started) to see how to
 install only some specific dependencies or other alternatives to install the library.
 The following is the corresponding `iden` versions and tested dependencies.
 
 | `iden`  | `coola`      | `objectory`  | `numpy`<sup>*</sup> | `pyyaml`<sup>*</sup> | `safetensors`<sup>*</sup> | `torch`<sup>*</sup> | `python`      |
 |---------|--------------|--------------|---------------------|----------------------|---------------------------|---------------------|---------------|
 | `main`  | `>=0.3,<1.0` | `>=0.1,<1.0` | `>=1.22,<2.0`       | `>=6.0,<7.0`         | `>=0.4,<1.0`              | `>=2.0,<3.0`        | `>=3.9,<3.12` |
+| `0.0.3` | `>=0.3,<1.0` | `>=0.1,<1.0` | `>=1.22,<2.0`       | `>=6.0,<7.0`         | `>=0.4,<1.0`              | `>=2.0,<3.0`        | `>=3.9,<3.12` |
 | `0.0.2` | `>=0.4,<1.0` | `>=0.1,<1.0` | `>=1.22,<2.0`       | `>=6.0,<7.0`         | `>=0.4,<1.0`              | `>=2.0,<2.1`        | `>=3.9,<3.12` |
 | `0.0.1` | `>=0.4,<1.0` | `>=0.1,<1.0` | `>=1.22,<2.0`       | `>=6.0,<7.0`         | `>=0.4,<1.0`              | `>=2.0,<2.1`        | `>=3.9,<3.12` |
 
 <sup>*</sup> indicates an optional dependency
 
 ## Contributing
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iden Version: 0.0.3a0 Summary: simple library to
+Metadata-Version: 2.1 Name: iden Version: 0.0.4 Summary: simple library to
 manage a dataset of shards to train machine learning models Home-page: https://
 github.com/durandtibo/iden License: BSD-3-Clause Keywords: dataset,shard
 Author: Thibaut Durand Author-email: durand.tibo+gh@gmail.com Requires-Python:
 >=3.9,<3.13 Classifier: Development Status :: 4 - Beta Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: BSD License Classifier: Operating System :: POSIX :: Linux
@@ -11,17 +11,18 @@
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries Provides-Extra: all
 Requires-Dist: coola (>=0.3,<1.0) Requires-Dist: numpy (>=1.22,<2.0) ; extra ==
 "all" Requires-Dist: objectory (>=0.1,<1.0) Requires-Dist: pyyaml (>=6.0,<7.0)
 ; extra == "all" Requires-Dist: safetensors (>=0.4,<1.0) ; extra == "all"
-Requires-Dist: torch (>=1.11,<3.0) ; extra == "all" Project-URL: Repository,
-https://github.com/durandtibo/iden Description-Content-Type: text/markdown #
-iden
+Requires-Dist: torch (>=1.11,<2.3) ; (sys_platform == "darwin" and
+platform_machine != "arm64") and (extra == "all") Requires-Dist: torch
+(>=1.11,<3.0) ; extra == "all" Project-URL: Repository, https://github.com/
+durandtibo/iden Description-Content-Type: text/markdown # iden
                   _[_C_I_]_[_N_i_g_h_t_l_y_ _T_e_s_t_s_]_[_N_i_g_h_t_l_y_ _P_a_c_k_a_g_e_ _T_e_s_t_s_]
                         _[_D_o_c_u_m_e_n_t_a_t_i_o_n_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_]
      _[_C_o_d_e_c_o_v_]_[_h_t_t_p_s_:_/_/_a_p_i_._c_o_d_e_c_l_i_m_a_t_e_._c_o_m_/_v_1_/_b_a_d_g_e_s_/_e_1_d_6_a_4_9_1_4_6_3_b_5_3_d_d_e_6_5_4_/
  _m_a_i_n_t_a_i_n_a_b_i_l_i_t_y_]_[_h_t_t_p_s_:_/_/_a_p_i_._c_o_d_e_c_l_i_m_a_t_e_._c_o_m_/_v_1_/_b_a_d_g_e_s_/_e_1_d_6_a_4_9_1_4_6_3_b_5_3_d_d_e_6_5_4_/
                                 _t_e_s_t___c_o_v_e_r_a_g_e_]
         _[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]_[_D_o_c_ _s_t_y_l_e_:_ _g_o_o_g_l_e_]_[_R_u_f_f_]_[_D_o_c_ _s_t_y_l_e_:_ _g_o_o_g_l_e_]
                      _[_P_Y_P_I_ _v_e_r_s_i_o_n_]_[_P_y_t_h_o_n_]_[_B_S_D_-_3_-_C_l_a_u_s_e_]
@@ -40,22 +41,24 @@
 see how to install only some specific dependencies or other alternatives to
 install the library. The following is the corresponding `iden` versions and
 tested dependencies. | `iden` | `coola` | `objectory` | `numpy`* | `pyyaml`* |
 `safetensors`* | `torch`* | `python` | |---------|--------------|--------------
 |---------------------|----------------------|---------------------------|-----
 ----------------|---------------| | `main` | `>=0.3,<1.0` | `>=0.1,<1.0` |
 `>=1.22,<2.0` | `>=6.0,<7.0` | `>=0.4,<1.0` | `>=2.0,<3.0` | `>=3.9,<3.12` | |
-`0.0.2` | `>=0.4,<1.0` | `>=0.1,<1.0` | `>=1.22,<2.0` | `>=6.0,<7.0` |
-`>=0.4,<1.0` | `>=2.0,<2.1` | `>=3.9,<3.12` | | `0.0.1` | `>=0.4,<1.0` |
+`0.0.3` | `>=0.3,<1.0` | `>=0.1,<1.0` | `>=1.22,<2.0` | `>=6.0,<7.0` |
+`>=0.4,<1.0` | `>=2.0,<3.0` | `>=3.9,<3.12` | | `0.0.2` | `>=0.4,<1.0` |
 `>=0.1,<1.0` | `>=1.22,<2.0` | `>=6.0,<7.0` | `>=0.4,<1.0` | `>=2.0,<2.1` |
-`>=3.9,<3.12` | * indicates an optional dependency ## Contributing Please check
-the instructions in [CONTRIBUTING.md](.github/CONTRIBUTING.md). ## Suggestions
-and Communication Everyone is welcome to contribute to the community. If you
-have any questions or suggestions, you can submit [Github Issues](https://
-github.com/durandtibo/iden/issues). We will reply to you as soon as possible.
-Thank you very much. ## API stability :warning: While `iden` is in development
-stage, no API is guaranteed to be stable from one release to the next. In fact,
-it is very likely that the API will change multiple times before a stable 1.0.0
-release. In practice, this means that upgrading `iden` to a new version will
-possibly break any code that was using the old version of `iden`. ## License
-`iden` is licensed under BSD 3-Clause "New" or "Revised" license available in
-[LICENSE](LICENSE) file.
+`>=3.9,<3.12` | | `0.0.1` | `>=0.4,<1.0` | `>=0.1,<1.0` | `>=1.22,<2.0` |
+`>=6.0,<7.0` | `>=0.4,<1.0` | `>=2.0,<2.1` | `>=3.9,<3.12` | * indicates an
+optional dependency ## Contributing Please check the instructions in
+[CONTRIBUTING.md](.github/CONTRIBUTING.md). ## Suggestions and Communication
+Everyone is welcome to contribute to the community. If you have any questions
+or suggestions, you can submit [Github Issues](https://github.com/durandtibo/
+iden/issues). We will reply to you as soon as possible. Thank you very much. ##
+API stability :warning: While `iden` is in development stage, no API is
+guaranteed to be stable from one release to the next. In fact, it is very
+likely that the API will change multiple times before a stable 1.0.0 release.
+In practice, this means that upgrading `iden` to a new version will possibly
+break any code that was using the old version of `iden`. ## License `iden` is
+licensed under BSD 3-Clause "New" or "Revised" license available in [LICENSE]
+(LICENSE) file.
```

