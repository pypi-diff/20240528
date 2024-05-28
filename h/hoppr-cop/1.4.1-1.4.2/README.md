# Comparing `tmp/hoppr_cop-1.4.1.tar.gz` & `tmp/hoppr_cop-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hoppr_cop-1.4.1.tar", max compression
+gzip compressed data, was "hoppr_cop-1.4.2.tar", max compression
```

## Comparing `hoppr_cop-1.4.1.tar` & `hoppr_cop-1.4.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     1084 2024-05-01 15:06:24.000000 hoppr_cop-1.4.1/LICENSE.md
--rw-r--r--   0        0        0       94 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/__init__.py
--rw-r--r--   0        0        0        0 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/combined/__init__.py
--rw-r--r--   0        0        0     7988 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/combined/cli.py
--rw-r--r--   0        0        0     9899 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/combined/combined_scanner.py
--rw-r--r--   0        0        0        0 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/combined/py.typed
--rw-r--r--   0        0        0    18103 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/enhancements/analysis_assessment.py
--rw-r--r--   0        0        0        0 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/enhancements/epss/__init__.py
--rw-r--r--   0        0        0      586 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/enhancements/epss/models.py
--rw-r--r--   0        0        0     4328 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/enhancements/epss_enhancer.py
--rw-r--r--   0        0        0        0 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/gemnasium/__init__.py
--rw-r--r--   0        0        0    13609 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/gemnasium/gemnasium_scanner.py
--rw-r--r--   0        0        0     1974 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/gemnasium/models.py
--rw-r--r--   0        0        0        0 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/gemnasium/py.typed
--rwxr-xr-x   0        0        0      113 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/gemnasium/semver
--rw-r--r--   0        0        0        0 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/grype/__init__.py
--rw-r--r--   0        0        0    14796 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/grype/grype_scanner.py
--rw-r--r--   0        0        0     8574 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/grype/models.py
--rw-r--r--   0        0        0        0 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/grype/py.typed
--rw-r--r--   0        0        0        0 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/hoppr_plugin/__init__.py
--rw-r--r--   0        0        0     4989 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/hoppr_plugin/hopprcop_plugin.py
--rw-r--r--   0        0        0        0 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/hoppr_plugin/py.typed
--rw-r--r--   0        0        0      478 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/ossindex/README.md
--rw-r--r--   0        0        0        0 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/ossindex/__init__.py
--rw-r--r--   0        0        0      832 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/ossindex/api/__init__.py
--rw-r--r--   0        0        0     1048 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/ossindex/api/exception.py
--rw-r--r--   0        0        0     9278 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/ossindex/api/model.py
--rw-r--r--   0        0        0    10293 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/ossindex/api/ossindex.py
--rw-r--r--   0        0        0      153 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/ossindex/api/py.typed
--rw-r--r--   0        0        0     2997 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/ossindex/api/serializer.py
--rw-r--r--   0        0        0    10447 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/ossindex/oss_index_scanner.py
--rw-r--r--   0        0        0        0 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/ossindex/py.typed
--rw-r--r--   0        0        0        0 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/py.typed
--rw-r--r--   0        0        0    19750 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/reporting/__init__.py
--rw-r--r--   0        0        0        0 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/reporting/gitlab/__init__.py
--rw-r--r--   0        0        0    23684 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/reporting/gitlab/models.py
--rw-r--r--   0        0        0     1729 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/reporting/models.py
--rw-r--r--   0        0        0        0 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/reporting/py.typed
--rw-r--r--   0        0        0    13776 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/reporting/templates/assets/vulnerabilities.css
--rw-r--r--   0        0        0    62168 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/reporting/templates/package-lock.json
--rw-r--r--   0        0        0       56 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/reporting/templates/package.json
--rw-r--r--   0        0        0      135 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/reporting/templates/tailwind.config.js
--rw-r--r--   0        0        0     3423 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/reporting/templates/vulnerabilities.html
--rw-r--r--   0        0        0       58 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/reporting/templates/vulnerability.css
--rw-r--r--   0        0        0    10840 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/reporting/templates/vulnerability_details.html
--rw-r--r--   0        0        0        0 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/trivy/__init__.py
--rw-r--r--   0        0        0        0 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/trivy/py.typed
--rw-r--r--   0        0        0    10960 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/trivy/trivy_scanner.py
--rw-r--r--   0        0        0    10374 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/utils.py
--rw-r--r--   0        0        0     4179 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/vulnerability_combiner.py
--rw-r--r--   0        0        0     2652 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/vulnerability_enhancer.py
--rw-r--r--   0        0        0     6973 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/vulnerability_scanner.py
--rw-r--r--   0        0        0     6425 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     1267 1970-01-01 00:00:00.000000 hoppr_cop-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1084 2024-05-28 21:11:18.000000 hoppr_cop-1.4.2/LICENSE.md
+-rw-r--r--   0        0        0       94 2024-05-28 21:11:18.000000 hoppr_cop-1.4.2/hopprcop/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 21:11:18.000000 hoppr_cop-1.4.2/hopprcop/combined/__init__.py
+-rw-r--r--   0        0        0     7988 2024-05-28 21:11:18.000000 hoppr_cop-1.4.2/hopprcop/combined/cli.py
+-rw-r--r--   0        0        0     9899 2024-05-28 21:11:18.000000 hoppr_cop-1.4.2/hopprcop/combined/combined_scanner.py
+-rw-r--r--   0        0        0        0 2024-05-28 21:11:18.000000 hoppr_cop-1.4.2/hopprcop/combined/py.typed
+-rw-r--r--   0        0        0    18103 2024-05-28 21:11:18.000000 hoppr_cop-1.4.2/hopprcop/enhancements/analysis_assessment.py
+-rw-r--r--   0        0        0        0 2024-05-28 21:11:18.000000 hoppr_cop-1.4.2/hopprcop/enhancements/epss/__init__.py
+-rw-r--r--   0        0        0      586 2024-05-28 21:11:18.000000 hoppr_cop-1.4.2/hopprcop/enhancements/epss/models.py
+-rw-r--r--   0        0        0     4328 2024-05-28 21:11:18.000000 hoppr_cop-1.4.2/hopprcop/enhancements/epss_enhancer.py
+-rw-r--r--   0        0        0        0 2024-05-28 21:11:18.000000 hoppr_cop-1.4.2/hopprcop/gemnasium/__init__.py
+-rw-r--r--   0        0        0    13609 2024-05-28 21:11:18.000000 hoppr_cop-1.4.2/hopprcop/gemnasium/gemnasium_scanner.py
+-rw-r--r--   0        0        0     1974 2024-05-28 21:11:18.000000 hoppr_cop-1.4.2/hopprcop/gemnasium/models.py
+-rw-r--r--   0        0        0        0 2024-05-28 21:11:18.000000 hoppr_cop-1.4.2/hopprcop/gemnasium/py.typed
+-rwxr-xr-x   0        0        0      113 2024-05-28 21:11:18.000000 hoppr_cop-1.4.2/hopprcop/gemnasium/semver
+-rw-r--r--   0        0        0        0 2024-05-28 21:11:18.000000 hoppr_cop-1.4.2/hopprcop/grype/__init__.py
+-rw-r--r--   0        0        0    14796 2024-05-28 21:11:18.000000 hoppr_cop-1.4.2/hopprcop/grype/grype_scanner.py
+-rw-r--r--   0        0        0     8588 2024-05-28 21:11:18.000000 hoppr_cop-1.4.2/hopprcop/grype/models.py
+-rw-r--r--   0        0        0        0 2024-05-28 21:11:18.000000 hoppr_cop-1.4.2/hopprcop/grype/py.typed
+-rw-r--r--   0        0        0        0 2024-05-28 21:11:18.000000 hoppr_cop-1.4.2/hopprcop/hoppr_plugin/__init__.py
+-rw-r--r--   0        0        0     4989 2024-05-28 21:11:18.000000 hoppr_cop-1.4.2/hopprcop/hoppr_plugin/hopprcop_plugin.py
+-rw-r--r--   0        0        0        0 2024-05-28 21:11:18.000000 hoppr_cop-1.4.2/hopprcop/hoppr_plugin/py.typed
+-rw-r--r--   0        0        0      478 2024-05-28 21:11:18.000000 hoppr_cop-1.4.2/hopprcop/ossindex/README.md
+-rw-r--r--   0        0        0        0 2024-05-28 21:11:18.000000 hoppr_cop-1.4.2/hopprcop/ossindex/__init__.py
+-rw-r--r--   0        0        0      832 2024-05-28 21:11:18.000000 hoppr_cop-1.4.2/hopprcop/ossindex/api/__init__.py
+-rw-r--r--   0        0        0     1048 2024-05-28 21:11:18.000000 hoppr_cop-1.4.2/hopprcop/ossindex/api/exception.py
+-rw-r--r--   0        0        0     9278 2024-05-28 21:11:18.000000 hoppr_cop-1.4.2/hopprcop/ossindex/api/model.py
+-rw-r--r--   0        0        0    10293 2024-05-28 21:11:18.000000 hoppr_cop-1.4.2/hopprcop/ossindex/api/ossindex.py
+-rw-r--r--   0        0        0      153 2024-05-28 21:11:18.000000 hoppr_cop-1.4.2/hopprcop/ossindex/api/py.typed
+-rw-r--r--   0        0        0     2997 2024-05-28 21:11:18.000000 hoppr_cop-1.4.2/hopprcop/ossindex/api/serializer.py
+-rw-r--r--   0        0        0    10447 2024-05-28 21:11:18.000000 hoppr_cop-1.4.2/hopprcop/ossindex/oss_index_scanner.py
+-rw-r--r--   0        0        0        0 2024-05-28 21:11:18.000000 hoppr_cop-1.4.2/hopprcop/ossindex/py.typed
+-rw-r--r--   0        0        0        0 2024-05-28 21:11:18.000000 hoppr_cop-1.4.2/hopprcop/py.typed
+-rw-r--r--   0        0        0    19750 2024-05-28 21:11:18.000000 hoppr_cop-1.4.2/hopprcop/reporting/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 21:11:18.000000 hoppr_cop-1.4.2/hopprcop/reporting/gitlab/__init__.py
+-rw-r--r--   0        0        0    23684 2024-05-28 21:11:18.000000 hoppr_cop-1.4.2/hopprcop/reporting/gitlab/models.py
+-rw-r--r--   0        0        0     1729 2024-05-28 21:11:18.000000 hoppr_cop-1.4.2/hopprcop/reporting/models.py
+-rw-r--r--   0        0        0        0 2024-05-28 21:11:18.000000 hoppr_cop-1.4.2/hopprcop/reporting/py.typed
+-rw-r--r--   0        0        0    13776 2024-05-28 21:11:18.000000 hoppr_cop-1.4.2/hopprcop/reporting/templates/assets/vulnerabilities.css
+-rw-r--r--   0        0        0    62168 2024-05-28 21:11:18.000000 hoppr_cop-1.4.2/hopprcop/reporting/templates/package-lock.json
+-rw-r--r--   0        0        0       56 2024-05-28 21:11:18.000000 hoppr_cop-1.4.2/hopprcop/reporting/templates/package.json
+-rw-r--r--   0        0        0      135 2024-05-28 21:11:18.000000 hoppr_cop-1.4.2/hopprcop/reporting/templates/tailwind.config.js
+-rw-r--r--   0        0        0     3423 2024-05-28 21:11:18.000000 hoppr_cop-1.4.2/hopprcop/reporting/templates/vulnerabilities.html
+-rw-r--r--   0        0        0       58 2024-05-28 21:11:18.000000 hoppr_cop-1.4.2/hopprcop/reporting/templates/vulnerability.css
+-rw-r--r--   0        0        0    10840 2024-05-28 21:11:18.000000 hoppr_cop-1.4.2/hopprcop/reporting/templates/vulnerability_details.html
+-rw-r--r--   0        0        0        0 2024-05-28 21:11:18.000000 hoppr_cop-1.4.2/hopprcop/trivy/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 21:11:18.000000 hoppr_cop-1.4.2/hopprcop/trivy/py.typed
+-rw-r--r--   0        0        0    11694 2024-05-28 21:11:18.000000 hoppr_cop-1.4.2/hopprcop/trivy/trivy_scanner.py
+-rw-r--r--   0        0        0    10374 2024-05-28 21:11:18.000000 hoppr_cop-1.4.2/hopprcop/utils.py
+-rw-r--r--   0        0        0     4179 2024-05-28 21:11:18.000000 hoppr_cop-1.4.2/hopprcop/vulnerability_combiner.py
+-rw-r--r--   0        0        0     2652 2024-05-28 21:11:18.000000 hoppr_cop-1.4.2/hopprcop/vulnerability_enhancer.py
+-rw-r--r--   0        0        0     6973 2024-05-28 21:11:18.000000 hoppr_cop-1.4.2/hopprcop/vulnerability_scanner.py
+-rw-r--r--   0        0        0     6425 2024-05-28 21:11:18.000000 hoppr_cop-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0     1267 1970-01-01 00:00:00.000000 hoppr_cop-1.4.2/PKG-INFO
```

### Comparing `hoppr_cop-1.4.1/LICENSE.md` & `hoppr_cop-1.4.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.4.1/hopprcop/combined/cli.py` & `hoppr_cop-1.4.2/hopprcop/combined/cli.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.4.1/hopprcop/combined/combined_scanner.py` & `hoppr_cop-1.4.2/hopprcop/combined/combined_scanner.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.4.1/hopprcop/enhancements/analysis_assessment.py` & `hoppr_cop-1.4.2/hopprcop/enhancements/analysis_assessment.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.4.1/hopprcop/enhancements/epss/models.py` & `hoppr_cop-1.4.2/hopprcop/enhancements/epss/models.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.4.1/hopprcop/enhancements/epss_enhancer.py` & `hoppr_cop-1.4.2/hopprcop/enhancements/epss_enhancer.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.4.1/hopprcop/gemnasium/gemnasium_scanner.py` & `hoppr_cop-1.4.2/hopprcop/gemnasium/gemnasium_scanner.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.4.1/hopprcop/gemnasium/models.py` & `hoppr_cop-1.4.2/hopprcop/gemnasium/models.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.4.1/hopprcop/grype/grype_scanner.py` & `hoppr_cop-1.4.2/hopprcop/grype/grype_scanner.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.4.1/hopprcop/grype/models.py` & `hoppr_cop-1.4.2/hopprcop/grype/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -197,15 +197,15 @@
     output_template_file: Annotated[str | None, Field(alias="output-template-file")] = None
     quiet: bool | None = None
     check_for_app_update: Annotated[bool | None, Field(alias="check-for-app-update")] = None
     only_fixed: Annotated[bool | None, Field(alias="only-fixed")] = None
     only_notfixed: Annotated[bool | None, Field(alias="only-notfixed")] = None
     platform: str | None = None
     search: Search | None = None
-    ignore: None
+    ignore: list | None = None
     exclude: list | None = None
     db: DatabaseConfig | None = None
     external_sources: Annotated[ExternalSources | None, Field(alias="externalSources")] = None
     match: ConfigMatch | None = None
     dev: Dev | None = None
     fail_on_severity: Annotated[str | None, Field(alias="fail-on-severity")] = None
     registry: Registry | None = None
```

### Comparing `hoppr_cop-1.4.1/hopprcop/hoppr_plugin/hopprcop_plugin.py` & `hoppr_cop-1.4.2/hopprcop/hoppr_plugin/hopprcop_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.4.1/hopprcop/ossindex/api/__init__.py` & `hoppr_cop-1.4.2/hopprcop/ossindex/api/__init__.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.4.1/hopprcop/ossindex/api/exception.py` & `hoppr_cop-1.4.2/hopprcop/ossindex/api/exception.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.4.1/hopprcop/ossindex/api/model.py` & `hoppr_cop-1.4.2/hopprcop/ossindex/api/model.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.4.1/hopprcop/ossindex/api/ossindex.py` & `hoppr_cop-1.4.2/hopprcop/ossindex/api/ossindex.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.4.1/hopprcop/ossindex/api/serializer.py` & `hoppr_cop-1.4.2/hopprcop/ossindex/api/serializer.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.4.1/hopprcop/ossindex/oss_index_scanner.py` & `hoppr_cop-1.4.2/hopprcop/ossindex/oss_index_scanner.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.4.1/hopprcop/reporting/__init__.py` & `hoppr_cop-1.4.2/hopprcop/reporting/__init__.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.4.1/hopprcop/reporting/gitlab/models.py` & `hoppr_cop-1.4.2/hopprcop/reporting/gitlab/models.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.4.1/hopprcop/reporting/models.py` & `hoppr_cop-1.4.2/hopprcop/reporting/models.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.4.1/hopprcop/reporting/templates/assets/vulnerabilities.css` & `hoppr_cop-1.4.2/hopprcop/reporting/templates/assets/vulnerabilities.css`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.4.1/hopprcop/reporting/templates/package-lock.json` & `hoppr_cop-1.4.2/hopprcop/reporting/templates/package-lock.json`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.4.1/hopprcop/reporting/templates/vulnerabilities.html` & `hoppr_cop-1.4.2/hopprcop/reporting/templates/vulnerabilities.html`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.4.1/hopprcop/reporting/templates/vulnerability_details.html` & `hoppr_cop-1.4.2/hopprcop/reporting/templates/vulnerability_details.html`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.4.1/hopprcop/trivy/trivy_scanner.py` & `hoppr_cop-1.4.2/hopprcop/trivy/trivy_scanner.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 from pathlib import Path
 from subprocess import PIPE, Popen
 from typing import TYPE_CHECKING, ClassVar
 
 import rich
 
-from hoppr import Affect, Component, HopprError, Sbom, Vulnerability
+from hoppr import Affect, Component, ComponentType, HopprError, Metadata, Sbom, Vulnerability
 from hoppr.utils import get_package_url
 from typing_extensions import deprecated
 
 from hopprcop.utils import build_bom_dict_from_purls, purl_check, unsupported_purl_feedback
 from hopprcop.vulnerability_scanner import VulnerabilitySuper
 
 
@@ -80,15 +80,15 @@
         super().__init__()
 
     def get_vulnerability_db(self) -> bool:
         """Downloads vulnerability database.
 
         Returns a boolean representation of success.
         """
-        args = ["trivy", "image", "--download-db-only", "--no-progress"]
+        args = ["trivy", "image", "--download-db-only", "--download-java-db-only", "--no-progress"]
         with Popen(args, stdout=PIPE, stdin=PIPE, stderr=PIPE) as process:
             # Trivy returns all messages as stderr in the 0.48.0 version.
             # To properly report the status of the database update the return code
             # is the primary check with scraping stderr being secondary.
             stdout, stderr = process.communicate()
             rtrn_code = process.returncode
             if rtrn_code == 0:
@@ -118,25 +118,29 @@
         Returns a list of CycloneDX vulnerabilities.
         """
         results: list[Vulnerability] = []
 
         _win32 = sys.platform == "win32"
         with tempfile.NamedTemporaryFile(mode="w+", delete=not _win32, encoding="utf-8") as bom_file:
             # Remove tools from metadata due to cyclonedx-go only having partial support for spec version 1.5 (as of 0.72.0)
+            # Add root component if it doesn't exist since trivy expects for this to be populated
             # TODO: roll back once full support is in cyclonedx-go
             copied_bom = bom.copy(deep=True)
-            if copied_bom.metadata:
-                copied_bom.metadata.tools = None
+            copied_bom.metadata = copied_bom.metadata or Metadata()
+            copied_bom.metadata.tools = None
+            copied_bom.metadata.component = copied_bom.metadata.component or Component(
+                type=ComponentType.LIBRARY, name="trivycomponent"
+            )
 
             bom_file.write(copied_bom.json())
             bom_file.flush()
 
-            args = ["trivy", "sbom", "--format", "cyclonedx", str(bom_file.name)]
+            args = ["trivy", "sbom", "--scanners", "vuln", "--format", "cyclonedx", str(bom_file.name)]
             if self.offline_mode:
-                args = [*args, "--skip-db-update", "--offline-scan"]
+                args = [*args, "--skip-db-update", "--skip-java-db-update", "--offline-scan"]
             cache = os.getenv("CACHE_DIR")
 
             # Check for unsupported purl types and report if found
             purls = [component.purl for component in bom.components or [] if component.purl]
             unsupported_purl_feedback(
                 self._scanner_name, self.supported_types, [get_package_url(purl) for purl in purls]
             )
@@ -189,25 +193,29 @@
         Returns a dictionary of package URL to vulnerabilities or none if no vulnerabilities are found.
         """
         results: dict[str, list[Vulnerability]] = {}
 
         _win32 = sys.platform == "win32"
         with tempfile.NamedTemporaryFile(mode="w+", delete=not _win32, encoding="utf-8") as bom_file:
             # Remove tools from metadata due to cyclonedx-go only having partial support for spec version 1.5 (as of 0.72.0)
+            # Add root component if it doesn't exist since trivy expects for this to be populated
             # TODO: roll back once full support is in cyclonedx-go
             copied_bom = bom.copy(deep=True)
-            if copied_bom.metadata:
-                copied_bom.metadata.tools = None
+            copied_bom.metadata = copied_bom.metadata or Metadata()
+            copied_bom.metadata.tools = None
+            copied_bom.metadata.component = copied_bom.metadata.component or Component(
+                type=ComponentType.LIBRARY, name="trivycomponent"
+            )
 
             bom_file.write(copied_bom.json())
             bom_file.flush()
 
-            args = ["trivy", "sbom", "--format", "cyclonedx", str(bom_file.name)]
+            args = ["trivy", "sbom", "--scanners", "vuln", "--format", "cyclonedx", str(bom_file.name)]
             if self.offline_mode:
-                args = [*args, "--skip-db-update", "--offline-scan"]
+                args = [*args, "--skip-db-update", "--skip-java-db-update", "--offline-scan"]
             cache = os.getenv("CACHE_DIR")
 
             # Check for unsupported purl types and report if found
             purls = [get_package_url(component.purl) for component in bom.components or [] if component.purl]
             unsupported_purl_feedback(self._scanner_name, self.supported_types, purls)
 
             if cache is not None:
```

### Comparing `hoppr_cop-1.4.1/hopprcop/utils.py` & `hoppr_cop-1.4.2/hopprcop/utils.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.4.1/hopprcop/vulnerability_combiner.py` & `hoppr_cop-1.4.2/hopprcop/vulnerability_combiner.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.4.1/hopprcop/vulnerability_enhancer.py` & `hoppr_cop-1.4.2/hopprcop/vulnerability_enhancer.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.4.1/hopprcop/vulnerability_scanner.py` & `hoppr_cop-1.4.2/hopprcop/vulnerability_scanner.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.4.1/pyproject.toml` & `hoppr_cop-1.4.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "hoppr-cop"
-version = "1.4.1"
+version = "1.4.2"
 description = ""
 authors = ["kganger <keith.e.ganger@lmco.com>"]
 license = "MIT"
 
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
```

### Comparing `hoppr_cop-1.4.1/PKG-INFO` & `hoppr_cop-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hoppr-cop
-Version: 1.4.1
+Version: 1.4.2
 Summary: 
 License: MIT
 Author: kganger
 Author-email: keith.e.ganger@lmco.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

