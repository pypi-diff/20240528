# Comparing `tmp/django-jalali-date-1.1.0.tar.gz` & `tmp/django_jalali_date-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-jalali-date-1.1.0.tar", last modified: Fri Dec 29 09:22:41 2023, max compression
+gzip compressed data, was "django_jalali_date-1.1.1.tar", last modified: Tue May 28 06:09:22 2024, max compression
```

## Comparing `django-jalali-date-1.1.0.tar` & `django_jalali_date-1.1.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-12-29 09:22:41.462859 django-jalali-date-1.1.0/
--rwxrwxrwx   0 root         (0) root         (0)     1070 2019-06-20 10:43:45.000000 django-jalali-date-1.1.0/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)       99 2019-06-20 10:43:45.000000 django-jalali-date-1.1.0/MANIFEST.in
--rwxrwxrwx   0 root         (0) root         (0)     8539 2023-12-29 09:22:41.463302 django-jalali-date-1.1.0/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     6166 2023-12-29 08:25:50.000000 django-jalali-date-1.1.0/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-12-29 09:22:41.411048 django-jalali-date-1.1.0/django_jalali_date.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     8539 2023-12-29 09:22:41.000000 django-jalali-date-1.1.0/django_jalali_date.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     2234 2023-12-29 09:22:41.000000 django-jalali-date-1.1.0/django_jalali_date.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-12-29 09:22:41.000000 django-jalali-date-1.1.0/django_jalali_date.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2019-06-23 18:27:50.000000 django-jalali-date-1.1.0/django_jalali_date.egg-info/not-zip-safe
--rwxrwxrwx   0 root         (0) root         (0)       17 2023-12-29 09:22:41.000000 django-jalali-date-1.1.0/django_jalali_date.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       12 2023-12-29 09:22:41.000000 django-jalali-date-1.1.0/django_jalali_date.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-12-29 09:22:41.416117 django-jalali-date-1.1.0/jalali_date/
--rwxrwxrwx   0 root         (0) root         (0)      523 2019-06-20 10:43:45.000000 django-jalali-date-1.1.0/jalali_date/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3401 2023-12-29 08:02:43.000000 django-jalali-date-1.1.0/jalali_date/admin.py
--rwxrwxrwx   0 root         (0) root         (0)     1930 2019-06-20 10:43:45.000000 django-jalali-date-1.1.0/jalali_date/fields.py
--rwxrwxrwx   0 root         (0) root         (0)     1277 2023-12-29 08:02:43.000000 django-jalali-date-1.1.0/jalali_date/settings.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-12-29 09:22:41.399883 django-jalali-date-1.1.0/jalali_date/static/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-12-29 09:22:41.401210 django-jalali-date-1.1.0/jalali_date/static/admin/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-12-29 09:22:41.417034 django-jalali-date-1.1.0/jalali_date/static/admin/jquery.ui.datepicker.jalali/
--rwxrwxrwx   0 root         (0) root         (0)     9386 2019-06-20 10:43:45.000000 django-jalali-date-1.1.0/jalali_date/static/admin/jquery.ui.datepicker.jalali/default.htm
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-12-29 09:22:41.432167 django-jalali-date-1.1.0/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/
--rwxrwxrwx   0 root         (0) root         (0)    45960 2019-06-20 10:43:45.000000 django-jalali-date-1.1.0/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/calendar.all.js
--rwxrwxrwx   0 root         (0) root         (0)     3991 2019-06-20 10:43:45.000000 django-jalali-date-1.1.0/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/calendar.js
--rwxrwxrwx   0 root         (0) root         (0)    93107 2019-06-20 10:43:45.000000 django-jalali-date-1.1.0/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery-1.10.2.min.js
--rwxrwxrwx   0 root         (0) root         (0)   140036 2019-06-20 10:43:45.000000 django-jalali-date-1.1.0/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery-1.10.2.min.map
--rwxrwxrwx   0 root         (0) root         (0)     8198 2019-06-20 10:43:45.000000 django-jalali-date-1.1.0/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery.ui.core.js
--rwxrwxrwx   0 root         (0) root         (0)     4296 2020-02-09 19:52:55.000000 django-jalali-date-1.1.0/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery.ui.datepicker-cc-fa.js
--rwxrwxrwx   0 root         (0) root         (0)    77969 2019-06-20 10:43:45.000000 django-jalali-date-1.1.0/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery.ui.datepicker-cc.js
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-12-29 09:22:41.400732 django-jalali-date-1.1.0/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-12-29 09:22:41.434446 django-jalali-date-1.1.0/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-12-29 09:22:41.441251 django-jalali-date-1.1.0/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/
--rwxrwxrwx   0 root         (0) root         (0)     6992 2019-06-20 10:43:45.000000 django-jalali-date-1.1.0/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_444444_256x240.png
--rwxrwxrwx   0 root         (0) root         (0)     6988 2019-06-20 10:43:45.000000 django-jalali-date-1.1.0/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_555555_256x240.png
--rwxrwxrwx   0 root         (0) root         (0)     4549 2019-06-20 10:43:45.000000 django-jalali-date-1.1.0/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_777620_256x240.png
--rwxrwxrwx   0 root         (0) root         (0)     6999 2019-06-20 10:43:45.000000 django-jalali-date-1.1.0/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_777777_256x240.png
--rwxrwxrwx   0 root         (0) root         (0)     4549 2019-06-20 10:43:45.000000 django-jalali-date-1.1.0/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_cc0000_256x240.png
--rwxrwxrwx   0 root         (0) root         (0)     6299 2019-06-20 10:43:45.000000 django-jalali-date-1.1.0/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_ffffff_256x240.png
--rwxrwxrwx   0 root         (0) root         (0)    19200 2019-06-20 10:43:45.000000 django-jalali-date-1.1.0/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/jquery-ui.min.css
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-12-29 09:22:41.452351 django-jalali-date-1.1.0/jalali_date/static/admin/js/
--rwxrwxrwx   0 root         (0) root         (0)   254855 2021-06-04 16:08:38.000000 django-jalali-date-1.1.0/jalali_date/static/admin/js/django_jalali..js
--rwxrwxrwx   0 root         (0) root         (0)   139534 2021-06-04 16:08:38.000000 django-jalali-date-1.1.0/jalali_date/static/admin/js/django_jalali.min.js
--rwxrwxrwx   0 root         (0) root         (0)      306 2021-06-04 16:07:42.000000 django-jalali-date-1.1.0/jalali_date/static/admin/js/main.js
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-12-29 09:22:41.401607 django-jalali-date-1.1.0/jalali_date/templates/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-12-29 09:22:41.453294 django-jalali-date-1.1.0/jalali_date/templates/admin/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-12-29 09:22:41.455469 django-jalali-date-1.1.0/jalali_date/templates/admin/edit_inline/
--rwxrwxrwx   0 root         (0) root         (0)     2365 2019-12-20 13:00:49.000000 django-jalali-date-1.1.0/jalali_date/templates/admin/edit_inline/jalali_stacked.html
--rwxrwxrwx   0 root         (0) root         (0)     4301 2019-12-20 13:00:49.000000 django-jalali-date-1.1.0/jalali_date/templates/admin/edit_inline/jalali_tabular.html
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-12-29 09:22:41.456980 django-jalali-date-1.1.0/jalali_date/templates/admin/includes/
--rwxrwxrwx   0 root         (0) root         (0)     2232 2023-12-29 07:46:19.000000 django-jalali-date-1.1.0/jalali_date/templates/admin/includes/jalali_fieldset.html
--rwxrwxrwx   0 root         (0) root         (0)      191 2019-06-20 10:43:45.000000 django-jalali-date-1.1.0/jalali_date/templates/admin/jalali_change_form.html
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-12-29 09:22:41.460094 django-jalali-date-1.1.0/jalali_date/templates/admin/widgets/
--rwxrwxrwx   0 root         (0) root         (0)      234 2020-02-07 19:35:37.000000 django-jalali-date-1.1.0/jalali_date/templates/admin/widgets/jalali_split_datetime.html
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-12-29 09:22:41.461953 django-jalali-date-1.1.0/jalali_date/templatetags/
--rwxrwxrwx   0 root         (0) root         (0)        0 2019-06-20 10:43:45.000000 django-jalali-date-1.1.0/jalali_date/templatetags/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     2002 2019-12-20 13:00:49.000000 django-jalali-date-1.1.0/jalali_date/templatetags/jalali_tags.py
--rwxrwxrwx   0 root         (0) root         (0)     2055 2021-12-13 19:19:21.000000 django-jalali-date-1.1.0/jalali_date/widgets.py
--rwxrwxrwx   0 root         (0) root         (0)       76 2023-12-29 09:22:41.464185 django-jalali-date-1.1.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1335 2023-12-29 08:10:20.000000 django-jalali-date-1.1.0/setup.py
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2024-05-28 06:09:22.442904 django_jalali_date-1.1.1/
+-rw-rw-r--   0 arman     (1000) arman     (1000)     1070 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/LICENSE
+-rw-rw-r--   0 arman     (1000) arman     (1000)       99 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/MANIFEST.in
+-rw-r--r--   0 arman     (1000) arman     (1000)     7115 2024-05-28 06:09:22.442904 django_jalali_date-1.1.1/PKG-INFO
+-rw-rw-r--   0 arman     (1000) arman     (1000)     6166 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/README.md
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2024-05-28 06:09:22.442904 django_jalali_date-1.1.1/django_jalali_date.egg-info/
+-rw-r--r--   0 arman     (1000) arman     (1000)     7115 2024-05-28 06:09:22.000000 django_jalali_date-1.1.1/django_jalali_date.egg-info/PKG-INFO
+-rw-rw-r--   0 arman     (1000) arman     (1000)     2234 2024-05-28 06:09:22.000000 django_jalali_date-1.1.1/django_jalali_date.egg-info/SOURCES.txt
+-rw-rw-r--   0 arman     (1000) arman     (1000)        1 2024-05-28 06:09:22.000000 django_jalali_date-1.1.1/django_jalali_date.egg-info/dependency_links.txt
+-rw-rw-r--   0 arman     (1000) arman     (1000)        1 2024-05-28 06:09:22.000000 django_jalali_date-1.1.1/django_jalali_date.egg-info/not-zip-safe
+-rw-rw-r--   0 arman     (1000) arman     (1000)       17 2024-05-28 06:09:22.000000 django_jalali_date-1.1.1/django_jalali_date.egg-info/requires.txt
+-rw-rw-r--   0 arman     (1000) arman     (1000)       12 2024-05-28 06:09:22.000000 django_jalali_date-1.1.1/django_jalali_date.egg-info/top_level.txt
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2024-05-28 06:09:22.434904 django_jalali_date-1.1.1/jalali_date/
+-rw-rw-r--   0 arman     (1000) arman     (1000)      523 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/jalali_date/__init__.py
+-rw-rw-r--   0 arman     (1000) arman     (1000)     3401 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/jalali_date/admin.py
+-rw-rw-r--   0 arman     (1000) arman     (1000)     1930 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/jalali_date/fields.py
+-rw-rw-r--   0 arman     (1000) arman     (1000)     1277 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/jalali_date/settings.py
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2024-05-28 06:09:22.434904 django_jalali_date-1.1.1/jalali_date/static/
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2024-05-28 06:09:22.434904 django_jalali_date-1.1.1/jalali_date/static/admin/
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2024-05-28 06:09:22.434904 django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/
+-rw-rw-r--   0 arman     (1000) arman     (1000)     9386 2024-05-28 05:49:47.000000 django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/default.htm
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2024-05-28 06:09:22.434904 django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/
+-rw-rw-r--   0 arman     (1000) arman     (1000)    45960 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/calendar.all.js
+-rw-rw-r--   0 arman     (1000) arman     (1000)     3991 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/calendar.js
+-rw-rw-r--   0 arman     (1000) arman     (1000)    93107 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery-1.10.2.min.js
+-rw-rw-r--   0 arman     (1000) arman     (1000)   140036 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery-1.10.2.min.map
+-rw-rw-r--   0 arman     (1000) arman     (1000)     8198 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery.ui.core.js
+-rw-rw-r--   0 arman     (1000) arman     (1000)     4296 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery.ui.datepicker-cc-fa.js
+-rw-rw-r--   0 arman     (1000) arman     (1000)    77969 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery.ui.datepicker-cc.js
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2024-05-28 06:09:22.434904 django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2024-05-28 06:09:22.434904 django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2024-05-28 06:09:22.438904 django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/
+-rw-rw-r--   0 arman     (1000) arman     (1000)     6992 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_444444_256x240.png
+-rw-rw-r--   0 arman     (1000) arman     (1000)     6988 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_555555_256x240.png
+-rw-rw-r--   0 arman     (1000) arman     (1000)     4549 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_777620_256x240.png
+-rw-rw-r--   0 arman     (1000) arman     (1000)     6999 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_777777_256x240.png
+-rw-rw-r--   0 arman     (1000) arman     (1000)     4549 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_cc0000_256x240.png
+-rw-rw-r--   0 arman     (1000) arman     (1000)     6299 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_ffffff_256x240.png
+-rw-rw-r--   0 arman     (1000) arman     (1000)    19200 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/jquery-ui.min.css
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2024-05-28 06:09:22.438904 django_jalali_date-1.1.1/jalali_date/static/admin/js/
+-rw-rw-r--   0 arman     (1000) arman     (1000)   254920 2024-05-28 05:45:55.000000 django_jalali_date-1.1.1/jalali_date/static/admin/js/django_jalali..js
+-rw-rw-r--   0 arman     (1000) arman     (1000)   139578 2024-05-28 05:49:08.000000 django_jalali_date-1.1.1/jalali_date/static/admin/js/django_jalali.min.js
+-rw-rw-r--   0 arman     (1000) arman     (1000)      338 2024-05-28 05:45:58.000000 django_jalali_date-1.1.1/jalali_date/static/admin/js/main.js
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2024-05-28 06:09:22.434904 django_jalali_date-1.1.1/jalali_date/templates/
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2024-05-28 06:09:22.438904 django_jalali_date-1.1.1/jalali_date/templates/admin/
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2024-05-28 06:09:22.438904 django_jalali_date-1.1.1/jalali_date/templates/admin/edit_inline/
+-rw-rw-r--   0 arman     (1000) arman     (1000)     2365 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/jalali_date/templates/admin/edit_inline/jalali_stacked.html
+-rw-rw-r--   0 arman     (1000) arman     (1000)     4301 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/jalali_date/templates/admin/edit_inline/jalali_tabular.html
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2024-05-28 06:09:22.442904 django_jalali_date-1.1.1/jalali_date/templates/admin/includes/
+-rw-rw-r--   0 arman     (1000) arman     (1000)     2232 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/jalali_date/templates/admin/includes/jalali_fieldset.html
+-rw-rw-r--   0 arman     (1000) arman     (1000)      191 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/jalali_date/templates/admin/jalali_change_form.html
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2024-05-28 06:09:22.442904 django_jalali_date-1.1.1/jalali_date/templates/admin/widgets/
+-rw-rw-r--   0 arman     (1000) arman     (1000)      234 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/jalali_date/templates/admin/widgets/jalali_split_datetime.html
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2024-05-28 06:09:22.442904 django_jalali_date-1.1.1/jalali_date/templatetags/
+-rw-rw-r--   0 arman     (1000) arman     (1000)        0 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/jalali_date/templatetags/__init__.py
+-rw-rw-r--   0 arman     (1000) arman     (1000)     2002 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/jalali_date/templatetags/jalali_tags.py
+-rw-rw-r--   0 arman     (1000) arman     (1000)     2055 2024-05-28 05:21:27.000000 django_jalali_date-1.1.1/jalali_date/widgets.py
+-rw-rw-r--   0 arman     (1000) arman     (1000)       76 2024-05-28 06:09:22.442904 django_jalali_date-1.1.1/setup.cfg
+-rw-rw-r--   0 arman     (1000) arman     (1000)     1335 2024-05-28 05:57:42.000000 django_jalali_date-1.1.1/setup.py
```

### Comparing `django-jalali-date-1.1.0/LICENSE` & `django_jalali_date-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-jalali-date-1.1.0/PKG-INFO` & `django_jalali_date-1.1.1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,206 +1,185 @@
-Metadata-Version: 2.1
-Name: django-jalali-date
-Version: 1.1.0
-Summary: Jalali Date support for user interface. Easy conversion of DateTimeFiled to JalaliDateTimeField within the admin site, views, forms and templates.
-Home-page: http://github.com/a-roomana/django-jalali-date
-Author: Arman Roomana
-Author-email: roomana.arman@gmail.com
-License: MIT
-Download-URL: https://pypi.python.org/pypi/django-jalali-date/
-Description: 
-        
-        [![PyPi Version](https://img.shields.io/pypi/v/django-jalali-date.svg)](https://pypi.python.org/pypi/django-jalali-date)
-        [![PyPI - Downloads](https://img.shields.io/pypi/dm/django-jalali-date.svg)](https://pypistats.org/packages/django-jalali-date)
-        [![GitHub stars](https://img.shields.io/github/stars/a-roomana/django-jalali-date.svg?style=social)](https://github.com/a-roomana/django-jalali-date)
-        # django-jalali-date
-        
-        Jalali Date support for user interface. Easy conversion of DateTimeField to JalaliDateTimeField within the admin site, view and templates.
-        
-        
-        ## Dependency
-        
-        To use this module you need to install jdatetime(and of course you need django) and pytz module which you can install it with easy_install or pip
-        
-        
-        ## Version Compatibility
-        #### Python
-        - python 3.8 and below is  compatible with 0.3.2 and below
-        - python 3.X and above is compatible with 1.0.0 and above
-        
-        #### Django
-        I tested the latest version on some Django versions on python 3.8
-        - django == 4.2
-        - django == 3.2.8
-        - django == 2.2.24
-        
-        I think it will work properly on other versions as well.
-        
-        If you plan to use it in Django 1.X, install version 0.3.2
-        
-        
-        
-        ## Install
-        
-            pip install django-jalali-date   
-        
-        
-        ## Usage
-        
-        #### settings.py
-        
-        - don't forget to make sure you've also added `jalali_date` to your `INSTALLED_APPS`.
-        - any global settings for a Django Jalali Date are kept in a single configuration dictionary named `JALALI_DATE_DEFAULTS`
-          - you can change the default display of dates by override `Strftime`
-          - you can use your own date picker by override `Static` 
-        ```python
-        INSTALLED_APPS = [
-        	'django_apps',
-        	
-        	'jalali_date',
-        	
-        	'my_apps',
-        ]
-        
-        # default settings (optional)
-        JALALI_DATE_DEFAULTS = {
-           # if change it to true then all dates of the list_display will convert to the Jalali.
-           'LIST_DISPLAY_AUTO_CONVERT': False,
-           'Strftime': {
-                'date': '%y/%m/%d',
-                'datetime': '%H:%M:%S _ %y/%m/%d',
-            },
-            'Static': {
-                'js': [
-                    # loading datepicker
-                    'admin/js/django_jalali.min.js',
-                    # OR
-                    # 'admin/jquery.ui.datepicker.jalali/scripts/jquery.ui.core.js',
-                    # 'admin/jquery.ui.datepicker.jalali/scripts/calendar.js',
-                    # 'admin/jquery.ui.datepicker.jalali/scripts/jquery.ui.datepicker-cc.js',
-                    # 'admin/jquery.ui.datepicker.jalali/scripts/jquery.ui.datepicker-cc-fa.js',
-                    # 'admin/js/main.js',
-                ],
-                'css': {
-                    'all': [
-                        'admin/jquery.ui.datepicker.jalali/themes/base/jquery-ui.min.css',
-                    ]
-                }
-            },
+
+
+[![PyPi Version](https://img.shields.io/pypi/v/django-jalali-date.svg)](https://pypi.python.org/pypi/django-jalali-date)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/django-jalali-date.svg)](https://pypistats.org/packages/django-jalali-date)
+[![GitHub stars](https://img.shields.io/github/stars/a-roomana/django-jalali-date.svg?style=social)](https://github.com/a-roomana/django-jalali-date)
+# django-jalali-date
+
+Jalali Date support for user interface. Easy conversion of DateTimeField to JalaliDateTimeField within the admin site, view and templates.
+
+
+## Dependency
+
+To use this module you need to install jdatetime(and of course you need django) and pytz module which you can install it with easy_install or pip
+
+
+## Version Compatibility
+#### Python
+- python 3.8 and below is  compatible with 0.3.2 and below
+- python 3.X and above is compatible with 1.0.0 and above
+
+#### Django
+I tested the latest version on some Django versions on python 3.8
+- django == 4.2
+- django == 3.2.8
+- django == 2.2.24
+
+I think it will work properly on other versions as well.
+
+If you plan to use it in Django 1.X, install version 0.3.2
+
+
+
+## Install
+
+    pip install django-jalali-date   
+
+
+## Usage
+
+#### settings.py
+
+- don't forget to make sure you've also added `jalali_date` to your `INSTALLED_APPS`.
+- any global settings for a Django Jalali Date are kept in a single configuration dictionary named `JALALI_DATE_DEFAULTS`
+  - you can change the default display of dates by override `Strftime`
+  - you can use your own date picker by override `Static` 
+```python
+INSTALLED_APPS = [
+	'django_apps',
+	
+	'jalali_date',
+	
+	'my_apps',
+]
+
+# default settings (optional)
+JALALI_DATE_DEFAULTS = {
+   # if change it to true then all dates of the list_display will convert to the Jalali.
+   'LIST_DISPLAY_AUTO_CONVERT': False,
+   'Strftime': {
+        'date': '%y/%m/%d',
+        'datetime': '%H:%M:%S _ %y/%m/%d',
+    },
+    'Static': {
+        'js': [
+            # loading datepicker
+            'admin/js/django_jalali.min.js',
+            # OR
+            # 'admin/jquery.ui.datepicker.jalali/scripts/jquery.ui.core.js',
+            # 'admin/jquery.ui.datepicker.jalali/scripts/calendar.js',
+            # 'admin/jquery.ui.datepicker.jalali/scripts/jquery.ui.datepicker-cc.js',
+            # 'admin/jquery.ui.datepicker.jalali/scripts/jquery.ui.datepicker-cc-fa.js',
+            # 'admin/js/main.js',
+        ],
+        'css': {
+            'all': [
+                'admin/jquery.ui.datepicker.jalali/themes/base/jquery-ui.min.css',
+            ]
         }
-        ```
-        
-        (Optional) If you want the names of the dates to be displayed in Farsi, please add the following command to the settings.
-        
-        If you are on windows:
-        ```python
-        LANGUAGE_CODE = 'fa'
-        
-        import locale
-        locale.setlocale(locale.LC_ALL, "Persian_Iran.UTF-8")
-        ```
-        If you are on other operating systems:
-        ```python
-        LANGUAGE_CODE = 'fa'
-        
-        import locale
-        locale.setlocale(locale.LC_ALL, "fa_IR.UTF-8")
-        ```
-        
-        
-        #### views.py
-        ```python
-        from jalali_date import datetime2jalali, date2jalali
-        
-        def my_view(request):
-        	jalali_join = datetime2jalali(request.user.date_joined).strftime('%y/%m/%d _ %H:%M:%S')
-        ```
-        #### forms.py
-        ```python
-        from django import forms
-        from jalali_date.fields import JalaliDateField, SplitJalaliDateTimeField
-        from jalali_date.widgets import AdminJalaliDateWidget, AdminSplitJalaliDateTime
-        
-        
-        class TestForm(forms.ModelForm):
-            class Meta:
-                model = TestModel
-                fields = ('name', 'date', 'date_time')
-        
-            def __init__(self, *args, **kwargs):
-                super(TestForm, self).__init__(*args, **kwargs)
-                self.fields['date'] = JalaliDateField(label=_('date'), # date format is  "yyyy-mm-dd"
-                    widget=AdminJalaliDateWidget # optional, to use default datepicker
-                )
-        
-                # you can added a "class" to this field for use your datepicker!
-                # self.fields['date'].widget.attrs.update({'class': 'jalali_date-date'})
-        
-                self.fields['date_time'] = SplitJalaliDateTimeField(label=_('date time'), 
-                    widget=AdminSplitJalaliDateTime # required, for decompress DatetimeField to JalaliDateField and JalaliTimeField
-                )
-        ```
-        
-        #### template.html
-        ```html    
-        {% load jalali_tags %}
-        
-        <p>{{ request.user.date_joined|to_jalali:'%y/%m/%d _ %H:%M:%S' }}</p>
-        
-        <form method="post">{% csrf_token %}
-            {{ form.as_p }}
-            <input type="submit">
-        </form>
-        
-        <!-- By default, Datepicker using jQuery, you need to set your script after loading jQuery! -->
-        	<!-- loading directly -->
-        		<link rel="stylesheet" href="{% static 'admin/jquery.ui.datepicker.jalali/themes/base/jquery-ui.min.css' %}">
-        		<script src="{% static 'admin/js/django_jalali.min.js' %}"></script>
-        	<!-- OR -->
-        	<!-- loading by form (if used AdminJalaliDateWidget) -->
-        		{{ form.media }}
-        ```
-        ![example-template-form](http://bayanbox.ir/view/4091856023129600494/photo-2019-04-06-11-11-03-min.jpg)
-        
-        #### admin.py
-        ```python
-        from django.contrib import admin
-        from jalali_date import datetime2jalali, date2jalali
-        from jalali_date.admin import ModelAdminJalaliMixin, StackedInlineJalaliMixin, TabularInlineJalaliMixin	
-            
-        class MyInlines1(TabularInlineJalaliMixin, admin.TabularInline):
-        	model = SecendModel
-        
-        class MyInlines2(StackedInlineJalaliMixin, admin.StackedInline):
-        	model = ThirdModel
-        	
-        @admin.register(FirstModel)
-        class FirstModelAdmin(ModelAdminJalaliMixin, admin.ModelAdmin):
-        	#for showing the Jalali date on the list_display, please change the LIST_DISPLAY_AUTO_CONVERT to true or create custom methods. for example:
-            list_display = ['some_fields', 'get_created_jalali']
-        	
-        	inlines = (MyInlines1, MyInlines2, )
-        	raw_id_fields = ('some_fields', )
-        	readonly_fields = ('some_fields', 'date_field',)
-        	# you can override formfield, for example:
-        	formfield_overrides = {
-        	    JSONField: {'widget': JSONEditor},
-        	}
-        	
-        	@admin.display(description='تاریخ ایجاد', ordering='created')
-        	def get_created_jalali(self, obj):
-        		return datetime2jalali(obj.created).strftime('%a, %d %b %Y %H:%M:%S')
-        ```
-        ![list-display](https://bayanbox.ir/view/6588806159227221741/Screenshot-from-2023-12-29-11-42-24.png)
-        ![example-admin](http://bayanbox.ir/view/2877111068605695571/Screenshot-from-2016-07-26-01-37-07.png)
-        
-Keywords: django jalali date
-Platform: any
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3
-Description-Content-Type: text/markdown
+    },
+}
+```
+
+(Optional) If you want the names of the dates to be displayed in Farsi, please add the following command to the settings.
+
+If you are on windows:
+```python
+LANGUAGE_CODE = 'fa'
+
+import locale
+locale.setlocale(locale.LC_ALL, "Persian_Iran.UTF-8")
+```
+If you are on other operating systems:
+```python
+LANGUAGE_CODE = 'fa'
+
+import locale
+locale.setlocale(locale.LC_ALL, "fa_IR.UTF-8")
+```
+
+
+#### views.py
+```python
+from jalali_date import datetime2jalali, date2jalali
+
+def my_view(request):
+	jalali_join = datetime2jalali(request.user.date_joined).strftime('%y/%m/%d _ %H:%M:%S')
+```
+#### forms.py
+```python
+from django import forms
+from jalali_date.fields import JalaliDateField, SplitJalaliDateTimeField
+from jalali_date.widgets import AdminJalaliDateWidget, AdminSplitJalaliDateTime
+
+
+class TestForm(forms.ModelForm):
+    class Meta:
+        model = TestModel
+        fields = ('name', 'date', 'date_time')
+
+    def __init__(self, *args, **kwargs):
+        super(TestForm, self).__init__(*args, **kwargs)
+        self.fields['date'] = JalaliDateField(label=_('date'), # date format is  "yyyy-mm-dd"
+            widget=AdminJalaliDateWidget # optional, to use default datepicker
+        )
+
+        # you can added a "class" to this field for use your datepicker!
+        # self.fields['date'].widget.attrs.update({'class': 'jalali_date-date'})
+
+        self.fields['date_time'] = SplitJalaliDateTimeField(label=_('date time'), 
+            widget=AdminSplitJalaliDateTime # required, for decompress DatetimeField to JalaliDateField and JalaliTimeField
+        )
+```
+
+#### template.html
+```html    
+{% load jalali_tags %}
+
+<p>{{ request.user.date_joined|to_jalali:'%y/%m/%d _ %H:%M:%S' }}</p>
+
+<form method="post">{% csrf_token %}
+    {{ form.as_p }}
+    <input type="submit">
+</form>
+
+<!-- By default, Datepicker using jQuery, you need to set your script after loading jQuery! -->
+	<!-- loading directly -->
+		<link rel="stylesheet" href="{% static 'admin/jquery.ui.datepicker.jalali/themes/base/jquery-ui.min.css' %}">
+		<script src="{% static 'admin/js/django_jalali.min.js' %}"></script>
+	<!-- OR -->
+	<!-- loading by form (if used AdminJalaliDateWidget) -->
+		{{ form.media }}
+```
+![example-template-form](http://bayanbox.ir/view/4091856023129600494/photo-2019-04-06-11-11-03-min.jpg)
+
+#### admin.py
+```python
+from django.contrib import admin
+from jalali_date import datetime2jalali, date2jalali
+from jalali_date.admin import ModelAdminJalaliMixin, StackedInlineJalaliMixin, TabularInlineJalaliMixin	
+    
+class MyInlines1(TabularInlineJalaliMixin, admin.TabularInline):
+	model = SecendModel
+
+class MyInlines2(StackedInlineJalaliMixin, admin.StackedInline):
+	model = ThirdModel
+	
+@admin.register(FirstModel)
+class FirstModelAdmin(ModelAdminJalaliMixin, admin.ModelAdmin):
+	#for showing the Jalali date on the list_display, please change the LIST_DISPLAY_AUTO_CONVERT to true or create custom methods. for example:
+    list_display = ['some_fields', 'get_created_jalali']
+	
+	inlines = (MyInlines1, MyInlines2, )
+	raw_id_fields = ('some_fields', )
+	readonly_fields = ('some_fields', 'date_field',)
+	# you can override formfield, for example:
+	formfield_overrides = {
+	    JSONField: {'widget': JSONEditor},
+	}
+	
+	@admin.display(description='تاریخ ایجاد', ordering='created')
+	def get_created_jalali(self, obj):
+		return datetime2jalali(obj.created).strftime('%a, %d %b %Y %H:%M:%S')
+```
+![list-display](https://bayanbox.ir/view/6588806159227221741/Screenshot-from-2023-12-29-11-42-24.png)
+![example-admin](http://bayanbox.ir/view/2877111068605695571/Screenshot-from-2016-07-26-01-37-07.png)
```

### Comparing `django-jalali-date-1.1.0/README.md` & `django_jalali_date-1.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+Metadata-Version: 2.1
+Name: django-jalali-date
+Version: 1.1.1
+Summary: Jalali Date support for user interface. Easy conversion of DateTimeFiled to JalaliDateTimeField within the admin site, views, forms and templates.
+Home-page: http://github.com/a-roomana/django-jalali-date
+Download-URL: https://pypi.python.org/pypi/django-jalali-date/
+Author: Arman Roomana
+Author-email: roomana.arman@gmail.com
+License: MIT
+Keywords: django jalali date
+Platform: any
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Django
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: django
+Requires-Dist: jdatetime
+
 
 
 [![PyPi Version](https://img.shields.io/pypi/v/django-jalali-date.svg)](https://pypi.python.org/pypi/django-jalali-date)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/django-jalali-date.svg)](https://pypistats.org/packages/django-jalali-date)
 [![GitHub stars](https://img.shields.io/github/stars/a-roomana/django-jalali-date.svg?style=social)](https://github.com/a-roomana/django-jalali-date)
 # django-jalali-date
```

### Comparing `django-jalali-date-1.1.0/django_jalali_date.egg-info/SOURCES.txt` & `django_jalali_date-1.1.1/django_jalali_date.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-jalali-date-1.1.0/jalali_date/__init__.py` & `django_jalali_date-1.1.1/jalali_date/__init__.py`

 * *Files identical despite different names*

### Comparing `django-jalali-date-1.1.0/jalali_date/admin.py` & `django_jalali_date-1.1.1/jalali_date/admin.py`

 * *Files identical despite different names*

### Comparing `django-jalali-date-1.1.0/jalali_date/fields.py` & `django_jalali_date-1.1.1/jalali_date/fields.py`

 * *Files identical despite different names*

### Comparing `django-jalali-date-1.1.0/jalali_date/settings.py` & `django_jalali_date-1.1.1/jalali_date/settings.py`

 * *Files identical despite different names*

### Comparing `django-jalali-date-1.1.0/jalali_date/static/admin/jquery.ui.datepicker.jalali/default.htm` & `django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/default.htm`

 * *Files identical despite different names*

### Comparing `django-jalali-date-1.1.0/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/calendar.all.js` & `django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/calendar.all.js`

 * *Files identical despite different names*

### Comparing `django-jalali-date-1.1.0/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/calendar.js` & `django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/calendar.js`

 * *Files identical despite different names*

### Comparing `django-jalali-date-1.1.0/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery-1.10.2.min.js` & `django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery-1.10.2.min.js`

 * *Files identical despite different names*

### Comparing `django-jalali-date-1.1.0/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery-1.10.2.min.map` & `django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery-1.10.2.min.map`

 * *Files identical despite different names*

### Comparing `django-jalali-date-1.1.0/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery.ui.core.js` & `django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery.ui.core.js`

 * *Files identical despite different names*

### Comparing `django-jalali-date-1.1.0/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery.ui.datepicker-cc-fa.js` & `django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery.ui.datepicker-cc-fa.js`

 * *Files identical despite different names*

### Comparing `django-jalali-date-1.1.0/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery.ui.datepicker-cc.js` & `django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery.ui.datepicker-cc.js`

 * *Files identical despite different names*

### Comparing `django-jalali-date-1.1.0/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_444444_256x240.png` & `django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `django-jalali-date-1.1.0/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_555555_256x240.png` & `django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `django-jalali-date-1.1.0/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_777620_256x240.png` & `django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `django-jalali-date-1.1.0/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_777777_256x240.png` & `django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `django-jalali-date-1.1.0/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_cc0000_256x240.png` & `django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `django-jalali-date-1.1.0/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_ffffff_256x240.png` & `django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `django-jalali-date-1.1.0/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/jquery-ui.min.css` & `django_jalali_date-1.1.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `django-jalali-date-1.1.0/jalali_date/static/admin/js/django_jalali..js` & `django_jalali_date-1.1.1/jalali_date/static/admin/js/django_jalali..js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -8278,24 +8278,26 @@
         if (typeof django !== "undefined") {
             JQ = django.jQuery;
         }
         JQ(".jalali_date-date").datepicker({
             dateFormat: "yy-mm-dd",
             changeMonth: !0,
             changeYear: !0,
+            yearRange: "c-70:c+10",
         });
         $('.add-row').click(function() {
             let JQ = jQuery || {};
             if (typeof django !== "undefined") {
                 JQ = django.jQuery;
             }
             // set delay to verify thats the new row was successfully created
             setTimeout(function() {
                 console.log('add-row')
                 JQ(".jalali_date-date").datepicker({
                     dateFormat: "yy-mm-dd",
                     changeMonth: !0,
                     changeYear: !0,
+                    yearRange: "c-70:c+10",
                 });
             }, 300)
         })
     });
```

### Comparing `django-jalali-date-1.1.0/jalali_date/static/admin/js/django_jalali.min.js` & `django_jalali_date-1.1.1/jalali_date/static/admin/js/django_jalali.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -4250,19 +4250,21 @@
         }
     }, e.datepicker.setDefaults(e.datepicker.regional.fa)
 }), $(document).ready(function() {
     let e = jQuery || {};
     "undefined" != typeof django && (e = django.jQuery), e(".jalali_date-date").datepicker({
         dateFormat: "yy-mm-dd",
         changeMonth: !0,
-        changeYear: !0
+        changeYear: !0,
+        yearRange: "c-70:c+10"
     }), $(".add-row").click(function() {
         let e = jQuery || {};
         "undefined" != typeof django && (e = django.jQuery), setTimeout(function() {
             console.log("add-row"), e(".jalali_date-date").datepicker({
                 dateFormat: "yy-mm-dd",
                 changeMonth: !0,
-                changeYear: !0
+                changeYear: !0,
+                yearRange: "c-70:c+10"
             })
         }, 300)
     })
 });
```

### Comparing `django-jalali-date-1.1.0/jalali_date/templates/admin/edit_inline/jalali_stacked.html` & `django_jalali_date-1.1.1/jalali_date/templates/admin/edit_inline/jalali_stacked.html`

 * *Files identical despite different names*

### Comparing `django-jalali-date-1.1.0/jalali_date/templates/admin/edit_inline/jalali_tabular.html` & `django_jalali_date-1.1.1/jalali_date/templates/admin/edit_inline/jalali_tabular.html`

 * *Files identical despite different names*

### Comparing `django-jalali-date-1.1.0/jalali_date/templates/admin/includes/jalali_fieldset.html` & `django_jalali_date-1.1.1/jalali_date/templates/admin/includes/jalali_fieldset.html`

 * *Files identical despite different names*

### Comparing `django-jalali-date-1.1.0/jalali_date/templatetags/jalali_tags.py` & `django_jalali_date-1.1.1/jalali_date/templatetags/jalali_tags.py`

 * *Files identical despite different names*

### Comparing `django-jalali-date-1.1.0/jalali_date/widgets.py` & `django_jalali_date-1.1.1/jalali_date/widgets.py`

 * *Files identical despite different names*

### Comparing `django-jalali-date-1.1.0/setup.py` & `django_jalali_date-1.1.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 def read_me(filename):
     return codecs.open(filename, encoding='utf-8').read()
 
 
 setup(
     name='django-jalali-date',
-    version='1.1.0',
+    version='1.1.1',
     python_requires='>=3',
     packages=find_packages(),
     include_package_data=True,
     description=(
         'Jalali Date support for user interface. Easy conversion of DateTimeFiled to JalaliDateTimeField within the admin site, views, forms and templates.'
     ),
     url='http://github.com/a-roomana/django-jalali-date',
```

