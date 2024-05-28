# Comparing `tmp/Furious-GUI-0.4.5.tar.gz` & `tmp/Furious-GUI-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Furious-GUI-0.4.5.tar", last modified: Wed May 15 05:15:52 2024, max compression
+gzip compressed data, was "Furious-GUI-0.4.6.tar", last modified: Tue May 28 07:49:57 2024, max compression
```

## Comparing `Furious-GUI-0.4.5.tar` & `Furious-GUI-0.4.6.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:15:52.299387 Furious-GUI-0.4.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:15:52.251387 Furious-GUI-0.4.5/Furious/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:15:52.251387 Furious-GUI-0.4.5/Furious/Core/
--rw-r--r--   0 runner    (1001) docker     (127)    16625 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Core/CoreManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Core/Hysteria1.py
--rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Core/Hysteria2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Core/Tun2socks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Core/XrayCore.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:15:52.247387 Furious-GUI-0.4.5/Furious/Data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:15:52.251387 Furious-GUI-0.4.5/Furious/Data/font/
--rw-r--r--   0 runner    (1001) docker     (127)   624892 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Data/font/CascadiaMono
--rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Data/font/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:15:52.255386 Furious-GUI-0.4.5/Furious/Data/hysteria/
--rw-r--r--   0 runner    (1001) docker     (127)  1974430 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Data/hysteria/bypass-Iran.acl
--rw-r--r--   0 runner    (1001) docker     (127)  1390176 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Data/hysteria/bypass-mainland-China.acl
--rw-r--r--   0 runner    (1001) docker     (127)  6444374 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Data/hysteria/country.mmdb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:15:52.283387 Furious-GUI-0.4.5/Furious/Data/xray/
--rw-r--r--   0 runner    (1001) docker     (127) 10715744 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Data/xray/geoip.dat
--rw-r--r--   0 runner    (1001) docker     (127)  6057957 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Data/xray/geosite.dat
--rw-r--r--   0 runner    (1001) docker     (127)  3199463 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Data/xray/iran.dat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:15:52.287387 Furious-GUI-0.4.5/Furious/Externals/
--rw-r--r--   0 runner    (1001) docker     (127)    40204 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Externals/GenTranslation.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Externals/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:15:52.291386 Furious-GUI-0.4.5/Furious/Interface/
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Interface/Application.py
--rw-r--r--   0 runner    (1001) docker     (127)     5813 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Interface/ConfigurationFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Interface/CoreFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Interface/Encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Interface/GuiEditorItemFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Interface/ItemUpdateProtocol.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Interface/Storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Interface/UserServersTableItem.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Interface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:15:52.291386 Furious-GUI-0.4.5/Furious/Library/
--rw-r--r--   0 runner    (1001) docker     (127)    55774 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Library/Configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4740 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Library/EmptyFactoryHelper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Library/Encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Library/Tcping.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Library/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:15:52.291386 Furious-GUI-0.4.5/Furious/PyFramework/
--rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/PyFramework/Ancestors.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/PyFramework/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:15:52.291386 Furious-GUI-0.4.5/Furious/QtFramework/
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/QtFramework/Ancestors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5970 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/QtFramework/CoreProcess.py
--rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/QtFramework/DNSResolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/QtFramework/DynamicTheme.py
--rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/QtFramework/DynamicTranslate.py
--rw-r--r--   0 runner    (1001) docker     (127)    11381 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/QtFramework/GuiEditorXXX.py
--rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/QtFramework/NetworkStateManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6856 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/QtFramework/QtGui.py
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/QtFramework/QtNetwork.py
--rw-r--r--   0 runner    (1001) docker     (127)    16523 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/QtFramework/QtWidgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     9416 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/QtFramework/TextEditor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/QtFramework/TextEditorTheme.py
--rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/QtFramework/UpdatesManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/QtFramework/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:15:52.291386 Furious-GUI-0.4.5/Furious/Storage/
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Storage/UserServers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Storage/UserSubs.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:15:52.295387 Furious-GUI-0.4.5/Furious/TrayActions/
--rw-r--r--   0 runner    (1001) docker     (127)    10277 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/TrayActions/Connect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/TrayActions/EditConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/TrayActions/Exit.py
--rw-r--r--   0 runner    (1001) docker     (127)     8689 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/TrayActions/Import.py
--rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/TrayActions/Language.py
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/TrayActions/Routing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/TrayActions/Settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/TrayActions/SystemProxy.py
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/TrayActions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:15:52.295387 Furious-GUI-0.4.5/Furious/Utility/
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Utility/AppMainProcess.py
--rw-r--r--   0 runner    (1001) docker     (127)    80238 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Utility/AppResources.py
--rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Utility/AppSettings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Utility/AppSettingsFn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Utility/Constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Utility/PySide6Legacy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6306 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Utility/StartupOnBoot.py
--rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Utility/SystemProxy.py
--rw-r--r--   0 runner    (1001) docker     (127)    15978 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Utility/SystemRoutingTable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Utility/SystemRuntime.py
--rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Utility/Utility.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:15:52.299387 Furious-GUI-0.4.5/Furious/Widget/
--rw-r--r--   0 runner    (1001) docker     (127)    12198 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Widget/Application.py
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Widget/ConnectProgressBar.py
--rw-r--r--   0 runner    (1001) docker     (127)     9602 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Widget/GuiHysteria1.py
--rw-r--r--   0 runner    (1001) docker     (127)    13476 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Widget/GuiHysteria2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Widget/GuiShadowsocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5854 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Widget/GuiTrojan.py
--rw-r--r--   0 runner    (1001) docker     (127)     9638 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Widget/GuiVLESS.py
--rw-r--r--   0 runner    (1001) docker     (127)     9578 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Widget/GuiVMess.py
--rw-r--r--   0 runner    (1001) docker     (127)    16043 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Widget/GuiVTLS.py
--rw-r--r--   0 runner    (1001) docker     (127)    32650 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Widget/GuiVTransport.py
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Widget/IndentSpinBox.py
--rw-r--r--   0 runner    (1001) docker     (127)     6972 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Widget/SystemTrayIcon.py
--rw-r--r--   0 runner    (1001) docker     (127)    50832 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Widget/UserServersQTableWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)     7979 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Widget/UserSubsQTableWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)     7592 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Widget/XrayAssetViewerQListWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Widget/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:15:52.299387 Furious-GUI-0.4.5/Furious/Window/
--rw-r--r--   0 runner    (1001) docker     (127)    15068 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Window/AppMainWindow.py
--rw-r--r--   0 runner    (1001) docker     (127)     5443 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Window/LogViewerWindow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Window/QRCodeWindow.py
--rw-r--r--   0 runner    (1001) docker     (127)    14571 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Window/TextEditorWindow.py
--rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Window/UserSubsWindow.py
--rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Window/XrayAssetViewerWindow.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/Window/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/Furious/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:15:52.299387 Furious-GUI-0.4.5/Furious_GUI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-15 05:15:52.000000 Furious-GUI-0.4.5/Furious_GUI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-05-15 05:15:52.000000 Furious-GUI-0.4.5/Furious_GUI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 05:15:52.000000 Furious-GUI-0.4.5/Furious_GUI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-15 05:15:52.000000 Furious-GUI-0.4.5/Furious_GUI.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-15 05:15:52.000000 Furious-GUI-0.4.5/Furious_GUI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 05:15:52.000000 Furious-GUI-0.4.5/Furious_GUI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-15 05:15:52.299387 Furious-GUI-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 05:15:52.299387 Furious-GUI-0.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-05-15 05:15:30.000000 Furious-GUI-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:49:57.390346 Furious-GUI-0.4.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:49:57.338347 Furious-GUI-0.4.6/Furious/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:49:57.338347 Furious-GUI-0.4.6/Furious/Core/
+-rw-r--r--   0 runner    (1001) docker     (127)    16625 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Core/CoreManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Core/Hysteria1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Core/Hysteria2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Core/Tun2socks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Core/XrayCore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:49:57.338347 Furious-GUI-0.4.6/Furious/Data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:49:57.342347 Furious-GUI-0.4.6/Furious/Data/font/
+-rw-r--r--   0 runner    (1001) docker     (127)   624892 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Data/font/CascadiaMono
+-rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Data/font/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:49:57.346347 Furious-GUI-0.4.6/Furious/Data/hysteria/
+-rw-r--r--   0 runner    (1001) docker     (127)  1974430 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Data/hysteria/bypass-Iran.acl
+-rw-r--r--   0 runner    (1001) docker     (127)  1390176 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Data/hysteria/bypass-mainland-China.acl
+-rw-r--r--   0 runner    (1001) docker     (127)  6444374 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Data/hysteria/country.mmdb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:49:57.374347 Furious-GUI-0.4.6/Furious/Data/xray/
+-rw-r--r--   0 runner    (1001) docker     (127) 10715744 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Data/xray/geoip.dat
+-rw-r--r--   0 runner    (1001) docker     (127)  6057957 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Data/xray/geosite.dat
+-rw-r--r--   0 runner    (1001) docker     (127)  3199463 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Data/xray/iran.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:49:57.378347 Furious-GUI-0.4.6/Furious/Externals/
+-rw-r--r--   0 runner    (1001) docker     (127)    40426 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Externals/GenTranslation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Externals/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:49:57.378347 Furious-GUI-0.4.6/Furious/Interface/
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Interface/Application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5813 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Interface/ConfigurationFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Interface/CoreFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Interface/Encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Interface/GuiEditorItemFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Interface/ItemUpdateProtocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Interface/Storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Interface/UserServersTableItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Interface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:49:57.378347 Furious-GUI-0.4.6/Furious/Library/
+-rw-r--r--   0 runner    (1001) docker     (127)    55774 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Library/Configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4740 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Library/EmptyFactoryHelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Library/Encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Library/Tcping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Library/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:49:57.378347 Furious-GUI-0.4.6/Furious/PyFramework/
+-rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/PyFramework/Ancestors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/PyFramework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:49:57.382346 Furious-GUI-0.4.6/Furious/QtFramework/
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/QtFramework/Ancestors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6215 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/QtFramework/CoreProcess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/QtFramework/DNSResolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/QtFramework/DynamicTheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/QtFramework/DynamicTranslate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11381 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/QtFramework/GuiEditorXXX.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/QtFramework/NetworkStateManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6856 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/QtFramework/QtGui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/QtFramework/QtNetwork.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17081 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/QtFramework/QtWidgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9416 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/QtFramework/TextEditor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/QtFramework/TextEditorTheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/QtFramework/UpdatesManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/QtFramework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:49:57.382346 Furious-GUI-0.4.6/Furious/Storage/
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Storage/UserServers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Storage/UserSubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:49:57.382346 Furious-GUI-0.4.6/Furious/TrayActions/
+-rw-r--r--   0 runner    (1001) docker     (127)    10277 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/TrayActions/Connect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/TrayActions/EditConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/TrayActions/Exit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8689 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/TrayActions/Import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/TrayActions/Language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/TrayActions/Routing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6851 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/TrayActions/Settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/TrayActions/SystemProxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/TrayActions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:49:57.386346 Furious-GUI-0.4.6/Furious/Utility/
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Utility/AppMainProcess.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80238 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Utility/AppResources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Utility/AppSettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Utility/AppSettingsFn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Utility/Constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Utility/PySide6Legacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6306 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Utility/StartupOnBoot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Utility/SystemProxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15978 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Utility/SystemRoutingTable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Utility/SystemRuntime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Utility/Utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:49:57.386346 Furious-GUI-0.4.6/Furious/Widget/
+-rw-r--r--   0 runner    (1001) docker     (127)    12198 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Widget/Application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Widget/ConnectProgressBar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9602 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Widget/GuiHysteria1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13476 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Widget/GuiHysteria2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Widget/GuiShadowsocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5854 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Widget/GuiTrojan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9638 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Widget/GuiVLESS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9578 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Widget/GuiVMess.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16043 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Widget/GuiVTLS.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32650 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Widget/GuiVTransport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Widget/IndentSpinBox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6972 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Widget/SystemTrayIcon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50871 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Widget/UserServersQTableWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7979 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Widget/UserSubsQTableWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8608 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Widget/XrayAssetViewerQListWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Widget/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:49:57.386346 Furious-GUI-0.4.6/Furious/Window/
+-rw-r--r--   0 runner    (1001) docker     (127)    15022 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Window/AppMainWindow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5443 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Window/LogViewerWindow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Window/QRCodeWindow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14196 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Window/TextEditorWindow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Window/UserSubsWindow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Window/XrayAssetViewerWindow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/Window/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/Furious/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:49:57.390346 Furious-GUI-0.4.6/Furious_GUI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-28 07:49:57.000000 Furious-GUI-0.4.6/Furious_GUI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-05-28 07:49:57.000000 Furious-GUI-0.4.6/Furious_GUI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 07:49:57.000000 Furious-GUI-0.4.6/Furious_GUI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-28 07:49:57.000000 Furious-GUI-0.4.6/Furious_GUI.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-28 07:49:57.000000 Furious-GUI-0.4.6/Furious_GUI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-28 07:49:57.000000 Furious-GUI-0.4.6/Furious_GUI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-28 07:49:57.390346 Furious-GUI-0.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 07:49:57.390346 Furious-GUI-0.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-05-28 07:49:34.000000 Furious-GUI-0.4.6/setup.py
```

### Comparing `Furious-GUI-0.4.5/Furious/Core/CoreManager.py` & `Furious-GUI-0.4.6/Furious/Core/CoreManager.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Core/Hysteria1.py` & `Furious-GUI-0.4.6/Furious/Core/Hysteria1.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Core/Hysteria2.py` & `Furious-GUI-0.4.6/Furious/Core/Hysteria2.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Core/Tun2socks.py` & `Furious-GUI-0.4.6/Furious/Core/Tun2socks.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Core/XrayCore.py` & `Furious-GUI-0.4.6/Furious/Core/XrayCore.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Core/__init__.py` & `Furious-GUI-0.4.6/Furious/Core/__init__.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Data/font/CascadiaMono` & `Furious-GUI-0.4.6/Furious/Data/font/CascadiaMono`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Data/font/LICENSE` & `Furious-GUI-0.4.6/Furious/Data/font/LICENSE`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Data/hysteria/bypass-Iran.acl` & `Furious-GUI-0.4.6/Furious/Data/hysteria/bypass-Iran.acl`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Data/hysteria/bypass-mainland-China.acl` & `Furious-GUI-0.4.6/Furious/Data/hysteria/bypass-mainland-China.acl`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Data/hysteria/country.mmdb` & `Furious-GUI-0.4.6/Furious/Data/hysteria/country.mmdb`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Data/xray/geoip.dat` & `Furious-GUI-0.4.6/Furious/Data/xray/geoip.dat`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Data/xray/geosite.dat` & `Furious-GUI-0.4.6/Furious/Data/xray/geosite.dat`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Data/xray/iran.dat` & `Furious-GUI-0.4.6/Furious/Data/xray/iran.dat`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Externals/GenTranslation.py` & `Furious-GUI-0.4.6/Furious/Externals/GenTranslation.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,15 +194,15 @@
     "Cancel": {
         "source": [
             "Furious.QtFramework.GuiEditorXXX",
             "Furious.Widget.IndentSpinBox",
             "Furious.Window.TextEditorWindow",
             "Furious.Window.UserSubsWindow"
         ],
-        "RU": "Отменить",
+        "RU": "Отмена",
         "ZH": "取消",
         "isReviewed": "True"
     },
     "Save Changes": {
         "source": [
             "Furious.Window.TextEditorWindow"
         ],
@@ -1325,9 +1325,17 @@
     "Select and press Enter to activate configuration and connect": {
         "source": [
             "Furious.TrayActions.Connect"
         ],
         "RU": "Выберите и нажмите Enter, чтобы активировать конфигурацию и подключиться",
         "ZH": "选择并按下Enter键以激活配置并连接",
         "isReviewed": "True"
+    },
+    "Power Save Mode": {
+        "source": [
+            "Furious.TrayActions.Settings"
+        ],
+        "RU": "Режим энергосбережения",
+        "ZH": "省电模式",
+        "isReviewed": "True"
     }
 }
```

### Comparing `Furious-GUI-0.4.5/Furious/Externals/__init__.py` & `Furious-GUI-0.4.6/Furious/Externals/__init__.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Interface/Application.py` & `Furious-GUI-0.4.6/Furious/Interface/Application.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Interface/ConfigurationFactory.py` & `Furious-GUI-0.4.6/Furious/Interface/ConfigurationFactory.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Interface/CoreFactory.py` & `Furious-GUI-0.4.6/Furious/Interface/CoreFactory.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Interface/Encoder.py` & `Furious-GUI-0.4.6/Furious/Interface/Encoder.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Interface/GuiEditorItemFactory.py` & `Furious-GUI-0.4.6/Furious/Interface/GuiEditorItemFactory.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Interface/ItemUpdateProtocol.py` & `Furious-GUI-0.4.6/Furious/Interface/ItemUpdateProtocol.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Interface/Storage.py` & `Furious-GUI-0.4.6/Furious/Interface/Storage.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Interface/UserServersTableItem.py` & `Furious-GUI-0.4.6/Furious/Interface/UserServersTableItem.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Interface/__init__.py` & `Furious-GUI-0.4.6/Furious/Interface/__init__.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Library/Configuration.py` & `Furious-GUI-0.4.6/Furious/Library/Configuration.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Library/EmptyFactoryHelper.py` & `Furious-GUI-0.4.6/Furious/Library/EmptyFactoryHelper.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Library/Encoder.py` & `Furious-GUI-0.4.6/Furious/Library/Encoder.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Library/Tcping.py` & `Furious-GUI-0.4.6/Furious/Library/Tcping.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Library/__init__.py` & `Furious-GUI-0.4.6/Furious/Library/__init__.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/PyFramework/Ancestors.py` & `Furious-GUI-0.4.6/Furious/PyFramework/Ancestors.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/PyFramework/__init__.py` & `Furious-GUI-0.4.6/Furious/PyFramework/__init__.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/QtFramework/Ancestors.py` & `Furious-GUI-0.4.6/Furious/QtFramework/Ancestors.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/QtFramework/CoreProcess.py` & `Furious-GUI-0.4.6/Furious/QtFramework/CoreProcess.py`

 * *Files 4% similar despite different names*

```diff
@@ -118,16 +118,22 @@
         self._msgTimer.start(self.MSG_PRODUCE_THRESHOLD)
 
         if waitCore:
             # Wait for the core to start up completely
             PySide6LegacyEventLoopWait(waitTime)
 
         if self.checkIsRunning():
-            # Start core daemon
-            self._daemonTimer.start(CORE_CHECK_ALIVE_INTERVAL)
+            if AppSettings.isStateON_('PowerSaveMode'):
+                # Power optimization
+                logger.info(f'no core daemon for {self.name()} in power save mode')
+
+                self._daemonTimer.stop()
+            else:
+                # Start core daemon
+                self._daemonTimer.start(CORE_CHECK_ALIVE_INTERVAL)
 
             return True
         else:
             return False
 
     def stop(self):
         if self.isRunning():
```

### Comparing `Furious-GUI-0.4.5/Furious/QtFramework/DNSResolver.py` & `Furious-GUI-0.4.6/Furious/QtFramework/DNSResolver.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/QtFramework/DynamicTheme.py` & `Furious-GUI-0.4.6/Furious/QtFramework/DynamicTheme.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/QtFramework/DynamicTranslate.py` & `Furious-GUI-0.4.6/Furious/QtFramework/DynamicTranslate.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/QtFramework/GuiEditorXXX.py` & `Furious-GUI-0.4.6/Furious/QtFramework/GuiEditorXXX.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/QtFramework/NetworkStateManager.py` & `Furious-GUI-0.4.6/Furious/QtFramework/NetworkStateManager.py`

 * *Files 6% similar despite different names*

```diff
@@ -101,20 +101,23 @@
         def abort(_networkReply):
             if isinstance(_networkReply, QNetworkReply):
                 _networkReply.abort()
 
         self.jobTimeoutTimer.timeout.connect(functools.partial(abort, networkReply))
         self.jobTimeoutTimer.start(NetworkStateManager.MIN_JOB_INTERVAL - 500)
 
-    def startTest(self):
-        self.jobArrangeTimer.start(NetworkStateManager.MIN_JOB_INTERVAL)
-
     def stopTest(self):
         self.jobArrangeTimer.stop()
 
     def connectedCallback(self):
-        self.jobInterval = NetworkStateManager.MIN_JOB_INTERVAL
+        if AppSettings.isStateON_('PowerSaveMode'):
+            # Power optimization
+            logger.info('no job for network state manager in power save mode')
+
+            self.jobArrangeTimer.stop()
+        else:
+            self.jobInterval = NetworkStateManager.MIN_JOB_INTERVAL
 
-        self.jobArrangeTimer.start(self.jobInterval)
+            self.jobArrangeTimer.start(self.jobInterval)
 
     def disconnectedCallback(self):
         self.jobArrangeTimer.stop()
```

### Comparing `Furious-GUI-0.4.5/Furious/QtFramework/QtGui.py` & `Furious-GUI-0.4.6/Furious/QtFramework/QtGui.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/QtFramework/QtNetwork.py` & `Furious-GUI-0.4.6/Furious/QtFramework/QtNetwork.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/QtFramework/QtWidgets.py` & `Furious-GUI-0.4.6/Furious/QtFramework/QtWidgets.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     'AppQMessageBox',
     'AppQPushButton',
     'AppQTableWidget',
     'AppQTabWidget',
     'AppQToolBar',
     'QuestionDeleteMBox',
     'NewChangesNextTimeMBox',
+    'showNewChangesNextTimeMBox',
 ]
 
 needTrans = functools.partial(needTransFn, source=__name__)
 
 
 def moveToCenter(widget, parent=None):
     geometry = widget.geometry()
@@ -588,7 +589,25 @@
 
 class NewChangesNextTimeMBox(AppQMessageBox):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self.setIcon(AppQMessageBox.Icon.Information)
         self.setText(_('New changes will take effect next time'))
+
+
+def showNewChangesNextTimeMBox(**kwargs):
+    try:
+        if APP().isSystemTrayConnected():
+            mbox = NewChangesNextTimeMBox(**kwargs)
+
+            if isinstance(mbox.parent(), QMainWindow):
+                mbox.setWindowModality(QtCore.Qt.WindowModality.WindowModal)
+            else:
+                mbox.setWindowModality(QtCore.Qt.WindowModality.ApplicationModal)
+
+            # Show the MessageBox asynchronously
+            mbox.open()
+    except Exception:
+        # Any non-exit exceptions
+
+        pass
```

### Comparing `Furious-GUI-0.4.5/Furious/QtFramework/TextEditor.py` & `Furious-GUI-0.4.6/Furious/QtFramework/TextEditor.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/QtFramework/TextEditorTheme.py` & `Furious-GUI-0.4.6/Furious/QtFramework/TextEditorTheme.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/QtFramework/UpdatesManager.py` & `Furious-GUI-0.4.6/Furious/QtFramework/UpdatesManager.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/QtFramework/__init__.py` & `Furious-GUI-0.4.6/Furious/QtFramework/__init__.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Storage/UserServers.py` & `Furious-GUI-0.4.6/Furious/Storage/UserServers.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Storage/UserSubs.py` & `Furious-GUI-0.4.6/Furious/Storage/UserSubs.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Storage/__init__.py` & `Furious-GUI-0.4.6/Furious/Storage/__init__.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/TrayActions/Connect.py` & `Furious-GUI-0.4.6/Furious/TrayActions/Connect.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/TrayActions/EditConfiguration.py` & `Furious-GUI-0.4.6/Furious/TrayActions/EditConfiguration.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/TrayActions/Exit.py` & `Furious-GUI-0.4.6/Furious/TrayActions/Exit.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/TrayActions/Import.py` & `Furious-GUI-0.4.6/Furious/TrayActions/Import.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/TrayActions/Language.py` & `Furious-GUI-0.4.6/Furious/TrayActions/Language.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/TrayActions/Routing.py` & `Furious-GUI-0.4.6/Furious/TrayActions/Routing.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/TrayActions/Settings.py` & `Furious-GUI-0.4.6/Furious/TrayActions/Settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,20 +23,21 @@
 
 import functools
 
 __all__ = ['SettingsAction']
 
 registerAppSettings('VPNMode', isBinary=True)
 registerAppSettings('DarkMode', isBinary=True)
+registerAppSettings('UseMonochromeTrayIcon', isBinary=True)
 registerAppSettings('StartupOnBoot', isBinary=True, default=BinarySettings.ON_)
+registerAppSettings('PowerSaveMode', isBinary=True)
 registerAppSettings(
     'ShowProgressBarWhenConnecting', isBinary=True, default=BinarySettings.ON_
 )
 registerAppSettings('ShowTabAndSpacesInEditor', isBinary=True)
-registerAppSettings('UseMonochromeTrayIcon', isBinary=True)
 
 needTrans = functools.partial(needTransFn, source=__name__)
 
 needTrans(
     'VPN Mode',
     'VPN Mode Disabled (Administrator)',
     'VPN Mode Disabled (root)',
@@ -56,24 +57,15 @@
         assert isAdministrator()
 
         if checked:
             AppSettings.turnON_('VPNMode')
         else:
             AppSettings.turnOFF('VPNMode')
 
-        try:
-            if APP().isSystemTrayConnected():
-                mbox = NewChangesNextTimeMBox()
-
-                # Show the MessageBox asynchronously
-                mbox.open()
-        except Exception:
-            # Any non-exit exceptions
-
-            pass
+        showNewChangesNextTimeMBox()
 
 
 class SettingsChildAction(AppQAction):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def triggeredCallback(self, checked):
@@ -93,59 +85,67 @@
 
                 try:
                     APP().switchToAutoMode()
                 except Exception:
                     # Any non-exit exceptions
 
                     pass
-        if self.textCompare('Startup On Boot'):
+        elif self.textCompare('Use Monochrome Tray Icon'):
+            # Settings turn on/off order matters here
+            if checked:
+                AppSettings.turnON_('UseMonochromeTrayIcon')
+
+                APP().systemTray.setMonochromeIcon()
+            else:
+                AppSettings.turnOFF('UseMonochromeTrayIcon')
+
+                if APP().isSystemTrayConnected():
+                    APP().systemTray.setConnectedIcon()
+                else:
+                    APP().systemTray.setDisconnectedIcon()
+        elif self.textCompare('Startup On Boot'):
             if checked:
                 StartupOnBoot.on_()
 
                 AppSettings.turnON_('StartupOnBoot')
             else:
                 StartupOnBoot.off()
 
                 AppSettings.turnOFF('StartupOnBoot')
-        if self.textCompare('Show Progress Bar When Connecting'):
+        elif self.textCompare('Power Save Mode'):
+            if checked:
+                AppSettings.turnON_('PowerSaveMode')
+            else:
+                AppSettings.turnOFF('PowerSaveMode')
+
+            showNewChangesNextTimeMBox()
+        elif self.textCompare('Show Progress Bar When Connecting'):
             if checked:
                 AppSettings.turnON_('ShowProgressBarWhenConnecting')
             else:
                 AppSettings.turnOFF('ShowProgressBarWhenConnecting')
-        if self.textCompare('Show Tab And Spaces In Editor'):
+        elif self.textCompare('Show Tab And Spaces In Editor'):
             if checked:
                 APP().mainWindow.showTabAndSpaces()
 
                 AppSettings.turnON_('ShowTabAndSpacesInEditor')
             else:
                 APP().mainWindow.hideTabAndSpaces()
 
                 AppSettings.turnOFF('ShowTabAndSpacesInEditor')
-        if self.textCompare('Use Monochrome Tray Icon'):
-            # Settings turn on/off order matters here
-            if checked:
-                AppSettings.turnON_('UseMonochromeTrayIcon')
-
-                APP().systemTray.setMonochromeIcon()
-            else:
-                AppSettings.turnOFF('UseMonochromeTrayIcon')
-
-                if APP().isSystemTrayConnected():
-                    APP().systemTray.setConnectedIcon()
-                else:
-                    APP().systemTray.setDisconnectedIcon()
 
 
 needTrans(
     'Settings',
     'Dark Mode',
+    'Use Monochrome Tray Icon',
     'Startup On Boot',
+    'Power Save Mode',
     'Show Progress Bar When Connecting',
     'Show Tab And Spaces In Editor',
-    'Use Monochrome Tray Icon',
 )
 
 
 class SettingsAction(AppQAction):
     def __init__(self, **kwargs):
         if PLATFORM == 'Windows' or PLATFORM == 'Darwin':
             extraActions = [
@@ -169,20 +169,27 @@
                     checked=AppSettings.isStateON_('DarkMode'),
                 ),
                 SettingsChildAction(
                     _('Use Monochrome Tray Icon'),
                     checkable=True,
                     checked=AppSettings.isStateON_('UseMonochromeTrayIcon'),
                 ),
+                AppQSeperator(),
                 SettingsChildAction(
                     _('Startup On Boot'),
                     checkable=True,
                     checked=AppSettings.isStateON_('StartupOnBoot'),
                 ),
                 SettingsChildAction(
+                    _('Power Save Mode'),
+                    checkable=True,
+                    checked=AppSettings.isStateON_('PowerSaveMode'),
+                ),
+                AppQSeperator(),
+                SettingsChildAction(
                     _('Show Progress Bar When Connecting'),
                     checkable=True,
                     checked=AppSettings.isStateON_('ShowProgressBarWhenConnecting'),
                 ),
                 SettingsChildAction(
                     _('Show Tab And Spaces In Editor'),
                     checkable=True,
```

### Comparing `Furious-GUI-0.4.5/Furious/TrayActions/SystemProxy.py` & `Furious-GUI-0.4.6/Furious/TrayActions/SystemProxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 class SystemProxyChildAction(AppQAction):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def triggeredCallback(self, checked):
         if self.textCompare('Automatically Configure System Proxy'):
             AppSettings.set('SystemProxyMode', 'Auto')
-        if self.textCompare('Do Not Change System Proxy'):
+        elif self.textCompare('Do Not Change System Proxy'):
             AppSettings.set('SystemProxyMode', 'NoChanges')
 
 
 needTrans(
     'System Proxy',
     'Automatically Configure System Proxy',
     'Do Not Change System Proxy',
```

### Comparing `Furious-GUI-0.4.5/Furious/TrayActions/__init__.py` & `Furious-GUI-0.4.6/Furious/TrayActions/__init__.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Utility/AppMainProcess.py` & `Furious-GUI-0.4.6/Furious/Utility/AppMainProcess.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Utility/AppResources.py` & `Furious-GUI-0.4.6/Furious/Utility/AppResources.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Utility/AppSettings.py` & `Furious-GUI-0.4.6/Furious/Utility/AppSettings.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Utility/AppSettingsFn.py` & `Furious-GUI-0.4.6/Furious/Utility/AppSettingsFn.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Utility/Constants.py` & `Furious-GUI-0.4.6/Furious/Utility/Constants.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Utility/PySide6Legacy.py` & `Furious-GUI-0.4.6/Furious/Utility/PySide6Legacy.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Utility/StartupOnBoot.py` & `Furious-GUI-0.4.6/Furious/Utility/StartupOnBoot.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Utility/SystemProxy.py` & `Furious-GUI-0.4.6/Furious/Utility/SystemProxy.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Utility/SystemRoutingTable.py` & `Furious-GUI-0.4.6/Furious/Utility/SystemRoutingTable.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Utility/SystemRuntime.py` & `Furious-GUI-0.4.6/Furious/Utility/SystemRuntime.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Utility/Utility.py` & `Furious-GUI-0.4.6/Furious/Utility/Utility.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Utility/__init__.py` & `Furious-GUI-0.4.6/Furious/Utility/__init__.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Version.py` & `Furious-GUI-0.4.6/Furious/Version.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-__version__ = '0.4.5'
+__version__ = '0.4.6'
```

### Comparing `Furious-GUI-0.4.5/Furious/Widget/Application.py` & `Furious-GUI-0.4.6/Furious/Widget/Application.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Widget/ConnectProgressBar.py` & `Furious-GUI-0.4.6/Furious/Widget/ConnectProgressBar.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Widget/GuiHysteria1.py` & `Furious-GUI-0.4.6/Furious/Widget/GuiHysteria1.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Widget/GuiHysteria2.py` & `Furious-GUI-0.4.6/Furious/Widget/GuiHysteria2.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Widget/GuiShadowsocks.py` & `Furious-GUI-0.4.6/Furious/Widget/GuiShadowsocks.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Widget/GuiTrojan.py` & `Furious-GUI-0.4.6/Furious/Widget/GuiTrojan.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Widget/GuiVLESS.py` & `Furious-GUI-0.4.6/Furious/Widget/GuiVLESS.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Widget/GuiVMess.py` & `Furious-GUI-0.4.6/Furious/Widget/GuiVMess.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Widget/GuiVTLS.py` & `Furious-GUI-0.4.6/Furious/Widget/GuiVTLS.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Widget/GuiVTransport.py` & `Furious-GUI-0.4.6/Furious/Widget/GuiVTransport.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Widget/IndentSpinBox.py` & `Furious-GUI-0.4.6/Furious/Widget/IndentSpinBox.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Widget/SystemTrayIcon.py` & `Furious-GUI-0.4.6/Furious/Widget/SystemTrayIcon.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Widget/UserServersQTableWidget.py` & `Furious-GUI-0.4.6/Furious/Widget/UserServersQTableWidget.py`

 * *Files 1% similar despite different names*

```diff
@@ -961,24 +961,15 @@
 
         modified = editor.inputToFactory(factory)
 
         # Still flush to row since remark may be modified
         self.flushRow(index, factory)
 
         if modified and index == AS_UserActivatedItemIndex():
-            try:
-                if APP().isSystemTrayConnected():
-                    mbox = NewChangesNextTimeMBox()
-
-                    # Show the MessageBox asynchronously
-                    mbox.open()
-            except Exception:
-                # Any non-exit exceptions
-
-                pass
+            showNewChangesNextTimeMBox()
 
         editor.accepted.disconnect()
         editor.rejected.disconnect()
 
     def handleGuiEditorRejected(self, editor: GuiEditorWidgetQDialog):
         editor.accepted.disconnect()
         editor.rejected.disconnect()
@@ -1277,15 +1268,24 @@
 
         def handleResultCode(_indexes, code):
             if code == PySide6LegacyEnumValueWrapper(AppQMessageBox.StandardButton.Yes):
                 self.deleteItemByIndex(_indexes)
             else:
                 pass
 
-        mbox = QuestionDeleteMBox(icon=AppQMessageBox.Icon.Question)
+        if PLATFORM == 'Windows':
+            # Windows
+            mbox = QuestionDeleteMBox(icon=AppQMessageBox.Icon.Question)
+        else:
+            # macOS & linux
+            mbox = QuestionDeleteMBox(
+                icon=AppQMessageBox.Icon.Question, parent=self.parent()
+            )
+            mbox.setWindowModality(QtCore.Qt.WindowModality.WindowModal)
+
         mbox.isMulti = bool(len(indexes) > 1)
         mbox.possibleRemark = f'{indexes[0] + 1} - {self.item(indexes[0], 0).text()}'
         mbox.setText(mbox.customText())
         mbox.finished.connect(functools.partial(handleResultCode, indexes))
 
         # dummy ref
         setattr(self, '_questionDeleteMBox', mbox)
```

### Comparing `Furious-GUI-0.4.5/Furious/Widget/UserSubsQTableWidget.py` & `Furious-GUI-0.4.6/Furious/Widget/UserSubsQTableWidget.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Widget/XrayAssetViewerQListWidget.py` & `Furious-GUI-0.4.6/Furious/Widget/XrayAssetViewerQListWidget.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,19 +19,21 @@
 
 from Furious.PyFramework import *
 from Furious.QtFramework import *
 from Furious.QtFramework import gettext as _
 from Furious.Utility import *
 
 from PySide6 import QtCore
+from PySide6.QtGui import *
 from PySide6.QtWidgets import *
 
 import os
 import shutil
 import logging
+import datetime
 import functools
 import darkdetect
 
 __all__ = ['XrayAssetViewerQListWidget']
 
 logger = logging.getLogger(__name__)
 
@@ -99,17 +101,36 @@
     @QtCore.Slot(QtCore.QPoint)
     def handleCustomContextMenuRequested(self, point):
         self.contextMenu.exec(self.mapToGlobal(point))
 
     def flushItemByTheme(self, theme: str):
         self.clear()
 
+        maxlen = max(
+            len(filename)
+            for filename in os.listdir(XRAY_ASSET_DIR)
+            if os.path.isfile(XRAY_ASSET_DIR / filename)
+        )
+
         for filename in os.listdir(XRAY_ASSET_DIR):
             if os.path.isfile(XRAY_ASSET_DIR / filename):
-                item = QListWidgetItem(filename)
+                try:
+                    # Exception may be raised
+                    epoch = os.path.getmtime(XRAY_ASSET_DIR / filename)
+                except Exception:
+                    # Any non-exit exceptions
+
+                    mdate = ''
+                else:
+                    mdate = datetime.datetime.fromtimestamp(epoch).strftime(
+                        '%Y-%m-%d %H:%M:%S'
+                    )
+
+                item = QListWidgetItem(f'{filename:{maxlen + 6}}{mdate}')
+                item.setFont(QFont(APP().customFontName))
 
                 if AppSettings.isStateON_('DarkMode'):
                     # Custom dark mode
                     item.setIcon(bootstrapIconWhite('file-earmark.svg'))
                 else:
                     if theme == 'Dark':
                         if PLATFORM == 'Windows':
@@ -198,15 +219,24 @@
                     os.remove(XRAY_ASSET_DIR / self.item(index).text())
 
                 self.flushItem()
             else:
                 # Do not delete
                 pass
 
-        mbox = QuestionDeleteMBox(icon=AppQMessageBox.Icon.Question)
+        if PLATFORM == 'Windows':
+            # Windows
+            mbox = QuestionDeleteMBox(icon=AppQMessageBox.Icon.Question)
+        else:
+            # macOS & linux
+            mbox = QuestionDeleteMBox(
+                icon=AppQMessageBox.Icon.Question, parent=self.parent()
+            )
+            mbox.setWindowModality(QtCore.Qt.WindowModality.WindowModal)
+
         mbox.isMulti = bool(len(indexes) > 1)
         mbox.possibleRemark = f'{self.item(indexes[0]).text()}'
         mbox.setText(mbox.customText())
         mbox.finished.connect(functools.partial(handleResultCode, indexes))
 
         # dummy ref
         setattr(self, '_questionDeleteMBox', mbox)
```

### Comparing `Furious-GUI-0.4.5/Furious/Widget/__init__.py` & `Furious-GUI-0.4.6/Furious/Widget/__init__.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Window/AppMainWindow.py` & `Furious-GUI-0.4.6/Furious/Window/AppMainWindow.py`

 * *Files 0% similar despite different names*

```diff
@@ -392,16 +392,14 @@
         # TODO: Custom status tip
         # self.setStatusBar(QStatusBar(self))
 
         self.networkState = AppQLabel(translatable=False)
 
         self.statusBar().addPermanentWidget(self.networkState)
 
-        self.networkStateManager.startTest()
-
         self._widget = QWidget()
         self._layout = QVBoxLayout(self._widget)
         self._layout.addWidget(self.mainTab)
 
         self.setCentralWidget(self._widget)
 
     def appendNewItemByFactory(self, factory: ConfigurationFactory):
```

### Comparing `Furious-GUI-0.4.5/Furious/Window/LogViewerWindow.py` & `Furious-GUI-0.4.6/Furious/Window/LogViewerWindow.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Window/QRCodeWindow.py` & `Furious-GUI-0.4.6/Furious/Window/QRCodeWindow.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Window/TextEditorWindow.py` & `Furious-GUI-0.4.6/Furious/Window/TextEditorWindow.py`

 * *Files 2% similar despite different names*

```diff
@@ -343,25 +343,15 @@
                 APP().mainWindow.flushRow(index, new)
             except Exception:
                 # Any non-exit exceptions
 
                 pass
 
             if index == AS_UserActivatedItemIndex():
-                try:
-                    if APP().isSystemTrayConnected():
-                        mbox = NewChangesNextTimeMBox(parent=self)
-                        mbox.setWindowModality(QtCore.Qt.WindowModality.WindowModal)
-
-                        # Show the MessageBox asynchronously
-                        mbox.open()
-                except Exception:
-                    # Any non-exit exceptions
-
-                    pass
+                showNewChangesNextTimeMBox(parent=self)
 
             self.markAsSaved()
 
             return True
 
     def saveAsFile(self):
         filename, selectedFilter = QFileDialog.getSaveFileName(
```

### Comparing `Furious-GUI-0.4.5/Furious/Window/UserSubsWindow.py` & `Furious-GUI-0.4.6/Furious/Window/UserSubsWindow.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/Window/XrayAssetViewerWindow.py` & `Furious-GUI-0.4.6/Furious/Window/XrayAssetViewerWindow.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,35 +50,43 @@
 
 class XrayAssetViewerWindow(AppQMainWindow):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self.setWindowTitle(_('Xray-core Asset File'))
 
-        self.xrayAssetViewerWidget = XrayAssetViewerQListWidget()
+        self.xrayAssetViewerWidget = XrayAssetViewerQListWidget(parent=self)
         self.setCentralWidget(self.xrayAssetViewerWidget)
 
+        if versionToValue(PYSIDE6_VERSION) <= versionToValue('6.1.3'):
+            openAssetDirectoryActions = [None]
+        else:
+            # openUrl will crash on PySide6 6.1.3, probably a Qt bug
+            openAssetDirectoryActions = [
+                AppQAction(
+                    _('Open Asset Directory'),
+                    callback=lambda: self.openAssetDirectory(),
+                    shortcut=QtCore.QKeyCombination(
+                        QtCore.Qt.KeyboardModifier.ControlModifier,
+                        QtCore.Qt.Key.Key_O,
+                    ),
+                ),
+            ]
+
         self.fileMenu = AppQMenu(
             AppQAction(
                 _('Refresh'),
                 callback=lambda: self.flushItem(),
                 shortcut=QtCore.QKeyCombination(
                     QtCore.Qt.KeyboardModifier.ControlModifier,
                     QtCore.Qt.Key.Key_R,
                 ),
             ),
             AppQSeperator(),
-            AppQAction(
-                _('Open Asset Directory'),
-                callback=lambda: self.openAssetDirectory(),
-                shortcut=QtCore.QKeyCombination(
-                    QtCore.Qt.KeyboardModifier.ControlModifier,
-                    QtCore.Qt.Key.Key_O,
-                ),
-            ),
+            *openAssetDirectoryActions,
             AppQAction(
                 _('Import From File...'),
                 callback=lambda: self.appendNewItem(),
             ),
             AppQSeperator(),
             AppQAction(
                 _('Exit'),
```

### Comparing `Furious-GUI-0.4.5/Furious/Window/__init__.py` & `Furious-GUI-0.4.6/Furious/Window/__init__.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/__init__.py` & `Furious-GUI-0.4.6/Furious/__init__.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious/__main__.py` & `Furious-GUI-0.4.6/Furious/__main__.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious_GUI.egg-info/PKG-INFO` & `Furious-GUI-0.4.6/Furious_GUI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Furious-GUI
-Version: 0.4.5
+Version: 0.4.6
 Summary: A GUI proxy client based on PySide6. Support Xray-core & hysteria
 Home-page: https://github.com/LorenEteval/Furious
 Author: Loren Eteval
 Author-email: loren.eteval@proton.me
 License: GPL v3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `Furious-GUI-0.4.5/Furious_GUI.egg-info/SOURCES.txt` & `Furious-GUI-0.4.6/Furious_GUI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/Furious_GUI.egg-info/requires.txt` & `Furious-GUI-0.4.6/Furious_GUI.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/LICENSE` & `Furious-GUI-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/PKG-INFO` & `Furious-GUI-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Furious-GUI
-Version: 0.4.5
+Version: 0.4.6
 Summary: A GUI proxy client based on PySide6. Support Xray-core & hysteria
 Home-page: https://github.com/LorenEteval/Furious
 Author: Loren Eteval
 Author-email: loren.eteval@proton.me
 License: GPL v3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `Furious-GUI-0.4.5/README.md` & `Furious-GUI-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.4.5/setup.py` & `Furious-GUI-0.4.6/setup.py`

 * *Files identical despite different names*

