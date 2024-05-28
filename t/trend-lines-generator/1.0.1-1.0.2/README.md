# Comparing `tmp/trend_lines_generator-1.0.1.tar.gz` & `tmp/trend_lines_generator-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trend_lines_generator-1.0.1.tar", max compression
+gzip compressed data, was "trend_lines_generator-1.0.2.tar", max compression
```

## Comparing `trend_lines_generator-1.0.1.tar` & `trend_lines_generator-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1470 2024-02-18 08:40:47.211778 trend_lines_generator-1.0.1/README.md
--rw-r--r--   0        0        0      618 2024-02-25 05:21:31.661103 trend_lines_generator-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      445 2024-02-18 08:40:47.214996 trend_lines_generator-1.0.1/trend_lines/__init__.py
--rw-r--r--   0        0        0       62 2024-02-18 08:40:47.215192 trend_lines_generator-1.0.1/trend_lines/factories/__init__.py
--rw-r--r--   0        0        0     2626 2024-02-25 05:21:03.289756 trend_lines_generator-1.0.1/trend_lines/factories/board.py
--rw-r--r--   0        0        0     7394 2024-02-18 08:46:44.991859 trend_lines_generator-1.0.1/trend_lines/generator.py
--rw-r--r--   0        0        0      172 2024-02-18 08:40:47.215685 trend_lines_generator-1.0.1/trend_lines/models/__init__.py
--rw-r--r--   0        0        0     2192 2024-02-18 08:45:29.054849 trend_lines_generator-1.0.1/trend_lines/models/board.py
--rw-r--r--   0        0        0     1837 2024-02-18 08:45:57.570938 trend_lines_generator-1.0.1/trend_lines/models/line.py
--rw-r--r--   0        0        0      225 2024-02-18 08:40:47.216026 trend_lines_generator-1.0.1/trend_lines/models/side.py
--rw-r--r--   0        0        0      663 2024-02-18 09:24:10.111464 trend_lines_generator-1.0.1/trend_lines/models/time.py
--rw-r--r--   0        0        0     1710 2024-02-18 08:40:47.216253 trend_lines_generator-1.0.1/trend_lines/utils.py
--rw-r--r--   0        0        0     2222 1970-01-01 00:00:00.000000 trend_lines_generator-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1470 2024-02-18 08:40:47.211778 trend_lines_generator-1.0.2/README.md
+-rw-r--r--   0        0        0      638 2024-05-28 11:51:14.736276 trend_lines_generator-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      445 2024-02-18 08:40:47.214996 trend_lines_generator-1.0.2/trend_lines/__init__.py
+-rw-r--r--   0        0        0       62 2024-02-18 08:40:47.215192 trend_lines_generator-1.0.2/trend_lines/factories/__init__.py
+-rw-r--r--   0        0        0     2645 2024-05-28 11:49:28.752457 trend_lines_generator-1.0.2/trend_lines/factories/board.py
+-rw-r--r--   0        0        0     7394 2024-02-18 08:46:44.991859 trend_lines_generator-1.0.2/trend_lines/generator.py
+-rw-r--r--   0        0        0      172 2024-02-18 08:40:47.215685 trend_lines_generator-1.0.2/trend_lines/models/__init__.py
+-rw-r--r--   0        0        0     2192 2024-02-18 08:45:29.054849 trend_lines_generator-1.0.2/trend_lines/models/board.py
+-rw-r--r--   0        0        0     1837 2024-02-18 08:45:57.570938 trend_lines_generator-1.0.2/trend_lines/models/line.py
+-rw-r--r--   0        0        0      225 2024-02-18 08:40:47.216026 trend_lines_generator-1.0.2/trend_lines/models/side.py
+-rw-r--r--   0        0        0      663 2024-02-18 09:24:10.111464 trend_lines_generator-1.0.2/trend_lines/models/time.py
+-rw-r--r--   0        0        0     1710 2024-02-18 08:40:47.216253 trend_lines_generator-1.0.2/trend_lines/utils.py
+-rw-r--r--   0        0        0     2264 1970-01-01 00:00:00.000000 trend_lines_generator-1.0.2/PKG-INFO
```

### Comparing `trend_lines_generator-1.0.1/README.md` & `trend_lines_generator-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `trend_lines_generator-1.0.1/pyproject.toml` & `trend_lines_generator-1.0.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tool.poetry]
 name = "trend-lines-generator"
-version = "1.0.1"
+version = "1.0.2"
 description = "Trend lines generator."
 authors = ["Oleksandr Polieno <polyenoom@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/nanvel/trend-lines-generator"
 keywords = ["trendlines", "trend lines", "trend", "ta", "resistance", "support", "technical", "indicators", "financial"]
 packages = [{include = "trend_lines"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pandas = "^2.2"
+pyarrow = "^16.1.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `trend_lines_generator-1.0.1/trend_lines/factories/board.py` & `trend_lines_generator-1.0.2/trend_lines/factories/board.py`

 * *Files 12% similar despite different names*

```diff
@@ -61,16 +61,16 @@
 
         df.rename(
             columns={f"{Side.LOW}_y": Side.LOW, f"{Side.HIGH}_y": Side.HIGH},
             inplace=True,
         )
         df.drop(columns=[f"{Side.LOW}_x", f"{Side.HIGH}_x"], inplace=True)
 
-        df[Side.LOW.value].interpolate(inplace=True)
-        df[Side.HIGH.value].interpolate(inplace=True)
+        df[Side.LOW.value] = df[Side.LOW.value].interpolate()
+        df[Side.HIGH.value] = df[Side.HIGH.value].interpolate()
 
         y_min = low_series.min()
         y_max = high_series.max()
         x_min = df.index[0]
         samples = len(df.index)
         dv = (y_max - y_min) / samples
```

### Comparing `trend_lines_generator-1.0.1/trend_lines/generator.py` & `trend_lines_generator-1.0.2/trend_lines/generator.py`

 * *Files identical despite different names*

### Comparing `trend_lines_generator-1.0.1/trend_lines/models/board.py` & `trend_lines_generator-1.0.2/trend_lines/models/board.py`

 * *Files identical despite different names*

### Comparing `trend_lines_generator-1.0.1/trend_lines/models/line.py` & `trend_lines_generator-1.0.2/trend_lines/models/line.py`

 * *Files identical despite different names*

### Comparing `trend_lines_generator-1.0.1/trend_lines/models/time.py` & `trend_lines_generator-1.0.2/trend_lines/models/time.py`

 * *Files identical despite different names*

### Comparing `trend_lines_generator-1.0.1/trend_lines/utils.py` & `trend_lines_generator-1.0.2/trend_lines/utils.py`

 * *Files identical despite different names*

### Comparing `trend_lines_generator-1.0.1/PKG-INFO` & `trend_lines_generator-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: trend-lines-generator
-Version: 1.0.1
+Version: 1.0.2
 Summary: Trend lines generator.
 Home-page: https://github.com/nanvel/trend-lines-generator
 License: MIT
 Keywords: trendlines,trend lines,trend,ta,resistance,support,technical,indicators,financial
 Author: Oleksandr Polieno
 Author-email: polyenoom@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pandas (>=2.2,<3.0)
+Requires-Dist: pyarrow (>=16.1.0,<17.0.0)
 Project-URL: Repository, https://github.com/nanvel/trend-lines-generator
 Description-Content-Type: text/markdown
 
 # Trend lines generator
 
 Usage example:
 ```python
```

