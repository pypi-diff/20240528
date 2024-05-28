# Comparing `tmp/django_simple_deploy-0.6.2.tar.gz` & `tmp/django_simple_deploy-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_simple_deploy-0.6.2.tar", last modified: Mon May 27 16:35:04 2024, max compression
+gzip compressed data, was "django_simple_deploy-0.6.3.tar", last modified: Tue May 28 19:45:11 2024, max compression
```

## Comparing `django_simple_deploy-0.6.2.tar` & `django_simple_deploy-0.6.3.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-27 16:35:04.557356 django_simple_deploy-0.6.2/
--rw-r--r--   0 eric       (501) staff       (20)     1484 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.2/LICENSE
--rw-r--r--   0 eric       (501) staff       (20)      121 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.2/MANIFEST.in
--rw-r--r--   0 eric       (501) staff       (20)     2805 2024-05-27 16:35:04.557300 django_simple_deploy-0.6.2/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)     1367 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.2/README.md
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-27 16:35:04.557075 django_simple_deploy-0.6.2/django_simple_deploy.egg-info/
--rw-r--r--   0 eric       (501) staff       (20)     2805 2024-05-27 16:35:04.000000 django_simple_deploy-0.6.2/django_simple_deploy.egg-info/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)     2804 2024-05-27 16:35:04.000000 django_simple_deploy-0.6.2/django_simple_deploy.egg-info/SOURCES.txt
--rw-r--r--   0 eric       (501) staff       (20)        1 2024-05-27 16:35:04.000000 django_simple_deploy-0.6.2/django_simple_deploy.egg-info/dependency_links.txt
--rw-r--r--   0 eric       (501) staff       (20)       42 2024-05-27 16:35:04.000000 django_simple_deploy-0.6.2/django_simple_deploy.egg-info/requires.txt
--rw-r--r--   0 eric       (501) staff       (20)       14 2024-05-27 16:35:04.000000 django_simple_deploy-0.6.2/django_simple_deploy.egg-info/top_level.txt
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-27 16:35:04.542937 django_simple_deploy-0.6.2/docs/
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-27 16:35:04.543895 django_simple_deploy-0.6.2/docs/contributing/
--rw-r--r--   0 eric       (501) staff       (20)     2239 2024-05-26 21:53:10.000000 django_simple_deploy-0.6.2/docs/contributing/architecture_notes.md
--rw-r--r--   0 eric       (501) staff       (20)      836 2024-05-23 00:41:20.000000 django_simple_deploy-0.6.2/docs/contributing/coding_guide.md
--rw-r--r--   0 eric       (501) staff       (20)    13922 2023-11-01 22:47:04.000000 django_simple_deploy-0.6.2/docs/contributing/development_environment.md
--rw-r--r--   0 eric       (501) staff       (20)     3471 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.2/docs/contributing/index.md
--rw-r--r--   0 eric       (501) staff       (20)     3392 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.2/docs/contributing/own_account.md
--rw-r--r--   0 eric       (501) staff       (20)      464 2024-05-26 21:53:10.000000 django_simple_deploy-0.6.2/docs/contributing/parking_lot.md
--rw-r--r--   0 eric       (501) staff       (20)     7296 2023-11-01 22:47:04.000000 django_simple_deploy-0.6.2/docs/contributing/test_run.md
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-27 16:35:04.544320 django_simple_deploy-0.6.2/docs/design_docs/
--rw-r--r--   0 eric       (501) staff       (20)     2727 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.2/docs/design_docs/rationale.md
--rw-r--r--   0 eric       (501) staff       (20)     5146 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.2/docs/design_docs/strengths_limitations.md
--rw-r--r--   0 eric       (501) staff       (20)     3589 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.2/docs/design_docs/use_cases.md
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-27 16:35:04.544605 django_simple_deploy-0.6.2/docs/general_documentation/
--rw-r--r--   0 eric       (501) staff       (20)     7738 2023-12-04 20:37:01.000000 django_simple_deploy-0.6.2/docs/general_documentation/choosing_platform.md
--rw-r--r--   0 eric       (501) staff       (20)     9197 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.2/docs/general_documentation/cli_reference.md
--rw-r--r--   0 eric       (501) staff       (20)     1543 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.2/docs/index.md
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-27 16:35:04.545292 django_simple_deploy-0.6.2/docs/maintaining/
--rw-r--r--   0 eric       (501) staff       (20)     4088 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.2/docs/maintaining/adr.md
--rw-r--r--   0 eric       (501) staff       (20)     1049 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.2/docs/maintaining/index.md
--rw-r--r--   0 eric       (501) staff       (20)     1831 2023-11-01 22:47:04.000000 django_simple_deploy-0.6.2/docs/maintaining/managing_releases.md
--rw-r--r--   0 eric       (501) staff       (20)     1518 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.2/docs/maintaining/merging_prs.md
--rw-r--r--   0 eric       (501) staff       (20)     3418 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.2/docs/maintaining/updating_docs.md
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-27 16:35:04.545809 django_simple_deploy-0.6.2/docs/quick_starts/
--rw-r--r--   0 eric       (501) staff       (20)      408 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.2/docs/quick_starts/index.md
--rw-r--r--   0 eric       (501) staff       (20)     4059 2023-12-04 20:37:01.000000 django_simple_deploy-0.6.2/docs/quick_starts/quick_start_flyio.md
--rw-r--r--   0 eric       (501) staff       (20)     3835 2023-12-06 08:10:57.000000 django_simple_deploy-0.6.2/docs/quick_starts/quick_start_heroku.md
--rw-r--r--   0 eric       (501) staff       (20)     3527 2024-05-23 00:41:20.000000 django_simple_deploy-0.6.2/docs/quick_starts/quick_start_platformsh.md
--rw-r--r--   0 eric       (501) staff       (20)       17 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.2/docs/requirements.txt
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-27 16:35:04.546075 django_simple_deploy-0.6.2/docs/roadmap/
--rw-r--r--   0 eric       (501) staff       (20)      222 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.2/docs/roadmap/index.md
--rw-r--r--   0 eric       (501) staff       (20)     6149 2023-12-06 08:10:57.000000 django_simple_deploy-0.6.2/docs/roadmap/reaching_one_point_o.md
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-27 16:35:04.546584 django_simple_deploy-0.6.2/docs/testing/
--rw-r--r--   0 eric       (501) staff       (20)     4740 2024-04-22 20:08:42.000000 django_simple_deploy-0.6.2/docs/testing/e2e_tests.md
--rw-r--r--   0 eric       (501) staff       (20)      665 2024-04-22 20:08:42.000000 django_simple_deploy-0.6.2/docs/testing/index.md
--rw-r--r--   0 eric       (501) staff       (20)     5142 2024-04-22 20:08:42.000000 django_simple_deploy-0.6.2/docs/testing/integration_tests.md
--rw-r--r--   0 eric       (501) staff       (20)     1251 2024-04-22 20:08:42.000000 django_simple_deploy-0.6.2/docs/testing/unit_tests.md
--rw-r--r--   0 eric       (501) staff       (20)      100 2023-05-09 23:04:33.000000 django_simple_deploy-0.6.2/pyproject.toml
--rw-r--r--   0 eric       (501) staff       (20)     1355 2024-05-27 16:35:04.557992 django_simple_deploy-0.6.2/setup.cfg
--rw-r--r--   0 eric       (501) staff       (20)       38 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.2/setup.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-27 16:35:04.546804 django_simple_deploy-0.6.2/simple_deploy/
--rw-r--r--   0 eric       (501) staff       (20)        0 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.2/simple_deploy/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)      157 2024-05-23 22:47:20.000000 django_simple_deploy-0.6.2/simple_deploy/apps.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-27 16:35:04.540474 django_simple_deploy-0.6.2/simple_deploy/management/
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-27 16:35:04.547712 django_simple_deploy-0.6.2/simple_deploy/management/commands/
--rw-r--r--   0 eric       (501) staff       (20)     3902 2024-04-22 20:08:42.000000 django_simple_deploy-0.6.2/simple_deploy/management/commands/cli.py
--rw-r--r--   0 eric       (501) staff       (20)     3342 2024-05-23 22:47:20.000000 django_simple_deploy-0.6.2/simple_deploy/management/commands/deploy_messages.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-27 16:35:04.547972 django_simple_deploy-0.6.2/simple_deploy/management/commands/fly_io/
--rw-r--r--   0 eric       (501) staff       (20)    29794 2024-05-25 19:59:51.000000 django_simple_deploy-0.6.2/simple_deploy/management/commands/fly_io/deploy.py
--rw-r--r--   0 eric       (501) staff       (20)     8089 2024-01-12 06:54:17.000000 django_simple_deploy-0.6.2/simple_deploy/management/commands/fly_io/deploy_messages.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-27 16:35:04.549005 django_simple_deploy-0.6.2/simple_deploy/management/commands/fly_io/templates/
--rw-r--r--   0 eric       (501) staff       (20)      507 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.2/simple_deploy/management/commands/fly_io/templates/dockerfile
--rw-r--r--   0 eric       (501) staff       (20)      555 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.2/simple_deploy/management/commands/fly_io/templates/dockerfile_pipenv
--rw-r--r--   0 eric       (501) staff       (20)      687 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.2/simple_deploy/management/commands/fly_io/templates/dockerfile_poetry
--rw-r--r--   0 eric       (501) staff       (20)      889 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.2/simple_deploy/management/commands/fly_io/templates/fly.toml
--rw-r--r--   0 eric       (501) staff       (20)     1428 2024-05-23 23:04:10.000000 django_simple_deploy-0.6.2/simple_deploy/management/commands/fly_io/templates/settings.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-27 16:35:04.553151 django_simple_deploy-0.6.2/simple_deploy/management/commands/heroku/
--rw-r--r--   0 eric       (501) staff       (20)    19163 2024-05-27 15:48:02.000000 django_simple_deploy-0.6.2/simple_deploy/management/commands/heroku/deploy.py
--rw-r--r--   0 eric       (501) staff       (20)     4650 2024-05-26 21:53:10.000000 django_simple_deploy-0.6.2/simple_deploy/management/commands/heroku/deploy_messages.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-27 16:35:04.553459 django_simple_deploy-0.6.2/simple_deploy/management/commands/heroku/templates/
--rw-r--r--   0 eric       (501) staff       (20)     1284 2024-05-27 15:48:02.000000 django_simple_deploy-0.6.2/simple_deploy/management/commands/heroku/templates/settings.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-27 16:35:04.555521 django_simple_deploy-0.6.2/simple_deploy/management/commands/platform_sh/
--rw-r--r--   0 eric       (501) staff       (20)    17108 2024-05-25 19:59:51.000000 django_simple_deploy-0.6.2/simple_deploy/management/commands/platform_sh/deploy.py
--rw-r--r--   0 eric       (501) staff       (20)     6698 2024-05-23 23:04:10.000000 django_simple_deploy-0.6.2/simple_deploy/management/commands/platform_sh/deploy_messages.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-27 16:35:04.556470 django_simple_deploy-0.6.2/simple_deploy/management/commands/platform_sh/templates/
--rw-r--r--   0 eric       (501) staff       (20)     1977 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.2/simple_deploy/management/commands/platform_sh/templates/pipenv.platform.app.yaml
--rw-r--r--   0 eric       (501) staff       (20)     1934 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.2/simple_deploy/management/commands/platform_sh/templates/platform.app.yaml
--rw-r--r--   0 eric       (501) staff       (20)     2423 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.2/simple_deploy/management/commands/platform_sh/templates/poetry.platform.app.yaml
--rw-r--r--   0 eric       (501) staff       (20)      249 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.2/simple_deploy/management/commands/platform_sh/templates/services.yaml
--rw-r--r--   0 eric       (501) staff       (20)     1072 2024-05-23 23:04:10.000000 django_simple_deploy-0.6.2/simple_deploy/management/commands/platform_sh/templates/settings.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-27 16:35:04.541072 django_simple_deploy-0.6.2/simple_deploy/management/commands/platform_sh/tests/
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-27 16:35:04.556618 django_simple_deploy-0.6.2/simple_deploy/management/commands/platform_sh/tests/unit_tests/
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-27 16:35:04.556773 django_simple_deploy-0.6.2/simple_deploy/management/commands/platform_sh/tests/unit_tests/resources/
--rw-r--r--   0 eric       (501) staff       (20)      640 2024-05-23 00:41:20.000000 django_simple_deploy-0.6.2/simple_deploy/management/commands/platform_sh/tests/unit_tests/resources/projects_info_output_csv.txt
--rw-r--r--   0 eric       (501) staff       (20)      673 2024-05-23 23:04:10.000000 django_simple_deploy-0.6.2/simple_deploy/management/commands/platform_sh/tests/unit_tests/test_plsh_utils.py
--rw-r--r--   0 eric       (501) staff       (20)      788 2024-05-23 23:04:10.000000 django_simple_deploy-0.6.2/simple_deploy/management/commands/platform_sh/utils.py
--rw-r--r--   0 eric       (501) staff       (20)    27315 2024-05-26 21:53:10.000000 django_simple_deploy-0.6.2/simple_deploy/management/commands/simple_deploy.py
--rw-r--r--   0 eric       (501) staff       (20)    12349 2024-05-25 22:52:28.000000 django_simple_deploy-0.6.2/simple_deploy/management/commands/utils.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-28 19:45:11.302088 django_simple_deploy-0.6.3/
+-rw-r--r--   0 eric       (501) staff       (20)     1484 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.3/LICENSE
+-rw-r--r--   0 eric       (501) staff       (20)      121 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.3/MANIFEST.in
+-rw-r--r--   0 eric       (501) staff       (20)     2805 2024-05-28 19:45:11.302009 django_simple_deploy-0.6.3/PKG-INFO
+-rw-r--r--   0 eric       (501) staff       (20)     1367 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.3/README.md
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-28 19:45:11.301761 django_simple_deploy-0.6.3/django_simple_deploy.egg-info/
+-rw-r--r--   0 eric       (501) staff       (20)     2805 2024-05-28 19:45:11.000000 django_simple_deploy-0.6.3/django_simple_deploy.egg-info/PKG-INFO
+-rw-r--r--   0 eric       (501) staff       (20)     2804 2024-05-28 19:45:11.000000 django_simple_deploy-0.6.3/django_simple_deploy.egg-info/SOURCES.txt
+-rw-r--r--   0 eric       (501) staff       (20)        1 2024-05-28 19:45:11.000000 django_simple_deploy-0.6.3/django_simple_deploy.egg-info/dependency_links.txt
+-rw-r--r--   0 eric       (501) staff       (20)       42 2024-05-28 19:45:11.000000 django_simple_deploy-0.6.3/django_simple_deploy.egg-info/requires.txt
+-rw-r--r--   0 eric       (501) staff       (20)       14 2024-05-28 19:45:11.000000 django_simple_deploy-0.6.3/django_simple_deploy.egg-info/top_level.txt
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-28 19:45:11.291033 django_simple_deploy-0.6.3/docs/
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-28 19:45:11.292017 django_simple_deploy-0.6.3/docs/contributing/
+-rw-r--r--   0 eric       (501) staff       (20)     2239 2024-05-26 21:53:10.000000 django_simple_deploy-0.6.3/docs/contributing/architecture_notes.md
+-rw-r--r--   0 eric       (501) staff       (20)      836 2024-05-23 00:41:20.000000 django_simple_deploy-0.6.3/docs/contributing/coding_guide.md
+-rw-r--r--   0 eric       (501) staff       (20)    13922 2023-11-01 22:47:04.000000 django_simple_deploy-0.6.3/docs/contributing/development_environment.md
+-rw-r--r--   0 eric       (501) staff       (20)     3471 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.3/docs/contributing/index.md
+-rw-r--r--   0 eric       (501) staff       (20)     3392 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.3/docs/contributing/own_account.md
+-rw-r--r--   0 eric       (501) staff       (20)     5115 2024-05-28 06:37:29.000000 django_simple_deploy-0.6.3/docs/contributing/parking_lot.md
+-rw-r--r--   0 eric       (501) staff       (20)     7296 2023-11-01 22:47:04.000000 django_simple_deploy-0.6.3/docs/contributing/test_run.md
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-28 19:45:11.292424 django_simple_deploy-0.6.3/docs/design_docs/
+-rw-r--r--   0 eric       (501) staff       (20)     2727 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.3/docs/design_docs/rationale.md
+-rw-r--r--   0 eric       (501) staff       (20)     5146 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.3/docs/design_docs/strengths_limitations.md
+-rw-r--r--   0 eric       (501) staff       (20)     3589 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.3/docs/design_docs/use_cases.md
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-28 19:45:11.292687 django_simple_deploy-0.6.3/docs/general_documentation/
+-rw-r--r--   0 eric       (501) staff       (20)     7738 2023-12-04 20:37:01.000000 django_simple_deploy-0.6.3/docs/general_documentation/choosing_platform.md
+-rw-r--r--   0 eric       (501) staff       (20)     9197 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.3/docs/general_documentation/cli_reference.md
+-rw-r--r--   0 eric       (501) staff       (20)     1543 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.3/docs/index.md
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-28 19:45:11.293313 django_simple_deploy-0.6.3/docs/maintaining/
+-rw-r--r--   0 eric       (501) staff       (20)     4088 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.3/docs/maintaining/adr.md
+-rw-r--r--   0 eric       (501) staff       (20)     1049 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.3/docs/maintaining/index.md
+-rw-r--r--   0 eric       (501) staff       (20)     1859 2024-05-27 16:42:26.000000 django_simple_deploy-0.6.3/docs/maintaining/managing_releases.md
+-rw-r--r--   0 eric       (501) staff       (20)     1666 2024-05-28 19:42:57.000000 django_simple_deploy-0.6.3/docs/maintaining/merging_prs.md
+-rw-r--r--   0 eric       (501) staff       (20)     3418 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.3/docs/maintaining/updating_docs.md
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-28 19:45:11.293836 django_simple_deploy-0.6.3/docs/quick_starts/
+-rw-r--r--   0 eric       (501) staff       (20)      408 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.3/docs/quick_starts/index.md
+-rw-r--r--   0 eric       (501) staff       (20)     4059 2023-12-04 20:37:01.000000 django_simple_deploy-0.6.3/docs/quick_starts/quick_start_flyio.md
+-rw-r--r--   0 eric       (501) staff       (20)     3835 2023-12-06 08:10:57.000000 django_simple_deploy-0.6.3/docs/quick_starts/quick_start_heroku.md
+-rw-r--r--   0 eric       (501) staff       (20)     3527 2024-05-23 00:41:20.000000 django_simple_deploy-0.6.3/docs/quick_starts/quick_start_platformsh.md
+-rw-r--r--   0 eric       (501) staff       (20)       17 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.3/docs/requirements.txt
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-28 19:45:11.294081 django_simple_deploy-0.6.3/docs/roadmap/
+-rw-r--r--   0 eric       (501) staff       (20)      222 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.3/docs/roadmap/index.md
+-rw-r--r--   0 eric       (501) staff       (20)     6149 2023-12-06 08:10:57.000000 django_simple_deploy-0.6.3/docs/roadmap/reaching_one_point_o.md
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-28 19:45:11.294597 django_simple_deploy-0.6.3/docs/testing/
+-rw-r--r--   0 eric       (501) staff       (20)     4740 2024-04-22 20:08:42.000000 django_simple_deploy-0.6.3/docs/testing/e2e_tests.md
+-rw-r--r--   0 eric       (501) staff       (20)      665 2024-04-22 20:08:42.000000 django_simple_deploy-0.6.3/docs/testing/index.md
+-rw-r--r--   0 eric       (501) staff       (20)     5142 2024-04-22 20:08:42.000000 django_simple_deploy-0.6.3/docs/testing/integration_tests.md
+-rw-r--r--   0 eric       (501) staff       (20)     1251 2024-04-22 20:08:42.000000 django_simple_deploy-0.6.3/docs/testing/unit_tests.md
+-rw-r--r--   0 eric       (501) staff       (20)      100 2023-05-09 23:04:33.000000 django_simple_deploy-0.6.3/pyproject.toml
+-rw-r--r--   0 eric       (501) staff       (20)     1355 2024-05-28 19:45:11.302794 django_simple_deploy-0.6.3/setup.cfg
+-rw-r--r--   0 eric       (501) staff       (20)       38 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.3/setup.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-28 19:45:11.294823 django_simple_deploy-0.6.3/simple_deploy/
+-rw-r--r--   0 eric       (501) staff       (20)        0 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.3/simple_deploy/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)      157 2024-05-23 22:47:20.000000 django_simple_deploy-0.6.3/simple_deploy/apps.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-28 19:45:11.288545 django_simple_deploy-0.6.3/simple_deploy/management/
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-28 19:45:11.296220 django_simple_deploy-0.6.3/simple_deploy/management/commands/
+-rw-r--r--   0 eric       (501) staff       (20)     3902 2024-04-22 20:08:42.000000 django_simple_deploy-0.6.3/simple_deploy/management/commands/cli.py
+-rw-r--r--   0 eric       (501) staff       (20)     3342 2024-05-23 22:47:20.000000 django_simple_deploy-0.6.3/simple_deploy/management/commands/deploy_messages.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-28 19:45:11.296512 django_simple_deploy-0.6.3/simple_deploy/management/commands/fly_io/
+-rw-r--r--   0 eric       (501) staff       (20)    29973 2024-05-28 19:42:57.000000 django_simple_deploy-0.6.3/simple_deploy/management/commands/fly_io/deploy.py
+-rw-r--r--   0 eric       (501) staff       (20)     8489 2024-05-28 19:42:57.000000 django_simple_deploy-0.6.3/simple_deploy/management/commands/fly_io/deploy_messages.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-28 19:45:11.297183 django_simple_deploy-0.6.3/simple_deploy/management/commands/fly_io/templates/
+-rw-r--r--   0 eric       (501) staff       (20)      507 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.3/simple_deploy/management/commands/fly_io/templates/dockerfile
+-rw-r--r--   0 eric       (501) staff       (20)      555 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.3/simple_deploy/management/commands/fly_io/templates/dockerfile_pipenv
+-rw-r--r--   0 eric       (501) staff       (20)      687 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.3/simple_deploy/management/commands/fly_io/templates/dockerfile_poetry
+-rw-r--r--   0 eric       (501) staff       (20)      889 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.3/simple_deploy/management/commands/fly_io/templates/fly.toml
+-rw-r--r--   0 eric       (501) staff       (20)     1416 2024-05-28 19:42:57.000000 django_simple_deploy-0.6.3/simple_deploy/management/commands/fly_io/templates/settings.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-28 19:45:11.297482 django_simple_deploy-0.6.3/simple_deploy/management/commands/heroku/
+-rw-r--r--   0 eric       (501) staff       (20)    19163 2024-05-28 19:42:57.000000 django_simple_deploy-0.6.3/simple_deploy/management/commands/heroku/deploy.py
+-rw-r--r--   0 eric       (501) staff       (20)     4650 2024-05-26 21:53:10.000000 django_simple_deploy-0.6.3/simple_deploy/management/commands/heroku/deploy_messages.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-28 19:45:11.298965 django_simple_deploy-0.6.3/simple_deploy/management/commands/heroku/templates/
+-rw-r--r--   0 eric       (501) staff       (20)     1285 2024-05-28 19:42:57.000000 django_simple_deploy-0.6.3/simple_deploy/management/commands/heroku/templates/settings.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-28 19:45:11.299467 django_simple_deploy-0.6.3/simple_deploy/management/commands/platform_sh/
+-rw-r--r--   0 eric       (501) staff       (20)    16563 2024-05-28 19:42:57.000000 django_simple_deploy-0.6.3/simple_deploy/management/commands/platform_sh/deploy.py
+-rw-r--r--   0 eric       (501) staff       (20)     7112 2024-05-28 19:42:57.000000 django_simple_deploy-0.6.3/simple_deploy/management/commands/platform_sh/deploy_messages.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-28 19:45:11.301110 django_simple_deploy-0.6.3/simple_deploy/management/commands/platform_sh/templates/
+-rw-r--r--   0 eric       (501) staff       (20)     1977 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.3/simple_deploy/management/commands/platform_sh/templates/pipenv.platform.app.yaml
+-rw-r--r--   0 eric       (501) staff       (20)     1934 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.3/simple_deploy/management/commands/platform_sh/templates/platform.app.yaml
+-rw-r--r--   0 eric       (501) staff       (20)     2423 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.3/simple_deploy/management/commands/platform_sh/templates/poetry.platform.app.yaml
+-rw-r--r--   0 eric       (501) staff       (20)      249 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.3/simple_deploy/management/commands/platform_sh/templates/services.yaml
+-rw-r--r--   0 eric       (501) staff       (20)     1072 2024-05-23 23:04:10.000000 django_simple_deploy-0.6.3/simple_deploy/management/commands/platform_sh/templates/settings.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-28 19:45:11.289162 django_simple_deploy-0.6.3/simple_deploy/management/commands/platform_sh/tests/
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-28 19:45:11.301234 django_simple_deploy-0.6.3/simple_deploy/management/commands/platform_sh/tests/unit_tests/
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-28 19:45:11.301566 django_simple_deploy-0.6.3/simple_deploy/management/commands/platform_sh/tests/unit_tests/resources/
+-rw-r--r--   0 eric       (501) staff       (20)      640 2024-05-23 00:41:20.000000 django_simple_deploy-0.6.3/simple_deploy/management/commands/platform_sh/tests/unit_tests/resources/projects_info_output_csv.txt
+-rw-r--r--   0 eric       (501) staff       (20)      673 2024-05-23 23:04:10.000000 django_simple_deploy-0.6.3/simple_deploy/management/commands/platform_sh/tests/unit_tests/test_plsh_utils.py
+-rw-r--r--   0 eric       (501) staff       (20)      788 2024-05-23 23:04:10.000000 django_simple_deploy-0.6.3/simple_deploy/management/commands/platform_sh/utils.py
+-rw-r--r--   0 eric       (501) staff       (20)    27314 2024-05-28 19:42:57.000000 django_simple_deploy-0.6.3/simple_deploy/management/commands/simple_deploy.py
+-rw-r--r--   0 eric       (501) staff       (20)    12349 2024-05-25 22:52:28.000000 django_simple_deploy-0.6.3/simple_deploy/management/commands/utils.py
```

### Comparing `django_simple_deploy-0.6.2/LICENSE` & `django_simple_deploy-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.2/PKG-INFO` & `django_simple_deploy-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-simple-deploy
-Version: 0.6.2
+Version: 0.6.3
 Summary: A management command that auto-configures a Django project for deployment.
 Author: Eric Matthes
 Author-email: ehmatthes@gmail.com
 License: BSD
 Project-URL: Documentation, https://django-simple-deploy.readthedocs.io/en/latest/
 Project-URL: GitHub, https://github.com/ehmatthes/django-simple-deploy
 Project-URL: Changelog, https://github.com/ehmatthes/django-simple-deploy/blob/main/CHANGELOG.md
```

### Comparing `django_simple_deploy-0.6.2/README.md` & `django_simple_deploy-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.2/django_simple_deploy.egg-info/PKG-INFO` & `django_simple_deploy-0.6.3/django_simple_deploy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-simple-deploy
-Version: 0.6.2
+Version: 0.6.3
 Summary: A management command that auto-configures a Django project for deployment.
 Author: Eric Matthes
 Author-email: ehmatthes@gmail.com
 License: BSD
 Project-URL: Documentation, https://django-simple-deploy.readthedocs.io/en/latest/
 Project-URL: GitHub, https://github.com/ehmatthes/django-simple-deploy
 Project-URL: Changelog, https://github.com/ehmatthes/django-simple-deploy/blob/main/CHANGELOG.md
```

### Comparing `django_simple_deploy-0.6.2/django_simple_deploy.egg-info/SOURCES.txt` & `django_simple_deploy-0.6.3/django_simple_deploy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.2/docs/contributing/architecture_notes.md` & `django_simple_deploy-0.6.3/docs/contributing/architecture_notes.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.2/docs/contributing/coding_guide.md` & `django_simple_deploy-0.6.3/docs/contributing/coding_guide.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.2/docs/contributing/development_environment.md` & `django_simple_deploy-0.6.3/docs/contributing/development_environment.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.2/docs/contributing/index.md` & `django_simple_deploy-0.6.3/docs/contributing/index.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.2/docs/contributing/own_account.md` & `django_simple_deploy-0.6.3/docs/contributing/own_account.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.2/docs/contributing/test_run.md` & `django_simple_deploy-0.6.3/docs/contributing/test_run.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.2/docs/design_docs/rationale.md` & `django_simple_deploy-0.6.3/docs/design_docs/rationale.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.2/docs/design_docs/strengths_limitations.md` & `django_simple_deploy-0.6.3/docs/design_docs/strengths_limitations.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.2/docs/design_docs/use_cases.md` & `django_simple_deploy-0.6.3/docs/design_docs/use_cases.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.2/docs/general_documentation/choosing_platform.md` & `django_simple_deploy-0.6.3/docs/general_documentation/choosing_platform.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.2/docs/general_documentation/cli_reference.md` & `django_simple_deploy-0.6.3/docs/general_documentation/cli_reference.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.2/docs/index.md` & `django_simple_deploy-0.6.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.2/docs/maintaining/adr.md` & `django_simple_deploy-0.6.3/docs/maintaining/adr.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.2/docs/maintaining/index.md` & `django_simple_deploy-0.6.3/docs/maintaining/index.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.2/docs/maintaining/managing_releases.md` & `django_simple_deploy-0.6.3/docs/maintaining/managing_releases.md`

 * *Files 19% similar despite different names*

```diff
@@ -27,25 +27,27 @@
 ```
 
 - View on PyPI:
 [https://pypi.org/project/django-simple-deploy/](https://pypi.org/project/django-simple-deploy/)
 
 - Test the released package:
 ```
-$ pytest integration_tests/platforms/<platform-name>/test_deployment.py --pypi -s
+$ pytest tests/e2e_tests/platforms/<platform-name> --pypi -s
 ```
 
     - Sometimes there's a stale cache that causes the previous release to be installed. If you don't check this version, you won't know whether the new release actually works. In the test output, verify that the new version was installed. Look for something like this:
 
 ```sh
-integration_tests/platforms/fly_io/test_deployment.py s
+$ pytest tests/e2e_tests/platforms/fly_io --pypi -s
 Temp project directory: ...
 ...
-Installing collected packages: toml, django-simple-deploy
-Successfully installed django-simple-deploy-0.5.16 toml-0.10.2
+Collecting django-simple-deploy
+  Downloading django_simple_deploy-0.6.2-py3-none-any.whl.metadata
+...
+Successfully installed Django-5.0.6 ... django-simple-deploy-0.6.2 ...
 ...
 ```
 
 Deleting branches
 ---
 
 Delete the remote and local development branches:
```

### Comparing `django_simple_deploy-0.6.2/docs/maintaining/merging_prs.md` & `django_simple_deploy-0.6.3/docs/maintaining/merging_prs.md`

 * *Files 9% similar despite different names*

```diff
@@ -18,8 +18,9 @@
 
 - Contributors should make all their changes on a development branch. They are free to make as many in-progress commits as they need, but should aim for a final atomic PR.
 - Contributors should create a PR on GitHub.
     - In the initial comment box when opening a PR, contributors should make any comments about the changes they've made that would help in code review.
 - When appropriate, a maintainer will merge the PR, using `squash and merge` through the GitHub interface.
     - In the comment box for the `Confirm squash and merge` step, write a one-line commit message summarizing the PR, appropriate for one-line `git log` output.
     - For more significant PRs, write a longer message summarizing the major points of what was done. When you're finished writing the message, please delete the bullet points from the individual commits in the PR.
+    - Update the changelog after merging a PR. Use an "Unreleased" section if a new release is not being made. This can be a direct commit to main.
 - Everyone pulls changes to their local `main` branch: `git pull origin main`
```

### Comparing `django_simple_deploy-0.6.2/docs/maintaining/updating_docs.md` & `django_simple_deploy-0.6.3/docs/maintaining/updating_docs.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.2/docs/quick_starts/quick_start_flyio.md` & `django_simple_deploy-0.6.3/docs/quick_starts/quick_start_flyio.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.2/docs/quick_starts/quick_start_heroku.md` & `django_simple_deploy-0.6.3/docs/quick_starts/quick_start_heroku.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.2/docs/quick_starts/quick_start_platformsh.md` & `django_simple_deploy-0.6.3/docs/quick_starts/quick_start_platformsh.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.2/docs/roadmap/reaching_one_point_o.md` & `django_simple_deploy-0.6.3/docs/roadmap/reaching_one_point_o.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.2/docs/testing/e2e_tests.md` & `django_simple_deploy-0.6.3/docs/testing/e2e_tests.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.2/docs/testing/index.md` & `django_simple_deploy-0.6.3/docs/testing/index.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.2/docs/testing/integration_tests.md` & `django_simple_deploy-0.6.3/docs/testing/integration_tests.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.2/docs/testing/unit_tests.md` & `django_simple_deploy-0.6.3/docs/testing/unit_tests.md`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.2/setup.cfg` & `django_simple_deploy-0.6.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-simple-deploy
-version = 0.6.2
+version = 0.6.3
 description = A management command that auto-configures a Django project for deployment.
 long_description = file: README.md
 long_description_content_type = text/markdown
 project_urls = 
 	Documentation = https://django-simple-deploy.readthedocs.io/en/latest/
 	GitHub = https://github.com/ehmatthes/django-simple-deploy
 	Changelog = https://github.com/ehmatthes/django-simple-deploy/blob/main/CHANGELOG.md
```

### Comparing `django_simple_deploy-0.6.2/simple_deploy/management/commands/cli.py` & `django_simple_deploy-0.6.3/simple_deploy/management/commands/cli.py`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.2/simple_deploy/management/commands/deploy_messages.py` & `django_simple_deploy-0.6.3/simple_deploy/management/commands/deploy_messages.py`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.2/simple_deploy/management/commands/fly_io/deploy.py` & `django_simple_deploy-0.6.3/simple_deploy/management/commands/fly_io/deploy.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,27 +39,24 @@
     # --- Public methods ---
 
     def deploy(self, *args, **options):
         """Coordinate the overall configuration and deployment."""
         self.sd.write_output("\nConfiguring project for deployment to Fly.io...")
 
         self._confirm_preliminary()
-
         self._validate_platform()
 
-        if self.sd.automate_all:
-            self._prep_automate_all()
-
-        self._set_on_flyio()
-        self._set_debug()
+        self._prep_automate_all()
+        self._set_env_vars()
         self._add_dockerfile()
         self._add_dockerignore()
         self._add_flytoml()
         self._modify_settings()
         self._add_requirements()
+
         self._conclude_automate_all()
         self._show_success_message()
 
     # --- Helper methods for deploy() ---
 
     def _confirm_preliminary(self):
         """Confirm acknwledgement of preliminary (pre-1.0) state of project."""
@@ -92,14 +89,15 @@
         """
         if self.sd.unit_testing:
             # Unit tests don't use the platform's CLI. Use the deployed project name
             # that was passed to the simple_deploy CLI.
             self.deployed_project_name = self.sd.deployed_project_name
             return
 
+        self._check_flyio_settings()
         self._validate_cli()
 
         # Make sure a Fly.io app has been created, or create one if  using
         # --automate-all. Get the name of that app, which will be the  same as
         # self.app_name.
         self.deployed_project_name = self._get_deployed_project_name()
 
@@ -107,14 +105,22 @@
         self._create_db()
 
     def _prep_automate_all(self):
         """Take any further actions needed if using automate_all."""
         # All necessary resources have been created earlier, during validation.
         pass
 
+    def _set_env_vars(self):
+        """Set Fly.io-specific environment variables."""
+        if self.sd.unit_testing:
+            return
+
+        self._set_on_flyio()
+        self._set_debug()
+
     def _set_on_flyio(self):
         """Set a secret, ON_FLYIO. This is used in settings.py to apply
         deployment-specific settings.
         """
         msg = "\nSetting ON_FLYIO secret..."
         self.sd.write_output(msg)
         self._set_secret("ON_FLYIO", "ON_FLYIO=1")
@@ -198,25 +204,18 @@
             }
             sd_utils.write_file_from_template(path, "fly.toml", context)
 
             msg = f"\n    Generated fly.toml: {path}"
             self.sd.write_output(msg)
 
     def _modify_settings(self):
-        """Add settings specific to Fly.io, if not already present."""
-        self.sd.write_output("\n  Checking for Fly.io-specific settings...")
+        """Add platformsh-specific settings."""
+        self.sd.write_output("\n  Adding a Fly.io-specific settings block...")
 
         settings_string = self.sd.settings_path.read_text()
-        if 'if os.environ.get("ON_FLYIO"):' in settings_string:
-            self.sd.write_output("\n    Found Fly.io settings block in settings.py.")
-            return
-
-        # No Fly-specific settings found; add Fly.io settings block.
-        self.sd.write_output("    No Fly.io settings found; adding settings...")
-
         safe_settings_string = mark_safe(settings_string)
         context = {
             "current_settings": safe_settings_string,
             "deployed_project_name": self.deployed_project_name,
         }
         sd_utils.write_file_from_template(self.sd.settings_path, "settings.py", context)
 
@@ -267,19 +266,19 @@
         if self.sd.automate_all:
             msg = self.messages.success_msg_automate_all(self.deployed_url)
         else:
             msg = self.messages.success_msg(log_output=self.sd.log_output)
         self.sd.write_output(msg)
 
     def _set_secret(self, needle, secret):
-        """Set a secret on Fly, if it's not already set."""
-        if self.sd.unit_testing:
-            msg = "  Skipping for unit testing."
-            self.sd.write_output(msg)
-            return
+        """Set a secret on Fly, if it's not already set.
+
+        DEV: Do we need to say that it's already set, and get confirmation to change
+        value? (Only needed if it's not set to same value.)
+        """
 
         # First check if secret has already been set.
         #   Don't log output of `fly secrets list`!
         cmd = f"fly secrets list -a {self.deployed_project_name} --json"
         output_obj = self.sd.run_quick_command(cmd)
         secrets_json = json.loads(output_obj.stdout.decode())
 
@@ -323,14 +322,24 @@
         if self.sd.on_macos:
             dockerignore_str += "\n.DS_Store\n"
 
         return dockerignore_str
 
     # --- Helper methods for _validate_platform() ---
 
+    def _check_flyio_settings(self):
+        """Check to see if a Fly.io settings block already exists."""
+        start_line = "# Fly.io settings."
+        self.sd.check_settings(
+            "Fly.io",
+            start_line,
+            self.messages.flyio_settings_found,
+            self.messages.cant_overwrite_settings,
+        )
+
     def _validate_cli(self):
         """Make sure the Fly.io CLI is installed, and user is authenticated."""
         cmd = "fly version"
 
         # This generates a FileNotFoundError on Ubuntu if the CLI is not installed.
         try:
             output_obj = self.sd.run_quick_command(cmd)
```

### Comparing `django_simple_deploy-0.6.2/simple_deploy/management/commands/fly_io/deploy_messages.py` & `django_simple_deploy-0.6.3/simple_deploy/management/commands/fly_io/deploy_messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,25 @@
 cli_logged_out = """
 You are currently logged out of the Fly.io CLI. Please log in,
   and then run simple_deploy again.
 You can log in from  the command line:
   $ fly auth login
 """
 
+flyio_settings_found = """
+There is already a Fly.io-specific settings block in settings.py. Is it okay to
+overwrite this block, and everything that follows in settings.py?
+"""
+
+cant_overwrite_settings = """
+In order to configure the project for deployment, we need to write a Fly.io-specific
+settings block. Please remove the current Fly.io-specific settings, and then run
+simple_deploy again.
+"""
+
 no_project_name = """
 A suitable Fly.io app to deploy against could not be found.
 
 The simple_deploy command expects that you've already created an app on Fly.io
 to push to.
 
 If you haven't done so, run the following command to create a new Fly.io app:
```

### Comparing `django_simple_deploy-0.6.2/simple_deploy/management/commands/fly_io/templates/dockerfile_pipenv` & `django_simple_deploy-0.6.3/simple_deploy/management/commands/fly_io/templates/dockerfile_pipenv`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.2/simple_deploy/management/commands/fly_io/templates/dockerfile_poetry` & `django_simple_deploy-0.6.3/simple_deploy/management/commands/fly_io/templates/dockerfile_poetry`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.2/simple_deploy/management/commands/fly_io/templates/fly.toml` & `django_simple_deploy-0.6.3/simple_deploy/management/commands/fly_io/templates/fly.toml`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.2/simple_deploy/management/commands/fly_io/templates/settings.py` & `django_simple_deploy-0.6.3/simple_deploy/management/commands/fly_io/templates/settings.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 {{current_settings}}
 
 
-# --- Settings for Fly.io. ---
+# Fly.io settings.
 import os
 
 if os.environ.get("ON_FLYIO_SETUP") or os.environ.get("ON_FLYIO"):
     # Static file configuration needs to take effect during the build process,
     #   and when deployed.
     # from https://whitenoise.evans.io/en/stable/#quickstart-for-django-apps
     STATIC_ROOT = os.path.join(BASE_DIR, "staticfiles")
```

### Comparing `django_simple_deploy-0.6.2/simple_deploy/management/commands/heroku/deploy.py` & `django_simple_deploy-0.6.3/simple_deploy/management/commands/heroku/deploy.py`

 * *Files 0% similar despite different names*

```diff
@@ -344,15 +344,15 @@
 
     # --- Utility methods ---
 
     def _check_heroku_settings(self):
         """Check to see if a Heroku settings block already exists."""
         start_line = "# Heroku settings."
         self.sd.check_settings(
-            "heroku",
+            "Heroku",
             start_line,
             self.messages.heroku_settings_found,
             self.messages.cant_overwrite_settings,
         )
 
     def _check_cli_installed(self):
         """Verify the Heroku CLI is installed on the user's system.
```

### Comparing `django_simple_deploy-0.6.2/simple_deploy/management/commands/heroku/deploy_messages.py` & `django_simple_deploy-0.6.3/simple_deploy/management/commands/heroku/deploy_messages.py`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.2/simple_deploy/management/commands/heroku/templates/settings.py` & `django_simple_deploy-0.6.3/simple_deploy/management/commands/heroku/templates/settings.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -33,8 +33,8 @@
         "staticfiles": {
             "BACKEND": "whitenoise.storage.CompressedManifestStaticFilesStorage",
         },
     }
 
     # Don't store the original (un-hashed filename) version of static files, to reduce slug size:
     # https://whitenoise.readthedocs.io/en/latest/django.html#WHITENOISE_KEEP_ONLY_HASHED_FILES
-    WHITENOISE_KEEP_ONLY_HASHED_FILES = True
+    WHITENOISE_KEEP_ONLY_HASHED_FILES = True
```

### Comparing `django_simple_deploy-0.6.2/simple_deploy/management/commands/platform_sh/deploy.py` & `django_simple_deploy-0.6.3/simple_deploy/management/commands/platform_sh/deploy.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,28 +38,23 @@
 
     def deploy(self, *args, **options):
         """Coordinate the overall configuration and deployment."""
 
         self.sd.write_output("\nConfiguring project for deployment to Platform.sh...")
 
         self._confirm_preliminary()
-
-        if self.sd.automate_all:
-            self._confirm_automate_all()
-
         self._validate_platform()
 
-        if self.sd.automate_all:
-            self._prep_automate_all()
-
-        self._add_platformsh_settings()
+        self._prep_automate_all()
+        self._modify_settings()
         self._add_requirements()
         self._generate_platform_app_yaml()
         self._make_platform_dir()
         self._generate_services_yaml()
+
         self._conclude_automate_all()
         self._show_success_message()
 
     # --- Helper methods for deploy() ---
 
     def _confirm_preliminary(self):
         """Confirm acknwledgement of preliminary (pre-1.0) state of project."""
@@ -94,50 +89,62 @@
         if self.sd.unit_testing:
             # Unit tests don't use the CLI. Use the deployed project name that was
             # passed to the simple_deploy CLI.
             self.deployed_project_name = self.sd.deployed_project_name
             self.sd.log_info(f"Deployed project name: {self.deployed_project_name}")
             return
 
+        self._check_plsh_settings()
         self._validate_cli()
 
         self.deployed_project_name = self._get_platformsh_project_name()
         self.sd.log_info(f"Deployed project name: {self.deployed_project_name}")
 
         self.org_name = self._get_org_name()
         self.sd.log_info(f"\nOrg name: {self.org_name}")
 
-    def _add_platformsh_settings(self):
-        """Add platformsh-specific settings.
+    def _prep_automate_all(self):
+        """Intial work for automating entire process.
 
-        The only project-specific setting is ALLOWED_HOSTS. That makes modifying
-        settings *much* easier than for other platforms. Just check if the settings are
-        present, and if not, dump them in.
+        Returns:
+            None: If creation of new project was successful.
 
-        DEV: Modify this to make a more specific ALLOWED_HOSTS entry instead of "*".
-        """
-        self.sd.write_output(
-            "\n  Checking if Platform.sh-specific settings present in settings.py..."
-        )
+        Raises:
+            SimpleDeployCommandError: If create command fails.
 
-        # PLATFORM_APPLICATION_NAME is an env var that's reliably set in the Platform.sh
-        # environment.
-        # See: https://docs.platform.sh/development/variables/use-variables.html#use-provided-variables
-        settings_string = self.sd.settings_path.read_text()
-        if 'if os.environ.get("PLATFORM_APPLICATION_NAME"):' in settings_string:
-            self.sd.write_output(
-                "\n    Found platform.sh settings block in settings.py."
-            )
+        Note: create command outputs project id to stdout if known, all other
+          output goes to stderr.
+        """
+        if not self.sd.automate_all:
             return
 
-        # Add platformsh settings block.
-        self.sd.write_output(
-            "    No platform.sh settings found in settings.py; adding settings..."
-        )
+        self.sd.write_output("  Running `platform create`...")
+        self.sd.write_output("    (Please be patient, this can take a few minutes.")
+        cmd = f"platform create --title { self.deployed_project_name } --org {self.org_name} --region {self.sd.region} --yes"
+
+        try:
+            # Note: if user can't create a project the returncode will be 6, not 1.
+            #   This may affect whether a CompletedProcess is returned, or an Exception
+            # is raised.
+            # Also, create command outputs project id to stdout if known, all other
+            # output goes to stderr.
+            self.sd.run_slow_command(cmd)
+        except subprocess.CalledProcessError as e:
+            error_msg = self.messages.unknown_create_error(e)
+            raise SimpleDeployCommandError(self.sd, error_msg)
 
+    def _modify_settings(self):
+        """Add platformsh-specific settings.
+
+        This settings block is currently the same for all users. The ALLOWED_HOSTS
+        setting should be customized.
+        """
+        self.sd.write_output("\n  Adding a Platform.sh-specific settings block...")
+
+        settings_string = self.sd.settings_path.read_text()
         safe_settings_string = mark_safe(settings_string)
         context = {"current_settings": safe_settings_string}
         sd_utils.write_file_from_template(self.sd.settings_path, "settings.py", context)
 
         msg = f"    Modified settings.py file: {self.sd.settings_path}"
         self.sd.write_output(msg)
 
@@ -257,46 +264,26 @@
         if self.sd.automate_all:
             msg = self.messages.success_msg_automate_all(self.deployed_url)
             self.sd.write_output(msg)
         else:
             msg = self.messages.success_msg(self.sd.log_output)
             self.sd.write_output(msg)
 
-    # --- Other helper methods ---
-
-    def _prep_automate_all(self):
-        """Intial work for automating entire process.
-
-        Returns:
-            None: If creation of new project was successful.
-
-        Raises:
-            SimpleDeployCommandError: If create command fails.
-
-        Note: create command outputs project id to stdout if known, all other
-          output goes to stderr.
-        """
-
-        self.sd.write_output("  Running `platform create`...")
-        self.sd.write_output("    (Please be patient, this can take a few minutes.")
-        cmd = f"platform create --title { self.deployed_project_name } --org {self.org_name} --region {self.sd.region} --yes"
-
-        try:
-            # Note: if user can't create a project the returncode will be 6, not 1.
-            #   This may affect whether a CompletedProcess is returned, or an Exception
-            # is raised.
-            # Also, create command outputs project id to stdout if known, all other
-            # output goes to stderr.
-            self.sd.run_slow_command(cmd)
-        except subprocess.CalledProcessError as e:
-            error_msg = self.messages.unknown_create_error(e)
-            raise SimpleDeployCommandError(self.sd, error_msg)
-
     # --- Helper methods for methods called from simple_deploy.py ---
 
+    def _check_plsh_settings(self):
+        """Check to see if a Platform.sh settings block already exists."""
+        start_line = "# Platform.sh settings."
+        self.sd.check_settings(
+            "Platform.sh",
+            start_line,
+            self.messages.plsh_settings_found,
+            self.messages.cant_overwrite_settings,
+        )
+
     def _validate_cli(self):
         """Make sure the Platform.sh CLI is installed, and user is authenticated."""
         cmd = "platform --version"
 
         # This generates a FileNotFoundError on Ubuntu if the CLI is not installed.
         try:
             output_obj = self.sd.run_quick_command(cmd)
```

### Comparing `django_simple_deploy-0.6.2/simple_deploy/management/commands/platform_sh/deploy_messages.py` & `django_simple_deploy-0.6.3/simple_deploy/management/commands/platform_sh/deploy_messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,25 @@
 cli_logged_out = """
 You are currently logged out of the Platform.sh CLI. Please log in,
   and then run simple_deploy again.
 You can log in from  the command line:
   $ platform login
 """
 
+plsh_settings_found = """
+There is already a Platform.sh-specific settings block in settings.py. Is it okay to
+overwrite this block, and everything that follows in settings.py?
+"""
+
+cant_overwrite_settings = """
+In order to configure the project for deployment, we need to write a Platform.sh-specific
+settings block. Please remove the current Platform.sh-specific settings, and then run
+simple_deploy again.
+"""
+
 no_project_name = """
 A Platform.sh project name could not be found.
 
 The simple_deploy command expects that you've already run `platform create`, or
 associated the local project with an existing project on Platform.sh.
 
 If you haven't done so, run the `platform create` command and then run
```

### Comparing `django_simple_deploy-0.6.2/simple_deploy/management/commands/platform_sh/templates/pipenv.platform.app.yaml` & `django_simple_deploy-0.6.3/simple_deploy/management/commands/platform_sh/templates/pipenv.platform.app.yaml`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.2/simple_deploy/management/commands/platform_sh/templates/platform.app.yaml` & `django_simple_deploy-0.6.3/simple_deploy/management/commands/platform_sh/templates/platform.app.yaml`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.2/simple_deploy/management/commands/platform_sh/templates/poetry.platform.app.yaml` & `django_simple_deploy-0.6.3/simple_deploy/management/commands/platform_sh/templates/poetry.platform.app.yaml`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.2/simple_deploy/management/commands/platform_sh/templates/settings.py` & `django_simple_deploy-0.6.3/simple_deploy/management/commands/platform_sh/templates/settings.py`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.2/simple_deploy/management/commands/platform_sh/tests/unit_tests/resources/projects_info_output_csv.txt` & `django_simple_deploy-0.6.3/simple_deploy/management/commands/platform_sh/tests/unit_tests/resources/projects_info_output_csv.txt`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.2/simple_deploy/management/commands/platform_sh/tests/unit_tests/test_plsh_utils.py` & `django_simple_deploy-0.6.3/simple_deploy/management/commands/platform_sh/tests/unit_tests/test_plsh_utils.py`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.2/simple_deploy/management/commands/platform_sh/utils.py` & `django_simple_deploy-0.6.3/simple_deploy/management/commands/platform_sh/utils.py`

 * *Files identical despite different names*

### Comparing `django_simple_deploy-0.6.2/simple_deploy/management/commands/simple_deploy.py` & `django_simple_deploy-0.6.3/simple_deploy/management/commands/simple_deploy.py`

 * *Files 0% similar despite different names*

```diff
@@ -251,15 +251,15 @@
             elif confirmed.lower() in ("n", "no"):
                 return False
             else:
                 self.write_output(
                     "  Please answer yes or no.", skip_logging=skip_logging
                 )
 
-    def check_settings(self, platform, start_line, msg_found, msg_cant_overwrite):
+    def check_settings(self, platform_name, start_line, msg_found, msg_cant_overwrite):
         """Check if a platform-specific settings block already exists.
 
         If so, ask if we can overwrite that block. This is much simpler than trying to
         keep track of individual settings.
 
         Returns:
             None
@@ -270,25 +270,25 @@
         """
         settings_text = self.settings_path.read_text()
 
         re_platform_settings = f"(.*)({start_line})(.*)"
         m = re.match(re_platform_settings, settings_text, re.DOTALL)
         
         if not m:
-            self.log_info(f"No {platform.title()}-specific settings block found.")
+            self.log_info(f"No {platform_name}-specific settings block found.")
             return
 
         # A platform-specific settings block exists. Get permission to overwrite it.
         if not self.get_confirmation(msg_found):
             raise sd_utils.SimpleDeployCommandError(self, msg_cant_overwrite)
 
         # Platform-specific settings exist, but we can remove them and start fresh.
         self.settings_path.write_text(m.group(1))
 
-        msg = f"  Removed existing {platform.title()}-specific settings block."
+        msg = f"  Removed existing {platform_name}-specific settings block."
         self.write_output(msg)
 
 
     def add_packages(self, package_list):
         """Add a set of packages to the project's requirements.
 
         This is a simple wrapper for add_package(), to make it easier to add multiple
```

### Comparing `django_simple_deploy-0.6.2/simple_deploy/management/commands/utils.py` & `django_simple_deploy-0.6.3/simple_deploy/management/commands/utils.py`

 * *Files identical despite different names*

