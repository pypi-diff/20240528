# Comparing `tmp/pyobjc-framework-libxpc-9.1b1.tar.gz` & `tmp/pyobjc-framework-libxpc-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-libxpc-9.1b1.tar", last modified: Sun Mar 26 11:44:50 2023, max compression
+gzip compressed data, was "pyobjc-framework-libxpc-9.2.tar", last modified: Wed Jun  7 00:32:40 2023, max compression
```

## Comparing `pyobjc-framework-libxpc-9.1b1.tar` & `pyobjc-framework-libxpc-9.2.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:44:50.779375 pyobjc-framework-libxpc-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:44:50.733948 pyobjc-framework-libxpc-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:44:50.742357 pyobjc-framework-libxpc-9.1b1/Lib/pyobjc_framework_libxpc.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2070 2023-03-26 11:44:50.000000 pyobjc-framework-libxpc-9.1b1/Lib/pyobjc_framework_libxpc.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)      772 2023-03-26 11:44:50.000000 pyobjc-framework-libxpc-9.1b1/Lib/pyobjc_framework_libxpc.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:44:50.000000 pyobjc-framework-libxpc-9.1b1/Lib/pyobjc_framework_libxpc.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-02-19 13:51:33.000000 pyobjc-framework-libxpc-9.1b1/Lib/pyobjc_framework_libxpc.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       19 2023-03-26 11:44:50.000000 pyobjc-framework-libxpc-9.1b1/Lib/pyobjc_framework_libxpc.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)        4 2023-03-26 11:44:50.000000 pyobjc-framework-libxpc-9.1b1/Lib/pyobjc_framework_libxpc.egg-info/top_level.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:44:50.749001 pyobjc-framework-libxpc-9.1b1/Lib/xpc/
--rw-r--r--   0 ronald     (501) staff       (20)      571 2023-02-19 10:50:37.000000 pyobjc-framework-libxpc-9.1b1/Lib/xpc/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    19267 2023-02-19 10:50:37.000000 pyobjc-framework-libxpc-9.1b1/Lib/xpc/_metadata.py
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2023-02-19 10:50:37.000000 pyobjc-framework-libxpc-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2023-02-19 10:50:37.000000 pyobjc-framework-libxpc-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:44:50.750902 pyobjc-framework-libxpc-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)    10163 2023-02-19 10:50:37.000000 pyobjc-framework-libxpc-9.1b1/Modules/_xpc.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:37.000000 pyobjc-framework-libxpc-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-libxpc-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1859 2023-03-26 11:44:50.778804 pyobjc-framework-libxpc-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:44:50.755425 pyobjc-framework-libxpc-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2023-02-19 10:50:37.000000 pyobjc-framework-libxpc-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     2761 2023-02-19 10:50:37.000000 pyobjc-framework-libxpc-9.1b1/PyObjCTest/test_activity.py
--rw-r--r--   0 ronald     (501) staff       (20)     2591 2023-03-26 10:46:05.000000 pyobjc-framework-libxpc-9.1b1/PyObjCTest/test_connection.py
--rw-r--r--   0 ronald     (501) staff       (20)      427 2023-02-19 10:50:37.000000 pyobjc-framework-libxpc-9.1b1/PyObjCTest/test_debug.py
--rw-r--r--   0 ronald     (501) staff       (20)      180 2023-02-19 10:50:37.000000 pyobjc-framework-libxpc-9.1b1/PyObjCTest/test_endpoint.py
--rw-r--r--   0 ronald     (501) staff       (20)      237 2023-02-19 10:50:37.000000 pyobjc-framework-libxpc-9.1b1/PyObjCTest/test_rich_error.py
--rw-r--r--   0 ronald     (501) staff       (20)     1979 2023-02-19 10:50:37.000000 pyobjc-framework-libxpc-9.1b1/PyObjCTest/test_session.py
--rw-r--r--   0 ronald     (501) staff       (20)    12736 2023-02-19 10:50:37.000000 pyobjc-framework-libxpc-9.1b1/PyObjCTest/test_xpc.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:44:50.756771 pyobjc-framework-libxpc-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)      229 2023-02-19 10:50:37.000000 pyobjc-framework-libxpc-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:44:50.769758 pyobjc-framework-libxpc-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    37293 2023-02-19 10:50:37.000000 pyobjc-framework-libxpc-9.1b1/metadata/raw/arm64-13.1.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    37317 2023-02-19 10:50:37.000000 pyobjc-framework-libxpc-9.1b1/metadata/raw/x86_64-13.1.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    16242 2023-02-19 10:50:37.000000 pyobjc-framework-libxpc-9.1b1/metadata/xpc.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-libxpc-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:44:50.779523 pyobjc-framework-libxpc-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      924 2023-03-25 14:20:32.000000 pyobjc-framework-libxpc-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:32:40.333510 pyobjc-framework-libxpc-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:32:40.297640 pyobjc-framework-libxpc-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:32:40.304784 pyobjc-framework-libxpc-9.2/Lib/pyobjc_framework_libxpc.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2068 2023-06-07 00:32:40.000000 pyobjc-framework-libxpc-9.2/Lib/pyobjc_framework_libxpc.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)      787 2023-06-07 00:32:40.000000 pyobjc-framework-libxpc-9.2/Lib/pyobjc_framework_libxpc.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:32:40.000000 pyobjc-framework-libxpc-9.2/Lib/pyobjc_framework_libxpc.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-02-19 13:51:33.000000 pyobjc-framework-libxpc-9.2/Lib/pyobjc_framework_libxpc.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       17 2023-06-07 00:32:40.000000 pyobjc-framework-libxpc-9.2/Lib/pyobjc_framework_libxpc.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        4 2023-06-07 00:32:40.000000 pyobjc-framework-libxpc-9.2/Lib/pyobjc_framework_libxpc.egg-info/top_level.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:32:40.308208 pyobjc-framework-libxpc-9.2/Lib/xpc/
+-rw-r--r--   0 ronald     (501) staff       (20)      571 2023-02-19 10:50:37.000000 pyobjc-framework-libxpc-9.2/Lib/xpc/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    19642 2023-05-27 09:46:34.000000 pyobjc-framework-libxpc-9.2/Lib/xpc/_metadata.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2023-02-19 10:50:37.000000 pyobjc-framework-libxpc-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2023-02-19 10:50:37.000000 pyobjc-framework-libxpc-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:32:40.310870 pyobjc-framework-libxpc-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)    10441 2023-05-04 11:00:07.000000 pyobjc-framework-libxpc-9.2/Modules/_xpc.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:37.000000 pyobjc-framework-libxpc-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-libxpc-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1857 2023-06-07 00:32:40.333116 pyobjc-framework-libxpc-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:32:40.327900 pyobjc-framework-libxpc-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2023-02-19 10:50:37.000000 pyobjc-framework-libxpc-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2761 2023-02-19 10:50:37.000000 pyobjc-framework-libxpc-9.2/PyObjCTest/test_activity.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2651 2023-05-04 11:00:07.000000 pyobjc-framework-libxpc-9.2/PyObjCTest/test_connection.py
+-rw-r--r--   0 ronald     (501) staff       (20)      427 2023-02-19 10:50:37.000000 pyobjc-framework-libxpc-9.2/PyObjCTest/test_debug.py
+-rw-r--r--   0 ronald     (501) staff       (20)      180 2023-02-19 10:50:37.000000 pyobjc-framework-libxpc-9.2/PyObjCTest/test_endpoint.py
+-rw-r--r--   0 ronald     (501) staff       (20)      277 2023-05-04 11:00:07.000000 pyobjc-framework-libxpc-9.2/PyObjCTest/test_rich_error.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1979 2023-02-19 10:50:37.000000 pyobjc-framework-libxpc-9.2/PyObjCTest/test_session.py
+-rw-r--r--   0 ronald     (501) staff       (20)    13188 2023-05-27 09:46:34.000000 pyobjc-framework-libxpc-9.2/PyObjCTest/test_xpc.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:32:40.329713 pyobjc-framework-libxpc-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)      229 2023-02-19 10:50:37.000000 pyobjc-framework-libxpc-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:32:40.331896 pyobjc-framework-libxpc-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    37293 2023-02-19 10:50:37.000000 pyobjc-framework-libxpc-9.2/metadata/raw/arm64-13.1.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    37317 2023-02-19 10:50:37.000000 pyobjc-framework-libxpc-9.2/metadata/raw/x86_64-13.1.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    16435 2023-05-27 09:46:34.000000 pyobjc-framework-libxpc-9.2/metadata/xpc.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-libxpc-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-libxpc-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:32:40.333603 pyobjc-framework-libxpc-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1005 2023-05-29 10:07:47.000000 pyobjc-framework-libxpc-9.2/setup.py
```

### Comparing `pyobjc-framework-libxpc-9.1b1/Lib/pyobjc_framework_libxpc.egg-info/PKG-INFO` & `pyobjc-framework-libxpc-9.2/Lib/pyobjc_framework_libxpc.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-libxpc
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for xpc on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,xpc
 Platform: MacOS X (>=10.8)
```

### Comparing `pyobjc-framework-libxpc-9.1b1/Lib/pyobjc_framework_libxpc.egg-info/SOURCES.txt` & `pyobjc-framework-libxpc-9.2/Lib/pyobjc_framework_libxpc.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/pyobjc_framework_libxpc.egg-info/PKG-INFO
 Lib/pyobjc_framework_libxpc.egg-info/SOURCES.txt
 Lib/pyobjc_framework_libxpc.egg-info/dependency_links.txt
 Lib/pyobjc_framework_libxpc.egg-info/not-zip-safe
 Lib/pyobjc_framework_libxpc.egg-info/requires.txt
 Lib/pyobjc_framework_libxpc.egg-info/top_level.txt
```

### Comparing `pyobjc-framework-libxpc-9.1b1/Lib/xpc/__init__.py` & `pyobjc-framework-libxpc-9.2/Lib/xpc/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-libxpc-9.1b1/Lib/xpc/_metadata.py` & `pyobjc-framework-libxpc-9.2/Lib/xpc/_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is generated by objective.metadata
 #
-# Last update: Sun Feb  5 13:43:27 2023
+# Last update: Thu May 18 11:17:32 2023
 #
 # flake8: noqa
 
 import objc, sys
 from typing import NewType
 
 if sys.maxsize > 2**32:
@@ -85,15 +85,20 @@
         {"arguments": {1: {"c_array_delimited_by_null": True, "type_modifier": "n"}}},
     ),
     "xpc_array_get_double": (b"d@Q",),
     "xpc_array_get_bool": (b"B@Q",),
     "xpc_dictionary_set_uuid": (
         b"v@^t^C",
         "",
-        {"arguments": {1: {"c_array_delimited_by_null": True, "type_modifier": "n"}}},
+        {
+            "arguments": {
+                1: {"c_array_delimited_by_null": True, "type_modifier": "n"},
+                2: {"c_array_of_fixed_length": 16, "type_modifier": "n"},
+            }
+        },
     ),
     "xpc_dictionary_set_double": (
         b"v@^td",
         "",
         {"arguments": {1: {"c_array_delimited_by_null": True, "type_modifier": "n"}}},
     ),
     "xpc_array_set_string": (
@@ -411,18 +416,29 @@
                         "retval": {"type": b"v"},
                         "arguments": {0: {"type": b"^v"}, 1: {"type": b"@"}},
                     }
                 }
             }
         },
     ),
-    "xpc_uuid_create": (b"@^C", "", {"retval": {"already_retained": True}}),
+    "xpc_uuid_create": (
+        b"@^C",
+        "",
+        {
+            "retval": {"already_retained": True},
+            "arguments": {0: {"c_array_of_fixed_length": 16, "type_modifier": "n"}},
+        },
+    ),
     "xpc_string_get_length": (b"Q@",),
     "xpc_connection_set_context": (b"v@^v",),
-    "xpc_array_set_uuid": (b"v@Q^C",),
+    "xpc_array_set_uuid": (
+        b"v@Q^C",
+        "",
+        {"arguments": {2: {"c_array_of_fixed_length": 16, "type_modifier": "n"}}},
+    ),
     "xpc_array_set_fd": (b"v@Qi",),
     "xpc_data_create": (
         b"@^vQ",
         "",
         {
             "retval": {"already_retained": True},
             "arguments": {0: {"c_array_length_in_arg": 1, "type_modifier": "n"}},
```

### Comparing `pyobjc-framework-libxpc-9.1b1/License.txt` & `pyobjc-framework-libxpc-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-libxpc-9.1b1/Modules/_xpc.m` & `pyobjc-framework-libxpc-9.2/Modules/_xpc.m`

 * *Files 7% similar despite different names*

```diff
@@ -127,14 +127,15 @@
 
     r = PyModule_AddObject(m, name, v);
 
     return r;
 }
 
 #pragma clang diagnostic push
+#pragma clang diagnostic ignored "-Wunknown-pragmas"
 #pragma clang diagnostic ignored "-Wunguarded-availability-new"
 
 static struct bytes_constants {
     const char*        name;
     const char* const* value;
 } BYTES_CONSTANTS[] = {
     {"XPC_ACTIVITY_INTERVAL", &XPC_ACTIVITY_INTERVAL},
@@ -142,15 +143,17 @@
     {"XPC_ACTIVITY_DELAY", &XPC_ACTIVITY_DELAY},
     {"XPC_ACTIVITY_GRACE_PERIOD", &XPC_ACTIVITY_GRACE_PERIOD},
     {"XPC_ACTIVITY_PRIORITY", &XPC_ACTIVITY_PRIORITY},
     {"XPC_ACTIVITY_PRIORITY_MAINTENANCE", &XPC_ACTIVITY_PRIORITY_MAINTENANCE},
     {"XPC_ACTIVITY_PRIORITY_UTILITY", &XPC_ACTIVITY_PRIORITY_UTILITY},
     {"XPC_ACTIVITY_ALLOW_BATTERY", &XPC_ACTIVITY_ALLOW_BATTERY},
     {"XPC_ACTIVITY_REQUIRE_SCREEN_SLEEP", &XPC_ACTIVITY_REQUIRE_SCREEN_SLEEP},
+#if PyObjC_BUILD_RELEASE >= 1200
     {"XPC_ACTIVITY_PREVENT_DEVICE_SLEEP", &XPC_ACTIVITY_PREVENT_DEVICE_SLEEP},
+#endif /* PyObjC_BUILD_RELEASE >= 1200 */
     {"XPC_ERROR_KEY_DESCRIPTION", &XPC_ERROR_KEY_DESCRIPTION},
     {"XPC_EVENT_KEY_NAME", &XPC_EVENT_KEY_NAME},
 
     {NULL, NULL}};
 
 static struct int64_constants {
     const char*    name;
@@ -245,21 +248,23 @@
     if (add_constant(m, "XPC_ERROR_CONNECTION_INVALID", @encode(xpc_object_t), &d) != 0)
         goto error;
 
     d = XPC_ERROR_TERMINATION_IMMINENT;
     if (add_constant(m, "XPC_ERROR_TERMINATION_IMMINENT", @encode(xpc_object_t), &d) != 0)
         goto error;
 
+#if PyObjC_BUILD_RELEASE >= 1200
     if (__builtin_available(macOS 12.0, *)) {
         d = XPC_ERROR_PEER_CODE_SIGNING_REQUIREMENT;
         if (add_constant(m, "XPC_ERROR_PEER_CODE_SIGNING_REQUIREMENT",
                          @encode(xpc_object_t), &d)
             != 0)
             goto error;
     }
+#endif /* PyObjC_BUILD_RELEASE >= 1200 */
 
     xpc_type_t t;
     t = XPC_TYPE_NULL;
     if (add_constant(m, "XPC_TYPE_NULL", @encode(xpc_type_t), &t) != 0)
         goto error;
 
     t = XPC_TYPE_BOOL;
@@ -310,21 +315,23 @@
     if (add_constant(m, "XPC_TYPE_DICTIONARY", @encode(xpc_type_t), &t) != 0)
         goto error;
 
     t = XPC_TYPE_ERROR;
     if (add_constant(m, "XPC_TYPE_ERROR", @encode(xpc_type_t), &t) != 0)
         goto error;
 
+#if PyObjC_BUILD_RELEASE >= 1300
     t = XPC_TYPE_SESSION;
     if (add_constant(m, "XPC_TYPE_SESSION", @encode(xpc_type_t), &t) != 0)
         goto error;
 
     t = XPC_TYPE_RICH_ERROR;
     if (add_constant(m, "XPC_TYPE_RICH_ERROR", @encode(xpc_type_t), &t) != 0)
         goto error;
+#endif /* PyObjC_BUILD_RELEASE >= 1300 */
 
     xpc_object_t b = XPC_BOOL_TRUE;
     if (add_constant(m, "XPC_BOOL_TRUE", @encode(xpc_object_t), &b) != 0)
         goto error;
 
     b = XPC_BOOL_FALSE;
     if (add_constant(m, "XPC_BOOL_FALSE", @encode(xpc_object_t), &b) != 0)
```

### Comparing `pyobjc-framework-libxpc-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-libxpc-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-libxpc-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-libxpc-9.2/Modules/pyobjc-compat.h`

 * *Files 2% similar despite different names*

```diff
@@ -301,14 +301,22 @@
 #define MAC_OS_X_VERSION_13_2 130200
 #endif
 
 #ifndef MAC_OS_X_VERSION_13_3
 #define MAC_OS_X_VERSION_13_3 130300
 #endif
 
+#ifndef MAC_OS_X_VERSION_13_4
+#define MAC_OS_X_VERSION_13_4 130400
+#endif
+
+#ifndef MAC_OS_X_VERSION_13_5
+#define MAC_OS_X_VERSION_13_5 130500
+#endif
+
 /*
  *
  * End of Cocoa definitions
  *
  */
 
 /*
@@ -499,10 +507,12 @@
     }
 
 #define PyObjC_LEAVE_GIL                                                                 \
     do {                                                                                 \
         PyGILState_Release(_GILState);                                                   \
     } while (0)
 
+extern PyObject* _Nullable PyObjC_get_tp_dict(PyTypeObject* _Nonnull tp);
+
 NS_ASSUME_NONNULL_END
 
 #endif /* PyObjC_COMPAT_H */
```

### Comparing `pyobjc-framework-libxpc-9.1b1/PKG-INFO` & `pyobjc-framework-libxpc-9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-libxpc
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for xpc on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,xpc
 Platform: MacOS X (>=10.8)
```

### Comparing `pyobjc-framework-libxpc-9.1b1/PyObjCTest/test_activity.py` & `pyobjc-framework-libxpc-9.2/PyObjCTest/test_activity.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-libxpc-9.1b1/PyObjCTest/test_connection.py` & `pyobjc-framework-libxpc-9.2/PyObjCTest/test_connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,24 +9,26 @@
 
 class TestConnection(TestCase):
     def test_constants(self):
         self.assertIsInstance(xpc.XPC_ERROR_CONNECTION_INTERRUPTED, objc.objc_object)
         self.assertIsInstance(xpc.XPC_ERROR_CONNECTION_INVALID, objc.objc_object)
         self.assertIsInstance(xpc.XPC_ERROR_TERMINATION_IMMINENT, objc.objc_object)
 
+        self.assertEqual(xpc.XPC_CONNECTION_MACH_SERVICE_LISTENER, 1 << 0)
+        self.assertEqual(xpc.XPC_CONNECTION_MACH_SERVICE_PRIVILEGED, 1 << 1)
+
+    @min_os_level("12.0")
+    def test_constants12_0(self):
         if (
             platform.mac_ver()[0] != "10.16"
         ):  # Skip test on Python's build with pre-11.0 SDK
             self.assertIsInstance(
                 xpc.XPC_ERROR_PEER_CODE_SIGNING_REQUIREMENT, objc.objc_object
             )
 
-        self.assertEqual(xpc.XPC_CONNECTION_MACH_SERVICE_LISTENER, 1 << 0)
-        self.assertEqual(xpc.XPC_CONNECTION_MACH_SERVICE_PRIVILEGED, 1 << 1)
-
     def test_functions(self):
         self.assertResultIsRetained(xpc.xpc_connection_create)
         self.assertArgIsIn(xpc.xpc_connection_create, 0)
         self.assertArgIsNullTerminated(xpc.xpc_connection_create, 0)
 
         self.assertResultIsRetained(xpc.xpc_connection_create_mach_service)
         self.assertArgIsIn(xpc.xpc_connection_create_mach_service, 0)
```

### Comparing `pyobjc-framework-libxpc-9.1b1/PyObjCTest/test_session.py` & `pyobjc-framework-libxpc-9.2/PyObjCTest/test_session.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-libxpc-9.1b1/PyObjCTest/test_xpc.py` & `pyobjc-framework-libxpc-9.2/PyObjCTest/test_xpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,25 +59,28 @@
         self.assertIsInstance(xpc.XPC_TYPE_STRING, objc.objc_class)
         self.assertIsInstance(xpc.XPC_TYPE_UUID, objc.objc_class)
         self.assertIsInstance(xpc.XPC_TYPE_FD, objc.objc_class)
         self.assertIsInstance(xpc.XPC_TYPE_SHMEM, objc.objc_class)
         self.assertIsInstance(xpc.XPC_TYPE_ARRAY, objc.objc_class)
         self.assertIsInstance(xpc.XPC_TYPE_DICTIONARY, objc.objc_class)
         self.assertIsInstance(xpc.XPC_TYPE_ERROR, objc.objc_class)
-        self.assertIsInstance(xpc.XPC_TYPE_SESSION, objc.objc_class)
-        self.assertIsInstance(xpc.XPC_TYPE_RICH_ERROR, objc.objc_class)
 
         self.assertIsInstance(xpc.XPC_BOOL_TRUE, objc.objc_object)
         self.assertIsInstance(xpc.XPC_BOOL_FALSE, objc.objc_object)
 
         self.assertIsInstance(xpc.XPC_ERROR_KEY_DESCRIPTION, bytes)
         self.assertIsInstance(xpc.XPC_EVENT_KEY_NAME, bytes)
 
         self.assertEqual(xpc.XPC_ARRAY_APPEND, 0xFFFFFFFFFFFFFFFF)
 
+    @min_os_level("13.0")
+    def test_constants13_0(self):
+        self.assertIsInstance(xpc.XPC_TYPE_SESSION, objc.objc_class)
+        self.assertIsInstance(xpc.XPC_TYPE_RICH_ERROR, objc.objc_class)
+
     def test_functions(self):
         self.assertNotHasAttr(xpc, "xpc_retain")
         self.assertNotHasAttr(xpc, "xpc_release")
 
         xpc.xpc_get_type
 
         self.assertResultIsRetained(xpc.xpc_copy)
@@ -134,14 +137,16 @@
         self.assertNotHasAttr(xpc, "xpc_string_create_with_format_and_arguments")
 
         xpc.xpc_string_get_length
 
         self.assertResultIsNullTerminated(xpc.xpc_string_get_string_ptr)
 
         self.assertResultIsRetained(xpc.xpc_uuid_create)
+        self.assertArgIsIn(xpc.xpc_uuid_create, 0)
+        self.assertArgIsFixedSize(xpc.xpc_uuid_create, 0, 16)
 
         self.assertResultHasType(xpc.xpc_uuid_get_bytes, b"^v")
         self.assertResultIsFixedSize(xpc.xpc_uuid_get_bytes, 16)
 
         self.assertResultIsRetained(xpc.xpc_fd_create)
 
         xpc.xpc_fd_dup
@@ -150,16 +155,14 @@
 
         self.assertArgIsOut(xpc.xpc_shmem_map, 1)
 
         self.assertResultIsRetained(xpc.xpc_array_create)
         self.assertArgIsIn(xpc.xpc_array_create, 0)
         self.assertArgSizeInArg(xpc.xpc_array_create, 0, 1)
 
-        self.assertResultIsRetained(xpc.xpc_array_create_empty)
-
         xpc.xpc_array_set_value
         xpc.xpc_array_append_value
         xpc.xpc_array_get_count
         xpc.xpc_array_get_value
 
         self.assertArgIsBlock(xpc.xpc_array_apply, 1, xpc_array_applier_t)
 
@@ -174,15 +177,17 @@
 
         self.assertArgIsIn(xpc.xpc_array_set_data, 2)
         self.assertArgSizeInArg(xpc.xpc_array_set_data, 2, 3)
 
         self.assertArgIsIn(xpc.xpc_array_set_string, 2)
         self.assertArgIsNullTerminated(xpc.xpc_array_set_string, 2)
 
-        xpc.xpc_array_set_uuid
+        self.assertArgIsIn(xpc.xpc_array_set_uuid, 2)
+        self.assertArgIsFixedSize(xpc.xpc_array_set_uuid, 2, 16)
+
         xpc.xpc_array_set_fd
         xpc.xpc_array_set_connection
         xpc.xpc_array_get_bool
         xpc.xpc_array_get_int64
         xpc.xpc_array_get_uint64
         xpc.xpc_array_get_double
         xpc.xpc_array_get_date
@@ -219,15 +224,14 @@
             return True
 
         xpc.xpc_dictionary_apply(value, applier)
         self.assertEqual(
             items, {(b"key1", xpc.XPC_BOOL_TRUE), (b"key2", xpc.XPC_BOOL_FALSE)}
         )
 
-        self.assertResultIsRetained(xpc.xpc_dictionary_create_empty)
         self.assertResultIsRetained(xpc.xpc_dictionary_create_reply)
 
         self.assertArgIsIn(xpc.xpc_dictionary_set_value, 1)
         self.assertArgIsNullTerminated(xpc.xpc_dictionary_set_value, 1)
 
         self.assertArgIsIn(xpc.xpc_dictionary_get_value, 1)
         self.assertArgIsNullTerminated(xpc.xpc_dictionary_get_value, 1)
@@ -261,14 +265,16 @@
         self.assertArgIsIn(xpc.xpc_dictionary_set_string, 1)
         self.assertArgIsNullTerminated(xpc.xpc_dictionary_set_string, 1)
         self.assertArgIsIn(xpc.xpc_dictionary_set_string, 2)
         self.assertArgIsNullTerminated(xpc.xpc_dictionary_set_string, 2)
 
         self.assertArgIsIn(xpc.xpc_dictionary_set_uuid, 1)
         self.assertArgIsNullTerminated(xpc.xpc_dictionary_set_uuid, 1)
+        self.assertArgIsIn(xpc.xpc_dictionary_set_uuid, 2)
+        self.assertArgIsFixedSize(xpc.xpc_dictionary_set_uuid, 2, 16)
 
         self.assertArgIsIn(xpc.xpc_dictionary_set_fd, 1)
         self.assertArgIsNullTerminated(xpc.xpc_dictionary_set_fd, 1)
 
         self.assertArgIsIn(xpc.xpc_dictionary_set_connection, 1)
         self.assertArgIsNullTerminated(xpc.xpc_dictionary_set_connection, 1)
 
@@ -326,7 +332,12 @@
 
         self.assertArgIsIn(xpc.xpc_dictionary_get_array, 1)
         self.assertArgIsNullTerminated(xpc.xpc_dictionary_get_array, 1)
 
     @min_os_level("10.15")
     def test_functions10_15(self):
         self.assertResultIsNullTerminated(xpc.xpc_type_get_name)
+
+    @min_os_level("11.0")
+    def test_functions11_0(self):
+        self.assertResultIsRetained(xpc.xpc_array_create_empty)
+        self.assertResultIsRetained(xpc.xpc_dictionary_create_empty)
```

### Comparing `pyobjc-framework-libxpc-9.1b1/metadata/raw/arm64-13.1.fwinfo` & `pyobjc-framework-libxpc-9.2/metadata/raw/arm64-13.1.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-libxpc-9.1b1/metadata/raw/x86_64-13.1.fwinfo` & `pyobjc-framework-libxpc-9.2/metadata/raw/x86_64-13.1.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-libxpc-9.1b1/metadata/xpc.fwinfo` & `pyobjc-framework-libxpc-9.2/metadata/xpc.fwinfo`

 * *Files 1% similar despite different names*

```diff
@@ -68,14 +68,17 @@
   "functions": {
    "xpc_retain": { "ignore": true },
    "xpc_release": { "ignore": true },
    "xpc_activity_copy_criteria": {
     "retval": { "already_retained": true }
    },
    "xpc_uuid_create": {
+    "args": {
+     "0": { "c_array_of_fixed_length": 16, "type_modifier": "n" }
+    },
     "retval": { "already_retained": true }
    },
    "xpc_endpoint_create": {
     "retval": { "already_retained": true }
    },
    "xpc_activity_register": {
     "args": {
@@ -216,15 +219,15 @@
    "xpc_array_set_string": {
     "args": {
      "2": { "type_override": "^t", "c_array_delimited_by_null": true, "type_modifier": "n" }
     }
    },
    "xpc_array_set_uuid": {
     "args": {
-     "2": {}
+     "2": { "type_modifier": "n", "c_array_of_fixed_length": 16 }
     }
    },
    "xpc_connection_create": {
     "args": {
      "0": { "type_override": "^t", "type_modifier": "n", "c_array_delimited_by_null": true }
     },
     "retval": { "already_retained": true }
@@ -429,15 +432,15 @@
     "args": {
      "1": { "type_override": "^t", "type_modifier": "n", "c_array_delimited_by_null": true }
     }
    },
    "xpc_dictionary_set_uuid": {
     "args": {
      "1": { "type_override": "^t", "type_modifier": "n", "c_array_delimited_by_null": true },
-     "2": {}
+     "2": { "type_modifier": "n", "c_array_of_fixed_length": 16 }
     }
    },
    "xpc_dictionary_set_value": {
     "args": {
      "1": { "type_override": "^t", "type_modifier": "n", "c_array_delimited_by_null": true }
     }
    },
```

### Comparing `pyobjc-framework-libxpc-9.1b1/pyobjc_setup.py` & `pyobjc-framework-libxpc-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-libxpc-9.1b1/setup.py` & `pyobjc-framework-libxpc-9.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,18 +2,23 @@
 Wrappers for the "xpc" library on macOS.
 
 These wrappers don't include documentation, please check Apple's documentation
 for information on how to use this framework and PyObjC's documentation
 for general tips and tricks regarding the translation between Python
 and (Objective-)C frameworks
 """
+import os
+import sys
 
-from pyobjc_setup import Extension, setup
+sys.path.insert(0, os.path.dirname(__file__))
 
-VERSION = "9.1b1"
+
+from pyobjc_setup import Extension, setup  # noqa: E402
+
+VERSION = "9.2"
 
 setup(
     name="pyobjc-framework-libxpc",
     description="Wrappers for xpc on macOS",
     min_os_level="10.8",
     packages=["xpc"],
     ext_modules=[
```

