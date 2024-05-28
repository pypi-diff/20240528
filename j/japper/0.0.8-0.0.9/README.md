# Comparing `tmp/japper-0.0.8.tar.gz` & `tmp/japper-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "japper-0.0.8.tar", last modified: Tue Mar 19 21:48:24 2024, max compression
+gzip compressed data, was "japper-0.0.9.tar", last modified: Wed Mar 20 05:01:54 2024, max compression
```

## Comparing `japper-0.0.8.tar` & `japper-0.0.9.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 yirugi     (501) staff       (20)        0 2024-03-19 21:48:24.124653 japper-0.0.8/
--rw-r--r--   0 yirugi     (501) staff       (20)     5232 2024-03-19 21:48:24.124016 japper-0.0.8/PKG-INFO
--rw-r--r--   0 yirugi     (501) staff       (20)     4599 2024-02-19 07:14:37.000000 japper-0.0.8/README.md
--rw-r--r--   0 yirugi     (501) staff       (20)     1327 2024-03-19 21:48:09.000000 japper-0.0.8/pyproject.toml
--rw-r--r--   0 yirugi     (501) staff       (20)       38 2024-03-19 21:48:24.124799 japper-0.0.8/setup.cfg
-drwxr-xr-x   0 yirugi     (501) staff       (20)        0 2024-03-19 21:48:24.096363 japper-0.0.8/src/
-drwxr-xr-x   0 yirugi     (501) staff       (20)        0 2024-03-19 21:48:24.102300 japper-0.0.8/src/japper/
--rw-r--r--   0 yirugi     (501) staff       (20)      373 2024-03-12 04:38:28.000000 japper-0.0.8/src/japper/__init__.py
--rw-r--r--   0 yirugi     (501) staff       (20)     1656 2024-02-17 08:05:35.000000 japper-0.0.8/src/japper/app_main_view.py
--rw-r--r--   0 yirugi     (501) staff       (20)     1229 2024-03-18 23:54:57.000000 japper-0.0.8/src/japper/appmode.html
--rw-r--r--   0 yirugi     (501) staff       (20)      190 2024-03-12 04:38:28.000000 japper-0.0.8/src/japper/base_controller.py
--rw-r--r--   0 yirugi     (501) staff       (20)      175 2024-02-17 03:15:52.000000 japper-0.0.8/src/japper/base_view.py
--rw-r--r--   0 yirugi     (501) staff       (20)      439 2024-02-17 08:47:58.000000 japper-0.0.8/src/japper/config.py
--rw-r--r--   0 yirugi     (501) staff       (20)     5192 2024-03-12 18:36:06.000000 japper-0.0.8/src/japper/debug.py
--rw-r--r--   0 yirugi     (501) staff       (20)     3920 2024-03-18 23:54:57.000000 japper-0.0.8/src/japper/global.html
--rw-r--r--   0 yirugi     (501) staff       (20)     4426 2024-02-21 07:21:30.000000 japper-0.0.8/src/japper/japper_app_main.py
--rw-r--r--   0 yirugi     (501) staff       (20)      465 2024-03-12 04:38:44.000000 japper-0.0.8/src/japper/page.py
--rwx------   0 yirugi     (501) staff       (20)     4862 2024-03-12 01:23:47.000000 japper-0.0.8/src/japper/utils.py
--rw-r--r--   0 yirugi     (501) staff       (20)     3116 2024-02-15 23:00:20.000000 japper-0.0.8/src/japper/vue_widget_logger.py
-drwxr-xr-x   0 yirugi     (501) staff       (20)        0 2024-03-19 21:48:24.107091 japper-0.0.8/src/japper/widgets/
--rw-r--r--   0 yirugi     (501) staff       (20)      157 2024-02-17 08:38:09.000000 japper-0.0.8/src/japper/widgets/__init__.py
--rwx------   0 yirugi     (501) staff       (20)     2283 2023-03-11 14:29:06.000000 japper-0.0.8/src/japper/widgets/fileupload.py
--rw-r--r--   0 yirugi     (501) staff       (20)      794 2024-03-18 19:52:57.000000 japper-0.0.8/src/japper/widgets/loading_dialog.py
--rwx------   0 yirugi     (501) staff       (20)     5306 2024-02-17 09:14:10.000000 japper-0.0.8/src/japper/widgets/navigation_menu.py
--rw-r--r--   0 yirugi     (501) staff       (20)     1013 2023-09-18 15:38:36.000000 japper-0.0.8/src/japper/widgets/toast_alert.py
-drwxr-xr-x   0 yirugi     (501) staff       (20)        0 2024-03-19 21:48:24.122596 japper-0.0.8/src/japper.egg-info/
--rw-r--r--   0 yirugi     (501) staff       (20)     5232 2024-03-19 21:48:24.000000 japper-0.0.8/src/japper.egg-info/PKG-INFO
--rw-r--r--   0 yirugi     (501) staff       (20)     2201 2024-03-19 21:48:24.000000 japper-0.0.8/src/japper.egg-info/SOURCES.txt
--rw-r--r--   0 yirugi     (501) staff       (20)        1 2024-03-19 21:48:24.000000 japper-0.0.8/src/japper.egg-info/dependency_links.txt
--rw-r--r--   0 yirugi     (501) staff       (20)       57 2024-03-19 21:48:24.000000 japper-0.0.8/src/japper.egg-info/entry_points.txt
--rw-r--r--   0 yirugi     (501) staff       (20)      100 2024-03-19 21:48:24.000000 japper-0.0.8/src/japper.egg-info/requires.txt
--rw-r--r--   0 yirugi     (501) staff       (20)       23 2024-03-19 21:48:24.000000 japper-0.0.8/src/japper.egg-info/top_level.txt
-drwxr-xr-x   0 yirugi     (501) staff       (20)        0 2024-03-19 21:48:24.110857 japper-0.0.8/src/japper_devtools/
--rw-r--r--   0 yirugi     (501) staff       (20)       27 2024-03-19 20:55:40.000000 japper-0.0.8/src/japper_devtools/__init__.py
--rw-r--r--   0 yirugi     (501) staff       (20)     8587 2024-03-19 06:40:06.000000 japper-0.0.8/src/japper_devtools/__main__.py
--rw-r--r--   0 yirugi     (501) staff       (20)     8180 2024-03-12 19:59:16.000000 japper-0.0.8/src/japper_devtools/main.py
--rwxr-xr-x   0 yirugi     (501) staff       (20)      243 2024-03-15 06:43:14.000000 japper-0.0.8/src/japper_devtools/parallel_cmd.sh
--rw-r--r--   0 yirugi     (501) staff       (20)     7446 2024-03-19 21:46:20.000000 japper-0.0.8/src/japper_devtools/project_init.py
-drwxr-xr-x   0 yirugi     (501) staff       (20)        0 2024-03-19 21:48:24.111695 japper-0.0.8/src/japper_devtools/static/
-drwxr-xr-x   0 yirugi     (501) staff       (20)        0 2024-03-19 21:48:24.096717 japper-0.0.8/src/japper_devtools/static/app/
-drwxr-xr-x   0 yirugi     (501) staff       (20)        0 2024-03-19 21:48:24.113100 japper-0.0.8/src/japper_devtools/static/app/assets/
--rw-r--r--   0 yirugi     (501) staff       (20)      111 2024-02-17 00:13:20.000000 japper-0.0.8/src/japper_devtools/static/app/assets/custom.html
--rw-r--r--   0 yirugi     (501) staff       (20)     1254 2024-02-06 21:19:58.000000 japper-0.0.8/src/japper_devtools/static/app/assets/icon.png
--rw-r--r--   0 yirugi     (501) staff       (20)    48362 2024-02-06 21:18:55.000000 japper-0.0.8/src/japper_devtools/static/app/assets/logo.png
-drwxr-xr-x   0 yirugi     (501) staff       (20)        0 2024-03-19 21:48:24.097185 japper-0.0.8/src/japper_devtools/static/container/
-drwxr-xr-x   0 yirugi     (501) staff       (20)        0 2024-03-19 21:48:24.114066 japper-0.0.8/src/japper_devtools/static/container/appmode/
--rwxr--r--   0 yirugi     (501) staff       (20)      622 2024-03-19 20:45:11.000000 japper-0.0.8/src/japper_devtools/static/container/appmode/Dockerfile
--rw-r--r--   0 yirugi     (501) staff       (20)      103 2024-03-19 20:45:36.000000 japper-0.0.8/src/japper_devtools/static/container/appmode/start.sh
-drwxr-xr-x   0 yirugi     (501) staff       (20)        0 2024-03-19 21:48:24.115063 japper-0.0.8/src/japper_devtools/static/container/dev/
--rwx------   0 yirugi     (501) staff       (20)      379 2024-03-19 03:53:56.000000 japper-0.0.8/src/japper_devtools/static/container/dev/Dockerfile
--rw-r--r--   0 yirugi     (501) staff       (20)      274 2024-03-19 04:29:15.000000 japper-0.0.8/src/japper_devtools/static/container/dev/start.sh
-drwxr-xr-x   0 yirugi     (501) staff       (20)        0 2024-03-19 21:48:24.115923 japper-0.0.8/src/japper_devtools/static/container/prod/
--rw-r--r--   0 yirugi     (501) staff       (20)      480 2024-03-19 03:53:51.000000 japper-0.0.8/src/japper_devtools/static/container/prod/Dockerfile
--rw-r--r--   0 yirugi     (501) staff       (20)      583 2024-03-19 04:29:20.000000 japper-0.0.8/src/japper_devtools/static/container/prod/start.sh
--rw-r--r--   0 yirugi     (501) staff       (20)      922 2024-02-06 02:57:05.000000 japper-0.0.8/src/japper_devtools/static/gitignore
-drwxr-xr-x   0 yirugi     (501) staff       (20)        0 2024-03-19 21:48:24.122023 japper-0.0.8/src/japper_devtools/templates/
--rw-r--r--   0 yirugi     (501) staff       (20)      298 2024-02-17 03:35:13.000000 japper-0.0.8/src/japper_devtools/templates/README.md.jinja2
--rw-r--r--   0 yirugi     (501) staff       (20)      648 2024-03-12 05:42:00.000000 japper-0.0.8/src/japper_devtools/templates/app.app_main.py.jinja2
--rw-r--r--   0 yirugi     (501) staff       (20)      145 2024-02-17 00:16:04.000000 japper-0.0.8/src/japper_devtools/templates/app.commons.__init__.py.jinja2
--rw-r--r--   0 yirugi     (501) staff       (20)      344 2024-02-17 07:05:34.000000 japper-0.0.8/src/japper_devtools/templates/app.commons.config.py.jinja2
--rw-r--r--   0 yirugi     (501) staff       (20)      665 2024-03-12 05:44:13.000000 japper-0.0.8/src/japper_devtools/templates/app.controllers.__name__.py.jinja2
--rw-r--r--   0 yirugi     (501) staff       (20)      692 2024-03-12 05:44:56.000000 japper-0.0.8/src/japper_devtools/templates/app.controllers.home.py.jinja2
--rw-r--r--   0 yirugi     (501) staff       (20)      671 2024-03-19 01:29:01.000000 japper-0.0.8/src/japper_devtools/templates/app.ipynb.jinja2
--rw-r--r--   0 yirugi     (501) staff       (20)      211 2024-02-17 09:12:32.000000 japper-0.0.8/src/japper_devtools/templates/app.models.__name__.py.jinja2
--rw-r--r--   0 yirugi     (501) staff       (20)      330 2024-02-17 03:43:03.000000 japper-0.0.8/src/japper_devtools/templates/app.models.home.py.jinja2
--rw-r--r--   0 yirugi     (501) staff       (20)      464 2024-03-12 05:45:17.000000 japper-0.0.8/src/japper_devtools/templates/app.views.__name__.py.jinja2
--rw-r--r--   0 yirugi     (501) staff       (20)     1644 2024-02-17 08:36:19.000000 japper-0.0.8/src/japper_devtools/templates/app.views.home.py.jinja2
--rw-r--r--   0 yirugi     (501) staff       (20)      600 2024-03-19 06:21:41.000000 japper-0.0.8/src/japper_devtools/templates/container.__name__.docker-compose__name__.yml.jinja2
--rw-r--r--   0 yirugi     (501) staff       (20)      171 2024-03-19 21:47:34.000000 japper-0.0.8/src/japper_devtools/templates/environment.yml.jinja2
--rw-r--r--   0 yirugi     (501) staff       (20)      269 2024-03-19 01:34:04.000000 japper-0.0.8/src/japper_devtools/templates/middleware.invoke.jinja2
--rw-r--r--   0 yirugi     (501) staff       (20)     9897 2024-03-19 21:48:00.000000 japper-0.0.8/src/japper_devtools/utils.py
+drwxr-xr-x   0 yirugi     (501) staff       (20)        0 2024-03-20 05:01:54.266033 japper-0.0.9/
+-rw-r--r--   0 yirugi     (501) staff       (20)     5232 2024-03-20 05:01:54.265439 japper-0.0.9/PKG-INFO
+-rw-r--r--   0 yirugi     (501) staff       (20)     4599 2024-02-19 07:14:37.000000 japper-0.0.9/README.md
+-rw-r--r--   0 yirugi     (501) staff       (20)     1327 2024-03-20 05:01:21.000000 japper-0.0.9/pyproject.toml
+-rw-r--r--   0 yirugi     (501) staff       (20)       38 2024-03-20 05:01:54.266151 japper-0.0.9/setup.cfg
+drwxr-xr-x   0 yirugi     (501) staff       (20)        0 2024-03-20 05:01:54.241416 japper-0.0.9/src/
+drwxr-xr-x   0 yirugi     (501) staff       (20)        0 2024-03-20 05:01:54.247163 japper-0.0.9/src/japper/
+-rw-r--r--   0 yirugi     (501) staff       (20)      373 2024-03-12 04:38:28.000000 japper-0.0.9/src/japper/__init__.py
+-rw-r--r--   0 yirugi     (501) staff       (20)     1656 2024-02-17 08:05:35.000000 japper-0.0.9/src/japper/app_main_view.py
+-rw-r--r--   0 yirugi     (501) staff       (20)     1204 2024-03-20 05:00:14.000000 japper-0.0.9/src/japper/appmode.html
+-rw-r--r--   0 yirugi     (501) staff       (20)      190 2024-03-12 04:38:28.000000 japper-0.0.9/src/japper/base_controller.py
+-rw-r--r--   0 yirugi     (501) staff       (20)      175 2024-02-17 03:15:52.000000 japper-0.0.9/src/japper/base_view.py
+-rw-r--r--   0 yirugi     (501) staff       (20)      439 2024-02-17 08:47:58.000000 japper-0.0.9/src/japper/config.py
+-rw-r--r--   0 yirugi     (501) staff       (20)     5288 2024-03-20 04:54:20.000000 japper-0.0.9/src/japper/debug.py
+-rw-r--r--   0 yirugi     (501) staff       (20)     3919 2024-03-20 04:56:27.000000 japper-0.0.9/src/japper/global.html
+-rw-r--r--   0 yirugi     (501) staff       (20)     4660 2024-03-20 01:45:41.000000 japper-0.0.9/src/japper/japper_app_main.py
+-rw-r--r--   0 yirugi     (501) staff       (20)      465 2024-03-12 04:38:44.000000 japper-0.0.9/src/japper/page.py
+-rwx------   0 yirugi     (501) staff       (20)     4862 2024-03-12 01:23:47.000000 japper-0.0.9/src/japper/utils.py
+-rw-r--r--   0 yirugi     (501) staff       (20)     3116 2024-02-15 23:00:20.000000 japper-0.0.9/src/japper/vue_widget_logger.py
+drwxr-xr-x   0 yirugi     (501) staff       (20)        0 2024-03-20 05:01:54.250940 japper-0.0.9/src/japper/widgets/
+-rw-r--r--   0 yirugi     (501) staff       (20)      157 2024-02-17 08:38:09.000000 japper-0.0.9/src/japper/widgets/__init__.py
+-rwx------   0 yirugi     (501) staff       (20)     2283 2023-03-11 14:29:06.000000 japper-0.0.9/src/japper/widgets/fileupload.py
+-rw-r--r--   0 yirugi     (501) staff       (20)      794 2024-03-18 19:52:57.000000 japper-0.0.9/src/japper/widgets/loading_dialog.py
+-rwx------   0 yirugi     (501) staff       (20)     5306 2024-02-17 09:14:10.000000 japper-0.0.9/src/japper/widgets/navigation_menu.py
+-rw-r--r--   0 yirugi     (501) staff       (20)     1013 2023-09-18 15:38:36.000000 japper-0.0.9/src/japper/widgets/toast_alert.py
+drwxr-xr-x   0 yirugi     (501) staff       (20)        0 2024-03-20 05:01:54.264203 japper-0.0.9/src/japper.egg-info/
+-rw-r--r--   0 yirugi     (501) staff       (20)     5232 2024-03-20 05:01:54.000000 japper-0.0.9/src/japper.egg-info/PKG-INFO
+-rw-r--r--   0 yirugi     (501) staff       (20)     2201 2024-03-20 05:01:54.000000 japper-0.0.9/src/japper.egg-info/SOURCES.txt
+-rw-r--r--   0 yirugi     (501) staff       (20)        1 2024-03-20 05:01:54.000000 japper-0.0.9/src/japper.egg-info/dependency_links.txt
+-rw-r--r--   0 yirugi     (501) staff       (20)       57 2024-03-20 05:01:54.000000 japper-0.0.9/src/japper.egg-info/entry_points.txt
+-rw-r--r--   0 yirugi     (501) staff       (20)      100 2024-03-20 05:01:54.000000 japper-0.0.9/src/japper.egg-info/requires.txt
+-rw-r--r--   0 yirugi     (501) staff       (20)       23 2024-03-20 05:01:54.000000 japper-0.0.9/src/japper.egg-info/top_level.txt
+drwxr-xr-x   0 yirugi     (501) staff       (20)        0 2024-03-20 05:01:54.253735 japper-0.0.9/src/japper_devtools/
+-rw-r--r--   0 yirugi     (501) staff       (20)       27 2024-03-19 20:55:40.000000 japper-0.0.9/src/japper_devtools/__init__.py
+-rw-r--r--   0 yirugi     (501) staff       (20)     8377 2024-03-20 04:24:49.000000 japper-0.0.9/src/japper_devtools/__main__.py
+-rw-r--r--   0 yirugi     (501) staff       (20)     8180 2024-03-12 19:59:16.000000 japper-0.0.9/src/japper_devtools/main.py
+-rwxr-xr-x   0 yirugi     (501) staff       (20)      243 2024-03-15 06:43:14.000000 japper-0.0.9/src/japper_devtools/parallel_cmd.sh
+-rw-r--r--   0 yirugi     (501) staff       (20)     7471 2024-03-20 04:34:26.000000 japper-0.0.9/src/japper_devtools/project_init.py
+drwxr-xr-x   0 yirugi     (501) staff       (20)        0 2024-03-20 05:01:54.254223 japper-0.0.9/src/japper_devtools/static/
+drwxr-xr-x   0 yirugi     (501) staff       (20)        0 2024-03-20 05:01:54.241790 japper-0.0.9/src/japper_devtools/static/app/
+drwxr-xr-x   0 yirugi     (501) staff       (20)        0 2024-03-20 05:01:54.255443 japper-0.0.9/src/japper_devtools/static/app/assets/
+-rw-r--r--   0 yirugi     (501) staff       (20)      111 2024-02-17 00:13:20.000000 japper-0.0.9/src/japper_devtools/static/app/assets/custom.html
+-rw-r--r--   0 yirugi     (501) staff       (20)     1254 2024-02-06 21:19:58.000000 japper-0.0.9/src/japper_devtools/static/app/assets/icon.png
+-rw-r--r--   0 yirugi     (501) staff       (20)    48362 2024-02-06 21:18:55.000000 japper-0.0.9/src/japper_devtools/static/app/assets/logo.png
+drwxr-xr-x   0 yirugi     (501) staff       (20)        0 2024-03-20 05:01:54.242288 japper-0.0.9/src/japper_devtools/static/container/
+drwxr-xr-x   0 yirugi     (501) staff       (20)        0 2024-03-20 05:01:54.256353 japper-0.0.9/src/japper_devtools/static/container/appmode/
+-rwxr--r--   0 yirugi     (501) staff       (20)      626 2024-03-20 01:24:25.000000 japper-0.0.9/src/japper_devtools/static/container/appmode/Dockerfile
+-rw-r--r--   0 yirugi     (501) staff       (20)      128 2024-03-20 02:27:02.000000 japper-0.0.9/src/japper_devtools/static/container/appmode/start.sh
+drwxr-xr-x   0 yirugi     (501) staff       (20)        0 2024-03-20 05:01:54.257101 japper-0.0.9/src/japper_devtools/static/container/dev/
+-rwx------   0 yirugi     (501) staff       (20)      379 2024-03-19 03:53:56.000000 japper-0.0.9/src/japper_devtools/static/container/dev/Dockerfile
+-rw-r--r--   0 yirugi     (501) staff       (20)      274 2024-03-19 04:29:15.000000 japper-0.0.9/src/japper_devtools/static/container/dev/start.sh
+drwxr-xr-x   0 yirugi     (501) staff       (20)        0 2024-03-20 05:01:54.257888 japper-0.0.9/src/japper_devtools/static/container/prod/
+-rw-r--r--   0 yirugi     (501) staff       (20)      480 2024-03-19 03:53:51.000000 japper-0.0.9/src/japper_devtools/static/container/prod/Dockerfile
+-rw-r--r--   0 yirugi     (501) staff       (20)      583 2024-03-19 04:29:20.000000 japper-0.0.9/src/japper_devtools/static/container/prod/start.sh
+-rw-r--r--   0 yirugi     (501) staff       (20)      922 2024-02-06 02:57:05.000000 japper-0.0.9/src/japper_devtools/static/gitignore
+drwxr-xr-x   0 yirugi     (501) staff       (20)        0 2024-03-20 05:01:54.263721 japper-0.0.9/src/japper_devtools/templates/
+-rw-r--r--   0 yirugi     (501) staff       (20)      298 2024-02-17 03:35:13.000000 japper-0.0.9/src/japper_devtools/templates/README.md.jinja2
+-rw-r--r--   0 yirugi     (501) staff       (20)      696 2024-03-20 01:47:06.000000 japper-0.0.9/src/japper_devtools/templates/app.app_main.py.jinja2
+-rw-r--r--   0 yirugi     (501) staff       (20)      145 2024-02-17 00:16:04.000000 japper-0.0.9/src/japper_devtools/templates/app.commons.__init__.py.jinja2
+-rw-r--r--   0 yirugi     (501) staff       (20)      344 2024-02-17 07:05:34.000000 japper-0.0.9/src/japper_devtools/templates/app.commons.config.py.jinja2
+-rw-r--r--   0 yirugi     (501) staff       (20)      665 2024-03-12 05:44:13.000000 japper-0.0.9/src/japper_devtools/templates/app.controllers.__name__.py.jinja2
+-rw-r--r--   0 yirugi     (501) staff       (20)      692 2024-03-12 05:44:56.000000 japper-0.0.9/src/japper_devtools/templates/app.controllers.home.py.jinja2
+-rw-r--r--   0 yirugi     (501) staff       (20)      671 2024-03-19 01:29:01.000000 japper-0.0.9/src/japper_devtools/templates/app.ipynb.jinja2
+-rw-r--r--   0 yirugi     (501) staff       (20)      211 2024-02-17 09:12:32.000000 japper-0.0.9/src/japper_devtools/templates/app.models.__name__.py.jinja2
+-rw-r--r--   0 yirugi     (501) staff       (20)      330 2024-02-17 03:43:03.000000 japper-0.0.9/src/japper_devtools/templates/app.models.home.py.jinja2
+-rw-r--r--   0 yirugi     (501) staff       (20)      464 2024-03-12 05:45:17.000000 japper-0.0.9/src/japper_devtools/templates/app.views.__name__.py.jinja2
+-rw-r--r--   0 yirugi     (501) staff       (20)     1644 2024-02-17 08:36:19.000000 japper-0.0.9/src/japper_devtools/templates/app.views.home.py.jinja2
+-rw-r--r--   0 yirugi     (501) staff       (20)      603 2024-03-20 03:00:04.000000 japper-0.0.9/src/japper_devtools/templates/container.__name__.docker-compose__name__.yml.jinja2
+-rw-r--r--   0 yirugi     (501) staff       (20)      171 2024-03-19 21:47:34.000000 japper-0.0.9/src/japper_devtools/templates/environment.yml.jinja2
+-rw-r--r--   0 yirugi     (501) staff       (20)      269 2024-03-19 01:34:04.000000 japper-0.0.9/src/japper_devtools/templates/middleware.invoke.jinja2
+-rw-r--r--   0 yirugi     (501) staff       (20)    12182 2024-03-20 05:01:34.000000 japper-0.0.9/src/japper_devtools/utils.py
```

### Comparing `japper-0.0.8/PKG-INFO` & `japper-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: japper
-Version: 0.0.8
+Version: 0.0.9
 Summary: Japper
 Author-email: "Kim, I Luk" <yirugi@gmail.com>
 License: MIT License
 Keywords: japper,Jupyter,ipyvuetify,voila
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
```

### Comparing `japper-0.0.8/README.md` & `japper-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `japper-0.0.8/pyproject.toml` & `japper-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "japper"
-version = "0.0.8"
+version = "0.0.9"
 dependencies = [
     "setuptools",
     "pdoc3",
     "ipyvuetify",
     "ipywidgets",
     "ipykernel",
     "jinja2",
```

### Comparing `japper-0.0.8/src/japper/app_main_view.py` & `japper-0.0.9/src/japper/app_main_view.py`

 * *Files identical despite different names*

### Comparing `japper-0.0.8/src/japper/appmode.html` & `japper-0.0.9/src/japper/appmode.html`

 * *Files 8% similar despite different names*

```diff
@@ -40,15 +40,14 @@
     body.appmode .container {
         width: 100%;
     }
 
     body.appmode div#notebook {
         padding-top: 0;
         padding-bottom: 0;
-        font-size: 1rem;
     }
 
     body.appmode .end_space {
         display: none;
     }
 
     body.appmode .v-navigation-drawer {
```

### Comparing `japper-0.0.8/src/japper/debug.py` & `japper-0.0.9/src/japper/debug.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,44 +29,46 @@
         self.debug_view_box = self.create_debug_view_box()
 
         self.debug_view_inited = True
         global debug_output
         debug_output = self.debug_output
 
     def display_debug_view(self):
+        # jupyter-widgets-output-area output_wrapper
         display(self.debug_view_box)
         run_js_with_wait("""
                             document.body.appendChild(document.querySelector('.debug-view'));
-                            document.querySelector('.debug-view .widget-output').style.display = 'none';
+                            document.querySelector('.debug-view .debug-output').style.display = 'none';
                         """, '.debug-view')
 
     def hide_debug_view(self, _=None):
         run_js("""
             document.querySelector('.debug-view').style.height = '50px';
-            document.querySelector('.debug-view .widget-output').style.display = 'none';
+            document.querySelector('.debug-view .debug-output').style.display = 'none';
             let btns = document.querySelectorAll('.debug-view button');
             btns[0].style.display = 'block';
             btns[1].style.display = 'none';
             btns[2].style.display = 'none';
         """)
 
     def show_debug_view(self, _=None):
         run_js("""
             document.querySelector('.debug-view').style.height = '270px';
-            document.querySelector('.debug-view .widget-output').style.display = 'block';
+            document.querySelector('.debug-view .debug-output').style.display = 'block';
             let btns = document.querySelectorAll('.debug-view button');
             btns[0].style.display = 'none';
             btns[1].style.display = 'block';
             btns[2].style.display = 'block';
         """)
 
     def create_debug_view_box(self):
         if self.debug_view_inited:
             return
         debug_output = ipyw.Output(layout={'width': '100%'})
+        debug_output.add_class('debug-output')
         btn_hide = ipyw.Button(description="HIDE", layout={'width': '80px', 'display': 'none'})
         btn_hide.on_click(self.hide_debug_view)
         btn_clear = ipyw.Button(description="CLEAR", layout={'width': '80px', 'display': 'none'})
         btn_clear.on_click(lambda _: debug_output.clear_output())
 
         btn_show = ipyw.Button(description="SHOW DEBUG PANEL", layout={'width': 'fit-content'})
         btn_show.on_click(self.show_debug_view)
@@ -110,15 +112,15 @@
     if not is_dev():
         return
     out = ' '.join([str(x) for x in msgs])
     with debug_output:
         print(out)
         run_js("""
             setTimeout(()=>{
-                let output_div = document.querySelector('.debug-view .widget-output');
+                let output_div = document.querySelector('.debug-view .debug-output');
                 output_div.scrollTo({top:output_div.scrollHeight, behavior: 'smooth'});
             }, 100);
         """)
 
         if forced_show:
             debug_view.show_debug_view()
```

### Comparing `japper-0.0.8/src/japper/global.html` & `japper-0.0.9/src/japper/global.html`

 * *Files 2% similar despite different names*

```diff
@@ -120,15 +120,15 @@
         background-color: white;
         padding: 10px;
         font-size: 11px;
         border-top: 1px solid grey;
         box-shadow: 0 -1px 1rem 0 rgb(0 0 0 / 25%);
     }
 
-    .debug-view .widget-output {
+    .debug-view .debug-output {
         border: 1px solid grey;
         -webkit-box-shadow: unset;
         box-shadow: unset;
         height: 200px;
         overflow-y: scroll;
     }
```

### Comparing `japper-0.0.8/src/japper/japper_app_main.py` & `japper-0.0.9/src/japper/japper_app_main.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,34 +31,38 @@
     def __init__(self):
         self.app_name = None
         self.nav_menu = None
         self.main_view = None
         self.pages = []
         self.default_page = None
 
-    def init_app(self, app_name: str = 'Japper App', favicon_path: str = None):
+    def init_app(self, app_name: str = 'Japper App', favicon_path: str = None, mygeohub_tool: bool = False):
         """
         Initialize the app
 
         :param app_name: Name of the app
         :param favicon_path: Path to the favicon
+        :param mygeohub_tool: Set this to True if the app is a MyGeoHub tool
         """
         # init_js_output()  # deprecated
         self.main_view = AppMainView()
         self.app_name = app_name
         utils.set_page_title(app_name)
         if favicon_path:
             utils.set_favicon(favicon_path)
 
         self.add_custom_html('app/assets/custom.html')
 
         # if dev mode, show the debug view
         if is_dev():
             debug_view.display_debug_view()
 
+        if mygeohub_tool:
+            self.set_appmode()
+
     def set_navigation_menu(self, mode: str = 'top', logo: str = None, title: str = None, nav_width: str = '230px'):
         """
         Set the navigation menu
 
         :param mode: 'top' or 'side'
         :param logo: Path to the logo
         :param title: Title of the navigation menu
@@ -142,7 +146,10 @@
         """
         utils.set_external_funcs(
             self.main_view.loading_dialog.show_loading,
             self.main_view.loading_dialog.hide_loading,
             self.main_view.toast_alert.alert,
             self.show_page
         )
+
+    def set_appmode(self):
+        utils.inject_html('appmode.html')
```

### Comparing `japper-0.0.8/src/japper/utils.py` & `japper-0.0.9/src/japper/utils.py`

 * *Files identical despite different names*

### Comparing `japper-0.0.8/src/japper/vue_widget_logger.py` & `japper-0.0.9/src/japper/vue_widget_logger.py`

 * *Files identical despite different names*

### Comparing `japper-0.0.8/src/japper/widgets/fileupload.py` & `japper-0.0.9/src/japper/widgets/fileupload.py`

 * *Files identical despite different names*

### Comparing `japper-0.0.8/src/japper/widgets/loading_dialog.py` & `japper-0.0.9/src/japper/widgets/loading_dialog.py`

 * *Files identical despite different names*

### Comparing `japper-0.0.8/src/japper/widgets/navigation_menu.py` & `japper-0.0.9/src/japper/widgets/navigation_menu.py`

 * *Files identical despite different names*

### Comparing `japper-0.0.8/src/japper/widgets/toast_alert.py` & `japper-0.0.9/src/japper/widgets/toast_alert.py`

 * *Files identical despite different names*

### Comparing `japper-0.0.8/src/japper.egg-info/PKG-INFO` & `japper-0.0.9/src/japper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: japper
-Version: 0.0.8
+Version: 0.0.9
 Summary: Japper
 Author-email: "Kim, I Luk" <yirugi@gmail.com>
 License: MIT License
 Keywords: japper,Jupyter,ipyvuetify,voila
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
```

### Comparing `japper-0.0.8/src/japper.egg-info/SOURCES.txt` & `japper-0.0.9/src/japper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `japper-0.0.8/src/japper_devtools/__main__.py` & `japper-0.0.9/src/japper_devtools/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import os
 import subprocess
 import rich_click as click
 from rich.console import Console
-from rich.panel import Panel
 
 console = Console()
 
 from .project_init import init_project_cli
-from .utils import save_config, load_config, build_docker_image, check_cur_conda_env, prompt, confirm, run_command
+from .utils import save_config, load_config, build_docker_image, check_cur_conda_env, prompt, confirm, run_command, \
+    run_japper_app, get_docker_up_cmd
 
 WORKING_DIR = os.getcwd().replace('\\', '/')
 MODULE_DIR = os.path.dirname(os.path.abspath(__file__))
 
 
 def get_config():
     config = load_config()
@@ -33,118 +33,117 @@
     if gui:
         pass
     else:
         init_project_cli(mygeohub=mygeohub)
 
 
 @click.command(help='Run this Japper project')
-@click.argument('mode', type=click.Choice(['dev', 'preview']))
+@click.argument('mode', type=click.Choice(['dev', 'preview', 'prod']))
 @click.option('-v', '--verbose', help="verbose mode", default=False, is_flag=True)
-def run(env, verbose):
+def run(mode, verbose):
     """
     Run the project in a specified environment.
     """
 
-    # todo: handle preview mode in both dev or appmode
-
     config = get_config()
+    run_env = 'docker' if config['dev_env'] == 'docker' else 'local'
+    mygeohub = 'mygeohub' in config
+    is_preview = mode == 'preview'
+
     if config['dev_env'] == 'manual':
-        console.print("The project is set to run in manual mode. Please run the project manually.", style='bold yellow')
+        console.print(
+            "The project is set to run in manual mode. Please make sure both voila and jupyterlab are installed",
+            style='bold yellow')
+
+    if mygeohub and mode == 'prod':
+        console.print("This is a MyGeoHub Tool. Production mode is not allowed.", style='bold red')
         return
 
-    log_file = f'{WORKING_DIR}/japper_run.log'
-    # clean the log
-    with open(log_file, 'w') as f:
-        f.write('')
-
-    console.print("Running the project in %s mode" % ('production preview' if env == 'prod' else 'development'),
-                  style="bold magenta")
-
-    if config['dev_env'] == 'docker':
-        # Build the docker image
-        build_docker_image(env, quiet=not verbose)
-        cmd = f'cd container/{env} && docker-compose up --remove-orphans'
-
-    elif config['dev_env'] == 'conda':
-        # check env fist
-        check_cur_conda_env(config['conda']['env_name'])
-        cmd = "voila ./app.ipynb --no-browser --port=8888 --debug --show_tracebacks=True"
-        if env == 'dev':
-            cmd = f"""{MODULE_DIR}/parallel_cmd.sh "{cmd}" "jupyter lab --allow-root --no-browser --port=8889 --IdentityProvider.token='' --ServerApp.password=''" """
+    if run_env == 'local' and mode == 'prod':
+        ret = confirm("The production mode will be run in Docker. Do you want to continue?")
+        if not ret:
+            return
+        run_env = 'docker'
+
+    mode_desc = {
+        'dev': 'development',
+        'preview': 'production preview',
+        'prod': 'production'
+    }
+
+    console.print(f"Running the project in '{mode_desc[mode]}' mode", style="bold magenta")
+    japper_up_msg = f"[green]Japper App [bold magenta]{config['project_title']}[/bold magenta] is running" + \
+                    f" \[[white]{mode_desc[mode]},{config['dev_env']}[/white]]\n\n"
+
+    if mygeohub:
+        japper_up_msg += " - App:   http://localhost:8888/apps/app.ipynb?appmode_scroll=0"
+        check_voila_running = False
+        check_jupyter_running = True
+
+        build_docker_image('appmode', quiet=not verbose, preview_mode=is_preview)
+        cmd = get_docker_up_cmd('appmode', preview_mode=is_preview)
 
-    console.print(f"Starting the app using {config['dev_env']}", style='bold cyan')
-    if not verbose:
-        console.print(
-            f"  App running logs are being written to file:///{log_file}\n"
-            + "  You can use -v or --verbose option to see the logs.", style='yellow')
 
-    # Message for container being up
-    container_up_msg = f"[green]Japper App [bold magenta]{config['project_title']}[/bold magenta] is running [{config['dev_env']}]\n\n" + \
-                       " - App:   http://localhost:8888/"
-    if env == 'dev':
-        container_up_msg += "\n - JuptyerLab: http://localhost:8889/lab"
-    container_up_msg += "\n\n[yellow]Press Ctrl+C to stop the container"
-
-    voila_running = False
-    jupyterlab_running = False
-    if env == 'prod':
-        jupyterlab_running = True  # no JupyterLab in production
-    container_initialized = False
-
-    # Initialize the Docker container
-    with console.status("[bold deep_sky_blue1] Initializing the app running environment...") as status:
-        process = subprocess.Popen(['bash', '-c', cmd], stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
-        while True:
-            text = process.stdout.read1().decode("utf-8")
-            if verbose:
-                print(text, end='', flush=True)
+    else:
+        japper_up_msg += " - App:   http://localhost:8888/"
+        if mode == 'dev':
+            japper_up_msg += "\n - JuptyerLab: http://localhost:8889/lab"
+
+        if run_env == 'docker':
+            docker_env = 'prod' if mode == 'prod' else 'dev'
+            # Build the docker image
+            build_docker_image(docker_env, quiet=not verbose, preview_mode=is_preview)
+            cmd = get_docker_up_cmd(docker_env, preview_mode=is_preview)
+
+        elif run_env == 'local':
+            # check env fist for conda env
+            if config['dev_env'] == 'conda':
+                check_cur_conda_env(config['conda']['env_name'])
+            cmd = "voila ./app.ipynb --no-browser --port=8888 --debug --show_tracebacks=True"
+            if mode == 'dev':
+                cmd = f"""export JAPPER_APP_DEV=1 && {MODULE_DIR}/parallel_cmd.sh "{cmd}" "jupyter lab --allow-root --no-browser --port=8889 --IdentityProvider.token='' --ServerApp.password=''" """
             else:
-                with open(log_file, 'a') as f:
-                    f.write(text)
+                cmd = "export JAPPER_APP_DEV=0 && " + cmd
 
-            if not container_initialized:
-                if '[Voila] Voilà is running at:' in text:
-                    voila_running = True
-                if 'Jupyter Server' in text and 'is running at:' in text:
-                    jupyterlab_running = True
-                if voila_running and jupyterlab_running:
-                    status.update(Panel(container_up_msg), spinner='dots', speed=0.1)
-                    container_initialized = True
-
-            if process.poll() is not None:
-                break
-        ret = process.poll()
+        check_voila_running = True
+        check_jupyter_running = mode == 'dev'
 
-    # Check the return code of the process
-    if ret != 0 and ret != 33280 and not verbose:
-        console.print(
-            f'Failed to start the app. ' +
-            f'Please check the logs in file:///{log_file}',
-            style='bold red')
-        exit(-1)
+    japper_up_msg += "\n\n[yellow]Press Ctrl+C to stop the container"
 
-    console.print("App stopped", style='bold yellow')
+    run_japper_app(cmd, verbose, japper_up_msg, check_voila_running, check_jupyter_running)
 
 
 @click.command(help="Build this Japper project")
-@click.argument('mode', type=click.Choice(['docker', 'hubzero']))
+@click.argument('mode', type=click.Choice(['docker']))
 def build(mode):
     config = get_config()
+
     if mode == 'docker':
+        if 'mygeohub' in config:
+            console.print("This is a MyGeoHub Tool. No build is required.", style='bold yellow')
+            return
+
+        if config['dev_env'] == 'conda':
+            ret = confirm(
+                "The project is set to run in conda environment. Do you want to build the production Docker image?")
+            if not ret:
+                return
+
         console.print("Building the Docker image in production environment", style='bold cyan')
         build_docker_image('prod')
         console.print(f"Docker image built successfully. Please check the image '{config['project_name']}'",
                       style='bold green')
 
 
 @click.command(help="Deploy this Japper project")
 @click.argument('target', type=click.Choice(['registry']), default='registry')
 @click.option('-t', '--tag', help="tag for container image", default='latest')
 def deploy(target, tag):
     config = get_config()
+
     if target == 'registry':
         if 'registry_url' not in config:
             registry_url = prompt("Enter the Docker registry URL", default='docker.io')
             # validate the registry URL
             if registry_url[:4] == 'http':
                 registry_url = registry_url.split('//')[1]
             if registry_url[-1] == '/':
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `japper-0.0.8/src/japper_devtools/main.py` & `japper-0.0.9/src/japper_devtools/main.py`

 * *Files identical despite different names*

### Comparing `japper-0.0.8/src/japper_devtools/project_init.py` & `japper-0.0.9/src/japper_devtools/project_init.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,21 +26,21 @@
         shutil.copy(src_path, dst_path)
 
 
 def create_docker_related_files(env, project_name):
     copy_static_files(f'container/{env}')
     render_template('container.__name__.docker-compose__name__.yml.jinja2', names=[env, ''],
                     japper_dev=JAPPER_DEV,
-                    prod_preview=False,
+                    add_dev_env=env != 'prod',
                     env=env,
                     project_name=project_name)
     if env != 'prod':
         render_template('container.__name__.docker-compose__name__.yml.jinja2', names=[env, '_preview'],
                         japper_dev=JAPPER_DEV,
-                        prod_preview=True,
+                        add_dev_env=False,
                         env=env,
                         project_name=project_name)
 
 
 def init_project(config):
     project_name = config['project_name']
     project_title = config['project_title']
@@ -56,15 +56,15 @@
 
     # copy static files
     copy_static_files('app')
     copy_static_files('gitignore', '.gitignore')
 
     # create app_main.py
     create_file('app/__init__.py', "from .app_main import AppMain\n")
-    render_template('app.app_main.py.jinja2', navigation_mode='top')
+    render_template('app.app_main.py.jinja2', navigation_mode='top', mygeohub=mygeohub)
 
     # create config.py
     render_template('app.commons.config.py.jinja2', project_title=project_title)
 
     # create home page
     render_template('app.controllers.home.py.jinja2')
     render_template('app.views.home.py.jinja2')
@@ -96,15 +96,14 @@
         # docker-related
         if dev_env == 'docker':
             create_docker_related_files('appmode', project_name)
 
     else:
         # create environment.yml
         render_template('environment.yml.jinja2', project_name=project_name, japper_runtime=True)
-
         create_docker_related_files('prod', project_name)
         if dev_env == 'conda':
             conda_env_name = config['conda']['env_name']
             use_existing_conda_env = config['conda']['use_existing_env']
 
             if not use_existing_conda_env:
                 # create conda env
```

### Comparing `japper-0.0.8/src/japper_devtools/static/app/assets/icon.png` & `japper-0.0.9/src/japper_devtools/static/app/assets/icon.png`

 * *Files identical despite different names*

### Comparing `japper-0.0.8/src/japper_devtools/static/app/assets/logo.png` & `japper-0.0.9/src/japper_devtools/static/app/assets/logo.png`

 * *Files identical despite different names*

### Comparing `japper-0.0.8/src/japper_devtools/static/container/appmode/Dockerfile` & `japper-0.0.9/src/japper_devtools/static/container/appmode/Dockerfile`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 FROM jupyter/base-notebook:notebook-6.4.0
 
 # setup conda environment
 COPY ./environment.yml /home/jovyan/.
 RUN mamba env update -n base --file /home/jovyan/environment.yml
-ADD --chown=jovyan:users ./container/dev/start.sh /home/jovyan/.
+ADD --chown=jovyan:users ./container/appmode/start.sh /home/jovyan/.
 RUN chmod +x /home/jovyan/start.sh
 
 # depress the warning message
 ENV PYDEVD_DISABLE_FILE_VALIDATION=1
 
 RUN pip install appmode && \
     jupyter nbextension     enable --py --sys-prefix appmode && \
```

### Comparing `japper-0.0.8/src/japper_devtools/static/container/prod/start.sh` & `japper-0.0.9/src/japper_devtools/static/container/prod/start.sh`

 * *Files identical despite different names*

### Comparing `japper-0.0.8/src/japper_devtools/static/gitignore` & `japper-0.0.9/src/japper_devtools/static/gitignore`

 * *Files identical despite different names*

### Comparing `japper-0.0.8/src/japper_devtools/templates/app.controllers.__name__.py.jinja2` & `japper-0.0.9/src/japper_devtools/templates/app.controllers.__name__.py.jinja2`

 * *Files identical despite different names*

### Comparing `japper-0.0.8/src/japper_devtools/templates/app.controllers.home.py.jinja2` & `japper-0.0.9/src/japper_devtools/templates/app.controllers.home.py.jinja2`

 * *Files identical despite different names*

### Comparing `japper-0.0.8/src/japper_devtools/templates/app.ipynb.jinja2` & `japper-0.0.9/src/japper_devtools/templates/app.ipynb.jinja2`

 * *Files identical despite different names*

### Comparing `japper-0.0.8/src/japper_devtools/templates/app.views.home.py.jinja2` & `japper-0.0.9/src/japper_devtools/templates/app.views.home.py.jinja2`

 * *Files identical despite different names*

### Comparing `japper-0.0.8/src/japper_devtools/templates/container.__name__.docker-compose__name__.yml.jinja2` & `japper-0.0.9/src/japper_devtools/templates/container.__name__.docker-compose__name__.yml.jinja2`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 name: {{ project_name }}
 services:
   {{ project_name }}-{{ env }}:
     build:
       context: ../../
       dockerfile: ./container/{{ env }}/Dockerfile
     volumes:
-      {% if env=='dev' or env=='appmode' %}- ../..:/home/jovyan/japper_app{% endif %}
-      {% if japper_dev %}- ../../../:/home/jovyan/japper{% endif %}
+        {% if env=='dev' or env=='appmode' %}- ../..:/home/jovyan/japper_app{% endif %}
+        {% if japper_dev %}- ../../../:/home/jovyan/japper{% endif %}
     ports:
       - "8888:8888"
       {% if env=='dev' %}- "8889:8889"{% endif %}
     {% if japper_dev %}command: /bin/bash -c "pip install -e /home/jovyan/japper && /home/jovyan/start.sh"{% endif %}
-  {% if not prod_preview %}
+    {% if add_dev_env %}
     environment:
       JAPPER_APP_DEV: 1
-  {% endif %}
+    {% endif %}
```

### Comparing `japper-0.0.8/src/japper_devtools/utils.py` & `japper-0.0.9/src/japper_devtools/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from re import sub
 import os, sys
 import subprocess
 import yaml
 from jinja2 import Environment, FileSystemLoader
 from rich.prompt import Prompt, Confirm
+from rich.panel import Panel
 
 from rich.console import Console
 
 console = Console()
 
 # jinja2 environment
 env = Environment(loader=FileSystemLoader(os.path.dirname(__file__) + '/templates'))
 
 CONFIG_FILENAME = 'japper.yml'
+WORKING_DIR = os.getcwd().replace('\\', '/')
 
 JAPPER_DEV = False
 
 
 class InitConfig:
     # Directories to be created
     DIRS_TO_CREATE = ['app', 'app/assets', 'app/commons', 'app/models', 'app/controllers', 'app/views', 'container']
@@ -252,25 +254,29 @@
     envs = [env.split()[0] for env in envs if env and env[0] != '#']
     return envs
 
 
 def check_cur_conda_env(app_env_name):
     cur_env = os.environ['CONDA_DEFAULT_ENV']
     if cur_env != app_env_name:
-        console.print(f"Please activate the conda environment {app_env_name} first", style='bold red')
+        console.print(
+            f"Please activate the conda environment {app_env_name} first: [white] conda activate {app_env_name}[/white]",
+            style='bold yellow')
         exit(-1)
 
 
 def build_docker_image(env, quiet=False, preview_mode=False):
     console.print('Build the Docker image', style='bold cyan')
-    cmd = f'cd container/{env} && docker-compose build'
-    if quiet:
-        cmd += ' -q'
+    cmd = f'cd container/{env} && docker-compose'
     if preview_mode:
         cmd += ' -f docker-compose_preview.yml'
+    cmd += ' build'
+    if quiet:
+        cmd += ' -q'
+
     run_command_with_bottom_msg(cmd, 'Building the Docker image...'
                                 , fail_msg='Failed to build the Docker image'
                                 , color_err=True)
 
 
 def run_command_with_bottom_msg(cmd, bottom_msg, fail_msg=None, color_err=False):
     if type(cmd) is not list:
@@ -291,7 +297,65 @@
         rc = process.poll()
 
     if rc != 0:
         if fail_msg:
             console.print(fail_msg, style='bold red')
         exit(-1)
     return rc
+
+
+def run_japper_app(cmd, verbose, japper_up_msg, check_voila_running, check_jupyter_running):
+    log_file = f'{WORKING_DIR}/japper_run.log'
+    # clean the log
+    with open(log_file, 'w') as f:
+        f.write('')
+
+    console.print(f"Starting the app", style='bold cyan')
+    if not verbose:
+        console.print(
+            f"  App running logs are being written to file:///{log_file}\n"
+            + "  You can use -v or --verbose option to see the logs.", style='yellow')
+
+    voila_running = not check_voila_running
+    jupyter_running = not check_jupyter_running
+    app_initialized = False
+
+    with console.status("[bold deep_sky_blue1] Initializing the app running environment...") as status:
+        process = subprocess.Popen(['bash', '-c', cmd], stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+        while True:
+            text = process.stdout.read1().decode("utf-8")
+            if verbose:
+                print(text, end='', flush=True)
+            else:
+                with open(log_file, 'a') as f:
+                    f.write(text)
+            if not app_initialized:
+                if '[Voila] Voilà is running at:' in text:
+                    voila_running = True
+                if 'Jupyter ' in text and 'is running at:' in text:
+                    jupyter_running = True
+                if voila_running and jupyter_running:
+                    status.update(Panel(japper_up_msg), spinner='dots', speed=0.1)
+                    app_initialized = True
+
+            if process.poll() is not None:
+                break
+        ret = process.poll()
+
+    # Check the return code of the process
+    if ret != 0 and ret != 33280 and not verbose:
+        console.print(
+            f'Failed to start the app. ' +
+            f'Please check the logs in file:///{log_file}',
+            style='bold red')
+        exit(-1)
+
+    console.print("App stopped", style='bold yellow')
+
+
+def get_docker_up_cmd(env, preview_mode):
+    cmd = f'cd container/{env} && docker-compose'
+    if preview_mode:
+        cmd += ' -f docker-compose_preview.yml'
+    cmd += ' up --remove-orphans'
+
+    return cmd
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

