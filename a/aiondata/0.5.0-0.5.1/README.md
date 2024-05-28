# Comparing `tmp/aiondata-0.5.0.tar.gz` & `tmp/aiondata-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiondata-0.5.0.tar", max compression
+gzip compressed data, was "aiondata-0.5.1.tar", max compression
```

## Comparing `aiondata-0.5.0.tar` & `aiondata-0.5.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11372 2024-05-21 14:11:42.805010 aiondata-0.5.0/LICENSE
--rw-r--r--   0        0        0     4606 2024-05-21 14:11:42.805010 aiondata-0.5.0/README.md
--rw-r--r--   0        0        0      436 2024-05-21 14:11:42.805010 aiondata-0.5.0/aiondata/__init__.py
--rw-r--r--   0        0        0     9582 2024-05-21 14:11:42.805010 aiondata-0.5.0/aiondata/bindingdb.py
--rw-r--r--   0        0        0     2326 2024-05-21 14:11:42.805010 aiondata-0.5.0/aiondata/datasets.py
--rw-r--r--   0        0        0     4714 2024-05-21 14:11:42.809010 aiondata-0.5.0/aiondata/moleculenet.py
--rw-r--r--   0        0        0     8692 2024-05-21 14:11:42.809010 aiondata-0.5.0/aiondata/protein_structure.py
--rw-r--r--   0        0        0     5413 2024-05-21 14:11:42.809010 aiondata-0.5.0/aiondata/weizmann_ccca.py
--rw-r--r--   0        0        0     1505 2024-05-21 14:11:42.809010 aiondata-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     6299 1970-01-01 00:00:00.000000 aiondata-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11372 2024-05-28 13:36:51.089076 aiondata-0.5.1/LICENSE
+-rw-r--r--   0        0        0     4606 2024-05-28 13:36:51.089076 aiondata-0.5.1/README.md
+-rw-r--r--   0        0        0      436 2024-05-28 13:36:51.089076 aiondata-0.5.1/aiondata/__init__.py
+-rw-r--r--   0        0        0     9804 2024-05-28 13:36:51.089076 aiondata-0.5.1/aiondata/bindingdb.py
+-rw-r--r--   0        0        0     2326 2024-05-28 13:36:51.089076 aiondata-0.5.1/aiondata/datasets.py
+-rw-r--r--   0        0        0     4714 2024-05-28 13:36:51.089076 aiondata-0.5.1/aiondata/moleculenet.py
+-rw-r--r--   0        0        0     8692 2024-05-28 13:36:51.089076 aiondata-0.5.1/aiondata/protein_structure.py
+-rw-r--r--   0        0        0     5413 2024-05-28 13:36:51.089076 aiondata-0.5.1/aiondata/weizmann_ccca.py
+-rw-r--r--   0        0        0     1505 2024-05-28 13:36:51.089076 aiondata-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     6299 1970-01-01 00:00:00.000000 aiondata-0.5.1/PKG-INFO
```

### Comparing `aiondata-0.5.0/LICENSE` & `aiondata-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiondata-0.5.0/README.md` & `aiondata-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `aiondata-0.5.0/aiondata/bindingdb.py` & `aiondata-0.5.1/aiondata/bindingdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -251,15 +251,22 @@
                 "BindingDB Target Chain Sequence",
                 "Ki (nM)",
                 "IC50 (nM)",
                 "Kd (nM)",
                 "EC50 (nM)",
                 "kon (M-1-s-1)",
                 "koff (s-1)",
+                "pH",
+                "Temp C",
             ]
         )
         ba_df = ba_df.rename({"BindingDB Target Chain Sequence": "Sequence"})
 
+        # Filter out rows with Sequences that are not valid
+        ba_df = ba_df.filter(
+            pl.col("Sequence").str.contains("^[ACDEFGHIKLMNPQRSTVWY]+$")
+        )
+
         # Remove spaces from BindingDB Target Chain Sequence column
         ba_df = ba_df.with_columns(pl.col("Sequence").str.replace_all(" ", ""))
 
         return ba_df
```

### Comparing `aiondata-0.5.0/aiondata/datasets.py` & `aiondata-0.5.1/aiondata/datasets.py`

 * *Files identical despite different names*

### Comparing `aiondata-0.5.0/aiondata/moleculenet.py` & `aiondata-0.5.1/aiondata/moleculenet.py`

 * *Files identical despite different names*

### Comparing `aiondata-0.5.0/aiondata/protein_structure.py` & `aiondata-0.5.1/aiondata/protein_structure.py`

 * *Files identical despite different names*

### Comparing `aiondata-0.5.0/aiondata/weizmann_ccca.py` & `aiondata-0.5.1/aiondata/weizmann_ccca.py`

 * *Files identical despite different names*

### Comparing `aiondata-0.5.0/pyproject.toml` & `aiondata-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiondata"
-version = "0.5.0"
+version = "0.5.1"
 description = "A common data access layer for AI-driven drug discovery."
 authors = ["JJ Ben-Joseph <jj@tensorspace.ai>"]
 license = "Apache"
 readme = "README.md"
 homepage = "https://www.github.com/aion-labs/aiondata"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `aiondata-0.5.0/PKG-INFO` & `aiondata-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiondata
-Version: 0.5.0
+Version: 0.5.1
 Summary: A common data access layer for AI-driven drug discovery.
 Home-page: https://www.github.com/aion-labs/aiondata
 License: Apache
 Author: JJ Ben-Joseph
 Author-email: jj@tensorspace.ai
 Requires-Python: >=3.10
 Classifier: Development Status :: 3 - Alpha
```

