# Comparing `tmp/pysmartdatamodels-0.8.tar.gz` & `tmp/pysmartdatamodels-0.8.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysmartdatamodels-0.8.tar", max compression
+gzip compressed data, was "pysmartdatamodels-0.8.0.1.tar", max compression
```

## Comparing `pysmartdatamodels-0.8.tar` & `pysmartdatamodels-0.8.0.1.tar`

### file list

```diff
@@ -1,35 +1,32 @@
--rw-r--r--   0        0        0     3202 2024-05-24 14:47:13.469524 pysmartdatamodels-0.8/pyproject.toml
--rw-r--r--   0        0        0     1229 2023-01-26 10:02:06.307000 pysmartdatamodels-0.8/pysmartdatamodels/LICENSE.txt
--rw-r--r--   0        0        0    30201 2024-05-24 14:43:02.933162 pysmartdatamodels-0.8/pysmartdatamodels/README.md
--rw-r--r--   0        0        0       48 2024-05-24 13:50:02.243519 pysmartdatamodels-0.8/pysmartdatamodels/__init__.py
--rw-r--r--   0        0        0     1539 2024-05-24 14:47:13.457524 pysmartdatamodels-0.8/pysmartdatamodels/changes_log.md
--rw-r--r--   0        0        0     5160 2024-05-24 14:56:00.138650 pysmartdatamodels-0.8/pysmartdatamodels/deleteme.py
--rw-r--r--   0        0        0  2820670 2024-05-24 14:56:38.290742 pysmartdatamodels-0.8/pysmartdatamodels/model-assets/datamodels_metadata.json
--rw-r--r--   0        0        0    42357 2024-05-24 14:56:27.262715 pysmartdatamodels-0.8/pysmartdatamodels/model-assets/official_list_data_models.json
--rw-r--r--   0        0        0 104229575 2024-05-24 14:56:37.718741 pysmartdatamodels-0.8/pysmartdatamodels/model-assets/smartdatamodels.json
--rw-r--r--   0        0        0      234 2023-03-28 15:11:09.148185 pysmartdatamodels-0.8/pysmartdatamodels/my_subject/CONTRIBUTORS.yaml
--rw-r--r--   0        0        0      500 2024-03-15 17:02:00.900471 pysmartdatamodels-0.8/pysmartdatamodels/my_subject/TODO
--rw-r--r--   0        0        0      365 2024-03-14 19:31:26.599477 pysmartdatamodels-0.8/pysmartdatamodels/my_subject/my_datamodel/ADOPTERS.yaml
--rw-r--r--   0        0        0     1163 2024-03-14 19:26:38.786086 pysmartdatamodels-0.8/pysmartdatamodels/my_subject/my_datamodel/examples/example-normalized.json
--rw-r--r--   0        0        0     1246 2024-03-14 19:30:26.335186 pysmartdatamodels-0.8/pysmartdatamodels/my_subject/my_datamodel/examples/example-normalized.jsonld
--rw-r--r--   0        0        0      772 2024-03-14 19:30:26.315186 pysmartdatamodels-0.8/pysmartdatamodels/my_subject/my_datamodel/examples/example.json
--rw-r--r--   0        0        0      890 2024-03-14 19:30:26.327186 pysmartdatamodels-0.8/pysmartdatamodels/my_subject/my_datamodel/examples/example.jsonld
--rw-r--r--   0        0        0      279 2022-06-06 18:29:55.272459 pysmartdatamodels-0.8/pysmartdatamodels/my_subject/my_datamodel/notes.yaml
--rw-r--r--   0        0        0      174 2020-09-07 13:41:22.197240 pysmartdatamodels-0.8/pysmartdatamodels/my_subject/notes.yaml
--rw-r--r--   0        0        0    69166 2024-05-24 14:19:21.465277 pysmartdatamodels-0.8/pysmartdatamodels/pysmartdatamodels.py
--rw-r--r--   0        0        0       37 2024-05-23 13:34:59.186946 pysmartdatamodels-0.8/pysmartdatamodels/test/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2024-05-23 13:34:59.186946 pysmartdatamodels-0.8/pysmartdatamodels/test/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2024-05-23 13:34:59.186946 pysmartdatamodels-0.8/pysmartdatamodels/test/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2024-05-24 11:15:48.686288 pysmartdatamodels-0.8/pysmartdatamodels/test/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      116 2024-05-24 14:49:15.889752 pysmartdatamodels-0.8/pysmartdatamodels/test/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2024-05-24 14:49:15.889752 pysmartdatamodels-0.8/pysmartdatamodels/test/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0    44725 2024-05-07 14:24:42.488274 pysmartdatamodels-0.8/pysmartdatamodels/test/__pycache__/test_pysmartdatamodels.cpython-311-pytest-8.2.0.pyc
--rw-r--r--   0        0        0    17366 2024-05-24 11:27:18.287657 pysmartdatamodels-0.8/pysmartdatamodels/test/__pycache__/test_pysmartdatamodels.cpython-38-pytest-7.2.0.pyc
--rw-r--r--   0        0        0    10579 2024-05-24 11:23:30.059153 pysmartdatamodels-0.8/pysmartdatamodels/test/test_pysmartdatamodels.py
--rw-r--r--   0        0        0        1 2024-04-12 11:47:14.872441 pysmartdatamodels-0.8/pysmartdatamodels/utils/__init__.py
--rw-r--r--   0        0        0      205 2024-05-07 12:49:00.435375 pysmartdatamodels-0.8/pysmartdatamodels/utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      187 2024-04-12 13:14:29.012534 pysmartdatamodels-0.8/pysmartdatamodels/utils/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0    85549 2024-05-07 12:49:00.447375 pysmartdatamodels-0.8/pysmartdatamodels/utils/__pycache__/common_utils.cpython-311.pyc
--rw-r--r--   0        0        0    53253 2024-04-12 13:14:29.036534 pysmartdatamodels-0.8/pysmartdatamodels/utils/__pycache__/common_utils.cpython-38.pyc
--rw-r--r--   0        0        0    81253 2024-04-12 12:10:43.397908 pysmartdatamodels-0.8/pysmartdatamodels/utils/common_utils.py
--rw-r--r--   0        0        0    31687 1970-01-01 00:00:00.000000 pysmartdatamodels-0.8/PKG-INFO
+-rw-r--r--   0        0        0     3186 2024-05-28 15:41:20.335167 pysmartdatamodels-0.8.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1229 2023-01-26 10:02:06.307000 pysmartdatamodels-0.8.0.1/pysmartdatamodels/LICENSE.txt
+-rw-r--r--   0        0        0    30201 2024-05-24 14:43:02.933162 pysmartdatamodels-0.8.0.1/pysmartdatamodels/README.md
+-rw-r--r--   0        0        0       33 2024-05-27 22:06:08.447960 pysmartdatamodels-0.8.0.1/pysmartdatamodels/__init__.py
+-rw-r--r--   0        0        0     1635 2024-05-28 15:43:14.867493 pysmartdatamodels-0.8.0.1/pysmartdatamodels/changes_log.md
+-rw-r--r--   0        0        0     5160 2024-05-24 14:56:00.138650 pysmartdatamodels-0.8.0.1/pysmartdatamodels/deleteme.py
+-rw-r--r--   0        0        0      285 2024-05-24 16:01:18.368461 pysmartdatamodels-0.8.0.1/pysmartdatamodels/deleteme2.py
+-rw-r--r--   0        0        0  2820670 2024-05-27 16:18:37.096062 pysmartdatamodels-0.8.0.1/pysmartdatamodels/model-assets/datamodels_metadata.json
+-rw-r--r--   0        0        0    42357 2024-05-27 16:18:22.608023 pysmartdatamodels-0.8.0.1/pysmartdatamodels/model-assets/official_list_data_models.json
+-rw-r--r--   0        0        0 104229575 2024-05-27 16:18:36.476060 pysmartdatamodels-0.8.0.1/pysmartdatamodels/model-assets/smartdatamodels.json
+-rw-r--r--   0        0        0      234 2023-03-28 15:11:09.148185 pysmartdatamodels-0.8.0.1/pysmartdatamodels/my_subject/CONTRIBUTORS.yaml
+-rw-r--r--   0        0        0      500 2024-03-15 17:02:00.900471 pysmartdatamodels-0.8.0.1/pysmartdatamodels/my_subject/TODO
+-rw-r--r--   0        0        0      365 2024-03-14 19:31:26.599477 pysmartdatamodels-0.8.0.1/pysmartdatamodels/my_subject/my_datamodel/ADOPTERS.yaml
+-rw-r--r--   0        0        0     1163 2024-03-14 19:26:38.786086 pysmartdatamodels-0.8.0.1/pysmartdatamodels/my_subject/my_datamodel/examples/example-normalized.json
+-rw-r--r--   0        0        0     1246 2024-03-14 19:30:26.335186 pysmartdatamodels-0.8.0.1/pysmartdatamodels/my_subject/my_datamodel/examples/example-normalized.jsonld
+-rw-r--r--   0        0        0      772 2024-03-14 19:30:26.315186 pysmartdatamodels-0.8.0.1/pysmartdatamodels/my_subject/my_datamodel/examples/example.json
+-rw-r--r--   0        0        0      890 2024-03-14 19:30:26.327186 pysmartdatamodels-0.8.0.1/pysmartdatamodels/my_subject/my_datamodel/examples/example.jsonld
+-rw-r--r--   0        0        0      279 2022-06-06 18:29:55.272459 pysmartdatamodels-0.8.0.1/pysmartdatamodels/my_subject/my_datamodel/notes.yaml
+-rw-r--r--   0        0        0      174 2020-09-07 13:41:22.197240 pysmartdatamodels-0.8.0.1/pysmartdatamodels/my_subject/notes.yaml
+-rw-r--r--   0        0        0    69184 2024-05-27 16:46:29.057766 pysmartdatamodels-0.8.0.1/pysmartdatamodels/pysmartdatamodels.py
+-rw-r--r--   0        0        0       37 2024-05-23 13:34:59.186946 pysmartdatamodels-0.8.0.1/pysmartdatamodels/test/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2024-05-23 13:34:59.186946 pysmartdatamodels-0.8.0.1/pysmartdatamodels/test/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2024-05-23 13:34:59.186946 pysmartdatamodels-0.8.0.1/pysmartdatamodels/test/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2024-05-24 11:15:48.686288 pysmartdatamodels-0.8.0.1/pysmartdatamodels/test/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      116 2024-05-24 14:49:15.889752 pysmartdatamodels-0.8.0.1/pysmartdatamodels/test/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2024-05-24 14:49:15.889752 pysmartdatamodels-0.8.0.1/pysmartdatamodels/test/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0    10579 2024-05-24 11:23:30.059153 pysmartdatamodels-0.8.0.1/pysmartdatamodels/test/test_pysmartdatamodels.py
+-rw-r--r--   0        0        0       28 2024-05-27 22:06:48.616093 pysmartdatamodels-0.8.0.1/pysmartdatamodels/utils/__init__.py
+-rw-r--r--   0        0        0      207 2024-05-27 16:08:42.490753 pysmartdatamodels-0.8.0.1/pysmartdatamodels/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    85551 2024-05-27 16:08:42.502753 pysmartdatamodels-0.8.0.1/pysmartdatamodels/utils/__pycache__/common_utils.cpython-311.pyc
+-rw-r--r--   0        0        0    81253 2024-04-12 12:10:43.397908 pysmartdatamodels-0.8.0.1/pysmartdatamodels/utils/common_utils.py
+-rw-r--r--   0        0        0    31673 1970-01-01 00:00:00.000000 pysmartdatamodels-0.8.0.1/PKG-INFO
```

### Comparing `pysmartdatamodels-0.8/pyproject.toml` & `pysmartdatamodels-0.8.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "pysmartdatamodels"
 repository = "https://github.com/smart-data-models/data-models/tree/master/pysmartdatamodels"
 description = "Open-licensed and free data models to model your digital twins, share data in data spaces or develop smart applications"
-version = "0.8"
+version = "0.8.0.1"
 authors = ["aabella <alberto.abella@fiware.org>", "jilin <jilin.he@fiware.org>"]
 readme = "./pysmartdatamodels/README.md"
 packages = [{include = "pysmartdatamodels"}]
 homepage = "https://github.com/smart-data-models/data-models/tree/master/pysmartdatamodels"
 classifiers = [
   "Development Status :: 4 - Beta",
   "Intended Audience :: Developers",
@@ -41,34 +41,34 @@
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11"
 ]
-dependencies = ["jsonref", "jsonschema", "pytz", "requests", "os-sys", "urllib.request", "rstr", "Faker", "string", "random", "fuzzywuzzy", "ruamel.yaml", "re", "pytz", "date-time", "json"]
-version = "0.8"
+dependencies = ["jsonref", "jsonschema", "pytz", "requests", "os-sys", "rstr", "Faker", "fuzzywuzzy", "python-Levenshtein", "ruamel.yaml", "date-time", "validator_collection"]
+version = "0.8.0.1"
 readme = "README.md"
 
 [project.urls]
 homepage = "https://github.com/smart-data-models/data-models/tree/master/pysmartdatamodels"
 bugTracker = "https://github.com/smart-data-models/data-models/issues"
 documentation = "https://github.com/smart-data-models/data-models/blob/master/pysmartdatamodels/README.md"
 issues = "https://github.com/smart-data-models/data-models/issues"
 source = "https://github.com/smart-data-models/data-models/tree/master/pysmartdatamodels"
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
 jsonref = ">=1.0.0"
 jsonschema = "^4.17.3"
-pytz = ">=2022.7.1, <2023.0.0"
+pytz = ">=2022.7.1"
 requests =  "^2.28.2"
 rstr = "^3.2.1"
-Faker = "^18.10.1"
+Faker = ">=18.10.1"
 urllib3 = "^2.0.7"
 validator-collection = "^1.5.0"
 fuzzywuzzy = ">=0.18"
 python-Levenshtein =">=0.25"
 "ruamel.yaml" = ">=0.18.1"
```

### Comparing `pysmartdatamodels-0.8/pysmartdatamodels/LICENSE.txt` & `pysmartdatamodels-0.8.0.1/pysmartdatamodels/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pysmartdatamodels-0.8/pysmartdatamodels/README.md` & `pysmartdatamodels-0.8.0.1/pysmartdatamodels/README.md`

 * *Files identical despite different names*

### Comparing `pysmartdatamodels-0.8/pysmartdatamodels/changes_log.md` & `pysmartdatamodels-0.8.0.1/pysmartdatamodels/changes_log.md`

 * *Files 15% similar despite different names*

```diff
@@ -23,8 +23,13 @@
 - for this function to be shown it has to be included a function to load the content open_jsonref
 - Extending the README.md  
 
 # version 0.8
 - No longer required the from pysmartdatamodels import pysmartdatamodels. therefore the usual code import line will be:
 - import pysmartdatamodels as sdm
 - Fix errors in __init__.py
-- Extended descriptions in README.md 
+- Extended descriptions in README.md 
+
+# version 0.8.0.1
+- Fix errors in __init__.py
+- Fix missing packages in dependencies section
+
```

### Comparing `pysmartdatamodels-0.8/pysmartdatamodels/deleteme.py` & `pysmartdatamodels-0.8.0.1/pysmartdatamodels/deleteme.py`

 * *Files identical despite different names*

### Comparing `pysmartdatamodels-0.8/pysmartdatamodels/model-assets/datamodels_metadata.json` & `pysmartdatamodels-0.8.0.1/pysmartdatamodels/model-assets/datamodels_metadata.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999805159379628%*

 * *Differences: {'102': "{'version': '0.0.9'}"}*

```diff
@@ -3327,15 +3327,15 @@
         "spec_IT": "https://raw.githubusercontent.com/smart-data-models/dataModel.Device/master/Device/doc/spec_IT.md",
         "spec_JA": "https://raw.githubusercontent.com/smart-data-models/dataModel.Device/master/Device/doc/spec_JA.md",
         "spec_KO": "https://raw.githubusercontent.com/smart-data-models/dataModel.Device/master/Device/doc/spec_KO.md",
         "spec_ZH": "https://raw.githubusercontent.com/smart-data-models/dataModel.Device/master/Device/doc/spec_ZH.md",
         "sql": "https://raw.githubusercontent.com/smart-data-models/dataModel.Device/master/Device/schema.sql",
         "subject": "dataModel.Device",
         "title": " Smart Data Models - Device schema",
-        "version": "0.0.8",
+        "version": "0.0.9",
         "yamlUrl": "https://raw.githubusercontent.com/smart-data-models/dataModel.Device/master/Device/model.yaml"
     },
     {
         "$id": "https://smart-data-models.github.io/dataModel.Device/DeviceMeasurement/schema.json",
         "@context": "https://raw.githubusercontent.com/smart-data-models/dataModel.Device/master/context.jsonld",
         "adopters": "https://raw.githubusercontent.com/smart-data-models/dataModel.Device/master/DeviceMeasurement/ADOPTERS.yaml",
         "contributors": "https://raw.githubusercontent.com/smart-data-models/dataModel.Device/master/CONTRIBUTORS.yaml",
```

### Comparing `pysmartdatamodels-0.8/pysmartdatamodels/model-assets/official_list_data_models.json` & `pysmartdatamodels-0.8.0.1/pysmartdatamodels/model-assets/official_list_data_models.json`

 * *Files identical despite different names*

### Comparing `pysmartdatamodels-0.8/pysmartdatamodels/model-assets/smartdatamodels.json` & `pysmartdatamodels-0.8.0.1/pysmartdatamodels/model-assets/smartdatamodels.json`

 * *Files identical despite different names*

### Comparing `pysmartdatamodels-0.8/pysmartdatamodels/my_subject/my_datamodel/examples/example-normalized.json` & `pysmartdatamodels-0.8.0.1/pysmartdatamodels/my_subject/my_datamodel/examples/example-normalized.json`

 * *Files identical despite different names*

### Comparing `pysmartdatamodels-0.8/pysmartdatamodels/my_subject/my_datamodel/examples/example-normalized.jsonld` & `pysmartdatamodels-0.8.0.1/pysmartdatamodels/my_subject/my_datamodel/examples/example-normalized.jsonld`

 * *Files identical despite different names*

### Comparing `pysmartdatamodels-0.8/pysmartdatamodels/my_subject/my_datamodel/examples/example.json` & `pysmartdatamodels-0.8.0.1/pysmartdatamodels/my_subject/my_datamodel/examples/example.json`

 * *Files identical despite different names*

### Comparing `pysmartdatamodels-0.8/pysmartdatamodels/my_subject/my_datamodel/examples/example.jsonld` & `pysmartdatamodels-0.8.0.1/pysmartdatamodels/my_subject/my_datamodel/examples/example.jsonld`

 * *Files identical despite different names*

### Comparing `pysmartdatamodels-0.8/pysmartdatamodels/pysmartdatamodels.py` & `pysmartdatamodels-0.8.0.1/pysmartdatamodels/pysmartdatamodels.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import pytz
 import requests
 
 from jsonschema import validate, Draft202012Validator
 
 import urllib.request
 
-from utils.common_utils import extract_subject_from_raw_url, extract_datamodel_from_raw_url, open_jsonref, parse_property2ngsild_example, normalized2keyvalues_v2, create_context, generate_random_string, is_metadata_properly_reported, is_metadata_existed,  schema_output_sum, message_after_check_schema, open_yaml, is_url_existed,  parse_payload_v2, parse_yamlDict
+from pysmartdatamodels.utils.common_utils import extract_subject_from_raw_url, extract_datamodel_from_raw_url, open_jsonref, parse_property2ngsild_example, normalized2keyvalues_v2, create_context, generate_random_string, is_metadata_properly_reported, is_metadata_existed,  schema_output_sum, message_after_check_schema, open_yaml, is_url_existed,  parse_payload_v2, parse_yamlDict
 
 
 path = __file__
 
 # Find the index of the last occurrence of /
 index = path.rfind(os.sep)
```

### Comparing `pysmartdatamodels-0.8/pysmartdatamodels/test/test_pysmartdatamodels.py` & `pysmartdatamodels-0.8.0.1/pysmartdatamodels/test/test_pysmartdatamodels.py`

 * *Files identical despite different names*

### Comparing `pysmartdatamodels-0.8/pysmartdatamodels/utils/__pycache__/common_utils.cpython-311.pyc` & `pysmartdatamodels-0.8.0.1/pysmartdatamodels/utils/__pycache__/common_utils.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -159,71 +159,71 @@
                 188 LOAD_CONST              16 (('well documented', 'already used', 'newly available', 'Metadata', 'Failed'))
                 190 LIST_EXTEND              1
                 192 STORE_NAME              29 (CHECKED_PROPERTY_CASES)
    
      55         194 LOAD_CONST              17 ('https://github\\.com/([^/]+)/([^/]+)/blob/([^/]+)/(.+)')
                 196 STORE_NAME              30 (github_url_pattern)
    
-     57         198 LOAD_CONST              18 (<code object is_url_existed, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 57>)
+     57         198 LOAD_CONST              18 (<code object is_url_existed, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 57>)
                 200 MAKE_FUNCTION            0
                 202 STORE_NAME              31 (is_url_existed)
    
      86         204 LOAD_CONST              19 ('fileUrl')
                 206 LOAD_NAME               32 (str)
                 208 BUILD_TUPLE              2
-                210 LOAD_CONST              20 (<code object open_json, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 86>)
+                210 LOAD_CONST              20 (<code object open_json, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 86>)
                 212 MAKE_FUNCTION            4 (annotations)
                 214 STORE_NAME              33 (open_json)
    
     117         216 LOAD_CONST              19 ('fileUrl')
                 218 LOAD_NAME               32 (str)
                 220 BUILD_TUPLE              2
-                222 LOAD_CONST              21 (<code object open_jsonref, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 117>)
+                222 LOAD_CONST              21 (<code object open_jsonref, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 117>)
                 224 MAKE_FUNCTION            4 (annotations)
                 226 STORE_NAME              34 (open_jsonref)
    
-    150         228 LOAD_CONST              22 (<code object open_yaml, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 150>)
+    150         228 LOAD_CONST              22 (<code object open_yaml, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 150>)
                 230 MAKE_FUNCTION            0
                 232 STORE_NAME              35 (open_yaml)
    
     179         234 LOAD_CONST              23 ('schemaUrl')
                 236 LOAD_NAME               32 (str)
                 238 LOAD_CONST              24 ('return')
                 240 LOAD_NAME               32 (str)
                 242 BUILD_TUPLE              4
-                244 LOAD_CONST              25 (<code object extract_datamodel_from_raw_url, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 179>)
+                244 LOAD_CONST              25 (<code object extract_datamodel_from_raw_url, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 179>)
                 246 MAKE_FUNCTION            4 (annotations)
                 248 STORE_NAME              36 (extract_datamodel_from_raw_url)
    
     209         250 LOAD_CONST              23 ('schemaUrl')
                 252 LOAD_NAME               32 (str)
                 254 LOAD_CONST              24 ('return')
                 256 LOAD_NAME               32 (str)
                 258 BUILD_TUPLE              4
-                260 LOAD_CONST              26 (<code object extract_subject_from_raw_url, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 209>)
+                260 LOAD_CONST              26 (<code object extract_subject_from_raw_url, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 209>)
                 262 MAKE_FUNCTION            4 (annotations)
                 264 STORE_NAME              37 (extract_subject_from_raw_url)
    
     238         266 LOAD_CONST              27 ('subject')
                 268 LOAD_NAME               32 (str)
                 270 LOAD_CONST              24 ('return')
                 272 LOAD_NAME               32 (str)
                 274 BUILD_TUPLE              4
-                276 LOAD_CONST              28 (<code object create_context, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 238>)
+                276 LOAD_CONST              28 (<code object create_context, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 238>)
                 278 MAKE_FUNCTION            4 (annotations)
                 280 STORE_NAME              38 (create_context)
    
     258         282 LOAD_NAME               39 (DeprecationWarning)
    
     259         284 LOAD_CONST              29 ('normalizedPayload')
                 286 LOAD_NAME               40 (dict)
                 288 LOAD_CONST              24 ('return')
                 290 LOAD_NAME               40 (dict)
                 292 BUILD_TUPLE              4
-                294 LOAD_CONST              30 (<code object normalized2keyvalues, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 258>)
+                294 LOAD_CONST              30 (<code object normalized2keyvalues, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 258>)
                 296 MAKE_FUNCTION            4 (annotations)
    
     258         298 PRECALL                  0
                 302 CALL                     0
    
     259         312 STORE_NAME              41 (normalized2keyvalues)
    
@@ -231,15 +231,15 @@
                 316 LOAD_CONST              29 ('normalizedPayload')
                 318 LOAD_NAME               40 (dict)
                 320 LOAD_CONST              31 ('level')
                 322 LOAD_NAME               42 (int)
                 324 LOAD_CONST              24 ('return')
                 326 LOAD_NAME               40 (dict)
                 328 BUILD_TUPLE              6
-                330 LOAD_CONST              32 (<code object normalized2keyvalues_v2, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 326>)
+                330 LOAD_CONST              32 (<code object normalized2keyvalues_v2, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 326>)
                 332 MAKE_FUNCTION            5 (defaults, annotations)
                 334 STORE_NAME              43 (normalized2keyvalues_v2)
    
     387         336 LOAD_CONST             103 ((True, 0))
                 338 LOAD_CONST              34 ('keyvaluesPayload')
                 340 LOAD_NAME               40 (dict)
                 342 LOAD_CONST              35 ('yamlDict')
@@ -247,173 +247,173 @@
                 346 LOAD_CONST              36 ('detailed')
                 348 LOAD_NAME               44 (bool)
                 350 LOAD_CONST              31 ('level')
                 352 LOAD_NAME               42 (int)
                 354 LOAD_CONST              24 ('return')
                 356 LOAD_NAME               40 (dict)
                 358 BUILD_TUPLE             10
-                360 LOAD_CONST              37 (<code object keyvalues2normalized_ngsild, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 387>)
+                360 LOAD_CONST              37 (<code object keyvalues2normalized_ngsild, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 387>)
                 362 MAKE_FUNCTION            5 (defaults, annotations)
                 364 STORE_NAME              45 (keyvalues2normalized_ngsild)
    
     514         366 LOAD_CONST             104 ((True,))
-                368 LOAD_CONST              38 (<code object keyvalues2normalized_ngsiv2, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 514>)
+                368 LOAD_CONST              38 (<code object keyvalues2normalized_ngsiv2, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 514>)
                 370 MAKE_FUNCTION            1 (defaults)
                 372 STORE_NAME              46 (keyvalues2normalized_ngsiv2)
    
     615         374 LOAD_CONST             105 ((4,))
                 376 LOAD_CONST              24 ('return')
                 378 LOAD_NAME               32 (str)
                 380 BUILD_TUPLE              2
-                382 LOAD_CONST              40 (<code object generate_random_string, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 615>)
+                382 LOAD_CONST              40 (<code object generate_random_string, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 615>)
                 384 MAKE_FUNCTION            5 (defaults, annotations)
                 386 STORE_NAME              47 (generate_random_string)
    
     635         388 LOAD_CONST              41 ('propertyName')
                 390 LOAD_NAME               32 (str)
                 392 LOAD_CONST              42 ('dataModel')
                 394 LOAD_NAME               32 (str)
                 396 LOAD_CONST              24 ('return')
                 398 LOAD_NAME               32 (str)
                 400 BUILD_TUPLE              6
-                402 LOAD_CONST              43 (<code object fake_uri, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 635>)
+                402 LOAD_CONST              43 (<code object fake_uri, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 635>)
                 404 MAKE_FUNCTION            4 (annotations)
                 406 STORE_NAME              48 (fake_uri)
    
     652         408 LOAD_CONST              41 ('propertyName')
                 410 LOAD_NAME               32 (str)
                 412 LOAD_CONST              42 ('dataModel')
                 414 LOAD_NAME               32 (str)
                 416 LOAD_CONST              24 ('return')
                 418 LOAD_NAME               40 (dict)
                 420 BUILD_TUPLE              6
-                422 LOAD_CONST              44 (<code object payload_uri, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 652>)
+                422 LOAD_CONST              44 (<code object payload_uri, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 652>)
                 424 MAKE_FUNCTION            4 (annotations)
                 426 STORE_NAME              49 (payload_uri)
    
-    666         428 LOAD_CONST              45 (<code object payload_relationship, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 666>)
+    666         428 LOAD_CONST              45 (<code object payload_relationship, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 666>)
                 430 MAKE_FUNCTION            0
                 432 STORE_NAME              50 (payload_relationship)
    
     683         434 LOAD_CONST              46 ('geo_type')
                 436 LOAD_NAME               32 (str)
                 438 LOAD_CONST              24 ('return')
                 440 LOAD_NAME               40 (dict)
                 442 BUILD_TUPLE              4
-                444 LOAD_CONST              47 (<code object fake_geoproperty, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 683>)
+                444 LOAD_CONST              47 (<code object fake_geoproperty, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 683>)
                 446 MAKE_FUNCTION            4 (annotations)
                 448 STORE_NAME              51 (fake_geoproperty)
    
     719         450 LOAD_CONST              46 ('geo_type')
                 452 LOAD_NAME               32 (str)
                 454 LOAD_CONST              24 ('return')
                 456 LOAD_NAME               40 (dict)
                 458 BUILD_TUPLE              4
-                460 LOAD_CONST              48 (<code object payload_geoproperty, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 719>)
+                460 LOAD_CONST              48 (<code object payload_geoproperty, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 719>)
                 462 MAKE_FUNCTION            4 (annotations)
                 464 STORE_NAME              52 (payload_geoproperty)
    
     736         466 LOAD_CONST              24 ('return')
                 468 LOAD_NAME               53 (float)
                 470 BUILD_TUPLE              2
-                472 LOAD_CONST              49 (<code object fake_number, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 736>)
+                472 LOAD_CONST              49 (<code object fake_number, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 736>)
                 474 MAKE_FUNCTION            4 (annotations)
                 476 STORE_NAME              54 (fake_number)
    
     772         478 LOAD_CONST              24 ('return')
                 480 LOAD_NAME               42 (int)
                 482 BUILD_TUPLE              2
-                484 LOAD_CONST              50 (<code object fake_integer, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 772>)
+                484 LOAD_CONST              50 (<code object fake_integer, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 772>)
                 486 MAKE_FUNCTION            4 (annotations)
                 488 STORE_NAME              55 (fake_integer)
    
     805         490 LOAD_CONST              24 ('return')
                 492 LOAD_NAME               40 (dict)
                 494 BUILD_TUPLE              2
-                496 LOAD_CONST              51 (<code object payload_number, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 805>)
+                496 LOAD_CONST              51 (<code object payload_number, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 805>)
                 498 MAKE_FUNCTION            4 (annotations)
                 500 STORE_NAME              56 (payload_number)
    
     830         502 LOAD_CONST              24 ('return')
                 504 LOAD_NAME               40 (dict)
                 506 BUILD_TUPLE              2
-                508 LOAD_CONST              52 (<code object payload_integer, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 830>)
+                508 LOAD_CONST              52 (<code object payload_integer, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 830>)
                 510 MAKE_FUNCTION            4 (annotations)
                 512 STORE_NAME              57 (payload_integer)
    
     851         514 LOAD_CONST              24 ('return')
                 516 LOAD_NAME               32 (str)
                 518 BUILD_TUPLE              2
-                520 LOAD_CONST              53 (<code object fake_datetime, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 851>)
+                520 LOAD_CONST              53 (<code object fake_datetime, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 851>)
                 522 MAKE_FUNCTION            4 (annotations)
                 524 STORE_NAME              58 (fake_datetime)
    
     865         526 LOAD_CONST              24 ('return')
                 528 LOAD_NAME               32 (str)
                 530 BUILD_TUPLE              2
-                532 LOAD_CONST              54 (<code object fake_date, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 865>)
+                532 LOAD_CONST              54 (<code object fake_date, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 865>)
                 534 MAKE_FUNCTION            4 (annotations)
                 536 STORE_NAME              59 (fake_date)
    
     878         538 LOAD_CONST              24 ('return')
                 540 LOAD_NAME               32 (str)
                 542 BUILD_TUPLE              2
-                544 LOAD_CONST              55 (<code object fake_time, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 878>)
+                544 LOAD_CONST              55 (<code object fake_time, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 878>)
                 546 MAKE_FUNCTION            4 (annotations)
                 548 STORE_NAME              60 (fake_time)
    
     891         550 LOAD_CONST              24 ('return')
                 552 LOAD_NAME               40 (dict)
                 554 BUILD_TUPLE              2
-                556 LOAD_CONST              56 (<code object payload_datetime, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 891>)
+                556 LOAD_CONST              56 (<code object payload_datetime, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 891>)
                 558 MAKE_FUNCTION            4 (annotations)
                 560 STORE_NAME              61 (payload_datetime)
    
     904         562 LOAD_CONST              24 ('return')
                 564 LOAD_NAME               40 (dict)
                 566 BUILD_TUPLE              2
-                568 LOAD_CONST              57 (<code object payload_date, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 904>)
+                568 LOAD_CONST              57 (<code object payload_date, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 904>)
                 570 MAKE_FUNCTION            4 (annotations)
                 572 STORE_NAME              62 (payload_date)
    
     917         574 LOAD_CONST              24 ('return')
                 576 LOAD_NAME               40 (dict)
                 578 BUILD_TUPLE              2
-                580 LOAD_CONST              58 (<code object payload_time, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 917>)
+                580 LOAD_CONST              58 (<code object payload_time, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 917>)
                 582 MAKE_FUNCTION            4 (annotations)
                 584 STORE_NAME              63 (payload_time)
    
     930         586 LOAD_CONST              42 ('dataModel')
                 588 LOAD_NAME               32 (str)
                 590 LOAD_CONST              24 ('return')
                 592 LOAD_NAME               32 (str)
                 594 BUILD_TUPLE              4
-                596 LOAD_CONST              59 (<code object fake_email, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 930>)
+                596 LOAD_CONST              59 (<code object fake_email, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 930>)
                 598 MAKE_FUNCTION            4 (annotations)
                 600 STORE_NAME              64 (fake_email)
    
     958         602 LOAD_CONST              42 ('dataModel')
                 604 LOAD_NAME               32 (str)
                 606 LOAD_CONST              24 ('return')
                 608 LOAD_NAME               40 (dict)
                 610 BUILD_TUPLE              4
-                612 LOAD_CONST              60 (<code object payload_email, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 958>)
+                612 LOAD_CONST              60 (<code object payload_email, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 958>)
                 614 MAKE_FUNCTION            4 (annotations)
                 616 STORE_NAME              65 (payload_email)
    
     975         618 LOAD_CONST              61 ('length')
                 620 LOAD_NAME               42 (int)
                 622 LOAD_CONST              62 ('min_length')
                 624 LOAD_NAME               42 (int)
                 626 LOAD_CONST              63 ('max_length')
                 628 LOAD_NAME               42 (int)
                 630 LOAD_CONST              24 ('return')
                 632 LOAD_NAME               32 (str)
                 634 BUILD_TUPLE              8
-                636 LOAD_CONST              64 (<code object fake_string, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 975>)
+                636 LOAD_CONST              64 (<code object fake_string, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 975>)
                 638 MAKE_FUNCTION            4 (annotations)
                 640 STORE_NAME              66 (fake_string)
    
     999         642 LOAD_CONST             106 (('',))
                 644 LOAD_CONST              61 ('length')
                 646 LOAD_NAME               42 (int)
                 648 LOAD_CONST              62 ('min_length')
@@ -421,160 +421,160 @@
                 652 LOAD_CONST              63 ('max_length')
                 654 LOAD_NAME               42 (int)
                 656 LOAD_CONST              66 ('pattern')
                 658 LOAD_NAME               32 (str)
                 660 LOAD_CONST              24 ('return')
                 662 LOAD_NAME               40 (dict)
                 664 BUILD_TUPLE             10
-                666 LOAD_CONST              67 (<code object payload_string, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 999>)
+                666 LOAD_CONST              67 (<code object payload_string, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 999>)
                 668 MAKE_FUNCTION            5 (defaults, annotations)
                 670 STORE_NAME              67 (payload_string)
    
    1022         672 LOAD_CONST              68 ('elements_list')
                 674 LOAD_NAME               68 (list)
                 676 LOAD_CONST              61 ('length')
                 678 LOAD_NAME               42 (int)
                 680 LOAD_CONST              24 ('return')
                 682 LOAD_NAME               32 (str)
                 684 BUILD_TUPLE              6
-                686 LOAD_CONST              69 (<code object fake_enum, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 1022>)
+                686 LOAD_CONST              69 (<code object fake_enum, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 1022>)
                 688 MAKE_FUNCTION            4 (annotations)
                 690 STORE_NAME              69 (fake_enum)
    
    1042         692 LOAD_CONST              68 ('elements_list')
                 694 LOAD_NAME               68 (list)
                 696 LOAD_CONST              61 ('length')
                 698 LOAD_NAME               42 (int)
                 700 LOAD_CONST              24 ('return')
                 702 LOAD_NAME               40 (dict)
                 704 BUILD_TUPLE              6
-                706 LOAD_CONST              70 (<code object payload_enum, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 1042>)
+                706 LOAD_CONST              70 (<code object payload_enum, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 1042>)
                 708 MAKE_FUNCTION            4 (annotations)
                 710 STORE_NAME              70 (payload_enum)
    
    1060         712 LOAD_CONST              24 ('return')
                 714 LOAD_NAME               44 (bool)
                 716 BUILD_TUPLE              2
-                718 LOAD_CONST              71 (<code object fake_boolean, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 1060>)
+                718 LOAD_CONST              71 (<code object fake_boolean, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 1060>)
                 720 MAKE_FUNCTION            4 (annotations)
                 722 STORE_NAME              71 (fake_boolean)
    
    1073         724 LOAD_CONST              24 ('return')
                 726 LOAD_NAME               40 (dict)
                 728 BUILD_TUPLE              2
-                730 LOAD_CONST              72 (<code object payload_boolean, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 1073>)
+                730 LOAD_CONST              72 (<code object payload_boolean, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 1073>)
                 732 MAKE_FUNCTION            4 (annotations)
                 734 STORE_NAME              72 (payload_boolean)
    
    1087         736 LOAD_CONST              24 ('return')
                 738 LOAD_NAME                8 (Tuple)
                 740 LOAD_NAME                7 (Dict)
                 742 LOAD_NAME               32 (str)
                 744 BUILD_TUPLE              2
                 746 BINARY_SUBSCR
                 756 BUILD_TUPLE              2
-                758 LOAD_CONST              73 (<code object parse_schema_description, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 1087>)
+                758 LOAD_CONST              73 (<code object parse_schema_description, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 1087>)
                 760 MAKE_FUNCTION            4 (annotations)
                 762 STORE_NAME              73 (parse_schema_description)
    
    1133         764 LOAD_CONST              74 ('concept')
                 766 LOAD_NAME               32 (str)
                 768 LOAD_CONST              24 ('return')
                 770 LOAD_CONST               1 (None)
                 772 BUILD_TUPLE              4
-                774 LOAD_CONST              75 (<code object echo, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 1133>)
+                774 LOAD_CONST              75 (<code object echo, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 1133>)
                 776 MAKE_FUNCTION            4 (annotations)
                 778 STORE_NAME              74 (echo)
    
    1152         780 LOAD_CONST             107 ((None,))
                 782 LOAD_CONST              76 ('type')
                 784 LOAD_NAME               32 (str)
                 786 LOAD_CONST              77 ('numItems')
                 788 LOAD_NAME               42 (int)
                 790 LOAD_CONST              24 ('return')
                 792 LOAD_NAME               68 (list)
                 794 BUILD_TUPLE              6
-                796 LOAD_CONST              78 (<code object fake_array, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 1152>)
+                796 LOAD_CONST              78 (<code object fake_array, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 1152>)
                 798 MAKE_FUNCTION            5 (defaults, annotations)
                 800 STORE_NAME              75 (fake_array)
    
    1187         802 LOAD_CONST              76 ('type')
                 804 LOAD_NAME               32 (str)
                 806 LOAD_CONST              77 ('numItems')
                 808 LOAD_NAME               42 (int)
                 810 LOAD_CONST              24 ('return')
                 812 LOAD_NAME               40 (dict)
                 814 BUILD_TUPLE              6
-                816 LOAD_CONST              79 (<code object payload_array, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 1187>)
+                816 LOAD_CONST              79 (<code object payload_array, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 1187>)
                 818 MAKE_FUNCTION            4 (annotations)
                 820 STORE_NAME              76 (payload_array)
    
-   1214         822 LOAD_CONST              80 (<code object parse_property, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 1214>)
+   1214         822 LOAD_CONST              80 (<code object parse_property, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 1214>)
                 824 MAKE_FUNCTION            0
                 826 STORE_NAME              77 (parse_property)
    
    1330         828 LOAD_CONST             102 ((0,))
                 830 LOAD_CONST              81 ('fullPayload')
                 832 LOAD_NAME               40 (dict)
                 834 LOAD_CONST              42 ('dataModel')
                 836 LOAD_NAME               32 (str)
                 838 LOAD_CONST              31 ('level')
                 840 LOAD_NAME               42 (int)
                 842 LOAD_CONST              24 ('return')
                 844 LOAD_NAME               40 (dict)
                 846 BUILD_TUPLE              8
-                848 LOAD_CONST              82 (<code object parse_property2ngsild_example, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 1330>)
+                848 LOAD_CONST              82 (<code object parse_property2ngsild_example, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 1330>)
                 850 MAKE_FUNCTION            5 (defaults, annotations)
                 852 STORE_NAME              78 (parse_property2ngsild_example)
    
    1538         854 LOAD_CONST              83 ('dict_a')
                 856 LOAD_NAME               40 (dict)
                 858 LOAD_CONST              84 ('dict_b')
                 860 LOAD_NAME               40 (dict)
                 862 LOAD_CONST              24 ('return')
                 864 LOAD_NAME               40 (dict)
                 866 BUILD_TUPLE              6
-                868 LOAD_CONST              85 (<code object merge_duplicate_attributes, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 1538>)
+                868 LOAD_CONST              85 (<code object merge_duplicate_attributes, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 1538>)
                 870 MAKE_FUNCTION            4 (annotations)
                 872 STORE_NAME              79 (merge_duplicate_attributes)
    
    1561         874 LOAD_CONST             108 ((1,))
                 876 LOAD_CONST              31 ('level')
                 878 LOAD_NAME               42 (int)
                 880 LOAD_CONST              24 ('return')
                 882 LOAD_NAME                8 (Tuple)
                 884 LOAD_NAME                7 (Dict)
                 886 LOAD_NAME                7 (Dict)
                 888 BUILD_TUPLE              2
                 890 BINARY_SUBSCR
                 900 BUILD_TUPLE              4
-                902 LOAD_CONST              87 (<code object parse_payload_v2, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 1561>)
+                902 LOAD_CONST              87 (<code object parse_payload_v2, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 1561>)
                 904 MAKE_FUNCTION            5 (defaults, annotations)
                 906 STORE_NAME              80 (parse_payload_v2)
    
    1695         908 LOAD_CONST             108 ((1,))
                 910 LOAD_CONST              88 ('datamodelRepoUrl')
                 912 LOAD_NAME               32 (str)
                 914 LOAD_CONST              31 ('level')
                 916 LOAD_NAME               42 (int)
                 918 LOAD_CONST              24 ('return')
                 920 LOAD_NAME               40 (dict)
                 922 BUILD_TUPLE              6
-                924 LOAD_CONST              89 (<code object parse_yamlDict, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 1695>)
+                924 LOAD_CONST              89 (<code object parse_yamlDict, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 1695>)
                 926 MAKE_FUNCTION            5 (defaults, annotations)
                 928 STORE_NAME              81 (parse_yamlDict)
    
    1823         930 LOAD_CONST              90 ('output')
                 932 LOAD_NAME               40 (dict)
                 934 LOAD_CONST              91 ('schemaDict')
                 936 LOAD_NAME               40 (dict)
                 938 LOAD_CONST              24 ('return')
                 940 LOAD_NAME               40 (dict)
                 942 BUILD_TUPLE              6
-                944 LOAD_CONST              92 (<code object is_metadata_properly_reported, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 1823>)
+                944 LOAD_CONST              92 (<code object is_metadata_properly_reported, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 1823>)
                 946 MAKE_FUNCTION            4 (annotations)
                 948 STORE_NAME              82 (is_metadata_properly_reported)
    
    1870         950 NOP
    
    1871         952 NOP
    
@@ -594,37 +594,37 @@
    1871         978 LOAD_NAME               68 (list)
    
    1870         980 LOAD_CONST              24 ('return')
    
    1871         982 LOAD_NAME               40 (dict)
    
    1870         984 BUILD_TUPLE             14
-                986 LOAD_CONST              97 (<code object is_metadata_existed, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 1870>)
+                986 LOAD_CONST              97 (<code object is_metadata_existed, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 1870>)
                 988 MAKE_FUNCTION            5 (defaults, annotations)
                 990 STORE_NAME              83 (is_metadata_existed)
    
    1963         992 LOAD_CONST              90 ('output')
                 994 LOAD_NAME               40 (dict)
                 996 LOAD_CONST              24 ('return')
                 998 LOAD_NAME               40 (dict)
                1000 BUILD_TUPLE              4
-               1002 LOAD_CONST              98 (<code object schema_output_sum, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 1963>)
+               1002 LOAD_CONST              98 (<code object schema_output_sum, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 1963>)
                1004 MAKE_FUNCTION            4 (annotations)
                1006 STORE_NAME              84 (schema_output_sum)
    
    2042        1008 LOAD_CONST              99 ('results')
                1010 LOAD_NAME               40 (dict)
                1012 LOAD_CONST              24 ('return')
                1014 LOAD_NAME               32 (str)
                1016 BUILD_TUPLE              4
-               1018 LOAD_CONST             100 (<code object message_after_check_schema, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 2042>)
+               1018 LOAD_CONST             100 (<code object message_after_check_schema, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 2042>)
                1020 MAKE_FUNCTION            4 (annotations)
                1022 STORE_NAME              85 (message_after_check_schema)
    
-   2094        1024 LOAD_CONST             101 (<code object convert_to_raw_github_url, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 2094>)
+   2094        1024 LOAD_CONST             101 (<code object convert_to_raw_github_url, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 2094>)
                1026 MAKE_FUNCTION            0
                1028 STORE_NAME              86 (convert_to_raw_github_url)
                1030 LOAD_CONST               1 (None)
                1032 RETURN_VALUE
    consts
       0
       None
@@ -706,15 +706,15 @@
             True
             False
             'wrong domain'
          names      ('requests', 'get', 'status_code', 'text')
          varnames   ('url', 'pointer')
          freevars   ()
          cellvars   ()
-         filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+         filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
          name       'is_url_existed'
          firstlineno 57
          lnotab 0x0213020128011601120214010201
       'fileUrl'
       code
          argcount  : 1
          nlocals   : 3
@@ -815,15 +815,15 @@
             'utf-8'
             None
             'r'
          names      ('requests', 'get', 'json', 'loads', 'content', 'decode', 'open', 'read')
          varnames   ('fileUrl', 'pointer', 'file')
          freevars   ()
          cellvars   ()
-         filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+         filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
          name       'open_json'
          firstlineno 86
          lnotab 0x020f1c02020128015a0102010c03020120014e010201
       code
          argcount  : 1
          nlocals   : 4
          stacksize : 5
@@ -934,15 +934,15 @@
             ('load_on_repr', 'merge_props')
             None
             'r'
          names      ('requests', 'get', 'jsonref', 'loads', 'content', 'decode', 'open', 'read')
          varnames   ('fileUrl', 'pointer', 'output', 'file')
          freevars   ()
          cellvars   ()
-         filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+         filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
          name       'open_jsonref'
          firstlineno 117
          lnotab 0x02101c02020128015e01060102010c030201200154010201
       code
          argcount  : 1
          nlocals   : 8
          stacksize : 6
@@ -1207,15 +1207,15 @@
             None
             'Failed to fetch content from URL: '
             'Error: '
          names      ('ruamel', 'yaml', 'YAML', 'os', 'path', 'splitext', 'lower', 'print', 'startswith', 're', 'match', 'github_url_pattern', 'convert_to_raw_github_url', 'requests', 'get', 'raise_for_status', 'load', 'content', 'decode', 'open', 'exceptions', 'RequestException', 'Exception')
          varnames   ('file_url', 'yaml', '_', 'file_extension', 'raw_github_url', 'response', 'file', 'e')
          freevars   ()
          cellvars   ()
-         filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+         filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
          name       'open_yaml'
          firstlineno 150
          lnotab
             0x020440010201440130011e022a0134011e01280128015a02280128015a
             02220128ff360226013801120138ff
       'schemaUrl'
       'return'
@@ -1303,15 +1303,15 @@
             'https:\\/\\/smart-data-models\\.github\\.io\\/.*\\/(.*)\\/schema\\.json'
             1
             'dataModel'
          names      ('re', 'search', 'IGNORECASE', 'group')
          varnames   ('schemaUrl', 're', 'patternRaw', 'patternPage', 'urlSearch', 'url2Search', 'dataModel')
          freevars   ()
          cellvars   ()
-         filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+         filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
          name       'extract_datamodel_from_raw_url'
          firstlineno 179
          lnotab 0x020f0802040104012e022e0104012c0104012c020401
       code
          argcount  : 1
          nlocals   : 7
          stacksize : 5
@@ -1411,15 +1411,15 @@
             1
             '/'
             'subject'
          names      ('re', 'search', 'IGNORECASE', 'group', 'split')
          varnames   ('schemaUrl', 're', 'patternRaw', 'patternPage', 'urlSearch', 'url2Search', 'subject')
          freevars   ()
          cellvars   ()
-         filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+         filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
          name       'extract_subject_from_raw_url'
          firstlineno 209
          lnotab 0x020f0801040104012e012e0104015e0104015e020401
       'subject'
       code
          argcount  : 1
          nlocals   : 1
@@ -1438,15 +1438,15 @@
             '\n    Creates the link to context.jsonld of given subject\n\n    Parameters:\n    - subject (str): The name of the subject.\n\n    Returns:\n    - str: The link of the context.jsonld\n\n    Example:\n    >>> create_context("dataModel.WasteWater")\n    \'https://smart-data-models.github.io/dataModel.WasteWater/context.jsonld\'\n    '
             'https://smart-data-models.github.io/'
             '/context.jsonld'
          names      ()
          varnames   ('subject',)
          freevars   ()
          cellvars   ()
-         filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+         filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
          name       'create_context'
          firstlineno 238
          lnotab 0x020e
       'normalizedPayload'
       code
          argcount  : 1
          nlocals   : 5
@@ -1545,15 +1545,15 @@
             'value'
             '@type'
             '@value'
          names      ()
          varnames   ('normalizedPayload', 'normalizedDict', 'output', 'element', 'value')
          freevars   ()
          cellvars   ()
-         filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+         filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
          name       'normalized2keyvalues'
          firstlineno 258
          lnotab 0x022d040104020801020314011c04080130020c021a0102012002
       'level'
       code
          argcount  : 2
          nlocals   : 6
@@ -1614,15 +1614,15 @@
                      132 LOAD_GLOBAL              6 (dict)
                      144 PRECALL                  2
                      148 CALL                     2
                      158 POP_JUMP_FORWARD_IF_FALSE    18 (to 196)
          
          343         160 LOAD_CLOSURE             1 (level)
                      162 BUILD_TUPLE              1
-                     164 LOAD_CONST               2 (<code object <listcomp>, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 343>)
+                     164 LOAD_CONST               2 (<code object <listcomp>, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 343>)
                      166 MAKE_FUNCTION            8 (closure)
                      168 LOAD_FAST                4 (body)
                      170 GET_ITER
                      172 PRECALL                  0
                      176 CALL                     0
                      186 LOAD_FAST                2 (output)
                      188 LOAD_FAST                3 (element)
@@ -1697,15 +1697,15 @@
                      470 LOAD_GLOBAL              6 (dict)
                      482 PRECALL                  2
                      486 CALL                     2
                      496 POP_JUMP_FORWARD_IF_FALSE    18 (to 534)
          
          364         498 LOAD_CLOSURE             1 (level)
                      500 BUILD_TUPLE              1
-                     502 LOAD_CONST               6 (<code object <listcomp>, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 364>)
+                     502 LOAD_CONST               6 (<code object <listcomp>, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 364>)
                      504 MAKE_FUNCTION            8 (closure)
          
          365         506 LOAD_FAST                5 (value)
          
          364         508 GET_ITER
                      510 PRECALL                  0
                      514 CALL                     0
@@ -1788,15 +1788,15 @@
                consts
                   1
                   'value'
                names      ('normalized2keyvalues_v2', 'get')
                varnames   ('.0', 'subprop')
                freevars   ('level',)
                cellvars   ()
-               filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+               filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
                name       '<listcomp>'
                firstlineno 343
                lnotab 0x
             '@value'
             'value'
             1
             code
@@ -1834,24 +1834,24 @@
                consts
                   1
                   'value'
                names      ('normalized2keyvalues_v2', 'get')
                varnames   ('.0', 'subvalue')
                freevars   ('level',)
                cellvars   ()
-               filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+               filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
                name       '<listcomp>'
                firstlineno 364
                lnotab 0x
             'object'
          names      ('items', 'isinstance', 'list', 'dict', 'normalized2keyvalues_v2')
          varnames   ('normalizedPayload', 'level', 'output', 'element', 'body', 'value')
          freevars   ()
          cellvars   ('level',)
-         filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+         filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
          name       'normalized2keyvalues_v2'
          firstlineno 326
          lnotab
             0x040b04013404640124032a0508011802080110032a013e046401080102
             ff1a050c0508011a040e040e02
       True
       'keyvaluesPayload'
@@ -1940,15 +1940,15 @@
                       24 LOAD_CONST               4 ('return')
                       26 LOAD_GLOBAL              4 (tuple)
                       38 LOAD_GLOBAL              6 (bool)
                       50 LOAD_GLOBAL              2 (str)
                       62 BUILD_TUPLE              2
                       64 BINARY_SUBSCR
                       74 BUILD_TUPLE              4
-                      76 LOAD_CONST               5 (<code object valid_date, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 402>)
+                      76 LOAD_CONST               5 (<code object valid_date, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 402>)
                       78 MAKE_FUNCTION            4 (annotations)
                       80 STORE_FAST               5 (valid_date)
          
          430          82 LOAD_FAST                0 (keyvaluesPayload)
                       84 STORE_FAST               6 (keyvaluesDict)
          
          431          86 BUILD_MAP                0
@@ -2596,15 +2596,15 @@
                   1
                   (True, 'DateTime')
                   (True, 'Date')
                names      ('re', 'datetime', 'time', 'fromisoformat', 'replace', 'split', 'match', 'ValueError', 'len')
                varnames   ('datestring', 're', 'time', 'date', 'validDate')
                freevars   ()
                cellvars   ()
-               filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+               filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
                name       'valid_date'
                firstlineno 402
                lnotab
                   0x020408010c0210010201560102010c010403360102012601120106ff08
                   0304014c0104010402
             ('id', 'type', '@context')
             'x-ngsi'
@@ -2627,15 +2627,15 @@
             '--- other type ---'
             'id'
             '@context'
          names      ('json', 'str', 'tuple', 'bool', 'isinstance', 'list', 'len', 'dict', 'range', 'append', 'keyvalues2normalized_ngsild', 'int', 'float', 'loads', 'print')
          varnames   ('keyvaluesPayload', 'yamlDict', 'detailed', 'level', 'json', 'valid_date', 'keyvaluesDict', 'output', 'element', 'item', 'tmpList', 'idx', 'dateFlag', 'dateType')
          freevars   ()
          cellvars   ()
-         filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+         filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
          name       'keyvalues2normalized_ngsild'
          firstlineno 387
          lnotab
             0x020d0802481c040104010a031601040236022e01040174010401480158
             0108ff22020e021a021a0236030c013001280130022e0104014c021a0236
             01280104022e010c0120010c01200220032e011a026c022e01180218022e
             01280218022e0128031e011e012a011e010e020801160108011601080116
@@ -2700,15 +2700,15 @@
                        8 STORE_FAST               2 (json)
          
          527          10 LOAD_CONST               3 ('datestring')
                       12 LOAD_GLOBAL              2 (str)
                       24 LOAD_CONST               4 ('return')
                       26 LOAD_GLOBAL              4 (bool)
                       38 BUILD_TUPLE              4
-                      40 LOAD_CONST               5 (<code object valid_date, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 527>)
+                      40 LOAD_CONST               5 (<code object valid_date, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 527>)
                       42 MAKE_FUNCTION            4 (annotations)
                       44 STORE_FAST               3 (valid_date)
          
          543          46 LOAD_FAST                0 (keyvaluesPayload)
                       48 STORE_FAST               4 (keyvaluesDict)
          
          544          50 BUILD_MAP                0
@@ -3135,15 +3135,15 @@
                   '^[0-9]{2,4}[-/][0-9]{2}[-/][0-9]{2,4}$'
                   False
                   True
                names      ('re', 'split', 'match', 'ValueError')
                varnames   ('datestring', 're', 'date', 'validDate')
                freevars   ()
                cellvars   ()
-               filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+               filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
                name       'valid_date'
                firstlineno 527
                lnotab 0x02040801360102012601120106ff080304010402
             'StructuredValue'
             'type'
             'value'
             'location'
@@ -3161,15 +3161,15 @@
             '--- other type ---'
             'id'
             '@context'
          names      ('json', 'str', 'bool', 'isinstance', 'list', 'len', 'dict', 'range', 'append', 'keyvalues2normalized_ngsiv2', 'int', 'float', 'loads', 'print')
          varnames   ('keyvaluesPayload', 'detailed', 'json', 'valid_date', 'keyvaluesDict', 'output', 'element', 'item', 'tmpList', 'idx')
          freevars   ()
          cellvars   ()
-         filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+         filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
          name       'keyvalues2normalized_ngsiv2'
          firstlineno 514
          lnotab
             0x020b08022410040104020a01040236030a0104017401040148015e010e
             021a021a0236020c010c020a01040134021a02360122020c030a0118026c
             020a01180218020a01280218020a0128031e011e012a011e010e02080122
             010801220108012202
@@ -3196,15 +3196,15 @@
                       48 BINARY_OP                0 (+)
                       52 STORE_DEREF              1 (characters)
          
          629          54 LOAD_CONST               1 ('')
                       56 LOAD_METHOD              3 (join)
                       78 LOAD_CLOSURE             1 (characters)
                       80 BUILD_TUPLE              1
-                      82 LOAD_CONST               2 (<code object <genexpr>, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 629>)
+                      82 LOAD_CONST               2 (<code object <genexpr>, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 629>)
                       84 MAKE_FUNCTION            8 (closure)
                       86 LOAD_GLOBAL              9 (NULL + range)
                       98 LOAD_FAST                0 (length)
                      100 PRECALL                  1
                      104 CALL                     1
                      114 GET_ITER
                      116 PRECALL                  0
@@ -3245,23 +3245,23 @@
                             62 RETURN_VALUE
                consts
                   None
                names      ('random', 'choice')
                varnames   ('.0', '_')
                freevars   ('characters',)
                cellvars   ()
-               filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+               filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
                name       '<genexpr>'
                firstlineno 629
                lnotab 0x
          names      ('string', 'ascii_letters', 'digits', 'join', 'range')
          varnames   ('length',)
          freevars   ()
          cellvars   ('characters',)
-         filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+         filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
          name       'generate_random_string'
          firstlineno 615
          lnotab 0x040d3201
       'propertyName'
       'dataModel'
       code
          argcount  : 2
@@ -3313,15 +3313,15 @@
             '????:########'
             'ABCDEFGHIJKLMNOPQRSTUVWXYZ'
             ('text', 'letters')
          names      ('str', 'fake', 'bothify')
          varnames   ('propertyName', 'dataModel', 'output')
          freevars   ()
          cellvars   ()
-         filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+         filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
          name       'fake_uri'
          firstlineno 635
          lnotab 0x020c50013e02
       code
          argcount  : 2
          nlocals   : 2
          stacksize : 5
@@ -3344,15 +3344,15 @@
             '\n       Generates a payload containing a URI value for a Property.\n       Parameters:\n       - propertyName (str): The name of the property.\n       - dataModel (str): The name of the data model.\n       Returns:\n       - dict: A payload containing a URI value.\n       Example:\n       >>> payload_uri("temperature", "WeatherObserved")\n       {\'type\': \'Property\', \'value\': \'urn:ngsi-ld:WeatherObserved:temperature:ABCD1234\'}\n       '
             'Property'
             ('type', 'value')
          names      ('fake_uri',)
          varnames   ('propertyName', 'dataModel')
          freevars   ()
          cellvars   ()
-         filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+         filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
          name       'payload_uri'
          firstlineno 652
          lnotab 0x020c
       code
          argcount  : 2
          nlocals   : 2
          stacksize : 5
@@ -3375,15 +3375,15 @@
             '\n        Generates a payload containing a URI value for a Relationship.\n        Parameters:\n        - propertyName (str): The name of the relationship property.\n        - dataModel (str): The name of the data model.\n        Returns:\n        - dict: A payload containing a relationship property.\n        Example:\n        >>> payload_relationship("belongsTo", "Building")\n        {\'type\': \'Relationship\', \'object\': \'urn:ngsi-ld:Building:belongsTo:ABCD1234\'}\n        TODO\n        Copy with different data structure relationships, like list and dict\n        '
             'object'
             ('type', 'value')
          names      ('fake_uri',)
          varnames   ('propertyName', 'dataModel')
          freevars   ()
          cellvars   ()
-         filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+         filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
          name       'payload_relationship'
          firstlineno 666
          lnotab 0x020e
       'geo_type'
       code
          argcount  : 1
          nlocals   : 2
@@ -3591,15 +3591,15 @@
             ('type', 'coordinates')
             'LineString'
             'Polygon'
          names      ('float', 'fake', 'latitude', 'longitude')
          varnames   ('geo_type', 'dict_value')
          freevars   ()
          cellvars   ()
-         filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+         filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
          name       'fake_geoproperty'
          firstlineno 683
          lnotab
             0x021104020c01a2010c010201960196fe0c040e01020196019601960196
             fc0807
       code
          argcount  : 1
@@ -3623,15 +3623,15 @@
             '\n    Generates a GeoJSON property payload with a fake geometry based on the given type.\n\n    Parameters:\n    - geo_type (str): The type of the geometry (e.g., "Point", "LineString", "Polygon").\n\n    Returns:\n    - dict: A GeoJSON property payload.\n\n    Example:\n    >>> payload_geoproperty("Point")\n    {\'type\': \'GeoProperty\', \'value\': {\'type\': \'Point\', \'coordinates\': [12.345, -67.890]}}\n    '
             'GeoProperty'
             ('type', 'value')
          names      ('fake_geoproperty',)
          varnames   ('geo_type',)
          freevars   ()
          cellvars   ()
-         filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+         filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
          name       'payload_geoproperty'
          firstlineno 719
          lnotab 0x020e
       code
          argcount  : 0
          nlocals   : 4
          stacksize : 6
@@ -3756,15 +3756,15 @@
             1
             2
             ('left_digits', 'right_digits', 'min_value', 'max_value')
          names      ('Faker', 'seed', 'isinstance', 'int', 'len', 'max', 'fake', 'pyfloat')
          varnames   ('args', 'left_digits', 'minimum', 'maximum')
          freevars   ()
          cellvars   ()
-         filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+         filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
          name       'fake_number'
          firstlineno 736
          lnotab 0x02172602360104010401060236016c018e02
       code
          argcount  : 0
          nlocals   : 3
          stacksize : 5
@@ -3871,15 +3871,15 @@
             0
             1
             1000
          names      ('Faker', 'seed', 'isinstance', 'int', 'len', 'max', 'fake', 'pyint')
          varnames   ('args', 'minimum', 'maximum')
          freevars   ()
          cellvars   ()
-         filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+         filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
          name       'fake_integer'
          firstlineno 772
          lnotab 0x021626023601040112026c018e02
       code
          argcount  : 0
          nlocals   : 1
          stacksize : 4
@@ -3898,15 +3898,15 @@
             "\n    Generates a payload for a fake number property based on the provided arguments.\n\n    Parameters:\n    - If only one argument is provided (an integer), it represents the maximum value (default is 1000).\n    - If more than one argument is provided as a tuple, the first element is the number of left digits (default is 6),\n      the second element is the minimum value (default is 0), and the third element is the maximum value\n      (default is maximum of 1000 or minimum + 1000).\n\n    Returns:\n    - dict: A payload dictionary with the type 'Property' and a fake number value.\n\n    Example:\n    >>> payload_number()\n    {'type': 'Property', 'value': 42.3}\n\n    >>> payload_number(50)\n    {'type': 'Property', 'value': 25.7}\n\n    >>> payload_number((6, 10, 50))\n    {'type': 'Property', 'value': 37.9}\n    "
             'Property'
             ('type', 'value')
          names      ('fake_number',)
          varnames   ('args',)
          freevars   ()
          cellvars   ()
-         filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+         filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
          name       'payload_number'
          firstlineno 805
          lnotab 0x0217
       code
          argcount  : 0
          nlocals   : 1
          stacksize : 4
@@ -3925,15 +3925,15 @@
             "\n    Generates a payload for a fake integer property based on the provided arguments.\n\n    Parameters:\n    - If only one argument is provided (an integer), it represents the maximum value (default is 1000).\n    - If more than one argument is provided as a tuple, the first element is the minimum value (default is 0),\n      and the second element is the maximum value (default is maximum of 1000 or minimum + 1000).\n\n    Returns:\n    - dict: A payload dictionary with the type 'Property' and a fake integer value.\n\n    Example:\n    >>> payload_integer()\n    {'type': 'Property', 'value': 42}\n\n    >>> payload_integer((10, 50))\n    {'type': 'Property', 'value': 37}\n    "
             'Property'
             ('type', 'value')
          names      ('fake_integer',)
          varnames   ('args',)
          freevars   ()
          cellvars   ()
-         filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+         filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
          name       'payload_integer'
          firstlineno 830
          lnotab 0x0213
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
@@ -3956,15 +3956,15 @@
             '%Y-%m-%dT%H:%M:%SZ'
             None
             ('pattern', 'end_datetime')
          names      ('fake', 'date')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+         filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
          name       'fake_datetime'
          firstlineno 851
          lnotab 0x020b
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
@@ -3987,15 +3987,15 @@
             '%Y-%m-%d'
             None
             ('pattern', 'end_datetime')
          names      ('fake', 'date')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+         filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
          name       'fake_date'
          firstlineno 865
          lnotab 0x020b
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
@@ -4018,15 +4018,15 @@
             '%H:%M:%SZ'
             None
             ('pattern', 'end_datetime')
          names      ('fake', 'date')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+         filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
          name       'fake_time'
          firstlineno 878
          lnotab 0x020b
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
@@ -4052,15 +4052,15 @@
             'DateTime'
             ('@type', '@value')
             ('type', 'value')
          names      ('fake_datetime',)
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+         filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
          name       'payload_datetime'
          firstlineno 891
          lnotab 0x020b
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
@@ -4086,15 +4086,15 @@
             'Date'
             ('@type', '@value')
             ('type', 'value')
          names      ('fake_date',)
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+         filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
          name       'payload_date'
          firstlineno 904
          lnotab 0x020b
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
@@ -4120,15 +4120,15 @@
             'Time'
             ('@type', '@value')
             ('type', 'value')
          names      ('fake_time',)
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+         filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
          name       'payload_time'
          firstlineno 917
          lnotab 0x020b
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 7
@@ -4193,15 +4193,15 @@
             0
             '.'
             '@'
          names      ('fake', 'random_choices', 'first_name', 'last_name', 'lower')
          varnames   ('dataModel', 'list_of_domains', 'dns_org')
          freevars   ()
          cellvars   ()
-         filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+         filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
          name       'fake_email'
          firstlineno 930
          lnotab 0x020e04072201020102fe100302fd0c05
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 4
@@ -4223,15 +4223,15 @@
             "\n    Generates a payload for a fake email property.\n\n    Parameters:\n    - dataModel (str): The data model to incorporate into the email address.\n\n    Returns:\n    - dict: A payload dictionary with the type 'Property' and a fake email value.\n\n    Example:\n    >>> payload_email('SmartCity')\n    {'type': 'Property', 'value': 'john.doe@smartcity.com'}\n    "
             'Property'
             ('type', 'value')
          names      ('fake_email',)
          varnames   ('dataModel',)
          freevars   ()
          cellvars   ()
-         filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+         filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
          name       'payload_email'
          firstlineno 958
          lnotab 0x020e
       'length'
       'min_length'
       'max_length'
       code
@@ -4289,15 +4289,15 @@
             ('nb',)
             0
             None
          names      ('random', 'randint', 'fake', 'paragraphs')
          varnames   ('length', 'min_length', 'max_length', 'paragraph_length')
          freevars   ()
          cellvars   ()
-         filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+         filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
          name       'fake_string'
          firstlineno 975
          lnotab 0x02102a030c015202
       ''
       'pattern'
       code
          argcount  : 4
@@ -4338,15 +4338,15 @@
             "\n    Generate a payload for a string property with optional pattern.\n\n    Parameters:\n    - length (int): Desired length of the string.\n    - min_length (int): Minimum possible length of the string.\n    - max_length (int): Maximum possible length of the string.\n    - pattern (str, optional): Regular expression pattern to match.\n\n    Returns:\n    - dict: Property payload.\n\n    Example:\n    >>> payload_string(1, 5, 10)\n    {'type': 'Property', 'value': 'Lorem ipsum'}\n    "
             'Property'
             ('type', 'value')
          names      ('rstr', 'xeger', 'fake_string')
          varnames   ('length', 'min_length', 'max_length', 'pattern')
          freevars   ()
          cellvars   ()
-         filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+         filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
          name       'payload_string'
          firstlineno 999
          lnotab 0x021104012e02
       'elements_list'
       code
          argcount  : 2
          nlocals   : 2
@@ -4389,15 +4389,15 @@
             1
             ('elements', 'length')
             0
          names      ('fake', 'random_choices')
          varnames   ('elements_list', 'length')
          freevars   ()
          cellvars   ()
-         filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+         filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
          name       'fake_enum'
          firstlineno 1022
          lnotab 0x020f0c014402
       code
          argcount  : 2
          nlocals   : 2
          stacksize : 5
@@ -4420,15 +4420,15 @@
             "\n    Generates a payload for a fake enum property.\n\n    Parameters:\n    - elements_list (list): The list of possible enum values.\n    - length (int): The number of enum values to generate.\n\n    Returns:\n    - dict: A payload dictionary with the type 'Property' and a fake enum value or values.\n\n    Example:\n    >>> payload_enum(['red', 'blue', 'green'], 3)\n    {'type': 'Property', 'value': ['red', 'blue', 'green']}\n    "
             'Property'
             ('type', 'value')
          names      ('fake_enum',)
          varnames   ('elements_list', 'length')
          freevars   ()
          cellvars   ()
-         filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+         filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
          name       'payload_enum'
          firstlineno 1042
          lnotab 0x020f
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
@@ -4458,15 +4458,15 @@
             1
             ('elements', 'length')
             0
          names      ('fake', 'random_choices')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+         filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
          name       'fake_boolean'
          firstlineno 1060
          lnotab 0x020b
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
@@ -4487,15 +4487,15 @@
             "\n    Generates a payload for a fake boolean property.\n\n    Returns:\n    - dict: A payload dictionary with the type 'Property' and a fake boolean value.\n\n    Example:\n    >>> payload_boolean()\n    {'type': 'Property', 'value': True}\n    "
             'Property'
             ('type', 'value')
          names      ('fake_boolean',)
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+         filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
          name       'payload_boolean'
          firstlineno 1073
          lnotab 0x020b
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 5
@@ -4778,15 +4778,15 @@
             'enum'
             'Privacy:'
             'privacy'
          names      ('replace', 'chr', 're', 'sub', 'split', 'list', 'copy', 'propertyTypes', 'remove', 'find', 'len', 'join')
          varnames   ('description', 'ngsiOutput', 'copiedDescription', 'item', 'raw')
          freevars   ()
          cellvars   ()
-         filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+         filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
          name       'parse_schema_description'
          firstlineno 1087
          lnotab
             0x020e040346012c022a0134020a0112010a012c0132012a015e0132012a
             015e0132012a015601340132012a0160022a02
       'concept'
       code
@@ -4836,15 +4836,15 @@
             '--- '
             ' ---'
             None
          names      ('print',)
          varnames   ('concept', 'variable')
          freevars   ()
          cellvars   ()
-         filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+         filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
          name       'echo'
          firstlineno 1133
          lnotab 0x020e2a011e01
       'type'
       'numItems'
       code
          argcount  : 3
@@ -4872,15 +4872,15 @@
          1172           4 LOAD_FAST                0 (type)
                         6 LOAD_CONST               1 ('number')
                         8 COMPARE_OP               2 (==)
                        14 POP_JUMP_FORWARD_IF_FALSE    27 (to 70)
          
          1173          16 LOAD_CLOSURE             2 (options)
                        18 BUILD_TUPLE              1
-                       20 LOAD_CONST               2 (<code object <listcomp>, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 1173>)
+                       20 LOAD_CONST               2 (<code object <listcomp>, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 1173>)
                        22 MAKE_FUNCTION            8 (closure)
                        24 LOAD_GLOBAL              1 (NULL + range)
                        36 LOAD_FAST                1 (numItems)
                        38 PRECALL                  1
                        42 CALL                     1
                        52 GET_ITER
                        54 PRECALL                  0
@@ -4888,15 +4888,15 @@
                        68 RETURN_VALUE
          
          1174     >>   70 LOAD_FAST                0 (type)
                        72 LOAD_CONST               3 ('boolean')
                        74 COMPARE_OP               2 (==)
                        80 POP_JUMP_FORWARD_IF_FALSE    25 (to 132)
          
-         1175          82 LOAD_CONST               4 (<code object <listcomp>, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 1175>)
+         1175          82 LOAD_CONST               4 (<code object <listcomp>, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 1175>)
                        84 MAKE_FUNCTION            0
                        86 LOAD_GLOBAL              1 (NULL + range)
                        98 LOAD_FAST                1 (numItems)
                       100 PRECALL                  1
                       104 CALL                     1
                       114 GET_ITER
                       116 PRECALL                  0
@@ -4906,15 +4906,15 @@
          1176     >>  132 LOAD_FAST                0 (type)
                       134 LOAD_CONST               5 ('string')
                       136 COMPARE_OP               2 (==)
                       142 POP_JUMP_FORWARD_IF_FALSE    27 (to 198)
          
          1177         144 LOAD_CLOSURE             2 (options)
                       146 BUILD_TUPLE              1
-                      148 LOAD_CONST               6 (<code object <listcomp>, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 1177>)
+                      148 LOAD_CONST               6 (<code object <listcomp>, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 1177>)
                       150 MAKE_FUNCTION            8 (closure)
                       152 LOAD_GLOBAL              1 (NULL + range)
                       164 LOAD_FAST                1 (numItems)
                       166 PRECALL                  1
                       170 CALL                     1
                       180 GET_ITER
                       182 PRECALL                  0
@@ -4922,15 +4922,15 @@
                       196 RETURN_VALUE
          
          1178     >>  198 LOAD_FAST                0 (type)
                       200 LOAD_CONST               7 ('date-time')
                       202 COMPARE_OP               2 (==)
                       208 POP_JUMP_FORWARD_IF_FALSE    25 (to 260)
          
-         1179         210 LOAD_CONST               8 (<code object <listcomp>, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 1179>)
+         1179         210 LOAD_CONST               8 (<code object <listcomp>, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 1179>)
                       212 MAKE_FUNCTION            0
                       214 LOAD_GLOBAL              1 (NULL + range)
                       226 LOAD_FAST                1 (numItems)
                       228 PRECALL                  1
                       232 CALL                     1
                       242 GET_ITER
                       244 PRECALL                  0
@@ -4940,15 +4940,15 @@
          1180     >>  260 LOAD_FAST                0 (type)
                       262 LOAD_CONST               9 ('enum')
                       264 COMPARE_OP               2 (==)
                       270 POP_JUMP_FORWARD_IF_FALSE    27 (to 326)
          
          1181         272 LOAD_CLOSURE             2 (options)
                       274 BUILD_TUPLE              1
-                      276 LOAD_CONST              10 (<code object <listcomp>, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 1181>)
+                      276 LOAD_CONST              10 (<code object <listcomp>, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 1181>)
                       278 MAKE_FUNCTION            8 (closure)
                       280 LOAD_GLOBAL              1 (NULL + range)
                       292 LOAD_FAST                1 (numItems)
                       294 PRECALL                  1
                       298 CALL                     1
                       308 GET_ITER
                       310 PRECALL                  0
@@ -4999,15 +4999,15 @@
                              42 JUMP_BACKWARD           18 (to 8)
                         >>   44 RETURN_VALUE
                consts
                names      ('fake_number',)
                varnames   ('.0', '_')
                freevars   ('options',)
                cellvars   ()
-               filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+               filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
                name       '<listcomp>'
                firstlineno 1173
                lnotab 0x
             'boolean'
             code
                argcount  : 1
                nlocals   : 2
@@ -5028,15 +5028,15 @@
                              38 JUMP_BACKWARD           17 (to 6)
                         >>   40 RETURN_VALUE
                consts
                names      ('fake_boolean',)
                varnames   ('.0', '_')
                freevars   ()
                cellvars   ()
-               filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+               filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
                name       '<listcomp>'
                firstlineno 1175
                lnotab 0x
             'string'
             code
                argcount  : 1
                nlocals   : 2
@@ -5060,15 +5060,15 @@
                              42 JUMP_BACKWARD           18 (to 8)
                         >>   44 RETURN_VALUE
                consts
                names      ('fake_string',)
                varnames   ('.0', '_')
                freevars   ('options',)
                cellvars   ()
-               filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+               filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
                name       '<listcomp>'
                firstlineno 1177
                lnotab 0x
             'date-time'
             code
                argcount  : 1
                nlocals   : 2
@@ -5089,15 +5089,15 @@
                              38 JUMP_BACKWARD           17 (to 6)
                         >>   40 RETURN_VALUE
                consts
                names      ('fake_datetime',)
                varnames   ('.0', '_')
                freevars   ()
                cellvars   ()
-               filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+               filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
                name       '<listcomp>'
                firstlineno 1179
                lnotab 0x
             'enum'
             code
                argcount  : 1
                nlocals   : 2
@@ -5121,26 +5121,26 @@
                              42 JUMP_BACKWARD           18 (to 8)
                         >>   44 RETURN_VALUE
                consts
                names      ('fake_enum',)
                varnames   ('.0', '_')
                freevars   ('options',)
                cellvars   ()
-               filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+               filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
                name       '<listcomp>'
                firstlineno 1181
                lnotab 0x
             'array'
             'object'
             None
          names      ('range',)
          varnames   ('type', 'numItems', 'options')
          freevars   ()
          cellvars   ('options',)
-         filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+         filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
          name       'fake_array'
          firstlineno 1152
          lnotab
             0x04140c0136010c0132010c0136010c0132010c0136010c0104010c0104
             ff
       code
          argcount  : 3
@@ -5181,15 +5181,15 @@
             'object'
             'Property'
             ('type', 'value')
          names      ('fake_array', 'pendingToImplement')
          varnames   ('type', 'numItems', 'options')
          freevars   ()
          cellvars   ()
-         filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+         filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
          name       'payload_array'
          firstlineno 1187
          lnotab 0x021510012802
       code
          argcount  : 3
          nlocals   : 15
          stacksize : 7
@@ -5282,15 +5282,15 @@
             00000069025300
                         0 MAKE_CELL                1 (dataModel)
                         2 MAKE_CELL                2 (level)
                         4 MAKE_CELL               15 (arrayPayload)
          
          1214           6 RESUME                   0
          
-         1216           8 LOAD_CONST               1 (<code object <listcomp>, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 1216>)
+         1216           8 LOAD_CONST               1 (<code object <listcomp>, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 1216>)
                        10 MAKE_FUNCTION            0
                        12 LOAD_FAST                0 (fullPayload)
                        14 LOAD_METHOD              0 (keys)
                        36 PRECALL                  0
                        40 CALL                     0
                        50 GET_ITER
                        52 PRECALL                  0
@@ -5300,15 +5300,15 @@
                        78 STORE_FAST               3 (prop)
          
          1218          80 LOAD_FAST                0 (fullPayload)
                        82 LOAD_FAST                3 (prop)
                        84 BINARY_SUBSCR
                        94 STORE_FAST               4 (payload)
          
-         1220          96 LOAD_CONST               3 (<code object <listcomp>, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 1220>)
+         1220          96 LOAD_CONST               3 (<code object <listcomp>, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 1220>)
                        98 MAKE_FUNCTION            0
                       100 LOAD_FAST                4 (payload)
                       102 GET_ITER
                       104 PRECALL                  0
                       108 CALL                     0
                       118 STORE_FAST               5 (keys)
          
@@ -5857,15 +5857,15 @@
                      2142 LOAD_CONST               4 ('required')
                      2144 DELETE_SUBSCR
          
          1310     >> 2146 LOAD_CLOSURE            15 (arrayPayload)
                      2148 LOAD_CLOSURE             1 (dataModel)
                      2150 LOAD_CLOSURE             2 (level)
                      2152 BUILD_TUPLE              3
-                     2154 LOAD_CONST              42 (<code object <listcomp>, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 1310>)
+                     2154 LOAD_CONST              42 (<code object <listcomp>, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 1310>)
                      2156 MAKE_FUNCTION            8 (closure)
                      2158 LOAD_GLOBAL             47 (NULL + range)
                      2170 LOAD_FAST               10 (arrayItems)
                      2172 PRECALL                  1
                      2176 CALL                     1
                      2186 GET_ITER
                      2188 PRECALL                  0
@@ -5991,15 +5991,15 @@
                              14 JUMP_BACKWARD            5 (to 6)
                         >>   16 RETURN_VALUE
                consts
                names      ()
                varnames   ('.0', 'p')
                freevars   ()
                cellvars   ()
-               filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+               filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
                name       '<listcomp>'
                firstlineno 1216
                lnotab 0x
             0
             code
                argcount  : 1
                nlocals   : 2
@@ -6016,15 +6016,15 @@
                              14 JUMP_BACKWARD            5 (to 6)
                         >>   16 RETURN_VALUE
                consts
                names      ()
                varnames   ('.0', 'k')
                freevars   ()
                cellvars   ()
-               filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+               filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
                name       '<listcomp>'
                firstlineno 1220
                lnotab 0x
             'required'
             'description'
             ''
             'Property'
@@ -6097,28 +6097,28 @@
                   'items'
                   1
                   'value'
                names      ('parse_property',)
                varnames   ('.0', 'i')
                freevars   ('arrayPayload', 'dataModel', 'level')
                cellvars   ()
-               filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+               filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
                name       '<listcomp>'
                firstlineno 1310
                lnotab 0x
             ('type', 'value')
             'object'
             'properties'
             'value'
             'oneOf'
          names      ('keys', 'parse_schema_description', 'fake_uri', 'payload_uri', 'list', 'rstr', 'xeger', 'parse_property', 'missingEntity', 'payload_geoproperty', 'payload_relationship', 'float', 'max', 'payload_number', 'int', 'payload_integer', 'payload_date', 'payload_time', 'payload_email', 'payload_string', 'payload_enum', 'payload_boolean', 'copy', 'range', 'pendingToImplement')
          varnames   ('fullPayload', 'dataModel', 'level', 'prop', 'payload', 'keys', 'metadata', 'keyPatterned', 'propertyName', 'argsNumber', 'arrayItems', 'valuesArray', 'valuesObject', 'objectPayload', 'p')
          freevars   ()
          cellvars   ('dataModel', 'level', 'arrayPayload')
-         filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+         filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
          name       'parse_property'
          firstlineno 1214
          lnotab
             0x08024802100218020801120208022c020801180124011801200108025a
             0128031401120150011801140128020e010c011e011801200118011e0108
             013e010a0118010402080134020a01080134023a011e0118010402080134
             020a010801340238011e01200130011c0118011c011801200130011e0118
@@ -6232,15 +6232,15 @@
             007225740f000000000000000000007c037c007c03190000000000000000
             0064381900000000000000000064021900000000000000000069017c017c
             02a6030000ab03000000000000000053007c037436000000000000000000
             0064327405000000000000000000007c037c01a6020000ab020000000000
             00000069025300
          1330           0 RESUME                   0
          
-         1347           2 LOAD_CONST               1 (<code object <listcomp>, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 1347>)
+         1347           2 LOAD_CONST               1 (<code object <listcomp>, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 1347>)
                         4 MAKE_FUNCTION            0
                         6 LOAD_FAST                0 (fullPayload)
                         8 LOAD_METHOD              0 (keys)
                        30 PRECALL                  0
                        34 CALL                     0
                        44 GET_ITER
                        46 PRECALL                  0
@@ -6250,15 +6250,15 @@
                        72 STORE_FAST               3 (prop)
          
          1348          74 LOAD_FAST                0 (fullPayload)
                        76 LOAD_FAST                3 (prop)
                        78 BINARY_SUBSCR
                        88 STORE_FAST               4 (payload)
          
-         1351          90 LOAD_CONST               3 (<code object <listcomp>, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 1351>)
+         1351          90 LOAD_CONST               3 (<code object <listcomp>, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 1351>)
                        92 MAKE_FUNCTION            0
                        94 LOAD_FAST                4 (payload)
                        96 GET_ITER
                        98 PRECALL                  0
                       102 CALL                     0
                       112 STORE_FAST               5 (keys)
          
@@ -7108,15 +7108,15 @@
                              14 JUMP_BACKWARD            5 (to 6)
                         >>   16 RETURN_VALUE
                consts
                names      ()
                varnames   ('.0', 'p')
                freevars   ()
                cellvars   ()
-               filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+               filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
                name       '<listcomp>'
                firstlineno 1347
                lnotab 0x
             0
             code
                argcount  : 1
                nlocals   : 2
@@ -7133,15 +7133,15 @@
                              14 JUMP_BACKWARD            5 (to 6)
                         >>   16 RETURN_VALUE
                consts
                names      ()
                varnames   ('.0', 'k')
                freevars   ()
                cellvars   ()
-               filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+               filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
                name       '<listcomp>'
                firstlineno 1351
                lnotab 0x
             'required'
             'description'
             'type'
             ''
@@ -7195,15 +7195,15 @@
             'oneOf'
             'anyOf'
             None
          names      ('keys', 'parse_schema_description', 'fake_uri', 'payload_uri', 'list', 'rstr', 'xeger', 'parse_property2ngsild_example', 'missingEntity', 'payload_geoproperty', 'payload_relationship', 'float', 'max', 'payload_number', 'int', 'payload_integer', 'payload_datetime', 'payload_date', 'payload_time', 'payload_email', 'payload_string', 'payload_enum', 'payload_boolean', 'copy', 'len', 'append', 'print', 'pendingToImplement')
          varnames   ('fullPayload', 'dataModel', 'level', 'prop', 'payload', 'keys', 'ngsiOutput', 'description', 'metadata', 'keyPatterned', 'propertyName', 'argsNumber', 'argsMin', 'argsMax', 'argsPattern', 'arrayItems', 'uniqueItems', 'arrayPayload', 'valuesArray', 'idx', 'tmp_value', 'valuesObject', 'objectPayload', 'p', 'objectOutput')
          freevars   ()
          cellvars   ()
-         filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+         filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
          name       'parse_property2ngsild_example'
          firstlineno 1330
          lnotab
             0x0211480110031803080112020803300116020802180224021801200208
             025a0128011401120136010aff10031804140128020e0224021e02180220
             0208023e020a0218020401080134020a01080134023a011e021802040108
             0134020a010801340238011e02200218011c0118011c0118011c01180120
@@ -7253,15 +7253,15 @@
                       112 RETURN_VALUE
          consts
             '\n    Merge two dictionaries where the values are lists, combining duplicate keys.\n\n    Parameters:\n        dict_a (dict): The first dictionary to be merged.\n        dict_b (dict): The second dictionary to be merged.\n\n    Returns:\n        dict: A new dictionary containing merged values for common keys.\n\n    Example:\n    >>> dict_a = {"1": [], "2": ["aa", "bb"]}\n    >>> dict_b = {"1": [], "2": ["cc"], "3": ["dd"]}\n    >>> merge_duplicate_attributes(dict_a, dict_b)\n    {"1": [], "2": ["aa", "bb", "cc"], "3": ["dd"]}\n    '
          names      ('items', 'get')
          varnames   ('dict_a', 'dict_b', 'key', 'values')
          freevars   ()
          cellvars   ()
-         filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+         filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
          name       'merge_duplicate_attributes'
          firstlineno 1538
          lnotab 0x021132033a01
       1
       code
          argcount  : 2
          nlocals   : 13
@@ -7357,15 +7357,15 @@
                        16 BUILD_MAP                1
                        18 STORE_DEREF             13 (attributes)
          
          1575          20 LOAD_CLOSURE            13 (attributes)
                        22 LOAD_CLOSURE             1 (level)
                        24 LOAD_CLOSURE            14 (output)
                        26 BUILD_TUPLE              3
-                       28 LOAD_CONST               1 (<code object process_allOf_oneOf_anyOf, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 1575>)
+                       28 LOAD_CONST               1 (<code object process_allOf_oneOf_anyOf, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 1575>)
                        30 MAKE_FUNCTION            8 (closure)
                        32 STORE_FAST               2 (process_allOf_oneOf_anyOf)
          
          1583          34 LOAD_DEREF               1 (level)
                        36 LOAD_CONST               2 (1)
                        38 COMPARE_OP               2 (==)
                        44 POP_JUMP_FORWARD_IF_FALSE    83 (to 212)
@@ -8021,15 +8021,15 @@
                   None
                   1
                   'properties'
                names      ('range', 'len', 'parse_payload_v2', 'dict', 'merge_duplicate_attributes')
                varnames   ('ofSubSchema', 'index', 'partialOutput', 'partialAttr')
                freevars   ('attributes', 'level', 'output')
                cellvars   ()
-               filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+               filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
                name       'process_allOf_oneOf_anyOf'
                firstlineno 1575
                lnotab 0x04023c013801120126ff060222fc
             1
             ('allOf', 'anyOf', 'oneOf', 'properties')
             'properties'
             8
@@ -8041,15 +8041,15 @@
             'integer'
             'number'
             (None, None)
          names      ('parse_payload_v2', 'merge_duplicate_attributes', 'isinstance', 'list', 'range', 'len', 'dict', 'append', 'parse_schema_description')
          varnames   ('schemaPayload', 'level', 'process_allOf_oneOf_anyOf', 'keys_to_check_level_one', 'key', 'partialAttr', 'index', 'partialOutput', 'subschema', 'prop', 'item', 'x_ngsi', 'description')
          freevars   ()
          cellvars   ('level', 'attributes', 'output')
-         filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+         filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
          name       'parse_payload_v2'
          firstlineno 1561
          lnotab
             0x080b040108020e080c020801080108070c013801220224f4040e0e042a
             013c0138011a0122042c020a0208010a01480144012401100102ff1e0102
             fe100322fb02090e020a011602020120010201160140033c030801220160
             010c013aff16024e0122fc02070c01480122010401240308010c012eff34
@@ -8637,15 +8637,15 @@
             'type_specific_text'
             "Type property doesn't match to data model name on level "
             'Missing Type property'
          names      ('isinstance', 'list', 'parse_yamlDict', 'dict', 'len', 'keys', 'exceptions', 'propertyTypes', 'str', 'incompleteDescription', 'withoutDescription', 'extract_datamodel_from_raw_url')
          varnames   ('yamlDict', 'datamodelRepoUrl', 'level', 'output', 'item', 'partialoutput', 'prop', 'propKey', 'propertyType', 'description')
          freevars   ()
          cellvars   ()
-         filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+         filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
          name       'parse_yamlDict'
          firstlineno 1695
          lnotab
             0x021904032a01080128011cfe04060a020e03aa01140128011c03380508
             0134011a0102063801080140011c0522020202280212010a011601380216
             021a0102ff12ff0e0102ff080402010a0116010e010cff120102ff04011c
             ff220302021c0226011601180216012402020116012a02180202021c0232
@@ -8842,15 +8842,15 @@
             'not possible to check '
             ' clause, '
             None
          names      ('checkers', 'is_url', 'is_url_existed', 'Exception', 'str')
          varnames   ('output', 'schemaDict', 'metadata_fields', 'field', 'value', 'e')
          freevars   ()
          cellvars   ()
-         filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+         filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
          name       'is_metadata_properly_reported'
          firstlineno 1823
          lnotab
             0x021208010a02080208010204080110020401280222012a02220222022c
             01120152ff0803
       'jsonDict'
       'message'
@@ -9307,15 +9307,15 @@
             " = '' in the header"
             'not possible to check '
             ' clause, '
          names      ('items', 'isinstance', 'str', 'list', 'KEYWORDS_FOR_CERTAIN_CHECK', 'len', 're', 'search', 'join', 'Exception')
          varnames   ('output', 'jsonDict', 'schemaUrl', 'message', 'checkall', 'checklist', 'metadata_fields', 'field', 'constraints', 'value', 'mf', 'e')
          freevars   ()
          cellvars   ()
-         filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+         filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
          name       'is_metadata_existed'
          firstlineno 1870
          lnotab
             0x021e08010a0308010801080108010601080114f9060a340102040a0110
             0318012a01220118012a01200308010c010c0128011e020aff16043a0120
             033a0120033e01200308011401080240ff1a032e01120154ff0803
       code
@@ -9393,15 +9393,15 @@
                        52 LOAD_CONST               4 ('metadata')
                        54 BINARY_SUBSCR
                        64 STORE_FAST               4 (metadata)
          
          1994          66 BUILD_MAP                0
                        68 STORE_FAST               5 (results)
          
-         1995          70 LOAD_CONST               5 (<code object <dictcomp>, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 1995>)
+         1995          70 LOAD_CONST               5 (<code object <dictcomp>, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 1995>)
                        72 MAKE_FUNCTION            0
                        74 LOAD_GLOBAL              0 (CHECKED_PROPERTY_CASES)
                        86 GET_ITER
                        88 PRECALL                  0
                        92 CALL                     0
                       102 STORE_FAST               5 (results)
          
@@ -9707,15 +9707,15 @@
                              16 JUMP_BACKWARD            6 (to 6)
                         >>   18 RETURN_VALUE
                consts
                names      ()
                varnames   ('.0', 'key')
                freevars   ()
                cellvars   ()
-               filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+               filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
                name       '<dictcomp>'
                firstlineno 1995
                lnotab 0x
             'Failed'
             'documented'
             'x-ngsi'
             'well documented'
@@ -9732,15 +9732,15 @@
             'newly available'
             'Metadata'
             'warning'
          names      ('CHECKED_PROPERTY_CASES', 'items', 'append', 'keys', 'list')
          varnames   ('output', 'documentationStatusOfProperties', 'alreadyUsedProperties', 'availableProperties', 'metadata', 'results', 'prop', 'value')
          freevars   ()
          cellvars   ()
-         filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+         filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
          name       'schema_output_sum'
          firstlineno 1963
          lnotab
             0x021a1001100110011002040122010a023402220238031402440122014e
             021402440122014e02200322014e02080202015401020122015afa040808
             0182020801820232014402
       'results'
@@ -9811,15 +9811,15 @@
                       176 POP_JUMP_FORWARD_IF_FALSE    68 (to 314)
          
          2079         178 LOAD_FAST                1 (message)
                       180 LOAD_CONST               7 ('\nHowever, We highly suggest you fix these properties:\n    ')
          
          2081         182 LOAD_GLOBAL              2 (newline)
                       194 LOAD_METHOD              2 (join)
-                      216 LOAD_CONST               8 (<code object <listcomp>, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 2081>)
+                      216 LOAD_CONST               8 (<code object <listcomp>, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 2081>)
                       218 MAKE_FUNCTION            0
                       220 LOAD_FAST                0 (results)
                       222 LOAD_CONST               9 ('Failed')
                       224 BINARY_SUBSCR
                       234 LOAD_METHOD              3 (items)
                       256 PRECALL                  0
                       260 CALL                     0
@@ -9848,15 +9848,15 @@
                       350 BINARY_SUBSCR
                       360 POP_JUMP_FORWARD_IF_FALSE    49 (to 460)
          
          2088         362 LOAD_FAST                1 (message)
                       364 LOAD_CONST              12 ('\nSome warnings related to metadata:\n    ')
                       366 LOAD_GLOBAL              2 (newline)
                       378 LOAD_METHOD              2 (join)
-                      400 LOAD_CONST              13 (<code object <listcomp>, file "/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py", line 2088>)
+                      400 LOAD_CONST              13 (<code object <listcomp>, file "/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py", line 2088>)
                       402 MAKE_FUNCTION            0
                       404 LOAD_FAST                0 (results)
                       406 LOAD_CONST              14 ('Metadata')
                       408 BINARY_SUBSCR
                       418 GET_ITER
                       420 PRECALL                  0
                       424 CALL                     0
@@ -9919,15 +9919,15 @@
                consts
                   ' - '
                   ', '
                names      ('newline', 'join')
                varnames   ('.0', 'text', 'pps')
                freevars   ()
                cellvars   ()
-               filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+               filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
                name       '<listcomp>'
                firstlineno 2081
                lnotab 0x
             'Failed'
             '\n        '
             '\nNo major issues with the named properties in general.'
             '\nSome warnings related to metadata:\n    '
@@ -9950,25 +9950,25 @@
                         >>   22 RETURN_VALUE
                consts
                   ' - '
                names      ()
                varnames   ('.0', 'text')
                freevars   ()
                cellvars   ()
-               filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+               filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
                name       '<listcomp>'
                firstlineno 2088
                lnotab 0x
             'Metadata'
             '\nNo warnings with metadata.'
          names      ('CHECKED_PROPERTY_CASES', 'newline', 'join', 'items')
          varnames   ('results', 'message', 'key')
          freevars   ()
          cellvars   ()
-         filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+         filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
          name       'message_after_check_schema'
          firstlineno 2042
          lnotab 0x021d04022201100154032601040276fe0e050a03260162020a02
       code
          argcount  : 1
          nlocals   : 7
          stacksize : 8
@@ -10059,15 +10059,15 @@
             'https://raw.githubusercontent.com/'
             '/'
             'Invalid GitHub URL format'
          names      ('re', 'match', 'github_url_pattern', 'group', 'print')
          varnames   ('input_url', 'match', 'owner', 'repository', 'branch', 'file_path', 'raw_github_url')
          freevars   ()
          cellvars   ()
-         filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+         filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
          name       'convert_to_raw_github_url'
          firstlineno 2094
          lnotab 0x0201340204012a012a012a012a011c010402
       (0,)
       (True, 0)
       (True,)
       (4,)
@@ -10075,15 +10075,15 @@
       (None,)
       (1,)
       ('', True, None)
    names      ('os', 'json', 'random', 're', 'string', 'jsonref', 'typing', 'Dict', 'Tuple', 'validator_collection', 'checkers', 'faker', 'Faker', 'requests', 'rstr', 'ruamel.yaml', 'ruamel', 'fake', 'pendingToImplement', 'missingEntity', 'newline', 'newsubline', 'propertyTypes', 'incompleteDescription', 'withoutDescription', 'wrongTypeDescription', 'missingTypeDescription', 'exceptions', 'KEYWORDS_FOR_CERTAIN_CHECK', 'CHECKED_PROPERTY_CASES', 'github_url_pattern', 'is_url_existed', 'str', 'open_json', 'open_jsonref', 'open_yaml', 'extract_datamodel_from_raw_url', 'extract_subject_from_raw_url', 'create_context', 'DeprecationWarning', 'dict', 'normalized2keyvalues', 'int', 'normalized2keyvalues_v2', 'bool', 'keyvalues2normalized_ngsild', 'keyvalues2normalized_ngsiv2', 'generate_random_string', 'fake_uri', 'payload_uri', 'payload_relationship', 'fake_geoproperty', 'payload_geoproperty', 'float', 'fake_number', 'fake_integer', 'payload_number', 'payload_integer', 'fake_datetime', 'fake_date', 'fake_time', 'payload_datetime', 'payload_date', 'payload_time', 'fake_email', 'payload_email', 'fake_string', 'payload_string', 'list', 'fake_enum', 'payload_enum', 'fake_boolean', 'payload_boolean', 'parse_schema_description', 'echo', 'fake_array', 'payload_array', 'parse_property', 'parse_property2ngsild_example', 'merge_duplicate_attributes', 'parse_payload_v2', 'parse_yamlDict', 'is_metadata_properly_reported', 'is_metadata_existed', 'schema_output_sum', 'message_after_check_schema', 'convert_to_raw_github_url')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/home/aabella/PycharmProjects/scaleup/PYTHON_PACKAGE/pysmartdatamodels/test/../utils/common_utils.py'
+   filename   '/home/aabella/PycharmProjects/pysmartdatamodels/PYTHON_PACKAGE/pysmartdatamodels/utils/common_utils.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff021108010801080108020801080110020c030c0108010801080314
       020401040204010401080304010401040104010802040108030402061d0c
       1f0c21061d101e101d101402010eff0e010243163d1e7f08650e14141114
       0e0611102410110c240c210c190c150c0e0c0d0c0d0c0d0c0d0c0d101c10
```

### Comparing `pysmartdatamodels-0.8/pysmartdatamodels/utils/common_utils.py` & `pysmartdatamodels-0.8.0.1/pysmartdatamodels/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `pysmartdatamodels-0.8/PKG-INFO` & `pysmartdatamodels-0.8.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysmartdatamodels
-Version: 0.8
+Version: 0.8.0.1
 Summary: Open-licensed and free data models to model your digital twins, share data in data spaces or develop smart applications
 Home-page: https://github.com/smart-data-models/data-models/tree/master/pysmartdatamodels
 Author: aabella
 Author-email: alberto.abella@fiware.org
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -13,20 +13,20 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: Faker (>=18.10.1,<19.0.0)
+Requires-Dist: Faker (>=18.10.1)
 Requires-Dist: fuzzywuzzy (>=0.18)
 Requires-Dist: jsonref (>=1.0.0)
 Requires-Dist: jsonschema (>=4.17.3,<5.0.0)
 Requires-Dist: python-Levenshtein (>=0.25)
-Requires-Dist: pytz (>=2022.7.1,<2023.0.0)
+Requires-Dist: pytz (>=2022.7.1)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: rstr (>=3.2.1,<4.0.0)
 Requires-Dist: ruamel.yaml (>=0.18.1)
 Requires-Dist: urllib3 (>=2.0.7,<3.0.0)
 Requires-Dist: validator-collection (>=1.5.0,<2.0.0)
 Project-URL: Repository, https://github.com/smart-data-models/data-models/tree/master/pysmartdatamodels
 Description-Content-Type: text/markdown
```

