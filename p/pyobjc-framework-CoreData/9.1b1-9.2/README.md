# Comparing `tmp/pyobjc-framework-CoreData-9.1b1.tar.gz` & `tmp/pyobjc-framework-CoreData-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-CoreData-9.1b1.tar", last modified: Sun Mar 26 11:20:17 2023, max compression
+gzip compressed data, was "pyobjc-framework-CoreData-9.2.tar", last modified: Wed Jun  7 00:10:17 2023, max compression
```

## Comparing `pyobjc-framework-CoreData-9.1b1.tar` & `pyobjc-framework-CoreData-9.2.tar`

### file list

```diff
@@ -1,114 +1,115 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:20:17.383093 pyobjc-framework-CoreData-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:20:17.084576 pyobjc-framework-CoreData-9.1b1/Examples/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:20:17.120739 pyobjc-framework-CoreData-9.1b1/Examples/DragApp/
--rw-r--r--   0 ronald     (501) staff       (20)     4664 2021-03-21 10:08:22.000000 pyobjc-framework-CoreData-9.1b1/Examples/DragApp/DragAppAppDelegate.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:20:17.144754 pyobjc-framework-CoreData-9.1b1/Examples/DragApp/DragApp_DataModel.xcdatamodel/
--rw-r--r--   0 ronald     (501) staff       (20)    10486 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.1b1/Examples/DragApp/DragApp_DataModel.xcdatamodel/elements
--rw-r--r--   0 ronald     (501) staff       (20)     6831 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.1b1/Examples/DragApp/DragApp_DataModel.xcdatamodel/layout
--rw-r--r--   0 ronald     (501) staff       (20)     6153 2023-03-03 17:21:59.000000 pyobjc-framework-CoreData-9.1b1/Examples/DragApp/DragSupportDataSource.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:20:17.084383 pyobjc-framework-CoreData-9.1b1/Examples/DragApp/English.lproj/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:20:17.150383 pyobjc-framework-CoreData-9.1b1/Examples/DragApp/English.lproj/MainMenu.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      448 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.1b1/Examples/DragApp/English.lproj/MainMenu.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      749 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.1b1/Examples/DragApp/English.lproj/MainMenu.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)   182753 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.1b1/Examples/DragApp/English.lproj/MainMenu.nib/keyedobjects.nib
--rw-r--r--   0 ronald     (501) staff       (20)     1372 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.1b1/Examples/DragApp/ReadMe.txt
--rw-r--r--   0 ronald     (501) staff       (20)      174 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.1b1/Examples/DragApp/main.py
--rw-r--r--   0 ronald     (501) staff       (20)      352 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.1b1/Examples/DragApp/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       95 2021-10-18 19:38:40.000000 pyobjc-framework-CoreData-9.1b1/Examples/DragApp/summary.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:20:17.175450 pyobjc-framework-CoreData-9.1b1/Examples/OutlineEdit/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:20:17.176396 pyobjc-framework-CoreData-9.1b1/Examples/OutlineEdit/English.lproj/
--rw-r--r--   0 ronald     (501) staff       (20)      266 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.1b1/Examples/OutlineEdit/English.lproj/InfoPlist.strings
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:20:17.178225 pyobjc-framework-CoreData-9.1b1/Examples/OutlineEdit/English.lproj/MainMenu.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      267 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.1b1/Examples/OutlineEdit/English.lproj/MainMenu.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      611 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.1b1/Examples/OutlineEdit/English.lproj/MainMenu.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)    14311 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.1b1/Examples/OutlineEdit/English.lproj/MainMenu.nib/keyedobjects.nib
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:20:17.179918 pyobjc-framework-CoreData-9.1b1/Examples/OutlineEdit/English.lproj/MyDocument.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      503 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.1b1/Examples/OutlineEdit/English.lproj/MyDocument.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      497 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.1b1/Examples/OutlineEdit/English.lproj/MyDocument.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)    11603 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.1b1/Examples/OutlineEdit/English.lproj/MyDocument.nib/keyedobjects.nib
--rw-r--r--   0 ronald     (501) staff       (20)     2828 2021-07-30 09:00:37.000000 pyobjc-framework-CoreData-9.1b1/Examples/OutlineEdit/MyDocument.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:20:17.180961 pyobjc-framework-CoreData-9.1b1/Examples/OutlineEdit/MyDocument.xcdatamodel/
--rw-r--r--   0 ronald     (501) staff       (20)    13467 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.1b1/Examples/OutlineEdit/MyDocument.xcdatamodel/elements
--rw-r--r--   0 ronald     (501) staff       (20)     7658 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.1b1/Examples/OutlineEdit/MyDocument.xcdatamodel/layout
--rw-r--r--   0 ronald     (501) staff       (20)      248 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.1b1/Examples/OutlineEdit/Note.py
--rw-r--r--   0 ronald     (501) staff       (20)      149 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.1b1/Examples/OutlineEdit/main.py
--rw-r--r--   0 ronald     (501) staff       (20)     1516 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.1b1/Examples/OutlineEdit/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       76 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.1b1/Examples/OutlineEdit/summary.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-CoreData-9.1b1/LICENSE.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:20:17.091947 pyobjc-framework-CoreData-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:20:17.183228 pyobjc-framework-CoreData-9.1b1/Lib/CoreData/
--rw-r--r--   0 ronald     (501) staff       (20)      794 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.1b1/Lib/CoreData/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     1749 2023-03-04 11:01:05.000000 pyobjc-framework-CoreData-9.1b1/Lib/CoreData/_convenience.py
--rw-r--r--   0 ronald     (501) staff       (20)    43576 2023-02-19 10:50:35.000000 pyobjc-framework-CoreData-9.1b1/Lib/CoreData/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:20:17.190853 pyobjc-framework-CoreData-9.1b1/Lib/pyobjc_framework_CoreData.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2291 2023-03-26 11:20:17.000000 pyobjc-framework-CoreData-9.1b1/Lib/pyobjc_framework_CoreData.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     3732 2023-03-26 11:20:17.000000 pyobjc-framework-CoreData-9.1b1/Lib/pyobjc_framework_CoreData.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:20:16.000000 pyobjc-framework-CoreData-9.1b1/Lib/pyobjc_framework_CoreData.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:44.000000 pyobjc-framework-CoreData-9.1b1/Lib/pyobjc_framework_CoreData.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:20:16.000000 pyobjc-framework-CoreData-9.1b1/Lib/pyobjc_framework_CoreData.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)        9 2023-03-26 11:20:16.000000 pyobjc-framework-CoreData-9.1b1/Lib/pyobjc_framework_CoreData.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:20:17.195696 pyobjc-framework-CoreData-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)     1036 2021-10-18 19:38:40.000000 pyobjc-framework-CoreData-9.1b1/Modules/_CoreData.m
--rw-r--r--   0 ronald     (501) staff       (20)      312 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.1b1/Modules/_CoreData_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:33.000000 pyobjc-framework-CoreData-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-02-19 12:24:44.000000 pyobjc-framework-CoreData-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     2080 2023-03-26 11:20:17.382492 pyobjc-framework-CoreData-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:20:17.287785 pyobjc-framework-CoreData-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     1247 2022-04-11 08:03:15.000000 pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_coredata.py
--rw-r--r--   0 ronald     (501) staff       (20)     1794 2021-03-21 10:08:22.000000 pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_coredatadefines.py
--rw-r--r--   0 ronald     (501) staff       (20)     4538 2021-03-21 10:08:22.000000 pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_coredataerrors.py
--rw-r--r--   0 ronald     (501) staff       (20)     5985 2023-03-25 14:06:55.000000 pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_managedkvo.py
--rw-r--r--   0 ronald     (501) staff       (20)      411 2021-03-21 10:08:22.000000 pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_nsatomicstore.py
--rw-r--r--   0 ronald     (501) staff       (20)     2174 2022-02-24 08:47:16.000000 pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_nsattributedescription.py
--rw-r--r--   0 ronald     (501) staff       (20)     1531 2021-07-30 09:00:37.000000 pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_nsbatchinsertrequest.py
--rw-r--r--   0 ronald     (501) staff       (20)      343 2021-03-21 10:08:22.000000 pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_nsbatchupdaterequest.py
--rw-r--r--   0 ronald     (501) staff       (20)     1037 2021-10-29 07:58:20.000000 pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_nscoredatacorespotlightdelegate.py
--rw-r--r--   0 ronald     (501) staff       (20)      429 2021-03-21 10:08:22.000000 pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_nsentitydescription.py
--rw-r--r--   0 ronald     (501) staff       (20)      624 2022-02-24 08:47:16.000000 pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_nsentitymapping.py
--rw-r--r--   0 ronald     (501) staff       (20)     2705 2021-03-21 10:08:22.000000 pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_nsentitymigrationpolicy.py
--rw-r--r--   0 ronald     (501) staff       (20)     1826 2022-06-25 20:17:38.000000 pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_nsfetchedresultscontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)      616 2022-02-24 08:47:16.000000 pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_nsfetchindexelementdescription.py
--rw-r--r--   0 ronald     (501) staff       (20)     1889 2022-02-24 08:47:16.000000 pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_nsfetchrequest.py
--rw-r--r--   0 ronald     (501) staff       (20)      513 2021-03-21 10:08:22.000000 pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_nsfetchrequestexpression.py
--rw-r--r--   0 ronald     (501) staff       (20)      837 2021-03-21 10:08:22.000000 pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_nsincrementalstore.py
--rw-r--r--   0 ronald     (501) staff       (20)     2338 2022-02-24 08:47:16.000000 pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_nsmanagedobject.py
--rw-r--r--   0 ronald     (501) staff       (20)     5373 2022-02-24 08:47:16.000000 pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_nsmanagedobjectcontext.py
--rw-r--r--   0 ronald     (501) staff       (20)      203 2021-03-21 10:08:22.000000 pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_nsmanagedobjectid.py
--rw-r--r--   0 ronald     (501) staff       (20)      302 2021-03-21 10:08:22.000000 pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_nsmanagedobjectmodel.py
--rw-r--r--   0 ronald     (501) staff       (20)      320 2021-03-21 10:08:22.000000 pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_nsmappingmodel.py
--rw-r--r--   0 ronald     (501) staff       (20)     1819 2022-02-24 08:47:16.000000 pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_nsmergepolicy.py
--rw-r--r--   0 ronald     (501) staff       (20)      890 2021-03-21 10:08:22.000000 pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_nsmigrationmanager.py
--rw-r--r--   0 ronald     (501) staff       (20)     1515 2022-10-18 09:53:24.000000 pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_nspersistentcloudKitcontainer.py
--rw-r--r--   0 ronald     (501) staff       (20)      817 2022-10-18 09:53:24.000000 pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_nspersistentcloudKitcontainerevent.py
--rw-r--r--   0 ronald     (501) staff       (20)     1416 2021-10-27 10:34:05.000000 pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_nspersistentcloudkitcontainer_sharing.py
--rw-r--r--   0 ronald     (501) staff       (20)      453 2021-03-21 10:08:22.000000 pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_nspersistentcontainer.py
--rw-r--r--   0 ronald     (501) staff       (20)      349 2021-03-21 10:08:22.000000 pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_nspersistenthistorychange.py
--rw-r--r--   0 ronald     (501) staff       (20)      893 2021-03-21 10:08:22.000000 pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_nspersistentstore.py
--rw-r--r--   0 ronald     (501) staff       (20)     9440 2022-02-24 08:47:16.000000 pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_nspersistentstorecoordinator.py
--rw-r--r--   0 ronald     (501) staff       (20)     1129 2021-03-21 10:08:22.000000 pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_nspersistentstoredescription.py
--rw-r--r--   0 ronald     (501) staff       (20)      892 2022-02-24 08:47:16.000000 pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_nspersistentstorerequest.py
--rw-r--r--   0 ronald     (501) staff       (20)     1906 2022-02-24 08:47:16.000000 pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_nspersistentstoreresult.py
--rw-r--r--   0 ronald     (501) staff       (20)     1094 2021-03-21 10:08:22.000000 pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_nspropertydescription.py
--rw-r--r--   0 ronald     (501) staff       (20)      789 2022-02-24 08:47:16.000000 pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_nsrelationshipdescription.py
--rw-r--r--   0 ronald     (501) staff       (20)      285 2021-10-18 19:38:40.000000 pyobjc-framework-CoreData-9.1b1/README.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:20:17.317476 pyobjc-framework-CoreData-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)    31168 2021-07-31 12:26:28.000000 pyobjc-framework-CoreData-9.1b1/metadata/CoreData.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       32 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:20:17.378807 pyobjc-framework-CoreData-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)   266508 2021-07-30 09:00:37.000000 pyobjc-framework-CoreData-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   267665 2022-02-24 08:47:16.000000 pyobjc-framework-CoreData-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   269193 2023-02-19 10:50:35.000000 pyobjc-framework-CoreData-9.1b1/metadata/raw/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   165470 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.1b1/metadata/raw/x86_64-10.10.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   245523 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.1b1/metadata/raw/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   263934 2021-03-21 10:08:22.000000 pyobjc-framework-CoreData-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   105640 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.1b1/metadata/raw/x86_64-10.6.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   125070 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.1b1/metadata/raw/x86_64-10.7.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   125868 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.1b1/metadata/raw/x86_64-10.8.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   266509 2021-07-30 09:00:37.000000 pyobjc-framework-CoreData-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   267666 2022-02-24 08:47:16.000000 pyobjc-framework-CoreData-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   269194 2023-02-19 10:50:35.000000 pyobjc-framework-CoreData-9.1b1/metadata/raw/x86_64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-CoreData-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:20:17.383230 pyobjc-framework-CoreData-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1273 2023-03-25 14:20:30.000000 pyobjc-framework-CoreData-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:10:17.905442 pyobjc-framework-CoreData-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:10:17.756405 pyobjc-framework-CoreData-9.2/Examples/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:10:17.779572 pyobjc-framework-CoreData-9.2/Examples/DragApp/
+-rw-r--r--   0 ronald     (501) staff       (20)     4664 2021-03-21 10:08:22.000000 pyobjc-framework-CoreData-9.2/Examples/DragApp/DragAppAppDelegate.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:10:17.781481 pyobjc-framework-CoreData-9.2/Examples/DragApp/DragApp_DataModel.xcdatamodel/
+-rw-r--r--   0 ronald     (501) staff       (20)    10486 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.2/Examples/DragApp/DragApp_DataModel.xcdatamodel/elements
+-rw-r--r--   0 ronald     (501) staff       (20)     6831 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.2/Examples/DragApp/DragApp_DataModel.xcdatamodel/layout
+-rw-r--r--   0 ronald     (501) staff       (20)     6153 2023-03-03 17:21:59.000000 pyobjc-framework-CoreData-9.2/Examples/DragApp/DragSupportDataSource.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:10:17.756217 pyobjc-framework-CoreData-9.2/Examples/DragApp/English.lproj/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:10:17.784622 pyobjc-framework-CoreData-9.2/Examples/DragApp/English.lproj/MainMenu.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      448 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.2/Examples/DragApp/English.lproj/MainMenu.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      749 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.2/Examples/DragApp/English.lproj/MainMenu.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)   182753 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.2/Examples/DragApp/English.lproj/MainMenu.nib/keyedobjects.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     1372 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.2/Examples/DragApp/ReadMe.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      174 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.2/Examples/DragApp/main.py
+-rw-r--r--   0 ronald     (501) staff       (20)      352 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.2/Examples/DragApp/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       95 2021-10-18 19:38:40.000000 pyobjc-framework-CoreData-9.2/Examples/DragApp/summary.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:10:17.795847 pyobjc-framework-CoreData-9.2/Examples/OutlineEdit/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:10:17.796718 pyobjc-framework-CoreData-9.2/Examples/OutlineEdit/English.lproj/
+-rw-r--r--   0 ronald     (501) staff       (20)      266 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.2/Examples/OutlineEdit/English.lproj/InfoPlist.strings
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:10:17.799254 pyobjc-framework-CoreData-9.2/Examples/OutlineEdit/English.lproj/MainMenu.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      267 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.2/Examples/OutlineEdit/English.lproj/MainMenu.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      611 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.2/Examples/OutlineEdit/English.lproj/MainMenu.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)    14311 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.2/Examples/OutlineEdit/English.lproj/MainMenu.nib/keyedobjects.nib
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:10:17.801267 pyobjc-framework-CoreData-9.2/Examples/OutlineEdit/English.lproj/MyDocument.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      503 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.2/Examples/OutlineEdit/English.lproj/MyDocument.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      497 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.2/Examples/OutlineEdit/English.lproj/MyDocument.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)    11603 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.2/Examples/OutlineEdit/English.lproj/MyDocument.nib/keyedobjects.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     2828 2021-07-30 09:00:37.000000 pyobjc-framework-CoreData-9.2/Examples/OutlineEdit/MyDocument.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:10:17.802527 pyobjc-framework-CoreData-9.2/Examples/OutlineEdit/MyDocument.xcdatamodel/
+-rw-r--r--   0 ronald     (501) staff       (20)    13467 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.2/Examples/OutlineEdit/MyDocument.xcdatamodel/elements
+-rw-r--r--   0 ronald     (501) staff       (20)     7658 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.2/Examples/OutlineEdit/MyDocument.xcdatamodel/layout
+-rw-r--r--   0 ronald     (501) staff       (20)      248 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.2/Examples/OutlineEdit/Note.py
+-rw-r--r--   0 ronald     (501) staff       (20)      149 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.2/Examples/OutlineEdit/main.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1516 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.2/Examples/OutlineEdit/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       76 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.2/Examples/OutlineEdit/summary.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-CoreData-9.2/LICENSE.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:10:17.757879 pyobjc-framework-CoreData-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:10:17.804661 pyobjc-framework-CoreData-9.2/Lib/CoreData/
+-rw-r--r--   0 ronald     (501) staff       (20)      794 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.2/Lib/CoreData/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1749 2023-03-04 11:01:05.000000 pyobjc-framework-CoreData-9.2/Lib/CoreData/_convenience.py
+-rw-r--r--   0 ronald     (501) staff       (20)    43576 2023-02-19 10:50:35.000000 pyobjc-framework-CoreData-9.2/Lib/CoreData/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:10:17.808578 pyobjc-framework-CoreData-9.2/Lib/pyobjc_framework_CoreData.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2289 2023-06-07 00:10:17.000000 pyobjc-framework-CoreData-9.2/Lib/pyobjc_framework_CoreData.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     3747 2023-06-07 00:10:17.000000 pyobjc-framework-CoreData-9.2/Lib/pyobjc_framework_CoreData.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:10:17.000000 pyobjc-framework-CoreData-9.2/Lib/pyobjc_framework_CoreData.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:44.000000 pyobjc-framework-CoreData-9.2/Lib/pyobjc_framework_CoreData.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:10:17.000000 pyobjc-framework-CoreData-9.2/Lib/pyobjc_framework_CoreData.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        9 2023-06-07 00:10:17.000000 pyobjc-framework-CoreData-9.2/Lib/pyobjc_framework_CoreData.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:10:17.821530 pyobjc-framework-CoreData-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)     1036 2021-10-18 19:38:40.000000 pyobjc-framework-CoreData-9.2/Modules/_CoreData.m
+-rw-r--r--   0 ronald     (501) staff       (20)      312 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.2/Modules/_CoreData_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:33.000000 pyobjc-framework-CoreData-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-05-29 07:18:42.000000 pyobjc-framework-CoreData-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     2078 2023-06-07 00:10:17.905044 pyobjc-framework-CoreData-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:10:17.860550 pyobjc-framework-CoreData-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1247 2022-04-11 08:03:15.000000 pyobjc-framework-CoreData-9.2/PyObjCTest/test_coredata.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1794 2021-03-21 10:08:22.000000 pyobjc-framework-CoreData-9.2/PyObjCTest/test_coredatadefines.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4538 2021-03-21 10:08:22.000000 pyobjc-framework-CoreData-9.2/PyObjCTest/test_coredataerrors.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6008 2023-05-27 09:46:33.000000 pyobjc-framework-CoreData-9.2/PyObjCTest/test_managedkvo.py
+-rw-r--r--   0 ronald     (501) staff       (20)      411 2021-03-21 10:08:22.000000 pyobjc-framework-CoreData-9.2/PyObjCTest/test_nsatomicstore.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2174 2022-02-24 08:47:16.000000 pyobjc-framework-CoreData-9.2/PyObjCTest/test_nsattributedescription.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1531 2021-07-30 09:00:37.000000 pyobjc-framework-CoreData-9.2/PyObjCTest/test_nsbatchinsertrequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)      343 2021-03-21 10:08:22.000000 pyobjc-framework-CoreData-9.2/PyObjCTest/test_nsbatchupdaterequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1037 2021-10-29 07:58:20.000000 pyobjc-framework-CoreData-9.2/PyObjCTest/test_nscoredatacorespotlightdelegate.py
+-rw-r--r--   0 ronald     (501) staff       (20)      429 2021-03-21 10:08:22.000000 pyobjc-framework-CoreData-9.2/PyObjCTest/test_nsentitydescription.py
+-rw-r--r--   0 ronald     (501) staff       (20)      624 2022-02-24 08:47:16.000000 pyobjc-framework-CoreData-9.2/PyObjCTest/test_nsentitymapping.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2705 2021-03-21 10:08:22.000000 pyobjc-framework-CoreData-9.2/PyObjCTest/test_nsentitymigrationpolicy.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1826 2022-06-25 20:17:38.000000 pyobjc-framework-CoreData-9.2/PyObjCTest/test_nsfetchedresultscontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)      616 2022-02-24 08:47:16.000000 pyobjc-framework-CoreData-9.2/PyObjCTest/test_nsfetchindexelementdescription.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1889 2022-02-24 08:47:16.000000 pyobjc-framework-CoreData-9.2/PyObjCTest/test_nsfetchrequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)      513 2021-03-21 10:08:22.000000 pyobjc-framework-CoreData-9.2/PyObjCTest/test_nsfetchrequestexpression.py
+-rw-r--r--   0 ronald     (501) staff       (20)      837 2021-03-21 10:08:22.000000 pyobjc-framework-CoreData-9.2/PyObjCTest/test_nsincrementalstore.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2338 2022-02-24 08:47:16.000000 pyobjc-framework-CoreData-9.2/PyObjCTest/test_nsmanagedobject.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5373 2022-02-24 08:47:16.000000 pyobjc-framework-CoreData-9.2/PyObjCTest/test_nsmanagedobjectcontext.py
+-rw-r--r--   0 ronald     (501) staff       (20)      203 2021-03-21 10:08:22.000000 pyobjc-framework-CoreData-9.2/PyObjCTest/test_nsmanagedobjectid.py
+-rw-r--r--   0 ronald     (501) staff       (20)      302 2021-03-21 10:08:22.000000 pyobjc-framework-CoreData-9.2/PyObjCTest/test_nsmanagedobjectmodel.py
+-rw-r--r--   0 ronald     (501) staff       (20)      320 2021-03-21 10:08:22.000000 pyobjc-framework-CoreData-9.2/PyObjCTest/test_nsmappingmodel.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1819 2022-02-24 08:47:16.000000 pyobjc-framework-CoreData-9.2/PyObjCTest/test_nsmergepolicy.py
+-rw-r--r--   0 ronald     (501) staff       (20)      890 2021-03-21 10:08:22.000000 pyobjc-framework-CoreData-9.2/PyObjCTest/test_nsmigrationmanager.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1515 2022-10-18 09:53:24.000000 pyobjc-framework-CoreData-9.2/PyObjCTest/test_nspersistentcloudKitcontainer.py
+-rw-r--r--   0 ronald     (501) staff       (20)      817 2022-10-18 09:53:24.000000 pyobjc-framework-CoreData-9.2/PyObjCTest/test_nspersistentcloudKitcontainerevent.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1416 2021-10-27 10:34:05.000000 pyobjc-framework-CoreData-9.2/PyObjCTest/test_nspersistentcloudkitcontainer_sharing.py
+-rw-r--r--   0 ronald     (501) staff       (20)      453 2021-03-21 10:08:22.000000 pyobjc-framework-CoreData-9.2/PyObjCTest/test_nspersistentcontainer.py
+-rw-r--r--   0 ronald     (501) staff       (20)      349 2021-03-21 10:08:22.000000 pyobjc-framework-CoreData-9.2/PyObjCTest/test_nspersistenthistorychange.py
+-rw-r--r--   0 ronald     (501) staff       (20)      893 2021-03-21 10:08:22.000000 pyobjc-framework-CoreData-9.2/PyObjCTest/test_nspersistentstore.py
+-rw-r--r--   0 ronald     (501) staff       (20)     9440 2022-02-24 08:47:16.000000 pyobjc-framework-CoreData-9.2/PyObjCTest/test_nspersistentstorecoordinator.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1129 2021-03-21 10:08:22.000000 pyobjc-framework-CoreData-9.2/PyObjCTest/test_nspersistentstoredescription.py
+-rw-r--r--   0 ronald     (501) staff       (20)      892 2022-02-24 08:47:16.000000 pyobjc-framework-CoreData-9.2/PyObjCTest/test_nspersistentstorerequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1906 2022-02-24 08:47:16.000000 pyobjc-framework-CoreData-9.2/PyObjCTest/test_nspersistentstoreresult.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1094 2021-03-21 10:08:22.000000 pyobjc-framework-CoreData-9.2/PyObjCTest/test_nspropertydescription.py
+-rw-r--r--   0 ronald     (501) staff       (20)      789 2022-02-24 08:47:16.000000 pyobjc-framework-CoreData-9.2/PyObjCTest/test_nsrelationshipdescription.py
+-rw-r--r--   0 ronald     (501) staff       (20)      285 2021-10-18 19:38:40.000000 pyobjc-framework-CoreData-9.2/README.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:10:17.877770 pyobjc-framework-CoreData-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)    31168 2021-07-31 12:26:28.000000 pyobjc-framework-CoreData-9.2/metadata/CoreData.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       32 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:10:17.902964 pyobjc-framework-CoreData-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)   266508 2021-07-30 09:00:37.000000 pyobjc-framework-CoreData-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   267665 2022-02-24 08:47:16.000000 pyobjc-framework-CoreData-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   269193 2023-02-19 10:50:35.000000 pyobjc-framework-CoreData-9.2/metadata/raw/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   165470 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.2/metadata/raw/x86_64-10.10.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   245523 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.2/metadata/raw/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   263934 2021-03-21 10:08:22.000000 pyobjc-framework-CoreData-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   105640 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.2/metadata/raw/x86_64-10.6.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   125070 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.2/metadata/raw/x86_64-10.7.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   125868 2020-11-30 18:45:14.000000 pyobjc-framework-CoreData-9.2/metadata/raw/x86_64-10.8.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   266509 2021-07-30 09:00:37.000000 pyobjc-framework-CoreData-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   267666 2022-02-24 08:47:16.000000 pyobjc-framework-CoreData-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   269194 2023-02-19 10:50:35.000000 pyobjc-framework-CoreData-9.2/metadata/raw/x86_64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-CoreData-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-CoreData-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:10:17.905776 pyobjc-framework-CoreData-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1344 2023-05-29 10:07:45.000000 pyobjc-framework-CoreData-9.2/setup.py
```

### Comparing `pyobjc-framework-CoreData-9.1b1/Examples/DragApp/DragAppAppDelegate.py` & `pyobjc-framework-CoreData-9.2/Examples/DragApp/DragAppAppDelegate.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/Examples/DragApp/DragApp_DataModel.xcdatamodel/elements` & `pyobjc-framework-CoreData-9.2/Examples/DragApp/DragApp_DataModel.xcdatamodel/elements`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/Examples/DragApp/DragApp_DataModel.xcdatamodel/layout` & `pyobjc-framework-CoreData-9.2/Examples/DragApp/DragApp_DataModel.xcdatamodel/layout`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/Examples/DragApp/DragSupportDataSource.py` & `pyobjc-framework-CoreData-9.2/Examples/DragApp/DragSupportDataSource.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/Examples/DragApp/English.lproj/MainMenu.nib/info.nib` & `pyobjc-framework-CoreData-9.2/Examples/DragApp/English.lproj/MainMenu.nib/info.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/Examples/DragApp/English.lproj/MainMenu.nib/keyedobjects.nib` & `pyobjc-framework-CoreData-9.2/Examples/DragApp/English.lproj/MainMenu.nib/keyedobjects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/Examples/DragApp/ReadMe.txt` & `pyobjc-framework-CoreData-9.2/Examples/DragApp/ReadMe.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/Examples/OutlineEdit/English.lproj/MainMenu.nib/info.nib` & `pyobjc-framework-CoreData-9.2/Examples/OutlineEdit/English.lproj/MainMenu.nib/info.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/Examples/OutlineEdit/English.lproj/MainMenu.nib/keyedobjects.nib` & `pyobjc-framework-CoreData-9.2/Examples/OutlineEdit/English.lproj/MainMenu.nib/keyedobjects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/Examples/OutlineEdit/English.lproj/MyDocument.nib/keyedobjects.nib` & `pyobjc-framework-CoreData-9.2/Examples/OutlineEdit/English.lproj/MyDocument.nib/keyedobjects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/Examples/OutlineEdit/MyDocument.py` & `pyobjc-framework-CoreData-9.2/Examples/OutlineEdit/MyDocument.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/Examples/OutlineEdit/MyDocument.xcdatamodel/elements` & `pyobjc-framework-CoreData-9.2/Examples/OutlineEdit/MyDocument.xcdatamodel/elements`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/Examples/OutlineEdit/MyDocument.xcdatamodel/layout` & `pyobjc-framework-CoreData-9.2/Examples/OutlineEdit/MyDocument.xcdatamodel/layout`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/Examples/OutlineEdit/setup.py` & `pyobjc-framework-CoreData-9.2/Examples/OutlineEdit/setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/LICENSE.txt` & `pyobjc-framework-CoreData-9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/Lib/CoreData/__init__.py` & `pyobjc-framework-CoreData-9.2/Lib/CoreData/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/Lib/CoreData/_convenience.py` & `pyobjc-framework-CoreData-9.2/Lib/CoreData/_convenience.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/Lib/CoreData/_metadata.py` & `pyobjc-framework-CoreData-9.2/Lib/CoreData/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/Lib/pyobjc_framework_CoreData.egg-info/PKG-INFO` & `pyobjc-framework-CoreData-9.2/Lib/pyobjc_framework_CoreData.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-CoreData
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework CoreData on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,CoreData
 Platform: MacOS X
```

### Comparing `pyobjc-framework-CoreData-9.1b1/Lib/pyobjc_framework_CoreData.egg-info/SOURCES.txt` & `pyobjc-framework-CoreData-9.2/Lib/pyobjc_framework_CoreData.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE.txt
 MANIFEST.in
 README.txt
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Examples/DragApp/DragAppAppDelegate.py
 Examples/DragApp/DragSupportDataSource.py
 Examples/DragApp/ReadMe.txt
 Examples/DragApp/main.py
 Examples/DragApp/setup.py
 Examples/DragApp/summary.txt
```

### Comparing `pyobjc-framework-CoreData-9.1b1/Modules/_CoreData.m` & `pyobjc-framework-CoreData-9.2/Modules/_CoreData.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-CoreData-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-CoreData-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-CoreData-9.1b1/PKG-INFO` & `pyobjc-framework-CoreData-9.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-CoreData
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework CoreData on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,CoreData
 Platform: MacOS X
```

### Comparing `pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_coredata.py` & `pyobjc-framework-CoreData-9.2/PyObjCTest/test_coredata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_coredatadefines.py` & `pyobjc-framework-CoreData-9.2/PyObjCTest/test_coredatadefines.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_coredataerrors.py` & `pyobjc-framework-CoreData-9.2/PyObjCTest/test_coredataerrors.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_managedkvo.py` & `pyobjc-framework-CoreData-9.2/PyObjCTest/test_managedkvo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #! /usr/bin/python
 
 import CoreData
 import Foundation
+from objc import super
 from PyObjCTools.TestSupport import TestCase
 
 
 class CoreDataTestObject(CoreData.NSManagedObject):
     def __getattr__(self, k):
         raise AttributeError(k)
```

### Comparing `pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_nsattributedescription.py` & `pyobjc-framework-CoreData-9.2/PyObjCTest/test_nsattributedescription.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_nsbatchinsertrequest.py` & `pyobjc-framework-CoreData-9.2/PyObjCTest/test_nsbatchinsertrequest.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_nscoredatacorespotlightdelegate.py` & `pyobjc-framework-CoreData-9.2/PyObjCTest/test_nscoredatacorespotlightdelegate.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_nsentitymapping.py` & `pyobjc-framework-CoreData-9.2/PyObjCTest/test_nsentitymapping.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_nsentitymigrationpolicy.py` & `pyobjc-framework-CoreData-9.2/PyObjCTest/test_nsentitymigrationpolicy.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_nsfetchedresultscontroller.py` & `pyobjc-framework-CoreData-9.2/PyObjCTest/test_nsfetchedresultscontroller.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_nsfetchindexelementdescription.py` & `pyobjc-framework-CoreData-9.2/PyObjCTest/test_nsfetchindexelementdescription.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_nsfetchrequest.py` & `pyobjc-framework-CoreData-9.2/PyObjCTest/test_nsfetchrequest.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_nsfetchrequestexpression.py` & `pyobjc-framework-CoreData-9.2/PyObjCTest/test_nsfetchrequestexpression.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_nsincrementalstore.py` & `pyobjc-framework-CoreData-9.2/PyObjCTest/test_nsincrementalstore.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_nsmanagedobject.py` & `pyobjc-framework-CoreData-9.2/PyObjCTest/test_nsmanagedobject.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_nsmanagedobjectcontext.py` & `pyobjc-framework-CoreData-9.2/PyObjCTest/test_nsmanagedobjectcontext.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_nsmergepolicy.py` & `pyobjc-framework-CoreData-9.2/PyObjCTest/test_nsmergepolicy.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_nsmigrationmanager.py` & `pyobjc-framework-CoreData-9.2/PyObjCTest/test_nsmigrationmanager.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_nspersistentcloudKitcontainer.py` & `pyobjc-framework-CoreData-9.2/PyObjCTest/test_nspersistentcloudKitcontainer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_nspersistentcloudKitcontainerevent.py` & `pyobjc-framework-CoreData-9.2/PyObjCTest/test_nspersistentcloudKitcontainerevent.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_nspersistentcloudkitcontainer_sharing.py` & `pyobjc-framework-CoreData-9.2/PyObjCTest/test_nspersistentcloudkitcontainer_sharing.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_nspersistentstore.py` & `pyobjc-framework-CoreData-9.2/PyObjCTest/test_nspersistentstore.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_nspersistentstorecoordinator.py` & `pyobjc-framework-CoreData-9.2/PyObjCTest/test_nspersistentstorecoordinator.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_nspersistentstoredescription.py` & `pyobjc-framework-CoreData-9.2/PyObjCTest/test_nspersistentstoredescription.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_nspersistentstorerequest.py` & `pyobjc-framework-CoreData-9.2/PyObjCTest/test_nspersistentstorerequest.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_nspersistentstoreresult.py` & `pyobjc-framework-CoreData-9.2/PyObjCTest/test_nspersistentstoreresult.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_nspropertydescription.py` & `pyobjc-framework-CoreData-9.2/PyObjCTest/test_nspropertydescription.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/PyObjCTest/test_nsrelationshipdescription.py` & `pyobjc-framework-CoreData-9.2/PyObjCTest/test_nsrelationshipdescription.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/metadata/CoreData.fwinfo` & `pyobjc-framework-CoreData-9.2/metadata/CoreData.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-CoreData-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-CoreData-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/metadata/raw/arm64-13.3.fwinfo` & `pyobjc-framework-CoreData-9.2/metadata/raw/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/metadata/raw/x86_64-10.10.fwinfo` & `pyobjc-framework-CoreData-9.2/metadata/raw/x86_64-10.10.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/metadata/raw/x86_64-10.15.fwinfo` & `pyobjc-framework-CoreData-9.2/metadata/raw/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-CoreData-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/metadata/raw/x86_64-10.6.fwinfo` & `pyobjc-framework-CoreData-9.2/metadata/raw/x86_64-10.6.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/metadata/raw/x86_64-10.7.fwinfo` & `pyobjc-framework-CoreData-9.2/metadata/raw/x86_64-10.7.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/metadata/raw/x86_64-10.8.fwinfo` & `pyobjc-framework-CoreData-9.2/metadata/raw/x86_64-10.8.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-CoreData-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-CoreData-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/metadata/raw/x86_64-13.3.fwinfo` & `pyobjc-framework-CoreData-9.2/metadata/raw/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/pyobjc_setup.py` & `pyobjc-framework-CoreData-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreData-9.1b1/setup.py` & `pyobjc-framework-CoreData-9.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,18 +5,22 @@
 
 These wrappers don't include documentation, please check Apple's documentation
 for information on how to use this framework and PyObjC's documentation
 for general tips and tricks regarding the translation between Python
 and (Objective-)C frameworks
 """
 import os
+import sys
 
-from pyobjc_setup import setup, Extension
+sys.path.insert(0, os.path.dirname(__file__))
 
-VERSION = "9.1b1"
+
+from pyobjc_setup import setup, Extension  # noqa: E402
+
+VERSION = "9.2"
 
 setup(
     name="pyobjc-framework-CoreData",
     description="Wrappers for the framework CoreData on macOS",
     packages=["CoreData"],
     ext_modules=[
         Extension(
```

