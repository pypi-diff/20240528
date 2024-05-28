# Comparing `tmp/JustDeepIt-0.2.3.tar.gz` & `tmp/JustDeepIt-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JustDeepIt-0.2.3.tar", last modified: Thu May 23 01:54:21 2024, max compression
+gzip compressed data, was "JustDeepIt-0.2.4.tar", last modified: Tue May 28 06:03:18 2024, max compression
```

## Comparing `JustDeepIt-0.2.3.tar` & `JustDeepIt-0.2.4.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:21.725402 JustDeepIt-0.2.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:21.717402 JustDeepIt-0.2.3/JustDeepIt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-23 01:54:21.000000 JustDeepIt-0.2.3/JustDeepIt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-05-23 01:54:21.000000 JustDeepIt-0.2.3/JustDeepIt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 01:54:21.000000 JustDeepIt-0.2.3/JustDeepIt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-23 01:54:21.000000 JustDeepIt-0.2.3/JustDeepIt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-23 01:54:21.000000 JustDeepIt-0.2.3/JustDeepIt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-23 01:54:21.000000 JustDeepIt-0.2.3/JustDeepIt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 01:54:21.000000 JustDeepIt-0.2.3/JustDeepIt.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-23 01:54:21.725402 JustDeepIt-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:21.717402 JustDeepIt-0.2.3/justdeepit/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:21.717402 JustDeepIt-0.2.3/justdeepit/app/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24123 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/appbase.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/appis.py
--rw-r--r--   0 runner    (1001) docker     (127)    10048 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/appod.py
--rw-r--r--   0 runner    (1001) docker     (127)    22300 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/appsod.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:21.717402 JustDeepIt-0.2.3/justdeepit/app/static/
--rw-r--r--   0 runner    (1001) docker     (127)    89501 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jquery-3.6.0.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   137972 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jquery-3.6.0.min.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:21.717402 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:21.721402 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/
--rwxr-xr-x   0 runner    (1001) docker     (127)      464 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/application.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      603 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/code.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      618 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/css.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      579 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/db.png
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/directory-lock.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      537 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/directory.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      651 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/doc.png
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/file-lock.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      294 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/file.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      653 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/film.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      582 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/flash.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      583 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/folder_open.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      734 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/html.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      633 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/java.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      668 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/linux.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      385 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/music.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      591 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/pdf.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      538 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/php.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      606 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/picture.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      588 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/ppt.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      856 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/psd.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      626 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/ruby.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      859 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/script.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     2530 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/spinner.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      342 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/txt.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      663 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/xls.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      386 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/zip.png
--rw-r--r--   0 runner    (1001) docker     (127)     6326 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/jQueryFileTree.css
--rw-r--r--   0 runner    (1001) docker     (127)     7361 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/jQueryFileTree.js
--rw-r--r--   0 runner    (1001) docker     (127)    14483 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/styles.css
--rw-r--r--   0 runner    (1001) docker     (127)    20646 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/static/utils.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:21.721402 JustDeepIt-0.2.3/justdeepit/app/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)    17454 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/templates/module.html
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/app/templates/shutdown.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:21.721402 JustDeepIt-0.2.3/justdeepit/models/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/models/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)    12931 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/models/instance_segment.py
--rw-r--r--   0 runner    (1001) docker     (127)    13500 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/models/object_detect.py
--rw-r--r--   0 runner    (1001) docker     (127)    12227 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/models/salient_object_detect.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:21.725402 JustDeepIt-0.2.3/justdeepit/models/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6720 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/models/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    13883 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/models/utils/mmdetbase.py
--rw-r--r--   0 runner    (1001) docker     (127)    36052 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/models/utils/u2net.py
--rw-r--r--   0 runner    (1001) docker     (127)    10173 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/models/utils/unet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:21.713402 JustDeepIt-0.2.3/justdeepit/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:21.725402 JustDeepIt-0.2.3/justdeepit/src/font/
--rw-r--r--   0 runner    (1001) docker     (127)   555264 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/src/font/NotoSans-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/src/font/OFL.txt
--rw-r--r--   0 runner    (1001) docker     (127)    56860 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/justdeepit/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 01:54:21.725402 JustDeepIt-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-23 01:52:13.000000 JustDeepIt-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:03:18.312703 JustDeepIt-0.2.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:03:18.300703 JustDeepIt-0.2.4/JustDeepIt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-28 06:03:18.000000 JustDeepIt-0.2.4/JustDeepIt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-05-28 06:03:18.000000 JustDeepIt-0.2.4/JustDeepIt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 06:03:18.000000 JustDeepIt-0.2.4/JustDeepIt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-28 06:03:18.000000 JustDeepIt-0.2.4/JustDeepIt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-28 06:03:18.000000 JustDeepIt-0.2.4/JustDeepIt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-28 06:03:18.000000 JustDeepIt-0.2.4/JustDeepIt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 06:03:18.000000 JustDeepIt-0.2.4/JustDeepIt.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-28 06:03:18.312703 JustDeepIt-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:03:18.300703 JustDeepIt-0.2.4/justdeepit/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/justdeepit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:03:18.304703 JustDeepIt-0.2.4/justdeepit/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/justdeepit/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24123 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/justdeepit/app/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/justdeepit/app/appbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/justdeepit/app/appis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10048 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/justdeepit/app/appod.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22300 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/justdeepit/app/appsod.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:03:18.304703 JustDeepIt-0.2.4/justdeepit/app/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    89501 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/justdeepit/app/static/jquery-3.6.0.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   137972 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/justdeepit/app/static/jquery-3.6.0.min.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:03:18.304703 JustDeepIt-0.2.4/justdeepit/app/static/jqueryfiletree/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:03:18.308703 JustDeepIt-0.2.4/justdeepit/app/static/jqueryfiletree/images/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      464 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/justdeepit/app/static/jqueryfiletree/images/application.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      603 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/justdeepit/app/static/jqueryfiletree/images/code.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      618 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/justdeepit/app/static/jqueryfiletree/images/css.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      579 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/justdeepit/app/static/jqueryfiletree/images/db.png
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/justdeepit/app/static/jqueryfiletree/images/directory-lock.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      537 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/justdeepit/app/static/jqueryfiletree/images/directory.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      651 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/justdeepit/app/static/jqueryfiletree/images/doc.png
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/justdeepit/app/static/jqueryfiletree/images/file-lock.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      294 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/justdeepit/app/static/jqueryfiletree/images/file.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      653 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/justdeepit/app/static/jqueryfiletree/images/film.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      582 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/justdeepit/app/static/jqueryfiletree/images/flash.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      583 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/justdeepit/app/static/jqueryfiletree/images/folder_open.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      734 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/justdeepit/app/static/jqueryfiletree/images/html.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      633 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/justdeepit/app/static/jqueryfiletree/images/java.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      668 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/justdeepit/app/static/jqueryfiletree/images/linux.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      385 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/justdeepit/app/static/jqueryfiletree/images/music.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      591 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/justdeepit/app/static/jqueryfiletree/images/pdf.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      538 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/justdeepit/app/static/jqueryfiletree/images/php.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      606 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/justdeepit/app/static/jqueryfiletree/images/picture.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      588 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/justdeepit/app/static/jqueryfiletree/images/ppt.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      856 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/justdeepit/app/static/jqueryfiletree/images/psd.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      626 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/justdeepit/app/static/jqueryfiletree/images/ruby.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      859 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/justdeepit/app/static/jqueryfiletree/images/script.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2530 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/justdeepit/app/static/jqueryfiletree/images/spinner.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      342 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/justdeepit/app/static/jqueryfiletree/images/txt.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      663 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/justdeepit/app/static/jqueryfiletree/images/xls.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      386 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/justdeepit/app/static/jqueryfiletree/images/zip.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6326 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/justdeepit/app/static/jqueryfiletree/jQueryFileTree.css
+-rw-r--r--   0 runner    (1001) docker     (127)     7361 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/justdeepit/app/static/jqueryfiletree/jQueryFileTree.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14483 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/justdeepit/app/static/styles.css
+-rw-r--r--   0 runner    (1001) docker     (127)    20646 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/justdeepit/app/static/utils.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:03:18.308703 JustDeepIt-0.2.4/justdeepit/app/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/justdeepit/app/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)    17454 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/justdeepit/app/templates/module.html
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/justdeepit/app/templates/shutdown.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:03:18.308703 JustDeepIt-0.2.4/justdeepit/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/justdeepit/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/justdeepit/models/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12931 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/justdeepit/models/instance_segment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13500 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/justdeepit/models/object_detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12227 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/justdeepit/models/salient_object_detect.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:03:18.308703 JustDeepIt-0.2.4/justdeepit/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/justdeepit/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6720 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/justdeepit/models/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13893 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/justdeepit/models/utils/mmdetbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36052 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/justdeepit/models/utils/u2net.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10173 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/justdeepit/models/utils/unet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:03:18.300703 JustDeepIt-0.2.4/justdeepit/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:03:18.312703 JustDeepIt-0.2.4/justdeepit/src/font/
+-rw-r--r--   0 runner    (1001) docker     (127)   555264 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/justdeepit/src/font/NotoSans-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/justdeepit/src/font/OFL.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    56860 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/justdeepit/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 06:03:18.312703 JustDeepIt-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-28 06:01:16.000000 JustDeepIt-0.2.4/setup.py
```

### Comparing `JustDeepIt-0.2.3/JustDeepIt.egg-info/PKG-INFO` & `JustDeepIt-0.2.4/JustDeepIt.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JustDeepIt
-Version: 0.2.3
+Version: 0.2.4
 Summary: a GUI tool for object detection and segmentation based on deep learning
 Home-page: https://github.com/biunit/JustDeepIt
 Author: Jianqiang Sun
 Author-email: sun@biunit.dev
 License: MIT
 Keywords: object detection,object segmentation
 Platform: UNKNOWN
```

### Comparing `JustDeepIt-0.2.3/JustDeepIt.egg-info/SOURCES.txt` & `JustDeepIt-0.2.4/JustDeepIt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.3/LICENSE` & `JustDeepIt-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.3/PKG-INFO` & `JustDeepIt-0.2.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JustDeepIt
-Version: 0.2.3
+Version: 0.2.4
 Summary: a GUI tool for object detection and segmentation based on deep learning
 Home-page: https://github.com/biunit/JustDeepIt
 Author: Jianqiang Sun
 Author-email: sun@biunit.dev
 License: MIT
 Keywords: object detection,object segmentation
 Platform: UNKNOWN
```

### Comparing `JustDeepIt-0.2.3/README.md` & `JustDeepIt-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.3/justdeepit/app/app.py` & `JustDeepIt-0.2.4/justdeepit/app/app.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.3/justdeepit/app/appbase.py` & `JustDeepIt-0.2.4/justdeepit/app/appbase.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.3/justdeepit/app/appis.py` & `JustDeepIt-0.2.4/justdeepit/app/appis.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.3/justdeepit/app/appod.py` & `JustDeepIt-0.2.4/justdeepit/app/appod.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.3/justdeepit/app/appsod.py` & `JustDeepIt-0.2.4/justdeepit/app/appsod.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.3/justdeepit/app/static/jquery-3.6.0.min.js` & `JustDeepIt-0.2.4/justdeepit/app/static/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.3/justdeepit/app/static/jquery-3.6.0.min.map` & `JustDeepIt-0.2.4/justdeepit/app/static/jquery-3.6.0.min.map`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/code.png` & `JustDeepIt-0.2.4/justdeepit/app/static/jqueryfiletree/images/code.png`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/css.png` & `JustDeepIt-0.2.4/justdeepit/app/static/jqueryfiletree/images/css.png`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/db.png` & `JustDeepIt-0.2.4/justdeepit/app/static/jqueryfiletree/images/db.png`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/directory-lock.png` & `JustDeepIt-0.2.4/justdeepit/app/static/jqueryfiletree/images/directory-lock.png`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/directory.png` & `JustDeepIt-0.2.4/justdeepit/app/static/jqueryfiletree/images/directory.png`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/doc.png` & `JustDeepIt-0.2.4/justdeepit/app/static/jqueryfiletree/images/doc.png`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/file-lock.png` & `JustDeepIt-0.2.4/justdeepit/app/static/jqueryfiletree/images/file-lock.png`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/film.png` & `JustDeepIt-0.2.4/justdeepit/app/static/jqueryfiletree/images/film.png`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/flash.png` & `JustDeepIt-0.2.4/justdeepit/app/static/jqueryfiletree/images/flash.png`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/folder_open.png` & `JustDeepIt-0.2.4/justdeepit/app/static/jqueryfiletree/images/folder_open.png`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/html.png` & `JustDeepIt-0.2.4/justdeepit/app/static/jqueryfiletree/images/html.png`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/java.png` & `JustDeepIt-0.2.4/justdeepit/app/static/jqueryfiletree/images/java.png`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/linux.png` & `JustDeepIt-0.2.4/justdeepit/app/static/jqueryfiletree/images/linux.png`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/pdf.png` & `JustDeepIt-0.2.4/justdeepit/app/static/jqueryfiletree/images/pdf.png`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/php.png` & `JustDeepIt-0.2.4/justdeepit/app/static/jqueryfiletree/images/php.png`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/picture.png` & `JustDeepIt-0.2.4/justdeepit/app/static/jqueryfiletree/images/picture.png`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/ppt.png` & `JustDeepIt-0.2.4/justdeepit/app/static/jqueryfiletree/images/ppt.png`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/psd.png` & `JustDeepIt-0.2.4/justdeepit/app/static/jqueryfiletree/images/psd.png`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/ruby.png` & `JustDeepIt-0.2.4/justdeepit/app/static/jqueryfiletree/images/ruby.png`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/script.png` & `JustDeepIt-0.2.4/justdeepit/app/static/jqueryfiletree/images/script.png`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/spinner.gif` & `JustDeepIt-0.2.4/justdeepit/app/static/jqueryfiletree/images/spinner.gif`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/images/xls.png` & `JustDeepIt-0.2.4/justdeepit/app/static/jqueryfiletree/images/xls.png`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/jQueryFileTree.css` & `JustDeepIt-0.2.4/justdeepit/app/static/jqueryfiletree/jQueryFileTree.css`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.3/justdeepit/app/static/jqueryfiletree/jQueryFileTree.js` & `JustDeepIt-0.2.4/justdeepit/app/static/jqueryfiletree/jQueryFileTree.js`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.3/justdeepit/app/static/styles.css` & `JustDeepIt-0.2.4/justdeepit/app/static/styles.css`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.3/justdeepit/app/static/utils.js` & `JustDeepIt-0.2.4/justdeepit/app/static/utils.js`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.3/justdeepit/app/templates/index.html` & `JustDeepIt-0.2.4/justdeepit/app/templates/index.html`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.3/justdeepit/app/templates/module.html` & `JustDeepIt-0.2.4/justdeepit/app/templates/module.html`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.3/justdeepit/app/templates/shutdown.html` & `JustDeepIt-0.2.4/justdeepit/app/templates/shutdown.html`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.3/justdeepit/models/instance_segment.py` & `JustDeepIt-0.2.4/justdeepit/models/instance_segment.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.3/justdeepit/models/object_detect.py` & `JustDeepIt-0.2.4/justdeepit/models/object_detect.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.3/justdeepit/models/salient_object_detect.py` & `JustDeepIt-0.2.4/justdeepit/models/salient_object_detect.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.3/justdeepit/models/utils/data.py` & `JustDeepIt-0.2.4/justdeepit/models/utils/data.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.3/justdeepit/models/utils/mmdetbase.py` & `JustDeepIt-0.2.4/justdeepit/models/utils/mmdetbase.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import numpy as np
 import pandas as pd
 import skimage
 import skimage.measure
 import PIL
 import torch
 import torch.multiprocessing
+import justdeepit
 from justdeepit.models.abstract import ModuleTemplate, JDIError
 from justdeepit.utils import ImageAnnotation, ImageAnnotations, load_images
 from justdeepit.models.utils.data import DataClass, DataPipeline, DataLoader
 
 logger = logging.getLogger(__name__)
 
 try:
@@ -74,14 +75,15 @@
         self.model_class = model_class
         self.cfg_fpath = model_config
         self.cfg = self.__set_config(model_config, model_weight, self.class_labels.class_labels)
         self.cfg.work_dir = os.path.abspath(self.workspace)
         logger.info(f'The workspace is set to `{self.workspace}`. '
                     f'Please locate the intermediate and final results '
                     f'within this workspace.')
+        self.mmdet_log_fpath = None
         
         # random seed
         if seed is None:
             seed = int(datetime.datetime.utcnow().timestamp())
         self.cfg.seed = seed
     
     
@@ -190,14 +192,15 @@
         else:
             raise ValueError('The model class is not supported.')
         self.cfg.merge_from_dict(dataloader.cfg)
         self.cfg.default_hooks.checkpoint.interval = 10
 
         # training
         runner = mmengine.runner.Runner.from_cfg(self.cfg)
+        self.mmdet_log_dpath = os.path.join(self.cfg.work_dir, runner.timestamp)
         runner.train()
     
     
     
     def __set_device(self, gpu=0):
         if gpu != 0 and gpu != 1:
             raise JDIError('The current JustDeepIt does not support multiple GPUs for trianing. '
@@ -244,58 +247,57 @@
         with open(os.path.join(self.cfg.work_dir, 'last_checkpoint')) as chkf:
             shutil.copy2(chkf.readline().strip(), weight_fpath)
         # config
         if config_fpath is None:
             config_fpath = os.path.splitext(weight_fpath)[0] + '.py'
         self.cfg.dump(config_fpath)
         # train log
-        self.parse_trainlog(os.path.splitext(weight_fpath)[0] + '.log')
+        self.save_trainlog(os.path.splitext(weight_fpath)[0] + '.log')
 
 
 
-    def parse_trainlog(self, output_prefix=None):
-        # get the latest log files
-        latest_log_dpath = self.__get_latest_trainlog(self.cfg.work_dir)
-        
+    def save_trainlog(self, output_prefix=None):
+        log_fpath = os.path.join(self.mmdet_log_dpath, 'vis_data', 'scalars.json')
+        #if not os.path.exists(log_fpath):
+        #    log_fpath = os.path.join(self.cfg.work_dir, self.cfg.experiment_name,
+        #                             f'{self.cfg.experiment_name}.log')
         train_log = []
         valid_log = []
-        test_log = []
-
-        with open(latest_log_dpath) as fh:
-            for log_line in fh:
-                if 'coco/bbox_mAP' in log_line:
-                    valid_log.append(log_line)
-                else:
-                    train_log.append(log_line)
-
-        train_log = pd.DataFrame(json.loads('[' + ','.join(train_log) + ']')).groupby('epoch').sum().drop(columns=['iter', 'step'])
 
+        if log_fpath.endswith('.json'):
+            train_log, valid_log = self.__parse_trainlog_json(log_fpath)
+        
         if output_prefix is not None:
-            train_log.to_csv(output_prefix + '.train.txt',
-                header=True, index=True, sep='\t')
+            if len(train_log) > 0:
+                train_log.to_csv(output_prefix + '.train.txt',
+                                 header=True, index=True, sep='\t')
+            if len(valid_log) > 0:
+                pd.DataFrame(
+                    json.loads('[' + ','.join(valid_log) + ']')
+                ).to_csv(output_prefix + '.valid.txt', header=True, index=False, sep='\t')
 
-        if output_prefix is not None and len(valid_log) > 0:
-            pd.DataFrame(json.loads('[' + ','.join(valid_log) + ']')).to_csv(output_prefix + '.valid.txt',
-                header=True, index=False, sep='\t')
 
 
+    def __parse_trainlog_json(self, log_fpath):
+        train_log = []
+        valid_log = []
+        with open(log_fpath) as fh:
+            for log_data in fh:
+                if 'coco/bbox_mAP' in log_data:
+                    valid_log.append(log_data)
+                else:
+                    train_log.append(log_data)
+            train_log = (
+                    pd.DataFrame(json.loads('[' + ','.join(train_log) + ']'))
+                        .groupby('epoch')
+                        .sum()
+                        .drop(columns=['iter', 'step'])
+                )
+        return train_log, valid_log
 
-    def __get_latest_trainlog(self, log_dpath):
-        latest_log_dpath = None
-        max_timestamp_ = 0
-        for fpath in glob.glob(os.path.join(log_dpath, '*')):
-            if os.path.isdir(fpath):
-                log_dpath = os.path.basename(fpath)
-                if len(os.path.basename(log_dpath)) == 15 and log_dpath[8] == '_':
-                    timesamp_ = int(log_dpath[0:8] + log_dpath[9:])
-                    if timesamp_ > max_timestamp_:
-                        max_timestamp_ = timesamp_
-                        latest_log_dpath = os.path.join(self.cfg.work_dir, log_dpath,
-                            'vis_data', 'scalars.json')
-        return latest_log_dpath
 
 
 
     def inference(self,
                   images,
                   score_cutoff=0.5,
                   batchsize=8,
@@ -318,15 +320,15 @@
                 persistent_workers=True,
                 drop_last=False,
                 sampler=dict(type='DefaultSampler', shuffle=False),
                 dataset=dict(
                     type='CocoDataset',
                     pipeline = pipeline.inference,
                     metainfo=self.cfg.metainfo))))
-
+ 
         # load model
         model = mmdet.apis.init_detector(self.cfg,
                                          self.cfg.load_from,
                                          device=self.cfg.device)
         
         # inference
         outputs = mmdet.apis.inference_detector(model, target_images)
```

### Comparing `JustDeepIt-0.2.3/justdeepit/models/utils/u2net.py` & `JustDeepIt-0.2.4/justdeepit/models/utils/u2net.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.3/justdeepit/models/utils/unet.py` & `JustDeepIt-0.2.4/justdeepit/models/utils/unet.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.3/justdeepit/src/font/NotoSans-Medium.ttf` & `JustDeepIt-0.2.4/justdeepit/src/font/NotoSans-Medium.ttf`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.3/justdeepit/src/font/OFL.txt` & `JustDeepIt-0.2.4/justdeepit/src/font/OFL.txt`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.3/justdeepit/utils.py` & `JustDeepIt-0.2.4/justdeepit/utils.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.2.3/setup.py` & `JustDeepIt-0.2.4/setup.py`

 * *Files identical despite different names*

