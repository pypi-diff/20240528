# Comparing `tmp/lute3_mandarin-0.0.2.tar.gz` & `tmp/lute3_mandarin-0.0.3b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lute3_mandarin-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lute3_mandarin-0.0.3b1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lute3_mandarin-0.0.2.tar` & `lute3_mandarin-0.0.3b1.tar`

### file list

```diff
@@ -1,9 +1,12 @@
--rw-r--r--   0        0        0      313 2024-05-18 03:42:18.966723 lute3_mandarin-0.0.2/.pytest.ini
--rw-r--r--   0        0        0      416 2024-05-18 03:42:18.966791 lute3_mandarin-0.0.2/definition.yaml
--rw-r--r--   0        0        0       52 2024-05-18 17:11:09.161433 lute3_mandarin-0.0.2/lute_mandarin_parser/__init__.py
--rw-r--r--   0        0        0     1990 2024-05-18 17:11:09.161780 lute3_mandarin-0.0.2/lute_mandarin_parser/parser.py
--rw-r--r--   0        0        0      496 2024-05-18 03:42:18.967762 lute3_mandarin-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1538 2024-05-18 03:42:18.967830 lute3_mandarin-0.0.2/requirements.txt
--rw-r--r--   0        0        0      823 2024-05-18 03:42:18.968199 lute3_mandarin-0.0.2/tests/conftest.py
--rw-r--r--   0        0        0     2485 2024-05-18 17:11:09.162123 lute3_mandarin-0.0.2/tests/test_MandarinParser.py
--rw-r--r--   0        0        0      238 1970-01-01 00:00:00.000000 lute3_mandarin-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      313 2024-05-18 03:42:18.966723 lute3_mandarin-0.0.3b1/.pytest.ini
+-rw-r--r--   0        0        0      205 2024-05-27 23:47:17.825356 lute3_mandarin-0.0.3b1/README.md
+-rw-r--r--   0        0        0     1365 2024-05-27 23:47:17.825551 lute3_mandarin-0.0.3b1/README_PyPi.md
+-rw-r--r--   0        0        0      416 2024-05-18 03:42:18.966791 lute3_mandarin-0.0.3b1/definition.yaml
+-rw-r--r--   0        0        0       54 2024-05-27 23:53:11.681963 lute3_mandarin-0.0.3b1/lute_mandarin_parser/__init__.py
+-rw-r--r--   0        0        0     4772 2024-05-27 23:47:17.826015 lute3_mandarin-0.0.3b1/lute_mandarin_parser/parser.py
+-rw-r--r--   0        0        0      525 2024-05-27 23:53:11.682082 lute3_mandarin-0.0.3b1/pyproject.toml
+-rw-r--r--   0        0        0     1538 2024-05-18 03:42:18.967830 lute3_mandarin-0.0.3b1/requirements.txt
+-rw-r--r--   0        0        0        0 2024-05-27 23:47:17.826244 lute3_mandarin-0.0.3b1/tests/__init__.py
+-rw-r--r--   0        0        0      823 2024-05-18 03:42:18.968199 lute3_mandarin-0.0.3b1/tests/conftest.py
+-rw-r--r--   0        0        0     4608 2024-05-27 23:47:17.826704 lute3_mandarin-0.0.3b1/tests/test_MandarinParser.py
+-rw-r--r--   0        0        0     1649 1970-01-01 00:00:00.000000 lute3_mandarin-0.0.3b1/PKG-INFO
```

### Comparing `lute3_mandarin-0.0.2/requirements.txt` & `lute3_mandarin-0.0.3b1/requirements.txt`

 * *Files identical despite different names*

### Comparing `lute3_mandarin-0.0.2/tests/conftest.py` & `lute3_mandarin-0.0.3b1/tests/conftest.py`

 * *Files identical despite different names*

