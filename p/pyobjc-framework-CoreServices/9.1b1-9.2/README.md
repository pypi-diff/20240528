# Comparing `tmp/pyobjc-framework-CoreServices-9.1b1.tar.gz` & `tmp/pyobjc-framework-CoreServices-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-CoreServices-9.1b1.tar", last modified: Sun Mar 26 11:21:56 2023, max compression
+gzip compressed data, was "pyobjc-framework-CoreServices-9.2.tar", last modified: Wed Jun  7 00:11:56 2023, max compression
```

## Comparing `pyobjc-framework-CoreServices-9.1b1.tar` & `pyobjc-framework-CoreServices-9.2.tar`

### file list

```diff
@@ -1,164 +1,165 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:21:56.124693 pyobjc-framework-CoreServices-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:21:55.846854 pyobjc-framework-CoreServices-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:21:55.851725 pyobjc-framework-CoreServices-9.1b1/Lib/CoreServices/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:21:55.853310 pyobjc-framework-CoreServices-9.1b1/Lib/CoreServices/CarbonCore/
--rw-r--r--   0 ronald     (501) staff       (20)      884 2020-11-30 18:45:14.000000 pyobjc-framework-CoreServices-9.1b1/Lib/CoreServices/CarbonCore/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    25717 2023-03-25 15:03:24.000000 pyobjc-framework-CoreServices-9.1b1/Lib/CoreServices/CarbonCore/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:21:55.857591 pyobjc-framework-CoreServices-9.1b1/Lib/CoreServices/DictionaryServices/
--rw-r--r--   0 ronald     (501) staff       (20)      784 2020-11-30 18:45:14.000000 pyobjc-framework-CoreServices-9.1b1/Lib/CoreServices/DictionaryServices/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     1005 2023-03-25 15:03:24.000000 pyobjc-framework-CoreServices-9.1b1/Lib/CoreServices/DictionaryServices/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:21:55.860415 pyobjc-framework-CoreServices-9.1b1/Lib/CoreServices/LaunchServices/
--rw-r--r--   0 ronald     (501) staff       (20)      791 2020-11-30 18:45:14.000000 pyobjc-framework-CoreServices-9.1b1/Lib/CoreServices/LaunchServices/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    38369 2023-03-25 15:03:24.000000 pyobjc-framework-CoreServices-9.1b1/Lib/CoreServices/LaunchServices/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:21:55.866997 pyobjc-framework-CoreServices-9.1b1/Lib/CoreServices/Metadata/
--rw-r--r--   0 ronald     (501) staff       (20)      815 2020-11-30 18:45:14.000000 pyobjc-framework-CoreServices-9.1b1/Lib/CoreServices/Metadata/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    14703 2023-03-25 15:03:24.000000 pyobjc-framework-CoreServices-9.1b1/Lib/CoreServices/Metadata/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:21:55.869086 pyobjc-framework-CoreServices-9.1b1/Lib/CoreServices/SearchKit/
--rw-r--r--   0 ronald     (501) staff       (20)     4162 2020-11-30 18:45:14.000000 pyobjc-framework-CoreServices-9.1b1/Lib/CoreServices/SearchKit/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    11338 2023-03-25 15:03:24.000000 pyobjc-framework-CoreServices-9.1b1/Lib/CoreServices/SearchKit/_metadata.py
--rw-r--r--   0 ronald     (501) staff       (20)      890 2020-11-30 18:45:14.000000 pyobjc-framework-CoreServices-9.1b1/Lib/CoreServices/__init__.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:21:55.873644 pyobjc-framework-CoreServices-9.1b1/Lib/pyobjc_framework_CoreServices.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2239 2023-03-26 11:21:55.000000 pyobjc-framework-CoreServices-9.1b1/Lib/pyobjc_framework_CoreServices.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     5184 2023-03-26 11:21:55.000000 pyobjc-framework-CoreServices-9.1b1/Lib/pyobjc_framework_CoreServices.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:21:55.000000 pyobjc-framework-CoreServices-9.1b1/Lib/pyobjc_framework_CoreServices.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:07.000000 pyobjc-framework-CoreServices-9.1b1/Lib/pyobjc_framework_CoreServices.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       52 2023-03-26 11:21:55.000000 pyobjc-framework-CoreServices-9.1b1/Lib/pyobjc_framework_CoreServices.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       13 2023-03-26 11:21:55.000000 pyobjc-framework-CoreServices-9.1b1/Lib/pyobjc_framework_CoreServices.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-CoreServices-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-CoreServices-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:21:55.876120 pyobjc-framework-CoreServices-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)     1469 2021-03-21 10:08:22.000000 pyobjc-framework-CoreServices-9.1b1/Modules/_CoreServices_inlines.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-CoreServices-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-CoreServices-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     2028 2023-03-26 11:21:56.124222 pyobjc-framework-CoreServices-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:21:56.007562 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:14.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     2459 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_aiff.py
--rw-r--r--   0 ronald     (501) staff       (20)     3686 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_aliases.py
--rw-r--r--   0 ronald     (501) staff       (20)     2853 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_avltree.py
--rw-r--r--   0 ronald     (501) staff       (20)      417 2021-03-21 10:08:22.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_backupcore.py
--rw-r--r--   0 ronald     (501) staff       (20)     5576 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_codefragments.py
--rw-r--r--   0 ronald     (501) staff       (20)    11956 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_collections.py
--rw-r--r--   0 ronald     (501) staff       (20)    10444 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_components.py
--rw-r--r--   0 ronald     (501) staff       (20)      650 2023-03-03 17:21:59.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_coreservices.py
--rw-r--r--   0 ronald     (501) staff       (20)     5100 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_datetimeutils.py
--rw-r--r--   0 ronald     (501) staff       (20)     3582 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_debugging.py
--rw-r--r--   0 ronald     (501) staff       (20)      752 2022-01-02 11:04:26.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_dictionaryservices.py
--rw-r--r--   0 ronald     (501) staff       (20)      571 2021-03-21 10:08:22.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_diskspacerecovery.py
--rw-r--r--   0 ronald     (501) staff       (20)     1547 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_driverservices.py
--rw-r--r--   0 ronald     (501) staff       (20)     1327 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_driversynchronization.py
--rw-r--r--   0 ronald     (501) staff       (20)     2857 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_endian.py
--rw-r--r--   0 ronald     (501) staff       (20)    51353 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_files.py
--rw-r--r--   0 ronald     (501) staff       (20)     4626 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_finder.py
--rw-r--r--   0 ronald     (501) staff       (20)     2439 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_fixmath.py
--rw-r--r--   0 ronald     (501) staff       (20)    14964 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_folders.py
--rw-r--r--   0 ronald     (501) staff       (20)     7049 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_fp.py
--rw-r--r--   0 ronald     (501) staff       (20)    60830 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_gestalt.py
--rw-r--r--   0 ronald     (501) staff       (20)    23221 2021-04-09 10:15:21.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_iconscore.py
--rw-r--r--   0 ronald     (501) staff       (20)     3398 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_intlresources.py
--rw-r--r--   0 ronald     (501) staff       (20)     2838 2021-04-09 10:15:21.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_launchservices.py
--rw-r--r--   0 ronald     (501) staff       (20)     4784 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_lowmem.py
--rw-r--r--   0 ronald     (501) staff       (20)    16710 2022-06-25 20:19:21.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_lsinfo.py
--rw-r--r--   0 ronald     (501) staff       (20)     6111 2022-01-02 11:04:26.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_lsopen.py
--rw-r--r--   0 ronald     (501) staff       (20)     1132 2021-03-21 10:08:22.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_lsquarantine.py
--rw-r--r--   0 ronald     (501) staff       (20)     6890 2021-03-21 10:08:22.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_lssharedfilelist.py
--rw-r--r--   0 ronald     (501) staff       (20)   119330 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_macerrors.py
--rw-r--r--   0 ronald     (501) staff       (20)     4818 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_machineexceptions.py
--rw-r--r--   0 ronald     (501) staff       (20)     2961 2022-01-02 11:04:26.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_maclocales.py
--rw-r--r--   0 ronald     (501) staff       (20)     7400 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_macmemory.py
--rw-r--r--   0 ronald     (501) staff       (20)     3662 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_math64.py
--rw-r--r--   0 ronald     (501) staff       (20)    13293 2021-03-21 10:08:22.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_mditem.py
--rw-r--r--   0 ronald     (501) staff       (20)     2652 2021-03-21 10:08:22.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_mdlabel.py
--rw-r--r--   0 ronald     (501) staff       (20)     4511 2022-01-02 11:04:26.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_mdquery.py
--rw-r--r--   0 ronald     (501) staff       (20)     1290 2021-03-21 10:08:22.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_mdschema.py
--rw-r--r--   0 ronald     (501) staff       (20)     8335 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_mixedmode.py
--rw-r--r--   0 ronald     (501) staff       (20)     8779 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_multiprocessing.py
--rw-r--r--   0 ronald     (501) staff       (20)     1096 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_multiprocessinginfo.py
--rw-r--r--   0 ronald     (501) staff       (20)     1822 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_numberformatting.py
--rw-r--r--   0 ronald     (501) staff       (20)     3767 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_osutils.py
--rw-r--r--   0 ronald     (501) staff       (20)    12757 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_pefbinaryformat.py
--rw-r--r--   0 ronald     (501) staff       (20)      861 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_plstringfuncs.py
--rw-r--r--   0 ronald     (501) staff       (20)     4857 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_resources.py
--rw-r--r--   0 ronald     (501) staff       (20)    36756 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_script.py
--rw-r--r--   0 ronald     (501) staff       (20)     1641 2021-03-21 10:08:22.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_searchkit.py
--rw-r--r--   0 ronald     (501) staff       (20)      717 2021-03-21 10:08:22.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_skanalysis.py
--rw-r--r--   0 ronald     (501) staff       (20)     1353 2021-03-21 10:08:22.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_skdocument.py
--rw-r--r--   0 ronald     (501) staff       (20)     6999 2023-03-03 17:21:59.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_skindex.py
--rw-r--r--   0 ronald     (501) staff       (20)     6266 2022-01-02 11:04:26.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_sksearch.py
--rw-r--r--   0 ronald     (501) staff       (20)     1873 2021-03-21 10:08:22.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_sksummary.py
--rw-r--r--   0 ronald     (501) staff       (20)     1899 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_stringcompare.py
--rw-r--r--   0 ronald     (501) staff       (20)    29082 2022-01-02 11:04:26.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_textcommon.py
--rw-r--r--   0 ronald     (501) staff       (20)     7981 2022-01-02 11:04:26.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_textencodingconvertor.py
--rw-r--r--   0 ronald     (501) staff       (20)     2324 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_textencodingplugin.py
--rw-r--r--   0 ronald     (501) staff       (20)     1634 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_textutils.py
--rw-r--r--   0 ronald     (501) staff       (20)     3558 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_threads.py
--rw-r--r--   0 ronald     (501) staff       (20)      944 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_timer.py
--rw-r--r--   0 ronald     (501) staff       (20)      620 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_toolutils.py
--rw-r--r--   0 ronald     (501) staff       (20)     5500 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_unicodeconvertor.py
--rw-r--r--   0 ronald     (501) staff       (20)     5103 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_unicodeutilities.py
--rw-r--r--   0 ronald     (501) staff       (20)     8714 2021-03-21 10:08:22.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_utcoretypes.py
--rw-r--r--   0 ronald     (501) staff       (20)      908 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_utcutils.py
--rw-r--r--   0 ronald     (501) staff       (20)     4112 2021-03-21 10:08:22.000000 pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_uttype.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:21:56.019553 pyobjc-framework-CoreServices-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)   361498 2022-04-11 14:24:52.000000 pyobjc-framework-CoreServices-9.1b1/metadata/CarbonCore.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)      932 2023-03-25 15:03:24.000000 pyobjc-framework-CoreServices-9.1b1/metadata/DictionaryServices.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    22802 2020-11-30 18:45:14.000000 pyobjc-framework-CoreServices-9.1b1/metadata/HIServices.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    13697 2021-03-21 10:08:22.000000 pyobjc-framework-CoreServices-9.1b1/metadata/LaunchServices.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     7420 2020-11-30 18:45:14.000000 pyobjc-framework-CoreServices-9.1b1/metadata/Metadata.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    26714 2020-11-30 18:45:14.000000 pyobjc-framework-CoreServices-9.1b1/metadata/PrintCore.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     8418 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.1b1/metadata/SearchKit.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)      948 2021-03-21 10:08:22.000000 pyobjc-framework-CoreServices-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:21:56.020355 pyobjc-framework-CoreServices-9.1b1/metadata/raw.AE/
--rw-r--r--   0 ronald     (501) staff       (20)    87175 2021-03-21 10:08:22.000000 pyobjc-framework-CoreServices-9.1b1/metadata/raw.AE/x86_64-10.16.fwinfo
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:21:56.051896 pyobjc-framework-CoreServices-9.1b1/metadata/raw.CarbonCore/
--rw-r--r--   0 ronald     (501) staff       (20)   521052 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.1b1/metadata/raw.CarbonCore/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   521045 2022-02-24 08:47:16.000000 pyobjc-framework-CoreServices-9.1b1/metadata/raw.CarbonCore/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   864305 2020-11-30 18:45:14.000000 pyobjc-framework-CoreServices-9.1b1/metadata/raw.CarbonCore/x86_64-10.13.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   522516 2020-11-30 18:45:14.000000 pyobjc-framework-CoreServices-9.1b1/metadata/raw.CarbonCore/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   522525 2021-03-21 10:08:22.000000 pyobjc-framework-CoreServices-9.1b1/metadata/raw.CarbonCore/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   522683 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.1b1/metadata/raw.CarbonCore/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   522676 2022-02-24 08:47:16.000000 pyobjc-framework-CoreServices-9.1b1/metadata/raw.CarbonCore/x86_64-12.3.fwinfo
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:21:56.064735 pyobjc-framework-CoreServices-9.1b1/metadata/raw.DictionaryServices/
--rw-r--r--   0 ronald     (501) staff       (20)     1442 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.1b1/metadata/raw.DictionaryServices/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     1461 2022-02-24 08:47:16.000000 pyobjc-framework-CoreServices-9.1b1/metadata/raw.DictionaryServices/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     1445 2020-11-30 18:45:14.000000 pyobjc-framework-CoreServices-9.1b1/metadata/raw.DictionaryServices/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     1443 2021-03-21 10:08:22.000000 pyobjc-framework-CoreServices-9.1b1/metadata/raw.DictionaryServices/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     1332 2020-11-30 18:45:14.000000 pyobjc-framework-CoreServices-9.1b1/metadata/raw.DictionaryServices/x86_64-10.6.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     1332 2020-11-30 18:45:14.000000 pyobjc-framework-CoreServices-9.1b1/metadata/raw.DictionaryServices/x86_64-10.7.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     1422 2020-11-30 18:45:14.000000 pyobjc-framework-CoreServices-9.1b1/metadata/raw.DictionaryServices/x86_64-10.8.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     1443 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.1b1/metadata/raw.DictionaryServices/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)     1462 2022-02-24 08:47:16.000000 pyobjc-framework-CoreServices-9.1b1/metadata/raw.DictionaryServices/x86_64-12.3.fwinfo
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:21:56.098978 pyobjc-framework-CoreServices-9.1b1/metadata/raw.LaunchServices/
--rw-r--r--   0 ronald     (501) staff       (20)    52179 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.1b1/metadata/raw.LaunchServices/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    52473 2022-02-24 08:47:16.000000 pyobjc-framework-CoreServices-9.1b1/metadata/raw.LaunchServices/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    53089 2022-06-25 20:19:21.000000 pyobjc-framework-CoreServices-9.1b1/metadata/raw.LaunchServices/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    61827 2020-11-30 18:45:14.000000 pyobjc-framework-CoreServices-9.1b1/metadata/raw.LaunchServices/x86_64-10.10.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    52182 2020-11-30 18:45:14.000000 pyobjc-framework-CoreServices-9.1b1/metadata/raw.LaunchServices/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    52180 2021-03-21 10:08:22.000000 pyobjc-framework-CoreServices-9.1b1/metadata/raw.LaunchServices/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    53070 2020-11-30 18:45:14.000000 pyobjc-framework-CoreServices-9.1b1/metadata/raw.LaunchServices/x86_64-10.6.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    53070 2020-11-30 18:45:14.000000 pyobjc-framework-CoreServices-9.1b1/metadata/raw.LaunchServices/x86_64-10.7.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    53138 2020-11-30 18:45:14.000000 pyobjc-framework-CoreServices-9.1b1/metadata/raw.LaunchServices/x86_64-10.8.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    52180 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.1b1/metadata/raw.LaunchServices/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    52474 2022-02-24 08:47:16.000000 pyobjc-framework-CoreServices-9.1b1/metadata/raw.LaunchServices/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    53090 2022-06-25 20:19:21.000000 pyobjc-framework-CoreServices-9.1b1/metadata/raw.LaunchServices/x86_64-13.0.fwinfo
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:21:56.104965 pyobjc-framework-CoreServices-9.1b1/metadata/raw.Metadata/
--rw-r--r--   0 ronald     (501) staff       (20)    31903 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.1b1/metadata/raw.Metadata/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    31922 2022-02-24 08:47:16.000000 pyobjc-framework-CoreServices-9.1b1/metadata/raw.Metadata/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    32019 2020-11-30 18:45:14.000000 pyobjc-framework-CoreServices-9.1b1/metadata/raw.Metadata/x86_64-10.13.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    31906 2020-11-30 18:45:14.000000 pyobjc-framework-CoreServices-9.1b1/metadata/raw.Metadata/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    31904 2021-03-21 10:08:22.000000 pyobjc-framework-CoreServices-9.1b1/metadata/raw.Metadata/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    31904 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.1b1/metadata/raw.Metadata/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    31923 2022-02-24 08:47:16.000000 pyobjc-framework-CoreServices-9.1b1/metadata/raw.Metadata/x86_64-12.3.fwinfo
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:21:56.122896 pyobjc-framework-CoreServices-9.1b1/metadata/raw.SearchKit/
--rw-r--r--   0 ronald     (501) staff       (20)    22148 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.1b1/metadata/raw.SearchKit/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    22305 2022-02-24 08:47:16.000000 pyobjc-framework-CoreServices-9.1b1/metadata/raw.SearchKit/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    22151 2020-11-30 18:45:14.000000 pyobjc-framework-CoreServices-9.1b1/metadata/raw.SearchKit/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    22149 2021-03-21 10:08:22.000000 pyobjc-framework-CoreServices-9.1b1/metadata/raw.SearchKit/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    22353 2020-11-30 18:45:14.000000 pyobjc-framework-CoreServices-9.1b1/metadata/raw.SearchKit/x86_64-10.6.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    22353 2020-11-30 18:45:14.000000 pyobjc-framework-CoreServices-9.1b1/metadata/raw.SearchKit/x86_64-10.7.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    22421 2020-11-30 18:45:14.000000 pyobjc-framework-CoreServices-9.1b1/metadata/raw.SearchKit/x86_64-10.8.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    22149 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.1b1/metadata/raw.SearchKit/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    22306 2022-02-24 08:47:16.000000 pyobjc-framework-CoreServices-9.1b1/metadata/raw.SearchKit/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-CoreServices-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:21:56.124798 pyobjc-framework-CoreServices-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1166 2023-03-25 14:20:31.000000 pyobjc-framework-CoreServices-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:11:56.641753 pyobjc-framework-CoreServices-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:11:56.454756 pyobjc-framework-CoreServices-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:11:56.460782 pyobjc-framework-CoreServices-9.2/Lib/CoreServices/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:11:56.462351 pyobjc-framework-CoreServices-9.2/Lib/CoreServices/CarbonCore/
+-rw-r--r--   0 ronald     (501) staff       (20)      884 2020-11-30 18:45:14.000000 pyobjc-framework-CoreServices-9.2/Lib/CoreServices/CarbonCore/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    25672 2023-05-27 09:46:33.000000 pyobjc-framework-CoreServices-9.2/Lib/CoreServices/CarbonCore/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:11:56.464307 pyobjc-framework-CoreServices-9.2/Lib/CoreServices/DictionaryServices/
+-rw-r--r--   0 ronald     (501) staff       (20)      784 2020-11-30 18:45:14.000000 pyobjc-framework-CoreServices-9.2/Lib/CoreServices/DictionaryServices/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1005 2023-05-27 09:46:33.000000 pyobjc-framework-CoreServices-9.2/Lib/CoreServices/DictionaryServices/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:11:56.465611 pyobjc-framework-CoreServices-9.2/Lib/CoreServices/LaunchServices/
+-rw-r--r--   0 ronald     (501) staff       (20)      791 2020-11-30 18:45:14.000000 pyobjc-framework-CoreServices-9.2/Lib/CoreServices/LaunchServices/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    37742 2023-05-27 09:46:33.000000 pyobjc-framework-CoreServices-9.2/Lib/CoreServices/LaunchServices/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:11:56.467845 pyobjc-framework-CoreServices-9.2/Lib/CoreServices/Metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)      815 2020-11-30 18:45:14.000000 pyobjc-framework-CoreServices-9.2/Lib/CoreServices/Metadata/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    14703 2023-05-27 09:46:33.000000 pyobjc-framework-CoreServices-9.2/Lib/CoreServices/Metadata/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:11:56.469433 pyobjc-framework-CoreServices-9.2/Lib/CoreServices/SearchKit/
+-rw-r--r--   0 ronald     (501) staff       (20)     4162 2020-11-30 18:45:14.000000 pyobjc-framework-CoreServices-9.2/Lib/CoreServices/SearchKit/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    11338 2023-05-27 09:46:33.000000 pyobjc-framework-CoreServices-9.2/Lib/CoreServices/SearchKit/_metadata.py
+-rw-r--r--   0 ronald     (501) staff       (20)      890 2020-11-30 18:45:14.000000 pyobjc-framework-CoreServices-9.2/Lib/CoreServices/__init__.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:11:56.473175 pyobjc-framework-CoreServices-9.2/Lib/pyobjc_framework_CoreServices.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2237 2023-06-07 00:11:56.000000 pyobjc-framework-CoreServices-9.2/Lib/pyobjc_framework_CoreServices.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     5199 2023-06-07 00:11:56.000000 pyobjc-framework-CoreServices-9.2/Lib/pyobjc_framework_CoreServices.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:11:56.000000 pyobjc-framework-CoreServices-9.2/Lib/pyobjc_framework_CoreServices.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:07.000000 pyobjc-framework-CoreServices-9.2/Lib/pyobjc_framework_CoreServices.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       48 2023-06-07 00:11:56.000000 pyobjc-framework-CoreServices-9.2/Lib/pyobjc_framework_CoreServices.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       13 2023-06-07 00:11:56.000000 pyobjc-framework-CoreServices-9.2/Lib/pyobjc_framework_CoreServices.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-CoreServices-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-CoreServices-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:11:56.475105 pyobjc-framework-CoreServices-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)     1469 2021-03-21 10:08:22.000000 pyobjc-framework-CoreServices-9.2/Modules/_CoreServices_inlines.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-CoreServices-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-CoreServices-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     2026 2023-06-07 00:11:56.641389 pyobjc-framework-CoreServices-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:11:56.541069 pyobjc-framework-CoreServices-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2020-11-30 18:45:14.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2459 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_aiff.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3686 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_aliases.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2853 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_avltree.py
+-rw-r--r--   0 ronald     (501) staff       (20)      417 2021-03-21 10:08:22.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_backupcore.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5576 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_codefragments.py
+-rw-r--r--   0 ronald     (501) staff       (20)    11956 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_collections.py
+-rw-r--r--   0 ronald     (501) staff       (20)    10444 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_components.py
+-rw-r--r--   0 ronald     (501) staff       (20)      650 2023-03-03 17:21:59.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_coreservices.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5100 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_datetimeutils.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3582 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_debugging.py
+-rw-r--r--   0 ronald     (501) staff       (20)      752 2022-01-02 11:04:26.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_dictionaryservices.py
+-rw-r--r--   0 ronald     (501) staff       (20)      571 2021-03-21 10:08:22.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_diskspacerecovery.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1547 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_driverservices.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1327 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_driversynchronization.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2857 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_endian.py
+-rw-r--r--   0 ronald     (501) staff       (20)    51353 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_files.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4626 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_finder.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2439 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_fixmath.py
+-rw-r--r--   0 ronald     (501) staff       (20)    14964 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_folders.py
+-rw-r--r--   0 ronald     (501) staff       (20)     7049 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_fp.py
+-rw-r--r--   0 ronald     (501) staff       (20)    60830 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_gestalt.py
+-rw-r--r--   0 ronald     (501) staff       (20)    23237 2023-05-27 09:46:33.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_iconscore.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3398 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_intlresources.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2838 2021-04-09 10:15:21.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_launchservices.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4784 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_lowmem.py
+-rw-r--r--   0 ronald     (501) staff       (20)    16710 2022-06-25 20:19:21.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_lsinfo.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6111 2022-01-02 11:04:26.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_lsopen.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1132 2021-03-21 10:08:22.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_lsquarantine.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6890 2021-03-21 10:08:22.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_lssharedfilelist.py
+-rw-r--r--   0 ronald     (501) staff       (20)   119330 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_macerrors.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4818 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_machineexceptions.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2961 2022-01-02 11:04:26.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_maclocales.py
+-rw-r--r--   0 ronald     (501) staff       (20)     7400 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_macmemory.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3662 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_math64.py
+-rw-r--r--   0 ronald     (501) staff       (20)    13294 2023-05-04 11:00:07.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_mditem.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2652 2021-03-21 10:08:22.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_mdlabel.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4511 2022-01-02 11:04:26.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_mdquery.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1290 2021-03-21 10:08:22.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_mdschema.py
+-rw-r--r--   0 ronald     (501) staff       (20)     8335 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_mixedmode.py
+-rw-r--r--   0 ronald     (501) staff       (20)     8779 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_multiprocessing.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1096 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_multiprocessinginfo.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1822 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_numberformatting.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3767 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_osutils.py
+-rw-r--r--   0 ronald     (501) staff       (20)    12757 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_pefbinaryformat.py
+-rw-r--r--   0 ronald     (501) staff       (20)      861 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_plstringfuncs.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4857 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_resources.py
+-rw-r--r--   0 ronald     (501) staff       (20)    36756 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_script.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1641 2021-03-21 10:08:22.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_searchkit.py
+-rw-r--r--   0 ronald     (501) staff       (20)      717 2021-03-21 10:08:22.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_skanalysis.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1353 2021-03-21 10:08:22.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_skdocument.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6999 2023-03-03 17:21:59.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_skindex.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6266 2022-01-02 11:04:26.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_sksearch.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1873 2021-03-21 10:08:22.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_sksummary.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1899 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_stringcompare.py
+-rw-r--r--   0 ronald     (501) staff       (20)    29082 2022-01-02 11:04:26.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_textcommon.py
+-rw-r--r--   0 ronald     (501) staff       (20)     7981 2022-01-02 11:04:26.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_textencodingconvertor.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2324 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_textencodingplugin.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1634 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_textutils.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3558 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_threads.py
+-rw-r--r--   0 ronald     (501) staff       (20)      944 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_timer.py
+-rw-r--r--   0 ronald     (501) staff       (20)      620 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_toolutils.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5500 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_unicodeconvertor.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5103 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_unicodeutilities.py
+-rw-r--r--   0 ronald     (501) staff       (20)     8714 2021-03-21 10:08:22.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_utcoretypes.py
+-rw-r--r--   0 ronald     (501) staff       (20)      908 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_utcutils.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4112 2021-03-21 10:08:22.000000 pyobjc-framework-CoreServices-9.2/PyObjCTest/test_uttype.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:11:56.561403 pyobjc-framework-CoreServices-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)   361807 2023-05-27 09:46:33.000000 pyobjc-framework-CoreServices-9.2/metadata/CarbonCore.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)      932 2023-03-25 15:03:24.000000 pyobjc-framework-CoreServices-9.2/metadata/DictionaryServices.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    22802 2020-11-30 18:45:14.000000 pyobjc-framework-CoreServices-9.2/metadata/HIServices.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    13777 2023-05-27 09:46:33.000000 pyobjc-framework-CoreServices-9.2/metadata/LaunchServices.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     7420 2020-11-30 18:45:14.000000 pyobjc-framework-CoreServices-9.2/metadata/Metadata.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    26714 2020-11-30 18:45:14.000000 pyobjc-framework-CoreServices-9.2/metadata/PrintCore.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     8418 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.2/metadata/SearchKit.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)      948 2021-03-21 10:08:22.000000 pyobjc-framework-CoreServices-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:11:56.567792 pyobjc-framework-CoreServices-9.2/metadata/raw.AE/
+-rw-r--r--   0 ronald     (501) staff       (20)    87175 2021-03-21 10:08:22.000000 pyobjc-framework-CoreServices-9.2/metadata/raw.AE/x86_64-10.16.fwinfo
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:11:56.586858 pyobjc-framework-CoreServices-9.2/metadata/raw.CarbonCore/
+-rw-r--r--   0 ronald     (501) staff       (20)   521052 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.2/metadata/raw.CarbonCore/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   521045 2022-02-24 08:47:16.000000 pyobjc-framework-CoreServices-9.2/metadata/raw.CarbonCore/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   864305 2020-11-30 18:45:14.000000 pyobjc-framework-CoreServices-9.2/metadata/raw.CarbonCore/x86_64-10.13.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   522516 2020-11-30 18:45:14.000000 pyobjc-framework-CoreServices-9.2/metadata/raw.CarbonCore/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   522525 2021-03-21 10:08:22.000000 pyobjc-framework-CoreServices-9.2/metadata/raw.CarbonCore/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   522683 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.2/metadata/raw.CarbonCore/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   522676 2022-02-24 08:47:16.000000 pyobjc-framework-CoreServices-9.2/metadata/raw.CarbonCore/x86_64-12.3.fwinfo
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:11:56.593970 pyobjc-framework-CoreServices-9.2/metadata/raw.DictionaryServices/
+-rw-r--r--   0 ronald     (501) staff       (20)     1442 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.2/metadata/raw.DictionaryServices/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     1461 2022-02-24 08:47:16.000000 pyobjc-framework-CoreServices-9.2/metadata/raw.DictionaryServices/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     1445 2020-11-30 18:45:14.000000 pyobjc-framework-CoreServices-9.2/metadata/raw.DictionaryServices/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     1443 2021-03-21 10:08:22.000000 pyobjc-framework-CoreServices-9.2/metadata/raw.DictionaryServices/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     1332 2020-11-30 18:45:14.000000 pyobjc-framework-CoreServices-9.2/metadata/raw.DictionaryServices/x86_64-10.6.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     1332 2020-11-30 18:45:14.000000 pyobjc-framework-CoreServices-9.2/metadata/raw.DictionaryServices/x86_64-10.7.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     1422 2020-11-30 18:45:14.000000 pyobjc-framework-CoreServices-9.2/metadata/raw.DictionaryServices/x86_64-10.8.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     1443 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.2/metadata/raw.DictionaryServices/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)     1462 2022-02-24 08:47:16.000000 pyobjc-framework-CoreServices-9.2/metadata/raw.DictionaryServices/x86_64-12.3.fwinfo
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:11:56.623306 pyobjc-framework-CoreServices-9.2/metadata/raw.LaunchServices/
+-rw-r--r--   0 ronald     (501) staff       (20)    52179 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.2/metadata/raw.LaunchServices/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    52473 2022-02-24 08:47:16.000000 pyobjc-framework-CoreServices-9.2/metadata/raw.LaunchServices/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    53089 2022-06-25 20:19:21.000000 pyobjc-framework-CoreServices-9.2/metadata/raw.LaunchServices/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    61827 2020-11-30 18:45:14.000000 pyobjc-framework-CoreServices-9.2/metadata/raw.LaunchServices/x86_64-10.10.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    52182 2020-11-30 18:45:14.000000 pyobjc-framework-CoreServices-9.2/metadata/raw.LaunchServices/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    52180 2021-03-21 10:08:22.000000 pyobjc-framework-CoreServices-9.2/metadata/raw.LaunchServices/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    53070 2020-11-30 18:45:14.000000 pyobjc-framework-CoreServices-9.2/metadata/raw.LaunchServices/x86_64-10.6.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    53070 2020-11-30 18:45:14.000000 pyobjc-framework-CoreServices-9.2/metadata/raw.LaunchServices/x86_64-10.7.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    53138 2020-11-30 18:45:14.000000 pyobjc-framework-CoreServices-9.2/metadata/raw.LaunchServices/x86_64-10.8.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    52180 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.2/metadata/raw.LaunchServices/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    52474 2022-02-24 08:47:16.000000 pyobjc-framework-CoreServices-9.2/metadata/raw.LaunchServices/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    53090 2022-06-25 20:19:21.000000 pyobjc-framework-CoreServices-9.2/metadata/raw.LaunchServices/x86_64-13.0.fwinfo
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:11:56.632997 pyobjc-framework-CoreServices-9.2/metadata/raw.Metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)    31903 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.2/metadata/raw.Metadata/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    31922 2022-02-24 08:47:16.000000 pyobjc-framework-CoreServices-9.2/metadata/raw.Metadata/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    32019 2020-11-30 18:45:14.000000 pyobjc-framework-CoreServices-9.2/metadata/raw.Metadata/x86_64-10.13.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    31906 2020-11-30 18:45:14.000000 pyobjc-framework-CoreServices-9.2/metadata/raw.Metadata/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    31904 2021-03-21 10:08:22.000000 pyobjc-framework-CoreServices-9.2/metadata/raw.Metadata/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    31904 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.2/metadata/raw.Metadata/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    31923 2022-02-24 08:47:16.000000 pyobjc-framework-CoreServices-9.2/metadata/raw.Metadata/x86_64-12.3.fwinfo
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:11:56.640568 pyobjc-framework-CoreServices-9.2/metadata/raw.SearchKit/
+-rw-r--r--   0 ronald     (501) staff       (20)    22148 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.2/metadata/raw.SearchKit/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    22305 2022-02-24 08:47:16.000000 pyobjc-framework-CoreServices-9.2/metadata/raw.SearchKit/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    22151 2020-11-30 18:45:14.000000 pyobjc-framework-CoreServices-9.2/metadata/raw.SearchKit/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    22149 2021-03-21 10:08:22.000000 pyobjc-framework-CoreServices-9.2/metadata/raw.SearchKit/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    22353 2020-11-30 18:45:14.000000 pyobjc-framework-CoreServices-9.2/metadata/raw.SearchKit/x86_64-10.6.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    22353 2020-11-30 18:45:14.000000 pyobjc-framework-CoreServices-9.2/metadata/raw.SearchKit/x86_64-10.7.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    22421 2020-11-30 18:45:14.000000 pyobjc-framework-CoreServices-9.2/metadata/raw.SearchKit/x86_64-10.8.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    22149 2021-07-30 09:00:37.000000 pyobjc-framework-CoreServices-9.2/metadata/raw.SearchKit/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    22306 2022-02-24 08:47:16.000000 pyobjc-framework-CoreServices-9.2/metadata/raw.SearchKit/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-CoreServices-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-CoreServices-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:11:56.641900 pyobjc-framework-CoreServices-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1237 2023-05-29 10:07:46.000000 pyobjc-framework-CoreServices-9.2/setup.py
```

### Comparing `pyobjc-framework-CoreServices-9.1b1/Lib/CoreServices/CarbonCore/__init__.py` & `pyobjc-framework-CoreServices-9.2/Lib/CoreServices/CarbonCore/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/Lib/CoreServices/CarbonCore/_metadata.py` & `pyobjc-framework-CoreServices-9.2/Lib/CoreServices/CarbonCore/_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is generated by objective.metadata
 #
-# Last update: Sat Mar 25 15:50:34 2023
+# Last update: Sat May 20 12:00:23 2023
 #
 # flake8: noqa
 
 import objc, sys
 from typing import NewType
 
 if sys.maxsize > 2**32:
@@ -245,15 +245,15 @@
                 2: {"type_modifier": "o"},
             }
         },
     ),
     "TECSetBasicOptions": (b"i^{OpaqueTECObjectRef=}I",),
     "CSBackupSetItemExcluded": (b"i^{__CFURL=}ZZ",),
     "CSDiskSpaceGetRecoveryEstimate": (b"Q^{__CFURL=}",),
-    "LocaleOperationCountNames": (b"iI^Q",),
+    "GetTextEncodingVariant": (b"II",),
     "TECDisposeSniffer": (b"i^{OpaqueTECSnifferObjectRef=}",),
     "TECConvertTextToMultipleEncodings": (
         b"i^{OpaqueTECObjectRef=}^CQ^Q^CQ^Q^{TextEncodingRun=QI}Q^Q",
         "",
         {
             "arguments": {
                 1: {"c_array_length_in_arg": 2, "type_modifier": "n"},
@@ -375,25 +375,14 @@
         },
     ),
     "LocaleRefFromLangOrRegionCode": (
         b"iss^^{OpaqueLocaleRef=}",
         "",
         {"arguments": {2: {"type_modifier": "o"}}},
     ),
-    "TECCreateConverterFromPath": (
-        b"i^^{OpaqueTECObjectRef=}^IQ",
-        "",
-        {
-            "retval": {"already_cfretained": True},
-            "arguments": {
-                0: {"type_modifier": "o"},
-                1: {"c_array_length_in_arg": 2, "type_modifier": "n"},
-            },
-        },
-    ),
     "TECCreateConverter": (
         b"i^^{OpaqueTECObjectRef=}II",
         "",
         {
             "retval": {"already_cfretained": True},
             "arguments": {0: {"type_modifier": "o"}},
         },
@@ -462,15 +451,25 @@
         {"arguments": {1: {"type_modifier": "o"}}},
     ),
     "GetScriptInfoFromTextEncoding": (
         b"iI^s^s",
         "",
         {"arguments": {1: {"type_modifier": "o"}, 2: {"type_modifier": "o"}}},
     ),
-    "GetTextEncodingVariant": (b"II",),
+    "TECCreateConverterFromPath": (
+        b"i^^{OpaqueTECObjectRef=}^IQ",
+        "",
+        {
+            "retval": {"already_cfretained": True},
+            "arguments": {
+                0: {"type_modifier": "o"},
+                1: {"c_array_length_in_arg": 2, "type_modifier": "n"},
+            },
+        },
+    ),
     "TECDisposeConverter": (b"i^{OpaqueTECObjectRef=}",),
     "TECGetTextEncodingFromInternetName": (
         b"i^I^C",
         "",
         {"arguments": {0: {"type_modifier": "o"}, 1: {"type_modifier": "n"}}},
     ),
     "CSDiskSpaceCancelRecovery": (b"v^{__CFUUID=}",),
```

### Comparing `pyobjc-framework-CoreServices-9.1b1/Lib/CoreServices/DictionaryServices/__init__.py` & `pyobjc-framework-CoreServices-9.2/Lib/CoreServices/DictionaryServices/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/Lib/CoreServices/DictionaryServices/_metadata.py` & `pyobjc-framework-CoreServices-9.2/Lib/CoreServices/DictionaryServices/_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is generated by objective.metadata
 #
-# Last update: Sat Mar 25 15:50:34 2023
+# Last update: Sat May 20 12:00:23 2023
 #
 # flake8: noqa
 
 import objc, sys
 from typing import NewType
 
 if sys.maxsize > 2**32:
```

### Comparing `pyobjc-framework-CoreServices-9.1b1/Lib/CoreServices/LaunchServices/__init__.py` & `pyobjc-framework-CoreServices-9.2/Lib/CoreServices/LaunchServices/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/Lib/CoreServices/LaunchServices/_metadata.py` & `pyobjc-framework-CoreServices-9.2/Lib/CoreServices/LaunchServices/_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is generated by objective.metadata
 #
-# Last update: Sat Mar 25 15:50:34 2023
+# Last update: Sat May 20 12:00:23 2023
 #
 # flake8: noqa
 
 import objc, sys
 from typing import NewType
 
 if sys.maxsize > 2**32:
@@ -109,19 +109,14 @@
         },
     ),
     "GetIconRefFromTypeInfo": (
         b"sII^{__CFString=}^{__CFString=}I^^{OpaqueIconRef=}",
         "",
         {"arguments": {5: {"type_modifier": "o"}}},
     ),
-    "ReadIconFromFSRef": (
-        b"i^{FSRef=[80C]}^^^{IconFamilyResource=Ii[1{IconFamilyElement=Ii[1C]}]}",
-        "",
-        {"arguments": {0: {"type_modifier": "n"}}},
-    ),
     "LSSharedFileListRemoveAllItems": (b"i^{OpaqueLSSharedFileListRef=}",),
     "LSCopyItemAttribute": (
         b"i^{FSRef=[80C]}I^{__CFString=}^@",
         "",
         {
             "retval": {"already_cfretained": True},
             "arguments": {
@@ -220,19 +215,14 @@
             "arguments": {
                 4: {"type_modifier": "o"},
                 5: {"already_cfretained": True, "type_modifier": "o"},
             }
         },
     ),
     "LSSharedFileListItemGetTypeID": (b"Q",),
-    "GetIconRefFromComponent": (
-        b"i^{ComponentRecord=[1q]}^^{OpaqueIconRef=}",
-        "",
-        {"arguments": {1: {"type_modifier": "o"}}},
-    ),
     "UTTypeCopyDeclaration": (
         b"^{__CFDictionary=}^{__CFString=}",
         "",
         {"retval": {"already_cfretained": True}},
     ),
     "LSSharedFileListSetProperty": (b"i^{OpaqueLSSharedFileListRef=}^{__CFString=}@",),
     "LSSharedFileListItemCopyResolvedURL": (
@@ -262,19 +252,14 @@
                             1: {"type": b"^v"},
                         },
                     }
                 }
             }
         },
     ),
-    "RegisterIconRefFromFSRef": (
-        b"iII^{FSRef=[80C]}^^{OpaqueIconRef=}",
-        "",
-        {"arguments": {2: {"type_modifier": "n"}}},
-    ),
     "LSCopyApplicationForMIMEType": (
         b"i^{__CFString=}I^^{__CFURL=}",
         "",
         {
             "retval": {"already_cfretained": True},
             "arguments": {2: {"already_cfretained": True, "type_modifier": "o"}},
         },
@@ -441,15 +426,22 @@
         {
             "arguments": {
                 0: {"type_modifier": "n"},
                 1: {"already_cfretained": True, "type_modifier": "o"},
             }
         },
     ),
-    "UTTypeConformsTo": (b"Z^{__CFString=}^{__CFString=}",),
+    "LSCopyItemInfoForURL": (
+        b"i^{__CFURL=}I^{LSItemInfoRecord=III^{__CFString=}}",
+        "",
+        {
+            "retval": {"already_cfretained": True},
+            "arguments": {2: {"type_modifier": "o"}},
+        },
+    ),
     "SetCustomIconsEnabled": (b"ssZ",),
     "LSRegisterFSRef": (
         b"i^{FSRef=[80C]}Z",
         "",
         {"arguments": {0: {"type_modifier": "n"}}},
     ),
     "LSSetItemAttribute": (
@@ -489,17 +481,14 @@
         b"i^{__CFString=}^^{__CFString=}",
         "",
         {
             "retval": {"already_cfretained": True},
             "arguments": {1: {"already_cfretained": True, "type_modifier": "o"}},
         },
     ),
-    "RegisterIconRefFromIconFamily": (
-        b"sII^^{IconFamilyResource=Ii[1{IconFamilyElement=Ii[1C]}]}^^{OpaqueIconRef=}",
-    ),
     "UTTypeIsDeclared": (b"Z^{__CFString=}",),
     "LSCopyDisplayNameForURL": (
         b"i^{__CFURL=}^^{__CFString=}",
         "",
         {
             "retval": {"already_cfretained": True},
             "arguments": {1: {"already_cfretained": True, "type_modifier": "o"}},
@@ -568,22 +557,15 @@
                     "already_cfretained": True,
                     "type_modifier": "o",
                 }
             },
         },
     ),
     "GetCustomIconsEnabled": (b"ss^Z", "", {"arguments": {1: {"type_modifier": "o"}}}),
-    "LSCopyItemInfoForURL": (
-        b"i^{__CFURL=}I^{LSItemInfoRecord=III^{__CFString=}}",
-        "",
-        {
-            "retval": {"already_cfretained": True},
-            "arguments": {2: {"type_modifier": "o"}},
-        },
-    ),
+    "UTTypeConformsTo": (b"Z^{__CFString=}^{__CFString=}",),
     "LSFindApplicationForInfo": (
         b"iI^{__CFString=}^{__CFString=}^{FSRef=[80C]}^^{__CFURL=}",
         "",
         {
             "arguments": {
                 3: {"type_modifier": "o"},
                 4: {"already_cfretained": True, "type_modifier": "o"},
```

### Comparing `pyobjc-framework-CoreServices-9.1b1/Lib/CoreServices/Metadata/__init__.py` & `pyobjc-framework-CoreServices-9.2/Lib/CoreServices/Metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/Lib/CoreServices/Metadata/_metadata.py` & `pyobjc-framework-CoreServices-9.2/Lib/CoreServices/Metadata/_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is generated by objective.metadata
 #
-# Last update: Sat Mar 25 15:50:34 2023
+# Last update: Sat May 20 12:00:22 2023
 #
 # flake8: noqa
 
 import objc, sys
 from typing import NewType
 
 if sys.maxsize > 2**32:
```

### Comparing `pyobjc-framework-CoreServices-9.1b1/Lib/CoreServices/SearchKit/__init__.py` & `pyobjc-framework-CoreServices-9.2/Lib/CoreServices/SearchKit/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/Lib/CoreServices/SearchKit/_metadata.py` & `pyobjc-framework-CoreServices-9.2/Lib/CoreServices/SearchKit/_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is generated by objective.metadata
 #
-# Last update: Sat Mar 25 15:50:34 2023
+# Last update: Sat May 20 12:00:23 2023
 #
 # flake8: noqa
 
 import objc, sys
 from typing import NewType
 
 if sys.maxsize > 2**32:
```

### Comparing `pyobjc-framework-CoreServices-9.1b1/Lib/CoreServices/__init__.py` & `pyobjc-framework-CoreServices-9.2/Lib/CoreServices/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/Lib/pyobjc_framework_CoreServices.egg-info/PKG-INFO` & `pyobjc-framework-CoreServices-9.2/Lib/pyobjc_framework_CoreServices.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-CoreServices
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework CoreServices on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,CoreServices,CoreServices.CarbonCore,CoreServices.LaunchServices,CoreServices.DictionaryServices,CoreServices.SearchKit,CoreServices.Metadata
 Platform: MacOS X
```

### Comparing `pyobjc-framework-CoreServices-9.1b1/Lib/pyobjc_framework_CoreServices.egg-info/SOURCES.txt` & `pyobjc-framework-CoreServices-9.2/Lib/pyobjc_framework_CoreServices.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/CoreServices/__init__.py
 Lib/CoreServices/CarbonCore/__init__.py
 Lib/CoreServices/CarbonCore/_metadata.py
 Lib/CoreServices/DictionaryServices/__init__.py
 Lib/CoreServices/DictionaryServices/_metadata.py
 Lib/CoreServices/LaunchServices/__init__.py
```

### Comparing `pyobjc-framework-CoreServices-9.1b1/License.txt` & `pyobjc-framework-CoreServices-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/Modules/_CoreServices_inlines.m` & `pyobjc-framework-CoreServices-9.2/Modules/_CoreServices_inlines.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-CoreServices-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-CoreServices-9.2/Modules/pyobjc-compat.h`

 * *Files 2% similar despite different names*

```diff
@@ -301,14 +301,22 @@
 #define MAC_OS_X_VERSION_13_2 130200
 #endif
 
 #ifndef MAC_OS_X_VERSION_13_3
 #define MAC_OS_X_VERSION_13_3 130300
 #endif
 
+#ifndef MAC_OS_X_VERSION_13_4
+#define MAC_OS_X_VERSION_13_4 130400
+#endif
+
+#ifndef MAC_OS_X_VERSION_13_5
+#define MAC_OS_X_VERSION_13_5 130500
+#endif
+
 /*
  *
  * End of Cocoa definitions
  *
  */
 
 /*
@@ -499,10 +507,12 @@
     }
 
 #define PyObjC_LEAVE_GIL                                                                 \
     do {                                                                                 \
         PyGILState_Release(_GILState);                                                   \
     } while (0)
 
+extern PyObject* _Nullable PyObjC_get_tp_dict(PyTypeObject* _Nonnull tp);
+
 NS_ASSUME_NONNULL_END
 
 #endif /* PyObjC_COMPAT_H */
```

### Comparing `pyobjc-framework-CoreServices-9.1b1/PKG-INFO` & `pyobjc-framework-CoreServices-9.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-CoreServices
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework CoreServices on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,CoreServices,CoreServices.CarbonCore,CoreServices.LaunchServices,CoreServices.DictionaryServices,CoreServices.SearchKit,CoreServices.Metadata
 Platform: MacOS X
```

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_aiff.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_aiff.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_aliases.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_aliases.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_avltree.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_avltree.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_codefragments.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_codefragments.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_collections.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_collections.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_components.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_components.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_coreservices.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_coreservices.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_datetimeutils.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_datetimeutils.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_debugging.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_debugging.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_dictionaryservices.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_dictionaryservices.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_diskspacerecovery.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_diskspacerecovery.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_driverservices.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_driverservices.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_driversynchronization.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_driversynchronization.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_endian.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_endian.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_files.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_files.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_finder.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_finder.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_fixmath.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_fixmath.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_folders.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_folders.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_fp.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_fp.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_gestalt.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_gestalt.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_iconscore.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_iconscore.py`

 * *Files 0% similar despite different names*

```diff
@@ -379,23 +379,23 @@
             self.assertArgIsOut(CoreServices.GetIconRefFromFileInfo, 7)
 
             self.assertArgIsOut(CoreServices.GetIconRefFromTypeInfo, 5)
 
             self.assertArgIsIn(CoreServices.GetIconRefFromIconFamilyPtr, 0)
             self.assertArgIsOut(CoreServices.GetIconRefFromIconFamilyPtr, 2)
 
-            self.assertArgIsOut(CoreServices.GetIconRefFromComponent, 1)
+            # self.assertArgIsOut(CoreServices.GetIconRefFromComponent, 1)
 
             # XXX: Untested for now...
-            CoreServices.RegisterIconRefFromIconFamily
-            CoreServices.RegisterIconRefFromFSRef
-            CoreServices.UnregisterIconRef
-            CoreServices.UpdateIconRef
-            CoreServices.OverrideIconRef
-            CoreServices.RemoveIconRefOverride
+            # CoreServices.RegisterIconRefFromIconFamily
+            # CoreServices.RegisterIconRefFromFSRef
+            # CoreServices.UnregisterIconRef
+            # CoreServices.UpdateIconRef
+            # CoreServices.OverrideIconRef
+            # CoreServices.RemoveIconRefOverride
 
             self.assertArgIsOut(CoreServices.CompositeIconRef, 2)
 
             self.assertArgIsOut(CoreServices.IsIconRefComposite, 1)
             self.assertArgIsOut(CoreServices.IsIconRefComposite, 2)
 
             self.assertResultIsBOOL(CoreServices.IsValidIconRef)
@@ -406,15 +406,15 @@
             self.assertArgHasType(
                 CoreServices.GetCustomIconsEnabled,
                 1,
                 objc._C_OUT + objc._C_PTR + objc._C_NSBOOL,
             )
 
             # Untested...
-            CoreServices.ReadIconFromFSRef
+            # CoreServices.ReadIconFromFSRef
 
         finally:
             err = CoreServices.ReleaseIconRef(icon)
             self.assertEqual(err, 0)
 
     def testOpaque(self):
         self.assertIsOpaquePointer(CoreServices.IconRef)
```

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_intlresources.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_intlresources.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_launchservices.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_launchservices.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_lowmem.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_lowmem.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_lsinfo.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_lsinfo.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_lsopen.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_lsopen.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_lsquarantine.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_lsquarantine.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_lssharedfilelist.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_lssharedfilelist.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_macerrors.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_macerrors.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_machineexceptions.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_machineexceptions.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_maclocales.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_maclocales.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_macmemory.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_macmemory.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_math64.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_math64.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_mditem.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_mditem.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,17 +14,17 @@
         self.assertResultIsCFRetained(CoreServices.MDItemCreateWithURL)
         self.assertResultIsCFRetained(CoreServices.MDItemsCreateWithURLs)
         self.assertResultIsCFRetained(CoreServices.MDItemCopyAttribute)
         self.assertResultIsCFRetained(CoreServices.MDItemCopyAttributes)
 
         self.assertResultIsCFRetained(CoreServices.MDItemCopyAttributeNames)
 
-    @min_os_level("10.10")
+    @min_os_level("10.12")
     def test_functions10_10(self):
-        # Documented on 10.9, but not available there
+        # Documented on 10.11, but not available there
         self.assertResultIsCFRetained(CoreServices.MDItemsCopyAttributes)
 
     @expectedFailure
     def test_functions_missing(self):
         # Link error on 10.13
         self.assertIsNullTerminated(CoreServices.MDItemCopyAttributeList)
         self.assertResultIsCFRetained(CoreServices.MDItemCopyAttributeList)
```

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_mdlabel.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_mdlabel.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_mdquery.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_mdquery.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_mdschema.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_mdschema.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_mixedmode.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_mixedmode.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_multiprocessing.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_multiprocessinginfo.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_multiprocessinginfo.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_numberformatting.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_numberformatting.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_osutils.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_osutils.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_pefbinaryformat.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_pefbinaryformat.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_plstringfuncs.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_plstringfuncs.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_resources.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_resources.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_script.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_script.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_searchkit.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_searchkit.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_skanalysis.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_skanalysis.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_skdocument.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_skdocument.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_skindex.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_skindex.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_sksearch.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_sksearch.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_sksummary.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_sksummary.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_stringcompare.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_stringcompare.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_textcommon.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_textcommon.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_textencodingconvertor.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_textencodingconvertor.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_textencodingplugin.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_textencodingplugin.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_textutils.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_textutils.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_threads.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_threads.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_timer.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_timer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_toolutils.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_toolutils.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_unicodeconvertor.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_unicodeconvertor.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_unicodeutilities.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_unicodeutilities.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_utcoretypes.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_utcoretypes.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_utcutils.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_utcutils.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/PyObjCTest/test_uttype.py` & `pyobjc-framework-CoreServices-9.2/PyObjCTest/test_uttype.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/metadata/CarbonCore.fwinfo` & `pyobjc-framework-CoreServices-9.2/metadata/CarbonCore.fwinfo`

 * *Files 0% similar despite different names*

```diff
@@ -6181,14 +6181,20 @@
    "AudioRecordingChunk": { "ignore": true },
    "ApplicationSpecificChunk": { "ignore": true },
    "Comment": { "ignore": true },
    "CommentsChunk": { "ignore": true },
    "TextChunk": { "ignore": true }
   },
   "functions": {
+   "LocaleOperationCountNames": { "ignore": true },
+   "RegisterIconRefFromIconFamily": { "ignore": true },
+   "GetIconRefFromComponent": { "ignore": true },
+   "RegisterIconRefFromIconFamily": { "ignore": true },
+   "RegisterIconRefFromFSRef": { "ignore": true },
+   "ReadIconFromFSRef": { "ignore": true },
    "ConvertBundlePreLocator": { "ignore": true },
    "PBFlushVolSync": { "ignore": true },
    "PBFlushVolAsync": { "ignore": true },
    "PBHOpenDenySync": { "ignore": true },
    "PBHOpenDenyAsync": { "ignore": true },
    "PBHOpenRFDenySync": { "ignore": true },
    "PBHOpenRFDenyAsync": { "ignore": true },
```

### Comparing `pyobjc-framework-CoreServices-9.1b1/metadata/DictionaryServices.fwinfo` & `pyobjc-framework-CoreServices-9.2/metadata/DictionaryServices.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/metadata/HIServices.fwinfo` & `pyobjc-framework-CoreServices-9.2/metadata/HIServices.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/metadata/LaunchServices.fwinfo` & `pyobjc-framework-CoreServices-9.2/metadata/LaunchServices.fwinfo`

 * *Files 1% similar despite different names*

```diff
@@ -85,14 +85,15 @@
    },
    "GetIconRef": {
     "args": {
      "3": { "type_modifier": "o" }
     }
    },
    "GetIconRefFromComponent": {
+    "ignore": true,
     "args": {
      "0": {},
      "1": { "type_modifier": "o" }
     }
    },
    "GetIconRefFromFile": {
     "args": {
@@ -588,26 +589,29 @@
    "ReadIconFile": {
     "args": {
      "0": {},
      "1": {}
     }
    },
    "ReadIconFromFSRef": {
+    "ignore": true,
     "args": {
      "0": { "type_modifier": "n" },
      "1": {}
     }
    },
    "RegisterIconRefFromFSRef": {
+    "ignore": true,
     "args": {
      "2": { "type_modifier": "n" },
      "3": {}
     }
    },
    "RegisterIconRefFromIconFamily": {
+    "ignore": true,
     "args": {
      "2": {},
      "3": {}
     }
    },
    "RegisterIconRefFromIconFile": {
     "args": {
```

### Comparing `pyobjc-framework-CoreServices-9.1b1/metadata/Metadata.fwinfo` & `pyobjc-framework-CoreServices-9.2/metadata/Metadata.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/metadata/PrintCore.fwinfo` & `pyobjc-framework-CoreServices-9.2/metadata/PrintCore.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/metadata/SearchKit.fwinfo` & `pyobjc-framework-CoreServices-9.2/metadata/SearchKit.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/metadata/metadata.ini` & `pyobjc-framework-CoreServices-9.2/metadata/metadata.ini`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/metadata/raw.AE/x86_64-10.16.fwinfo` & `pyobjc-framework-CoreServices-9.2/metadata/raw.AE/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/metadata/raw.CarbonCore/arm64-12.0.fwinfo` & `pyobjc-framework-CoreServices-9.2/metadata/raw.CarbonCore/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/metadata/raw.CarbonCore/arm64-12.3.fwinfo` & `pyobjc-framework-CoreServices-9.2/metadata/raw.CarbonCore/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/metadata/raw.CarbonCore/x86_64-10.13.fwinfo` & `pyobjc-framework-CoreServices-9.2/metadata/raw.CarbonCore/x86_64-10.13.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/metadata/raw.CarbonCore/x86_64-10.15.fwinfo` & `pyobjc-framework-CoreServices-9.2/metadata/raw.CarbonCore/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/metadata/raw.CarbonCore/x86_64-10.16.fwinfo` & `pyobjc-framework-CoreServices-9.2/metadata/raw.CarbonCore/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/metadata/raw.CarbonCore/x86_64-12.0.fwinfo` & `pyobjc-framework-CoreServices-9.2/metadata/raw.CarbonCore/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/metadata/raw.CarbonCore/x86_64-12.3.fwinfo` & `pyobjc-framework-CoreServices-9.2/metadata/raw.CarbonCore/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/metadata/raw.DictionaryServices/arm64-12.0.fwinfo` & `pyobjc-framework-CoreServices-9.2/metadata/raw.DictionaryServices/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/metadata/raw.DictionaryServices/arm64-12.3.fwinfo` & `pyobjc-framework-CoreServices-9.2/metadata/raw.DictionaryServices/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/metadata/raw.DictionaryServices/x86_64-10.15.fwinfo` & `pyobjc-framework-CoreServices-9.2/metadata/raw.DictionaryServices/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/metadata/raw.DictionaryServices/x86_64-10.16.fwinfo` & `pyobjc-framework-CoreServices-9.2/metadata/raw.DictionaryServices/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/metadata/raw.DictionaryServices/x86_64-10.6.fwinfo` & `pyobjc-framework-CoreServices-9.2/metadata/raw.DictionaryServices/x86_64-10.6.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/metadata/raw.DictionaryServices/x86_64-10.7.fwinfo` & `pyobjc-framework-CoreServices-9.2/metadata/raw.DictionaryServices/x86_64-10.7.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/metadata/raw.DictionaryServices/x86_64-10.8.fwinfo` & `pyobjc-framework-CoreServices-9.2/metadata/raw.DictionaryServices/x86_64-10.8.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/metadata/raw.DictionaryServices/x86_64-12.0.fwinfo` & `pyobjc-framework-CoreServices-9.2/metadata/raw.DictionaryServices/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/metadata/raw.DictionaryServices/x86_64-12.3.fwinfo` & `pyobjc-framework-CoreServices-9.2/metadata/raw.DictionaryServices/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/metadata/raw.LaunchServices/arm64-12.0.fwinfo` & `pyobjc-framework-CoreServices-9.2/metadata/raw.LaunchServices/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/metadata/raw.LaunchServices/arm64-12.3.fwinfo` & `pyobjc-framework-CoreServices-9.2/metadata/raw.LaunchServices/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/metadata/raw.LaunchServices/arm64-13.0.fwinfo` & `pyobjc-framework-CoreServices-9.2/metadata/raw.LaunchServices/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/metadata/raw.LaunchServices/x86_64-10.10.fwinfo` & `pyobjc-framework-CoreServices-9.2/metadata/raw.LaunchServices/x86_64-10.10.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/metadata/raw.LaunchServices/x86_64-10.15.fwinfo` & `pyobjc-framework-CoreServices-9.2/metadata/raw.LaunchServices/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/metadata/raw.LaunchServices/x86_64-10.16.fwinfo` & `pyobjc-framework-CoreServices-9.2/metadata/raw.LaunchServices/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/metadata/raw.LaunchServices/x86_64-10.6.fwinfo` & `pyobjc-framework-CoreServices-9.2/metadata/raw.LaunchServices/x86_64-10.6.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/metadata/raw.LaunchServices/x86_64-10.7.fwinfo` & `pyobjc-framework-CoreServices-9.2/metadata/raw.LaunchServices/x86_64-10.7.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/metadata/raw.LaunchServices/x86_64-10.8.fwinfo` & `pyobjc-framework-CoreServices-9.2/metadata/raw.LaunchServices/x86_64-10.8.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/metadata/raw.LaunchServices/x86_64-12.0.fwinfo` & `pyobjc-framework-CoreServices-9.2/metadata/raw.LaunchServices/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/metadata/raw.LaunchServices/x86_64-12.3.fwinfo` & `pyobjc-framework-CoreServices-9.2/metadata/raw.LaunchServices/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/metadata/raw.LaunchServices/x86_64-13.0.fwinfo` & `pyobjc-framework-CoreServices-9.2/metadata/raw.LaunchServices/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/metadata/raw.Metadata/arm64-12.0.fwinfo` & `pyobjc-framework-CoreServices-9.2/metadata/raw.Metadata/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/metadata/raw.Metadata/arm64-12.3.fwinfo` & `pyobjc-framework-CoreServices-9.2/metadata/raw.Metadata/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/metadata/raw.Metadata/x86_64-10.13.fwinfo` & `pyobjc-framework-CoreServices-9.2/metadata/raw.Metadata/x86_64-10.13.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/metadata/raw.Metadata/x86_64-10.15.fwinfo` & `pyobjc-framework-CoreServices-9.2/metadata/raw.Metadata/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/metadata/raw.Metadata/x86_64-10.16.fwinfo` & `pyobjc-framework-CoreServices-9.2/metadata/raw.Metadata/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/metadata/raw.Metadata/x86_64-12.0.fwinfo` & `pyobjc-framework-CoreServices-9.2/metadata/raw.Metadata/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/metadata/raw.Metadata/x86_64-12.3.fwinfo` & `pyobjc-framework-CoreServices-9.2/metadata/raw.Metadata/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/metadata/raw.SearchKit/arm64-12.0.fwinfo` & `pyobjc-framework-CoreServices-9.2/metadata/raw.SearchKit/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/metadata/raw.SearchKit/arm64-12.3.fwinfo` & `pyobjc-framework-CoreServices-9.2/metadata/raw.SearchKit/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/metadata/raw.SearchKit/x86_64-10.15.fwinfo` & `pyobjc-framework-CoreServices-9.2/metadata/raw.SearchKit/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/metadata/raw.SearchKit/x86_64-10.16.fwinfo` & `pyobjc-framework-CoreServices-9.2/metadata/raw.SearchKit/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/metadata/raw.SearchKit/x86_64-10.6.fwinfo` & `pyobjc-framework-CoreServices-9.2/metadata/raw.SearchKit/x86_64-10.6.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/metadata/raw.SearchKit/x86_64-10.7.fwinfo` & `pyobjc-framework-CoreServices-9.2/metadata/raw.SearchKit/x86_64-10.7.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/metadata/raw.SearchKit/x86_64-10.8.fwinfo` & `pyobjc-framework-CoreServices-9.2/metadata/raw.SearchKit/x86_64-10.8.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/metadata/raw.SearchKit/x86_64-12.0.fwinfo` & `pyobjc-framework-CoreServices-9.2/metadata/raw.SearchKit/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/metadata/raw.SearchKit/x86_64-12.3.fwinfo` & `pyobjc-framework-CoreServices-9.2/metadata/raw.SearchKit/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/pyobjc_setup.py` & `pyobjc-framework-CoreServices-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreServices-9.1b1/setup.py` & `pyobjc-framework-CoreServices-9.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,18 +3,22 @@
 
 These wrappers don't include documentation, please check Apple's documentation
 for information on how to use this framework and PyObjC's documentation
 for general tips and tricks regarding the translation between Python
 and (Objective-)C frameworks
 """
 import os
+import sys
 
-from pyobjc_setup import Extension, setup
+sys.path.insert(0, os.path.dirname(__file__))
 
-VERSION = "9.1b1"
+
+from pyobjc_setup import Extension, setup  # noqa: E402
+
+VERSION = "9.2"
 
 subpackages = [
     f"CoreServices.{fn}"
     for fn in os.listdir("Lib/CoreServices")
     if os.path.exists(os.path.join("Lib/CoreServices", fn, "__init__.py"))
 ]
```

