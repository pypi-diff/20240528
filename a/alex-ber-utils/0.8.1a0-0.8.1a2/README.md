# Comparing `tmp/alex_ber_utils-0.8.1a0.tar.gz` & `tmp/alex_ber_utils-0.8.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alex_ber_utils-0.8.1a0.tar", last modified: Wed Dec 13 10:24:05 2023, max compression
+gzip compressed data, was "alex_ber_utils-0.8.1a2.tar", last modified: Tue May 28 10:00:11 2024, max compression
```

## Comparing `alex_ber_utils-0.8.1a0.tar` & `alex_ber_utils-0.8.1a2.tar`

### file list

```diff
@@ -1,95 +1,99 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-13 10:24:05.616298 alex_ber_utils-0.8.1a0/
--rwxrwxrwx   0 root         (0) root         (0)    26556 2023-12-04 08:43:28.000000 alex_ber_utils-0.8.1a0/CHANGELOG.md
--rwxrwxrwx   0 root         (0) root         (0)     1295 2022-08-28 13:06:40.000000 alex_ber_utils-0.8.1a0/LICENSE.txt
--rwxrwxrwx   0 root         (0) root         (0)      195 2022-08-28 13:06:40.000000 alex_ber_utils-0.8.1a0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    32613 2023-12-13 10:24:05.616298 alex_ber_utils-0.8.1a0/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     3748 2023-12-03 14:57:11.000000 alex_ber_utils-0.8.1a0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-13 10:24:05.612297 alex_ber_utils-0.8.1a0/alex_ber_utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)    32613 2023-12-13 10:24:05.000000 alex_ber_utils-0.8.1a0/alex_ber_utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2145 2023-12-13 10:24:05.000000 alex_ber_utils-0.8.1a0/alex_ber_utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-13 10:24:05.000000 alex_ber_utils-0.8.1a0/alex_ber_utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-12-13 10:24:05.000000 alex_ber_utils-0.8.1a0/alex_ber_utils.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-13 10:24:05.000000 alex_ber_utils-0.8.1a0/alex_ber_utils.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      427 2023-12-13 10:24:05.000000 alex_ber_utils-0.8.1a0/alex_ber_utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-12-13 10:24:05.000000 alex_ber_utils-0.8.1a0/alex_ber_utils.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-13 10:24:05.592297 alex_ber_utils-0.8.1a0/alexber/
--rw-rw-r--   0 root         (0) root         (0)       55 2023-12-03 15:34:29.000000 alex_ber_utils-0.8.1a0/alexber/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-13 10:24:05.600297 alex_ber_utils-0.8.1a0/alexber/utils/
--rw-rw-r--   0 root         (0) root         (0)      250 2022-08-28 13:06:40.000000 alex_ber_utils-0.8.1a0/alexber/utils/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8188 2022-08-28 13:06:40.000000 alex_ber_utils-0.8.1a0/alexber/utils/_ymlparsers_extra.py
--rw-rw-r--   0 root         (0) root         (0)     3928 2022-08-28 13:06:40.000000 alex_ber_utils-0.8.1a0/alexber/utils/deploys.py
--rw-rw-r--   0 root         (0) root         (0)    17354 2022-08-28 13:06:40.000000 alex_ber_utils-0.8.1a0/alexber/utils/emails.py
--rw-rw-r--   0 root         (0) root         (0)     1425 2022-08-28 13:06:40.000000 alex_ber_utils-0.8.1a0/alexber/utils/enums.py
--rw-rw-r--   0 root         (0) root         (0)     1512 2022-08-28 13:06:40.000000 alex_ber_utils-0.8.1a0/alexber/utils/fabs.py
--rw-rw-r--   0 root         (0) root         (0)      857 2022-08-28 13:06:40.000000 alex_ber_utils-0.8.1a0/alexber/utils/files.py
--rw-rw-r--   0 root         (0) root         (0)     3300 2022-08-28 13:06:40.000000 alex_ber_utils-0.8.1a0/alexber/utils/importer.py
--rw-rw-r--   0 root         (0) root         (0)    19314 2022-08-28 13:06:40.000000 alex_ber_utils-0.8.1a0/alexber/utils/init_app_conf.py
--rw-rw-r--   0 root         (0) root         (0)     1385 2022-08-28 13:06:40.000000 alex_ber_utils-0.8.1a0/alexber/utils/inspects.py
--rw-rw-r--   0 root         (0) root         (0)    11144 2022-08-28 13:06:40.000000 alex_ber_utils-0.8.1a0/alexber/utils/mains.py
--rw-rw-r--   0 root         (0) root         (0)     4210 2022-08-28 13:06:40.000000 alex_ber_utils-0.8.1a0/alexber/utils/parsers.py
--rw-rw-r--   0 root         (0) root         (0)    10390 2022-08-28 13:06:40.000000 alex_ber_utils-0.8.1a0/alexber/utils/processinvokes.py
--rw-rw-r--   0 root         (0) root         (0)    16921 2023-08-07 07:45:37.000000 alex_ber_utils-0.8.1a0/alexber/utils/props.py
--rw-rw-r--   0 root         (0) root         (0)     2345 2023-12-13 10:08:38.000000 alex_ber_utils-0.8.1a0/alexber/utils/setups.py
--rw-rw-r--   0 root         (0) root         (0)     3204 2022-08-28 13:06:40.000000 alex_ber_utils-0.8.1a0/alexber/utils/stdlogging.py
--rw-rw-r--   0 root         (0) root         (0)      658 2022-08-28 13:06:40.000000 alex_ber_utils-0.8.1a0/alexber/utils/thread_locals.py
--rw-rw-r--   0 root         (0) root         (0)     1745 2022-08-28 13:06:40.000000 alex_ber_utils-0.8.1a0/alexber/utils/uuids.py
--rw-rw-r--   0 root         (0) root         (0)    11517 2022-08-28 13:06:40.000000 alex_ber_utils-0.8.1a0/alexber/utils/ymlparsers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-13 10:24:05.600297 alex_ber_utils-0.8.1a0/data/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-08-28 13:06:40.000000 alex_ber_utils-0.8.1a0/data/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       21 2023-12-03 16:39:05.000000 alex_ber_utils-0.8.1a0/req-env.txt
--rwxrwxrwx   0 root         (0) root         (0)       56 2023-12-03 18:59:03.000000 alex_ber_utils-0.8.1a0/req-fabric.txt
--rwxrwxrwx   0 root         (0) root         (0)       18 2022-08-28 13:06:40.000000 alex_ber_utils-0.8.1a0/req-md.txt
--rwxrwxrwx   0 root         (0) root         (0)       17 2023-12-03 16:27:06.000000 alex_ber_utils-0.8.1a0/req-piptools.txt
--rwxrwxrwx   0 root         (0) root         (0)       92 2023-12-03 14:26:09.000000 alex_ber_utils-0.8.1a0/req-tests.txt
--rwxrwxrwx   0 root         (0) root         (0)       32 2023-12-03 15:30:39.000000 alex_ber_utils-0.8.1a0/req-yml.txt
--rwxrwxrwx   0 root         (0) root         (0)       13 2023-12-03 13:28:22.000000 alex_ber_utils-0.8.1a0/req.txt
--rwxrwxrwx   0 root         (0) root         (0)       20 2023-12-03 12:25:56.000000 alex_ber_utils-0.8.1a0/requirements-env.txt
--rwxrwxrwx   0 root         (0) root         (0)      635 2023-12-03 18:56:31.000000 alex_ber_utils-0.8.1a0/requirements-fabric.txt
--rwxrwxrwx   0 root         (0) root         (0)       18 2023-08-03 21:18:06.000000 alex_ber_utils-0.8.1a0/requirements-md.txt
--rwxrwxrwx   0 root         (0) root         (0)      329 2023-12-03 12:57:25.000000 alex_ber_utils-0.8.1a0/requirements-piptools.txt
--rwxrwxrwx   0 root         (0) root         (0)      603 2023-12-03 13:07:38.000000 alex_ber_utils-0.8.1a0/requirements-tests.txt
--rwxrwxrwx   0 root         (0) root         (0)      395 2023-12-03 13:12:03.000000 alex_ber_utils-0.8.1a0/requirements-yml.txt
--rwxrwxr-x   0 root         (0) root         (0)       13 2023-12-13 10:13:58.000000 alex_ber_utils-0.8.1a0/requirements.txt
--rwxrwxrwx   0 root         (0) root         (0)      190 2023-12-13 10:24:05.616298 alex_ber_utils-0.8.1a0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     4217 2023-12-13 10:12:36.000000 alex_ber_utils-0.8.1a0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-13 10:24:05.600297 alex_ber_utils-0.8.1a0/tests/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-08-28 13:06:40.000000 alex_ber_utils-0.8.1a0/tests/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1931 2022-08-28 13:06:40.000000 alex_ber_utils-0.8.1a0/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-13 10:24:05.608297 alex_ber_utils-0.8.1a0/tests/utils/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-08-28 13:06:40.000000 alex_ber_utils-0.8.1a0/tests/utils/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6071 2022-08-28 13:06:40.000000 alex_ber_utils-0.8.1a0/tests/utils/deploys_test.py
--rw-rw-r--   0 root         (0) root         (0)     8680 2022-08-28 13:06:40.000000 alex_ber_utils-0.8.1a0/tests/utils/emails_test.py
--rw-rw-r--   0 root         (0) root         (0)    10227 2022-08-28 13:06:40.000000 alex_ber_utils-0.8.1a0/tests/utils/enums_mixin_test.py
--rw-rw-r--   0 root         (0) root         (0)     5067 2022-08-28 13:06:40.000000 alex_ber_utils-0.8.1a0/tests/utils/importer_test.py
--rw-rw-r--   0 root         (0) root         (0)    30475 2022-08-28 13:06:40.000000 alex_ber_utils-0.8.1a0/tests/utils/init_app_conf_test.py
--rw-rw-r--   0 root         (0) root         (0)     3654 2022-08-28 13:06:40.000000 alex_ber_utils-0.8.1a0/tests/utils/inspect_test.py
--rw-rw-r--   0 root         (0) root         (0)     1328 2022-08-28 13:06:40.000000 alex_ber_utils-0.8.1a0/tests/utils/mains_test.py
--rw-rw-r--   0 root         (0) root         (0)     2444 2022-08-28 13:06:40.000000 alex_ber_utils-0.8.1a0/tests/utils/method_overloading_test.py
--rw-rw-r--   0 root         (0) root         (0)     5106 2022-08-28 13:06:40.000000 alex_ber_utils-0.8.1a0/tests/utils/parsers_test.py
--rw-rw-r--   0 root         (0) root         (0)     5372 2022-08-28 13:06:40.000000 alex_ber_utils-0.8.1a0/tests/utils/processinvokes_test.py
--rw-rw-r--   0 root         (0) root         (0)     2047 2023-08-10 14:42:44.000000 alex_ber_utils-0.8.1a0/tests/utils/properties_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-13 10:24:05.608297 alex_ber_utils-0.8.1a0/tests/utils/splitpackage/
--rw-rw-r--   0 root         (0) root         (0)      116 2022-08-28 13:06:40.000000 alex_ber_utils-0.8.1a0/tests/utils/splitpackage/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        0 2022-08-28 13:06:40.000000 alex_ber_utils-0.8.1a0/tests/utils/splitpackage/mymodule.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-13 10:24:05.608297 alex_ber_utils-0.8.1a0/tests/utils/splitpackage_cont/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-08-28 13:06:40.000000 alex_ber_utils-0.8.1a0/tests/utils/splitpackage_cont/__init__.py
--rw-rw-r--   0 root         (0) root         (0)       34 2022-08-28 13:06:40.000000 alex_ber_utils-0.8.1a0/tests/utils/splitpackage_cont/other_module.py
--rw-rw-r--   0 root         (0) root         (0)     3914 2022-08-28 13:06:40.000000 alex_ber_utils-0.8.1a0/tests/utils/threadlocal_test.py
--rw-rw-r--   0 root         (0) root         (0)     1064 2022-08-28 13:06:40.000000 alex_ber_utils-0.8.1a0/tests/utils/uuids_test.py
--rw-rw-r--   0 root         (0) root         (0)    14847 2022-08-28 13:06:40.000000 alex_ber_utils-0.8.1a0/tests/utils/ymlparsers_extra_test.py
--rw-rw-r--   0 root         (0) root         (0)    27324 2022-08-28 13:06:40.000000 alex_ber_utils-0.8.1a0/tests/utils/ymlparsers_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-13 10:24:05.608297 alex_ber_utils-0.8.1a0/tests_data/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-08-28 13:06:40.000000 alex_ber_utils-0.8.1a0/tests_data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-13 10:24:05.608297 alex_ber_utils-0.8.1a0/tests_data/tests/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-08-28 13:06:40.000000 alex_ber_utils-0.8.1a0/tests_data/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-13 10:24:05.608297 alex_ber_utils-0.8.1a0/tests_data/tests/utils/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-08-28 13:06:40.000000 alex_ber_utils-0.8.1a0/tests_data/tests/utils/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      135 2022-08-28 13:06:40.000000 alex_ber_utils-0.8.1a0/tests_data/tests/utils/config.properties
--rw-rw-r--   0 root         (0) root         (0)       81 2022-08-28 13:06:40.000000 alex_ber_utils-0.8.1a0/tests_data/tests/utils/config2.properties
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-13 10:24:05.608297 alex_ber_utils-0.8.1a0/tests_data/tests/utils/initappconf/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-08-28 13:06:40.000000 alex_ber_utils-0.8.1a0/tests_data/tests/utils/initappconf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-13 10:24:05.612297 alex_ber_utils-0.8.1a0/tests_data/tests/utils/parser/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-08-28 13:06:40.000000 alex_ber_utils-0.8.1a0/tests_data/tests/utils/parser/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      187 2022-08-28 13:06:40.000000 alex_ber_utils-0.8.1a0/tests_data/tests/utils/parser/config.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-13 10:24:05.612297 alex_ber_utils-0.8.1a0/tests_data/tests/utils/ymlparsers/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-08-28 13:06:40.000000 alex_ber_utils-0.8.1a0/tests_data/tests/utils/ymlparsers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:00:11.089646 alex_ber_utils-0.8.1a2/
+-rwxrwxrwx   0 root         (0) root         (0)    26584 2024-05-28 09:24:26.000000 alex_ber_utils-0.8.1a2/CHANGELOG.md
+-rwxrwxrwx   0 root         (0) root         (0)     1295 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/LICENSE.txt
+-rwxrwxrwx   0 root         (0) root         (0)      195 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    31537 2024-05-28 10:00:11.090646 alex_ber_utils-0.8.1a2/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     3748 2024-01-28 16:28:53.000000 alex_ber_utils-0.8.1a2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:00:10.128175 alex_ber_utils-0.8.1a2/alex_ber_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    31537 2024-05-28 10:00:08.000000 alex_ber_utils-0.8.1a2/alex_ber_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2227 2024-05-28 10:00:09.000000 alex_ber_utils-0.8.1a2/alex_ber_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 10:00:08.000000 alex_ber_utils-0.8.1a2/alex_ber_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-28 10:00:08.000000 alex_ber_utils-0.8.1a2/alex_ber_utils.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 09:52:52.000000 alex_ber_utils-0.8.1a2/alex_ber_utils.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      427 2024-05-28 10:00:08.000000 alex_ber_utils-0.8.1a2/alex_ber_utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2024-05-28 10:00:08.000000 alex_ber_utils-0.8.1a2/alex_ber_utils.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:00:10.144635 alex_ber_utils-0.8.1a2/alexber/
+-rwxrwxrwx   0 root         (0) root         (0)       55 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/alexber/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:00:10.492171 alex_ber_utils-0.8.1a2/alexber/utils/
+-rwxrwxrwx   0 root         (0) root         (0)      250 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/alexber/utils/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     8188 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/alexber/utils/_ymlparsers_extra.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:00:10.512892 alex_ber_utils-0.8.1a2/alexber/utils/data/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/alexber/utils/data/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3928 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/alexber/utils/deploys.py
+-rwxrwxrwx   0 root         (0) root         (0)    17354 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/alexber/utils/emails.py
+-rwxrwxrwx   0 root         (0) root         (0)     1425 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/alexber/utils/enums.py
+-rwxrwxrwx   0 root         (0) root         (0)     1512 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/alexber/utils/fabs.py
+-rwxrwxrwx   0 root         (0) root         (0)      857 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/alexber/utils/files.py
+-rwxrwxrwx   0 root         (0) root         (0)     3300 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/alexber/utils/importer.py
+-rwxrwxrwx   0 root         (0) root         (0)    19314 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/alexber/utils/init_app_conf.py
+-rwxrwxrwx   0 root         (0) root         (0)     1385 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/alexber/utils/inspects.py
+-rwxrwxrwx   0 root         (0) root         (0)    11144 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/alexber/utils/mains.py
+-rwxrwxrwx   0 root         (0) root         (0)     4210 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/alexber/utils/parsers.py
+-rwxrwxrwx   0 root         (0) root         (0)     1316 2024-05-28 09:20:53.000000 alex_ber_utils-0.8.1a2/alexber/utils/pprint.py
+-rwxrwxrwx   0 root         (0) root         (0)    10390 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/alexber/utils/processinvokes.py
+-rwxrwxrwx   0 root         (0) root         (0)    16921 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/alexber/utils/props.py
+-rwxrwxrwx   0 root         (0) root         (0)     2296 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/alexber/utils/setups.py
+-rwxrwxrwx   0 root         (0) root         (0)     3204 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/alexber/utils/stdlogging.py
+-rwxrwxrwx   0 root         (0) root         (0)      658 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/alexber/utils/thread_locals.py
+-rwxrwxrwx   0 root         (0) root         (0)     1745 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/alexber/utils/uuids.py
+-rwxrwxrwx   0 root         (0) root         (0)    11517 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/alexber/utils/ymlparsers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:00:10.526102 alex_ber_utils-0.8.1a2/data/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/data/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       21 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/req-env.txt
+-rwxrwxrwx   0 root         (0) root         (0)       56 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/req-fabric.txt
+-rwxrwxrwx   0 root         (0) root         (0)       18 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/req-md.txt
+-rwxrwxrwx   0 root         (0) root         (0)       17 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/req-piptools.txt
+-rwxrwxrwx   0 root         (0) root         (0)       92 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/req-tests.txt
+-rwxrwxrwx   0 root         (0) root         (0)       32 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/req-yml.txt
+-rwxrwxrwx   0 root         (0) root         (0)       13 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/req.txt
+-rwxrwxrwx   0 root         (0) root         (0)       20 2024-05-28 08:02:25.000000 alex_ber_utils-0.8.1a2/requirements-env.txt
+-rwxrwxrwx   0 root         (0) root         (0)      636 2024-05-28 08:29:11.000000 alex_ber_utils-0.8.1a2/requirements-fabric.txt
+-rwxrwxrwx   0 root         (0) root         (0)      184 2024-05-28 08:29:34.000000 alex_ber_utils-0.8.1a2/requirements-md.txt
+-rwxrwxrwx   0 root         (0) root         (0)      523 2024-05-28 08:30:05.000000 alex_ber_utils-0.8.1a2/requirements-piptools.txt
+-rwxrwxrwx   0 root         (0) root         (0)      605 2024-05-28 08:30:34.000000 alex_ber_utils-0.8.1a2/requirements-tests.txt
+-rwxrwxrwx   0 root         (0) root         (0)      369 2024-05-28 08:33:31.000000 alex_ber_utils-0.8.1a2/requirements-yml.txt
+-rwxrwxrwx   0 root         (0) root         (0)      171 2024-05-28 08:33:31.000000 alex_ber_utils-0.8.1a2/requirements.txt
+-rwxrwxrwx   0 root         (0) root         (0)      190 2024-05-28 10:00:11.095645 alex_ber_utils-0.8.1a2/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     4905 2024-05-28 09:59:57.000000 alex_ber_utils-0.8.1a2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:00:10.548371 alex_ber_utils-0.8.1a2/tests/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1931 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:00:10.827083 alex_ber_utils-0.8.1a2/tests/utils/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests/utils/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     6071 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests/utils/deploys_test.py
+-rwxrwxrwx   0 root         (0) root         (0)     8680 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests/utils/emails_test.py
+-rwxrwxrwx   0 root         (0) root         (0)    10227 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests/utils/enums_mixin_test.py
+-rwxrwxrwx   0 root         (0) root         (0)     5067 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests/utils/importer_test.py
+-rwxrwxrwx   0 root         (0) root         (0)    30475 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests/utils/init_app_conf_test.py
+-rwxrwxrwx   0 root         (0) root         (0)     3654 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests/utils/inspect_test.py
+-rwxrwxrwx   0 root         (0) root         (0)     1328 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests/utils/mains_test.py
+-rwxrwxrwx   0 root         (0) root         (0)     2444 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests/utils/method_overloading_test.py
+-rwxrwxrwx   0 root         (0) root         (0)     5106 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests/utils/parsers_test.py
+-rwxrwxrwx   0 root         (0) root         (0)     2157 2024-05-28 09:22:01.000000 alex_ber_utils-0.8.1a2/tests/utils/pprint_test.py
+-rwxrwxrwx   0 root         (0) root         (0)     5372 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests/utils/processinvokes_test.py
+-rwxrwxrwx   0 root         (0) root         (0)     2047 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests/utils/properties_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:00:10.864784 alex_ber_utils-0.8.1a2/tests/utils/splitpackage/
+-rwxrwxrwx   0 root         (0) root         (0)      116 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests/utils/splitpackage/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests/utils/splitpackage/mymodule.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:00:10.899850 alex_ber_utils-0.8.1a2/tests/utils/splitpackage_cont/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests/utils/splitpackage_cont/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       34 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests/utils/splitpackage_cont/other_module.py
+-rwxrwxrwx   0 root         (0) root         (0)     3914 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests/utils/threadlocal_test.py
+-rwxrwxrwx   0 root         (0) root         (0)     1064 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests/utils/uuids_test.py
+-rwxrwxrwx   0 root         (0) root         (0)    14847 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests/utils/ymlparsers_extra_test.py
+-rwxrwxrwx   0 root         (0) root         (0)    27324 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests/utils/ymlparsers_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:00:10.914970 alex_ber_utils-0.8.1a2/tests_data/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests_data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:00:10.928026 alex_ber_utils-0.8.1a2/tests_data/tests/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests_data/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:00:10.991455 alex_ber_utils-0.8.1a2/tests_data/tests/utils/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests_data/tests/utils/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      135 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests_data/tests/utils/config.properties
+-rwxrwxrwx   0 root         (0) root         (0)       81 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests_data/tests/utils/config2.properties
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:00:11.011943 alex_ber_utils-0.8.1a2/tests_data/tests/utils/initappconf/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests_data/tests/utils/initappconf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:00:11.053488 alex_ber_utils-0.8.1a2/tests_data/tests/utils/parser/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests_data/tests/utils/parser/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      187 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests_data/tests/utils/parser/config.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:00:11.075644 alex_ber_utils-0.8.1a2/tests_data/tests/utils/ymlparsers/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a2/tests_data/tests/utils/ymlparsers/__init__.py
```

### Comparing `alex_ber_utils-0.8.1a0/CHANGELOG.md` & `alex_ber_utils-0.8.1a2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 \#https://pypi.org/manage/project/alex-ber-utils/releases/
 
 ## Unreleased
 
+## [0.8.1a] 04.12.2023
+
+
 ## [0.8.0] 04.12.2023
 
 ### Changed
 - In setup.cfg flag mock_use_standalone_module
 was changed to false (to use unittest.mock).
 - Many version of the packages in extra was updated to latest:
 - python-dotenv from 0.15.0 to 1.0.0.
```

### Comparing `alex_ber_utils-0.8.1a0/LICENSE.txt` & `alex_ber_utils-0.8.1a2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a0/PKG-INFO` & `alex_ber_utils-0.8.1a2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alex_ber_utils
-Version: 0.8.1a0
+Version: 0.8.1a2
 Summary: AlexBerUtils is collection of the small utilities
 Home-page: https://github.com/alex-ber/AlexBerUtils
 Author: Alexander Berkovich
 License: Apache 2.0
 Keywords: tools tool utils enum enums threadlocal UploadCommand upload uuid1mc uuid UUID UUID1 UUID4 UU1DMC issetdescriptor ismethod importer new_instance safe_eval is_empty parse_boolean Properties java.util.Properties
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -27,45 +27,22 @@
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Natural Language :: English
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Requires-Dist: pyyaml==6.0.1
 Provides-Extra: md
-Requires-Dist: multidispatch>=0.2; extra == "md"
 Provides-Extra: fabric
-Requires-Dist: fabric>=2.5.0; extra == "fabric"
-Requires-Dist: pyOpenSSL>=23.3.0; extra == "fabric"
-Requires-Dist: cryptography>=41.0.7; extra == "fabric"
 Provides-Extra: yaml
-Requires-Dist: PyYAML; extra == "yaml"
-Requires-Dist: HiYaPyCo>=0.4.16; extra == "yaml"
-Requires-Dist: Jinja2>1; extra == "yaml"
 Provides-Extra: yml
-Requires-Dist: PyYAML; extra == "yml"
-Requires-Dist: HiYaPyCo>=0.4.16; extra == "yml"
-Requires-Dist: Jinja2>1; extra == "yml"
 Provides-Extra: env
-Requires-Dist: python-dotenv>=1.0.0; extra == "env"
 Provides-Extra: tests
-Requires-Dist: exceptiongroup==1.2.0; extra == "tests"
-Requires-Dist: iniconfig==2.0.0; extra == "tests"
-Requires-Dist: packaging==23.2; extra == "tests"
-Requires-Dist: pluggy==1.3.0; extra == "tests"
-Requires-Dist: pytest==7.4.3; extra == "tests"
-Requires-Dist: pytest-assume==2.3.3; extra == "tests"
-Requires-Dist: pytest-asyncio==0.21.1; extra == "tests"
-Requires-Dist: pytest-mock==3.12.0; extra == "tests"
-Requires-Dist: pyyaml==6.0.1; extra == "tests"
-Requires-Dist: tomli==2.0.1; extra == "tests"
 Provides-Extra: piptools
-Requires-Dist: python-dotenv>=1.0.0; extra == "piptools"
+License-File: LICENSE.txt
 
 ## AlexBerUtils
 
 AlexBerUtils is collection of the small utilities. See CHANGELOG.md for detail description.
 
 
 
@@ -220,14 +197,17 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 \#https://pypi.org/manage/project/alex-ber-utils/releases/
 
 ## Unreleased
 
+## [0.8.1a] 04.12.2023
+
+
 ## [0.8.0] 04.12.2023
 
 ### Changed
 - In setup.cfg flag mock_use_standalone_module
 was changed to false (to use unittest.mock).
 - Many version of the packages in extra was updated to latest:
 - python-dotenv from 0.15.0 to 1.0.0.
```

### Comparing `alex_ber_utils-0.8.1a0/README.md` & `alex_ber_utils-0.8.1a2/README.md`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a0/alex_ber_utils.egg-info/PKG-INFO` & `alex_ber_utils-0.8.1a2/alex_ber_utils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alex-ber-utils
-Version: 0.8.1a0
+Version: 0.8.1a2
 Summary: AlexBerUtils is collection of the small utilities
 Home-page: https://github.com/alex-ber/AlexBerUtils
 Author: Alexander Berkovich
 License: Apache 2.0
 Keywords: tools tool utils enum enums threadlocal UploadCommand upload uuid1mc uuid UUID UUID1 UUID4 UU1DMC issetdescriptor ismethod importer new_instance safe_eval is_empty parse_boolean Properties java.util.Properties
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -27,45 +27,22 @@
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Natural Language :: English
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Requires-Dist: pyyaml==6.0.1
 Provides-Extra: md
-Requires-Dist: multidispatch>=0.2; extra == "md"
 Provides-Extra: fabric
-Requires-Dist: fabric>=2.5.0; extra == "fabric"
-Requires-Dist: pyOpenSSL>=23.3.0; extra == "fabric"
-Requires-Dist: cryptography>=41.0.7; extra == "fabric"
 Provides-Extra: yaml
-Requires-Dist: PyYAML; extra == "yaml"
-Requires-Dist: HiYaPyCo>=0.4.16; extra == "yaml"
-Requires-Dist: Jinja2>1; extra == "yaml"
 Provides-Extra: yml
-Requires-Dist: PyYAML; extra == "yml"
-Requires-Dist: HiYaPyCo>=0.4.16; extra == "yml"
-Requires-Dist: Jinja2>1; extra == "yml"
 Provides-Extra: env
-Requires-Dist: python-dotenv>=1.0.0; extra == "env"
 Provides-Extra: tests
-Requires-Dist: exceptiongroup==1.2.0; extra == "tests"
-Requires-Dist: iniconfig==2.0.0; extra == "tests"
-Requires-Dist: packaging==23.2; extra == "tests"
-Requires-Dist: pluggy==1.3.0; extra == "tests"
-Requires-Dist: pytest==7.4.3; extra == "tests"
-Requires-Dist: pytest-assume==2.3.3; extra == "tests"
-Requires-Dist: pytest-asyncio==0.21.1; extra == "tests"
-Requires-Dist: pytest-mock==3.12.0; extra == "tests"
-Requires-Dist: pyyaml==6.0.1; extra == "tests"
-Requires-Dist: tomli==2.0.1; extra == "tests"
 Provides-Extra: piptools
-Requires-Dist: python-dotenv>=1.0.0; extra == "piptools"
+License-File: LICENSE.txt
 
 ## AlexBerUtils
 
 AlexBerUtils is collection of the small utilities. See CHANGELOG.md for detail description.
 
 
 
@@ -220,14 +197,17 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 \#https://pypi.org/manage/project/alex-ber-utils/releases/
 
 ## Unreleased
 
+## [0.8.1a] 04.12.2023
+
+
 ## [0.8.0] 04.12.2023
 
 ### Changed
 - In setup.cfg flag mock_use_standalone_module
 was changed to false (to use unittest.mock).
 - Many version of the packages in extra was updated to latest:
 - python-dotenv from 0.15.0 to 1.0.0.
```

### Comparing `alex_ber_utils-0.8.1a0/alex_ber_utils.egg-info/SOURCES.txt` & `alex_ber_utils-0.8.1a2/alex_ber_utils.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -34,34 +34,37 @@
 alexber/utils/fabs.py
 alexber/utils/files.py
 alexber/utils/importer.py
 alexber/utils/init_app_conf.py
 alexber/utils/inspects.py
 alexber/utils/mains.py
 alexber/utils/parsers.py
+alexber/utils/pprint.py
 alexber/utils/processinvokes.py
 alexber/utils/props.py
 alexber/utils/setups.py
 alexber/utils/stdlogging.py
 alexber/utils/thread_locals.py
 alexber/utils/uuids.py
 alexber/utils/ymlparsers.py
+alexber/utils/data/__init__.py
 data/__init__.py
 tests/__init__.py
 tests/conftest.py
 tests/utils/__init__.py
 tests/utils/deploys_test.py
 tests/utils/emails_test.py
 tests/utils/enums_mixin_test.py
 tests/utils/importer_test.py
 tests/utils/init_app_conf_test.py
 tests/utils/inspect_test.py
 tests/utils/mains_test.py
 tests/utils/method_overloading_test.py
 tests/utils/parsers_test.py
+tests/utils/pprint_test.py
 tests/utils/processinvokes_test.py
 tests/utils/properties_test.py
 tests/utils/threadlocal_test.py
 tests/utils/uuids_test.py
 tests/utils/ymlparsers_extra_test.py
 tests/utils/ymlparsers_test.py
 tests/utils/splitpackage/__init__.py
```

### Comparing `alex_ber_utils-0.8.1a0/alexber/utils/_ymlparsers_extra.py` & `alex_ber_utils-0.8.1a2/alexber/utils/_ymlparsers_extra.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a0/alexber/utils/deploys.py` & `alex_ber_utils-0.8.1a2/alexber/utils/deploys.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a0/alexber/utils/emails.py` & `alex_ber_utils-0.8.1a2/alexber/utils/emails.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a0/alexber/utils/enums.py` & `alex_ber_utils-0.8.1a2/alexber/utils/enums.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a0/alexber/utils/fabs.py` & `alex_ber_utils-0.8.1a2/alexber/utils/fabs.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a0/alexber/utils/files.py` & `alex_ber_utils-0.8.1a2/alexber/utils/files.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a0/alexber/utils/importer.py` & `alex_ber_utils-0.8.1a2/alexber/utils/importer.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a0/alexber/utils/init_app_conf.py` & `alex_ber_utils-0.8.1a2/alexber/utils/init_app_conf.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a0/alexber/utils/inspects.py` & `alex_ber_utils-0.8.1a2/alexber/utils/inspects.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a0/alexber/utils/mains.py` & `alex_ber_utils-0.8.1a2/alexber/utils/mains.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a0/alexber/utils/parsers.py` & `alex_ber_utils-0.8.1a2/alexber/utils/parsers.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a0/alexber/utils/processinvokes.py` & `alex_ber_utils-0.8.1a2/alexber/utils/processinvokes.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a0/alexber/utils/props.py` & `alex_ber_utils-0.8.1a2/alexber/utils/props.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a0/alexber/utils/setups.py` & `alex_ber_utils-0.8.1a2/alexber/utils/setups.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,16 +46,15 @@
         self.status('Removing previous builds...')
         # rm -rf build *.egg-info dist
         _my_rmtree(os.path.join(_setup_dir, 'build'))
         _my_rmtree(os.path.join(_setup_dir, 'f{NAME}.egg-info'))
         _my_rmtree(os.path.join(_setup_dir, 'dist'))
 
         self.status('Building Source and Wheel distribution...')
-        os.system(f'{sys.executable} -m build')
-        #os.system(f'{sys.executable} setup.py sdist bdist_wheel')
+        os.system(f'{sys.executable} setup.py sdist bdist_wheel')
         #os.system('python3 setup.py sdist bdist_wheel')
 
         self.status('Uploading the package to PyPI via Twine...')
         # python3 -m keyring set https://upload.pypi.org/legacy/ alex-ber
         os.system('twine upload dist/*')
 
         self.status('Pushing git tags...')
```

### Comparing `alex_ber_utils-0.8.1a0/alexber/utils/stdlogging.py` & `alex_ber_utils-0.8.1a2/alexber/utils/stdlogging.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a0/alexber/utils/thread_locals.py` & `alex_ber_utils-0.8.1a2/alexber/utils/thread_locals.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a0/alexber/utils/uuids.py` & `alex_ber_utils-0.8.1a2/alexber/utils/uuids.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a0/alexber/utils/ymlparsers.py` & `alex_ber_utils-0.8.1a2/alexber/utils/ymlparsers.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a0/requirements-tests.txt` & `alex_ber_utils-0.8.1a2/requirements-tests.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    pip-compile requirements.in
 #
-exceptiongroup==1.2.0
+exceptiongroup==1.2.1
     # via pytest
 iniconfig==2.0.0
     # via pytest
-packaging==23.2
+packaging==24.0
     # via pytest
-pluggy==1.3.0
+pluggy==1.5.0
     # via pytest
 pytest==7.4.3
     # via
     #   -r requirements.in
     #   pytest-assume
     #   pytest-asyncio
     #   pytest-mock
@@ -23,8 +23,8 @@
 pytest-asyncio==0.21.1
     # via -r requirements.in
 pytest-mock==3.12.0
     # via -r requirements.in
 pyyaml==6.0.1
     # via -r requirements.in
 tomli==2.0.1
-    # via pytest
+    # via pytest
```

### Comparing `alex_ber_utils-0.8.1a0/setup.py` & `alex_ber_utils-0.8.1a2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,112 +1,128 @@
-import os
-
-import setuptools
-from setuptools import setup
-
-
-#VERSION should be defined before importing UploadCommand
-VERSION = '0.8.1a0'
-from alexber.utils import UploadCommand
-NAME = 'alex_ber_utils'
-SHORT_NAME = 'utils'
-VCS_URL = 'https://github.com/alex-ber/AlexBerUtils'
-DESCRIPTION = 'AlexBerUtils is collection of the small utilities'
-AUTHOR = 'Alexander Berkovich'
-
-
-base_dir = os.path.dirname(os.path.realpath(__file__))
-
-def get_content(filename):
-    with open(os.path.join(base_dir, filename)) as f:
-        content = f.read().splitlines()
-    return content
-
-install_requires = get_content('requirements.txt')
-tests_require = get_content('requirements-tests.txt')
-
-extras = {
-    'md': get_content('req-md.txt'),
-    'fabric' : get_content('req-fabric.txt'),
-    'yaml' : get_content('req-yml.txt'),
-    'yml' : get_content('req-yml.txt'),
-    'env' : get_content('req-env.txt'),
-    'tests': tests_require,
-    'piptools' : get_content('req-env.txt')
-}
-
-
-setup(
-    name=NAME,
-    version=VERSION,
-    url=VCS_URL,
-    author=AUTHOR,
-    description=DESCRIPTION,
-    long_description="\n\n".join([
-        open(os.path.join(base_dir, "README.md"), "r").read(),
-        open(os.path.join(base_dir, "CHANGELOG.md"), "r").read()
-    ]),
-    long_description_content_type="text/markdown",
-    packages=setuptools.find_packages(exclude=('tests', 'tests.*', 'data')),
-    # see https://stackoverflow.com/a/26533921
-    # see also https://stackoverflow.com/questions/24347450/how-do-you-add-additional-files-to-a-wheel
-    # data_files=[(f'Lib/site-packages/alexber/{SHORT_NAME}', ['data/config.yml', 'data/requirements-src.txt',
-    #                                                    'data/driver.py']),
-    #             #(f'lib/python3.7/site-packages/alexber/{SHORT_NAME}', ['requirements-src.txt'])
-    #             ],
-    # package_data={'alexber.{SHORT_NAME}': ['data/*', 'data/config.yml',
-    #                                   'data/requirements-stc.txt', 'data/requirements-dest.txt']},
-    package_data={f'alexber.{SHORT_NAME}': ['data/*'
-                                            ]},
-    include_package_data=True,
-    install_requires=install_requires,
-    # entry_points={"console_scripts": [
-    #     f"python-{SHORT_NAME}-tool=alexber.{SHORT_NAME}.data.__main__:main"
-    # ]},
-    # $ setup.py publish support.
-    # python3 setup.py upload
-    cmdclass={
-        'upload': UploadCommand,
-    },
-    extras_require=extras,
-    test_suite="tests",
-    tests_require=tests_require,
-    setup_requires=['pytest-runner'],
-    namespace_packages=('alexber',),
-    license='Apache 2.0',
-    keywords='tools tool utils enum enums threadlocal UploadCommand upload uuid1mc uuid UUID UUID1 UUID4 UU1DMC ' \
-             'issetdescriptor ismethod ' \
-             'importer new_instance safe_eval is_empty parse_boolean Properties java.util.Properties',
-    classifiers=[
-        # See: https://pypi.python.org/pypi?:action=list_classifiers
-        'Development Status :: 5 - Production/Stable',
-        'Environment :: Console',
-        'Intended Audience :: Developers',
-        'Intended Audience :: Education',
-        'License :: OSI Approved :: BSD License',
-
-        # List of python versions and their support status:
-        # https://en.wikipedia.org/wiki/CPython#Version_history
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-        'Programming Language :: Python :: Implementation :: CPython',
-        "Topic :: Utilities",
-        'Topic :: Software Development :: Libraries :: Python Modules',
-        'Topic :: Desktop Environment',
-        'Topic :: Education',
-        'Operating System :: OS Independent',
-        'Operating System :: Microsoft :: Windows',
-        'Operating System :: POSIX',
-        'Operating System :: Unix',
-        'Natural Language :: English',
-    ],
-    python_requires='>=3.6',
-    zip_safe=False,
-
-)
-
+import os
+
+import setuptools
+from setuptools import setup
+
+
+#VERSION should be defined before importing UploadCommand
+VERSION = '0.8.1a2'
+from alexber.utils import UploadCommand
+NAME = 'alex_ber_utils'
+SHORT_NAME = 'utils'
+VCS_URL = 'https://github.com/alex-ber/AlexBerUtils'
+DESCRIPTION = 'AlexBerUtils is collection of the small utilities'
+AUTHOR = 'Alexander Berkovich'
+
+
+base_dir = os.path.dirname(os.path.realpath(__file__))
+
+def get_content(filename):
+    with open(os.path.join(base_dir, filename)) as f:
+        content = f.read().splitlines()
+    return content
+
+install_requires = get_content('requirements.txt')
+tests_require = get_content('requirements-tests.txt')
+
+extras = {
+    'md': get_content('req-md.txt'),
+    'fabric' : get_content('req-fabric.txt'),
+    'yaml' : get_content('req-yml.txt'),
+    'yml' : get_content('req-yml.txt'),
+    'env' : get_content('req-env.txt'),
+    'tests': tests_require,
+    'piptools' : get_content('req-env.txt')
+}
+
+lnk_data = os.path.join('alexber', SHORT_NAME, 'data')
+
+
+
+try:
+    try:
+        os.unlink(lnk_data)
+    except OSError:
+        pass
+
+    os.symlink(os.path.join('..', '..', 'data'), lnk_data)
+
+    setup(
+        name=NAME,
+        version=VERSION,
+        url=VCS_URL,
+        author=AUTHOR,
+        description=DESCRIPTION,
+        long_description="\n\n".join([
+            open(os.path.join(base_dir, "README.md"), "r").read(),
+            open(os.path.join(base_dir, "CHANGELOG.md"), "r").read()
+        ]),
+        long_description_content_type="text/markdown",
+        packages=setuptools.find_packages(exclude=('tests', 'tests.*', 'data')),
+        # see https://stackoverflow.com/a/26533921
+        # see also https://stackoverflow.com/questions/24347450/how-do-you-add-additional-files-to-a-wheel
+        # data_files=[(f'Lib/site-packages/alexber/{SHORT_NAME}', ['data/config.yml', 'data/requirements-src.txt',
+        #                                                    'data/driver.py']),
+        #             #(f'lib/python3.7/site-packages/alexber/{SHORT_NAME}', ['requirements-src.txt'])
+        #             ],
+        # package_data={'alexber.{SHORT_NAME}': ['data/*', 'data/config.yml',
+        #                                   'data/requirements-stc.txt', 'data/requirements-dest.txt']},
+        package_data={f'alexber.{SHORT_NAME}': ['data/*'
+                                                ]},
+        include_package_data=True,
+        install_requires=install_requires,
+        # entry_points={"console_scripts": [
+        #     f"python-{SHORT_NAME}-tool=alexber.{SHORT_NAME}.data.__main__:main"
+        # ]},
+        # $ setup.py publish support.
+        # python3 setup.py upload
+        cmdclass={
+            'upload': UploadCommand,
+        },
+        extras_require=extras,
+        test_suite="tests",
+        tests_require=tests_require,
+        setup_requires=['pytest-runner'],
+        namespace_packages=('alexber',),
+        license='Apache 2.0',
+        keywords='tools tool utils enum enums threadlocal UploadCommand upload uuid1mc uuid UUID UUID1 UUID4 UU1DMC ' \
+                 'issetdescriptor ismethod ' \
+                 'importer new_instance safe_eval is_empty parse_boolean Properties java.util.Properties',
+        classifiers=[
+            # See: https://pypi.python.org/pypi?:action=list_classifiers
+            'Development Status :: 5 - Production/Stable',
+            'Environment :: Console',
+            'Intended Audience :: Developers',
+            'Intended Audience :: Education',
+            'License :: OSI Approved :: BSD License',
+
+            # List of python versions and their support status:
+            # https://en.wikipedia.org/wiki/CPython#Version_history
+            'Programming Language :: Python',
+            'Programming Language :: Python :: 3 :: Only',
+            'Programming Language :: Python :: 3.6',
+            'Programming Language :: Python :: 3.7',
+            'Programming Language :: Python :: 3.8',
+            'Programming Language :: Python :: 3.9',
+            'Programming Language :: Python :: 3.10',
+            'Programming Language :: Python :: 3.11',
+            'Programming Language :: Python :: Implementation :: CPython',
+            "Topic :: Utilities",
+            'Topic :: Software Development :: Libraries :: Python Modules',
+            'Topic :: Desktop Environment',
+            'Topic :: Education',
+            'Operating System :: OS Independent',
+            'Operating System :: Microsoft :: Windows',
+            'Operating System :: POSIX',
+            'Operating System :: Unix',
+            'Natural Language :: English',
+        ],
+        python_requires='>=3.6',
+        zip_safe=False,
+
+    )
+
+finally:
+    try:
+        os.unlink(lnk_data)
+    except OSError:
+        pass
```

### Comparing `alex_ber_utils-0.8.1a0/tests/conftest.py` & `alex_ber_utils-0.8.1a2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a0/tests/utils/deploys_test.py` & `alex_ber_utils-0.8.1a2/tests/utils/deploys_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a0/tests/utils/emails_test.py` & `alex_ber_utils-0.8.1a2/tests/utils/emails_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a0/tests/utils/enums_mixin_test.py` & `alex_ber_utils-0.8.1a2/tests/utils/enums_mixin_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a0/tests/utils/importer_test.py` & `alex_ber_utils-0.8.1a2/tests/utils/importer_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a0/tests/utils/init_app_conf_test.py` & `alex_ber_utils-0.8.1a2/tests/utils/init_app_conf_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a0/tests/utils/inspect_test.py` & `alex_ber_utils-0.8.1a2/tests/utils/inspect_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a0/tests/utils/mains_test.py` & `alex_ber_utils-0.8.1a2/tests/utils/mains_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a0/tests/utils/method_overloading_test.py` & `alex_ber_utils-0.8.1a2/tests/utils/method_overloading_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a0/tests/utils/parsers_test.py` & `alex_ber_utils-0.8.1a2/tests/utils/parsers_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a0/tests/utils/processinvokes_test.py` & `alex_ber_utils-0.8.1a2/tests/utils/processinvokes_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a0/tests/utils/properties_test.py` & `alex_ber_utils-0.8.1a2/tests/utils/properties_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a0/tests/utils/threadlocal_test.py` & `alex_ber_utils-0.8.1a2/tests/utils/threadlocal_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a0/tests/utils/uuids_test.py` & `alex_ber_utils-0.8.1a2/tests/utils/uuids_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a0/tests/utils/ymlparsers_extra_test.py` & `alex_ber_utils-0.8.1a2/tests/utils/ymlparsers_extra_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a0/tests/utils/ymlparsers_test.py` & `alex_ber_utils-0.8.1a2/tests/utils/ymlparsers_test.py`

 * *Files identical despite different names*

