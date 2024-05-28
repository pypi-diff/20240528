# Comparing `tmp/pdnssoc-cli-0.0.3.tar.gz` & `tmp/pdnssoc_cli-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdnssoc-cli-0.0.3.tar", last modified: Wed Mar  6 15:36:08 2024, max compression
+gzip compressed data, was "pdnssoc_cli-0.0.4.tar", last modified: Tue May 28 14:07:25 2024, max compression
```

## Comparing `pdnssoc-cli-0.0.3.tar` & `pdnssoc_cli-0.0.4.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 15:36:08.736541 pdnssoc-cli-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 15:36:08.728541 pdnssoc-cli-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 15:36:08.732541 pdnssoc-cli-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-03-06 15:35:46.000000 pdnssoc-cli-0.0.3/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-03-06 15:35:46.000000 pdnssoc-cli-0.0.3/.github/workflows/release_testpypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-03-06 15:35:46.000000 pdnssoc-cli-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-06 15:35:46.000000 pdnssoc-cli-0.0.3/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-03-06 15:35:46.000000 pdnssoc-cli-0.0.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-03-06 15:36:08.736541 pdnssoc-cli-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-06 15:35:46.000000 pdnssoc-cli-0.0.3/Pipfile
--rw-r--r--   0 runner    (1001) docker     (127)    50543 2024-03-06 15:35:46.000000 pdnssoc-cli-0.0.3/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-06 15:35:46.000000 pdnssoc-cli-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-03-06 15:35:46.000000 pdnssoc-cli-0.0.3/config.yml.sample
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-06 15:35:46.000000 pdnssoc-cli-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-03-06 15:36:08.740541 pdnssoc-cli-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-03-06 15:35:46.000000 pdnssoc-cli-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 15:36:08.732541 pdnssoc-cli-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 15:36:08.736541 pdnssoc-cli-0.0.3/src/pdnssoc_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-03-06 15:36:08.000000 pdnssoc-cli-0.0.3/src/pdnssoc_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-03-06 15:36:08.000000 pdnssoc-cli-0.0.3/src/pdnssoc_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 15:36:08.000000 pdnssoc-cli-0.0.3/src/pdnssoc_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-06 15:36:08.000000 pdnssoc-cli-0.0.3/src/pdnssoc_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 15:36:08.000000 pdnssoc-cli-0.0.3/src/pdnssoc_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-06 15:36:08.000000 pdnssoc-cli-0.0.3/src/pdnssoc_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-06 15:36:08.000000 pdnssoc-cli-0.0.3/src/pdnssoc_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 15:36:08.736541 pdnssoc-cli-0.0.3/src/pdnssoccli/
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-03-06 15:35:46.000000 pdnssoc-cli-0.0.3/src/pdnssoccli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-03-06 15:35:46.000000 pdnssoc-cli-0.0.3/src/pdnssoccli/pdnssoccli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 15:36:08.736541 pdnssoc-cli-0.0.3/src/pdnssoccli/subcommands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 15:35:46.000000 pdnssoc-cli-0.0.3/src/pdnssoccli/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-03-06 15:35:46.000000 pdnssoc-cli-0.0.3/src/pdnssoccli/subcommands/alert.py
--rw-r--r--   0 runner    (1001) docker     (127)    11445 2024-03-06 15:35:46.000000 pdnssoc-cli-0.0.3/src/pdnssoccli/subcommands/correlate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-03-06 15:35:46.000000 pdnssoc-cli-0.0.3/src/pdnssoccli/subcommands/daemonize.py
--rw-r--r--   0 runner    (1001) docker     (127)     6099 2024-03-06 15:35:46.000000 pdnssoc-cli-0.0.3/src/pdnssoccli/subcommands/fetch_iocs.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-06 15:35:46.000000 pdnssoc-cli-0.0.3/src/pdnssoccli/subcommands/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 15:36:08.736541 pdnssoc-cli-0.0.3/src/pdnssoccli/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 15:35:46.000000 pdnssoc-cli-0.0.3/src/pdnssoccli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-03-06 15:35:46.000000 pdnssoc-cli-0.0.3/src/pdnssoccli/utils/alert.py
--rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-03-06 15:35:46.000000 pdnssoc-cli-0.0.3/src/pdnssoccli/utils/correlation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-03-06 15:35:46.000000 pdnssoc-cli-0.0.3/src/pdnssoccli/utils/enrichment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-03-06 15:35:46.000000 pdnssoc-cli-0.0.3/src/pdnssoccli/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-03-06 15:35:46.000000 pdnssoc-cli-0.0.3/src/pdnssoccli/utils/time.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 15:36:08.736541 pdnssoc-cli-0.0.3/src/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-03-06 15:35:46.000000 pdnssoc-cli-0.0.3/src/resources/alert_email_template.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 15:36:08.736541 pdnssoc-cli-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-03-06 15:35:46.000000 pdnssoc-cli-0.0.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-03-06 15:35:46.000000 pdnssoc-cli-0.0.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:07:25.764868 pdnssoc_cli-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:07:25.756868 pdnssoc_cli-0.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:07:25.760868 pdnssoc_cli-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-28 14:07:01.000000 pdnssoc_cli-0.0.4/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-28 14:07:01.000000 pdnssoc_cli-0.0.4/.github/workflows/release_testpypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-28 14:07:01.000000 pdnssoc_cli-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-28 14:07:01.000000 pdnssoc_cli-0.0.4/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-28 14:07:01.000000 pdnssoc_cli-0.0.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-28 14:07:25.764868 pdnssoc_cli-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-28 14:07:01.000000 pdnssoc_cli-0.0.4/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (127)    50543 2024-05-28 14:07:01.000000 pdnssoc_cli-0.0.4/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-28 14:07:01.000000 pdnssoc_cli-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-05-28 14:07:01.000000 pdnssoc_cli-0.0.4/config.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-28 14:07:01.000000 pdnssoc_cli-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-28 14:07:25.768868 pdnssoc_cli-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-28 14:07:01.000000 pdnssoc_cli-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:07:25.756868 pdnssoc_cli-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:07:25.764868 pdnssoc_cli-0.0.4/src/pdnssoc_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-28 14:07:25.000000 pdnssoc_cli-0.0.4/src/pdnssoc_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-28 14:07:25.000000 pdnssoc_cli-0.0.4/src/pdnssoc_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 14:07:25.000000 pdnssoc_cli-0.0.4/src/pdnssoc_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-28 14:07:25.000000 pdnssoc_cli-0.0.4/src/pdnssoc_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 14:07:25.000000 pdnssoc_cli-0.0.4/src/pdnssoc_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-28 14:07:25.000000 pdnssoc_cli-0.0.4/src/pdnssoc_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-28 14:07:25.000000 pdnssoc_cli-0.0.4/src/pdnssoc_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:07:25.764868 pdnssoc_cli-0.0.4/src/pdnssoccli/
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-28 14:07:01.000000 pdnssoc_cli-0.0.4/src/pdnssoccli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-28 14:07:01.000000 pdnssoc_cli-0.0.4/src/pdnssoccli/pdnssoccli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:07:25.764868 pdnssoc_cli-0.0.4/src/pdnssoccli/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 14:07:01.000000 pdnssoc_cli-0.0.4/src/pdnssoccli/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-05-28 14:07:01.000000 pdnssoc_cli-0.0.4/src/pdnssoccli/subcommands/alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11464 2024-05-28 14:07:01.000000 pdnssoc_cli-0.0.4/src/pdnssoccli/subcommands/correlate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-05-28 14:07:01.000000 pdnssoc_cli-0.0.4/src/pdnssoccli/subcommands/daemonize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6137 2024-05-28 14:07:01.000000 pdnssoc_cli-0.0.4/src/pdnssoccli/subcommands/fetch_iocs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-28 14:07:01.000000 pdnssoc_cli-0.0.4/src/pdnssoccli/subcommands/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:07:25.764868 pdnssoc_cli-0.0.4/src/pdnssoccli/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 14:07:01.000000 pdnssoc_cli-0.0.4/src/pdnssoccli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-05-28 14:07:01.000000 pdnssoc_cli-0.0.4/src/pdnssoccli/utils/alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-05-28 14:07:01.000000 pdnssoc_cli-0.0.4/src/pdnssoccli/utils/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-05-28 14:07:01.000000 pdnssoc_cli-0.0.4/src/pdnssoccli/utils/enrichment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-28 14:07:01.000000 pdnssoc_cli-0.0.4/src/pdnssoccli/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-28 14:07:01.000000 pdnssoc_cli-0.0.4/src/pdnssoccli/utils/time.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:07:25.764868 pdnssoc_cli-0.0.4/src/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-05-28 14:07:01.000000 pdnssoc_cli-0.0.4/src/resources/alert_email_template.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:07:25.764868 pdnssoc_cli-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-28 14:07:01.000000 pdnssoc_cli-0.0.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-05-28 14:07:01.000000 pdnssoc_cli-0.0.4/tox.ini
```

### Comparing `pdnssoc-cli-0.0.3/.github/workflows/release_pypi.yml` & `pdnssoc_cli-0.0.4/.github/workflows/release_pypi.yml`

 * *Files identical despite different names*

### Comparing `pdnssoc-cli-0.0.3/.github/workflows/release_testpypi.yml` & `pdnssoc_cli-0.0.4/.github/workflows/release_testpypi.yml`

 * *Files identical despite different names*

### Comparing `pdnssoc-cli-0.0.3/.gitignore` & `pdnssoc_cli-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pdnssoc-cli-0.0.3/LICENSE.txt` & `pdnssoc_cli-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pdnssoc-cli-0.0.3/PKG-INFO` & `pdnssoc_cli-0.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pdnssoc-cli
-Version: 0.0.3
+Version: 0.0.4
 Summary: Correlate dnstap files with MISP
 Home-page: https://github.com/CERN-CERT/pdnssoc-cli
-Author: Christos Arvanitis
-Author-email: arvchristos@protonmail.com
+Author: CERN Computer Security Team
+Author-email: computer.security@cern.ch
 License: MIT
 Project-URL: Documentation, https://github.com/CERN-CERT/pdnssoc-cli
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown; charset=UTF-8
 License-File: LICENSE.txt
```

### Comparing `pdnssoc-cli-0.0.3/Pipfile.lock` & `pdnssoc_cli-0.0.4/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `pdnssoc-cli-0.0.3/README.md` & `pdnssoc_cli-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pdnssoc-cli-0.0.3/config.yml.sample` & `pdnssoc_cli-0.0.4/config.yml.sample`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # and attributes. Each of the server will be used serially,
 # for fetching initial attributes and querying for specific
 # events.
 misp_servers:
   - domain: "https://example-misp-instance.com"
     api_key: "API_KEY"
     verify_ssl: False
+    debug: False
 
     # PyMISP.search() arguments. For complete list of options
     # consult https://pymisp.readthedocs.io/en/latest/modules.html#pymisp.PyMISP.search
     args:
       enforce_warninglist: True # Suggested to reduce false positives
 
     # Restrict results by timestamp:
```

### Comparing `pdnssoc-cli-0.0.3/setup.cfg` & `pdnssoc_cli-0.0.4/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = pdnssoc-cli
 description = Correlate dnstap files with MISP
-author = Christos Arvanitis
-author_email = arvchristos@protonmail.com
+author = CERN Computer Security Team
+author_email = computer.security@cern.ch
 license = MIT
 license_files = LICENSE.txt
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8
 url = https://github.com/CERN-CERT/pdnssoc-cli
 project_urls = 
 	Documentation = https://github.com/CERN-CERT/pdnssoc-cli
```

### Comparing `pdnssoc-cli-0.0.3/src/pdnssoc_cli.egg-info/PKG-INFO` & `pdnssoc_cli-0.0.4/src/pdnssoc_cli.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pdnssoc-cli
-Version: 0.0.3
+Version: 0.0.4
 Summary: Correlate dnstap files with MISP
 Home-page: https://github.com/CERN-CERT/pdnssoc-cli
-Author: Christos Arvanitis
-Author-email: arvchristos@protonmail.com
+Author: CERN Computer Security Team
+Author-email: computer.security@cern.ch
 License: MIT
 Project-URL: Documentation, https://github.com/CERN-CERT/pdnssoc-cli
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown; charset=UTF-8
 License-File: LICENSE.txt
```

### Comparing `pdnssoc-cli-0.0.3/src/pdnssoc_cli.egg-info/SOURCES.txt` & `pdnssoc_cli-0.0.4/src/pdnssoc_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pdnssoc-cli-0.0.3/src/pdnssoccli/__init__.py` & `pdnssoc_cli-0.0.4/src/pdnssoccli/__init__.py`

 * *Files identical despite different names*

### Comparing `pdnssoc-cli-0.0.3/src/pdnssoccli/pdnssoccli.py` & `pdnssoc_cli-0.0.4/src/pdnssoccli/pdnssoccli.py`

 * *Files identical despite different names*

### Comparing `pdnssoc-cli-0.0.3/src/pdnssoccli/subcommands/alert.py` & `pdnssoc_cli-0.0.4/src/pdnssoccli/subcommands/alert.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 )
 @click.pass_context
 def alert(ctx,
     **kwargs):
 
     alerting_config = ctx.obj['CONFIG']['alerting']
     correlation_config = ctx.obj['CONFIG']['correlation']
-    alerting_start_dt = datetime.now()
+    alerting_start_dt = datetime.utcnow()
 
     # iterate through alert configs enabled
     for alert_type, alert_conf in ctx.obj['CONFIG']['alerting'].items():
         logger.info("Enabling {} alerting".format(alert_type))
         # Set up mailing here
 
 
@@ -67,15 +67,15 @@
 
         if not start_date:
             start_date = alerting_start_dt
     else:
         start_date = kwargs.get('start_date')
 
     if not kwargs.get('end_date'):
-        end_date = datetime.now()
+        end_date = datetime.utcnow()
     else:
         end_date = kwargs.get('end_date')
 
 
     pending_alerts = {}
     for file in files:
         file_path = Path(file)
@@ -116,8 +116,8 @@
     pdnssoc_alerting_utils.email_alerts(pending_alerts, alerting_config['email'], summary=True)
 
     #Send mails to each of the responsibles for a sensor
     pdnssoc_alerting_utils.email_alerts(pending_alerts, alerting_config['email'], summary=False)
 
     # Update the last alert file
     with pdnssoc_file_utils.write_generic(alerting_config['last_alerting_pointer_file']) as fp:
-        fp.write("{}\n".format(end_date.strftime("%Y-%m-%dT%H:%M:%S")))
+        fp.write("{}\n".format(end_date.strftime("%Y-%m-%dT%H:%M:%S")))
```

### Comparing `pdnssoc-cli-0.0.3/src/pdnssoccli/subcommands/correlate.py` & `pdnssoc_cli-0.0.4/src/pdnssoccli/subcommands/correlate.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
     ),
 )
 @click.pass_context
 def correlate(ctx,
     **kwargs):
 
     correlation_config = ctx.obj['CONFIG']['correlation']
-    correlation_start_dt = datetime.now()
+    correlation_start_dt = datetime.utcnow()
 
     retro_last_date = None
     if not kwargs.get('retro_lookup'):
         # Determine start date
         if not kwargs.get('start_date'):
             if 'last_correlation_pointer_file' in correlation_config:
                 last_correlation_path = Path(correlation_config['last_correlation_pointer_file'])
@@ -112,15 +112,15 @@
                     start_date = correlation_start_dt
             else:
                 start_date = correlation_start_dt
         else:
             start_date = kwargs.get('start_date')
 
         if not kwargs.get('end_date'):
-            end_date = datetime.now()
+            end_date = datetime.utcnow()
         else:
             end_date = kwargs.get('end_date')
 
         # Parse json file and only keep alerts in range
         logging.info(
             "Parsing alerts from: {} to {}".format(
                 start_date,
@@ -142,15 +142,15 @@
                     )
                     retro_last_date = timestamp
                     break
 
     # Set up MISP connections
     misp_connections = []
     for misp_conf in ctx.obj['CONFIG']["misp_servers"]:
-        misp = PyMISP(misp_conf['domain'], misp_conf['api_key'], ssl=misp_conf['verify_ssl'], debug=False)
+        misp = PyMISP(misp_conf['domain'], misp_conf['api_key'], ssl=misp_conf['verify_ssl'], debug=misp_conf['debug'])
         if misp:
             misp_connections.append((misp, misp_conf['args']))
 
 
     # Set up domain and ip blacklists
     domain_attributes = []
     domain_attributes_metadata = {}
```

### Comparing `pdnssoc-cli-0.0.3/src/pdnssoccli/subcommands/daemonize.py` & `pdnssoc_cli-0.0.4/src/pdnssoccli/subcommands/daemonize.py`

 * *Files identical despite different names*

### Comparing `pdnssoc-cli-0.0.3/src/pdnssoccli/subcommands/fetch_iocs.py` & `pdnssoc_cli-0.0.4/src/pdnssoccli/subcommands/fetch_iocs.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     **kwargs):
 
     correlation_config = ctx.obj['CONFIG']['correlation']
 
     # Set up MISP connections
     misp_connections = []
     for misp_conf in ctx.obj['CONFIG']["misp_servers"]:
-        misp = PyMISP(misp_conf['domain'], misp_conf['api_key'], True, debug=False)
+        misp = PyMISP(misp_conf['domain'], misp_conf['api_key'], misp_conf['verify_ssl'], debug=misp_conf['debug'])
         if misp:
             misp_connections.append((misp, misp_conf['args'], misp_conf['periods']['tags']))
 
     domain_attributes_old = []
     domain_attributes_new = []
     ips_attributes_new = []
     ips_attributes_old = []
@@ -62,15 +62,15 @@
         # Keep configured tag names to exclude them from catch all
         configured_tags = []
 
         for tag in tag_periods:
             configured_tags.extend(tag['names'])
 
             if tag['delta']:
-                misp_timestamp = datetime.now() - timedelta(**tag['delta'])
+                misp_timestamp = datetime.utcnow() - timedelta(**tag['delta'])
             else:
                 misp_timestamp=None
 
 
             tag_attributes = misp.search(
                 controller='attributes',
                 type_attribute=[
@@ -91,15 +91,15 @@
             )
 
             attributes.extend(tag_attributes)
 
         # Fetch catch all
 
         if misp_conf['periods']['generic']['delta']:
-            misp_timestamp = datetime.now() - timedelta(**misp_conf['periods']['generic']['delta'])
+            misp_timestamp = datetime.utcnow() - timedelta(**misp_conf['periods']['generic']['delta'])
         else:
             misp_timestamp=None
 
         catch_all_attributes = misp.search(
             controller='attributes',
             type_attribute=[
                 'domain',
```

### Comparing `pdnssoc-cli-0.0.3/src/pdnssoccli/utils/alert.py` & `pdnssoc_cli-0.0.4/src/pdnssoccli/utils/alert.py`

 * *Files identical despite different names*

### Comparing `pdnssoc-cli-0.0.3/src/pdnssoccli/utils/correlation.py` & `pdnssoc_cli-0.0.4/src/pdnssoccli/utils/correlation.py`

 * *Files identical despite different names*

### Comparing `pdnssoc-cli-0.0.3/src/pdnssoccli/utils/enrichment.py` & `pdnssoc_cli-0.0.4/src/pdnssoccli/utils/enrichment.py`

 * *Files identical despite different names*

### Comparing `pdnssoc-cli-0.0.3/src/pdnssoccli/utils/file.py` & `pdnssoc_cli-0.0.4/src/pdnssoccli/utils/file.py`

 * *Files identical despite different names*

### Comparing `pdnssoc-cli-0.0.3/src/pdnssoccli/utils/time.py` & `pdnssoc_cli-0.0.4/src/pdnssoccli/utils/time.py`

 * *Files identical despite different names*

### Comparing `pdnssoc-cli-0.0.3/src/resources/alert_email_template.html` & `pdnssoc_cli-0.0.4/src/resources/alert_email_template.html`

 * *Files identical despite different names*

### Comparing `pdnssoc-cli-0.0.3/tox.ini` & `pdnssoc_cli-0.0.4/tox.ini`

 * *Files identical despite different names*

