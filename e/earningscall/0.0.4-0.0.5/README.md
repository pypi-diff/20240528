# Comparing `tmp/earningscall-0.0.4.tar.gz` & `tmp/earningscall-0.0.5.tar.gz`

## Comparing `earningscall-0.0.4.tar` & `earningscall-0.0.5.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 earningscall-0.0.4/.python-version
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 earningscall-0.0.4/CHANGELOG.md
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 earningscall-0.0.4/DEVELOPMENT.md
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 earningscall-0.0.4/TODO.md
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 earningscall-0.0.4/requirements-dev.lock
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 earningscall-0.0.4/requirements.lock
--rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 earningscall-0.0.4/.github/workflows/release.yml
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 earningscall-0.0.4/earningscall/__init__.py
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 earningscall-0.0.4/earningscall/api.py
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 earningscall-0.0.4/earningscall/company.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 earningscall-0.0.4/earningscall/errors.py
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 earningscall-0.0.4/earningscall/event.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 earningscall-0.0.4/earningscall/exports.py
--rw-r--r--   0        0        0     5946 2020-02-02 00:00:00.000000 earningscall-0.0.4/earningscall/sectors.py
--rw-r--r--   0        0        0     7372 2020-02-02 00:00:00.000000 earningscall-0.0.4/earningscall/symbols.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 earningscall-0.0.4/earningscall/transcript.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 earningscall-0.0.4/earningscall/utils.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 earningscall-0.0.4/scripts/get_all_company_transcripts.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 earningscall-0.0.4/scripts/get_single_transcript.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 earningscall-0.0.4/scripts/list_all_companies.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 earningscall-0.0.4/tests/test_earnings_event.py
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 earningscall-0.0.4/tests/test_get_transcript.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 earningscall-0.0.4/tests/test_helper.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 earningscall-0.0.4/tests/test_simple.py
--rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 earningscall-0.0.4/tests/test_symbols.py
--rw-r--r--   0        0        0    60484 2020-02-02 00:00:00.000000 earningscall-0.0.4/tests/data/msft-transcript-response.yaml
--rw-r--r--   0        0        0   264578 2020-02-02 00:00:00.000000 earningscall-0.0.4/tests/data/symbols-v2.yaml
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 earningscall-0.0.4/tests/data/symbols.txt
--rw-r--r--   0        0        0   216684 2020-02-02 00:00:00.000000 earningscall-0.0.4/tests/data/symbols.yaml
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 earningscall-0.0.4/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 earningscall-0.0.4/LICENSE
--rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 earningscall-0.0.4/README.md
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 earningscall-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2935 2020-02-02 00:00:00.000000 earningscall-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 earningscall-0.0.5/.python-version
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 earningscall-0.0.5/CHANGELOG.md
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 earningscall-0.0.5/DEVELOPMENT.md
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 earningscall-0.0.5/TODO.md
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 earningscall-0.0.5/requirements-dev.lock
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 earningscall-0.0.5/requirements.lock
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 earningscall-0.0.5/.github/workflows/release.yml
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 earningscall-0.0.5/earningscall/__init__.py
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 earningscall-0.0.5/earningscall/api.py
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 earningscall-0.0.5/earningscall/company.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 earningscall-0.0.5/earningscall/errors.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 earningscall-0.0.5/earningscall/event.py
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 earningscall-0.0.5/earningscall/exports.py
+-rw-r--r--   0        0        0     5946 2020-02-02 00:00:00.000000 earningscall-0.0.5/earningscall/sectors.py
+-rw-r--r--   0        0        0     7722 2020-02-02 00:00:00.000000 earningscall-0.0.5/earningscall/symbols.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 earningscall-0.0.5/earningscall/transcript.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 earningscall-0.0.5/earningscall/utils.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 earningscall-0.0.5/scripts/get_all_company_transcripts.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 earningscall-0.0.5/scripts/get_single_transcript.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 earningscall-0.0.5/scripts/list_all_companies.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 earningscall-0.0.5/tests/test_earnings_event.py
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 earningscall-0.0.5/tests/test_get_transcript.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 earningscall-0.0.5/tests/test_helper.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 earningscall-0.0.5/tests/test_simple.py
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 earningscall-0.0.5/tests/test_symbols.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 earningscall-0.0.5/tests/data/demo-symbols-v2.yaml
+-rw-r--r--   0        0        0    60484 2020-02-02 00:00:00.000000 earningscall-0.0.5/tests/data/msft-transcript-response.yaml
+-rw-r--r--   0        0        0   264578 2020-02-02 00:00:00.000000 earningscall-0.0.5/tests/data/symbols-v2.yaml
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 earningscall-0.0.5/tests/data/symbols.txt
+-rw-r--r--   0        0        0   216684 2020-02-02 00:00:00.000000 earningscall-0.0.5/tests/data/symbols.yaml
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 earningscall-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 earningscall-0.0.5/LICENSE
+-rw-r--r--   0        0        0     3407 2020-02-02 00:00:00.000000 earningscall-0.0.5/README.md
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 earningscall-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 earningscall-0.0.5/PKG-INFO
```

### Comparing `earningscall-0.0.4/DEVELOPMENT.md` & `earningscall-0.0.5/DEVELOPMENT.md`

 * *Files identical despite different names*

### Comparing `earningscall-0.0.4/requirements-dev.lock` & `earningscall-0.0.5/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `earningscall-0.0.4/requirements.lock` & `earningscall-0.0.5/requirements.lock`

 * *Files identical despite different names*

### Comparing `earningscall-0.0.4/.github/workflows/release.yml` & `earningscall-0.0.5/.github/workflows/release.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # https://packaging.python.org/en/latest/guides/publishing-package-distribution-releases-using-github-actions-ci-cd-workflows/
-name: Publish Python 🐍 distribution 📦 to PyPI and TestPyPI
+name: Build and Release
 
 on: push
 
 jobs:
   build:
     name: Build distribution 📦
     runs-on: ubuntu-latest
```

### Comparing `earningscall-0.0.4/earningscall/api.py` & `earningscall-0.0.5/earningscall/api.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,14 +15,18 @@
 def get_api_key():
     global api_key
     if api_key is None:
         return os.environ.get("ECALL_API_KEY", "demo")
     return api_key
 
 
+def is_demo_account():
+    return get_api_key() == "demo"
+
+
 def get_events(exchange: str,
                symbol: str):
 
     log.debug(f"get_events exchange: {exchange} symbol: {symbol}")
     params = {
         "apikey": get_api_key(),
         "exchange": exchange,
@@ -37,15 +41,15 @@
 def get_transcript(exchange: str,
                    symbol: str,
                    year: int,
                    quarter: int) -> Optional[str]:
 
     log.debug(f"get_transcript year: {year} quarter: {quarter}")
     params = {
-        "apikey": "demo",
+        "apikey": get_api_key(),
         "exchange": exchange,
         "symbol": symbol,
         "year": str(year),
         "quarter": str(quarter),
     }
     response = requests.get(f"{API_BASE}/transcript", params=params)
     if response.status_code != 200:
@@ -57,11 +61,14 @@
     response = requests.get(f"{API_BASE}/symbols.txt")
     if response.status_code != 200:
         return None
     return response.text
 
 
 def get_symbols_v2():
-    response = requests.get(f"{API_BASE}/symbols-v2.txt")
+    params = {
+        "apikey": get_api_key(),
+    }
+    response = requests.get(f"{API_BASE}/symbols-v2.txt", params=params)
     if response.status_code != 200:
         return None
     return response.text
```

### Comparing `earningscall-0.0.4/earningscall/company.py` & `earningscall-0.0.5/earningscall/company.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,17 @@
 
 class Company:
 
     company_info: CompanyInfo
     name: str
     _events: [EarningsEvent]
 
-    def __init__(self, company_info):
+    def __init__(self, company_info: CompanyInfo):
+        if not company_info:
+            raise ValueError("company_info must be present.")
         self.company_info = company_info
         self.name = company_info.name
         self._events = None
 
     def __str__(self):
         return str(self.name)
```

### Comparing `earningscall-0.0.4/earningscall/event.py` & `earningscall-0.0.5/earningscall/event.py`

 * *Files identical despite different names*

### Comparing `earningscall-0.0.4/earningscall/sectors.py` & `earningscall-0.0.5/earningscall/sectors.py`

 * *Files identical despite different names*

### Comparing `earningscall-0.0.4/earningscall/symbols.py` & `earningscall-0.0.5/earningscall/symbols.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 import logging
 import re
 from collections import defaultdict
 from typing import Optional
 
-from earningscall.api import get_symbols_v2
+from earningscall.api import get_symbols_v2, is_demo_account
+from earningscall.errors import InsufficientApiAccessError
 from earningscall.sectors import sector_to_index, industry_to_index, index_to_sector, index_to_industry
 
 # WARNING: Add new indexes to the *END* of this list
 EXCHANGES_IN_ORDER = ["NYSE", "NASDAQ", "AMEX", "TSX", "TSXV", "OTC"]
 
 log = logging.getLogger(__file__)
 
@@ -123,14 +124,17 @@
         for exchange in EXCHANGES_IN_ORDER:
             try:
                 _symbol = self.get(exchange, symbol.upper())
                 if _symbol:
                     return _symbol
             except KeyError:
                 pass
+        if is_demo_account():
+            raise InsufficientApiAccessError(f"For full access, please get an API Key.  See: "
+                                             f"https://earningscall.biz/api-pricing")
         return None
 
     def remove_exchange_symbol(self, exchange_symbol: str):
         _symbol = self.by_exchange_and_sym[exchange_symbol]
         del self.by_name[_symbol.name]
         del self.by_exchange_and_sym[exchange_symbol]
 
@@ -220,7 +224,12 @@
 
 
 def get_symbols() -> Symbols:
     global _symbols
     if not _symbols:
         _symbols = load_symbols()
     return _symbols
+
+
+def clear_symbols():
+    global _symbols
+    _symbols = None
```

### Comparing `earningscall-0.0.4/tests/test_earnings_event.py` & `earningscall-0.0.5/tests/test_earnings_event.py`

 * *Files identical despite different names*

### Comparing `earningscall-0.0.4/tests/test_simple.py` & `earningscall-0.0.5/tests/test_simple.py`

 * *Files identical despite different names*

### Comparing `earningscall-0.0.4/tests/test_symbols.py` & `earningscall-0.0.5/tests/test_symbols.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,26 @@
 from earningscall.utils import data_path
 
 
 @responses.activate
 def test_load_symbols_txt_v2():
     ##
     responses.patch(API_BASE)
-    print("symbols path")
-    print(data_path("symbols-v2.yaml"))
     responses._add_from_file(file_path=data_path("symbols-v2.yaml"))
     ##
     symbols = Symbols.load_txt_v2()
     ##
     assert len(symbols) == 5807
     _symbol = symbols.get_exchange_symbol("NASDAQ_AAPL")
     assert _symbol.name == "Apple Inc."
     assert _symbol.exchange == "NASDAQ"
     assert _symbol.sector == "Technology"
     assert _symbol.industry == "Consumer Electronics"
     assert len(responses.calls) == 1
-    assert responses.calls[0].request.url == "https://v2.api.earningscall.biz/symbols-v2.txt"
+    assert responses.calls[0].request.url == "https://v2.api.earningscall.biz/symbols-v2.txt?apikey=demo"
 
 
 def test_symbols_serialization_to_text_v2():
     ##
     _symbols = Symbols()
     _symbols.add(CompanyInfo(exchange="TSX", symbol="TLRY", name="Tilray, Inc", sector="Energy",
                              industry="Electronic Gaming & Multimedia"))
```

### Comparing `earningscall-0.0.4/tests/data/msft-transcript-response.yaml` & `earningscall-0.0.5/tests/data/msft-transcript-response.yaml`

 * *Files identical despite different names*

### Comparing `earningscall-0.0.4/tests/data/symbols-v2.yaml` & `earningscall-0.0.5/tests/data/symbols-v2.yaml`

 * *Files identical despite different names*

### Comparing `earningscall-0.0.4/tests/data/symbols.yaml` & `earningscall-0.0.5/tests/data/symbols.yaml`

 * *Files identical despite different names*

### Comparing `earningscall-0.0.4/LICENSE` & `earningscall-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `earningscall-0.0.4/README.md` & `earningscall-0.0.5/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 # EarningsCall Python Library
 
-The EarningsCall Python library provides convenient access to the EarningsCall API from
+[![pypi](https://img.shields.io/pypi/v/earningscall.svg)](https://pypi.python.org/pypi/earningscall)
+[![Build Status](https://github.com/EarningsCall/earningscall-python/actions/workflows/release.yml/badge.svg?branch=master)](https://github.com/EarningsCall/earningscall-python/actions?query=branch%3Amaster)
+[![Coverage Status](https://coveralls.io/repos/github/EarningsCall/earningscall-python/badge.svg?branch=master)](https://coveralls.io/github/EarningsCall/earningscall-python?branch=master)
+
+The EarningsCall Python library provides convenient access to the [EarningsCall API](https://earningscall.biz/api-guide) from
 applications written in the Python language. It includes a pre-defined set of
 classes for API resources that initialize themselves dynamically from API
 responses.
 
 # Installation
 
 You don't need this source code unless you want to modify the package. If you just want to use the package, just run:
@@ -13,15 +17,14 @@
 pip install --upgrade earningscall
 ```
 
 # Requirements
 
 * Python 3.8+ (PyPI supported)
 
-
 ## Get Transcript for a Single Quarter
 
 ```python
 from earningscall import get_company
 
 
 company = get_company("aapl")  # Lookup Apple, Inc by its ticker symbol, "AAPL"
@@ -79,7 +82,28 @@
 
 ```python
 from earningscall import get_all_companies
 
 for company in get_all_companies():
     print(f"{company.company_info} -- {company.company_info.sector} -- {company.company_info.industry}")
 ```
+
+By default, this library grants you access to only two companies, Apple Inc. and Microsoft, Inc.
+
+To gain access 5,000+ companies please [signup here](https://earningscall.biz/api-pricing) to get your API key.
+
+Once you have access to your API key, you can set the API Key like this:
+
+```python
+
+import earningscall
+
+
+earningscall.api_key = "YOUR SECRET API KEY GOES HERE"
+```
+
+Alternatively, you can pass in your API key as an environment variable:
+
+```sh
+export ECALL_API_KEY="YOUR SECRET API KEY GOES HERE"
+python your-python-script.py
+```
```

### Comparing `earningscall-0.0.4/pyproject.toml` & `earningscall-0.0.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 [project]
 name = "earningscall"
-version = "0.0.4"
+version = "0.0.5"
 description = "The EarningsCall Python library."
 readme = "README.md"
 authors = [
     {name = "EarningsCall", email = "dev@earningscall.biz"},
 ]
 requires-python = ">= 3.8"
 dependencies = [
     "dataclasses>=0.6",
     "dataclasses-json>=0.6.4",
     "more_itertools>=10.0.0",
     "requests>=2.30.0",
 ]
 
 [project.urls]
+Homepage = "https://earningscall.biz"
 Documentation = "https://github.com/EarningsCall/earningscall-python"
+Repository = "https://github.com/EarningsCall/earningscall-python"
 Issues = "https://github.com/EarningsCall/earningscall-python/issues"
 Source = "https://github.com/EarningsCall/earningscall-python"
+Changelog = "https://github.com/EarningsCall/earningscall-python/blob/master/CHANGELOG.md"
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.rye]
 managed = true
```

