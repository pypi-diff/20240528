# Comparing `tmp/eyeballvul-0.4.0.tar.gz` & `tmp/eyeballvul-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eyeballvul-0.4.0.tar", max compression
+gzip compressed data, was "eyeballvul-0.4.1.tar", max compression
```

## Comparing `eyeballvul-0.4.0.tar` & `eyeballvul-0.4.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1065 2024-05-13 18:22:34.820247 eyeballvul-0.4.0/LICENSE
--rw-r--r--   0        0        0    25093 2024-05-27 14:31:53.885110 eyeballvul-0.4.0/README.md
--rw-r--r--   0        0        0      263 2024-05-27 14:00:42.100975 eyeballvul-0.4.0/eyeballvul/__init__.py
--rw-r--r--   0        0        0     8430 2024-05-27 14:32:06.013136 eyeballvul-0.4.0/eyeballvul/api.py
--rw-r--r--   0        0        0     2392 2024-05-27 12:27:10.873062 eyeballvul-0.4.0/eyeballvul/cli.py
--rw-r--r--   0        0        0       48 2024-04-24 12:29:04.251010 eyeballvul-0.4.0/eyeballvul/config/__init__.py
--rw-r--r--   0        0        0      710 2024-05-22 08:39:48.617888 eyeballvul-0.4.0/eyeballvul/config/config.toml
--rw-r--r--   0        0        0     1374 2024-05-24 07:20:46.698632 eyeballvul-0.4.0/eyeballvul/config/config_loader.py
--rw-r--r--   0        0        0    25925 2024-05-27 12:43:05.724118 eyeballvul-0.4.0/eyeballvul/converter.py
--rw-r--r--   0        0        0      731 2024-05-15 16:33:53.123068 eyeballvul-0.4.0/eyeballvul/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-25 09:14:27.186264 eyeballvul-0.4.0/eyeballvul/models/__init__.py
--rw-r--r--   0        0        0     3249 2024-05-15 15:40:32.119299 eyeballvul-0.4.0/eyeballvul/models/cache.py
--rw-r--r--   0        0        0      167 2024-05-13 18:05:00.254883 eyeballvul-0.4.0/eyeballvul/models/common.py
--rw-r--r--   0        0        0     3968 2024-05-17 10:05:11.804390 eyeballvul-0.4.0/eyeballvul/models/eyeballvul.py
--rw-r--r--   0        0        0     4039 2024-05-14 08:38:45.464076 eyeballvul-0.4.0/eyeballvul/models/osv.py
--rw-r--r--   0        0        0        0 2024-05-17 08:30:21.997460 eyeballvul-0.4.0/eyeballvul/py.typed
--rw-r--r--   0        0        0     8681 2024-05-22 08:21:37.785923 eyeballvul-0.4.0/eyeballvul/score.py
--rw-r--r--   0        0        0     6839 2024-05-21 13:35:15.816506 eyeballvul-0.4.0/eyeballvul/util.py
--rw-r--r--   0        0        0     1361 2024-05-27 14:33:16.997287 eyeballvul-0.4.0/pyproject.toml
--rw-r--r--   0        0        0    25775 1970-01-01 00:00:00.000000 eyeballvul-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-13 18:22:34.820247 eyeballvul-0.4.1/LICENSE
+-rw-r--r--   0        0        0    25714 2024-05-28 14:56:17.117042 eyeballvul-0.4.1/README.md
+-rw-r--r--   0        0        0      282 2024-05-28 14:49:06.591468 eyeballvul-0.4.1/eyeballvul/__init__.py
+-rw-r--r--   0        0        0     9460 2024-05-28 14:51:25.327684 eyeballvul-0.4.1/eyeballvul/api.py
+-rw-r--r--   0        0        0     2392 2024-05-27 12:27:10.873062 eyeballvul-0.4.1/eyeballvul/cli.py
+-rw-r--r--   0        0        0       48 2024-04-24 12:29:04.251010 eyeballvul-0.4.1/eyeballvul/config/__init__.py
+-rw-r--r--   0        0        0      710 2024-05-22 08:39:48.617888 eyeballvul-0.4.1/eyeballvul/config/config.toml
+-rw-r--r--   0        0        0     1374 2024-05-24 07:20:46.698632 eyeballvul-0.4.1/eyeballvul/config/config_loader.py
+-rw-r--r--   0        0        0    25925 2024-05-27 12:43:05.724118 eyeballvul-0.4.1/eyeballvul/converter.py
+-rw-r--r--   0        0        0      731 2024-05-15 16:33:53.123068 eyeballvul-0.4.1/eyeballvul/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-25 09:14:27.186264 eyeballvul-0.4.1/eyeballvul/models/__init__.py
+-rw-r--r--   0        0        0     3249 2024-05-15 15:40:32.119299 eyeballvul-0.4.1/eyeballvul/models/cache.py
+-rw-r--r--   0        0        0      167 2024-05-13 18:05:00.254883 eyeballvul-0.4.1/eyeballvul/models/common.py
+-rw-r--r--   0        0        0     3968 2024-05-17 10:05:11.804390 eyeballvul-0.4.1/eyeballvul/models/eyeballvul.py
+-rw-r--r--   0        0        0     4039 2024-05-14 08:38:45.464076 eyeballvul-0.4.1/eyeballvul/models/osv.py
+-rw-r--r--   0        0        0        0 2024-05-17 08:30:21.997460 eyeballvul-0.4.1/eyeballvul/py.typed
+-rw-r--r--   0        0        0     8681 2024-05-22 08:21:37.785923 eyeballvul-0.4.1/eyeballvul/score.py
+-rw-r--r--   0        0        0     6839 2024-05-21 13:35:15.816506 eyeballvul-0.4.1/eyeballvul/util.py
+-rw-r--r--   0        0        0     1361 2024-05-28 14:58:08.393545 eyeballvul-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0    26396 1970-01-01 00:00:00.000000 eyeballvul-0.4.1/PKG-INFO
```

### Comparing `eyeballvul-0.4.0/LICENSE` & `eyeballvul-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `eyeballvul-0.4.0/README.md` & `eyeballvul-0.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -76,28 +76,39 @@
   },
   "size": 4708779
 }
 ```
 ## How to use
 For any of the commands shown below, run `help(command_name)` to see its documentation.
 ```python
->>> from eyeballvul import get_commits, get_projects, get_vulns, get_revision
+>>> from eyeballvul import get_commits, get_projects, get_vulns, get_revision, get_revisions
 # `get_projects`: get the list of projects
 # get_projects() -> list[str]
 >>> projects = get_projects()
 # `get_commits`: get a list of commits, with possible filtering by date and project.
+# Important note: the filtering by date doesn't apply to the commit date, but to the
+# existence of at least one vuln associated with the commit within the date range!
 # get_commits(
 #     after: str | datetime | None = None,
 #     before: str | datetime | None = None,
 #     project: str | None = None,
 # ) -> list[str]
 >>> commits = get_commits()
 >>> commits = get_commits(after="2023-12-01")
 >>> commits = get_commits(after="2023-12-01", before="2024-03-01", project="https://github.com/torvalds/linux")
 
+# `get_revisions`: same as `get_commits`, except you get a list of `EyeballvulRevision` objects instead.
+# This method is faster than the equivalent [get_revision(commit) for commit in get_commits(...)] when no date range is provided.
+# get_revisions(
+#     after: str | datetime | None = None,
+#     before: str | datetime | None = None,
+#     project: str | None = None,
+# ) -> list[EyeballvulRevision]
+>>> revisions = get_revisions()
+
 # `get_revision`: get the revision corresponding to a given commit
 # get_revision(commit: str) -> EyeballvulRevision
 >>> revision = get_revision("some commit hash (40 characters)")
 
 # `get_vulns`: get a list of vulnerabilities, with possible filtering by date, project, and commit.
 # get_vulns(
 #     after: str | datetime | None = None,
```

### Comparing `eyeballvul-0.4.0/eyeballvul/api.py` & `eyeballvul-0.4.1/eyeballvul/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -126,14 +126,40 @@
     """
     vulns = get_vulns(after=after, before=before, project=project)
     commits = {commit for vuln in vulns for commit in vuln.commits}
     return list(commits)
 
 
 @typechecked
+def get_revisions(
+    after: str | datetime | None = None,
+    before: str | datetime | None = None,
+    project: str | None = None,
+) -> list[EyeballvulRevision]:
+    """
+    Same as `get_commits`, except that `EyeballvulRevision` objects are returned instead.
+
+    When no date range is provided, this method is faster than the equivalent `[get_revision(commit) for commit in get_commits(...)]`.
+    """
+    if after is None and before is None:
+        # If no date range is provided, we can directly query the database, which is much faster.
+        engine = create_engine(f"sqlite:///{Config.paths.db}/eyeballvul.db")
+        with Session(engine) as session:
+            query = select(EyeballvulRevision)
+            if project:
+                query = query.where(EyeballvulRevision.repo_url == project)
+            return list(session.exec(query).all())
+    else:
+        return [
+            get_revision(commit)
+            for commit in get_commits(after=after, before=before, project=project)
+        ]
+
+
+@typechecked
 def get_revision(commit: str) -> EyeballvulRevision:
     """
     Get the Eyeballvul revision that matches a commit hash.
 
     If no revision can be found, raise a ValueError.
     """
     if len(commit) != 40:
```

### Comparing `eyeballvul-0.4.0/eyeballvul/cli.py` & `eyeballvul-0.4.1/eyeballvul/cli.py`

 * *Files identical despite different names*

### Comparing `eyeballvul-0.4.0/eyeballvul/config/config.toml` & `eyeballvul-0.4.1/eyeballvul/config/config.toml`

 * *Files identical despite different names*

### Comparing `eyeballvul-0.4.0/eyeballvul/config/config_loader.py` & `eyeballvul-0.4.1/eyeballvul/config/config_loader.py`

 * *Files identical despite different names*

### Comparing `eyeballvul-0.4.0/eyeballvul/converter.py` & `eyeballvul-0.4.1/eyeballvul/converter.py`

 * *Files identical despite different names*

### Comparing `eyeballvul-0.4.0/eyeballvul/exceptions.py` & `eyeballvul-0.4.1/eyeballvul/exceptions.py`

 * *Files identical despite different names*

### Comparing `eyeballvul-0.4.0/eyeballvul/models/cache.py` & `eyeballvul-0.4.1/eyeballvul/models/cache.py`

 * *Files identical despite different names*

### Comparing `eyeballvul-0.4.0/eyeballvul/models/eyeballvul.py` & `eyeballvul-0.4.1/eyeballvul/models/eyeballvul.py`

 * *Files identical despite different names*

### Comparing `eyeballvul-0.4.0/eyeballvul/models/osv.py` & `eyeballvul-0.4.1/eyeballvul/models/osv.py`

 * *Files identical despite different names*

### Comparing `eyeballvul-0.4.0/eyeballvul/score.py` & `eyeballvul-0.4.1/eyeballvul/score.py`

 * *Files identical despite different names*

### Comparing `eyeballvul-0.4.0/eyeballvul/util.py` & `eyeballvul-0.4.1/eyeballvul/util.py`

 * *Files identical despite different names*

### Comparing `eyeballvul-0.4.0/pyproject.toml` & `eyeballvul-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eyeballvul"
-version = "0.4.0"
+version = "0.4.1"
 description = ""
 authors = ["Timothee Chauvin <timothee.chauvin28@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "eyeballvul" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `eyeballvul-0.4.0/PKG-INFO` & `eyeballvul-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eyeballvul
-Version: 0.4.0
+Version: 0.4.1
 Summary: 
 Author: Timothee Chauvin
 Author-email: timothee.chauvin28@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -96,28 +96,39 @@
   },
   "size": 4708779
 }
 ```
 ## How to use
 For any of the commands shown below, run `help(command_name)` to see its documentation.
 ```python
->>> from eyeballvul import get_commits, get_projects, get_vulns, get_revision
+>>> from eyeballvul import get_commits, get_projects, get_vulns, get_revision, get_revisions
 # `get_projects`: get the list of projects
 # get_projects() -> list[str]
 >>> projects = get_projects()
 # `get_commits`: get a list of commits, with possible filtering by date and project.
+# Important note: the filtering by date doesn't apply to the commit date, but to the
+# existence of at least one vuln associated with the commit within the date range!
 # get_commits(
 #     after: str | datetime | None = None,
 #     before: str | datetime | None = None,
 #     project: str | None = None,
 # ) -> list[str]
 >>> commits = get_commits()
 >>> commits = get_commits(after="2023-12-01")
 >>> commits = get_commits(after="2023-12-01", before="2024-03-01", project="https://github.com/torvalds/linux")
 
+# `get_revisions`: same as `get_commits`, except you get a list of `EyeballvulRevision` objects instead.
+# This method is faster than the equivalent [get_revision(commit) for commit in get_commits(...)] when no date range is provided.
+# get_revisions(
+#     after: str | datetime | None = None,
+#     before: str | datetime | None = None,
+#     project: str | None = None,
+# ) -> list[EyeballvulRevision]
+>>> revisions = get_revisions()
+
 # `get_revision`: get the revision corresponding to a given commit
 # get_revision(commit: str) -> EyeballvulRevision
 >>> revision = get_revision("some commit hash (40 characters)")
 
 # `get_vulns`: get a list of vulnerabilities, with possible filtering by date, project, and commit.
 # get_vulns(
 #     after: str | datetime | None = None,
```

