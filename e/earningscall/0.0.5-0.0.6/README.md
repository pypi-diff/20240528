# Comparing `tmp/earningscall-0.0.5.tar.gz` & `tmp/earningscall-0.0.6.tar.gz`

## Comparing `earningscall-0.0.5.tar` & `earningscall-0.0.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 earningscall-0.0.5/.python-version
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 earningscall-0.0.5/CHANGELOG.md
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 earningscall-0.0.5/DEVELOPMENT.md
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 earningscall-0.0.5/TODO.md
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 earningscall-0.0.5/requirements-dev.lock
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 earningscall-0.0.5/requirements.lock
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 earningscall-0.0.5/.github/workflows/release.yml
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 earningscall-0.0.5/earningscall/__init__.py
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 earningscall-0.0.5/earningscall/api.py
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 earningscall-0.0.5/earningscall/company.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 earningscall-0.0.5/earningscall/errors.py
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 earningscall-0.0.5/earningscall/event.py
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 earningscall-0.0.5/earningscall/exports.py
--rw-r--r--   0        0        0     5946 2020-02-02 00:00:00.000000 earningscall-0.0.5/earningscall/sectors.py
--rw-r--r--   0        0        0     7722 2020-02-02 00:00:00.000000 earningscall-0.0.5/earningscall/symbols.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 earningscall-0.0.5/earningscall/transcript.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 earningscall-0.0.5/earningscall/utils.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 earningscall-0.0.5/scripts/get_all_company_transcripts.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 earningscall-0.0.5/scripts/get_single_transcript.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 earningscall-0.0.5/scripts/list_all_companies.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 earningscall-0.0.5/tests/test_earnings_event.py
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 earningscall-0.0.5/tests/test_get_transcript.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 earningscall-0.0.5/tests/test_helper.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 earningscall-0.0.5/tests/test_simple.py
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 earningscall-0.0.5/tests/test_symbols.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 earningscall-0.0.5/tests/data/demo-symbols-v2.yaml
--rw-r--r--   0        0        0    60484 2020-02-02 00:00:00.000000 earningscall-0.0.5/tests/data/msft-transcript-response.yaml
--rw-r--r--   0        0        0   264578 2020-02-02 00:00:00.000000 earningscall-0.0.5/tests/data/symbols-v2.yaml
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 earningscall-0.0.5/tests/data/symbols.txt
--rw-r--r--   0        0        0   216684 2020-02-02 00:00:00.000000 earningscall-0.0.5/tests/data/symbols.yaml
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 earningscall-0.0.5/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 earningscall-0.0.5/LICENSE
--rw-r--r--   0        0        0     3407 2020-02-02 00:00:00.000000 earningscall-0.0.5/README.md
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 earningscall-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 earningscall-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 earningscall-0.0.6/.python-version
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 earningscall-0.0.6/CHANGELOG.md
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 earningscall-0.0.6/DEVELOPMENT.md
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 earningscall-0.0.6/TODO.md
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 earningscall-0.0.6/requirements-dev.lock
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 earningscall-0.0.6/requirements.lock
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 earningscall-0.0.6/.github/workflows/release.yml
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 earningscall-0.0.6/earningscall/__init__.py
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 earningscall-0.0.6/earningscall/api.py
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 earningscall-0.0.6/earningscall/company.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 earningscall-0.0.6/earningscall/errors.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 earningscall-0.0.6/earningscall/event.py
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 earningscall-0.0.6/earningscall/exports.py
+-rw-r--r--   0        0        0     5946 2020-02-02 00:00:00.000000 earningscall-0.0.6/earningscall/sectors.py
+-rw-r--r--   0        0        0     7722 2020-02-02 00:00:00.000000 earningscall-0.0.6/earningscall/symbols.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 earningscall-0.0.6/earningscall/transcript.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 earningscall-0.0.6/earningscall/utils.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 earningscall-0.0.6/scripts/get_all_company_transcripts.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 earningscall-0.0.6/scripts/get_single_transcript.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 earningscall-0.0.6/scripts/list_all_companies.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 earningscall-0.0.6/tests/test_earnings_event.py
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 earningscall-0.0.6/tests/test_get_transcript.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 earningscall-0.0.6/tests/test_helper.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 earningscall-0.0.6/tests/test_simple.py
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 earningscall-0.0.6/tests/test_symbols.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 earningscall-0.0.6/tests/data/demo-symbols-v2.yaml
+-rw-r--r--   0        0        0    60484 2020-02-02 00:00:00.000000 earningscall-0.0.6/tests/data/msft-transcript-response.yaml
+-rw-r--r--   0        0        0   264578 2020-02-02 00:00:00.000000 earningscall-0.0.6/tests/data/symbols-v2.yaml
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 earningscall-0.0.6/tests/data/symbols.txt
+-rw-r--r--   0        0        0   216684 2020-02-02 00:00:00.000000 earningscall-0.0.6/tests/data/symbols.yaml
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 earningscall-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 earningscall-0.0.6/LICENSE
+-rw-r--r--   0        0        0     3410 2020-02-02 00:00:00.000000 earningscall-0.0.6/README.md
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 earningscall-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 earningscall-0.0.6/PKG-INFO
```

### Comparing `earningscall-0.0.5/DEVELOPMENT.md` & `earningscall-0.0.6/DEVELOPMENT.md`

 * *Files identical despite different names*

### Comparing `earningscall-0.0.5/requirements-dev.lock` & `earningscall-0.0.6/requirements-dev.lock`

 * *Files 19% similar despite different names*

```diff
@@ -19,16 +19,14 @@
     # via earningscall
 idna==3.7
     # via requests
 iniconfig==2.0.0
     # via pytest
 marshmallow==3.21.2
     # via dataclasses-json
-more-itertools==10.2.0
-    # via earningscall
 mypy-extensions==1.0.0
     # via typing-inspect
 packaging==24.0
     # via marshmallow
     # via pytest
 pluggy==1.5.0
     # via pytest
```

### Comparing `earningscall-0.0.5/requirements.lock` & `earningscall-0.0.6/requirements.lock`

 * *Files 16% similar despite different names*

```diff
@@ -17,16 +17,14 @@
     # via earningscall
 dataclasses-json==0.6.6
     # via earningscall
 idna==3.7
     # via requests
 marshmallow==3.21.2
     # via dataclasses-json
-more-itertools==10.2.0
-    # via earningscall
 mypy-extensions==1.0.0
     # via typing-inspect
 packaging==24.0
     # via marshmallow
 requests==2.32.2
     # via earningscall
 typing-extensions==4.12.0
```

### Comparing `earningscall-0.0.5/.github/workflows/release.yml` & `earningscall-0.0.6/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `earningscall-0.0.5/earningscall/api.py` & `earningscall-0.0.6/earningscall/api.py`

 * *Files identical despite different names*

### Comparing `earningscall-0.0.5/earningscall/company.py` & `earningscall-0.0.6/earningscall/company.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,14 +26,16 @@
         return str(self.name)
 
     def name(self) -> str:
         return self.company_info.name
 
     def _get_events(self):
         raw_response = api.get_events(self.company_info.exchange, self.company_info.symbol)
+        if not raw_response:
+            return []
         return [EarningsEvent.from_dict(event) for event in raw_response["events"]]
 
     def events(self) -> [EarningsEvent]:
         if not self._events:
             self._events = self._get_events()
         return self._events
```

### Comparing `earningscall-0.0.5/earningscall/event.py` & `earningscall-0.0.6/earningscall/event.py`

 * *Files identical despite different names*

### Comparing `earningscall-0.0.5/earningscall/exports.py` & `earningscall-0.0.6/earningscall/exports.py`

 * *Files identical despite different names*

### Comparing `earningscall-0.0.5/earningscall/sectors.py` & `earningscall-0.0.6/earningscall/sectors.py`

 * *Files identical despite different names*

### Comparing `earningscall-0.0.5/earningscall/symbols.py` & `earningscall-0.0.6/earningscall/symbols.py`

 * *Files identical despite different names*

### Comparing `earningscall-0.0.5/tests/test_earnings_event.py` & `earningscall-0.0.6/tests/test_earnings_event.py`

 * *Files identical despite different names*

### Comparing `earningscall-0.0.5/tests/test_get_transcript.py` & `earningscall-0.0.6/tests/test_get_transcript.py`

 * *Files identical despite different names*

### Comparing `earningscall-0.0.5/tests/test_simple.py` & `earningscall-0.0.6/tests/test_simple.py`

 * *Files identical despite different names*

### Comparing `earningscall-0.0.5/tests/test_symbols.py` & `earningscall-0.0.6/tests/test_symbols.py`

 * *Files identical despite different names*

### Comparing `earningscall-0.0.5/tests/data/msft-transcript-response.yaml` & `earningscall-0.0.6/tests/data/msft-transcript-response.yaml`

 * *Files identical despite different names*

### Comparing `earningscall-0.0.5/tests/data/symbols-v2.yaml` & `earningscall-0.0.6/tests/data/symbols-v2.yaml`

 * *Files identical despite different names*

### Comparing `earningscall-0.0.5/tests/data/symbols.yaml` & `earningscall-0.0.6/tests/data/symbols.yaml`

 * *Files identical despite different names*

### Comparing `earningscall-0.0.5/LICENSE` & `earningscall-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `earningscall-0.0.5/README.md` & `earningscall-0.0.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 
 for company in get_all_companies():
     print(f"{company.company_info} -- {company.company_info.sector} -- {company.company_info.industry}")
 ```
 
 By default, this library grants you access to only two companies, Apple Inc. and Microsoft, Inc.
 
-To gain access 5,000+ companies please [signup here](https://earningscall.biz/api-pricing) to get your API key.
+To gain access to 5,000+ companies please [signup here](https://earningscall.biz/api-pricing) to get your API key.
 
 Once you have access to your API key, you can set the API Key like this:
 
 ```python
 
 import earningscall
```

### Comparing `earningscall-0.0.5/pyproject.toml` & `earningscall-0.0.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 [project]
 name = "earningscall"
-version = "0.0.5"
+version = "0.0.6"
 description = "The EarningsCall Python library."
 readme = "README.md"
 authors = [
     {name = "EarningsCall", email = "dev@earningscall.biz"},
 ]
 requires-python = ">= 3.8"
 dependencies = [
     "dataclasses>=0.6",
     "dataclasses-json>=0.6.4",
-    "more_itertools>=10.0.0",
     "requests>=2.30.0",
 ]
 
 [project.urls]
 Homepage = "https://earningscall.biz"
 Documentation = "https://github.com/EarningsCall/earningscall-python"
 Repository = "https://github.com/EarningsCall/earningscall-python"
```

### Comparing `earningscall-0.0.5/PKG-INFO` & `earningscall-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.3
 Name: earningscall
-Version: 0.0.5
+Version: 0.0.6
 Summary: The EarningsCall Python library.
 Project-URL: Homepage, https://earningscall.biz
 Project-URL: Documentation, https://github.com/EarningsCall/earningscall-python
 Project-URL: Repository, https://github.com/EarningsCall/earningscall-python
 Project-URL: Issues, https://github.com/EarningsCall/earningscall-python/issues
 Project-URL: Source, https://github.com/EarningsCall/earningscall-python
 Project-URL: Changelog, https://github.com/EarningsCall/earningscall-python/blob/master/CHANGELOG.md
 Author-email: EarningsCall <dev@earningscall.biz>
 License-File: LICENSE
 Requires-Python: >=3.8
 Requires-Dist: dataclasses-json>=0.6.4
 Requires-Dist: dataclasses>=0.6
-Requires-Dist: more-itertools>=10.0.0
 Requires-Dist: requests>=2.30.0
 Description-Content-Type: text/markdown
 
 # EarningsCall Python Library
 
 [![pypi](https://img.shields.io/pypi/v/earningscall.svg)](https://pypi.python.org/pypi/earningscall)
 [![Build Status](https://github.com/EarningsCall/earningscall-python/actions/workflows/release.yml/badge.svg?branch=master)](https://github.com/EarningsCall/earningscall-python/actions?query=branch%3Amaster)
@@ -104,15 +103,15 @@
 
 for company in get_all_companies():
     print(f"{company.company_info} -- {company.company_info.sector} -- {company.company_info.industry}")
 ```
 
 By default, this library grants you access to only two companies, Apple Inc. and Microsoft, Inc.
 
-To gain access 5,000+ companies please [signup here](https://earningscall.biz/api-pricing) to get your API key.
+To gain access to 5,000+ companies please [signup here](https://earningscall.biz/api-pricing) to get your API key.
 
 Once you have access to your API key, you can set the API Key like this:
 
 ```python
 
 import earningscall
```

