# Comparing `tmp/lintian_codeclimate-0.1.1.tar.gz` & `tmp/lintian_codeclimate-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lintian_codeclimate-0.1.1.tar", last modified: Thu May 16 11:45:36 2024, max compression
+gzip compressed data, was "lintian_codeclimate-0.1.2.tar", last modified: Tue May 28 13:49:51 2024, max compression
```

## Comparing `lintian_codeclimate-0.1.1.tar` & `lintian_codeclimate-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 11:45:36.047475 lintian_codeclimate-0.1.1/
--rw-rw-rw-   0 root         (0) root         (0)      432 2024-05-16 11:45:30.000000 lintian_codeclimate-0.1.1/.flake8
--rw-rw-rw-   0 root         (0) root         (0)      632 2024-05-16 11:45:30.000000 lintian_codeclimate-0.1.1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     2515 2024-05-16 11:45:30.000000 lintian_codeclimate-0.1.1/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1083 2024-05-16 11:45:30.000000 lintian_codeclimate-0.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1265 2024-05-16 11:45:36.047475 lintian_codeclimate-0.1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      392 2024-05-16 11:45:30.000000 lintian_codeclimate-0.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 11:45:36.044475 lintian_codeclimate-0.1.1/lintian_codeclimate/
--rw-rw-rw-   0 root         (0) root         (0)      337 2024-05-16 11:45:30.000000 lintian_codeclimate-0.1.1/lintian_codeclimate/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      273 2024-05-16 11:45:30.000000 lintian_codeclimate-0.1.1/lintian_codeclimate/__main__.py
--rw-r--r--   0 root         (0) root         (0)      411 2024-05-16 11:45:35.000000 lintian_codeclimate-0.1.1/lintian_codeclimate/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     7190 2024-05-16 11:45:30.000000 lintian_codeclimate-0.1.1/lintian_codeclimate/parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 11:45:36.046475 lintian_codeclimate-0.1.1/lintian_codeclimate/tests/
--rw-rw-rw-   0 root         (0) root         (0)      164 2024-05-16 11:45:30.000000 lintian_codeclimate-0.1.1/lintian_codeclimate/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2134 2024-05-16 11:45:30.000000 lintian_codeclimate-0.1.1/lintian_codeclimate/tests/test_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 11:45:36.046475 lintian_codeclimate-0.1.1/lintian_codeclimate.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1265 2024-05-16 11:45:36.000000 lintian_codeclimate-0.1.1/lintian_codeclimate.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      485 2024-05-16 11:45:36.000000 lintian_codeclimate-0.1.1/lintian_codeclimate.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 11:45:36.000000 lintian_codeclimate-0.1.1/lintian_codeclimate.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-05-16 11:45:36.000000 lintian_codeclimate-0.1.1/lintian_codeclimate.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-05-16 11:45:36.000000 lintian_codeclimate-0.1.1/lintian_codeclimate.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1380 2024-05-16 11:45:30.000000 lintian_codeclimate-0.1.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-16 11:45:36.047475 lintian_codeclimate-0.1.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 13:49:51.845375 lintian_codeclimate-0.1.2/
+-rw-rw-rw-   0 root         (0) root         (0)      480 2024-05-28 13:49:45.000000 lintian_codeclimate-0.1.2/.flake8
+-rw-rw-rw-   0 root         (0) root         (0)      632 2024-05-28 13:49:45.000000 lintian_codeclimate-0.1.2/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     2515 2024-05-28 13:49:45.000000 lintian_codeclimate-0.1.2/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1083 2024-05-28 13:49:45.000000 lintian_codeclimate-0.1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1265 2024-05-28 13:49:51.845375 lintian_codeclimate-0.1.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      392 2024-05-28 13:49:45.000000 lintian_codeclimate-0.1.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 13:49:51.843375 lintian_codeclimate-0.1.2/lintian_codeclimate/
+-rw-rw-rw-   0 root         (0) root         (0)      337 2024-05-28 13:49:45.000000 lintian_codeclimate-0.1.2/lintian_codeclimate/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      273 2024-05-28 13:49:45.000000 lintian_codeclimate-0.1.2/lintian_codeclimate/__main__.py
+-rw-r--r--   0 root         (0) root         (0)      411 2024-05-28 13:49:51.000000 lintian_codeclimate-0.1.2/lintian_codeclimate/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     7720 2024-05-28 13:49:45.000000 lintian_codeclimate-0.1.2/lintian_codeclimate/parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 13:49:51.844375 lintian_codeclimate-0.1.2/lintian_codeclimate/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      164 2024-05-28 13:49:45.000000 lintian_codeclimate-0.1.2/lintian_codeclimate/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6190 2024-05-28 13:49:45.000000 lintian_codeclimate-0.1.2/lintian_codeclimate/tests/test_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 13:49:51.844375 lintian_codeclimate-0.1.2/lintian_codeclimate.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1265 2024-05-28 13:49:51.000000 lintian_codeclimate-0.1.2/lintian_codeclimate.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      485 2024-05-28 13:49:51.000000 lintian_codeclimate-0.1.2/lintian_codeclimate.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 13:49:51.000000 lintian_codeclimate-0.1.2/lintian_codeclimate.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-05-28 13:49:51.000000 lintian_codeclimate-0.1.2/lintian_codeclimate.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-05-28 13:49:51.000000 lintian_codeclimate-0.1.2/lintian_codeclimate.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1380 2024-05-28 13:49:45.000000 lintian_codeclimate-0.1.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 13:49:51.845375 lintian_codeclimate-0.1.2/setup.cfg
```

### Comparing `lintian_codeclimate-0.1.1/.gitignore` & `lintian_codeclimate-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `lintian_codeclimate-0.1.1/.gitlab-ci.yml` & `lintian_codeclimate-0.1.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `lintian_codeclimate-0.1.1/LICENSE` & `lintian_codeclimate-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lintian_codeclimate-0.1.1/PKG-INFO` & `lintian_codeclimate-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lintian-codeclimate
-Version: 0.1.1
+Version: 0.1.2
 Summary: Codeclimate parser for lintian
 Author-email: Duncan Macleod <macleoddm@cardiff.ac.uk>
 License: MIT
 Project-URL: Homepage, https://gitlab.com/duncanmmacleod/lintian-codeclimate/
 Project-URL: Bug Tracker, https://gitlab.com/duncanmmacleod/lintian-codeclimate/-/issues/
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `lintian_codeclimate-0.1.1/lintian_codeclimate/parser.py` & `lintian_codeclimate-0.1.2/lintian_codeclimate/parser.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,38 +18,52 @@
 CWD = Path(os.curdir)
 
 CHECK_REGEX = re.compile(
     r"Check: (?P<path>debian\/[\w-]+)?(/)?(field(s)?/(?P<field>[\w-]+))?",
 )
 LINE_REGEX = re.compile(
     r"\A(?P<type>[A-Z]):\s+"
-    r"(?P<package>[\w-]+( source)?):\s+"
+    r"(?P<package>[\w-]+)(\s+(?P<class>(source|changes)))?:\s+"
     r"(?P<tag>[\w-]+)(\s+)?"
     r"(?P<desc>.*)?"
 )
 NOTES_REGEX = re.compile(
     r"\AN:(\s+)?(?P<content>.*)",
 )
 SEVERITY = {
     "I": "info",
     "P": "info",
     "W": "minor",
     "E": "major",
 }
 TAG_MAP = {
+    "bogus-mail-host": {
+        "block": None,
+        "pattern": r"(localhost|\.localdomain)",
+    },
+    "bogus-mail-host-in-debian-changelog": {
+        "block": None,
+        "pattern": r"(localhost|\.localdomain)",
+    },
     "copyright-refers-to-symlink-license": {
         "block": "license",
         "pattern": "{desc}",
     },
     "insecure-copyright-format-uri": {
         "field": "format",
     },
     "newer-standards-version": {
         "field": "standards-version",
     },
+    "no-nmu-in-changelog": {
+        "path": "debian/changelog",
+    },
+    "source-nmu-has-incorrect-version-number": {
+        "path": "debian/changelog",
+    },
     "pypi-homepage": {
         "field": "homepage",
     },
     "python-package-missing-depends-on-python": {
         "field": "depends",
     },
     "python3-script-but-no-python3-dep": {
@@ -58,14 +72,16 @@
     "uses-debhelper-compat-file": {
         "path": "debian/compat",
     },
 }
 DESC_INCLUDES_LINE_NUMBER = [
     "debian-changelog-line-too-long",
     "debian-changelog-has-wrong-day-of-week",
+    "no-nmu-in-changelog",
+    "source-nmu-has-incorrect-version-number",
 ]
 
 
 def _get_location_debian(
     stream,
     default=1,
     field=None,
@@ -77,15 +93,15 @@
     """
     start = 0
     inblock = block is None
     # if block given, but not field or pattern, match the start of the block
     if block and not (field or pattern):
         pattern = block
     for i, line in enumerate(stream, start=1):
-        if line.lower().startswith(block.lower()):
+        if block and line.lower().startswith(block.lower()):
             inblock = True
         if not inblock:  # keep looking
             continue
         if pattern and re.search(pattern, line, re.I):
             return (i, i)
         if field and line.lower().startswith(field):
             start = i
@@ -141,46 +157,45 @@
         "type": "issue",
         # include parsed information to assist in updated issues later
         "parsed": params,
     }
 
 
 def update_issue(issue, project_dir=CWD, note=None):
-    package = issue["parsed"]["package"]
+    params = issue.pop("parsed", {})
     tag = issue["check_name"]
 
     # find the detailed note (if parsed) and use that fill out
     # the body content, and the location
     loc_params = {
         "path": "debian/control",
     }
-    if package and not package.endswith(" source"):
-        loc_params["block"] = f"package: {package}"
+    if params.get("package") and params.get("class") is None:
+        loc_params["block"] = f"package: {params['package']}"
+    if params.get("class") == "changes":
+        loc_params["path"] = "debian/changelog"
     loc_params.update(TAG_MAP.get(tag, {}))
     if loc_params.get("pattern"):
-        loc_params["pattern"] = loc_params["pattern"].format(**issue["parsed"])
+        loc_params["pattern"] = loc_params["pattern"].format(**params)
     if note:
         issue["content"] = {"body": note}
         if match := CHECK_REGEX.search(note):
             for key, value in match.groupdict().items():
                 if value:
                     loc_params[key] = value
 
     if tag in DESC_INCLUDES_LINE_NUMBER:
-        loc_params["default"] = int(issue["parsed"]["desc"][-2])
+        loc_params["default"] = int(params["desc"][-2])
 
     # make path relative to project_dir
     loc_params["path"] = project_dir / loc_params["path"]
 
     # find location
     issue["location"] = get_location(**loc_params)
 
-    # remove parsed info
-    issue.pop("parsed", None)
-
     return issue
 
 
 def parse_stream(stream, project_dir=CWD):
     issues = []
     notes = defaultdict(list)
     currentnote = []
```

### Comparing `lintian_codeclimate-0.1.1/lintian_codeclimate.egg-info/PKG-INFO` & `lintian_codeclimate-0.1.2/lintian_codeclimate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lintian-codeclimate
-Version: 0.1.1
+Version: 0.1.2
 Summary: Codeclimate parser for lintian
 Author-email: Duncan Macleod <macleoddm@cardiff.ac.uk>
 License: MIT
 Project-URL: Homepage, https://gitlab.com/duncanmmacleod/lintian-codeclimate/
 Project-URL: Bug Tracker, https://gitlab.com/duncanmmacleod/lintian-codeclimate/-/issues/
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `lintian_codeclimate-0.1.1/pyproject.toml` & `lintian_codeclimate-0.1.2/pyproject.toml`

 * *Files identical despite different names*

