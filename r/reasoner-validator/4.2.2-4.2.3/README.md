# Comparing `tmp/reasoner_validator-4.2.2.tar.gz` & `tmp/reasoner_validator-4.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasoner_validator-4.2.2.tar", max compression
+gzip compressed data, was "reasoner_validator-4.2.3.tar", max compression
```

## Comparing `reasoner_validator-4.2.2.tar` & `reasoner_validator-4.2.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1153 2024-05-24 22:52:24.396746 reasoner_validator-4.2.2/LICENSE
--rw-r--r--   0        0        0    13727 2024-05-24 22:52:24.396746 reasoner_validator-4.2.2/README.md
--rw-r--r--   0        0        0      131 2024-05-24 22:52:24.396746 reasoner_validator-4.2.2/docs/.nojekyll
--rw-r--r--   0        0        0      634 2024-05-24 22:52:24.396746 reasoner_validator-4.2.2/docs/Makefile
--rw-r--r--   0        0        0     2291 2024-05-24 22:52:24.396746 reasoner_validator-4.2.2/docs/conf.py
--rw-r--r--   0        0        0    20564 2024-05-24 22:52:24.396746 reasoner_validator-4.2.2/docs/index.rst
--rw-r--r--   0        0        0      795 2024-05-24 22:52:24.396746 reasoner_validator-4.2.2/docs/make.bat
--rw-r--r--   0        0        0      136 2024-05-24 22:52:24.396746 reasoner_validator-4.2.2/docs/reasoner_validator.biolink.rst
--rw-r--r--   0        0        0      135 2024-05-24 22:52:24.396746 reasoner_validator-4.2.2/docs/reasoner_validator.report.rst
--rw-r--r--   0        0        0      152 2024-05-24 22:52:24.396746 reasoner_validator-4.2.2/docs/reasoner_validator.rst
--rw-r--r--   0        0        0      146 2024-05-24 22:52:24.396746 reasoner_validator-4.2.2/docs/reasoner_validator.trapi.mapping.rst
--rw-r--r--   0        0        0      144 2024-05-24 22:52:24.396746 reasoner_validator-4.2.2/docs/reasoner_validator.trapi.rst
--rw-r--r--   0        0        0      163 2024-05-24 22:52:24.396746 reasoner_validator-4.2.2/docs/reasoner_validator.validation_codes.rst
--rw-r--r--   0        0        0      157 2024-05-24 22:52:24.396746 reasoner_validator-4.2.2/docs/reasoner_validator.versioning.rst
--rw-r--r--   0        0        0    43781 2024-05-24 22:52:24.396746 reasoner_validator-4.2.2/docs/validation_codes_dictionary.md
--rw-r--r--   0        0        0     2368 2024-05-24 22:52:24.396746 reasoner_validator-4.2.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-24 22:52:24.396746 reasoner_validator-4.2.2/reasoner_validator/__init__.py
--rw-r--r--   0        0        0    97394 2024-05-24 22:52:24.400746 reasoner_validator-4.2.2/reasoner_validator/biolink/__init__.py
--rw-r--r--   0        0        0     4264 2024-05-24 22:52:24.400746 reasoner_validator-4.2.2/reasoner_validator/biolink/ontology.py
--rw-r--r--   0        0        0    47770 2024-05-24 22:52:24.400746 reasoner_validator-4.2.2/reasoner_validator/codes.yaml
--rw-r--r--   0        0        0     1761 2024-05-24 22:52:24.400746 reasoner_validator-4.2.2/reasoner_validator/github.py
--rw-r--r--   0        0        0     3995 2024-05-24 22:52:24.400746 reasoner_validator-4.2.2/reasoner_validator/message.py
--rw-r--r--   0        0        0    47007 2024-05-24 22:52:24.400746 reasoner_validator-4.2.2/reasoner_validator/report.py
--rw-r--r--   0        0        0    15057 2024-05-24 22:52:24.400746 reasoner_validator-4.2.2/reasoner_validator/trapi/__init__.py
--rw-r--r--   0        0        0     1120 2024-05-24 22:52:24.400746 reasoner_validator-4.2.2/reasoner_validator/trapi/mapping.py
--rw-r--r--   0        0        0     4834 2024-05-24 22:52:24.400746 reasoner_validator-4.2.2/reasoner_validator/utils/__init__.py
--rw-r--r--   0        0        0      886 2024-05-24 22:52:24.400746 reasoner_validator-4.2.2/reasoner_validator/utils/http.py
--rw-r--r--   0        0        0    14745 2024-05-24 22:52:24.400746 reasoner_validator-4.2.2/reasoner_validator/validation_codes.py
--rw-r--r--   0        0        0    42671 2024-05-24 22:52:24.400746 reasoner_validator-4.2.2/reasoner_validator/validator.py
--rw-r--r--   0        0        0    12127 2024-05-24 22:52:24.400746 reasoner_validator-4.2.2/reasoner_validator/versioning.py
--rw-r--r--   0        0        0      866 2024-05-24 22:52:24.400746 reasoner_validator-4.2.2/reasoner_validator/versions.yaml
--rw-r--r--   0        0        0     3594 2024-05-24 22:52:24.400746 reasoner_validator-4.2.2/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-05-24 22:52:24.400746 reasoner_validator-4.2.2/tests/conftest.py
--rw-r--r--   0        0        0   151988 2024-05-24 22:52:24.400746 reasoner_validator-4.2.2/tests/test_biolink_compliance_validation.py
--rw-r--r--   0        0        0    62107 2024-05-24 22:52:24.400746 reasoner_validator-4.2.2/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml
--rw-r--r--   0        0        0     3204 2024-05-24 22:52:24.400746 reasoner_validator-4.2.2/tests/test_ontology.py
--rw-r--r--   0        0        0    50742 2024-05-24 22:52:24.400746 reasoner_validator-4.2.2/tests/test_response_validator.py
--rw-r--r--   0        0        0     6157 2024-05-24 22:52:24.400746 reasoner_validator-4.2.2/tests/test_semver.py
--rw-r--r--   0        0        0     2327 2024-05-24 22:52:24.404746 reasoner_validator-4.2.2/tests/test_trapi_versioning.py
--rw-r--r--   0        0        0     1938 2024-05-24 22:52:24.404746 reasoner_validator-4.2.2/tests/test_utils.py
--rw-r--r--   0        0        0    36726 2024-05-24 22:52:24.404746 reasoner_validator-4.2.2/tests/test_validate.py
--rw-r--r--   0        0        0    30435 2024-05-24 22:52:24.404746 reasoner_validator-4.2.2/tests/test_validation_report.py
--rw-r--r--   0        0        0     3421 2024-05-24 22:52:24.404746 reasoner_validator-4.2.2/tests/test_workflows.py
--rw-r--r--   0        0        0    15315 1970-01-01 00:00:00.000000 reasoner_validator-4.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1153 2024-05-28 17:21:24.830292 reasoner_validator-4.2.3/LICENSE
+-rw-r--r--   0        0        0    13727 2024-05-28 17:21:24.830292 reasoner_validator-4.2.3/README.md
+-rw-r--r--   0        0        0      131 2024-05-28 17:21:24.830292 reasoner_validator-4.2.3/docs/.nojekyll
+-rw-r--r--   0        0        0      634 2024-05-28 17:21:24.830292 reasoner_validator-4.2.3/docs/Makefile
+-rw-r--r--   0        0        0     2291 2024-05-28 17:21:24.830292 reasoner_validator-4.2.3/docs/conf.py
+-rw-r--r--   0        0        0    20564 2024-05-28 17:21:24.830292 reasoner_validator-4.2.3/docs/index.rst
+-rw-r--r--   0        0        0      795 2024-05-28 17:21:24.830292 reasoner_validator-4.2.3/docs/make.bat
+-rw-r--r--   0        0        0      136 2024-05-28 17:21:24.830292 reasoner_validator-4.2.3/docs/reasoner_validator.biolink.rst
+-rw-r--r--   0        0        0      135 2024-05-28 17:21:24.830292 reasoner_validator-4.2.3/docs/reasoner_validator.report.rst
+-rw-r--r--   0        0        0      152 2024-05-28 17:21:24.830292 reasoner_validator-4.2.3/docs/reasoner_validator.rst
+-rw-r--r--   0        0        0      146 2024-05-28 17:21:24.830292 reasoner_validator-4.2.3/docs/reasoner_validator.trapi.mapping.rst
+-rw-r--r--   0        0        0      144 2024-05-28 17:21:24.830292 reasoner_validator-4.2.3/docs/reasoner_validator.trapi.rst
+-rw-r--r--   0        0        0      163 2024-05-28 17:21:24.830292 reasoner_validator-4.2.3/docs/reasoner_validator.validation_codes.rst
+-rw-r--r--   0        0        0      157 2024-05-28 17:21:24.830292 reasoner_validator-4.2.3/docs/reasoner_validator.versioning.rst
+-rw-r--r--   0        0        0    44182 2024-05-28 17:21:24.830292 reasoner_validator-4.2.3/docs/validation_codes_dictionary.md
+-rw-r--r--   0        0        0     2368 2024-05-28 17:21:24.834292 reasoner_validator-4.2.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-28 17:21:24.834292 reasoner_validator-4.2.3/reasoner_validator/__init__.py
+-rw-r--r--   0        0        0    97394 2024-05-28 17:21:24.834292 reasoner_validator-4.2.3/reasoner_validator/biolink/__init__.py
+-rw-r--r--   0        0        0     4577 2024-05-28 17:21:24.834292 reasoner_validator-4.2.3/reasoner_validator/biolink/ontology.py
+-rw-r--r--   0        0        0    48336 2024-05-28 17:21:24.834292 reasoner_validator-4.2.3/reasoner_validator/codes.yaml
+-rw-r--r--   0        0        0     1761 2024-05-28 17:21:24.834292 reasoner_validator-4.2.3/reasoner_validator/github.py
+-rw-r--r--   0        0        0     3995 2024-05-28 17:21:24.834292 reasoner_validator-4.2.3/reasoner_validator/message.py
+-rw-r--r--   0        0        0    47007 2024-05-28 17:21:24.834292 reasoner_validator-4.2.3/reasoner_validator/report.py
+-rw-r--r--   0        0        0    15140 2024-05-28 17:21:24.834292 reasoner_validator-4.2.3/reasoner_validator/trapi/__init__.py
+-rw-r--r--   0        0        0     1120 2024-05-28 17:21:24.834292 reasoner_validator-4.2.3/reasoner_validator/trapi/mapping.py
+-rw-r--r--   0        0        0     4834 2024-05-28 17:21:24.834292 reasoner_validator-4.2.3/reasoner_validator/utils/__init__.py
+-rw-r--r--   0        0        0      886 2024-05-28 17:21:24.834292 reasoner_validator-4.2.3/reasoner_validator/utils/http.py
+-rw-r--r--   0        0        0    14745 2024-05-28 17:21:24.834292 reasoner_validator-4.2.3/reasoner_validator/validation_codes.py
+-rw-r--r--   0        0        0    47483 2024-05-28 17:21:24.834292 reasoner_validator-4.2.3/reasoner_validator/validator.py
+-rw-r--r--   0        0        0    12127 2024-05-28 17:21:24.834292 reasoner_validator-4.2.3/reasoner_validator/versioning.py
+-rw-r--r--   0        0        0      475 2024-05-28 17:21:24.834292 reasoner_validator-4.2.3/reasoner_validator/versions.yaml
+-rw-r--r--   0        0        0     3594 2024-05-28 17:21:24.834292 reasoner_validator-4.2.3/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 17:21:24.834292 reasoner_validator-4.2.3/tests/conftest.py
+-rw-r--r--   0        0        0   151988 2024-05-28 17:21:24.834292 reasoner_validator-4.2.3/tests/test_biolink_compliance_validation.py
+-rw-r--r--   0        0        0    62107 2024-05-28 17:21:24.838292 reasoner_validator-4.2.3/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml
+-rw-r--r--   0        0        0     3204 2024-05-28 17:21:24.838292 reasoner_validator-4.2.3/tests/test_ontology.py
+-rw-r--r--   0        0        0    50577 2024-05-28 17:21:24.838292 reasoner_validator-4.2.3/tests/test_response_validator.py
+-rw-r--r--   0        0        0     6157 2024-05-28 17:21:24.838292 reasoner_validator-4.2.3/tests/test_semver.py
+-rw-r--r--   0        0        0     2327 2024-05-28 17:21:24.838292 reasoner_validator-4.2.3/tests/test_trapi_versioning.py
+-rw-r--r--   0        0        0     1938 2024-05-28 17:21:24.838292 reasoner_validator-4.2.3/tests/test_utils.py
+-rw-r--r--   0        0        0    36726 2024-05-28 17:21:24.838292 reasoner_validator-4.2.3/tests/test_validate.py
+-rw-r--r--   0        0        0    30435 2024-05-28 17:21:24.838292 reasoner_validator-4.2.3/tests/test_validation_report.py
+-rw-r--r--   0        0        0     3421 2024-05-28 17:21:24.838292 reasoner_validator-4.2.3/tests/test_workflows.py
+-rw-r--r--   0        0        0    15315 1970-01-01 00:00:00.000000 reasoner_validator-4.2.3/PKG-INFO
```

### Comparing `reasoner_validator-4.2.2/LICENSE` & `reasoner_validator-4.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.2.2/README.md` & `reasoner_validator-4.2.3/README.md`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.2.2/docs/Makefile` & `reasoner_validator-4.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.2.2/docs/conf.py` & `reasoner_validator-4.2.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.2.2/docs/index.rst` & `reasoner_validator-4.2.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.2.2/docs/make.bat` & `reasoner_validator-4.2.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.2.2/docs/validation_codes_dictionary.md` & `reasoner_validator-4.2.3/docs/validation_codes_dictionary.md`

 * *Files 1% similar despite different names*

```diff
@@ -900,18 +900,20 @@
 
 **Message:** Response returned an empty Message Knowledge Graph?
 
 **Description:** An empty Knowledge Graph is allowed but merits a boundary response warning?
 
 ### warning.trapi.response.message.knowledge_graph.node.category.imprecise
 
-**Message:** The category of the knowledge graph node matching an input node identifier is more generic than expected.
+**Message:** The category of the knowledge graph node is imprecise.
 
 **Context:** identifier, expected_category, observed_categories
 
+**Description:** The category of the knowledge graph node matching an input node identifier is more generic than expected.
+
 ### warning.trapi.response.message.results.empty
 
 **Message:** Response returned empty Message.results?
 
 **Description:** Empty Results is allowed but merits a boundary response warning?
 
 ### warning.trapi.response.workflow.runner_parameters.missing
@@ -1172,14 +1174,22 @@
 
 **Context:** identifier
 
 **Description:** A 'support_graph' may be required as an explanation for a given 'treats' statement assertion.
 
 ## Information
 
+### info.trapi.response.message.knowledge_graph.node.parent.match
+
+**Message:** Query node is ontological parent of its matching knowledge graph node
+
+**Context:** identifier, query_id, context
+
+**Description:** The knowledge graph node identifier was matched as an ontological subclass of the specified query node identifier.
+
 ### info.excluded
 
 **Message:** All test case S-P-O triples from resource test location, or specific user excluded S-P-O triples
 
 **Context:** identifier
 
 **Description:** Check the JSON KP test edge data file for specific 'exclude_tests' directives, either global to the file, or on specific edges.
```

### Comparing `reasoner_validator-4.2.2/pyproject.toml` & `reasoner_validator-4.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reasoner-validator"
-version = "4.2.2"
+version = "4.2.3"
 description = "Validation tools for Reasoner API"
 authors = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
     "Patrick Wang <patrickelvin@gmail.com>"
 ]
 maintainers = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
```

### Comparing `reasoner_validator-4.2.2/reasoner_validator/biolink/__init__.py` & `reasoner_validator-4.2.3/reasoner_validator/biolink/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.2.2/reasoner_validator/biolink/ontology.py` & `reasoner_validator-4.2.3/reasoner_validator/biolink/ontology.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 """
 Ontology KP interface
 """
 from typing import Optional
+from functools import lru_cache
+
 from reasoner_validator.biolink import get_biolink_model_toolkit
 from reasoner_validator.utils.http import post_query
 
 ONTOLOGY_KP_TRAPI_SERVER = "https://automat.renci.org/ubergraph/query"
 NODE_NORMALIZER_SERVER = "https://nodenormalization-sri.renci.org/get_normalized_nodes"
 
+CACHE_SIZE = 1024
+
 
 def convert_to_preferred(curie, allowed_list):
     """
     :param curie
     :param allowed_list
     """
     j = {'curies': [curie]}
     result = post_query(NODE_NORMALIZER_SERVER, j)
-    if not result:
+    if not (result and curie in result and result[curie] and 'equivalent_identifiers' in result[curie]):
         return None
     new_ids = [v['identifier'] for v in result[curie]['equivalent_identifiers']]
     for nid in new_ids:
         if nid.split(':')[0] in allowed_list:
             return nid
     return None
 
@@ -93,16 +97,21 @@
     if ancestor_count:
         ancestor_count.sort()
         return ancestor_count[-1][1]
     else:
         return None
 
 
+@lru_cache(CACHE_SIZE)
 def get_parent_concept(curie, category, biolink_version) -> Optional[str]:
     """
+    Given a CURIE of a concept and its category,
+    attempt to return the parent concept if available
+    within the specified Biolink Model release.
+
     :param curie: CURIE of a concept instance
     :param category: Biolink Category of the concept instance
     :param biolink_version: Biolink Model version to use in validation (SemVer string specification)
     """
     tk = get_biolink_model_toolkit(biolink_version=biolink_version)
     if not tk.is_category(category):
         assert False, f"'{category}' is not a Biolink Model Category!"
```

### Comparing `reasoner_validator-4.2.2/reasoner_validator/codes.yaml` & `reasoner_validator-4.2.3/reasoner_validator/codes.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -693,15 +693,16 @@
         knowledge_graph:
           empty:
             $message: "Response returned an empty Message Knowledge Graph?"
             $description: "An empty Knowledge Graph is allowed but merits a boundary response warning?"
           node:
             category:
               imprecise:
-                $message: "The category of the knowledge graph node matching an input node identifier is more generic than expected."
+                $message: "The category of the knowledge graph node is imprecise."
+                $description: "The category of the knowledge graph node matching an input node identifier is more generic than expected."
                 $context:
                   - identifier
                   - expected_category
                   - observed_categories
         results:
           empty:
             $message: "Response returned empty Message.results?"
@@ -931,14 +932,27 @@
         support_graph:
           missing:
             $message: "Edge with a treats-related predicate is missing its required 'support_graph' attribute"
             $context:
               - identifier
             $description: "A 'support_graph' may be required as an explanation for a given 'treats' statement assertion."
 info:
+  trapi:
+    response:
+      message:
+        knowledge_graph:
+          node:
+            parent:
+              match:
+                $message: "Query node is ontological parent of its matching knowledge graph node"
+                $context:
+                  - identifier
+                  - query_id
+                  - context
+                $description: "The knowledge graph node identifier was matched as an ontological subclass of the specified query node identifier."
   excluded:
     $message: "All test case S-P-O triples from resource test location, or specific user excluded S-P-O triples"
     $context:
       - identifier
     $description: "Check the JSON KP test edge data file for specific 'exclude_tests' directives, either global to the file, or on specific edges."
   compliant:
     $message: "Biolink Model-compliant TRAPI Message"
```

### Comparing `reasoner_validator-4.2.2/reasoner_validator/github.py` & `reasoner_validator-4.2.3/reasoner_validator/github.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.2.2/reasoner_validator/message.py` & `reasoner_validator-4.2.3/reasoner_validator/message.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.2.2/reasoner_validator/report.py` & `reasoner_validator-4.2.3/reasoner_validator/report.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.2.2/reasoner_validator/trapi/__init__.py` & `reasoner_validator-4.2.3/reasoner_validator/trapi/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,17 +36,19 @@
 TRAPI_1_4_0: str = str(TRAPI_1_4_0_SEMVER)
 TRAPI_1_4_1_SEMVER = SemVer.from_string("v1.4.1")
 TRAPI_1_4_1: str = str(TRAPI_1_4_1_SEMVER)
 TRAPI_1_4_2_SEMVER = SemVer.from_string("v1.4.2")
 TRAPI_1_4_2: str = str(TRAPI_1_4_2_SEMVER)
 TRAPI_1_5_0_BETA_SEMVER = SemVer.from_string("v1.5.0-beta")
 TRAPI_1_5_0_BETA: str = str(TRAPI_1_5_0_BETA_SEMVER)
+TRAPI_1_5_0_SEMVER = SemVer.from_string("v1.5.0")
+TRAPI_1_5_0: str = str(TRAPI_1_5_0_SEMVER)
 
-LATEST_TRAPI_RELEASE_SEMVER: SemVer = TRAPI_1_5_0_BETA_SEMVER
-LATEST_TRAPI_RELEASE: str = TRAPI_1_5_0_BETA
+LATEST_TRAPI_RELEASE_SEMVER: SemVer = TRAPI_1_5_0_SEMVER
+LATEST_TRAPI_RELEASE: str = TRAPI_1_5_0
 
 LATEST_TRAPI_MAJOR_MINOR_RELEASE: str = "1.5"
 LATEST_TRAPI_MAJOR_MINOR_RELEASE_SEMVER: SemVer = \
     SemVer.from_string(
         LATEST_TRAPI_MAJOR_MINOR_RELEASE,
         core_fields=['major', 'minor'],
         # generally also suppress extension fields
```

### Comparing `reasoner_validator-4.2.2/reasoner_validator/trapi/mapping.py` & `reasoner_validator-4.2.3/reasoner_validator/trapi/mapping.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.2.2/reasoner_validator/utils/__init__.py` & `reasoner_validator-4.2.3/reasoner_validator/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.2.2/reasoner_validator/utils/http.py` & `reasoner_validator-4.2.3/reasoner_validator/utils/http.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.2.2/reasoner_validator/validation_codes.py` & `reasoner_validator-4.2.3/reasoner_validator/validation_codes.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.2.2/reasoner_validator/validator.py` & `reasoner_validator-4.2.3/reasoner_validator/validator.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-from typing import Optional, List, Dict, Set
+from typing import Optional, List, Dict, Set, Tuple
 
 from reasoner_validator.biolink import (
     BiolinkValidator,
     get_biolink_model_toolkit
 )
+from reasoner_validator.biolink.ontology import get_parent_concept
 
 from reasoner_validator.report import TRAPIGraphType
 from reasoner_validator.trapi import (
     LATEST_TRAPI_RELEASE,
     TRAPI_1_4_0_SEMVER,
     check_node_edge_mappings
 )
@@ -414,99 +415,153 @@
                     #         )
                     #         # data_dump=f"Resolved aliases:\n{','.join(output_aliases)}\n" +
                     #         #           f"Result object IDs:\n{_output(object_ids,flat=True)}"
 
         # Only 'error' but not 'info' nor 'warning' messages invalidate the overall Message
         return False if self.has_errors() else True
 
-    def category_matched(self, source_categories: List[str], target_categories: List[str]) -> bool:
+    def category_matched(self, source_categories: List[str], target_categories: List[str]) -> Optional[str]:
         """
         For each 'source' Biolink Model category given (list of CURIEs as strings?),
         first get the union set of all parent (ancestral) categories, then check if
         at least one of these categories is matched to the list of target categories.
 
         :param source_categories: List[str], list of 'source' categories whose category hierarchy is to be matched.
         :param target_categories: List[str], list of 'target' categories to be matched against 'source'
                                              (or 'source parent' categories
-        :return: bool, True if a category match is found (as described above)
+        :return: bool, returned category matched (could be a generic parent of a 'source' category)
         """
         source_category_set: Set = set()
         # gather all the possible exact and ancestor (parent)
         # categories of source_categories to match...
         for source_category in source_categories:
             source_category_set.update(self.bmt.get_ancestors(source_category, formatted=True, mixin=False))
+
         # ...then check all the target categories against that source category set
-        return any([c in target_categories for c in source_category_set])
+        for category in source_category_set:
+            if category in target_categories:
+                return category
+
+        # Nothing matched
+        return None
+
+    def testcase_node_category_found(
+            self,
+            target,
+            identifier,
+            testcase,
+            node_details
+    ) -> Optional[str]:
+        # For this comparison, we assume that a specified node category plus all its
+        # parent categories, may be used to match the test testcase specified category.
+        test_case_category: str = testcase[f"{target}_category"]
+        if "categories" in node_details:
+            category: Optional[str] = self.category_matched(
+                source_categories=node_details["categories"],
+                target_categories=[test_case_category]
+            )
+            if category is not None:
+                # The 'identifier' was present in the list of KG nodes, plus there was a match of the target
+                # testcase category either exactly to a specified one of the indicated KG node categories or to
+                # an ancestral ("parent") category of one of the node categories. This is a completely regular
+                # result. For example, if a KG node return is "biolink:Gene", but the testcase query is only
+                # expecting to see a "biolink:BiologicalEntity", however, since the identifier is matched
+                # exactly, since the node match is good with greater categorical precision than expected.
+                return category
+
+            # if a direct category match failed, try matching the inverse
+            category = self.category_matched(
+                source_categories=[test_case_category],
+                target_categories=node_details["categories"]
+            )
+            if category is not None:
+                # The 'identifier' was present in the list of KG nodes;
+                # however, there was likely only a more general ("parent-level") category match
+                # of at least one of the KG node categories, to a parent category of the testcase category
+                # (since the 'exact match' match scenario was handled above). This is a less precise
+                # node match, hence we issue a warning. For example, maybe the KG node returned is only
+                # tagged as "biolink:NamedThing" but we are looking for a testcase with "biolink:Gene".
+                # Since the testcase identifier was matched exactly, we assume that the node is matched,
+                # but just with less than desired data type categorical precision.
+                self.report(
+                    code="warning.trapi.response.message.knowledge_graph.node.category.imprecise",
+                    identifier=identifier,
+                    expected_category=test_case_category,
+                    observed_categories=",".join(node_details["categories"])
+                )
+                return category
 
-    def testcase_node_found(self, target: str, identifiers: List[str], testcase: Dict, nodes: Dict) -> bool:
+        return None
+
+    def testcase_node_found(
+            self,
+            target: str,
+            target_id_aliases: List[str],
+            testcase: Dict,
+            nodes: Dict
+    ) -> Optional[Tuple[str, str, Optional[str]]]:
         """
-        Check for presence of the target identifier, with expected categories, in the "nodes" catalog.
-        If the identifier is found, and at least one KG node category is the expected category or a proper subclass
+        Check for presence of at least one of the given identifiers, with expected categories, in the "nodes" catalog.
+        If such identifier is found, and at least one KG node category is the expected category or a proper subclass
         category of the test testcase category, then return True; if the node is found but the testcase category is not
         the expected category but is a subclass category of the KG node categories (i.e. KG node categories
         are too general), then return False. If the identifier is NOT found in the nodes list or
         there is no overlap in the (expected or parent) testcase and node categories, then return False.
 
-        :param target: 'subject' or 'object'
-        :param identifiers: List of node (CURIE) identifiers to be checked in the "nodes" catalog
+        :param target: the concept node type of interest: the 'subject' or the 'object'
+        :param target_id_aliases: List of (CURIE) target identifier aliases to be matched against the "nodes" catalog
         :param testcase: Dict, full test testcase (to access the target node 'category')
-        :param nodes: Dict, nodes category indexed by node identifiers.
-        :return: bool, True if feasible node identifier and category match; False otherwise
+        :param nodes: Dict, details about knowledge graph nodes, indexed by node identifiers.
+        :return: Optional[Tuple[str, str, Optional[str]]], returns the KG node identifier, category, and
+                                                           query identifier matched (if applicable); None if no match
         """
         #
         #     "nodes": {
         #         "MONDO:0005148": {"name": "type-2 diabetes"},
         #         "CHEBI:6801": {"name": "metformin", "categories": ["biolink:Drug"]}
         #     }
         #
 
         # Sanity check
         assert target in ["subject", "object"]
-        for identifier in identifiers:
-            if identifier in nodes.keys():
+        for node_id in nodes.keys():
+            node_details = nodes[node_id]
+            category: Optional[str]
+            if node_id in target_id_aliases:
                 # Found the target node identifier, but is the expected category present?
-                # For this comparison, we assume that a specified node category plus all its
-                # parent categories, may be used to match the test testcase specified category.
-                node_details = nodes[identifier]
-                test_case_category: str = testcase[f"{target}_category"]
-                if "categories" in node_details:
-                    if self.category_matched(
-                            source_categories=node_details["categories"],
-                            target_categories=[test_case_category]
-                    ):
-                        # The 'identifier' was present in the list of KG nodes, plus there was a match of the target
-                        # testcase category either exactly to a specified one of the indicated KG node categories or to
-                        # an ancestral ("parent") category of one of the node categories. This is a completely regular
-                        # result. For example, if a KG node return is "biolink:Gene", but the testcase query is only
-                        # expecting to see a "biolink:BiologicalEntity", however, since the identifier is matched
-                        # exactly, since the node match is good with greater categorical precision than expected.
-                        return True
-                    elif self.category_matched(
-                            source_categories=[test_case_category],
-                            target_categories=node_details["categories"]
-                    ):
-                        # The 'identifier' was present in the list of KG nodes;
-                        # however, there was likely only a more general ("parent-level") category match
-                        # of at least one of the KG node categories, to a parent category of the testcase category
-                        # (since the 'exact match' match scenario was handled above). This is a less precise
-                        # node match, hence we issue a warning. For example, maybe the KG node returned is only
-                        # tagged as "biolink:NamedThing" but we are looking for a testcase with "biolink:Gene".
-                        # Since the testcase identifier was matched exactly, we assume that the node is matched,
-                        # but just with less than desired data type categorical precision.
-                        self.report(
-                            code="warning.trapi.response.message.knowledge_graph.node.category.imprecise",
-                            identifier=identifier,
-                            expected_category=test_case_category,
-                            observed_categories=",".join(node_details["categories"])
-                        )
-                        return True
+                category: Optional[str] = self.testcase_node_category_found(target, node_id, testcase, node_details)
+                if category:
+                    return node_id, category, None  # no query_id is given since the node is directly matched.
+            else:
+                # the current node identifier is not one of the target aliases, but we
+                # need to check whether the node_id is a subclass instance of an ontology
+                # term identifier which does match an alias of the target identifier
+                # For this search, we assume the testcase category
+                category = testcase[f"{target}_category"]
+                parent_of_node_id: Optional[str] = get_parent_concept(
+                    curie=node_id,
+                    category=category,
+                    biolink_version=self.get_biolink_version()
+                )
+                # TODO: do we need to worry about also making a more complete comparisons
+                #       of the aliases of the 'parent_of_node_id' against the 'target_id_aliases'?
+                if parent_of_node_id and parent_of_node_id in target_id_aliases:
+                    self.report(
+                        code="info.trapi.response.message.knowledge_graph.node.parent.match",
+                        identifier=parent_of_node_id,
+                        query_id=parent_of_node_id,
+                        context=target
+                    )
+                    return node_id, category, parent_of_node_id
 
-        # Target node identifier is missing from the list of KG nodes or categories is either missing
-        # or not annotated with any compatible category, hence, we deem the node effectively missing.
-        return False
+        # Target node identifier doesn't match directly or indirectly
+        # to node in the list of KG nodes or  categories are either
+        # missing or not annotated  with any compatible category,
+        # hence, we deem the node effectively missing.
+        return None
 
     @staticmethod
     def testcase_edge_bindings(q_edge_ids: List[str], target_edge_id: str, data: Dict) -> bool:
         """
         Check if target query edge id and knowledge graph edge id are in specified edge_bindings.
         :rtype: object
         :param q_edge_ids: List[str], expected query edge identifiers in a matching result
@@ -525,27 +580,32 @@
                             return True
         return False
 
     def testcase_result_found(
             self,
             query_graph: Dict,
             subject_id: str,
+            subject_query_id: Optional[str],
             object_id: str,
+            object_query_id: Optional[str],
             edge_id: str,
             results: List
     ) -> bool:
         """
         Validate that test testcase S--P->O edge is found bound to the Results?
         :param query_graph: Dict, query graph to which the results pertain
         :param subject_id: str, subject node (CURIE) identifier
-        :param object_id:  str, subject node (CURIE) identifier
-        :param edge_id:  str, subject node (CURIE) identifier
+        :param subject_query_id: Optional[str], subject node (CURIE) query node identifier (if applicable)
+        :param object_id:  str, object node (CURIE) identifier
+        :param object_query_id:  Optional[str], object node (CURIE) query node identifier (if applicable)
+        :param edge_id:  str, edge identifier
         :param results: List of (TRAPI-version specific) Result objects
         :return: bool, True if testcase S-P-O edge was found in the results
         """
+        # TODO: need to implement some kind of validation of 'subject_query_id' and 'object_query_id'
         assert query_graph, "testcase_result_found() encountered an empty query graph"
         q_edges: Dict = query_graph["edges"]
         q_edge_ids = list(q_edges.keys())
 
         result_found: bool = False
         result: Dict
 
@@ -654,14 +714,52 @@
 
             if subject_id_found and object_id_found and edge_id_found:
                 result_found = True
                 break
 
         return result_found
 
+    def resolve_testcase_node(
+            self,
+            target: str,
+            testcase: Dict,
+            nodes: Dict
+    ) -> Optional[Tuple[str, str, Optional[str]]]:
+        """
+        Resolve the knowledge graph node identifiers against the testcase
+        identifier of the 'target' context ('subject' or 'object' node).
+        If a direct match is not found for the testcase identifier,
+        check if the nodes identifiers returned in the knowledge graph
+        are strict ontological subclasses of the target testcase identifier
+        (e.g. the knowledge graph may return a subclass of an instance of
+        MONDO disease as requested by the testcase). Node matches must
+        also be compatible in terms of Biolink Model category.
+
+        :param target: 'subject' or 'object'
+        :param testcase: Dict, full test testcase (to access the target node 'category')
+        :param nodes: Dict, details about knowledge graph nodes, indexed by node identifiers
+        :return: Optional[Tuple[str, str, Optional[str]]], returns the KG node identifier, category, and
+                                                           query identifier matched (if applicable); None if no match
+        """
+        target_id: str = testcase[f"{target}_id"] if f"{target}_id" in testcase else testcase[target]
+        target_id_aliases = get_aliases(target_id)
+        match: Optional[Tuple[str, str, Optional[str]]] = \
+            self.testcase_node_found(target, target_id_aliases, testcase, nodes)
+        if match:
+            # Direct match! Return matched identifier and category
+            return match
+        else:
+            # Node matching failed... report the error
+            self.report(
+                code="error.trapi.response.message.knowledge_graph.node.missing",
+                identifier=target_id,
+                context=target
+            )
+            return None
+
     def testcase_input_found_in_response(
             self,
             testcase: Dict,
             response: Dict
     ) -> bool:
         """
         Predicate to validate if test data test case specified edge is returned
@@ -770,36 +868,30 @@
         # In the Knowledge Graph:
         #
         #     "nodes": {
         #         "MONDO:0005148": {"name": "type-2 diabetes"},
         #         "CHEBI:6801": {"name": "metformin", "categories": ["biolink:Drug"]}
         #     }
         #
+
         # Check for testcase 'subject_id' and 'object_id',
         # with expected categories, in nodes catalog
         nodes: Dict = knowledge_graph["nodes"]
-        subject_id: str = testcase["subject_id"] if "subject_id" in testcase else testcase["subject"]
-        subject_aliases = get_aliases(subject_id)
-        if not self.testcase_node_found("subject", subject_aliases, testcase, nodes):
-            self.report(
-                code="error.trapi.response.message.knowledge_graph.node.missing",
-                identifier=subject_id,
-                context="subject"
-            )
+
+        subject_node_match: Optional[Tuple[str, str, Optional[str]]] = \
+            self.resolve_testcase_node(target="subject", testcase=testcase, nodes=nodes)
+        if not subject_node_match:
             return False
+        subject_match, subject_category_match, subject_query_id = subject_node_match
 
-        object_id: str = testcase["object_id"] if "object_id" in testcase else testcase["object"]
-        object_aliases = get_aliases(object_id)
-        if not self.testcase_node_found("object", object_aliases, testcase, nodes):
-            self.report(
-                code="error.trapi.response.message.knowledge_graph.node.missing",
-                identifier=object_id,
-                context="object"
-            )
+        object_node_match: Optional[Tuple[str, str, Optional[str]]] = \
+            self.resolve_testcase_node(target="object", testcase=testcase, nodes=nodes)
+        if not object_node_match:
             return False
+        object_match, object_category_match, object_query_id = object_node_match
 
         # In the Knowledge Graph:
         #
         #     "edges": {
         #         "df87ff82": {
         #             "subject": "CHEBI:6801",
         #             "predicate": "biolink:treats",
@@ -816,55 +908,70 @@
         inverse_predicate_descendants: List[str] = list()  # may sometimes remain empty...
         if self.validate_biolink():
             predicate_descendants = self.bmt.get_descendants(predicate, formatted=True)
             inverse_predicate = self.get_inverse_predicate(predicate)
             if inverse_predicate:
                 inverse_predicate_descendants = self.bmt.get_descendants(inverse_predicate, formatted=True)
         else:
-            # simpler testcase in which we are ignoring deep Biolink Model validation
+            # simpler testcase in which we are
+            # ignoring deep Biolink Model validation
             predicate_descendants = [predicate]
 
         edge_id_match: Optional[str] = None
-        subject_match: Optional[str] = None
-        object_match: Optional[str] = None
+        edge_subject_match: Optional[str] = None
+        edge_subject_query_id_match: Optional[str] = None
+        edge_object_match: Optional[str] = None
+        edge_object_query_id_match: Optional[str] = None
         for edge_id, edge in edges.items():
             # Note: this edge search could be arduous on a big knowledge graph?
-            if edge["subject"] in subject_aliases and \
+            if edge["subject"] == subject_match and \
                     edge["predicate"] in predicate_descendants and \
-                    edge["object"] in object_aliases:
+                    edge["object"] == object_match:
                 edge_id_match = edge_id
-                subject_match = edge["subject"]
-                object_match = edge["object"]
+                edge_subject_query_id_match = subject_query_id
+                edge_subject_match = subject_match
+                edge_object_query_id_match = object_query_id
+                edge_object_match = object_match
                 break
-            elif edge["subject"] in object_aliases and \
+            elif edge["subject"] == object_match and \
                     edge["predicate"] in inverse_predicate_descendants and \
-                    edge["object"] in subject_aliases:
+                    edge["object"] == subject_match:
                 # observation of the inverse edge is also counted as a match?
-                subject_match = edge["subject"]
-                object_match = edge["object"]
+                edge_subject_match = object_match
+                edge_subject_query_id_match = object_query_id
+                edge_object_match = subject_match
+                edge_object_query_id_match = subject_query_id
                 edge_id_match = edge_id
                 break
 
-        edge_id: str = \
+        testcase_edge_id: str = \
             f"{testcase['idx']}|" +\
             f"({testcase['subject_id']}#{testcase['subject_category']})" + \
             f"-[{predicate}]->" + \
             f"({testcase['object_id']}#{testcase['object_category']})"
 
         if edge_id_match is None:
             self.report(
                 code="error.trapi.response.message.knowledge_graph.edge.missing",
-                identifier=edge_id
+                identifier=testcase_edge_id
             )
             return False
 
         results: List = message["results"]
-        if not self.testcase_result_found(query_graph, subject_match, object_match, edge_id_match, results):
+        if not self.testcase_result_found(
+            query_graph,
+            edge_subject_match,
+            edge_subject_query_id_match,
+            edge_object_match,
+            edge_object_query_id_match,
+            edge_id_match,
+            results
+        ):
             self.report(
                 code="error.trapi.response.message.result.missing",
-                identifier=edge_id
+                identifier=testcase_edge_id
             )
             return False
 
         # By this point, the testcase data assumed to be
         # successfully validated in the TRAPI Response?
         return True
```

### Comparing `reasoner_validator-4.2.2/reasoner_validator/versioning.py` & `reasoner_validator-4.2.3/reasoner_validator/versioning.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.2.2/tests/__init__.py` & `reasoner_validator-4.2.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.2.2/tests/test_biolink_compliance_validation.py` & `reasoner_validator-4.2.3/tests/test_biolink_compliance_validation.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.2.2/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml` & `reasoner_validator-4.2.3/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.2.2/tests/test_ontology.py` & `reasoner_validator-4.2.3/tests/test_ontology.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.2.2/tests/test_response_validator.py` & `reasoner_validator-4.2.3/tests/test_response_validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1202,50 +1202,50 @@
     validator: TRAPIResponseValidator = TRAPIResponseValidator()
     validator.check_compliance_of_trapi_response(response=response)
     validator.dump(file=stderr)
     print("\n"+"="*80+"\n", file=stderr)
 
 
 @pytest.mark.parametrize(
-    "source_categories,target_categories,outcome",
+    "source_categories,target_categories,category_matched",
     [
         (   # query 0 - empty lists don't have anything to match?
-            [], [], False
+            [], [], None
         ),
         (   # query 1 - exact matches should be true
-            ["biolink:Gene"], ["biolink:Gene"], True
+            ["biolink:Gene"], ["biolink:Gene"], "biolink:Gene"
         ),
         (   # query 2 - biolink:Protein is **not** directly matched in the
             #           'source' hierarchy (even though its parents could overlap)
-            ["biolink:Gene"], ["biolink:Drug"], False
+            ["biolink:Gene"], ["biolink:Drug"], None
         ),
         (   # query 3 - but a 'target' category list with at least one exact
             #           match of category to source will also be matched,
             #           even if other target entries don't match
-            ["biolink:Gene"], ["biolink:Gene", "biolink:Drug"], True
+            ["biolink:Gene"], ["biolink:Gene", "biolink:Drug"], "biolink:Gene"
         ),
         (   # query 4 - 'target' category matches at least one
             #           parent of the list of 'source' categories
-            ["biolink:Gene"], ["biolink:BiologicalEntity"], True
+            ["biolink:Gene"], ["biolink:BiologicalEntity"], "biolink:BiologicalEntity"
         ),
         (   # query 5 - a 'target' category list matches at least
             #           one match to a parent of the list of the
             #           'source' categories, will be matched,
             #           even if other target entries don't match
             #
-            ["biolink:Gene"], ["biolink:BiologicalEntity", "biolink:Drug"], True
+            ["biolink:Gene"], ["biolink:BiologicalEntity", "biolink:Drug"], "biolink:BiologicalEntity"
         )
     ]
 )
-def test_category_matched(source_categories: List[str], target_categories: List[str], outcome: bool):
+def test_category_matched(source_categories: List[str], target_categories: List[str], category_matched: Optional[str]):
     validator = TRAPIResponseValidator()
     assert validator.category_matched(
         source_categories,
         target_categories,
-    ) is outcome
+    ) == category_matched
 
 
 @pytest.mark.parametrize(
     "case,response",
     [
         (dict(), {"empty": "nonsense"}),
         ({"empty": "nonsense"}, dict()),
@@ -1448,21 +1448,15 @@
                 "message": {
                     "query_graph": SAMPLE_QUERY_GRAPH,
                     "knowledge_graph": {
                         "nodes": {
                             "MONDO:0005148": {"name": "type-2 diabetes", "categories": ["biolink:Disease"]},
                             # "ncats.drug:9100L32L2N": {"name": "metformin", "categories": ["biolink:Drug"]}
                         },
-                        "edges": {
-                            "df87ff82": {
-                                "subject": "CHEBI:3002",
-                                "predicate": "biolink:treated_by",
-                                "object": "MESH:D001249"
-                            }
-                        }
+                        "edges": SAMPLE_TEST_EDGES
                     },
                     "results": SAMPLE_TEST_RESULTS
                 }
             },
             "error.trapi.response.message.knowledge_graph.node.missing"
         ),
         (   # Query 7 - missing message edge
```

### Comparing `reasoner_validator-4.2.2/tests/test_semver.py` & `reasoner_validator-4.2.3/tests/test_semver.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.2.2/tests/test_trapi_versioning.py` & `reasoner_validator-4.2.3/tests/test_trapi_versioning.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.2.2/tests/test_utils.py` & `reasoner_validator-4.2.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.2.2/tests/test_validate.py` & `reasoner_validator-4.2.3/tests/test_validate.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.2.2/tests/test_validation_report.py` & `reasoner_validator-4.2.3/tests/test_validation_report.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.2.2/tests/test_workflows.py` & `reasoner_validator-4.2.3/tests/test_workflows.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.2.2/PKG-INFO` & `reasoner_validator-4.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-validator
-Version: 4.2.2
+Version: 4.2.3
 Summary: Validation tools for Reasoner API
 Home-page: https://github.com/NCATSTranslator
 License: MIT
 Keywords: NCATS,Biomedical Data Translator,Translator,ReasonerAPI,TRAPI,validation,Biolink Model
 Author: Richard Bruskiewich
 Author-email: richard.bruskiewich@delphinai.com
 Maintainer: Richard Bruskiewich
```

