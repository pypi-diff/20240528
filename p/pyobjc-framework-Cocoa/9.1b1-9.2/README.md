# Comparing `tmp/pyobjc-framework-Cocoa-9.1b1.tar.gz` & `tmp/pyobjc-framework-Cocoa-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-Cocoa-9.1b1.tar", last modified: Sun Mar 26 11:17:02 2023, max compression
+gzip compressed data, was "pyobjc-framework-Cocoa-9.2.tar", last modified: Wed Jun  7 00:07:59 2023, max compression
```

## Comparing `pyobjc-framework-Cocoa-9.1b1.tar` & `pyobjc-framework-Cocoa-9.2.tar`

### file list

```diff
@@ -1,1038 +1,1039 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:17:02.774383 pyobjc-framework-Cocoa-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.105123 pyobjc-framework-Cocoa-9.1b1/Examples/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.097504 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.147699 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/ClassBrowser/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.149706 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/ClassBrowser/ClassBrowser.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      909 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/ClassBrowser/ClassBrowser.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      495 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/ClassBrowser/ClassBrowser.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)     6756 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/ClassBrowser/ClassBrowser.nib/objects.nib
--rw-r--r--   0 ronald     (501) staff       (20)     3992 2022-01-02 11:20:34.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/ClassBrowser/ClassBrowser.py
--rw-r--r--   0 ronald     (501) staff       (20)      348 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/ClassBrowser/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)      122 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/ClassBrowser/summary.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.060698 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.217960 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/Bookmarks/
--rw-r--r--   0 ronald     (501) staff       (20)      209 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/Bookmarks/Bookmarks.py
--rw-r--r--   0 ronald     (501) staff       (20)     1317 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/Bookmarks/BookmarksDocument.py
--rw-r--r--   0 ronald     (501) staff       (20)     6568 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/Bookmarks/DNDArrayController.py
--rw-r--r--   0 ronald     (501) staff       (20)      891 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/Bookmarks/DNDTableView.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.053618 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/Bookmarks/English.lproj/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.227182 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/Bookmarks/English.lproj/BookmarksDocument.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      457 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/Bookmarks/English.lproj/BookmarksDocument.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      492 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/Bookmarks/English.lproj/BookmarksDocument.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)    73726 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/Bookmarks/English.lproj/BookmarksDocument.nib/keyedobjects.nib
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.238634 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/Bookmarks/English.lproj/MainMenu.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      109 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/Bookmarks/English.lproj/MainMenu.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      605 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/Bookmarks/English.lproj/MainMenu.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)   157569 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/Bookmarks/English.lproj/MainMenu.nib/keyedobjects.nib
--rw-r--r--   0 ronald     (501) staff       (20)      569 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/Bookmarks/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)      377 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/Bookmarks/summary.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.259703 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ControlledPreferences/
--rw-r--r--   0 ronald     (501) staff       (20)      307 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ControlledPreferences/ControlledPreferences.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.054024 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ControlledPreferences/English.lproj/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.263874 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ControlledPreferences/English.lproj/MainMenu.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      580 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ControlledPreferences/English.lproj/MainMenu.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      626 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ControlledPreferences/English.lproj/MainMenu.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)   194476 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ControlledPreferences/English.lproj/MainMenu.nib/keyedobjects.nib
--rw-r--r--   0 ronald     (501) staff       (20)      862 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ControlledPreferences/FontNameToDisplayNameTransformer.py
--rw-r--r--   0 ronald     (501) staff       (20)     2244 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ControlledPreferences/FontSampleDisplayView.py
--rw-r--r--   0 ronald     (501) staff       (20)     3451 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ControlledPreferences/PreferencesPanelController.py
--rw-r--r--   0 ronald     (501) staff       (20)      279 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ControlledPreferences/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)      404 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ControlledPreferences/summary.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.270896 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/CurrencyConvBinding/
--rw-r--r--   0 ronald     (501) staff       (20)      538 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/CurrencyConvBinding/Converter.py
--rw-r--r--   0 ronald     (501) staff       (20)      218 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/CurrencyConvBinding/CurrencyConvBinding.py
--rw-r--r--   0 ronald     (501) staff       (20)      152 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/CurrencyConvBinding/CurrencyConvBindingDocument.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.054818 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/CurrencyConvBinding/English.lproj/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.285504 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/CurrencyConvBinding/English.lproj/CurrencyConvBindingDocument.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      330 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/CurrencyConvBinding/English.lproj/CurrencyConvBindingDocument.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      494 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/CurrencyConvBinding/English.lproj/CurrencyConvBindingDocument.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)    38422 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/CurrencyConvBinding/English.lproj/CurrencyConvBindingDocument.nib/keyedobjects.nib
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.288786 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/CurrencyConvBinding/English.lproj/MainMenu.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      109 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/CurrencyConvBinding/English.lproj/MainMenu.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      605 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/CurrencyConvBinding/English.lproj/MainMenu.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)   157619 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/CurrencyConvBinding/English.lproj/MainMenu.nib/keyedobjects.nib
--rw-r--r--   0 ronald     (501) staff       (20)      619 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/CurrencyConvBinding/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)      368 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/CurrencyConvBinding/summary.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.293476 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/FilteringController/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.055738 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/FilteringController/English.lproj/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.305944 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/FilteringController/English.lproj/FilteringControllerDocument.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      676 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/FilteringController/English.lproj/FilteringControllerDocument.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      627 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/FilteringController/English.lproj/FilteringControllerDocument.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)    68377 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/FilteringController/English.lproj/FilteringControllerDocument.nib/keyedobjects.nib
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.314088 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/FilteringController/English.lproj/MainMenu.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      109 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/FilteringController/English.lproj/MainMenu.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      605 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/FilteringController/English.lproj/MainMenu.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)   157619 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/FilteringController/English.lproj/MainMenu.nib/keyedobjects.nib
--rw-r--r--   0 ronald     (501) staff       (20)     2289 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/FilteringController/FilteringArrayController.py
--rw-r--r--   0 ronald     (501) staff       (20)      183 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/FilteringController/FilteringController.py
--rw-r--r--   0 ronald     (501) staff       (20)     1710 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/FilteringController/FilteringControllerDocument.py
--rw-r--r--   0 ronald     (501) staff       (20)      619 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/FilteringController/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)      312 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/FilteringController/summary.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.372881 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/GraphicsBindings/
--rw-r--r--   0 ronald     (501) staff       (20)     5040 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/GraphicsBindings/Circle.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.056718 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/GraphicsBindings/English.lproj/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.375257 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/GraphicsBindings/English.lproj/GraphicsBindingsDocument.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      756 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/GraphicsBindings/English.lproj/GraphicsBindingsDocument.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      758 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/GraphicsBindings/English.lproj/GraphicsBindingsDocument.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)   120663 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/GraphicsBindings/English.lproj/GraphicsBindingsDocument.nib/keyedobjects.nib
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.378314 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/GraphicsBindings/English.lproj/MainMenu.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      109 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/GraphicsBindings/English.lproj/MainMenu.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      605 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/GraphicsBindings/English.lproj/MainMenu.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)   157604 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/GraphicsBindings/English.lproj/MainMenu.nib/keyedobjects.nib
--rw-r--r--   0 ronald     (501) staff       (20)     2336 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/GraphicsBindings/GraphicsArrayController.py
--rw-r--r--   0 ronald     (501) staff       (20)      456 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/GraphicsBindings/GraphicsBindings.py
--rw-r--r--   0 ronald     (501) staff       (20)     3372 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/GraphicsBindings/GraphicsBindingsDocument.py
--rw-r--r--   0 ronald     (501) staff       (20)     9438 2021-10-18 19:38:40.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/GraphicsBindings/GraphicsView.py
--rw-r--r--   0 ronald     (501) staff       (20)    16141 2023-03-03 17:21:59.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/GraphicsBindings/JoystickView.py
--rw-r--r--   0 ronald     (501) staff       (20)     1007 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/GraphicsBindings/RadiansToDegreesTransformer.py
--rw-r--r--   0 ronald     (501) staff       (20)      603 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/GraphicsBindings/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)      415 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/GraphicsBindings/summary.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.399385 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ManualBindings/
--rw-r--r--   0 ronald     (501) staff       (20)     3414 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ManualBindings/AppController.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.057222 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ManualBindings/English.lproj/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.412871 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ManualBindings/English.lproj/MainMenu.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      609 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ManualBindings/English.lproj/MainMenu.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      629 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ManualBindings/English.lproj/MainMenu.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)   171877 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ManualBindings/English.lproj/MainMenu.nib/keyedobjects.nib
--rw-r--r--   0 ronald     (501) staff       (20)      165 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ManualBindings/ManualBindings.py
--rw-r--r--   0 ronald     (501) staff       (20)      265 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ManualBindings/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)      403 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ManualBindings/summary.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.421459 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/MutableTableModel/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.057707 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/MutableTableModel/English.lproj/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.426441 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/MutableTableModel/English.lproj/MainMenu.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      296 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/MutableTableModel/English.lproj/MainMenu.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      606 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/MutableTableModel/English.lproj/MainMenu.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)   154575 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/MutableTableModel/English.lproj/MainMenu.nib/keyedobjects.nib
--rw-r--r--   0 ronald     (501) staff       (20)     1012 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/MutableTableModel/TableModelAppDelegate.py
--rw-r--r--   0 ronald     (501) staff       (20)      320 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/MutableTableModel/main.py
--rw-r--r--   0 ronald     (501) staff       (20)      292 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/MutableTableModel/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       68 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/MutableTableModel/summary.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.435140 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/TableModel/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.058202 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/TableModel/English.lproj/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.439479 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/TableModel/English.lproj/MainMenu.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      206 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/TableModel/English.lproj/MainMenu.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      606 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/TableModel/English.lproj/MainMenu.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)   149621 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/TableModel/English.lproj/MainMenu.nib/keyedobjects.nib
--rw-r--r--   0 ronald     (501) staff       (20)      755 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/TableModel/TableModelAppDelegate.py
--rw-r--r--   0 ronald     (501) staff       (20)      320 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/TableModel/main.py
--rw-r--r--   0 ronald     (501) staff       (20)      285 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/TableModel/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       61 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/TableModel/summary.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.465960 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/TableModelWithSearch/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.466543 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/TableModelWithSearch/English.lproj/
--rw-r--r--   0 ronald     (501) staff       (20)      530 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/TableModelWithSearch/English.lproj/InfoPlist.strings
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.475385 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/TableModelWithSearch/English.lproj/MainMenu.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      803 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/TableModelWithSearch/English.lproj/MainMenu.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      695 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/TableModelWithSearch/English.lproj/MainMenu.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)   160860 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/TableModelWithSearch/English.lproj/MainMenu.nib/keyedobjects.nib
--rw-r--r--   0 ronald     (501) staff       (20)     1678 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/TableModelWithSearch/FilteringArrayController.py
--rw-r--r--   0 ronald     (501) staff       (20)      692 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/TableModelWithSearch/TableModelWithSearchAppDelegate.py
--rw-r--r--   0 ronald     (501) staff       (20)     4110 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/TableModelWithSearch/ToolbarCreator.py
--rw-r--r--   0 ronald     (501) staff       (20)      422 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/TableModelWithSearch/main.py
--rw-r--r--   0 ronald     (501) staff       (20)      294 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/TableModelWithSearch/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       87 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/TableModelWithSearch/summary.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.516299 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/TemperatureTransformer/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.060071 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/TemperatureTransformer/English.lproj/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.519270 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/TemperatureTransformer/English.lproj/MainMenu.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      207 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/TemperatureTransformer/English.lproj/MainMenu.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      627 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/TemperatureTransformer/English.lproj/MainMenu.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)   126518 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/TemperatureTransformer/English.lproj/MainMenu.nib/keyedobjects.nib
--rw-r--r--   0 ronald     (501) staff       (20)      182 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/TemperatureTransformer/Transformer.py
--rw-r--r--   0 ronald     (501) staff       (20)     1757 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/TemperatureTransformer/TransformerAppDelegate.py
--rw-r--r--   0 ronald     (501) staff       (20)      270 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/TemperatureTransformer/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)      289 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/TemperatureTransformer/summary.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.539317 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ToDos/
--rw-r--r--   0 ronald     (501) staff       (20)     1919 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ToDos/Category.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.061985 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ToDos/English.lproj/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.543431 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ToDos/English.lproj/MainMenu.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      109 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ToDos/English.lproj/MainMenu.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      605 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ToDos/English.lproj/MainMenu.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)   157549 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ToDos/English.lproj/MainMenu.nib/keyedobjects.nib
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.557582 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ToDos/English.lproj/ToDosDocument.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      200 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ToDos/English.lproj/ToDosDocument.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      701 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ToDos/English.lproj/ToDosDocument.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)   114048 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ToDos/English.lproj/ToDosDocument.nib/keyedobjects.nib
--rw-r--r--   0 ronald     (501) staff       (20)      679 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ToDos/OverdueTransformer.py
--rw-r--r--   0 ronald     (501) staff       (20)      987 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ToDos/PriorityToColourTransformer.py
--rw-r--r--   0 ronald     (501) staff       (20)      131 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ToDos/ToDos.py
--rw-r--r--   0 ronald     (501) staff       (20)     1586 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ToDos/ToDosDocument.py
--rw-r--r--   0 ronald     (501) staff       (20)      549 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ToDos/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)      356 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ToDos/summary.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.566447 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CurrencyConverter/
--rw-r--r--   0 ronald     (501) staff       (20)      602 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CurrencyConverter/00README.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1125 2023-03-03 17:21:59.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CurrencyConverter/CurrencyConverter.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.567432 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CurrencyConverter/English.lproj/
--rw-r--r--   0 ronald     (501) staff       (20)      492 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CurrencyConverter/English.lproj/InfoPlist.strings
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.589620 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CurrencyConverter/English.lproj/MainMenu.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      453 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CurrencyConverter/English.lproj/MainMenu.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      552 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CurrencyConverter/English.lproj/MainMenu.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)     6767 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CurrencyConverter/English.lproj/MainMenu.nib/objects.nib
--rw-r--r--   0 ronald     (501) staff       (20)      271 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CurrencyConverter/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)      109 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CurrencyConverter/summary.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.636318 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/DatePicker/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.062925 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/DatePicker/English.lproj/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.639438 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/DatePicker/English.lproj/MainMenu.nib/
--rw-r--r--   0 ronald     (501) staff       (20)     2304 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/DatePicker/English.lproj/MainMenu.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)     1021 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/DatePicker/English.lproj/MainMenu.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)    43729 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/DatePicker/English.lproj/MainMenu.nib/keyedobjects.nib
--rw-r--r--   0 ronald     (501) staff       (20)    18184 2021-10-18 19:38:40.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/DatePicker/MyWindowController.py
--rw-r--r--   0 ronald     (501) staff       (20)      853 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/DatePicker/ReadMe.txt
--rw-r--r--   0 ronald     (501) staff       (20)      100 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/DatePicker/main.py
--rw-r--r--   0 ronald     (501) staff       (20)      251 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/DatePicker/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)      233 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/DatePicker/summary.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.642342 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/DotView/
--rw-r--r--   0 ronald     (501) staff       (20)     4028 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/DotView/DotView.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.643077 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/DotView/English.lproj/
--rw-r--r--   0 ronald     (501) staff       (20)    38956 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/DotView/English.lproj/MainMenu.xib
--rw-r--r--   0 ronald     (501) staff       (20)      251 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/DotView/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)      195 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/DotView/summary.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.645502 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/DragItemAround/
--rw-r--r--   0 ronald     (501) staff       (20)     5493 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/DragItemAround/DragItemAround.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.651468 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/DragItemAround/MainMenu.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      746 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/DragItemAround/MainMenu.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      590 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/DragItemAround/MainMenu.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)    15584 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/DragItemAround/MainMenu.nib/keyedobjects.nib
--rw-r--r--   0 ronald     (501) staff       (20)      264 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/DragItemAround/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       53 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/DragItemAround/summary.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.694894 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/FieldGraph/
--rw-r--r--   0 ronald     (501) staff       (20)     5564 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/FieldGraph/CGraphController.py
--rwxr-xr-x   0 ronald     (501) staff       (20)     2763 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/FieldGraph/CGraphModel.py
--rw-r--r--   0 ronald     (501) staff       (20)     8277 2023-03-03 17:21:59.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/FieldGraph/CGraphView.py
--rw-r--r--   0 ronald     (501) staff       (20)      422 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/FieldGraph/CrossCursor.tiff
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.695383 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/FieldGraph/English.lproj/
--rw-r--r--   0 ronald     (501) staff       (20)      552 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/FieldGraph/English.lproj/InfoPlist.strings
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.699202 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/FieldGraph/English.lproj/MainMenu.nib/
--rw-r--r--   0 ronald     (501) staff       (20)     2713 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/FieldGraph/English.lproj/MainMenu.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      655 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/FieldGraph/English.lproj/MainMenu.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)    25867 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/FieldGraph/English.lproj/MainMenu.nib/keyedobjects.nib
--rw-r--r--   0 ronald     (501) staff       (20)    13374 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/FieldGraph/English.lproj/MainMenu.nib/objects.nib
--rw-r--r--   0 ronald     (501) staff       (20)      163 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/FieldGraph/Main.py
--rw-r--r--   0 ronald     (501) staff       (20)   769739 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/FieldGraph/Map.png
--rw-r--r--   0 ronald     (501) staff       (20)      541 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/FieldGraph/fieldMath.py
--rw-r--r--   0 ronald     (501) staff       (20)      363 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/FieldGraph/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)      207 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/FieldGraph/summary.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.711051 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Formatter/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.714094 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Formatter/MainMenu.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      199 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Formatter/MainMenu.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      626 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Formatter/MainMenu.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)   120511 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Formatter/MainMenu.nib/keyedobjects.nib
--rw-r--r--   0 ronald     (501) staff       (20)      639 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Formatter/main.py
--rw-r--r--   0 ronald     (501) staff       (20)      249 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Formatter/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       75 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Formatter/summary.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.741801 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Grady/
--rw-r--r--   0 ronald     (501) staff       (20)      858 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Grady/AppDelegate.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.065172 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Grady/English.lproj/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.748520 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Grady/English.lproj/MainMenu.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      408 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Grady/English.lproj/MainMenu.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      565 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Grady/English.lproj/MainMenu.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)    13462 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Grady/English.lproj/MainMenu.nib/keyedobjects.nib
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.752836 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Grady/English.lproj/TestWindow.nib/
--rw-r--r--   0 ronald     (501) staff       (20)     1543 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Grady/English.lproj/TestWindow.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      454 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Grady/English.lproj/TestWindow.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)     8580 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Grady/English.lproj/TestWindow.nib/keyedobjects.nib
--rw-r--r--   0 ronald     (501) staff       (20)     2011 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Grady/MyBaseGradientView.py
--rw-r--r--   0 ronald     (501) staff       (20)      735 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Grady/MyBezierGradientView.py
--rw-r--r--   0 ronald     (501) staff       (20)      672 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Grady/MyRectGradientView.py
--rw-r--r--   0 ronald     (501) staff       (20)     3593 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Grady/MyWindowController.py
--rw-r--r--   0 ronald     (501) staff       (20)      255 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Grady/main.py
--rw-r--r--   0 ronald     (501) staff       (20)      246 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Grady/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       46 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Grady/summary.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.764506 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/PredicateEditorSample/
--rw-r--r--   0 ronald     (501) staff       (20)      784 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/PredicateEditorSample/CaseInsensitivePredicateTemplate.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.766415 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/PredicateEditorSample/English.lproj/
--rw-r--r--   0 ronald     (501) staff       (20)      328 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/PredicateEditorSample/English.lproj/Credits.rtf
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.771255 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/PredicateEditorSample/English.lproj/MainMenu.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      793 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/PredicateEditorSample/English.lproj/MainMenu.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      583 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/PredicateEditorSample/English.lproj/MainMenu.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)    42827 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/PredicateEditorSample/English.lproj/MainMenu.nib/keyedobjects.nib
--rw-r--r--   0 ronald     (501) staff       (20)    13274 2023-03-03 17:21:59.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/PredicateEditorSample/MyWindowController.py
--rw-r--r--   0 ronald     (501) staff       (20)     1744 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/PredicateEditorSample/ReadMe.txt
--rw-r--r--   0 ronald     (501) staff       (20)      154 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/PredicateEditorSample/main.py
--rw-r--r--   0 ronald     (501) staff       (20)      262 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/PredicateEditorSample/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)      386 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/PredicateEditorSample/summary.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.879867 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/PyInterpreter/
--rw-r--r--   0 ronald     (501) staff       (20)     1088 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/PyInterpreter/LICENSE.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.883709 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/PyInterpreter/PyInterpreter.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      549 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/PyInterpreter/PyInterpreter.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      585 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/PyInterpreter/PyInterpreter.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)    13395 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/PyInterpreter/PyInterpreter.nib/keyedobjects.nib
--rw-r--r--   0 ronald     (501) staff       (20)    18012 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/PyInterpreter/PyInterpreter.py
--rw-r--r--   0 ronald     (501) staff       (20)      439 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/PyInterpreter/README.txt
--rw-r--r--   0 ronald     (501) staff       (20)      353 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/PyInterpreter/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)      180 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/PyInterpreter/summary.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.889110 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/PythonBrowser/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.896101 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/PythonBrowser/MainMenu.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      471 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/PythonBrowser/MainMenu.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      561 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/PythonBrowser/MainMenu.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)     4884 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/PythonBrowser/MainMenu.nib/objects.nib
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.902594 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/PythonBrowser/PythonBrowser.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      313 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/PythonBrowser/PythonBrowser.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      450 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/PythonBrowser/PythonBrowser.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)     2035 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/PythonBrowser/PythonBrowser.nib/objects.nib
--rw-r--r--   0 ronald     (501) staff       (20)     3833 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/PythonBrowser/PythonBrowser.py
--rw-r--r--   0 ronald     (501) staff       (20)     5898 2021-10-18 19:38:40.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/PythonBrowser/PythonBrowserModel.py
--rw-r--r--   0 ronald     (501) staff       (20)      890 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/PythonBrowser/readme.txt
--rw-r--r--   0 ronald     (501) staff       (20)      257 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/PythonBrowser/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)      173 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/PythonBrowser/summary.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.914987 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/RoundTransparentWindow/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.919240 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/RoundTransparentWindow/MainMenu.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      699 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/RoundTransparentWindow/MainMenu.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      493 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/RoundTransparentWindow/MainMenu.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)     4124 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/RoundTransparentWindow/MainMenu.nib/objects.nib
--rw-r--r--   0 ronald     (501) staff       (20)     3829 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/RoundTransparentWindow/RoundTransparentWindow.py
--rw-r--r--   0 ronald     (501) staff       (20)   130322 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/RoundTransparentWindow/circle.tif
--rw-r--r--   0 ronald     (501) staff       (20)   107760 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/RoundTransparentWindow/pentagram.tif
--rw-r--r--   0 ronald     (501) staff       (20)      276 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/RoundTransparentWindow/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       51 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/RoundTransparentWindow/summary.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.927924 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/SimpleService/
--rw-r--r--   0 ronald     (501) staff       (20)     1588 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/SimpleService/README.rtf
--rw-r--r--   0 ronald     (501) staff       (20)     2816 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/SimpleService/ServiceTest.py
--rw-r--r--   0 ronald     (501) staff       (20)      325 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/SimpleService/SimpleService_main.py
--rwxr-xr-x   0 ronald     (501) staff       (20)      116 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/SimpleService/rebuild.py
--rw-r--r--   0 ronald     (501) staff       (20)     1001 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/SimpleService/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       54 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/SimpleService/summary.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.942667 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/TableModel/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.067360 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/TableModel/English.lproj/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.944988 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/TableModel/English.lproj/MainMenu.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      294 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/TableModel/English.lproj/MainMenu.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      586 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/TableModel/English.lproj/MainMenu.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)     6659 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/TableModel/English.lproj/MainMenu.nib/objects.nib
--rw-r--r--   0 ronald     (501) staff       (20)     3679 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/TableModel/TableModel.py
--rw-r--r--   0 ronald     (501) staff       (20)      314 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/TableModel/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       55 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/TableModel/summary.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.947293 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/TinyTinyEdit/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.954328 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/TinyTinyEdit/MainMenu.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      109 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/TinyTinyEdit/MainMenu.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      484 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/TinyTinyEdit/MainMenu.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)     7340 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/TinyTinyEdit/MainMenu.nib/objects.nib
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.956011 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/TinyTinyEdit/TinyTinyDocument.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      289 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/TinyTinyEdit/TinyTinyDocument.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      451 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/TinyTinyEdit/TinyTinyDocument.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)     1694 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/TinyTinyEdit/TinyTinyDocument.nib/objects.nib
--rw-r--r--   0 ronald     (501) staff       (20)     1180 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/TinyTinyEdit/TinyTinyEdit.py
--rw-r--r--   0 ronald     (501) staff       (20)      596 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/TinyTinyEdit/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       50 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/TinyTinyEdit/summary.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.977321 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/TinyURLService/
--rw-r--r--   0 ronald     (501) staff       (20)     1366 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/TinyURLService/README.rtf
--rw-r--r--   0 ronald     (501) staff       (20)     2574 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/TinyURLService/TinyURLService.py
--rwxr-xr-x   0 ronald     (501) staff       (20)      116 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/TinyURLService/rebuild.py
--rw-r--r--   0 ronald     (501) staff       (20)      688 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/TinyURLService/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)      105 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/TinyURLService/summary.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.991310 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Todo/
--rw-r--r--   0 ronald     (501) staff       (20)      784 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Todo/00ReadMe.txt
--rw-r--r--   0 ronald     (501) staff       (20)     5449 2023-03-03 17:21:59.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Todo/CalendarMatrix.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:17:00.024078 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Todo/English.lproj/
--rw-r--r--   0 ronald     (501) staff       (20)      436 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Todo/English.lproj/Credits.rtf
--rw-r--r--   0 ronald     (501) staff       (20)      416 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Todo/English.lproj/InfoPlist.strings
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:17:00.032544 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Todo/English.lproj/MainMenu.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      286 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Todo/English.lproj/MainMenu.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      243 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Todo/English.lproj/MainMenu.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)     5115 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Todo/English.lproj/MainMenu.nib/objects.nib
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:17:00.034587 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Todo/English.lproj/ToDoDocument.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      791 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Todo/English.lproj/ToDoDocument.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      422 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Todo/English.lproj/ToDoDocument.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)     4408 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Todo/English.lproj/ToDoDocument.nib/objects.nib
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:17:00.036542 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Todo/English.lproj/ToDoInfoWindow.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      980 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Todo/English.lproj/ToDoInfoWindow.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      596 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Todo/English.lproj/ToDoInfoWindow.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)     9393 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Todo/English.lproj/ToDoInfoWindow.nib/objects.nib
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:17:00.038898 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Todo/Icons/
--rw-r--r--   0 ronald     (501) staff       (20)    48041 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Todo/Icons/ToDoApp.icns
--rw-r--r--   0 ronald     (501) staff       (20)    50278 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Todo/Icons/ToDoDoc.icns
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:17:00.043326 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Todo/Images/
--rw-r--r--   0 ronald     (501) staff       (20)      422 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Todo/Images/DeferredMark.tiff
--rw-r--r--   0 ronald     (501) staff       (20)      412 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Todo/Images/DoneMark.tiff
--rw-r--r--   0 ronald     (501) staff       (20)      412 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Todo/Images/LeftArrow.tiff
--rw-r--r--   0 ronald     (501) staff       (20)      422 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Todo/Images/RightArrow.tiff
--rw-r--r--   0 ronald     (501) staff       (20)    11377 2023-03-03 17:21:59.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Todo/InfoWindowController.py
--rw-r--r--   0 ronald     (501) staff       (20)      674 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Todo/SelectionNotifyMatrix.py
--rw-r--r--   0 ronald     (501) staff       (20)     2304 2023-03-03 17:21:59.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Todo/ToDoCell.py
--rw-r--r--   0 ronald     (501) staff       (20)    11589 2023-03-03 17:21:59.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Todo/ToDoDocument.py
--rw-r--r--   0 ronald     (501) staff       (20)     4676 2023-03-03 17:21:59.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Todo/ToDoItem.py
--rw-r--r--   0 ronald     (501) staff       (20)      263 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Todo/TodoAppDelegate.py
--rw-r--r--   0 ronald     (501) staff       (20)      390 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Todo/main.py
--rw-r--r--   0 ronald     (501) staff       (20)      926 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Todo/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)      251 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Todo/summary.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:17:00.069605 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/WebServicesTool/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:17:00.071954 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/WebServicesTool/English.lproj/
--rw-r--r--   0 ronald     (501) staff       (20)      456 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/WebServicesTool/English.lproj/InfoPlist.strings
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:17:00.075626 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/WebServicesTool/English.lproj/MainMenu.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      304 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/WebServicesTool/English.lproj/MainMenu.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      484 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/WebServicesTool/English.lproj/MainMenu.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)     9289 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/WebServicesTool/English.lproj/MainMenu.nib/keyedobjects.nib
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:17:00.080408 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/WebServicesTool/English.lproj/WSTConnection.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      626 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/WebServicesTool/English.lproj/WSTConnection.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      585 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/WebServicesTool/English.lproj/WSTConnection.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)     8150 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/WebServicesTool/English.lproj/WSTConnection.nib/keyedobjects.nib
--rw-r--r--   0 ronald     (501) staff       (20)     1088 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/WebServicesTool/LICENSE.txt
--rw-r--r--   0 ronald     (501) staff       (20)      252 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/WebServicesTool/Main.py
--rw-r--r--   0 ronald     (501) staff       (20)     1956 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/WebServicesTool/Preferences.png
--rw-r--r--   0 ronald     (501) staff       (20)      735 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/WebServicesTool/README.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1623 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/WebServicesTool/Reload.png
--rw-r--r--   0 ronald     (501) staff       (20)    52383 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/WebServicesTool/WST.icns
--rw-r--r--   0 ronald     (501) staff       (20)    18131 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/WebServicesTool/WST.png
--rw-r--r--   0 ronald     (501) staff       (20)     1106 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/WebServicesTool/WSTApplicationDelegateClass.py
--rw-r--r--   0 ronald     (501) staff       (20)    18766 2021-10-18 19:38:40.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/WebServicesTool/WSTConnectionWindowControllerClass.py
--rw-r--r--   0 ronald     (501) staff       (20)      419 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/WebServicesTool/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)      191 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/WebServicesTool/summary.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.100569 pyobjc-framework-Cocoa-9.1b1/Examples/Foundation/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:17:00.104440 pyobjc-framework-Cocoa-9.1b1/Examples/Foundation/Scripts/
--rw-r--r--   0 ronald     (501) staff       (20)     1102 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/Foundation/Scripts/dictionary.py
--rw-r--r--   0 ronald     (501) staff       (20)     1266 2023-03-03 17:21:59.000000 pyobjc-framework-Cocoa-9.1b1/Examples/Foundation/Scripts/findPython.py
--rw-r--r--   0 ronald     (501) staff       (20)      500 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/Foundation/Scripts/pydict-to-objcdict.py
--rw-r--r--   0 ronald     (501) staff       (20)     2380 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.1b1/Examples/Foundation/Scripts/rendezvous.py
--rw-r--r--   0 ronald     (501) staff       (20)     1264 2022-02-06 09:24:04.000000 pyobjc-framework-Cocoa-9.1b1/Examples/Foundation/Scripts/simple-kvo.py
--rw-r--r--   0 ronald     (501) staff       (20)      501 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.1b1/Examples/Foundation/Scripts/super-call.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.103790 pyobjc-framework-Cocoa-9.1b1/Examples/OpenGL/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:17:00.158228 pyobjc-framework-Cocoa-9.1b1/Examples/OpenGL/OpenGLDemo/
--rw-r--r--   0 ronald     (501) staff       (20)     1088 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/OpenGL/OpenGLDemo/LICENSE.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:17:00.163452 pyobjc-framework-Cocoa-9.1b1/Examples/OpenGL/OpenGLDemo/OpenGLDemo.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      294 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/OpenGL/OpenGLDemo/OpenGLDemo.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      589 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/OpenGL/OpenGLDemo/OpenGLDemo.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)     4395 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/OpenGL/OpenGLDemo/OpenGLDemo.nib/objects.nib
--rw-r--r--   0 ronald     (501) staff       (20)     2257 2022-10-18 09:53:23.000000 pyobjc-framework-Cocoa-9.1b1/Examples/OpenGL/OpenGLDemo/OpenGLDemo.py
--rw-r--r--   0 ronald     (501) staff       (20)      403 2023-02-19 10:50:34.000000 pyobjc-framework-Cocoa-9.1b1/Examples/OpenGL/OpenGLDemo/README.txt
--rw-r--r--   0 ronald     (501) staff       (20)      352 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/OpenGL/OpenGLDemo/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)      225 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/OpenGL/OpenGLDemo/summary.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:17:00.165934 pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/
--rw-r--r--   0 ronald     (501) staff       (20)      120 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/README.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:17:00.216483 pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:17:00.258036 pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool/English.lproj/
--rw-r--r--   0 ronald     (501) staff       (20)      456 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool/English.lproj/InfoPlist.strings
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:17:00.264231 pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool/English.lproj/MainMenu.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      304 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool/English.lproj/MainMenu.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      484 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool/English.lproj/MainMenu.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)     9289 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool/English.lproj/MainMenu.nib/keyedobjects.nib
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:17:00.299815 pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool/English.lproj/WSTConnection.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      626 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool/English.lproj/WSTConnection.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      585 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool/English.lproj/WSTConnection.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)     8150 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool/English.lproj/WSTConnection.nib/keyedobjects.nib
--rw-r--r--   0 ronald     (501) staff       (20)     1088 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool/LICENSE.txt
--rw-r--r--   0 ronald     (501) staff       (20)      302 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool/Main.py
--rw-r--r--   0 ronald     (501) staff       (20)     1956 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool/Preferences.png
--rw-r--r--   0 ronald     (501) staff       (20)     1169 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool/ReadMe.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1623 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool/Reload.png
--rw-r--r--   0 ronald     (501) staff       (20)    52383 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool/WST.icns
--rw-r--r--   0 ronald     (501) staff       (20)    18131 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool/WST.png
--rw-r--r--   0 ronald     (501) staff       (20)     1423 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool/WSTApplicationDelegateClass.py
--rw-r--r--   0 ronald     (501) staff       (20)    16508 2023-03-03 17:21:59.000000 pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool/WSTConnectionWindowControllerClass.py
--rw-r--r--   0 ronald     (501) staff       (20)      419 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)      105 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool/summary.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:17:00.252171 pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool-CocoaBindings/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:17:00.252911 pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool-CocoaBindings/English.lproj/
--rw-r--r--   0 ronald     (501) staff       (20)      456 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool-CocoaBindings/English.lproj/InfoPlist.strings
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:17:00.255122 pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool-CocoaBindings/English.lproj/MainMenu.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      304 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool-CocoaBindings/English.lproj/MainMenu.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      484 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool-CocoaBindings/English.lproj/MainMenu.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)     9289 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool-CocoaBindings/English.lproj/MainMenu.nib/keyedobjects.nib
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:17:00.257154 pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool-CocoaBindings/English.lproj/WSTConnection.nib/
--rw-r--r--   0 ronald     (501) staff       (20)      626 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool-CocoaBindings/English.lproj/WSTConnection.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      585 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool-CocoaBindings/English.lproj/WSTConnection.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)     9876 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool-CocoaBindings/English.lproj/WSTConnection.nib/keyedobjects.nib
--rw-r--r--   0 ronald     (501) staff       (20)     1088 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool-CocoaBindings/LICENSE.txt
--rw-r--r--   0 ronald     (501) staff       (20)      302 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool-CocoaBindings/Main.py
--rw-r--r--   0 ronald     (501) staff       (20)     1956 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool-CocoaBindings/Preferences.png
--rw-r--r--   0 ronald     (501) staff       (20)     1083 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool-CocoaBindings/README.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1050 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool-CocoaBindings/RPCMethod.py
--rw-r--r--   0 ronald     (501) staff       (20)     1623 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool-CocoaBindings/Reload.png
--rw-r--r--   0 ronald     (501) staff       (20)    52383 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool-CocoaBindings/WST.icns
--rw-r--r--   0 ronald     (501) staff       (20)    18131 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool-CocoaBindings/WST.png
--rw-r--r--   0 ronald     (501) staff       (20)     1390 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool-CocoaBindings/WSTApplicationDelegateClass.py
--rw-r--r--   0 ronald     (501) staff       (20)    14871 2021-10-18 19:38:40.000000 pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool-CocoaBindings/WSTConnectionWindowControllerClass.py
--rw-r--r--   0 ronald     (501) staff       (20)      362 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool-CocoaBindings/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)      137 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool-CocoaBindings/summary.txt
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-Cocoa-9.1b1/LICENSE.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:16:59.115352 pyobjc-framework-Cocoa-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:17:00.318093 pyobjc-framework-Cocoa-9.1b1/Lib/AppKit/
--rw-r--r--   0 ronald     (501) staff       (20)     5010 2022-01-02 11:04:26.000000 pyobjc-framework-Cocoa-9.1b1/Lib/AppKit/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)   871462 2023-03-24 18:54:07.000000 pyobjc-framework-Cocoa-9.1b1/Lib/AppKit/_metadata.py
--rw-r--r--   0 ronald     (501) staff       (20)      650 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.1b1/Lib/AppKit/_nsapp.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:17:00.345321 pyobjc-framework-Cocoa-9.1b1/Lib/CGL/
--rw-r--r--   0 ronald     (501) staff       (20)     7034 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Lib/CGL/PyObjC.bridgesupport
--rw-r--r--   0 ronald     (501) staff       (20)      432 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Lib/CGL/__init__.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:17:00.346724 pyobjc-framework-Cocoa-9.1b1/Lib/Cocoa/
--rw-r--r--   0 ronald     (501) staff       (20)      534 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Lib/Cocoa/__init__.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:17:00.418552 pyobjc-framework-Cocoa-9.1b1/Lib/CoreFoundation/
--rw-r--r--   0 ronald     (501) staff       (20)     1076 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.1b1/Lib/CoreFoundation/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)   154013 2023-03-24 18:54:07.000000 pyobjc-framework-Cocoa-9.1b1/Lib/CoreFoundation/_metadata.py
--rw-r--r--   0 ronald     (501) staff       (20)     2880 2021-10-18 19:38:40.000000 pyobjc-framework-Cocoa-9.1b1/Lib/CoreFoundation/_static.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:17:00.426982 pyobjc-framework-Cocoa-9.1b1/Lib/Foundation/
--rw-r--r--   0 ronald     (501) staff       (20)     5761 2022-02-06 09:24:04.000000 pyobjc-framework-Cocoa-9.1b1/Lib/Foundation/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)      713 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.1b1/Lib/Foundation/_context.py
--rw-r--r--   0 ronald     (501) staff       (20)     1404 2021-08-04 10:13:27.000000 pyobjc-framework-Cocoa-9.1b1/Lib/Foundation/_functiondefines.py
--rw-r--r--   0 ronald     (501) staff       (20)   441138 2023-03-24 18:54:07.000000 pyobjc-framework-Cocoa-9.1b1/Lib/Foundation/_metadata.py
--rw-r--r--   0 ronald     (501) staff       (20)      394 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Lib/Foundation/_nsindexset.py
--rw-r--r--   0 ronald     (501) staff       (20)     8402 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Lib/Foundation/_nsobject.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:17:00.431627 pyobjc-framework-Cocoa-9.1b1/Lib/PyObjCTools/
--rw-r--r--   0 ronald     (501) staff       (20)      840 2021-10-18 19:38:40.000000 pyobjc-framework-Cocoa-9.1b1/Lib/PyObjCTools/AppCategories.py
--rw-r--r--   0 ronald     (501) staff       (20)     9669 2023-03-03 17:21:59.000000 pyobjc-framework-Cocoa-9.1b1/Lib/PyObjCTools/AppHelper.py
--rw-r--r--   0 ronald     (501) staff       (20)     7913 2022-10-29 10:49:37.000000 pyobjc-framework-Cocoa-9.1b1/Lib/PyObjCTools/Conversion.py
--rw-r--r--   0 ronald     (501) staff       (20)     1026 2021-10-18 19:38:40.000000 pyobjc-framework-Cocoa-9.1b1/Lib/PyObjCTools/FndCategories.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:17:00.449519 pyobjc-framework-Cocoa-9.1b1/Lib/pyobjc_framework_Cocoa.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2178 2023-03-26 11:16:59.000000 pyobjc-framework-Cocoa-9.1b1/Lib/pyobjc_framework_Cocoa.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)    40071 2023-03-26 11:16:59.000000 pyobjc-framework-Cocoa-9.1b1/Lib/pyobjc_framework_Cocoa.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:16:58.000000 pyobjc-framework-Cocoa-9.1b1/Lib/pyobjc_framework_Cocoa.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:28.000000 pyobjc-framework-Cocoa-9.1b1/Lib/pyobjc_framework_Cocoa.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       19 2023-03-26 11:16:58.000000 pyobjc-framework-Cocoa-9.1b1/Lib/pyobjc_framework_Cocoa.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       62 2023-03-26 11:16:58.000000 pyobjc-framework-Cocoa-9.1b1/Lib/pyobjc_framework_Cocoa.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/MANIFEST.in
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:17:00.564243 pyobjc-framework-Cocoa-9.1b1/Modules/
--rw-r--r--   0 ronald     (501) staff       (20)     1233 2022-10-18 09:53:23.000000 pyobjc-framework-Cocoa-9.1b1/Modules/_AppKit.m
--rw-r--r--   0 ronald     (501) staff       (20)     2793 2021-09-25 15:02:56.000000 pyobjc-framework-Cocoa-9.1b1/Modules/_AppKit_appmain.m
--rw-r--r--   0 ronald     (501) staff       (20)      204 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.1b1/Modules/_AppKit_carbon.m
--rw-r--r--   0 ronald     (501) staff       (20)     1603 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.1b1/Modules/_AppKit_inlines.m
--rw-r--r--   0 ronald     (501) staff       (20)     9531 2022-10-18 09:53:23.000000 pyobjc-framework-Cocoa-9.1b1/Modules/_AppKit_nsbezierpath.m
--rw-r--r--   0 ronald     (501) staff       (20)    15908 2022-02-17 10:15:09.000000 pyobjc-framework-Cocoa-9.1b1/Modules/_AppKit_nsbitmap.m
--rw-r--r--   0 ronald     (501) staff       (20)     3071 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.1b1/Modules/_AppKit_nsfont.m
--rw-r--r--   0 ronald     (501) staff       (20)     1918 2022-01-02 11:04:26.000000 pyobjc-framework-Cocoa-9.1b1/Modules/_AppKit_nsview.m
--rw-r--r--   0 ronald     (501) staff       (20)    11805 2022-06-15 11:57:00.000000 pyobjc-framework-Cocoa-9.1b1/Modules/_AppKit_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     2882 2021-10-26 08:03:21.000000 pyobjc-framework-Cocoa-9.1b1/Modules/_CoreFoundation.m
--rw-r--r--   0 ronald     (501) staff       (20)     2822 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.1b1/Modules/_CoreFoundation_CFBag.m
--rw-r--r--   0 ronald     (501) staff       (20)     2803 2021-10-18 19:38:40.000000 pyobjc-framework-Cocoa-9.1b1/Modules/_CoreFoundation_CFBinaryHeap.m
--rw-r--r--   0 ronald     (501) staff       (20)     2449 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.1b1/Modules/_CoreFoundation_CFBitVector.m
--rw-r--r--   0 ronald     (501) staff       (20)    12276 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Modules/_CoreFoundation_CFCalendar.m
--rw-r--r--   0 ronald     (501) staff       (20)     2568 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Modules/_CoreFoundation_CFDictionary.m
--rw-r--r--   0 ronald     (501) staff       (20)     4883 2021-10-26 08:03:21.000000 pyobjc-framework-Cocoa-9.1b1/Modules/_CoreFoundation_CFFileDescriptor.m
--rw-r--r--   0 ronald     (501) staff       (20)    11008 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Modules/_CoreFoundation_CFMachPort.m
--rw-r--r--   0 ronald     (501) staff       (20)     4939 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Modules/_CoreFoundation_CFMessagePort.m
--rw-r--r--   0 ronald     (501) staff       (20)     6619 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Modules/_CoreFoundation_CFNumber.m
--rw-r--r--   0 ronald     (501) staff       (20)     8015 2021-10-18 19:38:40.000000 pyobjc-framework-Cocoa-9.1b1/Modules/_CoreFoundation_CFNumberFormatter.m
--rw-r--r--   0 ronald     (501) staff       (20)     3070 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Modules/_CoreFoundation_CFReadStream.m
--rw-r--r--   0 ronald     (501) staff       (20)     4902 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Modules/_CoreFoundation_CFRunLoopObserver.m
--rw-r--r--   0 ronald     (501) staff       (20)     6424 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Modules/_CoreFoundation_CFRunLoopSource.m
--rw-r--r--   0 ronald     (501) staff       (20)     4777 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Modules/_CoreFoundation_CFRunLoopTimer.m
--rw-r--r--   0 ronald     (501) staff       (20)     1527 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Modules/_CoreFoundation_CFSet.m
--rw-r--r--   0 ronald     (501) staff       (20)    11376 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Modules/_CoreFoundation_CFSocket.m
--rw-r--r--   0 ronald     (501) staff       (20)     6203 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Modules/_CoreFoundation_CFTree.m
--rw-r--r--   0 ronald     (501) staff       (20)     2904 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/Modules/_CoreFoundation_CFWriteStream.m
--rw-r--r--   0 ronald     (501) staff       (20)     4309 2021-10-18 19:38:40.000000 pyobjc-framework-Cocoa-9.1b1/Modules/_CoreFoundation_inlines.m
--rw-r--r--   0 ronald     (501) staff       (20)     1033 2022-10-18 09:53:23.000000 pyobjc-framework-Cocoa-9.1b1/Modules/_Foundation.m
--rw-r--r--   0 ronald     (501) staff       (20)     6519 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.1b1/Modules/_Foundation_inlines.m
--rw-r--r--   0 ronald     (501) staff       (20)     4024 2022-01-02 11:04:26.000000 pyobjc-framework-Cocoa-9.1b1/Modules/_Foundation_netservice.m
--rw-r--r--   0 ronald     (501) staff       (20)     4088 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.1b1/Modules/_Foundation_protocols.m
--rw-r--r--   0 ronald     (501) staff       (20)     4882 2023-03-03 17:21:31.000000 pyobjc-framework-Cocoa-9.1b1/Modules/_Foundation_string.m
--rw-r--r--   0 ronald     (501) staff       (20)     3230 2021-10-18 19:38:40.000000 pyobjc-framework-Cocoa-9.1b1/Modules/_Foundation_typecode.m
--rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:34.000000 pyobjc-framework-Cocoa-9.1b1/Modules/pyobjc-api.h
--rw-r--r--   0 ronald     (501) staff       (20)    12869 2023-03-03 17:21:31.000000 pyobjc-framework-Cocoa-9.1b1/Modules/pyobjc-compat.h
--rw-r--r--   0 ronald     (501) staff       (20)     7419 2021-10-18 19:38:40.000000 pyobjc-framework-Cocoa-9.1b1/Modules/testhelper.m
--rw-r--r--   0 ronald     (501) staff       (20)     1967 2023-03-26 11:17:02.749435 pyobjc-framework-Cocoa-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:17:01.856789 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     3880 2023-03-03 17:21:59.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/guitest_graphics.py
--rw-r--r--   0 ronald     (501) staff       (20)      962 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/guitest_nsalert.py
--rw-r--r--   0 ronald     (501) staff       (20)      580 2022-01-02 11:04:26.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_appcategories.py
--rw-r--r--   0 ronald     (501) staff       (20)      563 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_apphelper.py
--rw-r--r--   0 ronald     (501) staff       (20)     4323 2022-06-25 20:11:26.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_appkit_protocols.py
--rw-r--r--   0 ronald     (501) staff       (20)     2151 2023-03-24 18:54:07.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_appkiterrors.py
--rw-r--r--   0 ronald     (501) staff       (20)     8801 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfarray.py
--rw-r--r--   0 ronald     (501) staff       (20)     5741 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfattributedstring.py
--rw-r--r--   0 ronald     (501) staff       (20)     5237 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfbag.py
--rw-r--r--   0 ronald     (501) staff       (20)    13234 2022-01-02 11:04:26.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfbase.py
--rw-r--r--   0 ronald     (501) staff       (20)     4755 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfbinaryheap.py
--rw-r--r--   0 ronald     (501) staff       (20)     4871 2021-04-09 10:15:21.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfbitvector.py
--rw-r--r--   0 ronald     (501) staff       (20)    14577 2022-06-26 21:30:10.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfbundle.py
--rw-r--r--   0 ronald     (501) staff       (20)     4356 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfbyteorder.py
--rw-r--r--   0 ronald     (501) staff       (20)    10072 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfcalendar.py
--rw-r--r--   0 ronald     (501) staff       (20)     1775 2022-07-30 15:06:02.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfcgtypes.py
--rw-r--r--   0 ronald     (501) staff       (20)     7834 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfcharacterset.py
--rw-r--r--   0 ronald     (501) staff       (20)     4857 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfdata.py
--rw-r--r--   0 ronald     (501) staff       (20)     5004 2023-03-25 14:19:27.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfdate.py
--rw-r--r--   0 ronald     (501) staff       (20)     9313 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfdateformatter.py
--rw-r--r--   0 ronald     (501) staff       (20)     6802 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfdictionary.py
--rw-r--r--   0 ronald     (501) staff       (20)     4582 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cferror.py
--rw-r--r--   0 ronald     (501) staff       (20)     1730 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cffiledescriptor.py
--rw-r--r--   0 ronald     (501) staff       (20)     4322 2022-10-29 10:34:19.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cffilesecurity.py
--rw-r--r--   0 ronald     (501) staff       (20)     7526 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cflocale.py
--rw-r--r--   0 ronald     (501) staff       (20)     2759 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfmachport.py
--rw-r--r--   0 ronald     (501) staff       (20)     4714 2021-06-07 08:31:49.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfmessageport.py
--rw-r--r--   0 ronald     (501) staff       (20)     5044 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfnotificationcenter.py
--rw-r--r--   0 ronald     (501) staff       (20)    10473 2022-01-02 11:04:26.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfnumber.py
--rw-r--r--   0 ronald     (501) staff       (20)     8538 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfnumberformatter.py
--rw-r--r--   0 ronald     (501) staff       (20)     1760 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfplugin.py
--rw-r--r--   0 ronald     (501) staff       (20)     6687 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfpreferences.py
--rw-r--r--   0 ronald     (501) staff       (20)     6541 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfpropertylist.py
--rw-r--r--   0 ronald     (501) staff       (20)    15035 2021-04-09 10:15:21.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfrunloop.py
--rw-r--r--   0 ronald     (501) staff       (20)     4969 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfset.py
--rw-r--r--   0 ronald     (501) staff       (20)     9224 2022-01-02 11:04:26.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfsocket.py
--rw-r--r--   0 ronald     (501) staff       (20)    22990 2023-03-03 17:21:59.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfstream.py
--rw-r--r--   0 ronald     (501) staff       (20)    34773 2023-03-24 18:54:07.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfstring.py
--rw-r--r--   0 ronald     (501) staff       (20)     3352 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfstringtokenizer.py
--rw-r--r--   0 ronald     (501) staff       (20)     5420 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cftimezone.py
--rw-r--r--   0 ronald     (501) staff       (20)     5171 2022-01-02 11:04:26.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cftree.py
--rw-r--r--   0 ronald     (501) staff       (20)    36145 2023-02-19 10:50:34.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfurl.py
--rw-r--r--   0 ronald     (501) staff       (20)     3938 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfurlaccess.py
--rw-r--r--   0 ronald     (501) staff       (20)     2937 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfurlenumerator.py
--rw-r--r--   0 ronald     (501) staff       (20)     6328 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfusernotification.py
--rw-r--r--   0 ronald     (501) staff       (20)     6022 2022-01-02 11:04:26.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfuuid.py
--rw-r--r--   0 ronald     (501) staff       (20)     4590 2022-01-02 11:04:26.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfxmlnode.py
--rw-r--r--   0 ronald     (501) staff       (20)     2797 2021-04-09 10:15:21.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfxmlparser.py
--rw-r--r--   0 ronald     (501) staff       (20)      967 2023-03-25 14:19:40.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cocoa.py
--rw-r--r--   0 ronald     (501) staff       (20)      874 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_constants.py
--rw-r--r--   0 ronald     (501) staff       (20)      994 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_convenience.py
--rw-r--r--   0 ronald     (501) staff       (20)     9051 2023-03-03 17:21:59.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_conversion.py
--rw-r--r--   0 ronald     (501) staff       (20)      466 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_fndcategories.py
--rw-r--r--   0 ronald     (501) staff       (20)     2253 2022-01-02 11:04:26.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_foundation.py
--rw-r--r--   0 ronald     (501) staff       (20)     6646 2022-06-23 11:03:28.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_foundationerrors.py
--rw-r--r--   0 ronald     (501) staff       (20)     4058 2023-03-03 17:21:59.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_globals.py
--rw-r--r--   0 ronald     (501) staff       (20)    21275 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_keyvalue.py
--rw-r--r--   0 ronald     (501) staff       (20)    34718 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsaccessibility.py
--rw-r--r--   0 ronald     (501) staff       (20)      822 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsaccessibilitycustomaction.py
--rw-r--r--   0 ronald     (501) staff       (20)     2335 2022-06-25 20:12:49.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsaccessibilitycustomrotor.py
--rw-r--r--   0 ronald     (501) staff       (20)    27068 2022-06-25 20:06:25.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsaccessibilityprotocols.py
--rw-r--r--   0 ronald     (501) staff       (20)      478 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsactioncell.py
--rw-r--r--   0 ronald     (501) staff       (20)     7307 2022-01-02 11:04:26.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsaffinetransform.py
--rw-r--r--   0 ronald     (501) staff       (20)     2233 2022-06-25 09:07:01.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsalert.py
--rw-r--r--   0 ronald     (501) staff       (20)      254 2022-06-25 20:11:55.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsalignmentfeedbackfilter.py
--rw-r--r--   0 ronald     (501) staff       (20)     2574 2022-06-25 09:02:27.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsanimation.py
--rw-r--r--   0 ronald     (501) staff       (20)      824 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsanimationcontext.py
--rw-r--r--   0 ronald     (501) staff       (20)     1596 2022-06-25 20:14:24.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsappearance.py
--rw-r--r--   0 ronald     (501) staff       (20)     2262 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsappleeventdescriptor.py
--rw-r--r--   0 ronald     (501) staff       (20)      798 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsappleeventmanager.py
--rw-r--r--   0 ronald     (501) staff       (20)     1302 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsapplescript.py
--rw-r--r--   0 ronald     (501) staff       (20)    19842 2022-12-16 16:43:02.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsapplication.py
--rw-r--r--   0 ronald     (501) staff       (20)      385 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsapplicationscripting.py
--rw-r--r--   0 ronald     (501) staff       (20)      376 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsarchiver.py
--rw-r--r--   0 ronald     (501) staff       (20)    19206 2023-03-03 17:21:59.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsarray.py
--rw-r--r--   0 ronald     (501) staff       (20)     1911 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsarraycontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)     6160 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsatstypesetter.py
--rw-r--r--   0 ronald     (501) staff       (20)    19107 2022-06-23 11:03:28.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsattributedstring.py
--rw-r--r--   0 ronald     (501) staff       (20)    12805 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsattributedstring_appkit.py
--rw-r--r--   0 ronald     (501) staff       (20)      406 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsautoreleasepool.py
--rw-r--r--   0 ronald     (501) staff       (20)     1044 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsbackgroundactivityscheduler.py
--rw-r--r--   0 ronald     (501) staff       (20)     7004 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsbezierpath.py
--rw-r--r--   0 ronald     (501) staff       (20)      504 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsbitmap.py
--rw-r--r--   0 ronald     (501) staff       (20)    12549 2023-03-03 17:21:59.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsbitmapimagerep.py
--rw-r--r--   0 ronald     (501) staff       (20)      982 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsbox.py
--rw-r--r--   0 ronald     (501) staff       (20)    11790 2022-06-25 09:03:05.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsbrowser.py
--rw-r--r--   0 ronald     (501) staff       (20)      375 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsbrowsercell.py
--rw-r--r--   0 ronald     (501) staff       (20)     2284 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsbundle.py
--rw-r--r--   0 ronald     (501) staff       (20)     1867 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsbutton.py
--rw-r--r--   0 ronald     (501) staff       (20)     4422 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsbuttoncell.py
--rw-r--r--   0 ronald     (501) staff       (20)      702 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsbuttontouchbaritem.py
--rw-r--r--   0 ronald     (501) staff       (20)     2635 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsbytecountformatter.py
--rw-r--r--   0 ronald     (501) staff       (20)     4721 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsbyteorder.py
--rw-r--r--   0 ronald     (501) staff       (20)     1451 2022-06-27 16:50:29.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nscache.py
--rw-r--r--   0 ronald     (501) staff       (20)      354 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nscachedimagerep.py
--rw-r--r--   0 ronald     (501) staff       (20)    10393 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nscalendar.py
--rw-r--r--   0 ronald     (501) staff       (20)     1233 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nscalendardate.py
--rw-r--r--   0 ronald     (501) staff       (20)     3293 2022-06-25 09:02:12.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nscandidatelisttouchbaritem.py
--rw-r--r--   0 ronald     (501) staff       (20)     9505 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nscell.py
--rw-r--r--   0 ronald     (501) staff       (20)      546 2021-04-09 10:15:21.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nscharacterset.py
--rw-r--r--   0 ronald     (501) staff       (20)      248 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsclassdescription.py
--rw-r--r--   0 ronald     (501) staff       (20)      705 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsclipview.py
--rw-r--r--   0 ronald     (501) staff       (20)     5724 2023-03-03 18:02:55.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nscoder.py
--rw-r--r--   0 ronald     (501) staff       (20)    11151 2022-06-25 09:00:51.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nscollectionview.py
--rw-r--r--   0 ronald     (501) staff       (20)     8268 2022-06-25 09:04:20.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nscollectionviewcompositionallayout.py
--rw-r--r--   0 ronald     (501) staff       (20)     4958 2022-06-25 09:00:54.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nscollectionviewflowlayout.py
--rw-r--r--   0 ronald     (501) staff       (20)     1847 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nscollectionviewlayout.py
--rw-r--r--   0 ronald     (501) staff       (20)     2922 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nscolor.py
--rw-r--r--   0 ronald     (501) staff       (20)      568 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nscolorlist.py
--rw-r--r--   0 ronald     (501) staff       (20)     2585 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nscolorpanel.py
--rw-r--r--   0 ronald     (501) staff       (20)      494 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nscolorpickertouchbaritem.py
--rw-r--r--   0 ronald     (501) staff       (20)      812 2022-06-25 09:03:15.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nscolorpicking.py
--rw-r--r--   0 ronald     (501) staff       (20)      290 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nscolorsampler.py
--rw-r--r--   0 ronald     (501) staff       (20)     1442 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nscolorspace.py
--rw-r--r--   0 ronald     (501) staff       (20)      801 2022-06-26 21:30:09.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nscolorwell.py
--rw-r--r--   0 ronald     (501) staff       (20)     1932 2022-06-25 09:00:04.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nscombobox.py
--rw-r--r--   0 ronald     (501) staff       (20)     1606 2022-06-25 09:00:01.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nscomboboxcell.py
--rw-r--r--   0 ronald     (501) staff       (20)      784 2022-06-15 11:57:00.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nscombobutton.py
--rw-r--r--   0 ronald     (501) staff       (20)     2409 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nscomparisonpredicate.py
--rw-r--r--   0 ronald     (501) staff       (20)      409 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nscompoundpredicate.py
--rw-r--r--   0 ronald     (501) staff       (20)     1836 2022-06-25 20:10:39.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsconnection.py
--rw-r--r--   0 ronald     (501) staff       (20)     3480 2022-06-25 09:01:58.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nscontrol.py
--rw-r--r--   0 ronald     (501) staff       (20)      619 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nscontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)      227 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nscredentialstorage.py
--rw-r--r--   0 ronald     (501) staff       (20)      578 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nscursor.py
--rw-r--r--   0 ronald     (501) staff       (20)      782 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nscustomimagerep.py
--rw-r--r--   0 ronald     (501) staff       (20)    16177 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsdata.py
--rw-r--r--   0 ronald     (501) staff       (20)      432 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsdate.py
--rw-r--r--   0 ronald     (501) staff       (20)     3475 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsdatecomponentsformatter.py
--rw-r--r--   0 ronald     (501) staff       (20)     3412 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsdateformatter.py
--rw-r--r--   0 ronald     (501) staff       (20)      407 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsdateinterval.py
--rw-r--r--   0 ronald     (501) staff       (20)      654 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsdateintervalformatter.py
--rw-r--r--   0 ronald     (501) staff       (20)      760 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsdatepicker.py
--rw-r--r--   0 ronald     (501) staff       (20)     2586 2022-06-25 20:13:11.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsdatepickercell.py
--rw-r--r--   0 ronald     (501) staff       (20)     1110 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsdebug.py
--rw-r--r--   0 ronald     (501) staff       (20)     4450 2022-06-25 09:00:10.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsdecimalnumber.py
--rw-r--r--   0 ronald     (501) staff       (20)    12696 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsdictionary.py
--rw-r--r--   0 ronald     (501) staff       (20)      333 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsdictionarycontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)      201 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsdistributedlock.py
--rw-r--r--   0 ronald     (501) staff       (20)     1956 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsdistributednotificationcenter.py
--rw-r--r--   0 ronald     (501) staff       (20)      514 2022-06-25 20:12:06.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsdocktile.py
--rw-r--r--   0 ronald     (501) staff       (20)    14204 2022-10-21 07:44:21.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsdocument.py
--rw-r--r--   0 ronald     (501) staff       (20)     5313 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsdocumentcontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)     9915 2022-06-25 09:03:23.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsdragging.py
--rw-r--r--   0 ronald     (501) staff       (20)      681 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsdraggingitem.py
--rw-r--r--   0 ronald     (501) staff       (20)      680 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsdraggingsession.py
--rw-r--r--   0 ronald     (501) staff       (20)     1710 2022-06-25 20:17:11.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsdrawer.py
--rw-r--r--   0 ronald     (501) staff       (20)     1183 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsenergyformatter.py
--rw-r--r--   0 ronald     (501) staff       (20)      592 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsenumerator.py
--rw-r--r--   0 ronald     (501) staff       (20)     5324 2021-04-09 08:48:53.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nserror.py
--rw-r--r--   0 ronald     (501) staff       (20)     2649 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nserrors.py
--rw-r--r--   0 ronald     (501) staff       (20)    20933 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsevent.py
--rw-r--r--   0 ronald     (501) staff       (20)     3432 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsexception.py
--rw-r--r--   0 ronald     (501) staff       (20)     1689 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsexpression.py
--rw-r--r--   0 ronald     (501) staff       (20)      602 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsextensioncontext.py
--rw-r--r--   0 ronald     (501) staff       (20)      421 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsextensionitem.py
--rw-r--r--   0 ronald     (501) staff       (20)      268 2022-06-25 20:15:06.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsextensionrequesthandling.py
--rw-r--r--   0 ronald     (501) staff       (20)     3425 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsfilecoordinator.py
--rw-r--r--   0 ronald     (501) staff       (20)     3371 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsfilehandle.py
--rw-r--r--   0 ronald     (501) staff       (20)    24938 2023-03-03 17:21:59.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsfilemanager.py
--rw-r--r--   0 ronald     (501) staff       (20)     1415 2022-06-25 20:09:20.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsfilepresenter.py
--rw-r--r--   0 ronald     (501) staff       (20)      614 2022-06-25 20:16:36.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsfilepromiseprovider.py
--rw-r--r--   0 ronald     (501) staff       (20)      369 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsfilepromisereceiver.py
--rw-r--r--   0 ronald     (501) staff       (20)     1910 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsfileversion.py
--rw-r--r--   0 ronald     (501) staff       (20)     2001 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsfilewrapper.py
--rw-r--r--   0 ronald     (501) staff       (20)     5203 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsfont.py
--rw-r--r--   0 ronald     (501) staff       (20)      505 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsfontassetrequest.py
--rw-r--r--   0 ronald     (501) staff       (20)     2728 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsfontcollection.py
--rw-r--r--   0 ronald     (501) staff       (20)     8020 2022-07-08 16:02:54.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsfontdescriptor.py
--rw-r--r--   0 ronald     (501) staff       (20)     2756 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsfontmanager.py
--rw-r--r--   0 ronald     (501) staff       (20)     2980 2022-06-25 09:03:19.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsfontpanel.py
--rw-r--r--   0 ronald     (501) staff       (20)      235 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsform.py
--rw-r--r--   0 ronald     (501) staff       (20)     2579 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsformatter.py
--rw-r--r--   0 ronald     (501) staff       (20)      180 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsformcell.py
--rw-r--r--   0 ronald     (501) staff       (20)      281 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsgarbagecollector.py
--rw-r--r--   0 ronald     (501) staff       (20)    10354 2022-07-30 15:06:02.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsgeometry.py
--rw-r--r--   0 ronald     (501) staff       (20)     4564 2022-06-25 20:15:42.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsgesturerecognizer.py
--rw-r--r--   0 ronald     (501) staff       (20)     2853 2022-06-25 09:02:03.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsglyphgenerator.py
--rw-r--r--   0 ronald     (501) staff       (20)      628 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsglyphinfo.py
--rw-r--r--   0 ronald     (501) staff       (20)      765 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsgradient.py
--rw-r--r--   0 ronald     (501) staff       (20)    15551 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsgraphics.py
--rw-r--r--   0 ronald     (501) staff       (20)     3082 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsgraphicscontext.py
--rw-r--r--   0 ronald     (501) staff       (20)     1476 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsgridview.py
--rw-r--r--   0 ronald     (501) staff       (20)      332 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsgrouptouchbaritem.py
--rw-r--r--   0 ronald     (501) staff       (20)     1238 2022-06-25 19:36:17.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nshapticfeedback.py
--rw-r--r--   0 ronald     (501) staff       (20)     2272 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nshashtable.py
--rw-r--r--   0 ronald     (501) staff       (20)      746 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nshelpmanager.py
--rw-r--r--   0 ronald     (501) staff       (20)      823 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nshfsfiletypes.py
--rw-r--r--   0 ronald     (501) staff       (20)     1393 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nshost.py
--rw-r--r--   0 ronald     (501) staff       (20)     1699 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nshttpcookie.py
--rw-r--r--   0 ronald     (501) staff       (20)      954 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nshttpcookiestorage.py
--rw-r--r--   0 ronald     (501) staff       (20)    17535 2023-03-03 17:21:59.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsimage.py
--rw-r--r--   0 ronald     (501) staff       (20)     1043 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsimagecell.py
--rw-r--r--   0 ronald     (501) staff       (20)     2312 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsimagerep.py
--rw-r--r--   0 ronald     (501) staff       (20)      517 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsimageview.py
--rw-r--r--   0 ronald     (501) staff       (20)     1292 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsindexpath.py
--rw-r--r--   0 ronald     (501) staff       (20)     4575 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsindexset.py
--rw-r--r--   0 ronald     (501) staff       (20)      286 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsinflectionrule.py
--rw-r--r--   0 ronald     (501) staff       (20)     2212 2022-06-25 09:02:21.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsinputmanager.py
--rw-r--r--   0 ronald     (501) staff       (20)     4321 2022-06-25 09:01:45.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsinputserver.py
--rw-r--r--   0 ronald     (501) staff       (20)      562 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsinterfacestyle.py
--rw-r--r--   0 ronald     (501) staff       (20)     2238 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsinvocation.py
--rw-r--r--   0 ronald     (501) staff       (20)     2620 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsiso8601dateformatter.py
--rw-r--r--   0 ronald     (501) staff       (20)     6223 2023-03-03 17:21:59.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsitemprovider.py
--rw-r--r--   0 ronald     (501) staff       (20)     1031 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsitemproviderreadingwriting.py
--rw-r--r--   0 ronald     (501) staff       (20)     2817 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsjavasetup.py
--rw-r--r--   0 ronald     (501) staff       (20)     1730 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsjsonserialization.py
--rw-r--r--   0 ronald     (501) staff       (20)     4689 2022-06-25 20:08:56.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nskeyedarchiver.py
--rw-r--r--   0 ronald     (501) staff       (20)     9456 2022-10-29 10:34:50.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nskeyvaluebinding.py
--rw-r--r--   0 ronald     (501) staff       (20)     2596 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nskeyvaluecoding.py
--rw-r--r--   0 ronald     (501) staff       (20)     3777 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nskeyvalueobservering.py
--rw-r--r--   0 ronald     (501) staff       (20)      245 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nslayoutanchor.py
--rw-r--r--   0 ronald     (501) staff       (20)     6975 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nslayoutconstraint.py
--rw-r--r--   0 ronald     (501) staff       (20)      237 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nslayoutguide.py
--rw-r--r--   0 ronald     (501) staff       (20)    31364 2022-10-29 10:33:31.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nslayoutmanager.py
--rw-r--r--   0 ronald     (501) staff       (20)     1475 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nslengthformatter.py
--rw-r--r--   0 ronald     (501) staff       (20)      863 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nslevelindicator.py
--rw-r--r--   0 ronald     (501) staff       (20)      787 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nslevelindicatorcell.py
--rw-r--r--   0 ronald     (501) staff       (20)     8110 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nslinguistictagger.py
--rw-r--r--   0 ronald     (501) staff       (20)     3449 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nslocale.py
--rw-r--r--   0 ronald     (501) staff       (20)     1361 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nslocalizedstring.py
--rw-r--r--   0 ronald     (501) staff       (20)     1017 2022-06-25 09:07:11.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nslock.py
--rw-r--r--   0 ronald     (501) staff       (20)     1803 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nslog.py
--rw-r--r--   0 ronald     (501) staff       (20)      326 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsmachport.py
--rw-r--r--   0 ronald     (501) staff       (20)      925 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsmaptable.py
--rw-r--r--   0 ronald     (501) staff       (20)     1233 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsmassformatter.py
--rw-r--r--   0 ronald     (501) staff       (20)     4059 2022-06-25 09:06:54.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsmatrix.py
--rw-r--r--   0 ronald     (501) staff       (20)      248 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsmeasurement.py
--rw-r--r--   0 ronald     (501) staff       (20)      636 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsmeasurementformatter.py
--rw-r--r--   0 ronald     (501) staff       (20)      645 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsmedialibrarybrowsercontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)     4383 2022-06-25 09:03:41.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsmenu.py
--rw-r--r--   0 ronald     (501) staff       (20)     1712 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsmenuitem.py
--rw-r--r--   0 ronald     (501) staff       (20)      402 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsmenuitemcell.py
--rw-r--r--   0 ronald     (501) staff       (20)      324 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsmenutoolbaritem.py
--rw-r--r--   0 ronald     (501) staff       (20)      116 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsmenuview.py
--rw-r--r--   0 ronald     (501) staff       (20)     4061 2022-06-25 09:01:25.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsmetadata.py
--rw-r--r--   0 ronald     (501) staff       (20)    14856 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsmetadataattributes.py
--rw-r--r--   0 ronald     (501) staff       (20)     1666 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsmethodsignature.py
--rw-r--r--   0 ronald     (501) staff       (20)     2701 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsmorphology.py
--rw-r--r--   0 ronald     (501) staff       (20)      113 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsmovie.py
--rw-r--r--   0 ronald     (501) staff       (20)      117 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsmovieview.py
--rw-r--r--   0 ronald     (501) staff       (20)     3555 2022-06-25 20:14:52.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsnetservices.py
--rw-r--r--   0 ronald     (501) staff       (20)      759 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsnib.py
--rw-r--r--   0 ronald     (501) staff       (20)      610 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsnibloading.py
--rw-r--r--   0 ronald     (501) staff       (20)      518 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsnotification.py
--rw-r--r--   0 ronald     (501) staff       (20)      659 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsnotificationqueue.py
--rw-r--r--   0 ronald     (501) staff       (20)      216 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsnull.py
--rw-r--r--   0 ronald     (501) staff       (20)     8581 2022-02-06 09:24:04.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsnumber.py
--rw-r--r--   0 ronald     (501) staff       (20)     6097 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsnumberformatter.py
--rw-r--r--   0 ronald     (501) staff       (20)    10649 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsobjcruntime.py
--rw-r--r--   0 ronald     (501) staff       (20)     6586 2022-06-25 09:03:53.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsobject.py
--rw-r--r--   0 ronald     (501) staff       (20)    17563 2022-01-02 11:20:34.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsobject_additions.py
--rw-r--r--   0 ronald     (501) staff       (20)     1115 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsobjectcontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)     8094 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsopengl.py
--rw-r--r--   0 ronald     (501) staff       (20)      598 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsopengllayer.py
--rw-r--r--   0 ronald     (501) staff       (20)      364 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsopenglview.py
--rw-r--r--   0 ronald     (501) staff       (20)     2560 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsopenpanel.py
--rw-r--r--   0 ronald     (501) staff       (20)     2940 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsoperation.py
--rw-r--r--   0 ronald     (501) staff       (20)      369 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsorderedcollectionchange.py
--rw-r--r--   0 ronald     (501) staff       (20)     1013 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsorderedcollectiondifference.py
--rw-r--r--   0 ronald     (501) staff       (20)     7814 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsorderedset.py
--rw-r--r--   0 ronald     (501) staff       (20)    10318 2022-06-25 09:04:29.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsoutlineview.py
--rw-r--r--   0 ronald     (501) staff       (20)      961 2023-03-03 17:21:59.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nspagecontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)      558 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nspagelayout.py
--rw-r--r--   0 ronald     (501) staff       (20)     3517 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nspanel.py
--rw-r--r--   0 ronald     (501) staff       (20)     1943 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsparagraphstyle.py
--rw-r--r--   0 ronald     (501) staff       (20)     6561 2022-06-25 09:02:33.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nspasteboard.py
--rw-r--r--   0 ronald     (501) staff       (20)      623 2022-06-25 20:17:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nspasteboarditem.py
--rw-r--r--   0 ronald     (501) staff       (20)      661 2022-06-25 20:06:33.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nspathcell.py
--rw-r--r--   0 ronald     (501) staff       (20)     1642 2023-03-03 17:21:59.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nspathcontrol.py
--rw-r--r--   0 ronald     (501) staff       (20)     5081 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nspathutilties.py
--rw-r--r--   0 ronald     (501) staff       (20)      305 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nspdfinfo.py
--rw-r--r--   0 ronald     (501) staff       (20)      689 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nspdfpanel.py
--rw-r--r--   0 ronald     (501) staff       (20)     1617 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nspersistentdocument.py
--rw-r--r--   0 ronald     (501) staff       (20)     2137 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nspersonnamecomponentsformatter.py
--rw-r--r--   0 ronald     (501) staff       (20)     1673 2022-10-18 09:53:24.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nspickertouchBaritem.py
--rw-r--r--   0 ronald     (501) staff       (20)      631 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nspointerarray.py
--rw-r--r--   0 ronald     (501) staff       (20)     1926 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nspointerfunctions.py
--rw-r--r--   0 ronald     (501) staff       (20)     2364 2022-06-25 20:16:15.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nspopover.py
--rw-r--r--   0 ronald     (501) staff       (20)      339 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nspopovertouchbaritem.py
--rw-r--r--   0 ronald     (501) staff       (20)      661 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nspopupbutton.py
--rw-r--r--   0 ronald     (501) staff       (20)     1275 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nspopupbuttoncell.py
--rw-r--r--   0 ronald     (501) staff       (20)     1763 2022-06-25 09:01:51.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsport.py
--rw-r--r--   0 ronald     (501) staff       (20)      254 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsportcoder.py
--rw-r--r--   0 ronald     (501) staff       (20)      201 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsportmessage.py
--rw-r--r--   0 ronald     (501) staff       (20)      678 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsportnameserver.py
--rw-r--r--   0 ronald     (501) staff       (20)     1068 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nspredicate.py
--rw-r--r--   0 ronald     (501) staff       (20)      274 2022-06-25 20:09:10.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nspreviewrepresentingactivityitem.py
--rw-r--r--   0 ronald     (501) staff       (20)     1085 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsprinter.py
--rw-r--r--   0 ronald     (501) staff       (20)     4954 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsprintinfo.py
--rw-r--r--   0 ronald     (501) staff       (20)     2064 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsprintoperation.py
--rw-r--r--   0 ronald     (501) staff       (20)     2035 2022-06-25 09:00:18.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsprintpanel.py
--rw-r--r--   0 ronald     (501) staff       (20)     5012 2022-06-23 11:03:28.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsprocessinfo.py
--rw-r--r--   0 ronald     (501) staff       (20)     3298 2022-06-25 20:14:49.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsprogress.py
--rw-r--r--   0 ronald     (501) staff       (20)     1535 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsprogressindicator.py
--rw-r--r--   0 ronald     (501) staff       (20)     2439 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nspropertylist.py
--rw-r--r--   0 ronald     (501) staff       (20)      560 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsproxy.py
--rw-r--r--   0 ronald     (501) staff       (20)     1496 2022-01-02 11:04:26.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsrange.py
--rw-r--r--   0 ronald     (501) staff       (20)     2424 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsregularexpression.py
--rw-r--r--   0 ronald     (501) staff       (20)      830 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsrelativedatetimeformatter.py
--rw-r--r--   0 ronald     (501) staff       (20)     1846 2022-06-25 09:00:41.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsresponder.py
--rw-r--r--   0 ronald     (501) staff       (20)     3699 2022-06-25 09:03:13.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsruleeditor.py
--rw-r--r--   0 ronald     (501) staff       (20)      598 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsrulermarker.py
--rw-r--r--   0 ronald     (501) staff       (20)     3217 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsrulerview.py
--rw-r--r--   0 ronald     (501) staff       (20)     1029 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsrunloop.py
--rw-r--r--   0 ronald     (501) staff       (20)     1562 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsrunningapplication.py
--rw-r--r--   0 ronald     (501) staff       (20)     4257 2022-06-25 09:01:27.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nssavepanel.py
--rw-r--r--   0 ronald     (501) staff       (20)     3879 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsscanner.py
--rw-r--r--   0 ronald     (501) staff       (20)     1474 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsscreen.py
--rw-r--r--   0 ronald     (501) staff       (20)     1070 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsscriptclassdescription.py
--rw-r--r--   0 ronald     (501) staff       (20)      328 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsscriptcoercionhandler.py
--rw-r--r--   0 ronald     (501) staff       (20)     1015 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsscriptcommand.py
--rw-r--r--   0 ronald     (501) staff       (20)      640 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsscriptcommanddescription.py
--rw-r--r--   0 ronald     (501) staff       (20)      979 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsscriptkeyvaluecoding.py
--rw-r--r--   0 ronald     (501) staff       (20)     2456 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsscriptobjectspecifier.py
--rw-r--r--   0 ronald     (501) staff       (20)      402 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsscriptstandardsuitecommands.py
--rw-r--r--   0 ronald     (501) staff       (20)     3270 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsscriptwhosetests.py
--rw-r--r--   0 ronald     (501) staff       (20)     2276 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsscroller.py
--rw-r--r--   0 ronald     (501) staff       (20)     3904 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsscrollview.py
--rw-r--r--   0 ronald     (501) staff       (20)     2663 2022-06-25 09:01:41.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsscrubber.py
--rw-r--r--   0 ronald     (501) staff       (20)      476 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsscrubberitemview.py
--rw-r--r--   0 ronald     (501) staff       (20)     1285 2022-06-25 09:07:45.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsscrubberlayout.py
--rw-r--r--   0 ronald     (501) staff       (20)     1093 2022-06-25 20:14:50.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nssearchfield.py
--rw-r--r--   0 ronald     (501) staff       (20)      819 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nssearchfieldcell.py
--rw-r--r--   0 ronald     (501) staff       (20)      405 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nssearchtoolbaritem.py
--rw-r--r--   0 ronald     (501) staff       (20)      284 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nssecuretextfield.py
--rw-r--r--   0 ronald     (501) staff       (20)      754 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nssegmentedcell.py
--rw-r--r--   0 ronald     (501) staff       (20)     2704 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nssegmentedcontrol.py
--rw-r--r--   0 ronald     (501) staff       (20)     6705 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsset.py
--rw-r--r--   0 ronald     (501) staff       (20)     3864 2022-06-25 08:59:53.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nssharingservice.py
--rw-r--r--   0 ronald     (501) staff       (20)      282 2022-06-25 20:17:40.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nssharingservicepickertoolbaritem.py
--rw-r--r--   0 ronald     (501) staff       (20)      520 2022-06-25 20:09:36.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nssharingservicepickertouchbaritem.py
--rw-r--r--   0 ronald     (501) staff       (20)      134 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nssimplehorizontaltypesetter.py
--rw-r--r--   0 ronald     (501) staff       (20)      662 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsslider.py
--rw-r--r--   0 ronald     (501) staff       (20)      429 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsslideraccessory.py
--rw-r--r--   0 ronald     (501) staff       (20)     1635 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsslidercell.py
--rw-r--r--   0 ronald     (501) staff       (20)      423 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsslidertouchbaritem.py
--rw-r--r--   0 ronald     (501) staff       (20)     1450 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nssortdescriptor.py
--rw-r--r--   0 ronald     (501) staff       (20)     1225 2022-06-25 20:13:58.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nssound.py
--rw-r--r--   0 ronald     (501) staff       (20)      603 2022-06-25 20:11:38.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsspeechrecognizer.py
--rw-r--r--   0 ronald     (501) staff       (20)     7341 2022-06-25 09:01:49.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsspeechsynthesizer.py
--rw-r--r--   0 ronald     (501) staff       (20)     7291 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsspellchecker.py
--rw-r--r--   0 ronald     (501) staff       (20)      256 2022-06-25 20:14:54.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsspellprotocol.py
--rw-r--r--   0 ronald     (501) staff       (20)     3384 2022-06-25 09:03:34.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsspellserver.py
--rw-r--r--   0 ronald     (501) staff       (20)     6101 2022-06-25 09:02:42.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nssplitview.py
--rw-r--r--   0 ronald     (501) staff       (20)     2083 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nssplitviewcontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)     1799 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nssplitviewitem.py
--rw-r--r--   0 ronald     (501) staff       (20)     2264 2022-06-25 09:04:25.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsstackview.py
--rw-r--r--   0 ronald     (501) staff       (20)      344 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsstatusbar.py
--rw-r--r--   0 ronald     (501) staff       (20)      320 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsstatusbarbutton.py
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsstatusitem.py
--rw-r--r--   0 ronald     (501) staff       (20)      371 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsstepper.py
--rw-r--r--   0 ronald     (501) staff       (20)      391 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nssteppercell.py
--rw-r--r--   0 ronald     (501) staff       (20)      557 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsstoryboard.py
--rw-r--r--   0 ronald     (501) staff       (20)      880 2022-06-25 20:15:21.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsstoryboardsegue.py
--rw-r--r--   0 ronald     (501) staff       (20)     7108 2022-06-25 09:02:59.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsstream.py
--rw-r--r--   0 ronald     (501) staff       (20)    23975 2022-10-21 10:39:37.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsstring.py
--rw-r--r--   0 ronald     (501) staff       (20)      762 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsstringdrawing.py
--rw-r--r--   0 ronald     (501) staff       (20)      924 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstablecolumn.py
--rw-r--r--   0 ronald     (501) staff       (20)      585 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstableheadercell.py
--rw-r--r--   0 ronald     (501) staff       (20)     1244 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstablerowview.py
--rw-r--r--   0 ronald     (501) staff       (20)    18911 2022-06-25 09:02:52.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstableview.py
--rw-r--r--   0 ronald     (501) staff       (20)     1162 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstableviewdiffabledatasource.py
--rw-r--r--   0 ronald     (501) staff       (20)      370 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstableviewrowaction.py
--rw-r--r--   0 ronald     (501) staff       (20)     1715 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstabview.py
--rw-r--r--   0 ronald     (501) staff       (20)     1185 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstabviewcontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)      524 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstabviewitem.py
--rw-r--r--   0 ronald     (501) staff       (20)     1325 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstask.py
--rw-r--r--   0 ronald     (501) staff       (20)     5617 2022-06-25 09:07:15.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstext.py
--rw-r--r--   0 ronald     (501) staff       (20)      295 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstextalternatives.py
--rw-r--r--   0 ronald     (501) staff       (20)     7781 2022-06-25 09:01:38.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstextattachment.py
--rw-r--r--   0 ronald     (501) staff       (20)     6544 2022-06-25 09:02:18.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstextcheckingclient.py
--rw-r--r--   0 ronald     (501) staff       (20)     5233 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstextcheckingresult.py
--rw-r--r--   0 ronald     (501) staff       (20)     1500 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstextcontainer.py
--rw-r--r--   0 ronald     (501) staff       (20)      598 2022-06-25 20:17:26.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstextcontent.py
--rw-r--r--   0 ronald     (501) staff       (20)      710 2022-06-25 20:11:36.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstextcontextmanager.py
--rw-r--r--   0 ronald     (501) staff       (20)      243 2022-06-15 11:57:00.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstextelement.py
--rw-r--r--   0 ronald     (501) staff       (20)     3134 2022-06-25 09:01:33.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstextfield.py
--rw-r--r--   0 ronald     (501) staff       (20)      627 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstextfieldcell.py
--rw-r--r--   0 ronald     (501) staff       (20)     5570 2022-06-25 09:02:15.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstextfinder.py
--rw-r--r--   0 ronald     (501) staff       (20)     4415 2022-06-25 09:03:44.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstextinputclient.py
--rw-r--r--   0 ronald     (501) staff       (20)      574 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstextinputcontext.py
--rw-r--r--   0 ronald     (501) staff       (20)     1150 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstextlayoutfragment.py
--rw-r--r--   0 ronald     (501) staff       (20)     3156 2022-06-25 20:06:42.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstextlayoutmanager.py
--rw-r--r--   0 ronald     (501) staff       (20)     1647 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstextlist.py
--rw-r--r--   0 ronald     (501) staff       (20)      725 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstextrange.py
--rw-r--r--   0 ronald     (501) staff       (20)      982 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstextselection.py
--rw-r--r--   0 ronald     (501) staff       (20)     6299 2022-06-25 09:02:36.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstextselectionnavigation.py
--rw-r--r--   0 ronald     (501) staff       (20)     3457 2022-06-25 09:00:23.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstextstorage.py
--rw-r--r--   0 ronald     (501) staff       (20)     1810 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstexttable.py
--rw-r--r--   0 ronald     (501) staff       (20)    20416 2023-03-03 17:21:59.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstextview.py
--rw-r--r--   0 ronald     (501) staff       (20)      623 2022-06-25 20:13:15.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstextviewportlayoutcontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)     2740 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsthread.py
--rw-r--r--   0 ronald     (501) staff       (20)     3674 2023-03-03 17:21:59.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstimer.py
--rw-r--r--   0 ronald     (501) staff       (20)     1075 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstimezone.py
--rw-r--r--   0 ronald     (501) staff       (20)      258 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstintconfiguration.py
--rw-r--r--   0 ronald     (501) staff       (20)      357 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstitlebaraccessoryview.py
--rw-r--r--   0 ronald     (501) staff       (20)      663 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstitlebaraccessoryviewcontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)     1750 2022-06-25 09:02:49.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstokenfield.py
--rw-r--r--   0 ronald     (501) staff       (20)     2726 2022-06-25 09:04:03.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstokenfieldcell.py
--rw-r--r--   0 ronald     (501) staff       (20)     2891 2022-06-25 09:02:44.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstoolbar.py
--rw-r--r--   0 ronald     (501) staff       (20)     2740 2022-06-27 15:56:12.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstoolbaritem.py
--rw-r--r--   0 ronald     (501) staff       (20)     1416 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstoolbaritemgroup.py
--rw-r--r--   0 ronald     (501) staff       (20)     1749 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstouch.py
--rw-r--r--   0 ronald     (501) staff       (20)     1017 2022-06-25 20:09:45.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstouchbar.py
--rw-r--r--   0 ronald     (501) staff       (20)     1076 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstouchbaritem.py
--rw-r--r--   0 ronald     (501) staff       (20)      923 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstrackingarea.py
--rw-r--r--   0 ronald     (501) staff       (20)     1342 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstreecontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)      306 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstreenode.py
--rw-r--r--   0 ronald     (501) staff       (20)    13133 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstypesetter.py
--rw-r--r--   0 ronald     (501) staff       (20)     1181 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsubiquitouskeyvaluestore.py
--rw-r--r--   0 ronald     (501) staff       (20)     4088 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsundomanager.py
--rw-r--r--   0 ronald     (501) staff       (20)    18970 2023-02-19 10:50:34.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsurl.py
--rw-r--r--   0 ronald     (501) staff       (20)      230 2022-06-25 20:16:07.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsurlauthenticationchallenge.py
--rw-r--r--   0 ronald     (501) staff       (20)      666 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsurlcache.py
--rw-r--r--   0 ronald     (501) staff       (20)     3750 2022-06-25 09:01:03.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsurlconnection.py
--rw-r--r--   0 ronald     (501) staff       (20)      637 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsurlcredential.py
--rw-r--r--   0 ronald     (501) staff       (20)      876 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsurlcredentialstorage.py
--rw-r--r--   0 ronald     (501) staff       (20)     1979 2022-06-25 09:07:21.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsurldownload.py
--rw-r--r--   0 ronald     (501) staff       (20)     5643 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsurlerror.py
--rw-r--r--   0 ronald     (501) staff       (20)     1803 2022-06-25 20:10:01.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsurlhandle.py
--rw-r--r--   0 ronald     (501) staff       (20)     1691 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsurlprotectionspace.py
--rw-r--r--   0 ronald     (501) staff       (20)      961 2022-06-25 09:07:23.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsurlprotocol.py
--rw-r--r--   0 ronald     (501) staff       (20)     3731 2022-10-18 09:53:23.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsurlrequest.py
--rw-r--r--   0 ronald     (501) staff       (20)      197 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsurlresponse.py
--rw-r--r--   0 ronald     (501) staff       (20)    16829 2022-06-25 09:04:09.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsurlsession.py
--rw-r--r--   0 ronald     (501) staff       (20)     2101 2022-06-25 20:10:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsuseractivity.py
--rw-r--r--   0 ronald     (501) staff       (20)     2909 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsuserdefaults.py
--rw-r--r--   0 ronald     (501) staff       (20)      391 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsuserdefaultscontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)      707 2022-06-25 20:07:12.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsuserinterfacecompression.py
--rw-r--r--   0 ronald     (501) staff       (20)      376 2022-06-25 20:15:48.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsuserinterfaceitemidentification.py
--rw-r--r--   0 ronald     (501) staff       (20)     1454 2022-06-25 09:01:56.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsuserinterfaceitemsearching.py
--rw-r--r--   0 ronald     (501) staff       (20)      617 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsuserinterfacelayout.py
--rw-r--r--   0 ronald     (501) staff       (20)      826 2022-06-25 09:03:56.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsuserinterfacevalidation.py
--rw-r--r--   0 ronald     (501) staff       (20)     1850 2022-06-25 20:13:01.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsusernotification.py
--rw-r--r--   0 ronald     (501) staff       (20)     1164 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsuserscripttask.py
--rw-r--r--   0 ronald     (501) staff       (20)      696 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsuuid.py
--rw-r--r--   0 ronald     (501) staff       (20)     1578 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsvalue.py
--rw-r--r--   0 ronald     (501) staff       (20)      821 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsvaluetransformer.py
--rw-r--r--   0 ronald     (501) staff       (20)    12513 2022-06-25 09:04:01.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsview.py
--rw-r--r--   0 ronald     (501) staff       (20)     1933 2022-06-25 09:00:36.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsviewcontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)     2281 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsvisualeffectview.py
--rw-r--r--   0 ronald     (501) staff       (20)    23697 2023-03-24 18:54:07.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nswindow.py
--rw-r--r--   0 ronald     (501) staff       (20)      606 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nswindowcontroller.py
--rw-r--r--   0 ronald     (501) staff       (20)     1347 2022-06-25 20:12:46.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nswindowrestoration.py
--rw-r--r--   0 ronald     (501) staff       (20)      756 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nswindowscripting.py
--rw-r--r--   0 ronald     (501) staff       (20)      915 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nswindowtabgroup.py
--rw-r--r--   0 ronald     (501) staff       (20)    15068 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsworkspace.py
--rw-r--r--   0 ronald     (501) staff       (20)     1488 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsxmldocument.py
--rw-r--r--   0 ronald     (501) staff       (20)      292 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsxmldtd.py
--rw-r--r--   0 ronald     (501) staff       (20)     1665 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsxmldtdnode.py
--rw-r--r--   0 ronald     (501) staff       (20)      330 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsxmlelement.py
--rw-r--r--   0 ronald     (501) staff       (20)     1484 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsxmlnode.py
--rw-r--r--   0 ronald     (501) staff       (20)     3244 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsxmlnodeoptions.py
--rw-r--r--   0 ronald     (501) staff       (20)     8643 2022-06-25 20:13:39.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsxmlparser.py
--rw-r--r--   0 ronald     (501) staff       (20)     2569 2022-06-25 20:17:50.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsxpcconnection.py
--rw-r--r--   0 ronald     (501) staff       (20)     2786 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nszone.py
--rw-r--r--   0 ronald     (501) staff       (20)      444 2023-03-03 17:21:59.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_osxcasts.py
--rw-r--r--   0 ronald     (501) staff       (20)     3521 2023-03-03 17:21:59.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_regr.py
--rw-r--r--   0 ronald     (501) staff       (20)     8720 2022-10-21 10:39:38.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_structs.py
--rw-r--r--   0 ronald     (501) staff       (20)      961 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_subclassing.py
--rw-r--r--   0 ronald     (501) staff       (20)     3411 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_threading.py
--rw-r--r--   0 ronald     (501) staff       (20)     1171 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_weirdness.py
--rw-r--r--   0 ronald     (501) staff       (20)      346 2021-10-18 19:38:40.000000 pyobjc-framework-Cocoa-9.1b1/README.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:17:01.879480 pyobjc-framework-Cocoa-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)   635537 2022-12-17 13:53:38.000000 pyobjc-framework-Cocoa-9.1b1/metadata/AppKit.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   103010 2023-03-24 18:54:07.000000 pyobjc-framework-Cocoa-9.1b1/metadata/CoreFoundation.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   329142 2023-03-24 18:54:07.000000 pyobjc-framework-Cocoa-9.1b1/metadata/Foundation.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)      328 2021-08-03 12:27:37.000000 pyobjc-framework-Cocoa-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:17:02.475075 pyobjc-framework-Cocoa-9.1b1/metadata/raw.AppKit/
--rw-r--r--   0 ronald     (501) staff       (20)  3375264 2022-12-17 13:53:35.000000 pyobjc-framework-Cocoa-9.1b1/metadata/raw.AppKit/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)  3414548 2022-12-17 13:53:35.000000 pyobjc-framework-Cocoa-9.1b1/metadata/raw.AppKit/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)  3448948 2022-12-17 13:53:36.000000 pyobjc-framework-Cocoa-9.1b1/metadata/raw.AppKit/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)  3449119 2022-12-17 13:53:36.000000 pyobjc-framework-Cocoa-9.1b1/metadata/raw.AppKit/arm64-13.1.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)  3451956 2023-03-24 18:54:07.000000 pyobjc-framework-Cocoa-9.1b1/metadata/raw.AppKit/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)  2614871 2022-12-17 13:53:36.000000 pyobjc-framework-Cocoa-9.1b1/metadata/raw.AppKit/x86_64-10.10.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)  3098132 2022-12-17 13:53:36.000000 pyobjc-framework-Cocoa-9.1b1/metadata/raw.AppKit/x86_64-10.14.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)  3210922 2022-12-17 13:53:36.000000 pyobjc-framework-Cocoa-9.1b1/metadata/raw.AppKit/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)  3270357 2022-12-17 13:53:37.000000 pyobjc-framework-Cocoa-9.1b1/metadata/raw.AppKit/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)  1861235 2022-12-17 13:53:37.000000 pyobjc-framework-Cocoa-9.1b1/metadata/raw.AppKit/x86_64-10.6.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)  1999920 2022-12-17 13:53:37.000000 pyobjc-framework-Cocoa-9.1b1/metadata/raw.AppKit/x86_64-10.7.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)  2037216 2022-12-17 13:53:37.000000 pyobjc-framework-Cocoa-9.1b1/metadata/raw.AppKit/x86_64-10.8.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)  3375265 2022-12-17 13:53:37.000000 pyobjc-framework-Cocoa-9.1b1/metadata/raw.AppKit/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)  3414549 2022-12-17 13:53:38.000000 pyobjc-framework-Cocoa-9.1b1/metadata/raw.AppKit/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)  3448949 2022-12-17 13:53:38.000000 pyobjc-framework-Cocoa-9.1b1/metadata/raw.AppKit/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)  3449120 2022-12-17 13:53:38.000000 pyobjc-framework-Cocoa-9.1b1/metadata/raw.AppKit/x86_64-13.1.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)  3451957 2023-03-24 18:54:07.000000 pyobjc-framework-Cocoa-9.1b1/metadata/raw.AppKit/x86_64-13.3.fwinfo
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:17:02.566303 pyobjc-framework-Cocoa-9.1b1/metadata/raw.CoreFoundation/
--rw-r--r--   0 ronald     (501) staff       (20)   312826 2021-08-03 12:27:37.000000 pyobjc-framework-Cocoa-9.1b1/metadata/raw.CoreFoundation/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   315024 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/metadata/raw.CoreFoundation/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   330943 2022-10-29 12:03:04.000000 pyobjc-framework-Cocoa-9.1b1/metadata/raw.CoreFoundation/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   331260 2023-02-19 10:50:34.000000 pyobjc-framework-Cocoa-9.1b1/metadata/raw.CoreFoundation/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   305789 2021-08-03 12:27:37.000000 pyobjc-framework-Cocoa-9.1b1/metadata/raw.CoreFoundation/x86_64-10.10.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   311591 2021-08-03 12:27:37.000000 pyobjc-framework-Cocoa-9.1b1/metadata/raw.CoreFoundation/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   312634 2021-08-03 12:27:37.000000 pyobjc-framework-Cocoa-9.1b1/metadata/raw.CoreFoundation/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   292849 2021-08-03 12:27:37.000000 pyobjc-framework-Cocoa-9.1b1/metadata/raw.CoreFoundation/x86_64-10.6.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   304008 2021-08-03 12:27:37.000000 pyobjc-framework-Cocoa-9.1b1/metadata/raw.CoreFoundation/x86_64-10.7.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   305298 2021-08-03 12:27:37.000000 pyobjc-framework-Cocoa-9.1b1/metadata/raw.CoreFoundation/x86_64-10.8.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   312873 2021-08-03 12:27:37.000000 pyobjc-framework-Cocoa-9.1b1/metadata/raw.CoreFoundation/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   315071 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/metadata/raw.CoreFoundation/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   331013 2022-10-29 12:03:04.000000 pyobjc-framework-Cocoa-9.1b1/metadata/raw.CoreFoundation/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)   331330 2023-02-19 10:50:34.000000 pyobjc-framework-Cocoa-9.1b1/metadata/raw.CoreFoundation/x86_64-13.3.fwinfo
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:17:02.744452 pyobjc-framework-Cocoa-9.1b1/metadata/raw.Foundation/
--rw-r--r--   0 ronald     (501) staff       (20)  1975821 2021-08-04 10:01:02.000000 pyobjc-framework-Cocoa-9.1b1/metadata/raw.Foundation/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)  1983710 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/metadata/raw.Foundation/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)  2013356 2022-10-18 09:53:23.000000 pyobjc-framework-Cocoa-9.1b1/metadata/raw.Foundation/arm64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)  2013588 2023-02-19 10:50:34.000000 pyobjc-framework-Cocoa-9.1b1/metadata/raw.Foundation/arm64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)  1595900 2021-08-03 12:27:37.000000 pyobjc-framework-Cocoa-9.1b1/metadata/raw.Foundation/x86_64-10.10.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)  1885998 2021-08-03 12:27:37.000000 pyobjc-framework-Cocoa-9.1b1/metadata/raw.Foundation/x86_64-10.15.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)  1937893 2021-08-03 12:27:37.000000 pyobjc-framework-Cocoa-9.1b1/metadata/raw.Foundation/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)  1219040 2021-08-03 12:27:37.000000 pyobjc-framework-Cocoa-9.1b1/metadata/raw.Foundation/x86_64-10.8.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)  1975537 2021-08-04 10:01:02.000000 pyobjc-framework-Cocoa-9.1b1/metadata/raw.Foundation/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)  1983921 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.1b1/metadata/raw.Foundation/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)  2013613 2022-10-18 09:53:23.000000 pyobjc-framework-Cocoa-9.1b1/metadata/raw.Foundation/x86_64-13.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)  2013845 2023-02-19 10:50:34.000000 pyobjc-framework-Cocoa-9.1b1/metadata/raw.Foundation/x86_64-13.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-Cocoa-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:17:02.774628 pyobjc-framework-Cocoa-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)     2530 2023-03-25 14:20:30.000000 pyobjc-framework-Cocoa-9.1b1/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       57 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.1b1/todo.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:59.616702 pyobjc-framework-Cocoa-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:57.866010 pyobjc-framework-Cocoa-9.2/Examples/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:57.854144 pyobjc-framework-Cocoa-9.2/Examples/AppKit/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:57.888209 pyobjc-framework-Cocoa-9.2/Examples/AppKit/ClassBrowser/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:57.890226 pyobjc-framework-Cocoa-9.2/Examples/AppKit/ClassBrowser/ClassBrowser.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      909 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/ClassBrowser/ClassBrowser.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      495 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/ClassBrowser/ClassBrowser.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     6756 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/ClassBrowser/ClassBrowser.nib/objects.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     3992 2022-01-02 11:20:34.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/ClassBrowser/ClassBrowser.py
+-rw-r--r--   0 ronald     (501) staff       (20)      348 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/ClassBrowser/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)      122 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/ClassBrowser/summary.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:57.844101 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:57.894757 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/Bookmarks/
+-rw-r--r--   0 ronald     (501) staff       (20)      209 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/Bookmarks/Bookmarks.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1317 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/Bookmarks/BookmarksDocument.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6568 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/Bookmarks/DNDArrayController.py
+-rw-r--r--   0 ronald     (501) staff       (20)      891 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/Bookmarks/DNDTableView.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:57.834624 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/Bookmarks/English.lproj/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:57.897365 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/Bookmarks/English.lproj/BookmarksDocument.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      457 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/Bookmarks/English.lproj/BookmarksDocument.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      492 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/Bookmarks/English.lproj/BookmarksDocument.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)    73726 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/Bookmarks/English.lproj/BookmarksDocument.nib/keyedobjects.nib
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:57.899520 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/Bookmarks/English.lproj/MainMenu.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      109 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/Bookmarks/English.lproj/MainMenu.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      605 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/Bookmarks/English.lproj/MainMenu.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)   157569 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/Bookmarks/English.lproj/MainMenu.nib/keyedobjects.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      569 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/Bookmarks/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)      377 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/Bookmarks/summary.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:57.914634 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ControlledPreferences/
+-rw-r--r--   0 ronald     (501) staff       (20)      307 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ControlledPreferences/ControlledPreferences.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:57.835351 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ControlledPreferences/English.lproj/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:57.923795 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ControlledPreferences/English.lproj/MainMenu.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      580 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ControlledPreferences/English.lproj/MainMenu.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      626 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ControlledPreferences/English.lproj/MainMenu.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)   194476 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ControlledPreferences/English.lproj/MainMenu.nib/keyedobjects.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      862 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ControlledPreferences/FontNameToDisplayNameTransformer.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2244 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ControlledPreferences/FontSampleDisplayView.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3451 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ControlledPreferences/PreferencesPanelController.py
+-rw-r--r--   0 ronald     (501) staff       (20)      279 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ControlledPreferences/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)      404 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ControlledPreferences/summary.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:57.933109 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/CurrencyConvBinding/
+-rw-r--r--   0 ronald     (501) staff       (20)      538 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/CurrencyConvBinding/Converter.py
+-rw-r--r--   0 ronald     (501) staff       (20)      218 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/CurrencyConvBinding/CurrencyConvBinding.py
+-rw-r--r--   0 ronald     (501) staff       (20)      152 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/CurrencyConvBinding/CurrencyConvBindingDocument.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:57.836602 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/CurrencyConvBinding/English.lproj/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:57.935442 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/CurrencyConvBinding/English.lproj/CurrencyConvBindingDocument.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      330 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/CurrencyConvBinding/English.lproj/CurrencyConvBindingDocument.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      494 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/CurrencyConvBinding/English.lproj/CurrencyConvBindingDocument.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)    38422 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/CurrencyConvBinding/English.lproj/CurrencyConvBindingDocument.nib/keyedobjects.nib
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:57.940482 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/CurrencyConvBinding/English.lproj/MainMenu.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      109 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/CurrencyConvBinding/English.lproj/MainMenu.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      605 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/CurrencyConvBinding/English.lproj/MainMenu.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)   157619 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/CurrencyConvBinding/English.lproj/MainMenu.nib/keyedobjects.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      619 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/CurrencyConvBinding/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)      368 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/CurrencyConvBinding/summary.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:57.947940 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/FilteringController/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:57.837360 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/FilteringController/English.lproj/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:57.950990 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/FilteringController/English.lproj/FilteringControllerDocument.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      676 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/FilteringController/English.lproj/FilteringControllerDocument.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      627 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/FilteringController/English.lproj/FilteringControllerDocument.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)    68377 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/FilteringController/English.lproj/FilteringControllerDocument.nib/keyedobjects.nib
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:57.955125 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/FilteringController/English.lproj/MainMenu.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      109 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/FilteringController/English.lproj/MainMenu.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      605 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/FilteringController/English.lproj/MainMenu.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)   157619 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/FilteringController/English.lproj/MainMenu.nib/keyedobjects.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     2289 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/FilteringController/FilteringArrayController.py
+-rw-r--r--   0 ronald     (501) staff       (20)      183 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/FilteringController/FilteringController.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1710 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/FilteringController/FilteringControllerDocument.py
+-rw-r--r--   0 ronald     (501) staff       (20)      619 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/FilteringController/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)      312 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/FilteringController/summary.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:57.972050 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/GraphicsBindings/
+-rw-r--r--   0 ronald     (501) staff       (20)     5040 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/GraphicsBindings/Circle.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:57.838090 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/GraphicsBindings/English.lproj/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:57.973885 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/GraphicsBindings/English.lproj/GraphicsBindingsDocument.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      756 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/GraphicsBindings/English.lproj/GraphicsBindingsDocument.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      758 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/GraphicsBindings/English.lproj/GraphicsBindingsDocument.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)   120663 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/GraphicsBindings/English.lproj/GraphicsBindingsDocument.nib/keyedobjects.nib
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:57.976471 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/GraphicsBindings/English.lproj/MainMenu.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      109 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/GraphicsBindings/English.lproj/MainMenu.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      605 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/GraphicsBindings/English.lproj/MainMenu.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)   157604 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/GraphicsBindings/English.lproj/MainMenu.nib/keyedobjects.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     2336 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/GraphicsBindings/GraphicsArrayController.py
+-rw-r--r--   0 ronald     (501) staff       (20)      456 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/GraphicsBindings/GraphicsBindings.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3372 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/GraphicsBindings/GraphicsBindingsDocument.py
+-rw-r--r--   0 ronald     (501) staff       (20)     9438 2021-10-18 19:38:40.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/GraphicsBindings/GraphicsView.py
+-rw-r--r--   0 ronald     (501) staff       (20)    16141 2023-03-03 17:21:59.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/GraphicsBindings/JoystickView.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1007 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/GraphicsBindings/RadiansToDegreesTransformer.py
+-rw-r--r--   0 ronald     (501) staff       (20)      603 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/GraphicsBindings/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)      415 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/GraphicsBindings/summary.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:57.980215 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ManualBindings/
+-rw-r--r--   0 ronald     (501) staff       (20)     3414 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ManualBindings/AppController.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:57.838676 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ManualBindings/English.lproj/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:57.981997 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ManualBindings/English.lproj/MainMenu.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      609 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ManualBindings/English.lproj/MainMenu.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      629 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ManualBindings/English.lproj/MainMenu.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)   171877 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ManualBindings/English.lproj/MainMenu.nib/keyedobjects.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      165 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ManualBindings/ManualBindings.py
+-rw-r--r--   0 ronald     (501) staff       (20)      265 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ManualBindings/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)      403 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ManualBindings/summary.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:57.985935 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/MutableTableModel/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:57.839368 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/MutableTableModel/English.lproj/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:57.995941 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/MutableTableModel/English.lproj/MainMenu.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      296 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/MutableTableModel/English.lproj/MainMenu.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      606 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/MutableTableModel/English.lproj/MainMenu.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)   154575 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/MutableTableModel/English.lproj/MainMenu.nib/keyedobjects.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     1012 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/MutableTableModel/TableModelAppDelegate.py
+-rw-r--r--   0 ronald     (501) staff       (20)      320 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/MutableTableModel/main.py
+-rw-r--r--   0 ronald     (501) staff       (20)      292 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/MutableTableModel/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       68 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/MutableTableModel/summary.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.007945 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/TableModel/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:57.839808 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/TableModel/English.lproj/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.013087 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/TableModel/English.lproj/MainMenu.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      206 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/TableModel/English.lproj/MainMenu.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      606 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/TableModel/English.lproj/MainMenu.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)   149621 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/TableModel/English.lproj/MainMenu.nib/keyedobjects.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      755 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/TableModel/TableModelAppDelegate.py
+-rw-r--r--   0 ronald     (501) staff       (20)      320 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/TableModel/main.py
+-rw-r--r--   0 ronald     (501) staff       (20)      285 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/TableModel/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       61 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/TableModel/summary.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.019065 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/TableModelWithSearch/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.019703 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/TableModelWithSearch/English.lproj/
+-rw-r--r--   0 ronald     (501) staff       (20)      530 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/TableModelWithSearch/English.lproj/InfoPlist.strings
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.032161 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/TableModelWithSearch/English.lproj/MainMenu.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      803 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/TableModelWithSearch/English.lproj/MainMenu.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      695 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/TableModelWithSearch/English.lproj/MainMenu.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)   160860 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/TableModelWithSearch/English.lproj/MainMenu.nib/keyedobjects.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     1678 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/TableModelWithSearch/FilteringArrayController.py
+-rw-r--r--   0 ronald     (501) staff       (20)      692 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/TableModelWithSearch/TableModelWithSearchAppDelegate.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4110 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/TableModelWithSearch/ToolbarCreator.py
+-rw-r--r--   0 ronald     (501) staff       (20)      422 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/TableModelWithSearch/main.py
+-rw-r--r--   0 ronald     (501) staff       (20)      294 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/TableModelWithSearch/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       87 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/TableModelWithSearch/summary.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.037201 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/TemperatureTransformer/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:57.843811 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/TemperatureTransformer/English.lproj/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.050219 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/TemperatureTransformer/English.lproj/MainMenu.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      207 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/TemperatureTransformer/English.lproj/MainMenu.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      627 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/TemperatureTransformer/English.lproj/MainMenu.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)   126518 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/TemperatureTransformer/English.lproj/MainMenu.nib/keyedobjects.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      182 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/TemperatureTransformer/Transformer.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1757 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/TemperatureTransformer/TransformerAppDelegate.py
+-rw-r--r--   0 ronald     (501) staff       (20)      270 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/TemperatureTransformer/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)      289 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/TemperatureTransformer/summary.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.058058 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ToDos/
+-rw-r--r--   0 ronald     (501) staff       (20)     1919 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ToDos/Category.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:57.844694 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ToDos/English.lproj/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.060485 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ToDos/English.lproj/MainMenu.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      109 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ToDos/English.lproj/MainMenu.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      605 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ToDos/English.lproj/MainMenu.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)   157549 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ToDos/English.lproj/MainMenu.nib/keyedobjects.nib
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.063067 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ToDos/English.lproj/ToDosDocument.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      200 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ToDos/English.lproj/ToDosDocument.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      701 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ToDos/English.lproj/ToDosDocument.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)   114048 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ToDos/English.lproj/ToDosDocument.nib/keyedobjects.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      679 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ToDos/OverdueTransformer.py
+-rw-r--r--   0 ronald     (501) staff       (20)      987 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ToDos/PriorityToColourTransformer.py
+-rw-r--r--   0 ronald     (501) staff       (20)      131 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ToDos/ToDos.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1586 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ToDos/ToDosDocument.py
+-rw-r--r--   0 ronald     (501) staff       (20)      549 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ToDos/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)      356 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ToDos/summary.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.066120 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CurrencyConverter/
+-rw-r--r--   0 ronald     (501) staff       (20)      602 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CurrencyConverter/00README.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1125 2023-03-03 17:21:59.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CurrencyConverter/CurrencyConverter.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.066788 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CurrencyConverter/English.lproj/
+-rw-r--r--   0 ronald     (501) staff       (20)      492 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CurrencyConverter/English.lproj/InfoPlist.strings
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.068572 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CurrencyConverter/English.lproj/MainMenu.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      453 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CurrencyConverter/English.lproj/MainMenu.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      552 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CurrencyConverter/English.lproj/MainMenu.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     6767 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CurrencyConverter/English.lproj/MainMenu.nib/objects.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      271 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CurrencyConverter/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)      109 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/CurrencyConverter/summary.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.074916 pyobjc-framework-Cocoa-9.2/Examples/AppKit/DatePicker/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:57.846029 pyobjc-framework-Cocoa-9.2/Examples/AppKit/DatePicker/English.lproj/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.077887 pyobjc-framework-Cocoa-9.2/Examples/AppKit/DatePicker/English.lproj/MainMenu.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)     2304 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/DatePicker/English.lproj/MainMenu.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     1021 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/DatePicker/English.lproj/MainMenu.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)    43729 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/DatePicker/English.lproj/MainMenu.nib/keyedobjects.nib
+-rw-r--r--   0 ronald     (501) staff       (20)    18184 2021-10-18 19:38:40.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/DatePicker/MyWindowController.py
+-rw-r--r--   0 ronald     (501) staff       (20)      853 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/DatePicker/ReadMe.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      100 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/DatePicker/main.py
+-rw-r--r--   0 ronald     (501) staff       (20)      251 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/DatePicker/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)      233 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/DatePicker/summary.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.081217 pyobjc-framework-Cocoa-9.2/Examples/AppKit/DotView/
+-rw-r--r--   0 ronald     (501) staff       (20)     4028 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/DotView/DotView.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.082094 pyobjc-framework-Cocoa-9.2/Examples/AppKit/DotView/English.lproj/
+-rw-r--r--   0 ronald     (501) staff       (20)    38956 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/DotView/English.lproj/MainMenu.xib
+-rw-r--r--   0 ronald     (501) staff       (20)      251 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/DotView/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)      195 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/DotView/summary.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.091616 pyobjc-framework-Cocoa-9.2/Examples/AppKit/DragItemAround/
+-rw-r--r--   0 ronald     (501) staff       (20)     5493 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/DragItemAround/DragItemAround.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.096756 pyobjc-framework-Cocoa-9.2/Examples/AppKit/DragItemAround/MainMenu.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      746 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/DragItemAround/MainMenu.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      590 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/DragItemAround/MainMenu.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)    15584 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/DragItemAround/MainMenu.nib/keyedobjects.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      264 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/DragItemAround/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       53 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/DragItemAround/summary.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.116874 pyobjc-framework-Cocoa-9.2/Examples/AppKit/FieldGraph/
+-rw-r--r--   0 ronald     (501) staff       (20)     5564 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/FieldGraph/CGraphController.py
+-rwxr-xr-x   0 ronald     (501) staff       (20)     2763 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/FieldGraph/CGraphModel.py
+-rw-r--r--   0 ronald     (501) staff       (20)     8277 2023-03-03 17:21:59.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/FieldGraph/CGraphView.py
+-rw-r--r--   0 ronald     (501) staff       (20)      422 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/FieldGraph/CrossCursor.tiff
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.117749 pyobjc-framework-Cocoa-9.2/Examples/AppKit/FieldGraph/English.lproj/
+-rw-r--r--   0 ronald     (501) staff       (20)      552 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/FieldGraph/English.lproj/InfoPlist.strings
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.129564 pyobjc-framework-Cocoa-9.2/Examples/AppKit/FieldGraph/English.lproj/MainMenu.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)     2713 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/FieldGraph/English.lproj/MainMenu.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      655 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/FieldGraph/English.lproj/MainMenu.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)    25867 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/FieldGraph/English.lproj/MainMenu.nib/keyedobjects.nib
+-rw-r--r--   0 ronald     (501) staff       (20)    13374 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/FieldGraph/English.lproj/MainMenu.nib/objects.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      163 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/FieldGraph/Main.py
+-rw-r--r--   0 ronald     (501) staff       (20)   769739 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/FieldGraph/Map.png
+-rw-r--r--   0 ronald     (501) staff       (20)      541 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/FieldGraph/fieldMath.py
+-rw-r--r--   0 ronald     (501) staff       (20)      363 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/FieldGraph/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)      207 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/FieldGraph/summary.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.132807 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Formatter/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.135555 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Formatter/MainMenu.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      199 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Formatter/MainMenu.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      626 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Formatter/MainMenu.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)   120511 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Formatter/MainMenu.nib/keyedobjects.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      639 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Formatter/main.py
+-rw-r--r--   0 ronald     (501) staff       (20)      249 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Formatter/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       75 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Formatter/summary.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.141556 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Grady/
+-rw-r--r--   0 ronald     (501) staff       (20)      858 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Grady/AppDelegate.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:57.848850 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Grady/English.lproj/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.143474 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Grady/English.lproj/MainMenu.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      408 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Grady/English.lproj/MainMenu.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      565 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Grady/English.lproj/MainMenu.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)    13462 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Grady/English.lproj/MainMenu.nib/keyedobjects.nib
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.145400 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Grady/English.lproj/TestWindow.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)     1543 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Grady/English.lproj/TestWindow.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      454 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Grady/English.lproj/TestWindow.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     8580 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Grady/English.lproj/TestWindow.nib/keyedobjects.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     2011 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Grady/MyBaseGradientView.py
+-rw-r--r--   0 ronald     (501) staff       (20)      735 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Grady/MyBezierGradientView.py
+-rw-r--r--   0 ronald     (501) staff       (20)      672 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Grady/MyRectGradientView.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3593 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Grady/MyWindowController.py
+-rw-r--r--   0 ronald     (501) staff       (20)      255 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Grady/main.py
+-rw-r--r--   0 ronald     (501) staff       (20)      246 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Grady/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       46 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Grady/summary.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.149067 pyobjc-framework-Cocoa-9.2/Examples/AppKit/PredicateEditorSample/
+-rw-r--r--   0 ronald     (501) staff       (20)      784 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/PredicateEditorSample/CaseInsensitivePredicateTemplate.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.149657 pyobjc-framework-Cocoa-9.2/Examples/AppKit/PredicateEditorSample/English.lproj/
+-rw-r--r--   0 ronald     (501) staff       (20)      328 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/PredicateEditorSample/English.lproj/Credits.rtf
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.151735 pyobjc-framework-Cocoa-9.2/Examples/AppKit/PredicateEditorSample/English.lproj/MainMenu.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      793 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/PredicateEditorSample/English.lproj/MainMenu.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      583 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/PredicateEditorSample/English.lproj/MainMenu.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)    42827 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/PredicateEditorSample/English.lproj/MainMenu.nib/keyedobjects.nib
+-rw-r--r--   0 ronald     (501) staff       (20)    13274 2023-03-03 17:21:59.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/PredicateEditorSample/MyWindowController.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1744 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/PredicateEditorSample/ReadMe.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      154 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/PredicateEditorSample/main.py
+-rw-r--r--   0 ronald     (501) staff       (20)      262 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/PredicateEditorSample/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)      386 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/PredicateEditorSample/summary.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.161759 pyobjc-framework-Cocoa-9.2/Examples/AppKit/PyInterpreter/
+-rw-r--r--   0 ronald     (501) staff       (20)     1088 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/PyInterpreter/LICENSE.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.169953 pyobjc-framework-Cocoa-9.2/Examples/AppKit/PyInterpreter/PyInterpreter.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      549 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/PyInterpreter/PyInterpreter.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      585 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/PyInterpreter/PyInterpreter.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)    13395 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/PyInterpreter/PyInterpreter.nib/keyedobjects.nib
+-rw-r--r--   0 ronald     (501) staff       (20)    18012 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/PyInterpreter/PyInterpreter.py
+-rw-r--r--   0 ronald     (501) staff       (20)      439 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/PyInterpreter/README.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      353 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/PyInterpreter/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)      180 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/PyInterpreter/summary.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.176259 pyobjc-framework-Cocoa-9.2/Examples/AppKit/PythonBrowser/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.180910 pyobjc-framework-Cocoa-9.2/Examples/AppKit/PythonBrowser/MainMenu.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      471 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/PythonBrowser/MainMenu.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      561 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/PythonBrowser/MainMenu.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     4884 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/PythonBrowser/MainMenu.nib/objects.nib
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.184118 pyobjc-framework-Cocoa-9.2/Examples/AppKit/PythonBrowser/PythonBrowser.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      313 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/PythonBrowser/PythonBrowser.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      450 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/PythonBrowser/PythonBrowser.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     2035 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/PythonBrowser/PythonBrowser.nib/objects.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     3833 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/PythonBrowser/PythonBrowser.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5898 2021-10-18 19:38:40.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/PythonBrowser/PythonBrowserModel.py
+-rw-r--r--   0 ronald     (501) staff       (20)      890 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/PythonBrowser/readme.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      257 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/PythonBrowser/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)      173 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/PythonBrowser/summary.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.191991 pyobjc-framework-Cocoa-9.2/Examples/AppKit/RoundTransparentWindow/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.195345 pyobjc-framework-Cocoa-9.2/Examples/AppKit/RoundTransparentWindow/MainMenu.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      699 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/RoundTransparentWindow/MainMenu.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      493 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/RoundTransparentWindow/MainMenu.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     4124 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/RoundTransparentWindow/MainMenu.nib/objects.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     3829 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/RoundTransparentWindow/RoundTransparentWindow.py
+-rw-r--r--   0 ronald     (501) staff       (20)   130322 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/RoundTransparentWindow/circle.tif
+-rw-r--r--   0 ronald     (501) staff       (20)   107760 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/RoundTransparentWindow/pentagram.tif
+-rw-r--r--   0 ronald     (501) staff       (20)      276 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/RoundTransparentWindow/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       51 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/RoundTransparentWindow/summary.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.200872 pyobjc-framework-Cocoa-9.2/Examples/AppKit/SimpleService/
+-rw-r--r--   0 ronald     (501) staff       (20)     1588 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/SimpleService/README.rtf
+-rw-r--r--   0 ronald     (501) staff       (20)     2816 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/SimpleService/ServiceTest.py
+-rw-r--r--   0 ronald     (501) staff       (20)      325 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/SimpleService/SimpleService_main.py
+-rwxr-xr-x   0 ronald     (501) staff       (20)      116 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/SimpleService/rebuild.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1001 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/SimpleService/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       54 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/SimpleService/summary.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.212307 pyobjc-framework-Cocoa-9.2/Examples/AppKit/TableModel/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:57.851966 pyobjc-framework-Cocoa-9.2/Examples/AppKit/TableModel/English.lproj/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.215666 pyobjc-framework-Cocoa-9.2/Examples/AppKit/TableModel/English.lproj/MainMenu.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      294 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/TableModel/English.lproj/MainMenu.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      586 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/TableModel/English.lproj/MainMenu.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     6659 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/TableModel/English.lproj/MainMenu.nib/objects.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     3679 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/TableModel/TableModel.py
+-rw-r--r--   0 ronald     (501) staff       (20)      314 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/TableModel/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       55 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/TableModel/summary.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.217954 pyobjc-framework-Cocoa-9.2/Examples/AppKit/TinyTinyEdit/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.220384 pyobjc-framework-Cocoa-9.2/Examples/AppKit/TinyTinyEdit/MainMenu.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      109 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/TinyTinyEdit/MainMenu.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      484 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/TinyTinyEdit/MainMenu.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     7340 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/TinyTinyEdit/MainMenu.nib/objects.nib
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.222102 pyobjc-framework-Cocoa-9.2/Examples/AppKit/TinyTinyEdit/TinyTinyDocument.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      289 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/TinyTinyEdit/TinyTinyDocument.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      451 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/TinyTinyEdit/TinyTinyDocument.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     1694 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/TinyTinyEdit/TinyTinyDocument.nib/objects.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     1180 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/TinyTinyEdit/TinyTinyEdit.py
+-rw-r--r--   0 ronald     (501) staff       (20)      596 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/TinyTinyEdit/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       50 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/TinyTinyEdit/summary.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.225519 pyobjc-framework-Cocoa-9.2/Examples/AppKit/TinyURLService/
+-rw-r--r--   0 ronald     (501) staff       (20)     1366 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/TinyURLService/README.rtf
+-rw-r--r--   0 ronald     (501) staff       (20)     2574 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/TinyURLService/TinyURLService.py
+-rwxr-xr-x   0 ronald     (501) staff       (20)      116 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/TinyURLService/rebuild.py
+-rw-r--r--   0 ronald     (501) staff       (20)      688 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/TinyURLService/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)      105 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/TinyURLService/summary.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.236581 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Todo/
+-rw-r--r--   0 ronald     (501) staff       (20)      784 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Todo/00ReadMe.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     5449 2023-03-03 17:21:59.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Todo/CalendarMatrix.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.239766 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Todo/English.lproj/
+-rw-r--r--   0 ronald     (501) staff       (20)      436 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Todo/English.lproj/Credits.rtf
+-rw-r--r--   0 ronald     (501) staff       (20)      416 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Todo/English.lproj/InfoPlist.strings
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.243404 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Todo/English.lproj/MainMenu.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      286 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Todo/English.lproj/MainMenu.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      243 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Todo/English.lproj/MainMenu.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     5115 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Todo/English.lproj/MainMenu.nib/objects.nib
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.253389 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Todo/English.lproj/ToDoDocument.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      791 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Todo/English.lproj/ToDoDocument.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      422 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Todo/English.lproj/ToDoDocument.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     4408 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Todo/English.lproj/ToDoDocument.nib/objects.nib
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.256453 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Todo/English.lproj/ToDoInfoWindow.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      980 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Todo/English.lproj/ToDoInfoWindow.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      596 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Todo/English.lproj/ToDoInfoWindow.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     9393 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Todo/English.lproj/ToDoInfoWindow.nib/objects.nib
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.258760 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Todo/Icons/
+-rw-r--r--   0 ronald     (501) staff       (20)    48041 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Todo/Icons/ToDoApp.icns
+-rw-r--r--   0 ronald     (501) staff       (20)    50278 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Todo/Icons/ToDoDoc.icns
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.264882 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Todo/Images/
+-rw-r--r--   0 ronald     (501) staff       (20)      422 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Todo/Images/DeferredMark.tiff
+-rw-r--r--   0 ronald     (501) staff       (20)      412 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Todo/Images/DoneMark.tiff
+-rw-r--r--   0 ronald     (501) staff       (20)      412 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Todo/Images/LeftArrow.tiff
+-rw-r--r--   0 ronald     (501) staff       (20)      422 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Todo/Images/RightArrow.tiff
+-rw-r--r--   0 ronald     (501) staff       (20)    11377 2023-03-03 17:21:59.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Todo/InfoWindowController.py
+-rw-r--r--   0 ronald     (501) staff       (20)      674 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Todo/SelectionNotifyMatrix.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2304 2023-03-03 17:21:59.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Todo/ToDoCell.py
+-rw-r--r--   0 ronald     (501) staff       (20)    11589 2023-03-03 17:21:59.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Todo/ToDoDocument.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4676 2023-03-03 17:21:59.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Todo/ToDoItem.py
+-rw-r--r--   0 ronald     (501) staff       (20)      263 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Todo/TodoAppDelegate.py
+-rw-r--r--   0 ronald     (501) staff       (20)      390 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Todo/main.py
+-rw-r--r--   0 ronald     (501) staff       (20)      926 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Todo/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)      251 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/Todo/summary.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.276895 pyobjc-framework-Cocoa-9.2/Examples/AppKit/WebServicesTool/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.277724 pyobjc-framework-Cocoa-9.2/Examples/AppKit/WebServicesTool/English.lproj/
+-rw-r--r--   0 ronald     (501) staff       (20)      456 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/WebServicesTool/English.lproj/InfoPlist.strings
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.280653 pyobjc-framework-Cocoa-9.2/Examples/AppKit/WebServicesTool/English.lproj/MainMenu.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      304 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/WebServicesTool/English.lproj/MainMenu.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      484 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/WebServicesTool/English.lproj/MainMenu.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     9289 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/WebServicesTool/English.lproj/MainMenu.nib/keyedobjects.nib
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.283488 pyobjc-framework-Cocoa-9.2/Examples/AppKit/WebServicesTool/English.lproj/WSTConnection.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      626 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/WebServicesTool/English.lproj/WSTConnection.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      585 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/WebServicesTool/English.lproj/WSTConnection.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     8150 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/WebServicesTool/English.lproj/WSTConnection.nib/keyedobjects.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     1088 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/WebServicesTool/LICENSE.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      252 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/WebServicesTool/Main.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1956 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/WebServicesTool/Preferences.png
+-rw-r--r--   0 ronald     (501) staff       (20)      735 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/WebServicesTool/README.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1623 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/WebServicesTool/Reload.png
+-rw-r--r--   0 ronald     (501) staff       (20)    52383 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/WebServicesTool/WST.icns
+-rw-r--r--   0 ronald     (501) staff       (20)    18131 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/WebServicesTool/WST.png
+-rw-r--r--   0 ronald     (501) staff       (20)     1106 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/WebServicesTool/WSTApplicationDelegateClass.py
+-rw-r--r--   0 ronald     (501) staff       (20)    18766 2021-10-18 19:38:40.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/WebServicesTool/WSTConnectionWindowControllerClass.py
+-rw-r--r--   0 ronald     (501) staff       (20)      419 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/WebServicesTool/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)      191 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/AppKit/WebServicesTool/summary.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:57.865458 pyobjc-framework-Cocoa-9.2/Examples/Foundation/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.296446 pyobjc-framework-Cocoa-9.2/Examples/Foundation/Scripts/
+-rw-r--r--   0 ronald     (501) staff       (20)     1102 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/Foundation/Scripts/dictionary.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1266 2023-03-03 17:21:59.000000 pyobjc-framework-Cocoa-9.2/Examples/Foundation/Scripts/findPython.py
+-rw-r--r--   0 ronald     (501) staff       (20)      500 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/Foundation/Scripts/pydict-to-objcdict.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2380 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.2/Examples/Foundation/Scripts/rendezvous.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1264 2022-02-06 09:24:04.000000 pyobjc-framework-Cocoa-9.2/Examples/Foundation/Scripts/simple-kvo.py
+-rw-r--r--   0 ronald     (501) staff       (20)      501 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.2/Examples/Foundation/Scripts/super-call.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:57.865715 pyobjc-framework-Cocoa-9.2/Examples/OpenGL/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.301477 pyobjc-framework-Cocoa-9.2/Examples/OpenGL/OpenGLDemo/
+-rw-r--r--   0 ronald     (501) staff       (20)     1088 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/OpenGL/OpenGLDemo/LICENSE.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.303829 pyobjc-framework-Cocoa-9.2/Examples/OpenGL/OpenGLDemo/OpenGLDemo.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      294 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/OpenGL/OpenGLDemo/OpenGLDemo.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      589 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/OpenGL/OpenGLDemo/OpenGLDemo.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     4395 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/OpenGL/OpenGLDemo/OpenGLDemo.nib/objects.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     2257 2022-10-18 09:53:23.000000 pyobjc-framework-Cocoa-9.2/Examples/OpenGL/OpenGLDemo/OpenGLDemo.py
+-rw-r--r--   0 ronald     (501) staff       (20)      403 2023-02-19 10:50:34.000000 pyobjc-framework-Cocoa-9.2/Examples/OpenGL/OpenGLDemo/README.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      352 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/OpenGL/OpenGLDemo/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)      225 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/OpenGL/OpenGLDemo/summary.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.304599 pyobjc-framework-Cocoa-9.2/Examples/Twisted/
+-rw-r--r--   0 ronald     (501) staff       (20)      120 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/Twisted/README.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.311956 pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.343518 pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool/English.lproj/
+-rw-r--r--   0 ronald     (501) staff       (20)      456 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool/English.lproj/InfoPlist.strings
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.351447 pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool/English.lproj/MainMenu.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      304 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool/English.lproj/MainMenu.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      484 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool/English.lproj/MainMenu.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     9289 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool/English.lproj/MainMenu.nib/keyedobjects.nib
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.363110 pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool/English.lproj/WSTConnection.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      626 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool/English.lproj/WSTConnection.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      585 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool/English.lproj/WSTConnection.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     8150 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool/English.lproj/WSTConnection.nib/keyedobjects.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     1088 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool/LICENSE.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      302 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool/Main.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1956 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool/Preferences.png
+-rw-r--r--   0 ronald     (501) staff       (20)     1169 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool/ReadMe.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1623 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool/Reload.png
+-rw-r--r--   0 ronald     (501) staff       (20)    52383 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool/WST.icns
+-rw-r--r--   0 ronald     (501) staff       (20)    18131 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool/WST.png
+-rw-r--r--   0 ronald     (501) staff       (20)     1423 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool/WSTApplicationDelegateClass.py
+-rw-r--r--   0 ronald     (501) staff       (20)    16508 2023-03-03 17:21:59.000000 pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool/WSTConnectionWindowControllerClass.py
+-rw-r--r--   0 ronald     (501) staff       (20)      419 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)      105 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool/summary.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.334694 pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool-CocoaBindings/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.335709 pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool-CocoaBindings/English.lproj/
+-rw-r--r--   0 ronald     (501) staff       (20)      456 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool-CocoaBindings/English.lproj/InfoPlist.strings
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.339060 pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool-CocoaBindings/English.lproj/MainMenu.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      304 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool-CocoaBindings/English.lproj/MainMenu.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      484 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool-CocoaBindings/English.lproj/MainMenu.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     9289 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool-CocoaBindings/English.lproj/MainMenu.nib/keyedobjects.nib
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.342259 pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool-CocoaBindings/English.lproj/WSTConnection.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)      626 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool-CocoaBindings/English.lproj/WSTConnection.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      585 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool-CocoaBindings/English.lproj/WSTConnection.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     9876 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool-CocoaBindings/English.lproj/WSTConnection.nib/keyedobjects.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     1088 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool-CocoaBindings/LICENSE.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      302 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool-CocoaBindings/Main.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1956 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool-CocoaBindings/Preferences.png
+-rw-r--r--   0 ronald     (501) staff       (20)     1083 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool-CocoaBindings/README.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1050 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool-CocoaBindings/RPCMethod.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1623 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool-CocoaBindings/Reload.png
+-rw-r--r--   0 ronald     (501) staff       (20)    52383 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool-CocoaBindings/WST.icns
+-rw-r--r--   0 ronald     (501) staff       (20)    18131 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool-CocoaBindings/WST.png
+-rw-r--r--   0 ronald     (501) staff       (20)     1390 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool-CocoaBindings/WSTApplicationDelegateClass.py
+-rw-r--r--   0 ronald     (501) staff       (20)    14871 2021-10-18 19:38:40.000000 pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool-CocoaBindings/WSTConnectionWindowControllerClass.py
+-rw-r--r--   0 ronald     (501) staff       (20)      362 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool-CocoaBindings/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)      137 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool-CocoaBindings/summary.txt
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-Cocoa-9.2/LICENSE.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:57.869084 pyobjc-framework-Cocoa-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.378057 pyobjc-framework-Cocoa-9.2/Lib/AppKit/
+-rw-r--r--   0 ronald     (501) staff       (20)     5116 2023-06-05 10:04:20.000000 pyobjc-framework-Cocoa-9.2/Lib/AppKit/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)   871462 2023-05-27 09:46:33.000000 pyobjc-framework-Cocoa-9.2/Lib/AppKit/_metadata.py
+-rw-r--r--   0 ronald     (501) staff       (20)      650 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.2/Lib/AppKit/_nsapp.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.386946 pyobjc-framework-Cocoa-9.2/Lib/CGL/
+-rw-r--r--   0 ronald     (501) staff       (20)     7034 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Lib/CGL/PyObjC.bridgesupport
+-rw-r--r--   0 ronald     (501) staff       (20)      432 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Lib/CGL/__init__.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.387739 pyobjc-framework-Cocoa-9.2/Lib/Cocoa/
+-rw-r--r--   0 ronald     (501) staff       (20)      640 2023-06-05 10:04:42.000000 pyobjc-framework-Cocoa-9.2/Lib/Cocoa/__init__.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.392187 pyobjc-framework-Cocoa-9.2/Lib/CoreFoundation/
+-rw-r--r--   0 ronald     (501) staff       (20)     1270 2023-06-06 12:09:06.000000 pyobjc-framework-Cocoa-9.2/Lib/CoreFoundation/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)   153344 2023-05-27 09:46:33.000000 pyobjc-framework-Cocoa-9.2/Lib/CoreFoundation/_metadata.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2880 2021-10-18 19:38:40.000000 pyobjc-framework-Cocoa-9.2/Lib/CoreFoundation/_static.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.398756 pyobjc-framework-Cocoa-9.2/Lib/Foundation/
+-rw-r--r--   0 ronald     (501) staff       (20)     5955 2023-06-06 12:09:06.000000 pyobjc-framework-Cocoa-9.2/Lib/Foundation/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)      713 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.2/Lib/Foundation/_context.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1404 2021-08-04 10:13:27.000000 pyobjc-framework-Cocoa-9.2/Lib/Foundation/_functiondefines.py
+-rw-r--r--   0 ronald     (501) staff       (20)   441694 2023-05-27 09:46:33.000000 pyobjc-framework-Cocoa-9.2/Lib/Foundation/_metadata.py
+-rw-r--r--   0 ronald     (501) staff       (20)      394 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Lib/Foundation/_nsindexset.py
+-rw-r--r--   0 ronald     (501) staff       (20)     8402 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Lib/Foundation/_nsobject.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.401066 pyobjc-framework-Cocoa-9.2/Lib/PyObjCTools/
+-rw-r--r--   0 ronald     (501) staff       (20)      840 2021-10-18 19:38:40.000000 pyobjc-framework-Cocoa-9.2/Lib/PyObjCTools/AppCategories.py
+-rw-r--r--   0 ronald     (501) staff       (20)     9669 2023-03-03 17:21:59.000000 pyobjc-framework-Cocoa-9.2/Lib/PyObjCTools/AppHelper.py
+-rw-r--r--   0 ronald     (501) staff       (20)     7913 2022-10-29 10:49:37.000000 pyobjc-framework-Cocoa-9.2/Lib/PyObjCTools/Conversion.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1026 2021-10-18 19:38:40.000000 pyobjc-framework-Cocoa-9.2/Lib/PyObjCTools/FndCategories.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.406615 pyobjc-framework-Cocoa-9.2/Lib/pyobjc_framework_Cocoa.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2176 2023-06-07 00:07:57.000000 pyobjc-framework-Cocoa-9.2/Lib/pyobjc_framework_Cocoa.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)    40086 2023-06-07 00:07:57.000000 pyobjc-framework-Cocoa-9.2/Lib/pyobjc_framework_Cocoa.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:07:57.000000 pyobjc-framework-Cocoa-9.2/Lib/pyobjc_framework_Cocoa.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:48:28.000000 pyobjc-framework-Cocoa-9.2/Lib/pyobjc_framework_Cocoa.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       17 2023-06-07 00:07:57.000000 pyobjc-framework-Cocoa-9.2/Lib/pyobjc_framework_Cocoa.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       62 2023-06-07 00:07:57.000000 pyobjc-framework-Cocoa-9.2/Lib/pyobjc_framework_Cocoa.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/MANIFEST.in
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:58.469966 pyobjc-framework-Cocoa-9.2/Modules/
+-rw-r--r--   0 ronald     (501) staff       (20)     1233 2022-10-18 09:53:23.000000 pyobjc-framework-Cocoa-9.2/Modules/_AppKit.m
+-rw-r--r--   0 ronald     (501) staff       (20)     2793 2021-09-25 15:02:56.000000 pyobjc-framework-Cocoa-9.2/Modules/_AppKit_appmain.m
+-rw-r--r--   0 ronald     (501) staff       (20)      204 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.2/Modules/_AppKit_carbon.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1603 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.2/Modules/_AppKit_inlines.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9531 2022-10-18 09:53:23.000000 pyobjc-framework-Cocoa-9.2/Modules/_AppKit_nsbezierpath.m
+-rw-r--r--   0 ronald     (501) staff       (20)    15908 2022-02-17 10:15:09.000000 pyobjc-framework-Cocoa-9.2/Modules/_AppKit_nsbitmap.m
+-rw-r--r--   0 ronald     (501) staff       (20)     3071 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.2/Modules/_AppKit_nsfont.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1918 2022-01-02 11:04:26.000000 pyobjc-framework-Cocoa-9.2/Modules/_AppKit_nsview.m
+-rw-r--r--   0 ronald     (501) staff       (20)    11805 2022-06-15 11:57:00.000000 pyobjc-framework-Cocoa-9.2/Modules/_AppKit_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     2882 2021-10-26 08:03:21.000000 pyobjc-framework-Cocoa-9.2/Modules/_CoreFoundation.m
+-rw-r--r--   0 ronald     (501) staff       (20)     2822 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.2/Modules/_CoreFoundation_CFBag.m
+-rw-r--r--   0 ronald     (501) staff       (20)     2803 2021-10-18 19:38:40.000000 pyobjc-framework-Cocoa-9.2/Modules/_CoreFoundation_CFBinaryHeap.m
+-rw-r--r--   0 ronald     (501) staff       (20)     2449 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.2/Modules/_CoreFoundation_CFBitVector.m
+-rw-r--r--   0 ronald     (501) staff       (20)    12276 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Modules/_CoreFoundation_CFCalendar.m
+-rw-r--r--   0 ronald     (501) staff       (20)     2568 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Modules/_CoreFoundation_CFDictionary.m
+-rw-r--r--   0 ronald     (501) staff       (20)     4883 2021-10-26 08:03:21.000000 pyobjc-framework-Cocoa-9.2/Modules/_CoreFoundation_CFFileDescriptor.m
+-rw-r--r--   0 ronald     (501) staff       (20)    11008 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Modules/_CoreFoundation_CFMachPort.m
+-rw-r--r--   0 ronald     (501) staff       (20)     4939 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Modules/_CoreFoundation_CFMessagePort.m
+-rw-r--r--   0 ronald     (501) staff       (20)     6619 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Modules/_CoreFoundation_CFNumber.m
+-rw-r--r--   0 ronald     (501) staff       (20)     8015 2021-10-18 19:38:40.000000 pyobjc-framework-Cocoa-9.2/Modules/_CoreFoundation_CFNumberFormatter.m
+-rw-r--r--   0 ronald     (501) staff       (20)     3070 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Modules/_CoreFoundation_CFReadStream.m
+-rw-r--r--   0 ronald     (501) staff       (20)     4902 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Modules/_CoreFoundation_CFRunLoopObserver.m
+-rw-r--r--   0 ronald     (501) staff       (20)     6424 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Modules/_CoreFoundation_CFRunLoopSource.m
+-rw-r--r--   0 ronald     (501) staff       (20)     4777 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Modules/_CoreFoundation_CFRunLoopTimer.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1527 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Modules/_CoreFoundation_CFSet.m
+-rw-r--r--   0 ronald     (501) staff       (20)    11376 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Modules/_CoreFoundation_CFSocket.m
+-rw-r--r--   0 ronald     (501) staff       (20)     6203 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Modules/_CoreFoundation_CFTree.m
+-rw-r--r--   0 ronald     (501) staff       (20)     2904 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/Modules/_CoreFoundation_CFWriteStream.m
+-rw-r--r--   0 ronald     (501) staff       (20)     4309 2021-10-18 19:38:40.000000 pyobjc-framework-Cocoa-9.2/Modules/_CoreFoundation_inlines.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1033 2022-10-18 09:53:23.000000 pyobjc-framework-Cocoa-9.2/Modules/_Foundation.m
+-rw-r--r--   0 ronald     (501) staff       (20)     6519 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.2/Modules/_Foundation_inlines.m
+-rw-r--r--   0 ronald     (501) staff       (20)     4024 2022-01-02 11:04:26.000000 pyobjc-framework-Cocoa-9.2/Modules/_Foundation_netservice.m
+-rw-r--r--   0 ronald     (501) staff       (20)     4088 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.2/Modules/_Foundation_protocols.m
+-rw-r--r--   0 ronald     (501) staff       (20)     4882 2023-03-03 17:21:31.000000 pyobjc-framework-Cocoa-9.2/Modules/_Foundation_string.m
+-rw-r--r--   0 ronald     (501) staff       (20)     3230 2021-10-18 19:38:40.000000 pyobjc-framework-Cocoa-9.2/Modules/_Foundation_typecode.m
+-rw-r--r--   0 ronald     (501) staff       (20)     9014 2023-02-19 10:50:34.000000 pyobjc-framework-Cocoa-9.2/Modules/pyobjc-api.h
+-rw-r--r--   0 ronald     (501) staff       (20)    13094 2023-06-06 07:56:22.000000 pyobjc-framework-Cocoa-9.2/Modules/pyobjc-compat.h
+-rw-r--r--   0 ronald     (501) staff       (20)     7419 2021-10-18 19:38:40.000000 pyobjc-framework-Cocoa-9.2/Modules/testhelper.m
+-rw-r--r--   0 ronald     (501) staff       (20)     1965 2023-06-07 00:07:59.615652 pyobjc-framework-Cocoa-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:59.173968 pyobjc-framework-Cocoa-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3880 2023-03-03 17:21:59.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/guitest_graphics.py
+-rw-r--r--   0 ronald     (501) staff       (20)      962 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/guitest_nsalert.py
+-rw-r--r--   0 ronald     (501) staff       (20)      580 2022-01-02 11:04:26.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_appcategories.py
+-rw-r--r--   0 ronald     (501) staff       (20)      563 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_apphelper.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4323 2022-06-25 20:11:26.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_appkit_protocols.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2151 2023-03-24 18:54:07.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_appkiterrors.py
+-rw-r--r--   0 ronald     (501) staff       (20)     8801 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfarray.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5741 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfattributedstring.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5237 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfbag.py
+-rw-r--r--   0 ronald     (501) staff       (20)    13234 2022-01-02 11:04:26.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfbase.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4755 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfbinaryheap.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4871 2021-04-09 10:15:21.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfbitvector.py
+-rw-r--r--   0 ronald     (501) staff       (20)    14577 2022-06-26 21:30:10.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfbundle.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4356 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfbyteorder.py
+-rw-r--r--   0 ronald     (501) staff       (20)    10072 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfcalendar.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1775 2022-07-30 15:06:02.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfcgtypes.py
+-rw-r--r--   0 ronald     (501) staff       (20)     7834 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfcharacterset.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4857 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfdata.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5004 2023-03-25 14:19:27.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfdate.py
+-rw-r--r--   0 ronald     (501) staff       (20)     9313 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfdateformatter.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6802 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfdictionary.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4582 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cferror.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1730 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cffiledescriptor.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4322 2022-10-29 10:34:19.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cffilesecurity.py
+-rw-r--r--   0 ronald     (501) staff       (20)     7526 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cflocale.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2759 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfmachport.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4714 2021-06-07 08:31:49.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfmessageport.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5044 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfnotificationcenter.py
+-rw-r--r--   0 ronald     (501) staff       (20)    10473 2022-01-02 11:04:26.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfnumber.py
+-rw-r--r--   0 ronald     (501) staff       (20)     8538 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfnumberformatter.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1760 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfplugin.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6687 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfpreferences.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6541 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfpropertylist.py
+-rw-r--r--   0 ronald     (501) staff       (20)    15035 2021-04-09 10:15:21.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfrunloop.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4969 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfset.py
+-rw-r--r--   0 ronald     (501) staff       (20)     9224 2022-01-02 11:04:26.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfsocket.py
+-rw-r--r--   0 ronald     (501) staff       (20)    22990 2023-03-03 17:21:59.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfstream.py
+-rw-r--r--   0 ronald     (501) staff       (20)    34799 2023-05-04 11:00:07.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfstring.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3352 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfstringtokenizer.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5420 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cftimezone.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5171 2022-01-02 11:04:26.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cftree.py
+-rw-r--r--   0 ronald     (501) staff       (20)    36145 2023-02-19 10:50:34.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfurl.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3938 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfurlaccess.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2937 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfurlenumerator.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6328 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfusernotification.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6022 2022-01-02 11:04:26.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfuuid.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4590 2022-01-02 11:04:26.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfxmlnode.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2797 2021-04-09 10:15:21.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfxmlparser.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1528 2023-05-04 11:00:07.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cocoa.py
+-rw-r--r--   0 ronald     (501) staff       (20)      874 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_constants.py
+-rw-r--r--   0 ronald     (501) staff       (20)      994 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_convenience.py
+-rw-r--r--   0 ronald     (501) staff       (20)     9051 2023-03-03 17:21:59.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_conversion.py
+-rw-r--r--   0 ronald     (501) staff       (20)      466 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_fndcategories.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2253 2022-01-02 11:04:26.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_foundation.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6646 2022-06-23 11:03:28.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_foundationerrors.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4058 2023-03-03 17:21:59.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_globals.py
+-rw-r--r--   0 ronald     (501) staff       (20)    21275 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_keyvalue.py
+-rw-r--r--   0 ronald     (501) staff       (20)    34718 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsaccessibility.py
+-rw-r--r--   0 ronald     (501) staff       (20)      822 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsaccessibilitycustomaction.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2335 2022-06-25 20:12:49.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsaccessibilitycustomrotor.py
+-rw-r--r--   0 ronald     (501) staff       (20)    27068 2022-06-25 20:06:25.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsaccessibilityprotocols.py
+-rw-r--r--   0 ronald     (501) staff       (20)      478 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsactioncell.py
+-rw-r--r--   0 ronald     (501) staff       (20)     7307 2022-01-02 11:04:26.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsaffinetransform.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2233 2022-06-25 09:07:01.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsalert.py
+-rw-r--r--   0 ronald     (501) staff       (20)      254 2022-06-25 20:11:55.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsalignmentfeedbackfilter.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2574 2022-06-25 09:02:27.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsanimation.py
+-rw-r--r--   0 ronald     (501) staff       (20)      824 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsanimationcontext.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1596 2022-06-25 20:14:24.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsappearance.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2262 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsappleeventdescriptor.py
+-rw-r--r--   0 ronald     (501) staff       (20)      798 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsappleeventmanager.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1302 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsapplescript.py
+-rw-r--r--   0 ronald     (501) staff       (20)    19842 2022-12-16 16:43:02.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsapplication.py
+-rw-r--r--   0 ronald     (501) staff       (20)      385 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsapplicationscripting.py
+-rw-r--r--   0 ronald     (501) staff       (20)      376 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsarchiver.py
+-rw-r--r--   0 ronald     (501) staff       (20)    19206 2023-03-03 17:21:59.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsarray.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1911 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsarraycontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6160 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsatstypesetter.py
+-rw-r--r--   0 ronald     (501) staff       (20)    19107 2022-06-23 11:03:28.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsattributedstring.py
+-rw-r--r--   0 ronald     (501) staff       (20)    12805 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsattributedstring_appkit.py
+-rw-r--r--   0 ronald     (501) staff       (20)      406 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsautoreleasepool.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1044 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsbackgroundactivityscheduler.py
+-rw-r--r--   0 ronald     (501) staff       (20)     7004 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsbezierpath.py
+-rw-r--r--   0 ronald     (501) staff       (20)      504 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsbitmap.py
+-rw-r--r--   0 ronald     (501) staff       (20)    12549 2023-03-03 17:21:59.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsbitmapimagerep.py
+-rw-r--r--   0 ronald     (501) staff       (20)      982 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsbox.py
+-rw-r--r--   0 ronald     (501) staff       (20)    11790 2022-06-25 09:03:05.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsbrowser.py
+-rw-r--r--   0 ronald     (501) staff       (20)      375 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsbrowsercell.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2284 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsbundle.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1867 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsbutton.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4422 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsbuttoncell.py
+-rw-r--r--   0 ronald     (501) staff       (20)      702 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsbuttontouchbaritem.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2635 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsbytecountformatter.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4721 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsbyteorder.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1451 2022-06-27 16:50:29.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nscache.py
+-rw-r--r--   0 ronald     (501) staff       (20)      354 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nscachedimagerep.py
+-rw-r--r--   0 ronald     (501) staff       (20)    10393 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nscalendar.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1233 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nscalendardate.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3293 2022-06-25 09:02:12.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nscandidatelisttouchbaritem.py
+-rw-r--r--   0 ronald     (501) staff       (20)     9505 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nscell.py
+-rw-r--r--   0 ronald     (501) staff       (20)      546 2021-04-09 10:15:21.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nscharacterset.py
+-rw-r--r--   0 ronald     (501) staff       (20)      248 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsclassdescription.py
+-rw-r--r--   0 ronald     (501) staff       (20)      705 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsclipview.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5724 2023-03-03 18:02:55.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nscoder.py
+-rw-r--r--   0 ronald     (501) staff       (20)    11151 2022-06-25 09:00:51.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nscollectionview.py
+-rw-r--r--   0 ronald     (501) staff       (20)     8268 2022-06-25 09:04:20.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nscollectionviewcompositionallayout.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4958 2022-06-25 09:00:54.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nscollectionviewflowlayout.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1847 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nscollectionviewlayout.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2922 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nscolor.py
+-rw-r--r--   0 ronald     (501) staff       (20)      568 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nscolorlist.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2585 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nscolorpanel.py
+-rw-r--r--   0 ronald     (501) staff       (20)      494 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nscolorpickertouchbaritem.py
+-rw-r--r--   0 ronald     (501) staff       (20)      812 2022-06-25 09:03:15.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nscolorpicking.py
+-rw-r--r--   0 ronald     (501) staff       (20)      290 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nscolorsampler.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1442 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nscolorspace.py
+-rw-r--r--   0 ronald     (501) staff       (20)      801 2022-06-26 21:30:09.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nscolorwell.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1932 2022-06-25 09:00:04.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nscombobox.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1606 2022-06-25 09:00:01.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nscomboboxcell.py
+-rw-r--r--   0 ronald     (501) staff       (20)      784 2022-06-15 11:57:00.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nscombobutton.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2409 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nscomparisonpredicate.py
+-rw-r--r--   0 ronald     (501) staff       (20)      409 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nscompoundpredicate.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1836 2022-06-25 20:10:39.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsconnection.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3480 2022-06-25 09:01:58.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nscontrol.py
+-rw-r--r--   0 ronald     (501) staff       (20)      619 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nscontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)      227 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nscredentialstorage.py
+-rw-r--r--   0 ronald     (501) staff       (20)      578 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nscursor.py
+-rw-r--r--   0 ronald     (501) staff       (20)      782 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nscustomimagerep.py
+-rw-r--r--   0 ronald     (501) staff       (20)    16177 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsdata.py
+-rw-r--r--   0 ronald     (501) staff       (20)      432 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsdate.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3475 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsdatecomponentsformatter.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3412 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsdateformatter.py
+-rw-r--r--   0 ronald     (501) staff       (20)      407 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsdateinterval.py
+-rw-r--r--   0 ronald     (501) staff       (20)      654 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsdateintervalformatter.py
+-rw-r--r--   0 ronald     (501) staff       (20)      760 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsdatepicker.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2586 2022-06-25 20:13:11.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsdatepickercell.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1110 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsdebug.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4450 2022-06-25 09:00:10.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsdecimalnumber.py
+-rw-r--r--   0 ronald     (501) staff       (20)    12696 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsdictionary.py
+-rw-r--r--   0 ronald     (501) staff       (20)      333 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsdictionarycontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)      201 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsdistributedlock.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1956 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsdistributednotificationcenter.py
+-rw-r--r--   0 ronald     (501) staff       (20)      514 2022-06-25 20:12:06.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsdocktile.py
+-rw-r--r--   0 ronald     (501) staff       (20)    14204 2022-10-21 07:44:21.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsdocument.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5313 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsdocumentcontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)     9915 2022-06-25 09:03:23.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsdragging.py
+-rw-r--r--   0 ronald     (501) staff       (20)      681 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsdraggingitem.py
+-rw-r--r--   0 ronald     (501) staff       (20)      680 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsdraggingsession.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1710 2022-06-25 20:17:11.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsdrawer.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1183 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsenergyformatter.py
+-rw-r--r--   0 ronald     (501) staff       (20)      592 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsenumerator.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5324 2021-04-09 08:48:53.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nserror.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2649 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nserrors.py
+-rw-r--r--   0 ronald     (501) staff       (20)    20933 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsevent.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3432 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsexception.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1689 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsexpression.py
+-rw-r--r--   0 ronald     (501) staff       (20)      602 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsextensioncontext.py
+-rw-r--r--   0 ronald     (501) staff       (20)      421 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsextensionitem.py
+-rw-r--r--   0 ronald     (501) staff       (20)      268 2022-06-25 20:15:06.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsextensionrequesthandling.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3425 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsfilecoordinator.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3371 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsfilehandle.py
+-rw-r--r--   0 ronald     (501) staff       (20)    24938 2023-03-03 17:21:59.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsfilemanager.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1415 2022-06-25 20:09:20.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsfilepresenter.py
+-rw-r--r--   0 ronald     (501) staff       (20)      614 2022-06-25 20:16:36.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsfilepromiseprovider.py
+-rw-r--r--   0 ronald     (501) staff       (20)      369 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsfilepromisereceiver.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1910 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsfileversion.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2001 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsfilewrapper.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5203 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsfont.py
+-rw-r--r--   0 ronald     (501) staff       (20)      505 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsfontassetrequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2728 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsfontcollection.py
+-rw-r--r--   0 ronald     (501) staff       (20)     8020 2022-07-08 16:02:54.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsfontdescriptor.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2756 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsfontmanager.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2980 2022-06-25 09:03:19.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsfontpanel.py
+-rw-r--r--   0 ronald     (501) staff       (20)      235 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsform.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2579 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsformatter.py
+-rw-r--r--   0 ronald     (501) staff       (20)      180 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsformcell.py
+-rw-r--r--   0 ronald     (501) staff       (20)      281 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsgarbagecollector.py
+-rw-r--r--   0 ronald     (501) staff       (20)    10354 2022-07-30 15:06:02.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsgeometry.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4564 2022-06-25 20:15:42.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsgesturerecognizer.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2853 2022-06-25 09:02:03.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsglyphgenerator.py
+-rw-r--r--   0 ronald     (501) staff       (20)      628 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsglyphinfo.py
+-rw-r--r--   0 ronald     (501) staff       (20)      765 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsgradient.py
+-rw-r--r--   0 ronald     (501) staff       (20)    15551 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsgraphics.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3082 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsgraphicscontext.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1476 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsgridview.py
+-rw-r--r--   0 ronald     (501) staff       (20)      332 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsgrouptouchbaritem.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1238 2022-06-25 19:36:17.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nshapticfeedback.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2272 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nshashtable.py
+-rw-r--r--   0 ronald     (501) staff       (20)      746 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nshelpmanager.py
+-rw-r--r--   0 ronald     (501) staff       (20)      823 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nshfsfiletypes.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1393 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nshost.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1699 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nshttpcookie.py
+-rw-r--r--   0 ronald     (501) staff       (20)      954 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nshttpcookiestorage.py
+-rw-r--r--   0 ronald     (501) staff       (20)    17535 2023-03-03 17:21:59.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsimage.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1043 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsimagecell.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2312 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsimagerep.py
+-rw-r--r--   0 ronald     (501) staff       (20)      517 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsimageview.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1292 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsindexpath.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4575 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsindexset.py
+-rw-r--r--   0 ronald     (501) staff       (20)      286 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsinflectionrule.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2212 2022-06-25 09:02:21.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsinputmanager.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4321 2022-06-25 09:01:45.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsinputserver.py
+-rw-r--r--   0 ronald     (501) staff       (20)      562 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsinterfacestyle.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2238 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsinvocation.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2620 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsiso8601dateformatter.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6223 2023-03-03 17:21:59.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsitemprovider.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1031 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsitemproviderreadingwriting.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2817 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsjavasetup.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1730 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsjsonserialization.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4689 2022-06-25 20:08:56.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nskeyedarchiver.py
+-rw-r--r--   0 ronald     (501) staff       (20)     9456 2022-10-29 10:34:50.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nskeyvaluebinding.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2596 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nskeyvaluecoding.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3777 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nskeyvalueobservering.py
+-rw-r--r--   0 ronald     (501) staff       (20)      245 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nslayoutanchor.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6975 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nslayoutconstraint.py
+-rw-r--r--   0 ronald     (501) staff       (20)      237 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nslayoutguide.py
+-rw-r--r--   0 ronald     (501) staff       (20)    31364 2022-10-29 10:33:31.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nslayoutmanager.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1475 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nslengthformatter.py
+-rw-r--r--   0 ronald     (501) staff       (20)      863 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nslevelindicator.py
+-rw-r--r--   0 ronald     (501) staff       (20)      787 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nslevelindicatorcell.py
+-rw-r--r--   0 ronald     (501) staff       (20)     8110 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nslinguistictagger.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3449 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nslocale.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1361 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nslocalizedstring.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1017 2022-06-25 09:07:11.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nslock.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1803 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nslog.py
+-rw-r--r--   0 ronald     (501) staff       (20)      326 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsmachport.py
+-rw-r--r--   0 ronald     (501) staff       (20)      925 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsmaptable.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1233 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsmassformatter.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4059 2022-06-25 09:06:54.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsmatrix.py
+-rw-r--r--   0 ronald     (501) staff       (20)      248 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsmeasurement.py
+-rw-r--r--   0 ronald     (501) staff       (20)      636 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsmeasurementformatter.py
+-rw-r--r--   0 ronald     (501) staff       (20)      645 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsmedialibrarybrowsercontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4383 2022-06-25 09:03:41.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsmenu.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1712 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsmenuitem.py
+-rw-r--r--   0 ronald     (501) staff       (20)      402 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsmenuitemcell.py
+-rw-r--r--   0 ronald     (501) staff       (20)      324 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsmenutoolbaritem.py
+-rw-r--r--   0 ronald     (501) staff       (20)      116 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsmenuview.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4061 2022-06-25 09:01:25.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsmetadata.py
+-rw-r--r--   0 ronald     (501) staff       (20)    14856 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsmetadataattributes.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1666 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsmethodsignature.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2701 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsmorphology.py
+-rw-r--r--   0 ronald     (501) staff       (20)      113 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsmovie.py
+-rw-r--r--   0 ronald     (501) staff       (20)      117 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsmovieview.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3555 2022-06-25 20:14:52.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsnetservices.py
+-rw-r--r--   0 ronald     (501) staff       (20)      759 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsnib.py
+-rw-r--r--   0 ronald     (501) staff       (20)      610 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsnibloading.py
+-rw-r--r--   0 ronald     (501) staff       (20)      518 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsnotification.py
+-rw-r--r--   0 ronald     (501) staff       (20)      659 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsnotificationqueue.py
+-rw-r--r--   0 ronald     (501) staff       (20)      216 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsnull.py
+-rw-r--r--   0 ronald     (501) staff       (20)     8581 2022-02-06 09:24:04.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsnumber.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6097 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsnumberformatter.py
+-rw-r--r--   0 ronald     (501) staff       (20)    10649 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsobjcruntime.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6586 2022-06-25 09:03:53.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsobject.py
+-rw-r--r--   0 ronald     (501) staff       (20)    17563 2022-01-02 11:20:34.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsobject_additions.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1115 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsobjectcontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)     8094 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsopengl.py
+-rw-r--r--   0 ronald     (501) staff       (20)      598 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsopengllayer.py
+-rw-r--r--   0 ronald     (501) staff       (20)      364 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsopenglview.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2560 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsopenpanel.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2940 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsoperation.py
+-rw-r--r--   0 ronald     (501) staff       (20)      369 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsorderedcollectionchange.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1013 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsorderedcollectiondifference.py
+-rw-r--r--   0 ronald     (501) staff       (20)     7814 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsorderedset.py
+-rw-r--r--   0 ronald     (501) staff       (20)    10318 2022-06-25 09:04:29.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsoutlineview.py
+-rw-r--r--   0 ronald     (501) staff       (20)      961 2023-03-03 17:21:59.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nspagecontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)      558 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nspagelayout.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3517 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nspanel.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1943 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsparagraphstyle.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6561 2022-06-25 09:02:33.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nspasteboard.py
+-rw-r--r--   0 ronald     (501) staff       (20)      623 2022-06-25 20:17:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nspasteboarditem.py
+-rw-r--r--   0 ronald     (501) staff       (20)      661 2022-06-25 20:06:33.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nspathcell.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1642 2023-03-03 17:21:59.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nspathcontrol.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5081 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nspathutilties.py
+-rw-r--r--   0 ronald     (501) staff       (20)      305 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nspdfinfo.py
+-rw-r--r--   0 ronald     (501) staff       (20)      689 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nspdfpanel.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1617 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nspersistentdocument.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2137 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nspersonnamecomponentsformatter.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1673 2022-10-18 09:53:24.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nspickertouchBaritem.py
+-rw-r--r--   0 ronald     (501) staff       (20)      631 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nspointerarray.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1926 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nspointerfunctions.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2364 2022-06-25 20:16:15.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nspopover.py
+-rw-r--r--   0 ronald     (501) staff       (20)      339 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nspopovertouchbaritem.py
+-rw-r--r--   0 ronald     (501) staff       (20)      661 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nspopupbutton.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1275 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nspopupbuttoncell.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1763 2022-06-25 09:01:51.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsport.py
+-rw-r--r--   0 ronald     (501) staff       (20)      254 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsportcoder.py
+-rw-r--r--   0 ronald     (501) staff       (20)      201 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsportmessage.py
+-rw-r--r--   0 ronald     (501) staff       (20)      678 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsportnameserver.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1068 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nspredicate.py
+-rw-r--r--   0 ronald     (501) staff       (20)      274 2022-06-25 20:09:10.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nspreviewrepresentingactivityitem.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1085 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsprinter.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4954 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsprintinfo.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2064 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsprintoperation.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2035 2022-06-25 09:00:18.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsprintpanel.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5012 2022-06-23 11:03:28.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsprocessinfo.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3298 2022-06-25 20:14:49.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsprogress.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1535 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsprogressindicator.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2439 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nspropertylist.py
+-rw-r--r--   0 ronald     (501) staff       (20)      560 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsproxy.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1496 2022-01-02 11:04:26.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsrange.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2424 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsregularexpression.py
+-rw-r--r--   0 ronald     (501) staff       (20)      830 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsrelativedatetimeformatter.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1846 2022-06-25 09:00:41.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsresponder.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3699 2022-06-25 09:03:13.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsruleeditor.py
+-rw-r--r--   0 ronald     (501) staff       (20)      598 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsrulermarker.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3217 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsrulerview.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1029 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsrunloop.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1562 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsrunningapplication.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4257 2022-06-25 09:01:27.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nssavepanel.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3879 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsscanner.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1474 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsscreen.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1070 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsscriptclassdescription.py
+-rw-r--r--   0 ronald     (501) staff       (20)      328 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsscriptcoercionhandler.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1015 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsscriptcommand.py
+-rw-r--r--   0 ronald     (501) staff       (20)      640 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsscriptcommanddescription.py
+-rw-r--r--   0 ronald     (501) staff       (20)      979 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsscriptkeyvaluecoding.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2456 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsscriptobjectspecifier.py
+-rw-r--r--   0 ronald     (501) staff       (20)      402 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsscriptstandardsuitecommands.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3270 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsscriptwhosetests.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2276 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsscroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3904 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsscrollview.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2663 2022-06-25 09:01:41.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsscrubber.py
+-rw-r--r--   0 ronald     (501) staff       (20)      476 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsscrubberitemview.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1285 2022-06-25 09:07:45.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsscrubberlayout.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1093 2022-06-25 20:14:50.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nssearchfield.py
+-rw-r--r--   0 ronald     (501) staff       (20)      819 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nssearchfieldcell.py
+-rw-r--r--   0 ronald     (501) staff       (20)      405 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nssearchtoolbaritem.py
+-rw-r--r--   0 ronald     (501) staff       (20)      284 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nssecuretextfield.py
+-rw-r--r--   0 ronald     (501) staff       (20)      754 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nssegmentedcell.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2704 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nssegmentedcontrol.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6705 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsset.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3864 2022-06-25 08:59:53.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nssharingservice.py
+-rw-r--r--   0 ronald     (501) staff       (20)      282 2022-06-25 20:17:40.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nssharingservicepickertoolbaritem.py
+-rw-r--r--   0 ronald     (501) staff       (20)      520 2022-06-25 20:09:36.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nssharingservicepickertouchbaritem.py
+-rw-r--r--   0 ronald     (501) staff       (20)      134 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nssimplehorizontaltypesetter.py
+-rw-r--r--   0 ronald     (501) staff       (20)      662 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsslider.py
+-rw-r--r--   0 ronald     (501) staff       (20)      429 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsslideraccessory.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1635 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsslidercell.py
+-rw-r--r--   0 ronald     (501) staff       (20)      423 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsslidertouchbaritem.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1450 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nssortdescriptor.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1225 2022-06-25 20:13:58.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nssound.py
+-rw-r--r--   0 ronald     (501) staff       (20)      603 2022-06-25 20:11:38.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsspeechrecognizer.py
+-rw-r--r--   0 ronald     (501) staff       (20)     7341 2022-06-25 09:01:49.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsspeechsynthesizer.py
+-rw-r--r--   0 ronald     (501) staff       (20)     7291 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsspellchecker.py
+-rw-r--r--   0 ronald     (501) staff       (20)      256 2022-06-25 20:14:54.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsspellprotocol.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3384 2022-06-25 09:03:34.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsspellserver.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6101 2022-06-25 09:02:42.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nssplitview.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2083 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nssplitviewcontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1799 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nssplitviewitem.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2264 2022-06-25 09:04:25.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsstackview.py
+-rw-r--r--   0 ronald     (501) staff       (20)      344 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsstatusbar.py
+-rw-r--r--   0 ronald     (501) staff       (20)      320 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsstatusbarbutton.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsstatusitem.py
+-rw-r--r--   0 ronald     (501) staff       (20)      371 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsstepper.py
+-rw-r--r--   0 ronald     (501) staff       (20)      391 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nssteppercell.py
+-rw-r--r--   0 ronald     (501) staff       (20)      557 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsstoryboard.py
+-rw-r--r--   0 ronald     (501) staff       (20)      880 2022-06-25 20:15:21.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsstoryboardsegue.py
+-rw-r--r--   0 ronald     (501) staff       (20)     7108 2022-06-25 09:02:59.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsstream.py
+-rw-r--r--   0 ronald     (501) staff       (20)    23975 2022-10-21 10:39:37.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsstring.py
+-rw-r--r--   0 ronald     (501) staff       (20)      762 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsstringdrawing.py
+-rw-r--r--   0 ronald     (501) staff       (20)      924 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstablecolumn.py
+-rw-r--r--   0 ronald     (501) staff       (20)      585 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstableheadercell.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1244 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstablerowview.py
+-rw-r--r--   0 ronald     (501) staff       (20)    18911 2022-06-25 09:02:52.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstableview.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1162 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstableviewdiffabledatasource.py
+-rw-r--r--   0 ronald     (501) staff       (20)      370 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstableviewrowaction.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1715 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstabview.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1185 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstabviewcontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)      524 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstabviewitem.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1325 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstask.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5617 2022-06-25 09:07:15.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstext.py
+-rw-r--r--   0 ronald     (501) staff       (20)      295 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstextalternatives.py
+-rw-r--r--   0 ronald     (501) staff       (20)     7781 2022-06-25 09:01:38.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstextattachment.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6544 2022-06-25 09:02:18.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstextcheckingclient.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5233 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstextcheckingresult.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1500 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstextcontainer.py
+-rw-r--r--   0 ronald     (501) staff       (20)      598 2022-06-25 20:17:26.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstextcontent.py
+-rw-r--r--   0 ronald     (501) staff       (20)      710 2022-06-25 20:11:36.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstextcontextmanager.py
+-rw-r--r--   0 ronald     (501) staff       (20)      243 2022-06-15 11:57:00.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstextelement.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3134 2022-06-25 09:01:33.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstextfield.py
+-rw-r--r--   0 ronald     (501) staff       (20)      627 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstextfieldcell.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5570 2022-06-25 09:02:15.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstextfinder.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4415 2022-06-25 09:03:44.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstextinputclient.py
+-rw-r--r--   0 ronald     (501) staff       (20)      574 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstextinputcontext.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1150 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstextlayoutfragment.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3156 2022-06-25 20:06:42.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstextlayoutmanager.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1647 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstextlist.py
+-rw-r--r--   0 ronald     (501) staff       (20)      725 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstextrange.py
+-rw-r--r--   0 ronald     (501) staff       (20)      982 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstextselection.py
+-rw-r--r--   0 ronald     (501) staff       (20)     6299 2022-06-25 09:02:36.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstextselectionnavigation.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3457 2022-06-25 09:00:23.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstextstorage.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1810 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstexttable.py
+-rw-r--r--   0 ronald     (501) staff       (20)    20416 2023-03-03 17:21:59.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstextview.py
+-rw-r--r--   0 ronald     (501) staff       (20)      623 2022-06-25 20:13:15.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstextviewportlayoutcontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2740 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsthread.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3674 2023-03-03 17:21:59.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstimer.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1075 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstimezone.py
+-rw-r--r--   0 ronald     (501) staff       (20)      258 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstintconfiguration.py
+-rw-r--r--   0 ronald     (501) staff       (20)      357 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstitlebaraccessoryview.py
+-rw-r--r--   0 ronald     (501) staff       (20)      663 2021-07-30 09:00:37.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstitlebaraccessoryviewcontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1750 2022-06-25 09:02:49.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstokenfield.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2726 2022-06-25 09:04:03.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstokenfieldcell.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2891 2022-06-25 09:02:44.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstoolbar.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2740 2022-06-27 15:56:12.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstoolbaritem.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1416 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstoolbaritemgroup.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1749 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstouch.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1017 2022-06-25 20:09:45.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstouchbar.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1076 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstouchbaritem.py
+-rw-r--r--   0 ronald     (501) staff       (20)      923 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstrackingarea.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1342 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstreecontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)      306 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstreenode.py
+-rw-r--r--   0 ronald     (501) staff       (20)    13133 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstypesetter.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1181 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsubiquitouskeyvaluestore.py
+-rw-r--r--   0 ronald     (501) staff       (20)     4088 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsundomanager.py
+-rw-r--r--   0 ronald     (501) staff       (20)    18970 2023-02-19 10:50:34.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsurl.py
+-rw-r--r--   0 ronald     (501) staff       (20)      230 2022-06-25 20:16:07.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsurlauthenticationchallenge.py
+-rw-r--r--   0 ronald     (501) staff       (20)      666 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsurlcache.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3750 2022-06-25 09:01:03.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsurlconnection.py
+-rw-r--r--   0 ronald     (501) staff       (20)      637 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsurlcredential.py
+-rw-r--r--   0 ronald     (501) staff       (20)      876 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsurlcredentialstorage.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1979 2022-06-25 09:07:21.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsurldownload.py
+-rw-r--r--   0 ronald     (501) staff       (20)     5643 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsurlerror.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1803 2022-06-25 20:10:01.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsurlhandle.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1691 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsurlprotectionspace.py
+-rw-r--r--   0 ronald     (501) staff       (20)      961 2022-06-25 09:07:23.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsurlprotocol.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3731 2022-10-18 09:53:23.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsurlrequest.py
+-rw-r--r--   0 ronald     (501) staff       (20)      197 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsurlresponse.py
+-rw-r--r--   0 ronald     (501) staff       (20)    16829 2022-06-25 09:04:09.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsurlsession.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2101 2022-06-25 20:10:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsuseractivity.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2909 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsuserdefaults.py
+-rw-r--r--   0 ronald     (501) staff       (20)      391 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsuserdefaultscontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)      707 2022-06-25 20:07:12.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsuserinterfacecompression.py
+-rw-r--r--   0 ronald     (501) staff       (20)      376 2022-06-25 20:15:48.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsuserinterfaceitemidentification.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1454 2022-06-25 09:01:56.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsuserinterfaceitemsearching.py
+-rw-r--r--   0 ronald     (501) staff       (20)      617 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsuserinterfacelayout.py
+-rw-r--r--   0 ronald     (501) staff       (20)      826 2022-06-25 09:03:56.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsuserinterfacevalidation.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1850 2022-06-25 20:13:01.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsusernotification.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1164 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsuserscripttask.py
+-rw-r--r--   0 ronald     (501) staff       (20)      696 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsuuid.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1578 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsvalue.py
+-rw-r--r--   0 ronald     (501) staff       (20)      821 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsvaluetransformer.py
+-rw-r--r--   0 ronald     (501) staff       (20)    12513 2022-06-25 09:04:01.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsview.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1933 2022-06-25 09:00:36.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsviewcontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2281 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsvisualeffectview.py
+-rw-r--r--   0 ronald     (501) staff       (20)    23697 2023-03-24 18:54:07.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nswindow.py
+-rw-r--r--   0 ronald     (501) staff       (20)      606 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nswindowcontroller.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1347 2022-06-25 20:12:46.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nswindowrestoration.py
+-rw-r--r--   0 ronald     (501) staff       (20)      756 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nswindowscripting.py
+-rw-r--r--   0 ronald     (501) staff       (20)      915 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nswindowtabgroup.py
+-rw-r--r--   0 ronald     (501) staff       (20)    15068 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsworkspace.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1488 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsxmldocument.py
+-rw-r--r--   0 ronald     (501) staff       (20)      292 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsxmldtd.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1665 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsxmldtdnode.py
+-rw-r--r--   0 ronald     (501) staff       (20)      330 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsxmlelement.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1484 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsxmlnode.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3244 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsxmlnodeoptions.py
+-rw-r--r--   0 ronald     (501) staff       (20)     8643 2022-06-25 20:13:39.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsxmlparser.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2569 2022-06-25 20:17:50.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsxpcconnection.py
+-rw-r--r--   0 ronald     (501) staff       (20)     2786 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nszone.py
+-rw-r--r--   0 ronald     (501) staff       (20)      444 2023-03-03 17:21:59.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_osxcasts.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3666 2023-05-04 11:00:07.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_regr.py
+-rw-r--r--   0 ronald     (501) staff       (20)     8720 2022-10-21 10:39:38.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_structs.py
+-rw-r--r--   0 ronald     (501) staff       (20)      961 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_subclassing.py
+-rw-r--r--   0 ronald     (501) staff       (20)     3411 2021-03-21 10:08:22.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_threading.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1171 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/PyObjCTest/test_weirdness.py
+-rw-r--r--   0 ronald     (501) staff       (20)      346 2021-10-18 19:38:40.000000 pyobjc-framework-Cocoa-9.2/README.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:59.222121 pyobjc-framework-Cocoa-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)   635537 2022-12-17 13:53:38.000000 pyobjc-framework-Cocoa-9.2/metadata/AppKit.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   103090 2023-05-27 09:46:33.000000 pyobjc-framework-Cocoa-9.2/metadata/CoreFoundation.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   329318 2023-05-27 09:46:33.000000 pyobjc-framework-Cocoa-9.2/metadata/Foundation.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)      328 2021-08-03 12:27:37.000000 pyobjc-framework-Cocoa-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:59.435996 pyobjc-framework-Cocoa-9.2/metadata/raw.AppKit/
+-rw-r--r--   0 ronald     (501) staff       (20)  3375264 2022-12-17 13:53:35.000000 pyobjc-framework-Cocoa-9.2/metadata/raw.AppKit/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)  3414548 2022-12-17 13:53:35.000000 pyobjc-framework-Cocoa-9.2/metadata/raw.AppKit/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)  3448948 2022-12-17 13:53:36.000000 pyobjc-framework-Cocoa-9.2/metadata/raw.AppKit/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)  3449119 2022-12-17 13:53:36.000000 pyobjc-framework-Cocoa-9.2/metadata/raw.AppKit/arm64-13.1.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)  3451956 2023-03-24 18:54:07.000000 pyobjc-framework-Cocoa-9.2/metadata/raw.AppKit/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)  2614871 2022-12-17 13:53:36.000000 pyobjc-framework-Cocoa-9.2/metadata/raw.AppKit/x86_64-10.10.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)  3098132 2022-12-17 13:53:36.000000 pyobjc-framework-Cocoa-9.2/metadata/raw.AppKit/x86_64-10.14.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)  3210922 2022-12-17 13:53:36.000000 pyobjc-framework-Cocoa-9.2/metadata/raw.AppKit/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)  3270357 2022-12-17 13:53:37.000000 pyobjc-framework-Cocoa-9.2/metadata/raw.AppKit/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)  1861235 2022-12-17 13:53:37.000000 pyobjc-framework-Cocoa-9.2/metadata/raw.AppKit/x86_64-10.6.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)  1999920 2022-12-17 13:53:37.000000 pyobjc-framework-Cocoa-9.2/metadata/raw.AppKit/x86_64-10.7.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)  2037216 2022-12-17 13:53:37.000000 pyobjc-framework-Cocoa-9.2/metadata/raw.AppKit/x86_64-10.8.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)  3375265 2022-12-17 13:53:37.000000 pyobjc-framework-Cocoa-9.2/metadata/raw.AppKit/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)  3414549 2022-12-17 13:53:38.000000 pyobjc-framework-Cocoa-9.2/metadata/raw.AppKit/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)  3448949 2022-12-17 13:53:38.000000 pyobjc-framework-Cocoa-9.2/metadata/raw.AppKit/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)  3449120 2022-12-17 13:53:38.000000 pyobjc-framework-Cocoa-9.2/metadata/raw.AppKit/x86_64-13.1.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)  3451957 2023-03-24 18:54:07.000000 pyobjc-framework-Cocoa-9.2/metadata/raw.AppKit/x86_64-13.3.fwinfo
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:59.512286 pyobjc-framework-Cocoa-9.2/metadata/raw.CoreFoundation/
+-rw-r--r--   0 ronald     (501) staff       (20)   312826 2021-08-03 12:27:37.000000 pyobjc-framework-Cocoa-9.2/metadata/raw.CoreFoundation/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   315024 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/metadata/raw.CoreFoundation/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   330943 2022-10-29 12:03:04.000000 pyobjc-framework-Cocoa-9.2/metadata/raw.CoreFoundation/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   331260 2023-02-19 10:50:34.000000 pyobjc-framework-Cocoa-9.2/metadata/raw.CoreFoundation/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   305789 2021-08-03 12:27:37.000000 pyobjc-framework-Cocoa-9.2/metadata/raw.CoreFoundation/x86_64-10.10.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   311591 2021-08-03 12:27:37.000000 pyobjc-framework-Cocoa-9.2/metadata/raw.CoreFoundation/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   312634 2021-08-03 12:27:37.000000 pyobjc-framework-Cocoa-9.2/metadata/raw.CoreFoundation/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   292849 2021-08-03 12:27:37.000000 pyobjc-framework-Cocoa-9.2/metadata/raw.CoreFoundation/x86_64-10.6.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   304008 2021-08-03 12:27:37.000000 pyobjc-framework-Cocoa-9.2/metadata/raw.CoreFoundation/x86_64-10.7.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   305298 2021-08-03 12:27:37.000000 pyobjc-framework-Cocoa-9.2/metadata/raw.CoreFoundation/x86_64-10.8.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   312873 2021-08-03 12:27:37.000000 pyobjc-framework-Cocoa-9.2/metadata/raw.CoreFoundation/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   315071 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/metadata/raw.CoreFoundation/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   331013 2022-10-29 12:03:04.000000 pyobjc-framework-Cocoa-9.2/metadata/raw.CoreFoundation/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)   331330 2023-02-19 10:50:34.000000 pyobjc-framework-Cocoa-9.2/metadata/raw.CoreFoundation/x86_64-13.3.fwinfo
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:07:59.606837 pyobjc-framework-Cocoa-9.2/metadata/raw.Foundation/
+-rw-r--r--   0 ronald     (501) staff       (20)  1975821 2021-08-04 10:01:02.000000 pyobjc-framework-Cocoa-9.2/metadata/raw.Foundation/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)  1983710 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/metadata/raw.Foundation/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)  2013356 2022-10-18 09:53:23.000000 pyobjc-framework-Cocoa-9.2/metadata/raw.Foundation/arm64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)  2013588 2023-02-19 10:50:34.000000 pyobjc-framework-Cocoa-9.2/metadata/raw.Foundation/arm64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)  1595900 2021-08-03 12:27:37.000000 pyobjc-framework-Cocoa-9.2/metadata/raw.Foundation/x86_64-10.10.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)  1885998 2021-08-03 12:27:37.000000 pyobjc-framework-Cocoa-9.2/metadata/raw.Foundation/x86_64-10.15.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)  1937893 2021-08-03 12:27:37.000000 pyobjc-framework-Cocoa-9.2/metadata/raw.Foundation/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)  1219040 2021-08-03 12:27:37.000000 pyobjc-framework-Cocoa-9.2/metadata/raw.Foundation/x86_64-10.8.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)  1975537 2021-08-04 10:01:02.000000 pyobjc-framework-Cocoa-9.2/metadata/raw.Foundation/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)  1983921 2022-02-24 08:47:16.000000 pyobjc-framework-Cocoa-9.2/metadata/raw.Foundation/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)  2013613 2022-10-18 09:53:23.000000 pyobjc-framework-Cocoa-9.2/metadata/raw.Foundation/x86_64-13.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)  2013845 2023-02-19 10:50:34.000000 pyobjc-framework-Cocoa-9.2/metadata/raw.Foundation/x86_64-13.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-Cocoa-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-Cocoa-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:07:59.616819 pyobjc-framework-Cocoa-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)     2601 2023-05-29 10:07:45.000000 pyobjc-framework-Cocoa-9.2/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       57 2020-11-30 18:45:14.000000 pyobjc-framework-Cocoa-9.2/todo.txt
```

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/ClassBrowser/ClassBrowser.nib/classes.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/ClassBrowser/ClassBrowser.nib/classes.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/ClassBrowser/ClassBrowser.nib/objects.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/ClassBrowser/ClassBrowser.nib/objects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/ClassBrowser/ClassBrowser.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/ClassBrowser/ClassBrowser.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/Bookmarks/BookmarksDocument.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/Bookmarks/BookmarksDocument.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/Bookmarks/DNDArrayController.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/Bookmarks/DNDArrayController.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/Bookmarks/DNDTableView.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/Bookmarks/DNDTableView.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/Bookmarks/English.lproj/BookmarksDocument.nib/keyedobjects.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/Bookmarks/English.lproj/BookmarksDocument.nib/keyedobjects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/Bookmarks/English.lproj/MainMenu.nib/info.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/Bookmarks/English.lproj/MainMenu.nib/info.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/Bookmarks/English.lproj/MainMenu.nib/keyedobjects.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/Bookmarks/English.lproj/MainMenu.nib/keyedobjects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/Bookmarks/setup.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/Bookmarks/setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ControlledPreferences/English.lproj/MainMenu.nib/classes.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ControlledPreferences/English.lproj/MainMenu.nib/classes.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ControlledPreferences/English.lproj/MainMenu.nib/info.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ControlledPreferences/English.lproj/MainMenu.nib/info.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ControlledPreferences/English.lproj/MainMenu.nib/keyedobjects.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ControlledPreferences/English.lproj/MainMenu.nib/keyedobjects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ControlledPreferences/FontNameToDisplayNameTransformer.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ControlledPreferences/FontNameToDisplayNameTransformer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ControlledPreferences/FontSampleDisplayView.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ControlledPreferences/FontSampleDisplayView.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ControlledPreferences/PreferencesPanelController.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ControlledPreferences/PreferencesPanelController.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/CurrencyConvBinding/Converter.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/CurrencyConvBinding/Converter.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/CurrencyConvBinding/English.lproj/CurrencyConvBindingDocument.nib/keyedobjects.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/CurrencyConvBinding/English.lproj/CurrencyConvBindingDocument.nib/keyedobjects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/CurrencyConvBinding/English.lproj/MainMenu.nib/info.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/CurrencyConvBinding/English.lproj/MainMenu.nib/info.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/CurrencyConvBinding/English.lproj/MainMenu.nib/keyedobjects.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/CurrencyConvBinding/English.lproj/MainMenu.nib/keyedobjects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/CurrencyConvBinding/setup.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/CurrencyConvBinding/setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/FilteringController/English.lproj/FilteringControllerDocument.nib/classes.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/FilteringController/English.lproj/FilteringControllerDocument.nib/classes.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/FilteringController/English.lproj/FilteringControllerDocument.nib/info.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/FilteringController/English.lproj/FilteringControllerDocument.nib/info.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/FilteringController/English.lproj/FilteringControllerDocument.nib/keyedobjects.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/FilteringController/English.lproj/FilteringControllerDocument.nib/keyedobjects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/FilteringController/English.lproj/MainMenu.nib/info.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/FilteringController/English.lproj/MainMenu.nib/info.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/FilteringController/English.lproj/MainMenu.nib/keyedobjects.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/FilteringController/English.lproj/MainMenu.nib/keyedobjects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/FilteringController/FilteringArrayController.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/FilteringController/FilteringArrayController.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/FilteringController/FilteringControllerDocument.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/FilteringController/FilteringControllerDocument.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/FilteringController/setup.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/FilteringController/setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/GraphicsBindings/Circle.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/GraphicsBindings/Circle.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/GraphicsBindings/English.lproj/GraphicsBindingsDocument.nib/classes.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/GraphicsBindings/English.lproj/GraphicsBindingsDocument.nib/classes.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/GraphicsBindings/English.lproj/GraphicsBindingsDocument.nib/info.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/GraphicsBindings/English.lproj/GraphicsBindingsDocument.nib/info.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/GraphicsBindings/English.lproj/GraphicsBindingsDocument.nib/keyedobjects.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/GraphicsBindings/English.lproj/GraphicsBindingsDocument.nib/keyedobjects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/GraphicsBindings/English.lproj/MainMenu.nib/info.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/GraphicsBindings/English.lproj/MainMenu.nib/info.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/GraphicsBindings/English.lproj/MainMenu.nib/keyedobjects.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/GraphicsBindings/English.lproj/MainMenu.nib/keyedobjects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/GraphicsBindings/GraphicsArrayController.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/GraphicsBindings/GraphicsArrayController.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/GraphicsBindings/GraphicsBindingsDocument.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/GraphicsBindings/GraphicsBindingsDocument.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/GraphicsBindings/GraphicsView.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/GraphicsBindings/GraphicsView.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/GraphicsBindings/JoystickView.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/GraphicsBindings/JoystickView.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/GraphicsBindings/RadiansToDegreesTransformer.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/GraphicsBindings/RadiansToDegreesTransformer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/GraphicsBindings/setup.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/GraphicsBindings/setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ManualBindings/AppController.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ManualBindings/AppController.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ManualBindings/English.lproj/MainMenu.nib/classes.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ManualBindings/English.lproj/MainMenu.nib/classes.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ManualBindings/English.lproj/MainMenu.nib/info.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ManualBindings/English.lproj/MainMenu.nib/info.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ManualBindings/English.lproj/MainMenu.nib/keyedobjects.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ManualBindings/English.lproj/MainMenu.nib/keyedobjects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/MutableTableModel/English.lproj/MainMenu.nib/info.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/MutableTableModel/English.lproj/MainMenu.nib/info.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/MutableTableModel/English.lproj/MainMenu.nib/keyedobjects.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/MutableTableModel/English.lproj/MainMenu.nib/keyedobjects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/MutableTableModel/TableModelAppDelegate.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/MutableTableModel/TableModelAppDelegate.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/TableModel/English.lproj/MainMenu.nib/info.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/TableModel/English.lproj/MainMenu.nib/info.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/TableModel/English.lproj/MainMenu.nib/keyedobjects.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/TableModel/English.lproj/MainMenu.nib/keyedobjects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/TableModel/TableModelAppDelegate.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/TableModel/TableModelAppDelegate.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/TableModelWithSearch/English.lproj/InfoPlist.strings` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/TableModelWithSearch/English.lproj/InfoPlist.strings`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/TableModelWithSearch/English.lproj/MainMenu.nib/classes.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/TableModelWithSearch/English.lproj/MainMenu.nib/classes.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/TableModelWithSearch/English.lproj/MainMenu.nib/info.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/TableModelWithSearch/English.lproj/MainMenu.nib/info.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/TableModelWithSearch/English.lproj/MainMenu.nib/keyedobjects.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/TableModelWithSearch/English.lproj/MainMenu.nib/keyedobjects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/TableModelWithSearch/FilteringArrayController.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/TableModelWithSearch/FilteringArrayController.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/TableModelWithSearch/TableModelWithSearchAppDelegate.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/TableModelWithSearch/TableModelWithSearchAppDelegate.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/TableModelWithSearch/ToolbarCreator.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/TableModelWithSearch/ToolbarCreator.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/TemperatureTransformer/English.lproj/MainMenu.nib/info.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/TemperatureTransformer/English.lproj/MainMenu.nib/info.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/TemperatureTransformer/English.lproj/MainMenu.nib/keyedobjects.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/TemperatureTransformer/English.lproj/MainMenu.nib/keyedobjects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/TemperatureTransformer/TransformerAppDelegate.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/TemperatureTransformer/TransformerAppDelegate.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ToDos/Category.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ToDos/Category.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ToDos/English.lproj/MainMenu.nib/info.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ToDos/English.lproj/MainMenu.nib/info.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ToDos/English.lproj/MainMenu.nib/keyedobjects.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ToDos/English.lproj/MainMenu.nib/keyedobjects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ToDos/English.lproj/ToDosDocument.nib/info.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ToDos/English.lproj/ToDosDocument.nib/info.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ToDos/English.lproj/ToDosDocument.nib/keyedobjects.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ToDos/English.lproj/ToDosDocument.nib/keyedobjects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ToDos/OverdueTransformer.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ToDos/OverdueTransformer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ToDos/PriorityToColourTransformer.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ToDos/PriorityToColourTransformer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ToDos/ToDosDocument.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ToDos/ToDosDocument.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CocoaBindings/ToDos/setup.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CocoaBindings/ToDos/setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CurrencyConverter/00README.txt` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CurrencyConverter/00README.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CurrencyConverter/CurrencyConverter.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CurrencyConverter/CurrencyConverter.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CurrencyConverter/English.lproj/MainMenu.nib/info.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CurrencyConverter/English.lproj/MainMenu.nib/info.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/CurrencyConverter/English.lproj/MainMenu.nib/objects.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/CurrencyConverter/English.lproj/MainMenu.nib/objects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/DatePicker/English.lproj/MainMenu.nib/classes.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/DatePicker/English.lproj/MainMenu.nib/classes.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/DatePicker/English.lproj/MainMenu.nib/info.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/DatePicker/English.lproj/MainMenu.nib/info.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/DatePicker/English.lproj/MainMenu.nib/keyedobjects.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/DatePicker/English.lproj/MainMenu.nib/keyedobjects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/DatePicker/MyWindowController.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/DatePicker/MyWindowController.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/DatePicker/ReadMe.txt` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/DatePicker/ReadMe.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/DotView/DotView.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/DotView/DotView.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/DotView/English.lproj/MainMenu.xib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/DotView/English.lproj/MainMenu.xib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/DragItemAround/DragItemAround.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/DragItemAround/DragItemAround.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/DragItemAround/MainMenu.nib/classes.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/DragItemAround/MainMenu.nib/classes.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/DragItemAround/MainMenu.nib/info.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/DragItemAround/MainMenu.nib/info.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/DragItemAround/MainMenu.nib/keyedobjects.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/DragItemAround/MainMenu.nib/keyedobjects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/FieldGraph/CGraphController.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/FieldGraph/CGraphController.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/FieldGraph/CGraphModel.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/FieldGraph/CGraphModel.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/FieldGraph/CGraphView.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/FieldGraph/CGraphView.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/FieldGraph/English.lproj/InfoPlist.strings` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/FieldGraph/English.lproj/InfoPlist.strings`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/FieldGraph/English.lproj/MainMenu.nib/classes.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/FieldGraph/English.lproj/MainMenu.nib/classes.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/FieldGraph/English.lproj/MainMenu.nib/info.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/FieldGraph/English.lproj/MainMenu.nib/info.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/FieldGraph/English.lproj/MainMenu.nib/keyedobjects.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/FieldGraph/English.lproj/MainMenu.nib/keyedobjects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/FieldGraph/English.lproj/MainMenu.nib/objects.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/FieldGraph/English.lproj/MainMenu.nib/objects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/FieldGraph/Map.png` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/FieldGraph/Map.png`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/FieldGraph/fieldMath.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/FieldGraph/fieldMath.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Formatter/MainMenu.nib/info.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/Formatter/MainMenu.nib/info.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Formatter/MainMenu.nib/keyedobjects.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/Formatter/MainMenu.nib/keyedobjects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Formatter/main.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/Formatter/main.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Grady/AppDelegate.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/Grady/AppDelegate.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Grady/English.lproj/MainMenu.nib/info.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/Grady/English.lproj/MainMenu.nib/info.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Grady/English.lproj/MainMenu.nib/keyedobjects.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/Grady/English.lproj/MainMenu.nib/keyedobjects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Grady/English.lproj/TestWindow.nib/classes.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/Grady/English.lproj/TestWindow.nib/classes.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Grady/English.lproj/TestWindow.nib/keyedobjects.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/Grady/English.lproj/TestWindow.nib/keyedobjects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Grady/MyBaseGradientView.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/Grady/MyBaseGradientView.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Grady/MyBezierGradientView.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/Grady/MyBezierGradientView.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Grady/MyRectGradientView.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/Grady/MyRectGradientView.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Grady/MyWindowController.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/Grady/MyWindowController.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/PredicateEditorSample/CaseInsensitivePredicateTemplate.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/PredicateEditorSample/CaseInsensitivePredicateTemplate.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/PredicateEditorSample/English.lproj/MainMenu.nib/classes.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/PredicateEditorSample/English.lproj/MainMenu.nib/classes.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/PredicateEditorSample/English.lproj/MainMenu.nib/info.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/PredicateEditorSample/English.lproj/MainMenu.nib/info.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/PredicateEditorSample/English.lproj/MainMenu.nib/keyedobjects.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/PredicateEditorSample/English.lproj/MainMenu.nib/keyedobjects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/PredicateEditorSample/MyWindowController.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/PredicateEditorSample/MyWindowController.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/PredicateEditorSample/ReadMe.txt` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/PredicateEditorSample/ReadMe.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/PyInterpreter/LICENSE.txt` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/PyInterpreter/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/PyInterpreter/PyInterpreter.nib/classes.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/PyInterpreter/PyInterpreter.nib/classes.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/PyInterpreter/PyInterpreter.nib/info.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/PyInterpreter/PyInterpreter.nib/info.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/PyInterpreter/PyInterpreter.nib/keyedobjects.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/PyInterpreter/PyInterpreter.nib/keyedobjects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/PyInterpreter/PyInterpreter.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/PyInterpreter/PyInterpreter.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/PythonBrowser/MainMenu.nib/info.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/PythonBrowser/MainMenu.nib/info.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/PythonBrowser/MainMenu.nib/objects.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/PythonBrowser/MainMenu.nib/objects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/PythonBrowser/PythonBrowser.nib/objects.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/PythonBrowser/PythonBrowser.nib/objects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/PythonBrowser/PythonBrowser.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/PythonBrowser/PythonBrowser.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/PythonBrowser/PythonBrowserModel.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/PythonBrowser/PythonBrowserModel.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/PythonBrowser/readme.txt` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/PythonBrowser/readme.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/RoundTransparentWindow/MainMenu.nib/classes.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/RoundTransparentWindow/MainMenu.nib/classes.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/RoundTransparentWindow/MainMenu.nib/objects.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/RoundTransparentWindow/MainMenu.nib/objects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/RoundTransparentWindow/RoundTransparentWindow.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/RoundTransparentWindow/RoundTransparentWindow.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/RoundTransparentWindow/circle.tif` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/RoundTransparentWindow/circle.tif`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/RoundTransparentWindow/pentagram.tif` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/RoundTransparentWindow/pentagram.tif`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/SimpleService/README.rtf` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/SimpleService/README.rtf`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/SimpleService/ServiceTest.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/SimpleService/ServiceTest.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/SimpleService/setup.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/SimpleService/setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/TableModel/English.lproj/MainMenu.nib/info.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/TableModel/English.lproj/MainMenu.nib/info.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/TableModel/English.lproj/MainMenu.nib/objects.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/TableModel/English.lproj/MainMenu.nib/objects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/TableModel/TableModel.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/TableModel/TableModel.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/TinyTinyEdit/MainMenu.nib/objects.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/TinyTinyEdit/MainMenu.nib/objects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/TinyTinyEdit/TinyTinyDocument.nib/objects.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/TinyTinyEdit/TinyTinyDocument.nib/objects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/TinyTinyEdit/TinyTinyEdit.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/TinyTinyEdit/TinyTinyEdit.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/TinyTinyEdit/setup.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/TinyTinyEdit/setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/TinyURLService/README.rtf` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/TinyURLService/README.rtf`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/TinyURLService/TinyURLService.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/TinyURLService/TinyURLService.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/TinyURLService/setup.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/TinyURLService/setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Todo/00ReadMe.txt` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/Todo/00ReadMe.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Todo/CalendarMatrix.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/Todo/CalendarMatrix.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Todo/English.lproj/MainMenu.nib/objects.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/Todo/English.lproj/MainMenu.nib/objects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Todo/English.lproj/ToDoDocument.nib/classes.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/Todo/English.lproj/ToDoDocument.nib/classes.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Todo/English.lproj/ToDoDocument.nib/objects.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/Todo/English.lproj/ToDoDocument.nib/objects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Todo/English.lproj/ToDoInfoWindow.nib/classes.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/Todo/English.lproj/ToDoInfoWindow.nib/classes.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Todo/English.lproj/ToDoInfoWindow.nib/info.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/Todo/English.lproj/ToDoInfoWindow.nib/info.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Todo/English.lproj/ToDoInfoWindow.nib/objects.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/Todo/English.lproj/ToDoInfoWindow.nib/objects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Todo/Icons/ToDoApp.icns` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/Todo/Icons/ToDoApp.icns`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Todo/Icons/ToDoDoc.icns` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/Todo/Icons/ToDoDoc.icns`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Todo/InfoWindowController.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/Todo/InfoWindowController.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Todo/SelectionNotifyMatrix.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/Todo/SelectionNotifyMatrix.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Todo/ToDoCell.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/Todo/ToDoCell.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Todo/ToDoDocument.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/Todo/ToDoDocument.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Todo/ToDoItem.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/Todo/ToDoItem.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/Todo/setup.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/Todo/setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/WebServicesTool/English.lproj/MainMenu.nib/keyedobjects.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/WebServicesTool/English.lproj/MainMenu.nib/keyedobjects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/WebServicesTool/English.lproj/WSTConnection.nib/classes.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/WebServicesTool/English.lproj/WSTConnection.nib/classes.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/WebServicesTool/English.lproj/WSTConnection.nib/info.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/WebServicesTool/English.lproj/WSTConnection.nib/info.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/WebServicesTool/English.lproj/WSTConnection.nib/keyedobjects.nib` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/WebServicesTool/English.lproj/WSTConnection.nib/keyedobjects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/WebServicesTool/LICENSE.txt` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/WebServicesTool/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/WebServicesTool/Preferences.png` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/WebServicesTool/Preferences.png`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/WebServicesTool/README.txt` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/WebServicesTool/README.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/WebServicesTool/Reload.png` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/WebServicesTool/Reload.png`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/WebServicesTool/WST.icns` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/WebServicesTool/WST.icns`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/WebServicesTool/WST.png` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/WebServicesTool/WST.png`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/WebServicesTool/WSTApplicationDelegateClass.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/WebServicesTool/WSTApplicationDelegateClass.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/AppKit/WebServicesTool/WSTConnectionWindowControllerClass.py` & `pyobjc-framework-Cocoa-9.2/Examples/AppKit/WebServicesTool/WSTConnectionWindowControllerClass.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/Foundation/Scripts/dictionary.py` & `pyobjc-framework-Cocoa-9.2/Examples/Foundation/Scripts/dictionary.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/Foundation/Scripts/findPython.py` & `pyobjc-framework-Cocoa-9.2/Examples/Foundation/Scripts/findPython.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/Foundation/Scripts/rendezvous.py` & `pyobjc-framework-Cocoa-9.2/Examples/Foundation/Scripts/rendezvous.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/Foundation/Scripts/simple-kvo.py` & `pyobjc-framework-Cocoa-9.2/Examples/Foundation/Scripts/simple-kvo.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/OpenGL/OpenGLDemo/LICENSE.txt` & `pyobjc-framework-Cocoa-9.2/Examples/OpenGL/OpenGLDemo/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/OpenGL/OpenGLDemo/OpenGLDemo.nib/info.nib` & `pyobjc-framework-Cocoa-9.2/Examples/OpenGL/OpenGLDemo/OpenGLDemo.nib/info.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/OpenGL/OpenGLDemo/OpenGLDemo.nib/objects.nib` & `pyobjc-framework-Cocoa-9.2/Examples/OpenGL/OpenGLDemo/OpenGLDemo.nib/objects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/OpenGL/OpenGLDemo/OpenGLDemo.py` & `pyobjc-framework-Cocoa-9.2/Examples/OpenGL/OpenGLDemo/OpenGLDemo.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool/English.lproj/MainMenu.nib/keyedobjects.nib` & `pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool/English.lproj/MainMenu.nib/keyedobjects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool/English.lproj/WSTConnection.nib/classes.nib` & `pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool/English.lproj/WSTConnection.nib/classes.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool/English.lproj/WSTConnection.nib/info.nib` & `pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool/English.lproj/WSTConnection.nib/info.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool/English.lproj/WSTConnection.nib/keyedobjects.nib` & `pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool/English.lproj/WSTConnection.nib/keyedobjects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool/LICENSE.txt` & `pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool/Preferences.png` & `pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool/Preferences.png`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool/ReadMe.txt` & `pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool/ReadMe.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool/Reload.png` & `pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool/Reload.png`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool/WST.icns` & `pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool/WST.icns`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool/WST.png` & `pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool/WST.png`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool/WSTApplicationDelegateClass.py` & `pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool/WSTApplicationDelegateClass.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool/WSTConnectionWindowControllerClass.py` & `pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool/WSTConnectionWindowControllerClass.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool-CocoaBindings/English.lproj/MainMenu.nib/keyedobjects.nib` & `pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool-CocoaBindings/English.lproj/MainMenu.nib/keyedobjects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool-CocoaBindings/English.lproj/WSTConnection.nib/classes.nib` & `pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool-CocoaBindings/English.lproj/WSTConnection.nib/classes.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool-CocoaBindings/English.lproj/WSTConnection.nib/info.nib` & `pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool-CocoaBindings/English.lproj/WSTConnection.nib/info.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool-CocoaBindings/English.lproj/WSTConnection.nib/keyedobjects.nib` & `pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool-CocoaBindings/English.lproj/WSTConnection.nib/keyedobjects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool-CocoaBindings/LICENSE.txt` & `pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool-CocoaBindings/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool-CocoaBindings/Preferences.png` & `pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool-CocoaBindings/Preferences.png`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool-CocoaBindings/README.txt` & `pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool-CocoaBindings/README.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool-CocoaBindings/RPCMethod.py` & `pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool-CocoaBindings/RPCMethod.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool-CocoaBindings/Reload.png` & `pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool-CocoaBindings/Reload.png`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool-CocoaBindings/WST.icns` & `pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool-CocoaBindings/WST.icns`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool-CocoaBindings/WST.png` & `pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool-CocoaBindings/WST.png`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool-CocoaBindings/WSTApplicationDelegateClass.py` & `pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool-CocoaBindings/WSTApplicationDelegateClass.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Examples/Twisted/WebServicesTool-CocoaBindings/WSTConnectionWindowControllerClass.py` & `pyobjc-framework-Cocoa-9.2/Examples/Twisted/WebServicesTool-CocoaBindings/WSTConnectionWindowControllerClass.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/LICENSE.txt` & `pyobjc-framework-Cocoa-9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Lib/AppKit/__init__.py` & `pyobjc-framework-Cocoa-9.2/Lib/AppKit/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,14 +54,16 @@
     _inline_list_,
     {
         "__doc__": __doc__,
         "objc": objc,
         "NSDictionaryOfVariableBindings": NSDictionaryOfVariableBindings,
         "__path__": __path__,
         "__loader__": globals().get("__loader__", None),
+        "__file__": globals().get("__file__", None),
+        "__spec__": globals().get("__spec__", None),
     },
     (Foundation,),
 )
 
 # NSApp is a global variable that can be changed in ObjC,
 # somewhat emulate that (it is *not* possible to assign to
 # NSApp in Python)
```

### Comparing `pyobjc-framework-Cocoa-9.1b1/Lib/AppKit/_metadata.py` & `pyobjc-framework-Cocoa-9.2/Lib/AppKit/_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is generated by objective.metadata
 #
-# Last update: Fri Mar 24 18:14:20 2023
+# Last update: Sat May 20 11:07:54 2023
 #
 # flake8: noqa
 
 import objc, sys
 from typing import NewType
 
 if sys.maxsize > 2**32:
```

### Comparing `pyobjc-framework-Cocoa-9.1b1/Lib/AppKit/_nsapp.py` & `pyobjc-framework-Cocoa-9.2/Lib/AppKit/_nsapp.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Lib/CGL/PyObjC.bridgesupport` & `pyobjc-framework-Cocoa-9.2/Lib/CGL/PyObjC.bridgesupport`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Lib/CoreFoundation/_metadata.py` & `pyobjc-framework-Cocoa-9.2/Lib/CoreFoundation/_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is generated by objective.metadata
 #
-# Last update: Sun Mar  5 11:06:45 2023
+# Last update: Sat May 20 11:07:43 2023
 #
 # flake8: noqa
 
 import objc, sys
 from typing import NewType
 
 if sys.maxsize > 2**32:
@@ -574,19 +574,14 @@
     "CFErrorCopyFailureReason": (
         b"^{__CFString=}^{__CFError=}",
         "",
         {"retval": {"already_cfretained": True}},
     ),
     "CFBinaryHeapContainsValue": (b"Z^{__CFBinaryHeap=}@",),
     "CFNumberFormatterGetStyle": (b"q^{__CFNumberFormatter=}",),
-    "CFXMLParserCreate": (
-        b"^{__CFXMLParser=}^{__CFAllocator=}^{__CFData=}^{__CFURL=}Qq^{_CFXMLParserCallBacks=q^?^?^?^?^?}^{_CFXMLParserContext=q^v^?^?^?}",
-        "",
-        {"retval": {"already_cfretained": True}},
-    ),
     "CFLocaleCopyPreferredLanguages": (
         b"^{__CFArray=}",
         "",
         {"retval": {"already_cfretained": True}},
     ),
     "CFBagCreateCopy": (
         b"^{__CFBag=}^{__CFAllocator=}^{__CFBag=}",
@@ -868,19 +863,14 @@
         b"^{__CFString=}^{__CFAllocator=}^{__CFNumberFormatter=}^{__CFNumber=}",
         "",
         {"retval": {"already_cfretained": True}},
     ),
     "CFCalendarGetMaximumRangeOfUnit": (b"{_CFRange=qq}^{__CFCalendar=}Q",),
     "CFRunLoopRemoveSource": (b"v^{__CFRunLoop=}^{__CFRunLoopSource=}^{__CFString=}",),
     "CFSwapInt32": (b"II",),
-    "CFXMLParserCreateWithDataFromURL": (
-        b"^{__CFXMLParser=}^{__CFAllocator=}^{__CFURL=}Qq^{_CFXMLParserCallBacks=q^?^?^?^?^?}^{_CFXMLParserContext=q^v^?^?^?}",
-        "",
-        {"retval": {"already_cfretained": True}},
-    ),
     "CFRunLoopTimerGetNextFireDate": (b"d^{__CFRunLoopTimer=}",),
     "CFBitVectorGetCountOfBit": (b"q^{__CFBitVector=}{_CFRange=qq}I",),
     "CFNotificationCenterGetDarwinNotifyCenter": (b"^{__CFNotificationCenter=}",),
     "CFPropertyListWrite": (
         b"q@^{__CFWriteStream=}qQ^^{__CFError=}",
         "",
         {
@@ -2855,17 +2845,14 @@
     ),
     "CFCharacterSetCreateWithBitmapRepresentation": (
         b"^{__CFCharacterSet=}^{__CFAllocator=}^{__CFData=}",
         "",
         {"retval": {"already_cfretained": True}},
     ),
     "CFBundleGetValueForInfoDictionaryKey": (b"@^{__CFBundle=}^{__CFString=}",),
-    "CFXMLParserGetCallBacks": (
-        b"v^{__CFXMLParser=}^{_CFXMLParserCallBacks=q^?^?^?^?^?}",
-    ),
     "CFWriteStreamUnscheduleFromRunLoop": (
         b"v^{__CFWriteStream=}^{__CFRunLoop=}^{__CFString=}",
     ),
     "CFAttributedStringCreateCopy": (
         b"^{__CFAttributedString=}^{__CFAllocator=}^{__CFAttributedString=}",
         "",
         {"retval": {"already_cfretained": True}},
@@ -3148,15 +3135,14 @@
         {"retval": {"already_cfretained": True}},
     ),
     "CFAttributedStringGetAttributesAndLongestEffectiveRange": (
         b"^{__CFDictionary=}^{__CFAttributedString=}q{_CFRange=qq}^{_CFRange=qq}",
         "",
         {"arguments": {3: {"type_modifier": "o"}}},
     ),
-    "CFXMLParserGetContext": (b"v^{__CFXMLParser=}^{_CFXMLParserContext=q^v^?^?^?}",),
     "CFCopyDescription": (
         b"^{__CFString=}@",
         "",
         {"retval": {"already_cfretained": True}},
     ),
     "CFDataDeleteBytes": (b"v^{__CFData=}{_CFRange=qq}",),
     "CFWriteStreamGetError": (b"{_CFStreamError=qi}^{__CFWriteStream=}",),
```

### Comparing `pyobjc-framework-Cocoa-9.1b1/Lib/CoreFoundation/_static.py` & `pyobjc-framework-Cocoa-9.2/Lib/CoreFoundation/_static.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Lib/Foundation/__init__.py` & `pyobjc-framework-Cocoa-9.2/Lib/Foundation/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -174,14 +174,16 @@
     {
         "__doc__": __doc__,
         "objc": objc,
         "YES": objc.YES,
         "NO": objc.NO,
         "__path__": __path__,
         "__loader__": globals().get("__loader__", None),
+        "__file__": globals().get("__file__", None),
+        "__spec__": globals().get("__spec__", None),
     },
     (CoreFoundation,),
 )
 
 
 del sys.modules["Foundation._metadata"]
 
@@ -196,17 +198,21 @@
 
 import Foundation._context  # isort:skip  # noqa: E402
 import Foundation._functiondefines  # isort:skip  # noqa: E402
 import Foundation._nsindexset  # isort:skip  # noqa: E402
 import Foundation._nsobject  # isort:skip  # noqa: E402
 
 for nm in dir(Foundation._functiondefines):
+    if nm.startswith("_"):
+        continue
     setattr(mod, nm, getattr(Foundation._functiondefines, nm))
 
 
 mod.NSIntegerMax = sys.maxsize
 mod.NSIntegerMin = -sys.maxsize - 1
 mod.NSUIntegerMax = (sys.maxsize * 2) + 1
 
 
 for nm in dir(Foundation._context):
+    if nm.startswith("_"):
+        continue
     setattr(mod, nm, getattr(Foundation._context, nm))
```

### Comparing `pyobjc-framework-Cocoa-9.1b1/Lib/Foundation/_context.py` & `pyobjc-framework-Cocoa-9.2/Lib/Foundation/_context.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Lib/Foundation/_functiondefines.py` & `pyobjc-framework-Cocoa-9.2/Lib/Foundation/_functiondefines.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Lib/Foundation/_metadata.py` & `pyobjc-framework-Cocoa-9.2/Lib/Foundation/_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is generated by objective.metadata
 #
-# Last update: Sun Mar  5 11:18:45 2023
+# Last update: Sat May 20 11:07:47 2023
 #
 # flake8: noqa
 
 import objc, sys
 from typing import NewType
 
 if sys.maxsize > 2**32:
@@ -443,15 +443,19 @@
             "arguments": {
                 0: {"type_modifier": "o"},
                 1: {"type_modifier": "n"},
                 2: {"type_modifier": "n"},
             }
         },
     ),
-    "NSEndMapTableEnumeration": (b"v^{_NSMapEnumerator=QQ^v}",),
+    "NSEndMapTableEnumeration": (
+        b"v^{_NSMapEnumerator=QQ^v}",
+        "",
+        {"arguments": {0: {"type_modifier": "N"}}},
+    ),
     "NSEqualRects": (
         b"Z{CGRect={CGPoint=dd}{CGSize=dd}}{CGRect={CGPoint=dd}{CGSize=dd}}",
     ),
     "NSIntegralRect": (
         b"{CGRect={CGPoint=dd}{CGSize=dd}}{CGRect={CGPoint=dd}{CGSize=dd}}",
     ),
     "NSEqualSizes": (b"Z{CGSize=dd}{CGSize=dd}",),
@@ -557,20 +561,34 @@
         {"retval": {"already_cfretained": True}},
     ),
     "NSSwapBigShortToHost": (b"SS",),
     "NSSwapHostShortToBig": (b"SS",),
     "NSStringFromPoint": (b"@{CGPoint=dd}",),
     "NSWidth": (b"d{CGRect={CGPoint=dd}{CGSize=dd}}",),
     "NSRealMemoryAvailable": (b"Q",),
-    "NSNextMapEnumeratorPair": (b"Z^{_NSMapEnumerator=QQ^v}^^v^^v",),
+    "NSNextMapEnumeratorPair": (
+        b"Z^{_NSMapEnumerator=QQ^v}^^v^^v",
+        "",
+        {
+            "arguments": {
+                0: {"type_modifier": "N"},
+                1: {"type_modifier": "o"},
+                2: {"type_modifier": "o"},
+            }
+        },
+    ),
     "NSAllHashTableObjects": (b"@@",),
     "NSPointFromCGPoint": (b"{CGPoint=dd}{CGPoint=dd}",),
     "NSSizeToCGSize": (b"{CGSize=dd}{CGSize=dd}",),
     "NSHashInsertKnownAbsent": (b"v@^v",),
-    "NSNextHashEnumeratorItem": (b"^v^{_NSHashEnumerator=QQ^v}",),
+    "NSNextHashEnumeratorItem": (
+        b"^v^{_NSHashEnumerator=QQ^v}",
+        "",
+        {"arguments": {0: {"type_modifier": "N"}}},
+    ),
     "NSSwapHostLongLongToLittle": (b"QQ",),
     "NSClassFromString": (b"#@",),
     "NSSwapLittleLongToHost": (b"QQ",),
     "NSMakePoint": (b"{CGPoint=dd}dd",),
     "NSSizeFromString": (b"{CGSize=dd}@",),
     "NSConvertHostFloatToSwapped": (b"{_NSSwappedFloat=I}f",),
     "NSIntersectsRect": (
@@ -641,25 +659,33 @@
     "NSHashInsertIfAbsent": (b"^v@^v",),
     "NSSwapBigIntToHost": (b"II",),
     "NSRecycleZone": (b"v^{_NSZone=}",),
     "NSStringFromProtocol": (b"@@",),
     "NSFrameAddress": (b"^vQ",),
     "NSCountFrames": (b"Q",),
     "CFBridgingRelease": (b"@@",),
-    "NSMapMember": (b"Z@^v^^v^^v",),
+    "NSMapMember": (
+        b"Z@^v^^v^^v",
+        "",
+        {"arguments": {2: {"type_modifier": "o"}, 3: {"type_modifier": "o"}}},
+    ),
     "NSDivideRect": (
         b"v{CGRect={CGPoint=dd}{CGSize=dd}}^{CGRect={CGPoint=dd}{CGSize=dd}}^{CGRect={CGPoint=dd}{CGSize=dd}}dQ",
         "",
         {"arguments": {1: {"type_modifier": "o"}, 2: {"type_modifier": "o"}}},
     ),
     "NSRangeFromString": (b"{_NSRange=QQ}@",),
     "NSMapGet": (b"^v@^v",),
     "NSHashInsert": (b"v@^v",),
     "NSSwapHostIntToLittle": (b"II",),
-    "NSEndHashTableEnumeration": (b"v^{_NSHashEnumerator=QQ^v}",),
+    "NSEndHashTableEnumeration": (
+        b"v^{_NSHashEnumerator=QQ^v}",
+        "",
+        {"arguments": {0: {"type_modifier": "N"}}},
+    ),
     "NSZoneName": (b"@^{_NSZone=}",),
     "NSSwapHostFloatToBig": (b"{_NSSwappedFloat=I}f",),
     "NSTemporaryDirectory": (b"@",),
     "NSDecimalMultiplyByPowerOf10": (
         b"Q^{_NSDecimal=b8b4b1b1b18[8S]}^{_NSDecimal=b8b4b1b1b18[8S]}sQ",
         "",
         {"arguments": {0: {"type_modifier": "o"}, 1: {"type_modifier": "n"}}},
```

### Comparing `pyobjc-framework-Cocoa-9.1b1/Lib/Foundation/_nsobject.py` & `pyobjc-framework-Cocoa-9.2/Lib/Foundation/_nsobject.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Lib/PyObjCTools/AppCategories.py` & `pyobjc-framework-Cocoa-9.2/Lib/PyObjCTools/AppCategories.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Lib/PyObjCTools/AppHelper.py` & `pyobjc-framework-Cocoa-9.2/Lib/PyObjCTools/AppHelper.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Lib/PyObjCTools/Conversion.py` & `pyobjc-framework-Cocoa-9.2/Lib/PyObjCTools/Conversion.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Lib/PyObjCTools/FndCategories.py` & `pyobjc-framework-Cocoa-9.2/Lib/PyObjCTools/FndCategories.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Lib/pyobjc_framework_Cocoa.egg-info/PKG-INFO` & `pyobjc-framework-Cocoa-9.2/Lib/pyobjc_framework_Cocoa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-Cocoa
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the Cocoa frameworks on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,Cocoa,CoreFoundation,Foundation,AppKit
 Platform: MacOS X
```

### Comparing `pyobjc-framework-Cocoa-9.1b1/Lib/pyobjc_framework_Cocoa.egg-info/SOURCES.txt` & `pyobjc-framework-Cocoa-9.2/Lib/pyobjc_framework_Cocoa.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE.txt
 MANIFEST.in
 README.txt
 pyobjc_setup.py
+pyproject.toml
 setup.py
 todo.txt
 Examples/AppKit/ClassBrowser/ClassBrowser.py
 Examples/AppKit/ClassBrowser/setup.py
 Examples/AppKit/ClassBrowser/summary.txt
 Examples/AppKit/ClassBrowser/ClassBrowser.nib/classes.nib
 Examples/AppKit/ClassBrowser/ClassBrowser.nib/info.nib
```

### Comparing `pyobjc-framework-Cocoa-9.1b1/Modules/_AppKit.m` & `pyobjc-framework-Cocoa-9.2/Modules/_AppKit.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Modules/_AppKit_appmain.m` & `pyobjc-framework-Cocoa-9.2/Modules/_AppKit_appmain.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Modules/_AppKit_inlines.m` & `pyobjc-framework-Cocoa-9.2/Modules/_AppKit_inlines.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Modules/_AppKit_nsbezierpath.m` & `pyobjc-framework-Cocoa-9.2/Modules/_AppKit_nsbezierpath.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Modules/_AppKit_nsbitmap.m` & `pyobjc-framework-Cocoa-9.2/Modules/_AppKit_nsbitmap.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Modules/_AppKit_nsfont.m` & `pyobjc-framework-Cocoa-9.2/Modules/_AppKit_nsfont.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Modules/_AppKit_nsview.m` & `pyobjc-framework-Cocoa-9.2/Modules/_AppKit_nsview.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Modules/_AppKit_protocols.m` & `pyobjc-framework-Cocoa-9.2/Modules/_AppKit_protocols.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Modules/_CoreFoundation.m` & `pyobjc-framework-Cocoa-9.2/Modules/_CoreFoundation.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Modules/_CoreFoundation_CFBag.m` & `pyobjc-framework-Cocoa-9.2/Modules/_CoreFoundation_CFBag.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Modules/_CoreFoundation_CFBinaryHeap.m` & `pyobjc-framework-Cocoa-9.2/Modules/_CoreFoundation_CFBinaryHeap.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Modules/_CoreFoundation_CFBitVector.m` & `pyobjc-framework-Cocoa-9.2/Modules/_CoreFoundation_CFBitVector.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Modules/_CoreFoundation_CFCalendar.m` & `pyobjc-framework-Cocoa-9.2/Modules/_CoreFoundation_CFCalendar.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Modules/_CoreFoundation_CFDictionary.m` & `pyobjc-framework-Cocoa-9.2/Modules/_CoreFoundation_CFDictionary.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Modules/_CoreFoundation_CFFileDescriptor.m` & `pyobjc-framework-Cocoa-9.2/Modules/_CoreFoundation_CFFileDescriptor.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Modules/_CoreFoundation_CFMachPort.m` & `pyobjc-framework-Cocoa-9.2/Modules/_CoreFoundation_CFMachPort.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Modules/_CoreFoundation_CFMessagePort.m` & `pyobjc-framework-Cocoa-9.2/Modules/_CoreFoundation_CFMessagePort.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Modules/_CoreFoundation_CFNumber.m` & `pyobjc-framework-Cocoa-9.2/Modules/_CoreFoundation_CFNumber.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Modules/_CoreFoundation_CFNumberFormatter.m` & `pyobjc-framework-Cocoa-9.2/Modules/_CoreFoundation_CFNumberFormatter.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Modules/_CoreFoundation_CFReadStream.m` & `pyobjc-framework-Cocoa-9.2/Modules/_CoreFoundation_CFReadStream.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Modules/_CoreFoundation_CFRunLoopObserver.m` & `pyobjc-framework-Cocoa-9.2/Modules/_CoreFoundation_CFRunLoopObserver.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Modules/_CoreFoundation_CFRunLoopSource.m` & `pyobjc-framework-Cocoa-9.2/Modules/_CoreFoundation_CFRunLoopSource.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Modules/_CoreFoundation_CFRunLoopTimer.m` & `pyobjc-framework-Cocoa-9.2/Modules/_CoreFoundation_CFRunLoopTimer.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Modules/_CoreFoundation_CFSet.m` & `pyobjc-framework-Cocoa-9.2/Modules/_CoreFoundation_CFSet.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Modules/_CoreFoundation_CFSocket.m` & `pyobjc-framework-Cocoa-9.2/Modules/_CoreFoundation_CFSocket.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Modules/_CoreFoundation_CFTree.m` & `pyobjc-framework-Cocoa-9.2/Modules/_CoreFoundation_CFTree.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Modules/_CoreFoundation_CFWriteStream.m` & `pyobjc-framework-Cocoa-9.2/Modules/_CoreFoundation_CFWriteStream.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Modules/_CoreFoundation_inlines.m` & `pyobjc-framework-Cocoa-9.2/Modules/_CoreFoundation_inlines.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Modules/_Foundation.m` & `pyobjc-framework-Cocoa-9.2/Modules/_Foundation.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Modules/_Foundation_inlines.m` & `pyobjc-framework-Cocoa-9.2/Modules/_Foundation_inlines.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Modules/_Foundation_netservice.m` & `pyobjc-framework-Cocoa-9.2/Modules/_Foundation_netservice.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Modules/_Foundation_protocols.m` & `pyobjc-framework-Cocoa-9.2/Modules/_Foundation_protocols.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Modules/_Foundation_string.m` & `pyobjc-framework-Cocoa-9.2/Modules/_Foundation_string.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Modules/_Foundation_typecode.m` & `pyobjc-framework-Cocoa-9.2/Modules/_Foundation_typecode.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Modules/pyobjc-api.h` & `pyobjc-framework-Cocoa-9.2/Modules/pyobjc-api.h`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/Modules/pyobjc-compat.h` & `pyobjc-framework-Cocoa-9.2/Modules/pyobjc-compat.h`

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

### Comparing `pyobjc-framework-Cocoa-9.1b1/Modules/testhelper.m` & `pyobjc-framework-Cocoa-9.2/Modules/testhelper.m`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PKG-INFO` & `pyobjc-framework-Cocoa-9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-Cocoa
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the Cocoa frameworks on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,Cocoa,CoreFoundation,Foundation,AppKit
 Platform: MacOS X
```

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/guitest_graphics.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/guitest_graphics.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/guitest_nsalert.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/guitest_nsalert.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_appcategories.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_appcategories.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_apphelper.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_apphelper.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_appkit_protocols.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_appkit_protocols.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_appkiterrors.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_appkiterrors.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfarray.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfarray.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfattributedstring.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfattributedstring.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfbag.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfbag.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfbase.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfbase.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfbinaryheap.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfbinaryheap.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfbitvector.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfbitvector.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfbundle.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfbundle.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfbyteorder.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfbyteorder.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfcalendar.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfcalendar.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfcgtypes.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfcgtypes.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfcharacterset.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfcharacterset.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfdata.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfdata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfdate.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfdate.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfdateformatter.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfdateformatter.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfdictionary.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfdictionary.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cferror.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cferror.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cffiledescriptor.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cffiledescriptor.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cffilesecurity.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cffilesecurity.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cflocale.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cflocale.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfmachport.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfmachport.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfmessageport.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfmessageport.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfnotificationcenter.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfnotificationcenter.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfnumber.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfnumber.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfnumberformatter.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfnumberformatter.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfplugin.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfplugin.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfpreferences.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfpreferences.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfpropertylist.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfpropertylist.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfrunloop.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfrunloop.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfset.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfset.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfsocket.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfsocket.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfstream.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfstream.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfstring.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfstring.py`

 * *Files 0% similar despite different names*

```diff
@@ -734,12 +734,13 @@
         self.assertIsInstance(v, int)
         self.assertIsInstance(ch, int)
 
         self.assertResultIsBOOL(CoreFoundation.CFStringIsHyphenationAvailableForLocale)
         v = CoreFoundation.CFStringIsHyphenationAvailableForLocale(loc)
         self.assertIsInstance(v, bool)
 
+    @min_os_level("13.0")
     def test_functions13_0(self):
         self.assertArgIsPrintf(
             CoreFoundation.CFStringCreateStringWithValidatedFormat, 3
         )
         self.assertArgIsOut(CoreFoundation.CFStringCreateStringWithValidatedFormat, 4)
```

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfstringtokenizer.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfstringtokenizer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cftimezone.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cftimezone.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cftree.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cftree.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfurl.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfurl.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfurlaccess.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfurlaccess.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfurlenumerator.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfurlenumerator.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfusernotification.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfusernotification.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfuuid.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfuuid.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfxmlnode.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfxmlnode.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_cfxmlparser.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_cfxmlparser.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_constants.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_constants.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_convenience.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_convenience.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_conversion.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_conversion.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_foundation.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_foundation.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_foundationerrors.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_foundationerrors.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_globals.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_globals.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_keyvalue.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_keyvalue.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsaccessibility.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsaccessibility.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsaccessibilitycustomaction.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsaccessibilitycustomaction.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsaccessibilitycustomrotor.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsaccessibilitycustomrotor.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsaccessibilityprotocols.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsaccessibilityprotocols.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsaffinetransform.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsaffinetransform.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsalert.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsalert.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsanimation.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsanimation.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsanimationcontext.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsanimationcontext.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsappearance.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsappearance.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsappleeventdescriptor.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsappleeventdescriptor.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsappleeventmanager.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsappleeventmanager.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsapplescript.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsapplescript.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsapplication.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsapplication.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsarray.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsarray.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsarraycontroller.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsarraycontroller.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsatstypesetter.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsatstypesetter.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsattributedstring.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsattributedstring.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsattributedstring_appkit.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsattributedstring_appkit.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsbackgroundactivityscheduler.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsbackgroundactivityscheduler.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsbezierpath.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsbezierpath.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsbitmapimagerep.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsbitmapimagerep.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsbox.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsbox.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsbrowser.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsbrowser.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsbundle.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsbundle.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsbutton.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsbutton.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsbuttoncell.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsbuttoncell.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsbuttontouchbaritem.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsbuttontouchbaritem.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsbytecountformatter.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsbytecountformatter.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsbyteorder.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsbyteorder.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nscache.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nscache.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nscalendar.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nscalendar.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nscalendardate.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nscalendardate.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nscandidatelisttouchbaritem.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nscandidatelisttouchbaritem.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nscell.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nscell.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nscharacterset.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nscharacterset.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsclipview.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsclipview.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nscoder.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nscoder.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nscollectionview.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nscollectionview.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nscollectionviewcompositionallayout.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nscollectionviewcompositionallayout.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nscollectionviewflowlayout.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nscollectionviewflowlayout.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nscollectionviewlayout.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nscollectionviewlayout.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nscolor.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nscolor.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nscolorlist.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nscolorlist.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nscolorpanel.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nscolorpanel.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nscolorpicking.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nscolorpicking.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nscolorspace.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nscolorspace.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nscolorwell.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nscolorwell.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nscombobox.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nscombobox.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nscomboboxcell.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nscomboboxcell.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nscombobutton.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nscombobutton.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nscomparisonpredicate.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nscomparisonpredicate.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsconnection.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsconnection.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nscontrol.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nscontrol.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nscontroller.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nscontroller.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nscursor.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nscursor.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nscustomimagerep.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nscustomimagerep.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsdata.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsdata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsdatecomponentsformatter.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsdatecomponentsformatter.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsdateformatter.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsdateformatter.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsdateintervalformatter.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsdateintervalformatter.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsdatepicker.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsdatepicker.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsdatepickercell.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsdatepickercell.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsdebug.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsdebug.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsdecimalnumber.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsdecimalnumber.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsdictionary.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsdictionary.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsdistributednotificationcenter.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsdistributednotificationcenter.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsdocktile.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsdocktile.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsdocument.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsdocument.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsdocumentcontroller.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsdocumentcontroller.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsdragging.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsdragging.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsdraggingitem.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsdraggingitem.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsdraggingsession.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsdraggingsession.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsdrawer.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsdrawer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsenergyformatter.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsenergyformatter.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsenumerator.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsenumerator.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nserror.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nserror.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nserrors.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nserrors.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsevent.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsevent.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsexception.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsexception.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsexpression.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsexpression.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsextensioncontext.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsextensioncontext.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsfilecoordinator.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsfilecoordinator.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsfilehandle.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsfilehandle.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsfilemanager.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsfilemanager.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsfilepresenter.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsfilepresenter.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsfilepromiseprovider.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsfilepromiseprovider.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsfileversion.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsfileversion.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsfilewrapper.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsfilewrapper.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsfont.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsfont.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsfontcollection.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsfontcollection.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsfontdescriptor.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsfontdescriptor.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsfontmanager.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsfontmanager.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsfontpanel.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsfontpanel.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsformatter.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsformatter.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsgeometry.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsgeometry.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsgesturerecognizer.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsgesturerecognizer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsglyphgenerator.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsglyphgenerator.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsglyphinfo.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsglyphinfo.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsgradient.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsgradient.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsgraphics.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsgraphics.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsgraphicscontext.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsgraphicscontext.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsgridview.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsgridview.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nshapticfeedback.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nshapticfeedback.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nshashtable.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nshashtable.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nshelpmanager.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nshelpmanager.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nshfsfiletypes.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nshfsfiletypes.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nshost.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nshost.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nshttpcookie.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nshttpcookie.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nshttpcookiestorage.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nshttpcookiestorage.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsimage.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsimage.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsimagecell.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsimagecell.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsimagerep.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsimagerep.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsimageview.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsimageview.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsindexpath.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsindexpath.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsindexset.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsindexset.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsinputmanager.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsinputmanager.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsinputserver.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsinputserver.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsinterfacestyle.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsinterfacestyle.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsinvocation.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsinvocation.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsiso8601dateformatter.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsiso8601dateformatter.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsitemprovider.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsitemprovider.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsitemproviderreadingwriting.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsitemproviderreadingwriting.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsjavasetup.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsjavasetup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsjsonserialization.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsjsonserialization.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nskeyedarchiver.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nskeyedarchiver.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nskeyvaluebinding.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nskeyvaluebinding.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nskeyvaluecoding.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nskeyvaluecoding.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nskeyvalueobservering.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nskeyvalueobservering.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nslayoutconstraint.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nslayoutconstraint.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nslayoutmanager.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nslayoutmanager.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nslengthformatter.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nslengthformatter.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nslevelindicator.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nslevelindicator.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nslevelindicatorcell.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nslevelindicatorcell.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nslinguistictagger.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nslinguistictagger.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nslocale.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nslocale.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nslocalizedstring.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nslocalizedstring.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nslock.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nslock.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nslog.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nslog.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsmaptable.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsmaptable.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsmassformatter.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsmassformatter.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsmatrix.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsmatrix.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsmeasurementformatter.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsmeasurementformatter.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsmedialibrarybrowsercontroller.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsmedialibrarybrowsercontroller.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsmenu.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsmenu.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsmenuitem.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsmenuitem.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsmetadata.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsmetadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsmetadataattributes.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsmetadataattributes.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsmethodsignature.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsmethodsignature.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsmorphology.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsmorphology.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsnetservices.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsnetservices.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsnib.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsnib.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsnibloading.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsnibloading.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsnotification.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsnotification.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsnotificationqueue.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsnotificationqueue.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsnumber.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsnumber.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsnumberformatter.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsnumberformatter.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsobjcruntime.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsobjcruntime.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsobject.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsobject.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsobject_additions.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsobject_additions.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsobjectcontroller.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsobjectcontroller.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsopengl.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsopengl.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsopengllayer.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsopengllayer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsopenpanel.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsopenpanel.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsoperation.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsoperation.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsorderedcollectiondifference.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsorderedcollectiondifference.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsorderedset.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsorderedset.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsoutlineview.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsoutlineview.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nspagecontroller.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nspagecontroller.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nspagelayout.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nspagelayout.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nspanel.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nspanel.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsparagraphstyle.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsparagraphstyle.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nspasteboard.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nspasteboard.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nspasteboarditem.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nspasteboarditem.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nspathcell.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nspathcell.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nspathcontrol.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nspathcontrol.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nspathutilties.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nspathutilties.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nspdfpanel.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nspdfpanel.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nspersistentdocument.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nspersistentdocument.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nspersonnamecomponentsformatter.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nspersonnamecomponentsformatter.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nspickertouchBaritem.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nspickertouchBaritem.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nspointerarray.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nspointerarray.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nspointerfunctions.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nspointerfunctions.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nspopover.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nspopover.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nspopupbutton.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nspopupbutton.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nspopupbuttoncell.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nspopupbuttoncell.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsport.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsport.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsportnameserver.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsportnameserver.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nspredicate.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nspredicate.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsprinter.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsprinter.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsprintinfo.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsprintinfo.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsprintoperation.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsprintoperation.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsprintpanel.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsprintpanel.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsprocessinfo.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsprocessinfo.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsprogress.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsprogress.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsprogressindicator.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsprogressindicator.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nspropertylist.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nspropertylist.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsproxy.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsproxy.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsrange.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsrange.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsregularexpression.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsregularexpression.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsrelativedatetimeformatter.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsrelativedatetimeformatter.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsresponder.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsresponder.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsruleeditor.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsruleeditor.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsrulermarker.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsrulermarker.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsrulerview.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsrulerview.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsrunloop.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsrunloop.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsrunningapplication.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsrunningapplication.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nssavepanel.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nssavepanel.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsscanner.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsscanner.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsscreen.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsscreen.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsscriptclassdescription.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsscriptclassdescription.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsscriptcommand.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsscriptcommand.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsscriptcommanddescription.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsscriptcommanddescription.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsscriptkeyvaluecoding.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsscriptkeyvaluecoding.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsscriptobjectspecifier.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsscriptobjectspecifier.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsscriptwhosetests.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsscriptwhosetests.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsscroller.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsscroller.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsscrollview.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsscrollview.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsscrubber.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsscrubber.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsscrubberlayout.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsscrubberlayout.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nssearchfield.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nssearchfield.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nssearchfieldcell.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nssearchfieldcell.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nssegmentedcell.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nssegmentedcell.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nssegmentedcontrol.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nssegmentedcontrol.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsset.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsset.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nssharingservice.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nssharingservice.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nssharingservicepickertouchbaritem.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nssharingservicepickertouchbaritem.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsslider.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsslider.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsslidercell.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsslidercell.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nssortdescriptor.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nssortdescriptor.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nssound.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nssound.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsspeechrecognizer.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsspeechrecognizer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsspeechsynthesizer.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsspeechsynthesizer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsspellchecker.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsspellchecker.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsspellserver.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsspellserver.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nssplitview.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nssplitview.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nssplitviewcontroller.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nssplitviewcontroller.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nssplitviewitem.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nssplitviewitem.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsstackview.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsstackview.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsstatusitem.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsstatusitem.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsstoryboard.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsstoryboard.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsstoryboardsegue.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsstoryboardsegue.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsstream.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsstream.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsstring.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsstring.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsstringdrawing.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsstringdrawing.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstablecolumn.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstablecolumn.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstableheadercell.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstableheadercell.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstablerowview.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstablerowview.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstableview.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstableview.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstableviewdiffabledatasource.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstableviewdiffabledatasource.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstabview.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstabview.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstabviewcontroller.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstabviewcontroller.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstabviewitem.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstabviewitem.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstask.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstask.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstext.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstext.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstextattachment.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstextattachment.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstextcheckingclient.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstextcheckingclient.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstextcheckingresult.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstextcheckingresult.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstextcontainer.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstextcontainer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstextcontent.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstextcontent.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstextcontextmanager.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstextcontextmanager.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstextfield.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstextfield.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstextfieldcell.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstextfieldcell.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstextfinder.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstextfinder.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstextinputclient.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstextinputclient.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstextinputcontext.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstextinputcontext.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstextlayoutfragment.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstextlayoutfragment.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstextlayoutmanager.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstextlayoutmanager.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstextlist.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstextlist.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstextrange.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstextrange.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstextselection.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstextselection.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstextselectionnavigation.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstextselectionnavigation.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstextstorage.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstextstorage.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstexttable.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstexttable.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstextview.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstextview.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstextviewportlayoutcontroller.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstextviewportlayoutcontroller.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsthread.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsthread.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstimer.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstimer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstimezone.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstimezone.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstitlebaraccessoryviewcontroller.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstitlebaraccessoryviewcontroller.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstokenfield.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstokenfield.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstokenfieldcell.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstokenfieldcell.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstoolbar.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstoolbar.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstoolbaritem.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstoolbaritem.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstoolbaritemgroup.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstoolbaritemgroup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstouch.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstouch.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstouchbar.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstouchbar.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstouchbaritem.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstouchbaritem.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstrackingarea.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstrackingarea.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstreecontroller.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstreecontroller.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nstypesetter.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nstypesetter.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsubiquitouskeyvaluestore.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsubiquitouskeyvaluestore.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsundomanager.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsundomanager.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsurl.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsurl.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsurlcache.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsurlcache.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsurlconnection.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsurlconnection.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsurlcredential.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsurlcredential.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsurlcredentialstorage.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsurlcredentialstorage.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsurldownload.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsurldownload.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsurlerror.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsurlerror.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsurlhandle.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsurlhandle.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsurlprotectionspace.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsurlprotectionspace.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsurlprotocol.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsurlprotocol.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsurlrequest.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsurlrequest.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsurlsession.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsurlsession.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsuseractivity.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsuseractivity.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsuserdefaults.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsuserdefaults.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsuserinterfacecompression.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsuserinterfacecompression.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsuserinterfaceitemsearching.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsuserinterfaceitemsearching.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsuserinterfacelayout.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsuserinterfacelayout.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsuserinterfacevalidation.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsuserinterfacevalidation.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsusernotification.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsusernotification.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsuserscripttask.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsuserscripttask.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsuuid.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsuuid.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsvalue.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsvalue.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsvaluetransformer.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsvaluetransformer.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsview.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsview.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsviewcontroller.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsviewcontroller.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsvisualeffectview.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsvisualeffectview.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nswindow.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nswindow.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nswindowcontroller.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nswindowcontroller.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nswindowrestoration.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nswindowrestoration.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nswindowscripting.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nswindowscripting.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nswindowtabgroup.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nswindowtabgroup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsworkspace.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsworkspace.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsxmldocument.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsxmldocument.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsxmldtdnode.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsxmldtdnode.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsxmlnode.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsxmlnode.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsxmlnodeoptions.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsxmlnodeoptions.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsxmlparser.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsxmlparser.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nsxpcconnection.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nsxpcconnection.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_nszone.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_nszone.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_regr.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_regr.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 import os
 from threading import Thread
 
 import AppKit
 import Foundation
 from Foundation import NSAutoreleasePool, NSLog, NSObject
-from PyObjCTools.TestSupport import TestCase, min_os_level
+from PyObjCTools.TestSupport import (
+    TestCase,
+    min_os_level,
+    expectedFailureIf,
+    os_level_key,
+    os_release,
+)
 
 
 class TestRegr(TestCase):
     def testFSRepr(self):
         fm = Foundation.NSFileManager.defaultManager()
         self.assertRaises(
             TypeError, fm.stringWithFileSystemRepresentation_length_, b"/var"
@@ -86,14 +92,15 @@
                 AppKit.NSOpenGLPFANoRecovery,
                 AppKit.NSOpenGLPFAColorSize,
                 32,
             )
         )
 
     @min_os_level("10.6")
+    @expectedFailureIf(os_level_key(os_release()) < os_level_key("10.12"))
     def testBinaryPlist(self):
         for pl in ({"key": 2**64 - 1}, {"key": 2**16 - 1}):
             with self.subTest(pl):
                 (
                     data,
                     error,
                 ) = Foundation.NSPropertyListSerialization.dataWithPropertyList_format_options_error_(  # noqa: B950
```

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_structs.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_structs.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_subclassing.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_subclassing.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_threading.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_threading.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/PyObjCTest/test_weirdness.py` & `pyobjc-framework-Cocoa-9.2/PyObjCTest/test_weirdness.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/metadata/AppKit.fwinfo` & `pyobjc-framework-Cocoa-9.2/metadata/AppKit.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/metadata/CoreFoundation.fwinfo` & `pyobjc-framework-Cocoa-9.2/metadata/CoreFoundation.fwinfo`

 * *Files 0% similar despite different names*

```diff
@@ -5617,43 +5617,47 @@
      "0": {}
     },
     "retval": {
      "already_cfretained": true
     }
    },
    "CFXMLParserCreate": {
+    "ignore": true,
     "args": {
      "0": {},
      "1": {},
      "2": {},
      "5": {},
      "6": {}
     },
     "retval": {
      "already_cfretained": true
     }
    },
    "CFXMLParserCreateWithDataFromURL": {
+    "ignore": true,
     "args": {
      "0": {},
      "1": {},
      "4": {},
      "5": {}
     },
     "retval": {
      "already_cfretained": true
     }
    },
    "CFXMLParserGetCallBacks": {
+    "ignore": true,
     "args": {
      "0": {},
      "1": {}
     }
    },
    "CFXMLParserGetContext": {
+    "ignore": true,
     "args": {
      "0": {},
      "1": {}
     }
    },
    "CFXMLParserGetDocument": {
     "args": {
```

### Comparing `pyobjc-framework-Cocoa-9.1b1/metadata/Foundation.fwinfo` & `pyobjc-framework-Cocoa-9.2/metadata/Foundation.fwinfo`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998191550925926%*

 * *Differences: {"'definitions'": "{'functions': {'NSEndHashTableEnumeration': {'args': {'0': {replace: "*

 * *                  "OrderedDict([('type_modifier', 'N')])}}}, 'NSEndMapTableEnumeration': {'args': "*

 * *                  "{'0': {replace: OrderedDict([('type_modifier', 'N')])}}}, 'NSMapMember': "*

 * *                  "{'args': {'2': {replace: OrderedDict([('type_modifier', 'o')])}, '3': {replace: "*

 * *                  "OrderedDict([('type_modifier', 'o')])}}}, 'NSNextHashEnumeratorItem': {'args': "*

 * *                  "{'0': {r […]*

```diff
@@ -17073,20 +17073,24 @@
                     "2": {
                         "type_modifier": "o"
                     }
                 }
             },
             "NSEndHashTableEnumeration": {
                 "args": {
-                    "0": {}
+                    "0": {
+                        "type_modifier": "N"
+                    }
                 }
             },
             "NSEndMapTableEnumeration": {
                 "args": {
-                    "0": {}
+                    "0": {
+                        "type_modifier": "N"
+                    }
                 }
             },
             "NSGetSizeAndAlignment": {
                 "args": {
                     "0": {
                         "c_array_delimited_by_null": true,
                         "type_modifier": "n",
@@ -17194,34 +17198,46 @@
                     "1": {},
                     "2": {}
                 }
             },
             "NSMapMember": {
                 "args": {
                     "1": {},
-                    "2": {},
-                    "3": {}
+                    "2": {
+                        "type_modifier": "o"
+                    },
+                    "3": {
+                        "type_modifier": "o"
+                    }
                 }
             },
             "NSMapRemove": {
                 "args": {
                     "1": {}
                 }
             },
             "NSNextHashEnumeratorItem": {
                 "args": {
-                    "0": {}
+                    "0": {
+                        "type_modifier": "N"
+                    }
                 },
                 "retval": {}
             },
             "NSNextMapEnumeratorPair": {
                 "args": {
-                    "0": {},
-                    "1": {},
-                    "2": {}
+                    "0": {
+                        "type_modifier": "N"
+                    },
+                    "1": {
+                        "type_modifier": "o"
+                    },
+                    "2": {
+                        "type_modifier": "o"
+                    }
                 }
             },
             "NSReallocateCollectable": {
                 "ignore": true
             },
             "NSRecycleZone": {
                 "args": {
```

### Comparing `pyobjc-framework-Cocoa-9.1b1/metadata/raw.AppKit/arm64-12.0.fwinfo` & `pyobjc-framework-Cocoa-9.2/metadata/raw.AppKit/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/metadata/raw.AppKit/arm64-12.3.fwinfo` & `pyobjc-framework-Cocoa-9.2/metadata/raw.AppKit/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/metadata/raw.AppKit/arm64-13.0.fwinfo` & `pyobjc-framework-Cocoa-9.2/metadata/raw.AppKit/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/metadata/raw.AppKit/arm64-13.1.fwinfo` & `pyobjc-framework-Cocoa-9.2/metadata/raw.AppKit/arm64-13.1.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/metadata/raw.AppKit/arm64-13.3.fwinfo` & `pyobjc-framework-Cocoa-9.2/metadata/raw.AppKit/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/metadata/raw.AppKit/x86_64-10.10.fwinfo` & `pyobjc-framework-Cocoa-9.2/metadata/raw.AppKit/x86_64-10.10.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/metadata/raw.AppKit/x86_64-10.14.fwinfo` & `pyobjc-framework-Cocoa-9.2/metadata/raw.AppKit/x86_64-10.14.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/metadata/raw.AppKit/x86_64-10.15.fwinfo` & `pyobjc-framework-Cocoa-9.2/metadata/raw.AppKit/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/metadata/raw.AppKit/x86_64-10.16.fwinfo` & `pyobjc-framework-Cocoa-9.2/metadata/raw.AppKit/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/metadata/raw.AppKit/x86_64-10.6.fwinfo` & `pyobjc-framework-Cocoa-9.2/metadata/raw.AppKit/x86_64-10.6.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/metadata/raw.AppKit/x86_64-10.7.fwinfo` & `pyobjc-framework-Cocoa-9.2/metadata/raw.AppKit/x86_64-10.7.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/metadata/raw.AppKit/x86_64-10.8.fwinfo` & `pyobjc-framework-Cocoa-9.2/metadata/raw.AppKit/x86_64-10.8.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/metadata/raw.AppKit/x86_64-12.0.fwinfo` & `pyobjc-framework-Cocoa-9.2/metadata/raw.AppKit/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/metadata/raw.AppKit/x86_64-12.3.fwinfo` & `pyobjc-framework-Cocoa-9.2/metadata/raw.AppKit/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/metadata/raw.AppKit/x86_64-13.0.fwinfo` & `pyobjc-framework-Cocoa-9.2/metadata/raw.AppKit/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/metadata/raw.AppKit/x86_64-13.1.fwinfo` & `pyobjc-framework-Cocoa-9.2/metadata/raw.AppKit/x86_64-13.1.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/metadata/raw.AppKit/x86_64-13.3.fwinfo` & `pyobjc-framework-Cocoa-9.2/metadata/raw.AppKit/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/metadata/raw.CoreFoundation/arm64-12.0.fwinfo` & `pyobjc-framework-Cocoa-9.2/metadata/raw.CoreFoundation/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/metadata/raw.CoreFoundation/arm64-12.3.fwinfo` & `pyobjc-framework-Cocoa-9.2/metadata/raw.CoreFoundation/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/metadata/raw.CoreFoundation/arm64-13.0.fwinfo` & `pyobjc-framework-Cocoa-9.2/metadata/raw.CoreFoundation/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/metadata/raw.CoreFoundation/arm64-13.3.fwinfo` & `pyobjc-framework-Cocoa-9.2/metadata/raw.CoreFoundation/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/metadata/raw.CoreFoundation/x86_64-10.10.fwinfo` & `pyobjc-framework-Cocoa-9.2/metadata/raw.CoreFoundation/x86_64-10.10.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/metadata/raw.CoreFoundation/x86_64-10.15.fwinfo` & `pyobjc-framework-Cocoa-9.2/metadata/raw.CoreFoundation/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/metadata/raw.CoreFoundation/x86_64-10.16.fwinfo` & `pyobjc-framework-Cocoa-9.2/metadata/raw.CoreFoundation/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/metadata/raw.CoreFoundation/x86_64-10.6.fwinfo` & `pyobjc-framework-Cocoa-9.2/metadata/raw.CoreFoundation/x86_64-10.6.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/metadata/raw.CoreFoundation/x86_64-10.7.fwinfo` & `pyobjc-framework-Cocoa-9.2/metadata/raw.CoreFoundation/x86_64-10.7.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/metadata/raw.CoreFoundation/x86_64-10.8.fwinfo` & `pyobjc-framework-Cocoa-9.2/metadata/raw.CoreFoundation/x86_64-10.8.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/metadata/raw.CoreFoundation/x86_64-12.0.fwinfo` & `pyobjc-framework-Cocoa-9.2/metadata/raw.CoreFoundation/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/metadata/raw.CoreFoundation/x86_64-12.3.fwinfo` & `pyobjc-framework-Cocoa-9.2/metadata/raw.CoreFoundation/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/metadata/raw.CoreFoundation/x86_64-13.0.fwinfo` & `pyobjc-framework-Cocoa-9.2/metadata/raw.CoreFoundation/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/metadata/raw.CoreFoundation/x86_64-13.3.fwinfo` & `pyobjc-framework-Cocoa-9.2/metadata/raw.CoreFoundation/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/metadata/raw.Foundation/arm64-12.0.fwinfo` & `pyobjc-framework-Cocoa-9.2/metadata/raw.Foundation/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/metadata/raw.Foundation/arm64-12.3.fwinfo` & `pyobjc-framework-Cocoa-9.2/metadata/raw.Foundation/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/metadata/raw.Foundation/arm64-13.0.fwinfo` & `pyobjc-framework-Cocoa-9.2/metadata/raw.Foundation/arm64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/metadata/raw.Foundation/arm64-13.3.fwinfo` & `pyobjc-framework-Cocoa-9.2/metadata/raw.Foundation/arm64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/metadata/raw.Foundation/x86_64-10.10.fwinfo` & `pyobjc-framework-Cocoa-9.2/metadata/raw.Foundation/x86_64-10.10.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/metadata/raw.Foundation/x86_64-10.15.fwinfo` & `pyobjc-framework-Cocoa-9.2/metadata/raw.Foundation/x86_64-10.15.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/metadata/raw.Foundation/x86_64-10.16.fwinfo` & `pyobjc-framework-Cocoa-9.2/metadata/raw.Foundation/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/metadata/raw.Foundation/x86_64-10.8.fwinfo` & `pyobjc-framework-Cocoa-9.2/metadata/raw.Foundation/x86_64-10.8.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/metadata/raw.Foundation/x86_64-12.0.fwinfo` & `pyobjc-framework-Cocoa-9.2/metadata/raw.Foundation/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/metadata/raw.Foundation/x86_64-12.3.fwinfo` & `pyobjc-framework-Cocoa-9.2/metadata/raw.Foundation/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/metadata/raw.Foundation/x86_64-13.0.fwinfo` & `pyobjc-framework-Cocoa-9.2/metadata/raw.Foundation/x86_64-13.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/metadata/raw.Foundation/x86_64-13.3.fwinfo` & `pyobjc-framework-Cocoa-9.2/metadata/raw.Foundation/x86_64-13.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/pyobjc_setup.py` & `pyobjc-framework-Cocoa-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-Cocoa-9.1b1/setup.py` & `pyobjc-framework-Cocoa-9.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,17 +5,21 @@
 These wrappers don't include documentation, please check Apple's documentation
 for information on how to use these frameworks and PyObjC's documentation
 for general tips and tricks regarding the translation between Python
 and (Objective-)C frameworks
 """
 import os
 
-from pyobjc_setup import Extension, setup
+import sys
 
-VERSION = "9.1b1"
+sys.path.insert(0, os.path.dirname(__file__))
+
+from pyobjc_setup import Extension, setup  # noqa: E402
+
+VERSION = "9.2"
 
 setup(
     name="pyobjc-framework-Cocoa",
     description="Wrappers for the Cocoa frameworks on macOS",
     packages=["Cocoa", "CoreFoundation", "Foundation", "AppKit", "PyObjCTools"],
     ext_modules=[
         # CoreFoundation
```

