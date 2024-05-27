# Comparing `tmp/clickup_sdk-0.1.2.tar.gz` & `tmp/clickup_sdk-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clickup_sdk-0.1.2.tar", max compression
+gzip compressed data, was "clickup_sdk-0.1.3.tar", max compression
```

## Comparing `clickup_sdk-0.1.2.tar` & `clickup_sdk-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2024-05-10 05:21:21.182882 clickup_sdk-0.1.2/README.md
--rw-r--r--   0        0        0       44 2024-05-26 14:08:35.681803 clickup_sdk-0.1.2/clickup_sdk/__init__.py
--rw-r--r--   0        0        0     3248 2024-05-26 14:47:35.219179 clickup_sdk-0.1.2/clickup_sdk/client/__init__.py
--rw-r--r--   0        0        0        0 2024-05-26 14:04:07.141190 clickup_sdk-0.1.2/clickup_sdk/common/__init__.py
--rw-r--r--   0        0        0     1601 2024-05-26 14:42:15.628095 clickup_sdk-0.1.2/clickup_sdk/common/utilities.py
--rw-r--r--   0        0        0       31 2024-05-26 14:05:44.847386 clickup_sdk-0.1.2/clickup_sdk/core/__init__.py
--rw-r--r--   0        0        0      758 2024-05-26 14:39:03.289105 clickup_sdk-0.1.2/clickup_sdk/core/models.py
--rw-r--r--   0        0        0      196 2024-05-26 14:05:39.307488 clickup_sdk-0.1.2/clickup_sdk/core/settings.py
--rw-r--r--   0        0        0      346 2024-05-26 13:56:37.537591 clickup_sdk-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 clickup_sdk-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-10 05:21:21.182882 clickup_sdk-0.1.3/README.md
+-rw-r--r--   0        0        0       44 2024-05-26 14:08:35.681803 clickup_sdk-0.1.3/clickup_sdk/__init__.py
+-rw-r--r--   0        0        0     3248 2024-05-26 14:47:35.219179 clickup_sdk-0.1.3/clickup_sdk/client/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-26 14:04:07.141190 clickup_sdk-0.1.3/clickup_sdk/common/__init__.py
+-rw-r--r--   0        0        0     1749 2024-05-27 22:19:00.868921 clickup_sdk-0.1.3/clickup_sdk/common/utilities.py
+-rw-r--r--   0        0        0       31 2024-05-26 14:05:44.847386 clickup_sdk-0.1.3/clickup_sdk/core/__init__.py
+-rw-r--r--   0        0        0      772 2024-05-27 22:17:01.691517 clickup_sdk-0.1.3/clickup_sdk/core/models.py
+-rw-r--r--   0        0        0      196 2024-05-26 14:05:39.307488 clickup_sdk-0.1.3/clickup_sdk/core/settings.py
+-rw-r--r--   0        0        0      346 2024-05-27 22:19:13.900637 clickup_sdk-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 clickup_sdk-0.1.3/PKG-INFO
```

### Comparing `clickup_sdk-0.1.2/clickup_sdk/client/__init__.py` & `clickup_sdk-0.1.3/clickup_sdk/client/__init__.py`

 * *Files identical despite different names*

### Comparing `clickup_sdk-0.1.2/clickup_sdk/common/utilities.py` & `clickup_sdk-0.1.3/clickup_sdk/common/utilities.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,13 +38,19 @@
                         ndigits=2,
                     )
                 case _:
                     custom_field_value = value
         else:
             custom_field_value = value
     elif custom_field_type == "drop_down":
-        drop_down_type_config = models.DropDownTypeConfig(**custom_field["type_config"])
-        option: int = value if value is not None else drop_down_type_config.default
-        custom_field_value = drop_down_type_config.options[option].name
+        type_config = custom_field["type_config"]
+        drop_down_type_config = models.DropDownTypeConfig(**type_config)
+        option: int | None = (
+            value if value is not None else drop_down_type_config.default
+        )
+        if option is None:
+            custom_field_value = None
+        else:
+            custom_field_value = drop_down_type_config.options[option].name
     else:
         custom_field_value = value
     return custom_field_value
```

### Comparing `clickup_sdk-0.1.2/clickup_sdk/core/models.py` & `clickup_sdk-0.1.3/clickup_sdk/core/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     id: UUID4
     name: str
     color: str
     orderindex: int
 
 
 class DropDownTypeConfig(BaseModel):
-    default: int
+    default: int | None = None
     options: list[DropDownOption]
 
 
 class Tag(BaseModel):
     name: str
```

### Comparing `clickup_sdk-0.1.2/PKG-INFO` & `clickup_sdk-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clickup-sdk
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Marco Carmona
 Author-email: marcocarmonapy@outlook.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

