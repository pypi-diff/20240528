# Comparing `tmp/solvency2_data-0.2.0.tar.gz` & `tmp/solvency2_data-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solvency2_data-0.2.0.tar", max compression
+gzip compressed data, was "solvency2_data-0.2.1.tar", max compression
```

## Comparing `solvency2_data-0.2.0.tar` & `solvency2_data-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1356 2024-04-09 11:12:58.000000 solvency2_data-0.2.0/LICENSE
--rw-r--r--   0        0        0     1573 2024-04-10 06:44:12.000000 solvency2_data-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1488 2024-04-10 06:44:06.000000 solvency2_data-0.2.0/README.md
--rw-r--r--   0        0        0      233 2024-04-09 11:12:58.000000 solvency2_data-0.2.0/solvency2_data/__init__.py
--rw-r--r--   0        0        0     4688 2024-04-09 11:12:58.000000 solvency2_data-0.2.0/solvency2_data/alternative_extrapolation.py
--rw-r--r--   0        0        0    16171 2024-04-09 11:12:58.000000 solvency2_data-0.2.0/solvency2_data/eiopa_data.py
--rw-r--r--   0        0        0    15807 2024-04-09 11:12:58.000000 solvency2_data-0.2.0/solvency2_data/rfr.py
--rw-r--r--   0        0        0     6314 2024-04-09 11:12:58.000000 solvency2_data-0.2.0/solvency2_data/scraping.py
--rw-r--r--   0        0        0    15376 2024-04-09 11:12:58.000000 solvency2_data-0.2.0/solvency2_data/smith_wilson.py
--rw-r--r--   0        0        0       83 2024-04-09 11:12:58.000000 solvency2_data-0.2.0/solvency2_data/solvency2_data.cfg
--rw-r--r--   0        0        0     8100 2024-04-09 11:12:58.000000 solvency2_data-0.2.0/solvency2_data/sqlite_handler.py
--rw-r--r--   0        0        0     1760 2024-04-09 11:12:58.000000 solvency2_data-0.2.0/solvency2_data/util.py
--rw-r--r--   0        0        0     2690 1970-01-01 00:00:00.000000 solvency2_data-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1356 2024-04-09 11:12:58.000000 solvency2_data-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1598 2024-05-28 09:42:42.000000 solvency2_data-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1488 2024-04-10 06:44:06.000000 solvency2_data-0.2.1/README.md
+-rw-r--r--   0        0        0      233 2024-04-09 11:12:58.000000 solvency2_data-0.2.1/solvency2_data/__init__.py
+-rw-r--r--   0        0        0     4688 2024-04-09 11:12:58.000000 solvency2_data-0.2.1/solvency2_data/alternative_extrapolation.py
+-rw-r--r--   0        0        0    16171 2024-04-09 11:12:58.000000 solvency2_data-0.2.1/solvency2_data/eiopa_data.py
+-rw-r--r--   0        0        0    16115 2024-05-28 09:37:26.000000 solvency2_data-0.2.1/solvency2_data/rfr.py
+-rw-r--r--   0        0        0     6314 2024-04-09 11:12:58.000000 solvency2_data-0.2.1/solvency2_data/scraping.py
+-rw-r--r--   0        0        0    15376 2024-04-09 11:12:58.000000 solvency2_data-0.2.1/solvency2_data/smith_wilson.py
+-rw-r--r--   0        0        0       83 2024-04-09 11:12:58.000000 solvency2_data-0.2.1/solvency2_data/solvency2_data.cfg
+-rw-r--r--   0        0        0     8100 2024-04-09 11:12:58.000000 solvency2_data-0.2.1/solvency2_data/sqlite_handler.py
+-rw-r--r--   0        0        0     1760 2024-04-09 11:12:58.000000 solvency2_data-0.2.1/solvency2_data/util.py
+-rw-r--r--   0        0        0     2690 1970-01-01 00:00:00.000000 solvency2_data-0.2.1/PKG-INFO
```

### Comparing `solvency2_data-0.2.0/LICENSE` & `solvency2_data-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `solvency2_data-0.2.0/pyproject.toml` & `solvency2_data-0.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "solvency2-data"
-version = "0.2.0"
+version = "0.2.1"
 description = "Package for reading the Solvency 2 Risk-Free Interest Rate Term Structures from the zip-files on the EIOPA website and deriving the term structures for alternative extrapolations"
 authors = ["Willem Jan Willemse <w.j.willemse@freedom.nl>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["solvency2", "eiopa", "pandas"]
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -45,7 +45,9 @@
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.5.3"
 mkdocs-material = "^9.5.17"
 mkdocstrings-python = "^1.9.2"
+
+[tool.setuptools_scm]
```

### Comparing `solvency2_data-0.2.0/README.md` & `solvency2_data-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `solvency2_data-0.2.0/solvency2_data/alternative_extrapolation.py` & `solvency2_data-0.2.1/solvency2_data/alternative_extrapolation.py`

 * *Files identical despite different names*

### Comparing `solvency2_data-0.2.0/solvency2_data/eiopa_data.py` & `solvency2_data-0.2.1/solvency2_data/eiopa_data.py`

 * *Files identical despite different names*

### Comparing `solvency2_data-0.2.0/solvency2_data/rfr.py` & `solvency2_data-0.2.1/solvency2_data/rfr.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,19 +199,24 @@
                 - "url": The URL from which the files were downloaded.
                 - "name_zipfile": The name of the downloaded zip file.
                 - "path_excelfile": The path where the Excel files are saved.
                 - "path_zipfile": The path where the zip file is saved.
     """
     cache = RFR_dict(input_date, cache)
 
-    if not (
-        os.path.isfile(join(cache["path_excelfile"], cache["name_excelfile"]))
-    ) or not (
-        os.path.isfile(join(cache["path_excelfile"], cache["name_excelfile_spreads"]))
-    ):
+    name_excelfile = None
+    name_excelfile_spreads = None
+
+    for file in os.listdir(cache["path_excelfile"]):
+        if file.lower() == cache["name_excelfile"].lower():
+            cache['name_excelfile'] = name_excelfile = file
+        if file.lower() == cache["name_excelfile_spreads"].lower():
+            cache['name_excelfile_spreads'] = name_excelfile_spreads = file
+
+    if name_excelfile is None or name_excelfile_spreads is None:
         # determine correct url and zipfile
         cache["url"] = eiopa_link(cache["input_date"], data_type="rfr")
         cache["name_zipfile"] = os.path.basename(cache["url"]).split("filename=")[-1]
 
         # download file
         request = urlopen(cache["url"])
 
@@ -221,17 +226,17 @@
         output.close()
 
         name_excelfile = None
         name_excelfile_spreads = None
         zip_ref = zipfile.ZipFile(join(cache["path_zipfile"], cache["name_zipfile"]))
         for idx, name in enumerate(zip_ref.namelist()):
             if name.lower() == cache["name_excelfile"].lower():
-                name_excelfile = name
+                cache["name_excelfile"] = name_excelfile = name
             if name.lower() == cache["name_excelfile_spreads"].lower():
-                name_excelfile_spreads = name
+                cache["name_excelfile_spreads"] = name_excelfile_spreads = name
         if name_excelfile is not None:
             zip_ref.extract(name_excelfile, cache["path_excelfile"])
         if name_excelfile_spreads is not None:
             zip_ref.extract(name_excelfile_spreads, cache["path_excelfile"])
         zip_ref.close()
 
         # remove zip file
```

### Comparing `solvency2_data-0.2.0/solvency2_data/scraping.py` & `solvency2_data-0.2.1/solvency2_data/scraping.py`

 * *Files identical despite different names*

### Comparing `solvency2_data-0.2.0/solvency2_data/smith_wilson.py` & `solvency2_data-0.2.1/solvency2_data/smith_wilson.py`

 * *Files identical despite different names*

### Comparing `solvency2_data-0.2.0/solvency2_data/sqlite_handler.py` & `solvency2_data-0.2.1/solvency2_data/sqlite_handler.py`

 * *Files identical despite different names*

### Comparing `solvency2_data-0.2.0/solvency2_data/util.py` & `solvency2_data-0.2.1/solvency2_data/util.py`

 * *Files identical despite different names*

### Comparing `solvency2_data-0.2.0/PKG-INFO` & `solvency2_data-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solvency2-data
-Version: 0.2.0
+Version: 0.2.1
 Summary: Package for reading the Solvency 2 Risk-Free Interest Rate Term Structures from the zip-files on the EIOPA website and deriving the term structures for alternative extrapolations
 License: MIT
 Keywords: solvency2,eiopa,pandas
 Author: Willem Jan Willemse
 Author-email: w.j.willemse@freedom.nl
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
```

