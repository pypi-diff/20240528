# Comparing `tmp/alex_ber_utils-0.8.1a2.tar.gz` & `tmp/alex_ber_utils-0.8.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alex_ber_utils-0.8.1a2.tar", last modified: Tue May 28 10:00:11 2024, max compression
+gzip compressed data, was "alex_ber_utils-0.8.1a3.tar", last modified: Tue May 28 10:37:46 2024, max compression
```

## Comparing `alex_ber_utils-0.8.1a2.tar` & `alex_ber_utils-0.8.1a3.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:00:11.089646 alex_ber_utils-0.8.1a2/
--rwxrwxrwx   0 root         (0) root         (0)    26584 2024-05-28 09:24:26.000000 alex_ber_utils-0.8.1a2/CHANGELOG.md
--rwxrwxrwx   0 root         (0) root         (0)     1295 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/LICENSE.txt
--rwxrwxrwx   0 root         (0) root         (0)      195 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    31537 2024-05-28 10:00:11.090646 alex_ber_utils-0.8.1a2/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     3748 2024-01-28 16:28:53.000000 alex_ber_utils-0.8.1a2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:00:10.128175 alex_ber_utils-0.8.1a2/alex_ber_utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)    31537 2024-05-28 10:00:08.000000 alex_ber_utils-0.8.1a2/alex_ber_utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2227 2024-05-28 10:00:09.000000 alex_ber_utils-0.8.1a2/alex_ber_utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 10:00:08.000000 alex_ber_utils-0.8.1a2/alex_ber_utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-28 10:00:08.000000 alex_ber_utils-0.8.1a2/alex_ber_utils.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 09:52:52.000000 alex_ber_utils-0.8.1a2/alex_ber_utils.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      427 2024-05-28 10:00:08.000000 alex_ber_utils-0.8.1a2/alex_ber_utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2024-05-28 10:00:08.000000 alex_ber_utils-0.8.1a2/alex_ber_utils.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:00:10.144635 alex_ber_utils-0.8.1a2/alexber/
--rwxrwxrwx   0 root         (0) root         (0)       55 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/alexber/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:00:10.492171 alex_ber_utils-0.8.1a2/alexber/utils/
--rwxrwxrwx   0 root         (0) root         (0)      250 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/alexber/utils/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     8188 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/alexber/utils/_ymlparsers_extra.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:00:10.512892 alex_ber_utils-0.8.1a2/alexber/utils/data/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/alexber/utils/data/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3928 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/alexber/utils/deploys.py
--rwxrwxrwx   0 root         (0) root         (0)    17354 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/alexber/utils/emails.py
--rwxrwxrwx   0 root         (0) root         (0)     1425 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/alexber/utils/enums.py
--rwxrwxrwx   0 root         (0) root         (0)     1512 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/alexber/utils/fabs.py
--rwxrwxrwx   0 root         (0) root         (0)      857 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/alexber/utils/files.py
--rwxrwxrwx   0 root         (0) root         (0)     3300 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/alexber/utils/importer.py
--rwxrwxrwx   0 root         (0) root         (0)    19314 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/alexber/utils/init_app_conf.py
--rwxrwxrwx   0 root         (0) root         (0)     1385 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/alexber/utils/inspects.py
--rwxrwxrwx   0 root         (0) root         (0)    11144 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/alexber/utils/mains.py
--rwxrwxrwx   0 root         (0) root         (0)     4210 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/alexber/utils/parsers.py
--rwxrwxrwx   0 root         (0) root         (0)     1316 2024-05-28 09:20:53.000000 alex_ber_utils-0.8.1a2/alexber/utils/pprint.py
--rwxrwxrwx   0 root         (0) root         (0)    10390 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/alexber/utils/processinvokes.py
--rwxrwxrwx   0 root         (0) root         (0)    16921 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/alexber/utils/props.py
--rwxrwxrwx   0 root         (0) root         (0)     2296 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/alexber/utils/setups.py
--rwxrwxrwx   0 root         (0) root         (0)     3204 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/alexber/utils/stdlogging.py
--rwxrwxrwx   0 root         (0) root         (0)      658 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/alexber/utils/thread_locals.py
--rwxrwxrwx   0 root         (0) root         (0)     1745 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/alexber/utils/uuids.py
--rwxrwxrwx   0 root         (0) root         (0)    11517 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/alexber/utils/ymlparsers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:00:10.526102 alex_ber_utils-0.8.1a2/data/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/data/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       21 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/req-env.txt
--rwxrwxrwx   0 root         (0) root         (0)       56 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/req-fabric.txt
--rwxrwxrwx   0 root         (0) root         (0)       18 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/req-md.txt
--rwxrwxrwx   0 root         (0) root         (0)       17 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/req-piptools.txt
--rwxrwxrwx   0 root         (0) root         (0)       92 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/req-tests.txt
--rwxrwxrwx   0 root         (0) root         (0)       32 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/req-yml.txt
--rwxrwxrwx   0 root         (0) root         (0)       13 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/req.txt
--rwxrwxrwx   0 root         (0) root         (0)       20 2024-05-28 08:02:25.000000 alex_ber_utils-0.8.1a2/requirements-env.txt
--rwxrwxrwx   0 root         (0) root         (0)      636 2024-05-28 08:29:11.000000 alex_ber_utils-0.8.1a2/requirements-fabric.txt
--rwxrwxrwx   0 root         (0) root         (0)      184 2024-05-28 08:29:34.000000 alex_ber_utils-0.8.1a2/requirements-md.txt
--rwxrwxrwx   0 root         (0) root         (0)      523 2024-05-28 08:30:05.000000 alex_ber_utils-0.8.1a2/requirements-piptools.txt
--rwxrwxrwx   0 root         (0) root         (0)      605 2024-05-28 08:30:34.000000 alex_ber_utils-0.8.1a2/requirements-tests.txt
--rwxrwxrwx   0 root         (0) root         (0)      369 2024-05-28 08:33:31.000000 alex_ber_utils-0.8.1a2/requirements-yml.txt
--rwxrwxrwx   0 root         (0) root         (0)      171 2024-05-28 08:33:31.000000 alex_ber_utils-0.8.1a2/requirements.txt
--rwxrwxrwx   0 root         (0) root         (0)      190 2024-05-28 10:00:11.095645 alex_ber_utils-0.8.1a2/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     4905 2024-05-28 09:59:57.000000 alex_ber_utils-0.8.1a2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:00:10.548371 alex_ber_utils-0.8.1a2/tests/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1931 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:00:10.827083 alex_ber_utils-0.8.1a2/tests/utils/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests/utils/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     6071 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests/utils/deploys_test.py
--rwxrwxrwx   0 root         (0) root         (0)     8680 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests/utils/emails_test.py
--rwxrwxrwx   0 root         (0) root         (0)    10227 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests/utils/enums_mixin_test.py
--rwxrwxrwx   0 root         (0) root         (0)     5067 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests/utils/importer_test.py
--rwxrwxrwx   0 root         (0) root         (0)    30475 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests/utils/init_app_conf_test.py
--rwxrwxrwx   0 root         (0) root         (0)     3654 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests/utils/inspect_test.py
--rwxrwxrwx   0 root         (0) root         (0)     1328 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests/utils/mains_test.py
--rwxrwxrwx   0 root         (0) root         (0)     2444 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests/utils/method_overloading_test.py
--rwxrwxrwx   0 root         (0) root         (0)     5106 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests/utils/parsers_test.py
--rwxrwxrwx   0 root         (0) root         (0)     2157 2024-05-28 09:22:01.000000 alex_ber_utils-0.8.1a2/tests/utils/pprint_test.py
--rwxrwxrwx   0 root         (0) root         (0)     5372 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests/utils/processinvokes_test.py
--rwxrwxrwx   0 root         (0) root         (0)     2047 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests/utils/properties_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:00:10.864784 alex_ber_utils-0.8.1a2/tests/utils/splitpackage/
--rwxrwxrwx   0 root         (0) root         (0)      116 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests/utils/splitpackage/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests/utils/splitpackage/mymodule.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:00:10.899850 alex_ber_utils-0.8.1a2/tests/utils/splitpackage_cont/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests/utils/splitpackage_cont/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       34 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests/utils/splitpackage_cont/other_module.py
--rwxrwxrwx   0 root         (0) root         (0)     3914 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests/utils/threadlocal_test.py
--rwxrwxrwx   0 root         (0) root         (0)     1064 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests/utils/uuids_test.py
--rwxrwxrwx   0 root         (0) root         (0)    14847 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests/utils/ymlparsers_extra_test.py
--rwxrwxrwx   0 root         (0) root         (0)    27324 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests/utils/ymlparsers_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:00:10.914970 alex_ber_utils-0.8.1a2/tests_data/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests_data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:00:10.928026 alex_ber_utils-0.8.1a2/tests_data/tests/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests_data/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:00:10.991455 alex_ber_utils-0.8.1a2/tests_data/tests/utils/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests_data/tests/utils/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      135 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests_data/tests/utils/config.properties
--rwxrwxrwx   0 root         (0) root         (0)       81 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests_data/tests/utils/config2.properties
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:00:11.011943 alex_ber_utils-0.8.1a2/tests_data/tests/utils/initappconf/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests_data/tests/utils/initappconf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:00:11.053488 alex_ber_utils-0.8.1a2/tests_data/tests/utils/parser/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests_data/tests/utils/parser/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      187 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests_data/tests/utils/parser/config.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:00:11.075644 alex_ber_utils-0.8.1a2/tests_data/tests/utils/ymlparsers/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests_data/tests/utils/ymlparsers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:37:46.163744 alex_ber_utils-0.8.1a3/
+-rwxrwxrwx   0 root         (0) root         (0)    26584 2024-05-28 09:24:26.000000 alex_ber_utils-0.8.1a3/CHANGELOG.md
+-rwxrwxrwx   0 root         (0) root         (0)     1295 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/LICENSE.txt
+-rwxrwxrwx   0 root         (0) root         (0)      195 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    31537 2024-05-28 10:37:46.164745 alex_ber_utils-0.8.1a3/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     3900 2024-05-28 10:26:01.000000 alex_ber_utils-0.8.1a3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:37:45.185086 alex_ber_utils-0.8.1a3/alex_ber_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    31537 2024-05-28 10:37:44.000000 alex_ber_utils-0.8.1a3/alex_ber_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2227 2024-05-28 10:37:44.000000 alex_ber_utils-0.8.1a3/alex_ber_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 10:37:44.000000 alex_ber_utils-0.8.1a3/alex_ber_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-28 10:37:44.000000 alex_ber_utils-0.8.1a3/alex_ber_utils.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 10:35:38.000000 alex_ber_utils-0.8.1a3/alex_ber_utils.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      427 2024-05-28 10:37:44.000000 alex_ber_utils-0.8.1a3/alex_ber_utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2024-05-28 10:37:44.000000 alex_ber_utils-0.8.1a3/alex_ber_utils.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:37:45.199310 alex_ber_utils-0.8.1a3/alexber/
+-rwxrwxrwx   0 root         (0) root         (0)       55 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/alexber/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:37:45.521759 alex_ber_utils-0.8.1a3/alexber/utils/
+-rwxrwxrwx   0 root         (0) root         (0)      250 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/alexber/utils/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     8188 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/alexber/utils/_ymlparsers_extra.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:37:45.540902 alex_ber_utils-0.8.1a3/alexber/utils/data/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/alexber/utils/data/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3928 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/alexber/utils/deploys.py
+-rwxrwxrwx   0 root         (0) root         (0)    17354 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/alexber/utils/emails.py
+-rwxrwxrwx   0 root         (0) root         (0)     1425 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/alexber/utils/enums.py
+-rwxrwxrwx   0 root         (0) root         (0)     1512 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/alexber/utils/fabs.py
+-rwxrwxrwx   0 root         (0) root         (0)      857 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/alexber/utils/files.py
+-rwxrwxrwx   0 root         (0) root         (0)     3300 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/alexber/utils/importer.py
+-rwxrwxrwx   0 root         (0) root         (0)    19314 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/alexber/utils/init_app_conf.py
+-rwxrwxrwx   0 root         (0) root         (0)     1385 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/alexber/utils/inspects.py
+-rwxrwxrwx   0 root         (0) root         (0)    11144 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/alexber/utils/mains.py
+-rwxrwxrwx   0 root         (0) root         (0)     4210 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/alexber/utils/parsers.py
+-rwxrwxrwx   0 root         (0) root         (0)     1316 2024-05-28 09:20:53.000000 alex_ber_utils-0.8.1a3/alexber/utils/pprint.py
+-rwxrwxrwx   0 root         (0) root         (0)    10390 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/alexber/utils/processinvokes.py
+-rwxrwxrwx   0 root         (0) root         (0)    16921 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/alexber/utils/props.py
+-rwxrwxrwx   0 root         (0) root         (0)     2296 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/alexber/utils/setups.py
+-rwxrwxrwx   0 root         (0) root         (0)     3204 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/alexber/utils/stdlogging.py
+-rwxrwxrwx   0 root         (0) root         (0)      658 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/alexber/utils/thread_locals.py
+-rwxrwxrwx   0 root         (0) root         (0)     1745 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/alexber/utils/uuids.py
+-rwxrwxrwx   0 root         (0) root         (0)    11517 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/alexber/utils/ymlparsers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:37:45.555005 alex_ber_utils-0.8.1a3/data/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/data/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       21 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/req-env.txt
+-rwxrwxrwx   0 root         (0) root         (0)       56 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/req-fabric.txt
+-rwxrwxrwx   0 root         (0) root         (0)       18 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/req-md.txt
+-rwxrwxrwx   0 root         (0) root         (0)       17 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/req-piptools.txt
+-rwxrwxrwx   0 root         (0) root         (0)       92 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/req-tests.txt
+-rwxrwxrwx   0 root         (0) root         (0)       32 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/req-yml.txt
+-rwxrwxrwx   0 root         (0) root         (0)       13 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/req.txt
+-rwxrwxrwx   0 root         (0) root         (0)       20 2024-05-28 08:02:25.000000 alex_ber_utils-0.8.1a3/requirements-env.txt
+-rwxrwxrwx   0 root         (0) root         (0)      636 2024-05-28 08:29:11.000000 alex_ber_utils-0.8.1a3/requirements-fabric.txt
+-rwxrwxrwx   0 root         (0) root         (0)      184 2024-05-28 08:29:34.000000 alex_ber_utils-0.8.1a3/requirements-md.txt
+-rwxrwxrwx   0 root         (0) root         (0)      523 2024-05-28 08:30:05.000000 alex_ber_utils-0.8.1a3/requirements-piptools.txt
+-rwxrwxrwx   0 root         (0) root         (0)      605 2024-05-28 08:30:34.000000 alex_ber_utils-0.8.1a3/requirements-tests.txt
+-rwxrwxrwx   0 root         (0) root         (0)      369 2024-05-28 08:33:31.000000 alex_ber_utils-0.8.1a3/requirements-yml.txt
+-rwxrwxrwx   0 root         (0) root         (0)      171 2024-05-28 08:33:31.000000 alex_ber_utils-0.8.1a3/requirements.txt
+-rwxrwxrwx   0 root         (0) root         (0)      190 2024-05-28 10:37:46.169745 alex_ber_utils-0.8.1a3/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     4905 2024-05-28 10:37:21.000000 alex_ber_utils-0.8.1a3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:37:45.576437 alex_ber_utils-0.8.1a3/tests/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/tests/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1931 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:37:45.893214 alex_ber_utils-0.8.1a3/tests/utils/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/tests/utils/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     6071 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/tests/utils/deploys_test.py
+-rwxrwxrwx   0 root         (0) root         (0)     8680 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/tests/utils/emails_test.py
+-rwxrwxrwx   0 root         (0) root         (0)    10227 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/tests/utils/enums_mixin_test.py
+-rwxrwxrwx   0 root         (0) root         (0)     5067 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/tests/utils/importer_test.py
+-rwxrwxrwx   0 root         (0) root         (0)    30475 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/tests/utils/init_app_conf_test.py
+-rwxrwxrwx   0 root         (0) root         (0)     3654 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/tests/utils/inspect_test.py
+-rwxrwxrwx   0 root         (0) root         (0)     1328 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/tests/utils/mains_test.py
+-rwxrwxrwx   0 root         (0) root         (0)     2444 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/tests/utils/method_overloading_test.py
+-rwxrwxrwx   0 root         (0) root         (0)     5106 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/tests/utils/parsers_test.py
+-rwxrwxrwx   0 root         (0) root         (0)     2157 2024-05-28 09:22:01.000000 alex_ber_utils-0.8.1a3/tests/utils/pprint_test.py
+-rwxrwxrwx   0 root         (0) root         (0)     5372 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/tests/utils/processinvokes_test.py
+-rwxrwxrwx   0 root         (0) root         (0)     2047 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/tests/utils/properties_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:37:45.932417 alex_ber_utils-0.8.1a3/tests/utils/splitpackage/
+-rwxrwxrwx   0 root         (0) root         (0)      116 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/tests/utils/splitpackage/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/tests/utils/splitpackage/mymodule.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:37:45.968492 alex_ber_utils-0.8.1a3/tests/utils/splitpackage_cont/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/tests/utils/splitpackage_cont/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       34 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/tests/utils/splitpackage_cont/other_module.py
+-rwxrwxrwx   0 root         (0) root         (0)     3914 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/tests/utils/threadlocal_test.py
+-rwxrwxrwx   0 root         (0) root         (0)     1064 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/tests/utils/uuids_test.py
+-rwxrwxrwx   0 root         (0) root         (0)    14847 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/tests/utils/ymlparsers_extra_test.py
+-rwxrwxrwx   0 root         (0) root         (0)    27324 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/tests/utils/ymlparsers_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:37:45.983996 alex_ber_utils-0.8.1a3/tests_data/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/tests_data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:37:45.997973 alex_ber_utils-0.8.1a3/tests_data/tests/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/tests_data/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:37:46.063219 alex_ber_utils-0.8.1a3/tests_data/tests/utils/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/tests_data/tests/utils/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      135 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/tests_data/tests/utils/config.properties
+-rwxrwxrwx   0 root         (0) root         (0)       81 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/tests_data/tests/utils/config2.properties
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:37:46.084456 alex_ber_utils-0.8.1a3/tests_data/tests/utils/initappconf/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/tests_data/tests/utils/initappconf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:37:46.126551 alex_ber_utils-0.8.1a3/tests_data/tests/utils/parser/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/tests_data/tests/utils/parser/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      187 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/tests_data/tests/utils/parser/config.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:37:46.149680 alex_ber_utils-0.8.1a3/tests_data/tests/utils/ymlparsers/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a3/tests_data/tests/utils/ymlparsers/__init__.py
```

### Comparing `alex_ber_utils-0.8.1a2/CHANGELOG.md` & `alex_ber_utils-0.8.1a3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a2/LICENSE.txt` & `alex_ber_utils-0.8.1a3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a2/PKG-INFO` & `alex_ber_utils-0.8.1a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alex_ber_utils
-Version: 0.8.1a2
+Version: 0.8.1a3
 Summary: AlexBerUtils is collection of the small utilities
 Home-page: https://github.com/alex-ber/AlexBerUtils
 Author: Alexander Berkovich
 License: Apache 2.0
 Keywords: tools tool utils enum enums threadlocal UploadCommand upload uuid1mc uuid UUID UUID1 UUID4 UU1DMC issetdescriptor ismethod importer new_instance safe_eval is_empty parse_boolean Properties java.util.Properties
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `alex_ber_utils-0.8.1a2/README.md` & `alex_ber_utils-0.8.1a3/README.md`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,152 +1,152 @@
-## AlexBerUtils
-
-AlexBerUtils is collection of the small utilities. See CHANGELOG.md for detail description.
-
-
-
-### Getting Help
-
-
-### QuickStart
-```bash
-python3 -m pip install -U alex-ber-utils
-```
-
-
-### Installing from Github
-
-```bash
-python3 -m pip install -U https://github.com/alex-ber/AlexBerUtils/archive/master.zip
-```
-Optionally installing tests requirements.
-
-```bash
-python3 -m pip install -U https://github.com/alex-ber/AlexBerUtils/archive/master.zip#egg=alex-ber-utils[tests]
-```
-
-Or explicitly:
-
-```bash
-wget https://github.com/alex-ber/AlexBerUtils/archive/master.zip -O master.zip; unzip master.zip; rm master.zip
-```
-And then installing from source (see below).
-
-
-### Installing from source
-```bash
-python3 -m pip install . # only installs "required"
-```
-```bash
-python3 -m pip install .[tests] # installs dependencies for tests
-```
-```bash
-python3 -m pip install .[piptools] # installs dependencies for pip-tools
-```
-```bash
-python3 -m pip install .[md]   # installs multidispatcher (used in method_overloading_test.py)
-```
-```bash
-python3 -m pip install .[fabric]   # installs fabric (used in fabs.py)
-```
-```bash
-python3 -m pip install .[yml]   # installs Yml related dependencies 
-                                # (used in ymlparsers.py, init_app_conf.py, deploys.py;
-                                # optionally used in ymlparsers_extra.py, emails.py)
-```
-```bash
-python3 -m pip install .[env]   # installs pydotenv (optionally used in deploys.py and mains.py)
-```
-
-#### Alternatively you install from requirements file:
-```bash
-python3 -m pip install -r requirements.txt # only installs "required"
-```
-```bash
-python3 -m pip install -r requirements-tests.txt # installs dependencies for tests
-```
-```bash
-python3 -m pip install -r requirements-piptools.txt # installs dependencies for pip-tools
-```
-```bash
-python3 -m pip install -r requirements-md.txt   # installs multidispatcher (used in method_overloading_test.py)
-```
-```bash
-python3 -m pip install -r requirements-fabric.txt   # installs fabric (used in fabs.py)
-```
-```bash
-python3 -m pip install -r requirements-yml.txt   # installs Yml related dependencies 
-                                                 # (used in ymlparsers.py, init_app_conf.py, deploys.py;
-                                                 # optionally used in ymlparsers_extra.py, emails.py)
-```
-```bash
-python3 -m pip install -r requirements-env.txt   # installs pydotenv (optionally used in deploys.py)
-```
-
-### Using Docker
-`alexberkovich/AlexBerUtils:latest`  contains all `AlexBerUtils` dependencies.
-This Dockerfile is very simple, you can take relevant part for you and put them into your Dockerfile.
-
-##
-Alternatively, you can use it as base Docker image for your project and add/upgrade 
-another dependencies as you need.
-
-For example:
-
-```Dockerfile
-FROM alexberkovich/alex_ber_utils:latest
-
-COPY requirements.txt etc/requirements.txt
-
-RUN set -ex && \
-    #latest pip,setuptools,wheel
-    pip install --upgrade pip setuptools wheel && \
-    pip install alex_ber_utils 
-    pip install -r etc/requirements.txt 
-
-CMD ["/bin/sh"]
-#CMD tail -f /dev/null
-```
-
-where `requirements.txt` is requirements for your project.
-
-  
-
-##
-
-From the directory with setup.py
-```bash
-python3 setup.py test #run all tests
-```
-
-or
-
-```bash
-
-pytest
-```
-
-## Installing new version
-See https://docs.python.org/3.1/distutils/uploading.html 
-
-
-## Installing new version to venv
-```bash
-python38 -m pip uninstall --yes alex_ber_utils
-python38 setup.py clean sdist bdist_wheel
-python38 -m pip install --find-links=./dist alex_ber_utils==0.6.5
-```
-
-##Manual upload
-```bash
-#python setup.py clean sdist upload
-```
-
-
-## Requirements
-
-
-AlexBerUtils requires the following modules.
-
-* Python 3.6+
-
-* PyYAML>=6.0.1
+## AlexBerUtils
+
+AlexBerUtils is collection of the small utilities. See CHANGELOG.md for detail description.
+
+
+
+### Getting Help
+
+
+### QuickStart
+```bash
+python3 -m pip install -U alex-ber-utils
+```
+
+
+### Installing from Github
+
+```bash
+python3 -m pip install -U https://github.com/alex-ber/AlexBerUtils/archive/master.zip
+```
+Optionally installing tests requirements.
+
+```bash
+python3 -m pip install -U https://github.com/alex-ber/AlexBerUtils/archive/master.zip#egg=alex-ber-utils[tests]
+```
+
+Or explicitly:
+
+```bash
+wget https://github.com/alex-ber/AlexBerUtils/archive/master.zip -O master.zip; unzip master.zip; rm master.zip
+```
+And then installing from source (see below).
+
+
+### Installing from source
+```bash
+python3 -m pip install . # only installs "required"
+```
+```bash
+python3 -m pip install .[tests] # installs dependencies for tests
+```
+```bash
+python3 -m pip install .[piptools] # installs dependencies for pip-tools
+```
+```bash
+python3 -m pip install .[md]   # installs multidispatcher (used in method_overloading_test.py)
+```
+```bash
+python3 -m pip install .[fabric]   # installs fabric (used in fabs.py)
+```
+```bash
+python3 -m pip install .[yml]   # installs Yml related dependencies 
+                                # (used in ymlparsers.py, init_app_conf.py, deploys.py;
+                                # optionally used in ymlparsers_extra.py, emails.py)
+```
+```bash
+python3 -m pip install .[env]   # installs pydotenv (optionally used in deploys.py and mains.py)
+```
+
+#### Alternatively you install from requirements file:
+```bash
+python3 -m pip install -r requirements.txt # only installs "required"
+```
+```bash
+python3 -m pip install -r requirements-tests.txt # installs dependencies for tests
+```
+```bash
+python3 -m pip install -r requirements-piptools.txt # installs dependencies for pip-tools
+```
+```bash
+python3 -m pip install -r requirements-md.txt   # installs multidispatcher (used in method_overloading_test.py)
+```
+```bash
+python3 -m pip install -r requirements-fabric.txt   # installs fabric (used in fabs.py)
+```
+```bash
+python3 -m pip install -r requirements-yml.txt   # installs Yml related dependencies 
+                                                 # (used in ymlparsers.py, init_app_conf.py, deploys.py;
+                                                 # optionally used in ymlparsers_extra.py, emails.py)
+```
+```bash
+python3 -m pip install -r requirements-env.txt   # installs pydotenv (optionally used in deploys.py)
+```
+
+### Using Docker
+`alexberkovich/AlexBerUtils:latest`  contains all `AlexBerUtils` dependencies.
+This Dockerfile is very simple, you can take relevant part for you and put them into your Dockerfile.
+
+##
+Alternatively, you can use it as base Docker image for your project and add/upgrade 
+another dependencies as you need.
+
+For example:
+
+```Dockerfile
+FROM alexberkovich/alex_ber_utils:latest
+
+COPY requirements.txt etc/requirements.txt
+
+RUN set -ex && \
+    #latest pip,setuptools,wheel
+    pip install --upgrade pip setuptools wheel && \
+    pip install alex_ber_utils 
+    pip install -r etc/requirements.txt 
+
+CMD ["/bin/sh"]
+#CMD tail -f /dev/null
+```
+
+where `requirements.txt` is requirements for your project.
+
+  
+
+##
+
+From the directory with setup.py
+```bash
+python3 setup.py test #run all tests
+```
+
+or
+
+```bash
+
+pytest
+```
+
+## Installing new version
+See https://docs.python.org/3.1/distutils/uploading.html 
+
+
+## Installing new version to venv
+```bash
+python38 -m pip uninstall --yes alex_ber_utils
+python38 setup.py clean sdist bdist_wheel
+python38 -m pip install --find-links=./dist alex_ber_utils==0.6.5
+```
+
+##Manual upload
+```bash
+#python setup.py clean sdist upload
+```
+
+
+## Requirements
+
+
+AlexBerUtils requires the following modules.
+
+* Python 3.6+
+
+* PyYAML>=6.0.1
```

### Comparing `alex_ber_utils-0.8.1a2/alex_ber_utils.egg-info/PKG-INFO` & `alex_ber_utils-0.8.1a3/alex_ber_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alex-ber-utils
-Version: 0.8.1a2
+Version: 0.8.1a3
 Summary: AlexBerUtils is collection of the small utilities
 Home-page: https://github.com/alex-ber/AlexBerUtils
 Author: Alexander Berkovich
 License: Apache 2.0
 Keywords: tools tool utils enum enums threadlocal UploadCommand upload uuid1mc uuid UUID UUID1 UUID4 UU1DMC issetdescriptor ismethod importer new_instance safe_eval is_empty parse_boolean Properties java.util.Properties
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `alex_ber_utils-0.8.1a2/alex_ber_utils.egg-info/SOURCES.txt` & `alex_ber_utils-0.8.1a3/alex_ber_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a2/alexber/utils/_ymlparsers_extra.py` & `alex_ber_utils-0.8.1a3/alexber/utils/_ymlparsers_extra.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a2/alexber/utils/deploys.py` & `alex_ber_utils-0.8.1a3/alexber/utils/deploys.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a2/alexber/utils/emails.py` & `alex_ber_utils-0.8.1a3/alexber/utils/emails.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a2/alexber/utils/enums.py` & `alex_ber_utils-0.8.1a3/alexber/utils/enums.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a2/alexber/utils/fabs.py` & `alex_ber_utils-0.8.1a3/alexber/utils/fabs.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a2/alexber/utils/files.py` & `alex_ber_utils-0.8.1a3/alexber/utils/files.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a2/alexber/utils/importer.py` & `alex_ber_utils-0.8.1a3/alexber/utils/importer.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a2/alexber/utils/init_app_conf.py` & `alex_ber_utils-0.8.1a3/alexber/utils/init_app_conf.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a2/alexber/utils/inspects.py` & `alex_ber_utils-0.8.1a3/alexber/utils/inspects.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a2/alexber/utils/mains.py` & `alex_ber_utils-0.8.1a3/alexber/utils/mains.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a2/alexber/utils/parsers.py` & `alex_ber_utils-0.8.1a3/alexber/utils/parsers.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a2/alexber/utils/pprint.py` & `alex_ber_utils-0.8.1a3/alexber/utils/pprint.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a2/alexber/utils/processinvokes.py` & `alex_ber_utils-0.8.1a3/alexber/utils/processinvokes.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a2/alexber/utils/props.py` & `alex_ber_utils-0.8.1a3/alexber/utils/props.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a2/alexber/utils/setups.py` & `alex_ber_utils-0.8.1a3/alexber/utils/setups.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a2/alexber/utils/stdlogging.py` & `alex_ber_utils-0.8.1a3/alexber/utils/stdlogging.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a2/alexber/utils/thread_locals.py` & `alex_ber_utils-0.8.1a3/alexber/utils/thread_locals.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a2/alexber/utils/uuids.py` & `alex_ber_utils-0.8.1a3/alexber/utils/uuids.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a2/alexber/utils/ymlparsers.py` & `alex_ber_utils-0.8.1a3/alexber/utils/ymlparsers.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a2/requirements-fabric.txt` & `alex_ber_utils-0.8.1a3/requirements-fabric.txt`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a2/requirements-piptools.txt` & `alex_ber_utils-0.8.1a3/requirements-piptools.txt`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a2/requirements-tests.txt` & `alex_ber_utils-0.8.1a3/requirements-tests.txt`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a2/setup.py` & `alex_ber_utils-0.8.1a3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 
 import setuptools
 from setuptools import setup
 
 
 #VERSION should be defined before importing UploadCommand
-VERSION = '0.8.1a2'
+VERSION = '0.8.1a3'
 from alexber.utils import UploadCommand
 NAME = 'alex_ber_utils'
 SHORT_NAME = 'utils'
 VCS_URL = 'https://github.com/alex-ber/AlexBerUtils'
 DESCRIPTION = 'AlexBerUtils is collection of the small utilities'
 AUTHOR = 'Alexander Berkovich'
```

### Comparing `alex_ber_utils-0.8.1a2/tests/conftest.py` & `alex_ber_utils-0.8.1a3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a2/tests/utils/deploys_test.py` & `alex_ber_utils-0.8.1a3/tests/utils/deploys_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a2/tests/utils/emails_test.py` & `alex_ber_utils-0.8.1a3/tests/utils/emails_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a2/tests/utils/enums_mixin_test.py` & `alex_ber_utils-0.8.1a3/tests/utils/enums_mixin_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a2/tests/utils/importer_test.py` & `alex_ber_utils-0.8.1a3/tests/utils/importer_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a2/tests/utils/init_app_conf_test.py` & `alex_ber_utils-0.8.1a3/tests/utils/init_app_conf_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a2/tests/utils/inspect_test.py` & `alex_ber_utils-0.8.1a3/tests/utils/inspect_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a2/tests/utils/mains_test.py` & `alex_ber_utils-0.8.1a3/tests/utils/mains_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a2/tests/utils/method_overloading_test.py` & `alex_ber_utils-0.8.1a3/tests/utils/method_overloading_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a2/tests/utils/parsers_test.py` & `alex_ber_utils-0.8.1a3/tests/utils/parsers_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a2/tests/utils/pprint_test.py` & `alex_ber_utils-0.8.1a3/tests/utils/pprint_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a2/tests/utils/processinvokes_test.py` & `alex_ber_utils-0.8.1a3/tests/utils/processinvokes_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a2/tests/utils/properties_test.py` & `alex_ber_utils-0.8.1a3/tests/utils/properties_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a2/tests/utils/threadlocal_test.py` & `alex_ber_utils-0.8.1a3/tests/utils/threadlocal_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a2/tests/utils/uuids_test.py` & `alex_ber_utils-0.8.1a3/tests/utils/uuids_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a2/tests/utils/ymlparsers_extra_test.py` & `alex_ber_utils-0.8.1a3/tests/utils/ymlparsers_extra_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a2/tests/utils/ymlparsers_test.py` & `alex_ber_utils-0.8.1a3/tests/utils/ymlparsers_test.py`

 * *Files identical despite different names*

