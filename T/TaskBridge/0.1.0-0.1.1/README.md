# Comparing `tmp/taskbridge-0.1.0.tar.gz` & `tmp/taskbridge-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskbridge-0.1.0.tar", max compression
+gzip compressed data, was "taskbridge-0.1.1.tar", max compression
```

## Comparing `taskbridge-0.1.0.tar` & `taskbridge-0.1.1.tar`

### file list

```diff
@@ -1,111 +1,111 @@
--rw-r--r--   0        0        0    35128 2024-05-28 10:12:50.913347 taskbridge-0.1.0/LICENSE
--rw-r--r--   0        0        0     7544 2024-05-28 11:13:13.824350 taskbridge-0.1.0/README.md
--rw-r--r--   0        0        0     1695 2024-05-28 10:12:50.936770 taskbridge-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      348 2024-05-28 10:12:50.937351 taskbridge-0.1.0/taskbridge/__init__.py
--rw-r--r--   0        0        0      138 2024-05-28 11:04:48.375560 taskbridge-0.1.0/taskbridge/cli/__init__.py
--rw-r--r--   0        0        0    19064 2024-05-28 11:06:15.575002 taskbridge-0.1.0/taskbridge/cli/tbcli.py
--rw-r--r--   0        0        0      680 2024-05-28 10:12:50.938068 taskbridge-0.1.0/taskbridge/gui/TaskBridge.py
--rw-r--r--   0        0        0      429 2024-05-28 11:04:04.016939 taskbridge-0.1.0/taskbridge/gui/__init__.py
--rw-r--r--   0        0        0     2839 2024-05-28 10:12:50.938560 taskbridge-0.1.0/taskbridge/gui/about.ui
--rw-r--r--   0        0        0    13473 2024-05-28 10:12:50.938821 taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/100.png
--rw-r--r--   0        0        0    13805 2024-05-28 10:12:50.939034 taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/102.png
--rw-r--r--   0        0        0   772414 2024-05-28 10:12:50.940652 taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/1024.png
--rw-r--r--   0        0        0    16622 2024-05-28 10:12:50.940972 taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/114.png
--rw-r--r--   0        0        0    17860 2024-05-28 10:12:50.941209 taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/120.png
--rw-r--r--   0        0        0    19866 2024-05-28 10:12:50.941528 taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/128.png
--rw-r--r--   0        0        0    23814 2024-05-28 10:12:50.941837 taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/144.png
--rw-r--r--   0        0        0    25818 2024-05-28 10:12:50.942007 taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/152.png
--rw-r--r--   0        0        0      822 2024-05-28 10:12:50.942220 taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/16.png
--rw-r--r--   0        0        0    30211 2024-05-28 10:12:50.942564 taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/167.png
--rw-r--r--   0        0        0    31652 2024-05-28 10:12:50.942909 taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/172.png
--rw-r--r--   0        0        0    34032 2024-05-28 10:12:50.943391 taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/180.png
--rw-r--r--   0        0        0    39070 2024-05-28 10:12:50.943886 taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/196.png
--rw-r--r--   0        0        0     1104 2024-05-28 10:12:50.944119 taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/20.png
--rw-r--r--   0        0        0    45736 2024-05-28 10:12:50.944656 taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/216.png
--rw-r--r--   0        0        0    60912 2024-05-28 10:12:50.945186 taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/256.png
--rw-r--r--   0        0        0     1922 2024-05-28 10:12:50.945387 taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/29.png
--rw-r--r--   0        0        0     2235 2024-05-28 10:12:50.945681 taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/32.png
--rw-r--r--   0        0        0     3180 2024-05-28 10:12:50.945872 taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/40.png
--rw-r--r--   0        0        0     4265 2024-05-28 10:12:50.946089 taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/48.png
--rw-r--r--   0        0        0     4543 2024-05-28 10:12:50.946359 taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/50.png
--rw-r--r--   0        0        0   206946 2024-05-28 10:12:50.950422 taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/512.png
--rw-r--r--   0        0        0     5252 2024-05-28 10:12:50.950722 taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/55.png
--rw-r--r--   0        0        0     5549 2024-05-28 10:12:50.951020 taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/57.png
--rw-r--r--   0        0        0     5649 2024-05-28 10:12:50.951179 taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/58.png
--rw-r--r--   0        0        0     5983 2024-05-28 10:12:50.951413 taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/60.png
--rw-r--r--   0        0        0     6583 2024-05-28 10:12:50.951648 taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/64.png
--rw-r--r--   0        0        0     6988 2024-05-28 10:12:50.951770 taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/66.png
--rw-r--r--   0        0        0     7993 2024-05-28 10:12:50.951890 taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/72.png
--rw-r--r--   0        0        0     8732 2024-05-28 10:12:50.952196 taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/76.png
--rw-r--r--   0        0        0     9417 2024-05-28 10:12:50.952599 taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/80.png
--rw-r--r--   0        0        0    10705 2024-05-28 10:12:50.952918 taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/87.png
--rw-r--r--   0        0        0    10894 2024-05-28 10:12:50.953132 taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/88.png
--rw-r--r--   0        0        0    11674 2024-05-28 10:12:50.953339 taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/92.png
--rw-r--r--   0        0        0     7139 2024-05-28 10:12:50.953567 taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/Contents.json
--rw-r--r--   0        0        0   772414 2024-05-28 10:12:50.954162 taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/appstore.png
--rw-r--r--   0        0        0   214701 2024-05-28 10:12:50.955002 taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/playstore.png
--rw-r--r--   0        0        0   998221 2024-05-28 10:12:50.957694 taskbridge-0.1.0/taskbridge/gui/assets/TaskBridge.icns
--rw-r--r--   0        0        0    17569 2024-05-28 10:12:50.958192 taskbridge-0.1.0/taskbridge/gui/assets/TaskBridge.iconset/icon_128x128.png
--rw-r--r--   0        0        0    50656 2024-05-28 10:12:50.958847 taskbridge-0.1.0/taskbridge/gui/assets/TaskBridge.iconset/icon_128x128@2x.png
--rw-r--r--   0        0        0     1699 2024-05-28 10:12:50.959128 taskbridge-0.1.0/taskbridge/gui/assets/TaskBridge.iconset/icon_16x16.png
--rw-r--r--   0        0        0     2759 2024-05-28 10:12:50.959494 taskbridge-0.1.0/taskbridge/gui/assets/TaskBridge.iconset/icon_16x16@2x.png
--rw-r--r--   0        0        0    50655 2024-05-28 10:12:50.960206 taskbridge-0.1.0/taskbridge/gui/assets/TaskBridge.iconset/icon_256x256.png
--rw-r--r--   0        0        0   159642 2024-05-28 10:12:50.961211 taskbridge-0.1.0/taskbridge/gui/assets/TaskBridge.iconset/icon_256x256@2x.png
--rw-r--r--   0        0        0     2759 2024-05-28 10:12:50.961450 taskbridge-0.1.0/taskbridge/gui/assets/TaskBridge.iconset/icon_32x32.png
--rw-r--r--   0        0        0     6510 2024-05-28 10:12:50.961765 taskbridge-0.1.0/taskbridge/gui/assets/TaskBridge.iconset/icon_32x32@2x.png
--rw-r--r--   0        0        0   159641 2024-05-28 10:12:50.962802 taskbridge-0.1.0/taskbridge/gui/assets/TaskBridge.iconset/icon_512x512.png
--rw-r--r--   0        0        0   551167 2024-05-28 10:12:50.964524 taskbridge-0.1.0/taskbridge/gui/assets/TaskBridge.iconset/icon_512x512@2x.png
--rw-r--r--   0        0        0   931253 2024-05-28 10:12:50.968883 taskbridge-0.1.0/taskbridge/gui/assets/source/TaskBridge_Icon.xcf
--rw-r--r--   0        0        0    69368 2024-05-28 10:12:50.971236 taskbridge-0.1.0/taskbridge/gui/assets/source/bridge.xcf
--rw-r--r--   0        0        0   658861 2024-05-28 10:12:50.972885 taskbridge-0.1.0/taskbridge/gui/assets/source/bridge_animated_black.xcf
--rw-r--r--   0        0        0    63732 2024-05-28 10:12:50.973309 taskbridge-0.1.0/taskbridge/gui/assets/source/bridge_animated_optimised.xcf
--rw-r--r--   0        0        0  1156034 2024-05-28 10:12:50.975394 taskbridge-0.1.0/taskbridge/gui/assets/source/bridge_animated_white.xcf
--rw-r--r--   0        0        0     3862 2024-05-28 10:12:50.975704 taskbridge-0.1.0/taskbridge/gui/assets/source/ios-arrow-round-up-7-512.png
--rw-r--r--   0        0        0     5539 2024-05-28 10:12:50.975944 taskbridge-0.1.0/taskbridge/gui/assets/source/ios-swap-7-512.png
--rw-r--r--   0        0        0     8361 2024-05-28 10:12:50.976299 taskbridge-0.1.0/taskbridge/gui/assets/source/local.png
--rw-r--r--   0        0        0     2197 2024-05-28 10:12:50.976549 taskbridge-0.1.0/taskbridge/gui/assets/source/local_and_remote_black.xcf
--rw-r--r--   0        0        0     3294 2024-05-28 10:12:50.976763 taskbridge-0.1.0/taskbridge/gui/assets/source/local_and_remote_white.xcf
--rw-r--r--   0        0        0    18816 2024-05-28 10:12:50.977106 taskbridge-0.1.0/taskbridge/gui/assets/source/remote.png
--rw-r--r--   0        0        0     1301 2024-05-28 10:12:50.977370 taskbridge-0.1.0/taskbridge/gui/assets/table/bidirectional_black.png
--rw-r--r--   0        0        0     1301 2024-05-28 10:12:50.977572 taskbridge-0.1.0/taskbridge/gui/assets/table/bidirectional_white.png
--rw-r--r--   0        0        0     1591 2024-05-28 10:12:50.977789 taskbridge-0.1.0/taskbridge/gui/assets/table/local_and_remote_black.png
--rw-r--r--   0        0        0     1686 2024-05-28 10:12:50.978040 taskbridge-0.1.0/taskbridge/gui/assets/table/local_and_remote_white.png
--rw-r--r--   0        0        0      965 2024-05-28 10:12:50.978308 taskbridge-0.1.0/taskbridge/gui/assets/table/local_black.png
--rw-r--r--   0        0        0     1950 2024-05-28 10:12:50.978538 taskbridge-0.1.0/taskbridge/gui/assets/table/local_to_remote_black.png
--rw-r--r--   0        0        0     1955 2024-05-28 10:12:50.978765 taskbridge-0.1.0/taskbridge/gui/assets/table/local_to_remote_white.png
--rw-r--r--   0        0        0      990 2024-05-28 10:12:50.979082 taskbridge-0.1.0/taskbridge/gui/assets/table/local_white.png
--rw-r--r--   0        0        0     1266 2024-05-28 10:12:50.979320 taskbridge-0.1.0/taskbridge/gui/assets/table/remote_black.png
--rw-r--r--   0        0        0     2885 2024-05-28 10:12:50.979551 taskbridge-0.1.0/taskbridge/gui/assets/table/remote_to_local_black.png
--rw-r--r--   0        0        0     2847 2024-05-28 10:12:50.979755 taskbridge-0.1.0/taskbridge/gui/assets/table/remote_to_local_white.png
--rw-r--r--   0        0        0     1290 2024-05-28 10:12:50.979981 taskbridge-0.1.0/taskbridge/gui/assets/table/remote_white.png
--rw-r--r--   0        0        0    17458 2024-05-28 10:12:50.980399 taskbridge-0.1.0/taskbridge/gui/assets/tray/bridge_animated_black.gif
--rw-r--r--   0        0        0    17522 2024-05-28 10:12:50.980793 taskbridge-0.1.0/taskbridge/gui/assets/tray/bridge_animated_white.gif
--rw-r--r--   0        0        0    47984 2024-05-28 10:12:50.981403 taskbridge-0.1.0/taskbridge/gui/assets/tray/bridge_black.png
--rw-r--r--   0        0        0    11350 2024-05-28 10:12:50.981753 taskbridge-0.1.0/taskbridge/gui/assets/tray/bridge_white.png
--rw-r--r--   0        0        0   387868 2024-05-28 10:12:50.983237 taskbridge-0.1.0/taskbridge/gui/assets/ui/TaskBridge.png
--rw-r--r--   0        0        0     4909 2024-05-28 10:12:50.983497 taskbridge-0.1.0/taskbridge/gui/assets/ui/refresh.png
--rw-r--r--   0        0        0     3701 2024-05-28 10:12:50.985394 taskbridge-0.1.0/taskbridge/gui/assets/ui/trash.png
--rw-r--r--   0        0        0    29098 2024-05-28 10:12:50.985662 taskbridge-0.1.0/taskbridge/gui/taskbridge.ui
--rw-r--r--   0        0        0      908 2024-05-28 10:12:50.985936 taskbridge-0.1.0/taskbridge/gui/viewmodel/__init__.py
--rw-r--r--   0        0        0      476 2024-05-28 10:12:50.986140 taskbridge-0.1.0/taskbridge/gui/viewmodel/mainwindow.py
--rw-r--r--   0        0        0     2703 2024-05-28 10:12:50.986369 taskbridge-0.1.0/taskbridge/gui/viewmodel/notecheckbox.py
--rw-r--r--   0        0        0     1918 2024-05-28 10:12:50.986595 taskbridge-0.1.0/taskbridge/gui/viewmodel/remindercheckbox.py
--rw-r--r--   0        0        0    45804 2024-05-28 10:12:50.986875 taskbridge-0.1.0/taskbridge/gui/viewmodel/taskbridgeapp.py
--rw-r--r--   0        0        0    13063 2024-05-28 10:12:50.987144 taskbridge-0.1.0/taskbridge/gui/viewmodel/threadedtasks.py
--rw-r--r--   0        0        0     1771 2024-05-28 10:12:50.987467 taskbridge-0.1.0/taskbridge/gui/viewmodel/trayicon.py
--rw-r--r--   0        0        0     3201 2024-05-28 10:12:50.987796 taskbridge-0.1.0/taskbridge/gui/viewmodel/ui_aboutwindow.py
--rw-r--r--   0        0        0    32872 2024-05-28 10:12:50.989411 taskbridge-0.1.0/taskbridge/gui/viewmodel/ui_mainwindow.py
--rw-r--r--   0        0        0     5496 2024-05-28 10:56:54.707655 taskbridge-0.1.0/taskbridge/helpers.py
--rw-r--r--   0        0        0      570 2024-05-28 10:12:50.989907 taskbridge-0.1.0/taskbridge/notes/__init__.py
--rw-r--r--   0        0        0     7391 2024-05-28 10:12:50.990114 taskbridge-0.1.0/taskbridge/notes/controller.py
--rw-r--r--   0        0        0      572 2024-05-28 10:58:25.084166 taskbridge-0.1.0/taskbridge/notes/model/__init__.py
--rw-r--r--   0        0        0    19383 2024-05-28 10:59:05.331708 taskbridge-0.1.0/taskbridge/notes/model/note.py
--rw-r--r--   0        0        0    43723 2024-05-28 10:12:50.991327 taskbridge-0.1.0/taskbridge/notes/model/notefolder.py
--rw-r--r--   0        0        0     6063 2024-05-28 10:12:50.991477 taskbridge-0.1.0/taskbridge/notes/model/notescript.py
--rw-r--r--   0        0        0      651 2024-05-28 10:59:05.329335 taskbridge-0.1.0/taskbridge/reminders/__init__.py
--rw-r--r--   0        0        0    10528 2024-05-28 10:12:50.991927 taskbridge-0.1.0/taskbridge/reminders/controller.py
--rw-r--r--   0        0        0      755 2024-05-28 10:12:50.992162 taskbridge-0.1.0/taskbridge/reminders/model/__init__.py
--rw-r--r--   0        0        0    16131 2024-05-28 10:12:50.992407 taskbridge-0.1.0/taskbridge/reminders/model/reminder.py
--rw-r--r--   0        0        0    47638 2024-05-28 10:12:50.992686 taskbridge-0.1.0/taskbridge/reminders/model/remindercontainer.py
--rw-r--r--   0        0        0     4942 2024-05-28 10:12:50.992846 taskbridge-0.1.0/taskbridge/reminders/model/reminderscript.py
--rw-r--r--   0        0        0     8969 1970-01-01 00:00:00.000000 taskbridge-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35128 2024-05-28 10:12:50.913347 taskbridge-0.1.1/LICENSE
+-rw-r--r--   0        0        0     7735 2024-05-28 11:55:55.707692 taskbridge-0.1.1/README.md
+-rw-r--r--   0        0        0     1694 2024-05-28 11:59:55.664499 taskbridge-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      348 2024-05-28 10:12:50.937351 taskbridge-0.1.1/taskbridge/__init__.py
+-rw-r--r--   0        0        0      138 2024-05-28 11:04:48.375560 taskbridge-0.1.1/taskbridge/cli/__init__.py
+-rw-r--r--   0        0        0    19064 2024-05-28 11:06:15.575002 taskbridge-0.1.1/taskbridge/cli/tbcli.py
+-rw-r--r--   0        0        0      680 2024-05-28 10:12:50.938068 taskbridge-0.1.1/taskbridge/gui/TaskBridge.py
+-rw-r--r--   0        0        0      429 2024-05-28 11:04:04.016939 taskbridge-0.1.1/taskbridge/gui/__init__.py
+-rw-r--r--   0        0        0     2839 2024-05-28 10:12:50.938560 taskbridge-0.1.1/taskbridge/gui/about.ui
+-rw-r--r--   0        0        0    13473 2024-05-28 10:12:50.938821 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/100.png
+-rw-r--r--   0        0        0    13805 2024-05-28 10:12:50.939034 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/102.png
+-rw-r--r--   0        0        0   772414 2024-05-28 10:12:50.940652 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/1024.png
+-rw-r--r--   0        0        0    16622 2024-05-28 10:12:50.940972 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/114.png
+-rw-r--r--   0        0        0    17860 2024-05-28 10:12:50.941209 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/120.png
+-rw-r--r--   0        0        0    19866 2024-05-28 10:12:50.941528 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/128.png
+-rw-r--r--   0        0        0    23814 2024-05-28 10:12:50.941837 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/144.png
+-rw-r--r--   0        0        0    25818 2024-05-28 10:12:50.942007 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/152.png
+-rw-r--r--   0        0        0      822 2024-05-28 10:12:50.942220 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/16.png
+-rw-r--r--   0        0        0    30211 2024-05-28 10:12:50.942564 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/167.png
+-rw-r--r--   0        0        0    31652 2024-05-28 10:12:50.942909 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/172.png
+-rw-r--r--   0        0        0    34032 2024-05-28 10:12:50.943391 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/180.png
+-rw-r--r--   0        0        0    39070 2024-05-28 10:12:50.943886 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/196.png
+-rw-r--r--   0        0        0     1104 2024-05-28 10:12:50.944119 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/20.png
+-rw-r--r--   0        0        0    45736 2024-05-28 10:12:50.944656 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/216.png
+-rw-r--r--   0        0        0    60912 2024-05-28 10:12:50.945186 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/256.png
+-rw-r--r--   0        0        0     1922 2024-05-28 10:12:50.945387 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/29.png
+-rw-r--r--   0        0        0     2235 2024-05-28 10:12:50.945681 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/32.png
+-rw-r--r--   0        0        0     3180 2024-05-28 10:12:50.945872 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/40.png
+-rw-r--r--   0        0        0     4265 2024-05-28 10:12:50.946089 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/48.png
+-rw-r--r--   0        0        0     4543 2024-05-28 10:12:50.946359 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/50.png
+-rw-r--r--   0        0        0   206946 2024-05-28 10:12:50.950422 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/512.png
+-rw-r--r--   0        0        0     5252 2024-05-28 10:12:50.950722 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/55.png
+-rw-r--r--   0        0        0     5549 2024-05-28 10:12:50.951020 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/57.png
+-rw-r--r--   0        0        0     5649 2024-05-28 10:12:50.951179 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/58.png
+-rw-r--r--   0        0        0     5983 2024-05-28 10:12:50.951413 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/60.png
+-rw-r--r--   0        0        0     6583 2024-05-28 10:12:50.951648 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/64.png
+-rw-r--r--   0        0        0     6988 2024-05-28 10:12:50.951770 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/66.png
+-rw-r--r--   0        0        0     7993 2024-05-28 10:12:50.951890 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/72.png
+-rw-r--r--   0        0        0     8732 2024-05-28 10:12:50.952196 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/76.png
+-rw-r--r--   0        0        0     9417 2024-05-28 10:12:50.952599 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/80.png
+-rw-r--r--   0        0        0    10705 2024-05-28 10:12:50.952918 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/87.png
+-rw-r--r--   0        0        0    10894 2024-05-28 10:12:50.953132 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/88.png
+-rw-r--r--   0        0        0    11674 2024-05-28 10:12:50.953339 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/92.png
+-rw-r--r--   0        0        0     7139 2024-05-28 10:12:50.953567 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/Contents.json
+-rw-r--r--   0        0        0   772414 2024-05-28 10:12:50.954162 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/appstore.png
+-rw-r--r--   0        0        0   214701 2024-05-28 10:12:50.955002 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/playstore.png
+-rw-r--r--   0        0        0   998221 2024-05-28 10:12:50.957694 taskbridge-0.1.1/taskbridge/gui/assets/TaskBridge.icns
+-rw-r--r--   0        0        0    17569 2024-05-28 10:12:50.958192 taskbridge-0.1.1/taskbridge/gui/assets/TaskBridge.iconset/icon_128x128.png
+-rw-r--r--   0        0        0    50656 2024-05-28 10:12:50.958847 taskbridge-0.1.1/taskbridge/gui/assets/TaskBridge.iconset/icon_128x128@2x.png
+-rw-r--r--   0        0        0     1699 2024-05-28 10:12:50.959128 taskbridge-0.1.1/taskbridge/gui/assets/TaskBridge.iconset/icon_16x16.png
+-rw-r--r--   0        0        0     2759 2024-05-28 10:12:50.959494 taskbridge-0.1.1/taskbridge/gui/assets/TaskBridge.iconset/icon_16x16@2x.png
+-rw-r--r--   0        0        0    50655 2024-05-28 10:12:50.960206 taskbridge-0.1.1/taskbridge/gui/assets/TaskBridge.iconset/icon_256x256.png
+-rw-r--r--   0        0        0   159642 2024-05-28 10:12:50.961211 taskbridge-0.1.1/taskbridge/gui/assets/TaskBridge.iconset/icon_256x256@2x.png
+-rw-r--r--   0        0        0     2759 2024-05-28 10:12:50.961450 taskbridge-0.1.1/taskbridge/gui/assets/TaskBridge.iconset/icon_32x32.png
+-rw-r--r--   0        0        0     6510 2024-05-28 10:12:50.961765 taskbridge-0.1.1/taskbridge/gui/assets/TaskBridge.iconset/icon_32x32@2x.png
+-rw-r--r--   0        0        0   159641 2024-05-28 10:12:50.962802 taskbridge-0.1.1/taskbridge/gui/assets/TaskBridge.iconset/icon_512x512.png
+-rw-r--r--   0        0        0   551167 2024-05-28 10:12:50.964524 taskbridge-0.1.1/taskbridge/gui/assets/TaskBridge.iconset/icon_512x512@2x.png
+-rw-r--r--   0        0        0   931253 2024-05-28 10:12:50.968883 taskbridge-0.1.1/taskbridge/gui/assets/source/TaskBridge_Icon.xcf
+-rw-r--r--   0        0        0    69368 2024-05-28 10:12:50.971236 taskbridge-0.1.1/taskbridge/gui/assets/source/bridge.xcf
+-rw-r--r--   0        0        0   658861 2024-05-28 10:12:50.972885 taskbridge-0.1.1/taskbridge/gui/assets/source/bridge_animated_black.xcf
+-rw-r--r--   0        0        0    63732 2024-05-28 10:12:50.973309 taskbridge-0.1.1/taskbridge/gui/assets/source/bridge_animated_optimised.xcf
+-rw-r--r--   0        0        0  1156034 2024-05-28 10:12:50.975394 taskbridge-0.1.1/taskbridge/gui/assets/source/bridge_animated_white.xcf
+-rw-r--r--   0        0        0     3862 2024-05-28 10:12:50.975704 taskbridge-0.1.1/taskbridge/gui/assets/source/ios-arrow-round-up-7-512.png
+-rw-r--r--   0        0        0     5539 2024-05-28 10:12:50.975944 taskbridge-0.1.1/taskbridge/gui/assets/source/ios-swap-7-512.png
+-rw-r--r--   0        0        0     8361 2024-05-28 10:12:50.976299 taskbridge-0.1.1/taskbridge/gui/assets/source/local.png
+-rw-r--r--   0        0        0     2197 2024-05-28 10:12:50.976549 taskbridge-0.1.1/taskbridge/gui/assets/source/local_and_remote_black.xcf
+-rw-r--r--   0        0        0     3294 2024-05-28 10:12:50.976763 taskbridge-0.1.1/taskbridge/gui/assets/source/local_and_remote_white.xcf
+-rw-r--r--   0        0        0    18816 2024-05-28 10:12:50.977106 taskbridge-0.1.1/taskbridge/gui/assets/source/remote.png
+-rw-r--r--   0        0        0     1301 2024-05-28 10:12:50.977370 taskbridge-0.1.1/taskbridge/gui/assets/table/bidirectional_black.png
+-rw-r--r--   0        0        0     1301 2024-05-28 10:12:50.977572 taskbridge-0.1.1/taskbridge/gui/assets/table/bidirectional_white.png
+-rw-r--r--   0        0        0     1591 2024-05-28 10:12:50.977789 taskbridge-0.1.1/taskbridge/gui/assets/table/local_and_remote_black.png
+-rw-r--r--   0        0        0     1686 2024-05-28 10:12:50.978040 taskbridge-0.1.1/taskbridge/gui/assets/table/local_and_remote_white.png
+-rw-r--r--   0        0        0      965 2024-05-28 10:12:50.978308 taskbridge-0.1.1/taskbridge/gui/assets/table/local_black.png
+-rw-r--r--   0        0        0     1950 2024-05-28 10:12:50.978538 taskbridge-0.1.1/taskbridge/gui/assets/table/local_to_remote_black.png
+-rw-r--r--   0        0        0     1955 2024-05-28 10:12:50.978765 taskbridge-0.1.1/taskbridge/gui/assets/table/local_to_remote_white.png
+-rw-r--r--   0        0        0      990 2024-05-28 10:12:50.979082 taskbridge-0.1.1/taskbridge/gui/assets/table/local_white.png
+-rw-r--r--   0        0        0     1266 2024-05-28 10:12:50.979320 taskbridge-0.1.1/taskbridge/gui/assets/table/remote_black.png
+-rw-r--r--   0        0        0     2885 2024-05-28 10:12:50.979551 taskbridge-0.1.1/taskbridge/gui/assets/table/remote_to_local_black.png
+-rw-r--r--   0        0        0     2847 2024-05-28 10:12:50.979755 taskbridge-0.1.1/taskbridge/gui/assets/table/remote_to_local_white.png
+-rw-r--r--   0        0        0     1290 2024-05-28 10:12:50.979981 taskbridge-0.1.1/taskbridge/gui/assets/table/remote_white.png
+-rw-r--r--   0        0        0    17458 2024-05-28 10:12:50.980399 taskbridge-0.1.1/taskbridge/gui/assets/tray/bridge_animated_black.gif
+-rw-r--r--   0        0        0    17522 2024-05-28 10:12:50.980793 taskbridge-0.1.1/taskbridge/gui/assets/tray/bridge_animated_white.gif
+-rw-r--r--   0        0        0    47984 2024-05-28 10:12:50.981403 taskbridge-0.1.1/taskbridge/gui/assets/tray/bridge_black.png
+-rw-r--r--   0        0        0    11350 2024-05-28 10:12:50.981753 taskbridge-0.1.1/taskbridge/gui/assets/tray/bridge_white.png
+-rw-r--r--   0        0        0   387868 2024-05-28 10:12:50.983237 taskbridge-0.1.1/taskbridge/gui/assets/ui/TaskBridge.png
+-rw-r--r--   0        0        0     4909 2024-05-28 10:12:50.983497 taskbridge-0.1.1/taskbridge/gui/assets/ui/refresh.png
+-rw-r--r--   0        0        0     3701 2024-05-28 10:12:50.985394 taskbridge-0.1.1/taskbridge/gui/assets/ui/trash.png
+-rw-r--r--   0        0        0    29098 2024-05-28 10:12:50.985662 taskbridge-0.1.1/taskbridge/gui/taskbridge.ui
+-rw-r--r--   0        0        0      908 2024-05-28 10:12:50.985936 taskbridge-0.1.1/taskbridge/gui/viewmodel/__init__.py
+-rw-r--r--   0        0        0      476 2024-05-28 10:12:50.986140 taskbridge-0.1.1/taskbridge/gui/viewmodel/mainwindow.py
+-rw-r--r--   0        0        0     2703 2024-05-28 10:12:50.986369 taskbridge-0.1.1/taskbridge/gui/viewmodel/notecheckbox.py
+-rw-r--r--   0        0        0     1918 2024-05-28 10:12:50.986595 taskbridge-0.1.1/taskbridge/gui/viewmodel/remindercheckbox.py
+-rw-r--r--   0        0        0    45804 2024-05-28 10:12:50.986875 taskbridge-0.1.1/taskbridge/gui/viewmodel/taskbridgeapp.py
+-rw-r--r--   0        0        0    13063 2024-05-28 10:12:50.987144 taskbridge-0.1.1/taskbridge/gui/viewmodel/threadedtasks.py
+-rw-r--r--   0        0        0     1771 2024-05-28 10:12:50.987467 taskbridge-0.1.1/taskbridge/gui/viewmodel/trayicon.py
+-rw-r--r--   0        0        0     3201 2024-05-28 10:12:50.987796 taskbridge-0.1.1/taskbridge/gui/viewmodel/ui_aboutwindow.py
+-rw-r--r--   0        0        0    32872 2024-05-28 10:12:50.989411 taskbridge-0.1.1/taskbridge/gui/viewmodel/ui_mainwindow.py
+-rw-r--r--   0        0        0     5496 2024-05-28 10:56:54.707655 taskbridge-0.1.1/taskbridge/helpers.py
+-rw-r--r--   0        0        0      570 2024-05-28 10:12:50.989907 taskbridge-0.1.1/taskbridge/notes/__init__.py
+-rw-r--r--   0        0        0     7391 2024-05-28 10:12:50.990114 taskbridge-0.1.1/taskbridge/notes/controller.py
+-rw-r--r--   0        0        0      572 2024-05-28 10:58:25.084166 taskbridge-0.1.1/taskbridge/notes/model/__init__.py
+-rw-r--r--   0        0        0    19383 2024-05-28 10:59:05.331708 taskbridge-0.1.1/taskbridge/notes/model/note.py
+-rw-r--r--   0        0        0    43723 2024-05-28 10:12:50.991327 taskbridge-0.1.1/taskbridge/notes/model/notefolder.py
+-rw-r--r--   0        0        0     6063 2024-05-28 10:12:50.991477 taskbridge-0.1.1/taskbridge/notes/model/notescript.py
+-rw-r--r--   0        0        0      651 2024-05-28 10:59:05.329335 taskbridge-0.1.1/taskbridge/reminders/__init__.py
+-rw-r--r--   0        0        0    10528 2024-05-28 10:12:50.991927 taskbridge-0.1.1/taskbridge/reminders/controller.py
+-rw-r--r--   0        0        0      755 2024-05-28 10:12:50.992162 taskbridge-0.1.1/taskbridge/reminders/model/__init__.py
+-rw-r--r--   0        0        0    16131 2024-05-28 10:12:50.992407 taskbridge-0.1.1/taskbridge/reminders/model/reminder.py
+-rw-r--r--   0        0        0    47638 2024-05-28 10:12:50.992686 taskbridge-0.1.1/taskbridge/reminders/model/remindercontainer.py
+-rw-r--r--   0        0        0     4942 2024-05-28 10:12:50.992846 taskbridge-0.1.1/taskbridge/reminders/model/reminderscript.py
+-rw-r--r--   0        0        0     9159 1970-01-01 00:00:00.000000 taskbridge-0.1.1/PKG-INFO
```

### Comparing `taskbridge-0.1.0/LICENSE` & `taskbridge-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/README.md` & `taskbridge-0.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 data from Windows, Linux or an Android device, you're stuck using web apps. TaskBridge is an attempt at solving this
 problem, by allowing notes and reminders to be synchronised to other cloud services which can more easily be accessed on 
 multiple devices. 
 
 > TaskBridge is in no way affiliated-with or endorsed by Apple, Inc.
 
 
-![screenflow_sync.gif](docs/screenflow_sync.gif)  ![screenflow_notes.gif](docs/screenflow_notes.gif)  ![screenflow_reminders.gif](docs/screenflow_reminders.gif)
+![screenflow_sync.gif](https://github.com/pint-sized/taskbridge/raw/main/docs/screenflow_sync.gif)  ![screenflow_notes.gif](https://github.com/pint-sized/taskbridge/raw/main/docs/screenflow_notes.gif)  ![screenflow_reminders.gif](https://github.com/pint-sized/taskbridge/raw/main/docs/screenflow_reminders.gif)
 
 ## Current Sync Support
 
 - Apple Notes can be synchronised with NextCloud Notes, or any other Markdown folder.
 - Apple Reminders can be synchronised with NextCloud Tasks, or most CalDAV VTODO calendars.
 
 ## Documentation
@@ -135,16 +135,17 @@
 
 For some reason, the Apple Reminders app is extremely slow to respond when there are many stored reminders. For most people, 
 the majority of their reminders are in the Completed section. Clearing this out greatly improves performance. Even with just 20-or-so 
 completed reminders, Reminder synchronisation takes **considerably** longer.
 
 **Can I use TaskBridge without a GUI?**
 
-Yes. A CLI is available for scripted/automated use. See `taskbridge/cli`. 
-A PyPi package is also available. Also, see the `taskbridge/notes` and `taskbridge/reminders` folders in the repository.
+Yes. A CLI is available for scripted/automated use. See `taskbridge/cli`.
+ A [PyPi package](https://pypi.org/project/TaskBridge/) is also available. Also, see the `taskbridge/notes` 
+and `taskbridge/reminders` folders in the repository.
 
 **Why don't you use the NextCloud Notes API?**
 
 The NextCloud Notes API is lacking some core features, such as support for adding attachments to Notes.
 
 **Why don't you use CloudKit?**
```

### Comparing `taskbridge-0.1.0/pyproject.toml` & `taskbridge-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "TaskBridge"
-version = "0.1.0"
+version = "0.1.1"
 description = "Export your Apple Reminders & Notes to NextCloud, a local folder, or CalDav - and keep them in sync!"
 keywords = ["sync", "note sync", "reminder sync", "cloud notes", "cloud reminders"]
-authors = ["Keith Vassallo <keith@vassallo.cloud>"]
+authors = ["Pint-Sized Software <hello@pintsized.dev>"]
 readme = "README.md"
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
   "Programming Language :: Python :: Implementation :: CPython",
   "Environment :: MacOS X",
   "Intended Audience :: End Users/Desktop",
   "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
   "Natural Language :: English",
   "Operating System :: MacOS",
   "Topic :: Utilities"
 ]
 license = "GPL-3.0-or-later"
 homepage = "https://taskbridge.app/"
-repository = "https://github.com/keithvassallomt/TaskBridge"
+repository = "https://github.com/pint-sized/taskbridge"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 PyQt6 = "^6.6.1"
 darkdetect = "^0.8.0"
 keyring = "^25.2.1"
 schedule = "^1.2.1"
```

### Comparing `taskbridge-0.1.0/taskbridge/cli/tbcli.py` & `taskbridge-0.1.1/taskbridge/cli/tbcli.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/TaskBridge.py` & `taskbridge-0.1.1/taskbridge/gui/TaskBridge.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/about.ui` & `taskbridge-0.1.1/taskbridge/gui/about.ui`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/100.png` & `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/100.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/102.png` & `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/102.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/1024.png` & `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/1024.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/114.png` & `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/114.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/120.png` & `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/120.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/128.png` & `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/128.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/144.png` & `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/144.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/152.png` & `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/152.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/16.png` & `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/16.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/167.png` & `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/167.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/172.png` & `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/172.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/180.png` & `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/180.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/196.png` & `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/196.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/20.png` & `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/20.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/216.png` & `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/216.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/256.png` & `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/256.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/29.png` & `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/29.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/32.png` & `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/32.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/40.png` & `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/40.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/48.png` & `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/48.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/50.png` & `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/50.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/512.png` & `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/512.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/55.png` & `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/55.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/57.png` & `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/57.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/58.png` & `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/58.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/60.png` & `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/60.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/64.png` & `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/64.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/66.png` & `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/66.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/72.png` & `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/72.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/76.png` & `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/76.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/80.png` & `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/80.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/87.png` & `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/87.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/88.png` & `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/88.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/92.png` & `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/92.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/Contents.json` & `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/Contents.json`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/appstore.png` & `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/appstore.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/AppIcons/playstore.png` & `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/playstore.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/TaskBridge.icns` & `taskbridge-0.1.1/taskbridge/gui/assets/TaskBridge.icns`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/TaskBridge.iconset/icon_128x128.png` & `taskbridge-0.1.1/taskbridge/gui/assets/TaskBridge.iconset/icon_128x128.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/TaskBridge.iconset/icon_128x128@2x.png` & `taskbridge-0.1.1/taskbridge/gui/assets/TaskBridge.iconset/icon_128x128@2x.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/TaskBridge.iconset/icon_16x16.png` & `taskbridge-0.1.1/taskbridge/gui/assets/TaskBridge.iconset/icon_16x16.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/TaskBridge.iconset/icon_16x16@2x.png` & `taskbridge-0.1.1/taskbridge/gui/assets/TaskBridge.iconset/icon_16x16@2x.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/TaskBridge.iconset/icon_256x256.png` & `taskbridge-0.1.1/taskbridge/gui/assets/TaskBridge.iconset/icon_256x256.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/TaskBridge.iconset/icon_256x256@2x.png` & `taskbridge-0.1.1/taskbridge/gui/assets/TaskBridge.iconset/icon_256x256@2x.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/TaskBridge.iconset/icon_32x32.png` & `taskbridge-0.1.1/taskbridge/gui/assets/TaskBridge.iconset/icon_32x32.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/TaskBridge.iconset/icon_32x32@2x.png` & `taskbridge-0.1.1/taskbridge/gui/assets/TaskBridge.iconset/icon_32x32@2x.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/TaskBridge.iconset/icon_512x512.png` & `taskbridge-0.1.1/taskbridge/gui/assets/TaskBridge.iconset/icon_512x512.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/TaskBridge.iconset/icon_512x512@2x.png` & `taskbridge-0.1.1/taskbridge/gui/assets/TaskBridge.iconset/icon_512x512@2x.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/source/TaskBridge_Icon.xcf` & `taskbridge-0.1.1/taskbridge/gui/assets/source/TaskBridge_Icon.xcf`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/source/bridge.xcf` & `taskbridge-0.1.1/taskbridge/gui/assets/source/bridge.xcf`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/source/bridge_animated_black.xcf` & `taskbridge-0.1.1/taskbridge/gui/assets/source/bridge_animated_black.xcf`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/source/bridge_animated_optimised.xcf` & `taskbridge-0.1.1/taskbridge/gui/assets/source/bridge_animated_optimised.xcf`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/source/bridge_animated_white.xcf` & `taskbridge-0.1.1/taskbridge/gui/assets/source/bridge_animated_white.xcf`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/source/ios-arrow-round-up-7-512.png` & `taskbridge-0.1.1/taskbridge/gui/assets/source/ios-arrow-round-up-7-512.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/source/ios-swap-7-512.png` & `taskbridge-0.1.1/taskbridge/gui/assets/source/ios-swap-7-512.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/source/local.png` & `taskbridge-0.1.1/taskbridge/gui/assets/source/local.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/source/local_and_remote_black.xcf` & `taskbridge-0.1.1/taskbridge/gui/assets/source/local_and_remote_black.xcf`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/source/local_and_remote_white.xcf` & `taskbridge-0.1.1/taskbridge/gui/assets/source/local_and_remote_white.xcf`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/source/remote.png` & `taskbridge-0.1.1/taskbridge/gui/assets/source/remote.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/table/bidirectional_black.png` & `taskbridge-0.1.1/taskbridge/gui/assets/table/bidirectional_black.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/table/bidirectional_white.png` & `taskbridge-0.1.1/taskbridge/gui/assets/table/bidirectional_white.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/table/local_and_remote_black.png` & `taskbridge-0.1.1/taskbridge/gui/assets/table/local_and_remote_black.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/table/local_and_remote_white.png` & `taskbridge-0.1.1/taskbridge/gui/assets/table/local_and_remote_white.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/table/local_black.png` & `taskbridge-0.1.1/taskbridge/gui/assets/table/local_black.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/table/local_to_remote_black.png` & `taskbridge-0.1.1/taskbridge/gui/assets/table/local_to_remote_black.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/table/local_to_remote_white.png` & `taskbridge-0.1.1/taskbridge/gui/assets/table/local_to_remote_white.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/table/local_white.png` & `taskbridge-0.1.1/taskbridge/gui/assets/table/local_white.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/table/remote_black.png` & `taskbridge-0.1.1/taskbridge/gui/assets/table/remote_black.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/table/remote_to_local_black.png` & `taskbridge-0.1.1/taskbridge/gui/assets/table/remote_to_local_black.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/table/remote_to_local_white.png` & `taskbridge-0.1.1/taskbridge/gui/assets/table/remote_to_local_white.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/table/remote_white.png` & `taskbridge-0.1.1/taskbridge/gui/assets/table/remote_white.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/tray/bridge_animated_black.gif` & `taskbridge-0.1.1/taskbridge/gui/assets/tray/bridge_animated_black.gif`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/tray/bridge_animated_white.gif` & `taskbridge-0.1.1/taskbridge/gui/assets/tray/bridge_animated_white.gif`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/tray/bridge_black.png` & `taskbridge-0.1.1/taskbridge/gui/assets/tray/bridge_black.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/tray/bridge_white.png` & `taskbridge-0.1.1/taskbridge/gui/assets/tray/bridge_white.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/ui/TaskBridge.png` & `taskbridge-0.1.1/taskbridge/gui/assets/ui/TaskBridge.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/ui/refresh.png` & `taskbridge-0.1.1/taskbridge/gui/assets/ui/refresh.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/assets/ui/trash.png` & `taskbridge-0.1.1/taskbridge/gui/assets/ui/trash.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/taskbridge.ui` & `taskbridge-0.1.1/taskbridge/gui/taskbridge.ui`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/viewmodel/__init__.py` & `taskbridge-0.1.1/taskbridge/gui/viewmodel/__init__.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/viewmodel/notecheckbox.py` & `taskbridge-0.1.1/taskbridge/gui/viewmodel/notecheckbox.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/viewmodel/remindercheckbox.py` & `taskbridge-0.1.1/taskbridge/gui/viewmodel/remindercheckbox.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/viewmodel/taskbridgeapp.py` & `taskbridge-0.1.1/taskbridge/gui/viewmodel/taskbridgeapp.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/viewmodel/threadedtasks.py` & `taskbridge-0.1.1/taskbridge/gui/viewmodel/threadedtasks.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/viewmodel/trayicon.py` & `taskbridge-0.1.1/taskbridge/gui/viewmodel/trayicon.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/viewmodel/ui_aboutwindow.py` & `taskbridge-0.1.1/taskbridge/gui/viewmodel/ui_aboutwindow.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/gui/viewmodel/ui_mainwindow.py` & `taskbridge-0.1.1/taskbridge/gui/viewmodel/ui_mainwindow.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/helpers.py` & `taskbridge-0.1.1/taskbridge/helpers.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/notes/__init__.py` & `taskbridge-0.1.1/taskbridge/notes/__init__.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/notes/controller.py` & `taskbridge-0.1.1/taskbridge/notes/controller.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/notes/model/__init__.py` & `taskbridge-0.1.1/taskbridge/notes/model/__init__.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/notes/model/note.py` & `taskbridge-0.1.1/taskbridge/notes/model/note.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/notes/model/notefolder.py` & `taskbridge-0.1.1/taskbridge/notes/model/notefolder.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/notes/model/notescript.py` & `taskbridge-0.1.1/taskbridge/notes/model/notescript.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/reminders/__init__.py` & `taskbridge-0.1.1/taskbridge/reminders/__init__.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/reminders/controller.py` & `taskbridge-0.1.1/taskbridge/reminders/controller.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/reminders/model/__init__.py` & `taskbridge-0.1.1/taskbridge/reminders/model/__init__.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/reminders/model/reminder.py` & `taskbridge-0.1.1/taskbridge/reminders/model/reminder.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/reminders/model/remindercontainer.py` & `taskbridge-0.1.1/taskbridge/reminders/model/remindercontainer.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/taskbridge/reminders/model/reminderscript.py` & `taskbridge-0.1.1/taskbridge/reminders/model/reminderscript.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.0/PKG-INFO` & `taskbridge-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: TaskBridge
-Version: 0.1.0
+Version: 0.1.1
 Summary: Export your Apple Reminders & Notes to NextCloud, a local folder, or CalDav - and keep them in sync!
 Home-page: https://taskbridge.app/
 License: GPL-3.0-or-later
 Keywords: sync,note sync,reminder sync,cloud notes,cloud reminders
-Author: Keith Vassallo
-Author-email: keith@vassallo.cloud
+Author: Pint-Sized Software
+Author-email: hello@pintsized.dev
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: MacOS X
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
@@ -24,15 +24,15 @@
 Requires-Dist: PyQt6 (>=6.6.1,<7.0.0)
 Requires-Dist: caldav (>=1.3.9,<2.0.0)
 Requires-Dist: darkdetect (>=0.8.0,<0.9.0)
 Requires-Dist: keyring (>=25.2.1,<26.0.0)
 Requires-Dist: markdown2 (>=2.4.13,<3.0.0)
 Requires-Dist: markdownify (>=0.12.1,<0.13.0)
 Requires-Dist: schedule (>=1.2.1,<2.0.0)
-Project-URL: Repository, https://github.com/keithvassallomt/TaskBridge
+Project-URL: Repository, https://github.com/pint-sized/taskbridge
 Description-Content-Type: text/markdown
 
 # TaskBridge
 
 Export your Apple Reminders & Notes to NextCloud, a local folder, or CalDav - and keep them in sync!
 
 [![Documentation Status](https://readthedocs.org/projects/taskbridge/badge/?version=latest)](https://taskbridge.readthedocs.io/en/latest/?badge=latest) ![example workflow](https://github.com/pint-sized/taskbridge/actions/workflows/python-app.yml/badge.svg) [![Coverage Status](https://coveralls.io/repos/github/pint-sized/taskbridge/badge.svg)](https://coveralls.io/github/pint-sized/taskbridge)
@@ -41,15 +41,15 @@
 data from Windows, Linux or an Android device, you're stuck using web apps. TaskBridge is an attempt at solving this
 problem, by allowing notes and reminders to be synchronised to other cloud services which can more easily be accessed on 
 multiple devices. 
 
 > TaskBridge is in no way affiliated-with or endorsed by Apple, Inc.
 
 
-![screenflow_sync.gif](docs/screenflow_sync.gif)  ![screenflow_notes.gif](docs/screenflow_notes.gif)  ![screenflow_reminders.gif](docs/screenflow_reminders.gif)
+![screenflow_sync.gif](https://github.com/pint-sized/taskbridge/raw/main/docs/screenflow_sync.gif)  ![screenflow_notes.gif](https://github.com/pint-sized/taskbridge/raw/main/docs/screenflow_notes.gif)  ![screenflow_reminders.gif](https://github.com/pint-sized/taskbridge/raw/main/docs/screenflow_reminders.gif)
 
 ## Current Sync Support
 
 - Apple Notes can be synchronised with NextCloud Notes, or any other Markdown folder.
 - Apple Reminders can be synchronised with NextCloud Tasks, or most CalDAV VTODO calendars.
 
 ## Documentation
@@ -168,16 +168,17 @@
 
 For some reason, the Apple Reminders app is extremely slow to respond when there are many stored reminders. For most people, 
 the majority of their reminders are in the Completed section. Clearing this out greatly improves performance. Even with just 20-or-so 
 completed reminders, Reminder synchronisation takes **considerably** longer.
 
 **Can I use TaskBridge without a GUI?**
 
-Yes. A CLI is available for scripted/automated use. See `taskbridge/cli`. 
-A PyPi package is also available. Also, see the `taskbridge/notes` and `taskbridge/reminders` folders in the repository.
+Yes. A CLI is available for scripted/automated use. See `taskbridge/cli`.
+ A [PyPi package](https://pypi.org/project/TaskBridge/) is also available. Also, see the `taskbridge/notes` 
+and `taskbridge/reminders` folders in the repository.
 
 **Why don't you use the NextCloud Notes API?**
 
 The NextCloud Notes API is lacking some core features, such as support for adding attachments to Notes.
 
 **Why don't you use CloudKit?**
```

