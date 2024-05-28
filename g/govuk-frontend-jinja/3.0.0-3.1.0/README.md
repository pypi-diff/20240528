# Comparing `tmp/govuk-frontend-jinja-3.0.0.tar.gz` & `tmp/govuk_frontend_jinja-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "govuk-frontend-jinja-3.0.0.tar", last modified: Thu Feb  8 16:06:57 2024, max compression
+gzip compressed data, was "govuk_frontend_jinja-3.1.0.tar", last modified: Tue May 28 13:37:18 2024, max compression
```

## Comparing `govuk-frontend-jinja-3.0.0.tar` & `govuk_frontend_jinja-3.1.0.tar`

### file list

```diff
@@ -1,87 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:06:57.962365 govuk-frontend-jinja-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-02-08 16:06:19.000000 govuk-frontend-jinja-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10688 2024-02-08 16:06:57.962365 govuk-frontend-jinja-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9663 2024-02-08 16:06:19.000000 govuk-frontend-jinja-3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:06:57.954365 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 16:06:19.000000 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:06:57.954365 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:06:57.954365 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:06:57.954365 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/accordion/
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-02-08 16:06:19.000000 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/accordion/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:06:57.954365 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/back-link/
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-02-08 16:06:19.000000 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/back-link/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:06:57.954365 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/breadcrumbs/
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-02-08 16:06:19.000000 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/breadcrumbs/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:06:57.954365 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/button/
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-02-08 16:06:19.000000 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/button/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:06:57.954365 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/character-count/
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-02-08 16:06:19.000000 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/character-count/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:06:57.954365 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/checkboxes/
--rw-r--r--   0 runner    (1001) docker     (127)     6056 2024-02-08 16:06:19.000000 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/checkboxes/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:06:57.958365 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/cookie-banner/
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-02-08 16:06:19.000000 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/cookie-banner/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:06:57.958365 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/date-input/
--rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-02-08 16:06:19.000000 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/date-input/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:06:57.958365 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/details/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-02-08 16:06:19.000000 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/details/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:06:57.958365 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/error-message/
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-02-08 16:06:19.000000 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/error-message/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:06:57.958365 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/error-summary/
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-02-08 16:06:19.000000 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/error-summary/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:06:57.958365 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/exit-this-page/
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-02-08 16:06:19.000000 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/exit-this-page/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:06:57.958365 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/fieldset/
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-02-08 16:06:19.000000 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/fieldset/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:06:57.958365 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/file-upload/
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-02-08 16:06:19.000000 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/file-upload/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:06:57.958365 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/footer/
--rw-r--r--   0 runner    (1001) docker     (127)     5007 2024-02-08 16:06:19.000000 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/footer/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:06:57.958365 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/header/
--rw-r--r--   0 runner    (1001) docker     (127)    10258 2024-02-08 16:06:19.000000 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/header/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:06:57.958365 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/hint/
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-02-08 16:06:19.000000 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/hint/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:06:57.958365 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/input/
--rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-02-08 16:06:19.000000 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/input/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:06:57.958365 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/inset-text/
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-02-08 16:06:19.000000 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/inset-text/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:06:57.958365 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/label/
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-02-08 16:06:19.000000 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/label/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:06:57.958365 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/notification-banner/
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-02-08 16:06:19.000000 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/notification-banner/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:06:57.958365 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/pagination/
--rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-02-08 16:06:19.000000 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/pagination/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:06:57.958365 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/panel/
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-02-08 16:06:19.000000 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/panel/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:06:57.958365 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/phase-banner/
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-02-08 16:06:19.000000 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/phase-banner/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:06:57.958365 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/radios/
--rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-02-08 16:06:19.000000 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/radios/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:06:57.958365 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/select/
--rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-02-08 16:06:19.000000 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/select/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:06:57.958365 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/skip-link/
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-02-08 16:06:19.000000 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/skip-link/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:06:57.958365 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/summary-list/
--rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-02-08 16:06:19.000000 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/summary-list/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:06:57.958365 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/table/
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-02-08 16:06:19.000000 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/table/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:06:57.962365 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/tabs/
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-02-08 16:06:19.000000 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/tabs/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:06:57.962365 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/tag/
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-02-08 16:06:19.000000 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/tag/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:06:57.962365 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/task-list/
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-02-08 16:06:19.000000 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/task-list/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:06:57.962365 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/textarea/
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-02-08 16:06:19.000000 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/textarea/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:06:57.962365 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/warning-text/
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-02-08 16:06:19.000000 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/warning-text/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:06:57.962365 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/macros/
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-02-08 16:06:19.000000 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/macros/i18n.html
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-02-08 16:06:19.000000 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/template.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:06:57.962365 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10688 2024-02-08 16:06:57.000000 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-02-08 16:06:57.000000 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-08 16:06:57.000000 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-08 16:06:57.000000 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-08 16:06:57.000000 govuk-frontend-jinja-3.0.0/govuk_frontend_jinja.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-02-08 16:06:57.962365 govuk-frontend-jinja-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-02-08 16:06:19.000000 govuk-frontend-jinja-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:37:18.503172 govuk_frontend_jinja-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-28 13:37:10.000000 govuk_frontend_jinja-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11008 2024-05-28 13:37:18.503172 govuk_frontend_jinja-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9983 2024-05-28 13:37:10.000000 govuk_frontend_jinja-3.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:37:18.495172 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 13:37:10.000000 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:37:18.495172 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:37:18.491172 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:37:18.495172 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/accordion/
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-05-28 13:37:10.000000 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/accordion/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:37:18.495172 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/back-link/
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-28 13:37:10.000000 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/back-link/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:37:18.495172 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/breadcrumbs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-28 13:37:10.000000 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/breadcrumbs/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:37:18.495172 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/button/
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-05-28 13:37:10.000000 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/button/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:37:18.495172 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/character-count/
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-05-28 13:37:10.000000 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/character-count/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:37:18.495172 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/checkboxes/
+-rw-r--r--   0 runner    (1001) docker     (127)     6080 2024-05-28 13:37:10.000000 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/checkboxes/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:37:18.495172 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/cookie-banner/
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-05-28 13:37:10.000000 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/cookie-banner/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:37:18.495172 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/date-input/
+-rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-05-28 13:37:10.000000 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/date-input/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:37:18.495172 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/details/
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-28 13:37:10.000000 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/details/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:37:18.495172 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/error-message/
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-28 13:37:10.000000 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/error-message/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:37:18.499172 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/error-summary/
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-28 13:37:10.000000 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/error-summary/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:37:18.499172 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/exit-this-page/
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-28 13:37:10.000000 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/exit-this-page/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:37:18.499172 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/fieldset/
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-28 13:37:10.000000 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/fieldset/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:37:18.499172 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/file-upload/
+-rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-05-28 13:37:10.000000 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/file-upload/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:37:18.499172 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/footer/
+-rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-05-28 13:37:10.000000 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/footer/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:37:18.499172 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/header/
+-rw-r--r--   0 runner    (1001) docker     (127)    10257 2024-05-28 13:37:10.000000 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/header/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:37:18.499172 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/hint/
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-28 13:37:10.000000 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/hint/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:37:18.499172 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/input/
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-05-28 13:37:10.000000 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/input/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:37:18.499172 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/inset-text/
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-28 13:37:10.000000 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/inset-text/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:37:18.499172 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/label/
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-28 13:37:10.000000 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/label/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:37:18.499172 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/notification-banner/
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-28 13:37:10.000000 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/notification-banner/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:37:18.499172 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/pagination/
+-rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-05-28 13:37:10.000000 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/pagination/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:37:18.499172 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/panel/
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-28 13:37:10.000000 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/panel/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:37:18.499172 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/password-input/
+-rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-05-28 13:37:10.000000 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/password-input/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:37:18.499172 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/phase-banner/
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-28 13:37:10.000000 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/phase-banner/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:37:18.499172 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/radios/
+-rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-05-28 13:37:10.000000 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/radios/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:37:18.499172 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/select/
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-05-28 13:37:10.000000 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/select/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:37:18.499172 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/skip-link/
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-28 13:37:10.000000 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/skip-link/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:37:18.499172 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/summary-list/
+-rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-05-28 13:37:10.000000 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/summary-list/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:37:18.499172 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/table/
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-28 13:37:10.000000 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/table/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:37:18.499172 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/tabs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-28 13:37:10.000000 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/tabs/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:37:18.499172 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/tag/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-28 13:37:10.000000 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/tag/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:37:18.503172 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/task-list/
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-28 13:37:10.000000 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/task-list/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:37:18.503172 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/textarea/
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-05-28 13:37:10.000000 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/textarea/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:37:18.503172 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/warning-text/
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-28 13:37:10.000000 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/warning-text/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:37:18.503172 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/macros/
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-05-28 13:37:10.000000 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/macros/attributes.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-28 13:37:10.000000 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/macros/i18n.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-05-28 13:37:10.000000 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/template.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:37:18.503172 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11008 2024-05-28 13:37:18.000000 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-05-28 13:37:18.000000 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 13:37:18.000000 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-28 13:37:18.000000 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-28 13:37:18.000000 govuk_frontend_jinja-3.1.0/govuk_frontend_jinja.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-28 13:37:18.503172 govuk_frontend_jinja-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-28 13:37:10.000000 govuk_frontend_jinja-3.1.0/setup.py
```

### Comparing `govuk-frontend-jinja-3.0.0/LICENSE` & `govuk_frontend_jinja-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `govuk-frontend-jinja-3.0.0/PKG-INFO` & `govuk_frontend_jinja-3.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: govuk-frontend-jinja
-Version: 3.0.0
+Version: 3.1.0
 Summary: GOV.UK Frontend Jinja Macros
 Home-page: https://github.com/LandRegistry/govuk-frontend-jinja
 Author: Matt Shaw
 Author-email: matthew.shaw@landregistry.gov.uk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -22,39 +22,41 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: jinja2!=3.0.0,!=3.0.1
 
 # GOV.UK Frontend Jinja Macros
 
 [![PyPI version](https://badge.fury.io/py/govuk-frontend-jinja.svg)](https://pypi.org/project/govuk-frontend-jinja/)
-![govuk-frontend 5.1.0](https://img.shields.io/badge/govuk--frontend%20version-5.1.0-005EA5?logo=gov.uk&style=flat)
+![govuk-frontend 5.4.0](https://img.shields.io/badge/govuk--frontend%20version-5.4.0-005EA5?logo=gov.uk&style=flat)
 [![Python package](https://github.com/LandRegistry/govuk-frontend-jinja/actions/workflows/python-package.yml/badge.svg)](https://github.com/LandRegistry/govuk-frontend-jinja/actions/workflows/python-package.yml)
 
 **GOV.UK Frontend Jinja is a [community tool](https://design-system.service.gov.uk/community/resources-and-tools/) of the [GOV.UK Design System](https://design-system.service.gov.uk/). The Design System team is not responsible for it and cannot support you with using it. Contact the [maintainers](#contributors) directly if you need [help](#support) or you want to request a feature.**
 
 This repository provides a complete set of [Jinja](https://jinja.palletsprojects.com/) macros that are kept up-to-date and 100% compliant with the original [GOV.UK Frontend](https://github.com/alphagov/govuk-frontend) Nunjucks macros. Porting is intentionally manual rather than automated to make updates simpler than maintaining an automated conversion routine. A [comprehensive test suite](https://github.com/matthew-shaw/govuk-frontend-diff) ensures compliance against the latest, and every subsequent, GOV.UK Frontend release.
 
 If you are looking to build a fully featured Flask app that integrates with [GOV.UK Frontend Jinja](https://github.com/LandRegistry/govuk-frontend-jinja) and [GOV.UK Frontend WTForms](https://github.com/LandRegistry/govuk-frontend-wtf) please use the [GOV.UK Frontend Flask](https://github.com/LandRegistry/govuk-frontend-flask) template repository to [generate your app](https://github.com/LandRegistry/govuk-frontend-flask/generate).
 
 ## Compatibility
 
 The following table shows the version of GOV.UK Frontend Jinja that you should use for your targeted version of GOV.UK Frontend:
 
 | GOV.UK Frontend Jinja Version | Target GOV.UK Frontend Version |
 | ----------------------------- | ------------------------------ |
+| [3.1.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/3.1.0) | [5.4.0](https://github.com/alphagov/govuk-frontend/releases/tag/v5.4.0) |
 | [3.0.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/3.0.0) | [5.1.0](https://github.com/alphagov/govuk-frontend/releases/tag/v5.1.0) |
 | [2.8.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.8.0) | [4.8.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.8.0) |
 | [2.7.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.7.0) | [4.7.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.7.0) |
 | [2.6.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.6.0) | [4.6.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.6.0) |
 | [2.5.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.5.0) | [4.5.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.5.0) |
 | [2.4.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.4.0) | [4.4.1](https://github.com/alphagov/govuk-frontend/releases/tag/v4.4.1) |
 | [2.3.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.3.0) | [4.2.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.2.0) |
 | [2.2.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.2.0) | [4.1.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.1.0) |
 | [2.1.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.1.0) | [4.0.1](https://github.com/alphagov/govuk-frontend/releases/tag/v4.0.1) |
 | [2.0.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.0.0) | [4.0.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.0.0) |
+| [1.6.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/1.6.0) | [3.15.0](https://github.com/alphagov/govuk-frontend/releases/tag/v3.15.0) |
 | [1.5.1](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/1.5.1) | [3.14.0](https://github.com/alphagov/govuk-frontend/releases/tag/v3.14.0) |
 | [1.4.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/1.4.0) | [3.13.0](https://github.com/alphagov/govuk-frontend/releases/tag/v3.13.0) |
 | [1.3.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/1.3.0) | [3.12.0](https://github.com/alphagov/govuk-frontend/releases/tag/v3.12.0) |
 | [1.2.1](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/1.2.1) | [3.11.0](https://github.com/alphagov/govuk-frontend/releases/tag/v3.11.0) |
 | [1.1.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/1.1.0) | [3.10.2](https://github.com/alphagov/govuk-frontend/releases/tag/v3.10.2) |
 | [1.0.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/1.0.0) | [3.8.1](https://github.com/alphagov/govuk-frontend/releases/tag/v3.8.1) |
 | [0.2.1](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/0.2.1) | [3.7.0](https://github.com/alphagov/govuk-frontend/releases/tag/v3.7.0) |
```

### Comparing `govuk-frontend-jinja-3.0.0/README.md` & `govuk_frontend_jinja-3.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 # GOV.UK Frontend Jinja Macros
 
 [![PyPI version](https://badge.fury.io/py/govuk-frontend-jinja.svg)](https://pypi.org/project/govuk-frontend-jinja/)
-![govuk-frontend 5.1.0](https://img.shields.io/badge/govuk--frontend%20version-5.1.0-005EA5?logo=gov.uk&style=flat)
+![govuk-frontend 5.4.0](https://img.shields.io/badge/govuk--frontend%20version-5.4.0-005EA5?logo=gov.uk&style=flat)
 [![Python package](https://github.com/LandRegistry/govuk-frontend-jinja/actions/workflows/python-package.yml/badge.svg)](https://github.com/LandRegistry/govuk-frontend-jinja/actions/workflows/python-package.yml)
 
 **GOV.UK Frontend Jinja is a [community tool](https://design-system.service.gov.uk/community/resources-and-tools/) of the [GOV.UK Design System](https://design-system.service.gov.uk/). The Design System team is not responsible for it and cannot support you with using it. Contact the [maintainers](#contributors) directly if you need [help](#support) or you want to request a feature.**
 
 This repository provides a complete set of [Jinja](https://jinja.palletsprojects.com/) macros that are kept up-to-date and 100% compliant with the original [GOV.UK Frontend](https://github.com/alphagov/govuk-frontend) Nunjucks macros. Porting is intentionally manual rather than automated to make updates simpler than maintaining an automated conversion routine. A [comprehensive test suite](https://github.com/matthew-shaw/govuk-frontend-diff) ensures compliance against the latest, and every subsequent, GOV.UK Frontend release.
 
 If you are looking to build a fully featured Flask app that integrates with [GOV.UK Frontend Jinja](https://github.com/LandRegistry/govuk-frontend-jinja) and [GOV.UK Frontend WTForms](https://github.com/LandRegistry/govuk-frontend-wtf) please use the [GOV.UK Frontend Flask](https://github.com/LandRegistry/govuk-frontend-flask) template repository to [generate your app](https://github.com/LandRegistry/govuk-frontend-flask/generate).
 
 ## Compatibility
 
 The following table shows the version of GOV.UK Frontend Jinja that you should use for your targeted version of GOV.UK Frontend:
 
 | GOV.UK Frontend Jinja Version | Target GOV.UK Frontend Version |
 | ----------------------------- | ------------------------------ |
+| [3.1.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/3.1.0) | [5.4.0](https://github.com/alphagov/govuk-frontend/releases/tag/v5.4.0) |
 | [3.0.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/3.0.0) | [5.1.0](https://github.com/alphagov/govuk-frontend/releases/tag/v5.1.0) |
 | [2.8.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.8.0) | [4.8.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.8.0) |
 | [2.7.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.7.0) | [4.7.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.7.0) |
 | [2.6.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.6.0) | [4.6.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.6.0) |
 | [2.5.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.5.0) | [4.5.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.5.0) |
 | [2.4.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.4.0) | [4.4.1](https://github.com/alphagov/govuk-frontend/releases/tag/v4.4.1) |
 | [2.3.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.3.0) | [4.2.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.2.0) |
 | [2.2.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.2.0) | [4.1.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.1.0) |
 | [2.1.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.1.0) | [4.0.1](https://github.com/alphagov/govuk-frontend/releases/tag/v4.0.1) |
 | [2.0.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.0.0) | [4.0.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.0.0) |
+| [1.6.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/1.6.0) | [3.15.0](https://github.com/alphagov/govuk-frontend/releases/tag/v3.15.0) |
 | [1.5.1](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/1.5.1) | [3.14.0](https://github.com/alphagov/govuk-frontend/releases/tag/v3.14.0) |
 | [1.4.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/1.4.0) | [3.13.0](https://github.com/alphagov/govuk-frontend/releases/tag/v3.13.0) |
 | [1.3.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/1.3.0) | [3.12.0](https://github.com/alphagov/govuk-frontend/releases/tag/v3.12.0) |
 | [1.2.1](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/1.2.1) | [3.11.0](https://github.com/alphagov/govuk-frontend/releases/tag/v3.11.0) |
 | [1.1.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/1.1.0) | [3.10.2](https://github.com/alphagov/govuk-frontend/releases/tag/v3.10.2) |
 | [1.0.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/1.0.0) | [3.8.1](https://github.com/alphagov/govuk-frontend/releases/tag/v3.8.1) |
 | [0.2.1](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/0.2.1) | [3.7.0](https://github.com/alphagov/govuk-frontend/releases/tag/v3.7.0) |
```

### Comparing `govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/accordion/macro.html` & `govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/accordion/macro.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 {% macro govukAccordion(params) %}
+{% from "govuk_frontend_jinja/macros/attributes.html" import govukAttributes %}
 {% from "govuk_frontend_jinja/macros/i18n.html" import govukI18nAttributes %}
 
 {%- macro _accordionItem(params, item, index) %}
   {%- set headingLevel = params.headingLevel if params.headingLevel else 2 %}
   <div class="govuk-accordion__section {%- if item.expanded %} govuk-accordion__section--expanded{% endif %}">
     <div class="govuk-accordion__section-header">
       <h{{ headingLevel }} class="govuk-accordion__section-heading">
@@ -56,13 +57,13 @@
 
   {{- govukI18nAttributes({
     'key': 'show-section-aria-label',
     'message': params.showSectionAriaLabelText
   }) -}}
 
   {%- if params.rememberExpanded is not undefined %} data-remember-expanded="{{ params.rememberExpanded | escape | lower }}"{% endif %}
-  {%- for attribute, value in (params.attributes.items() if params.attributes else {}.items()) %} {{ attribute }}="{{ value }}"{% endfor %}>
+  {{- govukAttributes(params.attributes) }}>
   {% for item in params['items'] %}
     {% if item %}{{ _accordionItem(params, item, loop.index) }}{% endif %}
   {% endfor %}
 </div>
 {% endmacro %}
```

### Comparing `govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/button/macro.html` & `govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/button/macro.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 {% macro govukButton(params) %}
-{# Set classes for this component #}
+{% from "govuk_frontend_jinja/macros/attributes.html" import govukAttributes %}
+
+{#- Set classes for this component #}
 {%- set classNames = "govuk-button" -%}
 
 {%- if params.classes %}
-  {% set classNames = classNames + " " + params.classes %}
+  {% set classNames = classNames ~ " " ~ params.classes %}
 {% endif %}
 
 {%- if params.isStartButton %}
-  {% set classNames = classNames + " govuk-button--start" %}
+  {% set classNames = classNames ~ " govuk-button--start" %}
 {% endif %}
 
 {#- Determine type of element to use, if not explicitly set #}
 {%- if params.element %}
   {% set element = params.element | lower %}
 {% else %}
   {% if params.href %}
@@ -28,15 +30,15 @@
   <svg class="govuk-button__start-icon" xmlns="http://www.w3.org/2000/svg" width="17.5" height="19" viewBox="0 0 33 40" aria-hidden="true" focusable="false">
     <path fill="currentColor" d="M0 0h13l20 20-20 20H0l20-20z"/>
   </svg>
 {%- endmacro -%}
 
 {#- Define common attributes that we can use across all element types #}
 
-{%- set commonAttributes %} class="{{ classNames }}" data-module="govuk-button" {%- for attribute, value in (params.attributes.items() if params.attributes else {}.items()) %} {{ attribute }}="{{ value }}"{% endfor %}{% if params.id %} id="{{ params.id }}"{% endif %}{% endset %}
+{%- set commonAttributes %} class="{{ classNames }}" data-module="govuk-button" {{- govukAttributes(params.attributes) -}} {% if params.id %} id="{{ params.id }}"{% endif %}{% endset %}
 
 {#- Define common attributes we can use for both button and input types #}
 
 {%- set buttonAttributes %}{% if params.name %} name="{{ params.name }}"{% endif %}{% if params.disabled %} disabled aria-disabled="true"{% endif %}{% if params.preventDoubleClick is not undefined %} data-prevent-double-click="{{ params.preventDoubleClick | lower }}"{% endif %}{% endset %}
 
 {#- Actually create a button... or a link! #}
```

#### html2text {}

```diff
@@ -1,29 +1,28 @@
-{% macro govukButton(params) %} {# Set classes for this component #} {%- set
-classNames = "govuk-button" -%} {%- if params.classes %} {% set classNames =
-classNames + " " + params.classes %} {% endif %} {%- if params.isStartButton %}
-{% set classNames = classNames + " govuk-button--start" %} {% endif %} {#-
-Determine type of element to use, if not explicitly set #} {%- if
-params.element %} {% set element = params.element | lower %} {% else %} {% if
-params.href %} {% set element = 'a' %} {% else %} {% set element = 'button' %}
-{% endif %} {% endif -%} {%- macro _startIcon() %} {#- The SVG needs
-`focusable="false"` so that Internet Explorer does not treat it as an
+{% macro govukButton(params) %} {% from "govuk_frontend_jinja/macros/
+attributes.html" import govukAttributes %} {#- Set classes for this component
+#} {%- set classNames = "govuk-button" -%} {%- if params.classes %} {% set
+classNames = classNames ~ " " ~ params.classes %} {% endif %} {%- if
+params.isStartButton %} {% set classNames = classNames ~ " govuk-button--start"
+%} {% endif %} {#- Determine type of element to use, if not explicitly set #}
+{%- if params.element %} {% set element = params.element | lower %} {% else %}
+{% if params.href %} {% set element = 'a' %} {% else %} {% set element =
+'button' %} {% endif %} {% endif -%} {%- macro _startIcon() %} {#- The SVG
+needs `focusable="false"` so that Internet Explorer does not treat it as an
 interactive element - without this it will be 'focusable' when using the
 keyboard to navigate. #} {%- endmacro -%} {#- Define common attributes that we
 can use across all element types #} {%- set commonAttributes %} class="{
-{ classNames }}" data-module="govuk-button" {%- for attribute, value in
-(params.attributes.items() if params.attributes else {}.items()) %} {
-{ attribute }}="{{ value }}"{% endfor %}{% if params.id %} id="{{ params.id }}"
-{% endif %}{% endset %} {#- Define common attributes we can use for both button
-and input types #} {%- set buttonAttributes %}{% if params.name %} name="{
-{ params.name }}"{% endif %}{% if params.disabled %} disabled aria-
-disabled="true"{% endif %}{% if params.preventDoubleClick is not undefined %}
-data-prevent-double-click="{{ params.preventDoubleClick | lower }}"{% endif %}
-{% endset %} {#- Actually create a button... or a link! #} {%- if element ==
-'a' %}
+{ classNames }}" data-module="govuk-button" {{- govukAttributes
+(params.attributes) -}} {% if params.id %} id="{{ params.id }}"{% endif %}{%
+endset %} {#- Define common attributes we can use for both button and input
+types #} {%- set buttonAttributes %}{% if params.name %} name="{{ params.name
+}}"{% endif %}{% if params.disabled %} disabled aria-disabled="true"{% endif %}
+{% if params.preventDoubleClick is not undefined %} data-prevent-double-click="
+{{ params.preventDoubleClick | lower }}"{% endif %}{% endset %} {#- Actually
+create a button... or a link! #} {%- if element == 'a' %}
 {- commonAttributes | safe }}> {{ params.html | safe | trim | indent(2) if
 params.html else params.text }} {{- _startIcon() | safe if params.isStartButton
 }}
 {%- elif element == 'button' %}
 %- if params.value %} value="{{ params.value }}"{% endif %} type="{
 { params.type if params.type else 'submit' }}" {{- buttonAttributes | safe }} {
 {- commonAttributes | safe }}> {{ params.html | safe | trim | indent(2) if
```

### Comparing `govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/checkboxes/macro.html` & `govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/checkboxes/macro.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 {% macro govukCheckboxes(params) %}
+{% from "govuk_frontend_jinja/macros/attributes.html" import govukAttributes %}
 {% from "govuk_frontend_jinja/components/error-message/macro.html" import govukErrorMessage %}
 {% from "govuk_frontend_jinja/components/fieldset/macro.html" import govukFieldset %}
 {% from "govuk_frontend_jinja/components/hint/macro.html" import govukHint %}
 {% from "govuk_frontend_jinja/components/label/macro.html" import govukLabel %}
 
 {#- If an id 'prefix' is not passed, fall back to using the name attribute
   instead. We need this for error messages and hints as well -#}
@@ -16,101 +17,104 @@
 {% if params.fieldset and params.fieldset.describedBy %}
   {% set ns.describedBy = params.fieldset.describedBy %}
 {% endif %}
 
 {#- fieldset is false by default -#}
 {% set hasFieldset = true if params.fieldset else false %}
 
+{%- macro _checkboxItem(params, item, index) %}
+  {#- If the user explicitly sets an id, use this instead of the regular idPrefix -#}
+  {#- The first id should not have a number suffix so it's easy to link to from the error summary component -#}
+  {% set itemId = item.id if item.id else idPrefix ~ ("-" ~ index if index > 1 else "") %}
+  {% set itemName = item.name if item.name else params.name %}
+  {% set conditionalId = "conditional-" ~ itemId %}
+  {%- if item.divider %}
+    <div class="govuk-checkboxes__divider">{{ item.divider }}</div>
+  {% else %}
+    {% set isChecked = item.checked | default((item.value in params.get('values', []) and item.checked is not false) if params.values else false, true) %}
+    {% set hasHint = true if item.hint and (item.hint.text or item.hint.html) %}
+    {% set itemHintId = itemId ~ "-item-hint" if hasHint else "" %}
+    {% set itemDescribedBy = ns.describedBy if not hasFieldset else "" %}
+    {% set itemDescribedBy = (itemDescribedBy ~ " " ~ itemHintId) | trim %}
+    <div class="govuk-checkboxes__item">
+      <input class="govuk-checkboxes__input" id="{{ itemId }}" name="{{ itemName }}" type="checkbox" value="{{ item.value }}"
+        {{-" checked" if isChecked }}
+        {{-" disabled" if item.disabled }}
+        {%- if item.conditional and item.conditional.html %} data-aria-controls="{{ conditionalId }}"{% endif -%}
+        {%- if item.behaviour %} data-behaviour="{{ item.behaviour }}"{% endif -%}
+        {%- if itemDescribedBy %} aria-describedby="{{ itemDescribedBy }}"{% endif -%}
+        {{- govukAttributes(item.attributes) }}>
+      {{ govukLabel({
+        'html': item.html,
+        'text': item.text,
+        'classes': 'govuk-checkboxes__label' ~ (' ' ~ item.label.classes if item.label and item.label.classes else ""),
+        'attributes': item.label.attributes if item.label,
+        'for': itemId
+      }) | trim | indent(6) }}
+      {% if hasHint %}
+      {{ govukHint({
+        'id': itemHintId,
+        'classes': 'govuk-checkboxes__hint' ~ (' ' ~ item.hint.classes if item.hint and item.hint.classes else ""),
+        'attributes': item.hint.attributes if item.hint,
+        'html': item.hint.html,
+        'text': item.hint.text
+      }) | trim | indent(6) }}
+      {% endif %}
+    </div>
+    {% if item.conditional and item.conditional.html %}
+    <div class="govuk-checkboxes__conditional {%- if not isChecked %} govuk-checkboxes__conditional--hidden{% endif %}" id="{{ conditionalId }}">
+      {{ item.conditional.html | safe | trim }}
+    </div>
+    {% endif %}
+  {% endif %}
+{% endmacro -%}
+
 {#- Capture the HTML so we can optionally nest it in a fieldset -#}
 {% set innerHtml %}
 {% if params.hint %}
-  {% set hintId = idPrefix + '-hint' %}
-  {% set ns.describedBy = ns.describedBy + ' ' + hintId if ns.describedBy else hintId %}
+  {% set hintId = idPrefix ~ '-hint' %}
+  {% set ns.describedBy = ns.describedBy ~ ' ' ~ hintId if ns.describedBy else hintId %}
   {{ govukHint({
     'id': hintId,
     'classes': params.hint.classes,
     'attributes': params.hint.attributes,
     'html': params.hint.html,
     'text': params.hint.text
   }) | trim | indent(2) }}
 {% endif %}
 {% if params.errorMessage %}
-  {% set errorId = idPrefix + '-error' %}
-  {% set ns.describedBy = ns.describedBy + ' ' + errorId if ns.describedBy else errorId %}
+  {% set errorId = idPrefix ~ '-error' %}
+  {% set ns.describedBy = ns.describedBy ~ ' ' ~ errorId if ns.describedBy else errorId %}
   {{ govukErrorMessage({
     'id': errorId,
     'classes': params.errorMessage.classes,
     'attributes': params.errorMessage.attributes,
     'html': params.errorMessage.html,
     'text': params.errorMessage.text,
     'visuallyHiddenText': params.errorMessage.visuallyHiddenText
   }) | trim | indent(2) }}
 {% endif %}
   <div class="govuk-checkboxes {%- if params.classes %} {{ params.classes }}{% endif %}"
-    {%- for attribute, value in (params.attributes.items() if params.attributes else {}.items()) %} {{ attribute }}="{{ value }}"{% endfor %} data-module="govuk-checkboxes">
+    {{- govukAttributes(params.attributes) }} data-module="govuk-checkboxes">
+    {% if params.formGroup and params.formGroup.beforeInputs %}
+    {{ params.formGroup.beforeInputs.html | safe | trim | indent(4) if params.formGroup and params.formGroup.beforeInputs.html else params.formGroup.beforeInputs.text }}
+    {% endif %}
     {% for item in params['items'] %}
       {% if item %}
-        {#- If the user explicitly sets an id, use this instead of the regular idPrefix -#}
-        {%- if item.id -%}
-          {%- set id = item.id -%}
-        {%- else -%}
-          {#- The first id should not have a number suffix so it's easy to link to from the error summary component -#}
-          {%- if loop.first -%}
-            {%- set id = idPrefix %}
-          {% else %}
-            {%- set id = idPrefix + "-" ~ loop.index -%}
-          {%- endif -%}
-        {%- endif -%}
-        {% set name = item.name if item.name else params.name %}
-        {% set conditionalId = "conditional-" + id %}
-        {%- if item.divider %}
-          <div class="govuk-checkboxes__divider">{{ item.divider }}</div>
-        {%- else %}
-          {% set isChecked = item.checked | default((item.value in params.get('values', []) and item.checked != false) if params.values else false, true) %}
-          {% set hasHint = true if item.hint and (item.hint.text or item.hint.html) %}
-          {% set itemHintId = id + "-item-hint" if hasHint else "" %}
-          {% set itemDescribedBy = ns.describedBy if not hasFieldset else "" %}
-          {% set itemDescribedBy = (itemDescribedBy + " " + itemHintId) | trim %}
-          <div class="govuk-checkboxes__item">
-            <input class="govuk-checkboxes__input" id="{{ id }}" name="{{ name }}" type="checkbox" value="{{ item.value }}"
-            {{-" checked" if isChecked }}
-            {{-" disabled" if item.disabled }}
-            {%- if item.conditional and item.conditional.html %} data-aria-controls="{{ conditionalId }}"{% endif -%}
-            {%- if item.behaviour %} data-behaviour="{{ item.behaviour }}"{% endif -%}
-            {%- if itemDescribedBy %} aria-describedby="{{ itemDescribedBy }}"{% endif -%}
-            {%- for attribute, value in (item.attributes.items() if item.attributes else {}.items()) %} {{ attribute }}="{{ value }}"{% endfor %}>
-            {{ govukLabel({
-              'html': item.html,
-              'text': item.text,
-              'classes': 'govuk-checkboxes__label' + (' ' + item.label.classes if item.label and item.label.classes else ''),
-              'attributes': item.label.attributes if item.label,
-              'for': id
-            }) | trim | indent(6) }}
-            {% if hasHint %}
-            {{ govukHint({
-              'id': itemHintId,
-              'classes': 'govuk-checkboxes__hint' + (' ' + item.hint.classes if item.hint.classes else ''),
-              'attributes': item.hint.attributes,
-              'html': item.hint.html,
-              'text': item.hint.text
-            }) | trim | indent(6) }}
-            {% endif %}
-          </div>
-          {% if item.conditional and item.conditional.html %}
-            <div class="govuk-checkboxes__conditional {%- if not isChecked %} govuk-checkboxes__conditional--hidden{% endif %}" id="{{ conditionalId }}">
-              {{ item.conditional.html | safe }}
-            </div>
-          {% endif %}
-        {% endif %}
+        {{- _checkboxItem(params, item, loop.index) -}}
       {% endif %}
     {% endfor %}
+    {% if params.formGroup and params.formGroup.afterInputs %}
+    {{ params.formGroup.afterInputs.html | safe | trim | indent(4) if params.formGroup and params.formGroup.afterInputs.html else params.formGroup.afterInputs.text }}
+    {% endif %}
   </div>
 {% endset -%}
 
-<div class="govuk-form-group {%- if params.errorMessage %} govuk-form-group--error{% endif %} {%- if params.formGroup and params.formGroup.classes %} {{ params.formGroup.classes }}{% endif %}" {%- for attribute, value in (params.formGroup.attributes.items() if params.formGroup and params.formGroup.attributes else {}.items()) %} {{ attribute }}="{{ value }}"{% endfor %}>
+<div class="govuk-form-group {%- if params.errorMessage %} govuk-form-group--error{% endif %} {%- if params.formGroup and params.formGroup.classes %} {{ params.formGroup.classes }}{% endif %}"
+  {{- govukAttributes(params.formGroup.attributes if params.formGroup) }}>
 {% if hasFieldset %}
   {{ govukFieldset({
     'describedBy': ns.describedBy,
     'classes': params.fieldset.classes,
     'attributes': params.fieldset.attributes,
     'legend': params.fieldset.legend,
     'html': innerHtml | trim
```

### Comparing `govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/cookie-banner/macro.html` & `govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/cookie-banner/macro.html`

 * *Files 25% similar despite different names*

```diff
@@ -1,66 +1,59 @@
 {% macro govukCookieBanner (params) %}
+{% from "govuk_frontend_jinja/macros/attributes.html" import govukAttributes %}
 {% from "govuk_frontend_jinja/components/button/macro.html" import govukButton -%}
 
 <div class="govuk-cookie-banner {%- if params.classes %} {{ params.classes }}{% endif %}" data-nosnippet role="region" aria-label="{{ params.ariaLabel | default("Cookie banner", true) }}"
   {%- if params.hidden %} hidden{% endif %}
-  {%- for attribute, value in (params.attributes.items() if params.attributes else {}.items()) %} {{ attribute }}="{{ value }}"{% endfor %}>
-
-  {%- for message in params.messages %}
-    <div class="govuk-cookie-banner__message {%- if message.classes %} {{ message.classes }}{% endif %} govuk-width-container" {%- if message.role %} role="{{ message.role }}"{% endif %}
-    {%- for attribute, value in (message.attributes.items() if message.attributes else {}.items()) %} {{ attribute }}="{{ value }}"{% endfor %}
+  {{- govukAttributes(params.attributes) }}>
+  {% for message in params.messages %}
+  <div class="govuk-cookie-banner__message {%- if message.classes %} {{ message.classes }}{% endif %} govuk-width-container" {%- if message.role %} role="{{ message.role }}"{% endif %}
+    {{- govukAttributes(message.attributes) -}}
     {%- if message.hidden %} hidden{% endif %}>
 
     <div class="govuk-grid-row">
       <div class="govuk-grid-column-two-thirds">
         {% if message.headingHtml or message.headingText %}
         <h2 class="govuk-cookie-banner__heading govuk-heading-m">
-          {%- if message.headingHtml -%}
-            {{ message.headingHtml | safe }}
-          {%- else -%}
-            {{ message.headingText }}
-          {%- endif -%}
+          {{ message.headingHtml | safe | trim | indent(10) if message.headingHtml else message.headingText }}
         </h2>
         {% endif %}
-
         <div class="govuk-cookie-banner__content">
-          {%- if message.html -%}
-            {{ message.html | safe }}
-          {%- elif message.text -%}
-            <p class="govuk-body">{{ message.text }}</p>
-          {%- endif -%}
+          {% if message.html %}
+          {{ message.html | safe | trim | indent(10) }}
+          {% elif message.text %}
+          <p class="govuk-body">{{ message.text }}</p>
+          {% endif %}
         </div>
       </div>
     </div>
 
-      {% if message.actions %}
-      <div class="govuk-button-group">
-        {% for action in message.actions %}
-          {% if action.href %}
-            {% if action.type == "button" %}
-              {{ govukButton({
-                "text": action.text,
-                "type": "button",
-                "classes": action.classes,
-                "href": action.href,
-                "attributes": action.attributes
-              }) | trim | indent(12) }}
-            {% else %}
-              <a class="govuk-link {%- if action.classes %} {{ action.classes }}{% endif %}" href="{{ action.href }}" {%- for attribute, value in (action.attributes.items() if action.attributes else {}.items()) %} {{ attribute }}="{{ value }}"{% endfor %}>{{ action.text }}</a>
-            {% endif %}
-          {% else %}
-            {{ govukButton({
-              "text": action.text,
-              "value": action.value,
-              "name": action.name,
-              "type": action.type,
-              "classes": action.classes,
-              "attributes": action.attributes
-            }) | trim | indent(12) }}
-          {% endif %}
-        {% endfor %}
-      </div>
-      {% endif %}
+    {% if message.actions %}
+    <div class="govuk-button-group">
+    {% for action in message.actions %}
+      {% set buttonHtml -%}
+        {% if not action.href or action.type == "button" %}
+          {{ govukButton({
+            "text": action.text,
+            "type": action.type if action.type else "button",
+            "name": action.name,
+            "value": action.value,
+            "classes": action.classes,
+            "href": action.href,
+            "attributes": action.attributes
+          }) }}
+        {% else %}
+          <a class="govuk-link {%- if action.classes %} {{ action.classes }}{% endif %}" href="{{ action.href }}"
+            {{- govukAttributes(action.attributes) }}>
+            {{- action.text -}}
+          </a>
+        {% endif %}
+      {%- endset %}
+      {{ buttonHtml | safe | trim | indent(6) }}
+    {% endfor %}
     </div>
+    {% endif %}
+
+  </div>
   {% endfor %}
 </div>
 {% endmacro %}
```

### Comparing `govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/date-input/macro.html` & `govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/date-input/macro.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 {% macro govukDateInput(params) %}
+{% from "govuk_frontend_jinja/macros/attributes.html" import govukAttributes %}
 {% from "govuk_frontend_jinja/components/error-message/macro.html" import govukErrorMessage %}
 {% from "govuk_frontend_jinja/components/fieldset/macro.html" import govukFieldset %}
 {% from "govuk_frontend_jinja/components/hint/macro.html" import govukHint %}
 {% from "govuk_frontend_jinja/components/input/macro.html" import govukInput %}
 
 {#- a record of other elements that we need to associate with the input using
   aria-describedby – for example hints or error messages -#}
-{% set ns = namespace() %}
-{% set ns.describedBy = params.fieldset.describedBy if params.fieldset and params.fieldset.describedBy else "" %}
+  {% set ns = namespace() %}
+  {% set ns.describedBy = params.fieldset.describedBy if params.fieldset and params.fieldset.describedBy else "" %}
 
 {#- fieldset is false by default -#}
 {% set hasFieldset = true if params.fieldset else false %}
 
 {%- if 'items' in params and params['items'] | length %}
   {% set dateInputItems = params['items'] %}
 {% else %}
@@ -30,62 +31,68 @@
     }
   ] %}
 {% endif %}
 
 {#- Capture the HTML so we can optionally nest it in a fieldset -#}
 {% set innerHtml %}
 {% if params.hint %}
-  {% set hintId = params.id + "-hint" %}
-  {% set ns.describedBy = ns.describedBy + " " + hintId if ns.describedBy else hintId %}
+  {% set hintId = params.id ~ "-hint" %}
+  {% set ns.describedBy = ns.describedBy ~ " " ~ hintId if ns.describedBy else hintId %}
   {{ govukHint({
     'id': hintId,
     'classes': params.hint.classes,
     'attributes': params.hint.attributes,
     'html': params.hint.html,
     'text': params.hint.text
   }) | trim | indent(2) }}
 {% endif %}
 {% if params.errorMessage %}
-  {% set errorId = params.id + "-error" %}
-  {% set ns.describedBy = ns.describedBy + " " + errorId if ns.describedBy else errorId %}
+  {% set errorId = params.id ~ "-error" %}
+  {% set ns.describedBy = ns.describedBy ~ " " ~ errorId if ns.describedBy else errorId %}
   {{ govukErrorMessage({
     'id': errorId,
     'classes': params.errorMessage.classes,
     'attributes': params.errorMessage.attributes,
     'html': params.errorMessage.html,
     'text': params.errorMessage.text,
     'visuallyHiddenText': params.errorMessage.visuallyHiddenText
   }) | trim | indent(2) }}
 {% endif %}
   <div class="govuk-date-input {%- if params.classes %} {{ params.classes }}{% endif %}"
-    {%- for attribute, value in (params.attributes.items() if params.attributes else {}.items()) %} {{ attribute }}="{{ value }}"{% endfor %}
+    {{- govukAttributes(params.attributes) -}}
     {%- if params.id %} id="{{ params.id }}"{% endif %}>
+    {% if params.formGroup and params.formGroup.beforeInputs %}
+    {{ params.formGroup.beforeInputs.html | safe | trim | indent(4) if params.formGroup and params.formGroup.beforeInputs.html else params.formGroup.beforeInputs.text }}
+    {% endif %}
     {% for item in dateInputItems %}
     <div class="govuk-date-input__item">
       {{ govukInput({
         'label': {
           'text': item.label if item.label else item.name | capitalize,
           'classes': "govuk-date-input__label"
         },
-        'id': item.id if item.id else (params.id + "-" + item.name),
-        'classes': "govuk-date-input__input " + (item.classes if item.classes else ''),
-        'name': (params.namePrefix + "-" + item.name) if params.namePrefix else item.name,
+        'id': item.id if item.id else (params.id ~ "-" ~ item.name),
+        'classes': "govuk-date-input__input " ~ (item.classes if item.classes),
+        'name': (params.namePrefix ~ "-" ~ item.name) if params.namePrefix else item.name,
         'value': item.value,
         'type': "text",
         'inputmode': item.inputmode if item.inputmode else "numeric",
         'autocomplete': item.autocomplete,
         'pattern': item.pattern,
         'attributes': item.attributes
       }) | trim | indent(6) }}
     </div>
-  {% endfor %}
+    {% endfor %}
+    {% if params.formGroup and params.formGroup.afterInputs %}
+    {{ params.formGroup.afterInputs.html | safe | trim | indent(4) if params.formGroup and params.formGroup.afterInputs.html else params.formGroup.afterInputs.text }}
+    {% endif %}
   </div>
 {% endset -%}
 
-<div class="govuk-form-group {%- if params.errorMessage %} govuk-form-group--error{% endif %} {%- if params.formGroup and params.formGroup.classes %} {{ params.formGroup.classes }}{% endif %}" {%- for attribute, value in (params.formGroup.attributes.items() if params.formGroup and params.formGroup.attributes else {}.items()) %} {{ attribute }}="{{ value }}"{% endfor %}>
+<div class="govuk-form-group {%- if params.errorMessage %} govuk-form-group--error{% endif %} {%- if params.formGroup and params.formGroup.classes %} {{ params.formGroup.classes }}{% endif %}" {{- govukAttributes(params.formGroup.attributes if params.formGroup) }}>
 {% if hasFieldset %}
   {# We override the fieldset's role to 'group' because otherwise JAWS does not
     announce the description for a fieldset comprised of text inputs, but
     adding the role to the fieldset always makes the output overly verbose for
     radio buttons or checkboxes. -#}
   {{ govukFieldset({
     'describedBy': ns.describedBy,
```

### Comparing `govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/details/macro.html` & `govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/panel/macro.html`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,18 @@
-{% macro govukDetails(params) %}
-<details {%- if params.id %} id="{{ params.id }}"{% endif %} class="govuk-details {%- if params.classes %} {{ params.classes }}{% endif %}" {%- for attribute, value in (params.attributes.items() if params.attributes else {}.items()) %} {{ attribute }}="{{ value }}"{% endfor %} {{- " open" if params.open }}>
-  <summary class="govuk-details__summary">
-    <span class="govuk-details__summary-text">
-      {{ params.summaryHtml | safe if params.summaryHtml else params.summaryText }}
-    </span>
-  </summary>
-  <div class="govuk-details__text">
-    {{ caller() if caller else (params.html | safe if params.html else params.text) }}
+{% macro govukPanel(params) %}
+{% from "govuk_frontend_jinja/macros/attributes.html" import govukAttributes -%}
+
+{% set headingLevel = params.headingLevel if params.headingLevel else 1 -%}
+
+<div class="govuk-panel govuk-panel--confirmation
+  {%- if params.classes %} {{ params.classes }}{% endif %}"
+  {{- govukAttributes(params.attributes) }}>
+  <h{{ headingLevel }} class="govuk-panel__title">
+    {{ params.titleHtml | safe if params.titleHtml else params.titleText }}
+  </h{{ headingLevel }}>
+  {% if caller or params.html or params.text %}
+  <div class="govuk-panel__body">
+    {{ caller() if caller else (params.html | safe | trim | indent(4) if params.html else params.text) }}
   </div>
-</details>
+  {% endif %}
+</div>
 {% endmacro %}
```

### Comparing `govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/error-summary/macro.html` & `govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/error-summary/macro.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 {% macro govukErrorSummary(params) %}
+{% from "govuk_frontend_jinja/macros/attributes.html" import govukAttributes -%}
+
 <div class="govuk-error-summary
   {%- if params.classes %} {{ params.classes }}{% endif %}"
   {%- if params.disableAutoFocus is not undefined %} data-disable-auto-focus="{{ params.disableAutoFocus | lower }}"{% endif %}
-  {%- for attribute, value in (params.attributes.items() if params.attributes else {}.items()) %} {{ attribute }}="{{ value }}"{% endfor %} data-module="govuk-error-summary">
+  {{- govukAttributes(params.attributes) }} data-module="govuk-error-summary">
   {#- Keep the role="alert" in a seperate child container to prevent a race condition between
   the focusing js at the alert, resulting in information getting missed in screen reader announcements #}
   <div role="alert">
     <h2 class="govuk-error-summary__title">
       {{ params.titleHtml | safe | trim | indent(6) if params.titleHtml else params.titleText }}
     </h2>
     <div class="govuk-error-summary__body">
       {% if caller or params.descriptionHtml or params.descriptionText %}
       <p>
         {{ caller() if caller else (params.descriptionHtml | safe | trim | indent(8) if params.descriptionHtml else params.descriptionText) }}
       </p>
       {% endif %}
-      <ul class="govuk-list govuk-error-summary__list">
-      {% for item in params.errorList %}
-        <li>
-        {% if item.href %}
-          <a href="{{ item.href }}" {%- for attribute, value in (item.attributes.items() if item.attributes else {}.items()) %} {{ attribute }}="{{ value }}"{% endfor %}>
-            {{- item.html | safe | trim | indent(12) if item.html else item.text -}}
-          </a>
-        {% else %}
-          {{ item.html | safe | trim | indent(10) if item.html else item.text }}
-        {% endif %}
-        </li>
-      {% endfor %}
-      </ul>
+      {% if params.errorList | length %}
+        <ul class="govuk-list govuk-error-summary__list">
+        {% for item in params.errorList %}
+          <li>
+          {% if item.href %}
+            <a href="{{ item.href }}"
+              {{- govukAttributes(item.attributes) }}>
+              {{- item.html | safe | trim | indent(12) if item.html else item.text -}}
+            </a>
+          {% else %}
+            {{ item.html | safe | trim | indent(10) if item.html else item.text }}
+          {% endif %}
+          </li>
+        {% endfor %}
+        </ul>
+      {% endif %}
     </div>
   </div>
 </div>
 {% endmacro %}
```

#### html2text {}

```diff
@@ -1,23 +1,22 @@
-{% macro govukErrorSummary(params) %}
+{% macro govukErrorSummary(params) %} {% from "govuk_frontend_jinja/macros/
+attributes.html" import govukAttributes -%}
 %- if params.disableAutoFocus is not undefined %} data-disable-auto-focus="{
-{ params.disableAutoFocus | lower }}"{% endif %} {%- for attribute, value in
-(params.attributes.items() if params.attributes else {}.items()) %} {
-{ attribute }}="{{ value }}"{% endfor %} data-module="govuk-error-summary"> {#-
-Keep the role="alert" in a seperate child container to prevent a race condition
-between the focusing js at the alert, resulting in information getting missed
-in screen reader announcements #}
+{ params.disableAutoFocus | lower }}"{% endif %} {{- govukAttributes
+(params.attributes) }} data-module="govuk-error-summary"> {#- Keep the
+role="alert" in a seperate child container to prevent a race condition between
+the focusing js at the alert, resulting in information getting missed in screen
+reader announcements #}
 ********** {{{{ ppaarraammss..ttiittlleeHHttmmll || ssaaffee || ttrriimm || iinnddeenntt((66)) iiff ppaarraammss..ttiittlleeHHttmmll eellssee
 ppaarraammss..ttiittlleeTTeexxtt }}}} **********
 {% if caller or params.descriptionHtml or params.descriptionText %}
 {{ caller() if caller else (params.descriptionHtml | safe | trim | indent(8) if
 params.descriptionHtml else params.descriptionText) }}
-{% endif %}
+{% endif %} {% if params.errorList | length %}
     * {% for item in params.errorList %}
-    * {% if item.href %} %- for attribute, value in (item.attributes.items() if
-      item.attributes else {}.items()) %} {{ attribute }}="{{ value }}"{%
-      endfor %}> {{- item.html | safe | trim | indent(12) if item.html else
-      item.text -}}
+    * {% if item.href %} {- govukAttributes(item.attributes) }}> {{- item.html
+      | safe | trim | indent(12) if item.html else item.text -}}
 {% else %} {{ item.html | safe | trim | indent(10) if item.html else item.text
 }} {% endif %}
 {% endfor %}
+{% endif %}
 {% endmacro %}
```

### Comparing `govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/exit-this-page/macro.html` & `govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/exit-this-page/macro.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 {% macro govukExitThisPage(params) %}
+{% from "govuk_frontend_jinja/macros/attributes.html" import govukAttributes %}
 {% from "govuk_frontend_jinja/components/button/macro.html" import govukButton %}
 
 {%- set defaultHtml %}
   <span class="govuk-visually-hidden">Emergency</span> Exit this page
 {% endset -%}
 
 <div
-  {%- if params.id %} id="{{ params.id }}"{% endif %} class="govuk-exit-this-page {%- if params.classes %} {{ params.classes }}{% endif %}" data-module="govuk-exit-this-page" {%- for attribute, value in (params.attributes.items() if params.attributes else {}.items()) %} {{ attribute }}="{{ value | lower }}"{% endfor %}
+  {%- if params.id %} id="{{ params.id }}"{% endif %} class="govuk-exit-this-page {%- if params.classes %} {{ params.classes }}{% endif %}" data-module="govuk-exit-this-page"
+  {{- govukAttributes(params.attributes) -}}
   {%- if params.activatedText %} data-i18n.activated="{{ params.activatedText | escape }}"{% endif %}
   {%- if params.timedOutText %} data-i18n.timed-out="{{ params.timedOutText | escape }}"{% endif %}
   {%- if params.pressTwoMoreTimesText %} data-i18n.press-two-more-times="{{ params.pressTwoMoreTimesText | escape }}"{% endif %}
   {%- if params.pressOneMoreTimeText %} data-i18n.press-one-more-time="{{ params.pressOneMoreTimeText | escape }}"{% endif %}
 >
   {{ govukButton({
     'html': params.html if (params.html or params.text) else defaultHtml,
```

### Comparing `govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/fieldset/macro.html` & `govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/fieldset/macro.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 {% macro govukFieldset(params) %}
+{% from "govuk_frontend_jinja/macros/attributes.html" import govukAttributes -%}
+
 <fieldset class="govuk-fieldset
   {%- if params.classes %} {{ params.classes }}{% endif %}"
   {%- if params.role %} role="{{ params.role }}"{% endif %}
   {%- if params.describedBy %} aria-describedby="{{ params.describedBy }}"{% endif %}
-  {%- for attribute, value in (params.attributes.items() if params.attributes else {}.items()) %} {{ attribute }}="{{ value }}"{% endfor %}>
+  {{- govukAttributes(params.attributes) }}>
   {% if params.legend.html or params.legend.text %}
   <legend class="govuk-fieldset__legend {%- if params.legend.classes %} {{ params.legend.classes }}{% endif %}">
   {% if params.legend.isPageHeading %}
     <h1 class="govuk-fieldset__heading">
       {{ params.legend.html | safe | trim | indent(6) if params.legend.html else params.legend.text }}
     </h1>
   {% else %}
```

### Comparing `govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/file-upload/macro.html` & `govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/textarea/macro.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,56 @@
-{% macro govukFileUpload(params) %}
+{% macro govukTextarea(params) %}
+{% from "govuk_frontend_jinja/macros/attributes.html" import govukAttributes %}
 {% from "govuk_frontend_jinja/components/error-message/macro.html" import govukErrorMessage %}
 {% from "govuk_frontend_jinja/components/hint/macro.html" import govukHint %}
 {% from "govuk_frontend_jinja/components/label/macro.html" import govukLabel %}
 
 {#- a record of other elements that we need to associate with the input using
   aria-describedby – for example hints or error messages -#}
 {% set describedBy = params.describedBy if params.describedBy else "" %}
-<div class="govuk-form-group {%- if params.errorMessage %} govuk-form-group--error{% endif %} {%- if params.formGroup and params.formGroup.classes %} {{ params.formGroup.classes }}{% endif %}" {%- for attribute, value in (params.formGroup.attributes.items() if params.formGroup and params.formGroup.attributes else {}.items()) %} {{ attribute }}="{{ value }}"{% endfor %}>
+<div class="govuk-form-group {%- if params.errorMessage %} govuk-form-group--error{% endif %} {%- if params.formGroup and params.formGroup.classes %} {{ params.formGroup.classes }}{% endif %}"
+  {{- govukAttributes(params.formGroup.attributes if params.formGroup) }}>
   {{ govukLabel({
     'html': params.label.html,
     'text': params.label.text,
     'classes': params.label.classes,
     'isPageHeading': params.label.isPageHeading,
     'attributes': params.label.attributes,
     'for': params.id
   }) | trim | indent(2) }}
 {% if params.hint %}
-  {% set hintId = params.id + '-hint' %}
-  {% set describedBy = describedBy + ' ' + hintId if describedBy else hintId %}
+  {% set hintId = params.id ~ '-hint' %}
+  {% set describedBy = describedBy ~ ' ' ~ hintId if describedBy else hintId %}
   {{ govukHint({
     'id': hintId,
     'classes': params.hint.classes,
     'attributes': params.hint.attributes,
     'html': params.hint.html,
     'text': params.hint.text
   }) | trim | indent(2) }}
 {% endif %}
 {% if params.errorMessage %}
-  {% set errorId = params.id + '-error' %}
-  {% set describedBy = describedBy + ' ' + errorId if describedBy else errorId %}
+  {% set errorId = params.id ~ '-error' %}
+  {% set describedBy = describedBy ~ ' ' ~ errorId if describedBy else errorId %}
   {{ govukErrorMessage({
     'id': errorId,
     'classes': params.errorMessage.classes,
     'attributes': params.errorMessage.attributes,
     'html': params.errorMessage.html,
     'text': params.errorMessage.text,
     'visuallyHiddenText': params.errorMessage.visuallyHiddenText
   }) | trim | indent(2) }}
 {% endif %}
-  <input class="govuk-file-upload {%- if params.classes %} {{ params.classes }}{% endif %} {%- if params.errorMessage %} govuk-file-upload--error{% endif %}" id="{{ params.id }}" name="{{ params.name }}" type="file"
-  {%- if params.value %} value="{{ params.value }}"{% endif %}
+{% if params.formGroup and params.formGroup.beforeInput %}
+  {{ params.formGroup.beforeInput.html | safe | trim | indent(2) if params.formGroup and params.formGroup.beforeInput.html else params.formGroup.beforeInput.text }}
+{% endif %}
+  <textarea class="govuk-textarea {%- if params.errorMessage %} govuk-textarea--error{% endif %} {%- if params.classes %} {{ params.classes }}{% endif %}" id="{{ params.id }}" name="{{ params.name }}" rows="{{ params.rows | default(5, true) }}"
+  {%- if (params.spellcheck is false) or (params.spellcheck is true) %} spellcheck="{{ params.spellcheck | lower }}"{% endif %}
   {%- if params.disabled %} disabled{% endif %}
   {%- if describedBy %} aria-describedby="{{ describedBy }}"{% endif %}
-  {%- for attribute, value in (params.attributes.items() if params.attributes else {}.items()) %} {{ attribute }}="{{ value }}"{% endfor %}>
+  {%- if params.autocomplete %} autocomplete="{{ params.autocomplete }}"{% endif %}
+  {{- govukAttributes(params.attributes) }}>{{ params.value }}</textarea>
+{% if params.formGroup and params.formGroup.afterInput %}
+  {{ params.formGroup.afterInput.html | safe | trim | indent(2) if params.formGroup and params.formGroup.afterInput.html else params.formGroup.afterInput.text }}
+{% endif %}
 </div>
 {% endmacro %}
```

### Comparing `govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/footer/macro.html` & `govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/footer/macro.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 {% macro govukFooter(params) %}
-<footer class="govuk-footer {%- if params.classes %} {{ params.classes }}{% endif %}" role="contentinfo"
-  {%- for attribute, value in (params.attributes.items() if params.attributes else {}.items()) %} {{ attribute }}="{{ value }}"{% endfor %}>
+{% from "govuk_frontend_jinja/macros/attributes.html" import govukAttributes -%}
+
+<footer class="govuk-footer {%- if params.classes %} {{ params.classes }}{% endif %}"
+  {{- govukAttributes(params.attributes) }}>
   <div class="govuk-width-container {%- if params.containerClasses %} {{ params.containerClasses }}{% endif %}">
     {% if params.navigation | length %}
       <div class="govuk-footer__navigation">
         {% for nav in params.navigation %}
           <div class="govuk-footer__section govuk-grid-column-{{ nav.width | default("full", true) }}">
             <h2 class="govuk-footer__heading govuk-heading-m">{{ nav.title }}</h2>
             {% if nav['items'] | length %}
               {% set listClasses = "govuk-footer__list--columns-" ~ nav.columns if nav.columns %}
               <ul class="govuk-footer__list {%- if listClasses %} {{ listClasses }}{% endif %}">
                 {% for item in nav['items'] %}
                   {% if item.href and item.text %}
                     <li class="govuk-footer__list-item">
-                      <a class="govuk-footer__link" href="{{ item.href }}" {%- for attribute, value in (item.attributes.items() if item.attributes else {}.items()) %} {{ attribute }}="{{ value }}"{% endfor %}>
+                      <a class="govuk-footer__link" href="{{ item.href }}"
+                        {{- govukAttributes(item.attributes) }}>
                         {{ item.text }}
                       </a>
                     </li>
                   {% endif %}
                 {% endfor %}
               </ul>
             {% endif %}
@@ -25,35 +28,36 @@
         {% endfor %}
       </div>
       <hr class="govuk-footer__section-break">
     {% endif %}
     <div class="govuk-footer__meta">
       <div class="govuk-footer__meta-item govuk-footer__meta-item--grow">
         {% if 'meta' in params %}
-          <h2 class="govuk-visually-hidden">{{ params.meta.visuallyHiddenTitle | default("Support links", true) }}</h2>
-          {% if 'items' in params.meta and (params.meta['items'] | length) %}
-            <ul class="govuk-footer__inline-list">
-              {% for item in params.meta['items'] %}
-                <li class="govuk-footer__inline-list-item">
-                  <a class="govuk-footer__link" href="{{ item.href }}" {%- for attribute, value in (item.attributes.items() if item.attributes else {}.items()) %} {{ attribute }}="{{ value }}"{% endfor %}>
-                    {{ item.text }}
-                  </a>
-                </li>
-              {% endfor %}
-            </ul>
-          {% endif %}
-          {% if params.meta.text or params.meta.html %}
-            <div class="govuk-footer__meta-custom">
-              {{ params.meta.html | safe if params.meta.html else params.meta.text }}
-            </div>
-          {% endif %}
+        <h2 class="govuk-visually-hidden">{{ params.meta.visuallyHiddenTitle | default("Support links", true) }}</h2>
+        {% if 'items' in params.meta and (params.meta['items'] | length) %}
+        <ul class="govuk-footer__inline-list">
+        {% for item in params.meta['items'] %}
+          <li class="govuk-footer__inline-list-item">
+            <a class="govuk-footer__link" href="{{ item.href }}"
+              {{- govukAttributes(item.attributes) }}>
+              {{ item.text }}
+            </a>
+          </li>
+        {% endfor %}
+        </ul>
+        {% endif %}
+        {% if params.meta.text or params.meta.html %}
+        <div class="govuk-footer__meta-custom">
+          {{ params.meta.html | safe | trim | indent(10) if params.meta.html else params.meta.text }}
+        </div>
+        {% endif %}
         {% endif %}
-        {#- The SVG needs `focusable="false"` so that Internet Explorer does not
-        treat it as an interactive element - without this it will be
-        'focusable' when using the keyboard to navigate. #}
+        {# The SVG needs `focusable="false"` so that Internet Explorer does not
+          treat it as an interactive element - without this it will be
+          'focusable' when using the keyboard to navigate. -#}
         <svg
           aria-hidden="true"
           focusable="false"
           class="govuk-footer__licence-logo"
           xmlns="http://www.w3.org/2000/svg"
           viewBox="0 0 483.2 195.7"
           height="17"
@@ -61,35 +65,35 @@
         >
           <path
             fill="currentColor"
             d="M421.5 142.8V.1l-50.7 32.3v161.1h112.4v-50.7zm-122.3-9.6A47.12 47.12 0 0 1 221 97.8c0-26 21.1-47.1 47.1-47.1 16.7 0 31.4 8.7 39.7 21.8l42.7-27.2A97.63 97.63 0 0 0 268.1 0c-36.5 0-68.3 20.1-85.1 49.7A98 98 0 0 0 97.8 0C43.9 0 0 43.9 0 97.8s43.9 97.8 97.8 97.8c36.5 0 68.3-20.1 85.1-49.7a97.76 97.76 0 0 0 149.6 25.4l19.4 22.2h3v-87.8h-80l24.3 27.5zM97.8 145c-26 0-47.1-21.1-47.1-47.1s21.1-47.1 47.1-47.1 47.2 21 47.2 47S123.8 145 97.8 145"
           />
         </svg>
         <span class="govuk-footer__licence-description">
-          {% if params.contentLicence and (params.contentLicence.html or params.contentLicence.text) %}
-            {{ params.contentLicence.html | safe if params.contentLicence.html else params.contentLicence.text }}
-          {% else %}
-            All content is available under the
-            <a
-              class="govuk-footer__link"
-              href="https://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/"
-              rel="license"
-            >Open Government Licence v3.0</a>, except where otherwise stated
-          {% endif %}
+        {% if params.contentLicence and (params.contentLicence.html or params.contentLicence.text) %}
+          {{ params.contentLicence.html | safe | trim | indent(10) if params.contentLicence.html else params.contentLicence.text }}
+        {% else %}
+          All content is available under the
+          <a
+            class="govuk-footer__link"
+            href="https://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/"
+            rel="license"
+          >Open Government Licence v3.0</a>, except where otherwise stated
+        {% endif %}
         </span>
       </div>
       <div class="govuk-footer__meta-item">
         <a
           class="govuk-footer__link govuk-footer__copyright-logo"
           href="https://www.nationalarchives.gov.uk/information-management/re-using-public-sector-information/uk-government-licensing-framework/crown-copyright/"
         >
-          {%- if params.copyright and (params.copyright.html or params.copyright.text) -%}
-            {{ params.copyright.html | safe if params.copyright.html else params.copyright.text }}
-          {%- else -%}
-            © Crown copyright
-          {%- endif -%}
+        {% if params.copyright and (params.copyright.html or params.copyright.text) %}
+          {{ params.copyright.html | safe | trim | indent(10) if params.copyright.html else params.copyright.text }}
+        {% else %}
+          © Crown copyright
+        {% endif %}
         </a>
       </div>
     </div>
   </div>
 </footer>
 {% endmacro %}
```

### Comparing `govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/header/macro.html` & `govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/header/macro.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 {% macro govukHeader(params) %}
-{% set menuButtonText = params.menuButtonText if params.menuButtonText else 'Menu' -%}
+{% from "govuk_frontend_jinja/macros/attributes.html" import govukAttributes %}
 
-{% set _stEdwardsCrown %}
+{%- set menuButtonText = params.menuButtonText if params.menuButtonText else 'Menu' -%}
+
+{%- set _stEdwardsCrown %}
 <svg
   focusable="false"
   role="img"
   class="govuk-header__logotype"
   xmlns="http://www.w3.org/2000/svg"
   viewBox="0 0 152 30"
   height="30"
@@ -13,81 +15,84 @@
   aria-label="GOV.UK"
 >
   <title>GOV.UK</title>
   <path d="M6.7 12.2c1 .4 2.1-.1 2.5-1s-.1-2.1-1-2.5c-1-.4-2.1.1-2.5 1-.4 1 0 2.1 1 2.5m-4.3 2.5c1 .4 2.1-.1 2.5-1s-.1-2.1-1-2.5c-1-.4-2.1.1-2.5 1-.5 1 0 2.1 1 2.5m-1.3 4.8c1 .4 2.1-.1 2.5-1 .4-1-.1-2.1-1-2.5-1-.4-2.1.1-2.5 1-.4 1 0 2.1 1 2.5m10.4-5.8c1 .4 2.1-.1 2.5-1s-.1-2.1-1-2.5c-1-.4-2.1.1-2.5 1s0 2.1 1 2.5m17.4-1.5c-1 .4-2.1-.1-2.5-1s.1-2.1 1-2.5c1-.4 2.1.1 2.5 1 .5 1 0 2.1-1 2.5m4.3 2.5c-1 .4-2.1-.1-2.5-1s.1-2.1 1-2.5c1-.4 2.1.1 2.5 1 .5 1 0 2.1-1 2.5m1.3 4.8c-1 .4-2.1-.1-2.5-1-.4-1 .1-2.1 1-2.5 1-.4 2.1.1 2.5 1 .4 1 0 2.1-1 2.5m-10.4-5.8c-1 .4-2.1-.1-2.5-1s.1-2.1 1-2.5c1-.4 2.1.1 2.5 1s0 2.1-1 2.5m-5.3-4.9 2.4 1.3V6.5l-2.4.8c-.1-.1-.1-.2-.2-.2s1-3 1-3h-3.4l1 3c-.1.1-.2.1-.2.2-.1.1-2.4-.7-2.4-.7v3.5L17 8.8c-.1.1 0 .2.1.3l-1.4 4.2c-.1.2-.1.4-.1.7 0 1.1.8 2.1 1.9 2.2h.6C19.2 16 20 15.1 20 14c0-.2 0-.4-.1-.7l-1.4-4.2c.2-.1.3-.2.3-.3m-1 20.3c4.6 0 8.9.3 12.8.9 1.1-4.6 2.4-7.2 3.8-9.1l-2.6-.9c.3 1.3.3 1.9 0 2.8-.4-.4-.8-1.2-1.1-2.4l-1.2 4.2c.8-.5 1.4-.9 2-.9-1.2 2.6-2.7 3.2-3.6 3-1.2-.2-1.7-1.3-1.5-2.2.3-1.3 1.6-1.6 2.2-.1 1.2-2.4-.8-3.1-2.1-2.4 1.9-1.9 2.2-3.6.6-5.7-2.2 1.7-2.2 3.3-1.2 5.6-1.3-1.5-3.3-.7-2.5 1.7.9-1.4 2.1-.5 2 .8-.2 1.2-1.7 2.1-3.7 2-2.8-.2-3-2.2-3-3.7.7-.1 1.9.5 3 2l.4-4.4c-1.1 1.2-2.2 1.4-3.3 1.4.4-1.2 2.1-3.1 2.1-3.1h-5.5s1.8 2 2.1 3.1c-1.1 0-2.2-.3-3.3-1.4l.4 4.4c1.1-1.5 2.3-2.1 3-2-.1 1.6-.2 3.5-3 3.7-1.9.2-3.5-.8-3.7-2-.2-1.3 1-2.2 1.9-.8.7-2.4-1.3-3.1-2.6-1.7 1-2.3 1-4-1.2-5.6-1.6 2.1-1.3 3.8.6 5.7-1.3-.7-3.2 0-2.1 2.4.6-1.5 1.9-1.1 2.2.1.2.9-.4 1.9-1.5 2.2-1 .2-2.5-.5-3.7-3 .7 0 1.3.4 2 .9L5 20.4c-.3 1.2-.7 1.9-1.2 2.4-.3-.8-.2-1.5 0-2.8l-2.6.9C2.7 22.8 4 25.4 5.1 30c3.8-.5 8.2-.9 12.7-.9m30.5-11.5c0 .9.1 1.7.3 2.5.2.8.6 1.5 1 2.2.5.6 1 1.1 1.7 1.5.7.4 1.5.6 2.5.6.9 0 1.7-.1 2.3-.4s1.1-.7 1.5-1.1c.4-.4.6-.9.8-1.5.1-.5.2-1 .2-1.5v-.2h-5.3v-3.2h9.4V28H59v-2.5c-.3.4-.6.8-1 1.1-.4.3-.8.6-1.3.9-.5.2-1 .4-1.6.6s-1.2.2-1.8.2c-1.5 0-2.9-.3-4-.8-1.2-.6-2.2-1.3-3-2.3-.8-1-1.4-2.1-1.8-3.4-.3-1.4-.5-2.8-.5-4.3s.2-2.9.7-4.2c.5-1.3 1.1-2.4 2-3.4.9-1 1.9-1.7 3.1-2.3 1.2-.6 2.6-.8 4.1-.8 1 0 1.9.1 2.8.3.9.2 1.7.6 2.4 1s1.4.9 1.9 1.5c.6.6 1 1.3 1.4 2l-3.7 2.1c-.2-.4-.5-.9-.8-1.2-.3-.4-.6-.7-1-1-.4-.3-.8-.5-1.3-.7-.5-.2-1.1-.2-1.7-.2-1 0-1.8.2-2.5.6-.7.4-1.3.9-1.7 1.5-.5.6-.8 1.4-1 2.2-.3.8-.4 1.9-.4 2.7zm36.4-4.3c-.4-1.3-1.1-2.4-2-3.4-.9-1-1.9-1.7-3.1-2.3-1.2-.6-2.6-.8-4.2-.8s-2.9.3-4.2.8c-1.1.6-2.2 1.4-3 2.3-.9 1-1.5 2.1-2 3.4-.4 1.3-.7 2.7-.7 4.2s.2 2.9.7 4.2c.4 1.3 1.1 2.4 2 3.4.9 1 1.9 1.7 3.1 2.3 1.2.6 2.6.8 4.2.8 1.5 0 2.9-.3 4.2-.8 1.2-.6 2.3-1.3 3.1-2.3.9-1 1.5-2.1 2-3.4.4-1.3.7-2.7.7-4.2-.1-1.5-.3-2.9-.8-4.2zM81 17.6c0 1-.1 1.9-.4 2.7-.2.8-.6 1.6-1.1 2.2-.5.6-1.1 1.1-1.7 1.4-.7.3-1.5.5-2.4.5-.9 0-1.7-.2-2.4-.5s-1.3-.8-1.7-1.4c-.5-.6-.8-1.3-1.1-2.2-.2-.8-.4-1.7-.4-2.7v-.1c0-1 .1-1.9.4-2.7.2-.8.6-1.6 1.1-2.2.5-.6 1.1-1.1 1.7-1.4.7-.3 1.5-.5 2.4-.5.9 0 1.7.2 2.4.5s1.3.8 1.7 1.4c.5.6.8 1.3 1.1 2.2.2.8.4 1.7.4 2.7v.1zM92.9 28 87 7h4.7l4 15.7h.1l4-15.7h4.7l-5.9 21h-5.7zm28.8-3.6c.6 0 1.2-.1 1.7-.3.5-.2 1-.4 1.4-.8.4-.4.7-.8.9-1.4.2-.6.3-1.2.3-2v-13h4.1v13.6c0 1.2-.2 2.2-.6 3.1s-1 1.7-1.8 2.4c-.7.7-1.6 1.2-2.7 1.5-1 .4-2.2.5-3.4.5-1.2 0-2.4-.2-3.4-.5-1-.4-1.9-.9-2.7-1.5-.8-.7-1.3-1.5-1.8-2.4-.4-.9-.6-2-.6-3.1V6.9h4.2v13c0 .8.1 1.4.3 2 .2.6.5 1 .9 1.4.4.4.8.6 1.4.8.6.2 1.1.3 1.8.3zm13-17.4h4.2v9.1l7.4-9.1h5.2l-7.2 8.4L152 28h-4.9l-5.5-9.4-2.7 3V28h-4.2V7zm-27.6 16.1c-1.5 0-2.7 1.2-2.7 2.7s1.2 2.7 2.7 2.7 2.7-1.2 2.7-2.7-1.2-2.7-2.7-2.7z"></path>
 </svg>
 {% endset %}
 
-{% set _tudorCrown %}
+{%- set _tudorCrown %}
 <svg
   focusable="false"
   role="img"
   class="govuk-header__logotype"
   xmlns="http://www.w3.org/2000/svg"
   viewBox="0 0 148 30"
   height="30"
   width="148"
   aria-label="GOV.UK"
 >
   <title>GOV.UK</title>
   <path d="M22.6 10.4c-1 .4-2-.1-2.4-1-.4-.9.1-2 1-2.4.9-.4 2 .1 2.4 1s-.1 2-1 2.4m-5.9 6.7c-.9.4-2-.1-2.4-1-.4-.9.1-2 1-2.4.9-.4 2 .1 2.4 1s-.1 2-1 2.4m10.8-3.7c-1 .4-2-.1-2.4-1-.4-.9.1-2 1-2.4.9-.4 2 .1 2.4 1s0 2-1 2.4m3.3 4.8c-1 .4-2-.1-2.4-1-.4-.9.1-2 1-2.4.9-.4 2 .1 2.4 1s-.1 2-1 2.4M17 4.7l2.3 1.2V2.5l-2.3.7-.2-.2.9-3h-3.4l.9 3-.2.2c-.1.1-2.3-.7-2.3-.7v3.4L15 4.7c.1.1.1.2.2.2l-1.3 4c-.1.2-.1.4-.1.6 0 1.1.8 2 1.9 2.2h.7c1-.2 1.9-1.1 1.9-2.1 0-.2 0-.4-.1-.6l-1.3-4c-.1-.2 0-.2.1-.3m-7.6 5.7c.9.4 2-.1 2.4-1 .4-.9-.1-2-1-2.4-.9-.4-2 .1-2.4 1s0 2 1 2.4m-5 3c.9.4 2-.1 2.4-1 .4-.9-.1-2-1-2.4-.9-.4-2 .1-2.4 1s.1 2 1 2.4m-3.2 4.8c.9.4 2-.1 2.4-1 .4-.9-.1-2-1-2.4-.9-.4-2 .1-2.4 1s0 2 1 2.4m14.8 11c4.4 0 8.6.3 12.3.8 1.1-4.5 2.4-7 3.7-8.8l-2.5-.9c.2 1.3.3 1.9 0 2.7-.4-.4-.8-1.1-1.1-2.3l-1.2 4c.7-.5 1.3-.8 2-.9-1.1 2.5-2.6 3.1-3.5 3-1.1-.2-1.7-1.2-1.5-2.1.3-1.2 1.5-1.5 2.1-.1 1.1-2.3-.8-3-2-2.3 1.9-1.9 2.1-3.5.6-5.6-2.1 1.6-2.1 3.2-1.2 5.5-1.2-1.4-3.2-.6-2.5 1.6.9-1.4 2.1-.5 1.9.8-.2 1.1-1.7 2.1-3.5 1.9-2.7-.2-2.9-2.1-2.9-3.6.7-.1 1.9.5 2.9 1.9l.4-4.3c-1.1 1.1-2.1 1.4-3.2 1.4.4-1.2 2.1-3 2.1-3h-5.4s1.7 1.9 2.1 3c-1.1 0-2.1-.2-3.2-1.4l.4 4.3c1-1.4 2.2-2 2.9-1.9-.1 1.5-.2 3.4-2.9 3.6-1.9.2-3.4-.8-3.5-1.9-.2-1.3 1-2.2 1.9-.8.7-2.3-1.2-3-2.5-1.6.9-2.2.9-3.9-1.2-5.5-1.5 2-1.3 3.7.6 5.6-1.2-.7-3.1 0-2 2.3.6-1.4 1.8-1.1 2.1.1.2.9-.3 1.9-1.5 2.1-.9.2-2.4-.5-3.5-3 .6 0 1.2.3 2 .9l-1.2-4c-.3 1.1-.7 1.9-1.1 2.3-.3-.8-.2-1.4 0-2.7l-2.9.9C1.3 23 2.6 25.5 3.7 30c3.7-.5 7.9-.8 12.3-.8m28.3-11.6c0 .9.1 1.7.3 2.5.2.8.6 1.5 1 2.2.5.6 1 1.1 1.7 1.5.7.4 1.5.6 2.5.6.9 0 1.7-.1 2.3-.4s1.1-.7 1.5-1.1c.4-.4.6-.9.8-1.5.1-.5.2-1 .2-1.5v-.2h-5.3v-3.2h9.4V28H55v-2.5c-.3.4-.6.8-1 1.1-.4.3-.8.6-1.3.9-.5.2-1 .4-1.6.6s-1.2.2-1.8.2c-1.5 0-2.9-.3-4-.8-1.2-.6-2.2-1.3-3-2.3-.8-1-1.4-2.1-1.8-3.4-.3-1.4-.5-2.8-.5-4.3s.2-2.9.7-4.2c.5-1.3 1.1-2.4 2-3.4.9-1 1.9-1.7 3.1-2.3 1.2-.6 2.6-.8 4.1-.8 1 0 1.9.1 2.8.3.9.2 1.7.6 2.4 1s1.4.9 1.9 1.5c.6.6 1 1.3 1.4 2l-3.7 2.1c-.2-.4-.5-.9-.8-1.2-.3-.4-.6-.7-1-1-.4-.3-.8-.5-1.3-.7-.5-.2-1.1-.2-1.7-.2-1 0-1.8.2-2.5.6-.7.4-1.3.9-1.7 1.5-.5.6-.8 1.4-1 2.2-.3.8-.4 1.9-.4 2.7zM71.5 6.8c1.5 0 2.9.3 4.2.8 1.2.6 2.3 1.3 3.1 2.3.9 1 1.5 2.1 2 3.4s.7 2.7.7 4.2-.2 2.9-.7 4.2c-.4 1.3-1.1 2.4-2 3.4-.9 1-1.9 1.7-3.1 2.3-1.2.6-2.6.8-4.2.8s-2.9-.3-4.2-.8c-1.2-.6-2.3-1.3-3.1-2.3-.9-1-1.5-2.1-2-3.4-.4-1.3-.7-2.7-.7-4.2s.2-2.9.7-4.2c.4-1.3 1.1-2.4 2-3.4.9-1 1.9-1.7 3.1-2.3 1.2-.5 2.6-.8 4.2-.8zm0 17.6c.9 0 1.7-.2 2.4-.5s1.3-.8 1.7-1.4c.5-.6.8-1.3 1.1-2.2.2-.8.4-1.7.4-2.7v-.1c0-1-.1-1.9-.4-2.7-.2-.8-.6-1.6-1.1-2.2-.5-.6-1.1-1.1-1.7-1.4-.7-.3-1.5-.5-2.4-.5s-1.7.2-2.4.5-1.3.8-1.7 1.4c-.5.6-.8 1.3-1.1 2.2-.2.8-.4 1.7-.4 2.7v.1c0 1 .1 1.9.4 2.7.2.8.6 1.6 1.1 2.2.5.6 1.1 1.1 1.7 1.4.6.3 1.4.5 2.4.5zM88.9 28 83 7h4.7l4 15.7h.1l4-15.7h4.7l-5.9 21h-5.7zm28.8-3.6c.6 0 1.2-.1 1.7-.3.5-.2 1-.4 1.4-.8.4-.4.7-.8.9-1.4.2-.6.3-1.2.3-2v-13h4.1v13.6c0 1.2-.2 2.2-.6 3.1s-1 1.7-1.8 2.4c-.7.7-1.6 1.2-2.7 1.5-1 .4-2.2.5-3.4.5-1.2 0-2.4-.2-3.4-.5-1-.4-1.9-.9-2.7-1.5-.8-.7-1.3-1.5-1.8-2.4-.4-.9-.6-2-.6-3.1V6.9h4.2v13c0 .8.1 1.4.3 2 .2.6.5 1 .9 1.4.4.4.8.6 1.4.8.6.2 1.1.3 1.8.3zm13-17.4h4.2v9.1l7.4-9.1h5.2l-7.2 8.4L148 28h-4.9l-5.5-9.4-2.7 3V28h-4.2V7zm-27.6 16.1c-1.5 0-2.7 1.2-2.7 2.7s1.2 2.7 2.7 2.7 2.7-1.2 2.7-2.7-1.2-2.7-2.7-2.7z"></path>
 </svg>
-{% endset %}
+{% endset -%}
 
-<header class="govuk-header {%- if params.classes %} {{ params.classes }}{% endif %}" role="banner" data-module="govuk-header"
-  {%- for attribute, value in (params.attributes.items() if params.attributes else {}.items()) %} {{ attribute }}="{{ value }}"{% endfor %}>
+<header class="govuk-header {%- if params.classes %} {{ params.classes }}{% endif %}" data-module="govuk-header"
+  {{- govukAttributes(params.attributes) }}>
   <div class="govuk-header__container {{ params.containerClasses | default("govuk-width-container", true) }}">
     <div class="govuk-header__logo">
       <a href="{{ params.homepageUrl | default("/", true) }}" class="govuk-header__link govuk-header__link--homepage">
         {#- The SVG needs `focusable="false"` so that Internet Explorer does
         not treat it as an interactive element - without this it will be
         'focusable' when using the keyboard to navigate.
 
         We use a single compound path for the logo to prevent subpixel rounding
         shifting different elements unevenly relative to one another. #}
-        {{ (_tudorCrown if params.useTudorCrown else _stEdwardsCrown) | safe }}
+        {{ (_stEdwardsCrown if (params.useTudorCrown is not undefined and params.useTudorCrown is false) else _tudorCrown) | safe | trim | indent(8) }}
         {% if (params.productName) %}
         <span class="govuk-header__product-name">
           {{ params.productName }}
         </span>
         {% endif %}
       </a>
     </div>
-    {% if params.serviceName or params.navigation | length %}
+  {% if params.serviceName or params.navigation | length %}
     <div class="govuk-header__content">
     {% if params.serviceName %}
-    {% if params.serviceUrl %}
+      {% if params.serviceUrl %}
       <a href="{{ params.serviceUrl }}" class="govuk-header__link govuk-header__service-name">
         {{ params.serviceName }}
       </a>
-    {% else%}
+      {% else %}
       <span class="govuk-header__service-name">
         {{ params.serviceName }}
       </span>
-    {% endif %}
+      {% endif %}
     {% endif %}
     {% if params.navigation | length %}
-    <nav aria-label="{{ params.navigationLabel | default(menuButtonText, true) }}" class="govuk-header__navigation {%- if params.navigationClasses %} {{ params.navigationClasses }}{% endif %}">
-      <button type="button" class="govuk-header__menu-button govuk-js-header-toggle" aria-controls="navigation" {%- if params.menuButtonLabel and params.menuButtonLabel != menuButtonText %} aria-label="{{ params.menuButtonLabel }}"{% endif %} hidden>{{ menuButtonText }}</button>
+      <nav aria-label="{{ params.navigationLabel | default(menuButtonText, true) }}" class="govuk-header__navigation {%- if params.navigationClasses %} {{ params.navigationClasses }}{% endif %}">
+        <button type="button" class="govuk-header__menu-button govuk-js-header-toggle" aria-controls="navigation" {%- if params.menuButtonLabel and params.menuButtonLabel != menuButtonText %} aria-label="{{ params.menuButtonLabel }}"{% endif %} hidden>
+          {{ menuButtonText }}
+        </button>
 
-      <ul id="navigation" class="govuk-header__navigation-list">
+        <ul id="navigation" class="govuk-header__navigation-list">
         {% for item in params.navigation %}
           {% if item.text or item.html %}
-            <li class="govuk-header__navigation-item {%- if item.active %} govuk-header__navigation-item--active{% endif %}">
-              {% if item.href %}
-                <a class="govuk-header__link" href="{{ item.href }}" {%- for attribute, value in (item.attributes.items() if item.attributes else {}.items()) %} {{ attribute }}="{{ value }}"{% endfor %}>
-              {% endif %}
-                {{ item.html | safe if item.html else item.text }}
-              {% if item.href %}
-                </a>
-              {% endif %}
-            </li>
+          <li class="govuk-header__navigation-item {%- if item.active %} govuk-header__navigation-item--active{% endif %}">
+            {% if item.href %}
+            <a class="govuk-header__link" href="{{ item.href }}"
+              {{- govukAttributes(item.attributes) -}}>
+            {% endif %}
+              {{ item.html | safe | trim | indent(14) if item.html else item.text }}
+            {% if item.href %}
+            </a>
+            {% endif %}
+          </li>
           {% endif %}
         {% endfor %}
-      </ul>
-    </nav>
+        </ul>
+      </nav>
     {% endif %}
     </div>
-    {% endif %}
+  {% endif %}
   </div>
 </header>
 {% endmacro %}
```

#### html2text {}

```diff
@@ -1,31 +1,32 @@
-{% macro govukHeader(params) %} {% set menuButtonText = params.menuButtonText
-if params.menuButtonText else 'Menu' -%} {% set _stEdwardsCrown %}
-{% endset %} {% set _tudorCrown %}
-{% endset %}
-%- for attribute, value in (params.attributes.items() if params.attributes else
-{}.items()) %} {{ attribute }}="{{ value }}"{% endfor %}>
+{% macro govukHeader(params) %} {% from "govuk_frontend_jinja/macros/
+attributes.html" import govukAttributes %} {%- set menuButtonText =
+params.menuButtonText if params.menuButtonText else 'Menu' -%} {%- set
+_stEdwardsCrown %}
+{% endset %} {%- set _tudorCrown %}
+{% endset -%}
+{- govukAttributes(params.attributes) }}>
 }">
 , true) }}" class="govuk-header__link govuk-header__link--homepage"> {#- The
 SVG needs `focusable="false"` so that Internet Explorer does not treat it as an
 interactive element - without this it will be 'focusable' when using the
 keyboard to navigate. We use a single compound path for the logo to prevent
 subpixel rounding shifting different elements unevenly relative to one another.
-#} {{ (_tudorCrown if params.useTudorCrown else _stEdwardsCrown) | safe }} {%
-if (params.productName) %} {{ params.productName }} {% endif %}
+#} {{ (_stEdwardsCrown if (params.useTudorCrown is not undefined and
+params.useTudorCrown is false) else _tudorCrown) | safe | trim | indent(8) }}
+{% if (params.productName) %} {{ params.productName }} {% endif %}
 {% if params.serviceName or params.navigation | length %}
 {% if params.serviceName %} {% if params.serviceUrl %} _{_{_ _p_a_r_a_m_s_._s_e_r_v_i_c_e_N_a_m_e_ _}_}
-{% else%} {{ params.serviceName }} {% endif %} {% endif %} {% if
+{% else %} {{ params.serviceName }} {% endif %} {% endif %} {% if
 params.navigation | length %}
 %- if params.menuButtonLabel and params.menuButtonLabel != menuButtonText %}
-aria-label="{{ params.menuButtonLabel }}"{% endif %} hidden>{{ menuButtonText
+aria-label="{{ params.menuButtonLabel }}"{% endif %} hidden> {{ menuButtonText
 }}
     * {% for item in params.navigation %} {% if item.text or item.html %}
-    * {% if item.href %} %- for attribute, value in (item.attributes.items() if
-      item.attributes else {}.items()) %} {{ attribute }}="{{ value }}"{%
-      endfor %}> {% endif %} {{ item.html | safe if item.html else item.text }}
-      {% if item.href %}
+    * {% if item.href %} {- govukAttributes(item.attributes) -}}> {% endif %} {
+      { item.html | safe | trim | indent(14) if item.html else item.text }} {%
+      if item.href %}
 {% endif %}
 {% endif %} {% endfor %}
 {% endif %}
 {% endif %}
 {% endmacro %}
```

### Comparing `govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/label/macro.html` & `govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/label/macro.html`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 {% macro govukLabel(params) %}
+{% from "govuk_frontend_jinja/macros/attributes.html" import govukAttributes -%}
+
 {% if params.html or params.text %}
 {% set labelHtml %}
 <label class="govuk-label {%- if params.classes %} {{ params.classes }}{% endif %}"
-  {%- for attribute, value in (params.attributes.items() if params.attributes else {}.items()) %} {{ attribute }}="{{ value }}"{% endfor %}
+  {{- govukAttributes(params.attributes) -}}
   {%- if params.for %} for="{{ params.for }}"{% endif %}>
   {{ params.html | safe | trim | indent(2) if params.html else params.text }}
 </label>
 {% endset -%}
 
 {% if params.isPageHeading %}
 <h1 class="govuk-label-wrapper">
```

### Comparing `govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/notification-banner/macro.html` & `govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/notification-banner/macro.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 {% macro govukNotificationBanner(params) %}
+{% from "govuk_frontend_jinja/macros/attributes.html" import govukAttributes %}
+
 {%- if params.type == "success" %}
-  {% set successBanner = True %}
+  {% set successBanner = true %}
 {% endif %}
 
 {%- if successBanner %}
-  {% set typeClass = "govuk-notification-banner--" + params.type %}
+  {% set typeClass = "govuk-notification-banner--" ~ params.type %}
 {% endif %}
 
 {%- if params.role %}
   {% set role = params.role %}
 {% elif successBanner %}
   {#- If type is success, add `role="alert"` to prioritise the information in the notification banner to users of assistive technologies -#}
   {% set role = "alert" %}
@@ -25,23 +27,25 @@
   {% set title = "Success" %}
 {%- else %}
   {% set title = "Important" %}
 {%- endif -%}
 
 <div class="govuk-notification-banner {%- if typeClass %} {{ typeClass }}{% endif %}{% if params.classes %} {{ params.classes }}{% endif %}" role="{{ role }}" aria-labelledby="{{ params.titleId | default("govuk-notification-banner-title", true) }}" data-module="govuk-notification-banner"
   {%- if params.disableAutoFocus is not undefined %} data-disable-auto-focus="{{ params.disableAutoFocus | lower }}"{% endif %}
-  {%- for attribute, value in (params.attributes.items() if params.attributes else {}.items()) %} {{ attribute }}="{{ value }}"{% endfor %}>
+  {{- govukAttributes(params.attributes) }}>
   <div class="govuk-notification-banner__header">
     <h{{ params.titleHeadingLevel | default(2, true) }} class="govuk-notification-banner__title" id="{{ params.titleId | default("govuk-notification-banner-title", true) }}">
       {{ title }}
     </h{{ params.titleHeadingLevel | default(2, true) }}>
   </div>
   <div class="govuk-notification-banner__content">
-    {%- if caller or params.html -%}
-      {{ caller() if caller else params.html | safe }}
-    {%- elif params.text -%}
-      {# Set default style for single line content #}
-      <p class="govuk-notification-banner__heading">{{ params.text }}</p>
-    {%- endif -%}
+  {% if caller or params.html %}
+    {{ caller() if caller else params.html | safe | trim | indent(4) }}
+  {% elif params.text %}
+    {# Set default style for single line content -#}
+    <p class="govuk-notification-banner__heading">
+      {{ params.text | trim | indent(6) }}
+    </p>
+  {% endif %}
   </div>
 </div>
 {% endmacro %}
```

### Comparing `govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/radios/macro.html` & `govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/radios/macro.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 {% macro govukRadios(params) %}
+{% from "govuk_frontend_jinja/macros/attributes.html" import govukAttributes %}
 {% from "govuk_frontend_jinja/components/error-message/macro.html" import govukErrorMessage %}
 {% from "govuk_frontend_jinja/components/fieldset/macro.html" import govukFieldset %}
 {% from "govuk_frontend_jinja/components/hint/macro.html" import govukHint %}
 {% from "govuk_frontend_jinja/components/label/macro.html" import govukLabel %}
 
 {#- If an id 'prefix' is not passed, fall back to using the name attribute
   instead. We need this for error messages and hints as well -#}
@@ -13,97 +14,100 @@
 {#- a record of other elements that we need to associate with the input using
   aria-describedby – for example hints or error messages -#}
 {% set ns.describedBy = params.fieldset.describedBy if params.fieldset and params.fieldset.describedBy else "" %}
 
 {#- fieldset is false by default -#}
 {% set hasFieldset = true if params.fieldset else false %}
 
+{%- macro _radioItem(params, item, index) %}
+  {#- If the user explicitly sets an id, use this instead of the regular idPrefix -#}
+  {#- The first id should not have a number suffix so it's easy to link to from the error summary component -#}
+  {% set itemId = item.id if item.id else idPrefix ~ ("-" ~ index if index > 1 else "") %}
+  {% set conditionalId = "conditional-" ~ itemId %}
+  {%- if item.divider %}
+    <div class="govuk-radios__divider">{{ item.divider }}</div>
+  {% else %}
+    {% set isChecked = item.checked | default((item.value == params.value and item.checked is not false) if params.value else false, true) %}
+    {% set hasHint = true if item.hint and (item.hint.text or item.hint.html) %}
+    {% set itemHintId = itemId ~ '-item-hint' %}
+    <div class="govuk-radios__item">
+      <input class="govuk-radios__input" id="{{ itemId }}" name="{{ params.name }}" type="radio" value="{{ item.value }}"
+        {{-" checked" if isChecked }}
+        {{-" disabled" if item.disabled }}
+        {%- if item.conditional and item.conditional.html %} data-aria-controls="{{ conditionalId }}"{% endif -%}
+        {%- if hasHint %} aria-describedby="{{ itemHintId }}"{% endif -%}
+        {{- govukAttributes(item.attributes) }}>
+      {{ govukLabel({
+        'html': item.html,
+        'text': item.text,
+        'classes': 'govuk-radios__label' ~ (' ' ~ item.label.classes if item.label and item.label.classes else ""),
+        'attributes': item.label.attributes if item.label,
+        'for': itemId
+      }) | trim | indent(6) }}
+      {% if hasHint %}
+      {{ govukHint({
+        'id': itemHintId,
+        'classes': 'govuk-radios__hint' ~ (' ' ~ item.hint.classes if item.hint and item.hint.classes else ""),
+        'attributes': item.hint.attributes if item.hint,
+        'html': item.hint.html,
+        'text': item.hint.text
+      }) | trim | indent(6) }}
+      {% endif %}
+    </div>
+    {% if item.conditional and item.conditional.html %}
+    <div class="govuk-radios__conditional {%- if not isChecked %} govuk-radios__conditional--hidden{% endif %}" id="{{ conditionalId }}">
+      {{ item.conditional.html | safe | trim }}
+    </div>
+    {% endif %}
+  {% endif %}
+{%- endmacro %}
+
 {#- Capture the HTML so we can optionally nest it in a fieldset -#}
 {% set innerHtml %}
 {% if params.hint %}
-  {% set hintId = idPrefix + '-hint' %}
-  {% set ns.describedBy = ns.describedBy + ' ' + hintId if ns.describedBy else hintId %}
+  {% set hintId = idPrefix ~ '-hint' %}
+  {% set ns.describedBy = ns.describedBy ~ ' ' ~ hintId if ns.describedBy else hintId %}
   {{ govukHint({
     'id': hintId,
     'classes': params.hint.classes,
     'attributes': params.hint.attributes,
     'html': params.hint.html,
     'text': params.hint.text
   }) | trim | indent(2) }}
 {% endif %}
 {% if params.errorMessage %}
-  {% set errorId = idPrefix + '-error' %}
-  {% set ns.describedBy = ns.describedBy + ' ' + errorId if ns.describedBy else errorId %}
+  {% set errorId = idPrefix ~ '-error' %}
+  {% set ns.describedBy = ns.describedBy ~ ' ' ~ errorId if ns.describedBy else errorId %}
   {{ govukErrorMessage({
     'id': errorId,
     'classes': params.errorMessage.classes,
     'attributes': params.errorMessage.attributes,
     'html': params.errorMessage.html,
     'text': params.errorMessage.text,
     'visuallyHiddenText': params.errorMessage.visuallyHiddenText
   }) | trim | indent(2) }}
 {% endif %}
   <div class="govuk-radios {%- if params.classes %} {{ params.classes }}{% endif %}"
-    {%- for attribute, value in (params.attributes.items() if params.attributes else {}.items()) %} {{ attribute }}="{{ value }}"{% endfor %} data-module="govuk-radios">
+    {{- govukAttributes(params.attributes) }} data-module="govuk-radios">
+    {% if params.formGroup and params.formGroup.beforeInputs %}
+    {{ params.formGroup.beforeInputs.html | safe | trim | indent(4) if params.formGroup and params.formGroup.beforeInputs.html else params.formGroup.beforeInputs.text }}
+    {% endif %}
     {% for item in params['items'] %}
       {% if item %}
-        {#- If the user explicitly sets an id, use this instead of the regular idPrefix -#}
-        {%- if item.id -%}
-          {%- set id = item.id -%}
-        {%- else -%}
-          {#- The first id should not have a number suffix so it's easy to link to from the error summary component -#}
-          {%- if loop.first -%}
-            {%- set id = idPrefix %}
-          {% else %}
-            {%- set id = idPrefix + "-" ~ loop.index -%}
-          {%- endif -%}
-        {%- endif -%}
-        {% set conditionalId = "conditional-" + id %}
-        {%- if item.divider %}
-        <div class="govuk-radios__divider">{{ item.divider }}</div>
-        {%- else %}
-        {% set isChecked = item.checked | default((item.value == params.value and item.checked != false) if params.value else false, true) %}
-        {% set hasHint = true if item.hint and (item.hint.text or item.hint.html) %}
-        {% set itemHintId = id + '-item-hint' %}
-        <div class="govuk-radios__item">
-          <input class="govuk-radios__input" id="{{ id }}" name="{{ params.name }}" type="radio" value="{{ item.value }}"
-          {{-" checked" if isChecked }}
-          {{-" disabled" if item.disabled }}
-          {%- if item.conditional and item.conditional.html %} data-aria-controls="{{ conditionalId }}"{% endif -%}
-          {%- if hasHint %} aria-describedby="{{ itemHintId }}"{% endif -%}
-          {%- for attribute, value in (item.attributes.items() if item.attributes else {}.items()) %} {{ attribute }}="{{ value }}"{% endfor %}>
-          {{ govukLabel({
-            'html': item.html,
-            'text': item.text,
-            'classes': 'govuk-radios__label' + (' ' + item.label.classes if item.label and item.label.classes else ''),
-            'attributes': item.label.attributes if item.label,
-            'for': id
-          }) | trim | indent(6) }}
-          {% if hasHint %}
-          {{ govukHint({
-            'id': itemHintId,
-            'classes': 'govuk-radios__hint' + (' ' + item.hint.classes if item.hint.classes else ''),
-            'attributes': item.hint.attributes,
-            'html': item.hint.html,
-            'text': item.hint.text
-          }) | trim | indent(6) }}
-          {% endif %}
-        </div>
-        {% if item.conditional and item.conditional.html %}
-          <div class="govuk-radios__conditional {%- if not isChecked %} govuk-radios__conditional--hidden{% endif %}" id="{{ conditionalId }}">
-            {{ item.conditional.html | safe }}
-          </div>
-        {% endif %}
-        {% endif %}
+        {{- _radioItem(params, item, loop.index) -}}
       {% endif %}
     {% endfor %}
+    {% if params.formGroup and params.formGroup.afterInputs %}
+    {{ params.formGroup.afterInputs.html | safe | trim | indent(4) if params.formGroup and params.formGroup.afterInputs.html else params.formGroup.afterInputs.text }}
+    {% endif %}
   </div>
 {% endset -%}
 
-<div class="govuk-form-group {%- if params.errorMessage %} govuk-form-group--error{% endif %} {%- if params.formGroup and params.formGroup.classes %} {{ params.formGroup.classes }}{% endif %}" {%- for attribute, value in (params.formGroup.attributes.items() if params.formGroup and params.formGroup.attributes else {}.items()) %} {{ attribute }}="{{ value }}"{% endfor %}>
+<div class="govuk-form-group {%- if params.errorMessage %} govuk-form-group--error{% endif %} {%- if params.formGroup and params.formGroup.classes %} {{ params.formGroup.classes }}{% endif %}"
+  {{- govukAttributes(params.formGroup.attributes if params.formGroup) }}>
 {% if hasFieldset %}
   {{ govukFieldset({
     'describedBy': ns.describedBy,
     'classes': params.fieldset.classes,
     'attributes': params.fieldset.attributes,
     'legend': params.fieldset.legend,
     'html': innerHtml | trim
```

### Comparing `govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/summary-list/macro.html` & `govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/summary-list/macro.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,93 +1,96 @@
 {% macro govukSummaryList(params) %}
+{% from "govuk_frontend_jinja/macros/attributes.html" import govukAttributes %}
+
 {%- macro _actionLink(action, cardTitle) %}
-  <a class="govuk-link {%- if action.classes %} {{ action.classes }}{% endif %}" href="{{ action.href }}" {%- for attribute, value in (action.attributes.items() if action.attributes else {}.items()) %} {{ attribute }}="{{ value }}"{% endfor %}>
-    {{- action.html | safe if action.html else action.text -}}
+  <a class="govuk-link {%- if action.classes %} {{ action.classes }}{% endif %}" href="{{ action.href }}"
+    {{- govukAttributes(action.attributes) }}>
+    {{- action.html | safe | indent(4) if action.html else action.text -}}
     {%- if action.visuallyHiddenText or cardTitle -%}
-      <span class="govuk-visually-hidden">
-        {%- if action.visuallyHiddenText %} {{ action.visuallyHiddenText }}{% endif -%}
-        {%- if cardTitle %} ({{ cardTitle.html | safe if cardTitle.html else cardTitle.text }}){% endif -%}
-      </span>
+    <span class="govuk-visually-hidden">
+      {%- if action.visuallyHiddenText %} {{ action.visuallyHiddenText }}{% endif -%}
+      {%- if cardTitle %} ({{ cardTitle.html | indent(6) | safe if cardTitle.html else cardTitle.text }}){% endif -%}
+    </span>
     {%- endif -%}
   </a>
 {% endmacro -%}
 
 {%- macro _summaryCard(params) %}
-  {%- set headingLevel = params.title.headingLevel if params.title and params.title.headingLevel else 2 -%}
+{%- set headingLevel = params.title.headingLevel if params.title and params.title.headingLevel else 2 -%}
 
-  <div class="govuk-summary-card {%- if params.classes %} {{ params.classes }}{% endif %}" {%- for attribute, value in (params.attributes.items() if params.attributes else {}.items()) %} {{ attribute }}="{{ value }}"{% endfor %}>
-    <div class="govuk-summary-card__title-wrapper">
-      {%- if params.title -%}
-        <h{{ headingLevel }} class="govuk-summary-card__title {%- if params.title.classes %} {{ params.title.classes }}{% endif %}">
-          {{- params.title.html | safe if params.title.html else params.title.text -}}
-        </h{{ headingLevel }}>
-      {%- endif -%}
-
-      {%- if params.actions and params.actions['items'] | length -%}
-        {%- if params.actions['items'] | length == 1 -%}
-          <div class="govuk-summary-card__actions {%- if params.actions.classes %} {{ params.actions.classes }}{% endif %}">
-            {{- _actionLink(params.actions['items'][0], params.title) -}}
-          </div>
-        {%- else -%}
-          <ul class="govuk-summary-card__actions {%- if params.actions.classes %} {{ params.actions.classes }}{% endif %}">
-            {%- for action in params.actions['items'] -%}
-              <li class="govuk-summary-card__action">
-                {{- _actionLink(action, params.title) -}}
-              </li>
-            {%- endfor -%}
-          </ul>
-        {% endif -%}
-      {%- endif -%}
+<div class="govuk-summary-card {%- if params.classes %} {{ params.classes }}{% endif %}"
+  {{- govukAttributes(params.attributes) }}>
+  <div class="govuk-summary-card__title-wrapper">
+  {% if params.title %}
+    <h{{ headingLevel }} class="govuk-summary-card__title {%- if params.title.classes %} {{ params.title.classes }}{% endif %}">
+      {{ params.title.html | safe | trim | indent(6) if params.title.html else params.title.text }}
+    </h{{ headingLevel }}>
+  {% endif %}
+  {% if params.actions and params.actions['items'] | length %}
+    {% if params.actions['items'] | length == 1 %}
+    <div class="govuk-summary-card__actions {%- if params.actions.classes %} {{ params.actions.classes }}{% endif %}">
+      {{ _actionLink(params.actions['items'][0], params.title) | trim | indent(4) }}
     </div>
+    {% else %}
+    <ul class="govuk-summary-card__actions {%- if params.actions.classes %} {{ params.actions.classes }}{% endif %}">
+      {% for action in params.actions['items'] %}
+      <li class="govuk-summary-card__action">
+        {{ _actionLink(action, params.title) | trim | indent(8) }}
+      </li>
+      {% endfor %}
+    </ul>
+    {% endif %}
+  {% endif %}
+  </div>
 
-    <div class="govuk-summary-card__content">
-      {{- caller() -}}
-    </div>
+  <div class="govuk-summary-card__content">
+    {{ caller() | trim }}
   </div>
+</div>
 {% endmacro -%}
 
-{# Determine if we need 2 or 3 columns #}
-{% set ns = namespace(anyRowHasActions = false) %}
+{#- Determine if we need 2 or 3 columns #}
+{%- set ns = namespace(anyRowHasActions = false) %}
 {% for row in params.rows %}
   {% set ns.anyRowHasActions = true if row.actions and row.actions['items'] | length else ns.anyRowHasActions %}
 {% endfor -%}
 
 {%- set summaryList -%}
-  <dl class="govuk-summary-list {%- if params.classes %} {{ params.classes }}{% endif %}" {%- for attribute, value in (params.attributes.items() if params.attributes else {}.items()) %} {{ attribute }}="{{ value }}"{% endfor %}>
-    {% for row in params.rows %}
-      {% if row %}
-        <div class="govuk-summary-list__row {%- if ns.anyRowHasActions and not (row.actions and row.actions['items']) %} govuk-summary-list__row--no-actions{% endif %} {%- if row.classes %} {{ row.classes }}{% endif %}">
-          <dt class="govuk-summary-list__key {%- if row.key.classes %} {{ row.key.classes }}{% endif %}">
-            {{ row.key.html | indent(4 if params.card else 0) | safe if row.key.html else row.key.text }}
-          </dt>
-          <dd class="govuk-summary-list__value {%- if row.value.classes %} {{ row.value.classes }}{% endif %}">
-            {{ row.value.html | indent(12 if params.card else 8) | safe | trim if row.value.html else row.value.text }}
-          </dd>
-          {% if row.actions and row.actions['items'] | length %}
-            <dd class="govuk-summary-list__actions {%- if row.actions.classes %} {{ row.actions.classes }}{% endif %}">
-              {% if row.actions['items'] | length == 1 %}
-                {{ _actionLink(row.actions['items'][0], params.card.title if params.card) | indent(16 if params.card else 12) | trim }}
-              {% else %}
-                <ul class="govuk-summary-list__actions-list">
-                  {%- for action in row.actions['items'] -%}
-                    <li class="govuk-summary-list__actions-list-item">
-                      {{- _actionLink(action, params.card.title if params.card) | indent(22 if params.card else 18) | trim -}}
-                    </li>
-                  {%- endfor -%}
-                </ul>
-              {% endif %}
-            </dd>
-          {% endif %}
-        </div>
+<dl class="govuk-summary-list {%- if params.classes %} {{ params.classes }}{% endif %}" {{- govukAttributes(params.attributes) }}>
+{% for row in params.rows %}
+  {% if row %}
+  <div class="govuk-summary-list__row {%- if ns.anyRowHasActions and not (row.actions and row.actions['items']) %} govuk-summary-list__row--no-actions{% endif %} {%- if row.classes %} {{ row.classes }}{% endif %}">
+    <dt class="govuk-summary-list__key {%- if row.key.classes %} {{ row.key.classes }}{% endif %}">
+      {{ row.key.html | safe | trim | indent(6) if row.key.html else row.key.text }}
+    </dt>
+    <dd class="govuk-summary-list__value {%- if row.value.classes %} {{ row.value.classes }}{% endif %}">
+      {{ row.value.html | safe | trim | indent(6) if row.value.html else row.value.text }}
+    </dd>
+    {% if row.actions and row.actions['items'] | length %}
+    <dd class="govuk-summary-list__actions {%- if row.actions.classes %} {{ row.actions.classes }}{% endif %}">
+      {% if row.actions and row.actions['items'] | length == 1 %}
+        {{- _actionLink(row.actions['items'][0], params.card.title if params.card) | trim | indent(6, true) }}
+      {% else %}
+      <ul class="govuk-summary-list__actions-list">
+        {% for action in row.actions['items'] %}
+        <li class="govuk-summary-list__actions-list-item">
+          {{ _actionLink(action, params.card.title if params.card) | trim | indent(8) }}
+        </li>
+        {% endfor %}
+      </ul>
       {% endif %}
-    {% endfor %}
-  </dl>
+    </dd>
+    {% endif %}
+  </div>
+  {% endif %}
+{% endfor %}
+</dl>
 {%- endset %}
 
 {%- if params.card -%}
   {% call _summaryCard(params.card) -%}
-    {{ summaryList | safe }}
+    {{ summaryList | safe | trim | indent(4) }}
   {%- endcall %}
 {%- else -%}
-  {{ summaryList | safe }}
+  {{ summaryList | safe | trim }}
 {%- endif %}
 {% endmacro %}
```

### Comparing `govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/table/macro.html` & `govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/task-list/macro.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,147 +1,128 @@
 00000000: 7b25 206d 6163 726f 2067 6f76 756b 5461  {% macro govukTa
-00000010: 626c 6528 7061 7261 6d73 2920 257d 0a3c  ble(params) %}.<
-00000020: 7461 626c 6520 636c 6173 733d 2267 6f76  table class="gov
-00000030: 756b 2d74 6162 6c65 0a20 207b 252d 2069  uk-table.  {%- i
-00000040: 6620 7061 7261 6d73 2e63 6c61 7373 6573  f params.classes
-00000050: 2025 7d20 7b7b 2070 6172 616d 732e 636c   %} {{ params.cl
-00000060: 6173 7365 7320 7d7d 7b25 2065 6e64 6966  asses }}{% endif
-00000070: 2025 7d22 207b 252d 2066 6f72 2061 7474   %}" {%- for att
-00000080: 7269 6275 7465 2c20 7661 6c75 6520 696e  ribute, value in
-00000090: 2028 7061 7261 6d73 2e61 7474 7269 6275   (params.attribu
-000000a0: 7465 732e 6974 656d 7328 2920 6966 2070  tes.items() if p
-000000b0: 6172 616d 732e 6174 7472 6962 7574 6573  arams.attributes
-000000c0: 2065 6c73 6520 7b7d 2e69 7465 6d73 2829   else {}.items()
-000000d0: 2920 257d 207b 7b20 6174 7472 6962 7574  ) %} {{ attribut
-000000e0: 6520 7d7d 3d22 7b7b 2076 616c 7565 207d  e }}="{{ value }
-000000f0: 7d22 7b25 2065 6e64 666f 7220 257d 3e0a  }"{% endfor %}>.
-00000100: 2020 7b25 2069 6620 7061 7261 6d73 2e63    {% if params.c
-00000110: 6170 7469 6f6e 2025 7d0a 2020 3c63 6170  aption %}.  <cap
-00000120: 7469 6f6e 2063 6c61 7373 3d22 676f 7675  tion class="govu
-00000130: 6b2d 7461 626c 655f 5f63 6170 7469 6f6e  k-table__caption
-00000140: 0a20 207b 252d 2069 6620 7061 7261 6d73  .  {%- if params
-00000150: 2e63 6170 7469 6f6e 436c 6173 7365 7320  .captionClasses 
-00000160: 257d 207b 7b20 7061 7261 6d73 2e63 6170  %} {{ params.cap
-00000170: 7469 6f6e 436c 6173 7365 7320 7d7d 7b25  tionClasses }}{%
-00000180: 2065 6e64 6966 2025 7d22 3e7b 7b20 7061   endif %}">{{ pa
-00000190: 7261 6d73 2e63 6170 7469 6f6e 207d 7d3c  rams.caption }}<
-000001a0: 2f63 6170 7469 6f6e 3e0a 2020 7b25 2065  /caption>.  {% e
-000001b0: 6e64 6966 2025 7d0a 2020 7b25 2069 6620  ndif %}.  {% if 
-000001c0: 7061 7261 6d73 2e68 6561 6420 257d 0a20  params.head %}. 
-000001d0: 203c 7468 6561 6420 636c 6173 733d 2267   <thead class="g
-000001e0: 6f76 756b 2d74 6162 6c65 5f5f 6865 6164  ovuk-table__head
-000001f0: 223e 0a20 2020 203c 7472 2063 6c61 7373  ">.    <tr class
-00000200: 3d22 676f 7675 6b2d 7461 626c 655f 5f72  ="govuk-table__r
-00000210: 6f77 223e 0a20 2020 207b 2520 666f 7220  ow">.    {% for 
-00000220: 6974 656d 2069 6e20 7061 7261 6d73 2e68  item in params.h
-00000230: 6561 6420 257d 0a20 2020 2020 203c 7468  ead %}.      <th
-00000240: 2073 636f 7065 3d22 636f 6c22 2063 6c61   scope="col" cla
-00000250: 7373 3d22 676f 7675 6b2d 7461 626c 655f  ss="govuk-table_
-00000260: 5f68 6561 6465 720a 2020 2020 2020 7b25  _header.      {%
-00000270: 2d20 6966 2069 7465 6d2e 666f 726d 6174  - if item.format
-00000280: 2025 7d20 676f 7675 6b2d 7461 626c 655f   %} govuk-table_
-00000290: 5f68 6561 6465 722d 2d7b 7b20 6974 656d  _header--{{ item
-000002a0: 2e66 6f72 6d61 7420 7d7d 7b25 2065 6e64  .format }}{% end
-000002b0: 6966 2025 7d0a 2020 2020 2020 7b25 2d20  if %}.      {%- 
-000002c0: 6966 2069 7465 6d2e 636c 6173 7365 7320  if item.classes 
-000002d0: 257d 207b 7b20 6974 656d 2e63 6c61 7373  %} {{ item.class
-000002e0: 6573 207d 7d7b 2520 656e 6469 6620 257d  es }}{% endif %}
-000002f0: 220a 2020 2020 2020 7b25 2d20 6966 2069  ".      {%- if i
-00000300: 7465 6d2e 636f 6c73 7061 6e20 257d 2063  tem.colspan %} c
-00000310: 6f6c 7370 616e 3d22 7b7b 2069 7465 6d2e  olspan="{{ item.
-00000320: 636f 6c73 7061 6e20 7d7d 227b 2520 656e  colspan }}"{% en
-00000330: 6469 6620 257d 0a20 2020 2020 207b 252d  dif %}.      {%-
-00000340: 2069 6620 6974 656d 2e72 6f77 7370 616e   if item.rowspan
-00000350: 2025 7d20 726f 7773 7061 6e3d 227b 7b20   %} rowspan="{{ 
-00000360: 6974 656d 2e72 6f77 7370 616e 207d 7d22  item.rowspan }}"
-00000370: 7b25 2065 6e64 6966 2025 7d7b 2520 666f  {% endif %}{% fo
-00000380: 7220 6174 7472 6962 7574 652c 2076 616c  r attribute, val
-00000390: 7565 2069 6e20 2869 7465 6d2e 6174 7472  ue in (item.attr
-000003a0: 6962 7574 6573 2e69 7465 6d73 2829 2069  ibutes.items() i
-000003b0: 6620 6974 656d 2e61 7474 7269 6275 7465  f item.attribute
-000003c0: 7320 656c 7365 207b 7d2e 6974 656d 7328  s else {}.items(
-000003d0: 2929 2025 7d20 7b7b 2061 7474 7269 6275  )) %} {{ attribu
-000003e0: 7465 207d 7d3d 227b 7b20 7661 6c75 6520  te }}="{{ value 
-000003f0: 7d7d 227b 2520 656e 6466 6f72 2025 7d3e  }}"{% endfor %}>
-00000400: 7b7b 2069 7465 6d2e 6874 6d6c 207c 7361  {{ item.html |sa
-00000410: 6665 2069 6620 6974 656d 2e68 746d 6c20  fe if item.html 
-00000420: 656c 7365 2069 7465 6d2e 7465 7874 207d  else item.text }
-00000430: 7d3c 2f74 683e 0a20 2020 207b 2520 656e  }</th>.    {% en
-00000440: 6466 6f72 2025 7d0a 2020 2020 3c2f 7472  dfor %}.    </tr
-00000450: 3e0a 2020 3c2f 7468 6561 643e 0a20 207b  >.  </thead>.  {
-00000460: 2520 656e 6469 6620 257d 0a20 203c 7462  % endif %}.  <tb
-00000470: 6f64 7920 636c 6173 733d 2267 6f76 756b  ody class="govuk
-00000480: 2d74 6162 6c65 5f5f 626f 6479 223e 0a20  -table__body">. 
-00000490: 2020 207b 2520 666f 7220 726f 7720 696e     {% for row in
-000004a0: 2070 6172 616d 732e 726f 7773 2025 7d0a   params.rows %}.
-000004b0: 2020 2020 2020 7b25 2069 6620 726f 7720        {% if row 
-000004c0: 257d 0a20 2020 2020 2020 203c 7472 2063  %}.        <tr c
-000004d0: 6c61 7373 3d22 676f 7675 6b2d 7461 626c  lass="govuk-tabl
-000004e0: 655f 5f72 6f77 223e 0a20 2020 2020 2020  e__row">.       
-000004f0: 207b 2520 666f 7220 6365 6c6c 2069 6e20   {% for cell in 
-00000500: 726f 7720 257d 0a20 2020 2020 2020 2020  row %}.         
-00000510: 207b 2520 7365 7420 636f 6d6d 6f6e 4174   {% set commonAt
-00000520: 7472 6962 7574 6573 2025 7d0a 2020 2020  tributes %}.    
-00000530: 2020 2020 2020 2020 7b25 2d20 6966 2063          {%- if c
-00000540: 656c 6c2e 636f 6c73 7061 6e20 257d 2063  ell.colspan %} c
-00000550: 6f6c 7370 616e 3d22 7b7b 2063 656c 6c2e  olspan="{{ cell.
-00000560: 636f 6c73 7061 6e20 7d7d 227b 2520 656e  colspan }}"{% en
-00000570: 6469 6620 257d 0a20 2020 2020 2020 2020  dif %}.         
-00000580: 2020 207b 252d 2069 6620 6365 6c6c 2e72     {%- if cell.r
-00000590: 6f77 7370 616e 2025 7d20 726f 7773 7061  owspan %} rowspa
-000005a0: 6e3d 227b 7b20 6365 6c6c 2e72 6f77 7370  n="{{ cell.rowsp
-000005b0: 616e 207d 7d22 7b25 2065 6e64 6966 2025  an }}"{% endif %
-000005c0: 7d7b 2520 666f 7220 6174 7472 6962 7574  }{% for attribut
-000005d0: 652c 2076 616c 7565 2069 6e20 2863 656c  e, value in (cel
-000005e0: 6c2e 6174 7472 6962 7574 6573 2e69 7465  l.attributes.ite
-000005f0: 6d73 2829 2069 6620 6365 6c6c 2e61 7474  ms() if cell.att
-00000600: 7269 6275 7465 7320 656c 7365 207b 7d2e  ributes else {}.
-00000610: 6974 656d 7328 2929 2025 7d20 7b7b 2061  items()) %} {{ a
-00000620: 7474 7269 6275 7465 207d 7d3d 227b 7b20  ttribute }}="{{ 
-00000630: 7661 6c75 6520 7d7d 227b 2520 656e 6466  value }}"{% endf
-00000640: 6f72 2025 7d0a 2020 2020 2020 2020 2020  or %}.          
-00000650: 7b25 2065 6e64 7365 7420 257d 0a20 2020  {% endset %}.   
-00000660: 2020 2020 2020 207b 2520 6966 206c 6f6f         {% if loo
-00000670: 702e 6669 7273 7420 616e 6420 7061 7261  p.first and para
-00000680: 6d73 2e66 6972 7374 4365 6c6c 4973 4865  ms.firstCellIsHe
-00000690: 6164 6572 2025 7d0a 2020 2020 2020 2020  ader %}.        
-000006a0: 2020 3c74 6820 7363 6f70 653d 2272 6f77    <th scope="row
-000006b0: 2220 636c 6173 733d 2267 6f76 756b 2d74  " class="govuk-t
-000006c0: 6162 6c65 5f5f 6865 6164 6572 207b 252d  able__header {%-
-000006d0: 2069 6620 6365 6c6c 2e63 6c61 7373 6573   if cell.classes
-000006e0: 2025 7d20 7b7b 2063 656c 6c2e 636c 6173   %} {{ cell.clas
-000006f0: 7365 7320 7d7d 7b25 2065 6e64 6966 2025  ses }}{% endif %
-00000700: 7d22 0a20 2020 2020 2020 2020 2020 207b  }".            {
-00000710: 7b2d 2063 6f6d 6d6f 6e41 7474 7269 6275  {- commonAttribu
-00000720: 7465 7320 7c20 7361 6665 202d 7d7d 0a20  tes | safe -}}. 
-00000730: 2020 2020 2020 2020 203e 7b7b 2063 656c           >{{ cel
-00000740: 6c2e 6874 6d6c 207c 2073 6166 6520 6966  l.html | safe if
-00000750: 2063 656c 6c2e 6874 6d6c 2065 6c73 6520   cell.html else 
-00000760: 6365 6c6c 2e74 6578 7420 7d7d 3c2f 7468  cell.text }}</th
-00000770: 3e0a 2020 2020 2020 2020 2020 7b25 2065  >.          {% e
-00000780: 6c73 6520 257d 0a20 2020 2020 2020 2020  lse %}.         
-00000790: 203c 7464 2063 6c61 7373 3d22 676f 7675   <td class="govu
-000007a0: 6b2d 7461 626c 655f 5f63 656c 6c0a 2020  k-table__cell.  
-000007b0: 2020 2020 2020 2020 2020 7b25 2d20 6966            {%- if
-000007c0: 2063 656c 6c2e 666f 726d 6174 2025 7d20   cell.format %} 
-000007d0: 676f 7675 6b2d 7461 626c 655f 5f63 656c  govuk-table__cel
-000007e0: 6c2d 2d7b 7b20 6365 6c6c 2e66 6f72 6d61  l--{{ cell.forma
-000007f0: 7420 7d7d 7b25 2065 6e64 6966 2025 7d0a  t }}{% endif %}.
-00000800: 2020 2020 2020 2020 2020 2020 7b25 2d20              {%- 
-00000810: 6966 2063 656c 6c2e 636c 6173 7365 7320  if cell.classes 
-00000820: 257d 207b 7b20 6365 6c6c 2e63 6c61 7373  %} {{ cell.class
-00000830: 6573 207d 7d7b 2520 656e 6469 6620 257d  es }}{% endif %}
-00000840: 220a 2020 2020 2020 2020 2020 2020 7b7b  ".            {{
-00000850: 2d20 636f 6d6d 6f6e 4174 7472 6962 7574  - commonAttribut
-00000860: 6573 207c 2073 6166 6520 2d7d 7d0a 2020  es | safe -}}.  
-00000870: 2020 2020 2020 2020 3e7b 7b20 6365 6c6c          >{{ cell
-00000880: 2e68 746d 6c20 7c20 7361 6665 2069 6620  .html | safe if 
-00000890: 6365 6c6c 2e68 746d 6c20 656c 7365 2063  cell.html else c
-000008a0: 656c 6c2e 7465 7874 207d 7d3c 2f74 643e  ell.text }}</td>
-000008b0: 0a20 2020 2020 2020 2020 207b 2520 656e  .          {% en
-000008c0: 6469 6620 257d 0a20 2020 2020 2020 207b  dif %}.        {
-000008d0: 2520 656e 6466 6f72 2025 7d0a 2020 2020  % endfor %}.    
-000008e0: 2020 2020 3c2f 7472 3e0a 2020 2020 2020      </tr>.      
-000008f0: 7b25 2065 6e64 6966 2025 7d0a 2020 2020  {% endif %}.    
-00000900: 7b25 2065 6e64 666f 7220 257d 0a20 203c  {% endfor %}.  <
-00000910: 2f74 626f 6479 3e0a 3c2f 7461 626c 653e  /tbody>.</table>
-00000920: 0a7b 2520 656e 646d 6163 726f 2025 7d0a  .{% endmacro %}.
+00000010: 736b 4c69 7374 2870 6172 616d 7329 2025  skList(params) %
+00000020: 7d0a 7b25 2066 726f 6d20 2267 6f76 756b  }.{% from "govuk
+00000030: 5f66 726f 6e74 656e 645f 6a69 6e6a 612f  _frontend_jinja/
+00000040: 6d61 6372 6f73 2f61 7474 7269 6275 7465  macros/attribute
+00000050: 732e 6874 6d6c 2220 696d 706f 7274 2067  s.html" import g
+00000060: 6f76 756b 4174 7472 6962 7574 6573 2025  ovukAttributes %
+00000070: 7d0a 7b25 2066 726f 6d20 2267 6f76 756b  }.{% from "govuk
+00000080: 5f66 726f 6e74 656e 645f 6a69 6e6a 612f  _frontend_jinja/
+00000090: 636f 6d70 6f6e 656e 7473 2f74 6167 2f6d  components/tag/m
+000000a0: 6163 726f 2e68 746d 6c22 2069 6d70 6f72  acro.html" impor
+000000b0: 7420 676f 7675 6b54 6167 2025 7d0a 0a7b  t govukTag %}..{
+000000c0: 252d 2073 6574 2069 6450 7265 6669 7820  %- set idPrefix 
+000000d0: 3d20 7061 7261 6d73 2e69 6450 7265 6669  = params.idPrefi
+000000e0: 7820 6966 2070 6172 616d 732e 6964 5072  x if params.idPr
+000000f0: 6566 6978 2065 6c73 6520 2274 6173 6b2d  efix else "task-
+00000100: 6c69 7374 2220 2d25 7d0a 0a7b 252d 206d  list" -%}..{%- m
+00000110: 6163 726f 205f 7461 736b 4c69 7374 4974  acro _taskListIt
+00000120: 656d 2870 6172 616d 732c 2069 7465 6d2c  em(params, item,
+00000130: 2069 6e64 6578 2920 257d 0a20 207b 252d   index) %}.  {%-
+00000140: 2073 6574 2068 696e 7449 6420 3d20 6964   set hintId = id
+00000150: 5072 6566 6978 207e 2022 2d22 207e 2069  Prefix ~ "-" ~ i
+00000160: 6e64 6578 207e 2022 2d68 696e 7422 2025  ndex ~ "-hint" %
+00000170: 7d0a 2020 7b25 2d20 7365 7420 7374 6174  }.  {%- set stat
+00000180: 7573 4964 203d 2069 6450 7265 6669 7820  usId = idPrefix 
+00000190: 7e20 222d 2220 7e20 696e 6465 7820 7e20  ~ "-" ~ index ~ 
+000001a0: 222d 7374 6174 7573 2220 257d 0a20 203c  "-status" %}.  <
+000001b0: 6c69 2063 6c61 7373 3d22 676f 7675 6b2d  li class="govuk-
+000001c0: 7461 736b 2d6c 6973 745f 5f69 7465 6d20  task-list__item 
+000001d0: 7b25 2d20 6966 2069 7465 6d2e 6872 6566  {%- if item.href
+000001e0: 2025 7d20 676f 7675 6b2d 7461 736b 2d6c   %} govuk-task-l
+000001f0: 6973 745f 5f69 7465 6d2d 2d77 6974 682d  ist__item--with-
+00000200: 6c69 6e6b 7b25 2065 6e64 6966 2025 7d7b  link{% endif %}{
+00000210: 252d 2069 6620 6974 656d 2e63 6c61 7373  %- if item.class
+00000220: 6573 2025 7d20 7b7b 2069 7465 6d2e 636c  es %} {{ item.cl
+00000230: 6173 7365 7320 7d7d 7b25 2065 6e64 6966  asses }}{% endif
+00000240: 2025 7d22 3e0a 2020 2020 3c64 6976 2063   %}">.    <div c
+00000250: 6c61 7373 3d22 676f 7675 6b2d 7461 736b  lass="govuk-task
+00000260: 2d6c 6973 745f 5f6e 616d 652d 616e 642d  -list__name-and-
+00000270: 6869 6e74 223e 0a20 2020 207b 2520 6966  hint">.    {% if
+00000280: 2069 7465 6d2e 6872 6566 2025 7d0a 2020   item.href %}.  
+00000290: 2020 2020 3c61 2063 6c61 7373 3d22 676f      <a class="go
+000002a0: 7675 6b2d 6c69 6e6b 2067 6f76 756b 2d74  vuk-link govuk-t
+000002b0: 6173 6b2d 6c69 7374 5f5f 6c69 6e6b 207b  ask-list__link {
+000002c0: 252d 2069 6620 6974 656d 2e74 6974 6c65  %- if item.title
+000002d0: 2e63 6c61 7373 6573 2025 7d20 7b7b 2069  .classes %} {{ i
+000002e0: 7465 6d2e 7469 746c 652e 636c 6173 7365  tem.title.classe
+000002f0: 7320 7d7d 7b25 2065 6e64 6966 2025 7d22  s }}{% endif %}"
+00000300: 2068 7265 663d 227b 7b20 6974 656d 2e68   href="{{ item.h
+00000310: 7265 6620 7d7d 2220 6172 6961 2d64 6573  ref }}" aria-des
+00000320: 6372 6962 6564 6279 3d22 7b7b 2068 696e  cribedby="{{ hin
+00000330: 7449 6420 7e20 2220 2220 6966 2069 7465  tId ~ " " if ite
+00000340: 6d2e 6869 6e74 207d 7d7b 7b20 7374 6174  m.hint }}{{ stat
+00000350: 7573 4964 207d 7d22 3e0a 2020 2020 2020  usId }}">.      
+00000360: 2020 7b7b 2069 7465 6d2e 7469 746c 652e    {{ item.title.
+00000370: 6874 6d6c 207c 2073 6166 6520 7c20 7472  html | safe | tr
+00000380: 696d 207c 2069 6e64 656e 7428 3829 2069  im | indent(8) i
+00000390: 6620 6974 656d 2e74 6974 6c65 2e68 746d  f item.title.htm
+000003a0: 6c20 656c 7365 2069 7465 6d2e 7469 746c  l else item.titl
+000003b0: 652e 7465 7874 207d 7d0a 2020 2020 2020  e.text }}.      
+000003c0: 3c2f 613e 0a20 2020 207b 2520 656c 7365  </a>.    {% else
+000003d0: 2025 7d0a 2020 2020 2020 3c64 6976 207b   %}.      <div {
+000003e0: 252d 2069 6620 6974 656d 2e74 6974 6c65  %- if item.title
+000003f0: 2e63 6c61 7373 6573 2025 7d20 636c 6173  .classes %} clas
+00000400: 733d 227b 7b20 6974 656d 2e74 6974 6c65  s="{{ item.title
+00000410: 2e63 6c61 7373 6573 207d 7d22 7b25 2065  .classes }}"{% e
+00000420: 6e64 6966 2025 7d3e 0a20 2020 2020 2020  ndif %}>.       
+00000430: 207b 7b20 6974 656d 2e74 6974 6c65 2e68   {{ item.title.h
+00000440: 746d 6c20 7c20 7361 6665 207c 2074 7269  tml | safe | tri
+00000450: 6d20 7c20 696e 6465 6e74 2838 2920 6966  m | indent(8) if
+00000460: 2069 7465 6d2e 7469 746c 652e 6874 6d6c   item.title.html
+00000470: 2065 6c73 6520 6974 656d 2e74 6974 6c65   else item.title
+00000480: 2e74 6578 7420 7d7d 0a20 2020 2020 203c  .text }}.      <
+00000490: 2f64 6976 3e0a 2020 2020 7b25 2065 6e64  /div>.    {% end
+000004a0: 6966 2025 7d0a 2020 2020 7b25 2069 6620  if %}.    {% if 
+000004b0: 6974 656d 2e68 696e 7420 257d 0a20 2020  item.hint %}.   
+000004c0: 2020 203c 6469 7620 6964 3d22 7b7b 2068     <div id="{{ h
+000004d0: 696e 7449 6420 7d7d 2220 636c 6173 733d  intId }}" class=
+000004e0: 2267 6f76 756b 2d74 6173 6b2d 6c69 7374  "govuk-task-list
+000004f0: 5f5f 6869 6e74 223e 0a20 2020 2020 2020  __hint">.       
+00000500: 207b 7b20 6974 656d 2e68 696e 742e 6874   {{ item.hint.ht
+00000510: 6d6c 207c 2073 6166 6520 7c20 7472 696d  ml | safe | trim
+00000520: 207c 2069 6e64 656e 7428 3829 2069 6620   | indent(8) if 
+00000530: 6974 656d 2e68 696e 742e 6874 6d6c 2065  item.hint.html e
+00000540: 6c73 6520 6974 656d 2e68 696e 742e 7465  lse item.hint.te
+00000550: 7874 207d 7d0a 2020 2020 2020 3c2f 6469  xt }}.      </di
+00000560: 763e 0a20 2020 207b 2520 656e 6469 6620  v>.    {% endif 
+00000570: 257d 0a20 2020 203c 2f64 6976 3e0a 2020  %}.    </div>.  
+00000580: 2020 3c64 6976 2063 6c61 7373 3d22 676f    <div class="go
+00000590: 7675 6b2d 7461 736b 2d6c 6973 745f 5f73  vuk-task-list__s
+000005a0: 7461 7475 7320 7b25 2d20 6966 2069 7465  tatus {%- if ite
+000005b0: 6d2e 7374 6174 7573 2e63 6c61 7373 6573  m.status.classes
+000005c0: 2025 7d20 7b7b 2069 7465 6d2e 7374 6174   %} {{ item.stat
+000005d0: 7573 2e63 6c61 7373 6573 207d 7d7b 2520  us.classes }}{% 
+000005e0: 656e 6469 6620 257d 2220 6964 3d22 7b7b  endif %}" id="{{
+000005f0: 2073 7461 7475 7349 6420 7d7d 223e 0a20   statusId }}">. 
+00000600: 2020 207b 2520 6966 2069 7465 6d2e 7374     {% if item.st
+00000610: 6174 7573 2e74 6167 2025 7d0a 2020 2020  atus.tag %}.    
+00000620: 2020 7b7b 2067 6f76 756b 5461 6728 6974    {{ govukTag(it
+00000630: 656d 2e73 7461 7475 732e 7461 6729 207c  em.status.tag) |
+00000640: 2074 7269 6d20 7c20 696e 6465 6e74 2836   trim | indent(6
+00000650: 2920 7d7d 0a20 2020 207b 2520 656c 7365  ) }}.    {% else
+00000660: 2025 7d0a 2020 2020 2020 7b7b 2069 7465   %}.      {{ ite
+00000670: 6d2e 7374 6174 7573 2e68 746d 6c20 7c20  m.status.html | 
+00000680: 7361 6665 207c 2074 7269 6d20 7c20 696e  safe | trim | in
+00000690: 6465 6e74 2836 2920 6966 2069 7465 6d2e  dent(6) if item.
+000006a0: 7374 6174 7573 2e68 746d 6c20 656c 7365  status.html else
+000006b0: 2069 7465 6d2e 7374 6174 7573 2e74 6578   item.status.tex
+000006c0: 7420 7d7d 0a20 2020 207b 2520 656e 6469  t }}.    {% endi
+000006d0: 6620 257d 0a20 2020 203c 2f64 6976 3e0a  f %}.    </div>.
+000006e0: 2020 3c2f 6c69 3e0a 7b25 2d20 656e 646d    </li>.{%- endm
+000006f0: 6163 726f 2025 7d0a 0a3c 756c 2063 6c61  acro %}..<ul cla
+00000700: 7373 3d22 676f 7675 6b2d 7461 736b 2d6c  ss="govuk-task-l
+00000710: 6973 7420 7b25 2d20 6966 2070 6172 616d  ist {%- if param
+00000720: 732e 636c 6173 7365 7320 257d 207b 7b20  s.classes %} {{ 
+00000730: 7061 7261 6d73 2e63 6c61 7373 6573 207d  params.classes }
+00000740: 7d7b 2520 656e 6469 6620 257d 220a 2020  }{% endif %}".  
+00000750: 7b7b 2d20 676f 7675 6b41 7474 7269 6275  {{- govukAttribu
+00000760: 7465 7328 7061 7261 6d73 2e61 7474 7269  tes(params.attri
+00000770: 6275 7465 7329 207d 7d3e 0a20 207b 2520  butes) }}>.  {% 
+00000780: 666f 7220 6974 656d 2069 6e20 7061 7261  for item in para
+00000790: 6d73 5b27 6974 656d 7327 5d20 257d 0a20  ms['items'] %}. 
+000007a0: 2020 207b 7b2d 205f 7461 736b 4c69 7374     {{- _taskList
+000007b0: 4974 656d 2870 6172 616d 732c 2069 7465  Item(params, ite
+000007c0: 6d2c 206c 6f6f 702e 696e 6465 7829 207d  m, loop.index) }
+000007d0: 7d0a 2020 7b25 2065 6e64 666f 7220 257d  }.  {% endfor %}
+000007e0: 0a3c 2f75 6c3e 0a7b 2520 656e 646d 6163  .</ul>.{% endmac
+000007f0: 726f 2025 7d                             ro %}
```

### Comparing `govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/tabs/macro.html` & `govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/tabs/macro.html`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,50 @@
 {% macro govukTabs(params) %}
+{% from "govuk_frontend_jinja/macros/attributes.html" import govukAttributes %}
+
+{%- macro _tabListItem(params, item, index) %}
+{% set tabPanelId = item.id if item.id else idPrefix ~ "-" ~ index -%}
+<li class="govuk-tabs__list-item {%- if index == 1 %} govuk-tabs__list-item--selected{% endif %}">
+  <a class="govuk-tabs__tab" href="#{{ tabPanelId }}"
+    {{- govukAttributes(item.attributes) }}>
+    {{ item.label }}
+  </a>
+</li>
+{% endmacro -%}
+
+{%- macro _tabPanel(params, item, index) %}
+{% set tabPanelId = item.id if item.id else idPrefix ~ "-" ~ index -%}
+<div class="govuk-tabs__panel {%- if index > 1 %} govuk-tabs__panel--hidden{% endif %}" id="{{ tabPanelId }}"
+  {{- govukAttributes(item.panel.attributes) }}>
+{% if item.panel.html %}
+  {{ item.panel.html | safe | trim | indent(2) }}
+{% elif item.panel.text %}
+  <p class="govuk-body">{{ item.panel.text }}</p>
+{% endif %}
+</div>
+{% endmacro -%}
+
 {#- If an id 'prefix' is not passed, fall back to using the name attribute
   instead. We need this for error messages and hints as well -#}
 {% set idPrefix = params.idPrefix if params.idPrefix -%}
 
-<div {%- if params.id %} id="{{ params.id }}"{% endif %} class="govuk-tabs {%- if params.classes %} {{ params.classes }}{% endif %}" {%- for attribute, value in (params.attributes.items() if params.attributes else {}.items()) %} {{ attribute }}="{{ value }}"{% endfor %} data-module="govuk-tabs">
+<div {%- if params.id %} id="{{ params.id }}"{% endif %} class="govuk-tabs {%- if params.classes %} {{ params.classes }}{% endif %}"
+  {{- govukAttributes(params.attributes) }} data-module="govuk-tabs">
   <h2 class="govuk-tabs__title">
     {{ params.title | default ("Contents") }}
   </h2>
-  {% if 'items' in params and params['items'] | length %}
+{% if 'items' in params and params['items'] | length %}
   <ul class="govuk-tabs__list">
     {% for item in params['items'] %}
       {% if item %}
-        {% set id = item.id if item.id else idPrefix + "-" ~ loop.index %}
-        <li class="govuk-tabs__list-item {%- if loop.index == 1 %} govuk-tabs__list-item--selected{% endif %}">
-          <a class="govuk-tabs__tab" href="#{{ id }}"
-            {%- for attribute, value in (item.attributes.items() if item.attributes else {}.items()) %} {{ attribute }}="{{ value }}"{% endfor %}>
-            {{ item.label }}
-          </a>
-        </li>
+        {{- _tabListItem(params, item, loop.index) | trim | indent(4, true) }}
       {% endif %}
     {% endfor %}
   </ul>
-  {% endif %}
-  {% if 'items' in params and params['items'] | length %}
-    {% for item in params['items'] %}
-      {% if item %}
-        {% set id = item.id if item.id else idPrefix + "-" ~ loop.index %}
-        <div class="govuk-tabs__panel {%- if loop.index > 1 %} govuk-tabs__panel--hidden{% endif %}" id="{{ id }}" {%- for attribute, value in (item.panel.attributes.items() if item.panel.attributes else {}.items()) %} {{ attribute }}="{{ value }}"{% endfor %}>
-          {% if item.panel.html %}
-            {{ item.panel.html | safe }}
-          {% elif item.panel.text %}
-            <p class="govuk-body">{{ item.panel.text }}</p>
-          {% endif %}
-        </div>
-      {% endif %}
-    {% endfor %}
-  {% endif %}
+  {% for item in params['items'] %}
+    {% if item %}
+      {{- _tabPanel(params, item, loop.index) | trim | indent(2, true) }}
+    {% endif %}
+  {% endfor %}
+{% endif %}
 </div>
 {% endmacro %}
```

### Comparing `govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/textarea/macro.html` & `govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/file-upload/macro.html`

 * *Files 26% similar despite different names*

```diff
@@ -1,48 +1,55 @@
-{% macro govukTextarea(params) %}
+{% macro govukFileUpload(params) %}
+{% from "govuk_frontend_jinja/macros/attributes.html" import govukAttributes %}
 {% from "govuk_frontend_jinja/components/error-message/macro.html" import govukErrorMessage %}
 {% from "govuk_frontend_jinja/components/hint/macro.html" import govukHint %}
 {% from "govuk_frontend_jinja/components/label/macro.html" import govukLabel %}
 
 {#- a record of other elements that we need to associate with the input using
   aria-describedby – for example hints or error messages -#}
 {% set describedBy = params.describedBy if params.describedBy else "" %}
-<div class="govuk-form-group {%- if params.errorMessage %} govuk-form-group--error{% endif %} {%- if params.formGroup and params.formGroup.classes %} {{ params.formGroup.classes }}{% endif %}" {%- for attribute, value in (params.formGroup.attributes.items() if params.formGroup and params.formGroup.attributes else {}.items()) %} {{ attribute }}="{{ value }}"{% endfor %}>
+<div class="govuk-form-group {%- if params.errorMessage %} govuk-form-group--error{% endif %} {%- if params.formGroup and params.formGroup.classes %} {{ params.formGroup.classes }}{% endif %}"
+  {{- govukAttributes(params.formGroup.attributes if params.formGroup) }}>
   {{ govukLabel({
     'html': params.label.html,
     'text': params.label.text,
     'classes': params.label.classes,
     'isPageHeading': params.label.isPageHeading,
     'attributes': params.label.attributes,
     'for': params.id
   }) | trim | indent(2) }}
 {% if params.hint %}
-  {% set hintId = params.id + '-hint' %}
-  {% set describedBy = describedBy + ' ' + hintId if describedBy else hintId %}
+  {% set hintId = params.id ~ '-hint' %}
+  {% set describedBy = describedBy ~ ' ' ~ hintId if describedBy else hintId %}
   {{ govukHint({
     'id': hintId,
     'classes': params.hint.classes,
     'attributes': params.hint.attributes,
     'html': params.hint.html,
     'text': params.hint.text
   }) | trim | indent(2) }}
 {% endif %}
 {% if params.errorMessage %}
-  {% set errorId = params.id + '-error' %}
-  {% set describedBy = describedBy + ' ' + errorId if describedBy else errorId %}
+  {% set errorId = params.id ~ '-error' %}
+  {% set describedBy = describedBy ~ ' ' ~ errorId if describedBy else errorId %}
   {{ govukErrorMessage({
     'id': errorId,
     'classes': params.errorMessage.classes,
     'attributes': params.errorMessage.attributes,
     'html': params.errorMessage.html,
     'text': params.errorMessage.text,
     'visuallyHiddenText': params.errorMessage.visuallyHiddenText
   }) | trim | indent(2) }}
 {% endif %}
-  <textarea class="govuk-textarea {%- if params.errorMessage %} govuk-textarea--error{% endif %} {%- if params.classes %} {{ params.classes }}{% endif %}" id="{{ params.id }}" name="{{ params.name }}" rows="{{ params.rows | default(5, true) }}"
-  {%- if (params.spellcheck == false) or (params.spellcheck == true) %} spellcheck="{{ params.spellcheck | lower }}"{% endif %}
+{% if params.formGroup and params.formGroup.beforeInput %}
+  {{ params.formGroup.beforeInput.html | safe | trim | indent(2) if params.formGroup and params.formGroup.beforeInput.html else params.formGroup.beforeInput.text }}
+{% endif %}
+  <input class="govuk-file-upload {%- if params.classes %} {{ params.classes }}{% endif %} {%- if params.errorMessage %} govuk-file-upload--error{% endif %}" id="{{ params.id }}" name="{{ params.name }}" type="file"
+  {%- if params.value %} value="{{ params.value }}"{% endif %}
   {%- if params.disabled %} disabled{% endif %}
   {%- if describedBy %} aria-describedby="{{ describedBy }}"{% endif %}
-  {%- if params.autocomplete %} autocomplete="{{ params.autocomplete }}"{% endif %}
-  {%- for attribute, value in (params.attributes.items() if params.attributes else {}.items()) %} {{ attribute }}="{{ value }}"{% endfor %}>{{ params.value }}</textarea>
+  {{- govukAttributes(params.attributes) }}>
+{% if params.formGroup and params.formGroup.afterInput %}
+  {{ params.formGroup.afterInput.html | safe | trim | indent(2) if params.formGroup and params.formGroup.afterInput.html else params.formGroup.afterInput.text }}
+{% endif %}
 </div>
 {% endmacro %}
```

### Comparing `govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/components/warning-text/macro.html` & `govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/components/details/macro.html`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,16 @@
-{% macro govukWarningText(params) %}
-<div class="govuk-warning-text {%- if params.classes %} {{ params.classes }}{% endif %}"
-  {%- for attribute, value in (params.attributes.items() if params.attributes else {}.items()) %} {{ attribute }}="{{ value }}"{% endfor -%}
-  >
-  <span class="govuk-warning-text__icon" aria-hidden="true">!</span>
-  <strong class="govuk-warning-text__text">
-    <span class="govuk-visually-hidden">{{ params.iconFallbackText | default("Warning", true) }}</span>
-    {{ params.html | safe if params.html else params.text }}
-  </strong>
-</div>
+{% macro govukDetails(params) %}
+{% from "govuk_frontend_jinja/macros/attributes.html" import govukAttributes -%}
+
+<details {%- if params.id %} id="{{ params.id }}"{% endif %} class="govuk-details {%- if params.classes %} {{ params.classes }}{% endif %}"
+  {{- govukAttributes(params.attributes) -}}
+  {{- " open" if params.open }}>
+  <summary class="govuk-details__summary">
+    <span class="govuk-details__summary-text">
+      {{ params.summaryHtml | safe | trim | indent(6) if params.summaryHtml else params.summaryText }}
+    </span>
+  </summary>
+  <div class="govuk-details__text">
+    {{ caller() if caller else (params.html | safe if params.html else params.text) }}
+  </div>
+</details>
 {% endmacro %}
```

### Comparing `govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/macros/i18n.html` & `govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/macros/i18n.html`

 * *Files identical despite different names*

### Comparing `govuk-frontend-jinja-3.0.0/govuk_frontend_jinja/templates/template.html` & `govuk_frontend_jinja-3.1.0/govuk_frontend_jinja/templates/template.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+{% from "govuk_frontend_jinja/macros/attributes.html" import govukAttributes %}
 {% from "govuk_frontend_jinja/components/skip-link/macro.html" import govukSkipLink -%}
 {% from "govuk_frontend_jinja/components/header/macro.html" import govukHeader -%}
 {% from "govuk_frontend_jinja/components/footer/macro.html" import govukFooter -%}
 <!DOCTYPE html>
 <html lang="{{ htmlLang | default('en', true) }}" class="govuk-template {%- if htmlClasses %} {{ htmlClasses }}{% endif %}">
   <head>
     <meta charset="utf-8">
@@ -17,18 +18,18 @@
       <link rel="manifest" href="{{ assetPath | default('/assets', true) }}/manifest.json">
     {% endblock %}
 
     {% block head %}{% endblock %}
 
     {#- OpenGraph images needs to be absolute, so we need either a URL for the image or for assetUrl to be set #}
     {% if opengraphImageUrl or assetUrl %}
-    <meta property="og:image" content="{{ opengraphImageUrl | default(assetUrl + '/images/govuk-opengraph-image.png', true) }}">
+    <meta property="og:image" content="{{ opengraphImageUrl | default(assetUrl ~ '/images/govuk-opengraph-image.png', true) }}">
     {% endif %}
   </head>
-  <body class="govuk-template__body {%- if bodyClasses %} {{ bodyClasses }}{% endif %}" {%- for attribute, value in bodyAttributes %} {{ attribute }}="{{ value }}"{% endfor %}>
+  <body class="govuk-template__body {%- if bodyClasses %} {{ bodyClasses }}{% endif %}" {{- govukAttributes(bodyAttributes) }}>
     <script {%- if cspNonce %} nonce="{{ cspNonce }}"{% endif %}>document.body.className += ' js-enabled' + ('noModule' in HTMLScriptElement.prototype ? ' govuk-frontend-supported' : '');</script>
     {% block bodyStart %}{% endblock %}
 
     {% block skipLink %}
       {{ govukSkipLink({
         'href': '#main-content',
         'text': 'Skip to main content'
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
+{% from "govuk_frontend_jinja/macros/attributes.html" import govukAttributes %}
 {% from "govuk_frontend_jinja/components/skip-link/macro.html" import
 govukSkipLink -%} {% from "govuk_frontend_jinja/components/header/macro.html"
 import govukHeader -%} {% from "govuk_frontend_jinja/components/footer/
 macro.html" import govukFooter -%}
 %- if pageTitleLang %} lang="{{ pageTitleLang }}"{% endif %}>{% block pageTitle
 %}GOV.UK - The best place to find government services and information{%
 endblock %}
 {#- Hardcoded value of $govuk-black #} {% block headIcons %}
 {#- Hardcoded value of $govuk-black #}
 {% endblock %} {% block head %}{% endblock %} {#- OpenGraph images needs to be
 absolute, so we need either a URL for the image or for assetUrl to be set #} {%
 if opengraphImageUrl or assetUrl %}
 {% endif %}
-%- for attribute, value in bodyAttributes %} {{ attribute }}="{{ value }}"{%
-endfor %}>
+{- govukAttributes(bodyAttributes) }}>
 %- if cspNonce %} nonce="{{ cspNonce }}"{% endif %}>document.body.className +=
 ' js-enabled' + ('noModule' in HTMLScriptElement.prototype ? ' govuk-frontend-
 supported' : '');
 {% block bodyStart %}{% endblock %} {% block skipLink %} {{ govukSkipLink(
 { 'href': '#main-content', 'text': 'Skip to main content' }) }} {% endblock %}
 {% block header %} {{ govukHeader({}) }} {% endblock %} {% block main %}
 {% block beforeContent %}{% endblock %}
```

### Comparing `govuk-frontend-jinja-3.0.0/govuk_frontend_jinja.egg-info/PKG-INFO` & `govuk_frontend_jinja-3.1.0/govuk_frontend_jinja.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: govuk-frontend-jinja
-Version: 3.0.0
+Version: 3.1.0
 Summary: GOV.UK Frontend Jinja Macros
 Home-page: https://github.com/LandRegistry/govuk-frontend-jinja
 Author: Matt Shaw
 Author-email: matthew.shaw@landregistry.gov.uk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -22,39 +22,41 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: jinja2!=3.0.0,!=3.0.1
 
 # GOV.UK Frontend Jinja Macros
 
 [![PyPI version](https://badge.fury.io/py/govuk-frontend-jinja.svg)](https://pypi.org/project/govuk-frontend-jinja/)
-![govuk-frontend 5.1.0](https://img.shields.io/badge/govuk--frontend%20version-5.1.0-005EA5?logo=gov.uk&style=flat)
+![govuk-frontend 5.4.0](https://img.shields.io/badge/govuk--frontend%20version-5.4.0-005EA5?logo=gov.uk&style=flat)
 [![Python package](https://github.com/LandRegistry/govuk-frontend-jinja/actions/workflows/python-package.yml/badge.svg)](https://github.com/LandRegistry/govuk-frontend-jinja/actions/workflows/python-package.yml)
 
 **GOV.UK Frontend Jinja is a [community tool](https://design-system.service.gov.uk/community/resources-and-tools/) of the [GOV.UK Design System](https://design-system.service.gov.uk/). The Design System team is not responsible for it and cannot support you with using it. Contact the [maintainers](#contributors) directly if you need [help](#support) or you want to request a feature.**
 
 This repository provides a complete set of [Jinja](https://jinja.palletsprojects.com/) macros that are kept up-to-date and 100% compliant with the original [GOV.UK Frontend](https://github.com/alphagov/govuk-frontend) Nunjucks macros. Porting is intentionally manual rather than automated to make updates simpler than maintaining an automated conversion routine. A [comprehensive test suite](https://github.com/matthew-shaw/govuk-frontend-diff) ensures compliance against the latest, and every subsequent, GOV.UK Frontend release.
 
 If you are looking to build a fully featured Flask app that integrates with [GOV.UK Frontend Jinja](https://github.com/LandRegistry/govuk-frontend-jinja) and [GOV.UK Frontend WTForms](https://github.com/LandRegistry/govuk-frontend-wtf) please use the [GOV.UK Frontend Flask](https://github.com/LandRegistry/govuk-frontend-flask) template repository to [generate your app](https://github.com/LandRegistry/govuk-frontend-flask/generate).
 
 ## Compatibility
 
 The following table shows the version of GOV.UK Frontend Jinja that you should use for your targeted version of GOV.UK Frontend:
 
 | GOV.UK Frontend Jinja Version | Target GOV.UK Frontend Version |
 | ----------------------------- | ------------------------------ |
+| [3.1.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/3.1.0) | [5.4.0](https://github.com/alphagov/govuk-frontend/releases/tag/v5.4.0) |
 | [3.0.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/3.0.0) | [5.1.0](https://github.com/alphagov/govuk-frontend/releases/tag/v5.1.0) |
 | [2.8.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.8.0) | [4.8.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.8.0) |
 | [2.7.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.7.0) | [4.7.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.7.0) |
 | [2.6.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.6.0) | [4.6.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.6.0) |
 | [2.5.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.5.0) | [4.5.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.5.0) |
 | [2.4.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.4.0) | [4.4.1](https://github.com/alphagov/govuk-frontend/releases/tag/v4.4.1) |
 | [2.3.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.3.0) | [4.2.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.2.0) |
 | [2.2.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.2.0) | [4.1.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.1.0) |
 | [2.1.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.1.0) | [4.0.1](https://github.com/alphagov/govuk-frontend/releases/tag/v4.0.1) |
 | [2.0.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/2.0.0) | [4.0.0](https://github.com/alphagov/govuk-frontend/releases/tag/v4.0.0) |
+| [1.6.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/1.6.0) | [3.15.0](https://github.com/alphagov/govuk-frontend/releases/tag/v3.15.0) |
 | [1.5.1](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/1.5.1) | [3.14.0](https://github.com/alphagov/govuk-frontend/releases/tag/v3.14.0) |
 | [1.4.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/1.4.0) | [3.13.0](https://github.com/alphagov/govuk-frontend/releases/tag/v3.13.0) |
 | [1.3.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/1.3.0) | [3.12.0](https://github.com/alphagov/govuk-frontend/releases/tag/v3.12.0) |
 | [1.2.1](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/1.2.1) | [3.11.0](https://github.com/alphagov/govuk-frontend/releases/tag/v3.11.0) |
 | [1.1.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/1.1.0) | [3.10.2](https://github.com/alphagov/govuk-frontend/releases/tag/v3.10.2) |
 | [1.0.0](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/1.0.0) | [3.8.1](https://github.com/alphagov/govuk-frontend/releases/tag/v3.8.1) |
 | [0.2.1](https://github.com/LandRegistry/govuk-frontend-jinja/releases/tag/0.2.1) | [3.7.0](https://github.com/alphagov/govuk-frontend/releases/tag/v3.7.0) |
```

### Comparing `govuk-frontend-jinja-3.0.0/govuk_frontend_jinja.egg-info/SOURCES.txt` & `govuk_frontend_jinja-3.1.0/govuk_frontend_jinja.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -28,19 +28,21 @@
 govuk_frontend_jinja/templates/components/hint/macro.html
 govuk_frontend_jinja/templates/components/input/macro.html
 govuk_frontend_jinja/templates/components/inset-text/macro.html
 govuk_frontend_jinja/templates/components/label/macro.html
 govuk_frontend_jinja/templates/components/notification-banner/macro.html
 govuk_frontend_jinja/templates/components/pagination/macro.html
 govuk_frontend_jinja/templates/components/panel/macro.html
+govuk_frontend_jinja/templates/components/password-input/macro.html
 govuk_frontend_jinja/templates/components/phase-banner/macro.html
 govuk_frontend_jinja/templates/components/radios/macro.html
 govuk_frontend_jinja/templates/components/select/macro.html
 govuk_frontend_jinja/templates/components/skip-link/macro.html
 govuk_frontend_jinja/templates/components/summary-list/macro.html
 govuk_frontend_jinja/templates/components/table/macro.html
 govuk_frontend_jinja/templates/components/tabs/macro.html
 govuk_frontend_jinja/templates/components/tag/macro.html
 govuk_frontend_jinja/templates/components/task-list/macro.html
 govuk_frontend_jinja/templates/components/textarea/macro.html
 govuk_frontend_jinja/templates/components/warning-text/macro.html
+govuk_frontend_jinja/templates/macros/attributes.html
 govuk_frontend_jinja/templates/macros/i18n.html
```

### Comparing `govuk-frontend-jinja-3.0.0/setup.py` & `govuk_frontend_jinja-3.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 components = []
 directories = glob.glob("govuk_frontend_jinja/**/**/*.html", recursive=True)
 for directory in directories:
     components.append(os.path.relpath(os.path.dirname(directory), "govuk_frontend_jinja") + "/*.html")
 
 setuptools.setup(
     name="govuk-frontend-jinja",
-    version="3.0.0",
+    version="3.1.0",
     author="Matt Shaw",
     author_email="matthew.shaw@landregistry.gov.uk",
     description="GOV.UK Frontend Jinja Macros",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/LandRegistry/govuk-frontend-jinja",
     packages=setuptools.find_packages(exclude=["tests"]),
```

