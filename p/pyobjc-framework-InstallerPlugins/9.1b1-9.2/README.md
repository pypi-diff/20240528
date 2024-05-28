# Comparing `tmp/pyobjc-framework-InstallerPlugins-9.1b1.tar.gz` & `tmp/pyobjc-framework-InstallerPlugins-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-InstallerPlugins-9.1b1.tar", last modified: Sun Mar 26 11:27:19 2023, max compression
+gzip compressed data, was "pyobjc-framework-InstallerPlugins-9.2.tar", last modified: Wed Jun  7 00:17:41 2023, max compression
```

## Comparing `pyobjc-framework-InstallerPlugins-9.1b1.tar` & `pyobjc-framework-InstallerPlugins-9.2.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:19.380817 pyobjc-framework-InstallerPlugins-9.1b1/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:19.297391 pyobjc-framework-InstallerPlugins-9.1b1/Examples/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:19.305562 pyobjc-framework-InstallerPlugins-9.1b1/Examples/InstallerPluginSample/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:19.297685 pyobjc-framework-InstallerPlugins-9.1b1/Examples/InstallerPluginSample/InstallerPluginsTestPackage.pkg/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:19.331483 pyobjc-framework-InstallerPlugins-9.1b1/Examples/InstallerPluginSample/InstallerPluginsTestPackage.pkg/Contents/
--rw-r--r--   0 ronald     (501) staff       (20)    35139 2020-11-30 18:45:15.000000 pyobjc-framework-InstallerPlugins-9.1b1/Examples/InstallerPluginSample/InstallerPluginsTestPackage.pkg/Contents/Archive.bom
--rw-r--r--   0 ronald     (501) staff       (20)      512 2020-11-30 18:45:15.000000 pyobjc-framework-InstallerPlugins-9.1b1/Examples/InstallerPluginSample/InstallerPluginsTestPackage.pkg/Contents/Archive.pax
--rw-r--r--   0 ronald     (501) staff       (20)     1495 2020-11-30 18:45:15.000000 pyobjc-framework-InstallerPlugins-9.1b1/Examples/InstallerPluginSample/InstallerPluginsTestPackage.pkg/Contents/Info.plist
--rw-r--r--   0 ronald     (501) staff       (20)        9 2020-11-30 18:45:15.000000 pyobjc-framework-InstallerPlugins-9.1b1/Examples/InstallerPluginSample/InstallerPluginsTestPackage.pkg/Contents/PkgInfo
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:19.334200 pyobjc-framework-InstallerPlugins-9.1b1/Examples/InstallerPluginSample/InstallerPluginsTestPackage.pkg/Contents/Resources/
--rw-r--r--   0 ronald     (501) staff       (20)      190 2020-11-30 18:45:15.000000 pyobjc-framework-InstallerPlugins-9.1b1/Examples/InstallerPluginSample/InstallerPluginsTestPackage.pkg/Contents/Resources/BundleVersions.plist
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:19.336080 pyobjc-framework-InstallerPlugins-9.1b1/Examples/InstallerPluginSample/InstallerPluginsTestPackage.pkg/Contents/Resources/English.lproj/
--rw-r--r--   0 ronald     (501) staff       (20)      339 2020-11-30 18:45:15.000000 pyobjc-framework-InstallerPlugins-9.1b1/Examples/InstallerPluginSample/InstallerPluginsTestPackage.pkg/Contents/Resources/English.lproj/Description.plist
--rw-r--r--   0 ronald     (501) staff       (20)      280 2020-11-30 18:45:15.000000 pyobjc-framework-InstallerPlugins-9.1b1/Examples/InstallerPluginSample/InstallerPluginsTestPackage.pkg/Contents/Resources/English.lproj/InstallerPluginsTestPackage.info
--rw-r--r--   0 ronald     (501) staff       (20)      726 2020-11-30 18:45:15.000000 pyobjc-framework-InstallerPlugins-9.1b1/Examples/InstallerPluginSample/InstallerPluginsTestPackage.pkg/Contents/Resources/English.lproj/Welcome.rtf
--rw-r--r--   0 ronald     (501) staff       (20)       44 2020-11-30 18:45:15.000000 pyobjc-framework-InstallerPlugins-9.1b1/Examples/InstallerPluginSample/InstallerPluginsTestPackage.pkg/Contents/Resources/InstallerPluginsTestPackage.sizes
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-InstallerPlugins-9.1b1/Examples/InstallerPluginSample/InstallerPluginsTestPackage.pkg/Contents/Resources/package_version
--rw-r--r--   0 ronald     (501) staff       (20)      454 2020-11-30 18:45:15.000000 pyobjc-framework-InstallerPlugins-9.1b1/Examples/InstallerPluginSample/InstallerSections.plist
--rw-r--r--   0 ronald     (501) staff       (20)     3140 2020-11-30 18:45:15.000000 pyobjc-framework-InstallerPlugins-9.1b1/Examples/InstallerPluginSample/ReadMe.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:19.337393 pyobjc-framework-InstallerPlugins-9.1b1/Examples/InstallerPluginSample/Registration/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:19.338181 pyobjc-framework-InstallerPlugins-9.1b1/Examples/InstallerPluginSample/Registration/English.lproj/
--rw-r--r--   0 ronald     (501) staff       (20)      262 2020-11-30 18:45:15.000000 pyobjc-framework-InstallerPlugins-9.1b1/Examples/InstallerPluginSample/Registration/English.lproj/Localizable.strings
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:19.340245 pyobjc-framework-InstallerPlugins-9.1b1/Examples/InstallerPluginSample/Registration/English.lproj/Registration.nib/
--rw-r--r--   0 ronald     (501) staff       (20)     1056 2020-11-30 18:45:15.000000 pyobjc-framework-InstallerPlugins-9.1b1/Examples/InstallerPluginSample/Registration/English.lproj/Registration.nib/classes.nib
--rw-r--r--   0 ronald     (501) staff       (20)      568 2020-11-30 18:45:15.000000 pyobjc-framework-InstallerPlugins-9.1b1/Examples/InstallerPluginSample/Registration/English.lproj/Registration.nib/info.nib
--rw-r--r--   0 ronald     (501) staff       (20)     6895 2020-11-30 18:45:15.000000 pyobjc-framework-InstallerPlugins-9.1b1/Examples/InstallerPluginSample/Registration/English.lproj/Registration.nib/keyedobjects.nib
--rw-r--r--   0 ronald     (501) staff       (20)     3074 2020-11-30 18:45:15.000000 pyobjc-framework-InstallerPlugins-9.1b1/Examples/InstallerPluginSample/Registration/RegistrationPane.py
--rw-r--r--   0 ronald     (501) staff       (20)      617 2020-11-30 18:45:15.000000 pyobjc-framework-InstallerPlugins-9.1b1/Examples/InstallerPluginSample/Registration/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       69 2020-11-30 18:45:15.000000 pyobjc-framework-InstallerPlugins-9.1b1/Examples/InstallerPluginSample/setup.py
--rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-InstallerPlugins-9.1b1/LICENSE.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:19.298897 pyobjc-framework-InstallerPlugins-9.1b1/Lib/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:19.341643 pyobjc-framework-InstallerPlugins-9.1b1/Lib/InstallerPlugins/
--rw-r--r--   0 ronald     (501) staff       (20)      735 2020-11-30 18:45:15.000000 pyobjc-framework-InstallerPlugins-9.1b1/Lib/InstallerPlugins/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     1732 2022-02-24 08:47:16.000000 pyobjc-framework-InstallerPlugins-9.1b1/Lib/InstallerPlugins/_metadata.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:19.351235 pyobjc-framework-InstallerPlugins-9.1b1/Lib/pyobjc_framework_InstallerPlugins.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)     2330 2023-03-26 11:27:19.000000 pyobjc-framework-InstallerPlugins-9.1b1/Lib/pyobjc_framework_InstallerPlugins.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)     2556 2023-03-26 11:27:19.000000 pyobjc-framework-InstallerPlugins-9.1b1/Lib/pyobjc_framework_InstallerPlugins.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2023-03-26 11:27:19.000000 pyobjc-framework-InstallerPlugins-9.1b1/Lib/pyobjc_framework_InstallerPlugins.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:21.000000 pyobjc-framework-InstallerPlugins-9.1b1/Lib/pyobjc_framework_InstallerPlugins.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (501) staff       (20)       49 2023-03-26 11:27:19.000000 pyobjc-framework-InstallerPlugins-9.1b1/Lib/pyobjc_framework_InstallerPlugins.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)       17 2023-03-26 11:27:19.000000 pyobjc-framework-InstallerPlugins-9.1b1/Lib/pyobjc_framework_InstallerPlugins.egg-info/top_level.txt
--rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-InstallerPlugins-9.1b1/MANIFEST.in
--rw-r--r--   0 ronald     (501) staff       (20)     2119 2023-03-26 11:27:19.379593 pyobjc-framework-InstallerPlugins-9.1b1/PKG-INFO
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:19.362544 pyobjc-framework-InstallerPlugins-9.1b1/PyObjCTest/
--rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-InstallerPlugins-9.1b1/PyObjCTest/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     1046 2022-02-24 08:47:16.000000 pyobjc-framework-InstallerPlugins-9.1b1/PyObjCTest/test_installerpane.py
--rw-r--r--   0 ronald     (501) staff       (20)      658 2022-04-11 08:03:15.000000 pyobjc-framework-InstallerPlugins-9.1b1/PyObjCTest/test_installerplugins.py
--rw-r--r--   0 ronald     (501) staff       (20)      292 2021-03-21 10:08:22.000000 pyobjc-framework-InstallerPlugins-9.1b1/PyObjCTest/test_installersection.py
--rw-r--r--   0 ronald     (501) staff       (20)      688 2021-03-21 10:08:22.000000 pyobjc-framework-InstallerPlugins-9.1b1/PyObjCTest/test_installerstate.py
--rw-r--r--   0 ronald     (501) staff       (20)      293 2021-10-18 19:38:40.000000 pyobjc-framework-InstallerPlugins-9.1b1/README.txt
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:19.365212 pyobjc-framework-InstallerPlugins-9.1b1/metadata/
--rw-r--r--   0 ronald     (501) staff       (20)     2185 2022-01-02 11:04:26.000000 pyobjc-framework-InstallerPlugins-9.1b1/metadata/InstallerPlugins.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)       47 2020-11-30 18:45:15.000000 pyobjc-framework-InstallerPlugins-9.1b1/metadata/metadata.ini
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-03-26 11:27:19.378722 pyobjc-framework-InstallerPlugins-9.1b1/metadata/raw/
--rw-r--r--   0 ronald     (501) staff       (20)    15969 2021-07-30 09:00:38.000000 pyobjc-framework-InstallerPlugins-9.1b1/metadata/raw/arm64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    16046 2022-02-24 08:47:16.000000 pyobjc-framework-InstallerPlugins-9.1b1/metadata/raw/arm64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    15970 2021-03-21 10:08:22.000000 pyobjc-framework-InstallerPlugins-9.1b1/metadata/raw/x86_64-10.16.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    10330 2020-11-30 18:45:15.000000 pyobjc-framework-InstallerPlugins-9.1b1/metadata/raw/x86_64-10.6.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    10330 2020-11-30 18:45:15.000000 pyobjc-framework-InstallerPlugins-9.1b1/metadata/raw/x86_64-10.7.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    10398 2020-11-30 18:45:15.000000 pyobjc-framework-InstallerPlugins-9.1b1/metadata/raw/x86_64-10.8.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    15970 2021-07-30 09:00:38.000000 pyobjc-framework-InstallerPlugins-9.1b1/metadata/raw/x86_64-12.0.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    16047 2022-02-24 08:47:16.000000 pyobjc-framework-InstallerPlugins-9.1b1/metadata/raw/x86_64-12.3.fwinfo
--rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-InstallerPlugins-9.1b1/pyobjc_setup.py
--rw-r--r--   0 ronald     (501) staff       (20)       38 2023-03-26 11:27:19.380947 pyobjc-framework-InstallerPlugins-9.1b1/setup.cfg
--rw-r--r--   0 ronald     (501) staff       (20)      844 2023-03-25 14:20:31.000000 pyobjc-framework-InstallerPlugins-9.1b1/setup.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:41.455520 pyobjc-framework-InstallerPlugins-9.2/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:41.393230 pyobjc-framework-InstallerPlugins-9.2/Examples/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:41.401727 pyobjc-framework-InstallerPlugins-9.2/Examples/InstallerPluginSample/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:41.393631 pyobjc-framework-InstallerPlugins-9.2/Examples/InstallerPluginSample/InstallerPluginsTestPackage.pkg/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:41.408651 pyobjc-framework-InstallerPlugins-9.2/Examples/InstallerPluginSample/InstallerPluginsTestPackage.pkg/Contents/
+-rw-r--r--   0 ronald     (501) staff       (20)    35139 2020-11-30 18:45:15.000000 pyobjc-framework-InstallerPlugins-9.2/Examples/InstallerPluginSample/InstallerPluginsTestPackage.pkg/Contents/Archive.bom
+-rw-r--r--   0 ronald     (501) staff       (20)      512 2020-11-30 18:45:15.000000 pyobjc-framework-InstallerPlugins-9.2/Examples/InstallerPluginSample/InstallerPluginsTestPackage.pkg/Contents/Archive.pax
+-rw-r--r--   0 ronald     (501) staff       (20)     1495 2020-11-30 18:45:15.000000 pyobjc-framework-InstallerPlugins-9.2/Examples/InstallerPluginSample/InstallerPluginsTestPackage.pkg/Contents/Info.plist
+-rw-r--r--   0 ronald     (501) staff       (20)        9 2020-11-30 18:45:15.000000 pyobjc-framework-InstallerPlugins-9.2/Examples/InstallerPluginSample/InstallerPluginsTestPackage.pkg/Contents/PkgInfo
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:41.410699 pyobjc-framework-InstallerPlugins-9.2/Examples/InstallerPluginSample/InstallerPluginsTestPackage.pkg/Contents/Resources/
+-rw-r--r--   0 ronald     (501) staff       (20)      190 2020-11-30 18:45:15.000000 pyobjc-framework-InstallerPlugins-9.2/Examples/InstallerPluginSample/InstallerPluginsTestPackage.pkg/Contents/Resources/BundleVersions.plist
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:41.412794 pyobjc-framework-InstallerPlugins-9.2/Examples/InstallerPluginSample/InstallerPluginsTestPackage.pkg/Contents/Resources/English.lproj/
+-rw-r--r--   0 ronald     (501) staff       (20)      339 2020-11-30 18:45:15.000000 pyobjc-framework-InstallerPlugins-9.2/Examples/InstallerPluginSample/InstallerPluginsTestPackage.pkg/Contents/Resources/English.lproj/Description.plist
+-rw-r--r--   0 ronald     (501) staff       (20)      280 2020-11-30 18:45:15.000000 pyobjc-framework-InstallerPlugins-9.2/Examples/InstallerPluginSample/InstallerPluginsTestPackage.pkg/Contents/Resources/English.lproj/InstallerPluginsTestPackage.info
+-rw-r--r--   0 ronald     (501) staff       (20)      726 2020-11-30 18:45:15.000000 pyobjc-framework-InstallerPlugins-9.2/Examples/InstallerPluginSample/InstallerPluginsTestPackage.pkg/Contents/Resources/English.lproj/Welcome.rtf
+-rw-r--r--   0 ronald     (501) staff       (20)       44 2020-11-30 18:45:15.000000 pyobjc-framework-InstallerPlugins-9.2/Examples/InstallerPluginSample/InstallerPluginsTestPackage.pkg/Contents/Resources/InstallerPluginsTestPackage.sizes
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-InstallerPlugins-9.2/Examples/InstallerPluginSample/InstallerPluginsTestPackage.pkg/Contents/Resources/package_version
+-rw-r--r--   0 ronald     (501) staff       (20)      454 2020-11-30 18:45:15.000000 pyobjc-framework-InstallerPlugins-9.2/Examples/InstallerPluginSample/InstallerSections.plist
+-rw-r--r--   0 ronald     (501) staff       (20)     3140 2020-11-30 18:45:15.000000 pyobjc-framework-InstallerPlugins-9.2/Examples/InstallerPluginSample/ReadMe.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:41.414279 pyobjc-framework-InstallerPlugins-9.2/Examples/InstallerPluginSample/Registration/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:41.415155 pyobjc-framework-InstallerPlugins-9.2/Examples/InstallerPluginSample/Registration/English.lproj/
+-rw-r--r--   0 ronald     (501) staff       (20)      262 2020-11-30 18:45:15.000000 pyobjc-framework-InstallerPlugins-9.2/Examples/InstallerPluginSample/Registration/English.lproj/Localizable.strings
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:41.417349 pyobjc-framework-InstallerPlugins-9.2/Examples/InstallerPluginSample/Registration/English.lproj/Registration.nib/
+-rw-r--r--   0 ronald     (501) staff       (20)     1056 2020-11-30 18:45:15.000000 pyobjc-framework-InstallerPlugins-9.2/Examples/InstallerPluginSample/Registration/English.lproj/Registration.nib/classes.nib
+-rw-r--r--   0 ronald     (501) staff       (20)      568 2020-11-30 18:45:15.000000 pyobjc-framework-InstallerPlugins-9.2/Examples/InstallerPluginSample/Registration/English.lproj/Registration.nib/info.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     6895 2020-11-30 18:45:15.000000 pyobjc-framework-InstallerPlugins-9.2/Examples/InstallerPluginSample/Registration/English.lproj/Registration.nib/keyedobjects.nib
+-rw-r--r--   0 ronald     (501) staff       (20)     3074 2020-11-30 18:45:15.000000 pyobjc-framework-InstallerPlugins-9.2/Examples/InstallerPluginSample/Registration/RegistrationPane.py
+-rw-r--r--   0 ronald     (501) staff       (20)      617 2020-11-30 18:45:15.000000 pyobjc-framework-InstallerPlugins-9.2/Examples/InstallerPluginSample/Registration/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       69 2020-11-30 18:45:15.000000 pyobjc-framework-InstallerPlugins-9.2/Examples/InstallerPluginSample/setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1249 2022-01-02 11:20:34.000000 pyobjc-framework-InstallerPlugins-9.2/LICENSE.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:41.395339 pyobjc-framework-InstallerPlugins-9.2/Lib/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:41.418672 pyobjc-framework-InstallerPlugins-9.2/Lib/InstallerPlugins/
+-rw-r--r--   0 ronald     (501) staff       (20)      735 2020-11-30 18:45:15.000000 pyobjc-framework-InstallerPlugins-9.2/Lib/InstallerPlugins/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1732 2022-02-24 08:47:16.000000 pyobjc-framework-InstallerPlugins-9.2/Lib/InstallerPlugins/_metadata.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:41.422025 pyobjc-framework-InstallerPlugins-9.2/Lib/pyobjc_framework_InstallerPlugins.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)     2328 2023-06-07 00:17:41.000000 pyobjc-framework-InstallerPlugins-9.2/Lib/pyobjc_framework_InstallerPlugins.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)     2571 2023-06-07 00:17:41.000000 pyobjc-framework-InstallerPlugins-9.2/Lib/pyobjc_framework_InstallerPlugins.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-07 00:17:41.000000 pyobjc-framework-InstallerPlugins-9.2/Lib/pyobjc_framework_InstallerPlugins.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2020-11-30 18:49:21.000000 pyobjc-framework-InstallerPlugins-9.2/Lib/pyobjc_framework_InstallerPlugins.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (501) staff       (20)       45 2023-06-07 00:17:41.000000 pyobjc-framework-InstallerPlugins-9.2/Lib/pyobjc_framework_InstallerPlugins.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       17 2023-06-07 00:17:41.000000 pyobjc-framework-InstallerPlugins-9.2/Lib/pyobjc_framework_InstallerPlugins.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (501) staff       (20)      260 2020-11-30 18:45:15.000000 pyobjc-framework-InstallerPlugins-9.2/MANIFEST.in
+-rw-r--r--   0 ronald     (501) staff       (20)     2117 2023-06-07 00:17:41.455112 pyobjc-framework-InstallerPlugins-9.2/PKG-INFO
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:41.435985 pyobjc-framework-InstallerPlugins-9.2/PyObjCTest/
+-rw-r--r--   0 ronald     (501) staff       (20)       18 2020-11-30 18:45:15.000000 pyobjc-framework-InstallerPlugins-9.2/PyObjCTest/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1046 2022-02-24 08:47:16.000000 pyobjc-framework-InstallerPlugins-9.2/PyObjCTest/test_installerpane.py
+-rw-r--r--   0 ronald     (501) staff       (20)      658 2022-04-11 08:03:15.000000 pyobjc-framework-InstallerPlugins-9.2/PyObjCTest/test_installerplugins.py
+-rw-r--r--   0 ronald     (501) staff       (20)      292 2021-03-21 10:08:22.000000 pyobjc-framework-InstallerPlugins-9.2/PyObjCTest/test_installersection.py
+-rw-r--r--   0 ronald     (501) staff       (20)      688 2021-03-21 10:08:22.000000 pyobjc-framework-InstallerPlugins-9.2/PyObjCTest/test_installerstate.py
+-rw-r--r--   0 ronald     (501) staff       (20)      293 2021-10-18 19:38:40.000000 pyobjc-framework-InstallerPlugins-9.2/README.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:41.437694 pyobjc-framework-InstallerPlugins-9.2/metadata/
+-rw-r--r--   0 ronald     (501) staff       (20)     2185 2022-01-02 11:04:26.000000 pyobjc-framework-InstallerPlugins-9.2/metadata/InstallerPlugins.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)       47 2020-11-30 18:45:15.000000 pyobjc-framework-InstallerPlugins-9.2/metadata/metadata.ini
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-07 00:17:41.454166 pyobjc-framework-InstallerPlugins-9.2/metadata/raw/
+-rw-r--r--   0 ronald     (501) staff       (20)    15969 2021-07-30 09:00:38.000000 pyobjc-framework-InstallerPlugins-9.2/metadata/raw/arm64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    16046 2022-02-24 08:47:16.000000 pyobjc-framework-InstallerPlugins-9.2/metadata/raw/arm64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    15970 2021-03-21 10:08:22.000000 pyobjc-framework-InstallerPlugins-9.2/metadata/raw/x86_64-10.16.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    10330 2020-11-30 18:45:15.000000 pyobjc-framework-InstallerPlugins-9.2/metadata/raw/x86_64-10.6.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    10330 2020-11-30 18:45:15.000000 pyobjc-framework-InstallerPlugins-9.2/metadata/raw/x86_64-10.7.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    10398 2020-11-30 18:45:15.000000 pyobjc-framework-InstallerPlugins-9.2/metadata/raw/x86_64-10.8.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    15970 2021-07-30 09:00:38.000000 pyobjc-framework-InstallerPlugins-9.2/metadata/raw/x86_64-12.0.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    16047 2022-02-24 08:47:16.000000 pyobjc-framework-InstallerPlugins-9.2/metadata/raw/x86_64-12.3.fwinfo
+-rw-r--r--   0 ronald     (501) staff       (20)    21186 2023-03-03 17:21:59.000000 pyobjc-framework-InstallerPlugins-9.2/pyobjc_setup.py
+-rw-r--r--   0 ronald     (501) staff       (20)       90 2023-04-27 08:17:30.000000 pyobjc-framework-InstallerPlugins-9.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-07 00:17:41.455623 pyobjc-framework-InstallerPlugins-9.2/setup.cfg
+-rw-r--r--   0 ronald     (501) staff       (20)      926 2023-05-29 10:07:46.000000 pyobjc-framework-InstallerPlugins-9.2/setup.py
```

### Comparing `pyobjc-framework-InstallerPlugins-9.1b1/Examples/InstallerPluginSample/InstallerPluginsTestPackage.pkg/Contents/Archive.bom` & `pyobjc-framework-InstallerPlugins-9.2/Examples/InstallerPluginSample/InstallerPluginsTestPackage.pkg/Contents/Archive.bom`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InstallerPlugins-9.1b1/Examples/InstallerPluginSample/InstallerPluginsTestPackage.pkg/Contents/Archive.pax` & `pyobjc-framework-InstallerPlugins-9.2/Examples/InstallerPluginSample/InstallerPluginsTestPackage.pkg/Contents/Archive.pax`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InstallerPlugins-9.1b1/Examples/InstallerPluginSample/InstallerPluginsTestPackage.pkg/Contents/Info.plist` & `pyobjc-framework-InstallerPlugins-9.2/Examples/InstallerPluginSample/InstallerPluginsTestPackage.pkg/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InstallerPlugins-9.1b1/Examples/InstallerPluginSample/InstallerPluginsTestPackage.pkg/Contents/Resources/English.lproj/Welcome.rtf` & `pyobjc-framework-InstallerPlugins-9.2/Examples/InstallerPluginSample/InstallerPluginsTestPackage.pkg/Contents/Resources/English.lproj/Welcome.rtf`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InstallerPlugins-9.1b1/Examples/InstallerPluginSample/ReadMe.txt` & `pyobjc-framework-InstallerPlugins-9.2/Examples/InstallerPluginSample/ReadMe.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InstallerPlugins-9.1b1/Examples/InstallerPluginSample/Registration/English.lproj/Registration.nib/classes.nib` & `pyobjc-framework-InstallerPlugins-9.2/Examples/InstallerPluginSample/Registration/English.lproj/Registration.nib/classes.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InstallerPlugins-9.1b1/Examples/InstallerPluginSample/Registration/English.lproj/Registration.nib/info.nib` & `pyobjc-framework-InstallerPlugins-9.2/Examples/InstallerPluginSample/Registration/English.lproj/Registration.nib/info.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InstallerPlugins-9.1b1/Examples/InstallerPluginSample/Registration/English.lproj/Registration.nib/keyedobjects.nib` & `pyobjc-framework-InstallerPlugins-9.2/Examples/InstallerPluginSample/Registration/English.lproj/Registration.nib/keyedobjects.nib`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InstallerPlugins-9.1b1/Examples/InstallerPluginSample/Registration/RegistrationPane.py` & `pyobjc-framework-InstallerPlugins-9.2/Examples/InstallerPluginSample/Registration/RegistrationPane.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InstallerPlugins-9.1b1/Examples/InstallerPluginSample/Registration/setup.py` & `pyobjc-framework-InstallerPlugins-9.2/Examples/InstallerPluginSample/Registration/setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InstallerPlugins-9.1b1/LICENSE.txt` & `pyobjc-framework-InstallerPlugins-9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InstallerPlugins-9.1b1/Lib/InstallerPlugins/__init__.py` & `pyobjc-framework-InstallerPlugins-9.2/Lib/InstallerPlugins/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InstallerPlugins-9.1b1/Lib/InstallerPlugins/_metadata.py` & `pyobjc-framework-InstallerPlugins-9.2/Lib/InstallerPlugins/_metadata.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InstallerPlugins-9.1b1/Lib/pyobjc_framework_InstallerPlugins.egg-info/PKG-INFO` & `pyobjc-framework-InstallerPlugins-9.2/Lib/pyobjc_framework_InstallerPlugins.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-InstallerPlugins
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework InstallerPlugins on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,InstallerPlugins
 Platform: MacOS X
```

### Comparing `pyobjc-framework-InstallerPlugins-9.1b1/Lib/pyobjc_framework_InstallerPlugins.egg-info/SOURCES.txt` & `pyobjc-framework-InstallerPlugins-9.2/Lib/pyobjc_framework_InstallerPlugins.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE.txt
 MANIFEST.in
 README.txt
 pyobjc_setup.py
+pyproject.toml
 setup.py
 Examples/InstallerPluginSample/InstallerSections.plist
 Examples/InstallerPluginSample/ReadMe.txt
 Examples/InstallerPluginSample/setup.py
 Examples/InstallerPluginSample/InstallerPluginsTestPackage.pkg/Contents/Archive.bom
 Examples/InstallerPluginSample/InstallerPluginsTestPackage.pkg/Contents/Archive.pax
 Examples/InstallerPluginSample/InstallerPluginsTestPackage.pkg/Contents/Info.plist
```

### Comparing `pyobjc-framework-InstallerPlugins-9.1b1/PKG-INFO` & `pyobjc-framework-InstallerPlugins-9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobjc-framework-InstallerPlugins
-Version: 9.1b1
+Version: 9.2
 Summary: Wrappers for the framework InstallerPlugins on macOS
 Home-page: https://github.com/ronaldoussoren/pyobjc
 Author: Ronald Oussoren
 Author-email: pyobjc-dev@lists.sourceforge.net
 License: MIT License
 Keywords: PyObjC,InstallerPlugins
 Platform: MacOS X
```

### Comparing `pyobjc-framework-InstallerPlugins-9.1b1/PyObjCTest/test_installerpane.py` & `pyobjc-framework-InstallerPlugins-9.2/PyObjCTest/test_installerpane.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InstallerPlugins-9.1b1/PyObjCTest/test_installerplugins.py` & `pyobjc-framework-InstallerPlugins-9.2/PyObjCTest/test_installerplugins.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InstallerPlugins-9.1b1/PyObjCTest/test_installerstate.py` & `pyobjc-framework-InstallerPlugins-9.2/PyObjCTest/test_installerstate.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InstallerPlugins-9.1b1/metadata/InstallerPlugins.fwinfo` & `pyobjc-framework-InstallerPlugins-9.2/metadata/InstallerPlugins.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InstallerPlugins-9.1b1/metadata/raw/arm64-12.0.fwinfo` & `pyobjc-framework-InstallerPlugins-9.2/metadata/raw/arm64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InstallerPlugins-9.1b1/metadata/raw/arm64-12.3.fwinfo` & `pyobjc-framework-InstallerPlugins-9.2/metadata/raw/arm64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InstallerPlugins-9.1b1/metadata/raw/x86_64-10.16.fwinfo` & `pyobjc-framework-InstallerPlugins-9.2/metadata/raw/x86_64-10.16.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InstallerPlugins-9.1b1/metadata/raw/x86_64-10.6.fwinfo` & `pyobjc-framework-InstallerPlugins-9.2/metadata/raw/x86_64-10.6.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InstallerPlugins-9.1b1/metadata/raw/x86_64-10.7.fwinfo` & `pyobjc-framework-InstallerPlugins-9.2/metadata/raw/x86_64-10.7.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InstallerPlugins-9.1b1/metadata/raw/x86_64-10.8.fwinfo` & `pyobjc-framework-InstallerPlugins-9.2/metadata/raw/x86_64-10.8.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InstallerPlugins-9.1b1/metadata/raw/x86_64-12.0.fwinfo` & `pyobjc-framework-InstallerPlugins-9.2/metadata/raw/x86_64-12.0.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InstallerPlugins-9.1b1/metadata/raw/x86_64-12.3.fwinfo` & `pyobjc-framework-InstallerPlugins-9.2/metadata/raw/x86_64-12.3.fwinfo`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InstallerPlugins-9.1b1/pyobjc_setup.py` & `pyobjc-framework-InstallerPlugins-9.2/pyobjc_setup.py`

 * *Files identical despite different names*

### Comparing `pyobjc-framework-InstallerPlugins-9.1b1/setup.py` & `pyobjc-framework-InstallerPlugins-9.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,17 +5,23 @@
 on macOS.
 
 These wrappers don't include documentation, please check Apple's documentation
 for information on how to use this framework and PyObjC's documentation
 for general tips and tricks regarding the translation between Python
 and (Objective-)C frameworks
 """
-from pyobjc_setup import setup
+import os
+import sys
 
-VERSION = "9.1b1"
+sys.path.insert(0, os.path.dirname(__file__))
+
+
+from pyobjc_setup import setup  # noqa: E402
+
+VERSION = "9.2"
 
 setup(
     name="pyobjc-framework-InstallerPlugins",
     description="Wrappers for the framework InstallerPlugins on macOS",
     packages=["InstallerPlugins"],
     version=VERSION,
     install_requires=["pyobjc-core>=" + VERSION, "pyobjc-framework-Cocoa>=" + VERSION],
```

