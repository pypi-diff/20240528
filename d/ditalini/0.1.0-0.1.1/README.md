# Comparing `tmp/ditalini-0.1.0.tar.gz` & `tmp/ditalini-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ditalini-0.1.0.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "ditalini-0.1.1.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `ditalini-0.1.0.tar` & `ditalini-0.1.1.tar`

### file list

```diff
@@ -1,34 +1,39 @@
--rw-r--r--   0        0        0      110 2022-11-09 12:37:21.000000 ditalini-0.1.0/.clang-format
--rw-r--r--   0        0        0      306 2022-11-09 12:37:21.000000 ditalini-0.1.0/.gitignore
--rw-r--r--   0        0        0     3784 2022-11-09 12:37:21.000000 ditalini-0.1.0/CMakeLists.txt
--rw-r--r--   0        0        0     1068 2022-11-09 12:37:21.000000 ditalini-0.1.0/LICENSE
--rw-r--r--   0        0        0      306 2022-11-09 12:37:21.000000 ditalini-0.1.0/README.md
--rw-r--r--   0        0        0      949 2022-11-09 12:37:21.000000 ditalini-0.1.0/app/main.cpp
--rw-r--r--   0        0        0      507 2022-11-09 12:37:21.000000 ditalini-0.1.0/cmake/Colors.cmake
--rw-r--r--   0        0        0      995 2022-11-09 12:37:21.000000 ditalini-0.1.0/cmake/ConfigSafeGuards.cmake
--rw-r--r--   0        0        0      209 2022-11-09 12:37:21.000000 ditalini-0.1.0/cmake/Doctest.cmake
--rw-r--r--   0        0        0      797 2022-11-09 12:37:21.000000 ditalini-0.1.0/cmake/Documentation.cmake
--rw-r--r--   0        0        0      736 2022-11-09 12:37:21.000000 ditalini-0.1.0/cmake/FindClangFormat.cmake
--rw-r--r--   0        0        0    11830 2022-11-09 12:37:21.000000 ditalini-0.1.0/cmake/LTO.cmake
--rw-r--r--   0        0        0      797 2022-11-09 12:37:21.000000 ditalini-0.1.0/cmake/Misc.cmake
--rw-r--r--   0        0        0     4543 2022-11-09 12:37:21.000000 ditalini-0.1.0/cmake/Warnings.cmake
--rw-r--r--   0        0        0     1128 2022-11-09 12:37:21.000000 ditalini-0.1.0/cmake/clang-format.cmake
--rw-r--r--   0        0        0   100440 2022-11-09 12:37:21.000000 ditalini-0.1.0/doc/Doxyfile.in
--rw-r--r--   0        0        0     4466 2022-11-09 12:37:21.000000 ditalini-0.1.0/doc/logo-small.png
--rw-r--r--   0        0        0      250 2022-11-09 12:37:21.000000 ditalini-0.1.0/examples/example_square.cpp
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 ditalini-0.1.0/include/.git-keep
--rw-r--r--   0        0        0      600 2022-11-09 12:37:21.000000 ditalini-0.1.0/include/ditalini.h
--rw-r--r--   0        0        0      478 2022-11-09 12:37:21.000000 ditalini-0.1.0/include/ditaliniConfig.h.in
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 ditalini-0.1.0/lib/.git-keep
--rw-r--r--   0        0        0      307 2022-11-09 12:37:21.000000 ditalini-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      163 2022-11-09 12:37:21.000000 ditalini-0.1.0/python/ditalini/README.md
--rw-r--r--   0        0        0       23 2022-11-09 12:37:21.000000 ditalini-0.1.0/python/ditalini/__init__.py
--rw-r--r--   0        0        0      360 2022-11-09 12:37:21.000000 ditalini-0.1.0/python/ditalini/ditalini_ext.cpp
--rw-r--r--   0        0        0      273 2022-11-09 12:37:21.000000 ditalini-0.1.0/python/ditalini/examples/example_square.py
--rw-r--r--   0        0        0       14 2022-11-09 12:37:21.000000 ditalini-0.1.0/requirements.txt
--rw-r--r--   0        0        0     5867 2022-11-09 12:37:21.000000 ditalini-0.1.0/setup.py
--rw-r--r--   0        0        0      347 2022-11-09 12:37:21.000000 ditalini-0.1.0/src/ditalini.cpp
--rw-r--r--   0        0        0     1092 2022-11-09 12:37:21.000000 ditalini-0.1.0/test/CMakeLists.txt
--rw-r--r--   0        0        0      202 2022-11-09 12:37:21.000000 ditalini-0.1.0/test/main.cpp
--rw-r--r--   0        0        0      213 2022-11-09 12:37:21.000000 ditalini-0.1.0/test/square.cpp
--rw-r--r--   0        0        0       96 2022-11-09 12:37:21.000000 ditalini-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      110 2022-11-09 12:37:21.000000 ditalini-0.1.1/.clang-format
+-rw-r--r--   0        0        0      125 2022-11-09 12:37:21.000000 ditalini-0.1.1/.git_archival.txt
+-rw-r--r--   0        0        0     1429 2022-11-09 12:37:21.000000 ditalini-0.1.1/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     1780 2022-11-09 12:37:21.000000 ditalini-0.1.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      340 2022-11-09 12:37:21.000000 ditalini-0.1.1/.gitignore
+-rw-r--r--   0        0        0     3888 2022-11-09 12:37:21.000000 ditalini-0.1.1/CMakeLists.txt
+-rw-r--r--   0        0        0     1068 2022-11-09 12:37:21.000000 ditalini-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2074 2022-11-09 12:37:21.000000 ditalini-0.1.1/README.md
+-rw-r--r--   0        0        0      950 2022-11-09 12:37:21.000000 ditalini-0.1.1/app/main.cpp
+-rw-r--r--   0        0        0      507 2022-11-09 12:37:21.000000 ditalini-0.1.1/cmake/Colors.cmake
+-rw-r--r--   0        0        0      995 2022-11-09 12:37:21.000000 ditalini-0.1.1/cmake/ConfigSafeGuards.cmake
+-rw-r--r--   0        0        0      209 2022-11-09 12:37:21.000000 ditalini-0.1.1/cmake/Doctest.cmake
+-rw-r--r--   0        0        0      797 2022-11-09 12:37:21.000000 ditalini-0.1.1/cmake/Documentation.cmake
+-rw-r--r--   0        0        0    12769 2022-11-09 12:37:21.000000 ditalini-0.1.1/cmake/DynamicVersion.cmake
+-rw-r--r--   0        0        0      736 2022-11-09 12:37:21.000000 ditalini-0.1.1/cmake/FindClangFormat.cmake
+-rw-r--r--   0        0        0    11830 2022-11-09 12:37:21.000000 ditalini-0.1.1/cmake/LTO.cmake
+-rw-r--r--   0        0        0      797 2022-11-09 12:37:21.000000 ditalini-0.1.1/cmake/Misc.cmake
+-rw-r--r--   0        0        0     4543 2022-11-09 12:37:21.000000 ditalini-0.1.1/cmake/Warnings.cmake
+-rw-r--r--   0        0        0     1128 2022-11-09 12:37:21.000000 ditalini-0.1.1/cmake/clang-format.cmake
+-rw-r--r--   0        0        0   100440 2022-11-09 12:37:21.000000 ditalini-0.1.1/doc/Doxyfile.in
+-rw-r--r--   0        0        0     4466 2022-11-09 12:37:21.000000 ditalini-0.1.1/doc/logo-small.png
+-rw-r--r--   0        0        0      250 2022-11-09 12:37:21.000000 ditalini-0.1.1/examples/example_square.cpp
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 ditalini-0.1.1/include/.git-keep
+-rw-r--r--   0        0        0      601 2022-11-09 12:37:21.000000 ditalini-0.1.1/include/ditalini.h
+-rw-r--r--   0        0        0      478 2022-11-09 12:37:21.000000 ditalini-0.1.1/include/ditaliniConfig.h.in
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 ditalini-0.1.1/lib/.git-keep
+-rw-r--r--   0        0        0     1361 2022-11-09 12:37:21.000000 ditalini-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      163 2022-11-09 12:37:21.000000 ditalini-0.1.1/python/ditalini/README.md
+-rw-r--r--   0        0        0       58 2022-11-09 12:37:21.000000 ditalini-0.1.1/python/ditalini/__init__.py
+-rw-r--r--   0        0        0      411 2022-11-09 12:37:21.000000 ditalini-0.1.1/python/ditalini/_version.py
+-rw-r--r--   0        0        0      360 2022-11-09 12:37:21.000000 ditalini-0.1.1/python/ditalini/ditalini_ext.cpp
+-rw-r--r--   0        0        0      273 2022-11-09 12:37:21.000000 ditalini-0.1.1/python/ditalini/examples/example_square.py
+-rw-r--r--   0        0        0      107 2022-11-09 12:37:21.000000 ditalini-0.1.1/python/ditalini/test/test_square.py
+-rw-r--r--   0        0        0       14 2022-11-09 12:37:21.000000 ditalini-0.1.1/requirements.txt
+-rw-r--r--   0        0        0      348 2022-11-09 12:37:21.000000 ditalini-0.1.1/src/ditalini.cpp
+-rw-r--r--   0        0        0     1092 2022-11-09 12:37:21.000000 ditalini-0.1.1/test/CMakeLists.txt
+-rw-r--r--   0        0        0      202 2022-11-09 12:37:21.000000 ditalini-0.1.1/test/main.cpp
+-rw-r--r--   0        0        0      230 2022-11-09 12:37:21.000000 ditalini-0.1.1/test/square.cpp
+-rw-r--r--   0        0        0     3702 2022-11-09 12:37:21.000000 ditalini-0.1.1/PKG-INFO
```

### Comparing `ditalini-0.1.0/CMakeLists.txt` & `ditalini-0.1.1/CMakeLists.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 cmake_minimum_required(VERSION 3.8)
+
+# Get ${VERSION} from git tag
+set(CMAKE_MODULE_PATH ${CMAKE_MODULE_PATH} "${CMAKE_SOURCE_DIR}/cmake/")
+include(DynamicVersion)
+dynamic_version(PROJECT_PREFIX Ditalini_)
+
 project(
   ditalini
-  VERSION 0.1.0
+  VERSION ${PROJECT_VERSION}
   DESCRIPTION "a modern C++ project template"
   LANGUAGES CXX)
 
 # Options: Things you can set via commandline options to cmake 
 # (e.g. -DENABLE_LTO=[ON|OFF])
 option(
   ENABLE_WARNINGS_SETTINGS
   "Allow target_set_warnings to add flags and defines.
   Set this to OFF if you want to provide your own warning parameters."
   ON)
 option(ENABLE_LTO "Enable link time optimization" ON)
 
 # Include cmake files
-set(CMAKE_MODULE_PATH ${CMAKE_MODULE_PATH} "${CMAKE_SOURCE_DIR}/cmake/")
 include(ConfigSafeGuards)
 include(Colors)
 include(CTest)
 include(Doctest)
 include(Documentation)
 include(LTO)
 include(Misc)
@@ -97,15 +102,15 @@
 # --------------------------------------------------------------------------------
 set(PYTHON_FILES
     python/ditalini/ditalini_ext.cpp)
 
 set(PYTHON_EXT_NAME ditalini_ext)
 
 # Try to import all Python components potentially needed by nanobind
-find_package(Python 3.11 EXACT REQUIRED
+find_package(Python 3.8 REQUIRED
   REQUIRED COMPONENTS Interpreter Development.Module
   OPTIONAL_COMPONENTS Development.SABIModule)
 
 # Detect the installed nanobind package and import it into CMake
 execute_process(
   COMMAND "${Python_EXECUTABLE}" -m nanobind --cmake_dir
   OUTPUT_STRIP_TRAILING_WHITESPACE OUTPUT_VARIABLE NB_DIR)
```

### Comparing `ditalini-0.1.0/LICENSE` & `ditalini-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ditalini-0.1.0/app/main.cpp` & `ditalini-0.1.1/app/main.cpp`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -26,8 +26,8 @@
 
   ditalini::Simulation sim = ditalini::Simulation(val);
 
   // Print the square of the input value.
   std::cout << "The square of " << val << " is " << sim.square() << ".\n";
 
   return 0;
-}
+}
```

### Comparing `ditalini-0.1.0/cmake/ConfigSafeGuards.cmake` & `ditalini-0.1.1/cmake/ConfigSafeGuards.cmake`

 * *Files identical despite different names*

### Comparing `ditalini-0.1.0/cmake/Documentation.cmake` & `ditalini-0.1.1/cmake/Documentation.cmake`

 * *Files identical despite different names*

### Comparing `ditalini-0.1.0/cmake/FindClangFormat.cmake` & `ditalini-0.1.1/cmake/FindClangFormat.cmake`

 * *Files identical despite different names*

### Comparing `ditalini-0.1.0/cmake/LTO.cmake` & `ditalini-0.1.1/cmake/LTO.cmake`

 * *Files identical despite different names*

### Comparing `ditalini-0.1.0/cmake/Misc.cmake` & `ditalini-0.1.1/cmake/Misc.cmake`

 * *Files identical despite different names*

### Comparing `ditalini-0.1.0/cmake/Warnings.cmake` & `ditalini-0.1.1/cmake/Warnings.cmake`

 * *Files identical despite different names*

### Comparing `ditalini-0.1.0/cmake/clang-format.cmake` & `ditalini-0.1.1/cmake/clang-format.cmake`

 * *Files identical despite different names*

### Comparing `ditalini-0.1.0/doc/Doxyfile.in` & `ditalini-0.1.1/doc/Doxyfile.in`

 * *Files identical despite different names*

### Comparing `ditalini-0.1.0/doc/logo-small.png` & `ditalini-0.1.1/doc/logo-small.png`

 * *Files identical despite different names*

### Comparing `ditalini-0.1.0/include/ditalini.h` & `ditalini-0.1.1/include/ditalini.h`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -25,8 +25,8 @@
 
  private:
   double value_;
 };
 
 }  // namespace ditalini
 
-#endif  // __DITALINI_H__
+#endif  // __DITALINI_H__
```

### Comparing `ditalini-0.1.0/test/CMakeLists.txt` & `ditalini-0.1.1/test/CMakeLists.txt`

 * *Files identical despite different names*

