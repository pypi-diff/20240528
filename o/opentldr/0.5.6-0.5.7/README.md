# Comparing `tmp/opentldr-0.5.6.tar.gz` & `tmp/opentldr-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentldr-0.5.6.tar", last modified: Thu May 23 14:30:30 2024, max compression
+gzip compressed data, was "opentldr-0.5.7.tar", last modified: Tue May 28 19:23:44 2024, max compression
```

## Comparing `opentldr-0.5.6.tar` & `opentldr-0.5.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:30:30.093306 opentldr-0.5.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-23 14:30:25.000000 opentldr-0.5.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:30:25.000000 opentldr-0.5.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8692 2024-05-23 14:30:30.093306 opentldr-0.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7764 2024-05-23 14:30:25.000000 opentldr-0.5.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-23 14:30:25.000000 opentldr-0.5.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 14:30:30.093306 opentldr-0.5.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:30:30.085306 opentldr-0.5.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:30:30.089306 opentldr-0.5.6/src/opentldr/
--rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-05-23 14:30:25.000000 opentldr-0.5.6/src/opentldr/AbstractDataRepo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-05-23 14:30:25.000000 opentldr-0.5.6/src/opentldr/DataRepo.py
--rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-05-23 14:30:25.000000 opentldr-0.5.6/src/opentldr/DataRepoJson.py
--rw-r--r--   0 runner    (1001) docker     (127)    28557 2024-05-23 14:30:25.000000 opentldr-0.5.6/src/opentldr/Domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-05-23 14:30:25.000000 opentldr-0.5.6/src/opentldr/FileSystemDataRepo.py
--rw-r--r--   0 runner    (1001) docker     (127)    38066 2024-05-23 14:30:25.000000 opentldr-0.5.6/src/opentldr/KnowledgeGraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-05-23 14:30:25.000000 opentldr-0.5.6/src/opentldr/S3DataRepo.py
--rw-r--r--   0 runner    (1001) docker     (127)     5518 2024-05-23 14:30:25.000000 opentldr-0.5.6/src/opentldr/Workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-23 14:30:25.000000 opentldr-0.5.6/src/opentldr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-23 14:30:25.000000 opentldr-0.5.6/src/opentldr/log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:30:30.093306 opentldr-0.5.6/src/opentldr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8692 2024-05-23 14:30:30.000000 opentldr-0.5.6/src/opentldr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-23 14:30:30.000000 opentldr-0.5.6/src/opentldr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 14:30:30.000000 opentldr-0.5.6/src/opentldr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-23 14:30:30.000000 opentldr-0.5.6/src/opentldr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-23 14:30:30.000000 opentldr-0.5.6/src/opentldr.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:30:30.093306 opentldr-0.5.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-23 14:30:25.000000 opentldr-0.5.6/tests/test_contentrepo.py
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-23 14:30:25.000000 opentldr-0.5.6/tests/test_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-23 14:30:25.000000 opentldr-0.5.6/tests/test_knowledgegraph.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-23 14:30:25.000000 opentldr-0.5.6/tests/test_workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:23:44.113656 opentldr-0.5.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-28 19:23:39.000000 opentldr-0.5.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 19:23:39.000000 opentldr-0.5.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8692 2024-05-28 19:23:44.113656 opentldr-0.5.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7764 2024-05-28 19:23:39.000000 opentldr-0.5.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-28 19:23:39.000000 opentldr-0.5.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 19:23:44.113656 opentldr-0.5.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:23:44.105656 opentldr-0.5.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:23:44.109656 opentldr-0.5.7/src/opentldr/
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-05-28 19:23:39.000000 opentldr-0.5.7/src/opentldr/AbstractDataRepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-05-28 19:23:39.000000 opentldr-0.5.7/src/opentldr/DataRepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-05-28 19:23:39.000000 opentldr-0.5.7/src/opentldr/DataRepoJson.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28557 2024-05-28 19:23:39.000000 opentldr-0.5.7/src/opentldr/Domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-05-28 19:23:39.000000 opentldr-0.5.7/src/opentldr/FileSystemDataRepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38066 2024-05-28 19:23:39.000000 opentldr-0.5.7/src/opentldr/KnowledgeGraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-05-28 19:23:39.000000 opentldr-0.5.7/src/opentldr/S3DataRepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5518 2024-05-28 19:23:39.000000 opentldr-0.5.7/src/opentldr/Workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-28 19:23:39.000000 opentldr-0.5.7/src/opentldr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-28 19:23:39.000000 opentldr-0.5.7/src/opentldr/log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:23:44.109656 opentldr-0.5.7/src/opentldr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8692 2024-05-28 19:23:44.000000 opentldr-0.5.7/src/opentldr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-28 19:23:44.000000 opentldr-0.5.7/src/opentldr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 19:23:44.000000 opentldr-0.5.7/src/opentldr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-28 19:23:44.000000 opentldr-0.5.7/src/opentldr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-28 19:23:44.000000 opentldr-0.5.7/src/opentldr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:23:44.109656 opentldr-0.5.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-28 19:23:39.000000 opentldr-0.5.7/tests/test_contentrepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-28 19:23:39.000000 opentldr-0.5.7/tests/test_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-28 19:23:39.000000 opentldr-0.5.7/tests/test_knowledgegraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-28 19:23:39.000000 opentldr-0.5.7/tests/test_workflow.py
```

### Comparing `opentldr-0.5.6/LICENSE` & `opentldr-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `opentldr-0.5.6/PKG-INFO` & `opentldr-0.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentldr
-Version: 0.5.6
+Version: 0.5.7
 Summary: An open framework for creation of a Tailored Daily Report.
 Author-email: Chris Argenta <cargenta@rockfishresearch.com>
 Project-URL: Source, https://github.com/RockfishResearch/OpenTLDR-Core.git
 Project-URL: Issues, https://github.com/RockfishResearch/OpenTLDR-Core/issues
 Project-URL: Documentation, http://www.opentldr.org/docs
 Project-URL: Homepage, http://www.opentldr.org
 Classifier: Programming Language :: Python :: 3
```

### Comparing `opentldr-0.5.6/README.md` & `opentldr-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `opentldr-0.5.6/pyproject.toml` & `opentldr-0.5.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=61.0']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "opentldr"
-version = "0.5.6"
+version = "0.5.7"
 authors = [
   { name="Chris Argenta", email="cargenta@rockfishresearch.com" },
 ]
 description = "An open framework for creation of a Tailored Daily Report."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `opentldr-0.5.6/src/opentldr/AbstractDataRepo.py` & `opentldr-0.5.7/src/opentldr/AbstractDataRepo.py`

 * *Files identical despite different names*

### Comparing `opentldr-0.5.6/src/opentldr/DataRepo.py` & `opentldr-0.5.7/src/opentldr/DataRepo.py`

 * *Files identical despite different names*

### Comparing `opentldr-0.5.6/src/opentldr/DataRepoJson.py` & `opentldr-0.5.7/src/opentldr/DataRepoJson.py`

 * *Files identical despite different names*

### Comparing `opentldr-0.5.6/src/opentldr/Domain.py` & `opentldr-0.5.7/src/opentldr/Domain.py`

 * *Files identical despite different names*

### Comparing `opentldr-0.5.6/src/opentldr/FileSystemDataRepo.py` & `opentldr-0.5.7/src/opentldr/FileSystemDataRepo.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
                                 list_of_uids.extend(self.clean_up_nodes())
                             
                             case '.json':
                                 log.info("Importing JSON File: {path}".format(path=fullpath))
                                 with open(fullpath) as f:
                                     raw:dict= json.load(f)
 
-                                    for c in self.import_order:
-                                        added_list=self._importByClass(raw,c)
+                                    for c2 in self.import_order:
+                                        added_list=self._importByClass(raw,c2)
                                         list_of_uids.extend(added_list)
                             
                             case _:
                                 log.warning("Skipping unknown-type file: {path}".format(path=fullpath))
                                 continue
         return list_of_uids
```

### Comparing `opentldr-0.5.6/src/opentldr/KnowledgeGraph.py` & `opentldr-0.5.7/src/opentldr/KnowledgeGraph.py`

 * *Files identical despite different names*

### Comparing `opentldr-0.5.6/src/opentldr/S3DataRepo.py` & `opentldr-0.5.7/src/opentldr/S3DataRepo.py`

 * *Files identical despite different names*

### Comparing `opentldr-0.5.6/src/opentldr/Workflow.py` & `opentldr-0.5.7/src/opentldr/Workflow.py`

 * *Files identical despite different names*

### Comparing `opentldr-0.5.6/src/opentldr.egg-info/PKG-INFO` & `opentldr-0.5.7/src/opentldr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentldr
-Version: 0.5.6
+Version: 0.5.7
 Summary: An open framework for creation of a Tailored Daily Report.
 Author-email: Chris Argenta <cargenta@rockfishresearch.com>
 Project-URL: Source, https://github.com/RockfishResearch/OpenTLDR-Core.git
 Project-URL: Issues, https://github.com/RockfishResearch/OpenTLDR-Core/issues
 Project-URL: Documentation, http://www.opentldr.org/docs
 Project-URL: Homepage, http://www.opentldr.org
 Classifier: Programming Language :: Python :: 3
```

### Comparing `opentldr-0.5.6/src/opentldr.egg-info/SOURCES.txt` & `opentldr-0.5.7/src/opentldr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opentldr-0.5.6/tests/test_knowledgegraph.py` & `opentldr-0.5.7/tests/test_knowledgegraph.py`

 * *Files identical despite different names*

### Comparing `opentldr-0.5.6/tests/test_workflow.py` & `opentldr-0.5.7/tests/test_workflow.py`

 * *Files identical despite different names*

