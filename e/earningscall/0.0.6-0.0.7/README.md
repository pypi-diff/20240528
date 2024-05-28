# Comparing `tmp/earningscall-0.0.6.tar.gz` & `tmp/earningscall-0.0.7.tar.gz`

## Comparing `earningscall-0.0.6.tar` & `earningscall-0.0.7.tar`

### file list

```diff
@@ -1,35 +1,36 @@
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 earningscall-0.0.6/.python-version
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 earningscall-0.0.6/CHANGELOG.md
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 earningscall-0.0.6/DEVELOPMENT.md
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 earningscall-0.0.6/TODO.md
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 earningscall-0.0.6/requirements-dev.lock
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 earningscall-0.0.6/requirements.lock
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 earningscall-0.0.6/.github/workflows/release.yml
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 earningscall-0.0.6/earningscall/__init__.py
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 earningscall-0.0.6/earningscall/api.py
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 earningscall-0.0.6/earningscall/company.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 earningscall-0.0.6/earningscall/errors.py
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 earningscall-0.0.6/earningscall/event.py
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 earningscall-0.0.6/earningscall/exports.py
--rw-r--r--   0        0        0     5946 2020-02-02 00:00:00.000000 earningscall-0.0.6/earningscall/sectors.py
--rw-r--r--   0        0        0     7722 2020-02-02 00:00:00.000000 earningscall-0.0.6/earningscall/symbols.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 earningscall-0.0.6/earningscall/transcript.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 earningscall-0.0.6/earningscall/utils.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 earningscall-0.0.6/scripts/get_all_company_transcripts.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 earningscall-0.0.6/scripts/get_single_transcript.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 earningscall-0.0.6/scripts/list_all_companies.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 earningscall-0.0.6/tests/test_earnings_event.py
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 earningscall-0.0.6/tests/test_get_transcript.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 earningscall-0.0.6/tests/test_helper.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 earningscall-0.0.6/tests/test_simple.py
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 earningscall-0.0.6/tests/test_symbols.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 earningscall-0.0.6/tests/data/demo-symbols-v2.yaml
--rw-r--r--   0        0        0    60484 2020-02-02 00:00:00.000000 earningscall-0.0.6/tests/data/msft-transcript-response.yaml
--rw-r--r--   0        0        0   264578 2020-02-02 00:00:00.000000 earningscall-0.0.6/tests/data/symbols-v2.yaml
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 earningscall-0.0.6/tests/data/symbols.txt
--rw-r--r--   0        0        0   216684 2020-02-02 00:00:00.000000 earningscall-0.0.6/tests/data/symbols.yaml
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 earningscall-0.0.6/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 earningscall-0.0.6/LICENSE
--rw-r--r--   0        0        0     3410 2020-02-02 00:00:00.000000 earningscall-0.0.6/README.md
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 earningscall-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 earningscall-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 earningscall-0.0.7/.python-version
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 earningscall-0.0.7/CHANGELOG.md
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 earningscall-0.0.7/DEVELOPMENT.md
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 earningscall-0.0.7/TODO.md
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 earningscall-0.0.7/requirements-dev.lock
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 earningscall-0.0.7/requirements.lock
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 earningscall-0.0.7/.github/workflows/release.yml
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 earningscall-0.0.7/earningscall/__init__.py
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 earningscall-0.0.7/earningscall/api.py
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 earningscall-0.0.7/earningscall/company.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 earningscall-0.0.7/earningscall/errors.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 earningscall-0.0.7/earningscall/event.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 earningscall-0.0.7/earningscall/exports.py
+-rw-r--r--   0        0        0     5946 2020-02-02 00:00:00.000000 earningscall-0.0.7/earningscall/sectors.py
+-rw-r--r--   0        0        0     7722 2020-02-02 00:00:00.000000 earningscall-0.0.7/earningscall/symbols.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 earningscall-0.0.7/earningscall/transcript.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 earningscall-0.0.7/earningscall/utils.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 earningscall-0.0.7/scripts/get_all_company_transcripts.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 earningscall-0.0.7/scripts/get_single_transcript.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 earningscall-0.0.7/scripts/list_all_companies.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 earningscall-0.0.7/tests/test_earnings_event.py
+-rw-r--r--   0        0        0     2684 2020-02-02 00:00:00.000000 earningscall-0.0.7/tests/test_get_transcript.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 earningscall-0.0.7/tests/test_helper.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 earningscall-0.0.7/tests/test_simple.py
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 earningscall-0.0.7/tests/test_symbols.py
+-rw-r--r--   0        0        0    60613 2020-02-02 00:00:00.000000 earningscall-0.0.7/tests/data/demo-symbols-v2-alpha.yaml
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 earningscall-0.0.7/tests/data/demo-symbols-v2.yaml
+-rw-r--r--   0        0        0    60484 2020-02-02 00:00:00.000000 earningscall-0.0.7/tests/data/msft-transcript-response.yaml
+-rw-r--r--   0        0        0   264578 2020-02-02 00:00:00.000000 earningscall-0.0.7/tests/data/symbols-v2.yaml
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 earningscall-0.0.7/tests/data/symbols.txt
+-rw-r--r--   0        0        0   216684 2020-02-02 00:00:00.000000 earningscall-0.0.7/tests/data/symbols.yaml
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 earningscall-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 earningscall-0.0.7/LICENSE
+-rw-r--r--   0        0        0     3410 2020-02-02 00:00:00.000000 earningscall-0.0.7/README.md
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 earningscall-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 earningscall-0.0.7/PKG-INFO
```

### Comparing `earningscall-0.0.6/requirements-dev.lock` & `earningscall-0.0.7/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `earningscall-0.0.6/requirements.lock` & `earningscall-0.0.7/requirements.lock`

 * *Files identical despite different names*

### Comparing `earningscall-0.0.6/.github/workflows/release.yml` & `earningscall-0.0.7/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `earningscall-0.0.6/earningscall/api.py` & `earningscall-0.0.7/earningscall/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import logging
 import os
 from typing import Optional
 
+import earningscall
 import requests
 
 
 log = logging.getLogger(__file__)
 
 DOMAIN = os.environ.get("ECALL_DOMAIN", "earningscall.biz")
 API_BASE = f"https://v2.api.{DOMAIN}"
-api_key: Optional[str] = None
 
 
 def get_api_key():
-    global api_key
-    if api_key is None:
+    api_key = earningscall.api_key
+    if not api_key:
         return os.environ.get("ECALL_API_KEY", "demo")
     return api_key
 
 
 def is_demo_account():
     return get_api_key() == "demo"
```

### Comparing `earningscall-0.0.6/earningscall/company.py` & `earningscall-0.0.7/earningscall/company.py`

 * *Files identical despite different names*

### Comparing `earningscall-0.0.6/earningscall/event.py` & `earningscall-0.0.7/earningscall/event.py`

 * *Files identical despite different names*

### Comparing `earningscall-0.0.6/earningscall/exports.py` & `earningscall-0.0.7/earningscall/exports.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,9 +14,10 @@
 
 def get_all_companies() -> [Company]:
     for company_info in get_symbols().get_all():
         yield Company(company_info=company_info)
 
 
 def get_sp500_companies() -> [Company]:
+    ## TODO: Actually only return SP500 companies.
     for company_info in get_symbols().get_all():
         yield Company(company_info=company_info)
```

### Comparing `earningscall-0.0.6/earningscall/sectors.py` & `earningscall-0.0.7/earningscall/sectors.py`

 * *Files identical despite different names*

### Comparing `earningscall-0.0.6/earningscall/symbols.py` & `earningscall-0.0.7/earningscall/symbols.py`

 * *Files identical despite different names*

### Comparing `earningscall-0.0.6/tests/test_earnings_event.py` & `earningscall-0.0.7/tests/test_earnings_event.py`

 * *Files identical despite different names*

### Comparing `earningscall-0.0.6/tests/test_simple.py` & `earningscall-0.0.7/tests/test_simple.py`

 * *Files identical despite different names*

### Comparing `earningscall-0.0.6/tests/test_symbols.py` & `earningscall-0.0.7/tests/test_symbols.py`

 * *Files identical despite different names*

### Comparing `earningscall-0.0.6/tests/data/msft-transcript-response.yaml` & `earningscall-0.0.7/tests/data/msft-transcript-response.yaml`

 * *Files identical despite different names*

### Comparing `earningscall-0.0.6/tests/data/symbols-v2.yaml` & `earningscall-0.0.7/tests/data/symbols-v2.yaml`

 * *Files identical despite different names*

### Comparing `earningscall-0.0.6/tests/data/symbols.yaml` & `earningscall-0.0.7/tests/data/symbols.yaml`

 * *Files identical despite different names*

### Comparing `earningscall-0.0.6/LICENSE` & `earningscall-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `earningscall-0.0.6/README.md` & `earningscall-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `earningscall-0.0.6/pyproject.toml` & `earningscall-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "earningscall"
-version = "0.0.6"
+version = "0.0.7"
 description = "The EarningsCall Python library."
 readme = "README.md"
 authors = [
     {name = "EarningsCall", email = "dev@earningscall.biz"},
 ]
 requires-python = ">= 3.8"
 dependencies = [
```

### Comparing `earningscall-0.0.6/PKG-INFO` & `earningscall-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: earningscall
-Version: 0.0.6
+Version: 0.0.7
 Summary: The EarningsCall Python library.
 Project-URL: Homepage, https://earningscall.biz
 Project-URL: Documentation, https://github.com/EarningsCall/earningscall-python
 Project-URL: Repository, https://github.com/EarningsCall/earningscall-python
 Project-URL: Issues, https://github.com/EarningsCall/earningscall-python/issues
 Project-URL: Source, https://github.com/EarningsCall/earningscall-python
 Project-URL: Changelog, https://github.com/EarningsCall/earningscall-python/blob/master/CHANGELOG.md
```

