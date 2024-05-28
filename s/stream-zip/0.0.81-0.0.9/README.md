# Comparing `tmp/stream_zip-0.0.81.tar.gz` & `tmp/stream-zip-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "stream-zip-0.0.9.tar", last modified: Wed Dec 29 20:42:05 2021, max compression
```

## Comparing `stream_zip-0.0.81.tar` & `stream-zip-0.0.9.tar`

### file list

```diff
@@ -1,7 +1,12 @@
--rw-r--r--   0        0        0    39593 2020-02-02 00:00:00.000000 stream_zip-0.0.81/stream_zip/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stream_zip-0.0.81/stream_zip/py.typed
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 stream_zip-0.0.81/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 stream_zip-0.0.81/LICENSE
--rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 stream_zip-0.0.81/README.md
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 stream_zip-0.0.81/pyproject.toml
--rw-r--r--   0        0        0     4045 2020-02-02 00:00:00.000000 stream_zip-0.0.81/PKG-INFO
+drwxr-xr-x   0 dituser    (501) staff       (20)        0 2021-12-29 20:42:05.333943 stream-zip-0.0.9/
+-rw-r--r--   0 dituser    (501) staff       (20)     1091 2021-12-29 07:32:01.000000 stream-zip-0.0.9/LICENSE
+-rw-r--r--   0 dituser    (501) staff       (20)     2287 2021-12-29 20:42:05.333320 stream-zip-0.0.9/PKG-INFO
+-rw-r--r--   0 dituser    (501) staff       (20)     1688 2021-12-29 20:40:51.000000 stream-zip-0.0.9/README.md
+-rw-r--r--   0 dituser    (501) staff       (20)       38 2021-12-29 20:42:05.334026 stream-zip-0.0.9/setup.cfg
+-rw-r--r--   0 dituser    (501) staff       (20)      811 2021-12-29 20:41:34.000000 stream-zip-0.0.9/setup.py
+drwxr-xr-x   0 dituser    (501) staff       (20)        0 2021-12-29 20:42:05.332940 stream-zip-0.0.9/stream_zip.egg-info/
+-rw-r--r--   0 dituser    (501) staff       (20)     2287 2021-12-29 20:42:05.000000 stream-zip-0.0.9/stream_zip.egg-info/PKG-INFO
+-rw-r--r--   0 dituser    (501) staff       (20)      176 2021-12-29 20:42:05.000000 stream-zip-0.0.9/stream_zip.egg-info/SOURCES.txt
+-rw-r--r--   0 dituser    (501) staff       (20)        1 2021-12-29 20:42:05.000000 stream-zip-0.0.9/stream_zip.egg-info/dependency_links.txt
+-rw-r--r--   0 dituser    (501) staff       (20)       11 2021-12-29 20:42:05.000000 stream-zip-0.0.9/stream_zip.egg-info/top_level.txt
+-rw-r--r--   0 dituser    (501) staff       (20)     7677 2021-12-29 20:32:55.000000 stream-zip-0.0.9/stream_zip.py
```

### Comparing `stream_zip-0.0.81/LICENSE` & `stream-zip-0.0.9/LICENSE`

 * *Files identical despite different names*

