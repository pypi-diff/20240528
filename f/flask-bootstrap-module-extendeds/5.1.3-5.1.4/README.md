# Comparing `tmp/flask_bootstrap_module_extendeds-5.1.3.tar.gz` & `tmp/flask_bootstrap_module_extendeds-5.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_bootstrap_module_extendeds-5.1.3.tar", last modified: Tue May 28 00:38:10 2024, max compression
+gzip compressed data, was "flask_bootstrap_module_extendeds-5.1.4.tar", last modified: Tue May 28 02:57:37 2024, max compression
```

## Comparing `flask_bootstrap_module_extendeds-5.1.3.tar` & `flask_bootstrap_module_extendeds-5.1.4.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 00:38:10.858766 flask_bootstrap_module_extendeds-5.1.3/
--rw-rw-rw-   0        0        0      111 2024-05-28 00:25:39.000000 flask_bootstrap_module_extendeds-5.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0      512 2024-05-28 00:38:10.857768 flask_bootstrap_module_extendeds-5.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       72 2024-05-27 22:54:19.000000 flask_bootstrap_module_extendeds-5.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-28 00:38:10.769007 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/
--rw-rw-rw-   0        0        0        0 2024-05-28 00:15:24.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/__init__.py
--rw-rw-rw-   0        0        0     2366 2023-12-09 17:30:07.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/_backwards.py
--rw-rw-rw-   0        0        0     2812 2023-12-09 17:30:07.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/_compat.py
--rw-rw-rw-   0        0        0     3806 2023-12-09 17:30:07.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/actions.py
--rw-rw-rw-   0        0        0     2021 2023-12-09 17:30:07.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/babel.py
--rw-rw-rw-   0        0        0    25372 2023-12-09 17:30:07.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/base.py
--rw-rw-rw-   0        0        0    10689 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/cli.py
--rw-rw-rw-   0        0        0      222 2023-12-09 17:30:07.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/consts.py
--rw-rw-rw-   0        0        0     4628 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/forms.py
--rw-rw-rw-   0        0        0     4269 2023-12-09 17:30:07.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/helpers.py
--rw-rw-rw-   0        0        0     3582 2023-12-09 17:30:07.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/menu.py
--rw-rw-rw-   0        0        0     3437 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/nav.py
--rw-rw-rw-   0        0        0     5911 2024-05-27 22:54:06.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/refusion.py
-drwxrwxrwx   0        0        0        0 2024-05-28 00:38:10.781973 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/static/
-drwxrwxrwx   0        0        0        0 2024-05-28 00:38:10.791944 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/static/css/
--rw-rw-rw-   0        0        0    26132 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/static/css/bootstrap-theme.css
--rw-rw-rw-   0        0        0    47706 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/static/css/bootstrap-theme.css.map
--rw-rw-rw-   0        0        0    23409 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/static/css/bootstrap-theme.min.css
--rw-rw-rw-   0        0        0   146010 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/static/css/bootstrap.css
--rw-rw-rw-   0        0        0   389287 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/static/css/bootstrap.css.map
--rw-rw-rw-   0        0        0   121200 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/static/css/bootstrap.min.css
-drwxrwxrwx   0        0        0        0 2024-05-28 00:38:10.799923 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/static/fonts/
--rw-rw-rw-   0        0        0    20127 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/static/fonts/glyphicons-halflings-regular.eot
--rw-rw-rw-   0        0        0   108738 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/static/fonts/glyphicons-halflings-regular.svg
--rw-rw-rw-   0        0        0    45404 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/static/fonts/glyphicons-halflings-regular.ttf
--rw-rw-rw-   0        0        0    23424 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/static/fonts/glyphicons-halflings-regular.woff
--rw-rw-rw-   0        0        0    18028 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/static/fonts/glyphicons-halflings-regular.woff2
--rw-rw-rw-   0        0        0   293430 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/static/jquery.js
--rw-rw-rw-   0        0        0    97163 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/static/jquery.min.js
--rw-rw-rw-   0        0        0   143947 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/static/jquery.min.map
-drwxrwxrwx   0        0        0        0 2024-05-28 00:38:10.804910 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/static/js/
--rw-rw-rw-   0        0        0    69707 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/static/js/bootstrap.js
--rw-rw-rw-   0        0        0    37045 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/static/js/bootstrap.min.js
--rw-rw-rw-   0        0        0      484 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/static/js/npm.js
-drwxrwxrwx   0        0        0        0 2024-05-28 00:38:10.738088 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/
-drwxrwxrwx   0        0        0        0 2024-05-28 00:38:10.810894 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/aioflask/
--rw-rw-rw-   0        0        0       44 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/aioflask/README
-drwxrwxrwx   0        0        0        0 2024-05-28 00:38:10.819870 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/aioflask/__pycache__/
--rw-rw-rw-   0        0        0     5072 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/aioflask/__pycache__/env.cpython-312.pyc
--rw-rw-rw-   0        0        0      857 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/aioflask/alembic.ini.mako
--rw-rw-rw-   0        0        0     3478 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/aioflask/env.py
--rw-rw-rw-   0        0        0      494 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/aioflask/script.py.mako
-drwxrwxrwx   0        0        0        0 2024-05-28 00:38:10.816877 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/aioflask-multidb/
--rw-rw-rw-   0        0        0       43 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/aioflask-multidb/README
-drwxrwxrwx   0        0        0        0 2024-05-28 00:38:10.817875 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/aioflask-multidb/__pycache__/
--rw-rw-rw-   0        0        0     8813 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/aioflask-multidb/__pycache__/env.cpython-312.pyc
--rw-rw-rw-   0        0        0      857 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/aioflask-multidb/alembic.ini.mako
--rw-rw-rw-   0        0        0     6573 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/aioflask-multidb/env.py
--rw-rw-rw-   0        0        0     1246 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/aioflask-multidb/script.py.mako
-drwxrwxrwx   0        0        0        0 2024-05-28 00:38:10.827849 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/bootstrap/
--rw-rw-rw-   0        0        0     1047 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/bootstrap/base.html
--rw-rw-rw-   0        0        0      287 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/bootstrap/fixes.html
--rw-rw-rw-   0        0        0     1607 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/bootstrap/google.html
--rw-rw-rw-   0        0        0     2020 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/bootstrap/pagination.html
--rw-rw-rw-   0        0        0     1490 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/bootstrap/utils.html
--rw-rw-rw-   0        0        0     8115 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/bootstrap/wtf.html
-drwxrwxrwx   0        0        0        0 2024-05-28 00:38:10.833832 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/flask/
--rw-rw-rw-   0        0        0       41 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/flask/README
-drwxrwxrwx   0        0        0        0 2024-05-28 00:38:10.854776 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/flask/__pycache__/
--rw-rw-rw-   0        0        0     4571 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/flask/__pycache__/env.cpython-312.pyc
--rw-rw-rw-   0        0        0      857 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/flask/alembic.ini.mako
--rw-rw-rw-   0        0        0     3344 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/flask/env.py
--rw-rw-rw-   0        0        0      494 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/flask/script.py.mako
-drwxrwxrwx   0        0        0        0 2024-05-28 00:38:10.839817 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/flask-multidb/
--rw-rw-rw-   0        0        0       40 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/flask-multidb/README
-drwxrwxrwx   0        0        0        0 2024-05-28 00:38:10.853779 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/
--rw-rw-rw-   0        0        0     1826 2024-04-15 00:52:26.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/admin.html
--rw-rw-rw-   0        0        0      851 2024-04-15 00:52:25.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/applications.html
--rw-rw-rw-   0        0        0     2871 2024-04-15 00:52:24.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/base.html
--rw-rw-rw-   0        0        0     7933 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/env.cpython-312.pyc
--rw-rw-rw-   0        0        0     1783 2024-04-15 00:52:23.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/index.html
--rw-rw-rw-   0        0        0      746 2024-04-15 00:52:25.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/login.html
--rw-rw-rw-   0        0        0      277 2024-04-15 00:52:24.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/logout.html
--rw-rw-rw-   0        0        0      853 2024-04-15 00:52:25.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/new_application.html
--rw-rw-rw-   0        0        0     1383 2024-04-15 00:52:24.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/register.html
--rw-rw-rw-   0        0        0      857 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/flask-multidb/alembic.ini.mako
--rw-rw-rw-   0        0        0     6190 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/flask-multidb/env.py
--rw-rw-rw-   0        0        0     1246 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/flask-multidb/script.py.mako
--rw-rw-rw-   0        0        0     3619 2023-12-09 17:30:07.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-28 00:38:10.856771 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds.egg-info/
--rw-rw-rw-   0        0        0      512 2024-05-28 00:38:10.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4418 2024-05-28 00:38:10.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 00:38:10.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-05-28 00:38:10.000000 flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-28 00:38:10.859763 flask_bootstrap_module_extendeds-5.1.3/setup.cfg
--rw-rw-rw-   0        0        0      822 2024-05-28 00:37:59.000000 flask_bootstrap_module_extendeds-5.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 02:57:37.667978 flask_bootstrap_module_extendeds-5.1.4/
+-rw-rw-rw-   0        0        0      111 2024-05-28 00:25:39.000000 flask_bootstrap_module_extendeds-5.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      512 2024-05-28 02:57:37.667978 flask_bootstrap_module_extendeds-5.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0       72 2024-05-27 22:54:19.000000 flask_bootstrap_module_extendeds-5.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 02:57:37.553746 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/
+-rw-rw-rw-   0        0        0        0 2024-05-28 00:15:24.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/__init__.py
+-rw-rw-rw-   0        0        0     2366 2023-12-09 17:30:07.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/_backwards.py
+-rw-rw-rw-   0        0        0     2812 2023-12-09 17:30:07.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/_compat.py
+-rw-rw-rw-   0        0        0     3806 2023-12-09 17:30:07.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/actions.py
+-rw-rw-rw-   0        0        0     2021 2023-12-09 17:30:07.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/babel.py
+-rw-rw-rw-   0        0        0    25372 2023-12-09 17:30:07.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/base.py
+-rw-rw-rw-   0        0        0    10689 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/cli.py
+-rw-rw-rw-   0        0        0      222 2023-12-09 17:30:07.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/consts.py
+-rw-rw-rw-   0        0        0     4628 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/forms.py
+-rw-rw-rw-   0        0        0     4269 2023-12-09 17:30:07.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/helpers.py
+-rw-rw-rw-   0        0        0     3582 2023-12-09 17:30:07.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/menu.py
+-rw-rw-rw-   0        0        0     3437 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/nav.py
+-rw-rw-rw-   0        0        0     5911 2024-05-27 22:54:06.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/refusion.py
+drwxrwxrwx   0        0        0        0 2024-05-28 02:57:37.568706 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/
+drwxrwxrwx   0        0        0        0 2024-05-28 02:57:37.585659 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/css/
+-rw-rw-rw-   0        0        0    26132 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/css/bootstrap-theme.css
+-rw-rw-rw-   0        0        0    47706 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/css/bootstrap-theme.css.map
+-rw-rw-rw-   0        0        0    23409 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/css/bootstrap-theme.min.css
+-rw-rw-rw-   0        0        0   146010 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/css/bootstrap.css
+-rw-rw-rw-   0        0        0   389287 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/css/bootstrap.css.map
+-rw-rw-rw-   0        0        0   121200 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/css/bootstrap.min.css
+drwxrwxrwx   0        0        0        0 2024-05-28 02:57:37.598625 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/fonts/
+-rw-rw-rw-   0        0        0    20127 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/fonts/glyphicons-halflings-regular.eot
+-rw-rw-rw-   0        0        0   108738 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/fonts/glyphicons-halflings-regular.svg
+-rw-rw-rw-   0        0        0    45404 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/fonts/glyphicons-halflings-regular.ttf
+-rw-rw-rw-   0        0        0    23424 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/fonts/glyphicons-halflings-regular.woff
+-rw-rw-rw-   0        0        0    18028 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/fonts/glyphicons-halflings-regular.woff2
+-rw-rw-rw-   0        0        0   293430 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/jquery.js
+-rw-rw-rw-   0        0        0    97163 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/jquery.min.js
+-rw-rw-rw-   0        0        0   143947 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/jquery.min.map
+drwxrwxrwx   0        0        0        0 2024-05-28 02:57:37.604608 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/js/
+-rw-rw-rw-   0        0        0    69707 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/js/bootstrap.js
+-rw-rw-rw-   0        0        0    37045 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/js/bootstrap.min.js
+-rw-rw-rw-   0        0        0      484 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/js/npm.js
+drwxrwxrwx   0        0        0        0 2024-05-28 02:57:37.517866 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/
+drwxrwxrwx   0        0        0        0 2024-05-28 02:57:37.611590 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/aioflask/
+-rw-rw-rw-   0        0        0       44 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/aioflask/README
+drwxrwxrwx   0        0        0        0 2024-05-28 02:57:37.621564 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/aioflask/__pycache__/
+-rw-rw-rw-   0        0        0     5072 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/aioflask/__pycache__/env.cpython-312.pyc
+-rw-rw-rw-   0        0        0      857 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/aioflask/alembic.ini.mako
+-rw-rw-rw-   0        0        0     3478 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/aioflask/env.py
+-rw-rw-rw-   0        0        0      494 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/aioflask/script.py.mako
+drwxrwxrwx   0        0        0        0 2024-05-28 02:57:37.618571 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/aioflask-multidb/
+-rw-rw-rw-   0        0        0       43 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/aioflask-multidb/README
+drwxrwxrwx   0        0        0        0 2024-05-28 02:57:37.620566 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/aioflask-multidb/__pycache__/
+-rw-rw-rw-   0        0        0     8813 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/aioflask-multidb/__pycache__/env.cpython-312.pyc
+-rw-rw-rw-   0        0        0      857 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/aioflask-multidb/alembic.ini.mako
+-rw-rw-rw-   0        0        0     6573 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/aioflask-multidb/env.py
+-rw-rw-rw-   0        0        0     1246 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/aioflask-multidb/script.py.mako
+drwxrwxrwx   0        0        0        0 2024-05-28 02:57:37.632534 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/bootstrap/
+-rw-rw-rw-   0        0        0     1047 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/bootstrap/base.html
+-rw-rw-rw-   0        0        0      287 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/bootstrap/fixes.html
+-rw-rw-rw-   0        0        0     1607 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/bootstrap/google.html
+-rw-rw-rw-   0        0        0     2020 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/bootstrap/pagination.html
+-rw-rw-rw-   0        0        0     1490 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/bootstrap/utils.html
+-rw-rw-rw-   0        0        0     8115 2024-04-14 23:46:26.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/bootstrap/wtf.html
+drwxrwxrwx   0        0        0        0 2024-05-28 02:57:37.639515 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask/
+-rw-rw-rw-   0        0        0       41 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask/README
+drwxrwxrwx   0        0        0        0 2024-05-28 02:57:37.663989 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask/__pycache__/
+-rw-rw-rw-   0        0        0     4571 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask/__pycache__/env.cpython-312.pyc
+-rw-rw-rw-   0        0        0      857 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask/alembic.ini.mako
+-rw-rw-rw-   0        0        0     3344 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask/env.py
+-rw-rw-rw-   0        0        0      494 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask/script.py.mako
+drwxrwxrwx   0        0        0        0 2024-05-28 02:57:37.647034 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask-multidb/
+-rw-rw-rw-   0        0        0       40 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask-multidb/README
+drwxrwxrwx   0        0        0        0 2024-05-28 02:57:37.662992 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/
+-rw-rw-rw-   0        0        0     1826 2024-04-15 00:52:26.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/admin.html
+-rw-rw-rw-   0        0        0      851 2024-04-15 00:52:25.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/applications.html
+-rw-rw-rw-   0        0        0     2871 2024-04-15 00:52:24.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/base.html
+-rw-rw-rw-   0        0        0     7933 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/env.cpython-312.pyc
+-rw-rw-rw-   0        0        0     1783 2024-04-15 00:52:23.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/index.html
+-rw-rw-rw-   0        0        0     1822 2024-05-28 02:56:45.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/login.html
+-rw-rw-rw-   0        0        0      277 2024-04-15 00:52:24.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/logout.html
+-rw-rw-rw-   0        0        0      853 2024-04-15 00:52:25.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/new_application.html
+-rw-rw-rw-   0        0        0     3454 2024-05-28 02:56:38.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/register.html
+-rw-rw-rw-   0        0        0      857 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask-multidb/alembic.ini.mako
+-rw-rw-rw-   0        0        0     6190 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask-multidb/env.py
+-rw-rw-rw-   0        0        0     1246 2024-05-24 14:36:43.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask-multidb/script.py.mako
+-rw-rw-rw-   0        0        0     3619 2023-12-09 17:30:07.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-28 02:57:37.666981 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds.egg-info/
+-rw-rw-rw-   0        0        0      512 2024-05-28 02:57:37.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4418 2024-05-28 02:57:37.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 02:57:37.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-05-28 02:57:37.000000 flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-28 02:57:37.668975 flask_bootstrap_module_extendeds-5.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      822 2024-05-28 02:53:31.000000 flask_bootstrap_module_extendeds-5.1.4/setup.py
```

### Comparing `flask_bootstrap_module_extendeds-5.1.3/PKG-INFO` & `flask_bootstrap_module_extendeds-5.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask_bootstrap_module_extendeds
-Version: 5.1.3
+Version: 5.1.4
 Summary: Flask bootstrap-library EXTENDED
 Home-page: https://github.com/yourusername/my_library
 Author: Dex
 Author-email: censored@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/_backwards.py` & `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/_backwards.py`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/_compat.py` & `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/_compat.py`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/actions.py` & `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/actions.py`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/babel.py` & `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/babel.py`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/base.py` & `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/base.py`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/cli.py` & `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/cli.py`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/forms.py` & `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/forms.py`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/helpers.py` & `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/helpers.py`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/menu.py` & `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/menu.py`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/nav.py` & `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/nav.py`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/refusion.py` & `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/refusion.py`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/static/css/bootstrap-theme.css` & `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/css/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/static/css/bootstrap-theme.css.map` & `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/css/bootstrap-theme.css.map`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/static/css/bootstrap-theme.min.css` & `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/static/css/bootstrap.css` & `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/static/css/bootstrap.css.map` & `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/static/css/bootstrap.min.css` & `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/static/fonts/glyphicons-halflings-regular.eot` & `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/static/fonts/glyphicons-halflings-regular.svg` & `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/static/fonts/glyphicons-halflings-regular.ttf` & `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/static/fonts/glyphicons-halflings-regular.woff` & `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/static/fonts/glyphicons-halflings-regular.woff2` & `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/static/jquery.js` & `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/jquery.js`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/static/jquery.min.js` & `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/jquery.min.js`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/static/jquery.min.map` & `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/jquery.min.map`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/static/js/bootstrap.js` & `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/static/js/bootstrap.min.js` & `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/aioflask/__pycache__/env.cpython-312.pyc` & `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/aioflask/__pycache__/env.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/aioflask/alembic.ini.mako` & `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/aioflask/alembic.ini.mako`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/aioflask/env.py` & `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/aioflask/env.py`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/aioflask-multidb/__pycache__/env.cpython-312.pyc` & `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/aioflask-multidb/__pycache__/env.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/aioflask-multidb/alembic.ini.mako` & `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/aioflask-multidb/alembic.ini.mako`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/aioflask-multidb/env.py` & `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/aioflask-multidb/env.py`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/aioflask-multidb/script.py.mako` & `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/aioflask-multidb/script.py.mako`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/bootstrap/base.html` & `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/bootstrap/base.html`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/bootstrap/google.html` & `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/bootstrap/google.html`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/bootstrap/pagination.html` & `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/bootstrap/pagination.html`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/bootstrap/utils.html` & `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/bootstrap/utils.html`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/bootstrap/wtf.html` & `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/bootstrap/wtf.html`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/flask/__pycache__/env.cpython-312.pyc` & `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask/__pycache__/env.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/flask/alembic.ini.mako` & `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask/alembic.ini.mako`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/flask/env.py` & `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask/env.py`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/admin.html` & `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/admin.html`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/applications.html` & `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/applications.html`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/base.html` & `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/base.html`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/env.cpython-312.pyc` & `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/env.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/index.html` & `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/index.html`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/new_application.html` & `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/new_application.html`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/register.html` & `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask-multidb/__pycache__/login.html`

 * *Files 25% similar despite different names*

```diff
@@ -1,87 +1,114 @@
 00000000: 7b25 2065 7874 656e 6473 2027 6261 7365  {% extends 'base
 00000010: 2e68 746d 6c27 2025 7d0d 0a0d 0a7b 2520  .html' %}....{% 
-00000020: 626c 6f63 6b20 7469 746c 6520 257d d0a0  block title %}..
-00000030: d0b5 d0b3 d0b8 d181 d182 d180 d0b0 d186  ................
+00000020: 626c 6f63 6b20 7469 746c 6520 257d d090  block title %}..
+00000030: d0b2 d182 d0be d180 d0b8 d0b7 d0b0 d186  ................
 00000040: d0b8 d18f 7b25 2065 6e64 626c 6f63 6b20  ....{% endblock 
 00000050: 257d 0d0a 0d0a 7b25 2062 6c6f 636b 2063  %}....{% block c
 00000060: 6f6e 7465 6e74 2025 7d0d 0a3c 6469 7620  ontent %}..<div 
 00000070: 636c 6173 733d 2263 6f6e 7461 696e 6572  class="container
 00000080: 223e 0d0a 2020 2020 3c68 3220 636c 6173  ">..    <h2 clas
-00000090: 733d 226d 742d 3522 3ed0 a0d0 b5d0 b3d0  s="mt-5">.......
-000000a0: b8d1 81d1 82d1 80d0 b0d1 86d0 b8d1 8f3c  ...............<
+00000090: 733d 226d 742d 3522 3ed0 90d0 b2d1 82d0  s="mt-5">.......
+000000a0: bed1 80d0 b8d0 b7d0 b0d1 86d0 b8d1 8f3c  ...............<
 000000b0: 2f68 323e 0d0a 2020 2020 3c66 6f72 6d20  /h2>..    <form 
-000000c0: 6d65 7468 6f64 3d22 706f 7374 223e 0d0a  method="post">..
-000000d0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-000000e0: 7373 3d22 6d62 2d33 223e 0d0a 2020 2020  ss="mb-3">..    
-000000f0: 2020 2020 2020 2020 3c6c 6162 656c 2066          <label f
-00000100: 6f72 3d22 7573 6572 6e61 6d65 2220 636c  or="username" cl
-00000110: 6173 733d 2266 6f72 6d2d 6c61 6265 6c22  ass="form-label"
-00000120: 3ed0 9bd0 bed0 b3d0 b8d0 bd3c 2f6c 6162  >..........</lab
-00000130: 656c 3e0d 0a20 2020 2020 2020 2020 2020  el>..           
-00000140: 203c 696e 7075 7420 7479 7065 3d22 7465   <input type="te
-00000150: 7874 2220 636c 6173 733d 2266 6f72 6d2d  xt" class="form-
-00000160: 636f 6e74 726f 6c22 2069 643d 2275 7365  control" id="use
-00000170: 726e 616d 6522 206e 616d 653d 2275 7365  rname" name="use
-00000180: 726e 616d 6522 2072 6571 7569 7265 643e  rname" required>
-00000190: 0d0a 2020 2020 2020 2020 3c2f 6469 763e  ..        </div>
-000001a0: 0d0a 2020 2020 2020 2020 3c64 6976 2063  ..        <div c
-000001b0: 6c61 7373 3d22 6d62 2d33 223e 0d0a 2020  lass="mb-3">..  
-000001c0: 2020 2020 2020 2020 2020 3c6c 6162 656c            <label
-000001d0: 2066 6f72 3d22 7061 7373 776f 7264 2220   for="password" 
-000001e0: 636c 6173 733d 2266 6f72 6d2d 6c61 6265  class="form-labe
-000001f0: 6c22 3ed0 9fd0 b0d1 80d0 bed0 bbd1 8c3c  l">............<
-00000200: 2f6c 6162 656c 3e0d 0a20 2020 2020 2020  /label>..       
-00000210: 2020 2020 203c 696e 7075 7420 7479 7065       <input type
-00000220: 3d22 7061 7373 776f 7264 2220 636c 6173  ="password" clas
-00000230: 733d 2266 6f72 6d2d 636f 6e74 726f 6c22  s="form-control"
-00000240: 2069 643d 2270 6173 7377 6f72 6422 206e   id="password" n
-00000250: 616d 653d 2270 6173 7377 6f72 6422 2072  ame="password" r
-00000260: 6571 7569 7265 643e 0d0a 2020 2020 2020  equired>..      
-00000270: 2020 3c2f 6469 763e 0d0a 2020 2020 2020    </div>..      
-00000280: 2020 3c64 6976 2063 6c61 7373 3d22 6d62    <div class="mb
-00000290: 2d33 223e 0d0a 2020 2020 2020 2020 2020  -3">..          
-000002a0: 2020 3c6c 6162 656c 2066 6f72 3d22 6675    <label for="fu
-000002b0: 6c6c 5f6e 616d 6522 2063 6c61 7373 3d22  ll_name" class="
-000002c0: 666f 726d 2d6c 6162 656c 223e d0a4 d098  form-label">....
-000002d0: d09e 3c2f 6c61 6265 6c3e 0d0a 2020 2020  ..</label>..    
-000002e0: 2020 2020 2020 2020 3c69 6e70 7574 2074          <input t
-000002f0: 7970 653d 2274 6578 7422 2063 6c61 7373  ype="text" class
-00000300: 3d22 666f 726d 2d63 6f6e 7472 6f6c 2220  ="form-control" 
-00000310: 6964 3d22 6675 6c6c 5f6e 616d 6522 206e  id="full_name" n
-00000320: 616d 653d 2266 756c 6c5f 6e61 6d65 2220  ame="full_name" 
-00000330: 7265 7175 6972 6564 3e0d 0a20 2020 2020  required>..     
-00000340: 2020 203c 2f64 6976 3e0d 0a20 2020 2020     </div>..     
-00000350: 2020 203c 6469 7620 636c 6173 733d 226d     <div class="m
-00000360: 622d 3322 3e0d 0a20 2020 2020 2020 2020  b-3">..         
-00000370: 2020 203c 6c61 6265 6c20 666f 723d 2270     <label for="p
-00000380: 686f 6e65 2220 636c 6173 733d 2266 6f72  hone" class="for
-00000390: 6d2d 6c61 6265 6c22 3ed0 a2d0 b5d0 bbd0  m-label">.......
-000003a0: b5d1 84d0 bed0 bd3c 2f6c 6162 656c 3e0d  .......</label>.
-000003b0: 0a20 2020 2020 2020 2020 2020 203c 696e  .            <in
-000003c0: 7075 7420 7479 7065 3d22 7465 7874 2220  put type="text" 
-000003d0: 636c 6173 733d 2266 6f72 6d2d 636f 6e74  class="form-cont
-000003e0: 726f 6c22 2069 643d 2270 686f 6e65 2220  rol" id="phone" 
-000003f0: 6e61 6d65 3d22 7068 6f6e 6522 2072 6571  name="phone" req
-00000400: 7569 7265 643e 0d0a 2020 2020 2020 2020  uired>..        
-00000410: 3c2f 6469 763e 0d0a 2020 2020 2020 2020  </div>..        
-00000420: 3c64 6976 2063 6c61 7373 3d22 6d62 2d33  <div class="mb-3
-00000430: 223e 0d0a 2020 2020 2020 2020 2020 2020  ">..            
-00000440: 3c6c 6162 656c 2066 6f72 3d22 656d 6169  <label for="emai
-00000450: 6c22 2063 6c61 7373 3d22 666f 726d 2d6c  l" class="form-l
-00000460: 6162 656c 223e 456d 6169 6c3c 2f6c 6162  abel">Email</lab
-00000470: 656c 3e0d 0a20 2020 2020 2020 2020 2020  el>..           
-00000480: 203c 696e 7075 7420 7479 7065 3d22 656d   <input type="em
-00000490: 6169 6c22 2063 6c61 7373 3d22 666f 726d  ail" class="form
-000004a0: 2d63 6f6e 7472 6f6c 2220 6964 3d22 656d  -control" id="em
-000004b0: 6169 6c22 206e 616d 653d 2265 6d61 696c  ail" name="email
-000004c0: 2220 7265 7175 6972 6564 3e0d 0a20 2020  " required>..   
-000004d0: 2020 2020 203c 2f64 6976 3e0d 0a20 2020       </div>..   
-000004e0: 2020 2020 203c 6275 7474 6f6e 2074 7970       <button typ
-000004f0: 653d 2273 7562 6d69 7422 2063 6c61 7373  e="submit" class
-00000500: 3d22 6274 6e20 6274 6e2d 7072 696d 6172  ="btn btn-primar
-00000510: 7922 3ed0 97d0 b0d1 80d0 b5d0 b3d0 b8d1  y">.............
-00000520: 81d1 82d1 80d0 b8d1 80d0 bed0 b2d0 b0d1  ................
-00000530: 82d1 8cd1 81d1 8f3c 2f62 7574 746f 6e3e  .......</button>
-00000540: 0d0a 2020 2020 3c2f 666f 726d 3e0d 0a3c  ..    </form>..<
-00000550: 2f64 6976 3e0d 0a7b 2520 656e 6462 6c6f  /div>..{% endblo
-00000560: 636b 2025 7d0d 0a                        ck %}..
+000000c0: 6d65 7468 6f64 3d22 706f 7374 2220 6964  method="post" id
+000000d0: 3d22 6c6f 6769 6e46 6f72 6d22 3e0d 0a20  ="loginForm">.. 
+000000e0: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+000000f0: 733d 226d 622d 3322 3e0d 0a20 2020 2020  s="mb-3">..     
+00000100: 2020 2020 2020 203c 6c61 6265 6c20 666f         <label fo
+00000110: 723d 2275 7365 726e 616d 6522 2063 6c61  r="username" cla
+00000120: 7373 3d22 666f 726d 2d6c 6162 656c 223e  ss="form-label">
+00000130: d09b d0be d0b3 d0b8 d0bd 3c2f 6c61 6265  ..........</labe
+00000140: 6c3e 0d0a 2020 2020 2020 2020 2020 2020  l>..            
+00000150: 3c69 6e70 7574 2074 7970 653d 2274 6578  <input type="tex
+00000160: 7422 2063 6c61 7373 3d22 666f 726d 2d63  t" class="form-c
+00000170: 6f6e 7472 6f6c 2220 6964 3d22 7573 6572  ontrol" id="user
+00000180: 6e61 6d65 2220 6e61 6d65 3d22 7573 6572  name" name="user
+00000190: 6e61 6d65 2220 7061 7474 6572 6e3d 225b  name" pattern="[
+000001a0: 412d 5a61 2d7a 5d2b 2220 7469 746c 653d  A-Za-z]+" title=
+000001b0: 22d0 9bd0 bed0 b3d0 b8d0 bd20 d0b4 d0be  ".......... ....
+000001c0: d0bb d0b6 d0b5 d0bd 20d1 81d0 bed0 b4d0  ........ .......
+000001d0: b5d1 80d0 b6d0 b0d1 82d1 8c20 d182 d0be  ........... ....
+000001e0: d0bb d18c d0ba d0be 20d0 b0d0 bdd0 b3d0  ........ .......
+000001f0: bbd0 b8d0 b9d1 81d0 bad0 b8d0 b520 d0b1  ............. ..
+00000200: d183 d0ba d0b2 d18b 2e22 2072 6571 7569  ........." requi
+00000210: 7265 643e 0d0a 2020 2020 2020 2020 3c2f  red>..        </
+00000220: 6469 763e 0d0a 2020 2020 2020 2020 3c64  div>..        <d
+00000230: 6976 2063 6c61 7373 3d22 6d62 2d33 223e  iv class="mb-3">
+00000240: 0d0a 2020 2020 2020 2020 2020 2020 3c6c  ..            <l
+00000250: 6162 656c 2066 6f72 3d22 7061 7373 776f  abel for="passwo
+00000260: 7264 2220 636c 6173 733d 2266 6f72 6d2d  rd" class="form-
+00000270: 6c61 6265 6c22 3ed0 9fd0 b0d1 80d0 bed0  label">.........
+00000280: bbd1 8c3c 2f6c 6162 656c 3e0d 0a20 2020  ...</label>..   
+00000290: 2020 2020 2020 2020 203c 696e 7075 7420           <input 
+000002a0: 7479 7065 3d22 7061 7373 776f 7264 2220  type="password" 
+000002b0: 636c 6173 733d 2266 6f72 6d2d 636f 6e74  class="form-cont
+000002c0: 726f 6c22 2069 643d 2270 6173 7377 6f72  rol" id="passwor
+000002d0: 6422 206e 616d 653d 2270 6173 7377 6f72  d" name="passwor
+000002e0: 6422 2070 6174 7465 726e 3d22 283f 3d2e  d" pattern="(?=.
+000002f0: 2a5b 2140 2324 255e 262a 5d29 283f 3d2e  *[!@#$%^&*])(?=.
+00000300: 2a5b 302d 395d 292e 7b38 2c7d 2220 7469  *[0-9]).{8,}" ti
+00000310: 746c 653d 22d0 9fd0 b0d1 80d0 bed0 bbd1  tle="...........
+00000320: 8c20 d0b4 d0be d0bb d0b6 d0b5 d0bd 20d1  . ............ .
+00000330: 81d0 bed0 b4d0 b5d1 80d0 b6d0 b0d1 82d1  ................
+00000340: 8c20 d0bc d0b8 d0bd d0b8 d0bc d183 d0bc  . ..............
+00000350: 2038 20d1 81d0 b8d0 bcd0 b2d0 bed0 bbd0   8 .............
+00000360: bed0 b220 d0b8 2031 20d1 81d0 bfd0 b5d1  ... .. 1 .......
+00000370: 86d0 b8d0 b0d0 bbd1 8cd0 bdd1 8bd0 b920  ............... 
+00000380: d181 d0b8 d0bc d0b2 d0be d0bb 2e22 2072  ............." r
+00000390: 6571 7569 7265 643e 0d0a 2020 2020 2020  equired>..      
+000003a0: 2020 3c2f 6469 763e 0d0a 2020 2020 2020    </div>..      
+000003b0: 2020 3c62 7574 746f 6e20 7479 7065 3d22    <button type="
+000003c0: 7375 626d 6974 2220 636c 6173 733d 2262  submit" class="b
+000003d0: 746e 2062 746e 2d70 7269 6d61 7279 223e  tn btn-primary">
+000003e0: d092 d0be d0b9 d182 d0b8 3c2f 6275 7474  ..........</butt
+000003f0: 6f6e 3e0d 0a20 2020 203c 2f66 6f72 6d3e  on>..    </form>
+00000400: 0d0a 3c2f 6469 763e 0d0a 0d0a 3c73 6372  ..</div>....<scr
+00000410: 6970 743e 0d0a 646f 6375 6d65 6e74 2e67  ipt>..document.g
+00000420: 6574 456c 656d 656e 7442 7949 6428 276c  etElementById('l
+00000430: 6f67 696e 466f 726d 2729 2e61 6464 4576  oginForm').addEv
+00000440: 656e 744c 6973 7465 6e65 7228 2773 7562  entListener('sub
+00000450: 6d69 7427 2c20 6675 6e63 7469 6f6e 2865  mit', function(e
+00000460: 7665 6e74 2920 7b0d 0a20 2020 2063 6f6e  vent) {..    con
+00000470: 7374 2075 7365 726e 616d 6520 3d20 646f  st username = do
+00000480: 6375 6d65 6e74 2e67 6574 456c 656d 656e  cument.getElemen
+00000490: 7442 7949 6428 2775 7365 726e 616d 6527  tById('username'
+000004a0: 292e 7661 6c75 653b 0d0a 2020 2020 636f  ).value;..    co
+000004b0: 6e73 7420 7061 7373 776f 7264 203d 2064  nst password = d
+000004c0: 6f63 756d 656e 742e 6765 7445 6c65 6d65  ocument.getEleme
+000004d0: 6e74 4279 4964 2827 7061 7373 776f 7264  ntById('password
+000004e0: 2729 2e76 616c 7565 3b0d 0a0d 0a20 2020  ').value;....   
+000004f0: 2063 6f6e 7374 2075 7365 726e 616d 6550   const usernameP
+00000500: 6174 7465 726e 203d 202f 5e5b 412d 5a61  attern = /^[A-Za
+00000510: 2d7a 5d2b 242f 3b0d 0a20 2020 2063 6f6e  -z]+$/;..    con
+00000520: 7374 2070 6173 7377 6f72 6450 6174 7465  st passwordPatte
+00000530: 726e 203d 202f 5e28 3f3d 2e2a 5b21 4023  rn = /^(?=.*[!@#
+00000540: 2425 5e26 2a5d 2928 3f3d 2e2a 5b30 2d39  $%^&*])(?=.*[0-9
+00000550: 5d29 2e7b 382c 7d24 2f3b 0d0a 0d0a 2020  ]).{8,}$/;....  
+00000560: 2020 6966 2028 2175 7365 726e 616d 6550    if (!usernameP
+00000570: 6174 7465 726e 2e74 6573 7428 7573 6572  attern.test(user
+00000580: 6e61 6d65 2929 207b 0d0a 2020 2020 2020  name)) {..      
+00000590: 2020 616c 6572 7428 27d0 9bd0 bed0 b3d0    alert('.......
+000005a0: b8d0 bd20 d0b4 d0be d0bb d0b6 d0b5 d0bd  ... ............
+000005b0: 20d1 81d0 bed0 b4d0 b5d1 80d0 b6d0 b0d1   ...............
+000005c0: 82d1 8c20 d182 d0be d0bb d18c d0ba d0be  ... ............
+000005d0: 20d0 b0d0 bdd0 b3d0 bbd0 b8d0 b9d1 81d0   ...............
+000005e0: bad0 b8d0 b520 d0b1 d183 d0ba d0b2 d18b  ..... ..........
+000005f0: 2e27 293b 0d0a 2020 2020 2020 2020 6576  .');..        ev
+00000600: 656e 742e 7072 6576 656e 7444 6566 6175  ent.preventDefau
+00000610: 6c74 2829 3b0d 0a20 2020 207d 2065 6c73  lt();..    } els
+00000620: 6520 6966 2028 2170 6173 7377 6f72 6450  e if (!passwordP
+00000630: 6174 7465 726e 2e74 6573 7428 7061 7373  attern.test(pass
+00000640: 776f 7264 2929 207b 0d0a 2020 2020 2020  word)) {..      
+00000650: 2020 616c 6572 7428 27d0 9fd0 b0d1 80d0    alert('.......
+00000660: bed0 bbd1 8c20 d0b4 d0be d0bb d0b6 d0b5  ..... ..........
+00000670: d0bd 20d1 81d0 bed0 b4d0 b5d1 80d0 b6d0  .. .............
+00000680: b0d1 82d1 8c20 d0bc d0b8 d0bd d0b8 d0bc  ..... ..........
+00000690: d183 d0bc 2038 20d1 81d0 b8d0 bcd0 b2d0  .... 8 .........
+000006a0: bed0 bbd0 bed0 b220 d0b8 2031 20d1 81d0  ....... .. 1 ...
+000006b0: bfd0 b5d1 86d0 b8d0 b0d0 bbd1 8cd0 bdd1  ................
+000006c0: 8bd0 b920 d181 d0b8 d0bc d0b2 d0be d0bb  ... ............
+000006d0: 2e27 293b 0d0a 2020 2020 2020 2020 6576  .');..        ev
+000006e0: 656e 742e 7072 6576 656e 7444 6566 6175  ent.preventDefau
+000006f0: 6c74 2829 3b0d 0a20 2020 207d 0d0a 7d29  lt();..    }..})
+00000700: 3b0d 0a3c 2f73 6372 6970 743e 0d0a 7b25  ;..</script>..{%
+00000710: 2065 6e64 626c 6f63 6b20 257d 0d0a        endblock %}..
```

### Comparing `flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/flask-multidb/alembic.ini.mako` & `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask-multidb/alembic.ini.mako`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/flask-multidb/env.py` & `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask-multidb/env.py`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/templates/flask-multidb/script.py.mako` & `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/templates/flask-multidb/script.py.mako`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds/tools.py` & `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds/tools.py`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds.egg-info/PKG-INFO` & `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask_bootstrap_module_extendeds
-Version: 5.1.3
+Version: 5.1.4
 Summary: Flask bootstrap-library EXTENDED
 Home-page: https://github.com/yourusername/my_library
 Author: Dex
 Author-email: censored@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `flask_bootstrap_module_extendeds-5.1.3/flask_bootstrap_module_extendeds.egg-info/SOURCES.txt` & `flask_bootstrap_module_extendeds-5.1.4/flask_bootstrap_module_extendeds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flask_bootstrap_module_extendeds-5.1.3/setup.py` & `flask_bootstrap_module_extendeds-5.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="flask_bootstrap_module_extendeds",
-    version="5.1.3",
+    version="5.1.4",
     author="Dex",
     author_email="censored@gmail.com",
     description="Flask bootstrap-library EXTENDED",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/yourusername/my_library",
     packages=find_packages(),
```

