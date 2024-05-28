# Comparing `tmp/fb_tools-2.5.2.tar.gz` & `tmp/fb_tools-2.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fb_tools-2.5.2.tar", last modified: Wed May 15 10:50:10 2024, max compression
+gzip compressed data, was "fb_tools-2.5.3.tar", last modified: Tue May 28 08:44:50 2024, max compression
```

## Comparing `fb_tools-2.5.2.tar` & `fb_tools-2.5.3.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:50:10.482114 fb_tools-2.5.2/
--rw-r--r--   0 root         (0) root         (0)     7652 2024-05-15 10:49:49.000000 fb_tools-2.5.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      120 2024-05-15 10:49:49.000000 fb_tools-2.5.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1887 2024-05-15 10:50:10.482114 fb_tools-2.5.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      503 2024-05-15 10:49:49.000000 fb_tools-2.5.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:50:10.470113 fb_tools-2.5.2/bin/
--rwxr-xr-x   0 root         (0) root         (0)     2298 2024-05-15 10:49:49.000000 fb_tools-2.5.2/bin/get-file-to-remove
--rwxr-xr-x   0 root         (0) root         (0)     2286 2024-05-15 10:49:49.000000 fb_tools-2.5.2/bin/myip
--rwxr-xr-x   0 root         (0) root         (0)     2293 2024-05-15 10:49:49.000000 fb_tools-2.5.2/bin/update-ddns
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:50:10.466113 fb_tools-2.5.2/lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:50:10.474114 fb_tools-2.5.2/lib/fb_tools/
--rw-r--r--   0 root         (0) root         (0)      606 2024-05-15 10:49:49.000000 fb_tools-2.5.2/lib/fb_tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29242 2024-05-15 10:49:49.000000 fb_tools-2.5.2/lib/fb_tools/app.py
--rw-r--r--   0 root         (0) root         (0)     8423 2024-05-15 10:49:49.000000 fb_tools-2.5.2/lib/fb_tools/argparse_actions.py
--rw-r--r--   0 root         (0) root         (0)     9465 2024-05-15 10:49:49.000000 fb_tools-2.5.2/lib/fb_tools/cfg_app.py
--rw-r--r--   0 root         (0) root         (0)    36990 2024-05-15 10:49:49.000000 fb_tools-2.5.2/lib/fb_tools/collections.py
--rw-r--r--   0 root         (0) root         (0)    30170 2024-05-15 10:49:49.000000 fb_tools-2.5.2/lib/fb_tools/common.py
--rw-r--r--   0 root         (0) root         (0)     7978 2024-05-15 10:49:49.000000 fb_tools-2.5.2/lib/fb_tools/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:50:10.474114 fb_tools-2.5.2/lib/fb_tools/ddns/
--rw-r--r--   0 root         (0) root         (0)    20366 2024-05-15 10:49:49.000000 fb_tools-2.5.2/lib/fb_tools/ddns/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12479 2024-05-15 10:49:49.000000 fb_tools-2.5.2/lib/fb_tools/ddns/config.py
--rw-r--r--   0 root         (0) root         (0)     4516 2024-05-15 10:49:49.000000 fb_tools-2.5.2/lib/fb_tools/ddns/errors.py
--rw-r--r--   0 root         (0) root         (0)     5594 2024-05-15 10:49:49.000000 fb_tools-2.5.2/lib/fb_tools/ddns/myip_app.py
--rw-r--r--   0 root         (0) root         (0)    27714 2024-05-15 10:49:49.000000 fb_tools-2.5.2/lib/fb_tools/ddns/update_app.py
--rw-r--r--   0 root         (0) root         (0)    19921 2024-05-15 10:49:49.000000 fb_tools-2.5.2/lib/fb_tools/errors.py
--rw-r--r--   0 root         (0) root         (0)    24586 2024-05-15 10:49:49.000000 fb_tools-2.5.2/lib/fb_tools/get_file_rm_app.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:50:10.478114 fb_tools-2.5.2/lib/fb_tools/handler/
--rw-r--r--   0 root         (0) root         (0)    13864 2024-05-15 10:49:49.000000 fb_tools-2.5.2/lib/fb_tools/handler/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42608 2024-05-15 10:49:49.000000 fb_tools-2.5.2/lib/fb_tools/handler/lock.py
--rw-r--r--   0 root         (0) root         (0)    44127 2024-05-15 10:49:49.000000 fb_tools-2.5.2/lib/fb_tools/handling_obj.py
--rw-r--r--   0 root         (0) root         (0)      460 2024-05-15 10:50:10.000000 fb_tools-2.5.2/lib/fb_tools/local_version.py
--rw-r--r--   0 root         (0) root         (0)    34985 2024-05-15 10:49:49.000000 fb_tools-2.5.2/lib/fb_tools/mailaddress.py
--rw-r--r--   0 root         (0) root         (0)     2391 2024-05-15 10:49:49.000000 fb_tools-2.5.2/lib/fb_tools/merge.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:50:10.478114 fb_tools-2.5.2/lib/fb_tools/multi_config/
--rw-r--r--   0 root         (0) root         (0)    20431 2024-05-15 10:49:49.000000 fb_tools-2.5.2/lib/fb_tools/multi_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12240 2024-05-15 10:49:49.000000 fb_tools-2.5.2/lib/fb_tools/multi_config/files.py
--rw-r--r--   0 root         (0) root         (0)     7783 2024-05-15 10:49:49.000000 fb_tools-2.5.2/lib/fb_tools/multi_config/inits.py
--rw-r--r--   0 root         (0) root         (0)    11922 2024-05-15 10:49:49.000000 fb_tools-2.5.2/lib/fb_tools/multi_config/read.py
--rw-r--r--   0 root         (0) root         (0)    11761 2024-05-15 10:49:49.000000 fb_tools-2.5.2/lib/fb_tools/obj.py
--rw-r--r--   0 root         (0) root         (0)    17133 2024-05-15 10:49:49.000000 fb_tools-2.5.2/lib/fb_tools/pidfile.py
--rw-r--r--   0 root         (0) root         (0)     3390 2024-05-15 10:49:49.000000 fb_tools-2.5.2/lib/fb_tools/xlate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:50:10.482114 fb_tools-2.5.2/lib/fb_tools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1887 2024-05-15 10:50:10.000000 fb_tools-2.5.2/lib/fb_tools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1582 2024-05-15 10:50:10.000000 fb_tools-2.5.2/lib/fb_tools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 10:50:10.000000 fb_tools-2.5.2/lib/fb_tools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2024-05-15 10:50:10.000000 fb_tools-2.5.2/lib/fb_tools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-15 10:50:10.000000 fb_tools-2.5.2/lib/fb_tools.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:50:10.478114 fb_tools-2.5.2/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:50:10.470113 fb_tools-2.5.2/locale/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:50:10.478114 fb_tools-2.5.2/locale/de/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)    47617 2024-05-15 10:50:10.000000 fb_tools-2.5.2/locale/de/LC_MESSAGES/fb_tools.mo
--rw-r--r--   0 root         (0) root         (0)    69131 2024-05-15 10:49:49.000000 fb_tools-2.5.2/locale/de/LC_MESSAGES/fb_tools.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:50:10.470113 fb_tools-2.5.2/locale/en/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:50:10.478114 fb_tools-2.5.2/locale/en/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     6156 2024-05-15 10:50:10.000000 fb_tools-2.5.2/locale/en/LC_MESSAGES/fb_tools.mo
--rw-r--r--   0 root         (0) root         (0)    49500 2024-05-15 10:49:49.000000 fb_tools-2.5.2/locale/en/LC_MESSAGES/fb_tools.po
--rw-r--r--   0 root         (0) root         (0)    47320 2024-05-15 10:49:49.000000 fb_tools-2.5.2/locale/fb_tools.pot
--rw-r--r--   0 root         (0) root         (0)     1800 2024-05-15 10:50:10.482114 fb_tools-2.5.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     8889 2024-05-15 10:49:49.000000 fb_tools-2.5.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:50:10.482114 fb_tools-2.5.2/test/
--rwxr-xr-x   0 root         (0) root         (0)      270 2024-05-15 10:49:49.000000 fb_tools-2.5.2/test/call_script.sh
--rwxr-xr-x   0 root         (0) root         (0)      438 2024-05-15 10:49:49.000000 fb_tools-2.5.2/test/call_sleep.sh
--rwxr-xr-x   0 root         (0) root         (0)      438 2024-05-15 10:49:49.000000 fb_tools-2.5.2/test/do_sleep
--rw-r--r--   0 root         (0) root         (0)     4756 2024-05-15 10:49:49.000000 fb_tools-2.5.2/test/general.py
--rwxr-xr-x   0 root         (0) root         (0)     5221 2024-05-15 10:49:49.000000 fb_tools-2.5.2/test/test_00_errors.py
--rwxr-xr-x   0 root         (0) root         (0)    26677 2024-05-15 10:49:49.000000 fb_tools-2.5.2/test/test_05_common.py
--rwxr-xr-x   0 root         (0) root         (0)     6873 2024-05-15 10:49:49.000000 fb_tools-2.5.2/test/test_10_base_object.py
--rwxr-xr-x   0 root         (0) root         (0)    61659 2024-05-15 10:49:49.000000 fb_tools-2.5.2/test/test_13_collections.py
--rwxr-xr-x   0 root         (0) root         (0)    52551 2024-05-15 10:49:49.000000 fb_tools-2.5.2/test/test_15_mailaddress.py
--rwxr-xr-x   0 root         (0) root         (0)    23387 2024-05-15 10:49:49.000000 fb_tools-2.5.2/test/test_17_multicfg.py
--rwxr-xr-x   0 root         (0) root         (0)     6078 2024-05-15 10:49:49.000000 fb_tools-2.5.2/test/test_18_pidfile.py
--rwxr-xr-x   0 root         (0) root         (0)    26258 2024-05-15 10:49:49.000000 fb_tools-2.5.2/test/test_20_handling_object.py
--rwxr-xr-x   0 root         (0) root         (0)     7698 2024-05-15 10:49:49.000000 fb_tools-2.5.2/test/test_25_ddns_update_status.py
--rwxr-xr-x   0 root         (0) root         (0)     8159 2024-05-15 10:49:49.000000 fb_tools-2.5.2/test/test_30_base_handler.py
--rwxr-xr-x   0 root         (0) root         (0)    15313 2024-05-15 10:49:49.000000 fb_tools-2.5.2/test/test_33_lock.py
--rwxr-xr-x   0 root         (0) root         (0)    10128 2024-05-15 10:49:49.000000 fb_tools-2.5.2/test/test_40_app_modules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:44:50.334167 fb_tools-2.5.3/
+-rw-r--r--   0 root         (0) root         (0)     7652 2024-05-28 08:44:18.000000 fb_tools-2.5.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      120 2024-05-28 08:44:18.000000 fb_tools-2.5.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1887 2024-05-28 08:44:50.334167 fb_tools-2.5.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      503 2024-05-28 08:44:18.000000 fb_tools-2.5.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:44:50.322167 fb_tools-2.5.3/bin/
+-rwxr-xr-x   0 root         (0) root         (0)     2298 2024-05-28 08:44:18.000000 fb_tools-2.5.3/bin/get-file-to-remove
+-rwxr-xr-x   0 root         (0) root         (0)     2286 2024-05-28 08:44:18.000000 fb_tools-2.5.3/bin/myip
+-rwxr-xr-x   0 root         (0) root         (0)     2293 2024-05-28 08:44:18.000000 fb_tools-2.5.3/bin/update-ddns
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:44:50.318167 fb_tools-2.5.3/lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:44:50.326167 fb_tools-2.5.3/lib/fb_tools/
+-rw-r--r--   0 root         (0) root         (0)      606 2024-05-28 08:44:18.000000 fb_tools-2.5.3/lib/fb_tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29242 2024-05-28 08:44:18.000000 fb_tools-2.5.3/lib/fb_tools/app.py
+-rw-r--r--   0 root         (0) root         (0)     8423 2024-05-28 08:44:18.000000 fb_tools-2.5.3/lib/fb_tools/argparse_actions.py
+-rw-r--r--   0 root         (0) root         (0)     9465 2024-05-28 08:44:18.000000 fb_tools-2.5.3/lib/fb_tools/cfg_app.py
+-rw-r--r--   0 root         (0) root         (0)    36990 2024-05-28 08:44:18.000000 fb_tools-2.5.3/lib/fb_tools/collections.py
+-rw-r--r--   0 root         (0) root         (0)    30170 2024-05-28 08:44:18.000000 fb_tools-2.5.3/lib/fb_tools/common.py
+-rw-r--r--   0 root         (0) root         (0)     7978 2024-05-28 08:44:18.000000 fb_tools-2.5.3/lib/fb_tools/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:44:50.326167 fb_tools-2.5.3/lib/fb_tools/ddns/
+-rw-r--r--   0 root         (0) root         (0)    20366 2024-05-28 08:44:18.000000 fb_tools-2.5.3/lib/fb_tools/ddns/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12479 2024-05-28 08:44:18.000000 fb_tools-2.5.3/lib/fb_tools/ddns/config.py
+-rw-r--r--   0 root         (0) root         (0)     4516 2024-05-28 08:44:18.000000 fb_tools-2.5.3/lib/fb_tools/ddns/errors.py
+-rw-r--r--   0 root         (0) root         (0)     5594 2024-05-28 08:44:18.000000 fb_tools-2.5.3/lib/fb_tools/ddns/myip_app.py
+-rw-r--r--   0 root         (0) root         (0)    27714 2024-05-28 08:44:18.000000 fb_tools-2.5.3/lib/fb_tools/ddns/update_app.py
+-rw-r--r--   0 root         (0) root         (0)    19921 2024-05-28 08:44:18.000000 fb_tools-2.5.3/lib/fb_tools/errors.py
+-rw-r--r--   0 root         (0) root         (0)    24586 2024-05-28 08:44:18.000000 fb_tools-2.5.3/lib/fb_tools/get_file_rm_app.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:44:50.326167 fb_tools-2.5.3/lib/fb_tools/handler/
+-rw-r--r--   0 root         (0) root         (0)    13864 2024-05-28 08:44:18.000000 fb_tools-2.5.3/lib/fb_tools/handler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    42608 2024-05-28 08:44:18.000000 fb_tools-2.5.3/lib/fb_tools/handler/lock.py
+-rw-r--r--   0 root         (0) root         (0)    44123 2024-05-28 08:44:18.000000 fb_tools-2.5.3/lib/fb_tools/handling_obj.py
+-rw-r--r--   0 root         (0) root         (0)      460 2024-05-28 08:44:50.000000 fb_tools-2.5.3/lib/fb_tools/local_version.py
+-rw-r--r--   0 root         (0) root         (0)    34985 2024-05-28 08:44:18.000000 fb_tools-2.5.3/lib/fb_tools/mailaddress.py
+-rw-r--r--   0 root         (0) root         (0)     2391 2024-05-28 08:44:18.000000 fb_tools-2.5.3/lib/fb_tools/merge.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:44:50.326167 fb_tools-2.5.3/lib/fb_tools/multi_config/
+-rw-r--r--   0 root         (0) root         (0)    20431 2024-05-28 08:44:18.000000 fb_tools-2.5.3/lib/fb_tools/multi_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12240 2024-05-28 08:44:18.000000 fb_tools-2.5.3/lib/fb_tools/multi_config/files.py
+-rw-r--r--   0 root         (0) root         (0)     7783 2024-05-28 08:44:18.000000 fb_tools-2.5.3/lib/fb_tools/multi_config/inits.py
+-rw-r--r--   0 root         (0) root         (0)    11922 2024-05-28 08:44:18.000000 fb_tools-2.5.3/lib/fb_tools/multi_config/read.py
+-rw-r--r--   0 root         (0) root         (0)    11761 2024-05-28 08:44:18.000000 fb_tools-2.5.3/lib/fb_tools/obj.py
+-rw-r--r--   0 root         (0) root         (0)    17133 2024-05-28 08:44:18.000000 fb_tools-2.5.3/lib/fb_tools/pidfile.py
+-rw-r--r--   0 root         (0) root         (0)     3390 2024-05-28 08:44:18.000000 fb_tools-2.5.3/lib/fb_tools/xlate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:44:50.334167 fb_tools-2.5.3/lib/fb_tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1887 2024-05-28 08:44:50.000000 fb_tools-2.5.3/lib/fb_tools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1582 2024-05-28 08:44:50.000000 fb_tools-2.5.3/lib/fb_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 08:44:50.000000 fb_tools-2.5.3/lib/fb_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2024-05-28 08:44:50.000000 fb_tools-2.5.3/lib/fb_tools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-28 08:44:50.000000 fb_tools-2.5.3/lib/fb_tools.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:44:50.330167 fb_tools-2.5.3/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:44:50.318167 fb_tools-2.5.3/locale/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:44:50.330167 fb_tools-2.5.3/locale/de/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)    47617 2024-05-28 08:44:50.000000 fb_tools-2.5.3/locale/de/LC_MESSAGES/fb_tools.mo
+-rw-r--r--   0 root         (0) root         (0)    69131 2024-05-28 08:44:18.000000 fb_tools-2.5.3/locale/de/LC_MESSAGES/fb_tools.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:44:50.318167 fb_tools-2.5.3/locale/en/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:44:50.330167 fb_tools-2.5.3/locale/en/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)     6156 2024-05-28 08:44:50.000000 fb_tools-2.5.3/locale/en/LC_MESSAGES/fb_tools.mo
+-rw-r--r--   0 root         (0) root         (0)    49500 2024-05-28 08:44:18.000000 fb_tools-2.5.3/locale/en/LC_MESSAGES/fb_tools.po
+-rw-r--r--   0 root         (0) root         (0)    47320 2024-05-28 08:44:18.000000 fb_tools-2.5.3/locale/fb_tools.pot
+-rw-r--r--   0 root         (0) root         (0)     1800 2024-05-28 08:44:50.334167 fb_tools-2.5.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     8889 2024-05-28 08:44:18.000000 fb_tools-2.5.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 08:44:50.334167 fb_tools-2.5.3/test/
+-rwxr-xr-x   0 root         (0) root         (0)      270 2024-05-28 08:44:18.000000 fb_tools-2.5.3/test/call_script.sh
+-rwxr-xr-x   0 root         (0) root         (0)      438 2024-05-28 08:44:18.000000 fb_tools-2.5.3/test/call_sleep.sh
+-rwxr-xr-x   0 root         (0) root         (0)      438 2024-05-28 08:44:18.000000 fb_tools-2.5.3/test/do_sleep
+-rw-r--r--   0 root         (0) root         (0)     4756 2024-05-28 08:44:18.000000 fb_tools-2.5.3/test/general.py
+-rwxr-xr-x   0 root         (0) root         (0)     5221 2024-05-28 08:44:18.000000 fb_tools-2.5.3/test/test_00_errors.py
+-rwxr-xr-x   0 root         (0) root         (0)    26677 2024-05-28 08:44:18.000000 fb_tools-2.5.3/test/test_05_common.py
+-rwxr-xr-x   0 root         (0) root         (0)     6873 2024-05-28 08:44:18.000000 fb_tools-2.5.3/test/test_10_base_object.py
+-rwxr-xr-x   0 root         (0) root         (0)    61659 2024-05-28 08:44:18.000000 fb_tools-2.5.3/test/test_13_collections.py
+-rwxr-xr-x   0 root         (0) root         (0)    52551 2024-05-28 08:44:18.000000 fb_tools-2.5.3/test/test_15_mailaddress.py
+-rwxr-xr-x   0 root         (0) root         (0)    23387 2024-05-28 08:44:18.000000 fb_tools-2.5.3/test/test_17_multicfg.py
+-rwxr-xr-x   0 root         (0) root         (0)     6078 2024-05-28 08:44:18.000000 fb_tools-2.5.3/test/test_18_pidfile.py
+-rwxr-xr-x   0 root         (0) root         (0)    26258 2024-05-28 08:44:18.000000 fb_tools-2.5.3/test/test_20_handling_object.py
+-rwxr-xr-x   0 root         (0) root         (0)     7698 2024-05-28 08:44:18.000000 fb_tools-2.5.3/test/test_25_ddns_update_status.py
+-rwxr-xr-x   0 root         (0) root         (0)     8159 2024-05-28 08:44:18.000000 fb_tools-2.5.3/test/test_30_base_handler.py
+-rwxr-xr-x   0 root         (0) root         (0)    15313 2024-05-28 08:44:18.000000 fb_tools-2.5.3/test/test_33_lock.py
+-rwxr-xr-x   0 root         (0) root         (0)    10128 2024-05-28 08:44:18.000000 fb_tools-2.5.3/test/test_40_app_modules.py
```

### Comparing `fb_tools-2.5.2/LICENSE` & `fb_tools-2.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.2/PKG-INFO` & `fb_tools-2.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fb_tools
-Version: 2.5.2
+Version: 2.5.3
 Summary: Modules for common used objects, error classes and methods.
 Home-page: https://github.com/fbrehm/python_fb_tools
 Author: Frank Brehm
 Author-email: frank@brehm-online.com
 License: LGPL3+
 Platform: posix
 Classifier: Development Status :: 4 - Beta
```

### Comparing `fb_tools-2.5.2/bin/get-file-to-remove` & `fb_tools-2.5.3/bin/get-file-to-remove`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.2/bin/myip` & `fb_tools-2.5.3/bin/myip`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.2/bin/update-ddns` & `fb_tools-2.5.3/bin/update-ddns`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.2/lib/fb_tools/__init__.py` & `fb_tools-2.5.3/lib/fb_tools/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,13 +11,13 @@
 DDNS_CFG_BASENAME = 'ddns.ini'
 MAX_TIMEOUT = 3600
 UTF8_ENCODING = 'utf-8'
 DEFAULT_ENCODING = UTF8_ENCODING
 DEFAULT_TERMINAL_WIDTH = 99
 DEFAULT_TERMINAL_HEIGHT = 40
 
-__version__ = '2.5.2'
+__version__ = '2.5.3'
 
 from .mailaddress import MailAddress, QualifiedMailAddress, MailAddressList     # noqa
 from .multi_config import BaseMultiConfig                                       # noqa
 
 # vim: ts=4 et list
```

### Comparing `fb_tools-2.5.2/lib/fb_tools/app.py` & `fb_tools-2.5.3/lib/fb_tools/app.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.2/lib/fb_tools/argparse_actions.py` & `fb_tools-2.5.3/lib/fb_tools/argparse_actions.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.2/lib/fb_tools/cfg_app.py` & `fb_tools-2.5.3/lib/fb_tools/cfg_app.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.2/lib/fb_tools/collections.py` & `fb_tools-2.5.3/lib/fb_tools/collections.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.2/lib/fb_tools/common.py` & `fb_tools-2.5.3/lib/fb_tools/common.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.2/lib/fb_tools/config.py` & `fb_tools-2.5.3/lib/fb_tools/config.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.2/lib/fb_tools/ddns/__init__.py` & `fb_tools-2.5.3/lib/fb_tools/ddns/__init__.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.2/lib/fb_tools/ddns/config.py` & `fb_tools-2.5.3/lib/fb_tools/ddns/config.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.2/lib/fb_tools/ddns/errors.py` & `fb_tools-2.5.3/lib/fb_tools/ddns/errors.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.2/lib/fb_tools/ddns/myip_app.py` & `fb_tools-2.5.3/lib/fb_tools/ddns/myip_app.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.2/lib/fb_tools/ddns/update_app.py` & `fb_tools-2.5.3/lib/fb_tools/ddns/update_app.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.2/lib/fb_tools/errors.py` & `fb_tools-2.5.3/lib/fb_tools/errors.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.2/lib/fb_tools/get_file_rm_app.py` & `fb_tools-2.5.3/lib/fb_tools/get_file_rm_app.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.2/lib/fb_tools/handler/__init__.py` & `fb_tools-2.5.3/lib/fb_tools/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.2/lib/fb_tools/handler/lock.py` & `fb_tools-2.5.3/lib/fb_tools/handler/lock.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.2/lib/fb_tools/handling_obj.py` & `fb_tools-2.5.3/lib/fb_tools/handling_obj.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 from .common import caller_search_path, encode_or_bust, pp, to_bool, to_str
 from .common import indent, is_sequence
 from .errors import AbortAppError, TimeoutOnPromptError
 from .errors import InterruptError, IoTimeoutError, ReadTimeoutError, WriteTimeoutError
 from .obj import FbBaseObject
 from .xlate import XLATOR, format_list
 
-__version__ = '2.2.4'
+__version__ = '2.2.5'
 LOG = logging.getLogger(__name__)
 
 _ = XLATOR.gettext
 ngettext = XLATOR.ngettext
 
 DEFAULT_FILEIO_TIMEOUT = 2
 DEFAULT_PROMPT_TIMEOUT = 30
@@ -1018,20 +1018,20 @@
                         continue
                 else:
                     break
 
         except (TimeoutOnPromptError, AbortAppError) as e:
             msg = _('Got a {}:').format(e.__class__.__name__) + ' ' + str(e)
             LOG.error(msg)
-            self.exit(10)
+            sys.exit(10)
 
         except KeyboardInterrupt:
             msg = _('Got a {}:').format('KeyboardInterrupt') + ' ' + msg_intr
             LOG.error(msg)
-            self.exit(10)
+            sys.exit(10)
 
         finally:
             signal.alarm(0)
 
         return ret_passwd
 
     # -------------------------------------------------------------------------
@@ -1102,21 +1102,21 @@
                     continue
                 # Repeat the question
 
         except (TimeoutOnPromptError, AbortAppError) as e:
             print()
             msg = _('Got a {}:').format(e.__class__.__name__) + ' ' + str(e)
             LOG.error(msg)
-            self.exit(10)
+            sys.exit(10)
 
         except KeyboardInterrupt:
             msg = _('Got a {}:').format('KeyboardInterrupt') + ' ' + msg_intr
             print()
             LOG.error(msg)
-            self.exit(10)
+            sys.exit(10)
 
         finally:
             signal.alarm(0)
 
 
 # =============================================================================
 class CompletedProcess(object):
```

### Comparing `fb_tools-2.5.2/lib/fb_tools/mailaddress.py` & `fb_tools-2.5.3/lib/fb_tools/mailaddress.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.2/lib/fb_tools/merge.py` & `fb_tools-2.5.3/lib/fb_tools/merge.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.2/lib/fb_tools/multi_config/__init__.py` & `fb_tools-2.5.3/lib/fb_tools/multi_config/__init__.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.2/lib/fb_tools/multi_config/files.py` & `fb_tools-2.5.3/lib/fb_tools/multi_config/files.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.2/lib/fb_tools/multi_config/inits.py` & `fb_tools-2.5.3/lib/fb_tools/multi_config/inits.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.2/lib/fb_tools/multi_config/read.py` & `fb_tools-2.5.3/lib/fb_tools/multi_config/read.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.2/lib/fb_tools/obj.py` & `fb_tools-2.5.3/lib/fb_tools/obj.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.2/lib/fb_tools/pidfile.py` & `fb_tools-2.5.3/lib/fb_tools/pidfile.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.2/lib/fb_tools/xlate.py` & `fb_tools-2.5.3/lib/fb_tools/xlate.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.2/lib/fb_tools.egg-info/PKG-INFO` & `fb_tools-2.5.3/lib/fb_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fb_tools
-Version: 2.5.2
+Version: 2.5.3
 Summary: Modules for common used objects, error classes and methods.
 Home-page: https://github.com/fbrehm/python_fb_tools
 Author: Frank Brehm
 Author-email: frank@brehm-online.com
 License: LGPL3+
 Platform: posix
 Classifier: Development Status :: 4 - Beta
```

### Comparing `fb_tools-2.5.2/lib/fb_tools.egg-info/SOURCES.txt` & `fb_tools-2.5.3/lib/fb_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.2/locale/de/LC_MESSAGES/fb_tools.mo` & `fb_tools-2.5.3/locale/de/LC_MESSAGES/fb_tools.mo`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.2/locale/de/LC_MESSAGES/fb_tools.po` & `fb_tools-2.5.3/locale/de/LC_MESSAGES/fb_tools.po`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.2/locale/en/LC_MESSAGES/fb_tools.mo` & `fb_tools-2.5.3/locale/en/LC_MESSAGES/fb_tools.mo`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.2/locale/en/LC_MESSAGES/fb_tools.po` & `fb_tools-2.5.3/locale/en/LC_MESSAGES/fb_tools.po`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.2/locale/fb_tools.pot` & `fb_tools-2.5.3/locale/fb_tools.pot`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.2/setup.cfg` & `fb_tools-2.5.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.2/setup.py` & `fb_tools-2.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.2/test/general.py` & `fb_tools-2.5.3/test/general.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.2/test/test_00_errors.py` & `fb_tools-2.5.3/test/test_00_errors.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.2/test/test_05_common.py` & `fb_tools-2.5.3/test/test_05_common.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.2/test/test_10_base_object.py` & `fb_tools-2.5.3/test/test_10_base_object.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.2/test/test_13_collections.py` & `fb_tools-2.5.3/test/test_13_collections.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.2/test/test_15_mailaddress.py` & `fb_tools-2.5.3/test/test_15_mailaddress.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.2/test/test_17_multicfg.py` & `fb_tools-2.5.3/test/test_17_multicfg.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.2/test/test_18_pidfile.py` & `fb_tools-2.5.3/test/test_18_pidfile.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.2/test/test_20_handling_object.py` & `fb_tools-2.5.3/test/test_20_handling_object.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.2/test/test_25_ddns_update_status.py` & `fb_tools-2.5.3/test/test_25_ddns_update_status.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.2/test/test_30_base_handler.py` & `fb_tools-2.5.3/test/test_30_base_handler.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.2/test/test_33_lock.py` & `fb_tools-2.5.3/test/test_33_lock.py`

 * *Files identical despite different names*

### Comparing `fb_tools-2.5.2/test/test_40_app_modules.py` & `fb_tools-2.5.3/test/test_40_app_modules.py`

 * *Files identical despite different names*

