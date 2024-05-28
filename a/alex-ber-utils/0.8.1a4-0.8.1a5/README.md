# Comparing `tmp/alex_ber_utils-0.8.1a4.tar.gz` & `tmp/alex_ber_utils-0.8.1a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alex_ber_utils-0.8.1a4.tar", last modified: Tue May 28 12:30:24 2024, max compression
+gzip compressed data, was "alex_ber_utils-0.8.1a5.tar", last modified: Tue May 28 15:24:02 2024, max compression
```

## Comparing `alex_ber_utils-0.8.1a4.tar` & `alex_ber_utils-0.8.1a5.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 12:30:24.664174 alex_ber_utils-0.8.1a4/
--rwxrwxrwx   0 root         (0) root         (0)    26584 2024-05-28 09:24:26.000000 alex_ber_utils-0.8.1a4/CHANGELOG.md
--rwxrwxrwx   0 root         (0) root         (0)     1295 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/LICENSE.txt
--rwxrwxrwx   0 root         (0) root         (0)      195 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    31537 2024-05-28 12:30:24.665463 alex_ber_utils-0.8.1a4/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     3900 2024-05-28 10:26:01.000000 alex_ber_utils-0.8.1a4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 12:30:23.258989 alex_ber_utils-0.8.1a4/alex_ber_utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)    31537 2024-05-28 12:30:21.000000 alex_ber_utils-0.8.1a4/alex_ber_utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2227 2024-05-28 12:30:22.000000 alex_ber_utils-0.8.1a4/alex_ber_utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 12:30:21.000000 alex_ber_utils-0.8.1a4/alex_ber_utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-28 12:30:21.000000 alex_ber_utils-0.8.1a4/alex_ber_utils.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 12:30:17.000000 alex_ber_utils-0.8.1a4/alex_ber_utils.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      427 2024-05-28 12:30:21.000000 alex_ber_utils-0.8.1a4/alex_ber_utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2024-05-28 12:30:21.000000 alex_ber_utils-0.8.1a4/alex_ber_utils.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 12:30:23.277776 alex_ber_utils-0.8.1a4/alexber/
--rwxrwxrwx   0 root         (0) root         (0)       55 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/alexber/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 12:30:23.785940 alex_ber_utils-0.8.1a4/alexber/utils/
--rwxrwxrwx   0 root         (0) root         (0)      250 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/alexber/utils/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     8188 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/alexber/utils/_ymlparsers_extra.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 12:30:23.813440 alex_ber_utils-0.8.1a4/alexber/utils/data/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-28 11:54:41.000000 alex_ber_utils-0.8.1a4/alexber/utils/data/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3928 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/alexber/utils/deploys.py
--rwxrwxrwx   0 root         (0) root         (0)    17354 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/alexber/utils/emails.py
--rwxrwxrwx   0 root         (0) root         (0)     1425 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/alexber/utils/enums.py
--rwxrwxrwx   0 root         (0) root         (0)     1512 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/alexber/utils/fabs.py
--rwxrwxrwx   0 root         (0) root         (0)      857 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/alexber/utils/files.py
--rwxrwxrwx   0 root         (0) root         (0)     3300 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/alexber/utils/importer.py
--rwxrwxrwx   0 root         (0) root         (0)    19314 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/alexber/utils/init_app_conf.py
--rwxrwxrwx   0 root         (0) root         (0)     1385 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/alexber/utils/inspects.py
--rwxrwxrwx   0 root         (0) root         (0)    11144 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/alexber/utils/mains.py
--rwxrwxrwx   0 root         (0) root         (0)     4210 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/alexber/utils/parsers.py
--rwxrwxrwx   0 root         (0) root         (0)     1676 2024-05-28 11:55:39.000000 alex_ber_utils-0.8.1a4/alexber/utils/pprint.py
--rwxrwxrwx   0 root         (0) root         (0)    10390 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/alexber/utils/processinvokes.py
--rwxrwxrwx   0 root         (0) root         (0)    16921 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/alexber/utils/props.py
--rwxrwxrwx   0 root         (0) root         (0)     2296 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/alexber/utils/setups.py
--rwxrwxrwx   0 root         (0) root         (0)     3204 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/alexber/utils/stdlogging.py
--rwxrwxrwx   0 root         (0) root         (0)      658 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/alexber/utils/thread_locals.py
--rwxrwxrwx   0 root         (0) root         (0)     1745 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/alexber/utils/uuids.py
--rwxrwxrwx   0 root         (0) root         (0)    11517 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/alexber/utils/ymlparsers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 12:30:23.832507 alex_ber_utils-0.8.1a4/data/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-28 11:54:41.000000 alex_ber_utils-0.8.1a4/data/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       21 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/req-env.txt
--rwxrwxrwx   0 root         (0) root         (0)       56 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/req-fabric.txt
--rwxrwxrwx   0 root         (0) root         (0)       18 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/req-md.txt
--rwxrwxrwx   0 root         (0) root         (0)       17 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/req-piptools.txt
--rwxrwxrwx   0 root         (0) root         (0)      107 2024-05-28 11:49:47.000000 alex_ber_utils-0.8.1a4/req-tests.txt
--rwxrwxrwx   0 root         (0) root         (0)       32 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/req-yml.txt
--rwxrwxrwx   0 root         (0) root         (0)       13 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/req.txt
--rwxrwxrwx   0 root         (0) root         (0)      204 2024-05-28 11:52:04.000000 alex_ber_utils-0.8.1a4/requirements-env.txt
--rwxrwxrwx   0 root         (0) root         (0)      669 2024-05-28 11:52:20.000000 alex_ber_utils-0.8.1a4/requirements-fabric.txt
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-28 11:49:47.000000 alex_ber_utils-0.8.1a4/requirements-md.txt
--rwxrwxrwx   0 root         (0) root         (0)      648 2024-05-28 11:52:40.000000 alex_ber_utils-0.8.1a4/requirements-piptools.txt
--rwxrwxrwx   0 root         (0) root         (0)      662 2024-05-28 11:58:27.000000 alex_ber_utils-0.8.1a4/requirements-tests.txt
--rwxrwxrwx   0 root         (0) root         (0)      387 2024-05-28 11:58:42.000000 alex_ber_utils-0.8.1a4/requirements-yml.txt
--rwxrwxrwx   0 root         (0) root         (0)      185 2024-05-28 11:51:48.000000 alex_ber_utils-0.8.1a4/requirements.txt
--rwxrwxrwx   0 root         (0) root         (0)      190 2024-05-28 12:30:24.674076 alex_ber_utils-0.8.1a4/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     4905 2024-05-28 12:08:57.000000 alex_ber_utils-0.8.1a4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 12:30:23.863068 alex_ber_utils-0.8.1a4/tests/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/tests/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1931 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 12:30:24.272491 alex_ber_utils-0.8.1a4/tests/utils/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/tests/utils/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     6071 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/tests/utils/deploys_test.py
--rwxrwxrwx   0 root         (0) root         (0)     8680 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/tests/utils/emails_test.py
--rwxrwxrwx   0 root         (0) root         (0)    10227 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/tests/utils/enums_mixin_test.py
--rwxrwxrwx   0 root         (0) root         (0)     5067 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/tests/utils/importer_test.py
--rwxrwxrwx   0 root         (0) root         (0)    30475 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/tests/utils/init_app_conf_test.py
--rwxrwxrwx   0 root         (0) root         (0)     3654 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/tests/utils/inspect_test.py
--rwxrwxrwx   0 root         (0) root         (0)     1328 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/tests/utils/mains_test.py
--rwxrwxrwx   0 root         (0) root         (0)     2444 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/tests/utils/method_overloading_test.py
--rwxrwxrwx   0 root         (0) root         (0)     5106 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/tests/utils/parsers_test.py
--rwxrwxrwx   0 root         (0) root         (0)     2157 2024-05-28 09:22:01.000000 alex_ber_utils-0.8.1a4/tests/utils/pprint_test.py
--rwxrwxrwx   0 root         (0) root         (0)     5372 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/tests/utils/processinvokes_test.py
--rwxrwxrwx   0 root         (0) root         (0)     2047 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/tests/utils/properties_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 12:30:24.334165 alex_ber_utils-0.8.1a4/tests/utils/splitpackage/
--rwxrwxrwx   0 root         (0) root         (0)      116 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/tests/utils/splitpackage/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/tests/utils/splitpackage/mymodule.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 12:30:24.388861 alex_ber_utils-0.8.1a4/tests/utils/splitpackage_cont/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/tests/utils/splitpackage_cont/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       34 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/tests/utils/splitpackage_cont/other_module.py
--rwxrwxrwx   0 root         (0) root         (0)     3914 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/tests/utils/threadlocal_test.py
--rwxrwxrwx   0 root         (0) root         (0)     1064 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/tests/utils/uuids_test.py
--rwxrwxrwx   0 root         (0) root         (0)    14847 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/tests/utils/ymlparsers_extra_test.py
--rwxrwxrwx   0 root         (0) root         (0)    27324 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/tests/utils/ymlparsers_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 12:30:24.410519 alex_ber_utils-0.8.1a4/tests_data/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/tests_data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 12:30:24.430255 alex_ber_utils-0.8.1a4/tests_data/tests/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/tests_data/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 12:30:24.520875 alex_ber_utils-0.8.1a4/tests_data/tests/utils/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/tests_data/tests/utils/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      135 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/tests_data/tests/utils/config.properties
--rwxrwxrwx   0 root         (0) root         (0)       81 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/tests_data/tests/utils/config2.properties
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 12:30:24.549936 alex_ber_utils-0.8.1a4/tests_data/tests/utils/initappconf/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/tests_data/tests/utils/initappconf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 12:30:24.610848 alex_ber_utils-0.8.1a4/tests_data/tests/utils/parser/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/tests_data/tests/utils/parser/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      187 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/tests_data/tests/utils/parser/config.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 12:30:24.643394 alex_ber_utils-0.8.1a4/tests_data/tests/utils/ymlparsers/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a4/tests_data/tests/utils/ymlparsers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:24:02.169125 alex_ber_utils-0.8.1a5/
+-rwxrwxrwx   0 root         (0) root         (0)    26584 2024-05-28 09:24:26.000000 alex_ber_utils-0.8.1a5/CHANGELOG.md
+-rwxrwxrwx   0 root         (0) root         (0)     1295 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/LICENSE.txt
+-rwxrwxrwx   0 root         (0) root         (0)      195 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    31537 2024-05-28 15:24:02.170125 alex_ber_utils-0.8.1a5/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     3900 2024-05-28 10:26:01.000000 alex_ber_utils-0.8.1a5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:24:01.223857 alex_ber_utils-0.8.1a5/alex_ber_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    31537 2024-05-28 15:23:59.000000 alex_ber_utils-0.8.1a5/alex_ber_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2227 2024-05-28 15:24:00.000000 alex_ber_utils-0.8.1a5/alex_ber_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 15:23:59.000000 alex_ber_utils-0.8.1a5/alex_ber_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-28 15:23:59.000000 alex_ber_utils-0.8.1a5/alex_ber_utils.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 15:23:15.000000 alex_ber_utils-0.8.1a5/alex_ber_utils.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      427 2024-05-28 15:23:59.000000 alex_ber_utils-0.8.1a5/alex_ber_utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2024-05-28 15:23:59.000000 alex_ber_utils-0.8.1a5/alex_ber_utils.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:24:01.235912 alex_ber_utils-0.8.1a5/alexber/
+-rwxrwxrwx   0 root         (0) root         (0)       55 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/alexber/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:24:01.554116 alex_ber_utils-0.8.1a5/alexber/utils/
+-rwxrwxrwx   0 root         (0) root         (0)      250 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/alexber/utils/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     8188 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/alexber/utils/_ymlparsers_extra.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:24:01.574393 alex_ber_utils-0.8.1a5/alexber/utils/data/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-28 11:54:41.000000 alex_ber_utils-0.8.1a5/alexber/utils/data/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3928 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/alexber/utils/deploys.py
+-rwxrwxrwx   0 root         (0) root         (0)    17354 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/alexber/utils/emails.py
+-rwxrwxrwx   0 root         (0) root         (0)     1425 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/alexber/utils/enums.py
+-rwxrwxrwx   0 root         (0) root         (0)     1512 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/alexber/utils/fabs.py
+-rwxrwxrwx   0 root         (0) root         (0)      857 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/alexber/utils/files.py
+-rwxrwxrwx   0 root         (0) root         (0)     3300 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/alexber/utils/importer.py
+-rwxrwxrwx   0 root         (0) root         (0)    19314 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/alexber/utils/init_app_conf.py
+-rwxrwxrwx   0 root         (0) root         (0)     1385 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/alexber/utils/inspects.py
+-rwxrwxrwx   0 root         (0) root         (0)    11144 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/alexber/utils/mains.py
+-rwxrwxrwx   0 root         (0) root         (0)     4210 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/alexber/utils/parsers.py
+-rwxrwxrwx   0 root         (0) root         (0)     1676 2024-05-28 11:55:39.000000 alex_ber_utils-0.8.1a5/alexber/utils/pprint.py
+-rwxrwxrwx   0 root         (0) root         (0)    10390 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/alexber/utils/processinvokes.py
+-rwxrwxrwx   0 root         (0) root         (0)    16921 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/alexber/utils/props.py
+-rwxrwxrwx   0 root         (0) root         (0)     2296 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/alexber/utils/setups.py
+-rwxrwxrwx   0 root         (0) root         (0)     3204 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/alexber/utils/stdlogging.py
+-rwxrwxrwx   0 root         (0) root         (0)      658 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/alexber/utils/thread_locals.py
+-rwxrwxrwx   0 root         (0) root         (0)     1745 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/alexber/utils/uuids.py
+-rwxrwxrwx   0 root         (0) root         (0)    11517 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/alexber/utils/ymlparsers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:24:01.587393 alex_ber_utils-0.8.1a5/data/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-28 11:54:41.000000 alex_ber_utils-0.8.1a5/data/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       21 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/req-env.txt
+-rwxrwxrwx   0 root         (0) root         (0)       56 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/req-fabric.txt
+-rwxrwxrwx   0 root         (0) root         (0)       18 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/req-md.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2024-05-28 15:09:21.000000 alex_ber_utils-0.8.1a5/req-piptools.txt
+-rwxrwxrwx   0 root         (0) root         (0)      113 2024-05-28 14:48:40.000000 alex_ber_utils-0.8.1a5/req-tests.txt
+-rwxrwxrwx   0 root         (0) root         (0)       32 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/req-yml.txt
+-rwxrwxrwx   0 root         (0) root         (0)       13 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/req.txt
+-rwxrwxrwx   0 root         (0) root         (0)      205 2024-05-28 14:53:19.000000 alex_ber_utils-0.8.1a5/requirements-env.txt
+-rwxrwxrwx   0 root         (0) root         (0)      670 2024-05-28 14:53:33.000000 alex_ber_utils-0.8.1a5/requirements-fabric.txt
+-rwxrwxrwx   0 root         (0) root         (0)      200 2024-05-28 14:53:45.000000 alex_ber_utils-0.8.1a5/requirements-md.txt
+-rwxrwxrwx   0 root         (0) root         (0)      601 2024-05-28 15:10:40.000000 alex_ber_utils-0.8.1a5/requirements-piptools.txt
+-rwxrwxrwx   0 root         (0) root         (0)      663 2024-05-28 15:10:10.000000 alex_ber_utils-0.8.1a5/requirements-tests.txt
+-rwxrwxrwx   0 root         (0) root         (0)      388 2024-05-28 14:54:21.000000 alex_ber_utils-0.8.1a5/requirements-yml.txt
+-rwxrwxrwx   0 root         (0) root         (0)      194 2024-05-28 14:53:06.000000 alex_ber_utils-0.8.1a5/requirements.txt
+-rwxrwxrwx   0 root         (0) root         (0)      190 2024-05-28 15:24:02.175126 alex_ber_utils-0.8.1a5/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     4905 2024-05-28 15:21:30.000000 alex_ber_utils-0.8.1a5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:24:01.608393 alex_ber_utils-0.8.1a5/tests/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/tests/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1931 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:24:01.894327 alex_ber_utils-0.8.1a5/tests/utils/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/tests/utils/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     6071 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/tests/utils/deploys_test.py
+-rwxrwxrwx   0 root         (0) root         (0)     8680 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/tests/utils/emails_test.py
+-rwxrwxrwx   0 root         (0) root         (0)    10227 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/tests/utils/enums_mixin_test.py
+-rwxrwxrwx   0 root         (0) root         (0)     5067 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/tests/utils/importer_test.py
+-rwxrwxrwx   0 root         (0) root         (0)    30475 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/tests/utils/init_app_conf_test.py
+-rwxrwxrwx   0 root         (0) root         (0)     3654 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/tests/utils/inspect_test.py
+-rwxrwxrwx   0 root         (0) root         (0)     1328 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/tests/utils/mains_test.py
+-rwxrwxrwx   0 root         (0) root         (0)     2444 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/tests/utils/method_overloading_test.py
+-rwxrwxrwx   0 root         (0) root         (0)     5106 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/tests/utils/parsers_test.py
+-rwxrwxrwx   0 root         (0) root         (0)     2157 2024-05-28 15:18:02.000000 alex_ber_utils-0.8.1a5/tests/utils/pprint_test.py
+-rwxrwxrwx   0 root         (0) root         (0)     5372 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/tests/utils/processinvokes_test.py
+-rwxrwxrwx   0 root         (0) root         (0)     2047 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/tests/utils/properties_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:24:01.930877 alex_ber_utils-0.8.1a5/tests/utils/splitpackage/
+-rwxrwxrwx   0 root         (0) root         (0)      116 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/tests/utils/splitpackage/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/tests/utils/splitpackage/mymodule.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:24:01.966098 alex_ber_utils-0.8.1a5/tests/utils/splitpackage_cont/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/tests/utils/splitpackage_cont/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       34 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/tests/utils/splitpackage_cont/other_module.py
+-rwxrwxrwx   0 root         (0) root         (0)     3914 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/tests/utils/threadlocal_test.py
+-rwxrwxrwx   0 root         (0) root         (0)     1064 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/tests/utils/uuids_test.py
+-rwxrwxrwx   0 root         (0) root         (0)    14847 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/tests/utils/ymlparsers_extra_test.py
+-rwxrwxrwx   0 root         (0) root         (0)    27324 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/tests/utils/ymlparsers_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:24:01.979099 alex_ber_utils-0.8.1a5/tests_data/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/tests_data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:24:01.993098 alex_ber_utils-0.8.1a5/tests_data/tests/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/tests_data/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:24:02.053757 alex_ber_utils-0.8.1a5/tests_data/tests/utils/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/tests_data/tests/utils/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      135 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/tests_data/tests/utils/config.properties
+-rwxrwxrwx   0 root         (0) root         (0)       81 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/tests_data/tests/utils/config2.properties
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:24:02.074273 alex_ber_utils-0.8.1a5/tests_data/tests/utils/initappconf/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/tests_data/tests/utils/initappconf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:24:02.134464 alex_ber_utils-0.8.1a5/tests_data/tests/utils/parser/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/tests_data/tests/utils/parser/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      187 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/tests_data/tests/utils/parser/config.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:24:02.155037 alex_ber_utils-0.8.1a5/tests_data/tests/utils/ymlparsers/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a5/tests_data/tests/utils/ymlparsers/__init__.py
```

### Comparing `alex_ber_utils-0.8.1a4/CHANGELOG.md` & `alex_ber_utils-0.8.1a5/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a4/LICENSE.txt` & `alex_ber_utils-0.8.1a5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a4/PKG-INFO` & `alex_ber_utils-0.8.1a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alex_ber_utils
-Version: 0.8.1a4
+Version: 0.8.1a5
 Summary: AlexBerUtils is collection of the small utilities
 Home-page: https://github.com/alex-ber/AlexBerUtils
 Author: Alexander Berkovich
 License: Apache 2.0
 Keywords: tools tool utils enum enums threadlocal UploadCommand upload uuid1mc uuid UUID UUID1 UUID4 UU1DMC issetdescriptor ismethod importer new_instance safe_eval is_empty parse_boolean Properties java.util.Properties
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `alex_ber_utils-0.8.1a4/README.md` & `alex_ber_utils-0.8.1a5/README.md`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a4/alex_ber_utils.egg-info/PKG-INFO` & `alex_ber_utils-0.8.1a5/alex_ber_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alex-ber-utils
-Version: 0.8.1a4
+Version: 0.8.1a5
 Summary: AlexBerUtils is collection of the small utilities
 Home-page: https://github.com/alex-ber/AlexBerUtils
 Author: Alexander Berkovich
 License: Apache 2.0
 Keywords: tools tool utils enum enums threadlocal UploadCommand upload uuid1mc uuid UUID UUID1 UUID4 UU1DMC issetdescriptor ismethod importer new_instance safe_eval is_empty parse_boolean Properties java.util.Properties
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `alex_ber_utils-0.8.1a4/alex_ber_utils.egg-info/SOURCES.txt` & `alex_ber_utils-0.8.1a5/alex_ber_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a4/alexber/utils/_ymlparsers_extra.py` & `alex_ber_utils-0.8.1a5/alexber/utils/_ymlparsers_extra.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a4/alexber/utils/deploys.py` & `alex_ber_utils-0.8.1a5/alexber/utils/deploys.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a4/alexber/utils/emails.py` & `alex_ber_utils-0.8.1a5/alexber/utils/emails.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a4/alexber/utils/enums.py` & `alex_ber_utils-0.8.1a5/alexber/utils/enums.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a4/alexber/utils/fabs.py` & `alex_ber_utils-0.8.1a5/alexber/utils/fabs.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a4/alexber/utils/files.py` & `alex_ber_utils-0.8.1a5/alexber/utils/files.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a4/alexber/utils/importer.py` & `alex_ber_utils-0.8.1a5/alexber/utils/importer.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a4/alexber/utils/init_app_conf.py` & `alex_ber_utils-0.8.1a5/alexber/utils/init_app_conf.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a4/alexber/utils/inspects.py` & `alex_ber_utils-0.8.1a5/alexber/utils/inspects.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a4/alexber/utils/mains.py` & `alex_ber_utils-0.8.1a5/alexber/utils/mains.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a4/alexber/utils/parsers.py` & `alex_ber_utils-0.8.1a5/alexber/utils/parsers.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a4/alexber/utils/pprint.py` & `alex_ber_utils-0.8.1a5/alexber/utils/pprint.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a4/alexber/utils/processinvokes.py` & `alex_ber_utils-0.8.1a5/alexber/utils/processinvokes.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a4/alexber/utils/props.py` & `alex_ber_utils-0.8.1a5/alexber/utils/props.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a4/alexber/utils/setups.py` & `alex_ber_utils-0.8.1a5/alexber/utils/setups.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a4/alexber/utils/stdlogging.py` & `alex_ber_utils-0.8.1a5/alexber/utils/stdlogging.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a4/alexber/utils/thread_locals.py` & `alex_ber_utils-0.8.1a5/alexber/utils/thread_locals.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a4/alexber/utils/uuids.py` & `alex_ber_utils-0.8.1a5/alexber/utils/uuids.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a4/alexber/utils/ymlparsers.py` & `alex_ber_utils-0.8.1a5/alexber/utils/ymlparsers.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a4/requirements-fabric.txt` & `alex_ber_utils-0.8.1a5/requirements-fabric.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    pip-compile --output-file=requirements-fabric.txt req-fabric.txt
 #
 bcrypt==4.1.3
     # via paramiko
 cffi==1.16.0
```

### Comparing `alex_ber_utils-0.8.1a4/requirements-piptools.txt` & `alex_ber_utils-0.8.1a5/requirements-piptools.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    pip-compile --output-file=requirements-piptools.txt req-piptools.txt
 #
 build==1.2.1
     # via pip-tools
 click==8.1.7
     # via pip-tools
-importlib-metadata==7.1.0
-    # via build
-packaging==24.0
-    # via build
+packaging==23.2
+    # via
+    #   -r req-piptools.txt
+    #   build
 pip-tools==7.4.1
     # via -r req-piptools.txt
 pyproject-hooks==1.1.0
     # via
     #   build
     #   pip-tools
 tomli==2.0.1
     # via
     #   build
     #   pip-tools
 wheel==0.43.0
     # via pip-tools
-zipp==3.19.0
-    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # pip
 # setuptools
```

### Comparing `alex_ber_utils-0.8.1a4/requirements-tests.txt` & `alex_ber_utils-0.8.1a5/requirements-tests.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    pip-compile --output-file=requirements-tests.txt req-tests.txt
 #
 exceptiongroup==1.2.1
     # via pytest
 iniconfig==2.0.0
     # via pytest
-packaging==24.0
+packaging==23.2
     # via
     #   -r req-tests.txt
     #   pytest
 pluggy==1.5.0
     # via pytest
 pytest==7.4.3
     # via
```

### Comparing `alex_ber_utils-0.8.1a4/setup.py` & `alex_ber_utils-0.8.1a5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 
 import setuptools
 from setuptools import setup
 
 
 #VERSION should be defined before importing UploadCommand
-VERSION = '0.8.1a4'
+VERSION = '0.8.1a5'
 from alexber.utils import UploadCommand
 NAME = 'alex_ber_utils'
 SHORT_NAME = 'utils'
 VCS_URL = 'https://github.com/alex-ber/AlexBerUtils'
 DESCRIPTION = 'AlexBerUtils is collection of the small utilities'
 AUTHOR = 'Alexander Berkovich'
```

### Comparing `alex_ber_utils-0.8.1a4/tests/conftest.py` & `alex_ber_utils-0.8.1a5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a4/tests/utils/deploys_test.py` & `alex_ber_utils-0.8.1a5/tests/utils/deploys_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a4/tests/utils/emails_test.py` & `alex_ber_utils-0.8.1a5/tests/utils/emails_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a4/tests/utils/enums_mixin_test.py` & `alex_ber_utils-0.8.1a5/tests/utils/enums_mixin_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a4/tests/utils/importer_test.py` & `alex_ber_utils-0.8.1a5/tests/utils/importer_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a4/tests/utils/init_app_conf_test.py` & `alex_ber_utils-0.8.1a5/tests/utils/init_app_conf_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a4/tests/utils/inspect_test.py` & `alex_ber_utils-0.8.1a5/tests/utils/inspect_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a4/tests/utils/mains_test.py` & `alex_ber_utils-0.8.1a5/tests/utils/mains_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a4/tests/utils/method_overloading_test.py` & `alex_ber_utils-0.8.1a5/tests/utils/method_overloading_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a4/tests/utils/parsers_test.py` & `alex_ber_utils-0.8.1a5/tests/utils/parsers_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a4/tests/utils/pprint_test.py` & `alex_ber_utils-0.8.1a5/tests/utils/pprint_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a4/tests/utils/processinvokes_test.py` & `alex_ber_utils-0.8.1a5/tests/utils/processinvokes_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a4/tests/utils/properties_test.py` & `alex_ber_utils-0.8.1a5/tests/utils/properties_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a4/tests/utils/threadlocal_test.py` & `alex_ber_utils-0.8.1a5/tests/utils/threadlocal_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a4/tests/utils/uuids_test.py` & `alex_ber_utils-0.8.1a5/tests/utils/uuids_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a4/tests/utils/ymlparsers_extra_test.py` & `alex_ber_utils-0.8.1a5/tests/utils/ymlparsers_extra_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a4/tests/utils/ymlparsers_test.py` & `alex_ber_utils-0.8.1a5/tests/utils/ymlparsers_test.py`

 * *Files identical despite different names*

