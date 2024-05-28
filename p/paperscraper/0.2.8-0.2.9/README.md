# Comparing `tmp/paperscraper-0.2.8.tar.gz` & `tmp/paperscraper-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paperscraper-0.2.8.tar", last modified: Fri Dec  8 05:24:51 2023, max compression
+gzip compressed data, was "paperscraper-0.2.9.tar", last modified: Sun Dec 24 14:10:25 2023, max compression
```

## Comparing `paperscraper-0.2.8.tar` & `paperscraper-0.2.9.tar`

### file list

```diff
@@ -1,49 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 05:24:51.168741 paperscraper-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2023-12-08 05:24:40.000000 paperscraper-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11646 2023-12-08 05:24:51.168741 paperscraper-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10568 2023-12-08 05:24:40.000000 paperscraper-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 05:24:51.164740 paperscraper-0.2.8/paperscraper/
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2023-12-08 05:24:40.000000 paperscraper-0.2.8/paperscraper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 05:24:51.164740 paperscraper-0.2.8/paperscraper/arxiv/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-08 05:24:40.000000 paperscraper-0.2.8/paperscraper/arxiv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2023-12-08 05:24:40.000000 paperscraper-0.2.8/paperscraper/arxiv/arxiv.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2023-12-08 05:24:40.000000 paperscraper-0.2.8/paperscraper/arxiv/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 05:24:51.164740 paperscraper-0.2.8/paperscraper/get_dumps/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2023-12-08 05:24:40.000000 paperscraper-0.2.8/paperscraper/get_dumps/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1484 2023-12-08 05:24:40.000000 paperscraper-0.2.8/paperscraper/get_dumps/biorxiv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2023-12-08 05:24:40.000000 paperscraper-0.2.8/paperscraper/get_dumps/chemrxiv.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1508 2023-12-08 05:24:40.000000 paperscraper-0.2.8/paperscraper/get_dumps/medrxiv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 05:24:51.164740 paperscraper-0.2.8/paperscraper/get_dumps/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 05:24:40.000000 paperscraper-0.2.8/paperscraper/get_dumps/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 05:24:51.164740 paperscraper-0.2.8/paperscraper/get_dumps/utils/chemrxiv/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2023-12-08 05:24:40.000000 paperscraper-0.2.8/paperscraper/get_dumps/utils/chemrxiv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4166 2023-12-08 05:24:40.000000 paperscraper-0.2.8/paperscraper/get_dumps/utils/chemrxiv/chemrxiv_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4482 2023-12-08 05:24:40.000000 paperscraper-0.2.8/paperscraper/get_dumps/utils/chemrxiv/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5428 2023-12-08 05:24:40.000000 paperscraper-0.2.8/paperscraper/journal_if.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2023-12-08 05:24:40.000000 paperscraper-0.2.8/paperscraper/load_dumps.py
--rw-r--r--   0 runner    (1001) docker     (127)     3603 2023-12-08 05:24:40.000000 paperscraper-0.2.8/paperscraper/pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)    16483 2023-12-08 05:24:40.000000 paperscraper-0.2.8/paperscraper/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     4830 2023-12-08 05:24:40.000000 paperscraper-0.2.8/paperscraper/postprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 05:24:51.164740 paperscraper-0.2.8/paperscraper/pubmed/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-08 05:24:40.000000 paperscraper-0.2.8/paperscraper/pubmed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3505 2023-12-08 05:24:40.000000 paperscraper-0.2.8/paperscraper/pubmed/pubmed.py
--rw-r--r--   0 runner    (1001) docker     (127)     4107 2023-12-08 05:24:40.000000 paperscraper-0.2.8/paperscraper/pubmed/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 05:24:51.164740 paperscraper-0.2.8/paperscraper/scholar/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-08 05:24:40.000000 paperscraper-0.2.8/paperscraper/scholar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3140 2023-12-08 05:24:40.000000 paperscraper-0.2.8/paperscraper/scholar/scholar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 05:24:51.164740 paperscraper-0.2.8/paperscraper/server_dumps/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2023-12-08 05:24:40.000000 paperscraper-0.2.8/paperscraper/server_dumps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2023-12-08 05:24:40.000000 paperscraper-0.2.8/paperscraper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 05:24:51.164740 paperscraper-0.2.8/paperscraper/xrxiv/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-12-08 05:24:40.000000 paperscraper-0.2.8/paperscraper/xrxiv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4816 2023-12-08 05:24:40.000000 paperscraper-0.2.8/paperscraper/xrxiv/xrxiv_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3264 2023-12-08 05:24:40.000000 paperscraper-0.2.8/paperscraper/xrxiv/xrxiv_query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 05:24:51.164740 paperscraper-0.2.8/paperscraper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11646 2023-12-08 05:24:51.000000 paperscraper-0.2.8/paperscraper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2023-12-08 05:24:51.000000 paperscraper-0.2.8/paperscraper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-08 05:24:51.000000 paperscraper-0.2.8/paperscraper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-08 05:24:51.000000 paperscraper-0.2.8/paperscraper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-12-08 05:24:51.000000 paperscraper-0.2.8/paperscraper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-12-08 05:24:51.000000 paperscraper-0.2.8/paperscraper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-08 05:24:51.168741 paperscraper-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2023-12-08 05:24:40.000000 paperscraper-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 14:10:25.367716 paperscraper-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2023-12-24 14:10:11.000000 paperscraper-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13218 2023-12-24 14:10:25.367716 paperscraper-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12140 2023-12-24 14:10:11.000000 paperscraper-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 14:10:25.363716 paperscraper-0.2.9/paperscraper/
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2023-12-24 14:10:11.000000 paperscraper-0.2.9/paperscraper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 14:10:25.367716 paperscraper-0.2.9/paperscraper/arxiv/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-24 14:10:11.000000 paperscraper-0.2.9/paperscraper/arxiv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2023-12-24 14:10:11.000000 paperscraper-0.2.9/paperscraper/arxiv/arxiv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2023-12-24 14:10:11.000000 paperscraper-0.2.9/paperscraper/arxiv/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 14:10:25.367716 paperscraper-0.2.9/paperscraper/get_dumps/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2023-12-24 14:10:11.000000 paperscraper-0.2.9/paperscraper/get_dumps/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1484 2023-12-24 14:10:11.000000 paperscraper-0.2.9/paperscraper/get_dumps/biorxiv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2023-12-24 14:10:11.000000 paperscraper-0.2.9/paperscraper/get_dumps/chemrxiv.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1508 2023-12-24 14:10:11.000000 paperscraper-0.2.9/paperscraper/get_dumps/medrxiv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 14:10:25.367716 paperscraper-0.2.9/paperscraper/get_dumps/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-24 14:10:11.000000 paperscraper-0.2.9/paperscraper/get_dumps/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 14:10:25.367716 paperscraper-0.2.9/paperscraper/get_dumps/utils/chemrxiv/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2023-12-24 14:10:11.000000 paperscraper-0.2.9/paperscraper/get_dumps/utils/chemrxiv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4166 2023-12-24 14:10:11.000000 paperscraper-0.2.9/paperscraper/get_dumps/utils/chemrxiv/chemrxiv_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4482 2023-12-24 14:10:11.000000 paperscraper-0.2.9/paperscraper/get_dumps/utils/chemrxiv/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4241 2023-12-24 14:10:11.000000 paperscraper-0.2.9/paperscraper/impact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2023-12-24 14:10:11.000000 paperscraper-0.2.9/paperscraper/load_dumps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3603 2023-12-24 14:10:11.000000 paperscraper-0.2.9/paperscraper/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16483 2023-12-24 14:10:11.000000 paperscraper-0.2.9/paperscraper/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4830 2023-12-24 14:10:11.000000 paperscraper-0.2.9/paperscraper/postprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 14:10:25.367716 paperscraper-0.2.9/paperscraper/pubmed/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-24 14:10:11.000000 paperscraper-0.2.9/paperscraper/pubmed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3505 2023-12-24 14:10:11.000000 paperscraper-0.2.9/paperscraper/pubmed/pubmed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4107 2023-12-24 14:10:11.000000 paperscraper-0.2.9/paperscraper/pubmed/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 14:10:25.367716 paperscraper-0.2.9/paperscraper/scholar/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-24 14:10:11.000000 paperscraper-0.2.9/paperscraper/scholar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2023-12-24 14:10:11.000000 paperscraper-0.2.9/paperscraper/scholar/scholar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 14:10:25.367716 paperscraper-0.2.9/paperscraper/server_dumps/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2023-12-24 14:10:11.000000 paperscraper-0.2.9/paperscraper/server_dumps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 14:10:25.367716 paperscraper-0.2.9/paperscraper/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-24 14:10:11.000000 paperscraper-0.2.9/paperscraper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2023-12-24 14:10:11.000000 paperscraper-0.2.9/paperscraper/tests/test_impactor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2023-12-24 14:10:11.000000 paperscraper-0.2.9/paperscraper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 14:10:25.367716 paperscraper-0.2.9/paperscraper/xrxiv/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2023-12-24 14:10:11.000000 paperscraper-0.2.9/paperscraper/xrxiv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4816 2023-12-24 14:10:11.000000 paperscraper-0.2.9/paperscraper/xrxiv/xrxiv_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2023-12-24 14:10:11.000000 paperscraper-0.2.9/paperscraper/xrxiv/xrxiv_query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 14:10:25.367716 paperscraper-0.2.9/paperscraper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13218 2023-12-24 14:10:25.000000 paperscraper-0.2.9/paperscraper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2023-12-24 14:10:25.000000 paperscraper-0.2.9/paperscraper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-24 14:10:25.000000 paperscraper-0.2.9/paperscraper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-24 14:10:25.000000 paperscraper-0.2.9/paperscraper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2023-12-24 14:10:25.000000 paperscraper-0.2.9/paperscraper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2023-12-24 14:10:25.000000 paperscraper-0.2.9/paperscraper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-24 14:10:25.367716 paperscraper-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2023-12-24 14:10:11.000000 paperscraper-0.2.9/setup.py
```

### Comparing `paperscraper-0.2.8/LICENSE` & `paperscraper-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.8/PKG-INFO` & `paperscraper-0.2.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paperscraper
-Version: 0.2.8
+Version: 0.2.9
 Summary: paperscraper: Package to scrape papers.
 Home-page: https://github.com/PhosphorylatedRabbits/paperscraper
 Author: Jannis Born, Matteo Manica
 Author-email: jannis.born@gmx.de, drugilsberg@gmail.com
 License: MIT
 Keywords: Academics,Science,Publication,Search,PubMed,Arxiv,Medrxiv,Biorxiv,Chemrxiv
 Classifier: Development Status :: 3 - Alpha
@@ -175,22 +175,49 @@
 title = 'Über formal unentscheidbare Sätze der Principia Mathematica und verwandter Systeme I.'
 get_citations_from_title(title)
 ```
 
 *NOTE*: The scholar endpoint does not require authentification but since it regularly
 prompts with captchas, it's difficult to apply large scale.
 
-#### Journal impact factor
+### Journal impact factor
 
-You can also retrieve the impact factor for all journals indexed by citefactor:
+You can also retrieve the impact factor for all journals:
 ```py
-from paperscraper.journal_if import Impactor
-i = Impactor()
+>>>from paperscraper.impact import Impactor
+>>>i = Impactor()
+>>>i.search("Nat Comms", threshold=85, sort_by='impact') 
+[
+    {'journal': 'Nature Communications', 'factor': 17.694, 'score': 94}, 
+    {'journal': 'Natural Computing', 'factor': 1.504, 'score': 88}
+]
+```
+This performs a fuzzy search with a threshold of 85. `threshold` defaults to 100 in which case an exact search
+is performed. You can also search by journal abbreviation, [E-ISSN](https://portal.issn.org) or [NLM ID](https://portal.issn.org).
+```py
+i.search("Nat Rev Earth Environ") # [{'journal': 'Nature Reviews Earth & Environment', 'factor': 37.214, 'score': 100}]
+i.search("101771060") # [{'journal': 'Nature Reviews Earth & Environment', 'factor': 37.214, 'score': 100}]
+i.search('2662-138X') # [{'journal': 'Nature Reviews Earth & Environment', 'factor': 37.214, 'score': 100}]
+
+# Filter results by impact factor
+i.search("Neural network", threshold=85, min_impact=1.5, max_impact=20)
+# [
+#   {'journal': 'IEEE Transactions on Neural Networks and Learning Systems', 'factor': 14.255, 'score': 93}, 
+#   {'journal': 'NEURAL NETWORKS', 'factor': 9.657, 'score': 91},
+#   {'journal': 'WORK-A Journal of Prevention Assessment & Rehabilitation', 'factor': 1.803, 'score': 86}, 
+#   {'journal': 'NETWORK-COMPUTATION IN NEURAL SYSTEMS', 'factor': 1.5, 'score': 92}
+# ]
+
+# Show all fields
+i.search("quantum information", threshold=90, return_all=True)
+# [
+#   {'factor': 10.758, 'jcr': 'Q1', 'journal_abbr': 'npj Quantum Inf', 'eissn': '2056-6387', 'journal': 'npj Quantum Information', 'nlm_id': '101722857', 'issn': '', 'score': 92},
+#   {'factor': 1.577, 'jcr': 'Q3', 'journal_abbr': 'Nation', 'eissn': '0027-8378', 'journal': 'NATION', 'nlm_id': '9877123', 'issn': '0027-8378', 'score': 91}
+# ]
 ```
-Then, `i.journal_to_if` should give you a dictionary wit journal to IF mappings for >9000 journals as of 2014.
 
 ### Plotting
 
 When multiple query searches are performed, two types of plots can be generated
 automatically: Venn diagrams and bar plots.
 
 #### Barplots
```

### Comparing `paperscraper-0.2.8/README.md` & `paperscraper-0.2.9/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -145,22 +145,49 @@
 title = 'Über formal unentscheidbare Sätze der Principia Mathematica und verwandter Systeme I.'
 get_citations_from_title(title)
 ```
 
 *NOTE*: The scholar endpoint does not require authentification but since it regularly
 prompts with captchas, it's difficult to apply large scale.
 
-#### Journal impact factor
+### Journal impact factor
 
-You can also retrieve the impact factor for all journals indexed by citefactor:
+You can also retrieve the impact factor for all journals:
 ```py
-from paperscraper.journal_if import Impactor
-i = Impactor()
+>>>from paperscraper.impact import Impactor
+>>>i = Impactor()
+>>>i.search("Nat Comms", threshold=85, sort_by='impact') 
+[
+    {'journal': 'Nature Communications', 'factor': 17.694, 'score': 94}, 
+    {'journal': 'Natural Computing', 'factor': 1.504, 'score': 88}
+]
+```
+This performs a fuzzy search with a threshold of 85. `threshold` defaults to 100 in which case an exact search
+is performed. You can also search by journal abbreviation, [E-ISSN](https://portal.issn.org) or [NLM ID](https://portal.issn.org).
+```py
+i.search("Nat Rev Earth Environ") # [{'journal': 'Nature Reviews Earth & Environment', 'factor': 37.214, 'score': 100}]
+i.search("101771060") # [{'journal': 'Nature Reviews Earth & Environment', 'factor': 37.214, 'score': 100}]
+i.search('2662-138X') # [{'journal': 'Nature Reviews Earth & Environment', 'factor': 37.214, 'score': 100}]
+
+# Filter results by impact factor
+i.search("Neural network", threshold=85, min_impact=1.5, max_impact=20)
+# [
+#   {'journal': 'IEEE Transactions on Neural Networks and Learning Systems', 'factor': 14.255, 'score': 93}, 
+#   {'journal': 'NEURAL NETWORKS', 'factor': 9.657, 'score': 91},
+#   {'journal': 'WORK-A Journal of Prevention Assessment & Rehabilitation', 'factor': 1.803, 'score': 86}, 
+#   {'journal': 'NETWORK-COMPUTATION IN NEURAL SYSTEMS', 'factor': 1.5, 'score': 92}
+# ]
+
+# Show all fields
+i.search("quantum information", threshold=90, return_all=True)
+# [
+#   {'factor': 10.758, 'jcr': 'Q1', 'journal_abbr': 'npj Quantum Inf', 'eissn': '2056-6387', 'journal': 'npj Quantum Information', 'nlm_id': '101722857', 'issn': '', 'score': 92},
+#   {'factor': 1.577, 'jcr': 'Q3', 'journal_abbr': 'Nation', 'eissn': '0027-8378', 'journal': 'NATION', 'nlm_id': '9877123', 'issn': '0027-8378', 'score': 91}
+# ]
 ```
-Then, `i.journal_to_if` should give you a dictionary wit journal to IF mappings for >9000 journals as of 2014.
 
 ### Plotting
 
 When multiple query searches are performed, two types of plots can be generated
 automatically: Venn diagrams and bar plots.
 
 #### Barplots
```

### Comparing `paperscraper-0.2.8/paperscraper/__init__.py` & `paperscraper-0.2.9/paperscraper/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Initialize the module."""
 __name__ = "paperscraper"
-__version__ = "0.2.8"
+__version__ = "0.2.9"
 
 import logging
 import os
 import sys
 from typing import List, Union
 
 from .load_dumps import QUERY_FN_DICT
```

### Comparing `paperscraper-0.2.8/paperscraper/arxiv/arxiv.py` & `paperscraper-0.2.9/paperscraper/arxiv/arxiv.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.8/paperscraper/arxiv/utils.py` & `paperscraper-0.2.9/paperscraper/arxiv/utils.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.8/paperscraper/get_dumps/biorxiv.py` & `paperscraper-0.2.9/paperscraper/get_dumps/biorxiv.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.8/paperscraper/get_dumps/chemrxiv.py` & `paperscraper-0.2.9/paperscraper/get_dumps/chemrxiv.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.8/paperscraper/get_dumps/medrxiv.py` & `paperscraper-0.2.9/paperscraper/get_dumps/medrxiv.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.8/paperscraper/get_dumps/utils/chemrxiv/chemrxiv_api.py` & `paperscraper-0.2.9/paperscraper/get_dumps/utils/chemrxiv/chemrxiv_api.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.8/paperscraper/get_dumps/utils/chemrxiv/utils.py` & `paperscraper-0.2.9/paperscraper/get_dumps/utils/chemrxiv/utils.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.8/paperscraper/load_dumps.py` & `paperscraper-0.2.9/paperscraper/load_dumps.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.8/paperscraper/pdf.py` & `paperscraper-0.2.9/paperscraper/pdf.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.8/paperscraper/plotting.py` & `paperscraper-0.2.9/paperscraper/plotting.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.8/paperscraper/postprocessing.py` & `paperscraper-0.2.9/paperscraper/postprocessing.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.8/paperscraper/pubmed/pubmed.py` & `paperscraper-0.2.9/paperscraper/pubmed/pubmed.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.8/paperscraper/pubmed/utils.py` & `paperscraper-0.2.9/paperscraper/pubmed/utils.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.8/paperscraper/scholar/scholar.py` & `paperscraper-0.2.9/paperscraper/scholar/scholar.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.8/paperscraper/utils.py` & `paperscraper-0.2.9/paperscraper/utils.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.8/paperscraper/xrxiv/xrxiv_api.py` & `paperscraper-0.2.9/paperscraper/xrxiv/xrxiv_api.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.8/paperscraper/xrxiv/xrxiv_query.py` & `paperscraper-0.2.9/paperscraper/xrxiv/xrxiv_query.py`

 * *Files identical despite different names*

### Comparing `paperscraper-0.2.8/paperscraper.egg-info/PKG-INFO` & `paperscraper-0.2.9/paperscraper.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paperscraper
-Version: 0.2.8
+Version: 0.2.9
 Summary: paperscraper: Package to scrape papers.
 Home-page: https://github.com/PhosphorylatedRabbits/paperscraper
 Author: Jannis Born, Matteo Manica
 Author-email: jannis.born@gmx.de, drugilsberg@gmail.com
 License: MIT
 Keywords: Academics,Science,Publication,Search,PubMed,Arxiv,Medrxiv,Biorxiv,Chemrxiv
 Classifier: Development Status :: 3 - Alpha
@@ -175,22 +175,49 @@
 title = 'Über formal unentscheidbare Sätze der Principia Mathematica und verwandter Systeme I.'
 get_citations_from_title(title)
 ```
 
 *NOTE*: The scholar endpoint does not require authentification but since it regularly
 prompts with captchas, it's difficult to apply large scale.
 
-#### Journal impact factor
+### Journal impact factor
 
-You can also retrieve the impact factor for all journals indexed by citefactor:
+You can also retrieve the impact factor for all journals:
 ```py
-from paperscraper.journal_if import Impactor
-i = Impactor()
+>>>from paperscraper.impact import Impactor
+>>>i = Impactor()
+>>>i.search("Nat Comms", threshold=85, sort_by='impact') 
+[
+    {'journal': 'Nature Communications', 'factor': 17.694, 'score': 94}, 
+    {'journal': 'Natural Computing', 'factor': 1.504, 'score': 88}
+]
+```
+This performs a fuzzy search with a threshold of 85. `threshold` defaults to 100 in which case an exact search
+is performed. You can also search by journal abbreviation, [E-ISSN](https://portal.issn.org) or [NLM ID](https://portal.issn.org).
+```py
+i.search("Nat Rev Earth Environ") # [{'journal': 'Nature Reviews Earth & Environment', 'factor': 37.214, 'score': 100}]
+i.search("101771060") # [{'journal': 'Nature Reviews Earth & Environment', 'factor': 37.214, 'score': 100}]
+i.search('2662-138X') # [{'journal': 'Nature Reviews Earth & Environment', 'factor': 37.214, 'score': 100}]
+
+# Filter results by impact factor
+i.search("Neural network", threshold=85, min_impact=1.5, max_impact=20)
+# [
+#   {'journal': 'IEEE Transactions on Neural Networks and Learning Systems', 'factor': 14.255, 'score': 93}, 
+#   {'journal': 'NEURAL NETWORKS', 'factor': 9.657, 'score': 91},
+#   {'journal': 'WORK-A Journal of Prevention Assessment & Rehabilitation', 'factor': 1.803, 'score': 86}, 
+#   {'journal': 'NETWORK-COMPUTATION IN NEURAL SYSTEMS', 'factor': 1.5, 'score': 92}
+# ]
+
+# Show all fields
+i.search("quantum information", threshold=90, return_all=True)
+# [
+#   {'factor': 10.758, 'jcr': 'Q1', 'journal_abbr': 'npj Quantum Inf', 'eissn': '2056-6387', 'journal': 'npj Quantum Information', 'nlm_id': '101722857', 'issn': '', 'score': 92},
+#   {'factor': 1.577, 'jcr': 'Q3', 'journal_abbr': 'Nation', 'eissn': '0027-8378', 'journal': 'NATION', 'nlm_id': '9877123', 'issn': '0027-8378', 'score': 91}
+# ]
 ```
-Then, `i.journal_to_if` should give you a dictionary wit journal to IF mappings for >9000 journals as of 2014.
 
 ### Plotting
 
 When multiple query searches are performed, two types of plots can be generated
 automatically: Venn diagrams and bar plots.
 
 #### Barplots
```

### Comparing `paperscraper-0.2.8/paperscraper.egg-info/SOURCES.txt` & `paperscraper-0.2.9/paperscraper.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 LICENSE
 README.md
 setup.py
 paperscraper/__init__.py
-paperscraper/journal_if.py
+paperscraper/impact.py
 paperscraper/load_dumps.py
 paperscraper/pdf.py
 paperscraper/plotting.py
 paperscraper/postprocessing.py
 paperscraper/utils.py
 paperscraper.egg-info/PKG-INFO
 paperscraper.egg-info/SOURCES.txt
@@ -27,10 +27,12 @@
 paperscraper/get_dumps/utils/chemrxiv/utils.py
 paperscraper/pubmed/__init__.py
 paperscraper/pubmed/pubmed.py
 paperscraper/pubmed/utils.py
 paperscraper/scholar/__init__.py
 paperscraper/scholar/scholar.py
 paperscraper/server_dumps/__init__.py
+paperscraper/tests/__init__.py
+paperscraper/tests/test_impactor.py
 paperscraper/xrxiv/__init__.py
 paperscraper/xrxiv/xrxiv_api.py
 paperscraper/xrxiv/xrxiv_query.py
```

### Comparing `paperscraper-0.2.8/setup.py` & `paperscraper-0.2.9/setup.py`

 * *Files identical despite different names*

