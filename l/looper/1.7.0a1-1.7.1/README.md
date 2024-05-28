# Comparing `tmp/looper-1.7.0a1.tar.gz` & `tmp/looper-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "looper-1.7.0a1.tar", last modified: Mon Jan 22 14:17:30 2024, max compression
+gzip compressed data, was "looper-1.7.1.tar", last modified: Tue May 28 16:17:49 2024, max compression
```

## Comparing `looper-1.7.0a1.tar` & `looper-1.7.1.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:17:30.981600 looper-1.7.0a1/
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-01-22 14:17:23.000000 looper-1.7.0a1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-01-22 14:17:23.000000 looper-1.7.0a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-01-22 14:17:30.981600 looper-1.7.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-01-22 14:17:23.000000 looper-1.7.0a1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5796 2024-01-22 14:17:23.000000 looper-1.7.0a1/logo_looper.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:17:30.973600 looper-1.7.0a1/looper/
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5907 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/cli_divvy.py
--rw-r--r--   0 runner    (1001) docker     (127)    26092 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/cli_looper.py
--rw-r--r--   0 runner    (1001) docker     (127)    30231 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/conductor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8558 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:17:30.973600 looper-1.7.0a1/looper/default_config/
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/default_config/divvy_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:17:30.977600 looper-1.7.0a1/looper/default_config/divvy_templates/
--rwxr-xr-x   0 runner    (1001) docker     (127)      164 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/default_config/divvy_templates/localhost_bulker_template.sub
--rwxr-xr-x   0 runner    (1001) docker     (127)      183 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/default_config/divvy_templates/localhost_docker_template.sub
--rwxr-xr-x   0 runner    (1001) docker     (127)      260 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/default_config/divvy_templates/localhost_singularity_template.sub
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/default_config/divvy_templates/localhost_template.sub
--rwxr-xr-x   0 runner    (1001) docker     (127)       84 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/default_config/divvy_templates/lsf_template.sub
--rwxr-xr-x   0 runner    (1001) docker     (127)      134 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/default_config/divvy_templates/sge_template.sub
--rwxr-xr-x   0 runner    (1001) docker     (127)      478 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/default_config/divvy_templates/slurm_singularity_template.sub
--rwxr-xr-x   0 runner    (1001) docker     (127)      304 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/default_config/divvy_templates/slurm_template.sub
--rw-r--r--   0 runner    (1001) docker     (127)    15688 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/divvy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:17:30.977600 looper-1.7.0a1/looper/jinja_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/jinja_templates/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/jinja_templates/footer_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/jinja_templates/head.html
--rw-r--r--   0 runner    (1001) docker     (127)    10794 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/jinja_templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     7843 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/jinja_templates/logo.html
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/jinja_templates/navbar.html
--rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/jinja_templates/navbar_links.html
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/jinja_templates/navbar_list_parent.html
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/jinja_templates/object.html
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/jinja_templates/project_object.html
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/jinja_templates/sample.html
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/jinja_templates/status.html
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/jinja_templates/status_table.html
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/jinja_templates/status_table_no_links.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:17:30.981600 looper-1.7.0a1/looper/jinja_templates_old/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/jinja_templates_old/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/jinja_templates_old/footer_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/jinja_templates_old/head.html
--rw-r--r--   0 runner    (1001) docker     (127)     8959 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/jinja_templates_old/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     7843 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/jinja_templates_old/logo.html
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/jinja_templates_old/navbar.html
--rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/jinja_templates_old/navbar_links.html
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/jinja_templates_old/navbar_list_parent.html
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/jinja_templates_old/object.html
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/jinja_templates_old/project_object.html
--rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/jinja_templates_old/sample.html
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/jinja_templates_old/status.html
--rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/jinja_templates_old/status_table.html
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/jinja_templates_old/status_table_no_links.html
--rwxr-xr-x   0 runner    (1001) docker     (127)    30407 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/looper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/parser_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    14974 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/pipeline_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     5747 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/processed_project.py
--rw-r--r--   0 runner    (1001) docker     (127)    36171 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/project.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:17:30.981600 looper-1.7.0a1/looper/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/schemas/divvy_config_schema.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/schemas/pipeline_interface_schema_generic.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/schemas/pipeline_interface_schema_project.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/schemas/pipeline_interface_schema_sample.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    27257 2024-01-22 14:17:23.000000 looper-1.7.0a1/looper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:17:30.981600 looper-1.7.0a1/looper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-01-22 14:17:30.000000 looper-1.7.0a1/looper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-01-22 14:17:30.000000 looper-1.7.0a1/looper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-22 14:17:30.000000 looper-1.7.0a1/looper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-01-22 14:17:30.000000 looper-1.7.0a1/looper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-01-22 14:17:30.000000 looper-1.7.0a1/looper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-22 14:17:30.000000 looper-1.7.0a1/looper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:17:30.981600 looper-1.7.0a1/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-01-22 14:17:23.000000 looper-1.7.0a1/requirements/requirements-all.txt
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-01-22 14:17:23.000000 looper-1.7.0a1/requirements/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-01-22 14:17:23.000000 looper-1.7.0a1/requirements/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-01-22 14:17:30.981600 looper-1.7.0a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-01-22 14:17:23.000000 looper-1.7.0a1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:17:30.981600 looper-1.7.0a1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-01-22 14:17:23.000000 looper-1.7.0a1/tests/test_clean.py
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-01-22 14:17:23.000000 looper-1.7.0a1/tests/test_desired_sample_range.py
--rw-r--r--   0 runner    (1001) docker     (127)     6934 2024-01-22 14:17:23.000000 looper-1.7.0a1/tests/test_natural_range.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:17:49.873745 looper-1.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-28 16:17:37.000000 looper-1.7.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-28 16:17:37.000000 looper-1.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-28 16:17:49.869745 looper-1.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-28 16:17:37.000000 looper-1.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5796 2024-05-28 16:17:37.000000 looper-1.7.1/logo_looper.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:17:49.861745 looper-1.7.1/looper/
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-28 16:17:37.000000 looper-1.7.1/looper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-28 16:17:37.000000 looper-1.7.1/looper/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-28 16:17:37.000000 looper-1.7.1/looper/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5907 2024-05-28 16:17:37.000000 looper-1.7.1/looper/cli_divvy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26367 2024-05-28 16:17:37.000000 looper-1.7.1/looper/cli_looper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30777 2024-05-28 16:17:37.000000 looper-1.7.1/looper/conductor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8558 2024-05-28 16:17:37.000000 looper-1.7.1/looper/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:17:49.861745 looper-1.7.1/looper/default_config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-28 16:17:37.000000 looper-1.7.1/looper/default_config/divvy_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:17:49.865745 looper-1.7.1/looper/default_config/divvy_templates/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      164 2024-05-28 16:17:37.000000 looper-1.7.1/looper/default_config/divvy_templates/localhost_bulker_template.sub
+-rwxr-xr-x   0 runner    (1001) docker     (127)      183 2024-05-28 16:17:37.000000 looper-1.7.1/looper/default_config/divvy_templates/localhost_docker_template.sub
+-rwxr-xr-x   0 runner    (1001) docker     (127)      260 2024-05-28 16:17:37.000000 looper-1.7.1/looper/default_config/divvy_templates/localhost_singularity_template.sub
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-28 16:17:37.000000 looper-1.7.1/looper/default_config/divvy_templates/localhost_template.sub
+-rwxr-xr-x   0 runner    (1001) docker     (127)       84 2024-05-28 16:17:37.000000 looper-1.7.1/looper/default_config/divvy_templates/lsf_template.sub
+-rwxr-xr-x   0 runner    (1001) docker     (127)      134 2024-05-28 16:17:37.000000 looper-1.7.1/looper/default_config/divvy_templates/sge_template.sub
+-rwxr-xr-x   0 runner    (1001) docker     (127)      478 2024-05-28 16:17:37.000000 looper-1.7.1/looper/default_config/divvy_templates/slurm_singularity_template.sub
+-rwxr-xr-x   0 runner    (1001) docker     (127)      304 2024-05-28 16:17:37.000000 looper-1.7.1/looper/default_config/divvy_templates/slurm_template.sub
+-rw-r--r--   0 runner    (1001) docker     (127)    15688 2024-05-28 16:17:37.000000 looper-1.7.1/looper/divvy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-05-28 16:17:37.000000 looper-1.7.1/looper/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:17:49.865745 looper-1.7.1/looper/jinja_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-28 16:17:37.000000 looper-1.7.1/looper/jinja_templates/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-05-28 16:17:37.000000 looper-1.7.1/looper/jinja_templates/footer_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-05-28 16:17:37.000000 looper-1.7.1/looper/jinja_templates/head.html
+-rw-r--r--   0 runner    (1001) docker     (127)    10794 2024-05-28 16:17:37.000000 looper-1.7.1/looper/jinja_templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7843 2024-05-28 16:17:37.000000 looper-1.7.1/looper/jinja_templates/logo.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-28 16:17:37.000000 looper-1.7.1/looper/jinja_templates/navbar.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-05-28 16:17:37.000000 looper-1.7.1/looper/jinja_templates/navbar_links.html
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-28 16:17:37.000000 looper-1.7.1/looper/jinja_templates/navbar_list_parent.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-28 16:17:37.000000 looper-1.7.1/looper/jinja_templates/object.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-28 16:17:37.000000 looper-1.7.1/looper/jinja_templates/project_object.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-05-28 16:17:37.000000 looper-1.7.1/looper/jinja_templates/sample.html
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-28 16:17:37.000000 looper-1.7.1/looper/jinja_templates/status.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-05-28 16:17:37.000000 looper-1.7.1/looper/jinja_templates/status_table.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-05-28 16:17:37.000000 looper-1.7.1/looper/jinja_templates/status_table_no_links.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:17:49.869745 looper-1.7.1/looper/jinja_templates_old/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-28 16:17:37.000000 looper-1.7.1/looper/jinja_templates_old/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-28 16:17:37.000000 looper-1.7.1/looper/jinja_templates_old/footer_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-05-28 16:17:37.000000 looper-1.7.1/looper/jinja_templates_old/head.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8959 2024-05-28 16:17:37.000000 looper-1.7.1/looper/jinja_templates_old/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7843 2024-05-28 16:17:37.000000 looper-1.7.1/looper/jinja_templates_old/logo.html
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-28 16:17:37.000000 looper-1.7.1/looper/jinja_templates_old/navbar.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-05-28 16:17:37.000000 looper-1.7.1/looper/jinja_templates_old/navbar_links.html
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-28 16:17:37.000000 looper-1.7.1/looper/jinja_templates_old/navbar_list_parent.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-28 16:17:37.000000 looper-1.7.1/looper/jinja_templates_old/object.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-28 16:17:37.000000 looper-1.7.1/looper/jinja_templates_old/project_object.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-05-28 16:17:37.000000 looper-1.7.1/looper/jinja_templates_old/sample.html
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-28 16:17:37.000000 looper-1.7.1/looper/jinja_templates_old/status.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-05-28 16:17:37.000000 looper-1.7.1/looper/jinja_templates_old/status_table.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-05-28 16:17:37.000000 looper-1.7.1/looper/jinja_templates_old/status_table_no_links.html
+-rwxr-xr-x   0 runner    (1001) docker     (127)    30448 2024-05-28 16:17:37.000000 looper-1.7.1/looper/looper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-05-28 16:17:37.000000 looper-1.7.1/looper/parser_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14974 2024-05-28 16:17:37.000000 looper-1.7.1/looper/pipeline_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5747 2024-05-28 16:17:37.000000 looper-1.7.1/looper/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-05-28 16:17:37.000000 looper-1.7.1/looper/processed_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36171 2024-05-28 16:17:37.000000 looper-1.7.1/looper/project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:17:49.869745 looper-1.7.1/looper/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-28 16:17:37.000000 looper-1.7.1/looper/schemas/divvy_config_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-28 16:17:37.000000 looper-1.7.1/looper/schemas/pipeline_interface_schema_generic.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-28 16:17:37.000000 looper-1.7.1/looper/schemas/pipeline_interface_schema_project.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-28 16:17:37.000000 looper-1.7.1/looper/schemas/pipeline_interface_schema_sample.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    27257 2024-05-28 16:17:37.000000 looper-1.7.1/looper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:17:49.869745 looper-1.7.1/looper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-28 16:17:49.000000 looper-1.7.1/looper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-05-28 16:17:49.000000 looper-1.7.1/looper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 16:17:49.000000 looper-1.7.1/looper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-28 16:17:49.000000 looper-1.7.1/looper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-28 16:17:49.000000 looper-1.7.1/looper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-28 16:17:49.000000 looper-1.7.1/looper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:17:49.869745 looper-1.7.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-28 16:17:37.000000 looper-1.7.1/requirements/requirements-all.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-28 16:17:37.000000 looper-1.7.1/requirements/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-28 16:17:37.000000 looper-1.7.1/requirements/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-28 16:17:49.873745 looper-1.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-05-28 16:17:37.000000 looper-1.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:17:49.869745 looper-1.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-28 16:17:37.000000 looper-1.7.1/tests/test_clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-28 16:17:37.000000 looper-1.7.1/tests/test_desired_sample_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6934 2024-05-28 16:17:37.000000 looper-1.7.1/tests/test_natural_range.py
```

### Comparing `looper-1.7.0a1/LICENSE.txt` & `looper-1.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `looper-1.7.0a1/PKG-INFO` & `looper-1.7.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: looper
-Version: 1.7.0a1
+Version: 1.7.1
 Summary: A pipeline submission engine that parses sample inputs and submits pipelines for each sample.
 Home-page: https://github.com/pepkit/looper
 Author: Nathan Sheffield, Vince Reuter, Michal Stolarczyk, Johanna Klughammer, Andre Rendeiro
 License: BSD2
 Keywords: bioinformatics,sequencing,ngs
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
@@ -19,15 +19,15 @@
 Requires-Dist: divvy>=0.5.0
 Requires-Dist: eido>=0.2.1
 Requires-Dist: jinja2
 Requires-Dist: logmuse>=0.2.0
 Requires-Dist: pandas>=2.0.2
 Requires-Dist: pephubclient>=0.1.2
 Requires-Dist: peppy>=0.40.0
-Requires-Dist: pipestat>=0.7.1a1
+Requires-Dist: pipestat<0.9.0,>=0.8.0
 Requires-Dist: pyyaml>=3.12
 Requires-Dist: rich>=9.10.0
 Requires-Dist: ubiquerg>=0.5.2
 Requires-Dist: yacman>=0.9.2
 
 # <img src="docs/img/looper_logo.svg" alt="looper logo" height="70">
```

### Comparing `looper-1.7.0a1/README.md` & `looper-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `looper-1.7.0a1/logo_looper.svg` & `looper-1.7.1/logo_looper.svg`

 * *Files identical despite different names*

### Comparing `looper-1.7.0a1/looper/__init__.py` & `looper-1.7.1/looper/__init__.py`

 * *Files identical despite different names*

### Comparing `looper-1.7.0a1/looper/cli_divvy.py` & `looper-1.7.1/looper/cli_divvy.py`

 * *Files identical despite different names*

### Comparing `looper-1.7.0a1/looper/cli_looper.py` & `looper-1.7.1/looper/cli_looper.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,27 +215,35 @@
                 nargs="+",
                 help="List of key-value pairs (k1=v1)",
             )
 
         for subparser in [run_subparser, rerun_subparser]:
             subparser.add_argument(
                 "-u",
-                "--lump",
+                "--lump-s",
                 default=None,
                 metavar="X",
                 type=html_range(min_val=0, max_val=100, step=0.1, value=0),
-                help="Total input file size (GB) to batch into one job",
+                help="Lump by size: total input file size (GB) to batch into one job",
             )
             subparser.add_argument(
                 "-n",
-                "--lumpn",
+                "--lump-n",
                 default=None,
                 metavar="N",
                 type=html_range(min_val=1, max_val="num_samples", value=1),
-                help="Number of commands to batch into one job",
+                help="Lump by number: number of samples to batch into one job",
+            )
+            subparser.add_argument(
+                "-j",
+                "--lump-j",
+                default=None,
+                metavar="J",
+                type=int,
+                help="Lump samples into number of jobs.",
             )
 
         check_subparser.add_argument(
             "--describe-codes",
             help="Show status codes description",
             action="store_true",
             default=False,
```

### Comparing `looper-1.7.0a1/looper/conductor.py` & `looper-1.7.1/looper/conductor.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import importlib
 import logging
 import os
 import subprocess
 import time
 import yaml
+from math import ceil
 from copy import copy, deepcopy
 from json import loads
 from subprocess import check_output
 from typing import *
 
 from eido import read_schema, get_input_files_size
 from eido.const import INPUT_FILE_SIZE_KEY, MISSING_KEY
@@ -128,14 +129,15 @@
         delay=0,
         extra_args=None,
         extra_args_override=None,
         ignore_flags=False,
         compute_variables=None,
         max_cmds=None,
         max_size=None,
+        max_jobs=None,
         automatic=True,
         collate=False,
     ):
         """
         Create a job submission manager.
 
         The most critical inputs are the pipeline interface and the pipeline
@@ -162,14 +164,16 @@
         :param dict[str] compute_variables: A dict with variables that will be made
             available to the compute package. For example, this should include
             the name of the cluster partition to which job or jobs will be submitted
         :param int | NoneType max_cmds: Upper bound on number of commands to
             include in a single job script.
         :param int | float | NoneType max_size: Upper bound on total file
             size of inputs used by the commands lumped into single job script.
+        :param int | float | NoneType max_jobs: Upper bound on total number of jobs to
+            group samples for submission.
         :param bool automatic: Whether the submission should be automatic once
             the pool reaches capacity.
         :param bool collate: Whether a collate job is to be submitted (runs on
             the project level, rather that on the sample level)
         """
         super(SubmissionConductor, self).__init__()
         self.collate = collate
@@ -196,14 +200,24 @@
 
         if self.extra_pipe_args:
             _LOGGER.debug(
                 "String appended to every pipeline command: "
                 "{}".format(self.extra_pipe_args)
             )
 
+        if max_jobs:
+            if max_jobs == 0 or max_jobs < 0:
+                raise ValueError(
+                    "If specified, max job command count must be a positive integer, greater than zero."
+                )
+
+            num_samples = len(self.prj.samples)
+            samples_per_job = num_samples / max_jobs
+            max_cmds = ceil(samples_per_job)
+
         if not self.collate:
             self.automatic = automatic
             if max_cmds is None and max_size is None:
                 self.max_cmds = 1
             elif (max_cmds is not None and max_cmds < 1) or (
                 max_size is not None and max_size < 0
             ):
```

### Comparing `looper-1.7.0a1/looper/const.py` & `looper-1.7.1/looper/const.py`

 * *Files identical despite different names*

### Comparing `looper-1.7.0a1/looper/default_config/divvy_config.yaml` & `looper-1.7.1/looper/default_config/divvy_config.yaml`

 * *Files identical despite different names*

### Comparing `looper-1.7.0a1/looper/divvy.py` & `looper-1.7.1/looper/divvy.py`

 * *Files identical despite different names*

### Comparing `looper-1.7.0a1/looper/exceptions.py` & `looper-1.7.1/looper/exceptions.py`

 * *Files identical despite different names*

### Comparing `looper-1.7.0a1/looper/jinja_templates/footer_index.html` & `looper-1.7.1/looper/jinja_templates/footer_index.html`

 * *Files identical despite different names*

### Comparing `looper-1.7.0a1/looper/jinja_templates/head.html` & `looper-1.7.1/looper/jinja_templates/head.html`

 * *Files identical despite different names*

### Comparing `looper-1.7.0a1/looper/jinja_templates/index.html` & `looper-1.7.1/looper/jinja_templates/index.html`

 * *Files identical despite different names*

### Comparing `looper-1.7.0a1/looper/jinja_templates/logo.html` & `looper-1.7.1/looper/jinja_templates/logo.html`

 * *Files identical despite different names*

### Comparing `looper-1.7.0a1/looper/jinja_templates/navbar.html` & `looper-1.7.1/looper/jinja_templates/navbar.html`

 * *Files identical despite different names*

### Comparing `looper-1.7.0a1/looper/jinja_templates/navbar_links.html` & `looper-1.7.1/looper/jinja_templates/navbar_links.html`

 * *Files identical despite different names*

### Comparing `looper-1.7.0a1/looper/jinja_templates/navbar_list_parent.html` & `looper-1.7.1/looper/jinja_templates/navbar_list_parent.html`

 * *Files identical despite different names*

### Comparing `looper-1.7.0a1/looper/jinja_templates/object.html` & `looper-1.7.1/looper/jinja_templates/object.html`

 * *Files identical despite different names*

### Comparing `looper-1.7.0a1/looper/jinja_templates/project_object.html` & `looper-1.7.1/looper/jinja_templates/project_object.html`

 * *Files identical despite different names*

### Comparing `looper-1.7.0a1/looper/jinja_templates/sample.html` & `looper-1.7.1/looper/jinja_templates/sample.html`

 * *Files identical despite different names*

### Comparing `looper-1.7.0a1/looper/jinja_templates/status_table.html` & `looper-1.7.1/looper/jinja_templates/status_table.html`

 * *Files identical despite different names*

### Comparing `looper-1.7.0a1/looper/jinja_templates/status_table_no_links.html` & `looper-1.7.1/looper/jinja_templates/status_table_no_links.html`

 * *Files identical despite different names*

### Comparing `looper-1.7.0a1/looper/jinja_templates_old/footer_index.html` & `looper-1.7.1/looper/jinja_templates_old/footer_index.html`

 * *Files identical despite different names*

### Comparing `looper-1.7.0a1/looper/jinja_templates_old/head.html` & `looper-1.7.1/looper/jinja_templates_old/head.html`

 * *Files identical despite different names*

### Comparing `looper-1.7.0a1/looper/jinja_templates_old/index.html` & `looper-1.7.1/looper/jinja_templates_old/index.html`

 * *Files identical despite different names*

### Comparing `looper-1.7.0a1/looper/jinja_templates_old/logo.html` & `looper-1.7.1/looper/jinja_templates_old/logo.html`

 * *Files identical despite different names*

### Comparing `looper-1.7.0a1/looper/jinja_templates_old/navbar.html` & `looper-1.7.1/looper/jinja_templates_old/navbar.html`

 * *Files identical despite different names*

### Comparing `looper-1.7.0a1/looper/jinja_templates_old/navbar_links.html` & `looper-1.7.1/looper/jinja_templates_old/navbar_links.html`

 * *Files identical despite different names*

### Comparing `looper-1.7.0a1/looper/jinja_templates_old/navbar_list_parent.html` & `looper-1.7.1/looper/jinja_templates_old/navbar_list_parent.html`

 * *Files identical despite different names*

### Comparing `looper-1.7.0a1/looper/jinja_templates_old/object.html` & `looper-1.7.1/looper/jinja_templates_old/object.html`

 * *Files identical despite different names*

### Comparing `looper-1.7.0a1/looper/jinja_templates_old/project_object.html` & `looper-1.7.1/looper/jinja_templates_old/project_object.html`

 * *Files identical despite different names*

### Comparing `looper-1.7.0a1/looper/jinja_templates_old/sample.html` & `looper-1.7.1/looper/jinja_templates_old/sample.html`

 * *Files identical despite different names*

### Comparing `looper-1.7.0a1/looper/jinja_templates_old/status_table.html` & `looper-1.7.1/looper/jinja_templates_old/status_table.html`

 * *Files identical despite different names*

### Comparing `looper-1.7.0a1/looper/jinja_templates_old/status_table_no_links.html` & `looper-1.7.1/looper/jinja_templates_old/status_table_no_links.html`

 * *Files identical despite different names*

### Comparing `looper-1.7.0a1/looper/looper.py` & `looper-1.7.1/looper/looper.py`

 * *Files 1% similar despite different names*

```diff
@@ -400,16 +400,17 @@
                 pipeline_interface=piface,
                 prj=self.prj,
                 compute_variables=comp_vars,
                 delay=args.time_delay,
                 extra_args=args.command_extra,
                 extra_args_override=args.command_extra_override,
                 ignore_flags=args.ignore_flags,
-                max_cmds=args.lumpn,
-                max_size=args.lump,
+                max_cmds=args.lump_n,
+                max_size=args.lump_s,
+                max_jobs=args.lump_j,
             )
             submission_conductors[piface.pipe_iface_file] = conductor
 
         _LOGGER.info(f"Pipestat compatible: {self.prj.pipestat_configured_project}")
         self.debug["Pipestat compatible"] = (
             self.prj.pipestat_configured_project or self.prj.pipestat_configured
         )
```

### Comparing `looper-1.7.0a1/looper/parser_types.py` & `looper-1.7.1/looper/parser_types.py`

 * *Files identical despite different names*

### Comparing `looper-1.7.0a1/looper/pipeline_interface.py` & `looper-1.7.1/looper/pipeline_interface.py`

 * *Files identical despite different names*

### Comparing `looper-1.7.0a1/looper/plugins.py` & `looper-1.7.1/looper/plugins.py`

 * *Files identical despite different names*

### Comparing `looper-1.7.0a1/looper/processed_project.py` & `looper-1.7.1/looper/processed_project.py`

 * *Files identical despite different names*

### Comparing `looper-1.7.0a1/looper/project.py` & `looper-1.7.1/looper/project.py`

 * *Files identical despite different names*

### Comparing `looper-1.7.0a1/looper/schemas/pipeline_interface_schema_generic.yaml` & `looper-1.7.1/looper/schemas/pipeline_interface_schema_generic.yaml`

 * *Files identical despite different names*

### Comparing `looper-1.7.0a1/looper/schemas/pipeline_interface_schema_project.yaml` & `looper-1.7.1/looper/schemas/pipeline_interface_schema_project.yaml`

 * *Files identical despite different names*

### Comparing `looper-1.7.0a1/looper/schemas/pipeline_interface_schema_sample.yaml` & `looper-1.7.1/looper/schemas/pipeline_interface_schema_sample.yaml`

 * *Files identical despite different names*

### Comparing `looper-1.7.0a1/looper/utils.py` & `looper-1.7.1/looper/utils.py`

 * *Files identical despite different names*

### Comparing `looper-1.7.0a1/looper.egg-info/PKG-INFO` & `looper-1.7.1/looper.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: looper
-Version: 1.7.0a1
+Version: 1.7.1
 Summary: A pipeline submission engine that parses sample inputs and submits pipelines for each sample.
 Home-page: https://github.com/pepkit/looper
 Author: Nathan Sheffield, Vince Reuter, Michal Stolarczyk, Johanna Klughammer, Andre Rendeiro
 License: BSD2
 Keywords: bioinformatics,sequencing,ngs
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
@@ -19,15 +19,15 @@
 Requires-Dist: divvy>=0.5.0
 Requires-Dist: eido>=0.2.1
 Requires-Dist: jinja2
 Requires-Dist: logmuse>=0.2.0
 Requires-Dist: pandas>=2.0.2
 Requires-Dist: pephubclient>=0.1.2
 Requires-Dist: peppy>=0.40.0
-Requires-Dist: pipestat>=0.7.1a1
+Requires-Dist: pipestat<0.9.0,>=0.8.0
 Requires-Dist: pyyaml>=3.12
 Requires-Dist: rich>=9.10.0
 Requires-Dist: ubiquerg>=0.5.2
 Requires-Dist: yacman>=0.9.2
 
 # <img src="docs/img/looper_logo.svg" alt="looper logo" height="70">
```

### Comparing `looper-1.7.0a1/looper.egg-info/SOURCES.txt` & `looper-1.7.1/looper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `looper-1.7.0a1/setup.py` & `looper-1.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `looper-1.7.0a1/tests/test_clean.py` & `looper-1.7.1/tests/test_clean.py`

 * *Files identical despite different names*

### Comparing `looper-1.7.0a1/tests/test_desired_sample_range.py` & `looper-1.7.1/tests/test_desired_sample_range.py`

 * *Files identical despite different names*

### Comparing `looper-1.7.0a1/tests/test_natural_range.py` & `looper-1.7.1/tests/test_natural_range.py`

 * *Files identical despite different names*

