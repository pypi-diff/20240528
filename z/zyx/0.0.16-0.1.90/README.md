# Comparing `tmp/zyx-0.0.16.tar.gz` & `tmp/zyx-0.1.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zyx-0.0.16.tar", last modified: Mon May  6 11:11:56 2024, max compression
+gzip compressed data, was "zyx-0.1.90.tar", last modified: Tue May 28 09:37:34 2024, max compression
```

## Comparing `zyx-0.0.16.tar` & `zyx-0.1.90.tar`

### file list

```diff
@@ -1,36 +1,24 @@
-drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-06 11:11:56.955212 zyx-0.0.16/
--rw-r--r--   0 hammad    (1001) hammad    (1001)      431 2024-05-06 11:11:56.955212 zyx-0.0.16/PKG-INFO
--rw-r--r--   0 hammad    (1001) hammad    (1001)       38 2024-05-06 11:11:56.955212 zyx-0.0.16/setup.cfg
--rw-r--r--   0 hammad    (1001) hammad    (1001)     1122 2024-05-06 11:11:42.000000 zyx-0.0.16/setup.py
-drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-06 11:11:56.950212 zyx-0.0.16/src/
-drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-06 11:11:56.951212 zyx-0.0.16/src/zyx/
--rw-r--r--   0 hammad    (1001) hammad    (1001)      493 2024-05-05 22:15:21.000000 zyx-0.0.16/src/zyx/__cli__.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)      225 2024-05-05 22:15:21.000000 zyx-0.0.16/src/zyx/__init__.py
-drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-06 11:11:56.953212 zyx-0.0.16/src/zyx/core/
--rw-r--r--   0 hammad    (1001) hammad    (1001)        0 2024-05-05 22:15:21.000000 zyx-0.0.16/src/zyx/core/__init__.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)      873 2024-05-06 10:48:37.000000 zyx-0.0.16/src/zyx/core/chat.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)     5030 2024-05-05 22:15:21.000000 zyx-0.0.16/src/zyx/core/input.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)     2863 2024-05-05 22:15:21.000000 zyx-0.0.16/src/zyx/core/lightning.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)     2425 2024-05-05 22:15:21.000000 zyx-0.0.16/src/zyx/core/loaders.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)     1976 2024-05-05 22:15:21.000000 zyx-0.0.16/src/zyx/core/print.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)     3506 2024-05-05 22:15:21.000000 zyx-0.0.16/src/zyx/core/validate_path.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)     1690 2024-05-05 22:15:21.000000 zyx-0.0.16/src/zyx/core/validate_type.py
-drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-06 11:11:56.954212 zyx-0.0.16/src/zyx/functions/
--rw-r--r--   0 hammad    (1001) hammad    (1001)      533 2024-05-05 22:15:21.000000 zyx-0.0.16/src/zyx/functions/__init__.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)     2079 2024-05-05 22:15:21.000000 zyx-0.0.16/src/zyx/functions/create_id.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)     1020 2024-05-05 22:15:21.000000 zyx-0.0.16/src/zyx/functions/generate_name.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)     1474 2024-05-05 22:15:21.000000 zyx-0.0.16/src/zyx/functions/get_system_info.py
-drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-06 11:11:56.954212 zyx-0.0.16/src/zyx/jupyter/
--rw-r--r--   0 hammad    (1001) hammad    (1001)       30 2024-05-05 22:15:21.000000 zyx-0.0.16/src/zyx/jupyter/__init__.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)     4026 2024-05-06 11:11:31.000000 zyx-0.0.16/src/zyx/jupyter/tailwind.py
-drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-06 11:11:56.955212 zyx-0.0.16/src/zyx/text/
--rw-r--r--   0 hammad    (1001) hammad    (1001)     1203 2024-05-05 22:15:21.000000 zyx-0.0.16/src/zyx/text/__chunker__.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)      153 2024-05-05 22:15:21.000000 zyx-0.0.16/src/zyx/text/__init__.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)      730 2024-05-05 22:15:21.000000 zyx-0.0.16/src/zyx/text/__read_doc__.py
-drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-06 11:11:56.955212 zyx-0.0.16/src/zyx.egg-info/
--rw-r--r--   0 hammad    (1001) hammad    (1001)      431 2024-05-06 11:11:56.000000 zyx-0.0.16/src/zyx.egg-info/PKG-INFO
--rw-r--r--   0 hammad    (1001) hammad    (1001)      706 2024-05-06 11:11:56.000000 zyx-0.0.16/src/zyx.egg-info/SOURCES.txt
--rw-r--r--   0 hammad    (1001) hammad    (1001)        1 2024-05-06 11:11:56.000000 zyx-0.0.16/src/zyx.egg-info/dependency_links.txt
--rw-r--r--   0 hammad    (1001) hammad    (1001)       41 2024-05-06 11:11:56.000000 zyx-0.0.16/src/zyx.egg-info/entry_points.txt
--rw-r--r--   0 hammad    (1001) hammad    (1001)      104 2024-05-06 11:11:56.000000 zyx-0.0.16/src/zyx.egg-info/requires.txt
--rw-r--r--   0 hammad    (1001) hammad    (1001)        4 2024-05-06 11:11:56.000000 zyx-0.0.16/src/zyx.egg-info/top_level.txt
+drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-28 09:37:34.663922 zyx-0.1.90/
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      424 2024-05-28 09:37:34.662922 zyx-0.1.90/PKG-INFO
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      789 2024-05-17 04:44:11.000000 zyx-0.1.90/README.md
+-rw-r--r--   0 hammad    (1001) hammad    (1001)       38 2024-05-28 09:37:34.663922 zyx-0.1.90/setup.cfg
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      643 2024-05-28 09:37:30.000000 zyx-0.1.90/setup.py
+drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-28 09:37:34.661922 zyx-0.1.90/tests/
+-rw-r--r--   0 hammad    (1001) hammad    (1001)        0 2024-05-28 08:17:16.000000 zyx-0.1.90/tests/test.py
+drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-28 09:37:34.661922 zyx-0.1.90/zyx/
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      117 2024-05-28 09:36:10.000000 zyx-0.1.90/zyx/__init__.py
+drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-28 09:37:34.662922 zyx-0.1.90/zyx/_core/
+-rw-r--r--   0 hammad    (1001) hammad    (1001)        0 2024-05-28 08:14:34.000000 zyx-0.1.90/zyx/_core/__init__.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      130 2024-05-28 08:15:22.000000 zyx-0.1.90/zyx/_core/_core.py
+drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-28 09:37:34.662922 zyx-0.1.90/zyx/_core/llms/
+-rw-r--r--   0 hammad    (1001) hammad    (1001)        0 2024-05-28 08:05:52.000000 zyx-0.1.90/zyx/_core/llms/__init__.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     4115 2024-05-28 08:57:55.000000 zyx-0.1.90/zyx/_core/llms/query.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     3549 2024-05-28 09:22:34.000000 zyx-0.1.90/zyx/_core/llms/query_url.py
+drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-28 09:37:34.662922 zyx-0.1.90/zyx/extensions/
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      604 2024-05-28 09:36:29.000000 zyx-0.1.90/zyx/extensions/__init__.py
+drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-28 09:37:34.662922 zyx-0.1.90/zyx.egg-info/
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      424 2024-05-28 09:37:34.000000 zyx-0.1.90/zyx.egg-info/PKG-INFO
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      329 2024-05-28 09:37:34.000000 zyx-0.1.90/zyx.egg-info/SOURCES.txt
+-rw-r--r--   0 hammad    (1001) hammad    (1001)        1 2024-05-28 09:37:34.000000 zyx-0.1.90/zyx.egg-info/dependency_links.txt
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      105 2024-05-28 09:37:34.000000 zyx-0.1.90/zyx.egg-info/requires.txt
+-rw-r--r--   0 hammad    (1001) hammad    (1001)        4 2024-05-28 09:37:34.000000 zyx-0.1.90/zyx.egg-info/top_level.txt
```

