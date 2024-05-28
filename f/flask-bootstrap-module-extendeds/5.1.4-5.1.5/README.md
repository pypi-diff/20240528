# Comparing `tmp/flask_bootstrap_module_extendeds-5.1.4.tar.gz` & `tmp/flask_bootstrap_module_extendeds-5.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_bootstrap_module_extendeds-5.1.4.tar", last modified: Tue May 28 02:57:37 2024, max compression
+gzip compressed data, was "flask_bootstrap_module_extendeds-5.1.5.tar", last modified: Tue May 28 03:07:36 2024, max compression
```

## Comparing `flask_bootstrap_module_extendeds-5.1.4.tar` & `flask_bootstrap_module_extendeds-5.1.5.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 02:57:37.667978 flask_bootstrap_module_extendeds-5.1.4/
--rw-rw-rw-   0        0        0      111 2024-05-28 00:25:39.000000 flask_bootstrap_module_extendeds-5.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0      512 2024-05-28 02:57:37.667978 flask_bootstrap_module_extendeds-5.1.4/PKG-INFO
--rw-rw-rw-   0        0        0       72 2024-05-27 22:54:19.000000 flask_bootstrap_module_extendeds-5.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-28 02:57:37.553746 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/
--rw-rw-rw-   0        0        0        0 2024-05-28 00:15:24.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/__init__.py
--rw-rw-rw-   0        0        0     2366 2023-12-09 17:30:07.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/_backwards.py
--rw-rw-rw-   0        0        0     2812 2023-12-09 17:30:07.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/_compat.py
--rw-rw-rw-   0        0        0     3806 2023-12-09 17:30:07.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/actions.py
--rw-rw-rw-   0        0        0     2021 2023-12-09 17:30:07.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/babel.py
--rw-rw-rw-   0        0        0    25372 2023-12-09 17:30:07.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/base.py
--rw-rw-rw-   0        0        0    10689 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/cli.py
--rw-rw-rw-   0        0        0      222 2023-12-09 17:30:07.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/consts.py
--rw-rw-rw-   0        0        0     4628 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/forms.py
--rw-rw-rw-   0        0        0     4269 2023-12-09 17:30:07.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/helpers.py
--rw-rw-rw-   0        0        0     3582 2023-12-09 17:30:07.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/menu.py
--rw-rw-rw-   0        0        0     3437 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/nav.py
--rw-rw-rw-   0        0        0     5911 2024-05-27 22:54:06.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/refusion.py
-drwxrwxrwx   0        0        0        0 2024-05-28 02:57:37.568706 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/
-drwxrwxrwx   0        0        0        0 2024-05-28 02:57:37.585659 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/css/
--rw-rw-rw-   0        0        0    26132 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/css/bootstrap-theme.css
--rw-rw-rw-   0        0        0    47706 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/css/bootstrap-theme.css.map
--rw-rw-rw-   0        0        0    23409 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/css/bootstrap-theme.min.css
--rw-rw-rw-   0        0        0   146010 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/css/bootstrap.css
--rw-rw-rw-   0        0        0   389287 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/css/bootstrap.css.map
--rw-rw-rw-   0        0        0   121200 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/css/bootstrap.min.css
-drwxrwxrwx   0        0        0        0 2024-05-28 02:57:37.598625 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/fonts/
--rw-rw-rw-   0        0        0    20127 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/fonts/glyphicons-halflings-regular.eot
--rw-rw-rw-   0        0        0   108738 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/fonts/glyphicons-halflings-regular.svg
--rw-rw-rw-   0        0        0    45404 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/fonts/glyphicons-halflings-regular.ttf
--rw-rw-rw-   0        0        0    23424 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/fonts/glyphicons-halflings-regular.woff
--rw-rw-rw-   0        0        0    18028 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/fonts/glyphicons-halflings-regular.woff2
--rw-rw-rw-   0        0        0   293430 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/jquery.js
--rw-rw-rw-   0        0        0    97163 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/jquery.min.js
--rw-rw-rw-   0        0        0   143947 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/jquery.min.map
-drwxrwxrwx   0        0        0        0 2024-05-28 02:57:37.604608 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/js/
--rw-rw-rw-   0        0        0    69707 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/js/bootstrap.js
--rw-rw-rw-   0        0        0    37045 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/js/bootstrap.min.js
--rw-rw-rw-   0        0        0      484 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/js/npm.js
-drwxrwxrwx   0        0        0        0 2024-05-28 02:57:37.517866 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/
-drwxrwxrwx   0        0        0        0 2024-05-28 02:57:37.611590 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/aioflask/
--rw-rw-rw-   0        0        0       44 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/aioflask/README
-drwxrwxrwx   0        0        0        0 2024-05-28 02:57:37.621564 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/aioflask/__pycache__/
--rw-rw-rw-   0        0        0     5072 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/aioflask/__pycache__/env.cpython-312.pyc
--rw-rw-rw-   0        0        0      857 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/aioflask/alembic.ini.mako
--rw-rw-rw-   0        0        0     3478 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/aioflask/env.py
--rw-rw-rw-   0        0        0      494 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/aioflask/script.py.mako
-drwxrwxrwx   0        0        0        0 2024-05-28 02:57:37.618571 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/aioflask-multidb/
--rw-rw-rw-   0        0        0       43 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/aioflask-multidb/README
-drwxrwxrwx   0        0        0        0 2024-05-28 02:57:37.620566 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/aioflask-multidb/__pycache__/
--rw-rw-rw-   0        0        0     8813 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/aioflask-multidb/__pycache__/env.cpython-312.pyc
--rw-rw-rw-   0        0        0      857 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/aioflask-multidb/alembic.ini.mako
--rw-rw-rw-   0        0        0     6573 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/aioflask-multidb/env.py
--rw-rw-rw-   0        0        0     1246 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/aioflask-multidb/script.py.mako
-drwxrwxrwx   0        0        0        0 2024-05-28 02:57:37.632534 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/bootstrap/
--rw-rw-rw-   0        0        0     1047 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/bootstrap/base.html
--rw-rw-rw-   0        0        0      287 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/bootstrap/fixes.html
--rw-rw-rw-   0        0        0     1607 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/bootstrap/google.html
--rw-rw-rw-   0        0        0     2020 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/bootstrap/pagination.html
--rw-rw-rw-   0        0        0     1490 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/bootstrap/utils.html
--rw-rw-rw-   0        0        0     8115 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/bootstrap/wtf.html
-drwxrwxrwx   0        0        0        0 2024-05-28 02:57:37.639515 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask/
--rw-rw-rw-   0        0        0       41 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask/README
-drwxrwxrwx   0        0        0        0 2024-05-28 02:57:37.663989 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask/__pycache__/
--rw-rw-rw-   0        0        0     4571 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask/__pycache__/env.cpython-312.pyc
--rw-rw-rw-   0        0        0      857 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask/alembic.ini.mako
--rw-rw-rw-   0        0        0     3344 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask/env.py
--rw-rw-rw-   0        0        0      494 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask/script.py.mako
-drwxrwxrwx   0        0        0        0 2024-05-28 02:57:37.647034 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask-multidb/
--rw-rw-rw-   0        0        0       40 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask-multidb/README
-drwxrwxrwx   0        0        0        0 2024-05-28 02:57:37.662992 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/
--rw-rw-rw-   0        0        0     1826 2024-04-15 00:52:26.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/admin.html
--rw-rw-rw-   0        0        0      851 2024-04-15 00:52:25.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/applications.html
--rw-rw-rw-   0        0        0     2871 2024-04-15 00:52:24.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/base.html
--rw-rw-rw-   0        0        0     7933 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/env.cpython-312.pyc
--rw-rw-rw-   0        0        0     1783 2024-04-15 00:52:23.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/index.html
--rw-rw-rw-   0        0        0     1822 2024-05-28 02:56:45.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/login.html
--rw-rw-rw-   0        0        0      277 2024-04-15 00:52:24.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/logout.html
--rw-rw-rw-   0        0        0      853 2024-04-15 00:52:25.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/new_application.html
--rw-rw-rw-   0        0        0     3454 2024-05-28 02:56:38.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/register.html
--rw-rw-rw-   0        0        0      857 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask-multidb/alembic.ini.mako
--rw-rw-rw-   0        0        0     6190 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask-multidb/env.py
--rw-rw-rw-   0        0        0     1246 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask-multidb/script.py.mako
--rw-rw-rw-   0        0        0     3619 2023-12-09 17:30:07.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-28 02:57:37.666981 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds.egg-info/
--rw-rw-rw-   0        0        0      512 2024-05-28 02:57:37.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4418 2024-05-28 02:57:37.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 02:57:37.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-05-28 02:57:37.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-28 02:57:37.668975 flask_bootstrap_module_extendeds-5.1.4/setup.cfg
--rw-rw-rw-   0        0        0      822 2024-05-28 02:53:31.000000 flask_bootstrap_module_extendeds-5.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 03:07:36.416903 flask_bootstrap_module_extendeds-5.1.5/
+-rw-rw-rw-   0        0        0      111 2024-05-28 00:25:39.000000 flask_bootstrap_module_extendeds-5.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      512 2024-05-28 03:07:36.416903 flask_bootstrap_module_extendeds-5.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0       72 2024-05-27 22:54:19.000000 flask_bootstrap_module_extendeds-5.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 03:07:36.330155 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/
+-rw-rw-rw-   0        0        0        0 2024-05-28 00:15:24.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/__init__.py
+-rw-rw-rw-   0        0        0     2366 2023-12-09 17:30:07.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/_backwards.py
+-rw-rw-rw-   0        0        0     2812 2023-12-09 17:30:07.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/_compat.py
+-rw-rw-rw-   0        0        0     3806 2023-12-09 17:30:07.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/actions.py
+-rw-rw-rw-   0        0        0     2021 2023-12-09 17:30:07.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/babel.py
+-rw-rw-rw-   0        0        0    25372 2023-12-09 17:30:07.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/base.py
+-rw-rw-rw-   0        0        0    10689 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/cli.py
+-rw-rw-rw-   0        0        0      222 2023-12-09 17:30:07.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/consts.py
+-rw-rw-rw-   0        0        0     4628 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/forms.py
+-rw-rw-rw-   0        0        0     4269 2023-12-09 17:30:07.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/helpers.py
+-rw-rw-rw-   0        0        0     3582 2023-12-09 17:30:07.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/menu.py
+-rw-rw-rw-   0        0        0     3437 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/nav.py
+-rw-rw-rw-   0        0        0     5911 2024-05-27 22:54:06.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/refusion.py
+drwxrwxrwx   0        0        0        0 2024-05-28 03:07:36.341107 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/static/
+drwxrwxrwx   0        0        0        0 2024-05-28 03:07:36.352076 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/static/css/
+-rw-rw-rw-   0        0        0    26132 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/static/css/bootstrap-theme.css
+-rw-rw-rw-   0        0        0    47706 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/static/css/bootstrap-theme.css.map
+-rw-rw-rw-   0        0        0    23409 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/static/css/bootstrap-theme.min.css
+-rw-rw-rw-   0        0        0   146010 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/static/css/bootstrap.css
+-rw-rw-rw-   0        0        0   389287 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/static/css/bootstrap.css.map
+-rw-rw-rw-   0        0        0   121200 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/static/css/bootstrap.min.css
+drwxrwxrwx   0        0        0        0 2024-05-28 03:07:36.360055 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/static/fonts/
+-rw-rw-rw-   0        0        0    20127 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/static/fonts/glyphicons-halflings-regular.eot
+-rw-rw-rw-   0        0        0   108738 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/static/fonts/glyphicons-halflings-regular.svg
+-rw-rw-rw-   0        0        0    45404 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/static/fonts/glyphicons-halflings-regular.ttf
+-rw-rw-rw-   0        0        0    23424 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/static/fonts/glyphicons-halflings-regular.woff
+-rw-rw-rw-   0        0        0    18028 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/static/fonts/glyphicons-halflings-regular.woff2
+-rw-rw-rw-   0        0        0   293430 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/static/jquery.js
+-rw-rw-rw-   0        0        0    97163 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/static/jquery.min.js
+-rw-rw-rw-   0        0        0   143947 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/static/jquery.min.map
+drwxrwxrwx   0        0        0        0 2024-05-28 03:07:36.364044 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/static/js/
+-rw-rw-rw-   0        0        0    69707 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/static/js/bootstrap.js
+-rw-rw-rw-   0        0        0    37045 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/static/js/bootstrap.min.js
+-rw-rw-rw-   0        0        0      484 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/static/js/npm.js
+drwxrwxrwx   0        0        0        0 2024-05-28 03:07:36.297616 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/
+drwxrwxrwx   0        0        0        0 2024-05-28 03:07:36.370028 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/aioflask/
+-rw-rw-rw-   0        0        0       44 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/aioflask/README
+drwxrwxrwx   0        0        0        0 2024-05-28 03:07:36.379004 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/aioflask/__pycache__/
+-rw-rw-rw-   0        0        0     5072 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/aioflask/__pycache__/env.cpython-312.pyc
+-rw-rw-rw-   0        0        0      857 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/aioflask/alembic.ini.mako
+-rw-rw-rw-   0        0        0     3478 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/aioflask/env.py
+-rw-rw-rw-   0        0        0      494 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/aioflask/script.py.mako
+drwxrwxrwx   0        0        0        0 2024-05-28 03:07:36.376012 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/aioflask-multidb/
+-rw-rw-rw-   0        0        0       43 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/aioflask-multidb/README
+drwxrwxrwx   0        0        0        0 2024-05-28 03:07:36.378007 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/aioflask-multidb/__pycache__/
+-rw-rw-rw-   0        0        0     8813 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/aioflask-multidb/__pycache__/env.cpython-312.pyc
+-rw-rw-rw-   0        0        0      857 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/aioflask-multidb/alembic.ini.mako
+-rw-rw-rw-   0        0        0     6573 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/aioflask-multidb/env.py
+-rw-rw-rw-   0        0        0     1246 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/aioflask-multidb/script.py.mako
+drwxrwxrwx   0        0        0        0 2024-05-28 03:07:36.387980 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/bootstrap/
+-rw-rw-rw-   0        0        0     1047 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/bootstrap/base.html
+-rw-rw-rw-   0        0        0      287 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/bootstrap/fixes.html
+-rw-rw-rw-   0        0        0     1607 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/bootstrap/google.html
+-rw-rw-rw-   0        0        0     2020 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/bootstrap/pagination.html
+-rw-rw-rw-   0        0        0     1490 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/bootstrap/utils.html
+-rw-rw-rw-   0        0        0     8115 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/bootstrap/wtf.html
+drwxrwxrwx   0        0        0        0 2024-05-28 03:07:36.393964 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/flask/
+-rw-rw-rw-   0        0        0       41 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/flask/README
+drwxrwxrwx   0        0        0        0 2024-05-28 03:07:36.413911 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/flask/__pycache__/
+-rw-rw-rw-   0        0        0     4571 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/flask/__pycache__/env.cpython-312.pyc
+-rw-rw-rw-   0        0        0      857 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/flask/alembic.ini.mako
+-rw-rw-rw-   0        0        0     3344 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/flask/env.py
+-rw-rw-rw-   0        0        0      494 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/flask/script.py.mako
+drwxrwxrwx   0        0        0        0 2024-05-28 03:07:36.398951 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/flask-multidb/
+-rw-rw-rw-   0        0        0       40 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/flask-multidb/README
+drwxrwxrwx   0        0        0        0 2024-05-28 03:07:36.411917 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/
+-rw-rw-rw-   0        0        0     1826 2024-04-15 00:52:26.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/env.ad-312.pyc
+-rw-rw-rw-   0        0        0      851 2024-04-15 00:52:25.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/env.aplic-312.pyc
+-rw-rw-rw-   0        0        0     2871 2024-04-15 00:52:24.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/env.base-312.pyc
+-rw-rw-rw-   0        0        0     7933 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/env.cpython-312.pyc
+-rw-rw-rw-   0        0        0     1783 2024-04-15 00:52:23.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/env.index-312.pyc
+-rw-rw-rw-   0        0        0     1822 2024-05-28 02:56:45.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/env.log-312.pyc
+-rw-rw-rw-   0        0        0      277 2024-04-15 00:52:24.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/env.logo-312.pyc
+-rw-rw-rw-   0        0        0      853 2024-04-15 00:52:25.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/env.naplic-312.pyc
+-rw-rw-rw-   0        0        0     3454 2024-05-28 02:56:38.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/env.reg-312.pyc
+-rw-rw-rw-   0        0        0      857 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/flask-multidb/alembic.ini.mako
+-rw-rw-rw-   0        0        0     6190 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/flask-multidb/env.py
+-rw-rw-rw-   0        0        0     1246 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/flask-multidb/script.py.mako
+-rw-rw-rw-   0        0        0     3619 2023-12-09 17:30:07.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-28 03:07:36.415905 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds.egg-info/
+-rw-rw-rw-   0        0        0      512 2024-05-28 03:07:36.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4446 2024-05-28 03:07:36.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 03:07:36.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-05-28 03:07:36.000000 flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-28 03:07:36.417901 flask_bootstrap_module_extendeds-5.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      822 2024-05-28 03:07:27.000000 flask_bootstrap_module_extendeds-5.1.5/setup.py
```

### Comparing `flask_bootstrap_module_extendeds-5.1.4/PKG-INFO` & `flask_bootstrap_module_extendeds-5.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask_bootstrap_module_extendeds
-Version: 5.1.4
+Version: 5.1.5
 Summary: Flask bootstrap-library EXTENDED
 Home-page: https://github.com/yourusername/my_library
 Author: Dex
 Author-email: censored@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/_backwards.py` & `flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/_backwards.py`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/_compat.py` & `flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/_compat.py`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/actions.py` & `flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/actions.py`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/babel.py` & `flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/babel.py`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/base.py` & `flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/base.py`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/cli.py` & `flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/cli.py`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/forms.py` & `flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/forms.py`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/helpers.py` & `flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/helpers.py`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/menu.py` & `flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/menu.py`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/nav.py` & `flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/nav.py`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/refusion.py` & `flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/refusion.py`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/css/bootstrap-theme.css` & `flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/static/css/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/css/bootstrap-theme.css.map` & `flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/static/css/bootstrap-theme.css.map`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/css/bootstrap-theme.min.css` & `flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/static/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/css/bootstrap.css` & `flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/static/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/css/bootstrap.css.map` & `flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/static/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/css/bootstrap.min.css` & `flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/fonts/glyphicons-halflings-regular.eot` & `flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/static/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/fonts/glyphicons-halflings-regular.svg` & `flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/static/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/fonts/glyphicons-halflings-regular.ttf` & `flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/static/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/fonts/glyphicons-halflings-regular.woff` & `flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/static/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/fonts/glyphicons-halflings-regular.woff2` & `flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/static/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/jquery.js` & `flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/static/jquery.js`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/jquery.min.js` & `flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/static/jquery.min.js`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/jquery.min.map` & `flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/static/jquery.min.map`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/js/bootstrap.js` & `flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/static/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/js/bootstrap.min.js` & `flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/aioflask/__pycache__/env.cpython-312.pyc` & `flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/aioflask/__pycache__/env.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/aioflask/alembic.ini.mako` & `flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/aioflask/alembic.ini.mako`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/aioflask/env.py` & `flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/aioflask/env.py`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/aioflask-multidb/__pycache__/env.cpython-312.pyc` & `flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/aioflask-multidb/__pycache__/env.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/aioflask-multidb/alembic.ini.mako` & `flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/aioflask-multidb/alembic.ini.mako`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/aioflask-multidb/env.py` & `flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/aioflask-multidb/env.py`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/aioflask-multidb/script.py.mako` & `flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/aioflask-multidb/script.py.mako`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/bootstrap/base.html` & `flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/bootstrap/base.html`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/bootstrap/google.html` & `flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/bootstrap/google.html`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/bootstrap/pagination.html` & `flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/bootstrap/pagination.html`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/bootstrap/utils.html` & `flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/bootstrap/utils.html`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/bootstrap/wtf.html` & `flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/bootstrap/wtf.html`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask/__pycache__/env.cpython-312.pyc` & `flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/flask/__pycache__/env.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask/alembic.ini.mako` & `flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/flask/alembic.ini.mako`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask/env.py` & `flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/flask/env.py`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/admin.html` & `flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/env.ad-312.pyc`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/applications.html` & `flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/env.aplic-312.pyc`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/base.html` & `flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/env.base-312.pyc`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/env.cpython-312.pyc` & `flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/env.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/index.html` & `flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/env.index-312.pyc`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/login.html` & `flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/env.log-312.pyc`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/new_application.html` & `flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/env.naplic-312.pyc`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/register.html` & `flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/env.reg-312.pyc`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask-multidb/alembic.ini.mako` & `flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/flask-multidb/alembic.ini.mako`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask-multidb/env.py` & `flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/flask-multidb/env.py`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask-multidb/script.py.mako` & `flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/templates/flask-multidb/script.py.mako`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/tools.py` & `flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds/tools.py`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds.egg-info/PKG-INFO` & `flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask_bootstrap_module_extendeds
-Version: 5.1.4
+Version: 5.1.5
 Summary: Flask bootstrap-library EXTENDED
 Home-page: https://github.com/yourusername/my_library
 Author: Dex
 Author-email: censored@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds.egg-info/SOURCES.txt` & `flask_bootstrap_module_extendeds-5.1.5/flask_bootstrap_module_extendeds.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -57,17 +57,17 @@
 flask_bootstrap_module_extendeds/templates/flask/alembic.ini.mako
 flask_bootstrap_module_extendeds/templates/flask/env.py
 flask_bootstrap_module_extendeds/templates/flask/script.py.mako
 flask_bootstrap_module_extendeds/templates/flask-multidb/README
 flask_bootstrap_module_extendeds/templates/flask-multidb/alembic.ini.mako
 flask_bootstrap_module_extendeds/templates/flask-multidb/env.py
 flask_bootstrap_module_extendeds/templates/flask-multidb/script.py.mako
-flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/admin.html
-flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/applications.html
-flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/base.html
+flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/env.ad-312.pyc
+flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/env.aplic-312.pyc
+flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/env.base-312.pyc
 flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/env.cpython-312.pyc
-flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/index.html
-flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/login.html
-flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/logout.html
-flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/new_application.html
-flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/register.html
+flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/env.index-312.pyc
+flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/env.log-312.pyc
+flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/env.logo-312.pyc
+flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/env.naplic-312.pyc
+flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/env.reg-312.pyc
 flask_bootstrap_module_extendeds/templates/flask/__pycache__/env.cpython-312.pyc
```

### Comparing `flask_bootstrap_module_extendeds-5.1.4/setup.py` & `flask_bootstrap_module_extendeds-5.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="flask_bootstrap_module_extendeds",
-    version="5.1.4",
+    version="5.1.5",
     author="Dex",
     author_email="censored@gmail.com",
     description="Flask bootstrap-library EXTENDED",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/yourusername/my_library",
     packages=find_packages(),
```

