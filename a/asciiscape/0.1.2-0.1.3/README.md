# Comparing `tmp/asciiscape-0.1.2.tar.gz` & `tmp/asciiscape-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asciiscape-0.1.2.tar", max compression
+gzip compressed data, was "asciiscape-0.1.3.tar", max compression
```

## Comparing `asciiscape-0.1.2.tar` & `asciiscape-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       54 2024-05-28 03:57:24.457110 asciiscape-0.1.2/asciiscape/__init__.py
--rw-r--r--   0        0        0      643 2024-05-28 03:52:33.834275 asciiscape-0.1.2/asciiscape/__main__.py
--rw-r--r--   0        0        0     4394 2024-05-27 21:14:10.147623 asciiscape-0.1.2/asciiscape/console.py
--rw-r--r--   0        0        0     5285 2024-05-27 23:07:17.455948 asciiscape-0.1.2/asciiscape/imgUtils.py
--rw-r--r--   0        0        0      496 2024-05-28 03:57:46.138843 asciiscape-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-28 03:34:12.243744 asciiscape-0.1.2/README.md
--rw-r--r--   0        0        0      476 1970-01-01 00:00:00.000000 asciiscape-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       31 2024-05-28 04:04:25.835254 asciiscape-0.1.3/asciiscape/__init__.py
+-rw-r--r--   0        0        0      643 2024-05-28 03:52:33.834275 asciiscape-0.1.3/asciiscape/__main__.py
+-rw-r--r--   0        0        0     4394 2024-05-27 21:14:10.147623 asciiscape-0.1.3/asciiscape/console.py
+-rw-r--r--   0        0        0     5285 2024-05-27 23:07:17.455948 asciiscape-0.1.3/asciiscape/imgUtils.py
+-rw-r--r--   0        0        0      496 2024-05-28 04:04:40.238078 asciiscape-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-28 03:34:12.243744 asciiscape-0.1.3/README.md
+-rw-r--r--   0        0        0      476 1970-01-01 00:00:00.000000 asciiscape-0.1.3/PKG-INFO
```

### Comparing `asciiscape-0.1.2/asciiscape/__main__.py` & `asciiscape-0.1.3/asciiscape/__main__.py`

 * *Files identical despite different names*

### Comparing `asciiscape-0.1.2/asciiscape/console.py` & `asciiscape-0.1.3/asciiscape/console.py`

 * *Files identical despite different names*

### Comparing `asciiscape-0.1.2/asciiscape/imgUtils.py` & `asciiscape-0.1.3/asciiscape/imgUtils.py`

 * *Files identical despite different names*

