# Comparing `tmp/workspace_clients-2.2.0-py3-none-any.whl.zip` & `tmp/workspace_clients-2.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 7406 bytes, number of entries: 9
--rw-r--r--  2.0 unx      321 b- defN 23-Oct-24 09:51 workspace_clients/__init__.py
+Zip file size: 7404 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      321 b- defN 24-May-24 11:23 workspace_clients/__init__.py
 -rw-r--r--  2.0 unx     5816 b- defN 23-Oct-23 16:47 workspace_clients/assets_client.py
 -rw-r--r--  2.0 unx     5850 b- defN 23-Oct-23 14:40 workspace_clients/containers_client.py
 -rw-r--r--  2.0 unx     4932 b- defN 23-Oct-23 14:40 workspace_clients/models.py
--rw-rw-rw-  2.0 unx      575 b- defN 24-Mar-12 11:16 workspace_clients-2.2.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      844 b- defN 24-Mar-12 11:16 workspace_clients-2.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-12 11:16 workspace_clients-2.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 24-Mar-12 11:16 workspace_clients-2.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      793 b- defN 24-Mar-12 11:16 workspace_clients-2.2.0.dist-info/RECORD
-9 files, 19241 bytes uncompressed, 6018 bytes compressed:  68.7%
+-rw-rw-rw-  2.0 unx      575 b- defN 24-May-28 09:11 workspace_clients-2.2.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      844 b- defN 24-May-28 09:11 workspace_clients-2.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-28 09:11 workspace_clients-2.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       18 b- defN 24-May-28 09:11 workspace_clients-2.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      793 b- defN 24-May-28 09:11 workspace_clients-2.2.1.dist-info/RECORD
+9 files, 19241 bytes uncompressed, 6016 bytes compressed:  68.7%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: workspace_clients/containers_client.py
 Comment: 
 
 Filename: workspace_clients/models.py
 Comment: 
 
-Filename: workspace_clients-2.2.0.dist-info/LICENSE.txt
+Filename: workspace_clients-2.2.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: workspace_clients-2.2.0.dist-info/METADATA
+Filename: workspace_clients-2.2.1.dist-info/METADATA
 Comment: 
 
-Filename: workspace_clients-2.2.0.dist-info/WHEEL
+Filename: workspace_clients-2.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: workspace_clients-2.2.0.dist-info/top_level.txt
+Filename: workspace_clients-2.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: workspace_clients-2.2.0.dist-info/RECORD
+Filename: workspace_clients-2.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## workspace_clients/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = "2.2.0"
+__version__ = "2.2.1"
 __all__ = [
     "WorkspaceServiceAssetsClient",
     "WorkspaceServiceContainersClient",
     "AssetModel",
     "ContainerModel",
 ]
```

## Comparing `workspace_clients-2.2.0.dist-info/LICENSE.txt` & `workspace_clients-2.2.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `workspace_clients-2.2.0.dist-info/METADATA` & `workspace_clients-2.2.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: workspace_clients
-Version: 2.2.0
+Version: 2.2.1
 Summary: E360 Workspace Service Client for Python
 Author: IQVIA
 Author-email: e360pypi@iqvia.com
 License: Apache License 2.0
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

## Comparing `workspace_clients-2.2.0.dist-info/RECORD` & `workspace_clients-2.2.1.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-workspace_clients/__init__.py,sha256=M3ibLrGqrRDd1pyrZWTAbIbZHSX0PTiJeLcWxeRnXlo,321
+workspace_clients/__init__.py,sha256=JEbor-WfczZXrM-6fNq6xH5lPPfC5rhmWY__h8Vcy_g,321
 workspace_clients/assets_client.py,sha256=Cf5k-wKEWWT6dO-B0nlftvU9fP1IDJez3MvbIh6fzEc,5816
 workspace_clients/containers_client.py,sha256=Qkz9Ooas-NGBAI1LDDSEwc-CYwkxQ2wIODzLNdehPPY,5850
 workspace_clients/models.py,sha256=U01DSm9rOP6Z4juKVE10F5pCLycj_Fo9wdx9Xez0k7A,4932
-workspace_clients-2.2.0.dist-info/LICENSE.txt,sha256=uoI1G5lxk8h5Ua5OqmR7137DhTctSXGt9z7EBa1yclI,575
-workspace_clients-2.2.0.dist-info/METADATA,sha256=JObmX0CPp0lLuRfCPjBO0WMOUybgSqyiW0RfGjWORdo,844
-workspace_clients-2.2.0.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-workspace_clients-2.2.0.dist-info/top_level.txt,sha256=OcFZqRKd24c0ia1xM66SQtx-SEIrvdlOu2JHUfXG8aw,18
-workspace_clients-2.2.0.dist-info/RECORD,,
+workspace_clients-2.2.1.dist-info/LICENSE.txt,sha256=uoI1G5lxk8h5Ua5OqmR7137DhTctSXGt9z7EBa1yclI,575
+workspace_clients-2.2.1.dist-info/METADATA,sha256=vuXj58q6H4-kOHvNuyM-yqR8djg7hFItKg8Wm9brQUA,844
+workspace_clients-2.2.1.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+workspace_clients-2.2.1.dist-info/top_level.txt,sha256=OcFZqRKd24c0ia1xM66SQtx-SEIrvdlOu2JHUfXG8aw,18
+workspace_clients-2.2.1.dist-info/RECORD,,
```

