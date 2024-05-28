# Comparing `tmp/pyobjc-framework-WebKit-9.1b1.tar.gz` & `tmp/pyobjc-framework-WebKit-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-WebKit-9.1b1.tar", last modified: Sun Mar 26 11:44:15 2023, max compression
+gzip compressed data, was "pyobjc-framework-WebKit-9.2.tar", last modified: Wed Jun  7 00:32:03 2023, max compression
```

## Comparing `pyobjc-framework-WebKit-9.1b1.tar` & `pyobjc-framework-WebKit-9.2.tar`

### file list

```diff
@@ -1,221 +1,222 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:44:15.190672 pyobjc-framework-WebKit-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:44:14.787029 pyobjc-framework-WebKit-9.1b1/Examples/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:44:14.800328 pyobjc-framework-WebKit-9.1b1/Examples/IEWebArchive/
--rw-r--r--   0 ronald     (501) staff       (20)      316 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/Examples/IEWebArchive/00Todo.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:44:14.802355 pyobjc-framework-WebKit-9.1b1/Examples/IEWebArchive/MHTDocument.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      301 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/Examples/IEWebArchive/MHTDocument.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      451 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/Examples/IEWebArchive/MHTDocument.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)     5145 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/Examples/IEWebArchive/MHTDocument.nib/keyedobjects.nib
--rw-r--r--   0 ronald     (501) staff       (20)     1314 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/Examples/IEWebArchive/MHTDocument.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:44:14.805871 pyobjc-framework-WebKit-9.1b1/Examples/IEWebArchive/MainMenu.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      270 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/Examples/IEWebArchive/MainMenu.nib/JavaCompiling.plist
--rw-r--r--   0 ronald     (501) staff       (20)     9767 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/Examples/IEWebArchive/MainMenu.nib/_MainMenu_EOArchive.java
--rw-r--r--   0 ronald     (501) staff       (20)      109 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/Examples/IEWebArchive/MainMenu.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      564 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/Examples/IEWebArchive/MainMenu.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)    13078 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/Examples/IEWebArchive/MainMenu.nib/keyedobjects.nib
--rw-r--r--   0 ronald     (501) staff       (20)     2877 2021-07-30 09:00:38.000000 pyobjc-framework-WebKit-9.1b1/Examples/IEWebArchive/loader.py
--rw-r--r--   0 ronald     (501) staff       (20)      125 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/Examples/IEWebArchive/main.py
--rw-r--r--   0 ronald     (501) staff       (20)   152598 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/Examples/IEWebArchive/python-home.mht
--rw-r--r--   0 ronald     (501) staff       (20)   141354 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/Examples/IEWebArchive/python-home.webarchive
--rw-r--r--   0 ronald     (501) staff       (20)      607 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/Examples/IEWebArchive/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       44 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/Examples/IEWebArchive/summary.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:44:14.820349 pyobjc-framework-WebKit-9.1b1/Examples/PyDocURLProtocol/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:44:14.822041 pyobjc-framework-WebKit-9.1b1/Examples/PyDocURLProtocol/PyDocBrowser.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      302 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/Examples/PyDocURLProtocol/PyDocBrowser.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      628 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/Examples/PyDocURLProtocol/PyDocBrowser.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)   129218 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/Examples/PyDocURLProtocol/PyDocBrowser.nib/keyedobjects.nib
--rw-r--r--   0 ronald     (501) staff       (20)      332 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/Examples/PyDocURLProtocol/PyDocBrowser.py
--rw-r--r--   0 ronald     (501) staff       (20)     1270 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/Examples/PyDocURLProtocol/PyDocEvents.py
--rw-r--r--   0 ronald     (501) staff       (20)     2260 2021-07-30 09:00:38.000000 pyobjc-framework-WebKit-9.1b1/Examples/PyDocURLProtocol/PyDocURLProtocol.py
--rw-r--r--   0 ronald     (501) staff       (20)      221 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/Examples/PyDocURLProtocol/pydochelper.py
--rw-r--r--   0 ronald     (501) staff       (20)      514 2021-10-18 19:38:40.000000 pyobjc-framework-WebKit-9.1b1/Examples/PyDocURLProtocol/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)      208 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/Examples/PyDocURLProtocol/summary.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:44:14.823198 pyobjc-framework-WebKit-9.1b1/Examples/SimpleJavaScript/
--rw-r--r--   0 ronald     (501) staff       (20)      726 2023-03-03 17:21:59.000000 pyobjc-framework-WebKit-9.1b1/Examples/SimpleJavaScript/simple_javascript.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:44:14.825573 pyobjc-framework-WebKit-9.1b1/Examples/UsingWebKitNightlyBuilds/
--rw-r--r--   0 ronald     (501) staff       (20)      867 2022-10-18 09:53:23.000000 pyobjc-framework-WebKit-9.1b1/Examples/UsingWebKitNightlyBuilds/00ReadMe.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1678 2023-03-03 17:21:59.000000 pyobjc-framework-WebKit-9.1b1/Examples/UsingWebKitNightlyBuilds/rewrite_headers.py
--rw-r--r--   0 ronald     (501) staff       (20)      687 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/Examples/UsingWebKitNightlyBuilds/setup.py.patch
--rw-r--r--   0 ronald     (501) staff       (20)       53 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/Examples/UsingWebKitNightlyBuilds/summary.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:44:14.828414 pyobjc-framework-WebKit-9.1b1/Examples/WebKitInterpreterPlugin/
--rw-r--r--   0 ronald     (501) staff       (20)    20412 2023-03-03 17:21:59.000000 pyobjc-framework-WebKit-9.1b1/Examples/WebKitInterpreterPlugin/WebKitInterpreter.py
--rw-r--r--   0 ronald     (501) staff       (20)      769 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/Examples/WebKitInterpreterPlugin/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)      196 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/Examples/WebKitInterpreterPlugin/summary.txt
--rw-r--r--   0 ronald     (501) staff       (20)      480 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/Examples/WebKitInterpreterPlugin/test.html
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-WebKit-9.1b1/LICENSE.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:44:14.787809 pyobjc-framework-WebKit-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:44:14.830498 pyobjc-framework-WebKit-9.1b1/Lib/JavaScriptCore/
--rw-r--r--   0 ronald     (501) staff       (20)     1246 2023-02-19 10:50:37.000000 pyobjc-framework-WebKit-9.1b1/Lib/JavaScriptCore/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    22182 2023-02-19 10:50:37.000000 pyobjc-framework-WebKit-9.1b1/Lib/JavaScriptCore/_metadata.py
--rw-r--r--   0 ronald     (501) staff       (20)      737 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/Lib/JavaScriptCore/_util.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:44:14.831978 pyobjc-framework-WebKit-9.1b1/Lib/WebKit/
--rw-r--r--   0 ronald     (501) staff       (20)      770 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/Lib/WebKit/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)   118326 2023-02-19 10:50:37.000000 pyobjc-framework-WebKit-9.1b1/Lib/WebKit/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:44:14.836352 pyobjc-framework-WebKit-9.1b1/Lib/pyobjc_framework_WebKit.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2301 2023-03-26 11:44:14.000000 pyobjc-framework-WebKit-9.1b1/Lib/pyobjc_framework_WebKit.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     7217 2023-03-26 11:44:14.000000 pyobjc-framework-WebKit-9.1b1/Lib/pyobjc_framework_WebKit.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:44:14.000000 pyobjc-framework-WebKit-9.1b1/Lib/pyobjc_framework_WebKit.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:51:02.000000 pyobjc-framework-WebKit-9.1b1/Lib/pyobjc_framework_WebKit.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:44:14.000000 pyobjc-framework-WebKit-9.1b1/Lib/pyobjc_framework_WebKit.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       22 2023-03-26 11:44:14.000000 pyobjc-framework-WebKit-9.1b1/Lib/pyobjc_framework_WebKit.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:44:14.838868 pyobjc-framework-WebKit-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)      765 2021-10-18 19:38:40.000000 pyobjc-framework-WebKit-9.1b1/Modules/_WebKit.m
--rw-r--r--   0 ronald     (501) staff       (20)     2623 2021-04-06 18:48:17.000000 pyobjc-framework-WebKit-9.1b1/Modules/_WebKit_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:37.000000 pyobjc-framework-WebKit-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-WebKit-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     2090 2023-03-26 11:44:15.190198 pyobjc-framework-WebKit-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:44:15.063984 pyobjc-framework-WebKit-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      206 2021-03-21 10:08:23.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_carbonutils.py
--rw-r--r--   0 ronald     (501) staff       (20)      175 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domattr.py
--rw-r--r--   0 ronald     (501) staff       (20)     1619 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domcssprimitivevalue.py
--rw-r--r--   0 ronald     (501) staff       (20)      969 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domcssrule.py
--rw-r--r--   0 ronald     (501) staff       (20)      215 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domcssstyledeclaration.py
--rw-r--r--   0 ronald     (501) staff       (20)      341 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domcssvalue.py
--rw-r--r--   0 ronald     (501) staff       (20)     2128 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domdocument.py
--rw-r--r--   0 ronald     (501) staff       (20)      696 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domelement.py
--rw-r--r--   0 ronald     (501) staff       (20)     1095 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domevent.py
--rw-r--r--   0 ronald     (501) staff       (20)      257 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domeventexception.py
--rw-r--r--   0 ronald     (501) staff       (20)      237 2022-06-25 20:09:28.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domeventlistener.py
--rw-r--r--   0 ronald     (501) staff       (20)     1066 2022-06-25 20:11:57.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domeventtarget.py
--rw-r--r--   0 ronald     (501) staff       (20)     1071 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domexception.py
--rw-r--r--   0 ronald     (501) staff       (20)      263 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domhtmlareaelement.py
--rw-r--r--   0 ronald     (501) staff       (20)      566 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domhtmlbuttonelement.py
--rw-r--r--   0 ronald     (501) staff       (20)      281 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domhtmldirectoryelement.py
--rw-r--r--   0 ronald     (501) staff       (20)      269 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domhtmldlistelement.py
--rw-r--r--   0 ronald     (501) staff       (20)      196 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domhtmlelement.py
--rw-r--r--   0 ronald     (501) staff       (20)      271 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domhtmlframeelement.py
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domhtmlhrelement.py
--rw-r--r--   0 ronald     (501) staff       (20)      335 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domhtmlimageelement.py
--rw-r--r--   0 ronald     (501) staff       (20)     1348 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domhtmlinputelement.py
--rw-r--r--   0 ronald     (501) staff       (20)      268 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domhtmllinkelement.py
--rw-r--r--   0 ronald     (501) staff       (20)      266 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domhtmlmenuelement.py
--rw-r--r--   0 ronald     (501) staff       (20)      272 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domhtmlobjectelement.py
--rw-r--r--   0 ronald     (501) staff       (20)      269 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domhtmlolistelement.py
--rw-r--r--   0 ronald     (501) staff       (20)      280 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domhtmloptgroupelement.py
--rw-r--r--   0 ronald     (501) staff       (20)      576 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domhtmloptionelement.py
--rw-r--r--   0 ronald     (501) staff       (20)      300 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domhtmlpreelement.py
--rw-r--r--   0 ronald     (501) staff       (20)      268 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domhtmlscriptelement.py
--rw-r--r--   0 ronald     (501) staff       (20)      710 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domhtmlselectelement.py
--rw-r--r--   0 ronald     (501) staff       (20)      271 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domhtmlstyleelement.py
--rw-r--r--   0 ronald     (501) staff       (20)      279 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domhtmltablecellelement.py
--rw-r--r--   0 ronald     (501) staff       (20)      207 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domhtmltexareaelement.py
--rw-r--r--   0 ronald     (501) staff       (20)      726 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domhtmltextareaelement.py
--rw-r--r--   0 ronald     (501) staff       (20)      269 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domhtmlulistelement.py
--rw-r--r--   0 ronald     (501) staff       (20)      276 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domimplementation.py
--rw-r--r--   0 ronald     (501) staff       (20)     6498 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domkeyboardevent.py
--rw-r--r--   0 ronald     (501) staff       (20)     2305 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_dommouseevent.py
--rw-r--r--   0 ronald     (501) staff       (20)      783 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_dommutationevent.py
--rw-r--r--   0 ronald     (501) staff       (20)     2079 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domnode.py
--rw-r--r--   0 ronald     (501) staff       (20)     1733 2022-06-25 09:29:20.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domnodefilter.py
--rw-r--r--   0 ronald     (501) staff       (20)      288 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domnodeiterator.py
--rw-r--r--   0 ronald     (501) staff       (20)      746 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domoverflowevent.py
--rw-r--r--   0 ronald     (501) staff       (20)      243 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domprogressevent.py
--rw-r--r--   0 ronald     (501) staff       (20)      833 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domrange.py
--rw-r--r--   0 ronald     (501) staff       (20)      315 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domrangeexception.py
--rw-r--r--   0 ronald     (501) staff       (20)      253 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domstylesheet.py
--rw-r--r--   0 ronald     (501) staff       (20)      564 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domtraversal.py
--rw-r--r--   0 ronald     (501) staff       (20)      200 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domtreewalker.py
--rw-r--r--   0 ronald     (501) staff       (20)      494 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domuievent.py
--rw-r--r--   0 ronald     (501) staff       (20)     1436 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domwheelevent.py
--rw-r--r--   0 ronald     (501) staff       (20)      305 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domxpathexception.py
--rw-r--r--   0 ronald     (501) staff       (20)      243 2022-06-25 20:17:46.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domxpathnsresolver.py
--rw-r--r--   0 ronald     (501) staff       (20)      904 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domxpathresult.py
--rw-r--r--   0 ronald     (501) staff       (20)      212 2022-04-11 08:03:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_javascriptcore.py
--rw-r--r--   0 ronald     (501) staff       (20)     1963 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_jsbase.py
--rw-r--r--   0 ronald     (501) staff       (20)      602 2023-02-19 10:50:37.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_jscontext.py
--rw-r--r--   0 ronald     (501) staff       (20)     4197 2023-03-25 12:41:55.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_jscontextref.py
--rw-r--r--   0 ronald     (501) staff       (20)     1773 2023-02-19 10:50:37.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_jsexport.py
--rw-r--r--   0 ronald     (501) staff       (20)      234 2021-03-21 10:08:23.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_jsmanagedvalue.py
--rw-r--r--   0 ronald     (501) staff       (20)    20045 2023-03-03 17:21:59.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_jsobjectref.py
--rw-r--r--   0 ronald     (501) staff       (20)     2424 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_jsstringref.py
--rw-r--r--   0 ronald     (501) staff       (20)      520 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_jsstringrefcf.py
--rw-r--r--   0 ronald     (501) staff       (20)     9404 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_jstypedarray.py
--rw-r--r--   0 ronald     (501) staff       (20)     2317 2021-07-30 14:02:33.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_jsvalue.py
--rw-r--r--   0 ronald     (501) staff       (20)     4907 2021-06-10 09:09:03.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_jsvalueref.py
--rw-r--r--   0 ronald     (501) staff       (20)      238 2021-03-21 10:08:23.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_jsvirtualmachine.py
--rw-r--r--   0 ronald     (501) staff       (20)     1128 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_nsattributedstring.py
--rw-r--r--   0 ronald     (501) staff       (20)      186 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_webarchive.py
--rw-r--r--   0 ronald     (501) staff       (20)      201 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_webbackforwardlist.py
--rw-r--r--   0 ronald     (501) staff       (20)      187 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_webdatasource.py
--rw-r--r--   0 ronald     (501) staff       (20)     1381 2022-06-25 20:06:40.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_webdocument.py
--rw-r--r--   0 ronald     (501) staff       (20)      237 2022-06-25 20:14:18.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_webdownload.py
--rw-r--r--   0 ronald     (501) staff       (20)     2775 2022-06-25 20:11:47.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_webeditingdelegate.py
--rw-r--r--   0 ronald     (501) staff       (20)      668 2022-06-25 09:28:56.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_webframeloaddelegate.py
--rw-r--r--   0 ronald     (501) staff       (20)      426 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_webframeview.py
--rw-r--r--   0 ronald     (501) staff       (20)      864 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_webhistory.py
--rw-r--r--   0 ronald     (501) staff       (20)      203 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_webhistoryitem.py
--rw-r--r--   0 ronald     (501) staff       (20)      764 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_webjavaplugin.py
--rw-r--r--   0 ronald     (501) staff       (20)     1948 2022-06-25 09:28:07.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_webkit.py
--rw-r--r--   0 ronald     (501) staff       (20)      754 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_webkitavailability.py
--rw-r--r--   0 ronald     (501) staff       (20)      879 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_webkiterrors.py
--rw-r--r--   0 ronald     (501) staff       (20)      311 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_webplugin.py
--rw-r--r--   0 ronald     (501) staff       (20)      681 2022-06-25 20:11:28.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_webpluginviewfactory.py
--rw-r--r--   0 ronald     (501) staff       (20)     1160 2022-06-25 20:07:59.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_webpolicydelegate.py
--rw-r--r--   0 ronald     (501) staff       (20)     3081 2022-02-24 08:47:17.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_webpreferences.py
--rw-r--r--   0 ronald     (501) staff       (20)      655 2022-06-25 09:28:25.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_webresourceloaddelegate.py
--rw-r--r--   0 ronald     (501) staff       (20)     1394 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_webscriptobject.py
--rw-r--r--   0 ronald     (501) staff       (20)     8808 2022-06-25 09:27:36.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_webuidelegate.py
--rw-r--r--   0 ronald     (501) staff       (20)     3643 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_webview.py
--rw-r--r--   0 ronald     (501) staff       (20)      887 2021-03-21 10:08:23.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_wkcontentruleliststore.py
--rw-r--r--   0 ronald     (501) staff       (20)      278 2021-07-30 09:00:38.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_wkdownload.py
--rw-r--r--   0 ronald     (501) staff       (20)     1569 2022-06-25 09:27:24.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_wkdownloaddelegate.py
--rw-r--r--   0 ronald     (501) staff       (20)     1507 2022-06-15 11:57:00.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_wkerror.py
--rw-r--r--   0 ronald     (501) staff       (20)      607 2021-07-30 09:00:38.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_wkfindconfiguration.py
--rw-r--r--   0 ronald     (501) staff       (20)      230 2021-07-30 09:00:38.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_wkfindresult.py
--rw-r--r--   0 ronald     (501) staff       (20)      231 2021-03-21 10:08:23.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_wkframeinfo.py
--rw-r--r--   0 ronald     (501) staff       (20)      475 2021-03-21 10:08:23.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_wkhttpcookiestore.py
--rw-r--r--   0 ronald     (501) staff       (20)      784 2022-02-24 08:47:17.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_wknavigationaction.py
--rw-r--r--   0 ronald     (501) staff       (20)     2320 2022-06-25 09:28:50.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_wknavigationdelegate.py
--rw-r--r--   0 ronald     (501) staff       (20)      329 2021-03-21 10:08:23.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_wknavigationresponse.py
--rw-r--r--   0 ronald     (501) staff       (20)      407 2021-03-21 10:08:23.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_wkopenpanelparameters.py
--rw-r--r--   0 ronald     (501) staff       (20)     2193 2023-02-19 10:50:37.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_wkpreferences.py
--rw-r--r--   0 ronald     (501) staff       (20)      254 2022-06-25 20:14:05.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_wkscriptmessagehandler.py
--rw-r--r--   0 ronald     (501) staff       (20)      642 2022-06-25 20:11:45.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_wkscriptmessagehandlerwithreply.py
--rw-r--r--   0 ronald     (501) staff       (20)      344 2021-03-21 10:08:23.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_wksnapshotconfiguration.py
--rw-r--r--   0 ronald     (501) staff       (20)     3111 2022-11-27 13:18:48.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_wkuidelegate.py
--rw-r--r--   0 ronald     (501) staff       (20)      880 2022-02-24 08:47:17.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_wkuserscript.py
--rw-r--r--   0 ronald     (501) staff       (20)      863 2022-10-18 09:54:01.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_wkwebpagepreferences.py
--rw-r--r--   0 ronald     (501) staff       (20)     1132 2022-07-08 16:02:54.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_wkwebsitedatarecord.py
--rw-r--r--   0 ronald     (501) staff       (20)      733 2021-03-21 10:08:23.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_wkwebsitedatastore.py
--rw-r--r--   0 ronald     (501) staff       (20)     5060 2023-02-19 10:50:37.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_wkwebview.py
--rw-r--r--   0 ronald     (501) staff       (20)     1883 2022-02-24 08:47:17.000000 pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_wkwebviewconfiguration.py
--rw-r--r--   0 ronald     (501) staff       (20)      307 2021-10-18 19:38:40.000000 pyobjc-framework-WebKit-9.1b1/README.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:44:15.075862 pyobjc-framework-WebKit-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)    24865 2021-07-30 14:12:01.000000 pyobjc-framework-WebKit-9.1b1/metadata/JavaScriptCore.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    68939 2022-11-27 13:18:48.000000 pyobjc-framework-WebKit-9.1b1/metadata/WebKit.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)      198 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:44:15.097600 pyobjc-framework-WebKit-9.1b1/metadata/raw.jc/
--rw-r--r--   0 ronald     (501) staff       (20)    65777 2021-08-04 10:01:04.000000 pyobjc-framework-WebKit-9.1b1/metadata/raw.jc/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    65796 2022-02-24 08:47:17.000000 pyobjc-framework-WebKit-9.1b1/metadata/raw.jc/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    68984 2023-03-03 17:21:59.000000 pyobjc-framework-WebKit-9.1b1/metadata/raw.jc/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    26161 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/metadata/raw.jc/x86_64-10.10.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    60816 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/metadata/raw.jc/x86_64-10.14.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    65239 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/metadata/raw.jc/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    65695 2021-03-21 10:08:23.000000 pyobjc-framework-WebKit-9.1b1/metadata/raw.jc/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    31674 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/metadata/raw.jc/x86_64-10.6.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    31712 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/metadata/raw.jc/x86_64-10.7.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    32145 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/metadata/raw.jc/x86_64-10.8.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    65778 2021-08-04 10:01:04.000000 pyobjc-framework-WebKit-9.1b1/metadata/raw.jc/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    65797 2022-02-24 08:47:17.000000 pyobjc-framework-WebKit-9.1b1/metadata/raw.jc/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    68985 2023-03-03 17:21:59.000000 pyobjc-framework-WebKit-9.1b1/metadata/raw.jc/x86_64-13.3.fwinfo
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:44:15.185267 pyobjc-framework-WebKit-9.1b1/metadata/raw.wk/
--rw-r--r--   0 ronald     (501) staff       (20)   776147 2021-08-04 10:01:02.000000 pyobjc-framework-WebKit-9.1b1/metadata/raw.wk/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   779208 2022-02-24 08:47:17.000000 pyobjc-framework-WebKit-9.1b1/metadata/raw.wk/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   783528 2022-10-18 09:53:23.000000 pyobjc-framework-WebKit-9.1b1/metadata/raw.wk/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   784908 2023-03-03 17:21:59.000000 pyobjc-framework-WebKit-9.1b1/metadata/raw.wk/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   728137 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/metadata/raw.wk/x86_64-10.10.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   725120 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/metadata/raw.wk/x86_64-10.14.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   737447 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/metadata/raw.wk/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   751735 2021-03-21 10:08:23.000000 pyobjc-framework-WebKit-9.1b1/metadata/raw.wk/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   452787 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/metadata/raw.wk/x86_64-10.6.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   453311 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/metadata/raw.wk/x86_64-10.7.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   453470 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.1b1/metadata/raw.wk/x86_64-10.8.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   775990 2021-08-04 10:01:02.000000 pyobjc-framework-WebKit-9.1b1/metadata/raw.wk/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   779209 2022-02-24 08:47:17.000000 pyobjc-framework-WebKit-9.1b1/metadata/raw.wk/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   783529 2022-10-18 09:53:23.000000 pyobjc-framework-WebKit-9.1b1/metadata/raw.wk/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   784909 2023-03-03 17:21:59.000000 pyobjc-framework-WebKit-9.1b1/metadata/raw.wk/x86_64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-WebKit-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:44:15.190772 pyobjc-framework-WebKit-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1276 2023-03-25 14:20:32.000000 pyobjc-framework-WebKit-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:32:03.195968 pyobjc-framework-WebKit-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:32:02.882544 pyobjc-framework-WebKit-9.2/Examples/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:32:02.895914 pyobjc-framework-WebKit-9.2/Examples/IEWebArchive/
+-rw-r--r--   0 ronald     (501) staff       (20)      316 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/Examples/IEWebArchive/00Todo.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:32:02.898302 pyobjc-framework-WebKit-9.2/Examples/IEWebArchive/MHTDocument.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      301 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/Examples/IEWebArchive/MHTDocument.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      451 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/Examples/IEWebArchive/MHTDocument.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     5145 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/Examples/IEWebArchive/MHTDocument.nib/keyedobjects.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     1314 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/Examples/IEWebArchive/MHTDocument.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:32:02.901858 pyobjc-framework-WebKit-9.2/Examples/IEWebArchive/MainMenu.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      270 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/Examples/IEWebArchive/MainMenu.nib/JavaCompiling.plist
+-rw-r--r--   0 ronald     (501) staff       (20)     9767 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/Examples/IEWebArchive/MainMenu.nib/_MainMenu_EOArchive.java
+-rw-r--r--   0 ronald     (501) staff       (20)      109 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/Examples/IEWebArchive/MainMenu.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      564 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/Examples/IEWebArchive/MainMenu.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)    13078 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/Examples/IEWebArchive/MainMenu.nib/keyedobjects.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     2877 2021-07-30 09:00:38.000000 pyobjc-framework-WebKit-9.2/Examples/IEWebArchive/loader.py
+-rw-r--r--   0 ronald     (501) staff       (20)      125 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/Examples/IEWebArchive/main.py
+-rw-r--r--   0 ronald     (501) staff       (20)   152598 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/Examples/IEWebArchive/python-home.mht
+-rw-r--r--   0 ronald     (501) staff       (20)   141354 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/Examples/IEWebArchive/python-home.webarchive
+-rw-r--r--   0 ronald     (501) staff       (20)      607 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/Examples/IEWebArchive/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       44 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/Examples/IEWebArchive/summary.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:32:02.905958 pyobjc-framework-WebKit-9.2/Examples/PyDocURLProtocol/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:32:02.914997 pyobjc-framework-WebKit-9.2/Examples/PyDocURLProtocol/PyDocBrowser.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      302 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/Examples/PyDocURLProtocol/PyDocBrowser.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      628 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/Examples/PyDocURLProtocol/PyDocBrowser.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)   129218 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/Examples/PyDocURLProtocol/PyDocBrowser.nib/keyedobjects.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      332 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/Examples/PyDocURLProtocol/PyDocBrowser.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1270 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/Examples/PyDocURLProtocol/PyDocEvents.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2260 2021-07-30 09:00:38.000000 pyobjc-framework-WebKit-9.2/Examples/PyDocURLProtocol/PyDocURLProtocol.py
+-rw-r--r--   0 ronald     (501) staff       (20)      221 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/Examples/PyDocURLProtocol/pydochelper.py
+-rw-r--r--   0 ronald     (501) staff       (20)      514 2021-10-18 19:38:40.000000 pyobjc-framework-WebKit-9.2/Examples/PyDocURLProtocol/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)      208 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/Examples/PyDocURLProtocol/summary.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:32:02.916236 pyobjc-framework-WebKit-9.2/Examples/SimpleJavaScript/
+-rw-r--r--   0 ronald     (501) staff       (20)      726 2023-03-03 17:21:59.000000 pyobjc-framework-WebKit-9.2/Examples/SimpleJavaScript/simple_javascript.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:32:02.918925 pyobjc-framework-WebKit-9.2/Examples/UsingWebKitNightlyBuilds/
+-rw-r--r--   0 ronald     (501) staff       (20)      867 2022-10-18 09:53:23.000000 pyobjc-framework-WebKit-9.2/Examples/UsingWebKitNightlyBuilds/00ReadMe.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1678 2023-03-03 17:21:59.000000 pyobjc-framework-WebKit-9.2/Examples/UsingWebKitNightlyBuilds/rewrite_headers.py
+-rw-r--r--   0 ronald     (501) staff       (20)      687 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/Examples/UsingWebKitNightlyBuilds/setup.py.patch
+-rw-r--r--   0 ronald     (501) staff       (20)       53 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/Examples/UsingWebKitNightlyBuilds/summary.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:32:02.921376 pyobjc-framework-WebKit-9.2/Examples/WebKitInterpreterPlugin/
+-rw-r--r--   0 ronald     (501) staff       (20)    20412 2023-03-03 17:21:59.000000 pyobjc-framework-WebKit-9.2/Examples/WebKitInterpreterPlugin/WebKitInterpreter.py
+-rw-r--r--   0 ronald     (501) staff       (20)      769 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/Examples/WebKitInterpreterPlugin/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)      196 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/Examples/WebKitInterpreterPlugin/summary.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      480 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/Examples/WebKitInterpreterPlugin/test.html
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-WebKit-9.2/LICENSE.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:32:02.883462 pyobjc-framework-WebKit-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:32:02.923360 pyobjc-framework-WebKit-9.2/Lib/JavaScriptCore/
+-rw-r--r--   0 ronald     (501) staff       (20)     1246 2023-02-19 10:50:37.000000 pyobjc-framework-WebKit-9.2/Lib/JavaScriptCore/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    22718 2023-05-27 09:46:33.000000 pyobjc-framework-WebKit-9.2/Lib/JavaScriptCore/_metadata.py
+-rw-r--r--   0 ronald     (501) staff       (20)      737 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/Lib/JavaScriptCore/_util.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:32:02.924584 pyobjc-framework-WebKit-9.2/Lib/WebKit/
+-rw-r--r--   0 ronald     (501) staff       (20)      770 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/Lib/WebKit/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)   118326 2023-05-27 09:46:33.000000 pyobjc-framework-WebKit-9.2/Lib/WebKit/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:32:02.928130 pyobjc-framework-WebKit-9.2/Lib/pyobjc_framework_WebKit.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2299 2023-06-07 00:32:02.000000 pyobjc-framework-WebKit-9.2/Lib/pyobjc_framework_WebKit.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     7232 2023-06-07 00:32:02.000000 pyobjc-framework-WebKit-9.2/Lib/pyobjc_framework_WebKit.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:32:02.000000 pyobjc-framework-WebKit-9.2/Lib/pyobjc_framework_WebKit.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:51:02.000000 pyobjc-framework-WebKit-9.2/Lib/pyobjc_framework_WebKit.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:32:02.000000 pyobjc-framework-WebKit-9.2/Lib/pyobjc_framework_WebKit.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       22 2023-06-07 00:32:02.000000 pyobjc-framework-WebKit-9.2/Lib/pyobjc_framework_WebKit.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:32:02.930589 pyobjc-framework-WebKit-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)      765 2021-10-18 19:38:40.000000 pyobjc-framework-WebKit-9.2/Modules/_WebKit.m
+-rw-r--r--   0 ronald     (501) staff       (20)     2623 2021-04-06 18:48:17.000000 pyobjc-framework-WebKit-9.2/Modules/_WebKit_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:37.000000 pyobjc-framework-WebKit-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-WebKit-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     2088 2023-06-07 00:32:03.195568 pyobjc-framework-WebKit-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:32:03.090959 pyobjc-framework-WebKit-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      206 2021-03-21 10:08:23.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_carbonutils.py
+-rw-r--r--   0 ronald     (501) staff       (20)      175 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_domattr.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1619 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_domcssprimitivevalue.py
+-rw-r--r--   0 ronald     (501) staff       (20)      969 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_domcssrule.py
+-rw-r--r--   0 ronald     (501) staff       (20)      215 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_domcssstyledeclaration.py
+-rw-r--r--   0 ronald     (501) staff       (20)      341 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_domcssvalue.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2128 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_domdocument.py
+-rw-r--r--   0 ronald     (501) staff       (20)      696 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_domelement.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1095 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_domevent.py
+-rw-r--r--   0 ronald     (501) staff       (20)      257 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_domeventexception.py
+-rw-r--r--   0 ronald     (501) staff       (20)      237 2022-06-25 20:09:28.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_domeventlistener.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1066 2022-06-25 20:11:57.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_domeventtarget.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1071 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_domexception.py
+-rw-r--r--   0 ronald     (501) staff       (20)      263 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_domhtmlareaelement.py
+-rw-r--r--   0 ronald     (501) staff       (20)      566 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_domhtmlbuttonelement.py
+-rw-r--r--   0 ronald     (501) staff       (20)      281 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_domhtmldirectoryelement.py
+-rw-r--r--   0 ronald     (501) staff       (20)      269 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_domhtmldlistelement.py
+-rw-r--r--   0 ronald     (501) staff       (20)      196 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_domhtmlelement.py
+-rw-r--r--   0 ronald     (501) staff       (20)      271 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_domhtmlframeelement.py
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_domhtmlhrelement.py
+-rw-r--r--   0 ronald     (501) staff       (20)      335 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_domhtmlimageelement.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1348 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_domhtmlinputelement.py
+-rw-r--r--   0 ronald     (501) staff       (20)      268 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_domhtmllinkelement.py
+-rw-r--r--   0 ronald     (501) staff       (20)      266 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_domhtmlmenuelement.py
+-rw-r--r--   0 ronald     (501) staff       (20)      272 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_domhtmlobjectelement.py
+-rw-r--r--   0 ronald     (501) staff       (20)      269 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_domhtmlolistelement.py
+-rw-r--r--   0 ronald     (501) staff       (20)      280 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_domhtmloptgroupelement.py
+-rw-r--r--   0 ronald     (501) staff       (20)      576 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_domhtmloptionelement.py
+-rw-r--r--   0 ronald     (501) staff       (20)      300 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_domhtmlpreelement.py
+-rw-r--r--   0 ronald     (501) staff       (20)      268 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_domhtmlscriptelement.py
+-rw-r--r--   0 ronald     (501) staff       (20)      710 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_domhtmlselectelement.py
+-rw-r--r--   0 ronald     (501) staff       (20)      271 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_domhtmlstyleelement.py
+-rw-r--r--   0 ronald     (501) staff       (20)      279 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_domhtmltablecellelement.py
+-rw-r--r--   0 ronald     (501) staff       (20)      207 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_domhtmltexareaelement.py
+-rw-r--r--   0 ronald     (501) staff       (20)      726 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_domhtmltextareaelement.py
+-rw-r--r--   0 ronald     (501) staff       (20)      269 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_domhtmlulistelement.py
+-rw-r--r--   0 ronald     (501) staff       (20)      276 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_domimplementation.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6498 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_domkeyboardevent.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2305 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_dommouseevent.py
+-rw-r--r--   0 ronald     (501) staff       (20)      783 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_dommutationevent.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2079 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_domnode.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1733 2022-06-25 09:29:20.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_domnodefilter.py
+-rw-r--r--   0 ronald     (501) staff       (20)      288 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_domnodeiterator.py
+-rw-r--r--   0 ronald     (501) staff       (20)      746 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_domoverflowevent.py
+-rw-r--r--   0 ronald     (501) staff       (20)      243 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_domprogressevent.py
+-rw-r--r--   0 ronald     (501) staff       (20)      833 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_domrange.py
+-rw-r--r--   0 ronald     (501) staff       (20)      315 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_domrangeexception.py
+-rw-r--r--   0 ronald     (501) staff       (20)      253 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_domstylesheet.py
+-rw-r--r--   0 ronald     (501) staff       (20)      564 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_domtraversal.py
+-rw-r--r--   0 ronald     (501) staff       (20)      200 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_domtreewalker.py
+-rw-r--r--   0 ronald     (501) staff       (20)      494 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_domuievent.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1436 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_domwheelevent.py
+-rw-r--r--   0 ronald     (501) staff       (20)      305 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_domxpathexception.py
+-rw-r--r--   0 ronald     (501) staff       (20)      243 2022-06-25 20:17:46.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_domxpathnsresolver.py
+-rw-r--r--   0 ronald     (501) staff       (20)      904 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_domxpathresult.py
+-rw-r--r--   0 ronald     (501) staff       (20)      212 2022-04-11 08:03:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_javascriptcore.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1963 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_jsbase.py
+-rw-r--r--   0 ronald     (501) staff       (20)      602 2023-02-19 10:50:37.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_jscontext.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4197 2023-03-25 12:41:55.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_jscontextref.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1773 2023-02-19 10:50:37.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_jsexport.py
+-rw-r--r--   0 ronald     (501) staff       (20)      234 2021-03-21 10:08:23.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_jsmanagedvalue.py
+-rw-r--r--   0 ronald     (501) staff       (20)    20120 2023-05-27 09:46:33.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_jsobjectref.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2424 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_jsstringref.py
+-rw-r--r--   0 ronald     (501) staff       (20)      520 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_jsstringrefcf.py
+-rw-r--r--   0 ronald     (501) staff       (20)     9404 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_jstypedarray.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2317 2021-07-30 14:02:33.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_jsvalue.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5311 2023-05-27 09:46:33.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_jsvalueref.py
+-rw-r--r--   0 ronald     (501) staff       (20)      238 2021-03-21 10:08:23.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_jsvirtualmachine.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1128 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_nsattributedstring.py
+-rw-r--r--   0 ronald     (501) staff       (20)      186 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_webarchive.py
+-rw-r--r--   0 ronald     (501) staff       (20)      201 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_webbackforwardlist.py
+-rw-r--r--   0 ronald     (501) staff       (20)      187 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_webdatasource.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1381 2022-06-25 20:06:40.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_webdocument.py
+-rw-r--r--   0 ronald     (501) staff       (20)      237 2022-06-25 20:14:18.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_webdownload.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2775 2022-06-25 20:11:47.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_webeditingdelegate.py
+-rw-r--r--   0 ronald     (501) staff       (20)      668 2022-06-25 09:28:56.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_webframeloaddelegate.py
+-rw-r--r--   0 ronald     (501) staff       (20)      426 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_webframeview.py
+-rw-r--r--   0 ronald     (501) staff       (20)      864 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_webhistory.py
+-rw-r--r--   0 ronald     (501) staff       (20)      203 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_webhistoryitem.py
+-rw-r--r--   0 ronald     (501) staff       (20)      764 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_webjavaplugin.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1948 2022-06-25 09:28:07.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_webkit.py
+-rw-r--r--   0 ronald     (501) staff       (20)      754 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_webkitavailability.py
+-rw-r--r--   0 ronald     (501) staff       (20)      879 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_webkiterrors.py
+-rw-r--r--   0 ronald     (501) staff       (20)      311 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_webplugin.py
+-rw-r--r--   0 ronald     (501) staff       (20)      681 2022-06-25 20:11:28.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_webpluginviewfactory.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1160 2022-06-25 20:07:59.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_webpolicydelegate.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3081 2022-02-24 08:47:17.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_webpreferences.py
+-rw-r--r--   0 ronald     (501) staff       (20)      655 2022-06-25 09:28:25.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_webresourceloaddelegate.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1394 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_webscriptobject.py
+-rw-r--r--   0 ronald     (501) staff       (20)     8808 2022-06-25 09:27:36.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_webuidelegate.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3643 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_webview.py
+-rw-r--r--   0 ronald     (501) staff       (20)      887 2021-03-21 10:08:23.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_wkcontentruleliststore.py
+-rw-r--r--   0 ronald     (501) staff       (20)      278 2021-07-30 09:00:38.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_wkdownload.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1569 2022-06-25 09:27:24.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_wkdownloaddelegate.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1507 2022-06-15 11:57:00.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_wkerror.py
+-rw-r--r--   0 ronald     (501) staff       (20)      607 2021-07-30 09:00:38.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_wkfindconfiguration.py
+-rw-r--r--   0 ronald     (501) staff       (20)      230 2021-07-30 09:00:38.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_wkfindresult.py
+-rw-r--r--   0 ronald     (501) staff       (20)      231 2021-03-21 10:08:23.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_wkframeinfo.py
+-rw-r--r--   0 ronald     (501) staff       (20)      475 2021-03-21 10:08:23.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_wkhttpcookiestore.py
+-rw-r--r--   0 ronald     (501) staff       (20)      784 2022-02-24 08:47:17.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_wknavigationaction.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2320 2022-06-25 09:28:50.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_wknavigationdelegate.py
+-rw-r--r--   0 ronald     (501) staff       (20)      329 2021-03-21 10:08:23.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_wknavigationresponse.py
+-rw-r--r--   0 ronald     (501) staff       (20)      407 2021-03-21 10:08:23.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_wkopenpanelparameters.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2193 2023-02-19 10:50:37.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_wkpreferences.py
+-rw-r--r--   0 ronald     (501) staff       (20)      254 2022-06-25 20:14:05.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_wkscriptmessagehandler.py
+-rw-r--r--   0 ronald     (501) staff       (20)      642 2022-06-25 20:11:45.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_wkscriptmessagehandlerwithreply.py
+-rw-r--r--   0 ronald     (501) staff       (20)      344 2021-03-21 10:08:23.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_wksnapshotconfiguration.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3111 2022-11-27 13:18:48.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_wkuidelegate.py
+-rw-r--r--   0 ronald     (501) staff       (20)      880 2022-02-24 08:47:17.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_wkuserscript.py
+-rw-r--r--   0 ronald     (501) staff       (20)      863 2022-10-18 09:54:01.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_wkwebpagepreferences.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1132 2022-07-08 16:02:54.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_wkwebsitedatarecord.py
+-rw-r--r--   0 ronald     (501) staff       (20)      733 2021-03-21 10:08:23.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_wkwebsitedatastore.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5060 2023-02-19 10:50:37.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_wkwebview.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1883 2022-02-24 08:47:17.000000 pyobjc-framework-WebKit-9.2/PyObjCTest/test_wkwebviewconfiguration.py
+-rw-r--r--   0 ronald     (501) staff       (20)      307 2021-10-18 19:38:40.000000 pyobjc-framework-WebKit-9.2/README.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:32:03.096111 pyobjc-framework-WebKit-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)    25033 2023-05-27 09:46:34.000000 pyobjc-framework-WebKit-9.2/metadata/JavaScriptCore.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    68939 2022-11-27 13:18:48.000000 pyobjc-framework-WebKit-9.2/metadata/WebKit.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)      198 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:32:03.110452 pyobjc-framework-WebKit-9.2/metadata/raw.jc/
+-rw-r--r--   0 ronald     (501) staff       (20)    65777 2021-08-04 10:01:04.000000 pyobjc-framework-WebKit-9.2/metadata/raw.jc/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    65796 2022-02-24 08:47:17.000000 pyobjc-framework-WebKit-9.2/metadata/raw.jc/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    68984 2023-03-03 17:21:59.000000 pyobjc-framework-WebKit-9.2/metadata/raw.jc/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    26161 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/metadata/raw.jc/x86_64-10.10.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    60816 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/metadata/raw.jc/x86_64-10.14.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    65239 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/metadata/raw.jc/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    65695 2021-03-21 10:08:23.000000 pyobjc-framework-WebKit-9.2/metadata/raw.jc/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    31674 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/metadata/raw.jc/x86_64-10.6.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    31712 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/metadata/raw.jc/x86_64-10.7.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    32145 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/metadata/raw.jc/x86_64-10.8.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    65778 2021-08-04 10:01:04.000000 pyobjc-framework-WebKit-9.2/metadata/raw.jc/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    65797 2022-02-24 08:47:17.000000 pyobjc-framework-WebKit-9.2/metadata/raw.jc/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    68985 2023-03-03 17:21:59.000000 pyobjc-framework-WebKit-9.2/metadata/raw.jc/x86_64-13.3.fwinfo
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:32:03.192460 pyobjc-framework-WebKit-9.2/metadata/raw.wk/
+-rw-r--r--   0 ronald     (501) staff       (20)   776147 2021-08-04 10:01:02.000000 pyobjc-framework-WebKit-9.2/metadata/raw.wk/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   779208 2022-02-24 08:47:17.000000 pyobjc-framework-WebKit-9.2/metadata/raw.wk/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   783528 2022-10-18 09:53:23.000000 pyobjc-framework-WebKit-9.2/metadata/raw.wk/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   784908 2023-03-03 17:21:59.000000 pyobjc-framework-WebKit-9.2/metadata/raw.wk/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   728137 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/metadata/raw.wk/x86_64-10.10.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   725120 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/metadata/raw.wk/x86_64-10.14.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   737447 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/metadata/raw.wk/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   751735 2021-03-21 10:08:23.000000 pyobjc-framework-WebKit-9.2/metadata/raw.wk/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   452787 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/metadata/raw.wk/x86_64-10.6.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   453311 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/metadata/raw.wk/x86_64-10.7.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   453470 2020-11-30 18:45:15.000000 pyobjc-framework-WebKit-9.2/metadata/raw.wk/x86_64-10.8.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   775990 2021-08-04 10:01:02.000000 pyobjc-framework-WebKit-9.2/metadata/raw.wk/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   779209 2022-02-24 08:47:17.000000 pyobjc-framework-WebKit-9.2/metadata/raw.wk/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   783529 2022-10-18 09:53:23.000000 pyobjc-framework-WebKit-9.2/metadata/raw.wk/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   784909 2023-03-03 17:21:59.000000 pyobjc-framework-WebKit-9.2/metadata/raw.wk/x86_64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-WebKit-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-WebKit-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:32:03.196072 pyobjc-framework-WebKit-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1347 2023-05-29 10:07:47.000000 pyobjc-framework-WebKit-9.2/setup.py
```

### Comparing `pyobjc-framework-WebKit-9.1b1/Examples/IEWebArchive/MHTDocument.nib/keyedobjects.nib` & `pyobjc-framework-WebKit-9.2/Examples/IEWebArchive/MHTDocument.nib/keyedobjects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/Examples/IEWebArchive/MHTDocument.py` & `pyobjc-framework-WebKit-9.2/Examples/IEWebArchive/MHTDocument.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/Examples/IEWebArchive/MainMenu.nib/_MainMenu_EOArchive.java` & `pyobjc-framework-WebKit-9.2/Examples/IEWebArchive/MainMenu.nib/_MainMenu_EOArchive.java`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/Examples/IEWebArchive/MainMenu.nib/info.nib` & `pyobjc-framework-WebKit-9.2/Examples/IEWebArchive/MainMenu.nib/info.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/Examples/IEWebArchive/MainMenu.nib/keyedobjects.nib` & `pyobjc-framework-WebKit-9.2/Examples/IEWebArchive/MainMenu.nib/keyedobjects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/Examples/IEWebArchive/loader.py` & `pyobjc-framework-WebKit-9.2/Examples/IEWebArchive/loader.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/Examples/IEWebArchive/python-home.mht` & `pyobjc-framework-WebKit-9.2/Examples/IEWebArchive/python-home.mht`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/Examples/IEWebArchive/python-home.webarchive` & `pyobjc-framework-WebKit-9.2/Examples/IEWebArchive/python-home.webarchive`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/Examples/IEWebArchive/setup.py` & `pyobjc-framework-WebKit-9.2/Examples/IEWebArchive/setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/Examples/PyDocURLProtocol/PyDocBrowser.nib/info.nib` & `pyobjc-framework-WebKit-9.2/Examples/PyDocURLProtocol/PyDocBrowser.nib/info.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/Examples/PyDocURLProtocol/PyDocBrowser.nib/keyedobjects.nib` & `pyobjc-framework-WebKit-9.2/Examples/PyDocURLProtocol/PyDocBrowser.nib/keyedobjects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/Examples/PyDocURLProtocol/PyDocEvents.py` & `pyobjc-framework-WebKit-9.2/Examples/PyDocURLProtocol/PyDocEvents.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/Examples/PyDocURLProtocol/PyDocURLProtocol.py` & `pyobjc-framework-WebKit-9.2/Examples/PyDocURLProtocol/PyDocURLProtocol.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/Examples/PyDocURLProtocol/setup.py` & `pyobjc-framework-WebKit-9.2/Examples/PyDocURLProtocol/setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/Examples/SimpleJavaScript/simple_javascript.py` & `pyobjc-framework-WebKit-9.2/Examples/SimpleJavaScript/simple_javascript.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/Examples/UsingWebKitNightlyBuilds/00ReadMe.txt` & `pyobjc-framework-WebKit-9.2/Examples/UsingWebKitNightlyBuilds/00ReadMe.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/Examples/UsingWebKitNightlyBuilds/rewrite_headers.py` & `pyobjc-framework-WebKit-9.2/Examples/UsingWebKitNightlyBuilds/rewrite_headers.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/Examples/UsingWebKitNightlyBuilds/setup.py.patch` & `pyobjc-framework-WebKit-9.2/Examples/UsingWebKitNightlyBuilds/setup.py.patch`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/Examples/WebKitInterpreterPlugin/WebKitInterpreter.py` & `pyobjc-framework-WebKit-9.2/Examples/WebKitInterpreterPlugin/WebKitInterpreter.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/Examples/WebKitInterpreterPlugin/setup.py` & `pyobjc-framework-WebKit-9.2/Examples/WebKitInterpreterPlugin/setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/LICENSE.txt` & `pyobjc-framework-WebKit-9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/Lib/JavaScriptCore/__init__.py` & `pyobjc-framework-WebKit-9.2/Lib/JavaScriptCore/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/Lib/JavaScriptCore/_metadata.py` & `pyobjc-framework-WebKit-9.2/Lib/JavaScriptCore/_metadata.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is generated by objective.metadata
 #
-# Last update: Fri Feb 17 22:02:03 2023
+# Last update: Thu May 18 11:29:09 2023
 #
 # flake8: noqa
 
 import objc, sys
 from typing import NewType
 
 if sys.maxsize > 2**32:
@@ -41,15 +41,18 @@
         "",
         {"arguments": {5: {"type_modifier": "o"}}},
     ),
     "JSClassRetain": (b"^{OpaqueJSClass=}^{OpaqueJSClass=}",),
     "JSValueCreateJSONString": (
         b"^{OpaqueJSString=}^{OpaqueJSContext=}^{OpaqueJSValue=}I^^{OpaqueJSValue=}",
         "",
-        {"retval": {"already_cfretained": True}},
+        {
+            "retval": {"already_cfretained": True},
+            "arguments": {3: {"type_modifier": "o"}},
+        },
     ),
     "JSObjectDeletePropertyForKey": (
         b"B^{OpaqueJSContext=}^{OpaqueJSValue=}^{OpaqueJSValue=}^^{OpaqueJSValue=}",
         "",
         {"arguments": {3: {"type_modifier": "o"}}},
     ),
     "JSValueGetTypedArrayType": (
@@ -107,29 +110,44 @@
             "retval": {"c_array_of_variable_length": True},
             "arguments": {2: {"type_modifier": "o"}},
         },
     ),
     "JSValueToStringCopy": (
         b"^{OpaqueJSString=}^{OpaqueJSContext=}^{OpaqueJSValue=}^^{OpaqueJSValue=}",
         "",
-        {"retval": {"already_cfretained": True}},
+        {
+            "retval": {"already_cfretained": True},
+            "arguments": {2: {"type_modifier": "o"}},
+        },
     ),
     "JSValueIsNumber": (b"B^{OpaqueJSContext=}^{OpaqueJSValue=}",),
     "JSObjectHasProperty": (
         b"B^{OpaqueJSContext=}^{OpaqueJSValue=}^{OpaqueJSString=}",
     ),
     "JSValueIsEqual": (
         b"B^{OpaqueJSContext=}^{OpaqueJSValue=}^{OpaqueJSValue=}^^{OpaqueJSValue=}",
+        "",
+        {"arguments": {3: {"type_modifier": "o"}}},
     ),
     "JSValueIsArray": (b"B^{OpaqueJSContext=}^{OpaqueJSValue=}",),
-    "JSValueToNumber": (b"d^{OpaqueJSContext=}^{OpaqueJSValue=}^^{OpaqueJSValue=}",),
+    "JSValueToNumber": (
+        b"d^{OpaqueJSContext=}^{OpaqueJSValue=}^^{OpaqueJSValue=}",
+        "",
+        {"arguments": {2: {"type_modifier": "o"}}},
+    ),
     "JSObjectMakeDeferredPromise": (
         b"^{OpaqueJSValue=}^{OpaqueJSContext=}^^{OpaqueJSValue=}^^{OpaqueJSValue=}^^{OpaqueJSValue=}",
         "",
-        {"arguments": {1: {"type_modifier": "o"}, 2: {"type_modifier": "o"}}},
+        {
+            "arguments": {
+                1: {"type_modifier": "o"},
+                2: {"type_modifier": "o"},
+                3: {"type_modifier": "o"},
+            }
+        },
     ),
     "JSObjectGetTypedArrayByteLength": (
         b"Q^{OpaqueJSContext=}^{OpaqueJSValue=}^^{OpaqueJSValue=}",
         "",
         {"arguments": {2: {"type_modifier": "o"}}},
     ),
     "JSValueUnprotect": (b"v^{OpaqueJSContext=}^{OpaqueJSValue=}",),
@@ -153,14 +171,16 @@
             }
         },
     ),
     "JSPropertyNameArrayGetCount": (b"Q^{OpaqueJSPropertyNameArray=}",),
     "JSStringGetLength": (b"Q^{OpaqueJSString=}",),
     "JSValueToObject": (
         b"^{OpaqueJSValue=}^{OpaqueJSContext=}^{OpaqueJSValue=}^^{OpaqueJSValue=}",
+        "",
+        {"arguments": {2: {"type_modifier": "o"}}},
     ),
     "JSValueIsString": (b"B^{OpaqueJSContext=}^{OpaqueJSValue=}",),
     "JSObjectCopyPropertyNames": (
         b"^{OpaqueJSPropertyNameArray=}^{OpaqueJSContext=}^{OpaqueJSValue=}",
         "",
         {"retval": {"already_cfretained": True}},
     ),
@@ -206,14 +226,16 @@
                 4: {"type_modifier": "o"},
             }
         },
     ),
     "JSObjectIsFunction": (b"B^{OpaqueJSContext=}^{OpaqueJSValue=}",),
     "JSValueIsInstanceOfConstructor": (
         b"B^{OpaqueJSContext=}^{OpaqueJSValue=}^{OpaqueJSValue=}^^{OpaqueJSValue=}",
+        "",
+        {"arguments": {3: {"type_modifier": "o"}}},
     ),
     "JSCheckScriptSyntax": (
         b"B^{OpaqueJSContext=}^{OpaqueJSString=}^{OpaqueJSString=}i^^{OpaqueJSValue=}",
         "",
         {"arguments": {4: {"type_modifier": "o"}}},
     ),
     "JSObjectIsConstructor": (b"B^{OpaqueJSContext=}^{OpaqueJSValue=}",),
```

### Comparing `pyobjc-framework-WebKit-9.1b1/Lib/JavaScriptCore/_util.py` & `pyobjc-framework-WebKit-9.2/Lib/JavaScriptCore/_util.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/Lib/WebKit/__init__.py` & `pyobjc-framework-WebKit-9.2/Lib/WebKit/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/Lib/WebKit/_metadata.py` & `pyobjc-framework-WebKit-9.2/Lib/WebKit/_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is generated by objective.metadata
 #
-# Last update: Fri Feb 17 22:02:03 2023
+# Last update: Thu May 18 11:29:08 2023
 #
 # flake8: noqa
 
 import objc, sys
 from typing import NewType
 
 if sys.maxsize > 2**32:
```

### Comparing `pyobjc-framework-WebKit-9.1b1/Lib/pyobjc_framework_WebKit.egg-info/PKG-INFO` & `pyobjc-framework-WebKit-9.2/Lib/pyobjc_framework_WebKit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-WebKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework WebKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,WebKit,JavaScriptCore
 Platform: MacOS X
```

### Comparing `pyobjc-framework-WebKit-9.1b1/Lib/pyobjc_framework_WebKit.egg-info/SOURCES.txt` & `pyobjc-framework-WebKit-9.2/Lib/pyobjc_framework_WebKit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE.txt
 MANIFEST.in
 README.txt
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Examples/IEWebArchive/00Todo.txt
 Examples/IEWebArchive/MHTDocument.py
 Examples/IEWebArchive/loader.py
 Examples/IEWebArchive/main.py
 Examples/IEWebArchive/python-home.mht
 Examples/IEWebArchive/python-home.webarchive
```

### Comparing `pyobjc-framework-WebKit-9.1b1/Modules/_WebKit.m` & `pyobjc-framework-WebKit-9.2/Modules/_WebKit.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/Modules/_WebKit_protocols.m` & `pyobjc-framework-WebKit-9.2/Modules/_WebKit_protocols.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-WebKit-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-WebKit-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-WebKit-9.1b1/PKG-INFO` & `pyobjc-framework-WebKit-9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-WebKit
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework WebKit on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,WebKit,JavaScriptCore
 Platform: MacOS X
```

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domcssprimitivevalue.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_domcssprimitivevalue.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domcssrule.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_domcssrule.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domdocument.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_domdocument.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domelement.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_domelement.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domevent.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_domevent.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domeventtarget.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_domeventtarget.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domexception.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_domexception.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domhtmlbuttonelement.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_domhtmlbuttonelement.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domhtmlinputelement.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_domhtmlinputelement.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domhtmloptionelement.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_domhtmloptionelement.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domhtmlselectelement.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_domhtmlselectelement.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domhtmltextareaelement.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_domhtmltextareaelement.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domkeyboardevent.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_domkeyboardevent.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_dommouseevent.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_dommouseevent.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_dommutationevent.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_dommutationevent.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domnode.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_domnode.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domnodefilter.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_domnodefilter.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domoverflowevent.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_domoverflowevent.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domrange.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_domrange.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domtraversal.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_domtraversal.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domwheelevent.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_domwheelevent.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_domxpathresult.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_domxpathresult.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_jsbase.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_jsbase.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_jscontext.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_jscontext.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_jscontextref.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_jscontextref.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_jsexport.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_jsexport.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_jsobjectref.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_jsobjectref.py`

 * *Files 0% similar despite different names*

```diff
@@ -553,14 +553,15 @@
         self.assertArgIsIn(func, 4)
         self.assertArgIsOut(func, 5)
 
     @min_os_level("10.15")
     def test_functions10_15(self):
         self.assertArgIsOut(JavaScriptCore.JSObjectMakeDeferredPromise, 1)
         self.assertArgIsOut(JavaScriptCore.JSObjectMakeDeferredPromise, 2)
+        self.assertArgIsOut(JavaScriptCore.JSObjectMakeDeferredPromise, 3)
 
         self.assertArgIsOut(JavaScriptCore.JSObjectHasPropertyForKey, 3)
 
         self.assertArgIsOut(JavaScriptCore.JSObjectGetPropertyForKey, 3)
 
         self.assertArgIsOut(JavaScriptCore.JSObjectSetPropertyForKey, 5)
```

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_jsstringref.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_jsstringref.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_jsstringrefcf.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_jsstringrefcf.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_jstypedarray.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_jstypedarray.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_jsvalue.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_jsvalue.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_jsvalueref.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_jsvalueref.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,18 +36,20 @@
         self.assertResultHasType(JavaScriptCore.JSValueIsNull, objc._C_BOOL)
         self.assertResultHasType(JavaScriptCore.JSValueIsBoolean, objc._C_BOOL)
         self.assertResultHasType(JavaScriptCore.JSValueIsNumber, objc._C_BOOL)
         self.assertResultHasType(JavaScriptCore.JSValueIsString, objc._C_BOOL)
         self.assertResultHasType(JavaScriptCore.JSValueIsObject, objc._C_BOOL)
         self.assertResultHasType(JavaScriptCore.JSValueIsObjectOfClass, objc._C_BOOL)
         self.assertResultHasType(JavaScriptCore.JSValueIsEqual, objc._C_BOOL)
+        self.assertArgIsOut(JavaScriptCore.JSValueIsEqual, 3)
         self.assertResultHasType(JavaScriptCore.JSValueIsStrictEqual, objc._C_BOOL)
         self.assertResultHasType(
             JavaScriptCore.JSValueIsInstanceOfConstructor, objc._C_BOOL
         )
+        self.assertArgIsOut(JavaScriptCore.JSValueIsInstanceOfConstructor, 3)
 
         self.assertResultHasType(
             JavaScriptCore.JSValueMakeUndefined, JavaScriptCore.JSValueRef.__typestr__
         )
         self.assertResultHasType(
             JavaScriptCore.JSValueMakeNull, JavaScriptCore.JSValueRef.__typestr__
         )
@@ -64,23 +66,27 @@
             JavaScriptCore.JSValueMakeFromJSONString,
             JavaScriptCore.JSValueRef.__typestr__,
         )
         self.assertResultHasType(
             JavaScriptCore.JSValueCreateJSONString,
             JavaScriptCore.JSStringRef.__typestr__,
         )
+        self.assertArgIsOut(JavaScriptCore.JSValueCreateJSONString, 3)
 
         self.assertResultHasType(JavaScriptCore.JSValueToBoolean, objc._C_BOOL)
         self.assertResultHasType(JavaScriptCore.JSValueToNumber, objc._C_DBL)
+        self.assertArgIsOut(JavaScriptCore.JSValueToNumber, 2)
         self.assertResultHasType(
             JavaScriptCore.JSValueToStringCopy, JavaScriptCore.JSStringRef.__typestr__
         )
+        self.assertArgIsOut(JavaScriptCore.JSValueToStringCopy, 2)
         self.assertResultHasType(
             JavaScriptCore.JSValueToObject, JavaScriptCore.JSObjectRef.__typestr__
         )
+        self.assertArgIsOut(JavaScriptCore.JSValueToObject, 2)
 
         self.assertArgHasType(
             JavaScriptCore.JSValueProtect, 0, JavaScriptCore.JSContextRef.__typestr__
         )
         self.assertArgHasType(
             JavaScriptCore.JSValueUnprotect, 0, JavaScriptCore.JSContextRef.__typestr__
         )
```

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_nsattributedstring.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_nsattributedstring.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_webdocument.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_webdocument.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_webeditingdelegate.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_webeditingdelegate.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_webframeloaddelegate.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_webframeloaddelegate.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_webhistory.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_webhistory.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_webjavaplugin.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_webjavaplugin.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_webkit.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_webkit.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_webkitavailability.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_webkitavailability.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_webkiterrors.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_webkiterrors.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_webpluginviewfactory.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_webpluginviewfactory.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_webpolicydelegate.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_webpolicydelegate.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_webpreferences.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_webpreferences.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_webresourceloaddelegate.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_webresourceloaddelegate.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_webscriptobject.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_webscriptobject.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_webuidelegate.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_webuidelegate.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_webview.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_webview.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_wkcontentruleliststore.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_wkcontentruleliststore.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_wkdownloaddelegate.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_wkdownloaddelegate.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_wkerror.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_wkerror.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_wkfindconfiguration.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_wkfindconfiguration.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_wknavigationaction.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_wknavigationaction.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_wknavigationdelegate.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_wknavigationdelegate.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_wkpreferences.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_wkpreferences.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_wkscriptmessagehandlerwithreply.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_wkscriptmessagehandlerwithreply.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_wkuidelegate.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_wkuidelegate.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_wkuserscript.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_wkuserscript.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_wkwebpagepreferences.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_wkwebpagepreferences.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_wkwebsitedatarecord.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_wkwebsitedatarecord.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_wkwebsitedatastore.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_wkwebsitedatastore.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_wkwebview.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_wkwebview.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/PyObjCTest/test_wkwebviewconfiguration.py` & `pyobjc-framework-WebKit-9.2/PyObjCTest/test_wkwebviewconfiguration.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/metadata/JavaScriptCore.fwinfo` & `pyobjc-framework-WebKit-9.2/metadata/JavaScriptCore.fwinfo`

 * *Files 0% similar despite different names*

```diff
@@ -679,15 +679,16 @@
      }
     },
     "retval": {}
    },
    "JSObjectMakeDeferredPromise": {
     "args": {
      "1": { "type_modifier": "o" },
-     "2": { "type_modifier": "o" }
+     "2": { "type_modifier": "o" },
+     "3": { "type_modifier": "o" }
     }
    },
    "JSObjectMakeDate": {
     "args": {
      "0": {},
      "2": { "type_modifier": "n", "c_array_length_in_arg": 1 },
      "3": { "type_modifier": "o" }
@@ -891,15 +892,15 @@
     },
     "retval": {}
    },
    "JSValueCreateJSONString": {
     "args": {
      "0": {},
      "1": {},
-     "3": {}
+     "3": { "type_modifier": "o" }
     },
     "retval": {
      "already_cfretained": true
     }
    },
    "JSValueGetType": {
     "args": {
@@ -914,23 +915,23 @@
     }
    },
    "JSValueIsEqual": {
     "args": {
      "0": {},
      "1": {},
      "2": {},
-     "3": {}
+     "3": { "type_modifier": "o" }
     }
    },
    "JSValueIsInstanceOfConstructor": {
     "args": {
      "0": {},
      "1": {},
      "2": {},
-     "3": {}
+     "3": { "type_modifier": "o" }
     }
    },
    "JSValueIsNull": {
     "args": {
      "0": {},
      "1": {}
     }
@@ -1023,30 +1024,30 @@
      "1": {}
     }
    },
    "JSValueToNumber": {
     "args": {
      "0": {},
      "1": {},
-     "2": {}
+     "2": { "type_modifier": "o" }
     }
    },
    "JSValueToObject": {
     "args": {
      "0": {},
      "1": {},
-     "2": {}
+     "2": { "type_modifier": "o" }
     },
     "retval": {}
    },
    "JSValueToStringCopy": {
     "args": {
      "0": {},
      "1": {},
-     "2": {}
+     "2": { "type_modifier": "o" }
     },
     "retval": {
      "already_cfretained": true
     }
    },
    "JSValueUnprotect": {
     "args": {
```

### Comparing `pyobjc-framework-WebKit-9.1b1/metadata/WebKit.fwinfo` & `pyobjc-framework-WebKit-9.2/metadata/WebKit.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/metadata/raw.jc/arm64-12.0.fwinfo` & `pyobjc-framework-WebKit-9.2/metadata/raw.jc/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/metadata/raw.jc/arm64-12.3.fwinfo` & `pyobjc-framework-WebKit-9.2/metadata/raw.jc/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/metadata/raw.jc/arm64-13.3.fwinfo` & `pyobjc-framework-WebKit-9.2/metadata/raw.jc/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/metadata/raw.jc/x86_64-10.10.fwinfo` & `pyobjc-framework-WebKit-9.2/metadata/raw.jc/x86_64-10.10.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/metadata/raw.jc/x86_64-10.14.fwinfo` & `pyobjc-framework-WebKit-9.2/metadata/raw.jc/x86_64-10.14.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/metadata/raw.jc/x86_64-10.15.fwinfo` & `pyobjc-framework-WebKit-9.2/metadata/raw.jc/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/metadata/raw.jc/x86_64-10.16.fwinfo` & `pyobjc-framework-WebKit-9.2/metadata/raw.jc/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/metadata/raw.jc/x86_64-10.6.fwinfo` & `pyobjc-framework-WebKit-9.2/metadata/raw.jc/x86_64-10.6.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/metadata/raw.jc/x86_64-10.7.fwinfo` & `pyobjc-framework-WebKit-9.2/metadata/raw.jc/x86_64-10.7.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/metadata/raw.jc/x86_64-10.8.fwinfo` & `pyobjc-framework-WebKit-9.2/metadata/raw.jc/x86_64-10.8.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/metadata/raw.jc/x86_64-12.0.fwinfo` & `pyobjc-framework-WebKit-9.2/metadata/raw.jc/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/metadata/raw.jc/x86_64-12.3.fwinfo` & `pyobjc-framework-WebKit-9.2/metadata/raw.jc/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/metadata/raw.jc/x86_64-13.3.fwinfo` & `pyobjc-framework-WebKit-9.2/metadata/raw.jc/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/metadata/raw.wk/arm64-12.0.fwinfo` & `pyobjc-framework-WebKit-9.2/metadata/raw.wk/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/metadata/raw.wk/arm64-12.3.fwinfo` & `pyobjc-framework-WebKit-9.2/metadata/raw.wk/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/metadata/raw.wk/arm64-13.0.fwinfo` & `pyobjc-framework-WebKit-9.2/metadata/raw.wk/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/metadata/raw.wk/arm64-13.3.fwinfo` & `pyobjc-framework-WebKit-9.2/metadata/raw.wk/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/metadata/raw.wk/x86_64-10.10.fwinfo` & `pyobjc-framework-WebKit-9.2/metadata/raw.wk/x86_64-10.10.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/metadata/raw.wk/x86_64-10.14.fwinfo` & `pyobjc-framework-WebKit-9.2/metadata/raw.wk/x86_64-10.14.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/metadata/raw.wk/x86_64-10.15.fwinfo` & `pyobjc-framework-WebKit-9.2/metadata/raw.wk/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/metadata/raw.wk/x86_64-10.16.fwinfo` & `pyobjc-framework-WebKit-9.2/metadata/raw.wk/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/metadata/raw.wk/x86_64-10.6.fwinfo` & `pyobjc-framework-WebKit-9.2/metadata/raw.wk/x86_64-10.6.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/metadata/raw.wk/x86_64-10.7.fwinfo` & `pyobjc-framework-WebKit-9.2/metadata/raw.wk/x86_64-10.7.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/metadata/raw.wk/x86_64-10.8.fwinfo` & `pyobjc-framework-WebKit-9.2/metadata/raw.wk/x86_64-10.8.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/metadata/raw.wk/x86_64-12.0.fwinfo` & `pyobjc-framework-WebKit-9.2/metadata/raw.wk/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/metadata/raw.wk/x86_64-12.3.fwinfo` & `pyobjc-framework-WebKit-9.2/metadata/raw.wk/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/metadata/raw.wk/x86_64-13.0.fwinfo` & `pyobjc-framework-WebKit-9.2/metadata/raw.wk/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/metadata/raw.wk/x86_64-13.3.fwinfo` & `pyobjc-framework-WebKit-9.2/metadata/raw.wk/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/pyobjc_setup.py` & `pyobjc-framework-WebKit-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-WebKit-9.1b1/setup.py` & `pyobjc-framework-WebKit-9.2/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,18 +5,22 @@
 
 These wrappers don't include documentation, please check Apple's documentation
 for information on how to use these frameworks and PyObjC's documentation
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
 
 setup(
     name="pyobjc-framework-WebKit",
     description="Wrappers for the framework WebKit on macOS",
     packages=["WebKit", "JavaScriptCore"],
     ext_modules=[
         Extension(
```

