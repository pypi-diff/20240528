# Comparing `tmp/voila_materialscloud_template-0.4.1.tar.gz` & `tmp/voila_materialscloud_template-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voila_materialscloud_template-0.4.1.tar", last modified: Fri May 17 21:08:16 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `voila_materialscloud_template-0.4.1.tar` & `voila_materialscloud_template-0.4.3.tar`

### file list

```diff
@@ -1,103 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:08:16.991226 voila_materialscloud_template-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-05-17 21:08:16.991226 voila_materialscloud_template-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     3294 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/copy_voila_template.py
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-17 21:08:16.991226 voila_materialscloud_template-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-17 21:08:13.000000 voila_materialscloud_template-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:08:16.971226 voila_materialscloud_template-0.4.1/share/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:08:16.975226 voila_materialscloud_template-0.4.1/share/jupyter/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:08:16.971226 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:08:16.975226 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:08:16.979226 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud/conf.json
--rw-r--r--   0 runner    (1001) docker     (127)    16864 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud/index.html.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:08:16.975226 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:08:16.987226 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)   546493 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud/static/css/index.css
--rw-r--r--   0 runner    (1001) docker     (127)   140563 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud/static/css/mcloud_theme.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    15629 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud/static/css/theme-dark.css
--rw-r--r--   0 runner    (1001) docker     (127)    14533 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud/static/css/theme-light.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:08:16.987226 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud/static/images/
--rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud/static/images/favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud/static/images/mcloud_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud/static/images/mcloud_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     9893 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud/static/images/mcloud_spinner.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:08:16.987226 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)    17536 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud/static/js/require.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:08:16.979226 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-discover/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-discover/conf.json
--rw-r--r--   0 runner    (1001) docker     (127)    16607 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-discover/index.html.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:08:16.975226 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-discover/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:08:16.979226 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-discover/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)   546493 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-discover/static/css/index.css
--rw-r--r--   0 runner    (1001) docker     (127)   140563 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-discover/static/css/mcloud_theme.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    15629 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-discover/static/css/theme-dark.css
--rw-r--r--   0 runner    (1001) docker     (127)    14533 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-discover/static/css/theme-light.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:08:16.979226 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-discover/static/images/
--rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-discover/static/images/favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-discover/static/images/mcloud_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-discover/static/images/mcloud_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     9893 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-discover/static/images/mcloud_spinner.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:08:16.979226 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-discover/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)    17536 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-discover/static/js/require.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:08:16.979226 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-iframe/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-iframe/conf.json
--rw-r--r--   0 runner    (1001) docker     (127)    13920 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-iframe/index.html.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:08:16.975226 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-iframe/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:08:16.983226 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-iframe/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)   546493 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-iframe/static/css/index.css
--rw-r--r--   0 runner    (1001) docker     (127)   140563 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-iframe/static/css/mcloud_theme.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    15629 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-iframe/static/css/theme-dark.css
--rw-r--r--   0 runner    (1001) docker     (127)    14533 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-iframe/static/css/theme-light.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:08:16.983226 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-iframe/static/images/
--rw-r--r--   0 runner    (1001) docker     (127)    18197 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-iframe/static/images/MaterialsCloud_Horizontal_White.png
--rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-iframe/static/images/favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-iframe/static/images/mcloud_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-iframe/static/images/mcloud_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     9893 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-iframe/static/images/mcloud_spinner.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:08:16.983226 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-iframe/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)    53386 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-iframe/static/js/iframeResizer.contentWindow.map
--rw-r--r--   0 runner    (1001) docker     (127)    14147 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-iframe/static/js/iframeResizer.contentWindow.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    17536 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-iframe/static/js/require.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:08:16.983226 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-tool/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-tool/conf.json
--rw-r--r--   0 runner    (1001) docker     (127)    16864 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-tool/index.html.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:08:16.975226 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-tool/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:08:16.987226 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-tool/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)   546493 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-tool/static/css/index.css
--rw-r--r--   0 runner    (1001) docker     (127)   140563 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-tool/static/css/mcloud_theme.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    15629 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-tool/static/css/theme-dark.css
--rw-r--r--   0 runner    (1001) docker     (127)    14533 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-tool/static/css/theme-light.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:08:16.987226 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-tool/static/images/
--rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-tool/static/images/favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-tool/static/images/mcloud_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-tool/static/images/mcloud_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     9893 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-tool/static/images/mcloud_spinner.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:08:16.987226 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-tool/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)    17536 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-tool/static/js/require.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:08:16.975226 voila_materialscloud_template-0.4.1/share/jupyter/voila/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:08:16.975226 voila_materialscloud_template-0.4.1/share/jupyter/voila/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:08:16.991226 voila_materialscloud_template-0.4.1/share/jupyter/voila/templates/materialscloud/
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/voila/templates/materialscloud/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/voila/templates/materialscloud/index.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/voila/templates/materialscloud/spinner.macro.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/voila/templates/materialscloud/tree.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:08:16.991226 voila_materialscloud_template-0.4.1/share/jupyter/voila/templates/materialscloud-discover/
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/voila/templates/materialscloud-discover/index.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/voila/templates/materialscloud-discover/spinner.macro.html.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:08:16.991226 voila_materialscloud_template-0.4.1/share/jupyter/voila/templates/materialscloud-iframe/
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/voila/templates/materialscloud-iframe/index.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/voila/templates/materialscloud-iframe/spinner.macro.html.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:08:16.991226 voila_materialscloud_template-0.4.1/share/jupyter/voila/templates/materialscloud-tool/
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/voila/templates/materialscloud-tool/index.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-17 21:08:07.000000 voila_materialscloud_template-0.4.1/share/jupyter/voila/templates/materialscloud-tool/spinner.macro.html.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:08:16.991226 voila_materialscloud_template-0.4.1/voila_materialscloud_template.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-05-17 21:08:16.000000 voila_materialscloud_template-0.4.1/voila_materialscloud_template.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-05-17 21:08:16.000000 voila_materialscloud_template-0.4.1/voila_materialscloud_template.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 21:08:16.000000 voila_materialscloud_template-0.4.1/voila_materialscloud_template.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-17 21:08:16.000000 voila_materialscloud_template-0.4.1/voila_materialscloud_template.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 21:08:16.000000 voila_materialscloud_template-0.4.1/voila_materialscloud_template.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/tasks.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/.github/static/release_tag_msg.txt
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/.github/workflows/ci-build.yml
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/.github/workflows/publish-on-pypi.yml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/docker/Dockerfile
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/docker/docker-compose.yml
+-rw-r--r--   0        0        0     6154 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/example-notebooks/example.ipynb
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud/conf.json
+-rw-r--r--   0        0        0    16864 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud/index.html.j2
+-rw-r--r--   0        0        0   546493 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud/static/css/index.css
+-rw-r--r--   0        0        0   140563 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud/static/css/mcloud_theme.min.css
+-rw-r--r--   0        0        0    15629 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud/static/css/theme-dark.css
+-rw-r--r--   0        0        0    14533 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud/static/css/theme-light.css
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud/static/images/favicon.png
+-rw-r--r--   0        0        0     3805 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud/static/images/mcloud_logo.png
+-rw-r--r--   0        0        0     3490 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud/static/images/mcloud_logo.svg
+-rw-r--r--   0        0        0     9893 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud/static/images/mcloud_spinner.svg
+-rw-r--r--   0        0        0    17536 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud/static/js/require.min.js
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud-discover/conf.json
+-rw-r--r--   0        0        0    16607 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud-discover/index.html.j2
+-rw-r--r--   0        0        0   546493 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud-discover/static/css/index.css
+-rw-r--r--   0        0        0   140563 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud-discover/static/css/mcloud_theme.min.css
+-rw-r--r--   0        0        0    15629 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud-discover/static/css/theme-dark.css
+-rw-r--r--   0        0        0    14533 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud-discover/static/css/theme-light.css
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud-discover/static/images/favicon.png
+-rw-r--r--   0        0        0     3805 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud-discover/static/images/mcloud_logo.png
+-rw-r--r--   0        0        0     3490 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud-discover/static/images/mcloud_logo.svg
+-rw-r--r--   0        0        0     9893 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud-discover/static/images/mcloud_spinner.svg
+-rw-r--r--   0        0        0    17536 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud-discover/static/js/require.min.js
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud-iframe/conf.json -> ../materialscloud/conf.json
+-rw-r--r--   0        0        0    13920 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud-iframe/index.html.j2
+-rw-r--r--   0        0        0    18197 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud-iframe/static/images/MaterialsCloud_Horizontal_White.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud-iframe/static/images/favicon.png -> ../../../materialscloud/static/images/favicon.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud-iframe/static/images/mcloud_logo.png -> ../../../materialscloud/static/images/mcloud_logo.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud-iframe/static/images/mcloud_logo.svg -> ../../../materialscloud/static/images/mcloud_logo.svg
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud-iframe/static/images/mcloud_spinner.svg -> ../../../materialscloud/static/images/mcloud_spinner.svg
+-rw-r--r--   0        0        0    53386 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud-iframe/static/js/iframeResizer.contentWindow.map
+-rw-r--r--   0        0        0    14147 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud-iframe/static/js/iframeResizer.contentWindow.min.js
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud-iframe/static/js/require.min.js -> ../../../materialscloud/static/js/require.min.js
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud-tool/conf.json
+-rw-r--r--   0        0        0    16864 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud-tool/index.html.j2
+-rw-r--r--   0        0        0   546493 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud-tool/static/css/index.css
+-rw-r--r--   0        0        0   140563 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud-tool/static/css/mcloud_theme.min.css
+-rw-r--r--   0        0        0    15629 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud-tool/static/css/theme-dark.css
+-rw-r--r--   0        0        0    14533 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud-tool/static/css/theme-light.css
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud-tool/static/images/favicon.png
+-rw-r--r--   0        0        0     3805 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud-tool/static/images/mcloud_logo.png
+-rw-r--r--   0        0        0     3490 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud-tool/static/images/mcloud_logo.svg
+-rw-r--r--   0        0        0     9893 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud-tool/static/images/mcloud_spinner.svg
+-rw-r--r--   0        0        0    17536 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud-tool/static/js/require.min.js
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/share/jupyter/voila/templates/materialscloud/base.html
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/share/jupyter/voila/templates/materialscloud/index.html.j2
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/share/jupyter/voila/templates/materialscloud/spinner.macro.html.j2
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/share/jupyter/voila/templates/materialscloud/tree.html
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/share/jupyter/voila/templates/materialscloud-discover/index.html.j2
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/share/jupyter/voila/templates/materialscloud-discover/spinner.macro.html.j2
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/share/jupyter/voila/templates/materialscloud-iframe/index.html.j2
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/share/jupyter/voila/templates/materialscloud-iframe/spinner.macro.html.j2 -> ../materialscloud/spinner.macro.html.j2
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/share/jupyter/voila/templates/materialscloud-tool/index.html.j2
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/share/jupyter/voila/templates/materialscloud-tool/spinner.macro.html.j2
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/.gitignore
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/LICENSE.txt
+-rw-r--r--   0        0        0     2662 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/README.md
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     5438 2020-02-02 00:00:00.000000 voila_materialscloud_template-0.4.3/PKG-INFO
```

### Comparing `voila_materialscloud_template-0.4.1/LICENSE` & `voila_materialscloud_template-0.4.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `voila_materialscloud_template-0.4.1/PKG-INFO` & `voila_materialscloud_template-0.4.3/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,19 @@
-Metadata-Version: 2.1
-Name: voila-materialscloud-template
-Version: 0.4.1
-Summary: Voilà template for Materials Cloud that implements the Materials Cloud header and CSS.
-Home-page: https://github.com/materialscloud-org/voila-materialscloud-template
-Author: Dou Du and Casper Welzel Andersen
-Author-email: dou.du@epfl.ch
-License: BSD
-Keywords: voila jupyter materialscloud
-Description-Content-Type: text/markdown
-Requires-Dist: voila~=0.4.4
-Requires-Dist: jupyter-core~=5.3.1
-Provides-Extra: dev
-Requires-Dist: invoke~=2.2; extra == "dev"
-Requires-Dist: ipywidgets~=8.1; extra == "dev"
-Requires-Dist: pylint~=2.17; extra == "dev"
-Requires-Dist: jupyterlab~=4.0; extra == "dev"
-Requires-Dist: widget-periodictable~=4.1; extra == "dev"
-
 # Voilà template for Materials Cloud
+
 [![PyPI - Version](https://img.shields.io/pypi/v/voila-materialscloud-template?color=4CC61E)](https://pypi.org/project/voila-materialscloud-template/)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/materialscloud-org/voila-materialscloud-template/main?urlpath=%2Fvoila%2Frender%2Fexample-notebooks%2Fexample.ipynb)
 
 This is the Voilà template for Materials Cloud, implements the standard header and CSS.
 
 Three templates are provided:
-* `materialscloud-tool` - highlights the [WORK](https://www.materialscloud.org/work)/Tools section in the header/breadcrumbs.
-* `materialscloud-discover` - highlights the [DISCOVER](https://www.materialscloud.org/discover) section in the header/breadcrumbs.
-* `materialscloud-iframe` - just adds a simple "Hosted on Materials Cloud" note at the bottom.
+
+- `materialscloud-tool` - highlights the [WORK](https://www.materialscloud.org/work)/Tools section in the header/breadcrumbs.
+- `materialscloud-discover` - highlights the [DISCOVER](https://www.materialscloud.org/discover) section in the header/breadcrumbs.
+- `materialscloud-iframe` - just adds a simple "Hosted on Materials Cloud" note at the bottom.
 
 ## Installation
 
 ```bash
 pip install voila-materialscloud-template
 ```
 
@@ -39,14 +22,15 @@
 ## Usage
 
 The main way is to use the `voila --template` option, e.g.:
 
 ```bash
 voila --template=materialscloud-tool example.ipynb
 ```
+
 Alternatively, you can write a `voila.json` file containing
 
 ```json
 {
   "VoilaConfiguration": {
     "template": "materialscloud-tool"
   },
@@ -66,15 +50,15 @@
 
 Option 1:
 
 ```bash
 pip install -e .[dev]
 ```
 
-Note: this will copy the templates to the jupyter folder, and they need to be modified directly there or re-copied if new tests are required.
+Note: this will copy the templates to the jupyter folder, and they need to be modified directly there or re-copied for changes to take effect.
 
 Option 2:
 
 It's more convenient to use a docker container and rebuild after modification:
 
 ```bash
 cd docker
@@ -84,15 +68,16 @@
 and access via `http://localhost:8866/`. The template and other voila configuration is specified in `voila.json`.
 
 Note: maybe there is an easier setup, e.g. with live-reload or similar.
 
 ### Making a new release
 
 To release a new version, just make a new release on Github with the correct version tag, without updating any versions manually. This will start the GitHub action that will
-* update version numbers in the repo and commits it;
-* tags this new commit with the version, overwriting the tag that was made by the Github release;
-* pushes commit & tag to Github;
-* publishes new version on PYPI.
+
+- update version numbers in the repo and commits it;
+- tags this new commit with the version, overwriting the tag that was made by the Github release;
+- pushes commit & tag to Github;
+- publishes new version on PYPI.
 
 ## License
 
 This repository and all files in it are licensed under the [BSD license](LICENSE), copyright (c) by Voilà contributors.
```

### Comparing `voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud/index.html.j2` & `voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud/index.html.j2`

 * *Files identical despite different names*

### Comparing `voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud/static/css/index.css` & `voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud/static/css/index.css`

 * *Files identical despite different names*

### Comparing `voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud/static/css/mcloud_theme.min.css` & `voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud/static/css/mcloud_theme.min.css`

 * *Files identical despite different names*

### Comparing `voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud/static/css/theme-dark.css` & `voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud/static/css/theme-dark.css`

 * *Files identical despite different names*

### Comparing `voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud/static/css/theme-light.css` & `voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud/static/css/theme-light.css`

 * *Files identical despite different names*

### Comparing `voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud/static/images/favicon.png` & `voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud/static/images/favicon.png`

 * *Files identical despite different names*

### Comparing `voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud/static/images/mcloud_logo.png` & `voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud/static/images/mcloud_logo.png`

 * *Files identical despite different names*

### Comparing `voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud/static/images/mcloud_logo.svg` & `voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud/static/images/mcloud_logo.svg`

 * *Files identical despite different names*

### Comparing `voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud/static/images/mcloud_spinner.svg` & `voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud/static/images/mcloud_spinner.svg`

 * *Files identical despite different names*

### Comparing `voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud/static/js/require.min.js` & `voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud/static/js/require.min.js`

 * *Files identical despite different names*

### Comparing `voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-discover/index.html.j2` & `voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud-discover/index.html.j2`

 * *Files identical despite different names*

### Comparing `voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-discover/static/css/index.css` & `voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud-discover/static/css/index.css`

 * *Files identical despite different names*

### Comparing `voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-discover/static/css/mcloud_theme.min.css` & `voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud-discover/static/css/mcloud_theme.min.css`

 * *Files identical despite different names*

### Comparing `voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-discover/static/css/theme-dark.css` & `voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud-discover/static/css/theme-dark.css`

 * *Files identical despite different names*

### Comparing `voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-discover/static/css/theme-light.css` & `voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud-discover/static/css/theme-light.css`

 * *Files identical despite different names*

### Comparing `voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-discover/static/images/favicon.png` & `voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud-discover/static/images/favicon.png`

 * *Files identical despite different names*

### Comparing `voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-discover/static/images/mcloud_logo.png` & `voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud-discover/static/images/mcloud_logo.png`

 * *Files identical despite different names*

### Comparing `voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-discover/static/images/mcloud_logo.svg` & `voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud-discover/static/images/mcloud_logo.svg`

 * *Files identical despite different names*

### Comparing `voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-discover/static/images/mcloud_spinner.svg` & `voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud-discover/static/images/mcloud_spinner.svg`

 * *Files identical despite different names*

### Comparing `voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-discover/static/js/require.min.js` & `voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud-discover/static/js/require.min.js`

 * *Files identical despite different names*

### Comparing `voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-iframe/index.html.j2` & `voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud-iframe/index.html.j2`

 * *Files identical despite different names*

### Comparing `voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-iframe/static/css/index.css` & `voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud-tool/static/css/index.css`

 * *Files identical despite different names*

### Comparing `voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-iframe/static/css/mcloud_theme.min.css` & `voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud-tool/static/css/mcloud_theme.min.css`

 * *Files identical despite different names*

### Comparing `voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-iframe/static/css/theme-dark.css` & `voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud-tool/static/css/theme-dark.css`

 * *Files identical despite different names*

### Comparing `voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-iframe/static/css/theme-light.css` & `voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud-tool/static/css/theme-light.css`

 * *Files identical despite different names*

### Comparing `voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-iframe/static/images/MaterialsCloud_Horizontal_White.png` & `voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud-iframe/static/images/MaterialsCloud_Horizontal_White.png`

 * *Files identical despite different names*

### Comparing `voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-iframe/static/images/favicon.png` & `voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud-tool/static/images/favicon.png`

 * *Files identical despite different names*

### Comparing `voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-iframe/static/images/mcloud_logo.png` & `voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud-tool/static/images/mcloud_logo.png`

 * *Files identical despite different names*

### Comparing `voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-iframe/static/images/mcloud_logo.svg` & `voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud-tool/static/images/mcloud_logo.svg`

 * *Files identical despite different names*

### Comparing `voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-iframe/static/images/mcloud_spinner.svg` & `voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud-tool/static/images/mcloud_spinner.svg`

 * *Files identical despite different names*

### Comparing `voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-iframe/static/js/iframeResizer.contentWindow.map` & `voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud-iframe/static/js/iframeResizer.contentWindow.map`

 * *Files identical despite different names*

### Comparing `voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-iframe/static/js/iframeResizer.contentWindow.min.js` & `voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud-iframe/static/js/iframeResizer.contentWindow.min.js`

 * *Files identical despite different names*

### Comparing `voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-iframe/static/js/require.min.js` & `voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud-tool/static/js/require.min.js`

 * *Files identical despite different names*

### Comparing `voila_materialscloud_template-0.4.1/share/jupyter/nbconvert/templates/materialscloud-tool/index.html.j2` & `voila_materialscloud_template-0.4.3/share/jupyter/nbconvert/templates/materialscloud-tool/index.html.j2`

 * *Files identical despite different names*

### Comparing `voila_materialscloud_template-0.4.1/share/jupyter/voila/templates/materialscloud/base.html` & `voila_materialscloud_template-0.4.3/share/jupyter/voila/templates/materialscloud/base.html`

 * *Files identical despite different names*

### Comparing `voila_materialscloud_template-0.4.1/share/jupyter/voila/templates/materialscloud/index.html.j2` & `voila_materialscloud_template-0.4.3/share/jupyter/voila/templates/materialscloud/index.html.j2`

 * *Files identical despite different names*

### Comparing `voila_materialscloud_template-0.4.1/share/jupyter/voila/templates/materialscloud/spinner.macro.html.j2` & `voila_materialscloud_template-0.4.3/share/jupyter/voila/templates/materialscloud/spinner.macro.html.j2`

 * *Files identical despite different names*

### Comparing `voila_materialscloud_template-0.4.1/share/jupyter/voila/templates/materialscloud-discover/index.html.j2` & `voila_materialscloud_template-0.4.3/share/jupyter/voila/templates/materialscloud-discover/index.html.j2`

 * *Files identical despite different names*

### Comparing `voila_materialscloud_template-0.4.1/share/jupyter/voila/templates/materialscloud-discover/spinner.macro.html.j2` & `voila_materialscloud_template-0.4.3/share/jupyter/voila/templates/materialscloud-discover/spinner.macro.html.j2`

 * *Files identical despite different names*

### Comparing `voila_materialscloud_template-0.4.1/share/jupyter/voila/templates/materialscloud-iframe/index.html.j2` & `voila_materialscloud_template-0.4.3/share/jupyter/voila/templates/materialscloud-iframe/index.html.j2`

 * *Files identical despite different names*

### Comparing `voila_materialscloud_template-0.4.1/share/jupyter/voila/templates/materialscloud-iframe/spinner.macro.html.j2` & `voila_materialscloud_template-0.4.3/share/jupyter/voila/templates/materialscloud-tool/spinner.macro.html.j2`

 * *Files identical despite different names*

### Comparing `voila_materialscloud_template-0.4.1/share/jupyter/voila/templates/materialscloud-tool/index.html.j2` & `voila_materialscloud_template-0.4.3/share/jupyter/voila/templates/materialscloud-tool/index.html.j2`

 * *Files identical despite different names*

