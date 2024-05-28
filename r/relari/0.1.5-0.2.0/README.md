# Comparing `tmp/relari-0.1.5.tar.gz` & `tmp/relari-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "relari-0.1.5.tar", max compression
+gzip compressed data, was "relari-0.2.0.tar", max compression
```

## Comparing `relari-0.1.5.tar` & `relari-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0     2100 2024-02-29 01:27:03.863704 relari-0.1.5/README.md
--rw-r--r--   0        0        0      464 2024-05-13 02:31:28.788172 relari-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       87 2024-05-12 03:52:38.259679 relari-0.1.5/relari/__init__.py
--rw-r--r--   0        0        0      234 2024-05-12 04:09:15.157060 relari-0.1.5/relari/datatypes.py
--rw-r--r--   0        0        0      199 2024-02-29 01:11:53.776623 relari-0.1.5/relari/eval/__init__.py
--rw-r--r--   0        0        0     5563 2024-04-05 23:41:22.980593 relari-0.1.5/relari/eval/dataset.py
--rw-r--r--   0        0        0     4790 2024-02-29 07:20:41.559538 relari-0.1.5/relari/eval/manager.py
--rw-r--r--   0        0        0     1670 2024-05-11 23:31:38.795184 relari-0.1.5/relari/eval/modules.py
--rw-r--r--   0        0        0     3413 2024-02-29 01:11:53.778019 relari-0.1.5/relari/eval/pipeline.py
--rw-r--r--   0        0        0     1771 2024-02-29 01:11:53.778261 relari-0.1.5/relari/eval/result_types.py
--rw-r--r--   0        0        0      123 2024-02-29 01:11:53.778488 relari-0.1.5/relari/eval/types.py
--rw-r--r--   0        0        0     1106 2024-02-29 01:11:53.779119 relari-0.1.5/relari/eval/utils.py
--rw-r--r--   0        0        0     5154 2024-05-12 04:49:31.332471 relari-0.1.5/relari/relari_client.py
--rw-r--r--   0        0        0     2665 1970-01-01 00:00:00.000000 relari-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      336 2024-05-27 07:29:13.379515 relari-0.2.0/README.md
+-rw-r--r--   0        0        0      546 2024-05-28 14:35:50.091566 relari-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      113 2024-05-28 03:18:53.949171 relari-0.2.0/relari/__init__.py
+-rw-r--r--   0        0        0     5621 2024-05-28 08:28:24.529167 relari-0.2.0/relari/__main__.py
+-rw-r--r--   0        0        0     1998 2024-05-28 13:43:35.219280 relari-0.2.0/relari/client.py
+-rw-r--r--   0        0        0      206 2024-05-27 16:52:46.275758 relari-0.2.0/relari/clients/__init__.py
+-rw-r--r--   0        0        0     1604 2024-05-27 16:55:27.358806 relari-0.2.0/relari/clients/datasets.py
+-rw-r--r--   0        0        0     1540 2024-05-28 06:05:58.743317 relari-0.2.0/relari/clients/evaluations.py
+-rw-r--r--   0        0        0     3160 2024-05-28 14:04:52.373308 relari-0.2.0/relari/clients/metrics.py
+-rw-r--r--   0        0        0      697 2024-05-27 16:55:15.931939 relari-0.2.0/relari/clients/projects.py
+-rw-r--r--   0        0        0     7950 2024-05-27 06:11:13.134537 relari-0.2.0/relari/core/dataset.py
+-rw-r--r--   0        0        0      176 2024-05-27 16:48:34.258726 relari-0.2.0/relari/core/experiment.py
+-rw-r--r--   0        0        0      647 2024-05-28 00:26:26.258955 relari-0.2.0/relari/core/types.py
+-rw-r--r--   0        0        0     1107 2024-05-27 00:11:51.833362 relari-0.2.0/relari/core/utils.py
+-rw-r--r--   0        0        0      873 2024-05-28 03:16:31.102017 relari-0.2.0/relari/metrics.py
+-rw-r--r--   0        0        0     1043 1970-01-01 00:00:00.000000 relari-0.2.0/PKG-INFO
```

### Comparing `relari-0.1.5/relari/eval/utils.py` & `relari-0.2.0/relari/core/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Type, get_origin
 
+
 def type_hint_to_str(type_hint: Type):
     if hasattr(type_hint, '__origin__'):  # Check if it's a generic type
         # Get the base type name (e.g., 'List' or 'Dict')
         base = type_hint.__origin__.__name__.title()
         # Recursively process the arguments (e.g., the contents of List, Dict, etc.)
         args = ", ".join(type_hint_to_str(arg) for arg in type_hint.__args__)
         return f"{base}[{args}]"
```

