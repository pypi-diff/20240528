# Comparing `tmp/isvirtual-1.1.0.tar.gz` & `tmp/isvirtual-1.2.0.tar.gz`

## Comparing `isvirtual-1.1.0.tar` & `isvirtual-1.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 isvirtual-1.1.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 isvirtual-1.1.0/.github/workflows/release.yml
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 isvirtual-1.1.0/src/VERSION.md
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 isvirtual-1.1.0/src/__init__.py
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 isvirtual-1.1.0/src/main.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 isvirtual-1.1.0/.gitignore
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 isvirtual-1.1.0/LICENSE
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 isvirtual-1.1.0/README.md
--rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 isvirtual-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     4193 2020-02-02 00:00:00.000000 isvirtual-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 isvirtual-1.2.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 isvirtual-1.2.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 isvirtual-1.2.0/src/VERSION.md
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 isvirtual-1.2.0/src/__init__.py
+-rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 isvirtual-1.2.0/src/main.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 isvirtual-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 isvirtual-1.2.0/LICENSE
+-rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 isvirtual-1.2.0/README.md
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 isvirtual-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4666 2020-02-02 00:00:00.000000 isvirtual-1.2.0/PKG-INFO
```

### Comparing `isvirtual-1.1.0/.github/workflows/publish.yml` & `isvirtual-1.2.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `isvirtual-1.1.0/.github/workflows/release.yml` & `isvirtual-1.2.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `isvirtual-1.1.0/LICENSE` & `isvirtual-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `isvirtual-1.1.0/README.md` & `isvirtual-1.2.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -18,43 +18,53 @@
 
 ## Python
 Simple check:
 ```python
 from isvirtual import is_virtual_env
 
 if __name__ == "__main__":
-    if is_virtual_env() is True:
-        print("You are within a virtual environment")
+    if is_virtual() is True:
+        print("You are within a virtual environment which can either be venv, virtualenv or conda.")
     else:
         print("You are not in a virtual env")
 ```
 
-You can also check if you are specifically in a `venv` or `virtualenv` environment:
+You can also check if you are specifically in a `venv`, `virtualenv` or `conda` environment:
 ```python
 from isvirtual import is_venv, is_virtualenv
 
 if __name__ == "__main__":
     if is_venv() is True:
         print("You are in a venv")
     elif is_virtualenv() is True:
         print("You are in a virtualenv")
+    elif is_conda() is True:
+        print("You are in a conda env")
     else:
-        print("You are not in a virtual env")
+        print("You are not in a any type of virtual env")
 ```
 
-You can also get the info from the env coming from `pyvenv.cfg`. The `sys.prefix` data is added to the original config file:
+You can also get the info from the env coming from `pyvenv.cfg` or load equivalent data from `conda` config. The `sys.prefix` data is added to the original config file under the key `prefix`:
 ```python
-from isvirtual import is_virtual_env, pyvenv_cfg
+from isvirtual import is_virtual_env, get_config
 
 if __name__ == "__main__":
-    if is_virtual_env() is True:
-        data = pyvenv_cfg()
-        print(data["home"])
+    data = get_config()
+    print(data["home"])
+```
+Result:
+```console
+home = /path/to/venv/python/bin
+include-system-site-packages = false
+version = 3.10.14
+prefix = /path/to/venv/dir
+prompt = nameOfYourProject
 ```
 
+Note that virtual environment created with `virtualenv` have more keys and the key `prompt` is not present by default in `venv` created environments.
 
 ## CLI
 ```console
 $ isvirtual
 Yes
 ```
```

### Comparing `isvirtual-1.1.0/pyproject.toml` & `isvirtual-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 [project.urls]
 Homepage = "https://github.com/AlexMili/isVirtual"
 Issues = "https://github.com/AlexMili/isVirtual/issues"
 Repository = "https://github.com/AlexMili/isVirtual"
 Documentation = "https://github.com/AlexMili/isVirtual"
 
 [project.scripts]
-isvirtual = "main:is_virtual_env_cli"
+isvirtual = "main:is_virtual_cli"
 
 [tool.hatch.build.targets.wheel]
 packages = ["./src"]
 
 [tool.hatch.version]
 path = "src/VERSION.md"
 pattern = "(?P<version>.*)"
```

### Comparing `isvirtual-1.1.0/PKG-INFO` & `isvirtual-1.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: isvirtual
-Version: 1.1.0
+Version: 1.2.0
 Summary: Detect if your script is running inside a virtual environment
 Project-URL: Homepage, https://github.com/AlexMili/isVirtual
 Project-URL: Issues, https://github.com/AlexMili/isVirtual/issues
 Project-URL: Repository, https://github.com/AlexMili/isVirtual
 Project-URL: Documentation, https://github.com/AlexMili/isVirtual
 Author: Alex Mili
 License: MIT License
@@ -67,43 +67,53 @@
 
 ## Python
 Simple check:
 ```python
 from isvirtual import is_virtual_env
 
 if __name__ == "__main__":
-    if is_virtual_env() is True:
-        print("You are within a virtual environment")
+    if is_virtual() is True:
+        print("You are within a virtual environment which can either be venv, virtualenv or conda.")
     else:
         print("You are not in a virtual env")
 ```
 
-You can also check if you are specifically in a `venv` or `virtualenv` environment:
+You can also check if you are specifically in a `venv`, `virtualenv` or `conda` environment:
 ```python
 from isvirtual import is_venv, is_virtualenv
 
 if __name__ == "__main__":
     if is_venv() is True:
         print("You are in a venv")
     elif is_virtualenv() is True:
         print("You are in a virtualenv")
+    elif is_conda() is True:
+        print("You are in a conda env")
     else:
-        print("You are not in a virtual env")
+        print("You are not in a any type of virtual env")
 ```
 
-You can also get the info from the env coming from `pyvenv.cfg`. The `sys.prefix` data is added to the original config file:
+You can also get the info from the env coming from `pyvenv.cfg` or load equivalent data from `conda` config. The `sys.prefix` data is added to the original config file under the key `prefix`:
 ```python
-from isvirtual import is_virtual_env, pyvenv_cfg
+from isvirtual import is_virtual_env, get_config
 
 if __name__ == "__main__":
-    if is_virtual_env() is True:
-        data = pyvenv_cfg()
-        print(data["home"])
+    data = get_config()
+    print(data["home"])
+```
+Result:
+```console
+home = /path/to/venv/python/bin
+include-system-site-packages = false
+version = 3.10.14
+prefix = /path/to/venv/dir
+prompt = nameOfYourProject
 ```
 
+Note that virtual environment created with `virtualenv` have more keys and the key `prompt` is not present by default in `venv` created environments.
 
 ## CLI
 ```console
 $ isvirtual
 Yes
 ```
```

