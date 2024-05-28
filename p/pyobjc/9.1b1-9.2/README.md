# Comparing `tmp/pyobjc-9.1b1.tar.gz` & `tmp/pyobjc-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-9.1b1.tar", last modified: Sun Mar 26 10:48:16 2023, max compression
+gzip compressed data, was "pyobjc-9.2.tar", last modified: Tue Jun  6 23:56:01 2023, max compression
```

## Comparing `pyobjc-9.1b1.tar` & `pyobjc-9.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 10:48:16.345915 pyobjc-9.1b1/
--rw-r--r--   0 ronald     (501) staff       (20)     1871 2023-03-26 10:48:16.345504 pyobjc-9.1b1/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)      344 2023-03-03 17:21:59.000000 pyobjc-9.1b1/README.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 10:48:16.340613 pyobjc-9.1b1/pyobjc.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2082 2023-03-26 10:48:16.000000 pyobjc-9.1b1/pyobjc.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)      193 2023-03-26 10:48:16.000000 pyobjc-9.1b1/pyobjc.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 10:48:16.000000 pyobjc-9.1b1/pyobjc.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)    11713 2023-03-26 10:48:16.000000 pyobjc-9.1b1/pyobjc.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 10:48:16.000000 pyobjc-9.1b1/pyobjc.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:51:08.000000 pyobjc-9.1b1/pyobjc.egg-info/zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 10:48:16.345992 pyobjc-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)    21267 2023-03-25 14:20:30.000000 pyobjc-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-06 23:56:01.511270 pyobjc-9.2/
+-rw-r--r--   0 ronald     (501) staff       (20)     1869 2023-06-06 23:56:01.510901 pyobjc-9.2/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)      344 2023-03-03 17:21:59.000000 pyobjc-9.2/README.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-06 23:56:01.509830 pyobjc-9.2/pyobjc.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2080 2023-06-06 23:56:01.000000 pyobjc-9.2/pyobjc.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)      193 2023-06-06 23:56:01.000000 pyobjc-9.2/pyobjc.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-06 23:56:01.000000 pyobjc-9.2/pyobjc.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)    11109 2023-06-06 23:56:01.000000 pyobjc-9.2/pyobjc.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-06 23:56:01.000000 pyobjc-9.2/pyobjc.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:51:08.000000 pyobjc-9.2/pyobjc.egg-info/zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-06 23:56:01.511366 pyobjc-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)    21460 2023-05-29 10:07:45.000000 pyobjc-9.2/setup.py
```

### Comparing `pyobjc-9.1b1/PKG-INFO` & `pyobjc-9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc
-Version: 9.1b1
+Version: 9.2
 Summary: Python<->ObjC Interoperability Module
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: Objective-C,bridge,Cocoa
 Platform: macOS
```

### Comparing `pyobjc-9.1b1/pyobjc.egg-info/PKG-INFO` & `pyobjc-9.2/pyobjc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc
-Version: 9.1b1
+Version: 9.2
 Summary: Python<->ObjC Interoperability Module
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: Objective-C,bridge,Cocoa
 Platform: macOS
```

### Comparing `pyobjc-9.1b1/pyobjc.egg-info/requires.txt` & `pyobjc-9.2/pyobjc.egg-info/requires.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,336 +1,336 @@
-pyobjc-core==9.1b1
-pyobjc-framework-AddressBook==9.1b1
-pyobjc-framework-AppleScriptKit==9.1b1
-pyobjc-framework-ApplicationServices==9.1b1
-pyobjc-framework-Automator==9.1b1
-pyobjc-framework-CFNetwork==9.1b1
-pyobjc-framework-Cocoa==9.1b1
-pyobjc-framework-CoreAudio==9.1b1
-pyobjc-framework-CoreAudioKit==9.1b1
-pyobjc-framework-CoreData==9.1b1
-pyobjc-framework-CoreMIDI==9.1b1
-pyobjc-framework-CoreServices==9.1b1
-pyobjc-framework-CoreText==9.1b1
-pyobjc-framework-DiscRecording==9.1b1
-pyobjc-framework-DiscRecordingUI==9.1b1
-pyobjc-framework-DiskArbitration==9.1b1
-pyobjc-framework-DVDPlayback==9.1b1
-pyobjc-framework-ExceptionHandling==9.1b1
-pyobjc-framework-InstallerPlugins==9.1b1
-pyobjc-framework-IOBluetooth==9.1b1
-pyobjc-framework-IOBluetoothUI==9.1b1
-pyobjc-framework-LatentSemanticMapping==9.1b1
-pyobjc-framework-LaunchServices==9.1b1
-pyobjc-framework-OSAKit==9.1b1
-pyobjc-framework-PreferencePanes==9.1b1
-pyobjc-framework-Quartz==9.1b1
-pyobjc-framework-ScreenSaver==9.1b1
-pyobjc-framework-Security==9.1b1
-pyobjc-framework-SecurityFoundation==9.1b1
-pyobjc-framework-SecurityInterface==9.1b1
-pyobjc-framework-SearchKit==9.1b1
-pyobjc-framework-SyncServices==9.1b1
-pyobjc-framework-SystemConfiguration==9.1b1
-pyobjc-framework-WebKit==9.1b1
+pyobjc-core==9.2
+pyobjc-framework-AddressBook==9.2
+pyobjc-framework-AppleScriptKit==9.2
+pyobjc-framework-ApplicationServices==9.2
+pyobjc-framework-Automator==9.2
+pyobjc-framework-CFNetwork==9.2
+pyobjc-framework-Cocoa==9.2
+pyobjc-framework-CoreAudio==9.2
+pyobjc-framework-CoreAudioKit==9.2
+pyobjc-framework-CoreData==9.2
+pyobjc-framework-CoreMIDI==9.2
+pyobjc-framework-CoreServices==9.2
+pyobjc-framework-CoreText==9.2
+pyobjc-framework-DiscRecording==9.2
+pyobjc-framework-DiscRecordingUI==9.2
+pyobjc-framework-DiskArbitration==9.2
+pyobjc-framework-DVDPlayback==9.2
+pyobjc-framework-ExceptionHandling==9.2
+pyobjc-framework-InstallerPlugins==9.2
+pyobjc-framework-IOBluetooth==9.2
+pyobjc-framework-IOBluetoothUI==9.2
+pyobjc-framework-LatentSemanticMapping==9.2
+pyobjc-framework-LaunchServices==9.2
+pyobjc-framework-OSAKit==9.2
+pyobjc-framework-PreferencePanes==9.2
+pyobjc-framework-Quartz==9.2
+pyobjc-framework-ScreenSaver==9.2
+pyobjc-framework-Security==9.2
+pyobjc-framework-SecurityFoundation==9.2
+pyobjc-framework-SecurityInterface==9.2
+pyobjc-framework-SearchKit==9.2
+pyobjc-framework-SyncServices==9.2
+pyobjc-framework-SystemConfiguration==9.2
+pyobjc-framework-WebKit==9.2
 
 [:platform_release >= "10.0"]
-pyobjc-framework-AppleScriptObjC==9.1b1
-pyobjc-framework-CoreLocation==9.1b1
-pyobjc-framework-CoreWLAN==9.1b1
-pyobjc-framework-ImageCaptureCore==9.1b1
-pyobjc-framework-IOSurface==9.1b1
-pyobjc-framework-NetFS==9.1b1
-pyobjc-framework-OpenDirectory==9.1b1
-pyobjc-framework-ServiceManagement==9.1b1
-pyobjc-framework-iTunesLibrary==9.1b1
+pyobjc-framework-AppleScriptObjC==9.2
+pyobjc-framework-CoreLocation==9.2
+pyobjc-framework-CoreWLAN==9.2
+pyobjc-framework-ImageCaptureCore==9.2
+pyobjc-framework-IOSurface==9.2
+pyobjc-framework-NetFS==9.2
+pyobjc-framework-OpenDirectory==9.2
+pyobjc-framework-ServiceManagement==9.2
+pyobjc-framework-iTunesLibrary==9.2
 
 [:platform_release >= "11.0"]
-pyobjc-framework-AVFoundation==9.1b1
-pyobjc-framework-CoreMedia==9.1b1
-pyobjc-framework-CoreMediaIO==9.1b1
-pyobjc-framework-IMServicePlugIn==9.1b1
-pyobjc-framework-StoreKit==9.1b1
-pyobjc-framework-SceneKit==9.1b1
+pyobjc-framework-AVFoundation==9.2
+pyobjc-framework-CoreMedia==9.2
+pyobjc-framework-CoreMediaIO==9.2
+pyobjc-framework-IMServicePlugIn==9.2
+pyobjc-framework-StoreKit==9.2
+pyobjc-framework-SceneKit==9.2
 
 [:platform_release >= "12.0"]
-pyobjc-framework-libdispatch==9.1b1
-pyobjc-framework-libxpc==9.1b1
-pyobjc-framework-AudioVideoBridging==9.1b1
-pyobjc-framework-Accounts==9.1b1
-pyobjc-framework-EventKit==9.1b1
-pyobjc-framework-GameCenter==9.1b1
-pyobjc-framework-Social==9.1b1
-pyobjc-framework-GameKit==9.1b1
-pyobjc-framework-VideoToolbox==9.1b1
+pyobjc-framework-libdispatch==9.2
+pyobjc-framework-libxpc==9.2
+pyobjc-framework-AudioVideoBridging==9.2
+pyobjc-framework-Accounts==9.2
+pyobjc-framework-EventKit==9.2
+pyobjc-framework-GameCenter==9.2
+pyobjc-framework-Social==9.2
+pyobjc-framework-GameKit==9.2
+pyobjc-framework-VideoToolbox==9.2
 
 [:platform_release >= "13.0"]
-pyobjc-framework-AVKit==9.1b1
-pyobjc-framework-GameController==9.1b1
-pyobjc-framework-MapKit==9.1b1
-pyobjc-framework-MediaAccessibility==9.1b1
-pyobjc-framework-MediaLibrary==9.1b1
-pyobjc-framework-MediaToolbox==9.1b1
-pyobjc-framework-SpriteKit==9.1b1
+pyobjc-framework-AVKit==9.2
+pyobjc-framework-GameController==9.2
+pyobjc-framework-MapKit==9.2
+pyobjc-framework-MediaAccessibility==9.2
+pyobjc-framework-MediaLibrary==9.2
+pyobjc-framework-MediaToolbox==9.2
+pyobjc-framework-SpriteKit==9.2
 
 [:platform_release >= "14.0"]
-pyobjc-framework-CloudKit==9.1b1
-pyobjc-framework-CoreBluetooth==9.1b1
-pyobjc-framework-CryptoTokenKit==9.1b1
-pyobjc-framework-FinderSync==9.1b1
-pyobjc-framework-LocalAuthentication==9.1b1
-pyobjc-framework-MultipeerConnectivity==9.1b1
-pyobjc-framework-NotificationCenter==9.1b1
+pyobjc-framework-CloudKit==9.2
+pyobjc-framework-CoreBluetooth==9.2
+pyobjc-framework-CryptoTokenKit==9.2
+pyobjc-framework-FinderSync==9.2
+pyobjc-framework-LocalAuthentication==9.2
+pyobjc-framework-MultipeerConnectivity==9.2
+pyobjc-framework-NotificationCenter==9.2
 
 [:platform_release >= "15.0"]
-pyobjc-framework-Contacts==9.1b1
-pyobjc-framework-ContactsUI==9.1b1
-pyobjc-framework-Metal==9.1b1
-pyobjc-framework-MetalKit==9.1b1
-pyobjc-framework-ModelIO==9.1b1
-pyobjc-framework-NetworkExtension==9.1b1
-pyobjc-framework-Photos==9.1b1
-pyobjc-framework-PhotosUI==9.1b1
-pyobjc-framework-SafariServices==9.1b1
-pyobjc-framework-GameplayKit==9.1b1
+pyobjc-framework-Contacts==9.2
+pyobjc-framework-ContactsUI==9.2
+pyobjc-framework-Metal==9.2
+pyobjc-framework-MetalKit==9.2
+pyobjc-framework-ModelIO==9.2
+pyobjc-framework-NetworkExtension==9.2
+pyobjc-framework-Photos==9.2
+pyobjc-framework-PhotosUI==9.2
+pyobjc-framework-GameplayKit==9.2
 
 [:platform_release >= "16.0"]
-pyobjc-framework-Intents==9.1b1
-pyobjc-framework-MediaPlayer==9.1b1
+pyobjc-framework-Intents==9.2
+pyobjc-framework-MediaPlayer==9.2
+pyobjc-framework-SafariServices==9.2
 
 [:platform_release >= "17.0"]
-pyobjc-framework-ColorSync==9.1b1
-pyobjc-framework-CoreML==9.1b1
-pyobjc-framework-CoreSpotlight==9.1b1
-pyobjc-framework-ExternalAccessory==9.1b1
-pyobjc-framework-MetalPerformanceShaders==9.1b1
-pyobjc-framework-Vision==9.1b1
+pyobjc-framework-ColorSync==9.2
+pyobjc-framework-CoreML==9.2
+pyobjc-framework-CoreSpotlight==9.2
+pyobjc-framework-ExternalAccessory==9.2
+pyobjc-framework-MetalPerformanceShaders==9.2
+pyobjc-framework-Vision==9.2
 
 [:platform_release >= "18.0"]
-pyobjc-framework-AdSupport==9.1b1
-pyobjc-framework-BusinessChat==9.1b1
-pyobjc-framework-NaturalLanguage==9.1b1
-pyobjc-framework-Network==9.1b1
-pyobjc-framework-UserNotifications==9.1b1
-pyobjc-framework-VideoSubscriberAccount==9.1b1
+pyobjc-framework-AdSupport==9.2
+pyobjc-framework-BusinessChat==9.2
+pyobjc-framework-NaturalLanguage==9.2
+pyobjc-framework-Network==9.2
+pyobjc-framework-UserNotifications==9.2
+pyobjc-framework-VideoSubscriberAccount==9.2
 
 [:platform_release >= "19.0"]
-pyobjc-framework-AuthenticationServices==9.1b1
-pyobjc-framework-AutomaticAssessmentConfiguration==9.1b1
-pyobjc-framework-CoreHaptics==9.1b1
-pyobjc-framework-CoreMotion==9.1b1
-pyobjc-framework-DeviceCheck==9.1b1
-pyobjc-framework-ExecutionPolicy==9.1b1
-pyobjc-framework-FileProvider==9.1b1
-pyobjc-framework-FileProviderUI==9.1b1
-pyobjc-framework-LinkPresentation==9.1b1
-pyobjc-framework-OSLog==9.1b1
-pyobjc-framework-PencilKit==9.1b1
-pyobjc-framework-PushKit==9.1b1
-pyobjc-framework-QuickLookThumbnailing==9.1b1
-pyobjc-framework-Speech==9.1b1
-pyobjc-framework-SoundAnalysis==9.1b1
-pyobjc-framework-SystemExtensions==9.1b1
+pyobjc-framework-AuthenticationServices==9.2
+pyobjc-framework-AutomaticAssessmentConfiguration==9.2
+pyobjc-framework-CoreHaptics==9.2
+pyobjc-framework-CoreMotion==9.2
+pyobjc-framework-DeviceCheck==9.2
+pyobjc-framework-ExecutionPolicy==9.2
+pyobjc-framework-FileProvider==9.2
+pyobjc-framework-FileProviderUI==9.2
+pyobjc-framework-LinkPresentation==9.2
+pyobjc-framework-OSLog==9.2
+pyobjc-framework-PencilKit==9.2
+pyobjc-framework-PushKit==9.2
+pyobjc-framework-QuickLookThumbnailing==9.2
+pyobjc-framework-Speech==9.2
+pyobjc-framework-SoundAnalysis==9.2
+pyobjc-framework-SystemExtensions==9.2
 
 [:platform_release >= "20.0"]
-pyobjc-framework-Accessibility==9.1b1
-pyobjc-framework-AdServices==9.1b1
-pyobjc-framework-AppTrackingTransparency==9.1b1
-pyobjc-framework-CallKit==9.1b1
-pyobjc-framework-ClassKit==9.1b1
-pyobjc-framework-KernelManagement==9.1b1
-pyobjc-framework-MetalPerformanceShadersGraph==9.1b1
-pyobjc-framework-MLCompute==9.1b1
-pyobjc-framework-PassKit==9.1b1
-pyobjc-framework-ReplayKit==9.1b1
-pyobjc-framework-ScreenTime==9.1b1
-pyobjc-framework-UniformTypeIdentifiers==9.1b1
-pyobjc-framework-UserNotificationsUI==9.1b1
-pyobjc-framework-Virtualization==9.1b1
+pyobjc-framework-Accessibility==9.2
+pyobjc-framework-AdServices==9.2
+pyobjc-framework-AppTrackingTransparency==9.2
+pyobjc-framework-CallKit==9.2
+pyobjc-framework-ClassKit==9.2
+pyobjc-framework-KernelManagement==9.2
+pyobjc-framework-MetalPerformanceShadersGraph==9.2
+pyobjc-framework-MLCompute==9.2
+pyobjc-framework-PassKit==9.2
+pyobjc-framework-ReplayKit==9.2
+pyobjc-framework-ScreenTime==9.2
+pyobjc-framework-UniformTypeIdentifiers==9.2
+pyobjc-framework-UserNotificationsUI==9.2
+pyobjc-framework-Virtualization==9.2
 
 [:platform_release >= "21.0"]
-pyobjc-framework-DataDetection==9.1b1
-pyobjc-framework-IntentsUI==9.1b1
-pyobjc-framework-LocalAuthenticationEmbeddedUI==9.1b1
-pyobjc-framework-MailKit==9.1b1
-pyobjc-framework-MetricKit==9.1b1
-pyobjc-framework-PHASE==9.1b1
-pyobjc-framework-ShazamKit==9.1b1
+pyobjc-framework-DataDetection==9.2
+pyobjc-framework-IntentsUI==9.2
+pyobjc-framework-LocalAuthenticationEmbeddedUI==9.2
+pyobjc-framework-MailKit==9.2
+pyobjc-framework-MetricKit==9.2
+pyobjc-framework-PHASE==9.2
+pyobjc-framework-ShazamKit==9.2
 
 [:platform_release >= "21.4"]
-pyobjc-framework-ScreenCaptureKit==9.1b1
+pyobjc-framework-ScreenCaptureKit==9.2
 
 [:platform_release >= "22.0"]
-pyobjc-framework-AVRouting==9.1b1
-pyobjc-framework-BackgroundAssets==9.1b1
-pyobjc-framework-ExtensionKit==9.1b1
-pyobjc-framework-HealthKit==9.1b1
-pyobjc-framework-MetalFX==9.1b1
-pyobjc-framework-SafetyKit==9.1b1
-pyobjc-framework-SharedWithYouCore==9.1b1
-pyobjc-framework-SharedWithYou==9.1b1
-pyobjc-framework-ThreadNetwork==9.1b1
+pyobjc-framework-AVRouting==9.2
+pyobjc-framework-BackgroundAssets==9.2
+pyobjc-framework-ExtensionKit==9.2
+pyobjc-framework-HealthKit==9.2
+pyobjc-framework-MetalFX==9.2
+pyobjc-framework-SafetyKit==9.2
+pyobjc-framework-SharedWithYouCore==9.2
+pyobjc-framework-SharedWithYou==9.2
+pyobjc-framework-ThreadNetwork==9.2
 
 [:platform_release >= "9.0"]
-pyobjc-framework-CalendarStore==9.1b1
-pyobjc-framework-Collaboration==9.1b1
-pyobjc-framework-DictionaryServices==9.1b1
-pyobjc-framework-FSEvents==9.1b1
-pyobjc-framework-InputMethodKit==9.1b1
-pyobjc-framework-InstantMessage==9.1b1
-pyobjc-framework-ScriptingBridge==9.1b1
+pyobjc-framework-CalendarStore==9.2
+pyobjc-framework-Collaboration==9.2
+pyobjc-framework-DictionaryServices==9.2
+pyobjc-framework-FSEvents==9.2
+pyobjc-framework-InputMethodKit==9.2
+pyobjc-framework-InstantMessage==9.2
+pyobjc-framework-ScriptingBridge==9.2
 
 [:platform_release >= "9.0" and platform_release < "18.0"]
-pyobjc-framework-PubSub==9.1b1
+pyobjc-framework-PubSub==9.2
 
 [allbindings]
-pyobjc-core==9.1b1
-pyobjc-framework-libdispatch==9.1b1
-pyobjc-framework-libxpc==9.1b1
-pyobjc-framework-Accessibility==9.1b1
-pyobjc-framework-AdServices==9.1b1
-pyobjc-framework-AdSupport==9.1b1
-pyobjc-framework-AppTrackingTransparency==9.1b1
-pyobjc-framework-AudioVideoBridging==9.1b1
-pyobjc-framework-AuthenticationServices==9.1b1
-pyobjc-framework-AutomaticAssessmentConfiguration==9.1b1
-pyobjc-framework-AVKit==9.1b1
-pyobjc-framework-AVFoundation==9.1b1
-pyobjc-framework-AVRouting==9.1b1
-pyobjc-framework-Accounts==9.1b1
-pyobjc-framework-AddressBook==9.1b1
-pyobjc-framework-AppleScriptKit==9.1b1
-pyobjc-framework-AppleScriptObjC==9.1b1
-pyobjc-framework-ApplicationServices==9.1b1
-pyobjc-framework-Automator==9.1b1
-pyobjc-framework-BackgroundAssets==9.1b1
-pyobjc-framework-BusinessChat==9.1b1
-pyobjc-framework-CFNetwork==9.1b1
-pyobjc-framework-CalendarStore==9.1b1
-pyobjc-framework-CallKit==9.1b1
-pyobjc-framework-ClassKit==9.1b1
-pyobjc-framework-CloudKit==9.1b1
-pyobjc-framework-Cocoa==9.1b1
-pyobjc-framework-Collaboration==9.1b1
-pyobjc-framework-ColorSync==9.1b1
-pyobjc-framework-Contacts==9.1b1
-pyobjc-framework-ContactsUI==9.1b1
-pyobjc-framework-CoreAudio==9.1b1
-pyobjc-framework-CoreAudioKit==9.1b1
-pyobjc-framework-CoreBluetooth==9.1b1
-pyobjc-framework-CoreData==9.1b1
-pyobjc-framework-CoreHaptics==9.1b1
-pyobjc-framework-CoreLocation==9.1b1
-pyobjc-framework-CoreMedia==9.1b1
-pyobjc-framework-CoreMediaIO==9.1b1
-pyobjc-framework-CoreMIDI==9.1b1
-pyobjc-framework-CoreML==9.1b1
-pyobjc-framework-CoreMotion==9.1b1
-pyobjc-framework-CoreServices==9.1b1
-pyobjc-framework-CoreSpotlight==9.1b1
-pyobjc-framework-CoreText==9.1b1
-pyobjc-framework-CoreWLAN==9.1b1
-pyobjc-framework-CryptoTokenKit==9.1b1
-pyobjc-framework-DataDetection==9.1b1
-pyobjc-framework-DeviceCheck==9.1b1
-pyobjc-framework-DictionaryServices==9.1b1
-pyobjc-framework-DiscRecording==9.1b1
-pyobjc-framework-DiscRecordingUI==9.1b1
-pyobjc-framework-DiskArbitration==9.1b1
-pyobjc-framework-DVDPlayback==9.1b1
-pyobjc-framework-EventKit==9.1b1
-pyobjc-framework-ExceptionHandling==9.1b1
-pyobjc-framework-ExecutionPolicy==9.1b1
-pyobjc-framework-ExternalAccessory==9.1b1
-pyobjc-framework-ExtensionKit==9.1b1
-pyobjc-framework-FileProvider==9.1b1
-pyobjc-framework-FileProviderUI==9.1b1
-pyobjc-framework-FSEvents==9.1b1
-pyobjc-framework-FinderSync==9.1b1
-pyobjc-framework-GameCenter==9.1b1
-pyobjc-framework-GameController==9.1b1
-pyobjc-framework-HealthKit==9.1b1
-pyobjc-framework-IMServicePlugIn==9.1b1
-pyobjc-framework-InputMethodKit==9.1b1
-pyobjc-framework-ImageCaptureCore==9.1b1
-pyobjc-framework-Intents==9.1b1
-pyobjc-framework-IntentsUI==9.1b1
-pyobjc-framework-InstallerPlugins==9.1b1
-pyobjc-framework-InstantMessage==9.1b1
-pyobjc-framework-IOBluetooth==9.1b1
-pyobjc-framework-IOBluetoothUI==9.1b1
-pyobjc-framework-IOSurface==9.1b1
-pyobjc-framework-KernelManagement==9.1b1
-pyobjc-framework-LatentSemanticMapping==9.1b1
-pyobjc-framework-LaunchServices==9.1b1
-pyobjc-framework-LinkPresentation==9.1b1
-pyobjc-framework-LocalAuthentication==9.1b1
-pyobjc-framework-LocalAuthenticationEmbeddedUI==9.1b1
-pyobjc-framework-MailKit==9.1b1
-pyobjc-framework-MapKit==9.1b1
-pyobjc-framework-MediaAccessibility==9.1b1
-pyobjc-framework-MediaLibrary==9.1b1
-pyobjc-framework-MediaPlayer==9.1b1
-pyobjc-framework-MediaToolbox==9.1b1
-pyobjc-framework-Metal==9.1b1
-pyobjc-framework-MetalFX==9.1b1
-pyobjc-framework-MetalKit==9.1b1
-pyobjc-framework-MetalPerformanceShaders==9.1b1
-pyobjc-framework-MetalPerformanceShadersGraph==9.1b1
-pyobjc-framework-MetricKit==9.1b1
-pyobjc-framework-MLCompute==9.1b1
-pyobjc-framework-ModelIO==9.1b1
-pyobjc-framework-MultipeerConnectivity==9.1b1
-pyobjc-framework-NaturalLanguage==9.1b1
-pyobjc-framework-NetFS==9.1b1
-pyobjc-framework-Network==9.1b1
-pyobjc-framework-NetworkExtension==9.1b1
-pyobjc-framework-NotificationCenter==9.1b1
-pyobjc-framework-OpenDirectory==9.1b1
-pyobjc-framework-OSAKit==9.1b1
-pyobjc-framework-OSLog==9.1b1
-pyobjc-framework-PassKit==9.1b1
-pyobjc-framework-PencilKit==9.1b1
-pyobjc-framework-PHASE==9.1b1
-pyobjc-framework-Photos==9.1b1
-pyobjc-framework-PhotosUI==9.1b1
-pyobjc-framework-PreferencePanes==9.1b1
-pyobjc-framework-PubSub==9.1b1
-pyobjc-framework-PushKit==9.1b1
-pyobjc-framework-Quartz==9.1b1
-pyobjc-framework-QuickLookThumbnailing==9.1b1
-pyobjc-framework-ReplayKit==9.1b1
-pyobjc-framework-SafetyKit==9.1b1
-pyobjc-framework-SafariServices==9.1b1
-pyobjc-framework-ScreenSaver==9.1b1
-pyobjc-framework-ScreenTime==9.1b1
-pyobjc-framework-ScriptingBridge==9.1b1
-pyobjc-framework-Security==9.1b1
-pyobjc-framework-SecurityFoundation==9.1b1
-pyobjc-framework-SecurityInterface==9.1b1
-pyobjc-framework-SearchKit==9.1b1
-pyobjc-framework-ServiceManagement==9.1b1
-pyobjc-framework-ShazamKit==9.1b1
-pyobjc-framework-Social==9.1b1
-pyobjc-framework-Speech==9.1b1
-pyobjc-framework-SpriteKit==9.1b1
-pyobjc-framework-StoreKit==9.1b1
-pyobjc-framework-SyncServices==9.1b1
-pyobjc-framework-SystemConfiguration==9.1b1
-pyobjc-framework-WebKit==9.1b1
-pyobjc-framework-GameKit==9.1b1
-pyobjc-framework-GameplayKit==9.1b1
-pyobjc-framework-SceneKit==9.1b1
-pyobjc-framework-SharedWithYouCore==9.1b1
-pyobjc-framework-SharedWithYou==9.1b1
-pyobjc-framework-SoundAnalysis==9.1b1
-pyobjc-framework-ScreenCaptureKit==9.1b1
-pyobjc-framework-SystemExtensions==9.1b1
-pyobjc-framework-ThreadNetwork==9.1b1
-pyobjc-framework-UniformTypeIdentifiers==9.1b1
-pyobjc-framework-UserNotifications==9.1b1
-pyobjc-framework-UserNotificationsUI==9.1b1
-pyobjc-framework-VideoSubscriberAccount==9.1b1
-pyobjc-framework-VideoToolbox==9.1b1
-pyobjc-framework-Virtualization==9.1b1
-pyobjc-framework-Vision==9.1b1
-pyobjc-framework-iTunesLibrary==9.1b1
+pyobjc-core==9.2
+pyobjc-framework-libdispatch==9.2
+pyobjc-framework-libxpc==9.2
+pyobjc-framework-Accessibility==9.2
+pyobjc-framework-AdServices==9.2
+pyobjc-framework-AdSupport==9.2
+pyobjc-framework-AppTrackingTransparency==9.2
+pyobjc-framework-AudioVideoBridging==9.2
+pyobjc-framework-AuthenticationServices==9.2
+pyobjc-framework-AutomaticAssessmentConfiguration==9.2
+pyobjc-framework-AVKit==9.2
+pyobjc-framework-AVFoundation==9.2
+pyobjc-framework-AVRouting==9.2
+pyobjc-framework-Accounts==9.2
+pyobjc-framework-AddressBook==9.2
+pyobjc-framework-AppleScriptKit==9.2
+pyobjc-framework-AppleScriptObjC==9.2
+pyobjc-framework-ApplicationServices==9.2
+pyobjc-framework-Automator==9.2
+pyobjc-framework-BackgroundAssets==9.2
+pyobjc-framework-BusinessChat==9.2
+pyobjc-framework-CFNetwork==9.2
+pyobjc-framework-CalendarStore==9.2
+pyobjc-framework-CallKit==9.2
+pyobjc-framework-ClassKit==9.2
+pyobjc-framework-CloudKit==9.2
+pyobjc-framework-Cocoa==9.2
+pyobjc-framework-Collaboration==9.2
+pyobjc-framework-ColorSync==9.2
+pyobjc-framework-Contacts==9.2
+pyobjc-framework-ContactsUI==9.2
+pyobjc-framework-CoreAudio==9.2
+pyobjc-framework-CoreAudioKit==9.2
+pyobjc-framework-CoreBluetooth==9.2
+pyobjc-framework-CoreData==9.2
+pyobjc-framework-CoreHaptics==9.2
+pyobjc-framework-CoreLocation==9.2
+pyobjc-framework-CoreMedia==9.2
+pyobjc-framework-CoreMediaIO==9.2
+pyobjc-framework-CoreMIDI==9.2
+pyobjc-framework-CoreML==9.2
+pyobjc-framework-CoreMotion==9.2
+pyobjc-framework-CoreServices==9.2
+pyobjc-framework-CoreSpotlight==9.2
+pyobjc-framework-CoreText==9.2
+pyobjc-framework-CoreWLAN==9.2
+pyobjc-framework-CryptoTokenKit==9.2
+pyobjc-framework-DataDetection==9.2
+pyobjc-framework-DeviceCheck==9.2
+pyobjc-framework-DictionaryServices==9.2
+pyobjc-framework-DiscRecording==9.2
+pyobjc-framework-DiscRecordingUI==9.2
+pyobjc-framework-DiskArbitration==9.2
+pyobjc-framework-DVDPlayback==9.2
+pyobjc-framework-EventKit==9.2
+pyobjc-framework-ExceptionHandling==9.2
+pyobjc-framework-ExecutionPolicy==9.2
+pyobjc-framework-ExternalAccessory==9.2
+pyobjc-framework-ExtensionKit==9.2
+pyobjc-framework-FileProvider==9.2
+pyobjc-framework-FileProviderUI==9.2
+pyobjc-framework-FSEvents==9.2
+pyobjc-framework-FinderSync==9.2
+pyobjc-framework-GameCenter==9.2
+pyobjc-framework-GameController==9.2
+pyobjc-framework-HealthKit==9.2
+pyobjc-framework-IMServicePlugIn==9.2
+pyobjc-framework-InputMethodKit==9.2
+pyobjc-framework-ImageCaptureCore==9.2
+pyobjc-framework-Intents==9.2
+pyobjc-framework-IntentsUI==9.2
+pyobjc-framework-InstallerPlugins==9.2
+pyobjc-framework-InstantMessage==9.2
+pyobjc-framework-IOBluetooth==9.2
+pyobjc-framework-IOBluetoothUI==9.2
+pyobjc-framework-IOSurface==9.2
+pyobjc-framework-KernelManagement==9.2
+pyobjc-framework-LatentSemanticMapping==9.2
+pyobjc-framework-LaunchServices==9.2
+pyobjc-framework-LinkPresentation==9.2
+pyobjc-framework-LocalAuthentication==9.2
+pyobjc-framework-LocalAuthenticationEmbeddedUI==9.2
+pyobjc-framework-MailKit==9.2
+pyobjc-framework-MapKit==9.2
+pyobjc-framework-MediaAccessibility==9.2
+pyobjc-framework-MediaLibrary==9.2
+pyobjc-framework-MediaPlayer==9.2
+pyobjc-framework-MediaToolbox==9.2
+pyobjc-framework-Metal==9.2
+pyobjc-framework-MetalFX==9.2
+pyobjc-framework-MetalKit==9.2
+pyobjc-framework-MetalPerformanceShaders==9.2
+pyobjc-framework-MetalPerformanceShadersGraph==9.2
+pyobjc-framework-MetricKit==9.2
+pyobjc-framework-MLCompute==9.2
+pyobjc-framework-ModelIO==9.2
+pyobjc-framework-MultipeerConnectivity==9.2
+pyobjc-framework-NaturalLanguage==9.2
+pyobjc-framework-NetFS==9.2
+pyobjc-framework-Network==9.2
+pyobjc-framework-NetworkExtension==9.2
+pyobjc-framework-NotificationCenter==9.2
+pyobjc-framework-OpenDirectory==9.2
+pyobjc-framework-OSAKit==9.2
+pyobjc-framework-OSLog==9.2
+pyobjc-framework-PassKit==9.2
+pyobjc-framework-PencilKit==9.2
+pyobjc-framework-PHASE==9.2
+pyobjc-framework-Photos==9.2
+pyobjc-framework-PhotosUI==9.2
+pyobjc-framework-PreferencePanes==9.2
+pyobjc-framework-PubSub==9.2
+pyobjc-framework-PushKit==9.2
+pyobjc-framework-Quartz==9.2
+pyobjc-framework-QuickLookThumbnailing==9.2
+pyobjc-framework-ReplayKit==9.2
+pyobjc-framework-SafetyKit==9.2
+pyobjc-framework-SafariServices==9.2
+pyobjc-framework-ScreenSaver==9.2
+pyobjc-framework-ScreenTime==9.2
+pyobjc-framework-ScriptingBridge==9.2
+pyobjc-framework-Security==9.2
+pyobjc-framework-SecurityFoundation==9.2
+pyobjc-framework-SecurityInterface==9.2
+pyobjc-framework-SearchKit==9.2
+pyobjc-framework-ServiceManagement==9.2
+pyobjc-framework-ShazamKit==9.2
+pyobjc-framework-Social==9.2
+pyobjc-framework-Speech==9.2
+pyobjc-framework-SpriteKit==9.2
+pyobjc-framework-StoreKit==9.2
+pyobjc-framework-SyncServices==9.2
+pyobjc-framework-SystemConfiguration==9.2
+pyobjc-framework-WebKit==9.2
+pyobjc-framework-GameKit==9.2
+pyobjc-framework-GameplayKit==9.2
+pyobjc-framework-SceneKit==9.2
+pyobjc-framework-SharedWithYouCore==9.2
+pyobjc-framework-SharedWithYou==9.2
+pyobjc-framework-SoundAnalysis==9.2
+pyobjc-framework-ScreenCaptureKit==9.2
+pyobjc-framework-SystemExtensions==9.2
+pyobjc-framework-ThreadNetwork==9.2
+pyobjc-framework-UniformTypeIdentifiers==9.2
+pyobjc-framework-UserNotifications==9.2
+pyobjc-framework-UserNotificationsUI==9.2
+pyobjc-framework-VideoSubscriberAccount==9.2
+pyobjc-framework-VideoToolbox==9.2
+pyobjc-framework-Virtualization==9.2
+pyobjc-framework-Vision==9.2
+pyobjc-framework-iTunesLibrary==9.2
```

### Comparing `pyobjc-9.1b1/setup.py` & `pyobjc-9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import subprocess
 import sys
 import tarfile
 
 from setuptools import setup, Command
 from setuptools.command import egg_info
 
-VERSION = "9.1b1"
+VERSION = "9.2"
 
 # Table with all framework wrappers and the OSX releases where they are
 # first supported, and where support was removed. The introduced column
 # is ``None`` when the framework is supported on OSX 10.4 or later. The
 # removed column is ``None`` when the framework is present ont he latest
 # supported OSX release.
 FRAMEWORK_WRAPPERS = [
@@ -133,15 +133,15 @@
     ("PreferencePanes", None, None),
     ("PubSub", "10.5", "10.14"),
     ("PushKit", "10.15", None),
     ("Quartz", None, None),
     ("QuickLookThumbnailing", "10.15", None),
     ("ReplayKit", "11.0", None),
     ("SafetyKit", "13.0", None),
-    ("SafariServices", "10.11", None),
+    ("SafariServices", "10.12", None),
     ("ScreenSaver", None, None),
     ("ScreenTime", "11.0", None),
     ("ScriptingBridge", "10.5", None),
     ("Security", None, None),
     ("SecurityFoundation", None, None),
     ("SecurityInterface", None, None),
     ("SearchKit", None, None),
@@ -394,14 +394,18 @@
                 print("Framework wrapper for %s does not contain MANIFEST.in" % (nm))
                 failures += 1
 
             if not os.path.exists(os.path.join(subdir, "setup.py")):
                 print("Framework wrapper for %s does not contain setup.py" % (nm))
                 failures += 1
 
+            if not os.path.exists(os.path.join(subdir, "pyproject.toml")):
+                print("Framework wrapper for %s does not contain pyproject.toml" % (nm))
+                failures += 1
+
             if not os.path.exists(os.path.join(subdir, "pyobjc_setup.py")):
                 print(
                     "Framework wrapper for %s does not contain pyobjc_setup.py" % (nm)
                 )
                 failures += 1
 
             else:
```

