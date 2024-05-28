# Comparing `tmp/asciiscape-0.1.6.tar.gz` & `tmp/asciiscape-0.1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asciiscape-0.1.6.tar", max compression
+gzip compressed data, was "asciiscape-0.1.6.1.tar", max compression
```

## Comparing `asciiscape-0.1.6.tar` & `asciiscape-0.1.6.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       31 2024-05-28 04:04:25.835254 asciiscape-0.1.6/asciiscape/__init__.py
--rw-r--r--   0        0        0      654 2024-05-28 04:12:13.050449 asciiscape-0.1.6/asciiscape/__main__.py
--rw-r--r--   0        0        0     4410 2024-05-28 04:10:11.855019 asciiscape-0.1.6/asciiscape/console.py
--rw-r--r--   0        0        0     5285 2024-05-27 23:07:17.455948 asciiscape-0.1.6/asciiscape/imgUtils.py
--rw-r--r--   0        0        0      496 2024-05-28 04:12:21.666107 asciiscape-0.1.6/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-28 03:34:12.243744 asciiscape-0.1.6/README.md
--rw-r--r--   0        0        0      476 1970-01-01 00:00:00.000000 asciiscape-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       31 2024-05-28 04:04:25.835254 asciiscape-0.1.6.1/asciiscape/__init__.py
+-rw-r--r--   0        0        0      654 2024-05-28 04:12:13.050449 asciiscape-0.1.6.1/asciiscape/__main__.py
+-rw-r--r--   0        0        0     4410 2024-05-28 04:10:11.855019 asciiscape-0.1.6.1/asciiscape/console.py
+-rw-r--r--   0        0        0     5285 2024-05-27 23:07:17.455948 asciiscape-0.1.6.1/asciiscape/imgUtils.py
+-rw-r--r--   0        0        0      498 2024-05-28 04:19:53.479265 asciiscape-0.1.6.1/pyproject.toml
+-rw-r--r--   0        0        0      274 2024-05-28 04:19:45.904447 asciiscape-0.1.6.1/README.md
+-rw-r--r--   0        0        0      744 1970-01-01 00:00:00.000000 asciiscape-0.1.6.1/PKG-INFO
```

### Comparing `asciiscape-0.1.6/asciiscape/__main__.py` & `asciiscape-0.1.6.1/asciiscape/__main__.py`

 * *Files identical despite different names*

### Comparing `asciiscape-0.1.6/asciiscape/console.py` & `asciiscape-0.1.6.1/asciiscape/console.py`

 * *Files identical despite different names*

### Comparing `asciiscape-0.1.6/asciiscape/imgUtils.py` & `asciiscape-0.1.6.1/asciiscape/imgUtils.py`

 * *Files identical despite different names*

