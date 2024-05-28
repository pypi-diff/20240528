# Comparing `tmp/vertagus-0.1.0b6.tar.gz` & `tmp/vertagus-0.1.0b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vertagus-0.1.0b6.tar", last modified: Wed May 22 17:42:07 2024, max compression
+gzip compressed data, was "vertagus-0.1.0b7.tar", last modified: Tue May 28 16:27:39 2024, max compression
```

## Comparing `vertagus-0.1.0b6.tar` & `vertagus-0.1.0b7.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:07.814748 vertagus-0.1.0b6/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1054 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-05-22 17:42:07.814748 vertagus-0.1.0b6/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     3791 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     1100 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 17:42:07.814748 vertagus-0.1.0b6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:07.802748 vertagus-0.1.0b6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:07.806748 vertagus-0.1.0b6/src/vertagus/
--rwxr-xr-x   0 runner    (1001) docker     (127)       73 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:07.806748 vertagus-0.1.0b6/src/vertagus/aliases/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/aliases/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1151 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/aliases/library.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      747 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/aliases/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:07.806748 vertagus-0.1.0b6/src/vertagus/cli/
--rwxr-xr-x   0 runner    (1001) docker     (127)       21 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      358 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:07.806748 vertagus-0.1.0b6/src/vertagus/cli/commands/
--rwxr-xr-x   0 runner    (1001) docker     (127)      108 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/cli/commands/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1199 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/cli/commands/create_aliases.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1188 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/cli/commands/create_tag.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1069 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/cli/commands/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:07.806748 vertagus-0.1.0b6/src/vertagus/configuration/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/configuration/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      682 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/configuration/load.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4485 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/configuration/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:07.810748 vertagus-0.1.0b6/src/vertagus/core/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/core/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      512 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/core/manifest_base.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      770 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/core/package_base.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5961 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/core/project.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      665 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/core/rule_bases.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      648 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/core/scm_base.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1586 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/core/stage.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      270 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/core/tag_base.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2981 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/factory.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1322 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:07.810748 vertagus-0.1.0b6/src/vertagus/providers/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:07.810748 vertagus-0.1.0b6/src/vertagus/providers/manifest/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/providers/manifest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/providers/manifest/json_manifest.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      724 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/providers/manifest/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:07.810748 vertagus-0.1.0b6/src/vertagus/providers/manifest/setuptools_/
--rwxr-xr-x   0 runner    (1001) docker     (127)       59 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/providers/manifest/setuptools_/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      830 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/providers/manifest/setuptools_/pyproject_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/providers/manifest/yaml_manifest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:07.810748 vertagus-0.1.0b6/src/vertagus/providers/scm/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/providers/scm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:07.810748 vertagus-0.1.0b6/src/vertagus/providers/scm/git_/
--rwxr-xr-x   0 runner    (1001) docker     (127)       27 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/providers/scm/git_/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4345 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/providers/scm/git_/git_scm.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      405 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/providers/scm/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:07.810748 vertagus-0.1.0b6/src/vertagus/rules/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/rules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:07.810748 vertagus-0.1.0b6/src/vertagus/rules/comparison/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/rules/comparison/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      908 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/rules/comparison/library.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      732 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/rules/comparison/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:07.810748 vertagus-0.1.0b6/src/vertagus/rules/single_version/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/rules/single_version/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1564 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/rules/single_version/library.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      729 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/rules/single_version/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:07.814748 vertagus-0.1.0b6/src/vertagus/utils/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      588 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/utils/config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      197 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/utils/factory.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      533 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/utils/regex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:07.814748 vertagus-0.1.0b6/src/vertagus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-05-22 17:42:07.000000 vertagus-0.1.0b6/src/vertagus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-22 17:42:07.000000 vertagus-0.1.0b6/src/vertagus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 17:42:07.000000 vertagus-0.1.0b6/src/vertagus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-22 17:42:07.000000 vertagus-0.1.0b6/src/vertagus.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-22 17:42:07.000000 vertagus-0.1.0b6/src/vertagus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 17:42:07.000000 vertagus-0.1.0b6/src/vertagus.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:07.814748 vertagus-0.1.0b6/test/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3650 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/test/test_factory.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1733 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/test/test_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:27:39.217214 vertagus-0.1.0b7/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1054 2024-05-28 16:27:31.000000 vertagus-0.1.0b7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-05-28 16:27:39.217214 vertagus-0.1.0b7/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3791 2024-05-28 16:27:31.000000 vertagus-0.1.0b7/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1100 2024-05-28 16:27:31.000000 vertagus-0.1.0b7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 16:27:39.217214 vertagus-0.1.0b7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:27:39.205214 vertagus-0.1.0b7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:27:39.209214 vertagus-0.1.0b7/src/vertagus/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       73 2024-05-28 16:27:31.000000 vertagus-0.1.0b7/src/vertagus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:27:39.209214 vertagus-0.1.0b7/src/vertagus/aliases/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:27:31.000000 vertagus-0.1.0b7/src/vertagus/aliases/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1151 2024-05-28 16:27:31.000000 vertagus-0.1.0b7/src/vertagus/aliases/library.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      747 2024-05-28 16:27:31.000000 vertagus-0.1.0b7/src/vertagus/aliases/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:27:39.209214 vertagus-0.1.0b7/src/vertagus/cli/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       21 2024-05-28 16:27:31.000000 vertagus-0.1.0b7/src/vertagus/cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      358 2024-05-28 16:27:31.000000 vertagus-0.1.0b7/src/vertagus/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:27:39.209214 vertagus-0.1.0b7/src/vertagus/cli/commands/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      108 2024-05-28 16:27:31.000000 vertagus-0.1.0b7/src/vertagus/cli/commands/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1199 2024-05-28 16:27:31.000000 vertagus-0.1.0b7/src/vertagus/cli/commands/create_aliases.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1188 2024-05-28 16:27:31.000000 vertagus-0.1.0b7/src/vertagus/cli/commands/create_tag.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1069 2024-05-28 16:27:31.000000 vertagus-0.1.0b7/src/vertagus/cli/commands/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:27:39.213214 vertagus-0.1.0b7/src/vertagus/configuration/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:27:31.000000 vertagus-0.1.0b7/src/vertagus/configuration/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      682 2024-05-28 16:27:31.000000 vertagus-0.1.0b7/src/vertagus/configuration/load.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4485 2024-05-28 16:27:31.000000 vertagus-0.1.0b7/src/vertagus/configuration/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:27:39.213214 vertagus-0.1.0b7/src/vertagus/core/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:27:31.000000 vertagus-0.1.0b7/src/vertagus/core/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      512 2024-05-28 16:27:31.000000 vertagus-0.1.0b7/src/vertagus/core/manifest_base.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      770 2024-05-28 16:27:31.000000 vertagus-0.1.0b7/src/vertagus/core/package_base.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6000 2024-05-28 16:27:31.000000 vertagus-0.1.0b7/src/vertagus/core/project.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      714 2024-05-28 16:27:31.000000 vertagus-0.1.0b7/src/vertagus/core/rule_bases.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      648 2024-05-28 16:27:31.000000 vertagus-0.1.0b7/src/vertagus/core/scm_base.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1586 2024-05-28 16:27:31.000000 vertagus-0.1.0b7/src/vertagus/core/stage.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      270 2024-05-28 16:27:31.000000 vertagus-0.1.0b7/src/vertagus/core/tag_base.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2981 2024-05-28 16:27:31.000000 vertagus-0.1.0b7/src/vertagus/factory.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1322 2024-05-28 16:27:31.000000 vertagus-0.1.0b7/src/vertagus/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:27:39.213214 vertagus-0.1.0b7/src/vertagus/providers/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:27:31.000000 vertagus-0.1.0b7/src/vertagus/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:27:39.213214 vertagus-0.1.0b7/src/vertagus/providers/manifest/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:27:31.000000 vertagus-0.1.0b7/src/vertagus/providers/manifest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-28 16:27:31.000000 vertagus-0.1.0b7/src/vertagus/providers/manifest/json_manifest.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      724 2024-05-28 16:27:31.000000 vertagus-0.1.0b7/src/vertagus/providers/manifest/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:27:39.213214 vertagus-0.1.0b7/src/vertagus/providers/manifest/setuptools_/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       59 2024-05-28 16:27:31.000000 vertagus-0.1.0b7/src/vertagus/providers/manifest/setuptools_/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      830 2024-05-28 16:27:31.000000 vertagus-0.1.0b7/src/vertagus/providers/manifest/setuptools_/pyproject_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-28 16:27:31.000000 vertagus-0.1.0b7/src/vertagus/providers/manifest/yaml_manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:27:39.213214 vertagus-0.1.0b7/src/vertagus/providers/scm/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:27:31.000000 vertagus-0.1.0b7/src/vertagus/providers/scm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:27:39.213214 vertagus-0.1.0b7/src/vertagus/providers/scm/git_/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       27 2024-05-28 16:27:31.000000 vertagus-0.1.0b7/src/vertagus/providers/scm/git_/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4345 2024-05-28 16:27:31.000000 vertagus-0.1.0b7/src/vertagus/providers/scm/git_/git_scm.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      405 2024-05-28 16:27:31.000000 vertagus-0.1.0b7/src/vertagus/providers/scm/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:27:39.213214 vertagus-0.1.0b7/src/vertagus/rules/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:27:31.000000 vertagus-0.1.0b7/src/vertagus/rules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:27:39.217214 vertagus-0.1.0b7/src/vertagus/rules/comparison/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:27:31.000000 vertagus-0.1.0b7/src/vertagus/rules/comparison/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1037 2024-05-28 16:27:31.000000 vertagus-0.1.0b7/src/vertagus/rules/comparison/library.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      732 2024-05-28 16:27:31.000000 vertagus-0.1.0b7/src/vertagus/rules/comparison/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:27:39.217214 vertagus-0.1.0b7/src/vertagus/rules/single_version/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:27:31.000000 vertagus-0.1.0b7/src/vertagus/rules/single_version/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1868 2024-05-28 16:27:31.000000 vertagus-0.1.0b7/src/vertagus/rules/single_version/library.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      729 2024-05-28 16:27:31.000000 vertagus-0.1.0b7/src/vertagus/rules/single_version/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:27:39.217214 vertagus-0.1.0b7/src/vertagus/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:27:31.000000 vertagus-0.1.0b7/src/vertagus/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      588 2024-05-28 16:27:31.000000 vertagus-0.1.0b7/src/vertagus/utils/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      197 2024-05-28 16:27:31.000000 vertagus-0.1.0b7/src/vertagus/utils/factory.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      533 2024-05-28 16:27:31.000000 vertagus-0.1.0b7/src/vertagus/utils/regex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:27:39.217214 vertagus-0.1.0b7/src/vertagus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-05-28 16:27:39.000000 vertagus-0.1.0b7/src/vertagus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-28 16:27:39.000000 vertagus-0.1.0b7/src/vertagus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 16:27:39.000000 vertagus-0.1.0b7/src/vertagus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-28 16:27:39.000000 vertagus-0.1.0b7/src/vertagus.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-28 16:27:39.000000 vertagus-0.1.0b7/src/vertagus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-28 16:27:39.000000 vertagus-0.1.0b7/src/vertagus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:27:39.217214 vertagus-0.1.0b7/test/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3650 2024-05-28 16:27:31.000000 vertagus-0.1.0b7/test/test_factory.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1733 2024-05-28 16:27:31.000000 vertagus-0.1.0b7/test/test_operations.py
```

### Comparing `vertagus-0.1.0b6/LICENSE` & `vertagus-0.1.0b7/LICENSE`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b6/PKG-INFO` & `vertagus-0.1.0b7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vertagus
-Version: 0.1.0b6
+Version: 0.1.0b7
 Summary: A tool to assist the maintenance of package versioning with scm tags
 Author-email: John Raines <johndanielraines@gmail.com>
 License: Copyright (c) 2024 John Raines
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `vertagus-0.1.0b6/README.md` & `vertagus-0.1.0b7/README.md`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b6/pyproject.toml` & `vertagus-0.1.0b7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vertagus"
-version = "0.1.0b6"
+version = "0.1.0b7"
 description = "A tool to assist the maintenance of package versioning with scm tags"
 readme = "README.md"
 authors = [
     {"name" = "John Raines", "email" = "johndanielraines@gmail.com"}
 ]
 dependencies = [
     "click",
```

### Comparing `vertagus-0.1.0b6/src/vertagus/aliases/library.py` & `vertagus-0.1.0b7/src/vertagus/aliases/library.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b6/src/vertagus/aliases/loader.py` & `vertagus-0.1.0b7/src/vertagus/aliases/loader.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b6/src/vertagus/cli/commands/create_aliases.py` & `vertagus-0.1.0b7/src/vertagus/cli/commands/create_aliases.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b6/src/vertagus/cli/commands/create_tag.py` & `vertagus-0.1.0b7/src/vertagus/cli/commands/create_tag.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b6/src/vertagus/cli/commands/validate.py` & `vertagus-0.1.0b7/src/vertagus/cli/commands/validate.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b6/src/vertagus/configuration/load.py` & `vertagus-0.1.0b7/src/vertagus/configuration/load.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b6/src/vertagus/configuration/types.py` & `vertagus-0.1.0b7/src/vertagus/configuration/types.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b6/src/vertagus/core/manifest_base.py` & `vertagus-0.1.0b7/src/vertagus/core/manifest_base.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b6/src/vertagus/core/package_base.py` & `vertagus-0.1.0b7/src/vertagus/core/package_base.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b6/src/vertagus/core/project.py` & `vertagus-0.1.0b7/src/vertagus/core/project.py`

 * *Files 10% similar despite different names*

```diff
@@ -60,35 +60,35 @@
     def _get_version_aliases(self, version: str) -> list[AliasBase]:
         return [alias(version) for alias in self.aliases]
 
     def _run_current_version_rules(self, current_version, stage_name=None):
         validated = True
         for rule in self._get_current_version_rules(stage_name):
             logger.info(
-                f"Validating {rule.__name__} for {current_version}"
+                f"Validating rule {rule.name!r} for {current_version}"
             )
             validated = rule.validate_version(current_version)
             if not validated:
                 logger.error(
-                    f"Validation failed for {rule.__name__}"
+                    f"Validation failed for rule {rule.name!r}: {rule.description}"
                 )
                 return validated
         return validated
 
     def _run_version_increment_rules(self, previous_version, current_version, stage_name=None):
         validated = True
         versions = [previous_version, current_version]
         for rule in self._get_version_increment_rules(stage_name):
             logger.info(
-                f"Validating {rule.__class__.__name__} for {versions}"
+                f"Validating rule {rule.name!r} for {versions}"
             )
             validated = rule.validate_comparison(versions)
             if not validated:
                 logger.error(
-                    f"Validation failed for {rule.__class__.__name__}"
+                    f"Validation failed for rule  {rule.name!r}: {rule.description}"
                 )
                 return validated
         return validated
 
     def _run_manifest_versions_comparison_rules(self, stage_name=None):
         validated = True
         for rule in self._get_manifest_versions_comparison_rules(stage_name):
@@ -99,20 +99,20 @@
                 self._get_manifests(stage_name)
                 if m.name in rule.manifest_names
             ]
             if not manifests:
                 raise ValueError(f"Manifests {rule.manifest_names} not found.")
             versions = [m.version for m in manifests]
             logger.info(
-                f"Validating {rule.__class__.__name__} for {versions}"
+                f"Validating rule {rule.name!r} for {versions}"
             )
             validated = rule.validate_comparison(versions)
             if not validated:
                 logger.error(
-                    f"Validation failed for {rule.__class__.__name__}"
+                    f"Validation failed for rule {rule.name!r}: {rule.description}"
                 )
                 return validated
         return validated
 
     def _get_manifests(self, stage_name=None):
         manifests = self._manifests.copy()
         if stage_name:
```

### Comparing `vertagus-0.1.0b6/src/vertagus/core/scm_base.py` & `vertagus-0.1.0b7/src/vertagus/core/scm_base.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b6/src/vertagus/core/stage.py` & `vertagus-0.1.0b7/src/vertagus/core/stage.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b6/src/vertagus/factory.py` & `vertagus-0.1.0b7/src/vertagus/factory.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b6/src/vertagus/operations.py` & `vertagus-0.1.0b7/src/vertagus/operations.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b6/src/vertagus/providers/manifest/json_manifest.py` & `vertagus-0.1.0b7/src/vertagus/providers/manifest/json_manifest.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b6/src/vertagus/providers/manifest/registry.py` & `vertagus-0.1.0b7/src/vertagus/providers/manifest/registry.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b6/src/vertagus/providers/manifest/setuptools_/pyproject_manifest.py` & `vertagus-0.1.0b7/src/vertagus/providers/manifest/setuptools_/pyproject_manifest.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b6/src/vertagus/providers/manifest/yaml_manifest.py` & `vertagus-0.1.0b7/src/vertagus/providers/manifest/yaml_manifest.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b6/src/vertagus/providers/scm/git_/git_scm.py` & `vertagus-0.1.0b7/src/vertagus/providers/scm/git_/git_scm.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b6/src/vertagus/rules/comparison/library.py` & `vertagus-0.1.0b7/src/vertagus/rules/comparison/library.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from packaging import version
 from vertagus.core.rule_bases import VersionComparisonRule
 
 
 class Increasing(VersionComparisonRule):
     name = "any_increment"
+    description = "Version must be greater than the previous one."
 
     def validate_comparison(self, versions: tuple[str, str]):
         version1, version2 = versions
         if not version1 and bool(version2):
             return True
         return version.parse(version1) < version.parse(version2)
 
 
 class ManifestsComparisonRule(VersionComparisonRule):
     name = "manifests_comparison"
+    description = "All manifests must have the same version."
 
     def __init__(self, config: dict):
         self.manifest_names = config["manifests"]
 
     def validate_comparison(self, versions: tuple[str, str]):
         if not versions:
             raise ValueError("No versions to compare.")
```

### Comparing `vertagus-0.1.0b6/src/vertagus/rules/comparison/loader.py` & `vertagus-0.1.0b7/src/vertagus/rules/comparison/loader.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b6/src/vertagus/rules/single_version/library.py` & `vertagus-0.1.0b7/src/vertagus/rules/single_version/library.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,37 @@
 import re
 from vertagus.core.rule_bases import SingleVersionRule
 from vertagus.utils import regex as regex_utils
 
 
+class classproperty(object):
+
+    def __init__(self, f):
+        self.f = f
+    
+    def __get__(self, obj, owner):
+        return self.f(owner)
+
+
 class NotEmpty(SingleVersionRule):
     name = "not_empty"
+    description = "Version must not be empty."
 
     @classmethod
     def validate_version(cls, version):
         return bool(version)
     
 
 class RegexRuleBase(SingleVersionRule):
     pattern: str = ""
 
+    @classproperty
+    def description(cls):
+        return f"Version must match the pattern: {cls.pattern}"
+
     @classmethod
     def validate_version(cls, version):
         return bool(re.match(cls.pattern, version))
 
 
 # Major-Minor-Patch Regex Rules
```

### Comparing `vertagus-0.1.0b6/src/vertagus/rules/single_version/loader.py` & `vertagus-0.1.0b7/src/vertagus/rules/single_version/loader.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b6/src/vertagus/utils/config.py` & `vertagus-0.1.0b7/src/vertagus/utils/config.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b6/src/vertagus/utils/regex.py` & `vertagus-0.1.0b7/src/vertagus/utils/regex.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b6/src/vertagus.egg-info/PKG-INFO` & `vertagus-0.1.0b7/src/vertagus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vertagus
-Version: 0.1.0b6
+Version: 0.1.0b7
 Summary: A tool to assist the maintenance of package versioning with scm tags
 Author-email: John Raines <johndanielraines@gmail.com>
 License: Copyright (c) 2024 John Raines
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `vertagus-0.1.0b6/src/vertagus.egg-info/SOURCES.txt` & `vertagus-0.1.0b7/src/vertagus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b6/test/test_factory.py` & `vertagus-0.1.0b7/test/test_factory.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b6/test/test_operations.py` & `vertagus-0.1.0b7/test/test_operations.py`

 * *Files identical despite different names*

