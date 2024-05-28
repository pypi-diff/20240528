# Comparing `tmp/pyobjc-framework-CoreMIDI-9.1b1.tar.gz` & `tmp/pyobjc-framework-CoreMIDI-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-CoreMIDI-9.1b1.tar", last modified: Sun Mar 26 11:20:50 2023, max compression
+gzip compressed data, was "pyobjc-framework-CoreMIDI-9.2.tar", last modified: Wed Jun  7 00:10:48 2023, max compression
```

## Comparing `pyobjc-framework-CoreMIDI-9.1b1.tar` & `pyobjc-framework-CoreMIDI-9.2.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:20:50.226813 pyobjc-framework-CoreMIDI-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:20:50.176454 pyobjc-framework-CoreMIDI-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:20:50.181437 pyobjc-framework-CoreMIDI-9.1b1/Lib/CoreMIDI/
--rw-r--r--   0 ronald     (501) staff       (20)      745 2021-07-31 13:12:15.000000 pyobjc-framework-CoreMIDI-9.1b1/Lib/CoreMIDI/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)    27492 2022-06-15 11:57:00.000000 pyobjc-framework-CoreMIDI-9.1b1/Lib/CoreMIDI/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:20:50.185456 pyobjc-framework-CoreMIDI-9.1b1/Lib/pyobjc_framework_CoreMIDI.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2094 2023-03-26 11:20:50.000000 pyobjc-framework-CoreMIDI-9.1b1/Lib/pyobjc_framework_CoreMIDI.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     1141 2023-03-26 11:20:50.000000 pyobjc-framework-CoreMIDI-9.1b1/Lib/pyobjc_framework_CoreMIDI.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:20:50.000000 pyobjc-framework-CoreMIDI-9.1b1/Lib/pyobjc_framework_CoreMIDI.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:48.000000 pyobjc-framework-CoreMIDI-9.1b1/Lib/pyobjc_framework_CoreMIDI.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:20:50.000000 pyobjc-framework-CoreMIDI-9.1b1/Lib/pyobjc_framework_CoreMIDI.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)        9 2023-03-26 11:20:50.000000 pyobjc-framework-CoreMIDI-9.1b1/Lib/pyobjc_framework_CoreMIDI.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-CoreMIDI-9.1b1/License.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2021-03-21 10:08:22.000000 pyobjc-framework-CoreMIDI-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:20:50.189160 pyobjc-framework-CoreMIDI-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)      754 2021-10-18 19:38:40.000000 pyobjc-framework-CoreMIDI-9.1b1/Modules/_CoreMIDI.m
--rw-r--r--   0 ronald     (501) staff       (20)     3124 2021-10-29 07:58:20.000000 pyobjc-framework-CoreMIDI-9.1b1/Modules/_CoreMIDI_inlines.m
--rw-r--r--   0 ronald     (501) staff       (20)      336 2021-10-18 19:38:40.000000 pyobjc-framework-CoreMIDI-9.1b1/Modules/_CoreMIDI_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-CoreMIDI-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-CoreMIDI-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     1883 2023-03-26 11:20:50.225922 pyobjc-framework-CoreMIDI-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:20:50.200834 pyobjc-framework-CoreMIDI-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       19 2021-03-21 10:08:22.000000 pyobjc-framework-CoreMIDI-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      200 2022-04-11 08:03:15.000000 pyobjc-framework-CoreMIDI-9.1b1/PyObjCTest/test_coremidi.py
--rw-r--r--   0 ronald     (501) staff       (20)      285 2022-06-15 11:57:00.000000 pyobjc-framework-CoreMIDI-9.1b1/PyObjCTest/test_midibluetoothconnection.py
--rw-r--r--   0 ronald     (501) staff       (20)     3971 2022-06-25 09:09:00.000000 pyobjc-framework-CoreMIDI-9.1b1/PyObjCTest/test_midicapabilityinquiry.py
--rw-r--r--   0 ronald     (501) staff       (20)     1225 2021-03-21 10:08:22.000000 pyobjc-framework-CoreMIDI-9.1b1/PyObjCTest/test_mididriver.py
--rw-r--r--   0 ronald     (501) staff       (20)     5529 2022-01-02 11:04:26.000000 pyobjc-framework-CoreMIDI-9.1b1/PyObjCTest/test_midimessages.py
--rw-r--r--   0 ronald     (501) staff       (20)     1297 2022-02-24 08:47:16.000000 pyobjc-framework-CoreMIDI-9.1b1/PyObjCTest/test_midinetworksession.py
--rw-r--r--   0 ronald     (501) staff       (20)     2197 2021-03-21 10:08:22.000000 pyobjc-framework-CoreMIDI-9.1b1/PyObjCTest/test_midiservices.py
--rw-r--r--   0 ronald     (501) staff       (20)     1357 2022-04-12 19:22:30.000000 pyobjc-framework-CoreMIDI-9.1b1/PyObjCTest/test_midisetup.py
--rw-r--r--   0 ronald     (501) staff       (20)     3729 2022-01-02 11:04:26.000000 pyobjc-framework-CoreMIDI-9.1b1/PyObjCTest/test_midithruconnection.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:20:50.202412 pyobjc-framework-CoreMIDI-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)    10237 2022-04-12 19:22:13.000000 pyobjc-framework-CoreMIDI-9.1b1/metadata/CoreMIDI.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       32 2021-03-21 10:08:22.000000 pyobjc-framework-CoreMIDI-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:20:50.224178 pyobjc-framework-CoreMIDI-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    84638 2021-08-04 10:01:04.000000 pyobjc-framework-CoreMIDI-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    85358 2022-02-24 08:47:16.000000 pyobjc-framework-CoreMIDI-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    89274 2022-06-15 11:57:00.000000 pyobjc-framework-CoreMIDI-9.1b1/metadata/raw/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    78517 2021-03-21 10:08:22.000000 pyobjc-framework-CoreMIDI-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    84639 2021-08-04 10:01:04.000000 pyobjc-framework-CoreMIDI-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    85359 2022-02-24 08:47:16.000000 pyobjc-framework-CoreMIDI-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    89275 2022-06-15 11:57:00.000000 pyobjc-framework-CoreMIDI-9.1b1/metadata/raw/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-CoreMIDI-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:20:50.227028 pyobjc-framework-CoreMIDI-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     1301 2023-03-25 14:20:31.000000 pyobjc-framework-CoreMIDI-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:10:48.469465 pyobjc-framework-CoreMIDI-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:10:48.418711 pyobjc-framework-CoreMIDI-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:10:48.427658 pyobjc-framework-CoreMIDI-9.2/Lib/CoreMIDI/
+-rw-r--r--   0 ronald     (501) staff       (20)      745 2021-07-31 13:12:15.000000 pyobjc-framework-CoreMIDI-9.2/Lib/CoreMIDI/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)    27455 2023-05-27 09:46:33.000000 pyobjc-framework-CoreMIDI-9.2/Lib/CoreMIDI/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:10:48.437319 pyobjc-framework-CoreMIDI-9.2/Lib/pyobjc_framework_CoreMIDI.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2092 2023-06-07 00:10:48.000000 pyobjc-framework-CoreMIDI-9.2/Lib/pyobjc_framework_CoreMIDI.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     1156 2023-06-07 00:10:48.000000 pyobjc-framework-CoreMIDI-9.2/Lib/pyobjc_framework_CoreMIDI.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:10:48.000000 pyobjc-framework-CoreMIDI-9.2/Lib/pyobjc_framework_CoreMIDI.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:48.000000 pyobjc-framework-CoreMIDI-9.2/Lib/pyobjc_framework_CoreMIDI.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:10:48.000000 pyobjc-framework-CoreMIDI-9.2/Lib/pyobjc_framework_CoreMIDI.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        9 2023-06-07 00:10:48.000000 pyobjc-framework-CoreMIDI-9.2/Lib/pyobjc_framework_CoreMIDI.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-CoreMIDI-9.2/License.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2021-03-21 10:08:22.000000 pyobjc-framework-CoreMIDI-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:10:48.442053 pyobjc-framework-CoreMIDI-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)      754 2021-10-18 19:38:40.000000 pyobjc-framework-CoreMIDI-9.2/Modules/_CoreMIDI.m
+-rw-r--r--   0 ronald     (501) staff       (20)     3124 2021-10-29 07:58:20.000000 pyobjc-framework-CoreMIDI-9.2/Modules/_CoreMIDI_inlines.m
+-rw-r--r--   0 ronald     (501) staff       (20)      336 2021-10-18 19:38:40.000000 pyobjc-framework-CoreMIDI-9.2/Modules/_CoreMIDI_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:35.000000 pyobjc-framework-CoreMIDI-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-CoreMIDI-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     1881 2023-06-07 00:10:48.468987 pyobjc-framework-CoreMIDI-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:10:48.451239 pyobjc-framework-CoreMIDI-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       19 2021-03-21 10:08:22.000000 pyobjc-framework-CoreMIDI-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      200 2022-04-11 08:03:15.000000 pyobjc-framework-CoreMIDI-9.2/PyObjCTest/test_coremidi.py
+-rw-r--r--   0 ronald     (501) staff       (20)      285 2022-06-15 11:57:00.000000 pyobjc-framework-CoreMIDI-9.2/PyObjCTest/test_midibluetoothconnection.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3971 2022-06-25 09:09:00.000000 pyobjc-framework-CoreMIDI-9.2/PyObjCTest/test_midicapabilityinquiry.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1376 2023-05-27 09:46:33.000000 pyobjc-framework-CoreMIDI-9.2/PyObjCTest/test_mididriver.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5600 2023-05-27 09:46:33.000000 pyobjc-framework-CoreMIDI-9.2/PyObjCTest/test_midimessages.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1297 2022-02-24 08:47:16.000000 pyobjc-framework-CoreMIDI-9.2/PyObjCTest/test_midinetworksession.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2476 2023-05-27 09:46:33.000000 pyobjc-framework-CoreMIDI-9.2/PyObjCTest/test_midiservices.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1357 2022-04-12 19:22:30.000000 pyobjc-framework-CoreMIDI-9.2/PyObjCTest/test_midisetup.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3729 2022-01-02 11:04:26.000000 pyobjc-framework-CoreMIDI-9.2/PyObjCTest/test_midithruconnection.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:10:48.453072 pyobjc-framework-CoreMIDI-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)    10994 2023-05-27 09:46:33.000000 pyobjc-framework-CoreMIDI-9.2/metadata/CoreMIDI.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       32 2021-03-21 10:08:22.000000 pyobjc-framework-CoreMIDI-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:10:48.467753 pyobjc-framework-CoreMIDI-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    84638 2021-08-04 10:01:04.000000 pyobjc-framework-CoreMIDI-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    85358 2022-02-24 08:47:16.000000 pyobjc-framework-CoreMIDI-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    89274 2022-06-15 11:57:00.000000 pyobjc-framework-CoreMIDI-9.2/metadata/raw/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    78517 2021-03-21 10:08:22.000000 pyobjc-framework-CoreMIDI-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    84639 2021-08-04 10:01:04.000000 pyobjc-framework-CoreMIDI-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    85359 2022-02-24 08:47:16.000000 pyobjc-framework-CoreMIDI-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    89275 2022-06-15 11:57:00.000000 pyobjc-framework-CoreMIDI-9.2/metadata/raw/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-CoreMIDI-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-CoreMIDI-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:10:48.469577 pyobjc-framework-CoreMIDI-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     1372 2023-05-29 10:07:45.000000 pyobjc-framework-CoreMIDI-9.2/setup.py
```

### Comparing `pyobjc-framework-CoreMIDI-9.1b1/Lib/CoreMIDI/__init__.py` & `pyobjc-framework-CoreMIDI-9.2/Lib/CoreMIDI/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMIDI-9.1b1/Lib/CoreMIDI/_metadata.py` & `pyobjc-framework-CoreMIDI-9.2/Lib/CoreMIDI/_metadata.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is generated by objective.metadata
 #
-# Last update: Wed Jun  8 19:44:46 2022
+# Last update: Sat May 27 11:21:46 2023
 #
 # flake8: noqa
 
 import objc, sys
 from typing import NewType
 
 if sys.maxsize > 2**32:
@@ -165,24 +165,15 @@
         "MIDINetworkConnectionPolicy": NewType("MIDINetworkConnectionPolicy", int),
     }
 )
 misc.update({})
 misc.update({})
 functions = {
     "MIDIObjectSetDictionaryProperty": (b"iI^{__CFString=}^{__CFDictionary=}",),
-    "MIDIThruConnectionParamsInitialize": (
-        b"v^{MIDIThruConnectionParams=II[8{MIDIThruConnectionEndpoint=Ii}]I[8{MIDIThruConnectionEndpoint=Ii}][16C]CCCC{MIDITransform=Ss}{MIDITransform=Ss}{MIDITransform=Ss}{MIDITransform=Ss}{MIDITransform=Ss}{MIDITransform=Ss}CCCC[3C]CSS[4S]}",
-        "",
-        {"arguments": {0: {"type_modifier": "n"}}},
-    ),
-    "MIDIReceived": (b"iI^{MIDIPacketList=I[1{MIDIPacket=QS[256C]}]}",),
     "MIDI1UPSysEx": (b"{MIDIMessage_64=II}CCCCCCCCC",),
-    "MIDIGetDriverDeviceList": (
-        b"I^^{MIDIDriverInterface=^v^?^?^?^?^?^?^?^?^?^?^?^?^?}",
-    ),
     "MIDIPortDisconnectSource": (b"iII",),
     "MIDI1UPChannelVoiceMessage": (b"ICCCCC",),
     "MIDI1UPNoteOff": (b"ICCCC",),
     "MIDI1UPSystemCommon": (b"ICCCC",),
     "MIDIMessageTypeForUPWord": (b"II",),
     "MIDIObjectSetDataProperty": (b"iI^{__CFString=}^{__CFData=}",),
     "MIDISetupDispose": (b"iI",),
@@ -193,22 +184,20 @@
         {"arguments": {1: {"type_modifier": "o"}}},
     ),
     "MIDIGetSerialPortDrivers": (
         b"i^^{__CFArray=}",
         "",
         {"arguments": {0: {"already_cfretained": True, "type_modifier": "o"}}},
     ),
-    "MIDISend": (b"iII^{MIDIPacketList=I[1{MIDIPacket=QS[256C]}]}",),
     "MIDISetupRemoveDevice": (b"iI",),
-    "MIDIPacketListInit": (
-        b"^{MIDIPacket=QS[256C]}^{MIDIPacketList=I[1{MIDIPacket=QS[256C]}]}",
-    ),
     "MIDIDeviceGetNumberOfEntities": (b"QI",),
-    "MIDIEventListInit": (
-        b"^{MIDIEventPacket=QI[64I]}^{MIDIEventList=iI[1{MIDIEventPacket=QI[64I]}]}i",
+    "MIDIThruConnectionParamsInitialize": (
+        b"v^{MIDIThruConnectionParams=II[8{MIDIThruConnectionEndpoint=Ii}]I[8{MIDIThruConnectionEndpoint=Ii}][16C]CCCC{MIDITransform=Ss}{MIDITransform=Ss}{MIDITransform=Ss}{MIDITransform=Ss}{MIDITransform=Ss}{MIDITransform=Ss}CCCC[3C]CSS[4S]}",
+        "",
+        {"arguments": {0: {"type_modifier": "n"}}},
     ),
     "MIDIEntityGetNumberOfDestinations": (b"QI",),
     "MIDIGetNumberOfExternalDevices": (b"Q",),
     "MIDIDeviceNewEntity": (
         b"iI^{__CFString=}iZQQ^I",
         "",
         {"arguments": {6: {"type_modifier": "o"}}},
@@ -228,49 +217,51 @@
                         "retval": {"type": b"v"},
                         "arguments": {
                             0: {"type": b"^{MIDIPacketList=I[1{MIDIPacket=QS[256C]}]}"},
                             1: {"type": b"^v"},
                             2: {"type": b"^v"},
                         },
                     }
-                }
+                },
+                4: {"type_modifier": "o"},
             },
         },
     ),
     "MIDI2PitchBend": (b"{MIDIMessage_64=II}CCI",),
     "MIDIPortConnectSource": (b"iII^v",),
     "MIDISetupToData": (
         b"iI^^{__CFData=}",
         "",
         {"arguments": {1: {"already_cfretained": True, "type_modifier": "o"}}},
     ),
-    "MIDISendEventList": (b"iII^{MIDIEventList=iI[1{MIDIEventPacket=QI[64I]}]}",),
-    "MIDIPacketListAdd": (
-        b"^{MIDIPacket=QS[256C]}^{MIDIPacketList=I[1{MIDIPacket=QS[256C]}]}Q^{MIDIPacket=QS[256C]}QQ^C",
-    ),
+    "MIDIThruConnectionSetParams": (b"iI^{__CFData=}",),
     "MIDIObjectSetStringProperty": (b"iI^{__CFString=}^{__CFString=}",),
     "MIDI2ChannelPressure": (b"{MIDIMessage_64=II}CCI",),
-    "MIDIObjectGetDictionaryProperty": (b"iI^{__CFString=}^^{__CFDictionary=}",),
+    "MIDIEndpointSetRefCons": (b"iI^v^v",),
+    "MIDIObjectGetDictionaryProperty": (
+        b"iI^{__CFString=}^^{__CFDictionary=}",
+        "",
+        {"arguments": {2: {"type_modifier": "o"}}},
+    ),
     "MIDIFlushOutput": (b"iI",),
     "MIDIClientDispose": (b"iI",),
     "MIDI2PerNotePitchBend": (b"{MIDIMessage_64=II}CCCI",),
     "MIDI1UPNoteOn": (b"ICCCC",),
     "MIDIDeviceDispose": (b"iI",),
     "MIDIDeviceListGetDevice": (b"IIQ",),
     "MIDIBluetoothDriverDisconnect": (b"i^{__CFString=}",),
     "MIDIEntityAddOrRemoveEndpoints": (b"iIQQ",),
-    "MIDIDestinationCreateWithBlock": (
-        b"iI^{__CFString=}^I@?",
-        "",
-        {"retval": {"already_cfretained": True}},
-    ),
     "MIDIGetSource": (b"IQ",),
-    "MIDIEndpointGetEntity": (b"iI^I",),
+    "MIDIEndpointGetEntity": (b"iI^I", "", {"arguments": {1: {"type_modifier": "o"}}}),
     "MIDI2RegisteredPNC": (b"{MIDIMessage_64=II}CCCCI",),
-    "MIDIObjectGetIntegerProperty": (b"iI^{__CFString=}^i",),
+    "MIDIObjectGetIntegerProperty": (
+        b"iI^{__CFString=}^i",
+        "",
+        {"arguments": {2: {"type_modifier": "o"}}},
+    ),
     "MIDIThruConnectionParamsSize": (
         b"Q^{MIDIThruConnectionParams=II[8{MIDIThruConnectionEndpoint=Ii}]I[8{MIDIThruConnectionEndpoint=Ii}][16C]CCCC{MIDITransform=Ss}{MIDITransform=Ss}{MIDITransform=Ss}{MIDITransform=Ss}{MIDITransform=Ss}{MIDITransform=Ss}CCCC[3C]CSS[4S]}",
     ),
     "MIDIGetDestination": (b"IQ",),
     "MIDIDestinationCreate": (
         b"iI^{__CFString=}^?^v^I",
         "",
@@ -282,27 +273,40 @@
                         "retval": {"type": b"v"},
                         "arguments": {
                             0: {"type": b"^{MIDIPacketList=I[1{MIDIPacket=QS[256C]}]}"},
                             1: {"type": b"^v"},
                             2: {"type": b"^v"},
                         },
                     }
-                }
+                },
+                4: {"type_modifier": "o"},
             },
         },
     ),
     "MIDI2NoteOn": (b"{MIDIMessage_64=II}CCCCSS",),
-    "MIDIDriverEnableMonitoring": (
-        b"i^^{MIDIDriverInterface=^v^?^?^?^?^?^?^?^?^?^?^?^?^?}Z",
-    ),
     "MIDI2RelAssignableControl": (b"{MIDIMessage_64=II}CCCCI",),
-    "MIDIObjectGetProperties": (b"iI^@Z",),
+    "MIDIObjectGetProperties": (
+        b"iI^@Z",
+        "",
+        {"arguments": {1: {"type_modifier": "o"}}},
+    ),
     "MIDISetupGetCurrent": (b"i^I", "", {"arguments": {0: {"type_modifier": "o"}}}),
-    "MIDIObjectGetDataProperty": (b"iI^{__CFString=}^^{__CFData=}",),
-    "MIDISetupCreate": (b"i^I", "", {"retval": {"already_cfretained": True}}),
+    "MIDIObjectGetDataProperty": (
+        b"iI^{__CFString=}^^{__CFData=}",
+        "",
+        {"arguments": {2: {"type_modifier": "o"}}},
+    ),
+    "MIDISetupCreate": (
+        b"i^I",
+        "",
+        {
+            "retval": {"already_cfretained": True},
+            "arguments": {0: {"type_modifier": "o"}},
+        },
+    ),
     "MIDIEndpointDispose": (b"iI",),
     "MIDIExternalDeviceCreate": (
         b"i^{__CFString=}^{__CFString=}^{__CFString=}^I",
         "",
         {
             "retval": {"already_cfretained": True},
             "arguments": {3: {"type_modifier": "o"}},
@@ -319,15 +323,16 @@
                     "callable": {
                         "retval": {"type": b"v"},
                         "arguments": {
                             0: {"type": b"^{MIDINotification=iI}"},
                             1: {"type": b"^v"},
                         },
                     }
-                }
+                },
+                3: {"type_modifier": "o"},
             },
         },
     ),
     "MIDIPacketNext": (b"^{MIDIPacket=QS[256C]}^{MIDIPacket=QS[256C]}",),
     "MIDIDeviceAddEntity": (
         b"iI^{__CFString=}ZQQ^I",
         "",
@@ -339,108 +344,127 @@
         {"arguments": {1: {"type_modifier": "o"}}},
     ),
     "MIDIThruConnectionDispose": (b"iI",),
     "MIDISetupInstall": (b"iI",),
     "MIDIDestinationCreateWithProtocol": (
         b"iI^{__CFString=}i^I@?",
         "",
-        {"retval": {"already_cfretained": True}},
+        {
+            "retval": {"already_cfretained": True},
+            "arguments": {3: {"type_modifier": "o"}},
+        },
+    ),
+    "MIDIObjectFindByUniqueID": (
+        b"ii^I^i",
+        "",
+        {"arguments": {1: {"type_modifier": "o"}, 2: {"type_modifier": "o"}}},
     ),
-    "MIDIObjectFindByUniqueID": (b"ii^I^i",),
     "MIDIObjectSetIntegerProperty": (b"iI^{__CFString=}i",),
     "MIDIEventPacketNext": (b"^{MIDIEventPacket=QI[64I]}^{MIDIEventPacket=QI[64I]}",),
     "MIDI2ChannelVoiceMessage": (b"{MIDIMessage_64=II}CCCSI",),
     "MIDIPortDispose": (b"iI",),
     "MIDIDeviceListAddDevice": (b"iII",),
     "MIDIGetNumberOfDestinations": (b"Q",),
+    "MIDIEndpointGetRefCons": (
+        b"iI^^v^^v",
+        "",
+        {"arguments": {1: {"type_modifier": "o"}, 2: {"type_modifier": "o"}}},
+    ),
     "MIDIRestart": (b"i",),
     "MIDIClientCreateWithBlock": (
         b"i^{__CFString=}^I@?",
         "",
-        {"retval": {"already_cfretained": True}},
+        {
+            "retval": {"already_cfretained": True},
+            "arguments": {1: {"type_modifier": "o"}},
+        },
     ),
     "MIDIThruConnectionGetParams": (
         b"iI^^{__CFData=}",
         "",
         {"arguments": {1: {"type_modifier": "o"}}},
     ),
-    "MIDIReceivedEventList": (b"iI^{MIDIEventList=iI[1{MIDIEventPacket=QI[64I]}]}",),
-    "MIDIObjectGetStringProperty": (b"iI^{__CFString=}^^{__CFString=}",),
+    "MIDIObjectGetStringProperty": (
+        b"iI^{__CFString=}^^{__CFString=}",
+        "",
+        {"arguments": {2: {"type_modifier": "o"}}},
+    ),
     "MIDIGetExternalDevice": (b"IQ",),
     "MIDI2RelRegisteredControl": (b"{MIDIMessage_64=II}CCCCI",),
     "MIDI2ProgramChange": (b"{MIDIMessage_64=II}CCBCCC",),
     "MIDIThruConnectionCreate": (
         b"i^{__CFString=}^{__CFData=}^I",
         "",
         {
             "retval": {"already_cfretained": True},
             "arguments": {2: {"type_modifier": "o"}},
         },
     ),
     "MIDIDeviceListDispose": (b"iI",),
-    "MIDISendSysex": (b"i^{MIDISysexSendRequest=I^CIZ[3C]^?^v}",),
     "MIDI2PerNoteManagment": (b"{MIDIMessage_64=II}CCCBB",),
     "MIDIGetSerialPortOwner": (
         b"i^{__CFString=}^^{__CFString=}",
         "",
         {"arguments": {1: {"type_modifier": "o"}}},
     ),
     "MIDIGetDevice": (b"IQ",),
-    "MIDIThruConnectionSetParams": (b"iI^{__CFData=}",),
     "MIDI2ControlChange": (b"{MIDIMessage_64=II}CCCI",),
     "MIDISetupRemoveExternalDevice": (b"iI",),
-    "MIDIEventListAdd": (
-        b"^{MIDIEventPacket=QI[64I]}^{MIDIEventList=iI[1{MIDIEventPacket=QI[64I]}]}Q^{MIDIEventPacket=QI[64I]}QQ^I",
-    ),
     "MIDIDeviceListGetNumberOfDevices": (b"QI",),
     "MIDIInputPortCreateWithProtocol": (
         b"iI^{__CFString=}i^I@?",
         "",
-        {"retval": {"already_cfretained": True}},
+        {
+            "retval": {"already_cfretained": True},
+            "arguments": {3: {"type_modifier": "o"}},
+        },
     ),
     "MIDIDeviceGetEntity": (b"IIQ",),
     "MIDI2NoteOff": (b"{MIDIMessage_64=II}CCCCSS",),
     "MIDI2PolyPressure": (b"{MIDIMessage_64=II}CCCI",),
     "MIDI1UPPitchBend": (b"ICCCC",),
-    "MIDIDeviceCreate": (
-        b"i^^{MIDIDriverInterface=^v^?^?^?^?^?^?^?^?^?^?^?^?^?}^{__CFString=}^{__CFString=}^{__CFString=}^I",
+    "MIDIOutputPortCreate": (
+        b"iI^{__CFString=}^I",
         "",
         {
             "retval": {"already_cfretained": True},
-            "arguments": {4: {"type_modifier": "o"}},
+            "arguments": {2: {"type_modifier": "o"}},
         },
     ),
-    "MIDIOutputPortCreate": (
-        b"iI^{__CFString=}^I",
-        "",
-        {"retval": {"already_cfretained": True}},
-    ),
     "MIDISourceCreateWithProtocol": (
         b"iI^{__CFString=}i^I",
         "",
-        {"retval": {"already_cfretained": True}},
+        {
+            "retval": {"already_cfretained": True},
+            "arguments": {3: {"type_modifier": "o"}},
+        },
     ),
     "MIDIEntityGetDestination": (b"IIQ",),
     "MIDIInputPortCreateWithBlock": (
         b"iI^{__CFString=}^I@?",
         "",
-        {"retval": {"already_cfretained": True}},
+        {
+            "retval": {"already_cfretained": True},
+            "arguments": {2: {"type_modifier": "o"}},
+        },
     ),
     "MIDI2AssignableControl": (b"{MIDIMessage_64=II}CCCCI",),
     "MIDI2AssignablePNC": (b"{MIDIMessage_64=II}CCCCI",),
     "MIDI2RegisteredControl": (b"{MIDIMessage_64=II}CCCCI",),
     "MIDIGetDriverIORunLoop": (b"^{__CFRunLoop=}",),
-    "MIDIEntityGetDevice": (b"iI^I",),
-    "MIDI1UPSysExArray": (b"{MIDIMessage_64=II}CC^C^C",),
+    "MIDIEntityGetDevice": (b"iI^I", "", {"arguments": {1: {"type_modifier": "o"}}}),
     "MIDIDeviceRemoveEntity": (b"iII",),
     "MIDIGetNumberOfSources": (b"Q",),
     "MIDISourceCreate": (
         b"iI^{__CFString=}^I",
         "",
-        {"retval": {"already_cfretained": True}},
+        {
+            "retval": {"already_cfretained": True},
+            "arguments": {2: {"type_modifier": "o"}},
+        },
     ),
     "MIDIEntityGetNumberOfSources": (b"QI",),
     "MIDIBluetoothDriverActivateAllConnections": (b"i",),
     "MIDIEntityGetSource": (b"IIQ",),
 }
 aliases = {"kMIDIStatusActiveSensing": "kMIDIStatusActiveSending"}
 misc.update(
```

### Comparing `pyobjc-framework-CoreMIDI-9.1b1/Lib/pyobjc_framework_CoreMIDI.egg-info/PKG-INFO` & `pyobjc-framework-CoreMIDI-9.2/Lib/pyobjc_framework_CoreMIDI.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-CoreMIDI
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework CoreMIDI on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,CoreMIDI
 Platform: MacOS X
```

### Comparing `pyobjc-framework-CoreMIDI-9.1b1/Lib/pyobjc_framework_CoreMIDI.egg-info/SOURCES.txt` & `pyobjc-framework-CoreMIDI-9.2/Lib/pyobjc_framework_CoreMIDI.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 License.txt
 MANIFEST.in
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Lib/CoreMIDI/__init__.py
 Lib/CoreMIDI/_metadata.py
 Lib/pyobjc_framework_CoreMIDI.egg-info/PKG-INFO
 Lib/pyobjc_framework_CoreMIDI.egg-info/SOURCES.txt
 Lib/pyobjc_framework_CoreMIDI.egg-info/dependency_links.txt
 Lib/pyobjc_framework_CoreMIDI.egg-info/not-zip-safe
```

### Comparing `pyobjc-framework-CoreMIDI-9.1b1/License.txt` & `pyobjc-framework-CoreMIDI-9.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMIDI-9.1b1/Modules/_CoreMIDI.m` & `pyobjc-framework-CoreMIDI-9.2/Modules/_CoreMIDI.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMIDI-9.1b1/Modules/_CoreMIDI_inlines.m` & `pyobjc-framework-CoreMIDI-9.2/Modules/_CoreMIDI_inlines.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMIDI-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-CoreMIDI-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMIDI-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-CoreMIDI-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-CoreMIDI-9.1b1/PKG-INFO` & `pyobjc-framework-CoreMIDI-9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-CoreMIDI
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework CoreMIDI on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,CoreMIDI
 Platform: MacOS X
```

### Comparing `pyobjc-framework-CoreMIDI-9.1b1/PyObjCTest/test_midicapabilityinquiry.py` & `pyobjc-framework-CoreMIDI-9.2/PyObjCTest/test_midicapabilityinquiry.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMIDI-9.1b1/PyObjCTest/test_mididriver.py` & `pyobjc-framework-CoreMIDI-9.2/PyObjCTest/test_mididriver.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,25 +7,27 @@
         self.assertIsOpaquePointer(CoreMIDI.MIDIDriverRef)
 
     def test_constants(self):
         if CoreMIDI.kMIDIDriverPropertyUsesSerial is not None:
             self.assertIsInstance(CoreMIDI.kMIDIDriverPropertyUsesSerial, str)
 
     def test_not_exposed(self):
+        self.assertNotHasAttr(CoreMIDI, "kMIDIDriverCreate")
         self.assertNotHasAttr(CoreMIDI, "kMIDIDriverTypeID")
         self.assertNotHasAttr(CoreMIDI, "kMIDIDriverInterfaceID")
         self.assertNotHasAttr(CoreMIDI, "kMIDIDriverInterface2ID")
         self.assertNotHasAttr(CoreMIDI, "kMIDIDriverInterfaceXID")
-
-        self.assertNotHasAttr(CoreMIDI, "MIDIEndpointSetRefCons")
-        self.assertNotHasAttr(CoreMIDI, "MIDIEndpointGetRefCons")
+        self.assertNotHasAttr(CoreMIDI, "MIDIDriverEnableMonitoring")
+        self.assertNotHasAttr(CoreMIDI, "MIDIGetDriverDeviceList")
 
     def test_functions(self):
-        self.assertArgIsOut(CoreMIDI.MIDIDeviceCreate, 4)
+        # self.assertArgIsOut(CoreMIDI.MIDIDeviceCreate, 4)
         CoreMIDI.MIDIDeviceDispose
         CoreMIDI.MIDIDeviceListGetNumberOfDevices
         CoreMIDI.MIDIDeviceListGetDevice
         CoreMIDI.MIDIDeviceListAddDevice
         CoreMIDI.MIDIDeviceListDispose
         CoreMIDI.MIDIGetDriverIORunLoop
-        CoreMIDI.MIDIGetDriverDeviceList
-        self.assertArgIsBOOL(CoreMIDI.MIDIDriverEnableMonitoring, 1)
+        # CoreMIDI.MIDIGetDriverDeviceList
+        # self.assertArgIsBOOL(CoreMIDI.MIDIDriverEnableMonitoring, 1)
+        CoreMIDI.MIDIEndpointSetRefCons
+        CoreMIDI.MIDIEndpointGetRefCons
```

### Comparing `pyobjc-framework-CoreMIDI-9.1b1/PyObjCTest/test_midimessages.py` & `pyobjc-framework-CoreMIDI-9.2/PyObjCTest/test_midimessages.py`

 * *Files 5% similar despite different names*

```diff
@@ -110,12 +110,13 @@
         CoreMIDI.MIDI2ProgramChange
         CoreMIDI.MIDI2ChannelPressure
         CoreMIDI.MIDI2PitchBend
         CoreMIDI.MIDI2PerNotePitchBend
 
     @min_sdk_level("12.0")
     def test_functions12_0(self):
-        CoreMIDI.MIDI1UPSysEx
-        CoreMIDI.MIDI1UPSysExArray
+        # These have an API that's not easily reproduced in Python
+        # CoreMIDI.MIDI1UPSysEx
+        # CoreMIDI.MIDI1UPSysExArray
 
         # 'MIDIUniversalMessage' is not available in Python
         self.assertNotHasAttr(CoreMIDI, "MIDIEventListForEachEvent")
```

### Comparing `pyobjc-framework-CoreMIDI-9.1b1/PyObjCTest/test_midinetworksession.py` & `pyobjc-framework-CoreMIDI-9.2/PyObjCTest/test_midinetworksession.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMIDI-9.1b1/PyObjCTest/test_midiservices.py` & `pyobjc-framework-CoreMIDI-9.2/PyObjCTest/test_midiservices.py`

 * *Files 19% similar despite different names*

```diff
@@ -44,7 +44,13 @@
             0x10 | CoreMIDI.kMIDIObjectType_Destination,
         )
 
         self.assertEqual(CoreMIDI.kMIDIObjectType_ExternalMask, 0x10)
 
         self.assertEqual(CoreMIDI.kMIDIProtocol_1_0, 1)
         self.assertEqual(CoreMIDI.kMIDIProtocol_2_0, 2)
+
+    def test_functions(self):
+        self.assertArgIsOut(CoreMIDI.MIDISourceCreateWithProtocol, 3)
+        self.assertArgIsOut(CoreMIDI.MIDISourceCreate, 2)
+        self.assertArgIsOut(CoreMIDI.MIDISetupCreate, 0)
+        self.assertArgIsOut(CoreMIDI.MIDIDestinationCreate, 4)
```

### Comparing `pyobjc-framework-CoreMIDI-9.1b1/PyObjCTest/test_midisetup.py` & `pyobjc-framework-CoreMIDI-9.2/PyObjCTest/test_midisetup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMIDI-9.1b1/PyObjCTest/test_midithruconnection.py` & `pyobjc-framework-CoreMIDI-9.2/PyObjCTest/test_midithruconnection.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMIDI-9.1b1/metadata/CoreMIDI.fwinfo` & `pyobjc-framework-CoreMIDI-9.2/metadata/CoreMIDI.fwinfo`

 * *Files 12% similar despite different names*

```diff
@@ -186,14 +186,15 @@
       "selector": "setEnabled:"
      }
     ]
    }
   },
   "formal_protocols": {},
   "functions": {
+   "MIDI1UPSysExArray": { "ignore": true },
    "MIDIEventListForEachEvent": { "ignore": true },
    "MIDIClientCreate": {
     "args": {
      "0": {},
      "1": {
       "function": {
        "args": [
@@ -206,21 +207,21 @@
        ],
        "retval": {
         "typestr": "v"
        }
       }
      },
      "2": {},
-     "3": {}
+     "3": { "type_modifier": "o"}
     }
    },
    "MIDIClientCreateWithBlock": {
     "args": {
      "0": {},
-     "1": {}
+     "1": { "type_modifier": "o"}
     }
    },
    "MIDIDestinationCreate": {
     "args": {
      "1": {},
      "2": {
       "function": {
@@ -237,36 +238,38 @@
        ],
        "retval": {
         "typestr": "v"
        }
       }
      },
      "3": {},
-     "4": {}
+     "4": {"type_modifier":"o"}
     }
    },
    "MIDIDestinationCreateWithBlock": {
+    "ignore": true,
     "args": {
      "1": {},
-     "2": {}
+     "2": {"type_modifier":"o"}
     }
    },
    "MIDIDestinationCreateWithProtocol": {
     "args": {
      "1": {},
-     "3": {}
+     "3": { "type_modifier": "o"}
     }
    },
    "MIDIDeviceAddEntity": {
     "args": {
      "1": {},
      "5": { "type_modifier": "o" }
     }
    },
    "MIDIDeviceCreate": {
+    "ignore": true,
     "args": {
      "0": {},
      "1": {},
      "2": {},
      "3": {},
      "4": { "type_modifier": "o" }
     }
@@ -274,51 +277,52 @@
    "MIDIDeviceNewEntity": {
     "args": {
      "1": {},
      "6": { "type_modifier": "o" }
     }
    },
    "MIDIDriverEnableMonitoring": {
+    "ignore": true,
     "args": {
      "0": {}
     }
    },
    "MIDIEndpointGetEntity": {
     "args": {
-     "1": {}
+     "1": { "type_modifier": "o" }
     }
    },
    "MIDIEndpointGetRefCons": {
-    "ignore": true,
     "args": {
-     "1": {},
-     "2": {}
+     "1": { "type_modifier": "o" },
+     "2": { "type_modifier": "o" }
     }
    },
    "MIDIEndpointSetRefCons": {
-    "ignore": true,
     "args": {
      "1": {},
      "2": {}
     }
    },
    "MIDIEntityGetDevice": {
     "args": {
-     "1": {}
+     "1": { "type_modifier": "o"}
     }
    },
    "MIDIEventListAdd": {
+    "ignore": true,
     "args": {
      "0": {},
      "2": {},
      "5": {}
     },
     "retval": {}
    },
    "MIDIEventListInit": {
+    "ignore": true,
     "args": {
      "0": {}
     },
     "retval": {}
    },
    "MIDIEventPacketNext": {
     "args": {
@@ -331,14 +335,15 @@
      "0": {},
      "1": {},
      "2": {},
      "3": { "type_modifier": "o" }
     }
    },
    "MIDIGetDriverDeviceList": {
+    "ignore": true,
     "args": {
      "0": {}
     }
    },
    "MIDIGetDriverIORunLoop": {
     "retval": {}
    },
@@ -371,62 +376,62 @@
        ],
        "retval": {
         "typestr": "v"
        }
       }
      },
      "3": {},
-     "4": {}
+     "4": { "type_modifier": "o" }
     }
    },
    "MIDIInputPortCreateWithBlock": {
     "args": {
      "1": {},
-     "2": {}
+     "2": { "type_modifier": "o" }
     }
    },
    "MIDIInputPortCreateWithProtocol": {
     "args": {
      "1": {},
-     "3": {}
+     "3": { "type_modifier": "o" }
     }
    },
    "MIDIObjectFindByUniqueID": {
     "args": {
-     "1": {},
-     "2": {}
+     "1": { "type_modifier": "o"},
+     "2": { "type_modifier": "o"}
     }
    },
    "MIDIObjectGetDataProperty": {
     "args": {
      "1": {},
-     "2": {}
+     "2": { "type_modifier": "o" }
     }
    },
    "MIDIObjectGetDictionaryProperty": {
     "args": {
      "1": {},
-     "2": {}
+     "2": { "type_modifier": "o" }
     }
    },
    "MIDIObjectGetIntegerProperty": {
     "args": {
      "1": {},
-     "2": {}
+     "2": { "type_modifier": "o" }
     }
    },
    "MIDIObjectGetProperties": {
     "args": {
-     "1": {}
+     "1": { "type_modifier": "o" }
     }
    },
    "MIDIObjectGetStringProperty": {
     "args": {
      "1": {},
-     "2": {}
+     "2": { "type_modifier": "o" }
     }
    },
    "MIDIObjectRemoveProperty": {
     "args": {
      "1": {}
     }
    },
@@ -452,26 +457,28 @@
      "1": {},
      "2": {}
     }
    },
    "MIDIOutputPortCreate": {
     "args": {
      "1": {},
-     "2": {}
+     "2": { "type_modifier": "o" }
     }
    },
    "MIDIPacketListAdd": {
+    "ignore": true,
     "args": {
      "0": {},
      "2": {},
      "5": {}
     },
     "retval": {}
    },
    "MIDIPacketListInit": {
+    "ignore": true,
     "args": {
      "0": {}
     },
     "retval": {}
    },
    "MIDIPacketNext": {
     "args": {
@@ -481,47 +488,52 @@
    },
    "MIDIPortConnectSource": {
     "args": {
      "2": {}
     }
    },
    "MIDIReceived": {
+    "ignore": true,
     "args": {
      "1": {}
     }
    },
    "MIDIReceivedEventList": {
+    "ignore": true,
     "args": {
      "1": {}
     }
    },
    "MIDISend": {
+    "ignore": true,
     "args": {
      "2": {}
     }
    },
    "MIDISendEventList": {
+    "ignore": true,
     "args": {
      "2": {}
     }
    },
    "MIDISendSysex": {
+    "ignore": true,
     "args": {
      "0": {}
     }
    },
    "MIDISetSerialPortOwner": {
     "args": {
      "0": {},
      "1": {}
     }
    },
    "MIDISetupCreate": {
     "args": {
-     "0": {}
+     "0": { "type_modifier": "o"}
     }
    },
    "MIDISetupFromData": {
     "args": {
      "0": {},
      "1": { "type_modifier": "o" }
     }
@@ -535,21 +547,21 @@
     "args": {
      "1": { "type_modifier": "o", "already_cfretained": true }
     }
    },
    "MIDISourceCreate": {
     "args": {
      "1": {},
-     "2": {}
+     "2": { "type_modifier": "o" }
     }
    },
    "MIDISourceCreateWithProtocol": {
     "args": {
      "1": {},
-     "3": {}
+     "3": { "type_modifier": "o" }
     }
    },
    "MIDIThruConnectionCreate": {
     "args": {
      "0": {},
      "1": {},
      "2": { "type_modifier": "o" }
```

### Comparing `pyobjc-framework-CoreMIDI-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-CoreMIDI-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMIDI-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-CoreMIDI-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMIDI-9.1b1/metadata/raw/arm64-13.0.fwinfo` & `pyobjc-framework-CoreMIDI-9.2/metadata/raw/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMIDI-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-CoreMIDI-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMIDI-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-CoreMIDI-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMIDI-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-CoreMIDI-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMIDI-9.1b1/metadata/raw/x86_64-13.0.fwinfo` & `pyobjc-framework-CoreMIDI-9.2/metadata/raw/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMIDI-9.1b1/pyobjc_setup.py` & `pyobjc-framework-CoreMIDI-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-CoreMIDI-9.1b1/setup.py` & `pyobjc-framework-CoreMIDI-9.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,18 +4,22 @@
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
     name="pyobjc-framework-CoreMIDI",
     description="Wrappers for the framework CoreMIDI on macOS",
     packages=["CoreMIDI"],
     ext_modules=[
         Extension(
```

