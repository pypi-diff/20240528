# Comparing `tmp/cookieplone-0.6.3.tar.gz` & `tmp/cookieplone-0.7.0.tar.gz`

## Comparing `cookieplone-0.6.3.tar` & `cookieplone-0.7.0.tar`

### file list

```diff
@@ -1,50 +1,59 @@
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 cookieplone-0.6.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 cookieplone-0.6.3/CHANGES.md
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 cookieplone-0.6.3/Makefile
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 cookieplone-0.6.3/tox.ini
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 cookieplone-0.6.3/.github/workflows/changelog.yml
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 cookieplone-0.6.3/.github/workflows/main.yml
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 cookieplone-0.6.3/cookieplone/__init__.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 cookieplone-0.6.3/cookieplone/__main__.py
--rw-r--r--   0        0        0     5801 2020-02-02 00:00:00.000000 cookieplone-0.6.3/cookieplone/cli.py
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 cookieplone-0.6.3/cookieplone/data.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 cookieplone-0.6.3/cookieplone/exceptions.py
--rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 cookieplone-0.6.3/cookieplone/generator.py
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 cookieplone-0.6.3/cookieplone/logger.py
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 cookieplone-0.6.3/cookieplone/repository.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 cookieplone-0.6.3/cookieplone/settings.py
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 cookieplone-0.6.3/cookieplone/filters/__init__.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 cookieplone-0.6.3/cookieplone/utils/__init__.py
--rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 cookieplone-0.6.3/cookieplone/utils/console.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 cookieplone-0.6.3/cookieplone/utils/containers.py
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 cookieplone-0.6.3/cookieplone/utils/files.py
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 cookieplone-0.6.3/cookieplone/utils/formatters.py
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 cookieplone-0.6.3/cookieplone/utils/git.py
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 cookieplone-0.6.3/cookieplone/utils/internal.py
--rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 cookieplone-0.6.3/cookieplone/utils/plone.py
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 cookieplone-0.6.3/cookieplone/utils/sanity.py
--rw-r--r--   0        0        0     4578 2020-02-02 00:00:00.000000 cookieplone-0.6.3/cookieplone/utils/validators.py
--rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 cookieplone-0.6.3/cookieplone/utils/versions.py
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 cookieplone-0.6.3/cookieplone/utils/commands/__init__.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 cookieplone-0.6.3/news/.changelog_template.jinja
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cookieplone-0.6.3/tests/__init__.py
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 cookieplone-0.6.3/tests/conftest.py
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 cookieplone-0.6.3/tests/test_cli.py
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 cookieplone-0.6.3/tests/test_filters.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 cookieplone-0.6.3/tests/_resources/plone/dependencies.zcml
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 cookieplone-0.6.3/tests/_resources/plone/metadata.xml
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 cookieplone-0.6.3/tests/utils/test_commands.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 cookieplone-0.6.3/tests/utils/test_console.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 cookieplone-0.6.3/tests/utils/test_containers.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 cookieplone-0.6.3/tests/utils/test_files.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 cookieplone-0.6.3/tests/utils/test_git.py
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 cookieplone-0.6.3/tests/utils/test_internal.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 cookieplone-0.6.3/tests/utils/test_plone.py
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 cookieplone-0.6.3/tests/utils/test_sanity.py
--rw-r--r--   0        0        0     5678 2020-02-02 00:00:00.000000 cookieplone-0.6.3/tests/utils/test_validators.py
--rw-r--r--   0        0        0     5363 2020-02-02 00:00:00.000000 cookieplone-0.6.3/tests/utils/test_versions.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 cookieplone-0.6.3/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 cookieplone-0.6.3/LICENSE
--rw-r--r--   0        0        0     5792 2020-02-02 00:00:00.000000 cookieplone-0.6.3/README.md
--rw-r--r--   0        0        0     4114 2020-02-02 00:00:00.000000 cookieplone-0.6.3/pyproject.toml
--rw-r--r--   0        0        0     7252 2020-02-02 00:00:00.000000 cookieplone-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 cookieplone-0.7.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 cookieplone-0.7.0/CHANGES.md
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 cookieplone-0.7.0/Makefile
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 cookieplone-0.7.0/tox.ini
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 cookieplone-0.7.0/.github/workflows/changelog.yml
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 cookieplone-0.7.0/.github/workflows/main.yml
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 cookieplone-0.7.0/cookieplone/__init__.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 cookieplone-0.7.0/cookieplone/__main__.py
+-rw-r--r--   0        0        0     6103 2020-02-02 00:00:00.000000 cookieplone-0.7.0/cookieplone/cli.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 cookieplone-0.7.0/cookieplone/data.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 cookieplone-0.7.0/cookieplone/exceptions.py
+-rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 cookieplone-0.7.0/cookieplone/generator.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 cookieplone-0.7.0/cookieplone/logger.py
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 cookieplone-0.7.0/cookieplone/repository.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 cookieplone-0.7.0/cookieplone/settings.py
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 cookieplone-0.7.0/cookieplone/filters/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cookieplone-0.7.0/cookieplone/templates/__init__.py
+-rw-r--r--   0        0        0     5315 2020-02-02 00:00:00.000000 cookieplone-0.7.0/cookieplone/templates/fixtures.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 cookieplone-0.7.0/cookieplone/templates/types.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 cookieplone-0.7.0/cookieplone/utils/__init__.py
+-rw-r--r--   0        0        0     5556 2020-02-02 00:00:00.000000 cookieplone-0.7.0/cookieplone/utils/console.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 cookieplone-0.7.0/cookieplone/utils/containers.py
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 cookieplone-0.7.0/cookieplone/utils/files.py
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 cookieplone-0.7.0/cookieplone/utils/formatters.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 cookieplone-0.7.0/cookieplone/utils/git.py
+-rw-r--r--   0        0        0     3015 2020-02-02 00:00:00.000000 cookieplone-0.7.0/cookieplone/utils/internal.py
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 cookieplone-0.7.0/cookieplone/utils/plone.py
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 cookieplone-0.7.0/cookieplone/utils/sanity.py
+-rw-r--r--   0        0        0     4578 2020-02-02 00:00:00.000000 cookieplone-0.7.0/cookieplone/utils/validators.py
+-rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 cookieplone-0.7.0/cookieplone/utils/versions.py
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 cookieplone-0.7.0/cookieplone/utils/commands/__init__.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 cookieplone-0.7.0/news/.changelog_template.jinja
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cookieplone-0.7.0/tests/__init__.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 cookieplone-0.7.0/tests/conftest.py
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 cookieplone-0.7.0/tests/test_cli.py
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 cookieplone-0.7.0/tests/test_filters.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 cookieplone-0.7.0/tests/_resources/plone/dependencies.zcml
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 cookieplone-0.7.0/tests/_resources/plone/metadata.xml
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 cookieplone-0.7.0/tests/_resources/templates/project/cookiecutter.json
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 cookieplone-0.7.0/tests/_resources/templates/project/{{ cookiecutter.__folder_name }}/README.md
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 cookieplone-0.7.0/tests/_resources/templates/sub/bar/cookiecutter.json
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 cookieplone-0.7.0/tests/_resources/templates/sub/bar/{{ cookiecutter.__folder_name }}/README.md
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 cookieplone-0.7.0/tests/templates/conftest.py
+-rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 cookieplone-0.7.0/tests/templates/test_fixtures.py
+-rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 cookieplone-0.7.0/tests/utils/test_commands.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 cookieplone-0.7.0/tests/utils/test_console.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 cookieplone-0.7.0/tests/utils/test_containers.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 cookieplone-0.7.0/tests/utils/test_files.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 cookieplone-0.7.0/tests/utils/test_git.py
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 cookieplone-0.7.0/tests/utils/test_internal.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 cookieplone-0.7.0/tests/utils/test_plone.py
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 cookieplone-0.7.0/tests/utils/test_sanity.py
+-rw-r--r--   0        0        0     5678 2020-02-02 00:00:00.000000 cookieplone-0.7.0/tests/utils/test_validators.py
+-rw-r--r--   0        0        0     5363 2020-02-02 00:00:00.000000 cookieplone-0.7.0/tests/utils/test_versions.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 cookieplone-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 cookieplone-0.7.0/LICENSE
+-rw-r--r--   0        0        0     5792 2020-02-02 00:00:00.000000 cookieplone-0.7.0/README.md
+-rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 cookieplone-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     7260 2020-02-02 00:00:00.000000 cookieplone-0.7.0/PKG-INFO
```

### Comparing `cookieplone-0.6.3/.pre-commit-config.yaml` & `cookieplone-0.7.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.3/CHANGES.md` & `cookieplone-0.7.0/CHANGES.md`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,22 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 0.7.0 (2024-05-27)
+
+
+### New features:
+
+- Add --info option to display current settings [@ericof] [#27](https://github.com/plone/cookieplone/issues/27)
+- Add pytest fixtures to be used in template development [@ericof] [#29](https://github.com/plone/cookieplone/issues/29)
+
 ## 0.6.3 (2024-05-17)
 
 
 ### Bug fixes:
 
 - Fix usage of formatter functions in a pipx environment [@ericof]
```

### Comparing `cookieplone-0.6.3/Makefile` & `cookieplone-0.7.0/Makefile`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.3/.github/workflows/changelog.yml` & `cookieplone-0.7.0/.github/workflows/changelog.yml`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.3/.github/workflows/main.yml` & `cookieplone-0.7.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.3/cookieplone/cli.py` & `cookieplone-0.7.0/cookieplone/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,14 +54,20 @@
         typer.Argument(callback=validate_extra_context, help="Extra context."),
     ] = None,
     output_dir: Annotated[
         data.OptionalPath,
         typer.Option("--output-dir", "-o", help="Where to generate the code."),
     ] = None,
     tag: Annotated[str, typer.Option(help="Tag.")] = "main",
+    info: Annotated[
+        bool,
+        typer.Option(
+            "--info", help="Display information about cookieplone installation."
+        ),
+    ] = False,
     version: Annotated[
         bool, typer.Option("--version", help="Display the version of cookieplone.")
     ] = False,
     no_input: Annotated[
         bool,
         typer.Option(
             "--no_input",
@@ -110,32 +116,38 @@
             "--debug-file", help="File to be used as a stream for DEBUG logging"
         ),
     ] = None,
     verbose: Annotated[bool, typer.Option("--verbose", "-v")] = False,
 ):
     """Generate a new Plone codebase."""
     if version:
-        console.base_print(internal.version_info())
+        console.version_screen()
         raise typer.Exit()
 
     configure_logger(stream_level="DEBUG" if verbose else "INFO", debug_file=debug_file)
     repository = os.environ.get(settings.REPO_LOCATION)
     if not repository:
-        repository = "gh:plone/cookieplone-templates"
+        repository = settings.REPO_DEFAULT
+
+    passwd = os.environ.get(
+        settings.REPO_PASSWORD, os.environ.get("COOKIECUTTER_REPO_PASSWORD")
+    )
+    tag = os.environ.get(settings.REPO_TAG) or tag
+
+    if info:
+        console.info_screen(repository=repository, passwd=passwd, tag=tag)
+        raise typer.Exit()
 
     repo_path = get_base_repository(repository)
     if not template:
         # Display template options
         template = prompt_for_template(repo_path)
     else:
         console.welcome_screen()
 
-    passwd = os.environ.get(
-        settings.REPO_PASSWORD, os.environ.get("COOKIECUTTER_REPO_PASSWORD")
-    )
     if not output_dir:
         output_dir = Path().cwd()
 
     replay_file = files.resolve_path(replay_file) if replay_file else replay_file
     if replay_file and replay_file.exists():
         # Use replay_file
         replay = replay_file
```

### Comparing `cookieplone-0.6.3/cookieplone/data.py` & `cookieplone-0.7.0/cookieplone/data.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.3/cookieplone/exceptions.py` & `cookieplone-0.7.0/cookieplone/exceptions.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.3/cookieplone/generator.py` & `cookieplone-0.7.0/cookieplone/generator.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.3/cookieplone/logger.py` & `cookieplone-0.7.0/cookieplone/logger.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.3/cookieplone/repository.py` & `cookieplone-0.7.0/cookieplone/repository.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.3/cookieplone/settings.py` & `cookieplone-0.7.0/cookieplone/settings.py`

 * *Files 19% similar despite different names*

```diff
@@ -25,12 +25,17 @@
 VOLTO_NODE = {
     16: 16,
     17: DEFAULT_NODE,
     18: 20,
 }
 MIN_DOCKER_VERSION = "20.10"
 
+## DEFAULT
+COOKIEPLONE_REPO = "https://github.com/plone/cookieplone"
+TEMPLATES_REPO = "https://github.com/plone/cookiecutter-plone"
+REPO_DEFAULT = "gh:plone/cookieplone-templates"
 
 ## Config
 QUIET_MODE_VAR = "COOKIEPLONE_QUIET_MODE_SWITCH"
 REPO_LOCATION = "COOKIEPLONE_REPOSITORY"
+REPO_TAG = "COOKIEPLONE_REPOSITORY_TAG"
 REPO_PASSWORD = "COOKIEPLONE_REPO_PASSWORD"  # noQA:S105
```

### Comparing `cookieplone-0.6.3/cookieplone/filters/__init__.py` & `cookieplone-0.7.0/cookieplone/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.3/cookieplone/utils/files.py` & `cookieplone-0.7.0/cookieplone/utils/files.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.3/cookieplone/utils/formatters.py` & `cookieplone-0.7.0/cookieplone/utils/formatters.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.3/cookieplone/utils/git.py` & `cookieplone-0.7.0/cookieplone/utils/git.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.3/cookieplone/utils/plone.py` & `cookieplone-0.7.0/cookieplone/utils/plone.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.3/cookieplone/utils/sanity.py` & `cookieplone-0.7.0/cookieplone/utils/sanity.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.3/cookieplone/utils/validators.py` & `cookieplone-0.7.0/cookieplone/utils/validators.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.3/cookieplone/utils/versions.py` & `cookieplone-0.7.0/cookieplone/utils/versions.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.3/cookieplone/utils/commands/__init__.py` & `cookieplone-0.7.0/cookieplone/utils/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.3/tests/conftest.py` & `cookieplone-0.7.0/tests/conftest.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import random
 import string
 from pathlib import Path
 
 import pytest
 from git import Repo
 
+pytest_plugins = "pytester"
+
 
 @pytest.fixture()
 def tmp_repo(tmp_path):
     repo = Repo.init(tmp_path)
     repo.index.add(tmp_path)
     repo.index.commit("test commit")
 
@@ -30,7 +32,13 @@
         cwd = Path.cwd()
         path = (cwd / "tests" / "_resources" / filepath).resolve()
         if path.exists():
             data = path.read_text()
         return data
 
     return func
+
+
+@pytest.fixture(scope="session")
+def project_source() -> Path:
+    path = (Path(__file__).parent / "_resources" / "templates").resolve()
+    return path
```

### Comparing `cookieplone-0.6.3/tests/test_cli.py` & `cookieplone-0.7.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.3/tests/test_filters.py` & `cookieplone-0.7.0/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.3/tests/utils/test_commands.py` & `cookieplone-0.7.0/tests/utils/test_commands.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.3/tests/utils/test_console.py` & `cookieplone-0.7.0/tests/utils/test_console.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.3/tests/utils/test_files.py` & `cookieplone-0.7.0/tests/utils/test_files.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.3/tests/utils/test_git.py` & `cookieplone-0.7.0/tests/utils/test_git.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.3/tests/utils/test_plone.py` & `cookieplone-0.7.0/tests/utils/test_plone.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.3/tests/utils/test_sanity.py` & `cookieplone-0.7.0/tests/utils/test_sanity.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.3/tests/utils/test_validators.py` & `cookieplone-0.7.0/tests/utils/test_validators.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.3/tests/utils/test_versions.py` & `cookieplone-0.7.0/tests/utils/test_versions.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.3/.gitignore` & `cookieplone-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.3/LICENSE` & `cookieplone-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.3/README.md` & `cookieplone-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `cookieplone-0.6.3/pyproject.toml` & `cookieplone-0.7.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -28,19 +28,22 @@
 dependencies = [
   "cookiecutter==2.6.0",
   "semver==3.0.2",
   "typer==0.12.3",
   "packaging==24.0",
   "gitpython==3.1.43",
   "xmltodict==0.13.0",
-  "black",
+  "black==24.4.2",
   "isort",
   "zpretty"
 ]
 
+[project.entry-points.pytest11]
+cookieplone = "cookieplone.templates.fixtures"
+
 [project.scripts]
 cookieplone = 'cookieplone.__main__:main'
 
 [project.urls]
 Documentation = "https://github.com/plone/cookieplone#readme"
 Issues = "https://github.com/plone/cookieplone/issues"
 Source = "https://github.com/plone/cookieplone"
```

### Comparing `cookieplone-0.6.3/PKG-INFO` & `cookieplone-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: cookieplone
-Version: 0.6.3
+Version: 0.7.0
 Summary: Create Plone projects, addons, documentation with ease!
 Project-URL: Documentation, https://github.com/plone/cookieplone#readme
 Project-URL: Issues, https://github.com/plone/cookieplone/issues
 Project-URL: Source, https://github.com/plone/cookieplone
 Author-email: Plone Community <dev@plone.org>
 License-Expression: MIT
 License-File: LICENSE
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Code Generators
 Requires-Python: >=3.10
-Requires-Dist: black
+Requires-Dist: black==24.4.2
 Requires-Dist: cookiecutter==2.6.0
 Requires-Dist: gitpython==3.1.43
 Requires-Dist: isort
 Requires-Dist: packaging==24.0
 Requires-Dist: semver==3.0.2
 Requires-Dist: typer==0.12.3
 Requires-Dist: xmltodict==0.13.0
```

