# Comparing `tmp/ditalini-0.1.1.tar.gz` & `tmp/ditalini-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ditalini-0.1.1.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "ditalini-0.1.2.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `ditalini-0.1.1.tar` & `ditalini-0.1.2.tar`

### file list

```diff
@@ -1,39 +1,40 @@
--rw-r--r--   0        0        0      110 2022-11-09 12:37:21.000000 ditalini-0.1.1/.clang-format
--rw-r--r--   0        0        0      125 2022-11-09 12:37:21.000000 ditalini-0.1.1/.git_archival.txt
--rw-r--r--   0        0        0     1429 2022-11-09 12:37:21.000000 ditalini-0.1.1/.github/workflows/python-package.yml
--rw-r--r--   0        0        0     1780 2022-11-09 12:37:21.000000 ditalini-0.1.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      340 2022-11-09 12:37:21.000000 ditalini-0.1.1/.gitignore
--rw-r--r--   0        0        0     3888 2022-11-09 12:37:21.000000 ditalini-0.1.1/CMakeLists.txt
--rw-r--r--   0        0        0     1068 2022-11-09 12:37:21.000000 ditalini-0.1.1/LICENSE
--rw-r--r--   0        0        0     2074 2022-11-09 12:37:21.000000 ditalini-0.1.1/README.md
--rw-r--r--   0        0        0      950 2022-11-09 12:37:21.000000 ditalini-0.1.1/app/main.cpp
--rw-r--r--   0        0        0      507 2022-11-09 12:37:21.000000 ditalini-0.1.1/cmake/Colors.cmake
--rw-r--r--   0        0        0      995 2022-11-09 12:37:21.000000 ditalini-0.1.1/cmake/ConfigSafeGuards.cmake
--rw-r--r--   0        0        0      209 2022-11-09 12:37:21.000000 ditalini-0.1.1/cmake/Doctest.cmake
--rw-r--r--   0        0        0      797 2022-11-09 12:37:21.000000 ditalini-0.1.1/cmake/Documentation.cmake
--rw-r--r--   0        0        0    12769 2022-11-09 12:37:21.000000 ditalini-0.1.1/cmake/DynamicVersion.cmake
--rw-r--r--   0        0        0      736 2022-11-09 12:37:21.000000 ditalini-0.1.1/cmake/FindClangFormat.cmake
--rw-r--r--   0        0        0    11830 2022-11-09 12:37:21.000000 ditalini-0.1.1/cmake/LTO.cmake
--rw-r--r--   0        0        0      797 2022-11-09 12:37:21.000000 ditalini-0.1.1/cmake/Misc.cmake
--rw-r--r--   0        0        0     4543 2022-11-09 12:37:21.000000 ditalini-0.1.1/cmake/Warnings.cmake
--rw-r--r--   0        0        0     1128 2022-11-09 12:37:21.000000 ditalini-0.1.1/cmake/clang-format.cmake
--rw-r--r--   0        0        0   100440 2022-11-09 12:37:21.000000 ditalini-0.1.1/doc/Doxyfile.in
--rw-r--r--   0        0        0     4466 2022-11-09 12:37:21.000000 ditalini-0.1.1/doc/logo-small.png
--rw-r--r--   0        0        0      250 2022-11-09 12:37:21.000000 ditalini-0.1.1/examples/example_square.cpp
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 ditalini-0.1.1/include/.git-keep
--rw-r--r--   0        0        0      601 2022-11-09 12:37:21.000000 ditalini-0.1.1/include/ditalini.h
--rw-r--r--   0        0        0      478 2022-11-09 12:37:21.000000 ditalini-0.1.1/include/ditaliniConfig.h.in
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 ditalini-0.1.1/lib/.git-keep
--rw-r--r--   0        0        0     1361 2022-11-09 12:37:21.000000 ditalini-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      163 2022-11-09 12:37:21.000000 ditalini-0.1.1/python/ditalini/README.md
--rw-r--r--   0        0        0       58 2022-11-09 12:37:21.000000 ditalini-0.1.1/python/ditalini/__init__.py
--rw-r--r--   0        0        0      411 2022-11-09 12:37:21.000000 ditalini-0.1.1/python/ditalini/_version.py
--rw-r--r--   0        0        0      360 2022-11-09 12:37:21.000000 ditalini-0.1.1/python/ditalini/ditalini_ext.cpp
--rw-r--r--   0        0        0      273 2022-11-09 12:37:21.000000 ditalini-0.1.1/python/ditalini/examples/example_square.py
--rw-r--r--   0        0        0      107 2022-11-09 12:37:21.000000 ditalini-0.1.1/python/ditalini/test/test_square.py
--rw-r--r--   0        0        0       14 2022-11-09 12:37:21.000000 ditalini-0.1.1/requirements.txt
--rw-r--r--   0        0        0      348 2022-11-09 12:37:21.000000 ditalini-0.1.1/src/ditalini.cpp
--rw-r--r--   0        0        0     1092 2022-11-09 12:37:21.000000 ditalini-0.1.1/test/CMakeLists.txt
--rw-r--r--   0        0        0      202 2022-11-09 12:37:21.000000 ditalini-0.1.1/test/main.cpp
--rw-r--r--   0        0        0      230 2022-11-09 12:37:21.000000 ditalini-0.1.1/test/square.cpp
--rw-r--r--   0        0        0     3702 2022-11-09 12:37:21.000000 ditalini-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      110 2022-11-09 12:37:21.000000 ditalini-0.1.2/.clang-format
+-rw-r--r--   0        0        0      125 2022-11-09 12:37:21.000000 ditalini-0.1.2/.git_archival.txt
+-rw-r--r--   0        0        0       32 2022-11-09 12:37:21.000000 ditalini-0.1.2/.gitattributes
+-rw-r--r--   0        0        0     1429 2022-11-09 12:37:21.000000 ditalini-0.1.2/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     1780 2022-11-09 12:37:21.000000 ditalini-0.1.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      340 2022-11-09 12:37:21.000000 ditalini-0.1.2/.gitignore
+-rw-r--r--   0        0        0     3888 2022-11-09 12:37:21.000000 ditalini-0.1.2/CMakeLists.txt
+-rw-r--r--   0        0        0     1068 2022-11-09 12:37:21.000000 ditalini-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2074 2022-11-09 12:37:21.000000 ditalini-0.1.2/README.md
+-rw-r--r--   0        0        0      950 2022-11-09 12:37:21.000000 ditalini-0.1.2/app/main.cpp
+-rw-r--r--   0        0        0      507 2022-11-09 12:37:21.000000 ditalini-0.1.2/cmake/Colors.cmake
+-rw-r--r--   0        0        0      995 2022-11-09 12:37:21.000000 ditalini-0.1.2/cmake/ConfigSafeGuards.cmake
+-rw-r--r--   0        0        0      209 2022-11-09 12:37:21.000000 ditalini-0.1.2/cmake/Doctest.cmake
+-rw-r--r--   0        0        0      797 2022-11-09 12:37:21.000000 ditalini-0.1.2/cmake/Documentation.cmake
+-rw-r--r--   0        0        0    12769 2022-11-09 12:37:21.000000 ditalini-0.1.2/cmake/DynamicVersion.cmake
+-rw-r--r--   0        0        0      736 2022-11-09 12:37:21.000000 ditalini-0.1.2/cmake/FindClangFormat.cmake
+-rw-r--r--   0        0        0    11830 2022-11-09 12:37:21.000000 ditalini-0.1.2/cmake/LTO.cmake
+-rw-r--r--   0        0        0      797 2022-11-09 12:37:21.000000 ditalini-0.1.2/cmake/Misc.cmake
+-rw-r--r--   0        0        0     4543 2022-11-09 12:37:21.000000 ditalini-0.1.2/cmake/Warnings.cmake
+-rw-r--r--   0        0        0     1128 2022-11-09 12:37:21.000000 ditalini-0.1.2/cmake/clang-format.cmake
+-rw-r--r--   0        0        0   100440 2022-11-09 12:37:21.000000 ditalini-0.1.2/doc/Doxyfile.in
+-rw-r--r--   0        0        0     4466 2022-11-09 12:37:21.000000 ditalini-0.1.2/doc/logo-small.png
+-rw-r--r--   0        0        0      250 2022-11-09 12:37:21.000000 ditalini-0.1.2/examples/example_square.cpp
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 ditalini-0.1.2/include/.git-keep
+-rw-r--r--   0        0        0      601 2022-11-09 12:37:21.000000 ditalini-0.1.2/include/ditalini.h
+-rw-r--r--   0        0        0      478 2022-11-09 12:37:21.000000 ditalini-0.1.2/include/ditaliniConfig.h.in
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 ditalini-0.1.2/lib/.git-keep
+-rw-r--r--   0        0        0     1361 2022-11-09 12:37:21.000000 ditalini-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      163 2022-11-09 12:37:21.000000 ditalini-0.1.2/python/ditalini/README.md
+-rw-r--r--   0        0        0       58 2022-11-09 12:37:21.000000 ditalini-0.1.2/python/ditalini/__init__.py
+-rw-r--r--   0        0        0      411 2022-11-09 12:37:21.000000 ditalini-0.1.2/python/ditalini/_version.py
+-rw-r--r--   0        0        0      360 2022-11-09 12:37:21.000000 ditalini-0.1.2/python/ditalini/ditalini_ext.cpp
+-rw-r--r--   0        0        0      273 2022-11-09 12:37:21.000000 ditalini-0.1.2/python/ditalini/examples/example_square.py
+-rw-r--r--   0        0        0      107 2022-11-09 12:37:21.000000 ditalini-0.1.2/python/ditalini/test/test_square.py
+-rw-r--r--   0        0        0       14 2022-11-09 12:37:21.000000 ditalini-0.1.2/requirements.txt
+-rw-r--r--   0        0        0      348 2022-11-09 12:37:21.000000 ditalini-0.1.2/src/ditalini.cpp
+-rw-r--r--   0        0        0     1092 2022-11-09 12:37:21.000000 ditalini-0.1.2/test/CMakeLists.txt
+-rw-r--r--   0        0        0      202 2022-11-09 12:37:21.000000 ditalini-0.1.2/test/main.cpp
+-rw-r--r--   0        0        0      230 2022-11-09 12:37:21.000000 ditalini-0.1.2/test/square.cpp
+-rw-r--r--   0        0        0     3702 2022-11-09 12:37:21.000000 ditalini-0.1.2/PKG-INFO
```

### Comparing `ditalini-0.1.1/.github/workflows/python-package.yml` & `ditalini-0.1.2/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `ditalini-0.1.1/.github/workflows/python-publish.yml` & `ditalini-0.1.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ditalini-0.1.1/CMakeLists.txt` & `ditalini-0.1.2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ditalini-0.1.1/LICENSE` & `ditalini-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ditalini-0.1.1/README.md` & `ditalini-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ditalini-0.1.1/app/main.cpp` & `ditalini-0.1.2/app/main.cpp`

 * *Files identical despite different names*

### Comparing `ditalini-0.1.1/cmake/ConfigSafeGuards.cmake` & `ditalini-0.1.2/cmake/ConfigSafeGuards.cmake`

 * *Files identical despite different names*

### Comparing `ditalini-0.1.1/cmake/Documentation.cmake` & `ditalini-0.1.2/cmake/Documentation.cmake`

 * *Files identical despite different names*

### Comparing `ditalini-0.1.1/cmake/DynamicVersion.cmake` & `ditalini-0.1.2/cmake/DynamicVersion.cmake`

 * *Files identical despite different names*

### Comparing `ditalini-0.1.1/cmake/FindClangFormat.cmake` & `ditalini-0.1.2/cmake/FindClangFormat.cmake`

 * *Files identical despite different names*

### Comparing `ditalini-0.1.1/cmake/LTO.cmake` & `ditalini-0.1.2/cmake/LTO.cmake`

 * *Files identical despite different names*

### Comparing `ditalini-0.1.1/cmake/Misc.cmake` & `ditalini-0.1.2/cmake/Misc.cmake`

 * *Files identical despite different names*

### Comparing `ditalini-0.1.1/cmake/Warnings.cmake` & `ditalini-0.1.2/cmake/Warnings.cmake`

 * *Files identical despite different names*

### Comparing `ditalini-0.1.1/cmake/clang-format.cmake` & `ditalini-0.1.2/cmake/clang-format.cmake`

 * *Files identical despite different names*

### Comparing `ditalini-0.1.1/doc/Doxyfile.in` & `ditalini-0.1.2/doc/Doxyfile.in`

 * *Files identical despite different names*

### Comparing `ditalini-0.1.1/doc/logo-small.png` & `ditalini-0.1.2/doc/logo-small.png`

 * *Files identical despite different names*

### Comparing `ditalini-0.1.1/include/ditalini.h` & `ditalini-0.1.2/include/ditalini.h`

 * *Files identical despite different names*

### Comparing `ditalini-0.1.1/pyproject.toml` & `ditalini-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ditalini-0.1.1/test/CMakeLists.txt` & `ditalini-0.1.2/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ditalini-0.1.1/PKG-INFO` & `ditalini-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ditalini
-Version: 0.1.1
+Version: 0.1.2
 Summary: A template for your awesome C++/Python scientific computing software project
 Author-Email: Philip Mocz <philip.mocz@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Philip Mocz
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

