# Comparing `tmp/pyobjc-core-9.1b1.tar.gz` & `tmp/pyobjc-core-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-core-9.1b1.tar", last modified: Sun Mar 26 10:48:33 2023, max compression
+gzip compressed data, was "pyobjc-core-9.2.tar", last modified: Tue Jun  6 23:56:14 2023, max compression
```

## Comparing `pyobjc-core-9.1b1.tar` & `pyobjc-core-9.2.tar`

### file list

```diff
@@ -1,460 +1,531 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 10:48:33.554811 pyobjc-core-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 10:48:32.493657 pyobjc-core-9.1b1/Examples/
--rw-r--r--   0 ronald     (501) staff       (20)    15940 2020-11-30 18:45:14.000000 pyobjc-core-9.1b1/Examples/00ReadMe.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 10:48:32.522386 pyobjc-core-9.1b1/Examples/GUITests/
--rw-r--r--   0 ronald     (501) staff       (20)      132 2020-11-30 18:45:14.000000 pyobjc-core-9.1b1/Examples/GUITests/00ReadMe.txt
--rwxr-xr-x   0 ronald     (501) staff       (20)     1444 2020-11-30 18:45:14.000000 pyobjc-core-9.1b1/Examples/GUITests/test_modalsession.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 10:48:32.477969 pyobjc-core-9.1b1/Examples/NonFunctional/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 10:48:32.550782 pyobjc-core-9.1b1/Examples/NonFunctional/RemotePyInterpreter/
--rw-r--r--   0 ronald     (501) staff       (20)     9185 2023-03-03 17:21:59.000000 pyobjc-core-9.1b1/Examples/NonFunctional/RemotePyInterpreter/AsyncPythonInterpreter.py
--rw-r--r--   0 ronald     (501) staff       (20)     4559 2021-07-30 09:00:36.000000 pyobjc-core-9.1b1/Examples/NonFunctional/RemotePyInterpreter/ConsoleReactor.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 10:48:32.478536 pyobjc-core-9.1b1/Examples/NonFunctional/RemotePyInterpreter/English.lproj/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 10:48:32.560267 pyobjc-core-9.1b1/Examples/NonFunctional/RemotePyInterpreter/English.lproj/MainMenu.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      109 2020-11-30 18:45:14.000000 pyobjc-core-9.1b1/Examples/NonFunctional/RemotePyInterpreter/English.lproj/MainMenu.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      605 2020-11-30 18:45:14.000000 pyobjc-core-9.1b1/Examples/NonFunctional/RemotePyInterpreter/English.lproj/MainMenu.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)   157619 2020-11-30 18:45:14.000000 pyobjc-core-9.1b1/Examples/NonFunctional/RemotePyInterpreter/English.lproj/MainMenu.nib/keyedobjects.nib
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 10:48:32.578174 pyobjc-core-9.1b1/Examples/NonFunctional/RemotePyInterpreter/English.lproj/RemotePyInterpreterDocument.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      771 2020-11-30 18:45:14.000000 pyobjc-core-9.1b1/Examples/NonFunctional/RemotePyInterpreter/English.lproj/RemotePyInterpreterDocument.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      495 2020-11-30 18:45:14.000000 pyobjc-core-9.1b1/Examples/NonFunctional/RemotePyInterpreter/English.lproj/RemotePyInterpreterDocument.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)    30650 2020-11-30 18:45:14.000000 pyobjc-core-9.1b1/Examples/NonFunctional/RemotePyInterpreter/English.lproj/RemotePyInterpreterDocument.nib/keyedobjects.nib
--rw-r--r--   0 ronald     (501) staff       (20)      343 2020-11-30 18:45:14.000000 pyobjc-core-9.1b1/Examples/NonFunctional/RemotePyInterpreter/README.txt
--rw-r--r--   0 ronald     (501) staff       (20)    16640 2021-07-30 09:00:36.000000 pyobjc-core-9.1b1/Examples/NonFunctional/RemotePyInterpreter/RemotePyInterpreter.py
--rw-r--r--   0 ronald     (501) staff       (20)     6907 2021-07-30 09:00:36.000000 pyobjc-core-9.1b1/Examples/NonFunctional/RemotePyInterpreter/netrepr.py
--rw-r--r--   0 ronald     (501) staff       (20)      585 2020-11-30 18:45:14.000000 pyobjc-core-9.1b1/Examples/NonFunctional/RemotePyInterpreter/remote_bootstrap.py
--rw-r--r--   0 ronald     (501) staff       (20)     4028 2020-11-30 18:45:14.000000 pyobjc-core-9.1b1/Examples/NonFunctional/RemotePyInterpreter/remote_console.py
--rw-r--r--   0 ronald     (501) staff       (20)     2807 2021-07-30 09:00:36.000000 pyobjc-core-9.1b1/Examples/NonFunctional/RemotePyInterpreter/remote_pipe.py
--rw-r--r--   0 ronald     (501) staff       (20)      853 2020-11-30 18:45:14.000000 pyobjc-core-9.1b1/Examples/NonFunctional/RemotePyInterpreter/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)     1492 2021-07-30 09:00:36.000000 pyobjc-core-9.1b1/Examples/NonFunctional/RemotePyInterpreter/tcpinterpreter.py
--rw-r--r--   0 ronald     (501) staff       (20)     3830 2021-07-30 09:00:36.000000 pyobjc-core-9.1b1/Examples/NonFunctional/RemotePyInterpreter/test_client.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 10:48:32.601153 pyobjc-core-9.1b1/Examples/Scripts/
--rwxr-xr-x   0 ronald     (501) staff       (20)     2467 2021-10-18 19:38:40.000000 pyobjc-core-9.1b1/Examples/Scripts/HelloWorld.py
--rwxr-xr-x   0 ronald     (501) staff       (20)     1832 2023-03-03 17:21:59.000000 pyobjc-core-9.1b1/Examples/Scripts/autoreadme.py
--rw-r--r--   0 ronald     (501) staff       (20)     1269 2020-11-30 18:45:14.000000 pyobjc-core-9.1b1/Examples/Scripts/instrumentSends.py
--rw-r--r--   0 ronald     (501) staff       (20)     3775 2021-07-30 09:00:36.000000 pyobjc-core-9.1b1/Examples/Scripts/kvo-debugging.py
--rw-r--r--   0 ronald     (501) staff       (20)      477 2020-11-30 18:45:14.000000 pyobjc-core-9.1b1/Examples/Scripts/signal-demo.py
--rw-r--r--   0 ronald     (501) staff       (20)     2649 2021-10-18 19:38:40.000000 pyobjc-core-9.1b1/Examples/Scripts/stdinreader.py
--rw-r--r--   0 ronald     (501) staff       (20)     1656 2020-11-30 18:45:14.000000 pyobjc-core-9.1b1/Examples/Scripts/subclassing-objective-c.py
--rw-r--r--   0 ronald     (501) staff       (20)     2535 2023-03-03 17:21:59.000000 pyobjc-core-9.1b1/Examples/Scripts/wmEnable.py
--rw-r--r--   0 ronald     (501) staff       (20)     6282 2020-11-30 18:45:14.000000 pyobjc-core-9.1b1/HISTORIC.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1323 2020-11-30 18:45:14.000000 pyobjc-core-9.1b1/Install.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 10:48:32.479425 pyobjc-core-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 10:48:32.604766 pyobjc-core-9.1b1/Lib/PyObjCTools/
--rw-r--r--   0 ronald     (501) staff       (20)    10350 2021-10-18 19:38:40.000000 pyobjc-core-9.1b1/Lib/PyObjCTools/KeyValueCoding.py
--rw-r--r--   0 ronald     (501) staff       (20)     1218 2022-01-02 11:04:25.000000 pyobjc-core-9.1b1/Lib/PyObjCTools/MachSignals.py
--rw-r--r--   0 ronald     (501) staff       (20)     2483 2022-01-02 11:04:25.000000 pyobjc-core-9.1b1/Lib/PyObjCTools/Signals.py
--rw-r--r--   0 ronald     (501) staff       (20)    44286 2023-03-25 15:03:24.000000 pyobjc-core-9.1b1/Lib/PyObjCTools/TestSupport.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 10:48:32.637077 pyobjc-core-9.1b1/Lib/objc/
--rw-r--r--   0 ronald     (501) staff       (20)     2724 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Lib/objc/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     1714 2022-02-06 09:24:04.000000 pyobjc-core-9.1b1/Lib/objc/_bridges.py
--rw-r--r--   0 ronald     (501) staff       (20)    26273 2023-03-26 10:43:00.000000 pyobjc-core-9.1b1/Lib/objc/_bridgesupport.py
--rw-r--r--   0 ronald     (501) staff       (20)    10129 2023-03-03 17:21:59.000000 pyobjc-core-9.1b1/Lib/objc/_callable_docstr.py
--rw-r--r--   0 ronald     (501) staff       (20)     2638 2022-01-02 11:04:25.000000 pyobjc-core-9.1b1/Lib/objc/_category.py
--rw-r--r--   0 ronald     (501) staff       (20)      893 2022-06-23 11:03:27.000000 pyobjc-core-9.1b1/Lib/objc/_compat.py
--rw-r--r--   0 ronald     (501) staff       (20)     1317 2021-07-30 09:00:36.000000 pyobjc-core-9.1b1/Lib/objc/_context.py
--rw-r--r--   0 ronald     (501) staff       (20)     3558 2022-06-30 10:21:22.000000 pyobjc-core-9.1b1/Lib/objc/_convenience.py
--rw-r--r--   0 ronald     (501) staff       (20)     3419 2021-10-18 19:38:40.000000 pyobjc-core-9.1b1/Lib/objc/_convenience_mapping.py
--rw-r--r--   0 ronald     (501) staff       (20)    10994 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Lib/objc/_convenience_nsarray.py
--rw-r--r--   0 ronald     (501) staff       (20)    11205 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Lib/objc/_convenience_nsdata.py
--rw-r--r--   0 ronald     (501) staff       (20)     3782 2021-10-18 19:38:40.000000 pyobjc-core-9.1b1/Lib/objc/_convenience_nsdecimal.py
--rw-r--r--   0 ronald     (501) staff       (20)     8263 2022-01-02 11:04:25.000000 pyobjc-core-9.1b1/Lib/objc/_convenience_nsdictionary.py
--rw-r--r--   0 ronald     (501) staff       (20)     3056 2021-07-30 09:00:36.000000 pyobjc-core-9.1b1/Lib/objc/_convenience_nsobject.py
--rw-r--r--   0 ronald     (501) staff       (20)     8714 2021-07-30 09:00:36.000000 pyobjc-core-9.1b1/Lib/objc/_convenience_nsset.py
--rw-r--r--   0 ronald     (501) staff       (20)      576 2020-11-30 18:45:14.000000 pyobjc-core-9.1b1/Lib/objc/_convenience_nsstring.py
--rw-r--r--   0 ronald     (501) staff       (20)     1252 2020-11-30 18:45:14.000000 pyobjc-core-9.1b1/Lib/objc/_convenience_sequence.py
--rw-r--r--   0 ronald     (501) staff       (20)    11927 2022-03-02 19:57:48.000000 pyobjc-core-9.1b1/Lib/objc/_descriptors.py
--rw-r--r--   0 ronald     (501) staff       (20)     4216 2022-01-02 11:04:25.000000 pyobjc-core-9.1b1/Lib/objc/_dyld.py
--rw-r--r--   0 ronald     (501) staff       (20)      634 2020-11-30 18:45:14.000000 pyobjc-core-9.1b1/Lib/objc/_framework.py
--rw-r--r--   0 ronald     (501) staff       (20)     2212 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Lib/objc/_informal_protocol.py
--rw-r--r--   0 ronald     (501) staff       (20)    16696 2023-03-03 17:21:59.000000 pyobjc-core-9.1b1/Lib/objc/_lazyimport.py
--rw-r--r--   0 ronald     (501) staff       (20)      898 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Lib/objc/_locking.py
--rw-r--r--   0 ronald     (501) staff       (20)    33278 2023-03-03 17:21:59.000000 pyobjc-core-9.1b1/Lib/objc/_properties.py
--rw-r--r--   0 ronald     (501) staff       (20)      898 2021-07-30 09:00:36.000000 pyobjc-core-9.1b1/Lib/objc/_protocols.py
--rw-r--r--   0 ronald     (501) staff       (20)    16349 2023-03-03 17:21:59.000000 pyobjc-core-9.1b1/Lib/objc/_pycoder.py
--rw-r--r--   0 ronald     (501) staff       (20)     2044 2021-07-30 09:00:36.000000 pyobjc-core-9.1b1/Lib/objc/_pythonify.py
--rw-r--r--   0 ronald     (501) staff       (20)     2230 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Lib/objc/_structtype.py
--rw-r--r--   0 ronald     (501) staff       (20)    22689 2023-03-03 17:20:38.000000 pyobjc-core-9.1b1/Lib/objc/_transform.py
--rw-r--r--   0 ronald     (501) staff       (20)    14079 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Lib/objc/simd.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 10:48:32.668654 pyobjc-core-9.1b1/Lib/pyobjc_core.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2451 2023-03-26 10:48:32.000000 pyobjc-core-9.1b1/Lib/pyobjc_core.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)    13746 2023-03-26 10:48:32.000000 pyobjc-core-9.1b1/Lib/pyobjc_core.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 10:48:32.000000 pyobjc-core-9.1b1/Lib/pyobjc_core.egg-info/dependency_links.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 10:48:32.669736 pyobjc-core-9.1b1/Lib/pyobjc_core.egg-info/include/
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-03-26 10:48:32.000000 pyobjc-core-9.1b1/Lib/pyobjc_core.egg-info/include/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-26 10:48:32.000000 pyobjc-core-9.1b1/Lib/pyobjc_core.egg-info/include/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:46:57.000000 pyobjc-core-9.1b1/Lib/pyobjc_core.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       28 2023-03-26 10:48:32.000000 pyobjc-core-9.1b1/Lib/pyobjc_core.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-core-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)    64814 2020-11-30 18:45:14.000000 pyobjc-core-9.1b1/MANIFEST
--rw-r--r--   0 ronald     (501) staff       (20)      317 2021-03-21 10:08:22.000000 pyobjc-core-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 10:48:32.683601 pyobjc-core-9.1b1/Misc/
--rw-r--r--   0 ronald     (501) staff       (20)     2377 2020-11-30 18:45:14.000000 pyobjc-core-9.1b1/Misc/announcement.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 10:48:32.707136 pyobjc-core-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)     4767 2022-02-06 09:24:04.000000 pyobjc-core-9.1b1/Modules/_machsignals.m
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 10:48:32.955074 pyobjc-core-9.1b1/Modules/objc/
--rw-r--r--   0 ronald     (501) staff       (20)      146 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/OC_BuiltinPythonArray.h
--rw-r--r--   0 ronald     (501) staff       (20)      373 2021-10-18 19:38:40.000000 pyobjc-core-9.1b1/Modules/objc/OC_BuiltinPythonArray.m
--rw-r--r--   0 ronald     (501) staff       (20)      144 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/OC_BuiltinPythonData.h
--rw-r--r--   0 ronald     (501) staff       (20)      282 2022-02-06 09:24:04.000000 pyobjc-core-9.1b1/Modules/objc/OC_BuiltinPythonData.m
--rw-r--r--   0 ronald     (501) staff       (20)      144 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/OC_BuiltinPythonDate.h
--rw-r--r--   0 ronald     (501) staff       (20)      282 2022-02-06 09:24:04.000000 pyobjc-core-9.1b1/Modules/objc/OC_BuiltinPythonDate.m
--rw-r--r--   0 ronald     (501) staff       (20)      156 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/OC_BuiltinPythonDictionary.h
--rw-r--r--   0 ronald     (501) staff       (20)      393 2021-10-18 19:38:40.000000 pyobjc-core-9.1b1/Modules/objc/OC_BuiltinPythonDictionary.m
--rw-r--r--   0 ronald     (501) staff       (20)      148 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/OC_BuiltinPythonNumber.h
--rw-r--r--   0 ronald     (501) staff       (20)      626 2022-01-02 11:20:34.000000 pyobjc-core-9.1b1/Modules/objc/OC_BuiltinPythonNumber.m
--rw-r--r--   0 ronald     (501) staff       (20)      142 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/OC_BuiltinPythonSet.h
--rw-r--r--   0 ronald     (501) staff       (20)      365 2021-10-18 19:38:40.000000 pyobjc-core-9.1b1/Modules/objc/OC_BuiltinPythonSet.m
--rw-r--r--   0 ronald     (501) staff       (20)      150 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/OC_BuiltinPythonUnicode.h
--rw-r--r--   0 ronald     (501) staff       (20)      379 2021-10-18 19:38:40.000000 pyobjc-core-9.1b1/Modules/objc/OC_BuiltinPythonUnicode.m
--rw-r--r--   0 ronald     (501) staff       (20)      731 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/OC_NSBundleHack.h
--rw-r--r--   0 ronald     (501) staff       (20)     3364 2022-02-06 09:24:04.000000 pyobjc-core-9.1b1/Modules/objc/OC_NSBundleHack.m
--rw-r--r--   0 ronald     (501) staff       (20)     3302 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/OC_PythonArray.h
--rw-r--r--   0 ronald     (501) staff       (20)    17717 2022-03-17 11:48:54.000000 pyobjc-core-9.1b1/Modules/objc/OC_PythonArray.m
--rw-r--r--   0 ronald     (501) staff       (20)     1845 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/OC_PythonData.h
--rw-r--r--   0 ronald     (501) staff       (20)     9389 2022-02-24 08:48:42.000000 pyobjc-core-9.1b1/Modules/objc/OC_PythonData.m
--rw-r--r--   0 ronald     (501) staff       (20)      361 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/OC_PythonDate.h
--rw-r--r--   0 ronald     (501) staff       (20)    10104 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/OC_PythonDate.m
--rw-r--r--   0 ronald     (501) staff       (20)     1511 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/OC_PythonDictionary.h
--rw-r--r--   0 ronald     (501) staff       (20)    15291 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/OC_PythonDictionary.m
--rw-r--r--   0 ronald     (501) staff       (20)      383 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/OC_PythonEnumerator.h
--rw-r--r--   0 ronald     (501) staff       (20)     2409 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/OC_PythonEnumerator.m
--rw-r--r--   0 ronald     (501) staff       (20)      372 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/OC_PythonNumber.h
--rw-r--r--   0 ronald     (501) staff       (20)    15050 2022-06-23 11:03:27.000000 pyobjc-core-9.1b1/Modules/objc/OC_PythonNumber.m
--rw-r--r--   0 ronald     (501) staff       (20)     3550 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/OC_PythonObject.h
--rw-r--r--   0 ronald     (501) staff       (20)    32682 2022-10-19 07:22:30.000000 pyobjc-core-9.1b1/Modules/objc/OC_PythonObject.m
--rw-r--r--   0 ronald     (501) staff       (20)      333 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/OC_PythonSet.h
--rw-r--r--   0 ronald     (501) staff       (20)    13924 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/OC_PythonSet.m
--rw-r--r--   0 ronald     (501) staff       (20)     1600 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/OC_PythonUnicode.h
--rw-r--r--   0 ronald     (501) staff       (20)    12786 2022-12-17 10:07:28.000000 pyobjc-core-9.1b1/Modules/objc/OC_PythonUnicode.m
--rw-r--r--   0 ronald     (501) staff       (20)      767 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/ObjCPointer.h
--rw-r--r--   0 ronald     (501) staff       (20)     4772 2023-02-19 10:59:41.000000 pyobjc-core-9.1b1/Modules/objc/ObjCPointer.m
--rw-r--r--   0 ronald     (501) staff       (20)      776 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/block_support.h
--rw-r--r--   0 ronald     (501) staff       (20)    18742 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/block_support.m
--rw-r--r--   0 ronald     (501) staff       (20)      965 2021-10-18 19:38:40.000000 pyobjc-core-9.1b1/Modules/objc/bundle-variables.h
--rw-r--r--   0 ronald     (501) staff       (20)    13729 2022-10-18 09:53:23.000000 pyobjc-core-9.1b1/Modules/objc/bundle-variables.m
--rw-r--r--   0 ronald     (501) staff       (20)      385 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/class-builder.h
--rw-r--r--   0 ronald     (501) staff       (20)    38209 2023-03-26 10:08:20.000000 pyobjc-core-9.1b1/Modules/objc/class-builder.m
--rw-r--r--   0 ronald     (501) staff       (20)      589 2022-01-02 11:04:25.000000 pyobjc-core-9.1b1/Modules/objc/class-list.h
--rw-r--r--   0 ronald     (501) staff       (20)     2036 2022-02-06 09:24:04.000000 pyobjc-core-9.1b1/Modules/objc/class-list.m
--rw-r--r--   0 ronald     (501) staff       (20)      677 2022-02-06 09:24:04.000000 pyobjc-core-9.1b1/Modules/objc/closure_pool.h
--rw-r--r--   0 ronald     (501) staff       (20)     3023 2022-02-06 09:24:04.000000 pyobjc-core-9.1b1/Modules/objc/closure_pool.m
--rw-r--r--   0 ronald     (501) staff       (20)      531 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/corefoundation.h
--rw-r--r--   0 ronald     (501) staff       (20)    11124 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/corefoundation.m
--rw-r--r--   0 ronald     (501) staff       (20)      169 2021-10-18 19:38:40.000000 pyobjc-core-9.1b1/Modules/objc/ctests.h
--rw-r--r--   0 ronald     (501) staff       (20)    31484 2023-02-19 13:33:58.000000 pyobjc-core-9.1b1/Modules/objc/ctests.m
--rw-r--r--   0 ronald     (501) staff       (20)      281 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/file_wrapper.h
--rw-r--r--   0 ronald     (501) staff       (20)    10599 2023-02-19 11:01:59.000000 pyobjc-core-9.1b1/Modules/objc/file_wrapper.m
--rw-r--r--   0 ronald     (501) staff       (20)      562 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/formal-protocol.h
--rw-r--r--   0 ronald     (501) staff       (20)    17150 2023-03-24 18:54:07.000000 pyobjc-core-9.1b1/Modules/objc/formal-protocol.m
--rw-r--r--   0 ronald     (501) staff       (20)      684 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/fsref.h
--rw-r--r--   0 ronald     (501) staff       (20)     5585 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/fsref.m
--rw-r--r--   0 ronald     (501) staff       (20)      625 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/function.h
--rw-r--r--   0 ronald     (501) staff       (20)    18319 2023-02-19 11:02:35.000000 pyobjc-core-9.1b1/Modules/objc/function.m
--rw-r--r--   0 ronald     (501) staff       (20)     5914 2022-10-18 09:53:23.000000 pyobjc-core-9.1b1/Modules/objc/helpers-authorization.m
--rw-r--r--   0 ronald     (501) staff       (20)    44063 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/helpers-foundation-nscoder.m
--rw-r--r--   0 ronald     (501) staff       (20)     7317 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/helpers-foundation-nsdata.m
--rw-r--r--   0 ronald     (501) staff       (20)    36267 2023-02-19 11:03:10.000000 pyobjc-core-9.1b1/Modules/objc/helpers-foundation-nsdecimal.m
--rw-r--r--   0 ronald     (501) staff       (20)     9933 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/helpers-foundation-nsinvocation.m
--rw-r--r--   0 ronald     (501) staff       (20)    13648 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/helpers-foundation-nsobject.m
--rw-r--r--   0 ronald     (501) staff       (20)   491043 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/helpers-vector.m
--rw-r--r--   0 ronald     (501) staff       (20)      861 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/helpers.h
--rw-r--r--   0 ronald     (501) staff       (20)     1115 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/instance-var.h
--rw-r--r--   0 ronald     (501) staff       (20)    17605 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/instance-var.m
--rw-r--r--   0 ronald     (501) staff       (20)      529 2021-10-18 19:38:40.000000 pyobjc-core-9.1b1/Modules/objc/ivar-accessor.h
--rw-r--r--   0 ronald     (501) staff       (20)     8594 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/ivar-accessor.m
--rw-r--r--   0 ronald     (501) staff       (20)      460 2022-01-02 11:04:25.000000 pyobjc-core-9.1b1/Modules/objc/libffi_extra.h
--rw-r--r--   0 ronald     (501) staff       (20)     2584 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/libffi_extra.m
--rw-r--r--   0 ronald     (501) staff       (20)     4877 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/libffi_support.h
--rw-r--r--   0 ronald     (501) staff       (20)   177231 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/libffi_support.m
--rw-r--r--   0 ronald     (501) staff       (20)      349 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/memview.h
--rw-r--r--   0 ronald     (501) staff       (20)     3327 2023-02-19 11:04:02.000000 pyobjc-core-9.1b1/Modules/objc/memview.m
--rw-r--r--   0 ronald     (501) staff       (20)      804 2022-10-18 09:53:23.000000 pyobjc-core-9.1b1/Modules/objc/meth-func.h
--rw-r--r--   0 ronald     (501) staff       (20)     6616 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/meth-func.m
--rw-r--r--   0 ronald     (501) staff       (20)      298 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/method-accessor.h
--rw-r--r--   0 ronald     (501) staff       (20)    19379 2023-02-19 11:04:33.000000 pyobjc-core-9.1b1/Modules/objc/method-accessor.m
--rw-r--r--   0 ronald     (501) staff       (20)     1738 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/method-imp.h
--rw-r--r--   0 ronald     (501) staff       (20)    20511 2023-02-19 11:04:59.000000 pyobjc-core-9.1b1/Modules/objc/method-imp.m
--rw-r--r--   0 ronald     (501) staff       (20)     3682 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/method-signature.h
--rw-r--r--   0 ronald     (501) staff       (20)    65997 2023-03-24 18:54:07.000000 pyobjc-core-9.1b1/Modules/objc/method-signature.m
--rw-r--r--   0 ronald     (501) staff       (20)    84210 2023-02-19 12:25:01.000000 pyobjc-core-9.1b1/Modules/objc/module.m
--rw-r--r--   0 ronald     (501) staff       (20)      202 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/objc-NULL.h
--rw-r--r--   0 ronald     (501) staff       (20)     1913 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/objc-NULL.m
--rw-r--r--   0 ronald     (501) staff       (20)     6317 2022-02-06 09:24:04.000000 pyobjc-core-9.1b1/Modules/objc/objc-class.h
--rw-r--r--   0 ronald     (501) staff       (20)   105026 2023-03-03 17:19:39.000000 pyobjc-core-9.1b1/Modules/objc/objc-class.m
--rw-r--r--   0 ronald     (501) staff       (20)     2256 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/objc-object.h
--rw-r--r--   0 ronald     (501) staff       (20)    41422 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/objc-object.m
--rw-r--r--   0 ronald     (501) staff       (20)     1816 2023-03-24 18:54:07.000000 pyobjc-core-9.1b1/Modules/objc/objc-runtime-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1598 2023-03-24 18:54:07.000000 pyobjc-core-9.1b1/Modules/objc/objc-runtime-compat.m
--rw-r--r--   0 ronald     (501) staff       (20)      172 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/objc_super.h
--rw-r--r--   0 ronald     (501) staff       (20)     7134 2023-03-03 17:19:39.000000 pyobjc-core-9.1b1/Modules/objc/objc_super.m
--rw-r--r--   0 ronald     (501) staff       (20)     4541 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/objc_support.h
--rw-r--r--   0 ronald     (501) staff       (20)    99903 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/objc_support.m
--rw-r--r--   0 ronald     (501) staff       (20)     5713 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/objc_util.h
--rw-r--r--   0 ronald     (501) staff       (20)    47205 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/objc_util.m
--rw-r--r--   0 ronald     (501) staff       (20)      392 2021-10-18 19:38:40.000000 pyobjc-core-9.1b1/Modules/objc/opaque-pointer.h
--rw-r--r--   0 ronald     (501) staff       (20)    13600 2022-04-11 08:03:15.000000 pyobjc-core-9.1b1/Modules/objc/opaque-pointer.m
--rw-r--r--   0 ronald     (501) staff       (20)     1462 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/options.h
--rw-r--r--   0 ronald     (501) staff       (20)    16737 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/options.m
--rw-r--r--   0 ronald     (501) staff       (20)     1165 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/pointer-support.h
--rw-r--r--   0 ronald     (501) staff       (20)     9538 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/pointer-support.m
--rw-r--r--   0 ronald     (501) staff       (20)     1027 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/proxy-registry.h
--rw-r--r--   0 ronald     (501) staff       (20)     2766 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/proxy-registry.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)     3118 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/pyobjc-api.m
--rw-r--r--   0 ronald     (501) staff       (20)     3105 2022-02-06 09:24:04.000000 pyobjc-core-9.1b1/Modules/objc/pyobjc-assert.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-02-19 12:24:44.000000 pyobjc-core-9.1b1/Modules/objc/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     5379 2022-03-17 11:48:54.000000 pyobjc-core-9.1b1/Modules/objc/pyobjc-compat.m
--rw-r--r--   0 ronald     (501) staff       (20)     5911 2021-10-18 19:38:40.000000 pyobjc-core-9.1b1/Modules/objc/pyobjc-unittest.h
--rw-r--r--   0 ronald     (501) staff       (20)     4785 2023-03-25 14:20:23.000000 pyobjc-core-9.1b1/Modules/objc/pyobjc.h
--rw-r--r--   0 ronald     (501) staff       (20)      435 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/pyobjc_unicode.h
--rw-r--r--   0 ronald     (501) staff       (20)    16531 2023-03-26 10:00:44.000000 pyobjc-core-9.1b1/Modules/objc/pyobjc_unicode.m
--rw-r--r--   0 ronald     (501) staff       (20)    22716 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/python-api-used.h
--rw-r--r--   0 ronald     (501) staff       (20)      482 2021-10-18 19:38:40.000000 pyobjc-core-9.1b1/Modules/objc/registry.h
--rw-r--r--   0 ronald     (501) staff       (20)     5666 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/registry.m
--rw-r--r--   0 ronald     (501) staff       (20)      747 2022-02-24 08:48:42.000000 pyobjc-core-9.1b1/Modules/objc/released-buffer.h
--rw-r--r--   0 ronald     (501) staff       (20)     1187 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/released-buffer.m
--rw-r--r--   0 ronald     (501) staff       (20)     4090 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/selector.h
--rw-r--r--   0 ronald     (501) staff       (20)    71123 2023-03-03 17:19:39.000000 pyobjc-core-9.1b1/Modules/objc/selector.m
--rw-r--r--   0 ronald     (501) staff       (20)      386 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/struct-sockaddr.h
--rw-r--r--   0 ronald     (501) staff       (20)     8929 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/struct-sockaddr.m
--rw-r--r--   0 ronald     (501) staff       (20)     6064 2022-01-02 11:04:25.000000 pyobjc-core-9.1b1/Modules/objc/struct-wrapper.h
--rw-r--r--   0 ronald     (501) staff       (20)    50114 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/struct-wrapper.m
--rw-r--r--   0 ronald     (501) staff       (20)     4174 2022-10-18 09:53:23.000000 pyobjc-core-9.1b1/Modules/objc/super-call.h
--rw-r--r--   0 ronald     (501) staff       (20)    12681 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/super-call.m
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 10:48:33.114736 pyobjc-core-9.1b1/Modules/objc/test/
--rw-r--r--   0 ronald     (501) staff       (20)     2570 2021-09-25 14:12:36.000000 pyobjc-core-9.1b1/Modules/objc/test/NULL.m
--rw-r--r--   0 ronald     (501) staff       (20)     3083 2022-02-06 09:24:04.000000 pyobjc-core-9.1b1/Modules/objc/test/arrayint.m
--rw-r--r--   0 ronald     (501) staff       (20)     8587 2021-09-25 14:12:36.000000 pyobjc-core-9.1b1/Modules/objc/test/arrays.m
--rw-r--r--   0 ronald     (501) staff       (20)     5752 2021-10-18 19:38:40.000000 pyobjc-core-9.1b1/Modules/objc/test/block.m
--rw-r--r--   0 ronald     (501) staff       (20)     8172 2022-02-06 09:24:04.000000 pyobjc-core-9.1b1/Modules/objc/test/bufsizeinarg.m
--rw-r--r--   0 ronald     (501) staff       (20)     1002 2021-09-25 14:12:36.000000 pyobjc-core-9.1b1/Modules/objc/test/cfsocket.m
--rw-r--r--   0 ronald     (501) staff       (20)      872 2021-09-25 14:12:36.000000 pyobjc-core-9.1b1/Modules/objc/test/classes.m
--rw-r--r--   0 ronald     (501) staff       (20)     1499 2021-09-25 14:12:36.000000 pyobjc-core-9.1b1/Modules/objc/test/clinmeth.m
--rw-r--r--   0 ronald     (501) staff       (20)     3145 2022-01-16 10:44:28.000000 pyobjc-core-9.1b1/Modules/objc/test/coding.m
--rw-r--r--   0 ronald     (501) staff       (20)     2232 2021-10-18 19:38:40.000000 pyobjc-core-9.1b1/Modules/objc/test/copying.m
--rw-r--r--   0 ronald     (501) staff       (20)     3645 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/test/corefoundation.m
--rw-r--r--   0 ronald     (501) staff       (20)     1354 2022-02-06 09:24:04.000000 pyobjc-core-9.1b1/Modules/objc/test/dataint.m
--rw-r--r--   0 ronald     (501) staff       (20)     2647 2022-02-06 09:24:04.000000 pyobjc-core-9.1b1/Modules/objc/test/dateint.m
--rw-r--r--   0 ronald     (501) staff       (20)     1332 2021-09-25 14:12:36.000000 pyobjc-core-9.1b1/Modules/objc/test/decimal.m
--rw-r--r--   0 ronald     (501) staff       (20)     2218 2021-09-25 14:12:36.000000 pyobjc-core-9.1b1/Modules/objc/test/deprecations.m
--rw-r--r--   0 ronald     (501) staff       (20)     1937 2022-02-06 09:24:04.000000 pyobjc-core-9.1b1/Modules/objc/test/dictint.m
--rw-r--r--   0 ronald     (501) staff       (20)     1182 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/test/enumeration.m
--rw-r--r--   0 ronald     (501) staff       (20)     2661 2022-01-02 11:04:25.000000 pyobjc-core-9.1b1/Modules/objc/test/exceptions.m
--rw-r--r--   0 ronald     (501) staff       (20)     1350 2022-02-06 09:24:04.000000 pyobjc-core-9.1b1/Modules/objc/test/filepointer.m
--rw-r--r--   0 ronald     (501) staff       (20)     2180 2021-10-18 19:38:40.000000 pyobjc-core-9.1b1/Modules/objc/test/fsref.m
--rw-r--r--   0 ronald     (501) staff       (20)      962 2022-01-02 11:04:25.000000 pyobjc-core-9.1b1/Modules/objc/test/gcov.m
--rw-r--r--   0 ronald     (501) staff       (20)     2301 2022-01-02 11:04:25.000000 pyobjc-core-9.1b1/Modules/objc/test/helpernsdata.m
--rw-r--r--   0 ronald     (501) staff       (20)     2651 2022-01-02 11:04:25.000000 pyobjc-core-9.1b1/Modules/objc/test/helpernsobject.m
--rw-r--r--   0 ronald     (501) staff       (20)     3745 2021-09-25 14:12:36.000000 pyobjc-core-9.1b1/Modules/objc/test/identity.m
--rw-r--r--   0 ronald     (501) staff       (20)     1925 2021-09-25 14:12:36.000000 pyobjc-core-9.1b1/Modules/objc/test/initialize.m
--rw-r--r--   0 ronald     (501) staff       (20)     2090 2021-09-25 14:12:36.000000 pyobjc-core-9.1b1/Modules/objc/test/instanceVariables.m
--rw-r--r--   0 ronald     (501) staff       (20)     1657 2021-10-18 19:38:40.000000 pyobjc-core-9.1b1/Modules/objc/test/locking.m
--rw-r--r--   0 ronald     (501) staff       (20)    18896 2021-10-18 19:38:40.000000 pyobjc-core-9.1b1/Modules/objc/test/metadata.m
--rw-r--r--   0 ronald     (501) staff       (20)    14015 2022-01-02 11:04:25.000000 pyobjc-core-9.1b1/Modules/objc/test/metadatafunction.m
--rw-r--r--   0 ronald     (501) staff       (20)      883 2022-03-17 11:48:54.000000 pyobjc-core-9.1b1/Modules/objc/test/methodaccess.m
--rw-r--r--   0 ronald     (501) staff       (20)     2689 2021-09-25 14:12:36.000000 pyobjc-core-9.1b1/Modules/objc/test/methodlookup.m
--rw-r--r--   0 ronald     (501) staff       (20)      659 2021-10-18 19:38:40.000000 pyobjc-core-9.1b1/Modules/objc/test/methres1.m
--rw-r--r--   0 ronald     (501) staff       (20)      648 2021-10-18 19:38:40.000000 pyobjc-core-9.1b1/Modules/objc/test/methres2.m
--rw-r--r--   0 ronald     (501) staff       (20)      932 2022-01-10 12:42:10.000000 pyobjc-core-9.1b1/Modules/objc/test/misc.m
--rw-r--r--   0 ronald     (501) staff       (20)      548 2022-01-02 11:04:25.000000 pyobjc-core-9.1b1/Modules/objc/test/missing1.m
--rw-r--r--   0 ronald     (501) staff       (20)      579 2022-01-02 11:04:25.000000 pyobjc-core-9.1b1/Modules/objc/test/missing2.m
--rw-r--r--   0 ronald     (501) staff       (20)      590 2022-01-02 11:04:25.000000 pyobjc-core-9.1b1/Modules/objc/test/missing3.m
--rw-r--r--   0 ronald     (501) staff       (20)      969 2022-03-17 11:48:54.000000 pyobjc-core-9.1b1/Modules/objc/test/nsobjectcategory.m
--rw-r--r--   0 ronald     (501) staff       (20)     3275 2022-02-06 09:24:04.000000 pyobjc-core-9.1b1/Modules/objc/test/nulldelimitedresult.m
--rw-r--r--   0 ronald     (501) staff       (20)    18000 2022-03-02 19:57:48.000000 pyobjc-core-9.1b1/Modules/objc/test/objectint.m
--rw-r--r--   0 ronald     (501) staff       (20)     3955 2022-01-02 11:04:25.000000 pyobjc-core-9.1b1/Modules/objc/test/opaque.m
--rw-r--r--   0 ronald     (501) staff       (20)     3002 2022-03-03 08:50:28.000000 pyobjc-core-9.1b1/Modules/objc/test/pointersupport.m
--rw-r--r--   0 ronald     (501) staff       (20)     2834 2021-10-18 19:38:40.000000 pyobjc-core-9.1b1/Modules/objc/test/properties.m
--rw-r--r--   0 ronald     (501) staff       (20)      946 2021-09-25 14:12:36.000000 pyobjc-core-9.1b1/Modules/objc/test/protected.m
--rw-r--r--   0 ronald     (501) staff       (20)     1906 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/test/protocol.m
--rw-r--r--   0 ronald     (501) staff       (20)     5523 2022-02-06 09:24:04.000000 pyobjc-core-9.1b1/Modules/objc/test/pythonnumber.m
--rw-r--r--   0 ronald     (501) staff       (20)     4549 2022-02-06 09:24:04.000000 pyobjc-core-9.1b1/Modules/objc/test/pythonset.m
--rw-r--r--   0 ronald     (501) staff       (20)     2296 2021-09-25 14:12:36.000000 pyobjc-core-9.1b1/Modules/objc/test/sequence.m
--rw-r--r--   0 ronald     (501) staff       (20)     4398 2022-02-06 09:24:04.000000 pyobjc-core-9.1b1/Modules/objc/test/sockaddr.m
--rw-r--r--   0 ronald     (501) staff       (20)     9499 2021-10-18 19:38:40.000000 pyobjc-core-9.1b1/Modules/objc/test/specialtypecodes.m
--rw-r--r--   0 ronald     (501) staff       (20)     2011 2022-02-06 09:24:04.000000 pyobjc-core-9.1b1/Modules/objc/test/stringint.m
--rw-r--r--   0 ronald     (501) staff       (20)     2056 2021-09-25 14:12:36.000000 pyobjc-core-9.1b1/Modules/objc/test/structargs.m
--rw-r--r--   0 ronald     (501) staff       (20)     1748 2022-01-02 11:04:25.000000 pyobjc-core-9.1b1/Modules/objc/test/structpointer1.m
--rw-r--r--   0 ronald     (501) staff       (20)     1110 2021-09-25 14:12:36.000000 pyobjc-core-9.1b1/Modules/objc/test/structpointer2.m
--rw-r--r--   0 ronald     (501) staff       (20)     1723 2021-09-25 14:12:36.000000 pyobjc-core-9.1b1/Modules/objc/test/structs.m
--rw-r--r--   0 ronald     (501) staff       (20)    49424 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/test/testbndl.m
--rw-r--r--   0 ronald     (501) staff       (20)   750751 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/test/testbndl2.m
--rw-r--r--   0 ronald     (501) staff       (20)     1894 2021-09-25 14:12:36.000000 pyobjc-core-9.1b1/Modules/objc/test/testclassandinst.m
--rw-r--r--   0 ronald     (501) staff       (20)     1715 2021-09-25 14:12:36.000000 pyobjc-core-9.1b1/Modules/objc/test/testoutputinitializer.m
--rw-r--r--   0 ronald     (501) staff       (20)     8370 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/test/vector.m
--rw-r--r--   0 ronald     (501) staff       (20)   278574 2022-10-19 07:22:30.000000 pyobjc-core-9.1b1/Modules/objc/test/vectorcall.m
--rw-r--r--   0 ronald     (501) staff       (20)     1145 2021-09-25 14:12:36.000000 pyobjc-core-9.1b1/Modules/objc/test/voidpointer.m
--rw-r--r--   0 ronald     (501) staff       (20)      761 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/varlist.h
--rw-r--r--   0 ronald     (501) staff       (20)    14359 2023-02-19 11:11:08.000000 pyobjc-core-9.1b1/Modules/objc/varlist.m
--rw-r--r--   0 ronald     (501) staff       (20)      180 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/Modules/objc/weakref.h
--rw-r--r--   0 ronald     (501) staff       (20)     5500 2023-02-19 11:14:37.000000 pyobjc-core-9.1b1/Modules/objc/weakref.m
--rw-r--r--   0 ronald     (501) staff       (20)     2240 2023-03-26 10:48:33.554987 pyobjc-core-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 10:48:33.489077 pyobjc-core-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       59 2020-11-30 18:45:14.000000 pyobjc-core-9.1b1/PyObjCTest/__init__.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 10:48:33.491714 pyobjc-core-9.1b1/PyObjCTest/archives/
--rw-r--r--   0 ronald     (501) staff       (20)     1940 2020-11-30 18:45:14.000000 pyobjc-core-9.1b1/PyObjCTest/archives/py2-oc2.3.keyed
--rw-r--r--   0 ronald     (501) staff       (20)      736 2020-11-30 18:45:14.000000 pyobjc-core-9.1b1/PyObjCTest/archives/py2-oc2.3.plain
--rw-r--r--   0 ronald     (501) staff       (20)     1706 2020-11-30 18:45:14.000000 pyobjc-core-9.1b1/PyObjCTest/archives/py3-oc3.0.keyed
--rw-r--r--   0 ronald     (501) staff       (20)      555 2020-11-30 18:45:14.000000 pyobjc-core-9.1b1/PyObjCTest/archives/py3-oc3.0.plain
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 10:48:32.482641 pyobjc-core-9.1b1/PyObjCTest/data_bridgesupport/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 10:48:33.492255 pyobjc-core-9.1b1/PyObjCTest/data_bridgesupport/bundle_data/
--rw-r--r--   0 ronald     (501) staff       (20)       65 2020-11-30 18:45:14.000000 pyobjc-core-9.1b1/PyObjCTest/data_bridgesupport/bundle_data/Test.bridgesupport
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 10:48:33.493509 pyobjc-core-9.1b1/PyObjCTest/data_bridgesupport/with_data/
--rw-r--r--   0 ronald     (501) staff       (20)      103 2020-11-30 18:45:14.000000 pyobjc-core-9.1b1/PyObjCTest/data_bridgesupport/with_data/Test.bridgesupport
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 10:48:33.495023 pyobjc-core-9.1b1/PyObjCTest/data_bridgesupport/with_data_dylib/
--rw-r--r--   0 ronald     (501) staff       (20)      105 2020-11-30 18:45:14.000000 pyobjc-core-9.1b1/PyObjCTest/data_bridgesupport/with_data_dylib/Test.bridgesupport
--rw-r--r--   0 ronald     (501) staff       (20)       13 2020-11-30 18:45:14.000000 pyobjc-core-9.1b1/PyObjCTest/data_bridgesupport/with_data_dylib/Test.dylib
--rw-r--r--   0 ronald     (501) staff       (20)     2742 2022-03-05 09:55:08.000000 pyobjc-core-9.1b1/PyObjCTest/dump-nsarchive-securecoding.m
--rw-r--r--   0 ronald     (501) staff       (20)     2450 2020-11-30 18:45:14.000000 pyobjc-core-9.1b1/PyObjCTest/dump-nsarchive.m
--rw-r--r--   0 ronald     (501) staff       (20)      410 2020-11-30 18:45:14.000000 pyobjc-core-9.1b1/PyObjCTest/fnd.py
--rw-r--r--   0 ronald     (501) staff       (20)     2983 2023-03-03 17:21:59.000000 pyobjc-core-9.1b1/PyObjCTest/helper_bridgesupport.py
--rw-r--r--   0 ronald     (501) staff       (20)     2919 2020-11-30 18:45:14.000000 pyobjc-core-9.1b1/PyObjCTest/keyvaluehelper.py
--rw-r--r--   0 ronald     (501) staff       (20)     1506 2023-03-03 17:21:59.000000 pyobjc-core-9.1b1/PyObjCTest/loader.py
--rw-r--r--   0 ronald     (501) staff       (20)     7342 2023-03-03 17:21:59.000000 pyobjc-core-9.1b1/PyObjCTest/test_NULL.py
--rw-r--r--   0 ronald     (501) staff       (20)     1200 2022-01-02 11:20:34.000000 pyobjc-core-9.1b1/PyObjCTest/test_allocatebuffer.py
--rw-r--r--   0 ronald     (501) staff       (20)     1021 2022-01-02 11:04:25.000000 pyobjc-core-9.1b1/PyObjCTest/test_api_import.py
--rw-r--r--   0 ronald     (501) staff       (20)    58541 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/PyObjCTest/test_archive_python.py
--rw-r--r--   0 ronald     (501) staff       (20)    13960 2023-03-03 17:21:59.000000 pyobjc-core-9.1b1/PyObjCTest/test_archiving_interop.py
--rw-r--r--   0 ronald     (501) staff       (20)    10830 2023-03-03 17:21:59.000000 pyobjc-core-9.1b1/PyObjCTest/test_archiving_secure_interop.py
--rw-r--r--   0 ronald     (501) staff       (20)    13566 2023-03-03 17:21:59.000000 pyobjc-core-9.1b1/PyObjCTest/test_array_interface.py
--rw-r--r--   0 ronald     (501) staff       (20)    25640 2022-01-02 11:04:25.000000 pyobjc-core-9.1b1/PyObjCTest/test_array_property.py
--rw-r--r--   0 ronald     (501) staff       (20)     6180 2023-03-03 17:21:59.000000 pyobjc-core-9.1b1/PyObjCTest/test_arrays.py
--rw-r--r--   0 ronald     (501) staff       (20)     3840 2023-03-03 17:21:59.000000 pyobjc-core-9.1b1/PyObjCTest/test_assocations.py
--rw-r--r--   0 ronald     (501) staff       (20)    14826 2022-01-02 11:04:25.000000 pyobjc-core-9.1b1/PyObjCTest/test_blocks.py
--rw-r--r--   0 ronald     (501) staff       (20)     5684 2022-02-06 09:24:04.000000 pyobjc-core-9.1b1/PyObjCTest/test_bridged_classes.py
--rw-r--r--   0 ronald     (501) staff       (20)     1855 2021-03-21 10:08:22.000000 pyobjc-core-9.1b1/PyObjCTest/test_bridges.py
--rw-r--r--   0 ronald     (501) staff       (20)   105009 2023-03-26 10:33:23.000000 pyobjc-core-9.1b1/PyObjCTest/test_bridgesupport.py
--rw-r--r--   0 ronald     (501) staff       (20)    12620 2022-02-06 09:24:04.000000 pyobjc-core-9.1b1/PyObjCTest/test_bufsizeinarg.py
--rw-r--r--   0 ronald     (501) staff       (20)     6970 2022-10-31 15:31:40.000000 pyobjc-core-9.1b1/PyObjCTest/test_bundleFunctions.py
--rw-r--r--   0 ronald     (501) staff       (20)     6338 2022-10-31 15:31:40.000000 pyobjc-core-9.1b1/PyObjCTest/test_bundleVariables.py
--rw-r--r--   0 ronald     (501) staff       (20)    34668 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/PyObjCTest/test_callable_docstr.py
--rw-r--r--   0 ronald     (501) staff       (20)     8948 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/PyObjCTest/test_callbacks.py
--rw-r--r--   0 ronald     (501) staff       (20)     3901 2023-03-03 17:21:59.000000 pyobjc-core-9.1b1/PyObjCTest/test_classandinst.py
--rw-r--r--   0 ronald     (501) staff       (20)     1199 2021-07-30 09:00:36.000000 pyobjc-core-9.1b1/PyObjCTest/test_classhooks.py
--rw-r--r--   0 ronald     (501) staff       (20)     2795 2022-01-02 11:04:25.000000 pyobjc-core-9.1b1/PyObjCTest/test_clinmeth.py
--rw-r--r--   0 ronald     (501) staff       (20)     2583 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/PyObjCTest/test_compat.py
--rw-r--r--   0 ronald     (501) staff       (20)     2615 2021-08-04 10:12:03.000000 pyobjc-core-9.1b1/PyObjCTest/test_constants.py
--rw-r--r--   0 ronald     (501) staff       (20)      735 2022-01-02 11:04:25.000000 pyobjc-core-9.1b1/PyObjCTest/test_context.py
--rw-r--r--   0 ronald     (501) staff       (20)    18105 2022-02-06 09:24:04.000000 pyobjc-core-9.1b1/PyObjCTest/test_convenience.py
--rw-r--r--   0 ronald     (501) staff       (20)    26647 2022-02-06 09:24:04.000000 pyobjc-core-9.1b1/PyObjCTest/test_conversion.py
--rw-r--r--   0 ronald     (501) staff       (20)     6891 2023-02-19 10:50:33.000000 pyobjc-core-9.1b1/PyObjCTest/test_copying.py
--rw-r--r--   0 ronald     (501) staff       (20)     4329 2023-03-03 17:21:59.000000 pyobjc-core-9.1b1/PyObjCTest/test_corefoundation.py
--rw-r--r--   0 ronald     (501) staff       (20)     2349 2023-03-03 17:21:59.000000 pyobjc-core-9.1b1/PyObjCTest/test_ctests.py
--rw-r--r--   0 ronald     (501) staff       (20)     8335 2022-10-18 09:53:23.000000 pyobjc-core-9.1b1/PyObjCTest/test_data_proxy.py
--rw-r--r--   0 ronald     (501) staff       (20)     9277 2022-06-30 10:21:22.000000 pyobjc-core-9.1b1/PyObjCTest/test_date_proxy.py
--rw-r--r--   0 ronald     (501) staff       (20)     1065 2021-03-21 10:08:22.000000 pyobjc-core-9.1b1/PyObjCTest/test_default_selector.py
--rw-r--r--   0 ronald     (501) staff       (20)     4123 2022-04-11 08:03:15.000000 pyobjc-core-9.1b1/PyObjCTest/test_deprecations.py
--rw-r--r--   0 ronald     (501) staff       (20)    29263 2023-03-03 17:21:59.000000 pyobjc-core-9.1b1/PyObjCTest/test_descriptors.py
--rw-r--r--   0 ronald     (501) staff       (20)    31640 2022-03-02 09:33:22.000000 pyobjc-core-9.1b1/PyObjCTest/test_dict_interface.py
--rw-r--r--   0 ronald     (501) staff       (20)     1876 2021-03-21 10:08:22.000000 pyobjc-core-9.1b1/PyObjCTest/test_dict_property.py
--rw-r--r--   0 ronald     (501) staff       (20)     5621 2023-03-03 17:21:59.000000 pyobjc-core-9.1b1/PyObjCTest/test_dict_proxy.py
--rw-r--r--   0 ronald     (501) staff       (20)    16783 2022-01-02 11:20:34.000000 pyobjc-core-9.1b1/PyObjCTest/test_dyld.py
--rw-r--r--   0 ronald     (501) staff       (20)      643 2023-02-19 10:50:34.000000 pyobjc-core-9.1b1/PyObjCTest/test_enumerator.py
--rw-r--r--   0 ronald     (501) staff       (20)     4340 2022-01-02 11:04:25.000000 pyobjc-core-9.1b1/PyObjCTest/test_exceptions.py
--rw-r--r--   0 ronald     (501) staff       (20)     8131 2022-02-06 09:24:04.000000 pyobjc-core-9.1b1/PyObjCTest/test_filepointer.py
--rw-r--r--   0 ronald     (501) staff       (20)      728 2021-06-05 10:25:38.000000 pyobjc-core-9.1b1/PyObjCTest/test_final.py
--rw-r--r--   0 ronald     (501) staff       (20)     2670 2021-03-21 10:08:22.000000 pyobjc-core-9.1b1/PyObjCTest/test_framework.py
--rw-r--r--   0 ronald     (501) staff       (20)     2792 2022-01-02 11:04:25.000000 pyobjc-core-9.1b1/PyObjCTest/test_fsref.py
--rw-r--r--   0 ronald     (501) staff       (20)    11393 2023-03-03 17:21:59.000000 pyobjc-core-9.1b1/PyObjCTest/test_functions.py
--rw-r--r--   0 ronald     (501) staff       (20)     1162 2022-01-02 11:04:25.000000 pyobjc-core-9.1b1/PyObjCTest/test_generic_class.py
--rw-r--r--   0 ronald     (501) staff       (20)     7731 2023-03-03 17:21:59.000000 pyobjc-core-9.1b1/PyObjCTest/test_hidden_selector.py
--rw-r--r--   0 ronald     (501) staff       (20)    11080 2023-03-03 17:21:59.000000 pyobjc-core-9.1b1/PyObjCTest/test_identity.py
--rw-r--r--   0 ronald     (501) staff       (20)     7231 2022-02-06 09:24:04.000000 pyobjc-core-9.1b1/PyObjCTest/test_imp.py
--rw-r--r--   0 ronald     (501) staff       (20)     2583 2021-03-21 10:08:22.000000 pyobjc-core-9.1b1/PyObjCTest/test_initialized.py
--rw-r--r--   0 ronald     (501) staff       (20)     2323 2023-02-19 10:50:34.000000 pyobjc-core-9.1b1/PyObjCTest/test_inspect_signatures.py
--rw-r--r--   0 ronald     (501) staff       (20)    12703 2022-01-22 09:56:31.000000 pyobjc-core-9.1b1/PyObjCTest/test_internals.py
--rw-r--r--   0 ronald     (501) staff       (20)    16659 2023-03-03 17:21:59.000000 pyobjc-core-9.1b1/PyObjCTest/test_ivar.py
--rw-r--r--   0 ronald     (501) staff       (20)    30224 2023-03-03 17:21:59.000000 pyobjc-core-9.1b1/PyObjCTest/test_keyvalue.py
--rw-r--r--   0 ronald     (501) staff       (20)     1915 2021-03-21 10:08:22.000000 pyobjc-core-9.1b1/PyObjCTest/test_keyvalue_prop.py
--rw-r--r--   0 ronald     (501) staff       (20)    26483 2022-01-02 11:04:25.000000 pyobjc-core-9.1b1/PyObjCTest/test_keyvaluecoding.py
--rw-r--r--   0 ronald     (501) staff       (20)    33095 2023-03-03 17:21:59.000000 pyobjc-core-9.1b1/PyObjCTest/test_lazy_import.py
--rw-r--r--   0 ronald     (501) staff       (20)     2527 2023-03-03 17:21:59.000000 pyobjc-core-9.1b1/PyObjCTest/test_leaks.py
--rw-r--r--   0 ronald     (501) staff       (20)    10113 2023-03-03 17:21:59.000000 pyobjc-core-9.1b1/PyObjCTest/test_list_proxy.py
--rw-r--r--   0 ronald     (501) staff       (20)     3982 2021-03-21 10:08:22.000000 pyobjc-core-9.1b1/PyObjCTest/test_locking.py
--rw-r--r--   0 ronald     (501) staff       (20)     3926 2022-01-02 11:04:25.000000 pyobjc-core-9.1b1/PyObjCTest/test_machsignals.py
--rw-r--r--   0 ronald     (501) staff       (20)    54600 2022-02-06 09:24:04.000000 pyobjc-core-9.1b1/PyObjCTest/test_metadata.py
--rw-r--r--   0 ronald     (501) staff       (20)    27855 2023-03-03 17:21:59.000000 pyobjc-core-9.1b1/PyObjCTest/test_metadata_function.py
--rw-r--r--   0 ronald     (501) staff       (20)    15256 2022-02-06 09:24:04.000000 pyobjc-core-9.1b1/PyObjCTest/test_metadata_imp.py
--rw-r--r--   0 ronald     (501) staff       (20)      803 2023-03-03 17:21:59.000000 pyobjc-core-9.1b1/PyObjCTest/test_metadata_inheritance.py
--rw-r--r--   0 ronald     (501) staff       (20)    32824 2022-02-06 09:24:04.000000 pyobjc-core-9.1b1/PyObjCTest/test_metadata_py.py
--rw-r--r--   0 ronald     (501) staff       (20)    16933 2022-02-06 09:24:04.000000 pyobjc-core-9.1b1/PyObjCTest/test_metadata_py2py.py
--rw-r--r--   0 ronald     (501) staff       (20)    17752 2023-02-19 10:50:34.000000 pyobjc-core-9.1b1/PyObjCTest/test_method_prototypes.py
--rw-r--r--   0 ronald     (501) staff       (20)    10358 2022-10-31 14:48:14.000000 pyobjc-core-9.1b1/PyObjCTest/test_methodaccess.py
--rw-r--r--   0 ronald     (501) staff       (20)    14062 2022-01-22 09:57:03.000000 pyobjc-core-9.1b1/PyObjCTest/test_methodedits.py
--rw-r--r--   0 ronald     (501) staff       (20)     5801 2023-02-19 10:50:34.000000 pyobjc-core-9.1b1/PyObjCTest/test_methodlookup.py
--rw-r--r--   0 ronald     (501) staff       (20)    59548 2023-03-03 17:21:59.000000 pyobjc-core-9.1b1/PyObjCTest/test_methods.py
--rw-r--r--   0 ronald     (501) staff       (20)  2870222 2023-03-03 17:21:59.000000 pyobjc-core-9.1b1/PyObjCTest/test_methods2.py
--rw-r--r--   0 ronald     (501) staff       (20)     2217 2022-01-02 11:04:26.000000 pyobjc-core-9.1b1/PyObjCTest/test_methres.py
--rw-r--r--   0 ronald     (501) staff       (20)     5686 2023-02-19 10:50:34.000000 pyobjc-core-9.1b1/PyObjCTest/test_nscoder.py
--rw-r--r--   0 ronald     (501) staff       (20)    29009 2022-03-02 19:57:48.000000 pyobjc-core-9.1b1/PyObjCTest/test_nsdata.py
--rw-r--r--   0 ronald     (501) staff       (20)     1214 2021-03-21 10:08:22.000000 pyobjc-core-9.1b1/PyObjCTest/test_nsdate_proxy.py
--rw-r--r--   0 ronald     (501) staff       (20)    13611 2023-02-19 10:50:34.000000 pyobjc-core-9.1b1/PyObjCTest/test_nsdecimal.py
--rw-r--r--   0 ronald     (501) staff       (20)     1065 2022-10-18 09:53:23.000000 pyobjc-core-9.1b1/PyObjCTest/test_nsinvocation.py
--rw-r--r--   0 ronald     (501) staff       (20)     6608 2022-03-17 11:48:54.000000 pyobjc-core-9.1b1/PyObjCTest/test_nsobject.py
--rw-r--r--   0 ronald     (501) staff       (20)     4984 2022-02-24 08:47:16.000000 pyobjc-core-9.1b1/PyObjCTest/test_nulldelimited.py
--rw-r--r--   0 ronald     (501) staff       (20)    45321 2023-03-03 17:21:59.000000 pyobjc-core-9.1b1/PyObjCTest/test_number_proxy.py
--rw-r--r--   0 ronald     (501) staff       (20)     4038 2023-03-03 17:21:59.000000 pyobjc-core-9.1b1/PyObjCTest/test_objc.py
--rw-r--r--   0 ronald     (501) staff       (20)     2106 2023-02-19 10:50:34.000000 pyobjc-core-9.1b1/PyObjCTest/test_objcpointer.py
--rw-r--r--   0 ronald     (501) staff       (20)    20238 2023-03-03 17:21:59.000000 pyobjc-core-9.1b1/PyObjCTest/test_object_property.py
--rw-r--r--   0 ronald     (501) staff       (20)    22970 2022-02-06 09:24:04.000000 pyobjc-core-9.1b1/PyObjCTest/test_object_proxy.py
--rw-r--r--   0 ronald     (501) staff       (20)     6550 2022-02-06 09:24:04.000000 pyobjc-core-9.1b1/PyObjCTest/test_opaque.py
--rw-r--r--   0 ronald     (501) staff       (20)    14120 2022-10-31 15:31:40.000000 pyobjc-core-9.1b1/PyObjCTest/test_options.py
--rw-r--r--   0 ronald     (501) staff       (20)      550 2021-03-21 10:08:22.000000 pyobjc-core-9.1b1/PyObjCTest/test_outputinitializer.py
--rw-r--r--   0 ronald     (501) staff       (20)      887 2022-01-02 11:04:26.000000 pyobjc-core-9.1b1/PyObjCTest/test_pickle.py
--rw-r--r--   0 ronald     (501) staff       (20)      426 2021-03-21 10:08:22.000000 pyobjc-core-9.1b1/PyObjCTest/test_pickling_objc.py
--rw-r--r--   0 ronald     (501) staff       (20)     6166 2023-03-03 17:21:59.000000 pyobjc-core-9.1b1/PyObjCTest/test_pointer_compat.py
--rw-r--r--   0 ronald     (501) staff       (20)     1514 2022-02-06 09:24:04.000000 pyobjc-core-9.1b1/PyObjCTest/test_posing.py
--rw-r--r--   0 ronald     (501) staff       (20)     5733 2021-07-30 09:00:36.000000 pyobjc-core-9.1b1/PyObjCTest/test_propertiesforclass.py
--rw-r--r--   0 ronald     (501) staff       (20)      310 2021-03-21 10:08:22.000000 pyobjc-core-9.1b1/PyObjCTest/test_protected.py
--rw-r--r--   0 ronald     (501) staff       (20)    29078 2023-03-03 17:21:59.000000 pyobjc-core-9.1b1/PyObjCTest/test_protocol.py
--rw-r--r--   0 ronald     (501) staff       (20)     1093 2022-01-02 11:04:26.000000 pyobjc-core-9.1b1/PyObjCTest/test_protocolNamed.py
--rw-r--r--   0 ronald     (501) staff       (20)     2983 2023-02-19 10:50:34.000000 pyobjc-core-9.1b1/PyObjCTest/test_python_method.py
--rw-r--r--   0 ronald     (501) staff       (20)    19425 2023-03-03 17:19:36.000000 pyobjc-core-9.1b1/PyObjCTest/test_regr.py
--rw-r--r--   0 ronald     (501) staff       (20)    16157 2022-01-02 11:04:26.000000 pyobjc-core-9.1b1/PyObjCTest/test_set_interface.py
--rw-r--r--   0 ronald     (501) staff       (20)    16022 2022-01-02 11:04:26.000000 pyobjc-core-9.1b1/PyObjCTest/test_set_property.py
--rw-r--r--   0 ronald     (501) staff       (20)    12947 2023-03-03 17:21:59.000000 pyobjc-core-9.1b1/PyObjCTest/test_set_proxy.py
--rw-r--r--   0 ronald     (501) staff       (20)     3319 2022-03-02 09:33:22.000000 pyobjc-core-9.1b1/PyObjCTest/test_signals.py
--rw-r--r--   0 ronald     (501) staff       (20)     3013 2023-02-19 10:50:34.000000 pyobjc-core-9.1b1/PyObjCTest/test_signatures.py
--rw-r--r--   0 ronald     (501) staff       (20)    11085 2023-02-19 10:50:34.000000 pyobjc-core-9.1b1/PyObjCTest/test_simd.py
--rw-r--r--   0 ronald     (501) staff       (20)     5840 2022-02-24 21:31:17.000000 pyobjc-core-9.1b1/PyObjCTest/test_sockaddr.py
--rw-r--r--   0 ronald     (501) staff       (20)     7090 2022-01-02 11:04:26.000000 pyobjc-core-9.1b1/PyObjCTest/test_specialtypecodes_charbyte.py
--rw-r--r--   0 ronald     (501) staff       (20)     7676 2022-01-02 11:04:26.000000 pyobjc-core-9.1b1/PyObjCTest/test_specialtypecodes_charint.py
--rw-r--r--   0 ronald     (501) staff       (20)    20176 2021-03-21 10:08:22.000000 pyobjc-core-9.1b1/PyObjCTest/test_specialtypecodes_methdef.py
--rw-r--r--   0 ronald     (501) staff       (20)     6352 2022-01-02 11:04:26.000000 pyobjc-core-9.1b1/PyObjCTest/test_specialtypecodes_nsbool.py
--rw-r--r--   0 ronald     (501) staff       (20)     2361 2021-03-21 10:08:22.000000 pyobjc-core-9.1b1/PyObjCTest/test_specialtypecodes_struct.py
--rw-r--r--   0 ronald     (501) staff       (20)     7050 2022-01-02 11:04:26.000000 pyobjc-core-9.1b1/PyObjCTest/test_specialtypecodes_unichar.py
--rw-r--r--   0 ronald     (501) staff       (20)     6331 2023-03-03 17:21:59.000000 pyobjc-core-9.1b1/PyObjCTest/test_splitsig.py
--rw-r--r--   0 ronald     (501) staff       (20)     4936 2022-02-06 09:24:04.000000 pyobjc-core-9.1b1/PyObjCTest/test_string_proxy.py
--rw-r--r--   0 ronald     (501) staff       (20)      899 2023-03-03 17:21:59.000000 pyobjc-core-9.1b1/PyObjCTest/test_structpointer.py
--rw-r--r--   0 ronald     (501) staff       (20)    34918 2023-02-19 10:50:34.000000 pyobjc-core-9.1b1/PyObjCTest/test_structs.py
--rw-r--r--   0 ronald     (501) staff       (20)    33789 2023-02-19 10:50:34.000000 pyobjc-core-9.1b1/PyObjCTest/test_subclass.py
--rw-r--r--   0 ronald     (501) staff       (20)     2013 2022-01-02 11:04:26.000000 pyobjc-core-9.1b1/PyObjCTest/test_synthesize.py
--rw-r--r--   0 ronald     (501) staff       (20)    93311 2023-03-03 17:21:59.000000 pyobjc-core-9.1b1/PyObjCTest/test_testsupport.py
--rw-r--r--   0 ronald     (501) staff       (20)    78678 2023-03-26 10:44:23.000000 pyobjc-core-9.1b1/PyObjCTest/test_transform.py
--rw-r--r--   0 ronald     (501) staff       (20)     7514 2023-03-03 17:21:59.000000 pyobjc-core-9.1b1/PyObjCTest/test_transform_integration.py
--rw-r--r--   0 ronald     (501) staff       (20)     2596 2022-01-02 11:04:26.000000 pyobjc-core-9.1b1/PyObjCTest/test_typecheck.py
--rw-r--r--   0 ronald     (501) staff       (20)     3148 2023-02-19 10:50:34.000000 pyobjc-core-9.1b1/PyObjCTest/test_unicode.py
--rw-r--r--   0 ronald     (501) staff       (20)     2426 2021-03-21 10:08:22.000000 pyobjc-core-9.1b1/PyObjCTest/test_usekvo.py
--rw-r--r--   0 ronald     (501) staff       (20)     1900 2021-03-21 10:08:22.000000 pyobjc-core-9.1b1/PyObjCTest/test_varargs.py
--rw-r--r--   0 ronald     (501) staff       (20)     2380 2023-02-19 10:50:34.000000 pyobjc-core-9.1b1/PyObjCTest/test_varlist.py
--rw-r--r--   0 ronald     (501) staff       (20)    21563 2023-02-19 10:50:34.000000 pyobjc-core-9.1b1/PyObjCTest/test_vector_proxy.py
--rw-r--r--   0 ronald     (501) staff       (20)  1646925 2022-10-19 07:22:30.000000 pyobjc-core-9.1b1/PyObjCTest/test_vectorcall.py
--rw-r--r--   0 ronald     (501) staff       (20)     1775 2022-01-22 09:56:32.000000 pyobjc-core-9.1b1/PyObjCTest/test_version_support.py
--rw-r--r--   0 ronald     (501) staff       (20)      444 2021-03-21 10:08:22.000000 pyobjc-core-9.1b1/PyObjCTest/test_voidpointer.py
--rw-r--r--   0 ronald     (501) staff       (20)     4115 2023-03-03 17:21:59.000000 pyobjc-core-9.1b1/PyObjCTest/test_weakref.py
--rw-r--r--   0 ronald     (501) staff       (20)     1172 2020-11-30 18:45:14.000000 pyobjc-core-9.1b1/README.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 10:48:33.550626 pyobjc-core-9.1b1/Tools/
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-core-9.1b1/Tools/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     1323 2021-09-24 07:19:41.000000 pyobjc-core-9.1b1/Tools/comparebench.py
--rw-r--r--   0 ronald     (501) staff       (20)     1662 2023-03-03 17:21:59.000000 pyobjc-core-9.1b1/Tools/gen_archive.py
--rwxr-xr-x   0 ronald     (501) staff       (20)    49625 2023-02-19 10:50:34.000000 pyobjc-core-9.1b1/Tools/generate-helpers-vector.py
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-core-9.1b1/Tools/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)     6919 2022-01-02 11:20:34.000000 pyobjc-core-9.1b1/Tools/pyobjcbench.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 10:48:33.552929 pyobjc-core-9.1b1/Tools/results/
--rw-r--r--   0 ronald     (501) staff       (20)      602 2021-10-02 09:43:54.000000 pyobjc-core-9.1b1/Tools/results/pyobjcbench-7.3.txt
--rw-r--r--   0 ronald     (501) staff       (20)      604 2021-09-30 19:06:24.000000 pyobjc-core-9.1b1/Tools/results/pyobjcbench-8.0b1.txt
--rw-r--r--   0 ronald     (501) staff       (20)      604 2021-10-02 09:43:31.000000 pyobjc-core-9.1b1/Tools/results/pyobjcbench-8.0b2.txt
--rwxr-xr-x   0 ronald     (501) staff       (20)      566 2022-10-18 09:53:23.000000 pyobjc-core-9.1b1/Tools/runtests-with-nuitka.py
--rw-r--r--   0 ronald     (501) staff       (20)      872 2022-10-18 09:53:23.000000 pyobjc-core-9.1b1/Tools/runtests.py
--rw-r--r--   0 ronald     (501) staff       (20)     3113 2023-03-26 10:19:28.000000 pyobjc-core-9.1b1/diff.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1943 2023-03-26 10:48:33.555699 pyobjc-core-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)    23169 2023-03-03 17:21:59.000000 pyobjc-core-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-06 23:56:14.413658 pyobjc-core-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-06 23:56:13.292850 pyobjc-core-9.2/Examples/
+-rw-r--r--   0 ronald     (501) staff       (20)    15940 2020-11-30 18:45:14.000000 pyobjc-core-9.2/Examples/00ReadMe.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-06 23:56:13.297493 pyobjc-core-9.2/Examples/GUITests/
+-rw-r--r--   0 ronald     (501) staff       (20)      132 2020-11-30 18:45:14.000000 pyobjc-core-9.2/Examples/GUITests/00ReadMe.txt
+-rwxr-xr-x   0 ronald     (501) staff       (20)     1444 2020-11-30 18:45:14.000000 pyobjc-core-9.2/Examples/GUITests/test_modalsession.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-06 23:56:13.279276 pyobjc-core-9.2/Examples/NonFunctional/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-06 23:56:13.316644 pyobjc-core-9.2/Examples/NonFunctional/RemotePyInterpreter/
+-rw-r--r--   0 ronald     (501) staff       (20)     9185 2023-03-03 17:21:59.000000 pyobjc-core-9.2/Examples/NonFunctional/RemotePyInterpreter/AsyncPythonInterpreter.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4559 2021-07-30 09:00:36.000000 pyobjc-core-9.2/Examples/NonFunctional/RemotePyInterpreter/ConsoleReactor.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-06 23:56:13.279849 pyobjc-core-9.2/Examples/NonFunctional/RemotePyInterpreter/English.lproj/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-06 23:56:13.319369 pyobjc-core-9.2/Examples/NonFunctional/RemotePyInterpreter/English.lproj/MainMenu.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      109 2020-11-30 18:45:14.000000 pyobjc-core-9.2/Examples/NonFunctional/RemotePyInterpreter/English.lproj/MainMenu.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      605 2020-11-30 18:45:14.000000 pyobjc-core-9.2/Examples/NonFunctional/RemotePyInterpreter/English.lproj/MainMenu.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)   157619 2020-11-30 18:45:14.000000 pyobjc-core-9.2/Examples/NonFunctional/RemotePyInterpreter/English.lproj/MainMenu.nib/keyedobjects.nib
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-06 23:56:13.323078 pyobjc-core-9.2/Examples/NonFunctional/RemotePyInterpreter/English.lproj/RemotePyInterpreterDocument.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      771 2020-11-30 18:45:14.000000 pyobjc-core-9.2/Examples/NonFunctional/RemotePyInterpreter/English.lproj/RemotePyInterpreterDocument.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      495 2020-11-30 18:45:14.000000 pyobjc-core-9.2/Examples/NonFunctional/RemotePyInterpreter/English.lproj/RemotePyInterpreterDocument.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)    30650 2020-11-30 18:45:14.000000 pyobjc-core-9.2/Examples/NonFunctional/RemotePyInterpreter/English.lproj/RemotePyInterpreterDocument.nib/keyedobjects.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      343 2020-11-30 18:45:14.000000 pyobjc-core-9.2/Examples/NonFunctional/RemotePyInterpreter/README.txt
+-rw-r--r--   0 ronald     (501) staff       (20)    16640 2021-07-30 09:00:36.000000 pyobjc-core-9.2/Examples/NonFunctional/RemotePyInterpreter/RemotePyInterpreter.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6907 2021-07-30 09:00:36.000000 pyobjc-core-9.2/Examples/NonFunctional/RemotePyInterpreter/netrepr.py
+-rw-r--r--   0 ronald     (501) staff       (20)      585 2020-11-30 18:45:14.000000 pyobjc-core-9.2/Examples/NonFunctional/RemotePyInterpreter/remote_bootstrap.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4028 2020-11-30 18:45:14.000000 pyobjc-core-9.2/Examples/NonFunctional/RemotePyInterpreter/remote_console.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2807 2021-07-30 09:00:36.000000 pyobjc-core-9.2/Examples/NonFunctional/RemotePyInterpreter/remote_pipe.py
+-rw-r--r--   0 ronald     (501) staff       (20)      853 2020-11-30 18:45:14.000000 pyobjc-core-9.2/Examples/NonFunctional/RemotePyInterpreter/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1492 2021-07-30 09:00:36.000000 pyobjc-core-9.2/Examples/NonFunctional/RemotePyInterpreter/tcpinterpreter.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3830 2021-07-30 09:00:36.000000 pyobjc-core-9.2/Examples/NonFunctional/RemotePyInterpreter/test_client.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-06 23:56:13.337478 pyobjc-core-9.2/Examples/Scripts/
+-rwxr-xr-x   0 ronald     (501) staff       (20)     2467 2021-10-18 19:38:40.000000 pyobjc-core-9.2/Examples/Scripts/HelloWorld.py
+-rwxr-xr-x   0 ronald     (501) staff       (20)     1832 2023-03-03 17:21:59.000000 pyobjc-core-9.2/Examples/Scripts/autoreadme.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1269 2020-11-30 18:45:14.000000 pyobjc-core-9.2/Examples/Scripts/instrumentSends.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3775 2021-07-30 09:00:36.000000 pyobjc-core-9.2/Examples/Scripts/kvo-debugging.py
+-rw-r--r--   0 ronald     (501) staff       (20)      477 2020-11-30 18:45:14.000000 pyobjc-core-9.2/Examples/Scripts/signal-demo.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2649 2021-10-18 19:38:40.000000 pyobjc-core-9.2/Examples/Scripts/stdinreader.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1656 2020-11-30 18:45:14.000000 pyobjc-core-9.2/Examples/Scripts/subclassing-objective-c.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2535 2023-03-03 17:21:59.000000 pyobjc-core-9.2/Examples/Scripts/wmEnable.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6282 2020-11-30 18:45:14.000000 pyobjc-core-9.2/HISTORIC.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1323 2020-11-30 18:45:14.000000 pyobjc-core-9.2/Install.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-06 23:56:13.280748 pyobjc-core-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-06 23:56:13.340001 pyobjc-core-9.2/Lib/PyObjCTools/
+-rw-r--r--   0 ronald     (501) staff       (20)    10350 2021-10-18 19:38:40.000000 pyobjc-core-9.2/Lib/PyObjCTools/KeyValueCoding.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1218 2022-01-02 11:04:25.000000 pyobjc-core-9.2/Lib/PyObjCTools/MachSignals.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2483 2022-01-02 11:04:25.000000 pyobjc-core-9.2/Lib/PyObjCTools/Signals.py
+-rw-r--r--   0 ronald     (501) staff       (20)    45744 2023-05-27 09:46:33.000000 pyobjc-core-9.2/Lib/PyObjCTools/TestSupport.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-06 23:56:13.377378 pyobjc-core-9.2/Lib/objc/
+-rw-r--r--   0 ronald     (501) staff       (20)     2724 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Lib/objc/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1714 2022-02-06 09:24:04.000000 pyobjc-core-9.2/Lib/objc/_bridges.py
+-rw-r--r--   0 ronald     (501) staff       (20)    26273 2023-03-26 10:43:00.000000 pyobjc-core-9.2/Lib/objc/_bridgesupport.py
+-rw-r--r--   0 ronald     (501) staff       (20)    10129 2023-03-03 17:21:59.000000 pyobjc-core-9.2/Lib/objc/_callable_docstr.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2638 2022-01-02 11:04:25.000000 pyobjc-core-9.2/Lib/objc/_category.py
+-rw-r--r--   0 ronald     (501) staff       (20)      893 2022-06-23 11:03:27.000000 pyobjc-core-9.2/Lib/objc/_compat.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1317 2021-07-30 09:00:36.000000 pyobjc-core-9.2/Lib/objc/_context.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3558 2022-06-30 10:21:22.000000 pyobjc-core-9.2/Lib/objc/_convenience.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3419 2021-10-18 19:38:40.000000 pyobjc-core-9.2/Lib/objc/_convenience_mapping.py
+-rw-r--r--   0 ronald     (501) staff       (20)    10994 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Lib/objc/_convenience_nsarray.py
+-rw-r--r--   0 ronald     (501) staff       (20)    11205 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Lib/objc/_convenience_nsdata.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3782 2021-10-18 19:38:40.000000 pyobjc-core-9.2/Lib/objc/_convenience_nsdecimal.py
+-rw-r--r--   0 ronald     (501) staff       (20)     8263 2022-01-02 11:04:25.000000 pyobjc-core-9.2/Lib/objc/_convenience_nsdictionary.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3056 2021-07-30 09:00:36.000000 pyobjc-core-9.2/Lib/objc/_convenience_nsobject.py
+-rw-r--r--   0 ronald     (501) staff       (20)     8714 2021-07-30 09:00:36.000000 pyobjc-core-9.2/Lib/objc/_convenience_nsset.py
+-rw-r--r--   0 ronald     (501) staff       (20)      576 2020-11-30 18:45:14.000000 pyobjc-core-9.2/Lib/objc/_convenience_nsstring.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1252 2020-11-30 18:45:14.000000 pyobjc-core-9.2/Lib/objc/_convenience_sequence.py
+-rw-r--r--   0 ronald     (501) staff       (20)    11927 2022-03-02 19:57:48.000000 pyobjc-core-9.2/Lib/objc/_descriptors.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4216 2022-01-02 11:04:25.000000 pyobjc-core-9.2/Lib/objc/_dyld.py
+-rw-r--r--   0 ronald     (501) staff       (20)      634 2020-11-30 18:45:14.000000 pyobjc-core-9.2/Lib/objc/_framework.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2212 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Lib/objc/_informal_protocol.py
+-rw-r--r--   0 ronald     (501) staff       (20)    16696 2023-03-03 17:21:59.000000 pyobjc-core-9.2/Lib/objc/_lazyimport.py
+-rw-r--r--   0 ronald     (501) staff       (20)      898 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Lib/objc/_locking.py
+-rw-r--r--   0 ronald     (501) staff       (20)    33278 2023-03-03 17:21:59.000000 pyobjc-core-9.2/Lib/objc/_properties.py
+-rw-r--r--   0 ronald     (501) staff       (20)      898 2021-07-30 09:00:36.000000 pyobjc-core-9.2/Lib/objc/_protocols.py
+-rw-r--r--   0 ronald     (501) staff       (20)    16349 2023-03-03 17:21:59.000000 pyobjc-core-9.2/Lib/objc/_pycoder.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2044 2021-07-30 09:00:36.000000 pyobjc-core-9.2/Lib/objc/_pythonify.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2230 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Lib/objc/_structtype.py
+-rw-r--r--   0 ronald     (501) staff       (20)    23779 2023-05-29 08:54:13.000000 pyobjc-core-9.2/Lib/objc/_transform.py
+-rw-r--r--   0 ronald     (501) staff       (20)    14079 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Lib/objc/simd.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-06 23:56:13.382219 pyobjc-core-9.2/Lib/pyobjc_core.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2449 2023-06-06 23:56:13.000000 pyobjc-core-9.2/Lib/pyobjc_core.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)    16097 2023-06-06 23:56:13.000000 pyobjc-core-9.2/Lib/pyobjc_core.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-06 23:56:13.000000 pyobjc-core-9.2/Lib/pyobjc_core.egg-info/dependency_links.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-06 23:56:13.383279 pyobjc-core-9.2/Lib/pyobjc_core.egg-info/include/
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-06-06 23:56:13.000000 pyobjc-core-9.2/Lib/pyobjc_core.egg-info/include/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 23:56:13.000000 pyobjc-core-9.2/Lib/pyobjc_core.egg-info/include/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:46:57.000000 pyobjc-core-9.2/Lib/pyobjc_core.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       28 2023-06-06 23:56:13.000000 pyobjc-core-9.2/Lib/pyobjc_core.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-core-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)    64814 2020-11-30 18:45:14.000000 pyobjc-core-9.2/MANIFEST
+-rw-r--r--   0 ronald     (501) staff       (20)      317 2021-03-21 10:08:22.000000 pyobjc-core-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-06 23:56:13.383693 pyobjc-core-9.2/Misc/
+-rw-r--r--   0 ronald     (501) staff       (20)     2377 2020-11-30 18:45:14.000000 pyobjc-core-9.2/Misc/announcement.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-06 23:56:13.384469 pyobjc-core-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)     4767 2022-02-06 09:24:04.000000 pyobjc-core-9.2/Modules/_machsignals.m
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-06 23:56:13.621671 pyobjc-core-9.2/Modules/objc/
+-rw-r--r--   0 ronald     (501) staff       (20)      146 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/OC_BuiltinPythonArray.h
+-rw-r--r--   0 ronald     (501) staff       (20)      373 2021-10-18 19:38:40.000000 pyobjc-core-9.2/Modules/objc/OC_BuiltinPythonArray.m
+-rw-r--r--   0 ronald     (501) staff       (20)      144 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/OC_BuiltinPythonData.h
+-rw-r--r--   0 ronald     (501) staff       (20)      282 2022-02-06 09:24:04.000000 pyobjc-core-9.2/Modules/objc/OC_BuiltinPythonData.m
+-rw-r--r--   0 ronald     (501) staff       (20)      144 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/OC_BuiltinPythonDate.h
+-rw-r--r--   0 ronald     (501) staff       (20)      282 2022-02-06 09:24:04.000000 pyobjc-core-9.2/Modules/objc/OC_BuiltinPythonDate.m
+-rw-r--r--   0 ronald     (501) staff       (20)      156 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/OC_BuiltinPythonDictionary.h
+-rw-r--r--   0 ronald     (501) staff       (20)      393 2021-10-18 19:38:40.000000 pyobjc-core-9.2/Modules/objc/OC_BuiltinPythonDictionary.m
+-rw-r--r--   0 ronald     (501) staff       (20)      148 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/OC_BuiltinPythonNumber.h
+-rw-r--r--   0 ronald     (501) staff       (20)      626 2022-01-02 11:20:34.000000 pyobjc-core-9.2/Modules/objc/OC_BuiltinPythonNumber.m
+-rw-r--r--   0 ronald     (501) staff       (20)      142 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/OC_BuiltinPythonSet.h
+-rw-r--r--   0 ronald     (501) staff       (20)      365 2021-10-18 19:38:40.000000 pyobjc-core-9.2/Modules/objc/OC_BuiltinPythonSet.m
+-rw-r--r--   0 ronald     (501) staff       (20)      150 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/OC_BuiltinPythonUnicode.h
+-rw-r--r--   0 ronald     (501) staff       (20)      379 2021-10-18 19:38:40.000000 pyobjc-core-9.2/Modules/objc/OC_BuiltinPythonUnicode.m
+-rw-r--r--   0 ronald     (501) staff       (20)      731 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/OC_NSBundleHack.h
+-rw-r--r--   0 ronald     (501) staff       (20)     3364 2022-02-06 09:24:04.000000 pyobjc-core-9.2/Modules/objc/OC_NSBundleHack.m
+-rw-r--r--   0 ronald     (501) staff       (20)     3302 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/OC_PythonArray.h
+-rw-r--r--   0 ronald     (501) staff       (20)    17717 2022-03-17 11:48:54.000000 pyobjc-core-9.2/Modules/objc/OC_PythonArray.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1845 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/OC_PythonData.h
+-rw-r--r--   0 ronald     (501) staff       (20)     9389 2022-02-24 08:48:42.000000 pyobjc-core-9.2/Modules/objc/OC_PythonData.m
+-rw-r--r--   0 ronald     (501) staff       (20)      361 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/OC_PythonDate.h
+-rw-r--r--   0 ronald     (501) staff       (20)    10104 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/OC_PythonDate.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1511 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/OC_PythonDictionary.h
+-rw-r--r--   0 ronald     (501) staff       (20)    15291 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/OC_PythonDictionary.m
+-rw-r--r--   0 ronald     (501) staff       (20)      383 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/OC_PythonEnumerator.h
+-rw-r--r--   0 ronald     (501) staff       (20)     2409 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/OC_PythonEnumerator.m
+-rw-r--r--   0 ronald     (501) staff       (20)      372 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/OC_PythonNumber.h
+-rw-r--r--   0 ronald     (501) staff       (20)    15050 2022-06-23 11:03:27.000000 pyobjc-core-9.2/Modules/objc/OC_PythonNumber.m
+-rw-r--r--   0 ronald     (501) staff       (20)     3550 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/OC_PythonObject.h
+-rw-r--r--   0 ronald     (501) staff       (20)    32682 2022-10-19 07:22:30.000000 pyobjc-core-9.2/Modules/objc/OC_PythonObject.m
+-rw-r--r--   0 ronald     (501) staff       (20)      333 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/OC_PythonSet.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13831 2023-05-28 18:52:21.000000 pyobjc-core-9.2/Modules/objc/OC_PythonSet.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1600 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/OC_PythonUnicode.h
+-rw-r--r--   0 ronald     (501) staff       (20)    12786 2022-12-17 10:07:28.000000 pyobjc-core-9.2/Modules/objc/OC_PythonUnicode.m
+-rw-r--r--   0 ronald     (501) staff       (20)      767 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/ObjCPointer.h
+-rw-r--r--   0 ronald     (501) staff       (20)     4772 2023-02-19 10:59:41.000000 pyobjc-core-9.2/Modules/objc/ObjCPointer.m
+-rw-r--r--   0 ronald     (501) staff       (20)      776 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/block_support.h
+-rw-r--r--   0 ronald     (501) staff       (20)    18742 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/block_support.m
+-rw-r--r--   0 ronald     (501) staff       (20)      965 2021-10-18 19:38:40.000000 pyobjc-core-9.2/Modules/objc/bundle-variables.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13729 2022-10-18 09:53:23.000000 pyobjc-core-9.2/Modules/objc/bundle-variables.m
+-rw-r--r--   0 ronald     (501) staff       (20)      385 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/class-builder.h
+-rw-r--r--   0 ronald     (501) staff       (20)    38209 2023-04-15 09:30:15.000000 pyobjc-core-9.2/Modules/objc/class-builder.m
+-rw-r--r--   0 ronald     (501) staff       (20)      589 2022-01-02 11:04:25.000000 pyobjc-core-9.2/Modules/objc/class-list.h
+-rw-r--r--   0 ronald     (501) staff       (20)     2036 2022-02-06 09:24:04.000000 pyobjc-core-9.2/Modules/objc/class-list.m
+-rw-r--r--   0 ronald     (501) staff       (20)      677 2022-02-06 09:24:04.000000 pyobjc-core-9.2/Modules/objc/closure_pool.h
+-rw-r--r--   0 ronald     (501) staff       (20)     3023 2022-02-06 09:24:04.000000 pyobjc-core-9.2/Modules/objc/closure_pool.m
+-rw-r--r--   0 ronald     (501) staff       (20)      531 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/corefoundation.h
+-rw-r--r--   0 ronald     (501) staff       (20)    11124 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/corefoundation.m
+-rw-r--r--   0 ronald     (501) staff       (20)      169 2021-10-18 19:38:40.000000 pyobjc-core-9.2/Modules/objc/ctests.h
+-rw-r--r--   0 ronald     (501) staff       (20)    31484 2023-02-19 13:33:58.000000 pyobjc-core-9.2/Modules/objc/ctests.m
+-rw-r--r--   0 ronald     (501) staff       (20)      281 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/file_wrapper.h
+-rw-r--r--   0 ronald     (501) staff       (20)    10599 2023-02-19 11:01:59.000000 pyobjc-core-9.2/Modules/objc/file_wrapper.m
+-rw-r--r--   0 ronald     (501) staff       (20)      562 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/formal-protocol.h
+-rw-r--r--   0 ronald     (501) staff       (20)    17150 2023-03-24 18:54:07.000000 pyobjc-core-9.2/Modules/objc/formal-protocol.m
+-rw-r--r--   0 ronald     (501) staff       (20)      684 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/fsref.h
+-rw-r--r--   0 ronald     (501) staff       (20)     5585 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/fsref.m
+-rw-r--r--   0 ronald     (501) staff       (20)      625 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/function.h
+-rw-r--r--   0 ronald     (501) staff       (20)    18319 2023-02-19 11:02:35.000000 pyobjc-core-9.2/Modules/objc/function.m
+-rw-r--r--   0 ronald     (501) staff       (20)     5914 2022-10-18 09:53:23.000000 pyobjc-core-9.2/Modules/objc/helpers-authorization.m
+-rw-r--r--   0 ronald     (501) staff       (20)    44063 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/helpers-foundation-nscoder.m
+-rw-r--r--   0 ronald     (501) staff       (20)     7317 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/helpers-foundation-nsdata.m
+-rw-r--r--   0 ronald     (501) staff       (20)    36763 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/helpers-foundation-nsdecimal.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9933 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/helpers-foundation-nsinvocation.m
+-rw-r--r--   0 ronald     (501) staff       (20)    13648 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/helpers-foundation-nsobject.m
+-rw-r--r--   0 ronald     (501) staff       (20)   492431 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/helpers-vector.m
+-rw-r--r--   0 ronald     (501) staff       (20)      861 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/helpers.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1115 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/instance-var.h
+-rw-r--r--   0 ronald     (501) staff       (20)    17605 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/instance-var.m
+-rw-r--r--   0 ronald     (501) staff       (20)      529 2021-10-18 19:38:40.000000 pyobjc-core-9.2/Modules/objc/ivar-accessor.h
+-rw-r--r--   0 ronald     (501) staff       (20)     8594 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/ivar-accessor.m
+-rw-r--r--   0 ronald     (501) staff       (20)      460 2022-01-02 11:04:25.000000 pyobjc-core-9.2/Modules/objc/libffi_extra.h
+-rw-r--r--   0 ronald     (501) staff       (20)     2584 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/libffi_extra.m
+-rw-r--r--   0 ronald     (501) staff       (20)     4877 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/libffi_support.h
+-rw-r--r--   0 ronald     (501) staff       (20)   180541 2023-05-27 09:46:33.000000 pyobjc-core-9.2/Modules/objc/libffi_support.m
+-rw-r--r--   0 ronald     (501) staff       (20)      349 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/memview.h
+-rw-r--r--   0 ronald     (501) staff       (20)     3327 2023-02-19 11:04:02.000000 pyobjc-core-9.2/Modules/objc/memview.m
+-rw-r--r--   0 ronald     (501) staff       (20)      804 2022-10-18 09:53:23.000000 pyobjc-core-9.2/Modules/objc/meth-func.h
+-rw-r--r--   0 ronald     (501) staff       (20)     6903 2023-05-29 10:21:37.000000 pyobjc-core-9.2/Modules/objc/meth-func.m
+-rw-r--r--   0 ronald     (501) staff       (20)      298 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/method-accessor.h
+-rw-r--r--   0 ronald     (501) staff       (20)    19388 2023-05-28 18:38:43.000000 pyobjc-core-9.2/Modules/objc/method-accessor.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1738 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/method-imp.h
+-rw-r--r--   0 ronald     (501) staff       (20)    20511 2023-02-19 11:04:59.000000 pyobjc-core-9.2/Modules/objc/method-imp.m
+-rw-r--r--   0 ronald     (501) staff       (20)     3719 2023-05-27 09:46:33.000000 pyobjc-core-9.2/Modules/objc/method-signature.h
+-rw-r--r--   0 ronald     (501) staff       (20)    66684 2023-05-27 09:46:33.000000 pyobjc-core-9.2/Modules/objc/method-signature.m
+-rw-r--r--   0 ronald     (501) staff       (20)    84443 2023-05-29 07:18:49.000000 pyobjc-core-9.2/Modules/objc/module.m
+-rw-r--r--   0 ronald     (501) staff       (20)      202 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/objc-NULL.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1913 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/objc-NULL.m
+-rw-r--r--   0 ronald     (501) staff       (20)     6317 2022-02-06 09:24:04.000000 pyobjc-core-9.2/Modules/objc/objc-class.h
+-rw-r--r--   0 ronald     (501) staff       (20)   106107 2023-05-29 09:30:59.000000 pyobjc-core-9.2/Modules/objc/objc-class.m
+-rw-r--r--   0 ronald     (501) staff       (20)     2256 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/objc-object.h
+-rw-r--r--   0 ronald     (501) staff       (20)    41490 2023-05-28 19:04:06.000000 pyobjc-core-9.2/Modules/objc/objc-object.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1816 2023-03-24 18:54:07.000000 pyobjc-core-9.2/Modules/objc/objc-runtime-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1598 2023-03-24 18:54:07.000000 pyobjc-core-9.2/Modules/objc/objc-runtime-compat.m
+-rw-r--r--   0 ronald     (501) staff       (20)      172 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/objc_super.h
+-rw-r--r--   0 ronald     (501) staff       (20)     7154 2023-05-28 18:40:37.000000 pyobjc-core-9.2/Modules/objc/objc_super.m
+-rw-r--r--   0 ronald     (501) staff       (20)     4541 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/objc_support.h
+-rw-r--r--   0 ronald     (501) staff       (20)    99903 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/objc_support.m
+-rw-r--r--   0 ronald     (501) staff       (20)     5758 2023-05-13 09:20:57.000000 pyobjc-core-9.2/Modules/objc/objc_util.h
+-rw-r--r--   0 ronald     (501) staff       (20)    47338 2023-05-13 09:20:57.000000 pyobjc-core-9.2/Modules/objc/objc_util.m
+-rw-r--r--   0 ronald     (501) staff       (20)      392 2021-10-18 19:38:40.000000 pyobjc-core-9.2/Modules/objc/opaque-pointer.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13600 2022-04-11 08:03:15.000000 pyobjc-core-9.2/Modules/objc/opaque-pointer.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1462 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/options.h
+-rw-r--r--   0 ronald     (501) staff       (20)    16737 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/options.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1165 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/pointer-support.h
+-rw-r--r--   0 ronald     (501) staff       (20)     9538 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/pointer-support.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1027 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/proxy-registry.h
+-rw-r--r--   0 ronald     (501) staff       (20)     2766 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/proxy-registry.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)     3118 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/pyobjc-api.m
+-rw-r--r--   0 ronald     (501) staff       (20)     3105 2022-02-06 09:24:04.000000 pyobjc-core-9.2/Modules/objc/pyobjc-assert.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-05-29 07:18:42.000000 pyobjc-core-9.2/Modules/objc/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     5846 2023-05-28 19:04:06.000000 pyobjc-core-9.2/Modules/objc/pyobjc-compat.m
+-rw-r--r--   0 ronald     (501) staff       (20)     5911 2021-10-18 19:38:40.000000 pyobjc-core-9.2/Modules/objc/pyobjc-unittest.h
+-rw-r--r--   0 ronald     (501) staff       (20)     4783 2023-05-29 10:07:35.000000 pyobjc-core-9.2/Modules/objc/pyobjc.h
+-rw-r--r--   0 ronald     (501) staff       (20)      435 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/pyobjc_unicode.h
+-rw-r--r--   0 ronald     (501) staff       (20)    16531 2023-03-26 10:00:44.000000 pyobjc-core-9.2/Modules/objc/pyobjc_unicode.m
+-rw-r--r--   0 ronald     (501) staff       (20)    22716 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/python-api-used.h
+-rw-r--r--   0 ronald     (501) staff       (20)      482 2021-10-18 19:38:40.000000 pyobjc-core-9.2/Modules/objc/registry.h
+-rw-r--r--   0 ronald     (501) staff       (20)     5666 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/registry.m
+-rw-r--r--   0 ronald     (501) staff       (20)      747 2022-02-24 08:48:42.000000 pyobjc-core-9.2/Modules/objc/released-buffer.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1187 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/released-buffer.m
+-rw-r--r--   0 ronald     (501) staff       (20)     4090 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/selector.h
+-rw-r--r--   0 ronald     (501) staff       (20)    71265 2023-05-29 09:03:25.000000 pyobjc-core-9.2/Modules/objc/selector.m
+-rw-r--r--   0 ronald     (501) staff       (20)      386 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/struct-sockaddr.h
+-rw-r--r--   0 ronald     (501) staff       (20)     8929 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/struct-sockaddr.m
+-rw-r--r--   0 ronald     (501) staff       (20)     6064 2022-01-02 11:04:25.000000 pyobjc-core-9.2/Modules/objc/struct-wrapper.h
+-rw-r--r--   0 ronald     (501) staff       (20)    50180 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/struct-wrapper.m
+-rw-r--r--   0 ronald     (501) staff       (20)     4174 2022-10-18 09:53:23.000000 pyobjc-core-9.2/Modules/objc/super-call.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13534 2023-06-06 12:09:08.000000 pyobjc-core-9.2/Modules/objc/super-call.m
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-06 23:56:13.800810 pyobjc-core-9.2/Modules/objc/test/
+-rw-r--r--   0 ronald     (501) staff       (20)     2570 2021-09-25 14:12:36.000000 pyobjc-core-9.2/Modules/objc/test/NULL.m
+-rw-r--r--   0 ronald     (501) staff       (20)     3083 2022-02-06 09:24:04.000000 pyobjc-core-9.2/Modules/objc/test/arrayint.m
+-rw-r--r--   0 ronald     (501) staff       (20)     8587 2021-09-25 14:12:36.000000 pyobjc-core-9.2/Modules/objc/test/arrays.m
+-rw-r--r--   0 ronald     (501) staff       (20)     5752 2021-10-18 19:38:40.000000 pyobjc-core-9.2/Modules/objc/test/block.m
+-rw-r--r--   0 ronald     (501) staff       (20)     8172 2022-02-06 09:24:04.000000 pyobjc-core-9.2/Modules/objc/test/bufsizeinarg.m
+-rw-r--r--   0 ronald     (501) staff       (20)   113310 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/categories_base.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1318 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_c42.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1318 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_c43.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1318 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_c44.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1318 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_c45.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1318 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_c46.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1318 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_c47.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1318 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_c48.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1318 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_c49.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1318 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_c50.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1318 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_c51.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1318 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_c52.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1318 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_c53.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1318 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_c54.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1318 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_c55.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1318 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_c56.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1318 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_c57.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1318 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_c58.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1318 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_c59.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1334 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_gp10.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1334 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_gp11.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1334 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_gp12.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1334 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_gp13.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1334 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_gp14.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1334 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_gp15.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1334 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_gp16.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1334 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_gp17.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1334 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_gp18.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1334 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_gp19.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1334 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_gp20.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1334 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_gp21.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1334 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_gp22.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1334 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_gp23.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1232 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_gp24.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1232 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_gp27.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1211 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_gp3.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1232 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_gp30.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1232 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_gp33.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1232 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_gp36.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1232 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_gp39.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1232 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_gp42.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1232 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_gp45.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1232 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_gp48.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1232 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_gp51.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1232 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_gp54.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1232 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_gp57.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1313 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_gp6.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1313 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_gp7.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1313 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_gp8.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1313 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_gp9.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1318 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_p24.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1318 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_p25.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1318 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_p26.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1318 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_p27.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1318 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_p28.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1318 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_p29.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1318 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_p30.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1318 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_p31.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1318 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_p32.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1318 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_p33.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1318 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_p34.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1318 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_p35.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1318 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_p36.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1318 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_p37.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1318 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_p38.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1318 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_p39.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1318 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_p40.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1318 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/category_p41.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1002 2021-09-25 14:12:36.000000 pyobjc-core-9.2/Modules/objc/test/cfsocket.m
+-rw-r--r--   0 ronald     (501) staff       (20)      872 2021-09-25 14:12:36.000000 pyobjc-core-9.2/Modules/objc/test/classes.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1499 2021-09-25 14:12:36.000000 pyobjc-core-9.2/Modules/objc/test/clinmeth.m
+-rw-r--r--   0 ronald     (501) staff       (20)     3145 2022-01-16 10:44:28.000000 pyobjc-core-9.2/Modules/objc/test/coding.m
+-rw-r--r--   0 ronald     (501) staff       (20)     2232 2021-10-18 19:38:40.000000 pyobjc-core-9.2/Modules/objc/test/copying.m
+-rw-r--r--   0 ronald     (501) staff       (20)     3645 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/test/corefoundation.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1354 2022-02-06 09:24:04.000000 pyobjc-core-9.2/Modules/objc/test/dataint.m
+-rw-r--r--   0 ronald     (501) staff       (20)     2647 2022-02-06 09:24:04.000000 pyobjc-core-9.2/Modules/objc/test/dateint.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1332 2021-09-25 14:12:36.000000 pyobjc-core-9.2/Modules/objc/test/decimal.m
+-rw-r--r--   0 ronald     (501) staff       (20)     2218 2021-09-25 14:12:36.000000 pyobjc-core-9.2/Modules/objc/test/deprecations.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1937 2022-02-06 09:24:04.000000 pyobjc-core-9.2/Modules/objc/test/dictint.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1182 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/test/enumeration.m
+-rw-r--r--   0 ronald     (501) staff       (20)     2661 2022-01-02 11:04:25.000000 pyobjc-core-9.2/Modules/objc/test/exceptions.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1350 2022-02-06 09:24:04.000000 pyobjc-core-9.2/Modules/objc/test/filepointer.m
+-rw-r--r--   0 ronald     (501) staff       (20)     2180 2021-10-18 19:38:40.000000 pyobjc-core-9.2/Modules/objc/test/fsref.m
+-rw-r--r--   0 ronald     (501) staff       (20)      962 2022-01-02 11:04:25.000000 pyobjc-core-9.2/Modules/objc/test/gcov.m
+-rw-r--r--   0 ronald     (501) staff       (20)     2301 2022-01-02 11:04:25.000000 pyobjc-core-9.2/Modules/objc/test/helpernsdata.m
+-rw-r--r--   0 ronald     (501) staff       (20)     2651 2022-01-02 11:04:25.000000 pyobjc-core-9.2/Modules/objc/test/helpernsobject.m
+-rw-r--r--   0 ronald     (501) staff       (20)     3745 2021-09-25 14:12:36.000000 pyobjc-core-9.2/Modules/objc/test/identity.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1925 2021-09-25 14:12:36.000000 pyobjc-core-9.2/Modules/objc/test/initialize.m
+-rw-r--r--   0 ronald     (501) staff       (20)     2090 2021-09-25 14:12:36.000000 pyobjc-core-9.2/Modules/objc/test/instanceVariables.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1657 2021-10-18 19:38:40.000000 pyobjc-core-9.2/Modules/objc/test/locking.m
+-rw-r--r--   0 ronald     (501) staff       (20)    18896 2021-10-18 19:38:40.000000 pyobjc-core-9.2/Modules/objc/test/metadata.m
+-rw-r--r--   0 ronald     (501) staff       (20)    14015 2022-01-02 11:04:25.000000 pyobjc-core-9.2/Modules/objc/test/metadatafunction.m
+-rw-r--r--   0 ronald     (501) staff       (20)      883 2022-03-17 11:48:54.000000 pyobjc-core-9.2/Modules/objc/test/methodaccess.m
+-rw-r--r--   0 ronald     (501) staff       (20)     2689 2021-09-25 14:12:36.000000 pyobjc-core-9.2/Modules/objc/test/methodlookup.m
+-rw-r--r--   0 ronald     (501) staff       (20)      659 2021-10-18 19:38:40.000000 pyobjc-core-9.2/Modules/objc/test/methres1.m
+-rw-r--r--   0 ronald     (501) staff       (20)      648 2021-10-18 19:38:40.000000 pyobjc-core-9.2/Modules/objc/test/methres2.m
+-rw-r--r--   0 ronald     (501) staff       (20)      932 2022-01-10 12:42:10.000000 pyobjc-core-9.2/Modules/objc/test/misc.m
+-rw-r--r--   0 ronald     (501) staff       (20)      548 2022-01-02 11:04:25.000000 pyobjc-core-9.2/Modules/objc/test/missing1.m
+-rw-r--r--   0 ronald     (501) staff       (20)      579 2022-01-02 11:04:25.000000 pyobjc-core-9.2/Modules/objc/test/missing2.m
+-rw-r--r--   0 ronald     (501) staff       (20)      590 2022-01-02 11:04:25.000000 pyobjc-core-9.2/Modules/objc/test/missing3.m
+-rw-r--r--   0 ronald     (501) staff       (20)      969 2022-03-17 11:48:54.000000 pyobjc-core-9.2/Modules/objc/test/nsobjectcategory.m
+-rw-r--r--   0 ronald     (501) staff       (20)     3275 2022-02-06 09:24:04.000000 pyobjc-core-9.2/Modules/objc/test/nulldelimitedresult.m
+-rw-r--r--   0 ronald     (501) staff       (20)    18000 2022-03-02 19:57:48.000000 pyobjc-core-9.2/Modules/objc/test/objectint.m
+-rw-r--r--   0 ronald     (501) staff       (20)     3955 2022-01-02 11:04:25.000000 pyobjc-core-9.2/Modules/objc/test/opaque.m
+-rw-r--r--   0 ronald     (501) staff       (20)     3002 2022-03-03 08:50:28.000000 pyobjc-core-9.2/Modules/objc/test/pointersupport.m
+-rw-r--r--   0 ronald     (501) staff       (20)     2834 2021-10-18 19:38:40.000000 pyobjc-core-9.2/Modules/objc/test/properties.m
+-rw-r--r--   0 ronald     (501) staff       (20)      946 2021-09-25 14:12:36.000000 pyobjc-core-9.2/Modules/objc/test/protected.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1906 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/test/protocol.m
+-rw-r--r--   0 ronald     (501) staff       (20)     5523 2022-02-06 09:24:04.000000 pyobjc-core-9.2/Modules/objc/test/pythonnumber.m
+-rw-r--r--   0 ronald     (501) staff       (20)     4549 2022-02-06 09:24:04.000000 pyobjc-core-9.2/Modules/objc/test/pythonset.m
+-rw-r--r--   0 ronald     (501) staff       (20)     2296 2021-09-25 14:12:36.000000 pyobjc-core-9.2/Modules/objc/test/sequence.m
+-rw-r--r--   0 ronald     (501) staff       (20)     4398 2022-02-06 09:24:04.000000 pyobjc-core-9.2/Modules/objc/test/sockaddr.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9499 2021-10-18 19:38:40.000000 pyobjc-core-9.2/Modules/objc/test/specialtypecodes.m
+-rw-r--r--   0 ronald     (501) staff       (20)     2011 2022-02-06 09:24:04.000000 pyobjc-core-9.2/Modules/objc/test/stringint.m
+-rw-r--r--   0 ronald     (501) staff       (20)     2056 2021-09-25 14:12:36.000000 pyobjc-core-9.2/Modules/objc/test/structargs.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1748 2022-01-02 11:04:25.000000 pyobjc-core-9.2/Modules/objc/test/structpointer1.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1110 2021-09-25 14:12:36.000000 pyobjc-core-9.2/Modules/objc/test/structpointer2.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1723 2021-09-25 14:12:36.000000 pyobjc-core-9.2/Modules/objc/test/structs.m
+-rw-r--r--   0 ronald     (501) staff       (20)    49424 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/test/testbndl.m
+-rw-r--r--   0 ronald     (501) staff       (20)   750751 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/test/testbndl2.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1894 2021-09-25 14:12:36.000000 pyobjc-core-9.2/Modules/objc/test/testclassandinst.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1715 2021-09-25 14:12:36.000000 pyobjc-core-9.2/Modules/objc/test/testoutputinitializer.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9114 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/vector.m
+-rw-r--r--   0 ronald     (501) staff       (20)   279993 2023-05-04 11:00:06.000000 pyobjc-core-9.2/Modules/objc/test/vectorcall.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1145 2021-09-25 14:12:36.000000 pyobjc-core-9.2/Modules/objc/test/voidpointer.m
+-rw-r--r--   0 ronald     (501) staff       (20)      761 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/varlist.h
+-rw-r--r--   0 ronald     (501) staff       (20)    14359 2023-02-19 11:11:08.000000 pyobjc-core-9.2/Modules/objc/varlist.m
+-rw-r--r--   0 ronald     (501) staff       (20)      180 2023-02-19 10:50:33.000000 pyobjc-core-9.2/Modules/objc/weakref.h
+-rw-r--r--   0 ronald     (501) staff       (20)     5500 2023-02-19 11:14:37.000000 pyobjc-core-9.2/Modules/objc/weakref.m
+-rw-r--r--   0 ronald     (501) staff       (20)     2238 2023-06-06 23:56:14.413847 pyobjc-core-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-06 23:56:14.238788 pyobjc-core-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       59 2020-11-30 18:45:14.000000 pyobjc-core-9.2/PyObjCTest/__init__.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-06 23:56:14.241080 pyobjc-core-9.2/PyObjCTest/archives/
+-rw-r--r--   0 ronald     (501) staff       (20)     1940 2020-11-30 18:45:14.000000 pyobjc-core-9.2/PyObjCTest/archives/py2-oc2.3.keyed
+-rw-r--r--   0 ronald     (501) staff       (20)      736 2020-11-30 18:45:14.000000 pyobjc-core-9.2/PyObjCTest/archives/py2-oc2.3.plain
+-rw-r--r--   0 ronald     (501) staff       (20)     1706 2020-11-30 18:45:14.000000 pyobjc-core-9.2/PyObjCTest/archives/py3-oc3.0.keyed
+-rw-r--r--   0 ronald     (501) staff       (20)      555 2020-11-30 18:45:14.000000 pyobjc-core-9.2/PyObjCTest/archives/py3-oc3.0.plain
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-06 23:56:13.283021 pyobjc-core-9.2/PyObjCTest/data_bridgesupport/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-06 23:56:14.241683 pyobjc-core-9.2/PyObjCTest/data_bridgesupport/bundle_data/
+-rw-r--r--   0 ronald     (501) staff       (20)       65 2020-11-30 18:45:14.000000 pyobjc-core-9.2/PyObjCTest/data_bridgesupport/bundle_data/Test.bridgesupport
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-06 23:56:14.242510 pyobjc-core-9.2/PyObjCTest/data_bridgesupport/with_data/
+-rw-r--r--   0 ronald     (501) staff       (20)      103 2020-11-30 18:45:14.000000 pyobjc-core-9.2/PyObjCTest/data_bridgesupport/with_data/Test.bridgesupport
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-06 23:56:14.243698 pyobjc-core-9.2/PyObjCTest/data_bridgesupport/with_data_dylib/
+-rw-r--r--   0 ronald     (501) staff       (20)      105 2020-11-30 18:45:14.000000 pyobjc-core-9.2/PyObjCTest/data_bridgesupport/with_data_dylib/Test.bridgesupport
+-rw-r--r--   0 ronald     (501) staff       (20)       13 2020-11-30 18:45:14.000000 pyobjc-core-9.2/PyObjCTest/data_bridgesupport/with_data_dylib/Test.dylib
+-rw-r--r--   0 ronald     (501) staff       (20)     2742 2022-03-05 09:55:08.000000 pyobjc-core-9.2/PyObjCTest/dump-nsarchive-securecoding.m
+-rw-r--r--   0 ronald     (501) staff       (20)     2450 2020-11-30 18:45:14.000000 pyobjc-core-9.2/PyObjCTest/dump-nsarchive.m
+-rw-r--r--   0 ronald     (501) staff       (20)      410 2020-11-30 18:45:14.000000 pyobjc-core-9.2/PyObjCTest/fnd.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2983 2023-03-03 17:21:59.000000 pyobjc-core-9.2/PyObjCTest/helper_bridgesupport.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2919 2020-11-30 18:45:14.000000 pyobjc-core-9.2/PyObjCTest/keyvaluehelper.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1506 2023-03-03 17:21:59.000000 pyobjc-core-9.2/PyObjCTest/loader.py
+-rw-r--r--   0 ronald     (501) staff       (20)     7342 2023-03-03 17:21:59.000000 pyobjc-core-9.2/PyObjCTest/test_NULL.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1200 2022-01-02 11:20:34.000000 pyobjc-core-9.2/PyObjCTest/test_allocatebuffer.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1021 2022-01-02 11:04:25.000000 pyobjc-core-9.2/PyObjCTest/test_api_import.py
+-rw-r--r--   0 ronald     (501) staff       (20)    58667 2023-05-04 11:00:06.000000 pyobjc-core-9.2/PyObjCTest/test_archive_python.py
+-rw-r--r--   0 ronald     (501) staff       (20)    14033 2023-05-04 11:00:06.000000 pyobjc-core-9.2/PyObjCTest/test_archiving_interop.py
+-rw-r--r--   0 ronald     (501) staff       (20)    10830 2023-03-03 17:21:59.000000 pyobjc-core-9.2/PyObjCTest/test_archiving_secure_interop.py
+-rw-r--r--   0 ronald     (501) staff       (20)    13566 2023-03-03 17:21:59.000000 pyobjc-core-9.2/PyObjCTest/test_array_interface.py
+-rw-r--r--   0 ronald     (501) staff       (20)    25640 2022-01-02 11:04:25.000000 pyobjc-core-9.2/PyObjCTest/test_array_property.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6180 2023-03-03 17:21:59.000000 pyobjc-core-9.2/PyObjCTest/test_arrays.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3840 2023-03-03 17:21:59.000000 pyobjc-core-9.2/PyObjCTest/test_assocations.py
+-rw-r--r--   0 ronald     (501) staff       (20)    14826 2022-01-02 11:04:25.000000 pyobjc-core-9.2/PyObjCTest/test_blocks.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5684 2022-02-06 09:24:04.000000 pyobjc-core-9.2/PyObjCTest/test_bridged_classes.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1855 2021-03-21 10:08:22.000000 pyobjc-core-9.2/PyObjCTest/test_bridges.py
+-rw-r--r--   0 ronald     (501) staff       (20)   105009 2023-03-26 10:33:23.000000 pyobjc-core-9.2/PyObjCTest/test_bridgesupport.py
+-rw-r--r--   0 ronald     (501) staff       (20)    12620 2022-02-06 09:24:04.000000 pyobjc-core-9.2/PyObjCTest/test_bufsizeinarg.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6970 2022-10-31 15:31:40.000000 pyobjc-core-9.2/PyObjCTest/test_bundleFunctions.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6338 2022-10-31 15:31:40.000000 pyobjc-core-9.2/PyObjCTest/test_bundleVariables.py
+-rw-r--r--   0 ronald     (501) staff       (20)    34668 2023-02-19 10:50:33.000000 pyobjc-core-9.2/PyObjCTest/test_callable_docstr.py
+-rw-r--r--   0 ronald     (501) staff       (20)     8948 2023-02-19 10:50:33.000000 pyobjc-core-9.2/PyObjCTest/test_callbacks.py
+-rw-r--r--   0 ronald     (501) staff       (20)   122281 2023-05-04 11:00:06.000000 pyobjc-core-9.2/PyObjCTest/test_categories.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3901 2023-03-03 17:21:59.000000 pyobjc-core-9.2/PyObjCTest/test_classandinst.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1199 2021-07-30 09:00:36.000000 pyobjc-core-9.2/PyObjCTest/test_classhooks.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2795 2022-01-02 11:04:25.000000 pyobjc-core-9.2/PyObjCTest/test_clinmeth.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2583 2023-02-19 10:50:33.000000 pyobjc-core-9.2/PyObjCTest/test_compat.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2615 2021-08-04 10:12:03.000000 pyobjc-core-9.2/PyObjCTest/test_constants.py
+-rw-r--r--   0 ronald     (501) staff       (20)      735 2022-01-02 11:04:25.000000 pyobjc-core-9.2/PyObjCTest/test_context.py
+-rw-r--r--   0 ronald     (501) staff       (20)    18128 2023-05-27 09:46:33.000000 pyobjc-core-9.2/PyObjCTest/test_convenience.py
+-rw-r--r--   0 ronald     (501) staff       (20)    26647 2022-02-06 09:24:04.000000 pyobjc-core-9.2/PyObjCTest/test_conversion.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6891 2023-02-19 10:50:33.000000 pyobjc-core-9.2/PyObjCTest/test_copying.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4329 2023-03-03 17:21:59.000000 pyobjc-core-9.2/PyObjCTest/test_corefoundation.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2349 2023-03-03 17:21:59.000000 pyobjc-core-9.2/PyObjCTest/test_ctests.py
+-rw-r--r--   0 ronald     (501) staff       (20)     8728 2023-05-04 11:00:06.000000 pyobjc-core-9.2/PyObjCTest/test_data_proxy.py
+-rw-r--r--   0 ronald     (501) staff       (20)     9484 2023-05-04 11:00:06.000000 pyobjc-core-9.2/PyObjCTest/test_date_proxy.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1065 2021-03-21 10:08:22.000000 pyobjc-core-9.2/PyObjCTest/test_default_selector.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4123 2022-04-11 08:03:15.000000 pyobjc-core-9.2/PyObjCTest/test_deprecations.py
+-rw-r--r--   0 ronald     (501) staff       (20)    29263 2023-03-03 17:21:59.000000 pyobjc-core-9.2/PyObjCTest/test_descriptors.py
+-rw-r--r--   0 ronald     (501) staff       (20)    31640 2022-03-02 09:33:22.000000 pyobjc-core-9.2/PyObjCTest/test_dict_interface.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1876 2021-03-21 10:08:22.000000 pyobjc-core-9.2/PyObjCTest/test_dict_property.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5621 2023-03-03 17:21:59.000000 pyobjc-core-9.2/PyObjCTest/test_dict_proxy.py
+-rw-r--r--   0 ronald     (501) staff       (20)    16783 2022-01-02 11:20:34.000000 pyobjc-core-9.2/PyObjCTest/test_dyld.py
+-rw-r--r--   0 ronald     (501) staff       (20)      643 2023-02-19 10:50:34.000000 pyobjc-core-9.2/PyObjCTest/test_enumerator.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4340 2022-01-02 11:04:25.000000 pyobjc-core-9.2/PyObjCTest/test_exceptions.py
+-rw-r--r--   0 ronald     (501) staff       (20)     8131 2022-02-06 09:24:04.000000 pyobjc-core-9.2/PyObjCTest/test_filepointer.py
+-rw-r--r--   0 ronald     (501) staff       (20)      728 2021-06-05 10:25:38.000000 pyobjc-core-9.2/PyObjCTest/test_final.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2670 2021-03-21 10:08:22.000000 pyobjc-core-9.2/PyObjCTest/test_framework.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2792 2022-01-02 11:04:25.000000 pyobjc-core-9.2/PyObjCTest/test_fsref.py
+-rw-r--r--   0 ronald     (501) staff       (20)    11393 2023-03-03 17:21:59.000000 pyobjc-core-9.2/PyObjCTest/test_functions.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1162 2022-01-02 11:04:25.000000 pyobjc-core-9.2/PyObjCTest/test_generic_class.py
+-rw-r--r--   0 ronald     (501) staff       (20)     7731 2023-03-03 17:21:59.000000 pyobjc-core-9.2/PyObjCTest/test_hidden_selector.py
+-rw-r--r--   0 ronald     (501) staff       (20)    11080 2023-03-03 17:21:59.000000 pyobjc-core-9.2/PyObjCTest/test_identity.py
+-rw-r--r--   0 ronald     (501) staff       (20)     7231 2022-02-06 09:24:04.000000 pyobjc-core-9.2/PyObjCTest/test_imp.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2583 2021-03-21 10:08:22.000000 pyobjc-core-9.2/PyObjCTest/test_initialized.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2323 2023-02-19 10:50:34.000000 pyobjc-core-9.2/PyObjCTest/test_inspect_signatures.py
+-rw-r--r--   0 ronald     (501) staff       (20)    12703 2022-01-22 09:56:31.000000 pyobjc-core-9.2/PyObjCTest/test_internals.py
+-rw-r--r--   0 ronald     (501) staff       (20)    16659 2023-03-03 17:21:59.000000 pyobjc-core-9.2/PyObjCTest/test_ivar.py
+-rw-r--r--   0 ronald     (501) staff       (20)    30224 2023-03-03 17:21:59.000000 pyobjc-core-9.2/PyObjCTest/test_keyvalue.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1915 2021-03-21 10:08:22.000000 pyobjc-core-9.2/PyObjCTest/test_keyvalue_prop.py
+-rw-r--r--   0 ronald     (501) staff       (20)    26483 2022-01-02 11:04:25.000000 pyobjc-core-9.2/PyObjCTest/test_keyvaluecoding.py
+-rw-r--r--   0 ronald     (501) staff       (20)    33095 2023-03-03 17:21:59.000000 pyobjc-core-9.2/PyObjCTest/test_lazy_import.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2527 2023-03-03 17:21:59.000000 pyobjc-core-9.2/PyObjCTest/test_leaks.py
+-rw-r--r--   0 ronald     (501) staff       (20)    10113 2023-03-03 17:21:59.000000 pyobjc-core-9.2/PyObjCTest/test_list_proxy.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3982 2021-03-21 10:08:22.000000 pyobjc-core-9.2/PyObjCTest/test_locking.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3926 2022-01-02 11:04:25.000000 pyobjc-core-9.2/PyObjCTest/test_machsignals.py
+-rw-r--r--   0 ronald     (501) staff       (20)    54600 2022-02-06 09:24:04.000000 pyobjc-core-9.2/PyObjCTest/test_metadata.py
+-rw-r--r--   0 ronald     (501) staff       (20)    27855 2023-03-03 17:21:59.000000 pyobjc-core-9.2/PyObjCTest/test_metadata_function.py
+-rw-r--r--   0 ronald     (501) staff       (20)    15256 2022-02-06 09:24:04.000000 pyobjc-core-9.2/PyObjCTest/test_metadata_imp.py
+-rw-r--r--   0 ronald     (501) staff       (20)      803 2023-03-03 17:21:59.000000 pyobjc-core-9.2/PyObjCTest/test_metadata_inheritance.py
+-rw-r--r--   0 ronald     (501) staff       (20)    32824 2022-02-06 09:24:04.000000 pyobjc-core-9.2/PyObjCTest/test_metadata_py.py
+-rw-r--r--   0 ronald     (501) staff       (20)    16933 2022-02-06 09:24:04.000000 pyobjc-core-9.2/PyObjCTest/test_metadata_py2py.py
+-rw-r--r--   0 ronald     (501) staff       (20)    17752 2023-02-19 10:50:34.000000 pyobjc-core-9.2/PyObjCTest/test_method_prototypes.py
+-rw-r--r--   0 ronald     (501) staff       (20)    10381 2023-05-27 09:46:33.000000 pyobjc-core-9.2/PyObjCTest/test_methodaccess.py
+-rw-r--r--   0 ronald     (501) staff       (20)    14062 2022-01-22 09:57:03.000000 pyobjc-core-9.2/PyObjCTest/test_methodedits.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5801 2023-02-19 10:50:34.000000 pyobjc-core-9.2/PyObjCTest/test_methodlookup.py
+-rw-r--r--   0 ronald     (501) staff       (20)    59548 2023-03-03 17:21:59.000000 pyobjc-core-9.2/PyObjCTest/test_methods.py
+-rw-r--r--   0 ronald     (501) staff       (20)  2870222 2023-03-03 17:21:59.000000 pyobjc-core-9.2/PyObjCTest/test_methods2.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2217 2022-01-02 11:04:26.000000 pyobjc-core-9.2/PyObjCTest/test_methres.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5686 2023-02-19 10:50:34.000000 pyobjc-core-9.2/PyObjCTest/test_nscoder.py
+-rw-r--r--   0 ronald     (501) staff       (20)    29009 2022-03-02 19:57:48.000000 pyobjc-core-9.2/PyObjCTest/test_nsdata.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1214 2021-03-21 10:08:22.000000 pyobjc-core-9.2/PyObjCTest/test_nsdate_proxy.py
+-rw-r--r--   0 ronald     (501) staff       (20)    13611 2023-02-19 10:50:34.000000 pyobjc-core-9.2/PyObjCTest/test_nsdecimal.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1065 2022-10-18 09:53:23.000000 pyobjc-core-9.2/PyObjCTest/test_nsinvocation.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6608 2022-03-17 11:48:54.000000 pyobjc-core-9.2/PyObjCTest/test_nsobject.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4984 2022-02-24 08:47:16.000000 pyobjc-core-9.2/PyObjCTest/test_nulldelimited.py
+-rw-r--r--   0 ronald     (501) staff       (20)    45321 2023-03-03 17:21:59.000000 pyobjc-core-9.2/PyObjCTest/test_number_proxy.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4038 2023-03-03 17:21:59.000000 pyobjc-core-9.2/PyObjCTest/test_objc.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2106 2023-02-19 10:50:34.000000 pyobjc-core-9.2/PyObjCTest/test_objcpointer.py
+-rw-r--r--   0 ronald     (501) staff       (20)    20238 2023-03-03 17:21:59.000000 pyobjc-core-9.2/PyObjCTest/test_object_property.py
+-rw-r--r--   0 ronald     (501) staff       (20)    22970 2022-02-06 09:24:04.000000 pyobjc-core-9.2/PyObjCTest/test_object_proxy.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6550 2022-02-06 09:24:04.000000 pyobjc-core-9.2/PyObjCTest/test_opaque.py
+-rw-r--r--   0 ronald     (501) staff       (20)    14120 2022-10-31 15:31:40.000000 pyobjc-core-9.2/PyObjCTest/test_options.py
+-rw-r--r--   0 ronald     (501) staff       (20)      550 2021-03-21 10:08:22.000000 pyobjc-core-9.2/PyObjCTest/test_outputinitializer.py
+-rw-r--r--   0 ronald     (501) staff       (20)      887 2022-01-02 11:04:26.000000 pyobjc-core-9.2/PyObjCTest/test_pickle.py
+-rw-r--r--   0 ronald     (501) staff       (20)      426 2021-03-21 10:08:22.000000 pyobjc-core-9.2/PyObjCTest/test_pickling_objc.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6166 2023-03-03 17:21:59.000000 pyobjc-core-9.2/PyObjCTest/test_pointer_compat.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1514 2022-02-06 09:24:04.000000 pyobjc-core-9.2/PyObjCTest/test_posing.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5733 2021-07-30 09:00:36.000000 pyobjc-core-9.2/PyObjCTest/test_propertiesforclass.py
+-rw-r--r--   0 ronald     (501) staff       (20)      310 2021-03-21 10:08:22.000000 pyobjc-core-9.2/PyObjCTest/test_protected.py
+-rw-r--r--   0 ronald     (501) staff       (20)    29394 2023-05-04 11:00:06.000000 pyobjc-core-9.2/PyObjCTest/test_protocol.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1093 2022-01-02 11:04:26.000000 pyobjc-core-9.2/PyObjCTest/test_protocolNamed.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3327 2023-04-09 10:06:25.000000 pyobjc-core-9.2/PyObjCTest/test_python_method.py
+-rw-r--r--   0 ronald     (501) staff       (20)    19425 2023-03-03 17:19:36.000000 pyobjc-core-9.2/PyObjCTest/test_regr.py
+-rw-r--r--   0 ronald     (501) staff       (20)    16157 2022-01-02 11:04:26.000000 pyobjc-core-9.2/PyObjCTest/test_set_interface.py
+-rw-r--r--   0 ronald     (501) staff       (20)    16022 2022-01-02 11:04:26.000000 pyobjc-core-9.2/PyObjCTest/test_set_property.py
+-rw-r--r--   0 ronald     (501) staff       (20)    12947 2023-03-03 17:21:59.000000 pyobjc-core-9.2/PyObjCTest/test_set_proxy.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3319 2022-03-02 09:33:22.000000 pyobjc-core-9.2/PyObjCTest/test_signals.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3013 2023-02-19 10:50:34.000000 pyobjc-core-9.2/PyObjCTest/test_signatures.py
+-rw-r--r--   0 ronald     (501) staff       (20)    11085 2023-02-19 10:50:34.000000 pyobjc-core-9.2/PyObjCTest/test_simd.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5840 2022-02-24 21:31:17.000000 pyobjc-core-9.2/PyObjCTest/test_sockaddr.py
+-rw-r--r--   0 ronald     (501) staff       (20)     7090 2022-01-02 11:04:26.000000 pyobjc-core-9.2/PyObjCTest/test_specialtypecodes_charbyte.py
+-rw-r--r--   0 ronald     (501) staff       (20)     7676 2022-01-02 11:04:26.000000 pyobjc-core-9.2/PyObjCTest/test_specialtypecodes_charint.py
+-rw-r--r--   0 ronald     (501) staff       (20)    20176 2021-03-21 10:08:22.000000 pyobjc-core-9.2/PyObjCTest/test_specialtypecodes_methdef.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6352 2022-01-02 11:04:26.000000 pyobjc-core-9.2/PyObjCTest/test_specialtypecodes_nsbool.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2361 2021-03-21 10:08:22.000000 pyobjc-core-9.2/PyObjCTest/test_specialtypecodes_struct.py
+-rw-r--r--   0 ronald     (501) staff       (20)     7050 2022-01-02 11:04:26.000000 pyobjc-core-9.2/PyObjCTest/test_specialtypecodes_unichar.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6331 2023-03-03 17:21:59.000000 pyobjc-core-9.2/PyObjCTest/test_splitsig.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5270 2023-05-04 11:00:06.000000 pyobjc-core-9.2/PyObjCTest/test_string_proxy.py
+-rw-r--r--   0 ronald     (501) staff       (20)      899 2023-03-03 17:21:59.000000 pyobjc-core-9.2/PyObjCTest/test_structpointer.py
+-rw-r--r--   0 ronald     (501) staff       (20)    34918 2023-02-19 10:50:34.000000 pyobjc-core-9.2/PyObjCTest/test_structs.py
+-rw-r--r--   0 ronald     (501) staff       (20)    36093 2023-05-13 09:20:57.000000 pyobjc-core-9.2/PyObjCTest/test_subclass.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2013 2022-01-02 11:04:26.000000 pyobjc-core-9.2/PyObjCTest/test_synthesize.py
+-rw-r--r--   0 ronald     (501) staff       (20)    93554 2023-05-27 09:46:33.000000 pyobjc-core-9.2/PyObjCTest/test_testsupport.py
+-rw-r--r--   0 ronald     (501) staff       (20)    82866 2023-05-29 09:00:29.000000 pyobjc-core-9.2/PyObjCTest/test_transform.py
+-rw-r--r--   0 ronald     (501) staff       (20)     7514 2023-03-03 17:21:59.000000 pyobjc-core-9.2/PyObjCTest/test_transform_integration.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2596 2022-01-02 11:04:26.000000 pyobjc-core-9.2/PyObjCTest/test_typecheck.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3148 2023-02-19 10:50:34.000000 pyobjc-core-9.2/PyObjCTest/test_unicode.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2426 2021-03-21 10:08:22.000000 pyobjc-core-9.2/PyObjCTest/test_usekvo.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1900 2021-03-21 10:08:22.000000 pyobjc-core-9.2/PyObjCTest/test_varargs.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2380 2023-02-19 10:50:34.000000 pyobjc-core-9.2/PyObjCTest/test_varlist.py
+-rw-r--r--   0 ronald     (501) staff       (20)    21740 2023-05-04 11:00:06.000000 pyobjc-core-9.2/PyObjCTest/test_vector_proxy.py
+-rw-r--r--   0 ronald     (501) staff       (20)  1655689 2023-05-04 11:00:07.000000 pyobjc-core-9.2/PyObjCTest/test_vectorcall.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1775 2022-01-22 09:56:32.000000 pyobjc-core-9.2/PyObjCTest/test_version_support.py
+-rw-r--r--   0 ronald     (501) staff       (20)      444 2021-03-21 10:08:22.000000 pyobjc-core-9.2/PyObjCTest/test_voidpointer.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4115 2023-03-03 17:21:59.000000 pyobjc-core-9.2/PyObjCTest/test_weakref.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1172 2020-11-30 18:45:14.000000 pyobjc-core-9.2/README.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-06 23:56:14.409587 pyobjc-core-9.2/Tools/
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-core-9.2/Tools/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     1446 2023-05-04 11:00:07.000000 pyobjc-core-9.2/Tools/comparebench.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1662 2023-03-03 17:21:59.000000 pyobjc-core-9.2/Tools/gen_archive.py
+-rw-r--r--   0 ronald     (501) staff       (20)    23741 2023-05-04 11:00:07.000000 pyobjc-core-9.2/Tools/generate-category-tests.py
+-rwxr-xr-x   0 ronald     (501) staff       (20)    49737 2023-05-04 11:00:07.000000 pyobjc-core-9.2/Tools/generate-helpers-vector.py
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-core-9.2/Tools/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6919 2022-01-02 11:20:34.000000 pyobjc-core-9.2/Tools/pyobjcbench.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-06 23:56:14.412206 pyobjc-core-9.2/Tools/results/
+-rw-r--r--   0 ronald     (501) staff       (20)      602 2021-10-02 09:43:54.000000 pyobjc-core-9.2/Tools/results/pyobjcbench-7.3.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      604 2021-09-30 19:06:24.000000 pyobjc-core-9.2/Tools/results/pyobjcbench-8.0b1.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      604 2021-10-02 09:43:31.000000 pyobjc-core-9.2/Tools/results/pyobjcbench-8.0b2.txt
+-rwxr-xr-x   0 ronald     (501) staff       (20)      566 2022-10-18 09:53:23.000000 pyobjc-core-9.2/Tools/runtests-with-nuitka.py
+-rw-r--r--   0 ronald     (501) staff       (20)      872 2022-10-18 09:53:23.000000 pyobjc-core-9.2/Tools/runtests.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3113 2023-03-26 10:19:28.000000 pyobjc-core-9.2/diff.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-core-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)     1943 2023-06-06 23:56:14.414563 pyobjc-core-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)    23169 2023-06-06 09:49:42.000000 pyobjc-core-9.2/setup.py
```

### Comparing `pyobjc-core-9.1b1/Examples/00ReadMe.txt` & `pyobjc-core-9.2/Examples/00ReadMe.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Examples/GUITests/test_modalsession.py` & `pyobjc-core-9.2/Examples/GUITests/test_modalsession.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Examples/NonFunctional/RemotePyInterpreter/AsyncPythonInterpreter.py` & `pyobjc-core-9.2/Examples/NonFunctional/RemotePyInterpreter/AsyncPythonInterpreter.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Examples/NonFunctional/RemotePyInterpreter/ConsoleReactor.py` & `pyobjc-core-9.2/Examples/NonFunctional/RemotePyInterpreter/ConsoleReactor.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Examples/NonFunctional/RemotePyInterpreter/English.lproj/MainMenu.nib/info.nib` & `pyobjc-core-9.2/Examples/NonFunctional/RemotePyInterpreter/English.lproj/MainMenu.nib/info.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Examples/NonFunctional/RemotePyInterpreter/English.lproj/MainMenu.nib/keyedobjects.nib` & `pyobjc-core-9.2/Examples/NonFunctional/RemotePyInterpreter/English.lproj/MainMenu.nib/keyedobjects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Examples/NonFunctional/RemotePyInterpreter/English.lproj/RemotePyInterpreterDocument.nib/classes.nib` & `pyobjc-core-9.2/Examples/NonFunctional/RemotePyInterpreter/English.lproj/RemotePyInterpreterDocument.nib/classes.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Examples/NonFunctional/RemotePyInterpreter/English.lproj/RemotePyInterpreterDocument.nib/keyedobjects.nib` & `pyobjc-core-9.2/Examples/NonFunctional/RemotePyInterpreter/English.lproj/RemotePyInterpreterDocument.nib/keyedobjects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Examples/NonFunctional/RemotePyInterpreter/RemotePyInterpreter.py` & `pyobjc-core-9.2/Examples/NonFunctional/RemotePyInterpreter/RemotePyInterpreter.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Examples/NonFunctional/RemotePyInterpreter/netrepr.py` & `pyobjc-core-9.2/Examples/NonFunctional/RemotePyInterpreter/netrepr.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Examples/NonFunctional/RemotePyInterpreter/remote_bootstrap.py` & `pyobjc-core-9.2/Examples/NonFunctional/RemotePyInterpreter/remote_bootstrap.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Examples/NonFunctional/RemotePyInterpreter/remote_console.py` & `pyobjc-core-9.2/Examples/NonFunctional/RemotePyInterpreter/remote_console.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Examples/NonFunctional/RemotePyInterpreter/remote_pipe.py` & `pyobjc-core-9.2/Examples/NonFunctional/RemotePyInterpreter/remote_pipe.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Examples/NonFunctional/RemotePyInterpreter/setup.py` & `pyobjc-core-9.2/Examples/NonFunctional/RemotePyInterpreter/setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Examples/NonFunctional/RemotePyInterpreter/tcpinterpreter.py` & `pyobjc-core-9.2/Examples/NonFunctional/RemotePyInterpreter/tcpinterpreter.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Examples/NonFunctional/RemotePyInterpreter/test_client.py` & `pyobjc-core-9.2/Examples/NonFunctional/RemotePyInterpreter/test_client.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Examples/Scripts/HelloWorld.py` & `pyobjc-core-9.2/Examples/Scripts/HelloWorld.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Examples/Scripts/autoreadme.py` & `pyobjc-core-9.2/Examples/Scripts/autoreadme.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Examples/Scripts/instrumentSends.py` & `pyobjc-core-9.2/Examples/Scripts/instrumentSends.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Examples/Scripts/kvo-debugging.py` & `pyobjc-core-9.2/Examples/Scripts/kvo-debugging.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Examples/Scripts/stdinreader.py` & `pyobjc-core-9.2/Examples/Scripts/stdinreader.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Examples/Scripts/subclassing-objective-c.py` & `pyobjc-core-9.2/Examples/Scripts/subclassing-objective-c.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Examples/Scripts/wmEnable.py` & `pyobjc-core-9.2/Examples/Scripts/wmEnable.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/HISTORIC.txt` & `pyobjc-core-9.2/HISTORIC.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Install.txt` & `pyobjc-core-9.2/Install.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Lib/PyObjCTools/KeyValueCoding.py` & `pyobjc-core-9.2/Lib/PyObjCTools/KeyValueCoding.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Lib/PyObjCTools/MachSignals.py` & `pyobjc-core-9.2/Lib/PyObjCTools/MachSignals.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Lib/PyObjCTools/Signals.py` & `pyobjc-core-9.2/Lib/PyObjCTools/Signals.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Lib/PyObjCTools/TestSupport.py` & `pyobjc-core-9.2/Lib/PyObjCTools/TestSupport.py`

 * *Files 1% similar despite different names*

```diff
@@ -1174,14 +1174,44 @@
                 if rest.startswith(objc._C_STRUCT_B):
                     name, fields = objc.splitStructSignature(rest)
                     if not fields:
                         self.fail(
                             f"{value}: {idx}: byref to empty struct (handle/CFType?): {tp} {class_name or ''}"
                         )
 
+            if not isinstance(value, objc.selector):
+                # This gives too many false positives for selectors (sadly)
+                if (
+                    tp.startswith(objc._C_PTR)
+                    and tp not in (b"^v", b"^?")
+                    and tp != b"^{AudioBufferList=I[1{AudioBuffer=II^v}]}"
+                    and tp != b"^{_CFArrayCallBacks=q^?^?^?^?}"
+                ):
+                    if tp[1:].startswith(objc._C_STRUCT_B):
+                        name, fields = objc.splitStructSignature(tp[1:])
+                        if not fields:
+                            continue
+
+                    if idx == "retval":
+                        if any(
+                            x in meta
+                            for x in {
+                                "deref_result_pointer",
+                                "c_array_delimited_by_null",
+                                "c_array_of_variable_length",
+                                "c_array_length_in_arg",
+                                "c_array_delimited_by_null",
+                                "c_array_size_in_arg",
+                            }
+                        ):
+                            continue
+                    self.fail(
+                        f"{value}: {idx}: pointer argument, but no by-ref annotation:{tp!r} {class_name or ''}"
+                    )
+
     def assertCallableMetadataIsSane(
         self, module, *, exclude_cocoa=True, exclude_attrs=()
     ):
         # Do some sanity checking on module metadata for
         # callables.
         #
         # This test is *very* expensive, made slightly
@@ -1265,15 +1295,17 @@
                 parent = todo.pop()
                 if isinstance(parent, objc.ObjCLazyModule):
                     module_names.extend(parent._ObjCLazyModule__funcmap or ())
                     todo.extend(parent._ObjCLazyModule__parents or ())
                     module_names.extend(parent.__dict__.keys())
                 else:
                     module_names.extend(dir(module))
-            module_names.sort()
+
+            # The module_names list might contain duplicates
+            module_names = sorted(set(module_names))
         else:
             module_names = sorted(dir(module))
 
         for _idx, nm in enumerate(module_names):
             # print(f"{_idx}/{len(module_names)} {nm}")
             if nm in exclude_names:
                 continue
```

### Comparing `pyobjc-core-9.1b1/Lib/objc/__init__.py` & `pyobjc-core-9.2/Lib/objc/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Lib/objc/_bridges.py` & `pyobjc-core-9.2/Lib/objc/_bridges.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Lib/objc/_bridgesupport.py` & `pyobjc-core-9.2/Lib/objc/_bridgesupport.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Lib/objc/_callable_docstr.py` & `pyobjc-core-9.2/Lib/objc/_callable_docstr.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Lib/objc/_category.py` & `pyobjc-core-9.2/Lib/objc/_category.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Lib/objc/_compat.py` & `pyobjc-core-9.2/Lib/objc/_compat.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Lib/objc/_context.py` & `pyobjc-core-9.2/Lib/objc/_context.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Lib/objc/_convenience.py` & `pyobjc-core-9.2/Lib/objc/_convenience.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Lib/objc/_convenience_mapping.py` & `pyobjc-core-9.2/Lib/objc/_convenience_mapping.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Lib/objc/_convenience_nsarray.py` & `pyobjc-core-9.2/Lib/objc/_convenience_nsarray.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Lib/objc/_convenience_nsdata.py` & `pyobjc-core-9.2/Lib/objc/_convenience_nsdata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Lib/objc/_convenience_nsdecimal.py` & `pyobjc-core-9.2/Lib/objc/_convenience_nsdecimal.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Lib/objc/_convenience_nsdictionary.py` & `pyobjc-core-9.2/Lib/objc/_convenience_nsdictionary.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Lib/objc/_convenience_nsobject.py` & `pyobjc-core-9.2/Lib/objc/_convenience_nsobject.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Lib/objc/_convenience_nsset.py` & `pyobjc-core-9.2/Lib/objc/_convenience_nsset.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Lib/objc/_convenience_nsstring.py` & `pyobjc-core-9.2/Lib/objc/_convenience_nsstring.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Lib/objc/_convenience_sequence.py` & `pyobjc-core-9.2/Lib/objc/_convenience_sequence.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Lib/objc/_descriptors.py` & `pyobjc-core-9.2/Lib/objc/_descriptors.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Lib/objc/_dyld.py` & `pyobjc-core-9.2/Lib/objc/_dyld.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Lib/objc/_framework.py` & `pyobjc-core-9.2/Lib/objc/_framework.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Lib/objc/_informal_protocol.py` & `pyobjc-core-9.2/Lib/objc/_informal_protocol.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Lib/objc/_lazyimport.py` & `pyobjc-core-9.2/Lib/objc/_lazyimport.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Lib/objc/_locking.py` & `pyobjc-core-9.2/Lib/objc/_locking.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Lib/objc/_properties.py` & `pyobjc-core-9.2/Lib/objc/_properties.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Lib/objc/_protocols.py` & `pyobjc-core-9.2/Lib/objc/_protocols.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Lib/objc/_pycoder.py` & `pyobjc-core-9.2/Lib/objc/_pycoder.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Lib/objc/_pythonify.py` & `pyobjc-core-9.2/Lib/objc/_pythonify.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Lib/objc/_structtype.py` & `pyobjc-core-9.2/Lib/objc/_structtype.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Lib/objc/_transform.py` & `pyobjc-core-9.2/Lib/objc/_transform.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 """
 import objc
 import types
 import inspect
 import dis
 import keyword
 import warnings
+import sys
 from ._informal_protocol import _informal_protocol_for_selector
 
 # only public objc_method until the python_method implementation
 # in C is gone
 __all__ = ("objc_method", "python_method")
 
 
@@ -43,14 +44,29 @@
     for p in protocols:
         if not isinstance(p, (objc.formal_protocol, objc.informal_protocol)):
             raise TypeError(
                 "protocols list contains object that isn't an Objective-C "
                 f"protocol, but type {type(p).__name__}"
             )
 
+    if "__classcell__" in class_dict and "__module__" in class_dict:
+        mod = sys.modules.get(class_dict["__module__"], None)
+        if mod is not None:
+            try:
+                ok = mod.super is objc.super
+            except AttributeError:
+                ok = False
+
+            if not ok:
+                warnings.warn(
+                    "Objective-C subclass uses super(), but super is not objc.super",
+                    category=objc.ObjCSuperWarning,
+                    stacklevel=2,
+                )
+
     super_ivars = set()
     for v in class_object.__dict__.values():
         if isinstance(v, objc.ivar):
             super_ivars.add(v.__name__)
 
     class_dict["__objc_python_subclass__"] = True
     process_slots(class_dict, instance_variables, class_object)
@@ -60,20 +76,25 @@
     # loop# cannot be merged into the next one.
     for key, value in list(class_dict.items()):
         setup = getattr(value, "__pyobjc_class_setup__", NO_VALUE)
         if setup is not NO_VALUE:
             setup(key, class_dict, instance_methods, class_methods)
 
     for key, value in list(class_dict.items()):
+        old_value = value
         new_value = transformAttribute(key, value, class_object, protocols)
         if new_value is not value:
             class_dict[key] = new_value
             value = new_value
 
         if isinstance(value, objc.selector):
+            if isinstance(old_value, python_method):
+                continue
+
+        if isinstance(value, objc.selector):
             canonical = value.selector.decode().replace(":", "_")
 
             if value.isClassMethod:
                 del class_dict[key]
                 if not value.isHidden:
                     meta_dict[key] = value
                     if canonical != key:
@@ -470,16 +491,18 @@
                     f"{value!r} has {pos-1} positional arguments"
                 )
 
     # XXX: This is needed because SomeClass.pyobjc_instanceMethods.hiddenSelector.isHidden
     #      is false :-(
     ishidden = False
     for cls in class_object.mro():  # pragma: no branch
-        if cls is object:
-            break
+        if not issubclass(cls, objc.objc_object):
+            # Skip all non-objc class in the MRO to ignore
+            # mixin classees.
+            continue
         if selname in cls.pyobjc_hiddenSelectors(isclass):
             ishidden = True
             break
 
     return objc.selector(
         value, selname, signature, isClassMethod=isclass, isHidden=ishidden
     )
@@ -520,14 +543,20 @@
         if inst.opname == "RETURN_VALUE":
             assert prev is not None
             if prev.opname == "LOAD_CONST" and prev.arg != 0:
                 return True
             elif prev.opname != "LOAD_CONST":
                 return True
 
+        elif inst.opname == "RETURN_CONST" and inst.arg != 0:
+            # New in Python 3.12.
+            # XXX: This will give a false positive for functions
+            #      that only contain "return None" paths for
+            #      returning a value.
+            return True
         prev = inst
 
     return False
 
 
 def default_selector(name):
     """
```

### Comparing `pyobjc-core-9.1b1/Lib/objc/simd.py` & `pyobjc-core-9.2/Lib/objc/simd.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Lib/pyobjc_core.egg-info/PKG-INFO` & `pyobjc-core-9.2/Lib/pyobjc_core.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-core
-Version: 9.1b1
+Version: 9.2
 Summary: Python<->ObjC Interoperability Module
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren, bbum, SteveM, LeleG, many others stretching back through the reaches of time...
 Author-email: RonaldOussoren@mac.com
 Maintainer: Ronald Oussoren
 Maintainer-email: RonaldOussoren@mac.com
 License: MIT License
```

### Comparing `pyobjc-core-9.1b1/Lib/pyobjc_core.egg-info/SOURCES.txt` & `pyobjc-core-9.2/Lib/pyobjc_core.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 HISTORIC.txt
 Install.txt
 License.txt
 MANIFEST
 MANIFEST.in
 README.txt
 diff.txt
+pyproject.toml
 setup.cfg
 setup.py
 Examples/00ReadMe.txt
 Examples/GUITests/00ReadMe.txt
 Examples/GUITests/test_modalsession.py
 Examples/NonFunctional/RemotePyInterpreter/AsyncPythonInterpreter.py
 Examples/NonFunctional/RemotePyInterpreter/ConsoleReactor.py
@@ -212,14 +213,82 @@
 Modules/objc/weakref.h
 Modules/objc/weakref.m
 Modules/objc/test/NULL.m
 Modules/objc/test/arrayint.m
 Modules/objc/test/arrays.m
 Modules/objc/test/block.m
 Modules/objc/test/bufsizeinarg.m
+Modules/objc/test/categories_base.m
+Modules/objc/test/category_c42.m
+Modules/objc/test/category_c43.m
+Modules/objc/test/category_c44.m
+Modules/objc/test/category_c45.m
+Modules/objc/test/category_c46.m
+Modules/objc/test/category_c47.m
+Modules/objc/test/category_c48.m
+Modules/objc/test/category_c49.m
+Modules/objc/test/category_c50.m
+Modules/objc/test/category_c51.m
+Modules/objc/test/category_c52.m
+Modules/objc/test/category_c53.m
+Modules/objc/test/category_c54.m
+Modules/objc/test/category_c55.m
+Modules/objc/test/category_c56.m
+Modules/objc/test/category_c57.m
+Modules/objc/test/category_c58.m
+Modules/objc/test/category_c59.m
+Modules/objc/test/category_gp10.m
+Modules/objc/test/category_gp11.m
+Modules/objc/test/category_gp12.m
+Modules/objc/test/category_gp13.m
+Modules/objc/test/category_gp14.m
+Modules/objc/test/category_gp15.m
+Modules/objc/test/category_gp16.m
+Modules/objc/test/category_gp17.m
+Modules/objc/test/category_gp18.m
+Modules/objc/test/category_gp19.m
+Modules/objc/test/category_gp20.m
+Modules/objc/test/category_gp21.m
+Modules/objc/test/category_gp22.m
+Modules/objc/test/category_gp23.m
+Modules/objc/test/category_gp24.m
+Modules/objc/test/category_gp27.m
+Modules/objc/test/category_gp3.m
+Modules/objc/test/category_gp30.m
+Modules/objc/test/category_gp33.m
+Modules/objc/test/category_gp36.m
+Modules/objc/test/category_gp39.m
+Modules/objc/test/category_gp42.m
+Modules/objc/test/category_gp45.m
+Modules/objc/test/category_gp48.m
+Modules/objc/test/category_gp51.m
+Modules/objc/test/category_gp54.m
+Modules/objc/test/category_gp57.m
+Modules/objc/test/category_gp6.m
+Modules/objc/test/category_gp7.m
+Modules/objc/test/category_gp8.m
+Modules/objc/test/category_gp9.m
+Modules/objc/test/category_p24.m
+Modules/objc/test/category_p25.m
+Modules/objc/test/category_p26.m
+Modules/objc/test/category_p27.m
+Modules/objc/test/category_p28.m
+Modules/objc/test/category_p29.m
+Modules/objc/test/category_p30.m
+Modules/objc/test/category_p31.m
+Modules/objc/test/category_p32.m
+Modules/objc/test/category_p33.m
+Modules/objc/test/category_p34.m
+Modules/objc/test/category_p35.m
+Modules/objc/test/category_p36.m
+Modules/objc/test/category_p37.m
+Modules/objc/test/category_p38.m
+Modules/objc/test/category_p39.m
+Modules/objc/test/category_p40.m
+Modules/objc/test/category_p41.m
 Modules/objc/test/cfsocket.m
 Modules/objc/test/classes.m
 Modules/objc/test/clinmeth.m
 Modules/objc/test/coding.m
 Modules/objc/test/copying.m
 Modules/objc/test/corefoundation.m
 Modules/objc/test/dataint.m
@@ -295,14 +364,15 @@
 PyObjCTest/test_bridges.py
 PyObjCTest/test_bridgesupport.py
 PyObjCTest/test_bufsizeinarg.py
 PyObjCTest/test_bundleFunctions.py
 PyObjCTest/test_bundleVariables.py
 PyObjCTest/test_callable_docstr.py
 PyObjCTest/test_callbacks.py
+PyObjCTest/test_categories.py
 PyObjCTest/test_classandinst.py
 PyObjCTest/test_classhooks.py
 PyObjCTest/test_clinmeth.py
 PyObjCTest/test_compat.py
 PyObjCTest/test_constants.py
 PyObjCTest/test_context.py
 PyObjCTest/test_convenience.py
@@ -419,14 +489,15 @@
 PyObjCTest/data_bridgesupport/bundle_data/Test.bridgesupport
 PyObjCTest/data_bridgesupport/with_data/Test.bridgesupport
 PyObjCTest/data_bridgesupport/with_data_dylib/Test.bridgesupport
 PyObjCTest/data_bridgesupport/with_data_dylib/Test.dylib
 Tools/MANIFEST.in
 Tools/comparebench.py
 Tools/gen_archive.py
+Tools/generate-category-tests.py
 Tools/generate-helpers-vector.py
 Tools/pyobjc_setup.py
 Tools/pyobjcbench.py
 Tools/runtests-with-nuitka.py
 Tools/runtests.py
 Tools/results/pyobjcbench-7.3.txt
 Tools/results/pyobjcbench-8.0b1.txt
```

### Comparing `pyobjc-core-9.1b1/Lib/pyobjc_core.egg-info/include/pyobjc-api.h` & `pyobjc-core-9.2/Lib/pyobjc_core.egg-info/include/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Lib/pyobjc_core.egg-info/include/pyobjc-compat.h` & `pyobjc-core-9.2/Lib/pyobjc_core.egg-info/include/pyobjc-compat.h`

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

### Comparing `pyobjc-core-9.1b1/License.txt` & `pyobjc-core-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/MANIFEST` & `pyobjc-core-9.2/MANIFEST`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Misc/announcement.txt` & `pyobjc-core-9.2/Misc/announcement.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/_machsignals.m` & `pyobjc-core-9.2/Modules/_machsignals.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/OC_BuiltinPythonNumber.m` & `pyobjc-core-9.2/Modules/objc/OC_BuiltinPythonNumber.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/OC_NSBundleHack.h` & `pyobjc-core-9.2/Modules/objc/OC_NSBundleHack.h`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/OC_NSBundleHack.m` & `pyobjc-core-9.2/Modules/objc/OC_NSBundleHack.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/OC_PythonArray.h` & `pyobjc-core-9.2/Modules/objc/OC_PythonArray.h`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/OC_PythonArray.m` & `pyobjc-core-9.2/Modules/objc/OC_PythonArray.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/OC_PythonData.h` & `pyobjc-core-9.2/Modules/objc/OC_PythonData.h`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/OC_PythonData.m` & `pyobjc-core-9.2/Modules/objc/OC_PythonData.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/OC_PythonDate.m` & `pyobjc-core-9.2/Modules/objc/OC_PythonDate.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/OC_PythonDictionary.h` & `pyobjc-core-9.2/Modules/objc/OC_PythonDictionary.h`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/OC_PythonDictionary.m` & `pyobjc-core-9.2/Modules/objc/OC_PythonDictionary.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/OC_PythonEnumerator.m` & `pyobjc-core-9.2/Modules/objc/OC_PythonEnumerator.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/OC_PythonNumber.m` & `pyobjc-core-9.2/Modules/objc/OC_PythonNumber.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/OC_PythonObject.h` & `pyobjc-core-9.2/Modules/objc/OC_PythonObject.h`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/OC_PythonObject.m` & `pyobjc-core-9.2/Modules/objc/OC_PythonObject.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/OC_PythonSet.m` & `pyobjc-core-9.2/Modules/objc/OC_PythonSet.m`

 * *Files 2% similar despite different names*

```diff
@@ -17,19 +17,18 @@
 
     SET_FIELD_INCREF(value, v);
     return self;
 }
 
 - (PyObject*)__pyobjc_PythonObject__
 {
-    /* XXX: This assertion is needed for correctness, without
-     * it
-     * ``PyObjCTest.test_archive_python.TestArchivePlainPython.test_recursive_frozenset_subclass_and_inst``
-     * causes a segmentation fault.
-     */
+    if (value == NULL) {
+        PyErr_SetString(PyObjCExc_Error, "OC_PythonSet without a value");
+        return NULL;
+    }
     PyObjC_Assert(value != NULL, ((PyObject* _Nonnull)NULL));
     Py_INCREF(value);
     return value;
 }
 
 - (PyObject*)__pyobjc_PythonTransient__:(int*)cookie
 {
@@ -100,15 +99,15 @@
     return [OC_PythonSet class];
 }
 
 - (void)encodeWithCoder:(NSCoder*)coder
 {
     int code;
     if (PyAnySet_CheckExact(value)) {
-        if (PyFrozenSet_Check(value)) {
+        if (PyFrozenSet_CheckExact(value)) {
             code = 1;
         } else {
             code = 2;
         }
 
         if ([coder allowsKeyedCoding]) {
             [coder encodeInt32:code forKey:@"pytype"];
```

### Comparing `pyobjc-core-9.1b1/Modules/objc/OC_PythonUnicode.h` & `pyobjc-core-9.2/Modules/objc/OC_PythonUnicode.h`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/OC_PythonUnicode.m` & `pyobjc-core-9.2/Modules/objc/OC_PythonUnicode.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/ObjCPointer.h` & `pyobjc-core-9.2/Modules/objc/ObjCPointer.h`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/ObjCPointer.m` & `pyobjc-core-9.2/Modules/objc/ObjCPointer.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/block_support.h` & `pyobjc-core-9.2/Modules/objc/block_support.h`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/block_support.m` & `pyobjc-core-9.2/Modules/objc/block_support.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/bundle-variables.h` & `pyobjc-core-9.2/Modules/objc/bundle-variables.h`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/bundle-variables.m` & `pyobjc-core-9.2/Modules/objc/bundle-variables.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/class-builder.m` & `pyobjc-core-9.2/Modules/objc/class-builder.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/class-list.h` & `pyobjc-core-9.2/Modules/objc/class-list.h`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/class-list.m` & `pyobjc-core-9.2/Modules/objc/class-list.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/closure_pool.h` & `pyobjc-core-9.2/Modules/objc/closure_pool.h`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/closure_pool.m` & `pyobjc-core-9.2/Modules/objc/closure_pool.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/corefoundation.h` & `pyobjc-core-9.2/Modules/objc/corefoundation.h`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/corefoundation.m` & `pyobjc-core-9.2/Modules/objc/corefoundation.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/ctests.m` & `pyobjc-core-9.2/Modules/objc/ctests.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/file_wrapper.m` & `pyobjc-core-9.2/Modules/objc/file_wrapper.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/formal-protocol.h` & `pyobjc-core-9.2/Modules/objc/formal-protocol.h`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/formal-protocol.m` & `pyobjc-core-9.2/Modules/objc/formal-protocol.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/fsref.h` & `pyobjc-core-9.2/Modules/objc/fsref.h`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/fsref.m` & `pyobjc-core-9.2/Modules/objc/fsref.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/function.h` & `pyobjc-core-9.2/Modules/objc/function.h`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/function.m` & `pyobjc-core-9.2/Modules/objc/function.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/helpers-authorization.m` & `pyobjc-core-9.2/Modules/objc/helpers-authorization.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/helpers-foundation-nscoder.m` & `pyobjc-core-9.2/Modules/objc/helpers-foundation-nscoder.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/helpers-foundation-nsdata.m` & `pyobjc-core-9.2/Modules/objc/helpers-foundation-nsdata.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/helpers-foundation-nsdecimal.m` & `pyobjc-core-9.2/Modules/objc/helpers-foundation-nsdecimal.m`

 * *Files 1% similar despite different names*

```diff
@@ -258,16 +258,23 @@
          * PyObject_Repr(), but that might give an incorrect
          * value for float subclasses with an overridden __repr__,
          * which includes for example a float enum:
          *
          *     class FloatEnum(float, enum.Enum): ...
          */
         NSString* stringVal;
-        stringVal = [[NSString alloc]
-            initWithFormat:@"%.*g", DBL_DECIMAL_DIG, PyFloat_AsDouble(pyValue)];
+        stringVal = [[NSString alloc] initWithFormat:@"%.*g",
+#ifdef DBL_DECIMAL_DIG
+                                                     DBL_DECIMAL_DIG,
+#else
+                                                     /* With Xcode 7.3 (macOS 10.11) the
+                                                        public macro is not available */
+                                                     __DBL_DECIMAL_DIG__,
+#endif
+                                                     PyFloat_AsDouble(pyValue)];
         if (stringVal == nil) {
             PyErr_SetString(PyObjCExc_Error, "Converting double to NSString failed");
             return -1;
         }
 
         @try {
             DecimalFromString(outResult, stringVal, NULL);
@@ -1052,15 +1059,19 @@
       Py_DECREF(result);
       PyGILState_Release(state);
       return *res;
 
   error:
       Py_XDECREF(v);
       PyObjCErr_ToObjCWithGILState(&state);
+#pragma clang diagnostic push
+#pragma clang diagnostic ignored "-Wunreachable-code"
+
       __builtin_unreachable(); // LCOV_EXCL_LINE
+#pragma clang diagnostic pop
     };
     return imp_implementationWithBlock(block);
 }
 
 int
 PyObjC_setup_nsdecimal(PyObject* m)
 {
```

### Comparing `pyobjc-core-9.1b1/Modules/objc/helpers-foundation-nsinvocation.m` & `pyobjc-core-9.2/Modules/objc/helpers-foundation-nsinvocation.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/helpers-foundation-nsobject.m` & `pyobjc-core-9.2/Modules/objc/helpers-foundation-nsobject.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/helpers-vector.m` & `pyobjc-core-9.2/Modules/objc/helpers-vector.m`

 * *Files 0% similar despite different names*

```diff
@@ -4,17 +4,34 @@
  *     ** DO NOT EDIT **
  */
 // LCOV_EXCL_START
 #import "pyobjc.h"
 #include <simd/simd.h>
 
 #import <GameplayKit/GameplayKit.h>
-#import <MetalPerformanceShaders/MetalPerformanceShaders.h>
 #import <ModelIO/ModelIO.h>
 
+#if PyObjC_BUILD_RELEASE >= 1013
+#import <MetalPerformanceShaders/MetalPerformanceShaders.h>
+#endif
+
+#if PyObjC_BULD_RELEASE < 1013
+#define simd_uchar16 vector_uchar16
+#define simd_float2 vector_float2
+#define simd_float3 vector_float3
+#define simd_float4 vector_float4
+#define simd_double2 vector_double2
+#define simd_double3 vector_double3
+#define simd_double4 vector_double4
+#define simd_uint2 vector_uint2
+#define simd_uint3 vector_uint3
+#define simd_int2 vector_int2
+#define simd_int4 vector_int4
+#endif /*  PyObjC_BULD_RELEASE < 1013 */
+
 NS_ASSUME_NONNULL_BEGIN
 
 static inline int
 extract_method_info(PyObject* method, PyObject* self, bool* isIMP, id* self_obj,
                     Class* super_class, int* flags, PyObjCMethodSignature** methinfo)
 {
     *isIMP = !!PyObjCIMP_Check(method);
@@ -6111,14 +6128,15 @@
           }
           PyObjCErr_ToObjCWithGILState(&state);
         };
 
     return imp_implementationWithBlock(block);
 }
 
+#if PyObjC_BUILD_RELEASE >= 1012
 static PyObject* _Nullable call_id_id_GKBox(PyObject* method, PyObject* self,
                                             PyObject* const* arguments, size_t nargs)
 {
     struct objc_super super;
     id                rv;
     id                arg0;
     GKBox             arg1;
@@ -6334,14 +6352,15 @@
           Py_CLEAR(args[i]);
       }
       PyObjCErr_ToObjCWithGILState(&state);
     };
 
     return imp_implementationWithBlock(block);
 }
+#endif /*  PyObjC_BUILD_RELEASE >= 1012 */
 
 static PyObject* _Nullable call_id_id_MDLAxisAlignedBoundingBox_f(
     PyObject* method, PyObject* self, PyObject* const* arguments, size_t nargs)
 {
     struct objc_super         super;
     id                        rv;
     id                        arg0;
@@ -8064,14 +8083,15 @@
           }
           PyObjCErr_ToObjCWithGILState(&state);
         };
 
     return imp_implementationWithBlock(block);
 }
 
+#if PyObjC_BUILD_RELEASE >= 1012
 static PyObject* _Nullable call_id_GKBox(PyObject* method, PyObject* self,
                                          PyObject* const* arguments, size_t nargs)
 {
     struct objc_super super;
     id                rv;
     GKBox             arg0;
 
@@ -8497,14 +8517,15 @@
           Py_CLEAR(args[i]);
       }
       PyObjCErr_ToObjCWithGILState(&state);
     };
 
     return imp_implementationWithBlock(block);
 }
+#endif /*  PyObjC_BUILD_RELEASE >= 1012 */
 
 static PyObject* _Nullable call_id_MDLVoxelIndexExtent(PyObject* method, PyObject* self,
                                                        PyObject* const* arguments,
                                                        size_t           nargs)
 {
     struct objc_super   super;
     id                  rv;
@@ -12345,14 +12366,15 @@
           }
           PyObjCErr_ToObjCWithGILState(&state);
         };
 
     return imp_implementationWithBlock(block);
 }
 
+#if PyObjC_BUILD_RELEASE >= 1013
 static PyObject* _Nullable call_v_simd_float4x4(PyObject* method, PyObject* self,
                                                 PyObject* const* arguments, size_t nargs)
 {
     struct objc_super super;
     simd_float4x4     arg0;
 
     if (PyObjC_CheckArgCount(method, 1, 1, nargs) == -1)
@@ -12891,15 +12913,17 @@
               Py_CLEAR(args[i]);
           }
           PyObjCErr_ToObjCWithGILState(&state);
         };
 
     return imp_implementationWithBlock(block);
 }
+#endif /* PyObjC_BUILD_RELEASE >= 1013 */
 
+#if PyObjC_BUILD_RELEASE >= 1012
 static PyObject* _Nullable call_GKBox(PyObject* method, PyObject* self,
                                       PyObject* const* arguments
                                       __attribute__((__unused__)),
                                       size_t nargs)
 {
     struct objc_super super;
     GKBox             rv;
@@ -13205,14 +13229,15 @@
               Py_CLEAR(args[i]);
           }
           PyObjCErr_ToObjCWithGILState(&state);
         };
 
     return imp_implementationWithBlock(block);
 }
+#endif /* PyObjC_BUILD_RELEASE >= 1012 */
 
 static PyObject* _Nullable call_MDLAxisAlignedBoundingBox(PyObject*        method,
                                                           PyObject*        self,
                                                           PyObject* const* arguments
                                                           __attribute__((__unused__)),
                                                           size_t nargs)
 {
@@ -13647,14 +13672,15 @@
       }
       PyObjCErr_ToObjCWithGILState(&state);
     };
 
     return imp_implementationWithBlock(block);
 }
 
+#if PyObjC_BUILD_RELEASE >= 1013
 static PyObject* _Nullable call_MPSAxisAlignedBoundingBox(PyObject*        method,
                                                           PyObject*        self,
                                                           PyObject* const* arguments
                                                           __attribute__((__unused__)),
                                                           size_t nargs)
 {
     struct objc_super         super;
@@ -13859,14 +13885,15 @@
           Py_CLEAR(args[i]);
       }
       PyObjCErr_ToObjCWithGILState(&state);
     };
 
     return imp_implementationWithBlock(block);
 }
+#endif /* PyObjC_BUILD_RELEASE >= 1013 */
 
 static PyObject* _Nullable call_matrix_double4x4(PyObject* method, PyObject* self,
                                                  PyObject* const* arguments
                                                  __attribute__((__unused__)),
                                                  size_t nargs)
 {
     struct objc_super super;
@@ -14616,14 +14643,15 @@
       }
       PyObjCErr_ToObjCWithGILState(&state);
     };
 
     return imp_implementationWithBlock(block);
 }
 
+#if PyObjC_BUILD_RELEASE >= 1013
 static PyObject* _Nullable call_simd_float4x4(PyObject* method, PyObject* self,
                                               PyObject* const* arguments
                                               __attribute__((__unused__)),
                                               size_t nargs)
 {
     struct objc_super super;
     simd_float4x4     rv;
@@ -15153,14 +15181,16 @@
           Py_CLEAR(args[i]);
       }
       PyObjCErr_ToObjCWithGILState(&state);
     };
 
     return imp_implementationWithBlock(block);
 }
+#endif /* PyObjC_BUILD_RELEASE > 1013 */
+
 int
 PyObjC_setup_simd(PyObject* module __attribute__((__unused__)))
 {
 
     if (PyObjC_RegisterSignatureMapping( // LCOV_BR_EXCL_LINE
             "<16C>@:", call_v16C, mkimp_v16C)
         == -1) {
@@ -15530,25 +15560,27 @@
 
     if (PyObjC_RegisterSignatureMapping( // LCOV_BR_EXCL_LINE
             "@@:@q<2i>fffff", call_id_id_q_v2i_f_f_f_f_f, mkimp_id_id_q_v2i_f_f_f_f_f)
         == -1) {
         return -1; // LCOV_EXCL_LINE
     }
 
+#if PyObjC_BUILD_RELEASE >= 1012
     if (PyObjC_RegisterSignatureMapping( // LCOV_BR_EXCL_LINE
             "@@:@{GKBox=<3f><3f>}", call_id_id_GKBox, mkimp_id_id_GKBox)
         == -1) {
         return -1; // LCOV_EXCL_LINE
     }
 
     if (PyObjC_RegisterSignatureMapping( // LCOV_BR_EXCL_LINE
             "@@:@{GKQuad=<2f><2f>}", call_id_id_GKQuad, mkimp_id_id_GKQuad)
         == -1) {
         return -1; // LCOV_EXCL_LINE
     }
+#endif /* PyObjC_BUILD_RELEASE >= 1012 */
 
     if (PyObjC_RegisterSignatureMapping( // LCOV_BR_EXCL_LINE
             "@@:@{_MDLAxisAlignedBoundingBox=<3f><3f>}f",
             call_id_id_MDLAxisAlignedBoundingBox_f,
             mkimp_id_id_MDLAxisAlignedBoundingBox_f)
         == -1) {
         return -1; // LCOV_EXCL_LINE
@@ -15645,14 +15677,15 @@
 
     if (PyObjC_RegisterSignatureMapping( // LCOV_BR_EXCL_LINE
             "@@:ff@<2i>", call_id_f_f_id_v2i, mkimp_id_f_f_id_v2i)
         == -1) {
         return -1; // LCOV_EXCL_LINE
     }
 
+#if PyObjC_BUILD_RELEASE >= 1012
     if (PyObjC_RegisterSignatureMapping( // LCOV_BR_EXCL_LINE
             "@@:{GKBox=<3f><3f>}", call_id_GKBox, mkimp_id_GKBox)
         == -1) {
         return -1; // LCOV_EXCL_LINE
     }
 
     if (PyObjC_RegisterSignatureMapping( // LCOV_BR_EXCL_LINE
@@ -15668,14 +15701,15 @@
     }
 
     if (PyObjC_RegisterSignatureMapping( // LCOV_BR_EXCL_LINE
             "@@:{GKQuad=<2f><2f>}f", call_id_GKQuad_f, mkimp_id_GKQuad_f)
         == -1) {
         return -1; // LCOV_EXCL_LINE
     }
+#endif /* PyObjC_BUILD_RELEASE >= 1012 */
 
     if (PyObjC_RegisterSignatureMapping( // LCOV_BR_EXCL_LINE
             "@@:{_MDLVoxelIndexExtent=<4i><4i>}", call_id_MDLVoxelIndexExtent,
             mkimp_id_MDLVoxelIndexExtent)
         == -1) {
         return -1; // LCOV_EXCL_LINE
     }
@@ -15917,14 +15951,15 @@
     if (PyObjC_RegisterSignatureMapping( // LCOV_BR_EXCL_LINE
             "v@:{_matrix_float4x4=[4<4f>]}d", call_v_matrix_float4x4_d,
             mkimp_v_matrix_float4x4_d)
         == -1) {
         return -1; // LCOV_EXCL_LINE
     }
 
+#if PyObjC_BUILD_RELEASE >= 1013
     if (PyObjC_RegisterSignatureMapping( // LCOV_BR_EXCL_LINE
             "v@:{_simd_float4x4=[4<4f>]}", call_v_simd_float4x4, mkimp_v_simd_float4x4)
         == -1) {
         return -1; // LCOV_EXCL_LINE
     }
 
     if (PyObjC_RegisterSignatureMapping( // LCOV_BR_EXCL_LINE
@@ -15946,15 +15981,17 @@
     }
 
     if (PyObjC_RegisterSignatureMapping( // LCOV_BR_EXCL_LINE
             "v@:{_simd_quatf=<4f>}d", call_v_simd_quatf_d, mkimp_v_simd_quatf_d)
         == -1) {
         return -1; // LCOV_EXCL_LINE
     }
+#endif /*  PyObjC_BUILD_RELEASE >= 1013 */
 
+#if PyObjC_BUILD_RELEASE >= 1012
     if (PyObjC_RegisterSignatureMapping( // LCOV_BR_EXCL_LINE
             "{GKBox=<3f><3f>}@:", call_GKBox, mkimp_GKBox)
         == -1) {
         return -1; // LCOV_EXCL_LINE
     }
 
     if (PyObjC_RegisterSignatureMapping( // LCOV_BR_EXCL_LINE
@@ -15964,14 +16001,15 @@
     }
 
     if (PyObjC_RegisterSignatureMapping( // LCOV_BR_EXCL_LINE
             "{GKTriangle=[3<3f>]}@:Q", call_GKTriangle_Q, mkimp_GKTriangle_Q)
         == -1) {
         return -1; // LCOV_EXCL_LINE
     }
+#endif /*  PyObjC_BUILD_RELEASE >= 1012 */
 
     if (PyObjC_RegisterSignatureMapping( // LCOV_BR_EXCL_LINE
             "{_MDLAxisAlignedBoundingBox=<3f><3f>}@:", call_MDLAxisAlignedBoundingBox,
             mkimp_MDLAxisAlignedBoundingBox)
         == -1) {
         return -1; // LCOV_EXCL_LINE
     }
@@ -15993,14 +16031,15 @@
     if (PyObjC_RegisterSignatureMapping( // LCOV_BR_EXCL_LINE
             "{_MDLVoxelIndexExtent=<4i><4i>}@:", call_MDLVoxelIndexExtent,
             mkimp_MDLVoxelIndexExtent)
         == -1) {
         return -1; // LCOV_EXCL_LINE
     }
 
+#if PyObjC_BUILD_RELEASE >= 1013
     if (PyObjC_RegisterSignatureMapping( // LCOV_BR_EXCL_LINE
             "{_MPSAxisAlignedBoundingBox=<3f><3f>}@:", call_MPSAxisAlignedBoundingBox,
             mkimp_MPSAxisAlignedBoundingBox)
         == -1) {
         return -1; // LCOV_EXCL_LINE
     }
 
@@ -16013,14 +16052,15 @@
 
     if (PyObjC_RegisterSignatureMapping( // LCOV_BR_EXCL_LINE
             "{_MPSImageHistogramInfo=QB<4f><4f>}@:", call_MPSImageHistogramInfo,
             mkimp_MPSImageHistogramInfo)
         == -1) {
         return -1; // LCOV_EXCL_LINE
     }
+#endif /* PyObjC_BUILD_RELEASE >= 1013 */
 
     if (PyObjC_RegisterSignatureMapping( // LCOV_BR_EXCL_LINE
             "{_matrix_double4x4=[4<4d>]}@:", call_matrix_double4x4,
             mkimp_matrix_double4x4)
         == -1) {
         return -1; // LCOV_EXCL_LINE
     }
@@ -16060,14 +16100,15 @@
     if (PyObjC_RegisterSignatureMapping( // LCOV_BR_EXCL_LINE
             "{_matrix_float4x4=[4<4f>]}@:d", call_matrix_float4x4_d,
             mkimp_matrix_float4x4_d)
         == -1) {
         return -1; // LCOV_EXCL_LINE
     }
 
+#if PyObjC_BUILD_RELEASE >= 1013
     if (PyObjC_RegisterSignatureMapping( // LCOV_BR_EXCL_LINE
             "{_simd_float4x4=[4<4f>]}@:", call_simd_float4x4, mkimp_simd_float4x4)
         == -1) {
         return -1; // LCOV_EXCL_LINE
     }
 
     if (PyObjC_RegisterSignatureMapping( // LCOV_BR_EXCL_LINE
@@ -16090,12 +16131,13 @@
     }
 
     if (PyObjC_RegisterSignatureMapping( // LCOV_BR_EXCL_LINE
             "{_simd_quatf=<4f>}@:d", call_simd_quatf_d, mkimp_simd_quatf_d)
         == -1) {
         return -1; // LCOV_EXCL_LINE
     }
+#endif /* PyObjC_BUILD_RELEASE >= 1013 */
 
     return 0;
 }
 NS_ASSUME_NONNULL_END
 // LCOV_EXCL_STOP
```

### Comparing `pyobjc-core-9.1b1/Modules/objc/helpers.h` & `pyobjc-core-9.2/Modules/objc/helpers.h`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/instance-var.h` & `pyobjc-core-9.2/Modules/objc/instance-var.h`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/instance-var.m` & `pyobjc-core-9.2/Modules/objc/instance-var.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/ivar-accessor.h` & `pyobjc-core-9.2/Modules/objc/ivar-accessor.h`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/ivar-accessor.m` & `pyobjc-core-9.2/Modules/objc/ivar-accessor.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/libffi_extra.m` & `pyobjc-core-9.2/Modules/objc/libffi_extra.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/libffi_support.h` & `pyobjc-core-9.2/Modules/objc/libffi_support.h`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/libffi_support.m` & `pyobjc-core-9.2/Modules/objc/libffi_support.m`

 * *Files 2% similar despite different names*

```diff
@@ -1281,14 +1281,20 @@
                             methinfo->argtype[i]->alreadyRetained,
                             methinfo->argtype[i]->alreadyCFRetained);
                         break;
 
                     case PyObjC_kVariableLengthArray:
                         v = PyObjCVarList_New(resttype, *(void**)args[i]);
                         break;
+
+                    case PyObjC_kDerefResultPointer:
+                        PyErr_SetString(PyObjCExc_Error,
+                                        "using 'deref_result_pointer' for an argument");
+                        v = NULL;
+                        break;
                     }
                 }
 
             } else {
                 if (argtype[1] == _C_ARY_B) {
                     v = pythonify_c_value(argtype + 1, *(void**)(args[i]));
 
@@ -1352,14 +1358,19 @@
                     count = methinfo->argtype[i]->arrayArg;
                     v     = PyBytes_FromStringAndSize(args[i], count);
                     break;
 
                 case PyObjC_kVariableLengthArray:
                     v = PyObjCVarList_New(gCharEncoding, args[i]);
                     break;
+                case PyObjC_kDerefResultPointer:
+                    PyErr_SetString(PyObjCExc_Error,
+                                    "using 'deref_result_pointer' for an argument");
+                    v = NULL;
+                    break;
                 }
             }
             break;
 
         case _C_ARY_B:
             /* An array is actually a pointer to the first
              * element of the array. Libffi passes a pointer to
@@ -1495,14 +1506,20 @@
                         err = depythonify_c_return_array_count(
                             rest, count, res, resp, methinfo->rettype->alreadyRetained,
                             methinfo->rettype->alreadyCFRetained);
                         if (err == -1) {
                             Py_DECREF(res);
                             goto error;
                         }
+                        break;
+                    case PyObjC_kDerefResultPointer:
+                        PyErr_SetString(PyObjCExc_Error,
+                                        "using 'deref_result_pointer' for python "
+                                        "callable is not supported");
+                        goto error;
                     }
                 }
 
             } else {
                 err = depythonify_c_return_value(rettype, res, resp);
 
                 if (methinfo->rettype->alreadyRetained) {
@@ -1669,14 +1686,18 @@
                         argtype, -1, YES, res, *(void**)args[i],
                         methinfo->argtype[i]->alreadyRetained,
                         methinfo->argtype[i]->alreadyCFRetained);
                     if (err == -1) {
                         goto error;
                     }
                     break;
+                case PyObjC_kDerefResultPointer:
+                    PyErr_SetString(PyObjCExc_Error,
+                                    "using 'deref_result_pointer' for argument value");
+                    goto error;
                 }
 
                 break;
             }
 
             PyGILState_Release(state);
             return;
@@ -1772,14 +1793,19 @@
                                 goto error;
                             }
                         } else {
                             /* Wait until after the arguments have been depythonified */
                             *(void**)resp = NULL;
                             break;
                         }
+                    case PyObjC_kDerefResultPointer:
+                        PyErr_SetString(PyObjCExc_Error,
+                                        "'deref_result_pointer' for a callable "
+                                        "implemented in python is not supported ");
+                        goto error;
                     }
                 }
 
             } else {
                 err = depythonify_c_return_value(rettype, real_res, resp);
 
                 if (methinfo->rettype->alreadyRetained) {
@@ -1932,14 +1958,18 @@
                     argtype, count, YES, PyTuple_GET_ITEM(res, idx++), *(void**)args[i],
                     methinfo->argtype[i]->alreadyRetained,
                     methinfo->argtype[i]->alreadyCFRetained);
                 if (err == -1) {
                     goto error;
                 }
                 break;
+            case PyObjC_kDerefResultPointer:
+                PyErr_SetString(PyObjCExc_Error,
+                                "'deref_result_pointer' for an argument value");
+                goto error;
             }
         }
 
         if (unlikely(haveCountArg)) {
             if (real_res == NULL) {
                 idx = 0;
             } else {
@@ -1987,14 +2017,18 @@
                         argtype, count, NO, PyTuple_GET_ITEM(res, idx++),
                         *(void**)args[i], methinfo->argtype[i]->alreadyRetained,
                         methinfo->argtype[i]->alreadyCFRetained);
                     if (err == -1) {
                         goto error;
                     }
                     break;
+                case PyObjC_kDerefResultPointer:
+                    PyErr_SetString(PyObjCExc_Error,
+                                    "'deref_result_pointer' for an argument value");
+                    goto error;
                 }
             }
         }
 
         if (*rettype != _C_VOID) {
             const char* unqualified = PyObjCRT_SkipTypeQualifiers(rettype);
             if (unqualified[0] == _C_PTR || unqualified[0] == _C_CHARPTR) {
@@ -2870,14 +2904,18 @@
                 arglist[i] = &ffi_type_pointer;
                 values[i]  = byref + i;
                 break;
 
             case PyObjC_kArrayCountInArg:
                 have_counted_array = YES;
                 break;
+            case PyObjC_kDerefResultPointer:
+                PyErr_SetString(PyObjCExc_Error,
+                                "'deref_result_pointer' for an argument value");
+                return -1;
             }
 
         } else {
             /* Encode argument, maybe after allocating space */
 
             if (argtype[0] == _C_OUT)
                 argtype++;
@@ -3440,14 +3478,19 @@
                                 if (byref_attr[i].token == -1) {
                                     return -1;
                                 }
 
                                 arglist[i] = &ffi_type_pointer;
                                 values[i]  = byref + i;
                                 break;
+                            case PyObjC_kDerefResultPointer:
+                                PyErr_SetString(
+                                    PyObjCExc_Error,
+                                    "'deref_result_pointer' for an argument value");
+                                return -1;
                             }
                         }
                     }
                     break;
 
                 case _C_CHARPTR:
                     if (argument != PyObjC_NULL) {
@@ -3470,14 +3513,19 @@
                                 NO, NO, gCharEncoding, argument, byref + i, &count,
                                 &byref_attr[i].obj, &byref_attr[i].view);
                             if (byref_attr[i].token == -1) {
                                 return -1;
                             }
                             arglist[i] = &ffi_type_pointer;
                             values[i]  = byref + i;
+                        case PyObjC_kDerefResultPointer:
+                            PyErr_SetString(
+                                PyObjCExc_Error,
+                                "'deref_result_pointer' for an argument value");
+                            return -1;
                         }
                     }
                 }
             }
         }
     }
 
@@ -3712,14 +3760,27 @@
 
                         if (objc_result == NULL) {
                             return NULL;
                         }
                     }
                     break;
 
+                case PyObjC_kDerefResultPointer:
+                    if (*(void**)pRetval == NULL) {
+                        Py_INCREF(PyObjC_NULL);
+                        objc_result = PyObjC_NULL;
+                    } else {
+                        objc_result = pythonify_c_value(tp + 1, pRetval);
+                        if (objc_result == NULL) {
+                            return NULL;
+                        }
+                    }
+
+                    break;
+
                 default:
                     PyErr_Format(PyExc_SystemError, "Unhandled pointer type: %d",
                                  methinfo->rettype->ptrType);
                     return NULL;
                 }
 
                 if (methinfo->free_result) {
@@ -3988,14 +4049,19 @@
                                     methinfo->argtype[i]->alreadyRetained,
                                     methinfo->argtype[i]->alreadyCFRetained);
                             }
 
                             if (v == NULL)
                                 goto error_cleanup;
                             break;
+                        case PyObjC_kDerefResultPointer:
+                            PyErr_SetString(
+                                PyObjCExc_Error,
+                                "'deref_result_pointer' for an argument value");
+                            goto error_cleanup;
                         }
                     }
 
                     if (result != NULL) {
                         if (PyTuple_SetItem(result, py_arg++, v) < 0) {
 
                             Py_DECREF(v);
```

### Comparing `pyobjc-core-9.1b1/Modules/objc/memview.m` & `pyobjc-core-9.2/Modules/objc/memview.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/meth-func.h` & `pyobjc-core-9.2/Modules/objc/meth-func.h`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/meth-func.m` & `pyobjc-core-9.2/Modules/objc/meth-func.m`

 * *Files 3% similar despite different names*

```diff
@@ -53,14 +53,17 @@
             Py_DECREF(func);
         }
     }
     PyErr_Format(PyExc_TypeError, "%R is not a python function or method", value);
     return NULL;
 }
 
+/*
+ * XXX: This duplicates code in Lib/objc/_transform.py!
+ */
 bool
 PyObjC_returns_value(PyObject* value)
 {
     bool      rv = false;
     Py_buffer buf;
 
     if (!PyFunction_Check(value) && !PyMethod_Check(value)) {
@@ -133,14 +136,21 @@
         if (op == LOAD_CONST && ((unsigned char*)buf.buf)[i + 1] == 0) {
             was_none = true;
         } else {
             if (op == RETURN_VALUE && !was_none) {
                 rv = true;
                 break;
             }
+#if PY_VERSION_HEX >= 0x030c0000
+            else if (op == RETURN_CONST && ((unsigned char*)buf.buf)[i + 1] != 0) {
+                rv = true;
+                break;
+            }
+#endif /* PY_VERSION_HEX >= 0x030c0000 */
+
             was_none = false;
         }
     }
 
 #else  /* PY_VERSION_HEX < 0x03060000 */
     for (i = 0; i < buf.len; ++i) {
         int op = ((unsigned char*)buf.buf)[i];
```

### Comparing `pyobjc-core-9.1b1/Modules/objc/method-accessor.m` & `pyobjc-core-9.2/Modules/objc/method-accessor.m`

 * *Files 0% similar despite different names*

```diff
@@ -417,15 +417,15 @@
 
             len = PyTuple_GET_SIZE(mro);
             for (i = 0; i < len && result == NULL; i++) {
                 PyObject* c = PyTuple_GET_ITEM(mro, i);
                 if (!PyObjCClass_Check(c))
                     continue;
 
-                PyObject* dict = ((PyTypeObject*)c)->tp_dict;
+                PyObject* dict = PyObjC_get_tp_dict((PyTypeObject*)c);
                 PyObject* v    = PyDict_GetItemWithError(dict, name);
                 if (v == NULL && PyErr_Occurred()) { // LCOV_BR_EXCL_LINE
                     return NULL;                     // LCOV_EXCL_LINE
 
                 } else if (v != NULL) {
                     if (PyObjCSelector_Check(v)) {
                         /* Found it, use the
```

### Comparing `pyobjc-core-9.1b1/Modules/objc/method-imp.h` & `pyobjc-core-9.2/Modules/objc/method-imp.h`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/method-imp.m` & `pyobjc-core-9.2/Modules/objc/method-imp.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/method-signature.h` & `pyobjc-core-9.2/Modules/objc/method-signature.h`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 #endif /* __has_feature(objc_fixed_enum) */
 {
     PyObjC_kPointerPlain        = 0,
     PyObjC_kNullTerminatedArray = 1,
     PyObjC_kArrayCountInArg     = 2,
     PyObjC_kFixedLengthArray    = 3,
     PyObjC_kVariableLengthArray = 4,
+    PyObjC_kDerefResultPointer  = 5,
 };
 
 typedef struct _PyObjCMethodSignature PyObjCMethodSignature;
 
 struct _PyObjC_ArgDescr {
     /* If typeOverride the type field should be freed when the descriptor
      * is cleaned up, otherwise is isn't owned by this descriptor.
```

### Comparing `pyobjc-core-9.1b1/Modules/objc/method-signature.m` & `pyobjc-core-9.2/Modules/objc/method-signature.m`

 * *Files 1% similar despite different names*

```diff
@@ -880,14 +880,28 @@
             descr->ptrType  = PyObjC_kVariableLengthArray;
             descr->arrayArg = 0;
             descr->arrayArg = 0;
         }
     }
 
     if (meta) {
+        d = PyDict_GetItemStringWithError(meta, "deref_result_pointer");
+        if (d == NULL && PyErr_Occurred()) { // LCOV_BR_EXCL_LINE
+            return -1;                       // LCOV_EXCL_LINE
+        } else if (d != NULL && PyObject_IsTrue(d)) {
+            if (descr == NULL || descr->tmpl)
+                return -2;
+
+            descr->ptrType  = PyObjC_kDerefResultPointer;
+            descr->arrayArg = 0;
+            descr->arrayArg = 0;
+        }
+    }
+
+    if (meta) {
         d = PyDict_GetItemStringWithError(meta, "c_array_length_in_arg");
         if (d == NULL && PyErr_Occurred()) { // LCOV_BR_EXCL_LINE
             return -1;                       // LCOV_EXCL_LINE
         } else if (d != NULL) {
             if (PyLong_Check(d)) {
                 if (descr == NULL || descr->tmpl)
                     return -2;
@@ -1793,14 +1807,19 @@
         if (r == -1)    // LCOV_BR_EXCL_LINE
             goto error; // LCOV_EXCL_LINE
         break;
     case PyObjC_kVariableLengthArray:
         r = PyDict_SetItemString(result, "c_array_of_variable_length", Py_True);
         if (r == -1)    // LCOV_BR_EXCL_LINE
             goto error; // LCOV_EXCL_LINE
+
+    case PyObjC_kDerefResultPointer:
+        r = PyDict_SetItemString(result, "deref_result_pointer", Py_True);
+        if (r == -1)    // LCOV_BR_EXCL_LINE
+            goto error; // LCOV_EXCL_LINE
     }
 
     if (descr->ptrType != PyObjC_kPointerPlain && descr->arraySizeInRetval) {
         v = PyBool_FromLong(descr->arraySizeInRetval);
         if (v == NULL)  // LCOV_BR_EXCL_LINE
             goto error; // LCOV_EXCL_LINE
         r = PyDict_SetItemString(result, "c_array_length_in_result", v);
```

### Comparing `pyobjc-core-9.1b1/Modules/objc/module.m` & `pyobjc-core-9.2/Modules/objc/module.m`

 * *Files 0% similar despite different names*

```diff
@@ -1712,23 +1712,28 @@
     if (!PyUnicode_Check(object)) { // LCOV_BR_EXCL_LINE
         // LCOV_EXCL_START
         PyErr_SetString(PyExc_TypeError, "Expecting a string");
         return NULL;
         // LCOV_EXCL_STOP
     }
 
-    if (contains_func) {
-        const char* path = PyUnicode_AsUTF8(object);
-        if (path == NULL) {
-            return NULL;
-        }
+    /* Always fetch the C string to get consistent
+     * behaviour in error cases, even on systems
+     * without this system API.
+     */
+    const char* path = PyUnicode_AsUTF8(object);
+    if (path == NULL) {
+        return NULL;
+    }
 
+    if (contains_func) {
         int result = contains_func(path);
         return PyBool_FromLong(result);
     } else {
+
         Py_INCREF(Py_False);
         return Py_False;
     }
 }
 
 #endif
 
@@ -2154,14 +2159,16 @@
     {"MAC_OS_X_VERSION_12_4", MAC_OS_X_VERSION_12_4},
     {"MAC_OS_X_VERSION_12_5", MAC_OS_X_VERSION_12_5},
     {"MAC_OS_X_VERSION_12_6", MAC_OS_X_VERSION_12_6},
     {"MAC_OS_X_VERSION_13_0", MAC_OS_X_VERSION_13_0},
     {"MAC_OS_X_VERSION_13_1", MAC_OS_X_VERSION_13_1},
     {"MAC_OS_X_VERSION_13_2", MAC_OS_X_VERSION_13_2},
     {"MAC_OS_X_VERSION_13_3", MAC_OS_X_VERSION_13_3},
+    {"MAC_OS_X_VERSION_13_4", MAC_OS_X_VERSION_13_4},
+    {"MAC_OS_X_VERSION_13_5", MAC_OS_X_VERSION_13_5},
     {"PyObjC_BUILD_RELEASE", PyObjC_BUILD_RELEASE},
     {"_NSNotFound", NSNotFound},
     {"OBJC_ASSOCIATION_ASSIGN", OBJC_ASSOCIATION_ASSIGN},
     {"OBJC_ASSOCIATION_RETAIN_NONATOMIC", OBJC_ASSOCIATION_RETAIN_NONATOMIC},
     {"OBJC_ASSOCIATION_COPY_NONATOMIC", OBJC_ASSOCIATION_COPY_NONATOMIC},
     {"OBJC_ASSOCIATION_RETAIN", OBJC_ASSOCIATION_RETAIN},
     {"OBJC_ASSOCIATION_COPY", OBJC_ASSOCIATION_COPY},
@@ -2199,14 +2206,15 @@
  * - Encode dependencies somehow
  * - Script that extracts function names and dependencies,
  *   using topsort to generate this array.
  */
 static setup_function _Nullable setup_functions[] = {
     PyObjC_InitProxyRegistry, /* Must be first */
 
+    PyObjCUtil_Init,
     PyObjCPointerWrapper_Init,
     PyObjC_SetupOptions,
     PyObjC_setup_nsdecimal,
     PyObjCPointer_Setup,
     FILE_Setup,
     PyObjCFormalProtocol_Setup,
     PyObjCFunc_Setup,
@@ -2215,15 +2223,14 @@
     PyObjCMethodSignature_Setup,
     PyObjCUnicode_Setup,
     PyObjCInitNULL,
     PyObjCInstanceVariable_Setup,
     PyObjCMemView_Setup,
     PyObjCWeakRef_Setup,
     PyObjCMethodAccessor_Setup,
-    PyObjCUtil_Init,
     PyObjCIMP_SetUp,
     PyObjC_init_ctests,
     PyObjCSelector_Setup,
     PyObjC_setup_nsdata,
     PyObjC_setup_nscoder,
     PyObjC_setup_nsobject,
     PyObjC_setup_simd,
```

### Comparing `pyobjc-core-9.1b1/Modules/objc/objc-NULL.m` & `pyobjc-core-9.2/Modules/objc/objc-NULL.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/objc-class.h` & `pyobjc-core-9.2/Modules/objc/objc-class.h`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/objc-class.m` & `pyobjc-core-9.2/Modules/objc/objc-class.m`

 * *Files 0% similar despite different names*

```diff
@@ -842,15 +842,17 @@
             Py_DECREF(metadict);
             Py_DECREF(hiddenSelectors);
             Py_DECREF(hiddenClassSelectors);
             return NULL;
             // LCOV_EXCL_STOP
         }
 
-        if (PyDict_Update(metatype->tp_dict, metadict) == -1) { // LCOV_BR_EXCL_LINE
+        if (PyDict_Update( // LCOV_BR_EXCL_LINE
+                PyObjC_get_tp_dict(metatype), metadict)
+            == -1) {
             // LCOV_EXCL_START
             Py_XDECREF(orig_slots);
             Py_DECREF(old_dict);
             Py_DECREF(protocols);
             Py_DECREF(real_bases);
             Py_DECREF(metadict);
             Py_DECREF(hiddenSelectors);
@@ -1113,15 +1115,15 @@
     PyObject*    result;
     Class        cls;
     Method*      methods;
     unsigned int method_count, i;
     char         selbuf[2048];
 
     /* Start of with keys in __dict__ */
-    result = PyDict_Keys(((PyTypeObject*)self)->tp_dict);
+    result = PyDict_Keys(PyObjC_get_tp_dict((PyTypeObject*)self));
     if (result == NULL) { // LCOV_BR_EXCL_LINE
         return NULL;      // LCOV_EXCL_LINE
     }
 
     cls = objc_metaclass_locate(self);
     if (cls == NULL) {
         /* This happens for the root of the class tree */
@@ -1229,15 +1231,18 @@
         if (PyObjCClass_Check(base)) {
             if (PyObjCClass_CheckMethodList(base, 0) < 0) {
                 return NULL;
             }
             dict = ((PyTypeObject*)base)->tp_dict;
 
         } else if (PyType_Check(base)) { // LCOV_BR_EXCL_LINE
-            dict = ((PyTypeObject*)base)->tp_dict;
+            dict = PyObjC_get_tp_dict((PyTypeObject*)base);
+            if (dict == NULL) {
+                continue;
+            }
 
         } else {
             /* Cannot happen: non-class on MRO  */
             return NULL; // LCOV_EXCL_LINE
         }
 
         PyObjC_Assert(dict && PyDict_Check(dict), NULL);
@@ -1347,15 +1352,15 @@
                 Py_DECREF(class_for_base);
                 if (descr == NULL) { // LCOV_BR_EXCL_LINE
                     return NULL;     //  LCOV_EXCL_LINE
                 }
 
                 /* add to __dict__ 'cache' */
                 if (PyDict_SetItem( // LCOV_BR_EXCL_LINE
-                        ((PyTypeObject*)base)->tp_dict, name, descr)
+                        PyObjC_get_tp_dict((PyTypeObject*)base), name, descr)
                     == -1) {
                     // LCOV_EXCL_START
                     Py_DECREF(descr);
                     return NULL;
                     // LCOV_EXCL_STOP
                 }
 
@@ -1376,15 +1381,15 @@
 }
 
 PyObject* _Nullable PyObjCMetaClass_TryResolveSelector(PyObject* base, PyObject* name,
                                                        SEL sel)
 {
     Class     cls;
     Method    m;
-    PyObject* dict = ((PyTypeObject*)base)->tp_dict;
+    PyObject* dict = PyObjC_get_tp_dict((PyTypeObject*)base);
 
     Py_BEGIN_ALLOW_THREADS
         @try { /* XXX: Can this raise?, and is it necessary to give up the GIL here? */
             cls = objc_metaclass_locate(base);
             if (cls == Nil) {
                 /* XXX: Fix for a sporadic crash when resolving methods */
                 m = nil;
@@ -1463,24 +1468,26 @@
         return NULL;   // LCOV_EXCL_LINE
     }
     PyObjC_Assert(PyTuple_Check(mro), NULL);
     n = PyTuple_GET_SIZE(mro);
     for (i = 0; i < n; i++) {
         base = PyTuple_GET_ITEM(mro, i);
         if (PyType_Check(base)) { // LCOV_BR_EXCL_LINE
-            dict = ((PyTypeObject*)base)->tp_dict;
+            dict = PyObjC_get_tp_dict((PyTypeObject*)base);
 
         } else {
             /* Cannot happen: non-type in MRO */
             return NULL; // LCOV_EXCL_LINE
         }
 
-        descr = PyDict_GetItem(dict, name);
-        if (descr != NULL) {
-            return descr;
+        if (dict != NULL) {
+            descr = PyDict_GetItem(dict, name);
+            if (descr != NULL) {
+                return descr;
+            }
         }
 
         if (PyObjCClass_Check(base)) {
             /*Class cls = objc_metaclass_locate(base);*/
             Class  cls = PyObjCClass_GetClass(base);
             Method m;
 
@@ -1676,22 +1683,22 @@
         if (f != NULL && PyDescr_IsData(descr)) {
             result = f(descr, self, (PyObject*)Py_TYPE(self));
             goto done;
         }
     }
 
     if (strcmp(PyObjC_Unicode_Fast_Bytes(name), "__dict__") == 0) {
-
-        result = ((PyTypeObject*)self)->tp_dict;
+        /* XXX: Is this correct */
+        result = PyObjC_get_tp_dict((PyTypeObject*)self);
         goto done;
     }
 
     if (descr == NULL) {
-        descr = _type_lookup_instance(((PyTypeObject*)self)->tp_dict, (PyTypeObject*)self,
-                                      name);
+        descr = _type_lookup_instance(PyObjC_get_tp_dict((PyTypeObject*)self),
+                                      (PyTypeObject*)self, name);
         if (descr != NULL) {
             f = Py_TYPE(descr)->tp_descr_get;
             if (f != NULL) {
                 result = f(descr, NULL, self);
                 goto done;
             }
         } else if (descr != NULL) {
@@ -1710,15 +1717,15 @@
         }
         if (PyErr_Occurred()) {
             return NULL;
         }
     }
 
     if (descr == NULL) {
-        descr = _type_lookup_instance_harder(((PyTypeObject*)self)->tp_dict,
+        descr = _type_lookup_instance_harder(PyObjC_get_tp_dict((PyTypeObject*)self),
                                              (PyTypeObject*)self, name);
         if (descr != NULL) {
             f = Py_TYPE(descr)->tp_descr_get;
         }
         if (PyErr_Occurred()) {
             /* XXX: can this happen without descr being NULL? */
             return NULL;
@@ -1753,15 +1760,15 @@
     name_bytes = PyObjC_Unicode_Fast_Bytes(name);
     if (name_bytes == NULL) {
         return NULL;
     }
     result = PyObjCSelector_FindNative(self, name_bytes);
 
     if (result != NULL) {
-        int res = PyDict_SetItem(((PyTypeObject*)self)->tp_dict, name, result);
+        int res = PyDict_SetItem(PyObjC_get_tp_dict((PyTypeObject*)self), name, result);
         PyObjCNativeSelector* x = (PyObjCNativeSelector*)result;
 
         if (x->base.sel_flags & PyObjCSelector_kCLASS_METHOD) {
             x->base.sel_self = self;
             Py_INCREF(x->base.sel_self);
         }
         if (res < 0) { // LCOV_BR_EXCL_LINE
@@ -1809,25 +1816,37 @@
                 if (protocols == NULL) {
                     return -1;
                 }
             } else {
                 return -1;
             }
         }
-        value = PyObjC_TransformAttribute(name, value, self, protocols);
+        PyObject* old_value = value;
+        value               = PyObjC_TransformAttribute(name, value, self, protocols);
         Py_DECREF(protocols);
         if (value == NULL) {
             return -1;
         }
 
         if (PyObjCNativeSelector_Check(value)) {
-            Py_DECREF(value);
-            PyErr_SetString(PyExc_TypeError,
-                            "Assigning native selectors is not supported");
-            return -1;
+            /* XXX:
+             *   The test for old_value is not ideal and is present
+             *   to make it possible to use ``python_method(sel)`` to
+             *   create an alias for ``sel``. Can't check for ``python_method``
+             *   here because that type is python only.
+             *
+             *   Remove this once there is a good and documented way to
+             *   accomplish this.
+             */
+            if (value == old_value) {
+                Py_DECREF(value);
+                PyErr_SetString(PyExc_TypeError,
+                                "Assigning native selectors is not supported");
+                return -1;
+            }
 
         } else if (((PyObjCClassObject*)self)->isCFWrapper) {
             /* This is a wrapper class for a CoreFoundation type
              * that isn't tollfree bridged. Don't update the
              * Objective-C class because all CF types share the
              * same ObjC class (except for the toll-free bridged
              * ones).
@@ -1905,18 +1924,19 @@
                 // LCOV_EXCL_STOP
 
             } else if (hidden) {
                 Py_DECREF(value);
 
             } else {
                 if (PyObjCSelector_IsClassMethod(value)) {
-                    r = PyDict_SetItem(Py_TYPE(self)->tp_dict, name, value);
+                    r = PyDict_SetItem(PyObjC_get_tp_dict(Py_TYPE(self)), name, value);
 
                 } else {
-                    r = PyDict_SetItem(((PyTypeObject*)self)->tp_dict, name, value);
+                    r = PyDict_SetItem(PyObjC_get_tp_dict((PyTypeObject*)self), name,
+                                       value);
                 }
 
                 Py_DECREF(value);
                 if (r == -1) { // LCOV_BR_EXCL_LINE
                     // LCOV_EXCL_START
                     PyErr_NoMemory();
                     return -1;
@@ -2239,15 +2259,15 @@
     PyObject*    result;
     Class        cls;
     Method*      methods;
     unsigned int method_count, i;
     char         selbuf[2048];
 
     /* Start of with keys in __dict__ */
-    result = PyDict_Keys(((PyTypeObject*)self)->tp_dict);
+    result = PyDict_Keys(PyObjC_get_tp_dict((PyTypeObject*)self));
     if (result == NULL) { // LCOV_BR_EXCL_LINE
         return NULL;      // LCOV_EXCL_LINE
     }
 
     cls = PyObjCClass_GetClass(self);
 
     while (cls != NULL) {
@@ -2556,16 +2576,19 @@
     info->lookup_cache         = NULL;
 
     objc_class_register(objc_class, result);
 
     /*
      * Support the buffer protocol in the wrappers for NSData and
      * NSMutableData, the only two classes where this makes sense.
+     *
+     * XXX: This changes the 'result' class after it is 'ready', which
+     *      could be problematic.
      */
-    if (strcmp(className, "NSData") == 0) {
+    if (PyObjC_class_isSubclassOf(objc_class, [NSData class])) {
         ((PyTypeObject*)result)->tp_as_buffer = &nsdata_as_buffer;
         PyType_Modified((PyTypeObject*)result);
         PyType_Ready((PyTypeObject*)result);
 
     } else if (strcmp(className, "NSBlock") == 0) {
         ((PyTypeObject*)result)->tp_basicsize = sizeof(PyObjCBlockObject);
         PyType_Modified((PyTypeObject*)result);
@@ -2948,17 +2971,17 @@
         if (!PyObjCClass_Check(c)) {
             continue;
         }
 
         PyObject* dict;
 
         if (class_method) {
-            dict = Py_TYPE(c)->tp_dict;
+            dict = PyObjC_get_tp_dict(Py_TYPE(c));
         } else {
-            dict = ((PyTypeObject*)c)->tp_dict;
+            dict = PyObjC_get_tp_dict((PyTypeObject*)c);
         }
 
         PyObject*  value = NULL;
         Py_ssize_t pos   = 0;
 
         while (PyDict_Next(dict, &pos, NULL, &value)) {
             if (!PyObjCSelector_Check(value))
@@ -3106,15 +3129,15 @@
                 || PyObjC_is_ascii_string(k, "__slots__")
                 || PyObjC_is_ascii_string(k, "__mro__")) {
 
                 continue;
             }
 
         } else {
-            if (PyDict_SetItem(((PyTypeObject*)cls)->tp_dict, k, v) == -1) {
+            if (PyDict_SetItem(PyObjC_get_tp_dict((PyTypeObject*)cls), k, v) == -1) {
                 PyErr_Clear();
             }
             continue;
         }
 
         if (PyType_Type.tp_setattro(cls, k, v) == -1) {
             PyErr_Clear();
@@ -3334,19 +3357,19 @@
         PyObjC_class_addMethodList((Class _Nonnull)object_getClass(targetClass),
                                    classMethodsToAdd, (unsigned)curClassMethodIndex);
     }
 
     PyMem_Free(classMethodsToAdd);
     classMethodsToAdd = NULL;
 
-    r = PyDict_Merge(((PyTypeObject*)classObject)->tp_dict, extraDict, 1);
+    r = PyDict_Merge(PyObjC_get_tp_dict((PyTypeObject*)classObject), extraDict, 1);
     if (r == -1)                       // LCOV_BR_EXCL_LINE
         goto cleanup_and_return_error; // LCOV_EXCL_LINE
 
-    r = PyDict_Merge(Py_TYPE(classObject)->tp_dict, metaDict, 1);
+    r = PyDict_Merge(PyObjC_get_tp_dict(Py_TYPE(classObject)), metaDict, 1);
     if (r == -1)                       // LCOV_BR_EXCL_LINE
         goto cleanup_and_return_error; // LCOV_EXCL_LINE
 
     Py_DECREF(protocols);
     Py_DECREF(extraDict);
     extraDict = NULL;
     Py_DECREF(metaDict);
```

### Comparing `pyobjc-core-9.1b1/Modules/objc/objc-object.h` & `pyobjc-core-9.2/Modules/objc/objc-object.h`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/objc-object.m` & `pyobjc-core-9.2/Modules/objc/objc-object.m`

 * *Files 1% similar despite different names*

```diff
@@ -275,15 +275,15 @@
 PyObject* _Nullable PyObjCClass_TryResolveSelector(PyObject* base, PyObject* name,
                                                    SEL sel)
 {
     Class cls = PyObjCClass_GetClass(base);
     if (cls == NULL) {
         return NULL;
     }
-    PyObject* dict = ((PyTypeObject*)base)->tp_dict;
+    PyObject* dict = PyObjC_get_tp_dict((PyTypeObject*)base);
     Method    m    = class_getInstanceMethod(cls, sel);
     if (m) {
 #ifndef PyObjC_FAST_BUT_INEXACT
         int   use = 1;
         Class sup = class_getSuperclass(cls);
         if (sup) {
             Method m_sup = class_getInstanceMethod(sup, sel);
@@ -371,18 +371,19 @@
                 }
             }
 
             if (PyObjCClass_CheckMethodList(base, 0) < 0) { // LCOV_BR_EXCL_LINE
                 return NULL;                                // LCOV_EXCL_LINE
             }
 
-            dict = ((PyTypeObject*)base)->tp_dict;
+            dict = PyObjC_get_tp_dict((PyTypeObject*)base);
 
         } else if (PyType_Check(base)) {
-            dict = ((PyTypeObject*)base)->tp_dict;
+
+            dict = PyObjC_get_tp_dict((PyTypeObject*)base);
 
         } else {
             /* XXX: Can this ever happen? */
             return NULL;
         }
 
         PyObjC_Assert(dict && PyDict_Check(dict), NULL);
@@ -504,15 +505,16 @@
                 descr = PyObjCSelector_NewNative(cls, meth_name, encoding, 0);
                 free(methods);
                 if (descr == NULL) {
                     return NULL;
                 }
 
                 /* add to __dict__ 'cache' */
-                if (PyDict_SetItem(((PyTypeObject*)base)->tp_dict, name, descr) == -1) {
+                if (PyDict_SetItem(PyObjC_get_tp_dict((PyTypeObject*)base), name, descr)
+                    == -1) {
                     Py_DECREF(descr);
                     return NULL;
                 }
 
                 /* and return as a borrowed reference */
                 Py_DECREF(descr);
                 return descr;
@@ -1003,15 +1005,15 @@
     PyObject*    result;
     Class        cls;
     Method*      methods;
     unsigned int method_count, i;
     char         selbuf[2048];
 
     /* Start of with keys in __dict__ */
-    result = PyDict_Keys(Py_TYPE(self)->tp_dict);
+    result = PyDict_Keys(PyObjC_get_tp_dict(Py_TYPE(self)));
     if (result == NULL) { // LCOV_BR_EXCL_LINE
         return NULL;      // LCOV_EXCL_LINE
     }
 
     if (PyObjCObject_IsMagic(self)) {
         /* "magic cookie" objects don't have Objective-C methods */
         return result;
```

### Comparing `pyobjc-core-9.1b1/Modules/objc/objc-runtime-compat.h` & `pyobjc-core-9.2/Modules/objc/objc-runtime-compat.h`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/objc-runtime-compat.m` & `pyobjc-core-9.2/Modules/objc/objc-runtime-compat.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/objc_super.m` & `pyobjc-core-9.2/Modules/objc/objc_super.m`

 * *Files 1% similar despite different names*

```diff
@@ -93,18 +93,18 @@
             if (PyObjCClass_Check(tmp)) {
                 if (PyObjCClass_CheckMethodList(tmp, NO) < 0) { // LCOV_BR_EXCL_LINE
                     return NULL;                                // LCOV_EXCL_LINE
                 }
             }
 
             if (PyObjCClass_Check(tmp) && PyObjCClass_Check(su->obj)) {
-                dict = Py_TYPE(tmp)->tp_dict;
+                dict = PyObjC_get_tp_dict(Py_TYPE(tmp));
 
             } else if (PyType_Check(tmp)) {
-                dict = ((PyTypeObject*)tmp)->tp_dict;
+                dict = PyObjC_get_tp_dict((PyTypeObject*)tmp);
 
             } else {
                 continue;
             }
 
             res = PyDict_GetItemWithError(dict, name);
             if (res == NULL && PyErr_Occurred()) { // LCOV_BR_EXCL_LINE
```

### Comparing `pyobjc-core-9.1b1/Modules/objc/objc_support.h` & `pyobjc-core-9.2/Modules/objc/objc_support.h`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/objc_support.m` & `pyobjc-core-9.2/Modules/objc/objc_support.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/objc_util.h` & `pyobjc-core-9.2/Modules/objc/objc_util.h`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 extern PyObject* PyObjCExc_UnInitDeallocWarning;
 extern PyObject* PyObjCExc_ObjCRevivalWarning;
 extern PyObject* PyObjCExc_LockError;
 extern PyObject* PyObjCExc_BadPrototypeError;
 extern PyObject* PyObjCExc_UnknownPointerError;
 extern PyObject* PyObjCExc_DeprecationWarning;
 extern PyObject* PyObjCExc_ObjCPointerWarning;
+extern PyObject* PyObjCExc_ObjCSuperWarning;
 
 extern int PyObjC_CheckArgCount(PyObject* callable, size_t min_args, size_t max_args,
                                 size_t nargsf);
 extern int PyObjC_CheckNoKwnames(PyObject* callable, PyObject* _Nullable kwnames);
 
 extern PyObject* _Nullable PyObjC_MakeCVoidP(void* _Nullable ptr);
```

### Comparing `pyobjc-core-9.1b1/Modules/objc/objc_util.m` & `pyobjc-core-9.2/Modules/objc/objc_util.m`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 PyObject* PyObjCExc_UnInitDeallocWarning;
 PyObject* PyObjCExc_ObjCRevivalWarning;
 PyObject* PyObjCExc_LockError;
 PyObject* PyObjCExc_BadPrototypeError;
 PyObject* PyObjCExc_UnknownPointerError;
 PyObject* PyObjCExc_DeprecationWarning;
 PyObject* PyObjCExc_ObjCPointerWarning;
+PyObject* PyObjCExc_ObjCSuperWarning;
 
 PyObject* PyObjCNM_insert;
 PyObject* PyObjCNM_append;
 PyObject* PyObjCNM_extend;
 PyObject* PyObjCNM_timestamp;
 PyObject* PyObjCNM_fromtimestamp;
 PyObject* PyObjCNM_strftime;
@@ -53,14 +54,15 @@
             PyExc_Warning);
     NEW_EXC(PyObjCExc_LockError, "LockError", PyObjCExc_Error);
     NEW_EXC(PyObjCExc_BadPrototypeError, "BadPrototypeError", PyObjCExc_Error);
     NEW_EXC(PyObjCExc_UnknownPointerError, "UnknownPointerError", PyObjCExc_Error);
     NEW_EXC(PyObjCExc_DeprecationWarning, "ApiDeprecationWarning",
             PyExc_DeprecationWarning);
     NEW_EXC(PyObjCExc_ObjCPointerWarning, "ObjCPointerWarning", PyExc_Warning);
+    NEW_EXC(PyObjCExc_ObjCSuperWarning, "ObjCSuperWarning", PyExc_Warning);
 
 #undef NEW_EXC
 
 #define NEW_STR(identifier, strvalue)                                                    \
     identifier = PyUnicode_InternFromString(strvalue);                                   \
     if (identifier == NULL) {                                                            \
         return -1;                                                                       \
@@ -393,15 +395,18 @@
     if (exc == nil)                // LCOV_BR_EXCL_LINE
         PyObjCErr_InternalError(); // LCOV_EXCL_LINE
 
     if (state) {
         PyGILState_Release(*state);
     }
     @throw exc;
+#pragma clang diagnostic push
+#pragma clang diagnostic ignored "-Wunreachable-code"
     __builtin_unreachable();
+#pragma clang diagnostic pop
 }
 
 char* _Nullable PyObjCUtil_Strdup(const char* value)
 {
     Py_ssize_t len;
     char*      result;
 
@@ -1523,17 +1528,16 @@
                                2 | PY_VECTORCALL_ARGUMENTS_OFFSET, NULL);
 }
 
 PyObject* _Nullable PyObjC_TransformAttribute(PyObject* name, PyObject* value,
                                               PyObject* class_object, PyObject* protocols)
 {
     if (PyObjC_transformAttribute == NULL || PyObjC_transformAttribute == Py_None) {
-        PyErr_SetString(PyObjCExc_InternalError,
-                        "objc.options._transformAttribute is not set");
-        return NULL;
+        Py_INCREF(value);
+        return value;
     }
     PyObject* args[5] = {NULL, name, value, class_object, protocols};
     return PyObject_Vectorcall(PyObjC_transformAttribute, args + 1,
                                4 | PY_VECTORCALL_ARGUMENTS_OFFSET, NULL);
 }
 
 bool
```

### Comparing `pyobjc-core-9.1b1/Modules/objc/opaque-pointer.m` & `pyobjc-core-9.2/Modules/objc/opaque-pointer.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/options.h` & `pyobjc-core-9.2/Modules/objc/options.h`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/options.m` & `pyobjc-core-9.2/Modules/objc/options.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/pointer-support.h` & `pyobjc-core-9.2/Modules/objc/pointer-support.h`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/pointer-support.m` & `pyobjc-core-9.2/Modules/objc/pointer-support.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/proxy-registry.h` & `pyobjc-core-9.2/Modules/objc/proxy-registry.h`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/proxy-registry.m` & `pyobjc-core-9.2/Modules/objc/proxy-registry.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/pyobjc-api.h` & `pyobjc-core-9.2/Modules/objc/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/pyobjc-api.m` & `pyobjc-core-9.2/Modules/objc/pyobjc-api.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/pyobjc-assert.h` & `pyobjc-core-9.2/Modules/objc/pyobjc-assert.h`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/pyobjc-compat.h` & `pyobjc-core-9.2/Modules/objc/pyobjc-compat.h`

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

### Comparing `pyobjc-core-9.1b1/Modules/objc/pyobjc-compat.m` & `pyobjc-core-9.2/Modules/objc/pyobjc-compat.m`

 * *Files 3% similar despite different names*

```diff
@@ -98,14 +98,20 @@
 
     if (!PyUnicode_IS_ASCII(object)) {
         /* The code below raises the correct error in a roundabout
          * way. That's because UnicodeEncodeError expects more
          * than one argument.
          */
         PyObject* r = PyUnicode_AsASCIIString(object);
+        if (unlikely(r != NULL)) {
+            PyErr_SetString(PyObjCExc_Error, "Raising UnicodeError failed");
+            Py_DECREF(r);
+            return NULL;
+        }
+
         PyObjC_Assert(r == NULL, NULL);
         return NULL;
     }
 
     return (const char*)(PyUnicode_DATA(object));
 }
 
@@ -197,8 +203,27 @@
     Py_DECREF(tuple);
     Py_DECREF(callable);
     return res;
 }
 
 #endif
 
+#if PY_VERSION_HEX >= 0x030c0000
+extern PyObject* _Nonnull _PyType_GetDict(PyTypeObject* _Nonnull tp);
+
+extern PyObject*
+PyObjC_get_tp_dict(PyTypeObject* tp)
+{
+    return _PyType_GetDict(tp);
+}
+
+#else
+
+extern PyObject*
+PyObjC_get_tp_dict(PyTypeObject* tp)
+{
+    return tp->tp_dict;
+}
+
+#endif
+
 NS_ASSUME_NONNULL_END
```

### Comparing `pyobjc-core-9.1b1/Modules/objc/pyobjc-unittest.h` & `pyobjc-core-9.2/Modules/objc/pyobjc-unittest.h`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/pyobjc.h` & `pyobjc-core-9.2/Modules/objc/pyobjc.h`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #define PyObjC_H
 
 /*
  * Central include file for PyObjC.
  *
  */
 
-#define OBJC_VERSION "9.1b1"
+#define OBJC_VERSION "9.2"
 
 #define PY_SSIZE_T_CLEAN
 #include <Python.h>
 
 #include "structmember.h"
 
 #include <AvailabilityMacros.h>
```

### Comparing `pyobjc-core-9.1b1/Modules/objc/pyobjc_unicode.m` & `pyobjc-core-9.2/Modules/objc/pyobjc_unicode.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/python-api-used.h` & `pyobjc-core-9.2/Modules/objc/python-api-used.h`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/registry.m` & `pyobjc-core-9.2/Modules/objc/registry.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/released-buffer.h` & `pyobjc-core-9.2/Modules/objc/released-buffer.h`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/released-buffer.m` & `pyobjc-core-9.2/Modules/objc/released-buffer.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/selector.h` & `pyobjc-core-9.2/Modules/objc/selector.h`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/selector.m` & `pyobjc-core-9.2/Modules/objc/selector.m`

 * *Files 1% similar despite different names*

```diff
@@ -1173,14 +1173,19 @@
 #endif
 
 PyObject*
 PyObjCSelector_New(PyObject* callable, SEL selector, const char* _Nullable signature,
                    int class_method, Class _Nullable cls)
 {
     PyObjCPythonSelector* result;
+
+    /*
+     * XXX: Investigate using the python helper in objc._transform instead of
+     *      replicating part of the logic here.
+     */
     if (signature == NULL && PyObjCPythonSelector_Check(callable)) {
         signature = PyObjCUtil_Strdup(
             ((PyObjCPythonSelector*)callable)->base.sel_python_signature);
 
     } else if (signature == NULL) {
         const char* selname = sel_getName(selector);
         size_t      len     = strlen(selname);
```

### Comparing `pyobjc-core-9.1b1/Modules/objc/struct-sockaddr.m` & `pyobjc-core-9.2/Modules/objc/struct-sockaddr.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/struct-wrapper.h` & `pyobjc-core-9.2/Modules/objc/struct-wrapper.h`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/struct-wrapper.m` & `pyobjc-core-9.2/Modules/objc/struct-wrapper.m`

 * *Files 1% similar despite different names*

```diff
@@ -87,17 +87,19 @@
     return res;
 }
 
 static PyObject* _Nullable struct_sq_slice(PyObject* self, Py_ssize_t ilow,
                                            Py_ssize_t ihigh)
 {
     PyObject*  result;
-    Py_ssize_t i, len;
+    Py_ssize_t i;
 
-    len = STRUCT_LENGTH(self);
+#ifdef PyObjC_DEBUG
+    Py_ssize_t len = STRUCT_LENGTH(self);
+#endif
     PyObjC_Assert(ilow >= 0, NULL);
     PyObjC_Assert(ihigh <= len, NULL);
 
     result = PyTuple_New(ihigh - ilow);
     if (result == NULL) {
         return NULL; // LCOV_EXCL_LINE
     }
@@ -148,23 +150,25 @@
     return 0;
 }
 
 static int
 struct_sq_ass_slice(PyObject* self, Py_ssize_t ilow, Py_ssize_t ihigh, PyObject* v)
 {
     PyObject*  seq;
-    Py_ssize_t i, len;
+    Py_ssize_t i;
 
     if (v == NULL) {
         PyErr_Format(PyExc_TypeError, "Cannot delete items in instances of %.100s",
                      Py_TYPE(self)->tp_name);
         return -1;
     }
 
-    len = STRUCT_LENGTH(self);
+#ifdef PyObjC_DEBUG
+    Py_ssize_t len = STRUCT_LENGTH(self);
+#endif
     PyObjC_Assert(ilow >= 0, -1);
     PyObjC_Assert(ilow <= len, -1);
     PyObjC_Assert(ihigh >= 0, -1);
     PyObjC_Assert(ihigh <= len, -1);
 
     seq = PySequence_Fast(v, "Must assign sequence to slice");
     if (seq == NULL)
```

### Comparing `pyobjc-core-9.1b1/Modules/objc/super-call.h` & `pyobjc-core-9.2/Modules/objc/super-call.h`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/super-call.m` & `pyobjc-core-9.2/Modules/objc/super-call.m`

 * *Files 2% similar despite different names*

```diff
@@ -407,14 +407,38 @@
         return retval;
     } else {
         PyErr_Clear();
 
         retval =
             PyObjCFFI_MakeIMPForSignature(methinfo, PyObjCSelector_GetSelector(sel), imp);
 
+        if (retval == NULL && PyErr_ExceptionMatches(PyExc_NotImplementedError)) {
+            PyObject* exc       = NULL;
+            PyObject* tp        = NULL;
+            PyObject* traceback = NULL;
+
+            PyErr_Fetch(&tp, &exc, &traceback);
+            PyErr_NormalizeException(&tp, &exc, &traceback);
+
+            Py_INCREF(exc);
+            PyErr_Restore(tp, exc, traceback);
+
+            PyErr_Format(PyExc_NotImplementedError, "Cannot generate IMP for %s",
+                         sel_getName(aSelector));
+
+            PyObject* new_exc = NULL;
+
+            PyErr_Fetch(&tp, &new_exc, &traceback);
+            PyErr_NormalizeException(&tp, &new_exc, &traceback);
+            Py_INCREF(new_exc);
+            PyErr_Restore(tp, new_exc, traceback);
+            PyException_SetCause(new_exc, exc);
+            Py_DECREF(new_exc);
+        }
+
         return retval;
     }
 }
 
 // LCOV_EXCL_START
 /* The two functions below are never called */
 IMP
```

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/NULL.m` & `pyobjc-core-9.2/Modules/objc/test/NULL.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/arrayint.m` & `pyobjc-core-9.2/Modules/objc/test/arrayint.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/arrays.m` & `pyobjc-core-9.2/Modules/objc/test/arrays.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/block.m` & `pyobjc-core-9.2/Modules/objc/test/block.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/bufsizeinarg.m` & `pyobjc-core-9.2/Modules/objc/test/bufsizeinarg.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/cfsocket.m` & `pyobjc-core-9.2/Modules/objc/test/cfsocket.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/classes.m` & `pyobjc-core-9.2/Modules/objc/test/classes.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/clinmeth.m` & `pyobjc-core-9.2/Modules/objc/test/clinmeth.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/coding.m` & `pyobjc-core-9.2/Modules/objc/test/coding.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/copying.m` & `pyobjc-core-9.2/Modules/objc/test/copying.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/corefoundation.m` & `pyobjc-core-9.2/Modules/objc/test/corefoundation.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/dataint.m` & `pyobjc-core-9.2/Modules/objc/test/dataint.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/dateint.m` & `pyobjc-core-9.2/Modules/objc/test/dateint.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/decimal.m` & `pyobjc-core-9.2/Modules/objc/test/decimal.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/deprecations.m` & `pyobjc-core-9.2/Modules/objc/test/deprecations.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/dictint.m` & `pyobjc-core-9.2/Modules/objc/test/dictint.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/enumeration.m` & `pyobjc-core-9.2/Modules/objc/test/enumeration.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/exceptions.m` & `pyobjc-core-9.2/Modules/objc/test/exceptions.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/filepointer.m` & `pyobjc-core-9.2/Modules/objc/test/filepointer.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/fsref.m` & `pyobjc-core-9.2/Modules/objc/test/fsref.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/gcov.m` & `pyobjc-core-9.2/Modules/objc/test/gcov.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/helpernsdata.m` & `pyobjc-core-9.2/Modules/objc/test/helpernsdata.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/helpernsobject.m` & `pyobjc-core-9.2/Modules/objc/test/helpernsobject.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/identity.m` & `pyobjc-core-9.2/Modules/objc/test/identity.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/initialize.m` & `pyobjc-core-9.2/Modules/objc/test/initialize.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/instanceVariables.m` & `pyobjc-core-9.2/Modules/objc/test/instanceVariables.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/locking.m` & `pyobjc-core-9.2/Modules/objc/test/locking.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/metadata.m` & `pyobjc-core-9.2/Modules/objc/test/metadata.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/metadatafunction.m` & `pyobjc-core-9.2/Modules/objc/test/metadatafunction.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/methodaccess.m` & `pyobjc-core-9.2/Modules/objc/test/methodaccess.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/methodlookup.m` & `pyobjc-core-9.2/Modules/objc/test/methodlookup.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/methres1.m` & `pyobjc-core-9.2/Modules/objc/test/methres1.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/methres2.m` & `pyobjc-core-9.2/Modules/objc/test/methres2.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/misc.m` & `pyobjc-core-9.2/Modules/objc/test/misc.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/missing1.m` & `pyobjc-core-9.2/Modules/objc/test/missing1.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/missing2.m` & `pyobjc-core-9.2/Modules/objc/test/missing2.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/missing3.m` & `pyobjc-core-9.2/Modules/objc/test/missing3.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/nsobjectcategory.m` & `pyobjc-core-9.2/Modules/objc/test/nsobjectcategory.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/nulldelimitedresult.m` & `pyobjc-core-9.2/Modules/objc/test/nulldelimitedresult.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/objectint.m` & `pyobjc-core-9.2/Modules/objc/test/objectint.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/opaque.m` & `pyobjc-core-9.2/Modules/objc/test/opaque.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/pointersupport.m` & `pyobjc-core-9.2/Modules/objc/test/pointersupport.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/properties.m` & `pyobjc-core-9.2/Modules/objc/test/properties.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/protected.m` & `pyobjc-core-9.2/Modules/objc/test/protected.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/protocol.m` & `pyobjc-core-9.2/Modules/objc/test/protocol.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/pythonnumber.m` & `pyobjc-core-9.2/Modules/objc/test/pythonnumber.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/pythonset.m` & `pyobjc-core-9.2/Modules/objc/test/pythonset.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/sequence.m` & `pyobjc-core-9.2/Modules/objc/test/sequence.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/sockaddr.m` & `pyobjc-core-9.2/Modules/objc/test/sockaddr.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/specialtypecodes.m` & `pyobjc-core-9.2/Modules/objc/test/specialtypecodes.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/stringint.m` & `pyobjc-core-9.2/Modules/objc/test/stringint.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/structargs.m` & `pyobjc-core-9.2/Modules/objc/test/structargs.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/structpointer1.m` & `pyobjc-core-9.2/Modules/objc/test/structpointer1.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/structpointer2.m` & `pyobjc-core-9.2/Modules/objc/test/structpointer2.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/structs.m` & `pyobjc-core-9.2/Modules/objc/test/structs.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/testbndl.m` & `pyobjc-core-9.2/Modules/objc/test/testbndl.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/testbndl2.m` & `pyobjc-core-9.2/Modules/objc/test/testbndl2.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/testclassandinst.m` & `pyobjc-core-9.2/Modules/objc/test/testclassandinst.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/testoutputinitializer.m` & `pyobjc-core-9.2/Modules/objc/test/testoutputinitializer.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/vector.m` & `pyobjc-core-9.2/Modules/objc/test/vector.m`

 * *Files 14% similar despite different names*

```diff
@@ -2,17 +2,33 @@
 #include "pyobjc-api.h"
 #import <simd/simd.h>
 #include <stdarg.h>
 
 #import <Foundation/Foundation.h>
 
 #import <GameplayKit/GameplayKit.h>
+#if PyObjC_BUILD_RELEASE >= 1013
 #import <MetalPerformanceShaders/MetalPerformanceShaders.h>
+#endif /* PyObjC_BUILD_RELEASE >= 1013 */
 #import <ModelIO/ModelIO.h>
 
+#if PyObjC_BULD_RELEASE < 1013
+#define simd_uchar16 vector_uchar16
+#define simd_float2 vector_float2
+#define simd_float3 vector_float3
+#define simd_float4 vector_float4
+#define simd_double2 vector_double2
+#define simd_double3 vector_double3
+#define simd_double4 vector_double4
+#define simd_uint2 vector_uint2
+#define simd_uint3 vector_uint3
+#define simd_int2 vector_int2
+#define simd_int4 vector_int4
+#endif /*  PyObjC_BULD_RELEASE < 1013 */
+
 @interface OC_Vector : NSObject {
     PyObject* values;
 }
 @end
 
 @implementation OC_Vector
 - (instancetype)init
@@ -105,25 +121,29 @@
 GET_VALUE(getVectorUChar16, simd_uchar16,
           ((simd_uchar16){1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 14, 16}))
 GET_VALUE(getVectorDouble2, simd_double2, ((simd_double2){-42.9, 42.8}))
 GET_VALUE(getVectorFloat2, simd_float2, ((simd_float2){-9.5, 10.5}))
 GET_VALUE(getVectorFloat3, simd_float3, ((simd_float3){-8.5, 9.5, 12.5}))
 GET_VALUE(getVectorFloat4, simd_float4, ((simd_float4){-7.5, 13.5, 14.5, 16.5}))
 GET_VALUE(getVectorInt2, simd_int2, ((simd_int2){42, 43}))
+#if PyObjC_BUILD_RELEASE >= 1012
 GET_VALUE(getGKBox, GKBox, ((GKBox){{1.5, 2.5, 3.5}, {4.5, 5.5, 6.5}}))
 GET_VALUE(getGKQuad, GKQuad, ((GKQuad){{7.5, 8.5}, {9.5, 10.5}}))
+#endif /*  PyObjC_BUILD_RELEASE >= 1012 */
 GET_VALUE(getMDLAxisAlignedBoundingBox, MDLAxisAlignedBoundingBox,
           ((MDLAxisAlignedBoundingBox){{11.5, 12.5, 13.5}, {14.5, 15.5, 16.5}}))
 GET_VALUE(getMDLVoxelIndexExtent, MDLVoxelIndexExtent,
           ((MDLVoxelIndexExtent){{-1, -2, -3, -4}, {-5, -6, -7, -8}}))
+#if PyObjC_BUILD_RELEASE >= 1013
 GET_VALUE(getMPSAxisAlignedBoundingBox, MPSAxisAlignedBoundingBox,
           ((MPSAxisAlignedBoundingBox){{-1.5, -2.5, -3.5}, {-5.5, -6.5, -7.5}}))
 GET_VALUE(getMPSImageHistogramInfo, MPSImageHistogramInfo,
           ((MPSImageHistogramInfo){
               1ULL << 40, YES, {-8.5, -9.5, -10.5, -11.5}, {-12.5, -13.5, -14.5, -15.5}}))
+#endif /* PyObjC_BUILD_RELEASE >= 1013 */
 GET_VALUE(getMatrixDouble4x4, matrix_double4x4,
           ((matrix_double4x4){{{-20.5, -21.5, -22.5, -23.5},
                                {-30.5, -31.5, -32.5, -33.5},
                                {-40.5, -41.5, -42.5, -43.5},
                                {-50.5, -51.5, -52.5, -53.5}}}))
 GET_VALUE(getMatrixFloat2x2, matrix_float2x2,
           ((matrix_float2x2){{{-20.5, -21.5}, {-30.5, -31.5}}}))
@@ -132,20 +152,22 @@
                               {-130.5, -131.5, -132.5},
                               {-140.5, -141.5, -142.5}}}))
 GET_VALUE(getMatrixFloat4x4, matrix_float4x4,
           ((matrix_float4x4){{{-220.5, -221.5, -222.5, 10.5},
                               {-230.5, -231.5, -232.5, 11.5},
                               {-240.5, -241.5, -242.5, 12.5},
                               {-250.5, -251.5, -252.5, 13.5}}}))
+#if PyObjC_BUILD_RELEASE >= 1013
 GET_VALUE(getSimdFloat4x4, simd_float4x4,
           ((simd_float4x4){{{-320.5, -321.5, -322.5, 1.5},
                             {-330.5, -331.5, -332.5, 2.5},
                             {-340.5, -341.5, -342.5, 3.5},
                             {-350.5, -351.5, -352.5, 4.5}}}))
 GET_VALUE(getSimdQuatf, simd_quatf, ((simd_quatf){{-420.5, -421.5, -422.5}}))
+#endif /* PyObjC_BUILD_RELEASE >= 1013 */
 
 SET_VALUE_VALUE(setVectorFloat3, andFloat3, simd_float3, "<3f>", simd_float3, "<3f>")
 SET_VALUE_VALUE(setVectorFloat3, andInt4, simd_float3, "<3f>", simd_int4, "<4i>")
 SET_VALUE_VALUE(setVectorInt4, andFloat3, simd_int4, "<4i>", simd_float3, "<3f>")
 SET_VALUE_VALUE(setId, andFloat2, id, "@", simd_float2, "<2f>")
 SET_VALUE_VALUE(setId, andFloat3, id, "@", simd_float3, "<3f>")
 SET_VALUE_VALUE(setId, andFloat4, id, "@", simd_float4, "<4f>")
```

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/vectorcall.m` & `pyobjc-core-9.2/Modules/objc/test/vectorcall.m`

 * *Files 0% similar despite different names*

```diff
@@ -7,17 +7,33 @@
 #include "pyobjc-api.h"
 #import <simd/simd.h>
 #include <stdarg.h>
 
 #import <Foundation/Foundation.h>
 
 #import <GameplayKit/GameplayKit.h>
+#if PyObjC_BUILD_RELEASE >= 1013
 #import <MetalPerformanceShaders/MetalPerformanceShaders.h>
+#endif /* PyObjC_BUILD_RELEASE >= 1013 */
 #import <ModelIO/ModelIO.h>
 
+#if PyObjC_BULD_RELEASE < 1013
+#define simd_uchar16 vector_uchar16
+#define simd_float2 vector_float2
+#define simd_float3 vector_float3
+#define simd_float4 vector_float4
+#define simd_double2 vector_double2
+#define simd_double3 vector_double3
+#define simd_double4 vector_double4
+#define simd_uint2 vector_uint2
+#define simd_uint3 vector_uint3
+#define simd_int2 vector_int2
+#define simd_int4 vector_int4
+#endif /*  PyObjC_BULD_RELEASE < 1013 */
+
 @interface OC_VectorCall : NSObject {
     PyObject* values;
 }
 @end
 
 static PyObject* clsvalues   = NULL;
 static BOOL      shouldRaise = NO;
@@ -3326,14 +3342,15 @@
             PyObjC_GIL_FORWARD_EXC();
         if (PyList_Append(items, tmp) == -1)
             PyObjC_GIL_FORWARD_EXC();
     PyObjC_END_WITH_GIL
     return @"hello";
 }
 
+#if PyObjC_BUILD_RELEASE >= 1012
 - (id)idid:(id)arg0 GKBox:(GKBox)arg1
 {
     PyObject* items;
     PyObject* tmp;
 
     if ([self shouldRaise]) {
         shouldRaise = NO;
@@ -3437,14 +3454,15 @@
         if (tmp == NULL)
             PyObjC_GIL_FORWARD_EXC();
         if (PyList_Append(items, tmp) == -1)
             PyObjC_GIL_FORWARD_EXC();
     PyObjC_END_WITH_GIL
     return @"hello";
 }
+#endif /* PyObjC_BUILD_RELEASE >= 1012 */
 
 - (id)idid:(id)arg0
     MDLAxisAlignedBoundingBox:(MDLAxisAlignedBoundingBox)arg1
                             f:(float)arg2
 {
     PyObject* items;
     PyObject* tmp;
@@ -4521,14 +4539,15 @@
             PyObjC_GIL_FORWARD_EXC();
         if (PyList_Append(items, tmp) == -1)
             PyObjC_GIL_FORWARD_EXC();
     PyObjC_END_WITH_GIL
     return @"hello";
 }
 
+#if PyObjC_BUILD_RELEASE >= 1012
 - (id)idGKBox:(GKBox)arg0
 {
     PyObject* items;
     PyObject* tmp;
 
     if ([self shouldRaise]) {
         shouldRaise = NO;
@@ -4724,14 +4743,15 @@
         if (tmp == NULL)
             PyObjC_GIL_FORWARD_EXC();
         if (PyList_Append(items, tmp) == -1)
             PyObjC_GIL_FORWARD_EXC();
     PyObjC_END_WITH_GIL
     return @"hello";
 }
+#endif /*  PyObjC_BUILD_RELEASE >= 1012 */
 
 - (id)idMDLVoxelIndexExtent:(MDLVoxelIndexExtent)arg0
 {
     PyObject* items;
     PyObject* tmp;
 
     if ([self shouldRaise]) {
@@ -6581,14 +6601,15 @@
         if (tmp == NULL)
             PyObjC_GIL_FORWARD_EXC();
         if (PyList_Append(items, tmp) == -1)
             PyObjC_GIL_FORWARD_EXC();
     PyObjC_END_WITH_GIL
 }
 
+#if PyObjC_BUILD_RELEASE >= 1013
 - (void)vsimdfloat4x4:(simd_float4x4)arg0
 {
     PyObject* items;
     PyObject* tmp;
 
     if ([self shouldRaise]) {
         shouldRaise = NO;
@@ -6830,14 +6851,17 @@
         tmp = PyObjC_ObjCToPython("d", &arg1);
         if (tmp == NULL)
             PyObjC_GIL_FORWARD_EXC();
         if (PyList_Append(items, tmp) == -1)
             PyObjC_GIL_FORWARD_EXC();
     PyObjC_END_WITH_GIL
 }
+#endif /* PyObjC_BUILD_RELEASE >= 1013 */
+
+#if PyObjC_BUILD_RELEASE >= 1012
 
 - (GKBox)GKBox
 {
     if ([self shouldRaise]) {
         shouldRaise = NO;
         [NSException raise:@"SimpleException" format:@"hello world"];
     }
@@ -6940,14 +6964,15 @@
         if (PyList_Append(items, tmp) == -1)
             PyObjC_GIL_FORWARD_EXC();
     PyObjC_END_WITH_GIL
     return (GKTriangle){{(vector_float3){-18.5, -19.5, -110.5},
                          (vector_float3){-111.5, -112.5, -113.5},
                          (vector_float3){-17.5, 11.5, 122.5}}};
 }
+#endif /* PyObjC_BUILD_RELEASE >= 1012 */
 
 - (MDLAxisAlignedBoundingBox)MDLAxisAlignedBoundingBox
 {
     if ([self shouldRaise]) {
         shouldRaise = NO;
         [NSException raise:@"SimpleException" format:@"hello world"];
     }
@@ -7101,14 +7126,15 @@
         if (clsvalues == NULL)
             PyObjC_GIL_FORWARD_EXC();
     PyObjC_END_WITH_GIL
     return (MDLVoxelIndexExtent){(vector_int4){100, 101, 102, 103},
                                  (vector_int4){-20, -21, -22, -23}};
 }
 
+#if PyObjC_BUILD_RELEASE >= 1013
 - (MPSAxisAlignedBoundingBox)MPSAxisAlignedBoundingBox
 {
     if ([self shouldRaise]) {
         shouldRaise = NO;
         [NSException raise:@"SimpleException" format:@"hello world"];
     }
 
@@ -7166,14 +7192,15 @@
         if (clsvalues == NULL)
             PyObjC_GIL_FORWARD_EXC();
     PyObjC_END_WITH_GIL
     return (MPSImageHistogramInfo){4398046511104, YES,
                                    (vector_float4){1.0, 2.0, 3.0, 4.0},
                                    (vector_float4){-1.0, -2.0, -3.0, -4.0}};
 }
+#endif /* PyObjC_BUILD_RELEASE >= 1013 */
 
 - (matrix_double4x4)matrixdouble4x4
 {
     if ([self shouldRaise]) {
         shouldRaise = NO;
         [NSException raise:@"SimpleException" format:@"hello world"];
     }
@@ -7459,14 +7486,15 @@
             PyObjC_GIL_FORWARD_EXC();
     PyObjC_END_WITH_GIL
     return (matrix_float4x4){
         {(vector_float4){0.0, 1.5, 3.0, 4.5}, (vector_float4){0.0, 1.5, 3.0, 4.5},
          (vector_float4){0.0, 1.5, 3.0, 4.5}, (vector_float4){0.0, 1.5, 3.0, 4.5}}};
 }
 
+#if PyObjC_BUILD_RELEASE >= 1013
 - (simd_float4x4)simdfloat4x4
 {
     if ([self shouldRaise]) {
         shouldRaise = NO;
         [NSException raise:@"SimpleException" format:@"hello world"];
     }
 
@@ -7674,14 +7702,15 @@
         if (tmp == NULL)
             PyObjC_GIL_FORWARD_EXC();
         if (PyList_Append(items, tmp) == -1)
             PyObjC_GIL_FORWARD_EXC();
     PyObjC_END_WITH_GIL
     return (simd_quatf){(vector_float4){0.0, 1.5, 3.0, 4.5}};
 }
+#endif /* PyObjC_BUILD_RELEASE >= 1013 */
 
 @end
 
 @interface OC_VectorCallInvoke : NSObject {
 }
 @end
 
@@ -8407,14 +8436,15 @@
         if (PyObjC_PythonToObjC("@", inter, &cinter) == -1) {
             PyObjC_GIL_FORWARD_EXC();
         }
     PyObjC_END_WITH_GIL
     return cinter;
 }
 
+#if PyObjC_BUILD_RELEASE >= 1012
 + (id)ididGKBoxOn:(OC_VectorCall*)value
 {
     id result = [value
          idid:@"hello"
         GKBox:(GKBox){(vector_float3){1.0, 2.0, 3.0}, (vector_float3){4.0, 5.0, 6.0}}];
     id cinter;
     PyObjC_BEGIN_WITH_GIL
@@ -8436,14 +8466,15 @@
         PyObject* inter = PyObjC_ObjCToPython("@", &result);
         if (PyObjC_PythonToObjC("@", inter, &cinter) == -1) {
             PyObjC_GIL_FORWARD_EXC();
         }
     PyObjC_END_WITH_GIL
     return cinter;
 }
+#endif /* PyObjC_BUILD_RELEASE >= 1012 */
 
 + (id)ididMDLAxisAlignedBoundingBoxfOn:(OC_VectorCall*)value
 {
     id result = [value idid:@"hello"
         MDLAxisAlignedBoundingBox:(MDLAxisAlignedBoundingBox) {
             (vector_float3){-8.0, -9.0, -10.0}, (vector_float3) { -11.0, -12.0, -13.0 }
         }
@@ -8657,14 +8688,15 @@
         if (PyObjC_PythonToObjC("@", inter, &cinter) == -1) {
             PyObjC_GIL_FORWARD_EXC();
         }
     PyObjC_END_WITH_GIL
     return cinter;
 }
 
+#if PyObjC_BUILD_RELEASE >= 1012
 + (id)idGKBoxOn:(OC_VectorCall*)value
 {
     id result = [value
         idGKBox:(GKBox){(vector_float3){1.0, 2.0, 3.0}, (vector_float3){4.0, 5.0, 6.0}}];
     id cinter;
     PyObjC_BEGIN_WITH_GIL
         PyObject* inter = PyObjC_ObjCToPython("@", &result);
@@ -8716,14 +8748,15 @@
         PyObject* inter = PyObjC_ObjCToPython("@", &result);
         if (PyObjC_PythonToObjC("@", inter, &cinter) == -1) {
             PyObjC_GIL_FORWARD_EXC();
         }
     PyObjC_END_WITH_GIL
     return cinter;
 }
+#endif /* PyObjC_BUILD_RELEASE >= 1012 */
 
 + (id)idMDLVoxelIndexExtentOn:(OC_VectorCall*)value
 {
     id result = [value
         idMDLVoxelIndexExtent:(MDLVoxelIndexExtent){(vector_int4){100, 101, 102, 103},
                                                     (vector_int4){-20, -21, -22, -23}}];
     id cinter;
@@ -9029,14 +9062,15 @@
                 0.0, 1.5, 3.0, 4.5
             }
         }
     }
                          d:-557000000000.0];
 }
 
+#if PyObjC_BUILD_RELEASE >= 1013
 + (void)vsimdfloat4x4On:(OC_VectorCall*)value
 {
     [value vsimdfloat4x4:(simd_float4x4){{(vector_float4){0.0, 1.5, 3.0, 4.5},
                                           (vector_float4){0.0, 1.5, 3.0, 4.5},
                                           (vector_float4){0.0, 1.5, 3.0, 4.5},
                                           (vector_float4){0.0, 1.5, 3.0, 4.5}}}];
 }
@@ -9065,15 +9099,17 @@
 + (void)vsimdquatfdOn:(OC_VectorCall*)value
 {
     [value vsimdquatf:(simd_quatf) {
         (vector_float4) { 0.0, 1.5, 3.0, 4.5 }
     }
                     d:-557000000000.0];
 }
+#endif /* PyObjC_BUILD_RELEASE >= 1013*/
 
+#if PyObjC_BUILD_RELEASE >= 1012
 + (id)GKBoxOn:(OC_VectorCall*)value
 {
     id    cinter;
     GKBox result = [value GKBox];
     PyObjC_BEGIN_WITH_GIL
         PyObject* inter = PyObjC_ObjCToPython("{GKBox=<3f><3f>}", &result);
         if (PyObjC_PythonToObjC("@", inter, &cinter) == -1) {
@@ -9104,14 +9140,15 @@
         PyObject* inter = PyObjC_ObjCToPython("{GKTriangle=[3<3f>]}", &result);
         if (PyObjC_PythonToObjC("@", inter, &cinter) == -1) {
             PyObjC_GIL_FORWARD_EXC();
         }
     PyObjC_END_WITH_GIL
     return cinter;
 }
+#endif /* PyObjC_BUILD_RELEASE >= 1012 */
 
 + (id)MDLAxisAlignedBoundingBoxOn:(OC_VectorCall*)value
 {
     id                        cinter;
     MDLAxisAlignedBoundingBox result = [value MDLAxisAlignedBoundingBox];
     PyObjC_BEGIN_WITH_GIL
         PyObject* inter =
@@ -9161,14 +9198,15 @@
         if (PyObjC_PythonToObjC("@", inter, &cinter) == -1) {
             PyObjC_GIL_FORWARD_EXC();
         }
     PyObjC_END_WITH_GIL
     return cinter;
 }
 
+#if PyObjC_BUILD_RELEASE >= 1013
 + (id)MPSAxisAlignedBoundingBoxOn:(OC_VectorCall*)value
 {
     id                        cinter;
     MPSAxisAlignedBoundingBox result = [value MPSAxisAlignedBoundingBox];
     PyObjC_BEGIN_WITH_GIL
         PyObject* inter =
             PyObjC_ObjCToPython("{_MPSAxisAlignedBoundingBox=<3f><3f>}", &result);
@@ -9188,14 +9226,15 @@
             PyObjC_ObjCToPython("{_MPSImageHistogramInfo=QZ<4f><4f>}", &result);
         if (PyObjC_PythonToObjC("@", inter, &cinter) == -1) {
             PyObjC_GIL_FORWARD_EXC();
         }
     PyObjC_END_WITH_GIL
     return cinter;
 }
+#endif /* PyObjC_BUILD_RELEASE >= 1013 */
 
 + (id)matrixdouble4x4On:(OC_VectorCall*)value
 {
     id               cinter;
     matrix_double4x4 result = [value matrixdouble4x4];
     PyObjC_BEGIN_WITH_GIL
         PyObject* inter = PyObjC_ObjCToPython("{_matrix_double4x4=[4<4d>]}", &result);
@@ -9280,14 +9319,15 @@
         if (PyObjC_PythonToObjC("@", inter, &cinter) == -1) {
             PyObjC_GIL_FORWARD_EXC();
         }
     PyObjC_END_WITH_GIL
     return cinter;
 }
 
+#if PyObjC_BUILD_RELEASE >= 1013
 + (id)simdfloat4x4On:(OC_VectorCall*)value
 {
     id            cinter;
     simd_float4x4 result = [value simdfloat4x4];
     PyObjC_BEGIN_WITH_GIL
         PyObject* inter = PyObjC_ObjCToPython("{_simd_float4x4=[4<4f>]}", &result);
         if (PyObjC_PythonToObjC("@", inter, &cinter) == -1) {
@@ -9353,14 +9393,15 @@
         PyObject* inter = PyObjC_ObjCToPython("{_simd_quatf=<4f>}", &result);
         if (PyObjC_PythonToObjC("@", inter, &cinter) == -1) {
             PyObjC_GIL_FORWARD_EXC();
         }
     PyObjC_END_WITH_GIL
     return cinter;
 }
+#endif /* PyObjC_BUILD_RELEASE >= 1013 */
 
 @end
 
 static PyMethodDef mod_methods[] = {{0, 0, 0, 0}};
 
 static struct PyModuleDef mod_module = {
     PyModuleDef_HEAD_INIT, "vectorcall", NULL, 0, mod_methods, NULL, NULL, NULL, NULL};
```

### Comparing `pyobjc-core-9.1b1/Modules/objc/test/voidpointer.m` & `pyobjc-core-9.2/Modules/objc/test/voidpointer.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/varlist.h` & `pyobjc-core-9.2/Modules/objc/varlist.h`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/varlist.m` & `pyobjc-core-9.2/Modules/objc/varlist.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Modules/objc/weakref.m` & `pyobjc-core-9.2/Modules/objc/weakref.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PKG-INFO` & `pyobjc-core-9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-core
-Version: 9.1b1
+Version: 9.2
 Summary: Python<->ObjC Interoperability Module
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren, bbum, SteveM, LeleG, many others stretching back through the reaches of time...
 Author-email: RonaldOussoren@mac.com
 Maintainer: Ronald Oussoren
 Maintainer-email: RonaldOussoren@mac.com
 License: MIT License
```

### Comparing `pyobjc-core-9.1b1/PyObjCTest/archives/py2-oc2.3.keyed` & `pyobjc-core-9.2/PyObjCTest/archives/py2-oc2.3.keyed`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/archives/py2-oc2.3.plain` & `pyobjc-core-9.2/PyObjCTest/archives/py2-oc2.3.plain`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/archives/py3-oc3.0.keyed` & `pyobjc-core-9.2/PyObjCTest/archives/py3-oc3.0.keyed`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/archives/py3-oc3.0.plain` & `pyobjc-core-9.2/PyObjCTest/archives/py3-oc3.0.plain`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/dump-nsarchive-securecoding.m` & `pyobjc-core-9.2/PyObjCTest/dump-nsarchive-securecoding.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/dump-nsarchive.m` & `pyobjc-core-9.2/PyObjCTest/dump-nsarchive.m`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/helper_bridgesupport.py` & `pyobjc-core-9.2/PyObjCTest/helper_bridgesupport.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/keyvaluehelper.py` & `pyobjc-core-9.2/PyObjCTest/keyvaluehelper.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/loader.py` & `pyobjc-core-9.2/PyObjCTest/loader.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_NULL.py` & `pyobjc-core-9.2/PyObjCTest/test_NULL.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_allocatebuffer.py` & `pyobjc-core-9.2/PyObjCTest/test_allocatebuffer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_api_import.py` & `pyobjc-core-9.2/PyObjCTest/test_api_import.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_archive_python.py` & `pyobjc-core-9.2/PyObjCTest/test_archive_python.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     NSUnarchiver,
 )
 from PyObjCTools.TestSupport import (
     TestCase,
     skipUnless,
     expectedFailure,
     expectedFailureIf,
+    min_os_level,
     os_level_key,
     os_release,
     pyobjc_options,
     cast_ulonglong,
 )
 
 import copyreg
@@ -1765,41 +1766,44 @@
 # XXX: This class is empty!
 #
 class TestArchivePythonObjCSubclass(TestCase):
     pass
 
 
 class TestSecureArchivingPython(TestCase):
+    @min_os_level("10.13")
     def test_secure_archive_sequence(self):
         archive = NSKeyedArchiver.alloc().initRequiringSecureCoding_(True)
         sequence = collections.UserList()
         sequence.append(1)
         sequence.append(2)
 
         with self.assertRaisesRegex(
             objc.error,
             "Class 'OC_PythonArray' disallows secure coding. It must return YES from supportsSecureCoding",
         ):
             archive.encodeObject_forKey_(sequence, "sequence")
 
         archive.finishEncoding()
 
+    @min_os_level("10.13")
     def test_secure_archive_mapping(self):
         archive = NSKeyedArchiver.alloc().initRequiringSecureCoding_(True)
         mapping = collections.UserDict()
         mapping["key"] = 1
 
         with self.assertRaisesRegex(
             objc.error,
             "Class 'OC_PythonDictionary' disallows secure coding. It must return YES from supportsSecureCoding",
         ):
             archive.encodeObject_forKey_(mapping, "mapping")
 
         archive.finishEncoding()
 
+    @min_os_level("10.13")
     def test_secure_archive_set(self):
         archive = NSKeyedArchiver.alloc().initRequiringSecureCoding_(True)
 
         class UserSet(set):
             pass
 
         bag = UserSet()
@@ -1809,14 +1813,15 @@
             objc.error,
             "Class 'OC_PythonSet' disallows secure coding. It must return YES from supportsSecureCoding",
         ):
             archive.encodeObject_forKey_(bag, "bag")
 
         archive.finishEncoding()
 
+    @min_os_level("10.13")
     def test_secure_archive_object(self):
         archive = NSKeyedArchiver.alloc().initRequiringSecureCoding_(True)
 
         value = object()
 
         with self.assertRaisesRegex(
             objc.error,
```

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_archiving_interop.py` & `pyobjc-core-9.2/PyObjCTest/test_archiving_interop.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,21 @@
 import datetime
 import platform
 import subprocess
 import tempfile
 from plistlib import loads
 
 import objc
-from PyObjCTools.TestSupport import TestCase, os_release, os_level_key, cast_ulonglong
+from PyObjCTools.TestSupport import (
+    TestCase,
+    os_release,
+    os_level_key,
+    cast_ulonglong,
+    min_os_level,
+)
 
 
 MYDIR = os.path.dirname(os.path.abspath(__file__))
 
 
 NSArray = objc.lookUpClass("NSArray")
 NSArchiver = objc.lookUpClass("NSArchiver")
@@ -138,25 +144,27 @@
                 if testval > 2**63 and os_level_key(os_release()) < os_level_key(
                     "10.14"
                 ):
                     self.assertEqual(cast_ulonglong(converted[0]), testval)
                 else:
                     self.assertEqual(converted[0], testval)
 
-        with self.subTest("overflow"):
-            testval = 2**64
-            v = NSArray.arrayWithObject_(testval)
-            data = NSKeyedArchiver.archivedDataWithRootObject_(v)
+    @min_os_level("10.12")
+    def test_interop_int_overflow(self):
+        # Known error on macOS 10.11
+        testval = 2**64
+        v = NSArray.arrayWithObject_(testval)
+        data = NSKeyedArchiver.archivedDataWithRootObject_(v)
 
-            with tempfile.NamedTemporaryFile() as fp:
-                fp.write(data.bytes())
-                fp.flush()
+        with tempfile.NamedTemporaryFile() as fp:
+            fp.write(data.bytes())
+            fp.flush()
 
-                with self.assertRaises(subprocess.CalledProcessError):
-                    subprocess.check_output([self.progpath, "keyed", fp.name])
+            with self.assertRaises(subprocess.CalledProcessError):
+                subprocess.check_output([self.progpath, "keyed", fp.name])
 
     def test_interop_data(self):
         for testval in (b"hello world",):
             v = NSArray.arrayWithObject_(testval)
             data = NSKeyedArchiver.archivedDataWithRootObject_(v)
 
             with tempfile.NamedTemporaryFile() as fp:
```

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_archiving_secure_interop.py` & `pyobjc-core-9.2/PyObjCTest/test_archiving_secure_interop.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_array_interface.py` & `pyobjc-core-9.2/PyObjCTest/test_array_interface.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_array_property.py` & `pyobjc-core-9.2/PyObjCTest/test_array_property.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_arrays.py` & `pyobjc-core-9.2/PyObjCTest/test_arrays.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_assocations.py` & `pyobjc-core-9.2/PyObjCTest/test_assocations.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_blocks.py` & `pyobjc-core-9.2/PyObjCTest/test_blocks.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_bridged_classes.py` & `pyobjc-core-9.2/PyObjCTest/test_bridged_classes.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_bridges.py` & `pyobjc-core-9.2/PyObjCTest/test_bridges.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_bridgesupport.py` & `pyobjc-core-9.2/PyObjCTest/test_bridgesupport.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_bufsizeinarg.py` & `pyobjc-core-9.2/PyObjCTest/test_bufsizeinarg.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_bundleFunctions.py` & `pyobjc-core-9.2/PyObjCTest/test_bundleFunctions.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_bundleVariables.py` & `pyobjc-core-9.2/PyObjCTest/test_bundleVariables.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_callable_docstr.py` & `pyobjc-core-9.2/PyObjCTest/test_callable_docstr.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_callbacks.py` & `pyobjc-core-9.2/PyObjCTest/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_classandinst.py` & `pyobjc-core-9.2/PyObjCTest/test_classandinst.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_classhooks.py` & `pyobjc-core-9.2/PyObjCTest/test_classhooks.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_clinmeth.py` & `pyobjc-core-9.2/PyObjCTest/test_clinmeth.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_compat.py` & `pyobjc-core-9.2/PyObjCTest/test_compat.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_constants.py` & `pyobjc-core-9.2/PyObjCTest/test_constants.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_context.py` & `pyobjc-core-9.2/PyObjCTest/test_context.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_convenience.py` & `pyobjc-core-9.2/PyObjCTest/test_convenience.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import sys
 import collections.abc
 
 import objc
 import objc._convenience as convenience
+from objc import super
 from PyObjCTest.sequence import OC_TestSequence, OC_TestMutableSequence
 from PyObjCTools.TestSupport import TestCase
 
 objc.addConvenienceForBasicSequence("OC_TestSequence", False)
 objc.addConvenienceForBasicSequence("OC_TestMutableSequence", True)
```

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_conversion.py` & `pyobjc-core-9.2/PyObjCTest/test_conversion.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_copying.py` & `pyobjc-core-9.2/PyObjCTest/test_copying.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_corefoundation.py` & `pyobjc-core-9.2/PyObjCTest/test_corefoundation.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_ctests.py` & `pyobjc-core-9.2/PyObjCTest/test_ctests.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_data_proxy.py` & `pyobjc-core-9.2/PyObjCTest/test_data_proxy.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,14 @@
-from PyObjCTools.TestSupport import TestCase, pyobjc_options
+from PyObjCTools.TestSupport import (
+    TestCase,
+    pyobjc_options,
+    os_level_key,
+    os_release,
+    min_os_level,
+)
 from PyObjCTest.dataint import OC_DataInt
 from PyObjCTest.pythonset import OC_TestSet
 from itertools import count
 import array
 import objc
 
 NSKeyedArchiver = objc.lookUpClass("NSKeyedArchiver")
@@ -90,20 +96,24 @@
             self.assertIs(cls, OC_BuiltinPythonData)
         else:
             self.assertIs(cls, OC_PythonData)
 
     def test_roundtrip_through_keyedarchive(self):
         data = self.bytes_class(b"hello to you too")
 
-        (
-            blob,
-            err,
-        ) = NSKeyedArchiver.archivedDataWithRootObject_requiringSecureCoding_error_(
-            data, False, None
-        )
+        if os_level_key(os_release()) >= os_level_key("10.13"):
+            (
+                blob,
+                err,
+            ) = NSKeyedArchiver.archivedDataWithRootObject_requiringSecureCoding_error_(
+                data, False, None
+            )
+        else:
+            blob = NSKeyedArchiver.archivedDataWithRootObject_(data)
+            err = None
         self.assertIs(err, None)
         self.assertIsInstance(blob, NSData)
 
         copy = NSKeyedUnarchiver.unarchiveObjectWithData_(blob)
         self.assertIsInstance(copy, self.bytes_class)
         self.assertEqual(copy, data)
 
@@ -199,15 +209,17 @@
         def raise_exception(coder, value):
             raise RuntimeError("Cannot encode")
 
         with pyobjc_options(_nscoding_encoder=raise_exception):
             with self.assertRaisesRegex(RuntimeError, "Cannot encode"):
                 NSKeyedArchiver.archivedDataWithRootObject_(data)
 
+    @min_os_level("10.12")
     def test_decoding_raises(self):
+        # This is a known failure on macOS 10.11 due to behaviour of NSArchiver
         data = SomeBytes(b"world")
 
         def raise_exception(coder, value):
             raise RuntimeError("Cannot decode")
 
         with pyobjc_options(_nscoding_decoder=raise_exception):
             blob = NSKeyedArchiver.archivedDataWithRootObject_(data)
@@ -219,14 +231,15 @@
         with self.subTest(bytes):
             self.assertIs(OC_TestSet.classOf_(b""), OC_BuiltinPythonData)
         with self.subTest(bytearray):
             self.assertIs(OC_TestSet.classOf_(bytearray()), OC_BuiltinPythonData)
         with self.subTest(SomeBytes):
             self.assertIs(OC_TestSet.classOf_(SomeBytes()), OC_PythonData)
 
+    @min_os_level("10.13")
     def test_secure_coding(self):
         for cls in (bytes, bytearray):
             with self.subTest(cls):
                 data = cls(b"hello")
                 (
                     blob,
                     err,
```

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_date_proxy.py` & `pyobjc-core-9.2/PyObjCTest/test_date_proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from PyObjCTools.TestSupport import TestCase
+from PyObjCTools.TestSupport import TestCase, min_os_level
 from unittest import SkipTest
 from PyObjCTest.dateint import OC_DateInt
 from PyObjCTest.pythonset import OC_TestSet
 
 
 import datetime
 import time
@@ -132,33 +132,38 @@
         for offset in (-10, 0, 10):
             with self.subTest(offset=offset):
                 value2 = self.value + datetime.timedelta(seconds=offset)
                 v = OC_DateInt.date_equalToDate_(value2, self.value)
                 self.assertEqual(int(v), int(value2 == self.value))
 
     def test_roundtrip_through_keyedarchive(self):
-        (
-            blob,
-            err,
-        ) = NSKeyedArchiver.archivedDataWithRootObject_requiringSecureCoding_error_(
-            self.value, False, None
-        )
+        try:
+            (
+                blob,
+                err,
+            ) = NSKeyedArchiver.archivedDataWithRootObject_requiringSecureCoding_error_(
+                self.value, False, None
+            )
+        except AttributeError:
+            blob = NSKeyedArchiver.archivedDataWithRootObject_(self.value)
+            err = None
         self.assertIs(err, None)
         self.assertIsInstance(blob, NSData)
 
         copy = NSKeyedUnarchiver.unarchiveObjectWithData_(blob)
         self.assertEqual(copy, self.value)
 
     def test_roundtrip_through_archive(self):
         blob = NSArchiver.archivedDataWithRootObject_(self.value)
         self.assertIsInstance(blob, NSData)
 
         copy = NSUnarchiver.unarchiveObjectWithData_(blob)
         self.assertEqual(copy, self.value)
 
+    @min_os_level("10.13")
     def test_roundtrip_through_secure_keyedarchive(self):
         if (
             type(self.value) in (datetime.date, datetime.datetime)
             and getattr(self.value, "tzinfo", None) is None
         ):
             (
                 blob,
```

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_default_selector.py` & `pyobjc-core-9.2/PyObjCTest/test_default_selector.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_deprecations.py` & `pyobjc-core-9.2/PyObjCTest/test_deprecations.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_descriptors.py` & `pyobjc-core-9.2/PyObjCTest/test_descriptors.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_dict_interface.py` & `pyobjc-core-9.2/PyObjCTest/test_dict_interface.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_dict_property.py` & `pyobjc-core-9.2/PyObjCTest/test_dict_property.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_dict_proxy.py` & `pyobjc-core-9.2/PyObjCTest/test_dict_proxy.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_dyld.py` & `pyobjc-core-9.2/PyObjCTest/test_dyld.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_enumerator.py` & `pyobjc-core-9.2/PyObjCTest/test_enumerator.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_exceptions.py` & `pyobjc-core-9.2/PyObjCTest/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_filepointer.py` & `pyobjc-core-9.2/PyObjCTest/test_filepointer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_final.py` & `pyobjc-core-9.2/PyObjCTest/test_final.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_framework.py` & `pyobjc-core-9.2/PyObjCTest/test_framework.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_fsref.py` & `pyobjc-core-9.2/PyObjCTest/test_fsref.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_functions.py` & `pyobjc-core-9.2/PyObjCTest/test_functions.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_generic_class.py` & `pyobjc-core-9.2/PyObjCTest/test_generic_class.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_hidden_selector.py` & `pyobjc-core-9.2/PyObjCTest/test_hidden_selector.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_identity.py` & `pyobjc-core-9.2/PyObjCTest/test_identity.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_imp.py` & `pyobjc-core-9.2/PyObjCTest/test_imp.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_initialized.py` & `pyobjc-core-9.2/PyObjCTest/test_initialized.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_inspect_signatures.py` & `pyobjc-core-9.2/PyObjCTest/test_inspect_signatures.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_internals.py` & `pyobjc-core-9.2/PyObjCTest/test_internals.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_ivar.py` & `pyobjc-core-9.2/PyObjCTest/test_ivar.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_keyvalue.py` & `pyobjc-core-9.2/PyObjCTest/test_keyvalue.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_keyvalue_prop.py` & `pyobjc-core-9.2/PyObjCTest/test_keyvalue_prop.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_keyvaluecoding.py` & `pyobjc-core-9.2/PyObjCTest/test_keyvaluecoding.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_lazy_import.py` & `pyobjc-core-9.2/PyObjCTest/test_lazy_import.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_leaks.py` & `pyobjc-core-9.2/PyObjCTest/test_leaks.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_list_proxy.py` & `pyobjc-core-9.2/PyObjCTest/test_list_proxy.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_locking.py` & `pyobjc-core-9.2/PyObjCTest/test_locking.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_machsignals.py` & `pyobjc-core-9.2/PyObjCTest/test_machsignals.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_metadata.py` & `pyobjc-core-9.2/PyObjCTest/test_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_metadata_function.py` & `pyobjc-core-9.2/PyObjCTest/test_metadata_function.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_metadata_imp.py` & `pyobjc-core-9.2/PyObjCTest/test_metadata_imp.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_metadata_inheritance.py` & `pyobjc-core-9.2/PyObjCTest/test_metadata_inheritance.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_metadata_py.py` & `pyobjc-core-9.2/PyObjCTest/test_metadata_py.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_metadata_py2py.py` & `pyobjc-core-9.2/PyObjCTest/test_metadata_py2py.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_method_prototypes.py` & `pyobjc-core-9.2/PyObjCTest/test_method_prototypes.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_methodaccess.py` & `pyobjc-core-9.2/PyObjCTest/test_methodaccess.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import objc
+from objc import super
 import gc
 from .test_ivar import nilObject, NilHelper
 from PyObjCTools.TestSupport import TestCase, expectedFailure
 
 NSObject = objc.lookUpClass("NSObject")
 # _NSZombie = objc.lookUpClass('_NSZombie')
 NSProxy = objc.lookUpClass("NSProxy")
```

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_methodedits.py` & `pyobjc-core-9.2/PyObjCTest/test_methodedits.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_methodlookup.py` & `pyobjc-core-9.2/PyObjCTest/test_methodlookup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_methods.py` & `pyobjc-core-9.2/PyObjCTest/test_methods.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_methods2.py` & `pyobjc-core-9.2/PyObjCTest/test_methods2.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_methres.py` & `pyobjc-core-9.2/PyObjCTest/test_methres.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_nscoder.py` & `pyobjc-core-9.2/PyObjCTest/test_nscoder.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_nsdata.py` & `pyobjc-core-9.2/PyObjCTest/test_nsdata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_nsdate_proxy.py` & `pyobjc-core-9.2/PyObjCTest/test_nsdate_proxy.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_nsdecimal.py` & `pyobjc-core-9.2/PyObjCTest/test_nsdecimal.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_nsinvocation.py` & `pyobjc-core-9.2/PyObjCTest/test_nsinvocation.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_nsobject.py` & `pyobjc-core-9.2/PyObjCTest/test_nsobject.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_nulldelimited.py` & `pyobjc-core-9.2/PyObjCTest/test_nulldelimited.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_number_proxy.py` & `pyobjc-core-9.2/PyObjCTest/test_number_proxy.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_objc.py` & `pyobjc-core-9.2/PyObjCTest/test_objc.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_objcpointer.py` & `pyobjc-core-9.2/PyObjCTest/test_objcpointer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_object_property.py` & `pyobjc-core-9.2/PyObjCTest/test_object_property.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_object_proxy.py` & `pyobjc-core-9.2/PyObjCTest/test_object_proxy.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_opaque.py` & `pyobjc-core-9.2/PyObjCTest/test_opaque.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_options.py` & `pyobjc-core-9.2/PyObjCTest/test_options.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_outputinitializer.py` & `pyobjc-core-9.2/PyObjCTest/test_outputinitializer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_pickle.py` & `pyobjc-core-9.2/PyObjCTest/test_pickle.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_pointer_compat.py` & `pyobjc-core-9.2/PyObjCTest/test_pointer_compat.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_posing.py` & `pyobjc-core-9.2/PyObjCTest/test_posing.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_propertiesforclass.py` & `pyobjc-core-9.2/PyObjCTest/test_propertiesforclass.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_protocol.py` & `pyobjc-core-9.2/PyObjCTest/test_protocol.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 import objc
 from PyObjCTest.protocol import OC_TestProtocol
-from PyObjCTools.TestSupport import TestCase
+from PyObjCTools.TestSupport import (
+    TestCase,
+    expectedFailureIf,
+    os_release,
+    os_level_key,
+)
 
 # Most useful systems will at least have 'NSObject'.
 NSObject = objc.lookUpClass("NSObject")
 
 
 MyProto = objc.informal_protocol(
     "MyProto",
@@ -423,15 +428,17 @@
             )
 
         with self.assertRaisesRegex(
             TypeError, ".*selectors need to be a sequence of objc.selector instances"
         ):
             objc.formal_protocol("selectors", None, 42)
 
+    @expectedFailureIf(os_level_key(os_release()) < os_level_key("10.12"))
     def testMethodInfo(self):
+        # Protocol creation bug in at least 10.11
         self.assertCountEqual(
             MyProtocol.instanceMethods(),
             [
                 {"typestr": b"I@:", "required": True, "selector": b"protoMethod"},
                 {
                     "typestr": b"v@:ii",
                     "required": True,
@@ -826,15 +833,17 @@
                 None,
                 [
                     objc.selector(None, selector=b"fooMethod:", signature=b"v@:i"),
                     "hello",
                 ],
             )
 
+    @expectedFailureIf(os_level_key(os_release()) < os_level_key("10.12"))
     def testMethodInfo(self):
+        # Protocol creation bug in at least 10.11
         self.assertCountEqual(
             MyProtocol3.instanceMethods(),
             [
                 {"typestr": b"I@:", "required": True, "selector": b"protoMethod"},
                 {
                     "typestr": b"v@:ii",
                     "required": True,
```

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_protocolNamed.py` & `pyobjc-core-9.2/PyObjCTest/test_protocolNamed.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_python_method.py` & `pyobjc-core-9.2/PyObjCTest/test_python_method.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import objc
 import gc
 from PyObjCTools.TestSupport import TestCase
 
 NSObject = objc.lookUpClass("NSObject")
+NSMutableArray = objc.lookUpClass("NSMutableArray")
 
 
 class TestPythonMethod(TestCase):
     def test_usage_basic(self):
         class MyClass:
             @objc.python_method
             def my_method(self, a):
@@ -71,14 +72,23 @@
 
         o = Foo()
         self.assertEqual(o.args(1, 2), (1, 2))
 
         o = Foo()
         self.assertEqual(o.args(b=1, a=2), (2, 1))
 
+    def test_create_alias(self):
+        NSMutableArray.ocInitWithArray = objc.python_method(
+            NSMutableArray.initWithArray_
+        )
+
+        o = NSMutableArray.alloc().ocInitWithArray([1, 2])
+        self.assertIsInstance(o, NSMutableArray)
+        self.assertEqual(o, [1, 2])
+
     def test_gc(self):
         deallocated = False
 
         class Cleanup:
             def __del__(self):
                 nonlocal deallocated
                 deallocated = True
```

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_regr.py` & `pyobjc-core-9.2/PyObjCTest/test_regr.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_set_interface.py` & `pyobjc-core-9.2/PyObjCTest/test_set_interface.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_set_property.py` & `pyobjc-core-9.2/PyObjCTest/test_set_property.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_set_proxy.py` & `pyobjc-core-9.2/PyObjCTest/test_set_proxy.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_signals.py` & `pyobjc-core-9.2/PyObjCTest/test_signals.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_signatures.py` & `pyobjc-core-9.2/PyObjCTest/test_signatures.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_simd.py` & `pyobjc-core-9.2/PyObjCTest/test_simd.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_sockaddr.py` & `pyobjc-core-9.2/PyObjCTest/test_sockaddr.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_specialtypecodes_charbyte.py` & `pyobjc-core-9.2/PyObjCTest/test_specialtypecodes_charbyte.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_specialtypecodes_charint.py` & `pyobjc-core-9.2/PyObjCTest/test_specialtypecodes_charint.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_specialtypecodes_methdef.py` & `pyobjc-core-9.2/PyObjCTest/test_specialtypecodes_methdef.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_specialtypecodes_nsbool.py` & `pyobjc-core-9.2/PyObjCTest/test_specialtypecodes_nsbool.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_specialtypecodes_struct.py` & `pyobjc-core-9.2/PyObjCTest/test_specialtypecodes_struct.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_specialtypecodes_unichar.py` & `pyobjc-core-9.2/PyObjCTest/test_specialtypecodes_unichar.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_splitsig.py` & `pyobjc-core-9.2/PyObjCTest/test_splitsig.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_string_proxy.py` & `pyobjc-core-9.2/PyObjCTest/test_string_proxy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from PyObjCTools.TestSupport import TestCase, pyobjc_options
+from PyObjCTools.TestSupport import TestCase, pyobjc_options, min_os_level
 from PyObjCTest.objectint import OC_ObjectInt
 from PyObjCTest.stringint import OC_StringInt
 
 import objc
 
 NSData = objc.lookUpClass("NSData")
 NSError = objc.lookUpClass("NSError")
@@ -48,14 +48,15 @@
         blob = NSKeyedArchiver.archivedDataWithRootObject_(self.test_value)
         self.assertIsInstance(blob, NSData)
 
         copy = NSKeyedUnarchiver.unarchiveObjectWithData_(blob)
         self.assertEqual(copy, self.test_value)
         self.assertIsInstance(copy, type(self.test_value))
 
+    @min_os_level("10.13")
     def test_secure_keyedarchiving(self):
         (
             blob,
             error,
         ) = NSKeyedArchiver.archivedDataWithRootObject_requiringSecureCoding_error_(
             self.test_value, True, None
         )
@@ -114,28 +115,36 @@
         with pyobjc_options(_nscoding_encoder=failed):
             with self.assertRaisesRegex(TypeError, "Cannot encode"):
                 NSKeyedArchiver.archivedDataWithRootObject_(MyString("jojo"))
 
             # This should not fail:
             NSKeyedArchiver.archivedDataWithRootObject_("putty")
 
+        blob = NSKeyedArchiver.archivedDataWithRootObject_(MyString("jojo"))
+
+        with pyobjc_options(_nscoding_decoder=None):
+            with self.assertRaisesRegex(
+                ValueError,
+                "NSInvalidArgumentException - decoding Python objects is not supported",
+            ):
+                NSKeyedUnarchiver.unarchiveObjectWithData_(blob)
+
         with pyobjc_options(_nscoding_encoder=None):
             with self.assertRaisesRegex(
                 ValueError,
                 "NSInvalidArgumentException - encoding Python objects is not supported",
             ):
                 NSKeyedArchiver.archivedDataWithRootObject_(MyString("jojo"))
 
             # This should not fail:
             NSKeyedArchiver.archivedDataWithRootObject_("putty")
 
+    @min_os_level("10.12")
+    def test_keyedarchiving_raises(self):
+        # Known error on macOS 10.11 due to behaviour of NSCoder
+        def failed(*args, **kwds):
+            raise TypeError("Cannot encode")
+
         blob = NSKeyedArchiver.archivedDataWithRootObject_(MyString("jojo"))
         with pyobjc_options(_nscoding_decoder=failed):
             with self.assertRaisesRegex(TypeError, "Cannot encode"):
                 NSKeyedUnarchiver.unarchiveObjectWithData_(blob)
-
-        with pyobjc_options(_nscoding_decoder=None):
-            with self.assertRaisesRegex(
-                ValueError,
-                "NSInvalidArgumentException - decoding Python objects is not supported",
-            ):
-                NSKeyedUnarchiver.unarchiveObjectWithData_(blob)
```

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_structpointer.py` & `pyobjc-core-9.2/PyObjCTest/test_structpointer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_structs.py` & `pyobjc-core-9.2/PyObjCTest/test_structs.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_subclass.py` & `pyobjc-core-9.2/PyObjCTest/test_subclass.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import objc
 import sys
 import io
 import warnings
+import builtins
 from PyObjCTest.testbndl import PyObjC_TestClass3
 from PyObjCTools.TestSupport import TestCase
 from .objectint import OC_ObjectInt
+from objc import super
 
 # Most useful systems will at least have 'NSObject'.
 NSObject = objc.lookUpClass("NSObject")
 NSArray = objc.lookUpClass("NSArray")
 NSData = objc.lookUpClass("NSData")
 NSAutoreleasePool = objc.lookUpClass("NSAutoreleasePool")
 
@@ -1067,7 +1069,85 @@
         class ClassWithDirAsSelector(NSObject):
             method = objc.selector(dir, selector=b"method", signature=b"@@:")
 
         self.assertEqual(ClassWithDirAsSelector.method.signature, b"@@:")
 
         obj = ClassWithDirAsSelector.alloc().init()
         self.assertEqual(obj.method(), dir(obj))
+
+
+class TestMixin(TestCase):
+    def test_basic(self):
+        class Mixin:
+            pass
+
+        class MixinBase1(NSObject, Mixin):
+            pass
+
+        class MixinUser1(MixinBase1):
+            def method(self):
+                pass
+
+    def test_ignore_selectors_in_mix(self):
+        class Mixin:
+            def method(self):
+                return 42
+
+            method = objc.selector(method, signature=b"d@:")
+
+        class MixinBase2(NSObject, Mixin):
+            pass
+
+        class MixinUser2(MixinBase2):
+            def method(self):
+                return 1
+
+        self.assertResultHasType(MixinUser2.method, b"@")
+
+
+class TestSuperUsage(TestCase):
+    def setUp(self):
+        self.unbound = object()
+        self.globals = globals()
+        self.orig_super = self.globals.get("super", self.unbound)
+
+    def tearDown(self):
+        if self.orig_super is not self.unbound:
+            self.globals["super"] = self.orig_super
+        elif "super" in self.globals:
+            del self.globals["super"]
+
+    def test_bound_super(self):
+        self.globals["super"] = objc.super
+
+        with warnings.catch_warnings():
+            warnings.simplefilter("error", category=objc.ObjCSuperWarning)
+
+            class OC_TestSuperUsage1(NSObject):
+                def init(self):
+                    self = super().init()
+                    return self
+
+    def test_unbound_super(self):
+        if "super" in self.globals:
+            del self.globals["super"]
+
+        with warnings.catch_warnings():
+            with self.assertRaises(objc.ObjCSuperWarning):
+                warnings.simplefilter("error", category=objc.ObjCSuperWarning)
+
+                class OC_TestSuperUsage2(NSObject):
+                    def init(self):
+                        self = super().init()
+                        return self
+
+    def test_wrong_super(self):
+        self.globals["super"] = builtins.super
+
+        with warnings.catch_warnings():
+            with self.assertRaises(objc.ObjCSuperWarning):
+                warnings.simplefilter("error", category=objc.ObjCSuperWarning)
+
+                class OC_TestSuperUsage3(NSObject):
+                    def init(self):
+                        self = super().init()
+                        return self
```

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_synthesize.py` & `pyobjc-core-9.2/PyObjCTest/test_synthesize.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_testsupport.py` & `pyobjc-core-9.2/PyObjCTest/test_testsupport.py`

 * *Files 0% similar despite different names*

```diff
@@ -2270,16 +2270,17 @@
             with self.subTest(f"{idx}: _C_PTR + _C_CHR (skip check)"):
                 try:
                     func = Function(
                         idx,
                         {"type": objc._C_PTR + objc._C_CHR},
                     )
                     self._validateCallableMetadata(func, skip_simple_charptr_check=True)
-                except self.failureException:
-                    self.fail("Unexpected test failure")
+                except self.failureException as exc:
+                    if "pointer argument, but no by-ref annotation" not in str(exc):
+                        self.fail("Unexpected test failure")
 
             with self.subTest(f"{idx}: null-delimited _C_CHARPTR"):
                 with self.assertRaisesRegex(
                     self.failureException,
                     r"null-delimited 'char\*', use _C_CHAR_AS_TEXT instead",
                 ):
                     func = Function(
@@ -2316,15 +2317,18 @@
                     )
                     self._validateCallableMetadata(func)
 
             with self.subTest(f"{idx}: size arg ok (int)"):
                 try:
                     func = Function(
                         idx,
-                        {"type": objc._C_PTR + objc._C_INT, "c_array_size_in_arg": 0},
+                        {
+                            "type": objc._C_IN + objc._C_PTR + objc._C_INT,
+                            "c_array_size_in_arg": 0,
+                        },
                     )
                     self._validateCallableMetadata(func)
                 except self.failureException:
                     self.fail("Unexpected failure")
 
             with self.subTest(f"{idx}: size arg out of range (int)"):
                 with self.assertRaisesRegex(
@@ -2337,15 +2341,15 @@
                     self._validateCallableMetadata(func)
 
             with self.subTest(f"{idx}: size arg tuple ok"):
                 try:
                     func = Function(
                         idx,
                         {
-                            "type": objc._C_PTR + objc._C_INT,
+                            "type": objc._C_IN + objc._C_PTR + objc._C_INT,
                             "c_array_size_in_arg": (0, 1),
                         },
                     )
                     self._validateCallableMetadata(func)
                 except self.failureException:
                     self.fail("Unexpected failure")
 
@@ -2437,19 +2441,20 @@
                 m.NSObject = NSObject
 
                 try:
                     self.assertCallableMetadataIsSane(m, exclude_cocoa=False)
                 except self.failureException:
                     self.fail("Unexpected failure")
 
-            fn.assert_any_call(
-                NSObject.pyobjc_instanceMethods.description,
-                "NSObject",
-                skip_simple_charptr_check=True,
-            )
+            if 0:
+                fn.assert_any_call(
+                    NSObject.pyobjc_instanceMethods.description,
+                    "NSObject",
+                    skip_simple_charptr_check=True,
+                )
             fn.assert_any_call(
                 NSObject.pyobjc_classMethods.description,
                 "NSObject",
                 skip_simple_charptr_check=True,
             )
 
         with self.subTest("validate instance variables are not checked"):
```

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_transform.py` & `pyobjc-core-9.2/PyObjCTest/test_transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,14 @@
-from PyObjCTools.TestSupport import TestCase, min_python_release
+from PyObjCTools.TestSupport import (
+    TestCase,
+    min_python_release,
+    os_level_key,
+    os_release,
+    expectedFailureIf,
+)
 
 import objc
 from objc import _transform
 import types
 import inspect
 import functools
 import sys
@@ -209,27 +215,43 @@
 
 
 class TransformerHelper(NSObject):
     def hiddenMethod(self):
         return "Boo!"
 
     hiddenMethod = objc.selector(hiddenMethod, isHidden=True)
+    assert hiddenMethod.signature == b"@@:", hiddenMethod.signature
 
     def hiddenClassMethod(self):
         return "Hi there!"
 
     hiddenClassMethod = objc.selector(
         hiddenClassMethod, isHidden=True, isClassMethod=True
     )
+    assert hiddenClassMethod.signature == b"@@:", hiddenClassMethod.signature
 
 
 class TransformerHelper2(TransformerHelper):
     pass
 
 
+class Mixin:
+    def method1(self):
+        return 1
+
+    def method2(self):
+        return 1
+
+    method2 = objc.selector(method2, signature=b"d@:")
+
+
+class TransformerHelperWithMixin(NSObject, Mixin):
+    pass
+
+
 class TestTransformer(TestCase):
     transformer = staticmethod(_transform.transformAttribute)
 
     def assertSignaturesEqual(self, a, b):
         # This assertion ignores numeric junk in signatures, currently
         # only present with the C implementation for transformer.
         self.assertEqual(
@@ -1010,15 +1032,17 @@
                 octransformreturningshort_,
                 NSObject,
                 [],
             )
             self.assertIsInstance(out, objc.selector)
             self.assertSignaturesEqual(out.signature, b"s@:@f")
 
+    @expectedFailureIf(os_level_key(os_release()) < os_level_key("10.12"))
     def test_protocol_method(self):
+        # Protocol creation bug in at least 10.11
         with self.subTest("ObjC protocol, instance method match"):
 
             def method1(self):
                 return 4
 
             out = self.transformer("method1", method1, NSObject, [OC_TestProtocol])
             self.assertIsInstance(out, objc.selector)
@@ -1145,21 +1169,25 @@
     def test_inherit_hidden_method(self):
         # First check that the method is actually hidden:
         o = TransformerHelper.new()
         with self.assertRaisesRegex(AttributeError, "hiddenMethod"):
             o.hiddenMethod()
 
         self.assertEqual(o.pyobjc_instanceMethods.hiddenMethod(), "Boo!")
+        self.assertEqual(o.pyobjc_instanceMethods.hiddenMethod.signature, b"@@:")
 
         with self.assertRaisesRegex(AttributeError, "hiddenClassMethod"):
             TransformerHelper.hiddenClassMethod()
 
         self.assertEqual(
             TransformerHelper.pyobjc_classMethods.hiddenClassMethod(), "Hi there!"
         )
+        self.assertEqual(
+            TransformerHelper.pyobjc_classMethods.hiddenClassMethod.signature, b"@@:"
+        )
 
         def hiddenMethod(self):
             return "bar"
 
         @classmethod
         def hiddenClassMethod(self):
             return "foo"
@@ -1252,14 +1280,33 @@
                 return 1
 
             with self.assertRaisesRegex(
                 TypeError, "method name is of type int, not a string"
             ):
                 self.transformer(42, doit, NSObject, [])
 
+    def test_mixin_is_ignored(self):
+        with self.subTest("regular method in mixin"):
+
+            def method1(self):
+                pass
+
+            out = self.transformer("method1", method1, TransformerHelperWithMixin, [])
+            self.assertIsInstance(out, objc.selector)
+            self.assertEqual(out.signature, b"v@:")
+
+        with self.subTest("selector in mixin"):
+
+            def method2(self):
+                pass
+
+            out = self.transformer("method2", method2, TransformerHelperWithMixin, [])
+            self.assertIsInstance(out, objc.selector)
+            self.assertEqual(out.signature, b"v@:")
+
 
 class OC_TransformWithoutDict(NSObject):
     __slots__ = ()
 
 
 class OC_TransformWithDict(NSObject):
     pass
@@ -2116,14 +2163,39 @@
         self.assertEqual(len(rval[2]), 1)
         self.assertEqual(rval[2][0], b"classvalue")
         self.assertEqual(len(hidden_instance_methods), 1)
         self.assertEqual(len(hidden_class_methods), 1)
         self.assertEqual(hidden_instance_methods[b"instancevalue"], None)
         self.assertEqual(hidden_class_methods[b"classvalue"], None)
 
+    def test_rename_selector(self):
+        # This is used by some code that tries to give a
+        # nicer interface to ObjC classes
+
+        class_dict = {"makeArray": objc.python_method(NSMutableArray.initWithArray_)}
+        meta_dict = {}
+        hidden_instance_methods = {}
+        hidden_class_methods = {}
+
+        rval = self.processor(
+            class_dict,
+            meta_dict,
+            NSMutableArray,
+            [],
+            hidden_instance_methods,
+            hidden_class_methods,
+        )
+
+        self.assertValidResult(rval)
+        self.assertEqual(len(rval[1]), 0)
+        self.assertEqual(len(rval[2]), 0)
+        self.assertEqual(len(hidden_instance_methods), 0)
+        self.assertEqual(len(hidden_class_methods), 0)
+        self.assertEqual(class_dict["makeArray"], NSMutableArray.initWithArray_)
+
     @min_python_release(
         "3.9"
     )  # Test doesn't work on older Python versions due to stdlib changes
     def test_class_dict_is_transformed(self):
         # This test just makes sure that the attribute transformer is actually used,
         # that way this testcase doesn't have to test the transformer indirectly.
         #
@@ -2210,7 +2282,78 @@
                 [42],
                 hidden_instance_methods,
                 hidden_class_methods,
             )
 
     # XXX: Should test validate_protocols here, but is already fully covered by
     #      tests in test_protocols.
+
+    # XXX: Add tests using mixin classes as a super-class
+
+
+class TestUtilities(TestCase):
+    def test_returns_value(self):
+        with self.subTest("function returns constant value"):
+
+            def func():
+                return 1
+
+            self.assertTrue(_transform.returns_value(func))
+
+        with self.subTest("function returns value"):
+
+            def func():
+                return x**3  # noqa: F821
+
+            self.assertTrue(_transform.returns_value(func))
+
+        with self.subTest("function returns value in multiple paths"):
+
+            def func():
+                if not x:  # noqa: F821
+                    return None
+                else:
+                    return 42 / x  # noqa: F821
+
+            self.assertTrue(_transform.returns_value(func))
+
+        with self.subTest("function returns in multiple paths"):
+
+            def func():
+                if not x:  # noqa: F821
+                    return
+                else:
+                    return 42 / x  # noqa: F821
+
+            self.assertTrue(_transform.returns_value(func))
+
+        with self.subTest("function returns value in nesting"):
+
+            def func():
+                if x == 1:  # noqa: F821
+                    return 1
+
+            self.assertTrue(_transform.returns_value(func))
+
+        with self.subTest("function returns no value"):
+
+            def func():
+                return
+
+            self.assertFalse(_transform.returns_value(func))
+
+        with self.subTest("function without return"):
+
+            def func():
+                if x == 1:  # noqa: F821
+                    y = x * 2  # noqa: F821, F841
+
+            self.assertFalse(_transform.returns_value(func))
+
+    @expectedFailureIf(sys.version_info[:2] >= (3, 12))
+    def test_returns_None(self):
+        with self.subTest("function returns constant value"):
+
+            def func():
+                return None
+
+            self.assertTrue(_transform.returns_value(func))
```

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_transform_integration.py` & `pyobjc-core-9.2/PyObjCTest/test_transform_integration.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_typecheck.py` & `pyobjc-core-9.2/PyObjCTest/test_typecheck.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_unicode.py` & `pyobjc-core-9.2/PyObjCTest/test_unicode.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_usekvo.py` & `pyobjc-core-9.2/PyObjCTest/test_usekvo.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_varargs.py` & `pyobjc-core-9.2/PyObjCTest/test_varargs.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_varlist.py` & `pyobjc-core-9.2/PyObjCTest/test_varlist.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_vector_proxy.py` & `pyobjc-core-9.2/PyObjCTest/test_vector_proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from PyObjCTools.TestSupport import TestCase
+from PyObjCTools.TestSupport import TestCase, min_sdk_level
 import objc
 from objc import simd
 
 from .vector import OC_Vector
 
 CASES = [
     (simd.vector_uchar16, range(16)),
@@ -354,26 +354,28 @@
         oc = OC_Vector.alloc().init()
         result = oc.getVectorInt2()
         self.assertEqual(result, simd.vector_int2(42, 43))
 
         with self.assertRaisesRegex(TypeError, "expected no arguments, got 2"):
             oc.getVectorInt2(44, 42)
 
+    @min_sdk_level("10.12")
     def test_getGKBox(self):
         self.assertResultHasType(OC_Vector.getGKBox, GKBox.__typestr__)
         oc = OC_Vector.alloc().init()
         result = oc.getGKBox()
         self.assertEqual(
             result,
             GKBox(simd.vector_float3(1.5, 2.5, 3.5), simd.vector_float3(4.5, 5.5, 6.5)),
         )
 
         with self.assertRaisesRegex(TypeError, "expected no arguments, got 2"):
             oc.getGKBox(44, 42)
 
+    @min_sdk_level("10.12")
     def test_getGKQuad(self):
         self.assertResultHasType(OC_Vector.getGKQuad, GKQuad.__typestr__)
         oc = OC_Vector.alloc().init()
         result = oc.getGKQuad()
         self.assertEqual(
             result, GKQuad(simd.vector_float2(7.5, 8.5), simd.vector_float2(9.5, 10.5))
         )
@@ -411,14 +413,15 @@
                 simd.vector_int4(-1, -2, -3, -4), simd.vector_int4(-5, -6, -7, -8)
             ),
         )
 
         with self.assertRaisesRegex(TypeError, "expected no arguments, got 2"):
             oc.getMDLVoxelIndexExtent(44, 42)
 
+    @min_sdk_level("10.13")
     def test_getMPSAxisAlignedBoundingBox(self):
         self.assertResultHasType(
             OC_Vector.getMPSAxisAlignedBoundingBox,
             MPSAxisAlignedBoundingBox.__typestr__,
         )
         oc = OC_Vector.alloc().init()
         result = oc.getMPSAxisAlignedBoundingBox()
@@ -429,14 +432,15 @@
                 simd.vector_float3(-5.5, -6.5, -7.5),
             ),
         )
 
         with self.assertRaisesRegex(TypeError, "expected no arguments, got 2"):
             oc.getMPSAxisAlignedBoundingBox(44, 42)
 
+    @min_sdk_level("10.13")
     def test_getMPSImageHistogramInfo(self):
         self.assertResultHasType(
             OC_Vector.getMPSImageHistogramInfo, MPSImageHistogramInfo.__typestr__
         )
         oc = OC_Vector.alloc().init()
         result = oc.getMPSImageHistogramInfo()
         self.assertEqual(
@@ -529,14 +533,15 @@
                 )
             ),
         )
 
         with self.assertRaisesRegex(TypeError, "expected no arguments, got 2"):
             oc.getMatrixFloat4x4(44, 42)
 
+    @min_sdk_level("10.13")
     def test_getSimdFloat4x4(self):
         self.assertResultHasType(
             OC_Vector.getSimdFloat4x4, simd.simd_float4x4.__typestr__
         )
         oc = OC_Vector.alloc().init()
         result = oc.getSimdFloat4x4()
         self.assertEqual(
@@ -550,37 +555,38 @@
                 )
             ),
         )
 
         with self.assertRaisesRegex(TypeError, "expected no arguments, got 2"):
             oc.getSimdFloat4x4(44, 42)
 
+    @min_sdk_level("10.13")
     def test_getSimdQuatf(self):
         self.assertResultHasType(OC_Vector.getSimdQuatf, simd.simd_quatf.__typestr__)
         oc = OC_Vector.alloc().init()
         result = oc.getSimdQuatf()
         self.assertEqual(
             result, simd.simd_quatf(simd.vector_float4(-420.5, -421.5, -422.5, 0))
         )
 
         with self.assertRaisesRegex(TypeError, "expected no arguments, got 2"):
             oc.getSimdQuatf(44, 42)
 
     def test_with_unsupported_vector_type(self):
         with self.assertRaisesRegex(
-            NotImplementedError, "^Vector types not supported by libffi caller$"
+            NotImplementedError, "Cannot generate IMP for mymethodWithA:b:c:"
         ):
 
             class OC_VectorProxyUnsupportedA(objc.lookUpClass("NSObject")):
                 @objc.objc_method(signature=b"<3f>@:<4f><3f><2f>")
                 def mymethodWithA_b_c_(self, a, b, c):
                     return 1
 
         with self.assertRaisesRegex(
-            NotImplementedError, "^Vector types not supported by libffi caller$"
+            NotImplementedError, "Cannot generate IMP for mymethodWithA:b:c:"
         ):
 
             class OC_VectorProxyUnsupportedB(objc.lookUpClass("NSObject")):
                 @objc.objc_method(signature=b"<3f>@:<4f><3f><2f>", isclass=True)
                 def mymethodWithA_b_c_(self, a, b, c):
                     return 1
```

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_vectorcall.py` & `pyobjc-core-9.2/PyObjCTest/test_vectorcall.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 #
 # This file is generated using Tools/generate-helpers-vector.py
 #
 #    ** DO NOT EDIT **
 #
-from PyObjCTools.TestSupport import TestCase
+from PyObjCTools.TestSupport import TestCase, os_release, os_level_key, skipUnless
 import objc
 from functools import partial
 from objc import simd
 
 
 # Needs to be replaced by minimal definitions for
 # CGColor and CGColorSpace
-import Quartz  # noqa: F401
+try:
+    import Quartz  # noqa: F401
+except ImportError:
+    pass
 
 from .vectorcall import OC_VectorCall, OC_VectorCallInvoke
 
 
 class NoObjCClass:
     @property
     def __pyobjc_object__(self):
@@ -868,14 +871,26 @@
 objc.registerMetaDataForSelector(
     b"NSObject", b"simdquatfd:", {"full_signature": b"{_simd_quatf=<4f>}@:d"}
 )
 objc.registerMetaDataForSelector(
     b"NSObject", b"clssimdquatfd:", {"full_signature": b"{_simd_quatf=<4f>}@:d"}
 )
 
+if os_level_key(os_release()) >= os_level_key("10.12"):
+    HAVE_GK = 1
+else:
+    HAVE_GK = 0
+
+if os_level_key(os_release()) >= os_level_key("10.13"):
+    HAVE_SIMD_STRUCTS = 1
+    HAVE_MPS = 1
+else:
+    HAVE_SIMD_STRUCTS = 0
+    HAVE_MPS = 0
+
 
 class OC_VectorCallInstance(objc.lookUpClass("NSObject")):
     def v16C(self):
         self.argvalues = None
         if getattr(self, "shouldRaise", False):
             raise RuntimeError("failure!")
         return objc.simd.vector_uchar16(
@@ -1321,31 +1336,33 @@
             arg6,
             arg7,
         )
         if getattr(self, "shouldRaise", False):
             raise RuntimeError("failure!")
         return "hello"
 
-    def idid_GKBox_(self, arg0, arg1):
-        self.argvalues = (
-            arg0,
-            arg1,
-        )
-        if getattr(self, "shouldRaise", False):
-            raise RuntimeError("failure!")
-        return "hello"
+    if HAVE_GK:
 
-    def idid_GKQuad_(self, arg0, arg1):
-        self.argvalues = (
-            arg0,
-            arg1,
-        )
-        if getattr(self, "shouldRaise", False):
-            raise RuntimeError("failure!")
-        return "hello"
+        def idid_GKBox_(self, arg0, arg1):
+            self.argvalues = (
+                arg0,
+                arg1,
+            )
+            if getattr(self, "shouldRaise", False):
+                raise RuntimeError("failure!")
+            return "hello"
+
+        def idid_GKQuad_(self, arg0, arg1):
+            self.argvalues = (
+                arg0,
+                arg1,
+            )
+            if getattr(self, "shouldRaise", False):
+                raise RuntimeError("failure!")
+            return "hello"
 
     def idid_MDLAxisAlignedBoundingBox_f_(self, arg0, arg1, arg2):
         self.argvalues = (
             arg0,
             arg1,
             arg2,
         )
@@ -1486,43 +1503,45 @@
             arg2,
             arg3,
         )
         if getattr(self, "shouldRaise", False):
             raise RuntimeError("failure!")
         return "hello"
 
-    def idGKBox_(self, arg0):
-        self.argvalues = (arg0,)
-        if getattr(self, "shouldRaise", False):
-            raise RuntimeError("failure!")
-        return "hello"
-
-    def idGKBox_f_(self, arg0, arg1):
-        self.argvalues = (
-            arg0,
-            arg1,
-        )
-        if getattr(self, "shouldRaise", False):
-            raise RuntimeError("failure!")
-        return "hello"
-
-    def idGKQuad_(self, arg0):
-        self.argvalues = (arg0,)
-        if getattr(self, "shouldRaise", False):
-            raise RuntimeError("failure!")
-        return "hello"
+    if HAVE_GK:
 
-    def idGKQuad_f_(self, arg0, arg1):
-        self.argvalues = (
-            arg0,
-            arg1,
-        )
-        if getattr(self, "shouldRaise", False):
-            raise RuntimeError("failure!")
-        return "hello"
+        def idGKBox_(self, arg0):
+            self.argvalues = (arg0,)
+            if getattr(self, "shouldRaise", False):
+                raise RuntimeError("failure!")
+            return "hello"
+
+        def idGKBox_f_(self, arg0, arg1):
+            self.argvalues = (
+                arg0,
+                arg1,
+            )
+            if getattr(self, "shouldRaise", False):
+                raise RuntimeError("failure!")
+            return "hello"
+
+        def idGKQuad_(self, arg0):
+            self.argvalues = (arg0,)
+            if getattr(self, "shouldRaise", False):
+                raise RuntimeError("failure!")
+            return "hello"
+
+        def idGKQuad_f_(self, arg0, arg1):
+            self.argvalues = (
+                arg0,
+                arg1,
+            )
+            if getattr(self, "shouldRaise", False):
+                raise RuntimeError("failure!")
+            return "hello"
 
     def idMDLVoxelIndexExtent_(self, arg0):
         self.argvalues = (arg0,)
         if getattr(self, "shouldRaise", False):
             raise RuntimeError("failure!")
         return "hello"
 
@@ -1767,74 +1786,81 @@
         self.argvalues = (
             arg0,
             arg1,
         )
         if getattr(self, "shouldRaise", False):
             raise RuntimeError("failure!")
 
-    def vsimdfloat4x4_(self, arg0):
-        self.argvalues = (arg0,)
-        if getattr(self, "shouldRaise", False):
-            raise RuntimeError("failure!")
+    if HAVE_SIMD_STRUCTS:
 
-    def vsimdquatd_d_(self, arg0, arg1):
-        self.argvalues = (
-            arg0,
-            arg1,
-        )
-        if getattr(self, "shouldRaise", False):
-            raise RuntimeError("failure!")
-
-    def vsimdquatf_(self, arg0):
-        self.argvalues = (arg0,)
-        if getattr(self, "shouldRaise", False):
-            raise RuntimeError("failure!")
-
-    def vsimdquatf_v3f_(self, arg0, arg1):
-        self.argvalues = (
-            arg0,
-            arg1,
-        )
-        if getattr(self, "shouldRaise", False):
-            raise RuntimeError("failure!")
-
-    def vsimdquatf_d_(self, arg0, arg1):
-        self.argvalues = (
-            arg0,
-            arg1,
-        )
-        if getattr(self, "shouldRaise", False):
-            raise RuntimeError("failure!")
-
-    def GKBox(self):
-        self.argvalues = None
-        if getattr(self, "shouldRaise", False):
-            raise RuntimeError("failure!")
-        return (
-            objc.simd.vector_float3(1.0, 2.0, 3.0),
-            objc.simd.vector_float3(4.0, 5.0, 6.0),
-        )
+        def vsimdfloat4x4_(self, arg0):
+            self.argvalues = (arg0,)
+            if getattr(self, "shouldRaise", False):
+                raise RuntimeError("failure!")
+
+        def vsimdquatd_d_(self, arg0, arg1):
+            self.argvalues = (
+                arg0,
+                arg1,
+            )
+            if getattr(self, "shouldRaise", False):
+                raise RuntimeError("failure!")
+
+        def vsimdquatf_(self, arg0):
+            self.argvalues = (arg0,)
+            if getattr(self, "shouldRaise", False):
+                raise RuntimeError("failure!")
+
+        def vsimdquatf_v3f_(self, arg0, arg1):
+            self.argvalues = (
+                arg0,
+                arg1,
+            )
+            if getattr(self, "shouldRaise", False):
+                raise RuntimeError("failure!")
+
+        def vsimdquatf_d_(self, arg0, arg1):
+            self.argvalues = (
+                arg0,
+                arg1,
+            )
+            if getattr(self, "shouldRaise", False):
+                raise RuntimeError("failure!")
+
+    if HAVE_GK:
+
+        def GKBox(self):
+            self.argvalues = None
+            if getattr(self, "shouldRaise", False):
+                raise RuntimeError("failure!")
+            return (
+                objc.simd.vector_float3(1.0, 2.0, 3.0),
+                objc.simd.vector_float3(4.0, 5.0, 6.0),
+            )
 
-    def GKQuad(self):
-        self.argvalues = None
-        if getattr(self, "shouldRaise", False):
-            raise RuntimeError("failure!")
-        return (objc.simd.vector_float2(9.0, 10.0), objc.simd.vector_float2(11.0, 12.0))
+        def GKQuad(self):
+            self.argvalues = None
+            if getattr(self, "shouldRaise", False):
+                raise RuntimeError("failure!")
+            return (
+                objc.simd.vector_float2(9.0, 10.0),
+                objc.simd.vector_float2(11.0, 12.0),
+            )
 
-    def GKTriangleQ_(self, arg0):
-        self.argvalues = (arg0,)
-        if getattr(self, "shouldRaise", False):
-            raise RuntimeError("failure!")
-        return (
-            (
-                objc.simd.vector_float3(-18.5, -19.5, -110.5),
-                objc.simd.vector_float3(-111.5, -112.5, -113.5),
-                objc.simd.vector_float3(-17.5, 11.5, 122.5),
-            ),
-        )
+        def GKTriangleQ_(self, arg0):
+            self.argvalues = (arg0,)
+            if getattr(self, "shouldRaise", False):
+                raise RuntimeError("failure!")
+            return (
+                (
+                    objc.simd.vector_float3(-18.5, -19.5, -110.5),
+                    objc.simd.vector_float3(-111.5, -112.5, -113.5),
+                    objc.simd.vector_float3(-17.5, 11.5, 122.5),
+                ),
+            )
 
     def MDLAxisAlignedBoundingBox(self):
         self.argvalues = None
         if getattr(self, "shouldRaise", False):
             raise RuntimeError("failure!")
         return (
             objc.simd.vector_float3(-8.0, -9.0, -10.0),
@@ -1864,33 +1890,35 @@
         if getattr(self, "shouldRaise", False):
             raise RuntimeError("failure!")
         return (
             objc.simd.vector_int4(100, 101, 102, 103),
             objc.simd.vector_int4(-20, -21, -22, -23),
         )
 
-    def MPSAxisAlignedBoundingBox(self):
-        self.argvalues = None
-        if getattr(self, "shouldRaise", False):
-            raise RuntimeError("failure!")
-        return (
-            objc.simd.vector_float3(1.5, 2.5, 3.5),
-            objc.simd.vector_float3(4.5, 5.5, 6.5),
-        )
+    if HAVE_MPS:
 
-    def MPSImageHistogramInfo(self):
-        self.argvalues = None
-        if getattr(self, "shouldRaise", False):
-            raise RuntimeError("failure!")
-        return (
-            4398046511104,
-            True,
-            objc.simd.vector_float4(1.0, 2.0, 3.0, 4.0),
-            objc.simd.vector_float4(-1.0, -2.0, -3.0, -4.0),
-        )
+        def MPSAxisAlignedBoundingBox(self):
+            self.argvalues = None
+            if getattr(self, "shouldRaise", False):
+                raise RuntimeError("failure!")
+            return (
+                objc.simd.vector_float3(1.5, 2.5, 3.5),
+                objc.simd.vector_float3(4.5, 5.5, 6.5),
+            )
+
+        def MPSImageHistogramInfo(self):
+            self.argvalues = None
+            if getattr(self, "shouldRaise", False):
+                raise RuntimeError("failure!")
+            return (
+                4398046511104,
+                True,
+                objc.simd.vector_float4(1.0, 2.0, 3.0, 4.0),
+                objc.simd.vector_float4(-1.0, -2.0, -3.0, -4.0),
+            )
 
     def matrixdouble4x4(self):
         self.argvalues = None
         if getattr(self, "shouldRaise", False):
             raise RuntimeError("failure!")
         return simd.matrix_double4x4(
             (
@@ -1972,60 +2000,62 @@
                 objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
                 objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
                 objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
                 objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
             )
         )
 
-    def simdfloat4x4(self):
-        self.argvalues = None
-        if getattr(self, "shouldRaise", False):
-            raise RuntimeError("failure!")
-        return simd.simd_float4x4(
-            (
-                objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
-                objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
-                objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
-                objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
+    if HAVE_SIMD_STRUCTS:
+
+        def simdfloat4x4(self):
+            self.argvalues = None
+            if getattr(self, "shouldRaise", False):
+                raise RuntimeError("failure!")
+            return simd.simd_float4x4(
+                (
+                    objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
+                    objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
+                    objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
+                    objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
+                )
             )
-        )
 
-    def simdfloat4x4simdfloat4x4_id_(self, arg0, arg1):
-        self.argvalues = (
-            arg0,
-            arg1,
-        )
-        if getattr(self, "shouldRaise", False):
-            raise RuntimeError("failure!")
-        return simd.simd_float4x4(
-            (
-                objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
-                objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
-                objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
-                objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
+        def simdfloat4x4simdfloat4x4_id_(self, arg0, arg1):
+            self.argvalues = (
+                arg0,
+                arg1,
+            )
+            if getattr(self, "shouldRaise", False):
+                raise RuntimeError("failure!")
+            return simd.simd_float4x4(
+                (
+                    objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
+                    objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
+                    objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
+                    objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
+                )
             )
-        )
 
-    def simdquatdd_(self, arg0):
-        self.argvalues = (arg0,)
-        if getattr(self, "shouldRaise", False):
-            raise RuntimeError("failure!")
-        return simd.simd_quatd(objc.simd.vector_double4(0.0, 1.5, 3.0, 4.5))
+        def simdquatdd_(self, arg0):
+            self.argvalues = (arg0,)
+            if getattr(self, "shouldRaise", False):
+                raise RuntimeError("failure!")
+            return simd.simd_quatd(objc.simd.vector_double4(0.0, 1.5, 3.0, 4.5))
 
-    def simdquatf(self):
-        self.argvalues = None
-        if getattr(self, "shouldRaise", False):
-            raise RuntimeError("failure!")
-        return simd.simd_quatf(objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5))
+        def simdquatf(self):
+            self.argvalues = None
+            if getattr(self, "shouldRaise", False):
+                raise RuntimeError("failure!")
+            return simd.simd_quatf(objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5))
 
-    def simdquatfd_(self, arg0):
-        self.argvalues = (arg0,)
-        if getattr(self, "shouldRaise", False):
-            raise RuntimeError("failure!")
-        return simd.simd_quatf(objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5))
+        def simdquatfd_(self, arg0):
+            self.argvalues = (arg0,)
+            if getattr(self, "shouldRaise", False):
+                raise RuntimeError("failure!")
+            return simd.simd_quatf(objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5))
 
 
 class OC_VectorCallClass(objc.lookUpClass("NSObject")):
     @classmethod
     def v16C(self):
         self.argvalues = None
         if getattr(self, "shouldRaise", False):
@@ -2522,33 +2552,35 @@
             arg6,
             arg7,
         )
         if getattr(self, "shouldRaise", False):
             raise RuntimeError("failure!")
         return "hello"
 
-    @classmethod
-    def idid_GKBox_(self, arg0, arg1):
-        self.argvalues = (
-            arg0,
-            arg1,
-        )
-        if getattr(self, "shouldRaise", False):
-            raise RuntimeError("failure!")
-        return "hello"
+    if HAVE_GK:
 
-    @classmethod
-    def idid_GKQuad_(self, arg0, arg1):
-        self.argvalues = (
-            arg0,
-            arg1,
-        )
-        if getattr(self, "shouldRaise", False):
-            raise RuntimeError("failure!")
-        return "hello"
+        @classmethod
+        def idid_GKBox_(self, arg0, arg1):
+            self.argvalues = (
+                arg0,
+                arg1,
+            )
+            if getattr(self, "shouldRaise", False):
+                raise RuntimeError("failure!")
+            return "hello"
+
+        @classmethod
+        def idid_GKQuad_(self, arg0, arg1):
+            self.argvalues = (
+                arg0,
+                arg1,
+            )
+            if getattr(self, "shouldRaise", False):
+                raise RuntimeError("failure!")
+            return "hello"
 
     @classmethod
     def idid_MDLAxisAlignedBoundingBox_f_(self, arg0, arg1, arg2):
         self.argvalues = (
             arg0,
             arg1,
             arg2,
@@ -2702,47 +2734,49 @@
             arg2,
             arg3,
         )
         if getattr(self, "shouldRaise", False):
             raise RuntimeError("failure!")
         return "hello"
 
-    @classmethod
-    def idGKBox_(self, arg0):
-        self.argvalues = (arg0,)
-        if getattr(self, "shouldRaise", False):
-            raise RuntimeError("failure!")
-        return "hello"
-
-    @classmethod
-    def idGKBox_f_(self, arg0, arg1):
-        self.argvalues = (
-            arg0,
-            arg1,
-        )
-        if getattr(self, "shouldRaise", False):
-            raise RuntimeError("failure!")
-        return "hello"
-
-    @classmethod
-    def idGKQuad_(self, arg0):
-        self.argvalues = (arg0,)
-        if getattr(self, "shouldRaise", False):
-            raise RuntimeError("failure!")
-        return "hello"
+    if HAVE_GK:
 
-    @classmethod
-    def idGKQuad_f_(self, arg0, arg1):
-        self.argvalues = (
-            arg0,
-            arg1,
-        )
-        if getattr(self, "shouldRaise", False):
-            raise RuntimeError("failure!")
-        return "hello"
+        @classmethod
+        def idGKBox_(self, arg0):
+            self.argvalues = (arg0,)
+            if getattr(self, "shouldRaise", False):
+                raise RuntimeError("failure!")
+            return "hello"
+
+        @classmethod
+        def idGKBox_f_(self, arg0, arg1):
+            self.argvalues = (
+                arg0,
+                arg1,
+            )
+            if getattr(self, "shouldRaise", False):
+                raise RuntimeError("failure!")
+            return "hello"
+
+        @classmethod
+        def idGKQuad_(self, arg0):
+            self.argvalues = (arg0,)
+            if getattr(self, "shouldRaise", False):
+                raise RuntimeError("failure!")
+            return "hello"
+
+        @classmethod
+        def idGKQuad_f_(self, arg0, arg1):
+            self.argvalues = (
+                arg0,
+                arg1,
+            )
+            if getattr(self, "shouldRaise", False):
+                raise RuntimeError("failure!")
+            return "hello"
 
     @classmethod
     def idMDLVoxelIndexExtent_(self, arg0):
         self.argvalues = (arg0,)
         if getattr(self, "shouldRaise", False):
             raise RuntimeError("failure!")
         return "hello"
@@ -3021,82 +3055,89 @@
         self.argvalues = (
             arg0,
             arg1,
         )
         if getattr(self, "shouldRaise", False):
             raise RuntimeError("failure!")
 
-    @classmethod
-    def vsimdfloat4x4_(self, arg0):
-        self.argvalues = (arg0,)
-        if getattr(self, "shouldRaise", False):
-            raise RuntimeError("failure!")
+    if HAVE_SIMD_STRUCTS:
 
-    @classmethod
-    def vsimdquatd_d_(self, arg0, arg1):
-        self.argvalues = (
-            arg0,
-            arg1,
-        )
-        if getattr(self, "shouldRaise", False):
-            raise RuntimeError("failure!")
-
-    @classmethod
-    def vsimdquatf_(self, arg0):
-        self.argvalues = (arg0,)
-        if getattr(self, "shouldRaise", False):
-            raise RuntimeError("failure!")
-
-    @classmethod
-    def vsimdquatf_v3f_(self, arg0, arg1):
-        self.argvalues = (
-            arg0,
-            arg1,
-        )
-        if getattr(self, "shouldRaise", False):
-            raise RuntimeError("failure!")
-
-    @classmethod
-    def vsimdquatf_d_(self, arg0, arg1):
-        self.argvalues = (
-            arg0,
-            arg1,
-        )
-        if getattr(self, "shouldRaise", False):
-            raise RuntimeError("failure!")
-
-    @classmethod
-    def GKBox(self):
-        self.argvalues = None
-        if getattr(self, "shouldRaise", False):
-            raise RuntimeError("failure!")
-        return (
-            objc.simd.vector_float3(1.0, 2.0, 3.0),
-            objc.simd.vector_float3(4.0, 5.0, 6.0),
-        )
-
-    @classmethod
-    def GKQuad(self):
-        self.argvalues = None
-        if getattr(self, "shouldRaise", False):
-            raise RuntimeError("failure!")
-        return (objc.simd.vector_float2(9.0, 10.0), objc.simd.vector_float2(11.0, 12.0))
+        @classmethod
+        def vsimdfloat4x4_(self, arg0):
+            self.argvalues = (arg0,)
+            if getattr(self, "shouldRaise", False):
+                raise RuntimeError("failure!")
+
+        @classmethod
+        def vsimdquatd_d_(self, arg0, arg1):
+            self.argvalues = (
+                arg0,
+                arg1,
+            )
+            if getattr(self, "shouldRaise", False):
+                raise RuntimeError("failure!")
+
+        @classmethod
+        def vsimdquatf_(self, arg0):
+            self.argvalues = (arg0,)
+            if getattr(self, "shouldRaise", False):
+                raise RuntimeError("failure!")
+
+        @classmethod
+        def vsimdquatf_v3f_(self, arg0, arg1):
+            self.argvalues = (
+                arg0,
+                arg1,
+            )
+            if getattr(self, "shouldRaise", False):
+                raise RuntimeError("failure!")
+
+        @classmethod
+        def vsimdquatf_d_(self, arg0, arg1):
+            self.argvalues = (
+                arg0,
+                arg1,
+            )
+            if getattr(self, "shouldRaise", False):
+                raise RuntimeError("failure!")
+
+    if HAVE_GK:
+
+        @classmethod
+        def GKBox(self):
+            self.argvalues = None
+            if getattr(self, "shouldRaise", False):
+                raise RuntimeError("failure!")
+            return (
+                objc.simd.vector_float3(1.0, 2.0, 3.0),
+                objc.simd.vector_float3(4.0, 5.0, 6.0),
+            )
 
-    @classmethod
-    def GKTriangleQ_(self, arg0):
-        self.argvalues = (arg0,)
-        if getattr(self, "shouldRaise", False):
-            raise RuntimeError("failure!")
-        return (
-            (
-                objc.simd.vector_float3(-18.5, -19.5, -110.5),
-                objc.simd.vector_float3(-111.5, -112.5, -113.5),
-                objc.simd.vector_float3(-17.5, 11.5, 122.5),
-            ),
-        )
+        @classmethod
+        def GKQuad(self):
+            self.argvalues = None
+            if getattr(self, "shouldRaise", False):
+                raise RuntimeError("failure!")
+            return (
+                objc.simd.vector_float2(9.0, 10.0),
+                objc.simd.vector_float2(11.0, 12.0),
+            )
+
+        @classmethod
+        def GKTriangleQ_(self, arg0):
+            self.argvalues = (arg0,)
+            if getattr(self, "shouldRaise", False):
+                raise RuntimeError("failure!")
+            return (
+                (
+                    objc.simd.vector_float3(-18.5, -19.5, -110.5),
+                    objc.simd.vector_float3(-111.5, -112.5, -113.5),
+                    objc.simd.vector_float3(-17.5, 11.5, 122.5),
+                ),
+            )
 
     @classmethod
     def MDLAxisAlignedBoundingBox(self):
         self.argvalues = None
         if getattr(self, "shouldRaise", False):
             raise RuntimeError("failure!")
         return (
@@ -3130,35 +3171,37 @@
         if getattr(self, "shouldRaise", False):
             raise RuntimeError("failure!")
         return (
             objc.simd.vector_int4(100, 101, 102, 103),
             objc.simd.vector_int4(-20, -21, -22, -23),
         )
 
-    @classmethod
-    def MPSAxisAlignedBoundingBox(self):
-        self.argvalues = None
-        if getattr(self, "shouldRaise", False):
-            raise RuntimeError("failure!")
-        return (
-            objc.simd.vector_float3(1.5, 2.5, 3.5),
-            objc.simd.vector_float3(4.5, 5.5, 6.5),
-        )
+    if HAVE_MPS:
 
-    @classmethod
-    def MPSImageHistogramInfo(self):
-        self.argvalues = None
-        if getattr(self, "shouldRaise", False):
-            raise RuntimeError("failure!")
-        return (
-            4398046511104,
-            True,
-            objc.simd.vector_float4(1.0, 2.0, 3.0, 4.0),
-            objc.simd.vector_float4(-1.0, -2.0, -3.0, -4.0),
-        )
+        @classmethod
+        def MPSAxisAlignedBoundingBox(self):
+            self.argvalues = None
+            if getattr(self, "shouldRaise", False):
+                raise RuntimeError("failure!")
+            return (
+                objc.simd.vector_float3(1.5, 2.5, 3.5),
+                objc.simd.vector_float3(4.5, 5.5, 6.5),
+            )
+
+        @classmethod
+        def MPSImageHistogramInfo(self):
+            self.argvalues = None
+            if getattr(self, "shouldRaise", False):
+                raise RuntimeError("failure!")
+            return (
+                4398046511104,
+                True,
+                objc.simd.vector_float4(1.0, 2.0, 3.0, 4.0),
+                objc.simd.vector_float4(-1.0, -2.0, -3.0, -4.0),
+            )
 
     @classmethod
     def matrixdouble4x4(self):
         self.argvalues = None
         if getattr(self, "shouldRaise", False):
             raise RuntimeError("failure!")
         return simd.matrix_double4x4(
@@ -3247,65 +3290,67 @@
                 objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
                 objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
                 objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
                 objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
             )
         )
 
-    @classmethod
-    def simdfloat4x4(self):
-        self.argvalues = None
-        if getattr(self, "shouldRaise", False):
-            raise RuntimeError("failure!")
-        return simd.simd_float4x4(
-            (
-                objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
-                objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
-                objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
-                objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
+    if HAVE_SIMD_STRUCTS:
+
+        @classmethod
+        def simdfloat4x4(self):
+            self.argvalues = None
+            if getattr(self, "shouldRaise", False):
+                raise RuntimeError("failure!")
+            return simd.simd_float4x4(
+                (
+                    objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
+                    objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
+                    objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
+                    objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
+                )
             )
-        )
 
-    @classmethod
-    def simdfloat4x4simdfloat4x4_id_(self, arg0, arg1):
-        self.argvalues = (
-            arg0,
-            arg1,
-        )
-        if getattr(self, "shouldRaise", False):
-            raise RuntimeError("failure!")
-        return simd.simd_float4x4(
-            (
-                objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
-                objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
-                objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
-                objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
+        @classmethod
+        def simdfloat4x4simdfloat4x4_id_(self, arg0, arg1):
+            self.argvalues = (
+                arg0,
+                arg1,
+            )
+            if getattr(self, "shouldRaise", False):
+                raise RuntimeError("failure!")
+            return simd.simd_float4x4(
+                (
+                    objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
+                    objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
+                    objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
+                    objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
+                )
             )
-        )
 
-    @classmethod
-    def simdquatdd_(self, arg0):
-        self.argvalues = (arg0,)
-        if getattr(self, "shouldRaise", False):
-            raise RuntimeError("failure!")
-        return simd.simd_quatd(objc.simd.vector_double4(0.0, 1.5, 3.0, 4.5))
+        @classmethod
+        def simdquatdd_(self, arg0):
+            self.argvalues = (arg0,)
+            if getattr(self, "shouldRaise", False):
+                raise RuntimeError("failure!")
+            return simd.simd_quatd(objc.simd.vector_double4(0.0, 1.5, 3.0, 4.5))
 
-    @classmethod
-    def simdquatf(self):
-        self.argvalues = None
-        if getattr(self, "shouldRaise", False):
-            raise RuntimeError("failure!")
-        return simd.simd_quatf(objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5))
+        @classmethod
+        def simdquatf(self):
+            self.argvalues = None
+            if getattr(self, "shouldRaise", False):
+                raise RuntimeError("failure!")
+            return simd.simd_quatf(objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5))
 
-    @classmethod
-    def simdquatfd_(self, arg0):
-        self.argvalues = (arg0,)
-        if getattr(self, "shouldRaise", False):
-            raise RuntimeError("failure!")
-        return simd.simd_quatf(objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5))
+        @classmethod
+        def simdquatfd_(self, arg0):
+            self.argvalues = (arg0,)
+            if getattr(self, "shouldRaise", False):
+                raise RuntimeError("failure!")
+            return simd.simd_quatf(objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5))
 
 
 class TestVectorCall(TestCase):
     def __init__(self, *args, **kwds):
         super().__init__(*args, **kwds)
         self.addTypeEqualityFunc(simd.matrix_float2x2, "assertMatrixEqual")
         self.addTypeEqualityFunc(simd.matrix_float3x3, "assertMatrixEqual")
@@ -20568,14 +20613,15 @@
         value.shouldRaise = True
         try:
             with self.assertRaisesRegex(RuntimeError, "failure"):
                 OC_VectorCallInvoke.ididqv2ifffffOn_(value)
         finally:
             del value.shouldRaise
 
+    @skipUnless(HAVE_GK, "GK related test")
     def test_idid_GKBox_(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertFalse(OC_VectorCall.idid_GKBox_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.idid_GKBox_, b"@")
         self.assertArgHasType(OC_VectorCall.idid_GKBox_, 0, b"@")
@@ -20645,14 +20691,15 @@
                 "hello",
                 (
                     objc.simd.vector_float3(1.0, 2.0, 3.0),
                     objc.simd.vector_float3(4.0, 5.0, 6.0),
                 ),
             )
 
+    @skipUnless(HAVE_GK, "GK related test")
     def test_clsidid_GKBox_(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertTrue(OC_VectorCall.clsidid_GKBox_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.clsidid_GKBox_, b"@")
         self.assertArgHasType(OC_VectorCall.clsidid_GKBox_, 0, b"@")
@@ -20722,14 +20769,15 @@
                 "hello",
                 (
                     objc.simd.vector_float3(1.0, 2.0, 3.0),
                     objc.simd.vector_float3(4.0, 5.0, 6.0),
                 ),
             )
 
+    @skipUnless(HAVE_GK, "GK related test")
     def test_idid_GKBox__imp(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertFalse(OC_VectorCall.idid_GKBox_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.idid_GKBox_, b"@")
         self.assertArgHasType(OC_VectorCall.idid_GKBox_, 0, b"@")
@@ -20822,14 +20870,15 @@
                 "hello",
                 (
                     objc.simd.vector_float3(1.0, 2.0, 3.0),
                     objc.simd.vector_float3(4.0, 5.0, 6.0),
                 ),
             )
 
+    @skipUnless(HAVE_GK, "GK related test")
     def test_clsidid_GKBox__imp(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertTrue(OC_VectorCall.clsidid_GKBox_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.clsidid_GKBox_, b"@")
         self.assertArgHasType(OC_VectorCall.clsidid_GKBox_, 0, b"@")
@@ -20914,14 +20963,15 @@
                 "hello",
                 (
                     objc.simd.vector_float3(1.0, 2.0, 3.0),
                     objc.simd.vector_float3(4.0, 5.0, 6.0),
                 ),
             )
 
+    @skipUnless(HAVE_GK, "GK related test")
     def test_imp_idid_GKBox_(self):
         value = OC_VectorCallInstance.alloc().init()
         value.argvalues = 1
         result = OC_VectorCallInvoke.ididGKBoxOn_(value)
         self.assertEqual(result, "hello")
         self.assertEqual(
             value.argvalues,
@@ -20938,14 +20988,15 @@
         value.shouldRaise = True
         try:
             with self.assertRaisesRegex(RuntimeError, "failure"):
                 OC_VectorCallInvoke.ididGKBoxOn_(value)
         finally:
             del value.shouldRaise
 
+    @skipUnless(HAVE_GK, "GK related test")
     def test_imp_idid_GKBox__cls(self):
         value = OC_VectorCallClass
         value.argvalues = 1
         result = OC_VectorCallInvoke.ididGKBoxOn_(value)
         self.assertEqual(result, "hello")
         self.assertEqual(
             value.argvalues,
@@ -20962,14 +21013,15 @@
         value.shouldRaise = True
         try:
             with self.assertRaisesRegex(RuntimeError, "failure"):
                 OC_VectorCallInvoke.ididGKBoxOn_(value)
         finally:
             del value.shouldRaise
 
+    @skipUnless(HAVE_GK, "GK related test")
     def test_idid_GKQuad_(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertFalse(OC_VectorCall.idid_GKQuad_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.idid_GKQuad_, b"@")
         self.assertArgHasType(OC_VectorCall.idid_GKQuad_, 0, b"@")
@@ -21033,14 +21085,15 @@
                 "hello",
                 (
                     objc.simd.vector_float2(9.0, 10.0),
                     objc.simd.vector_float2(11.0, 12.0),
                 ),
             )
 
+    @skipUnless(HAVE_GK, "GK related test")
     def test_clsidid_GKQuad_(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertTrue(OC_VectorCall.clsidid_GKQuad_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.clsidid_GKQuad_, b"@")
         self.assertArgHasType(OC_VectorCall.clsidid_GKQuad_, 0, b"@")
@@ -21104,14 +21157,15 @@
                 "hello",
                 (
                     objc.simd.vector_float2(9.0, 10.0),
                     objc.simd.vector_float2(11.0, 12.0),
                 ),
             )
 
+    @skipUnless(HAVE_GK, "GK related test")
     def test_idid_GKQuad__imp(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertFalse(OC_VectorCall.idid_GKQuad_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.idid_GKQuad_, b"@")
         self.assertArgHasType(OC_VectorCall.idid_GKQuad_, 0, b"@")
@@ -21198,14 +21252,15 @@
                 "hello",
                 (
                     objc.simd.vector_float2(9.0, 10.0),
                     objc.simd.vector_float2(11.0, 12.0),
                 ),
             )
 
+    @skipUnless(HAVE_GK, "GK related test")
     def test_clsidid_GKQuad__imp(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertTrue(OC_VectorCall.clsidid_GKQuad_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.clsidid_GKQuad_, b"@")
         self.assertArgHasType(OC_VectorCall.clsidid_GKQuad_, 0, b"@")
@@ -21284,14 +21339,15 @@
                 "hello",
                 (
                     objc.simd.vector_float2(9.0, 10.0),
                     objc.simd.vector_float2(11.0, 12.0),
                 ),
             )
 
+    @skipUnless(HAVE_GK, "GK related test")
     def test_imp_idid_GKQuad_(self):
         value = OC_VectorCallInstance.alloc().init()
         value.argvalues = 1
         result = OC_VectorCallInvoke.ididGKQuadOn_(value)
         self.assertEqual(result, "hello")
         self.assertEqual(
             value.argvalues,
@@ -21308,14 +21364,15 @@
         value.shouldRaise = True
         try:
             with self.assertRaisesRegex(RuntimeError, "failure"):
                 OC_VectorCallInvoke.ididGKQuadOn_(value)
         finally:
             del value.shouldRaise
 
+    @skipUnless(HAVE_GK, "GK related test")
     def test_imp_idid_GKQuad__cls(self):
         value = OC_VectorCallClass
         value.argvalues = 1
         result = OC_VectorCallInvoke.ididGKQuadOn_(value)
         self.assertEqual(result, "hello")
         self.assertEqual(
             value.argvalues,
@@ -27894,14 +27951,15 @@
         value.shouldRaise = True
         try:
             with self.assertRaisesRegex(RuntimeError, "failure"):
                 OC_VectorCallInvoke.idffidv2iOn_(value)
         finally:
             del value.shouldRaise
 
+    @skipUnless(HAVE_GK, "GK related test")
     def test_idGKBox_(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertFalse(OC_VectorCall.idGKBox_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.idGKBox_, b"@")
         self.assertArgHasType(OC_VectorCall.idGKBox_, 0, b"{GKBox=<3f><3f>}")
@@ -27957,14 +28015,15 @@
             caller(
                 (
                     objc.simd.vector_float3(1.0, 2.0, 3.0),
                     objc.simd.vector_float3(4.0, 5.0, 6.0),
                 )
             )
 
+    @skipUnless(HAVE_GK, "GK related test")
     def test_clsidGKBox_(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertTrue(OC_VectorCall.clsidGKBox_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.clsidGKBox_, b"@")
         self.assertArgHasType(OC_VectorCall.clsidGKBox_, 0, b"{GKBox=<3f><3f>}")
@@ -28020,14 +28079,15 @@
             caller(
                 (
                     objc.simd.vector_float3(1.0, 2.0, 3.0),
                     objc.simd.vector_float3(4.0, 5.0, 6.0),
                 )
             )
 
+    @skipUnless(HAVE_GK, "GK related test")
     def test_idGKBox__imp(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertFalse(OC_VectorCall.idGKBox_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.idGKBox_, b"@")
         self.assertArgHasType(OC_VectorCall.idGKBox_, 0, b"{GKBox=<3f><3f>}")
@@ -28104,14 +28164,15 @@
                 NoObjCValueObject,
                 (
                     objc.simd.vector_float3(1.0, 2.0, 3.0),
                     objc.simd.vector_float3(4.0, 5.0, 6.0),
                 ),
             )
 
+    @skipUnless(HAVE_GK, "GK related test")
     def test_clsidGKBox__imp(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertTrue(OC_VectorCall.clsidGKBox_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.clsidGKBox_, b"@")
         self.assertArgHasType(OC_VectorCall.clsidGKBox_, 0, b"{GKBox=<3f><3f>}")
@@ -28181,14 +28242,15 @@
                 42,
                 (
                     objc.simd.vector_float3(1.0, 2.0, 3.0),
                     objc.simd.vector_float3(4.0, 5.0, 6.0),
                 ),
             )
 
+    @skipUnless(HAVE_GK, "GK related test")
     def test_imp_idGKBox_(self):
         value = OC_VectorCallInstance.alloc().init()
         value.argvalues = 1
         result = OC_VectorCallInvoke.idGKBoxOn_(value)
         self.assertEqual(result, "hello")
         self.assertEqual(
             value.argvalues,
@@ -28204,14 +28266,15 @@
         value.shouldRaise = True
         try:
             with self.assertRaisesRegex(RuntimeError, "failure"):
                 OC_VectorCallInvoke.idGKBoxOn_(value)
         finally:
             del value.shouldRaise
 
+    @skipUnless(HAVE_GK, "GK related test")
     def test_imp_idGKBox__cls(self):
         value = OC_VectorCallClass
         value.argvalues = 1
         result = OC_VectorCallInvoke.idGKBoxOn_(value)
         self.assertEqual(result, "hello")
         self.assertEqual(
             value.argvalues,
@@ -28227,14 +28290,15 @@
         value.shouldRaise = True
         try:
             with self.assertRaisesRegex(RuntimeError, "failure"):
                 OC_VectorCallInvoke.idGKBoxOn_(value)
         finally:
             del value.shouldRaise
 
+    @skipUnless(HAVE_GK, "GK related test")
     def test_idGKBox_f_(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertFalse(OC_VectorCall.idGKBox_f_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.idGKBox_f_, b"@")
         self.assertArgHasType(OC_VectorCall.idGKBox_f_, 0, b"{GKBox=<3f><3f>}")
@@ -28309,14 +28373,15 @@
                 (
                     objc.simd.vector_float3(1.0, 2.0, 3.0),
                     objc.simd.vector_float3(4.0, 5.0, 6.0),
                 ),
                 2500000000.0,
             )
 
+    @skipUnless(HAVE_GK, "GK related test")
     def test_clsidGKBox_f_(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertTrue(OC_VectorCall.clsidGKBox_f_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.clsidGKBox_f_, b"@")
         self.assertArgHasType(OC_VectorCall.clsidGKBox_f_, 0, b"{GKBox=<3f><3f>}")
@@ -28391,14 +28456,15 @@
                 (
                     objc.simd.vector_float3(1.0, 2.0, 3.0),
                     objc.simd.vector_float3(4.0, 5.0, 6.0),
                 ),
                 2500000000.0,
             )
 
+    @skipUnless(HAVE_GK, "GK related test")
     def test_idGKBox_f__imp(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertFalse(OC_VectorCall.idGKBox_f_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.idGKBox_f_, b"@")
         self.assertArgHasType(OC_VectorCall.idGKBox_f_, 0, b"{GKBox=<3f><3f>}")
@@ -28496,14 +28562,15 @@
                 (
                     objc.simd.vector_float3(1.0, 2.0, 3.0),
                     objc.simd.vector_float3(4.0, 5.0, 6.0),
                 ),
                 2500000000.0,
             )
 
+    @skipUnless(HAVE_GK, "GK related test")
     def test_clsidGKBox_f__imp(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertTrue(OC_VectorCall.clsidGKBox_f_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.clsidGKBox_f_, b"@")
         self.assertArgHasType(OC_VectorCall.clsidGKBox_f_, 0, b"{GKBox=<3f><3f>}")
@@ -28593,14 +28660,15 @@
                 (
                     objc.simd.vector_float3(1.0, 2.0, 3.0),
                     objc.simd.vector_float3(4.0, 5.0, 6.0),
                 ),
                 2500000000.0,
             )
 
+    @skipUnless(HAVE_GK, "GK related test")
     def test_imp_idGKBox_f_(self):
         value = OC_VectorCallInstance.alloc().init()
         value.argvalues = 1
         result = OC_VectorCallInvoke.idGKBoxfOn_(value)
         self.assertEqual(result, "hello")
         self.assertEqual(
             value.argvalues,
@@ -28617,14 +28685,15 @@
         value.shouldRaise = True
         try:
             with self.assertRaisesRegex(RuntimeError, "failure"):
                 OC_VectorCallInvoke.idGKBoxfOn_(value)
         finally:
             del value.shouldRaise
 
+    @skipUnless(HAVE_GK, "GK related test")
     def test_imp_idGKBox_f__cls(self):
         value = OC_VectorCallClass
         value.argvalues = 1
         result = OC_VectorCallInvoke.idGKBoxfOn_(value)
         self.assertEqual(result, "hello")
         self.assertEqual(
             value.argvalues,
@@ -28641,14 +28710,15 @@
         value.shouldRaise = True
         try:
             with self.assertRaisesRegex(RuntimeError, "failure"):
                 OC_VectorCallInvoke.idGKBoxfOn_(value)
         finally:
             del value.shouldRaise
 
+    @skipUnless(HAVE_GK, "GK related test")
     def test_idGKQuad_(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertFalse(OC_VectorCall.idGKQuad_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.idGKQuad_, b"@")
         self.assertArgHasType(OC_VectorCall.idGKQuad_, 0, b"{GKQuad=<2f><2f>}")
@@ -28698,14 +28768,15 @@
             caller(
                 (
                     objc.simd.vector_float2(9.0, 10.0),
                     objc.simd.vector_float2(11.0, 12.0),
                 )
             )
 
+    @skipUnless(HAVE_GK, "GK related test")
     def test_clsidGKQuad_(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertTrue(OC_VectorCall.clsidGKQuad_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.clsidGKQuad_, b"@")
         self.assertArgHasType(OC_VectorCall.clsidGKQuad_, 0, b"{GKQuad=<2f><2f>}")
@@ -28755,14 +28826,15 @@
             caller(
                 (
                     objc.simd.vector_float2(9.0, 10.0),
                     objc.simd.vector_float2(11.0, 12.0),
                 )
             )
 
+    @skipUnless(HAVE_GK, "GK related test")
     def test_idGKQuad__imp(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertFalse(OC_VectorCall.idGKQuad_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.idGKQuad_, b"@")
         self.assertArgHasType(OC_VectorCall.idGKQuad_, 0, b"{GKQuad=<2f><2f>}")
@@ -28833,14 +28905,15 @@
                 NoObjCValueObject,
                 (
                     objc.simd.vector_float2(9.0, 10.0),
                     objc.simd.vector_float2(11.0, 12.0),
                 ),
             )
 
+    @skipUnless(HAVE_GK, "GK related test")
     def test_clsidGKQuad__imp(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertTrue(OC_VectorCall.clsidGKQuad_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.clsidGKQuad_, b"@")
         self.assertArgHasType(OC_VectorCall.clsidGKQuad_, 0, b"{GKQuad=<2f><2f>}")
@@ -28904,14 +28977,15 @@
                 42,
                 (
                     objc.simd.vector_float2(9.0, 10.0),
                     objc.simd.vector_float2(11.0, 12.0),
                 ),
             )
 
+    @skipUnless(HAVE_GK, "GK related test")
     def test_imp_idGKQuad_(self):
         value = OC_VectorCallInstance.alloc().init()
         value.argvalues = 1
         result = OC_VectorCallInvoke.idGKQuadOn_(value)
         self.assertEqual(result, "hello")
         self.assertEqual(
             value.argvalues,
@@ -28927,14 +29001,15 @@
         value.shouldRaise = True
         try:
             with self.assertRaisesRegex(RuntimeError, "failure"):
                 OC_VectorCallInvoke.idGKQuadOn_(value)
         finally:
             del value.shouldRaise
 
+    @skipUnless(HAVE_GK, "GK related test")
     def test_imp_idGKQuad__cls(self):
         value = OC_VectorCallClass
         value.argvalues = 1
         result = OC_VectorCallInvoke.idGKQuadOn_(value)
         self.assertEqual(result, "hello")
         self.assertEqual(
             value.argvalues,
@@ -28950,14 +29025,15 @@
         value.shouldRaise = True
         try:
             with self.assertRaisesRegex(RuntimeError, "failure"):
                 OC_VectorCallInvoke.idGKQuadOn_(value)
         finally:
             del value.shouldRaise
 
+    @skipUnless(HAVE_GK, "GK related test")
     def test_idGKQuad_f_(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertFalse(OC_VectorCall.idGKQuad_f_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.idGKQuad_f_, b"@")
         self.assertArgHasType(OC_VectorCall.idGKQuad_f_, 0, b"{GKQuad=<2f><2f>}")
@@ -29026,14 +29102,15 @@
                 (
                     objc.simd.vector_float2(9.0, 10.0),
                     objc.simd.vector_float2(11.0, 12.0),
                 ),
                 2500000000.0,
             )
 
+    @skipUnless(HAVE_GK, "GK related test")
     def test_clsidGKQuad_f_(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertTrue(OC_VectorCall.clsidGKQuad_f_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.clsidGKQuad_f_, b"@")
         self.assertArgHasType(OC_VectorCall.clsidGKQuad_f_, 0, b"{GKQuad=<2f><2f>}")
@@ -29102,14 +29179,15 @@
                 (
                     objc.simd.vector_float2(9.0, 10.0),
                     objc.simd.vector_float2(11.0, 12.0),
                 ),
                 2500000000.0,
             )
 
+    @skipUnless(HAVE_GK, "GK related test")
     def test_idGKQuad_f__imp(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertFalse(OC_VectorCall.idGKQuad_f_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.idGKQuad_f_, b"@")
         self.assertArgHasType(OC_VectorCall.idGKQuad_f_, 0, b"{GKQuad=<2f><2f>}")
@@ -29201,14 +29279,15 @@
                 (
                     objc.simd.vector_float2(9.0, 10.0),
                     objc.simd.vector_float2(11.0, 12.0),
                 ),
                 2500000000.0,
             )
 
+    @skipUnless(HAVE_GK, "GK related test")
     def test_clsidGKQuad_f__imp(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertTrue(OC_VectorCall.clsidGKQuad_f_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.clsidGKQuad_f_, b"@")
         self.assertArgHasType(OC_VectorCall.clsidGKQuad_f_, 0, b"{GKQuad=<2f><2f>}")
@@ -29292,14 +29371,15 @@
                 (
                     objc.simd.vector_float2(9.0, 10.0),
                     objc.simd.vector_float2(11.0, 12.0),
                 ),
                 2500000000.0,
             )
 
+    @skipUnless(HAVE_GK, "GK related test")
     def test_imp_idGKQuad_f_(self):
         value = OC_VectorCallInstance.alloc().init()
         value.argvalues = 1
         result = OC_VectorCallInvoke.idGKQuadfOn_(value)
         self.assertEqual(result, "hello")
         self.assertEqual(
             value.argvalues,
@@ -29316,14 +29396,15 @@
         value.shouldRaise = True
         try:
             with self.assertRaisesRegex(RuntimeError, "failure"):
                 OC_VectorCallInvoke.idGKQuadfOn_(value)
         finally:
             del value.shouldRaise
 
+    @skipUnless(HAVE_GK, "GK related test")
     def test_imp_idGKQuad_f__cls(self):
         value = OC_VectorCallClass
         value.argvalues = 1
         result = OC_VectorCallInvoke.idGKQuadfOn_(value)
         self.assertEqual(result, "hello")
         self.assertEqual(
             value.argvalues,
@@ -40609,14 +40690,15 @@
         value.shouldRaise = True
         try:
             with self.assertRaisesRegex(RuntimeError, "failure"):
                 OC_VectorCallInvoke.vmatrixfloat4x4dOn_(value)
         finally:
             del value.shouldRaise
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_vsimdfloat4x4_(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertFalse(OC_VectorCall.vsimdfloat4x4_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.vsimdfloat4x4_, b"v")
         self.assertArgHasType(
@@ -40690,14 +40772,15 @@
                         objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
                         objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
                         objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
                     )
                 )
             )
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_clsvsimdfloat4x4_(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertTrue(OC_VectorCall.clsvsimdfloat4x4_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.clsvsimdfloat4x4_, b"v")
         self.assertArgHasType(
@@ -40771,14 +40854,15 @@
                         objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
                         objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
                         objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
                     )
                 )
             )
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_vsimdfloat4x4__imp(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertFalse(OC_VectorCall.vsimdfloat4x4_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.vsimdfloat4x4_, b"v")
         self.assertArgHasType(
@@ -40881,14 +40965,15 @@
                         objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
                         objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
                         objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
                     )
                 ),
             )
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_clsvsimdfloat4x4__imp(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertTrue(OC_VectorCall.clsvsimdfloat4x4_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.clsvsimdfloat4x4_, b"v")
         self.assertArgHasType(
@@ -40980,14 +41065,15 @@
                         objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
                         objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
                         objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
                     )
                 ),
             )
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_imp_vsimdfloat4x4_(self):
         value = OC_VectorCallInstance.alloc().init()
         value.argvalues = 1
         result = OC_VectorCallInvoke.vsimdfloat4x4On_(value)
         self.assertIs(result, None)
         self.assertEqual(
             value.argvalues,
@@ -41007,14 +41093,15 @@
         value.shouldRaise = True
         try:
             with self.assertRaisesRegex(RuntimeError, "failure"):
                 OC_VectorCallInvoke.vsimdfloat4x4On_(value)
         finally:
             del value.shouldRaise
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_imp_vsimdfloat4x4__cls(self):
         value = OC_VectorCallClass
         value.argvalues = 1
         result = OC_VectorCallInvoke.vsimdfloat4x4On_(value)
         self.assertIs(result, None)
         self.assertEqual(
             value.argvalues,
@@ -41034,14 +41121,15 @@
         value.shouldRaise = True
         try:
             with self.assertRaisesRegex(RuntimeError, "failure"):
                 OC_VectorCallInvoke.vsimdfloat4x4On_(value)
         finally:
             del value.shouldRaise
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_vsimdquatd_d_(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertFalse(OC_VectorCall.vsimdquatd_d_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.vsimdquatd_d_, b"v")
         self.assertArgHasType(OC_VectorCall.vsimdquatd_d_, 0, b"{_simd_quatd=<4d>}")
@@ -41092,14 +41180,15 @@
         OC_VectorCall.setRaise()
         with self.assertRaisesRegex(objc.error, "SimpleException"):
             caller(
                 simd.simd_quatd(objc.simd.vector_double4(0.0, 1.5, 3.0, 4.5)),
                 -557000000000.0,
             )
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_clsvsimdquatd_d_(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertTrue(OC_VectorCall.clsvsimdquatd_d_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.clsvsimdquatd_d_, b"v")
         self.assertArgHasType(OC_VectorCall.clsvsimdquatd_d_, 0, b"{_simd_quatd=<4d>}")
@@ -41150,14 +41239,15 @@
         OC_VectorCall.setRaise()
         with self.assertRaisesRegex(objc.error, "SimpleException"):
             caller(
                 simd.simd_quatd(objc.simd.vector_double4(0.0, 1.5, 3.0, 4.5)),
                 -557000000000.0,
             )
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_vsimdquatd_d__imp(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertFalse(OC_VectorCall.vsimdquatd_d_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.vsimdquatd_d_, b"v")
         self.assertArgHasType(OC_VectorCall.vsimdquatd_d_, 0, b"{_simd_quatd=<4d>}")
@@ -41225,14 +41315,15 @@
         with self.assertRaisesRegex(TypeError, "Cannot proxy"):
             imp(
                 NoObjCValueObject,
                 simd.simd_quatd(objc.simd.vector_double4(0.0, 1.5, 3.0, 4.5)),
                 -557000000000.0,
             )
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_clsvsimdquatd_d__imp(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertTrue(OC_VectorCall.clsvsimdquatd_d_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.clsvsimdquatd_d_, b"v")
         self.assertArgHasType(OC_VectorCall.clsvsimdquatd_d_, 0, b"{_simd_quatd=<4d>}")
@@ -41295,14 +41386,15 @@
         ):
             imp(
                 42,
                 simd.simd_quatd(objc.simd.vector_double4(0.0, 1.5, 3.0, 4.5)),
                 -557000000000.0,
             )
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_imp_vsimdquatd_d_(self):
         value = OC_VectorCallInstance.alloc().init()
         value.argvalues = 1
         result = OC_VectorCallInvoke.vsimdquatddOn_(value)
         self.assertIs(result, None)
         self.assertEqual(
             value.argvalues,
@@ -41316,14 +41408,15 @@
         value.shouldRaise = True
         try:
             with self.assertRaisesRegex(RuntimeError, "failure"):
                 OC_VectorCallInvoke.vsimdquatddOn_(value)
         finally:
             del value.shouldRaise
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_imp_vsimdquatd_d__cls(self):
         value = OC_VectorCallClass
         value.argvalues = 1
         result = OC_VectorCallInvoke.vsimdquatddOn_(value)
         self.assertIs(result, None)
         self.assertEqual(
             value.argvalues,
@@ -41337,14 +41430,15 @@
         value.shouldRaise = True
         try:
             with self.assertRaisesRegex(RuntimeError, "failure"):
                 OC_VectorCallInvoke.vsimdquatddOn_(value)
         finally:
             del value.shouldRaise
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_vsimdquatf_(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertFalse(OC_VectorCall.vsimdquatf_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.vsimdquatf_, b"v")
         self.assertArgHasType(OC_VectorCall.vsimdquatf_, 0, b"{_simd_quatf=<4f>}")
@@ -41382,14 +41476,15 @@
             caller(None)
 
         # Exception handling
         OC_VectorCall.setRaise()
         with self.assertRaisesRegex(objc.error, "SimpleException"):
             caller(simd.simd_quatf(objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5)))
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_clsvsimdquatf_(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertTrue(OC_VectorCall.clsvsimdquatf_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.clsvsimdquatf_, b"v")
         self.assertArgHasType(OC_VectorCall.clsvsimdquatf_, 0, b"{_simd_quatf=<4f>}")
@@ -41427,14 +41522,15 @@
             caller(None)
 
         # Exception handling
         OC_VectorCall.setRaise()
         with self.assertRaisesRegex(objc.error, "SimpleException"):
             caller(simd.simd_quatf(objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5)))
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_vsimdquatf__imp(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertFalse(OC_VectorCall.vsimdquatf_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.vsimdquatf_, b"v")
         self.assertArgHasType(OC_VectorCall.vsimdquatf_, 0, b"{_simd_quatf=<4f>}")
@@ -41484,14 +41580,15 @@
 
         with self.assertRaisesRegex(TypeError, "Cannot proxy"):
             imp(
                 NoObjCValueObject,
                 simd.simd_quatf(objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5)),
             )
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_clsvsimdquatf__imp(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertTrue(OC_VectorCall.clsvsimdquatf_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.clsvsimdquatf_, b"v")
         self.assertArgHasType(OC_VectorCall.clsvsimdquatf_, 0, b"{_simd_quatf=<4f>}")
@@ -41537,14 +41634,15 @@
 
         # Call with invalid type for self
         with self.assertRaisesRegex(
             TypeError, "Need Objective-C object or class as self"
         ):
             imp(42, simd.simd_quatf(objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5)))
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_imp_vsimdquatf_(self):
         value = OC_VectorCallInstance.alloc().init()
         value.argvalues = 1
         result = OC_VectorCallInvoke.vsimdquatfOn_(value)
         self.assertIs(result, None)
         self.assertEqual(
             value.argvalues,
@@ -41555,14 +41653,15 @@
         value.shouldRaise = True
         try:
             with self.assertRaisesRegex(RuntimeError, "failure"):
                 OC_VectorCallInvoke.vsimdquatfOn_(value)
         finally:
             del value.shouldRaise
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_imp_vsimdquatf__cls(self):
         value = OC_VectorCallClass
         value.argvalues = 1
         result = OC_VectorCallInvoke.vsimdquatfOn_(value)
         self.assertIs(result, None)
         self.assertEqual(
             value.argvalues,
@@ -41573,14 +41672,15 @@
         value.shouldRaise = True
         try:
             with self.assertRaisesRegex(RuntimeError, "failure"):
                 OC_VectorCallInvoke.vsimdquatfOn_(value)
         finally:
             del value.shouldRaise
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_vsimdquatf_v3f_(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertFalse(OC_VectorCall.vsimdquatf_v3f_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.vsimdquatf_v3f_, b"v")
         self.assertArgHasType(OC_VectorCall.vsimdquatf_v3f_, 0, b"{_simd_quatf=<4f>}")
@@ -41631,14 +41731,15 @@
         OC_VectorCall.setRaise()
         with self.assertRaisesRegex(objc.error, "SimpleException"):
             caller(
                 simd.simd_quatf(objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5)),
                 objc.simd.vector_float3(0.0, 1.5, 3.0),
             )
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_clsvsimdquatf_v3f_(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertTrue(OC_VectorCall.clsvsimdquatf_v3f_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.clsvsimdquatf_v3f_, b"v")
         self.assertArgHasType(
@@ -41691,14 +41792,15 @@
         OC_VectorCall.setRaise()
         with self.assertRaisesRegex(objc.error, "SimpleException"):
             caller(
                 simd.simd_quatf(objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5)),
                 objc.simd.vector_float3(0.0, 1.5, 3.0),
             )
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_vsimdquatf_v3f__imp(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertFalse(OC_VectorCall.vsimdquatf_v3f_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.vsimdquatf_v3f_, b"v")
         self.assertArgHasType(OC_VectorCall.vsimdquatf_v3f_, 0, b"{_simd_quatf=<4f>}")
@@ -41766,14 +41868,15 @@
         with self.assertRaisesRegex(TypeError, "Cannot proxy"):
             imp(
                 NoObjCValueObject,
                 simd.simd_quatf(objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5)),
                 objc.simd.vector_float3(0.0, 1.5, 3.0),
             )
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_clsvsimdquatf_v3f__imp(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertTrue(OC_VectorCall.clsvsimdquatf_v3f_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.clsvsimdquatf_v3f_, b"v")
         self.assertArgHasType(
@@ -41838,14 +41941,15 @@
         ):
             imp(
                 42,
                 simd.simd_quatf(objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5)),
                 objc.simd.vector_float3(0.0, 1.5, 3.0),
             )
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_imp_vsimdquatf_v3f_(self):
         value = OC_VectorCallInstance.alloc().init()
         value.argvalues = 1
         result = OC_VectorCallInvoke.vsimdquatfv3fOn_(value)
         self.assertIs(result, None)
         self.assertEqual(
             value.argvalues,
@@ -41859,14 +41963,15 @@
         value.shouldRaise = True
         try:
             with self.assertRaisesRegex(RuntimeError, "failure"):
                 OC_VectorCallInvoke.vsimdquatfv3fOn_(value)
         finally:
             del value.shouldRaise
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_imp_vsimdquatf_v3f__cls(self):
         value = OC_VectorCallClass
         value.argvalues = 1
         result = OC_VectorCallInvoke.vsimdquatfv3fOn_(value)
         self.assertIs(result, None)
         self.assertEqual(
             value.argvalues,
@@ -41880,14 +41985,15 @@
         value.shouldRaise = True
         try:
             with self.assertRaisesRegex(RuntimeError, "failure"):
                 OC_VectorCallInvoke.vsimdquatfv3fOn_(value)
         finally:
             del value.shouldRaise
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_vsimdquatf_d_(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertFalse(OC_VectorCall.vsimdquatf_d_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.vsimdquatf_d_, b"v")
         self.assertArgHasType(OC_VectorCall.vsimdquatf_d_, 0, b"{_simd_quatf=<4f>}")
@@ -41938,14 +42044,15 @@
         OC_VectorCall.setRaise()
         with self.assertRaisesRegex(objc.error, "SimpleException"):
             caller(
                 simd.simd_quatf(objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5)),
                 -557000000000.0,
             )
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_clsvsimdquatf_d_(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertTrue(OC_VectorCall.clsvsimdquatf_d_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.clsvsimdquatf_d_, b"v")
         self.assertArgHasType(OC_VectorCall.clsvsimdquatf_d_, 0, b"{_simd_quatf=<4f>}")
@@ -41996,14 +42103,15 @@
         OC_VectorCall.setRaise()
         with self.assertRaisesRegex(objc.error, "SimpleException"):
             caller(
                 simd.simd_quatf(objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5)),
                 -557000000000.0,
             )
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_vsimdquatf_d__imp(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertFalse(OC_VectorCall.vsimdquatf_d_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.vsimdquatf_d_, b"v")
         self.assertArgHasType(OC_VectorCall.vsimdquatf_d_, 0, b"{_simd_quatf=<4f>}")
@@ -42071,14 +42179,15 @@
         with self.assertRaisesRegex(TypeError, "Cannot proxy"):
             imp(
                 NoObjCValueObject,
                 simd.simd_quatf(objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5)),
                 -557000000000.0,
             )
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_clsvsimdquatf_d__imp(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertTrue(OC_VectorCall.clsvsimdquatf_d_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.clsvsimdquatf_d_, b"v")
         self.assertArgHasType(OC_VectorCall.clsvsimdquatf_d_, 0, b"{_simd_quatf=<4f>}")
@@ -42141,14 +42250,15 @@
         ):
             imp(
                 42,
                 simd.simd_quatf(objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5)),
                 -557000000000.0,
             )
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_imp_vsimdquatf_d_(self):
         value = OC_VectorCallInstance.alloc().init()
         value.argvalues = 1
         result = OC_VectorCallInvoke.vsimdquatfdOn_(value)
         self.assertIs(result, None)
         self.assertEqual(
             value.argvalues,
@@ -42162,14 +42272,15 @@
         value.shouldRaise = True
         try:
             with self.assertRaisesRegex(RuntimeError, "failure"):
                 OC_VectorCallInvoke.vsimdquatfdOn_(value)
         finally:
             del value.shouldRaise
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_imp_vsimdquatf_d__cls(self):
         value = OC_VectorCallClass
         value.argvalues = 1
         result = OC_VectorCallInvoke.vsimdquatfdOn_(value)
         self.assertIs(result, None)
         self.assertEqual(
             value.argvalues,
@@ -42183,14 +42294,15 @@
         value.shouldRaise = True
         try:
             with self.assertRaisesRegex(RuntimeError, "failure"):
                 OC_VectorCallInvoke.vsimdquatfdOn_(value)
         finally:
             del value.shouldRaise
 
+    @skipUnless(HAVE_GK, "GK related test")
     def test_GKBox(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertFalse(OC_VectorCall.GKBox.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.GKBox, b"{GKBox=<3f><3f>}")
 
@@ -42220,14 +42332,15 @@
             caller("hello")
 
         # Exception handling
         OC_VectorCall.setRaise()
         with self.assertRaisesRegex(objc.error, "SimpleException"):
             caller()
 
+    @skipUnless(HAVE_GK, "GK related test")
     def test_clsGKBox(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertTrue(OC_VectorCall.clsGKBox.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.clsGKBox, b"{GKBox=<3f><3f>}")
 
@@ -42257,14 +42370,15 @@
             caller("hello")
 
         # Exception handling
         OC_VectorCall.setRaise()
         with self.assertRaisesRegex(objc.error, "SimpleException"):
             caller()
 
+    @skipUnless(HAVE_GK, "GK related test")
     def test_GKBox_imp(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertFalse(OC_VectorCall.GKBox.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.GKBox, b"{GKBox=<3f><3f>}")
 
@@ -42307,14 +42421,15 @@
             )
 
         with self.assertRaisesRegex(TypeError, "Cannot proxy"):
             imp(
                 NoObjCValueObject,
             )
 
+    @skipUnless(HAVE_GK, "GK related test")
     def test_clsGKBox_imp(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertTrue(OC_VectorCall.clsGKBox.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.clsGKBox, b"{GKBox=<3f><3f>}")
 
@@ -42354,14 +42469,15 @@
         with self.assertRaisesRegex(
             TypeError, "Need Objective-C object or class as self"
         ):
             imp(
                 42,
             )
 
+    @skipUnless(HAVE_GK, "GK related test")
     def test_imp_GKBox(self):
         value = OC_VectorCallInstance.alloc().init()
         value.argvalues = 1
         result = OC_VectorCallInvoke.GKBoxOn_(value)
         self.assertEqual(
             result,
             (
@@ -42375,14 +42491,15 @@
         value.shouldRaise = True
         try:
             with self.assertRaisesRegex(RuntimeError, "failure"):
                 OC_VectorCallInvoke.GKBoxOn_(value)
         finally:
             del value.shouldRaise
 
+    @skipUnless(HAVE_GK, "GK related test")
     def test_imp_GKBox_cls(self):
         value = OC_VectorCallClass
         value.argvalues = 1
         result = OC_VectorCallInvoke.GKBoxOn_(value)
         self.assertEqual(
             result,
             (
@@ -42396,14 +42513,15 @@
         value.shouldRaise = True
         try:
             with self.assertRaisesRegex(RuntimeError, "failure"):
                 OC_VectorCallInvoke.GKBoxOn_(value)
         finally:
             del value.shouldRaise
 
+    @skipUnless(HAVE_GK, "GK related test")
     def test_GKQuad(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertFalse(OC_VectorCall.GKQuad.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.GKQuad, b"{GKQuad=<2f><2f>}")
 
@@ -42430,14 +42548,15 @@
             caller("hello")
 
         # Exception handling
         OC_VectorCall.setRaise()
         with self.assertRaisesRegex(objc.error, "SimpleException"):
             caller()
 
+    @skipUnless(HAVE_GK, "GK related test")
     def test_clsGKQuad(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertTrue(OC_VectorCall.clsGKQuad.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.clsGKQuad, b"{GKQuad=<2f><2f>}")
 
@@ -42464,14 +42583,15 @@
             caller("hello")
 
         # Exception handling
         OC_VectorCall.setRaise()
         with self.assertRaisesRegex(objc.error, "SimpleException"):
             caller()
 
+    @skipUnless(HAVE_GK, "GK related test")
     def test_GKQuad_imp(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertFalse(OC_VectorCall.GKQuad.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.GKQuad, b"{GKQuad=<2f><2f>}")
 
@@ -42511,14 +42631,15 @@
             )
 
         with self.assertRaisesRegex(TypeError, "Cannot proxy"):
             imp(
                 NoObjCValueObject,
             )
 
+    @skipUnless(HAVE_GK, "GK related test")
     def test_clsGKQuad_imp(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertTrue(OC_VectorCall.clsGKQuad.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.clsGKQuad, b"{GKQuad=<2f><2f>}")
 
@@ -42555,14 +42676,15 @@
         with self.assertRaisesRegex(
             TypeError, "Need Objective-C object or class as self"
         ):
             imp(
                 42,
             )
 
+    @skipUnless(HAVE_GK, "GK related test")
     def test_imp_GKQuad(self):
         value = OC_VectorCallInstance.alloc().init()
         value.argvalues = 1
         result = OC_VectorCallInvoke.GKQuadOn_(value)
         self.assertEqual(
             result,
             (objc.simd.vector_float2(9.0, 10.0), objc.simd.vector_float2(11.0, 12.0)),
@@ -42573,14 +42695,15 @@
         value.shouldRaise = True
         try:
             with self.assertRaisesRegex(RuntimeError, "failure"):
                 OC_VectorCallInvoke.GKQuadOn_(value)
         finally:
             del value.shouldRaise
 
+    @skipUnless(HAVE_GK, "GK related test")
     def test_imp_GKQuad_cls(self):
         value = OC_VectorCallClass
         value.argvalues = 1
         result = OC_VectorCallInvoke.GKQuadOn_(value)
         self.assertEqual(
             result,
             (objc.simd.vector_float2(9.0, 10.0), objc.simd.vector_float2(11.0, 12.0)),
@@ -42591,14 +42714,15 @@
         value.shouldRaise = True
         try:
             with self.assertRaisesRegex(RuntimeError, "failure"):
                 OC_VectorCallInvoke.GKQuadOn_(value)
         finally:
             del value.shouldRaise
 
+    @skipUnless(HAVE_GK, "GK related test")
     def test_GKTriangleQ_(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertFalse(OC_VectorCall.GKTriangleQ_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.GKTriangleQ_, b"{GKTriangle=[3<3f>]}")
         self.assertArgHasType(OC_VectorCall.GKTriangleQ_, 0, b"Q")
@@ -42641,14 +42765,15 @@
             caller(None)
 
         # Exception handling
         OC_VectorCall.setRaise()
         with self.assertRaisesRegex(objc.error, "SimpleException"):
             caller(35184372088832)
 
+    @skipUnless(HAVE_GK, "GK related test")
     def test_clsGKTriangleQ_(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertTrue(OC_VectorCall.clsGKTriangleQ_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.clsGKTriangleQ_, b"{GKTriangle=[3<3f>]}")
         self.assertArgHasType(OC_VectorCall.clsGKTriangleQ_, 0, b"Q")
@@ -42691,14 +42816,15 @@
             caller(None)
 
         # Exception handling
         OC_VectorCall.setRaise()
         with self.assertRaisesRegex(objc.error, "SimpleException"):
             caller(35184372088832)
 
+    @skipUnless(HAVE_GK, "GK related test")
     def test_GKTriangleQ__imp(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertFalse(OC_VectorCall.GKTriangleQ_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.GKTriangleQ_, b"{GKTriangle=[3<3f>]}")
         self.assertArgHasType(OC_VectorCall.GKTriangleQ_, 0, b"Q")
@@ -42750,14 +42876,15 @@
         # Call with invalid type for self
         with self.assertRaisesRegex(ValueError, "unrecognized selector"):
             imp(42, 35184372088832)
 
         with self.assertRaisesRegex(TypeError, "Cannot proxy"):
             imp(NoObjCValueObject, 35184372088832)
 
+    @skipUnless(HAVE_GK, "GK related test")
     def test_clsGKTriangleQ__imp(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertTrue(OC_VectorCall.clsGKTriangleQ_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.clsGKTriangleQ_, b"{GKTriangle=[3<3f>]}")
         self.assertArgHasType(OC_VectorCall.clsGKTriangleQ_, 0, b"Q")
@@ -42808,14 +42935,15 @@
 
         # Call with invalid type for self
         with self.assertRaisesRegex(
             TypeError, "Need Objective-C object or class as self"
         ):
             imp(42, 35184372088832)
 
+    @skipUnless(HAVE_GK, "GK related test")
     def test_imp_GKTriangleQ_(self):
         value = OC_VectorCallInstance.alloc().init()
         value.argvalues = 1
         result = OC_VectorCallInvoke.GKTriangleQOn_(value)
         self.assertEqual(
             result,
             (
@@ -42832,14 +42960,15 @@
         value.shouldRaise = True
         try:
             with self.assertRaisesRegex(RuntimeError, "failure"):
                 OC_VectorCallInvoke.GKTriangleQOn_(value)
         finally:
             del value.shouldRaise
 
+    @skipUnless(HAVE_GK, "GK related test")
     def test_imp_GKTriangleQ__cls(self):
         value = OC_VectorCallClass
         value.argvalues = 1
         result = OC_VectorCallInvoke.GKTriangleQOn_(value)
         self.assertEqual(
             result,
             (
@@ -43824,14 +43953,15 @@
         value.shouldRaise = True
         try:
             with self.assertRaisesRegex(RuntimeError, "failure"):
                 OC_VectorCallInvoke.MDLVoxelIndexExtentOn_(value)
         finally:
             del value.shouldRaise
 
+    @skipUnless(HAVE_MPS, "MPS not available")
     def test_MPSAxisAlignedBoundingBox(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertFalse(OC_VectorCall.MPSAxisAlignedBoundingBox.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(
             OC_VectorCall.MPSAxisAlignedBoundingBox,
@@ -43864,14 +43994,15 @@
             caller("hello")
 
         # Exception handling
         OC_VectorCall.setRaise()
         with self.assertRaisesRegex(objc.error, "SimpleException"):
             caller()
 
+    @skipUnless(HAVE_MPS, "MPS not available")
     def test_clsMPSAxisAlignedBoundingBox(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertTrue(OC_VectorCall.clsMPSAxisAlignedBoundingBox.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(
             OC_VectorCall.clsMPSAxisAlignedBoundingBox,
@@ -43904,14 +44035,15 @@
             caller("hello")
 
         # Exception handling
         OC_VectorCall.setRaise()
         with self.assertRaisesRegex(objc.error, "SimpleException"):
             caller()
 
+    @skipUnless(HAVE_MPS, "MPS not available")
     def test_MPSAxisAlignedBoundingBox_imp(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertFalse(OC_VectorCall.MPSAxisAlignedBoundingBox.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(
             OC_VectorCall.MPSAxisAlignedBoundingBox,
@@ -43957,14 +44089,15 @@
             )
 
         with self.assertRaisesRegex(TypeError, "Cannot proxy"):
             imp(
                 NoObjCValueObject,
             )
 
+    @skipUnless(HAVE_MPS, "MPS not available")
     def test_clsMPSAxisAlignedBoundingBox_imp(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertTrue(OC_VectorCall.clsMPSAxisAlignedBoundingBox.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(
             OC_VectorCall.clsMPSAxisAlignedBoundingBox,
@@ -44007,14 +44140,15 @@
         with self.assertRaisesRegex(
             TypeError, "Need Objective-C object or class as self"
         ):
             imp(
                 42,
             )
 
+    @skipUnless(HAVE_MPS, "MPS not available")
     def test_imp_MPSAxisAlignedBoundingBox(self):
         value = OC_VectorCallInstance.alloc().init()
         value.argvalues = 1
         result = OC_VectorCallInvoke.MPSAxisAlignedBoundingBoxOn_(value)
         self.assertEqual(
             result,
             (
@@ -44028,14 +44162,15 @@
         value.shouldRaise = True
         try:
             with self.assertRaisesRegex(RuntimeError, "failure"):
                 OC_VectorCallInvoke.MPSAxisAlignedBoundingBoxOn_(value)
         finally:
             del value.shouldRaise
 
+    @skipUnless(HAVE_MPS, "MPS not available")
     def test_imp_MPSAxisAlignedBoundingBox_cls(self):
         value = OC_VectorCallClass
         value.argvalues = 1
         result = OC_VectorCallInvoke.MPSAxisAlignedBoundingBoxOn_(value)
         self.assertEqual(
             result,
             (
@@ -44049,14 +44184,15 @@
         value.shouldRaise = True
         try:
             with self.assertRaisesRegex(RuntimeError, "failure"):
                 OC_VectorCallInvoke.MPSAxisAlignedBoundingBoxOn_(value)
         finally:
             del value.shouldRaise
 
+    @skipUnless(HAVE_MPS, "MPS not available")
     def test_MPSImageHistogramInfo(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertFalse(OC_VectorCall.MPSImageHistogramInfo.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(
             OC_VectorCall.MPSImageHistogramInfo, b"{_MPSImageHistogramInfo=QZ<4f><4f>}"
@@ -44090,14 +44226,15 @@
             caller("hello")
 
         # Exception handling
         OC_VectorCall.setRaise()
         with self.assertRaisesRegex(objc.error, "SimpleException"):
             caller()
 
+    @skipUnless(HAVE_MPS, "MPS not available")
     def test_clsMPSImageHistogramInfo(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertTrue(OC_VectorCall.clsMPSImageHistogramInfo.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(
             OC_VectorCall.clsMPSImageHistogramInfo,
@@ -44132,14 +44269,15 @@
             caller("hello")
 
         # Exception handling
         OC_VectorCall.setRaise()
         with self.assertRaisesRegex(objc.error, "SimpleException"):
             caller()
 
+    @skipUnless(HAVE_MPS, "MPS not available")
     def test_MPSImageHistogramInfo_imp(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertFalse(OC_VectorCall.MPSImageHistogramInfo.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(
             OC_VectorCall.MPSImageHistogramInfo, b"{_MPSImageHistogramInfo=QZ<4f><4f>}"
@@ -44186,14 +44324,15 @@
             )
 
         with self.assertRaisesRegex(TypeError, "Cannot proxy"):
             imp(
                 NoObjCValueObject,
             )
 
+    @skipUnless(HAVE_MPS, "MPS not available")
     def test_clsMPSImageHistogramInfo_imp(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertTrue(OC_VectorCall.clsMPSImageHistogramInfo.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(
             OC_VectorCall.clsMPSImageHistogramInfo,
@@ -44238,14 +44377,15 @@
         with self.assertRaisesRegex(
             TypeError, "Need Objective-C object or class as self"
         ):
             imp(
                 42,
             )
 
+    @skipUnless(HAVE_MPS, "MPS not available")
     def test_imp_MPSImageHistogramInfo(self):
         value = OC_VectorCallInstance.alloc().init()
         value.argvalues = 1
         result = OC_VectorCallInvoke.MPSImageHistogramInfoOn_(value)
         self.assertEqual(
             result,
             (
@@ -44261,14 +44401,15 @@
         value.shouldRaise = True
         try:
             with self.assertRaisesRegex(RuntimeError, "failure"):
                 OC_VectorCallInvoke.MPSImageHistogramInfoOn_(value)
         finally:
             del value.shouldRaise
 
+    @skipUnless(HAVE_MPS, "MPS not available")
     def test_imp_MPSImageHistogramInfo_cls(self):
         value = OC_VectorCallClass
         value.argvalues = 1
         result = OC_VectorCallInvoke.MPSImageHistogramInfoOn_(value)
         self.assertEqual(
             result,
             (
@@ -46097,14 +46238,15 @@
         value.shouldRaise = True
         try:
             with self.assertRaisesRegex(RuntimeError, "failure"):
                 OC_VectorCallInvoke.matrixfloat4x4dOn_(value)
         finally:
             del value.shouldRaise
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_simdfloat4x4(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertFalse(OC_VectorCall.simdfloat4x4.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(
             OC_VectorCall.simdfloat4x4, b"{_simd_float4x4=[4<4f>]}"
@@ -46140,14 +46282,15 @@
             caller("hello")
 
         # Exception handling
         OC_VectorCall.setRaise()
         with self.assertRaisesRegex(objc.error, "SimpleException"):
             caller()
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_clssimdfloat4x4(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertTrue(OC_VectorCall.clssimdfloat4x4.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(
             OC_VectorCall.clssimdfloat4x4, b"{_simd_float4x4=[4<4f>]}"
@@ -46183,14 +46326,15 @@
             caller("hello")
 
         # Exception handling
         OC_VectorCall.setRaise()
         with self.assertRaisesRegex(objc.error, "SimpleException"):
             caller()
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_simdfloat4x4_imp(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertFalse(OC_VectorCall.simdfloat4x4.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(
             OC_VectorCall.simdfloat4x4, b"{_simd_float4x4=[4<4f>]}"
@@ -46239,14 +46383,15 @@
             )
 
         with self.assertRaisesRegex(TypeError, "Cannot proxy"):
             imp(
                 NoObjCValueObject,
             )
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_clssimdfloat4x4_imp(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertTrue(OC_VectorCall.clssimdfloat4x4.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(
             OC_VectorCall.clssimdfloat4x4, b"{_simd_float4x4=[4<4f>]}"
@@ -46292,14 +46437,15 @@
         with self.assertRaisesRegex(
             TypeError, "Need Objective-C object or class as self"
         ):
             imp(
                 42,
             )
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_imp_simdfloat4x4(self):
         value = OC_VectorCallInstance.alloc().init()
         value.argvalues = 1
         result = OC_VectorCallInvoke.simdfloat4x4On_(value)
         self.assertEqual(
             result,
             simd.simd_float4x4(
@@ -46317,14 +46463,15 @@
         value.shouldRaise = True
         try:
             with self.assertRaisesRegex(RuntimeError, "failure"):
                 OC_VectorCallInvoke.simdfloat4x4On_(value)
         finally:
             del value.shouldRaise
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_imp_simdfloat4x4_cls(self):
         value = OC_VectorCallClass
         value.argvalues = 1
         result = OC_VectorCallInvoke.simdfloat4x4On_(value)
         self.assertEqual(
             result,
             simd.simd_float4x4(
@@ -46342,14 +46489,15 @@
         value.shouldRaise = True
         try:
             with self.assertRaisesRegex(RuntimeError, "failure"):
                 OC_VectorCallInvoke.simdfloat4x4On_(value)
         finally:
             del value.shouldRaise
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_simdfloat4x4simdfloat4x4_id_(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertFalse(OC_VectorCall.simdfloat4x4simdfloat4x4_id_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(
             OC_VectorCall.simdfloat4x4simdfloat4x4_id_, b"{_simd_float4x4=[4<4f>]}"
@@ -46462,14 +46610,15 @@
                         objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
                         objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
                     )
                 ),
                 "hello",
             )
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_clssimdfloat4x4simdfloat4x4_id_(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertTrue(OC_VectorCall.clssimdfloat4x4simdfloat4x4_id_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(
             OC_VectorCall.clssimdfloat4x4simdfloat4x4_id_, b"{_simd_float4x4=[4<4f>]}"
@@ -46584,14 +46733,15 @@
                         objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
                         objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
                     )
                 ),
                 "hello",
             )
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_simdfloat4x4simdfloat4x4_id__imp(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertFalse(OC_VectorCall.simdfloat4x4simdfloat4x4_id_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(
             OC_VectorCall.simdfloat4x4simdfloat4x4_id_, b"{_simd_float4x4=[4<4f>]}"
@@ -46735,14 +46885,15 @@
                         objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
                         objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
                     )
                 ),
                 "hello",
             )
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_clssimdfloat4x4simdfloat4x4_id__imp(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertTrue(OC_VectorCall.clssimdfloat4x4simdfloat4x4_id_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(
             OC_VectorCall.clssimdfloat4x4simdfloat4x4_id_, b"{_simd_float4x4=[4<4f>]}"
@@ -46876,14 +47027,15 @@
                         objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
                         objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5),
                     )
                 ),
                 "hello",
             )
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_imp_simdfloat4x4simdfloat4x4_id_(self):
         value = OC_VectorCallInstance.alloc().init()
         value.argvalues = 1
         result = OC_VectorCallInvoke.simdfloat4x4simdfloat4x4idOn_(value)
         self.assertEqual(
             result,
             simd.simd_float4x4(
@@ -46914,14 +47066,15 @@
         value.shouldRaise = True
         try:
             with self.assertRaisesRegex(RuntimeError, "failure"):
                 OC_VectorCallInvoke.simdfloat4x4simdfloat4x4idOn_(value)
         finally:
             del value.shouldRaise
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_imp_simdfloat4x4simdfloat4x4_id__cls(self):
         value = OC_VectorCallClass
         value.argvalues = 1
         result = OC_VectorCallInvoke.simdfloat4x4simdfloat4x4idOn_(value)
         self.assertEqual(
             result,
             simd.simd_float4x4(
@@ -46952,14 +47105,15 @@
         value.shouldRaise = True
         try:
             with self.assertRaisesRegex(RuntimeError, "failure"):
                 OC_VectorCallInvoke.simdfloat4x4simdfloat4x4idOn_(value)
         finally:
             del value.shouldRaise
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_simdquatdd_(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertFalse(OC_VectorCall.simdquatdd_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.simdquatdd_, b"{_simd_quatd=<4d>}")
         self.assertArgHasType(OC_VectorCall.simdquatdd_, 0, b"d")
@@ -46995,14 +47149,15 @@
             caller(None)
 
         # Exception handling
         OC_VectorCall.setRaise()
         with self.assertRaisesRegex(objc.error, "SimpleException"):
             caller(-557000000000.0)
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_clssimdquatdd_(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertTrue(OC_VectorCall.clssimdquatdd_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.clssimdquatdd_, b"{_simd_quatd=<4d>}")
         self.assertArgHasType(OC_VectorCall.clssimdquatdd_, 0, b"d")
@@ -47038,14 +47193,15 @@
             caller(None)
 
         # Exception handling
         OC_VectorCall.setRaise()
         with self.assertRaisesRegex(objc.error, "SimpleException"):
             caller(-557000000000.0)
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_simdquatdd__imp(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertFalse(OC_VectorCall.simdquatdd_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.simdquatdd_, b"{_simd_quatd=<4d>}")
         self.assertArgHasType(OC_VectorCall.simdquatdd_, 0, b"d")
@@ -47090,14 +47246,15 @@
         # Call with invalid type for self
         with self.assertRaisesRegex(ValueError, "unrecognized selector"):
             imp(42, -557000000000.0)
 
         with self.assertRaisesRegex(TypeError, "Cannot proxy"):
             imp(NoObjCValueObject, -557000000000.0)
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_clssimdquatdd__imp(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertTrue(OC_VectorCall.clssimdquatdd_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.clssimdquatdd_, b"{_simd_quatd=<4d>}")
         self.assertArgHasType(OC_VectorCall.clssimdquatdd_, 0, b"d")
@@ -47141,14 +47298,15 @@
 
         # Call with invalid type for self
         with self.assertRaisesRegex(
             TypeError, "Need Objective-C object or class as self"
         ):
             imp(42, -557000000000.0)
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_imp_simdquatdd_(self):
         value = OC_VectorCallInstance.alloc().init()
         value.argvalues = 1
         result = OC_VectorCallInvoke.simdquatddOn_(value)
         self.assertEqual(
             result, simd.simd_quatd(objc.simd.vector_double4(0.0, 1.5, 3.0, 4.5))
         )
@@ -47158,14 +47316,15 @@
         value.shouldRaise = True
         try:
             with self.assertRaisesRegex(RuntimeError, "failure"):
                 OC_VectorCallInvoke.simdquatddOn_(value)
         finally:
             del value.shouldRaise
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_imp_simdquatdd__cls(self):
         value = OC_VectorCallClass
         value.argvalues = 1
         result = OC_VectorCallInvoke.simdquatddOn_(value)
         self.assertEqual(
             result, simd.simd_quatd(objc.simd.vector_double4(0.0, 1.5, 3.0, 4.5))
         )
@@ -47175,14 +47334,15 @@
         value.shouldRaise = True
         try:
             with self.assertRaisesRegex(RuntimeError, "failure"):
                 OC_VectorCallInvoke.simdquatddOn_(value)
         finally:
             del value.shouldRaise
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_simdquatf(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertFalse(OC_VectorCall.simdquatf.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.simdquatf, b"{_simd_quatf=<4f>}")
 
@@ -47208,14 +47368,15 @@
             caller("hello")
 
         # Exception handling
         OC_VectorCall.setRaise()
         with self.assertRaisesRegex(objc.error, "SimpleException"):
             caller()
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_clssimdquatf(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertTrue(OC_VectorCall.clssimdquatf.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.clssimdquatf, b"{_simd_quatf=<4f>}")
 
@@ -47241,14 +47402,15 @@
             caller("hello")
 
         # Exception handling
         OC_VectorCall.setRaise()
         with self.assertRaisesRegex(objc.error, "SimpleException"):
             caller()
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_simdquatf_imp(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertFalse(OC_VectorCall.simdquatf.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.simdquatf, b"{_simd_quatf=<4f>}")
 
@@ -47287,14 +47449,15 @@
             )
 
         with self.assertRaisesRegex(TypeError, "Cannot proxy"):
             imp(
                 NoObjCValueObject,
             )
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_clssimdquatf_imp(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertTrue(OC_VectorCall.clssimdquatf.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.clssimdquatf, b"{_simd_quatf=<4f>}")
 
@@ -47330,14 +47493,15 @@
         with self.assertRaisesRegex(
             TypeError, "Need Objective-C object or class as self"
         ):
             imp(
                 42,
             )
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_imp_simdquatf(self):
         value = OC_VectorCallInstance.alloc().init()
         value.argvalues = 1
         result = OC_VectorCallInvoke.simdquatfOn_(value)
         self.assertEqual(
             result, simd.simd_quatf(objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5))
         )
@@ -47347,14 +47511,15 @@
         value.shouldRaise = True
         try:
             with self.assertRaisesRegex(RuntimeError, "failure"):
                 OC_VectorCallInvoke.simdquatfOn_(value)
         finally:
             del value.shouldRaise
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_imp_simdquatf_cls(self):
         value = OC_VectorCallClass
         value.argvalues = 1
         result = OC_VectorCallInvoke.simdquatfOn_(value)
         self.assertEqual(
             result, simd.simd_quatf(objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5))
         )
@@ -47364,14 +47529,15 @@
         value.shouldRaise = True
         try:
             with self.assertRaisesRegex(RuntimeError, "failure"):
                 OC_VectorCallInvoke.simdquatfOn_(value)
         finally:
             del value.shouldRaise
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_simdquatfd_(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertFalse(OC_VectorCall.simdquatfd_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.simdquatfd_, b"{_simd_quatf=<4f>}")
         self.assertArgHasType(OC_VectorCall.simdquatfd_, 0, b"d")
@@ -47407,14 +47573,15 @@
             caller(None)
 
         # Exception handling
         OC_VectorCall.setRaise()
         with self.assertRaisesRegex(objc.error, "SimpleException"):
             caller(-557000000000.0)
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_clssimdquatfd_(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertTrue(OC_VectorCall.clssimdquatfd_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.clssimdquatfd_, b"{_simd_quatf=<4f>}")
         self.assertArgHasType(OC_VectorCall.clssimdquatfd_, 0, b"d")
@@ -47450,14 +47617,15 @@
             caller(None)
 
         # Exception handling
         OC_VectorCall.setRaise()
         with self.assertRaisesRegex(objc.error, "SimpleException"):
             caller(-557000000000.0)
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_simdquatfd__imp(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertFalse(OC_VectorCall.simdquatfd_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.simdquatfd_, b"{_simd_quatf=<4f>}")
         self.assertArgHasType(OC_VectorCall.simdquatfd_, 0, b"d")
@@ -47502,14 +47670,15 @@
         # Call with invalid type for self
         with self.assertRaisesRegex(ValueError, "unrecognized selector"):
             imp(42, -557000000000.0)
 
         with self.assertRaisesRegex(TypeError, "Cannot proxy"):
             imp(NoObjCValueObject, -557000000000.0)
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_clssimdquatfd__imp(self):
         OC_VectorCall.clearRaise()
         # Verify method type
         self.assertTrue(OC_VectorCall.clssimdquatfd_.isClassMethod)
         # Check that the signature is as expected
         self.assertResultHasType(OC_VectorCall.clssimdquatfd_, b"{_simd_quatf=<4f>}")
         self.assertArgHasType(OC_VectorCall.clssimdquatfd_, 0, b"d")
@@ -47553,14 +47722,15 @@
 
         # Call with invalid type for self
         with self.assertRaisesRegex(
             TypeError, "Need Objective-C object or class as self"
         ):
             imp(42, -557000000000.0)
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_imp_simdquatfd_(self):
         value = OC_VectorCallInstance.alloc().init()
         value.argvalues = 1
         result = OC_VectorCallInvoke.simdquatfdOn_(value)
         self.assertEqual(
             result, simd.simd_quatf(objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5))
         )
@@ -47570,14 +47740,15 @@
         value.shouldRaise = True
         try:
             with self.assertRaisesRegex(RuntimeError, "failure"):
                 OC_VectorCallInvoke.simdquatfdOn_(value)
         finally:
             del value.shouldRaise
 
+    @skipUnless(HAVE_SIMD_STRUCTS, "no simd structs available")
     def test_imp_simdquatfd__cls(self):
         value = OC_VectorCallClass
         value.argvalues = 1
         result = OC_VectorCallInvoke.simdquatfdOn_(value)
         self.assertEqual(
             result, simd.simd_quatf(objc.simd.vector_float4(0.0, 1.5, 3.0, 4.5))
         )
```

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_version_support.py` & `pyobjc-core-9.2/PyObjCTest/test_version_support.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/PyObjCTest/test_weakref.py` & `pyobjc-core-9.2/PyObjCTest/test_weakref.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/README.txt` & `pyobjc-core-9.2/README.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Tools/comparebench.py` & `pyobjc-core-9.2/Tools/comparebench.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,15 +32,19 @@
     fmt = " | ".join(["{:40s}"] + ["{:16s}"] * len(results))
     print(fmt.format(*headers))
     print("+".join(["-" * 41] + ["-" * 18] * len(results)))
     for key in keys:
         base = results[0]["bench"][key]
         row = [key]
         for r in results:
-            cur = r["bench"][key]
+            try:
+                cur = r["bench"][key]
+            except KeyError as exc:
+                print(f"{key}: {exc!r}")
+                continue
             if cur == base:
                 row.append(f"{cur:.3f}")
             else:
                 row.append(f"{cur:.3f} ({((cur-base)/base)*100:+.1f}%)")
         print(fmt.format(*row))
```

### Comparing `pyobjc-core-9.1b1/Tools/gen_archive.py` & `pyobjc-core-9.2/Tools/gen_archive.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Tools/generate-helpers-vector.py` & `pyobjc-core-9.2/Tools/generate-helpers-vector.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,19 @@
 XXX: Also use this for simple basic methods '-(id)method',
      '-(void)method:arg', and '(void)method', but this also
      needs the 'imp' variants.
 
 XXX: Use subtests
 
 XXX: Use jinja2 in code generation
+
+XXX: 'simd_' to 'vector_'
+
+XXX: 'GK..' types are only available on recentisch macOS
+     versions, add guards.
 """
 
 import objc
 from objc import simd
 import typing
 import pathlib
 import Quartz  # noqa: F401
```

### Comparing `pyobjc-core-9.1b1/Tools/pyobjc_setup.py` & `pyobjc-core-9.2/Tools/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Tools/pyobjcbench.py` & `pyobjc-core-9.2/Tools/pyobjcbench.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Tools/results/pyobjcbench-7.3.txt` & `pyobjc-core-9.2/Tools/results/pyobjcbench-7.3.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Tools/results/pyobjcbench-8.0b1.txt` & `pyobjc-core-9.2/Tools/results/pyobjcbench-8.0b1.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Tools/results/pyobjcbench-8.0b2.txt` & `pyobjc-core-9.2/Tools/results/pyobjcbench-8.0b2.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Tools/runtests-with-nuitka.py` & `pyobjc-core-9.2/Tools/runtests-with-nuitka.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/Tools/runtests.py` & `pyobjc-core-9.2/Tools/runtests.py`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/diff.txt` & `pyobjc-core-9.2/diff.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/setup.cfg` & `pyobjc-core-9.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyobjc-core-9.1b1/setup.py` & `pyobjc-core-9.2/setup.py`

 * *Files identical despite different names*

