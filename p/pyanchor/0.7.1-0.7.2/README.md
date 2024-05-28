# Comparing `tmp/pyanchor-0.7.1.tar.gz` & `tmp/pyanchor-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyanchor-0.7.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyanchor-0.7.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyanchor-0.7.1.tar` & `pyanchor-0.7.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0       37 2024-05-06 21:17:39.909050 pyanchor-0.7.1/.coveragerc
--rw-r--r--   0        0        0       19 2024-05-06 21:17:39.909050 pyanchor-0.7.1/.github/FUNDING.yml
--rw-r--r--   0        0        0      609 2024-05-06 21:17:39.909050 pyanchor-0.7.1/.github/workflows/release.yml
--rw-r--r--   0        0        0      727 2024-05-06 21:17:39.909050 pyanchor-0.7.1/.github/workflows/run_tests.yml
--rw-r--r--   0        0        0     1829 2024-05-06 21:17:39.909050 pyanchor-0.7.1/.gitignore
--rw-r--r--   0        0        0     5226 2024-05-06 21:17:39.909050 pyanchor-0.7.1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1078 2024-05-06 21:17:39.909050 pyanchor-0.7.1/LICENSE
--rw-r--r--   0        0        0     5062 2024-05-06 21:17:39.909050 pyanchor-0.7.1/README.md
--rw-r--r--   0        0        0    50295 2024-05-06 21:17:39.909050 pyanchor-0.7.1/assets/example-help.gif
--rw-r--r--   0        0        0    57660 2024-05-06 21:17:39.909050 pyanchor-0.7.1/assets/example-single-page-verbose.gif
--rw-r--r--   0        0        0    43821 2024-05-06 21:17:39.909050 pyanchor-0.7.1/assets/example-single-page.gif
--rw-r--r--   0        0        0   171021 2024-05-06 21:17:39.913050 pyanchor-0.7.1/assets/example-sitemap-verbose.gif
--rw-r--r--   0        0        0    59788 2024-05-06 21:17:39.913050 pyanchor-0.7.1/assets/example-sitemap.gif
--rw-r--r--   0        0        0       62 2024-05-06 21:17:39.913050 pyanchor-0.7.1/pyanchor/__init__.py
--rw-r--r--   0        0        0     2946 2024-05-06 21:17:39.913050 pyanchor-0.7.1/pyanchor/cli.py
--rw-r--r--   0        0        0     5802 2024-05-06 21:17:39.913050 pyanchor-0.7.1/pyanchor/link_checker.py
--rw-r--r--   0        0        0      936 2024-05-06 21:17:39.913050 pyanchor-0.7.1/pyproject.toml
--rw-r--r--   0        0        0      156 2024-05-06 21:17:39.913050 pyanchor-0.7.1/pytest.ini
--rw-r--r--   0        0        0      306 2024-05-06 21:17:39.913050 pyanchor-0.7.1/requirements.in
--rw-r--r--   0        0        0    33678 2024-05-06 21:17:39.913050 pyanchor-0.7.1/requirements.txt
--rw-r--r--   0        0        0        0 2024-05-06 21:17:39.913050 pyanchor-0.7.1/tests/__init__.py
--rw-r--r--   0        0        0      580 2024-05-06 21:17:39.913050 pyanchor-0.7.1/tests/conftest.py
--rw-r--r--   0        0        0     1139 2024-05-06 21:17:39.913050 pyanchor-0.7.1/tests/test_cli.py
--rw-r--r--   0        0        0     1427 2024-05-06 21:17:39.913050 pyanchor-0.7.1/tests/test_link_checker.py
--rw-r--r--   0        0        0       35 2024-05-06 21:17:39.913050 pyanchor-0.7.1/tests/test_webapp/.flaskenv
--rw-r--r--   0        0        0     1143 2024-05-06 21:17:39.913050 pyanchor-0.7.1/tests/test_webapp/app.py
--rw-r--r--   0        0        0      236 2024-05-06 21:17:39.913050 pyanchor-0.7.1/tests/test_webapp/templates/error.html
--rw-r--r--   0        0        0     1034 2024-05-06 21:17:39.913050 pyanchor-0.7.1/tests/test_webapp/templates/index.html
--rw-r--r--   0        0        0     1940 2024-05-06 21:17:39.913050 pyanchor-0.7.1/tests/test_webapp/templates/sitemap.xml
--rw-r--r--   0        0        0      371 2024-05-06 21:17:39.913050 pyanchor-0.7.1/tests/test_webapp/templates/success.html
--rw-r--r--   0        0        0     5950 1970-01-01 00:00:00.000000 pyanchor-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0       37 2024-05-28 16:57:37.583107 pyanchor-0.7.2/.coveragerc
+-rw-r--r--   0        0        0       19 2024-05-28 16:57:37.583107 pyanchor-0.7.2/.github/FUNDING.yml
+-rw-r--r--   0        0        0      609 2024-05-28 16:57:37.583107 pyanchor-0.7.2/.github/workflows/release.yml
+-rw-r--r--   0        0        0      727 2024-05-28 16:57:37.583107 pyanchor-0.7.2/.github/workflows/run_tests.yml
+-rw-r--r--   0        0        0     1829 2024-05-28 16:57:37.583107 pyanchor-0.7.2/.gitignore
+-rw-r--r--   0        0        0     5226 2024-05-28 16:57:37.583107 pyanchor-0.7.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1078 2024-05-28 16:57:37.583107 pyanchor-0.7.2/LICENSE
+-rw-r--r--   0        0        0     5062 2024-05-28 16:57:37.583107 pyanchor-0.7.2/README.md
+-rw-r--r--   0        0        0    50295 2024-05-28 16:57:37.583107 pyanchor-0.7.2/assets/example-help.gif
+-rw-r--r--   0        0        0    57660 2024-05-28 16:57:37.583107 pyanchor-0.7.2/assets/example-single-page-verbose.gif
+-rw-r--r--   0        0        0    43821 2024-05-28 16:57:37.583107 pyanchor-0.7.2/assets/example-single-page.gif
+-rw-r--r--   0        0        0   171021 2024-05-28 16:57:37.583107 pyanchor-0.7.2/assets/example-sitemap-verbose.gif
+-rw-r--r--   0        0        0    59788 2024-05-28 16:57:37.587107 pyanchor-0.7.2/assets/example-sitemap.gif
+-rw-r--r--   0        0        0       62 2024-05-28 16:57:37.587107 pyanchor-0.7.2/pyanchor/__init__.py
+-rw-r--r--   0        0        0     2946 2024-05-28 16:57:37.587107 pyanchor-0.7.2/pyanchor/cli.py
+-rw-r--r--   0        0        0     5802 2024-05-28 16:57:37.587107 pyanchor-0.7.2/pyanchor/link_checker.py
+-rw-r--r--   0        0        0      936 2024-05-28 16:57:37.587107 pyanchor-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0      156 2024-05-28 16:57:37.587107 pyanchor-0.7.2/pytest.ini
+-rw-r--r--   0        0        0      306 2024-05-28 16:57:37.587107 pyanchor-0.7.2/requirements.in
+-rw-r--r--   0        0        0    33678 2024-05-28 16:57:37.587107 pyanchor-0.7.2/requirements.txt
+-rw-r--r--   0        0        0        0 2024-05-28 16:57:37.587107 pyanchor-0.7.2/tests/__init__.py
+-rw-r--r--   0        0        0      580 2024-05-28 16:57:37.587107 pyanchor-0.7.2/tests/conftest.py
+-rw-r--r--   0        0        0     1139 2024-05-28 16:57:37.587107 pyanchor-0.7.2/tests/test_cli.py
+-rw-r--r--   0        0        0     1427 2024-05-28 16:57:37.587107 pyanchor-0.7.2/tests/test_link_checker.py
+-rw-r--r--   0        0        0       35 2024-05-28 16:57:37.587107 pyanchor-0.7.2/tests/test_webapp/.flaskenv
+-rw-r--r--   0        0        0     1143 2024-05-28 16:57:37.587107 pyanchor-0.7.2/tests/test_webapp/app.py
+-rw-r--r--   0        0        0      236 2024-05-28 16:57:37.587107 pyanchor-0.7.2/tests/test_webapp/templates/error.html
+-rw-r--r--   0        0        0     1034 2024-05-28 16:57:37.587107 pyanchor-0.7.2/tests/test_webapp/templates/index.html
+-rw-r--r--   0        0        0     1940 2024-05-28 16:57:37.587107 pyanchor-0.7.2/tests/test_webapp/templates/sitemap.xml
+-rw-r--r--   0        0        0      371 2024-05-28 16:57:37.587107 pyanchor-0.7.2/tests/test_webapp/templates/success.html
+-rw-r--r--   0        0        0     5950 1970-01-01 00:00:00.000000 pyanchor-0.7.2/PKG-INFO
```

### Comparing `pyanchor-0.7.1/.github/workflows/release.yml` & `pyanchor-0.7.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pyanchor-0.7.1/.github/workflows/run_tests.yml` & `pyanchor-0.7.2/.github/workflows/run_tests.yml`

 * *Files identical despite different names*

### Comparing `pyanchor-0.7.1/.gitignore` & `pyanchor-0.7.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pyanchor-0.7.1/CODE_OF_CONDUCT.md` & `pyanchor-0.7.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pyanchor-0.7.1/LICENSE` & `pyanchor-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyanchor-0.7.1/README.md` & `pyanchor-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `pyanchor-0.7.1/assets/example-help.gif` & `pyanchor-0.7.2/assets/example-help.gif`

 * *Files identical despite different names*

### Comparing `pyanchor-0.7.1/assets/example-single-page-verbose.gif` & `pyanchor-0.7.2/assets/example-single-page-verbose.gif`

 * *Files identical despite different names*

### Comparing `pyanchor-0.7.1/assets/example-single-page.gif` & `pyanchor-0.7.2/assets/example-single-page.gif`

 * *Files identical despite different names*

### Comparing `pyanchor-0.7.1/assets/example-sitemap-verbose.gif` & `pyanchor-0.7.2/assets/example-sitemap-verbose.gif`

 * *Files identical despite different names*

### Comparing `pyanchor-0.7.1/assets/example-sitemap.gif` & `pyanchor-0.7.2/assets/example-sitemap.gif`

 * *Files identical despite different names*

### Comparing `pyanchor-0.7.1/pyanchor/cli.py` & `pyanchor-0.7.2/pyanchor/cli.py`

 * *Files identical despite different names*

### Comparing `pyanchor-0.7.1/pyanchor/link_checker.py` & `pyanchor-0.7.2/pyanchor/link_checker.py`

 * *Files identical despite different names*

### Comparing `pyanchor-0.7.1/pyproject.toml` & `pyanchor-0.7.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyanchor-0.7.1/requirements.txt` & `pyanchor-0.7.2/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -423,17 +423,17 @@
     --hash=sha256:578d5d15ac4a25e5f961c938b85a05b09fdaae9deef3bb6de9a6e766622ca7a6 \
     --hash=sha256:e7f0f5b1617d2210a2cabc266dfe2f4c75a8d32fb89eafb7ad9d06f6d076d470
     # via -r requirements.in
 python-dotenv==0.20.0 \
     --hash=sha256:b7e3b04a59693c42c36f9ab1cc2acc46fa5df8c78e178fc33a8d4cd05c8d498f \
     --hash=sha256:d92a187be61fe482e4fd675b6d52200e7be63a12b724abbf931a40ce4fa92938
     # via -r requirements.in
-requests==2.31.0 \
-    --hash=sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f \
-    --hash=sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1
+requests==2.32.0 \
+    --hash=sha256:f2c3881dddb70d056c5bd7600a4fae312b2a300e39be6a118d30b90bd27262b5 \
+    --hash=sha256:fa5490319474c82ef1d2c9bc459d3652e3ae4ef4c4ebdd18a21145a47ca4b6b8
     # via
     #   -r requirements.in
     #   flit
 soupsieve==2.5 \
     --hash=sha256:5663d5a7b3bfaeee0bc4372e7fc48f9cff4940b3eec54a6451cc5299f1097690 \
     --hash=sha256:eaa337ff55a1579b6549dc679565eac1e3d000563bcb1c8ab0d0fefbc0c2cdc7
     # via beautifulsoup4
```

### Comparing `pyanchor-0.7.1/tests/conftest.py` & `pyanchor-0.7.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyanchor-0.7.1/tests/test_cli.py` & `pyanchor-0.7.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pyanchor-0.7.1/tests/test_link_checker.py` & `pyanchor-0.7.2/tests/test_link_checker.py`

 * *Files identical despite different names*

### Comparing `pyanchor-0.7.1/tests/test_webapp/app.py` & `pyanchor-0.7.2/tests/test_webapp/app.py`

 * *Files identical despite different names*

### Comparing `pyanchor-0.7.1/tests/test_webapp/templates/index.html` & `pyanchor-0.7.2/tests/test_webapp/templates/index.html`

 * *Files identical despite different names*

### Comparing `pyanchor-0.7.1/tests/test_webapp/templates/sitemap.xml` & `pyanchor-0.7.2/tests/test_webapp/templates/sitemap.xml`

 * *Files identical despite different names*

### Comparing `pyanchor-0.7.1/PKG-INFO` & `pyanchor-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyanchor
-Version: 0.7.1
+Version: 0.7.2
 Summary: Check you site for broken links!
 Home-page: https://github.com/EndlessTrax/pyanchor/
 Author: Ricky White
 Author-email: ricky@whitelionmedia.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyanchor Version: 0.7.1 Summary: Check you site for
+Metadata-Version: 2.1 Name: pyanchor Version: 0.7.2 Summary: Check you site for
 broken links! Home-page: https://github.com/EndlessTrax/pyanchor/ Author: Ricky
 White Author-email: ricky@whitelionmedia.com Requires-Python: >=3.8
 Description-Content-Type: text/markdown Classifier: License :: OSI Approved ::
 MIT License Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Requires-Dist: beautifulsoup4==4.11.1
```

