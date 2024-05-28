# Comparing `tmp/factorio_randovania_mod-0.3.0.tar.gz` & `tmp/factorio_randovania_mod-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "factorio_randovania_mod-0.3.0.tar", last modified: Mon May 27 10:16:25 2024, max compression
+gzip compressed data, was "factorio_randovania_mod-0.3.1.tar", last modified: Mon May 27 13:37:45 2024, max compression
```

## Comparing `factorio_randovania_mod-0.3.0.tar` & `factorio_randovania_mod-0.3.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:16:25.545808 factorio_randovania_mod-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:16:25.533808 factorio_randovania_mod-0.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/.github/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:16:25.537808 factorio_randovania_mod-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/.github/workflows/python.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-27 10:16:25.545808 factorio_randovania_mod-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 10:16:25.545808 factorio_randovania_mod-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:16:25.533808 factorio_randovania_mod-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:16:25.537808 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:16:25.537808 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/__pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/__pyinstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/__pyinstaller/hook-factorio_randovania_mod.py
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/color_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/configuration.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7044 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/creator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:16:25.537808 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/files/
--rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/files/schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/locale_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:16:25.541808 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/lua_src/
--rw-r--r--   0 runner    (1001) docker     (127)     5223 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/lua_src/control.lua
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/lua_src/data-updates.lua
--rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/lua_src/data.lua
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:16:25.533808 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/lua_src/graphics/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:16:25.541808 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/lua_src/graphics/icons/
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/lua_src/graphics/icons/nothing.png
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/lua_src/info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:16:25.533808 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/lua_src/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:16:25.541808 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/lua_src/locale/en/
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/lua_src/locale/en/strings.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:16:25.541808 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/lua_src/prototypes/
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/lua_src/prototypes/burners.lua
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/lua_src/prototypes/extra-tiers.lua
--rw-r--r--   0 runner    (1001) docker     (127)     5525 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/lua_src/prototypes/tech.lua
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/lua_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/mod_lua_api.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-27 10:16:25.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:16:25.541808 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-27 10:16:25.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-27 10:16:25.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 10:16:25.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-27 10:16:25.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-27 10:16:25.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-27 10:16:25.000000 factorio_randovania_mod-0.3.0/src/factorio_randovania_mod.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:16:25.541808 factorio_randovania_mod-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/tests/test_color_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/tests/test_creator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:16:25.541808 factorio_randovania_mod-0.3.0/tests/test_files/
--rw-r--r--   0 runner    (1001) docker     (127)   117666 2024-05-27 10:16:20.000000 factorio_randovania_mod-0.3.0/tests/test_files/patcher_a.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:37:45.541919 factorio_randovania_mod-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:37:45.533919 factorio_randovania_mod-0.3.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/.github/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:37:45.533919 factorio_randovania_mod-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/.github/workflows/python.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-27 13:37:45.541919 factorio_randovania_mod-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 13:37:45.541919 factorio_randovania_mod-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:37:45.533919 factorio_randovania_mod-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:37:45.537919 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:37:45.537919 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/__pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/__pyinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/__pyinstaller/hook-factorio_randovania_mod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/color_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/configuration.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7044 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/creator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:37:45.537919 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/files/
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/files/schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/locale_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:37:45.537919 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/lua_src/
+-rw-r--r--   0 runner    (1001) docker     (127)     5223 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/lua_src/control.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/lua_src/data-updates.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/lua_src/data.lua
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:37:45.533919 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/lua_src/graphics/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:37:45.537919 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/lua_src/graphics/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/lua_src/graphics/icons/nothing.png
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/lua_src/info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:37:45.533919 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/lua_src/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:37:45.537919 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/lua_src/locale/en/
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/lua_src/locale/en/strings.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:37:45.541919 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/lua_src/prototypes/
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/lua_src/prototypes/burners.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/lua_src/prototypes/extra-tiers.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     5525 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/lua_src/prototypes/tech.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/lua_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/mod_lua_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-27 13:37:45.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:37:45.541919 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-27 13:37:45.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-27 13:37:45.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 13:37:45.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-27 13:37:45.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-27 13:37:45.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-27 13:37:45.000000 factorio_randovania_mod-0.3.1/src/factorio_randovania_mod.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:37:45.541919 factorio_randovania_mod-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/tests/test_color_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/tests/test_creator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:37:45.541919 factorio_randovania_mod-0.3.1/tests/test_files/
+-rw-r--r--   0 runner    (1001) docker     (127)   117666 2024-05-27 13:37:40.000000 factorio_randovania_mod-0.3.1/tests/test_files/patcher_a.json
```

### Comparing `factorio_randovania_mod-0.3.0/.github/dependabot.yml` & `factorio_randovania_mod-0.3.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.3.0/.github/workflows/python.yml` & `factorio_randovania_mod-0.3.1/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.3.0/.gitignore` & `factorio_randovania_mod-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.3.0/.pre-commit-config.yaml` & `factorio_randovania_mod-0.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.3.0/LICENSE` & `factorio_randovania_mod-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.3.0/PKG-INFO` & `factorio_randovania_mod-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: factorio-randovania-mod
-Version: 0.3.0
+Version: 0.3.1
 Summary: Generator of Factorio Randomizer mods for Randovania
 Author: Henrique Gemignani Passos Lima
 Project-URL: Homepage, https://github.com/randovania/factorio-randovania-mod
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `factorio_randovania_mod-0.3.0/pyproject.toml` & `factorio_randovania_mod-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/cli.py` & `factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/cli.py`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/color_util.py` & `factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/color_util.py`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/configuration.pyi` & `factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/configuration.pyi`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/creator.py` & `factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/creator.py`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/files/schema.json` & `factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/files/schema.json`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/locale_lib.py` & `factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/locale_lib.py`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/lua_src/control.lua` & `factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/lua_src/control.lua`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/lua_src/data-updates.lua` & `factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/lua_src/data-updates.lua`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/lua_src/data.lua` & `factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/lua_src/data.lua`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/lua_src/graphics/icons/nothing.png` & `factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/lua_src/graphics/icons/nothing.png`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/lua_src/locale/en/strings.cfg` & `factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/lua_src/locale/en/strings.cfg`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/lua_src/prototypes/burners.lua` & `factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/lua_src/prototypes/burners.lua`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/lua_src/prototypes/extra-tiers.lua` & `factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/lua_src/prototypes/extra-tiers.lua`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/lua_src/prototypes/tech.lua` & `factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/lua_src/prototypes/tech.lua`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/lua_util.py` & `factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/lua_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     if set(key).issubset(string.ascii_letters + "_"):
         return key
     else:
         return f'["{key}"]'
 
 
 def wrap(data: typing.Any, indent: str = "") -> str:
-    if isinstance(data, list):
+    if isinstance(data, list | tuple):
         return "{" + ", ".join(wrap(item, indent) for item in data) + "}"
 
     if isinstance(data, dict):
         return (
             "{\n"
             + "\n".join(
                 f"{indent}    {_dict_key(key)} = {wrap(value, f'{indent}    ')}," for key, value in data.items()
```

### Comparing `factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/mod_lua_api.py` & `factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/mod_lua_api.py`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.3.0/src/factorio_randovania_mod/schema.py` & `factorio_randovania_mod-0.3.1/src/factorio_randovania_mod/schema.py`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.3.0/src/factorio_randovania_mod.egg-info/PKG-INFO` & `factorio_randovania_mod-0.3.1/src/factorio_randovania_mod.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: factorio-randovania-mod
-Version: 0.3.0
+Version: 0.3.1
 Summary: Generator of Factorio Randomizer mods for Randovania
 Author: Henrique Gemignani Passos Lima
 Project-URL: Homepage, https://github.com/randovania/factorio-randovania-mod
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `factorio_randovania_mod-0.3.0/src/factorio_randovania_mod.egg-info/SOURCES.txt` & `factorio_randovania_mod-0.3.1/src/factorio_randovania_mod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.3.0/tests/test_files/patcher_a.json` & `factorio_randovania_mod-0.3.1/tests/test_files/patcher_a.json`

 * *Files identical despite different names*

