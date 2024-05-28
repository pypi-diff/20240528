# Comparing `tmp/fake_git_history-1.0.0.tar.gz` & `tmp/fake_git_history-1.0.1.tar.gz`

## Comparing `fake_git_history-1.0.0.tar` & `fake_git_history-1.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0   288825 2020-02-02 00:00:00.000000 fake_git_history-1.0.0/contribution-graph.gif
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 fake_git_history-1.0.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 fake_git_history-1.0.0/fake_git_history/__init__.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 fake_git_history-1.0.0/fake_git_history/__main__.py
--rw-r--r--   0        0        0    16437 2020-02-02 00:00:00.000000 fake_git_history-1.0.0/fake_git_history/cli.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 fake_git_history-1.0.0/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 fake_git_history-1.0.0/LICENSE
--rw-r--r--   0        0        0    11714 2020-02-02 00:00:00.000000 fake_git_history-1.0.0/README.md
--rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 fake_git_history-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    14863 2020-02-02 00:00:00.000000 fake_git_history-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0   288825 2020-02-02 00:00:00.000000 fake_git_history-1.0.1/contribution-graph.gif
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 fake_git_history-1.0.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 fake_git_history-1.0.1/fake_git_history/__init__.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 fake_git_history-1.0.1/fake_git_history/__main__.py
+-rw-r--r--   0        0        0    16606 2020-02-02 00:00:00.000000 fake_git_history-1.0.1/fake_git_history/cli.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 fake_git_history-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 fake_git_history-1.0.1/LICENSE
+-rw-r--r--   0        0        0    11714 2020-02-02 00:00:00.000000 fake_git_history-1.0.1/README.md
+-rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 fake_git_history-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0    14863 2020-02-02 00:00:00.000000 fake_git_history-1.0.1/PKG-INFO
```

### Comparing `fake_git_history-1.0.0/contribution-graph.gif` & `fake_git_history-1.0.1/contribution-graph.gif`

 * *Files identical despite different names*

### Comparing `fake_git_history-1.0.0/.github/workflows/python-publish.yml` & `fake_git_history-1.0.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `fake_git_history-1.0.0/fake_git_history/__main__.py` & `fake_git_history-1.0.1/fake_git_history/__main__.py`

 * *Files identical despite different names*

### Comparing `fake_git_history-1.0.0/fake_git_history/cli.py` & `fake_git_history-1.0.1/fake_git_history/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 import string
 import os
 import subprocess
 import re
 
 import rong  # type: ignore
 
+__version__ = "1.0.1"
+
 
 class Commit(NamedTuple):
     message: str
     date: str
 
 
 class FakeGitHistory:
@@ -170,15 +172,19 @@
         """Disable verbose mode."""
         self._log.okmsg("Verbose mode disabled.")
         self._verbose = False
         self._log.debug = False
 
     def version(self) -> None:
         """Show the version."""
-        print("Fake Git History version 1.0.0")
+        rong.Text(
+            text=f"Fake Git History version v{__version__}",
+            fg=rong.ForegroundColor.GREEN,
+            styles=[rong.Style.BOLD],
+        ).print()
 
     def set_auto_git_push(self) -> None:
         """Set auto git push."""
         self._auto_git_push = True
         self._log.primary("Auto git push enabled.")
 
     def worker(
@@ -520,9 +526,10 @@
         fgh.set_remote_origin(
             remote_origin=args.remote_origin
         )
     if args.auto_git_push:
         fgh.set_auto_git_push()
     if args.version:
         fgh.version()
+        exit()
 
     fgh.run()
```

### Comparing `fake_git_history-1.0.0/LICENSE` & `fake_git_history-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fake_git_history-1.0.0/README.md` & `fake_git_history-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `fake_git_history-1.0.0/pyproject.toml` & `fake_git_history-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 "Bug Tracker" = "https://github.com/Almas-Ali/fake-git-history/issues"
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.hatch.version]
-path = "fake_git_history/__init__.py"
+path = "fake_git_history/cli.py"
 
 [tool.ruff]
 line-length = 60
 target-version = "py311"
 respect-gitignore = false
 
 [tool.ruff.format]
```

### Comparing `fake_git_history-1.0.0/PKG-INFO` & `fake_git_history-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fake-git-history
-Version: 1.0.0
+Version: 1.0.1
 Summary: A simple utility to generate fake git history for a Github and Gitlab profile.
 Project-URL: Homepage, https://github.com/Almas-Ali/fake-git-history
 Project-URL: Documentation, https://github.com/Almas-Ali/fake-git-history#readme
 Project-URL: Repository, https://github.com/Almas-Ali/fake-git-history
 Project-URL: Bug Tracker, https://github.com/Almas-Ali/fake-git-history/issues
 Author-email: "Md. Almas Ali" <almaspr3@gmail.com>
 Maintainer-email: "Md. Almas Ali" <almaspr3@gmail.com>
```

