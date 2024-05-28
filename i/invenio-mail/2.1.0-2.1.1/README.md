# Comparing `tmp/invenio-mail-2.1.0.tar.gz` & `tmp/invenio-mail-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-mail-2.1.0.tar", last modified: Thu Nov 30 13:32:13 2023, max compression
+gzip compressed data, was "dist/invenio-mail-2.1.1.tar", last modified: Tue May 28 12:25:52 2024, max compression
```

## Comparing `invenio-mail-2.1.0.tar` & `invenio-mail-2.1.1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 13:32:13.000000 invenio-mail-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2023-11-30 13:32:03.000000 invenio-mail-2.1.0/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (127)      666 2023-11-30 13:32:03.000000 invenio-mail-2.1.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-11-30 13:32:03.000000 invenio-mail-2.1.0/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 13:32:13.000000 invenio-mail-2.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 13:32:13.000000 invenio-mail-2.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      955 2023-11-30 13:32:03.000000 invenio-mail-2.1.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2023-11-30 13:32:03.000000 invenio-mail-2.1.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      416 2023-11-30 13:32:03.000000 invenio-mail-2.1.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)      900 2023-11-30 13:32:03.000000 invenio-mail-2.1.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2023-11-30 13:32:03.000000 invenio-mail-2.1.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)      346 2023-11-30 13:32:03.000000 invenio-mail-2.1.0/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2023-11-30 13:32:03.000000 invenio-mail-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      863 2023-11-30 13:32:03.000000 invenio-mail-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2023-11-30 13:32:13.000000 invenio-mail-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      991 2023-11-30 13:32:03.000000 invenio-mail-2.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 13:32:13.000000 invenio-mail-2.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     7433 2023-11-30 13:32:03.000000 invenio-mail-2.1.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      452 2023-11-30 13:32:03.000000 invenio-mail-2.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      247 2023-11-30 13:32:03.000000 invenio-mail-2.1.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)      247 2023-11-30 13:32:03.000000 invenio-mail-2.1.0/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10024 2023-11-30 13:32:03.000000 invenio-mail-2.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2023-11-30 13:32:03.000000 invenio-mail-2.1.0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)      252 2023-11-30 13:32:03.000000 invenio-mail-2.1.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      825 2023-11-30 13:32:03.000000 invenio-mail-2.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      247 2023-11-30 13:32:03.000000 invenio-mail-2.1.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      253 2023-11-30 13:32:03.000000 invenio-mail-2.1.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6993 2023-11-30 13:32:03.000000 invenio-mail-2.1.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-11-30 13:32:03.000000 invenio-mail-2.1.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      261 2023-11-30 13:32:03.000000 invenio-mail-2.1.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 13:32:13.000000 invenio-mail-2.1.0/invenio_mail/
--rw-r--r--   0 runner    (1001) docker     (127)     3223 2023-11-30 13:32:03.000000 invenio-mail-2.1.0/invenio_mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2023-11-30 13:32:03.000000 invenio-mail-2.1.0/invenio_mail/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2023-11-30 13:32:03.000000 invenio-mail-2.1.0/invenio_mail/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2023-11-30 13:32:03.000000 invenio-mail-2.1.0/invenio_mail/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2023-11-30 13:32:03.000000 invenio-mail-2.1.0/invenio_mail/ext.py
--rw-r--r--   0 runner    (1001) docker     (127)     2775 2023-11-30 13:32:03.000000 invenio-mail-2.1.0/invenio_mail/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 13:32:13.000000 invenio-mail-2.1.0/invenio_mail.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2023-11-30 13:32:12.000000 invenio-mail-2.1.0/invenio_mail.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-11-30 13:32:13.000000 invenio-mail-2.1.0/invenio_mail.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-30 13:32:12.000000 invenio-mail-2.1.0/invenio_mail.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      184 2023-11-30 13:32:12.000000 invenio-mail-2.1.0/invenio_mail.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-30 13:32:12.000000 invenio-mail-2.1.0/invenio_mail.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      167 2023-11-30 13:32:12.000000 invenio-mail-2.1.0/invenio_mail.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-11-30 13:32:12.000000 invenio-mail-2.1.0/invenio_mail.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2023-11-30 13:32:03.000000 invenio-mail-2.1.0/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)      477 2023-11-30 13:32:03.000000 invenio-mail-2.1.0/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2023-11-30 13:32:13.000000 invenio-mail-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      401 2023-11-30 13:32:03.000000 invenio-mail-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 13:32:13.000000 invenio-mail-2.1.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 13:32:13.000000 invenio-mail-2.1.0/tests/attachments/
--rw-r--r--   0 runner    (1001) docker     (127)    97458 2023-11-30 13:32:03.000000 invenio-mail-2.1.0/tests/attachments/invenio.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2023-11-30 13:32:03.000000 invenio-mail-2.1.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 13:32:13.000000 invenio-mail-2.1.0/tests/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 13:32:13.000000 invenio-mail-2.1.0/tests/templates/invenio_mail/
--rw-r--r--   0 runner    (1001) docker     (127)      679 2023-11-30 13:32:03.000000 invenio-mail-2.1.0/tests/templates/invenio_mail/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      528 2023-11-30 13:32:03.000000 invenio-mail-2.1.0/tests/templates/invenio_mail/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2023-11-30 13:32:03.000000 invenio-mail-2.1.0/tests/test_invenio_mail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2023-11-30 13:32:03.000000 invenio-mail-2.1.0/tests/test_invenio_mail_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2023-11-30 13:32:03.000000 invenio-mail-2.1.0/tests/test_invenio_mail_tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:25:52.000000 invenio-mail-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-28 12:25:45.000000 invenio-mail-2.1.1/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-28 12:25:45.000000 invenio-mail-2.1.1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-28 12:25:45.000000 invenio-mail-2.1.1/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:25:52.000000 invenio-mail-2.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:25:52.000000 invenio-mail-2.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-28 12:25:45.000000 invenio-mail-2.1.1/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-28 12:25:45.000000 invenio-mail-2.1.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-28 12:25:45.000000 invenio-mail-2.1.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-28 12:25:45.000000 invenio-mail-2.1.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-05-28 12:25:45.000000 invenio-mail-2.1.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-28 12:25:45.000000 invenio-mail-2.1.1/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-28 12:25:45.000000 invenio-mail-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-28 12:25:45.000000 invenio-mail-2.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-05-28 12:25:52.000000 invenio-mail-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-28 12:25:45.000000 invenio-mail-2.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:25:52.000000 invenio-mail-2.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7433 2024-05-28 12:25:45.000000 invenio-mail-2.1.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-28 12:25:45.000000 invenio-mail-2.1.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-28 12:25:45.000000 invenio-mail-2.1.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-28 12:25:45.000000 invenio-mail-2.1.1/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10032 2024-05-28 12:25:45.000000 invenio-mail-2.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-28 12:25:45.000000 invenio-mail-2.1.1/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-28 12:25:45.000000 invenio-mail-2.1.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-28 12:25:45.000000 invenio-mail-2.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-28 12:25:45.000000 invenio-mail-2.1.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-28 12:25:45.000000 invenio-mail-2.1.1/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-05-28 12:25:45.000000 invenio-mail-2.1.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-28 12:25:45.000000 invenio-mail-2.1.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-28 12:25:45.000000 invenio-mail-2.1.1/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:25:52.000000 invenio-mail-2.1.1/invenio_mail/
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-05-28 12:25:45.000000 invenio-mail-2.1.1/invenio_mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-28 12:25:45.000000 invenio-mail-2.1.1/invenio_mail/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-28 12:25:45.000000 invenio-mail-2.1.1/invenio_mail/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-28 12:25:45.000000 invenio-mail-2.1.1/invenio_mail/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-28 12:25:45.000000 invenio-mail-2.1.1/invenio_mail/ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-05-28 12:25:45.000000 invenio-mail-2.1.1/invenio_mail/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:25:52.000000 invenio-mail-2.1.1/invenio_mail.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-05-28 12:25:52.000000 invenio-mail-2.1.1/invenio_mail.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-28 12:25:52.000000 invenio-mail-2.1.1/invenio_mail.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 12:25:52.000000 invenio-mail-2.1.1/invenio_mail.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-28 12:25:52.000000 invenio-mail-2.1.1/invenio_mail.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 12:25:52.000000 invenio-mail-2.1.1/invenio_mail.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-28 12:25:52.000000 invenio-mail-2.1.1/invenio_mail.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-28 12:25:52.000000 invenio-mail-2.1.1/invenio_mail.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-28 12:25:45.000000 invenio-mail-2.1.1/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      477 2024-05-28 12:25:45.000000 invenio-mail-2.1.1/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-28 12:25:52.000000 invenio-mail-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-28 12:25:45.000000 invenio-mail-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:25:52.000000 invenio-mail-2.1.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:25:52.000000 invenio-mail-2.1.1/tests/attachments/
+-rw-r--r--   0 runner    (1001) docker     (127)    97458 2024-05-28 12:25:45.000000 invenio-mail-2.1.1/tests/attachments/invenio.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-28 12:25:45.000000 invenio-mail-2.1.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:25:52.000000 invenio-mail-2.1.1/tests/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:25:52.000000 invenio-mail-2.1.1/tests/templates/invenio_mail/
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-28 12:25:45.000000 invenio-mail-2.1.1/tests/templates/invenio_mail/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-28 12:25:45.000000 invenio-mail-2.1.1/tests/templates/invenio_mail/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-28 12:25:45.000000 invenio-mail-2.1.1/tests/test_invenio_mail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-28 12:25:45.000000 invenio-mail-2.1.1/tests/test_invenio_mail_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-05-28 12:25:45.000000 invenio-mail-2.1.1/tests/test_invenio_mail_tasks.py
```

### Comparing `invenio-mail-2.1.0/.editorconfig` & `invenio-mail-2.1.1/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-mail-2.1.0/.github/workflows/pypi-publish.yml` & `invenio-mail-2.1.1/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-mail-2.1.0/.github/workflows/tests.yml` & `invenio-mail-2.1.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-mail-2.1.0/CHANGES.rst` & `invenio-mail-2.1.1/CHANGES.rst`

 * *Files 18% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 
     Invenio is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version 2.1.1 (released 2024-05-28)
+
+- installation: upper pin flask-mail due to breaking changes in v0.10.0
+
 Version 2.1.0 (released 2023-11-29)
 
 - add a func to send e-mails with inline attachments
 
 Version 2.0.0 (released 2023-10-06)
 
 - config: introduce MAIL_DEFAULT_REPLY_TO
```

### Comparing `invenio-mail-2.1.0/CONTRIBUTING.rst` & `invenio-mail-2.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-mail-2.1.0/LICENSE` & `invenio-mail-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-mail-2.1.0/MANIFEST.in` & `invenio-mail-2.1.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-mail-2.1.0/PKG-INFO` & `invenio-mail-2.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-mail
-Version: 2.1.0
+Version: 2.1.1
 Summary: Invenio-Mail is an integration layer between Invenio and Flask-Mail.
 Home-page: https://github.com/inveniosoftware/invenio-mail
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -40,14 +40,18 @@
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 2.1.1 (released 2024-05-28)
+        
+        - installation: upper pin flask-mail due to breaking changes in v0.10.0
+        
         Version 2.1.0 (released 2023-11-29)
         
         - add a func to send e-mails with inline attachments
         
         Version 2.0.0 (released 2023-10-06)
         
         - config: introduce MAIL_DEFAULT_REPLY_TO
```

### Comparing `invenio-mail-2.1.0/README.rst` & `invenio-mail-2.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-mail-2.1.0/docs/Makefile` & `invenio-mail-2.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-mail-2.1.0/docs/conf.py` & `invenio-mail-2.1.1/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -304,12 +304,12 @@
 # texinfo_no_detailmenu = False
 
 
 # Example configuration for intersphinx: refer to the Python standard library.
 intersphinx_mapping = {
     "python": ("https://docs.python.org/", None),
     "flask": ("https://flask.palletsprojects.com", None),
-    "flask_mail": ("https://pythonhosted.org/Flask-Mail/", None),
+    "flask_mail": ("https://flask-mail.readthedocs.io/en/latest/", None),
 }
 
 # Autodoc configuraton.
 autoclass_content = "both"
```

### Comparing `invenio-mail-2.1.0/docs/index.rst` & `invenio-mail-2.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-mail-2.1.0/docs/make.bat` & `invenio-mail-2.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-mail-2.1.0/invenio_mail/__init__.py` & `invenio-mail-2.1.1/invenio_mail/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,10 +96,10 @@
        install_requires = ['Flask-Mail>=0.9.1',]
        #...
     )
 """
 
 from .ext import InvenioMail
 
-__version__ = "2.1.0"
+__version__ = "2.1.1"
 
 __all__ = ("__version__", "InvenioMail")
```

### Comparing `invenio-mail-2.1.0/invenio_mail/api.py` & `invenio-mail-2.1.1/invenio_mail/api.py`

 * *Files identical despite different names*

### Comparing `invenio-mail-2.1.0/invenio_mail/config.py` & `invenio-mail-2.1.1/invenio_mail/config.py`

 * *Files identical despite different names*

### Comparing `invenio-mail-2.1.0/invenio_mail/ext.py` & `invenio-mail-2.1.1/invenio_mail/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-mail-2.1.0/invenio_mail/tasks.py` & `invenio-mail-2.1.1/invenio_mail/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-mail-2.1.0/invenio_mail.egg-info/PKG-INFO` & `invenio-mail-2.1.1/invenio_mail.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-mail
-Version: 2.1.0
+Version: 2.1.1
 Summary: Invenio-Mail is an integration layer between Invenio and Flask-Mail.
 Home-page: https://github.com/inveniosoftware/invenio-mail
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -40,14 +40,18 @@
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 2.1.1 (released 2024-05-28)
+        
+        - installation: upper pin flask-mail due to breaking changes in v0.10.0
+        
         Version 2.1.0 (released 2023-11-29)
         
         - add a func to send e-mails with inline attachments
         
         Version 2.0.0 (released 2023-10-06)
         
         - config: introduce MAIL_DEFAULT_REPLY_TO
```

### Comparing `invenio-mail-2.1.0/invenio_mail.egg-info/SOURCES.txt` & `invenio-mail-2.1.1/invenio_mail.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-mail-2.1.0/setup.cfg` & `invenio-mail-2.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 [options]
 include_package_data = True
 packages = find:
 python_requires = >=3.7
 zip_safe = False
 install_requires = 
 	Flask>=0.11.1
-	Flask-Mail>=0.9.1
+	Flask-Mail>=0.9.1,<0.10.0
 
 [options.extras_require]
 tests = 
 	pytest-black>=0.3.0,<0.3.10
 	pytest-invenio>=1.4.0
 	Flask-CeleryExt>=0.2.2
 	Flask-CeleryExt>=0.2.2
```

### Comparing `invenio-mail-2.1.0/tests/attachments/invenio.svg` & `invenio-mail-2.1.1/tests/attachments/invenio.svg`

 * *Files identical despite different names*

### Comparing `invenio-mail-2.1.0/tests/conftest.py` & `invenio-mail-2.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-mail-2.1.0/tests/templates/invenio_mail/base.html` & `invenio-mail-2.1.1/tests/templates/invenio_mail/base.html`

 * *Files identical despite different names*

### Comparing `invenio-mail-2.1.0/tests/templates/invenio_mail/base.txt` & `invenio-mail-2.1.1/tests/templates/invenio_mail/base.txt`

 * *Files identical despite different names*

### Comparing `invenio-mail-2.1.0/tests/test_invenio_mail.py` & `invenio-mail-2.1.1/tests/test_invenio_mail.py`

 * *Files identical despite different names*

### Comparing `invenio-mail-2.1.0/tests/test_invenio_mail_api.py` & `invenio-mail-2.1.1/tests/test_invenio_mail_api.py`

 * *Files identical despite different names*

### Comparing `invenio-mail-2.1.0/tests/test_invenio_mail_tasks.py` & `invenio-mail-2.1.1/tests/test_invenio_mail_tasks.py`

 * *Files identical despite different names*

