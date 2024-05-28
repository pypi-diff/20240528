# Comparing `tmp/mg-pso-gui-0.1.96.tar.gz` & `tmp/mg-pso-gui-0.1.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mg-pso-gui-0.1.96.tar", last modified: Tue May 28 05:48:50 2024, max compression
+gzip compressed data, was "mg-pso-gui-0.1.97.tar", last modified: Tue May 28 06:06:56 2024, max compression
```

## Comparing `mg-pso-gui-0.1.96.tar` & `mg-pso-gui-0.1.97.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 05:48:50.360576 mg-pso-gui-0.1.96/
--rw-r--r--   0 robertcordingly   (501) staff       (20)     9458 2024-05-28 05:48:50.359920 mg-pso-gui-0.1.96/PKG-INFO
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 05:48:50.359417 mg-pso-gui-0.1.96/mg_pso_gui.egg-info/
--rw-r--r--   0 robertcordingly   (501) staff       (20)     9458 2024-05-28 05:48:50.000000 mg-pso-gui-0.1.96/mg_pso_gui.egg-info/PKG-INFO
--rw-r--r--   0 robertcordingly   (501) staff       (20)     1871 2024-05-28 05:48:50.000000 mg-pso-gui-0.1.96/mg_pso_gui.egg-info/SOURCES.txt
--rw-r--r--   0 robertcordingly   (501) staff       (20)        1 2024-05-28 05:48:50.000000 mg-pso-gui-0.1.96/mg_pso_gui.egg-info/dependency_links.txt
--rw-r--r--   0 robertcordingly   (501) staff       (20)      117 2024-05-28 05:48:50.000000 mg-pso-gui-0.1.96/mg_pso_gui.egg-info/entry_points.txt
--rw-r--r--   0 robertcordingly   (501) staff       (20)       76 2024-05-28 05:48:50.000000 mg-pso-gui-0.1.96/mg_pso_gui.egg-info/requires.txt
--rw-r--r--   0 robertcordingly   (501) staff       (20)        9 2024-05-28 05:48:50.000000 mg-pso-gui-0.1.96/mg_pso_gui.egg-info/top_level.txt
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 05:48:50.334795 mg-pso-gui-0.1.96/mgpsogui/
--rw-r--r--   0 robertcordingly   (501) staff       (20)       42 2023-10-10 00:40:24.000000 mg-pso-gui-0.1.96/mgpsogui/__init__.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 05:48:50.336017 mg-pso-gui-0.1.96/mgpsogui/gui/
--rwxr--r--   0 robertcordingly   (501) staff       (20)    24244 2024-05-21 09:15:18.000000 mg-pso-gui-0.1.96/mgpsogui/gui/HomePage.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)    12527 2024-05-21 08:47:30.000000 mg-pso-gui-0.1.96/mgpsogui/gui/OptionManager.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 05:48:50.336786 mg-pso-gui-0.1.96/mgpsogui/gui/PlatformTab/
--rw-r--r--   0 robertcordingly   (501) staff       (20)    10486 2024-02-14 07:13:08.000000 mg-pso-gui-0.1.96/mgpsogui/gui/PlatformTab/PlatformTab.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2024-02-13 05:36:09.000000 mg-pso-gui-0.1.96/mgpsogui/gui/PlatformTab/__init__.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 05:48:50.337467 mg-pso-gui-0.1.96/mgpsogui/gui/RunTab/
--rw-r--r--   0 robertcordingly   (501) staff       (20)     1839 2024-03-20 19:57:02.000000 mg-pso-gui-0.1.96/mgpsogui/gui/RunTab/RunTab.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2024-02-13 06:41:01.000000 mg-pso-gui-0.1.96/mgpsogui/gui/RunTab/__init__.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 05:48:50.341870 mg-pso-gui-0.1.96/mgpsogui/gui/SetupTab/
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2866 2024-02-14 07:40:24.000000 mg-pso-gui-0.1.96/mgpsogui/gui/SetupTab/BoundsEditorWindow.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)    12268 2024-02-14 08:06:06.000000 mg-pso-gui-0.1.96/mgpsogui/gui/SetupTab/BoundsList.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2784 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.96/mgpsogui/gui/SetupTab/CalibrationParametersView.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     4092 2024-02-13 06:33:07.000000 mg-pso-gui-0.1.96/mgpsogui/gui/SetupTab/FunctionsList.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     7352 2023-10-18 05:17:22.000000 mg-pso-gui-0.1.96/mgpsogui/gui/SetupTab/ListParametersView.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2003 2024-05-21 09:16:16.000000 mg-pso-gui-0.1.96/mgpsogui/gui/SetupTab/OptimalParameterView.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2443 2024-05-21 09:01:39.000000 mg-pso-gui-0.1.96/mgpsogui/gui/SetupTab/SetupTab.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2739 2024-02-13 05:33:08.000000 mg-pso-gui-0.1.96/mgpsogui/gui/SetupTab/StaticParameterView.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     5937 2024-05-21 09:12:51.000000 mg-pso-gui-0.1.96/mgpsogui/gui/SetupTab/StepView.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2024-02-13 05:20:36.000000 mg-pso-gui-0.1.96/mgpsogui/gui/SetupTab/__init__.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 05:48:50.342869 mg-pso-gui-0.1.96/mgpsogui/gui/VisualizeTab/
--rw-r--r--   0 robertcordingly   (501) staff       (20)    13322 2024-05-15 21:08:56.000000 mg-pso-gui-0.1.96/mgpsogui/gui/VisualizeTab/SideBar.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     3477 2024-04-10 18:55:43.000000 mg-pso-gui-0.1.96/mgpsogui/gui/VisualizeTab/VisualizeTab.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2024-02-14 03:49:32.000000 mg-pso-gui-0.1.96/mgpsogui/gui/VisualizeTab/__init__.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2023-10-03 21:33:58.000000 mg-pso-gui-0.1.96/mgpsogui/gui/__init__.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 05:48:50.352251 mg-pso-gui-0.1.96/mgpsogui/gui/images/
--rw-r--r--   0 robertcordingly   (501) staff       (20)   433752 2024-02-27 04:32:36.000000 mg-pso-gui-0.1.96/mgpsogui/gui/images/IGOW 4 Logo.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2989 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.96/mgpsogui/gui/images/collapse.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2654 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.96/mgpsogui/gui/images/down.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2922 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.96/mgpsogui/gui/images/expand.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2790 2024-02-14 06:41:01.000000 mg-pso-gui-0.1.96/mgpsogui/gui/images/play.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)     4657 2024-02-14 06:39:03.000000 mg-pso-gui-0.1.96/mgpsogui/gui/images/refresh.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)    31242 2024-02-14 08:26:13.000000 mg-pso-gui-0.1.96/mgpsogui/gui/images/refresh_hd.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2153 2024-02-14 06:41:07.000000 mg-pso-gui-0.1.96/mgpsogui/gui/images/stop.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)     3642 2024-03-20 06:12:19.000000 mg-pso-gui-0.1.96/mgpsogui/gui/images/test.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2958 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.96/mgpsogui/gui/images/trash.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2457 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.96/mgpsogui/gui/images/up.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)      148 2023-10-04 08:06:40.000000 mg-pso-gui-0.1.96/mgpsogui/mgpsogui.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     4713 2023-11-08 23:03:41.000000 mg-pso-gui-0.1.96/mgpsogui/start.yaml
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 05:48:50.353839 mg-pso-gui-0.1.96/mgpsogui/util/
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 05:48:50.354531 mg-pso-gui-0.1.96/mgpsogui/util/CTkToolTip/
--rw-rw-r--   0 robertcordingly   (501) staff       (20)      225 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.96/mgpsogui/util/CTkToolTip/__init__.py
--rw-rw-r--   0 robertcordingly   (501) staff       (20)     6329 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.96/mgpsogui/util/CTkToolTip/ctk_tooltip.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)    15076 2024-04-24 19:47:23.000000 mg-pso-gui-0.1.96/mgpsogui/util/GraphGenerator.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     3481 2024-05-28 05:35:43.000000 mg-pso-gui-0.1.96/mgpsogui/util/PSORunner.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2023-10-03 21:32:18.000000 mg-pso-gui-0.1.96/mgpsogui/util/__init__.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 05:48:50.355072 mg-pso-gui-0.1.96/mgpsogui/util/recosu/
--rw-r--r--   0 robertcordingly   (501) staff       (20)      236 2024-03-06 06:18:26.000000 mg-pso-gui-0.1.96/mgpsogui/util/recosu/__init__.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 05:48:50.356654 mg-pso-gui-0.1.96/mgpsogui/util/recosu/pso/
--rw-r--r--   0 robertcordingly   (501) staff       (20)      247 2024-03-06 06:18:26.000000 mg-pso-gui-0.1.96/mgpsogui/util/recosu/pso/__init__.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2721 2024-03-20 06:01:30.000000 mg-pso-gui-0.1.96/mgpsogui/util/recosu/pso/csip_access.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)    12827 2024-05-28 05:48:44.000000 mg-pso-gui-0.1.96/mgpsogui/util/recosu/pso/pso.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 05:48:50.358030 mg-pso-gui-0.1.96/mgpsogui/util/recosu/utils/
--rw-r--r--   0 robertcordingly   (501) staff       (20)      196 2024-03-06 06:18:26.000000 mg-pso-gui-0.1.96/mgpsogui/util/recosu/utils/__init__.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 05:48:50.358888 mg-pso-gui-0.1.96/mgpsogui/util/recosu/utils/plot/
--rw-r--r--   0 robertcordingly   (501) staff       (20)       71 2024-03-06 06:18:26.000000 mg-pso-gui-0.1.96/mgpsogui/util/recosu/utils/plot/__init__.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     3779 2024-03-06 06:18:27.000000 mg-pso-gui-0.1.96/mgpsogui/util/recosu/utils/plot/cost_steps.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     3023 2024-03-06 06:18:27.000000 mg-pso-gui-0.1.96/mgpsogui/util/recosu/utils/trace_writer.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     3951 2024-03-06 06:18:27.000000 mg-pso-gui-0.1.96/mgpsogui/util/recosu/utils/utils.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)       38 2024-05-28 05:48:50.360690 mg-pso-gui-0.1.96/setup.cfg
--rw-r--r--   0 robertcordingly   (501) staff       (20)     1526 2024-05-28 05:48:48.000000 mg-pso-gui-0.1.96/setup.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 06:06:56.154569 mg-pso-gui-0.1.97/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     9458 2024-05-28 06:06:56.153723 mg-pso-gui-0.1.97/PKG-INFO
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 06:06:56.153233 mg-pso-gui-0.1.97/mg_pso_gui.egg-info/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     9458 2024-05-28 06:06:56.000000 mg-pso-gui-0.1.97/mg_pso_gui.egg-info/PKG-INFO
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     1871 2024-05-28 06:06:56.000000 mg-pso-gui-0.1.97/mg_pso_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 robertcordingly   (501) staff       (20)        1 2024-05-28 06:06:56.000000 mg-pso-gui-0.1.97/mg_pso_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 robertcordingly   (501) staff       (20)      117 2024-05-28 06:06:56.000000 mg-pso-gui-0.1.97/mg_pso_gui.egg-info/entry_points.txt
+-rw-r--r--   0 robertcordingly   (501) staff       (20)       76 2024-05-28 06:06:56.000000 mg-pso-gui-0.1.97/mg_pso_gui.egg-info/requires.txt
+-rw-r--r--   0 robertcordingly   (501) staff       (20)        9 2024-05-28 06:06:56.000000 mg-pso-gui-0.1.97/mg_pso_gui.egg-info/top_level.txt
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 06:06:56.123310 mg-pso-gui-0.1.97/mgpsogui/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)       42 2023-10-10 00:40:24.000000 mg-pso-gui-0.1.97/mgpsogui/__init__.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 06:06:56.125121 mg-pso-gui-0.1.97/mgpsogui/gui/
+-rwxr--r--   0 robertcordingly   (501) staff       (20)    24244 2024-05-21 09:15:18.000000 mg-pso-gui-0.1.97/mgpsogui/gui/HomePage.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)    12527 2024-05-21 08:47:30.000000 mg-pso-gui-0.1.97/mgpsogui/gui/OptionManager.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 06:06:56.125899 mg-pso-gui-0.1.97/mgpsogui/gui/PlatformTab/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)    10486 2024-02-14 07:13:08.000000 mg-pso-gui-0.1.97/mgpsogui/gui/PlatformTab/PlatformTab.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2024-02-13 05:36:09.000000 mg-pso-gui-0.1.97/mgpsogui/gui/PlatformTab/__init__.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 06:06:56.126633 mg-pso-gui-0.1.97/mgpsogui/gui/RunTab/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     1839 2024-03-20 19:57:02.000000 mg-pso-gui-0.1.97/mgpsogui/gui/RunTab/RunTab.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2024-02-13 06:41:01.000000 mg-pso-gui-0.1.97/mgpsogui/gui/RunTab/__init__.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 06:06:56.132214 mg-pso-gui-0.1.97/mgpsogui/gui/SetupTab/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2866 2024-02-14 07:40:24.000000 mg-pso-gui-0.1.97/mgpsogui/gui/SetupTab/BoundsEditorWindow.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)    12268 2024-02-14 08:06:06.000000 mg-pso-gui-0.1.97/mgpsogui/gui/SetupTab/BoundsList.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2784 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.97/mgpsogui/gui/SetupTab/CalibrationParametersView.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     4092 2024-02-13 06:33:07.000000 mg-pso-gui-0.1.97/mgpsogui/gui/SetupTab/FunctionsList.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     7352 2023-10-18 05:17:22.000000 mg-pso-gui-0.1.97/mgpsogui/gui/SetupTab/ListParametersView.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2003 2024-05-21 09:16:16.000000 mg-pso-gui-0.1.97/mgpsogui/gui/SetupTab/OptimalParameterView.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2443 2024-05-21 09:01:39.000000 mg-pso-gui-0.1.97/mgpsogui/gui/SetupTab/SetupTab.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2739 2024-02-13 05:33:08.000000 mg-pso-gui-0.1.97/mgpsogui/gui/SetupTab/StaticParameterView.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     5937 2024-05-21 09:12:51.000000 mg-pso-gui-0.1.97/mgpsogui/gui/SetupTab/StepView.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2024-02-13 05:20:36.000000 mg-pso-gui-0.1.97/mgpsogui/gui/SetupTab/__init__.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 06:06:56.133676 mg-pso-gui-0.1.97/mgpsogui/gui/VisualizeTab/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)    13322 2024-05-15 21:08:56.000000 mg-pso-gui-0.1.97/mgpsogui/gui/VisualizeTab/SideBar.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     3477 2024-04-10 18:55:43.000000 mg-pso-gui-0.1.97/mgpsogui/gui/VisualizeTab/VisualizeTab.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2024-02-14 03:49:32.000000 mg-pso-gui-0.1.97/mgpsogui/gui/VisualizeTab/__init__.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2023-10-03 21:33:58.000000 mg-pso-gui-0.1.97/mgpsogui/gui/__init__.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 06:06:56.146201 mg-pso-gui-0.1.97/mgpsogui/gui/images/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)   433752 2024-02-27 04:32:36.000000 mg-pso-gui-0.1.97/mgpsogui/gui/images/IGOW 4 Logo.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2989 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.97/mgpsogui/gui/images/collapse.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2654 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.97/mgpsogui/gui/images/down.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2922 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.97/mgpsogui/gui/images/expand.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2790 2024-02-14 06:41:01.000000 mg-pso-gui-0.1.97/mgpsogui/gui/images/play.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     4657 2024-02-14 06:39:03.000000 mg-pso-gui-0.1.97/mgpsogui/gui/images/refresh.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)    31242 2024-02-14 08:26:13.000000 mg-pso-gui-0.1.97/mgpsogui/gui/images/refresh_hd.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2153 2024-02-14 06:41:07.000000 mg-pso-gui-0.1.97/mgpsogui/gui/images/stop.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     3642 2024-03-20 06:12:19.000000 mg-pso-gui-0.1.97/mgpsogui/gui/images/test.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2958 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.97/mgpsogui/gui/images/trash.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2457 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.97/mgpsogui/gui/images/up.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)      148 2023-10-04 08:06:40.000000 mg-pso-gui-0.1.97/mgpsogui/mgpsogui.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     4713 2023-11-08 23:03:41.000000 mg-pso-gui-0.1.97/mgpsogui/start.yaml
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 06:06:56.147670 mg-pso-gui-0.1.97/mgpsogui/util/
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 06:06:56.148350 mg-pso-gui-0.1.97/mgpsogui/util/CTkToolTip/
+-rw-rw-r--   0 robertcordingly   (501) staff       (20)      225 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.97/mgpsogui/util/CTkToolTip/__init__.py
+-rw-rw-r--   0 robertcordingly   (501) staff       (20)     6329 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.97/mgpsogui/util/CTkToolTip/ctk_tooltip.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)    15076 2024-04-24 19:47:23.000000 mg-pso-gui-0.1.97/mgpsogui/util/GraphGenerator.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     3481 2024-05-28 05:35:43.000000 mg-pso-gui-0.1.97/mgpsogui/util/PSORunner.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2023-10-03 21:32:18.000000 mg-pso-gui-0.1.97/mgpsogui/util/__init__.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 06:06:56.148957 mg-pso-gui-0.1.97/mgpsogui/util/recosu/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)      236 2024-03-06 06:18:26.000000 mg-pso-gui-0.1.97/mgpsogui/util/recosu/__init__.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 06:06:56.150342 mg-pso-gui-0.1.97/mgpsogui/util/recosu/pso/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)      247 2024-03-06 06:18:26.000000 mg-pso-gui-0.1.97/mgpsogui/util/recosu/pso/__init__.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2721 2024-03-20 06:01:30.000000 mg-pso-gui-0.1.97/mgpsogui/util/recosu/pso/csip_access.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)    12821 2024-05-28 06:06:48.000000 mg-pso-gui-0.1.97/mgpsogui/util/recosu/pso/pso.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 06:06:56.151713 mg-pso-gui-0.1.97/mgpsogui/util/recosu/utils/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)      196 2024-03-06 06:18:26.000000 mg-pso-gui-0.1.97/mgpsogui/util/recosu/utils/__init__.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 06:06:56.152695 mg-pso-gui-0.1.97/mgpsogui/util/recosu/utils/plot/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)       71 2024-03-06 06:18:26.000000 mg-pso-gui-0.1.97/mgpsogui/util/recosu/utils/plot/__init__.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     3779 2024-03-06 06:18:27.000000 mg-pso-gui-0.1.97/mgpsogui/util/recosu/utils/plot/cost_steps.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     3023 2024-03-06 06:18:27.000000 mg-pso-gui-0.1.97/mgpsogui/util/recosu/utils/trace_writer.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     3951 2024-03-06 06:18:27.000000 mg-pso-gui-0.1.97/mgpsogui/util/recosu/utils/utils.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)       38 2024-05-28 06:06:56.154692 mg-pso-gui-0.1.97/setup.cfg
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     1526 2024-05-28 06:06:53.000000 mg-pso-gui-0.1.97/setup.py
```

### Comparing `mg-pso-gui-0.1.96/PKG-INFO` & `mg-pso-gui-0.1.97/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mg-pso-gui
-Version: 0.1.96
+Version: 0.1.97
 Summary: GUI for MG-PSO
 Author: Robert Cordingly
 Author-email: <rcording@uw.ed>
 Keywords: python,muti-group,pso,particle,swarm,optimization,gui
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mg-pso-gui-0.1.96/mg_pso_gui.egg-info/PKG-INFO` & `mg-pso-gui-0.1.97/mg_pso_gui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mg-pso-gui
-Version: 0.1.96
+Version: 0.1.97
 Summary: GUI for MG-PSO
 Author: Robert Cordingly
 Author-email: <rcording@uw.ed>
 Keywords: python,muti-group,pso,particle,swarm,optimization,gui
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mg-pso-gui-0.1.96/mg_pso_gui.egg-info/SOURCES.txt` & `mg-pso-gui-0.1.97/mg_pso_gui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.96/mgpsogui/gui/HomePage.py` & `mg-pso-gui-0.1.97/mgpsogui/gui/HomePage.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.96/mgpsogui/gui/OptionManager.py` & `mg-pso-gui-0.1.97/mgpsogui/gui/OptionManager.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.96/mgpsogui/gui/PlatformTab/PlatformTab.py` & `mg-pso-gui-0.1.97/mgpsogui/gui/PlatformTab/PlatformTab.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.96/mgpsogui/gui/RunTab/RunTab.py` & `mg-pso-gui-0.1.97/mgpsogui/gui/RunTab/RunTab.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.96/mgpsogui/gui/SetupTab/BoundsEditorWindow.py` & `mg-pso-gui-0.1.97/mgpsogui/gui/SetupTab/BoundsEditorWindow.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.96/mgpsogui/gui/SetupTab/BoundsList.py` & `mg-pso-gui-0.1.97/mgpsogui/gui/SetupTab/BoundsList.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.96/mgpsogui/gui/SetupTab/CalibrationParametersView.py` & `mg-pso-gui-0.1.97/mgpsogui/gui/SetupTab/CalibrationParametersView.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.96/mgpsogui/gui/SetupTab/FunctionsList.py` & `mg-pso-gui-0.1.97/mgpsogui/gui/SetupTab/FunctionsList.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.96/mgpsogui/gui/SetupTab/ListParametersView.py` & `mg-pso-gui-0.1.97/mgpsogui/gui/SetupTab/ListParametersView.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.96/mgpsogui/gui/SetupTab/OptimalParameterView.py` & `mg-pso-gui-0.1.97/mgpsogui/gui/SetupTab/OptimalParameterView.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.96/mgpsogui/gui/SetupTab/SetupTab.py` & `mg-pso-gui-0.1.97/mgpsogui/gui/SetupTab/SetupTab.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.96/mgpsogui/gui/SetupTab/StaticParameterView.py` & `mg-pso-gui-0.1.97/mgpsogui/gui/SetupTab/StaticParameterView.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.96/mgpsogui/gui/SetupTab/StepView.py` & `mg-pso-gui-0.1.97/mgpsogui/gui/SetupTab/StepView.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.96/mgpsogui/gui/VisualizeTab/SideBar.py` & `mg-pso-gui-0.1.97/mgpsogui/gui/VisualizeTab/SideBar.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.96/mgpsogui/gui/VisualizeTab/VisualizeTab.py` & `mg-pso-gui-0.1.97/mgpsogui/gui/VisualizeTab/VisualizeTab.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.96/mgpsogui/gui/images/IGOW 4 Logo.png` & `mg-pso-gui-0.1.97/mgpsogui/gui/images/IGOW 4 Logo.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.96/mgpsogui/gui/images/collapse.png` & `mg-pso-gui-0.1.97/mgpsogui/gui/images/collapse.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.96/mgpsogui/gui/images/down.png` & `mg-pso-gui-0.1.97/mgpsogui/gui/images/down.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.96/mgpsogui/gui/images/expand.png` & `mg-pso-gui-0.1.97/mgpsogui/gui/images/expand.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.96/mgpsogui/gui/images/play.png` & `mg-pso-gui-0.1.97/mgpsogui/gui/images/play.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.96/mgpsogui/gui/images/refresh.png` & `mg-pso-gui-0.1.97/mgpsogui/gui/images/refresh.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.96/mgpsogui/gui/images/refresh_hd.png` & `mg-pso-gui-0.1.97/mgpsogui/gui/images/refresh_hd.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.96/mgpsogui/gui/images/stop.png` & `mg-pso-gui-0.1.97/mgpsogui/gui/images/stop.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.96/mgpsogui/gui/images/test.png` & `mg-pso-gui-0.1.97/mgpsogui/gui/images/test.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.96/mgpsogui/gui/images/trash.png` & `mg-pso-gui-0.1.97/mgpsogui/gui/images/trash.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.96/mgpsogui/gui/images/up.png` & `mg-pso-gui-0.1.97/mgpsogui/gui/images/up.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.96/mgpsogui/start.yaml` & `mg-pso-gui-0.1.97/mgpsogui/start.yaml`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.96/mgpsogui/util/CTkToolTip/ctk_tooltip.py` & `mg-pso-gui-0.1.97/mgpsogui/util/CTkToolTip/ctk_tooltip.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.96/mgpsogui/util/GraphGenerator.py` & `mg-pso-gui-0.1.97/mgpsogui/util/GraphGenerator.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.96/mgpsogui/util/PSORunner.py` & `mg-pso-gui-0.1.97/mgpsogui/util/PSORunner.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.96/mgpsogui/util/recosu/pso/csip_access.py` & `mg-pso-gui-0.1.97/mgpsogui/util/recosu/pso/csip_access.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.96/mgpsogui/util/recosu/pso/pso.py` & `mg-pso-gui-0.1.97/mgpsogui/util/recosu/pso/pso.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from typing import Dict, List, Set, Tuple
 import numpy as np
 import copy
 import datetime
 import queue
 import json
 import os
-from multiprocessing import Queue
+from multiprocessing import Queue as MPQueue
 
 
 def eval_cost(x, iteration, step_param_names, step_objfunc, calib_params, req_queue, files, url, param, conf: Dict, rnd,
               step):
     particles = len(x[:, 0])
 
     pfail_count = conf.get('particles_fail', 1)  # Number of particles allowed to fail.
@@ -78,15 +78,15 @@
 
     print(flush=True)
     return cost
 
 def global_best(steps: Dict, rounds: Tuple, args: Dict, n_particles: int, iters: int, options: Dict,
                 oh_strategy: Dict = None, n_threads: int = 4, rtol: float = 0.001, ftol: float = -np.inf,
                 ftol_iter: int = 1, full_trace: List = None, rtol_iter: int = 1,
-                conf: Dict = None, metainfo: Dict = None, cost_target: float = -np.inf, result_queue: Queue = None) -> Tuple:
+                conf: Dict = None, metainfo: Dict = None, cost_target: float = -np.inf, result_queue: MPQueue = None) -> Tuple:
     """Performs a stepwise particle swarm optimization PSO using a global best approach.
 
         Parameters
         ----------
         steps : Dict
             step definitions
         rounds : tuple
@@ -174,16 +174,14 @@
     step_trace['rtol_iter'] = rtol_iter
     step_trace['n_threads'] = n_threads
     step_trace['n_particles'] = n_particles
     step_trace['n_steps'] = len(steps)
     step_trace['steps'] = copy.deepcopy(steps)
     #step_trace['args'] = args BUG MUST BE REMOVED
 
-    print("Starting PSO with {} rounds, {} threads, {} particles, {} iterations, {} steps")
-
     if step_file is not None:
         with open(step_file, "w") as fo:
             json.dump(step_trace, fo)
 
     print("Wrote step trace")
 
     # best round cost
@@ -238,29 +236,35 @@
                                              len(param_names),
                                              oh_strategy=step.get('oh_strategy', oh_strategy),
                                              options=step.get('options', options),
                                              bounds=bounds,
                                              ftol=step.get('ftol', ftol),
                                              ftol_iter=step.get('ftol_iter', ftol_iter),
                                              cost_target=step.get('cost_target', cost_target))
-            print('\n>>>>> R{}/S{}  particle params: {}  calibrated params: {}\n'.format(r + 1, s + 1, param_names,
-                                                                                         args['calib_params']))
+                
+            print('\n>>>>> R{}/S{}  particle params: {}  calibrated params: {}\n'.format(r + 1, s + 1, param_names, args['calib_params']))
 
-            if result_queue is not None:
-                result_queue.put('\n>>>>> R{}/S{}  particle params: {}  calibrated params: {}\n'.format(r + 1, s + 1, param_names, args['calib_params']))
+            #if result_queue is not None:
+            #    result_queue.put('\n>>>>> R{}/S{}  particle params: {}  calibrated params: {}\n'.format(r + 1, s + 1, param_names, args['calib_params']))
+            
+            print("Filled request queue...")
             
             args['rnd'] = r + 1
             args['step'] = s + 1
 
+            print("Evaluating cost...")
+
             # perform optimization
             cost, pos = optimizer[s].optimize(eval_cost, iters=step.get('iters', iters), **args)
             if cost is None:
                 early_exit = True
                 break
 
+            print("Finished evaluation...")
+
             # capture the best cost
             # if cost < best_cost[s] and np.abs(cost - best_cost[s]) > rtol:
             if cost < best_cost[s]:
                 best_cost[s] = cost
                 no_improvement[s] = False
                 utils.annotate_step(best_cost[s], pos, steps, s)
```

### Comparing `mg-pso-gui-0.1.96/mgpsogui/util/recosu/utils/plot/cost_steps.py` & `mg-pso-gui-0.1.97/mgpsogui/util/recosu/utils/plot/cost_steps.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.96/mgpsogui/util/recosu/utils/trace_writer.py` & `mg-pso-gui-0.1.97/mgpsogui/util/recosu/utils/trace_writer.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.96/mgpsogui/util/recosu/utils/utils.py` & `mg-pso-gui-0.1.97/mgpsogui/util/recosu/utils/utils.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.96/setup.py` & `mg-pso-gui-0.1.97/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.1.96'
+VERSION = '0.1.97'
 DESCRIPTION = 'GUI for MG-PSO'
 LONG_DESCRIPTION = open('../README.md').read()
 
 # Setting up
 setup(
     name="mg-pso-gui",
     version=VERSION,
```

