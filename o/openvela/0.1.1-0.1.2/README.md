# Comparing `tmp/openvela-0.1.1.tar.gz` & `tmp/openvela-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openvela-0.1.1.tar", max compression
+gzip compressed data, was "openvela-0.1.2.tar", max compression
```

## Comparing `openvela-0.1.1.tar` & `openvela-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35149 2024-05-24 18:16:21.789096 openvela-0.1.1/LICENSE
--rw-r--r--   0        0        0       26 2024-05-24 18:16:21.789096 openvela-0.1.1/README.md
--rw-r--r--   0        0        0      415 2024-05-24 18:16:21.789096 openvela-0.1.1/openvela/__main__.py
--rw-r--r--   0        0        0      930 2024-05-24 18:16:21.789096 openvela-0.1.1/openvela/agents.py
--rw-r--r--   0        0        0     1796 2024-05-24 18:16:21.789096 openvela-0.1.1/openvela/llms.py
--rw-r--r--   0        0        0      869 2024-05-24 18:16:21.789096 openvela-0.1.1/openvela/logs.py
--rw-r--r--   0        0        0     1224 2024-05-24 18:16:21.789096 openvela-0.1.1/openvela/memory.py
--rw-r--r--   0        0        0      838 2024-05-24 18:16:21.789096 openvela-0.1.1/openvela/prompt.py
--rw-r--r--   0        0        0      859 2024-05-24 18:16:21.789096 openvela-0.1.1/openvela/tasks.py
--rw-r--r--   0        0        0      107 2024-05-24 18:16:21.789096 openvela-0.1.1/openvela/tools.py
--rw-r--r--   0        0        0      290 2024-05-24 18:16:21.789096 openvela-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      356 1970-01-01 00:00:00.000000 openvela-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-28 12:36:07.889838 openvela-0.1.2/LICENSE
+-rw-r--r--   0        0        0       26 2024-05-28 12:36:07.889838 openvela-0.1.2/README.md
+-rw-r--r--   0        0        0      415 2024-05-28 12:36:07.889838 openvela-0.1.2/openvela/__main__.py
+-rw-r--r--   0        0        0      930 2024-05-28 12:36:07.889838 openvela-0.1.2/openvela/agents.py
+-rw-r--r--   0        0        0     1796 2024-05-28 12:36:07.889838 openvela-0.1.2/openvela/llms.py
+-rw-r--r--   0        0        0      869 2024-05-28 12:36:07.889838 openvela-0.1.2/openvela/logs.py
+-rw-r--r--   0        0        0     1224 2024-05-28 12:36:07.889838 openvela-0.1.2/openvela/memory.py
+-rw-r--r--   0        0        0      838 2024-05-28 12:36:07.889838 openvela-0.1.2/openvela/prompt.py
+-rw-r--r--   0        0        0      859 2024-05-28 12:36:07.889838 openvela-0.1.2/openvela/tasks.py
+-rw-r--r--   0        0        0      107 2024-05-28 12:36:07.889838 openvela-0.1.2/openvela/tools.py
+-rw-r--r--   0        0        0      290 2024-05-28 12:36:07.889838 openvela-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      356 1970-01-01 00:00:00.000000 openvela-0.1.2/PKG-INFO
```

### Comparing `openvela-0.1.1/LICENSE` & `openvela-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openvela-0.1.1/openvela/agents.py` & `openvela-0.1.2/openvela/agents.py`

 * *Files identical despite different names*

### Comparing `openvela-0.1.1/openvela/llms.py` & `openvela-0.1.2/openvela/llms.py`

 * *Files identical despite different names*

### Comparing `openvela-0.1.1/openvela/logs.py` & `openvela-0.1.2/openvela/logs.py`

 * *Files identical despite different names*

### Comparing `openvela-0.1.1/openvela/memory.py` & `openvela-0.1.2/openvela/memory.py`

 * *Files identical despite different names*

### Comparing `openvela-0.1.1/openvela/prompt.py` & `openvela-0.1.2/openvela/prompt.py`

 * *Files identical despite different names*

### Comparing `openvela-0.1.1/openvela/tasks.py` & `openvela-0.1.2/openvela/tasks.py`

 * *Files identical despite different names*

