# Comparing `tmp/cally-0.4.0.tar.gz` & `tmp/cally-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cally-0.4.0.tar", last modified: Wed Apr 10 09:19:34 2024, max compression
+gzip compressed data, was "cally-0.4.1.tar", last modified: Tue May 28 09:11:50 2024, max compression
```

## Comparing `cally-0.4.0.tar` & `cally-0.4.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:19:34.620816 cally-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-10 09:19:30.000000 cally-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    27479 2024-04-10 09:19:34.620816 cally-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5618 2024-04-10 09:19:30.000000 cally-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-10 09:19:30.000000 cally-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 09:19:34.620816 cally-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:19:34.608816 cally-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:19:34.612816 cally-0.4.0/src/cally/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:19:34.612816 cally-0.4.0/src/cally/cdk/
--rw-r--r--   0 runner    (1001) docker     (127)     7760 2024-04-10 09:19:30.000000 cally-0.4.0/src/cally/cdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:19:30.000000 cally-0.4.0/src/cally/cdk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:19:34.612816 cally-0.4.0/src/cally/cdk/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:19:30.000000 cally-0.4.0/src/cally/cdk/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:19:34.612816 cally-0.4.0/src/cally/cdk/stacks/
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-10 09:19:30.000000 cally-0.4.0/src/cally/cdk/stacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:19:34.612816 cally-0.4.0/src/cally/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-10 09:19:30.000000 cally-0.4.0/src/cally/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-10 09:19:30.000000 cally-0.4.0/src/cally/cli/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:19:34.616816 cally-0.4.0/src/cally/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:19:30.000000 cally-0.4.0/src/cally/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-10 09:19:30.000000 cally-0.4.0/src/cally/cli/commands/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-10 09:19:30.000000 cally-0.4.0/src/cally/cli/commands/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-10 09:19:30.000000 cally-0.4.0/src/cally/cli/commands/tf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:19:34.616816 cally-0.4.0/src/cally/cli/config/
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-10 09:19:30.000000 cally-0.4.0/src/cally/cli/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-04-10 09:19:30.000000 cally-0.4.0/src/cally/cli/config/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-10 09:19:30.000000 cally-0.4.0/src/cally/cli/config/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-10 09:19:30.000000 cally-0.4.0/src/cally/cli/config/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-10 09:19:30.000000 cally-0.4.0/src/cally/cli/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:19:30.000000 cally-0.4.0/src/cally/cli/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:19:34.616816 cally-0.4.0/src/cally/cli/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:19:30.000000 cally-0.4.0/src/cally/cli/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-10 09:19:30.000000 cally-0.4.0/src/cally/cli/tools/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-10 09:19:30.000000 cally-0.4.0/src/cally/cli/tools/terraform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:19:34.616816 cally-0.4.0/src/cally/testing/
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-10 09:19:30.000000 cally-0.4.0/src/cally/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-10 09:19:30.000000 cally-0.4.0/src/cally/testing/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-10 09:19:30.000000 cally-0.4.0/src/cally/testing/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:19:30.000000 cally-0.4.0/src/cally/testing/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:19:34.616816 cally-0.4.0/src/cally.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    27479 2024-04-10 09:19:34.000000 cally-0.4.0/src/cally.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-10 09:19:34.000000 cally-0.4.0/src/cally.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 09:19:34.000000 cally-0.4.0/src/cally.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-10 09:19:34.000000 cally-0.4.0/src/cally.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-10 09:19:34.000000 cally-0.4.0/src/cally.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-10 09:19:34.000000 cally-0.4.0/src/cally.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:11:50.448250 cally-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-05-28 09:11:46.000000 cally-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    27576 2024-05-28 09:11:50.448250 cally-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5618 2024-05-28 09:11:46.000000 cally-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-28 09:11:46.000000 cally-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 09:11:50.448250 cally-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:11:50.440250 cally-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:11:50.440250 cally-0.4.1/src/cally/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:11:50.444250 cally-0.4.1/src/cally/cdk/
+-rw-r--r--   0 runner    (1001) docker     (127)     9835 2024-05-28 09:11:46.000000 cally-0.4.1/src/cally/cdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:11:46.000000 cally-0.4.1/src/cally/cdk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:11:50.444250 cally-0.4.1/src/cally/cdk/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:11:46.000000 cally-0.4.1/src/cally/cdk/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:11:50.444250 cally-0.4.1/src/cally/cdk/stacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-28 09:11:46.000000 cally-0.4.1/src/cally/cdk/stacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:11:50.444250 cally-0.4.1/src/cally/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-28 09:11:46.000000 cally-0.4.1/src/cally/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-28 09:11:46.000000 cally-0.4.1/src/cally/cli/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:11:50.444250 cally-0.4.1/src/cally/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:11:46.000000 cally-0.4.1/src/cally/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-28 09:11:46.000000 cally-0.4.1/src/cally/cli/commands/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-28 09:11:46.000000 cally-0.4.1/src/cally/cli/commands/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-28 09:11:46.000000 cally-0.4.1/src/cally/cli/commands/tf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:11:50.444250 cally-0.4.1/src/cally/cli/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-28 09:11:46.000000 cally-0.4.1/src/cally/cli/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-28 09:11:46.000000 cally-0.4.1/src/cally/cli/config/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-28 09:11:46.000000 cally-0.4.1/src/cally/cli/config/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-28 09:11:46.000000 cally-0.4.1/src/cally/cli/config/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-28 09:11:46.000000 cally-0.4.1/src/cally/cli/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:11:46.000000 cally-0.4.1/src/cally/cli/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:11:50.448250 cally-0.4.1/src/cally/cli/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:11:46.000000 cally-0.4.1/src/cally/cli/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-05-28 09:11:46.000000 cally-0.4.1/src/cally/cli/tools/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-28 09:11:46.000000 cally-0.4.1/src/cally/cli/tools/terraform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:11:50.448250 cally-0.4.1/src/cally/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-28 09:11:46.000000 cally-0.4.1/src/cally/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-28 09:11:46.000000 cally-0.4.1/src/cally/testing/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-28 09:11:46.000000 cally-0.4.1/src/cally/testing/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:11:46.000000 cally-0.4.1/src/cally/testing/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:11:50.448250 cally-0.4.1/src/cally.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    27576 2024-05-28 09:11:50.000000 cally-0.4.1/src/cally.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-28 09:11:50.000000 cally-0.4.1/src/cally.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 09:11:50.000000 cally-0.4.1/src/cally.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-28 09:11:50.000000 cally-0.4.1/src/cally.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-28 09:11:50.000000 cally-0.4.1/src/cally.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-28 09:11:50.000000 cally-0.4.1/src/cally.egg-info/top_level.txt
```

### Comparing `cally-0.4.0/LICENSE` & `cally-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cally-0.4.0/PKG-INFO` & `cally-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cally
-Version: 0.4.0
+Version: 0.4.1
 Summary: A config as infrastructure foundation for your Internal Developer Platform
 Author-email: Leon Wright <techman83@gmail.com>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
@@ -399,14 +399,15 @@
 Requires-Dist: ruff; extra == "development"
 Requires-Dist: types-PyYAML; extra == "development"
 Requires-Dist: sphinx; extra == "development"
 Requires-Dist: sphinx-autobuild; extra == "development"
 Requires-Dist: sphinx-issues; extra == "development"
 Requires-Dist: sphinxcontrib-log-cabinet; extra == "development"
 Requires-Dist: sphinx-tabs; extra == "development"
+Requires-Dist: sphinx-click; extra == "development"
 Requires-Dist: Pallets-Sphinx-Themes; extra == "development"
 Provides-Extra: test
 Requires-Dist: black; extra == "test"
 Requires-Dist: build; extra == "test"
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: pytest; extra == "test"
@@ -418,14 +419,15 @@
 Provides-Extra: provider-build
 Requires-Dist: build; extra == "provider-build"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-issues; extra == "docs"
 Requires-Dist: sphinxcontrib-log-cabinet; extra == "docs"
 Requires-Dist: sphinx-tabs; extra == "docs"
+Requires-Dist: sphinx-click; extra == "docs"
 Requires-Dist: Pallets-Sphinx-Themes; extra == "docs"
 
 # Cally
 A config as infrastructure foundation for your Internal Developer Platform
 
 ### Why
 To provide a powerful, but consisent configuration, and CLI to common Platform Engineering tasks
```

### Comparing `cally-0.4.0/README.md` & `cally-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `cally-0.4.0/pyproject.toml` & `cally-0.4.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 
   # docs
   "sphinx",
   "sphinx-autobuild",
   "sphinx-issues",
   "sphinxcontrib-log-cabinet",
   "sphinx-tabs",
+  "sphinx-click",
   "Pallets-Sphinx-Themes",
 ]
 test = [
   "black",
   "build",
   "coverage",
   "mypy",
@@ -63,14 +64,15 @@
   "build"
 ]
 docs = [
   "sphinx",
   "sphinx-issues",
   "sphinxcontrib-log-cabinet",
   "sphinx-tabs",
+  "sphinx-click",
   "Pallets-Sphinx-Themes",
 ]
 
 [project.scripts]
 cally = "cally.cli:cally"
 
 [tool.black]
```

### Comparing `cally-0.4.0/src/cally/cdk/stacks/__init__.py` & `cally-0.4.1/src/cally/cdk/stacks/__init__.py`

 * *Files identical despite different names*

### Comparing `cally-0.4.0/src/cally/cli/__init__.py` & `cally-0.4.1/src/cally/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `cally-0.4.0/src/cally/cli/commands/tf.py` & `cally-0.4.1/src/cally/cli/commands/tf.py`

 * *Files identical despite different names*

### Comparing `cally-0.4.0/src/cally/cli/config/__init__.py` & `cally-0.4.1/src/cally/cli/config/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,14 +67,17 @@
     ctx: click.Context, param: click.Parameter, value: Union[str, int]
 ) -> Union[str, int]:
     setattr(ctx.obj, str(param.name), value)
     return value
 
 
 def service_options(func):
+    """This decorator, can be used on any custom commands where you expect
+    a service and environment to be set.
+    """
     options = [
         click.option(
             '--environment',
             envvar='CALLY_ENVIRONMENT',
             expose_value=False,
             required=True,
             help='Environment to operate within',
```

### Comparing `cally-0.4.0/src/cally/cli/config/loader.py` & `cally-0.4.1/src/cally/cli/config/loader.py`

 * *Files identical despite different names*

### Comparing `cally-0.4.0/src/cally/cli/config/types.py` & `cally-0.4.1/src/cally/cli/config/types.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,14 +17,19 @@
 
     def backend_config(self, service: dict) -> dict:
         return {self.path_key: self.path.format(**service), **self.config}
 
 
 @dataclass
 class CallyStackService(CallyService):
+    """This dataclass is automatically passed to the CallyStack class during
+    instantiation. Allowing access to any service property, though it is
+    recommended to use the documented functions.
+    """
+
     stack_type: str
     backend: CallyBackend = field(default_factory=CallyBackend)
     providers: dict = field(default_factory=dict)
     stack_vars: dict = field(default_factory=dict)
 
     def __setattr__(self, prop, val):
         if prop == 'backend' and isinstance(val, dict):
@@ -40,11 +45,14 @@
     def backend_config(self) -> dict:
         return self.backend.backend_config(self.to_dict())
 
     def get_provider_vars(self, provider: str) -> dict:
         return self.providers.get(provider, {})
 
     def get_stack_var(self, var: str, default: Optional[Any] = None) -> Any:
+        """Any stack var, configured on the service is available via this method, with
+        the ability to provide a default.
+        """
         return self.stack_vars.get(var, default)
 
     def to_dict(self) -> dict:
         return asdict(self)
```

### Comparing `cally-0.4.0/src/cally/cli/config/validators.py` & `cally-0.4.1/src/cally/cli/config/validators.py`

 * *Files identical despite different names*

### Comparing `cally-0.4.0/src/cally/cli/constants.py` & `cally-0.4.1/src/cally/cli/constants.py`

 * *Files identical despite different names*

### Comparing `cally-0.4.0/src/cally/cli/tools/provider.py` & `cally-0.4.1/src/cally/cli/tools/provider.py`

 * *Files identical despite different names*

### Comparing `cally-0.4.0/src/cally/cli/tools/terraform.py` & `cally-0.4.1/src/cally/cli/tools/terraform.py`

 * *Files identical despite different names*

### Comparing `cally-0.4.0/src/cally/testing/__init__.py` & `cally-0.4.1/src/cally/testing/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,14 +9,20 @@
 from cally.cli.config import CallyConfig
 
 from .constants import HOME_ENVS
 from .exceptions import CallyTestingTestdataError
 
 
 class CallyTestHarness(TestCase):
+    """Cally provides a Test Harness as good base for building robust unit testing
+    for your IDP and IAC. It takes care of ensuring a clean environment, and discrete
+    working directory for each unittest, along with providing some useful methods for
+    getting testdata or default service objects.
+    """
+
     working: TemporaryDirectory
     _testdata: Path
 
     def setUp(self):
         self.current_working = Path().cwd()
         self.working = TemporaryDirectory()
         self.env_patcher = mock.patch.dict(
@@ -34,14 +40,15 @@
     def tearDown(self):
         self.env_patcher.stop()
         os.chdir(self.current_working)
         self.working.cleanup()
 
     @property
     def testdata(self) -> Path:
+        """Attempts to find a directory called 'testdata' within your tests directory"""
         if getattr(self, '_testdata', None) is None:
             for parent in Path(getfile(self.__class__)).parents:
                 testdata = Path(parent, 'testdata')
                 if testdata.exists() and testdata.is_dir():
                     self._testdata = testdata
                     return self._testdata
                 if parent.is_dir() and parent.name == 'tests':
@@ -49,28 +56,40 @@
             raise CallyTestingTestdataError(
                 "No testdata found, expected structure <project_root>/tests/testdata"
             )
         return self._testdata
 
     @staticmethod
     def get_cally_config(service='test', environment='cally') -> CallyConfig:
+        """Returns a CallyConfig object, with a service and environment pre-configured as
+        'test' and 'cally'"""
         config = CallyConfig(config_file=Path('not-required.yaml'))
         config.service = service
         config.environment = environment
         return config
 
     def get_test_file(self, filename) -> Path:
+        """Loads a the specified file path as a Path object, from the testdata
+        directory
+        """
         return Path(self.testdata, filename)
 
     def load_test_file(self, filename) -> str:
+        """Loads a testdata file and reads it in as text"""
         return self.get_test_file(filename).read_text()
 
     def load_json_file(self, filename) -> dict:
+        """Loads a json testdata file and returns it as a dictionary"""
         return json.loads(self.load_test_file(filename))
 
 
 class CallyTfTestHarness(CallyTestHarness):
+    """This is an extension of the Cally Test harness, specifically for testing
+    Stacks."""
 
     def synth_stack(self, stack: CallyStack) -> dict:
+        """When passed a CallyStack object, synths it and returns the dictionary
+        payload generated by the cdktf. Can be used to unit test your stacks.
+        """
         stack.synth_stack(self.working.name)
         output_file = Path(self.working.name, 'stacks', stack.name, 'cdk.tf.json')
         return json.loads(output_file.read_text())
```

### Comparing `cally-0.4.0/src/cally.egg-info/PKG-INFO` & `cally-0.4.1/src/cally.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cally
-Version: 0.4.0
+Version: 0.4.1
 Summary: A config as infrastructure foundation for your Internal Developer Platform
 Author-email: Leon Wright <techman83@gmail.com>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
@@ -399,14 +399,15 @@
 Requires-Dist: ruff; extra == "development"
 Requires-Dist: types-PyYAML; extra == "development"
 Requires-Dist: sphinx; extra == "development"
 Requires-Dist: sphinx-autobuild; extra == "development"
 Requires-Dist: sphinx-issues; extra == "development"
 Requires-Dist: sphinxcontrib-log-cabinet; extra == "development"
 Requires-Dist: sphinx-tabs; extra == "development"
+Requires-Dist: sphinx-click; extra == "development"
 Requires-Dist: Pallets-Sphinx-Themes; extra == "development"
 Provides-Extra: test
 Requires-Dist: black; extra == "test"
 Requires-Dist: build; extra == "test"
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: pytest; extra == "test"
@@ -418,14 +419,15 @@
 Provides-Extra: provider-build
 Requires-Dist: build; extra == "provider-build"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-issues; extra == "docs"
 Requires-Dist: sphinxcontrib-log-cabinet; extra == "docs"
 Requires-Dist: sphinx-tabs; extra == "docs"
+Requires-Dist: sphinx-click; extra == "docs"
 Requires-Dist: Pallets-Sphinx-Themes; extra == "docs"
 
 # Cally
 A config as infrastructure foundation for your Internal Developer Platform
 
 ### Why
 To provide a powerful, but consisent configuration, and CLI to common Platform Engineering tasks
```

### Comparing `cally-0.4.0/src/cally.egg-info/SOURCES.txt` & `cally-0.4.1/src/cally.egg-info/SOURCES.txt`

 * *Files identical despite different names*

