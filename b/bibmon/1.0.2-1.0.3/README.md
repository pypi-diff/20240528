# Comparing `tmp/bibmon-1.0.2.tar.gz` & `tmp/bibmon-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bibmon-1.0.2.tar", last modified: Thu May 23 19:59:19 2024, max compression
+gzip compressed data, was "bibmon-1.0.3.tar", last modified: Tue May 28 18:02:25 2024, max compression
```

## Comparing `bibmon-1.0.2.tar` & `bibmon-1.0.3.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 19:59:19.542899 bibmon-1.0.2/
--rw-rw-rw-   0        0        0    11554 2024-05-23 18:28:30.000000 bibmon-1.0.2/LICENSE.md
--rw-rw-rw-   0        0        0     3604 2024-05-23 19:59:19.542899 bibmon-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3248 2024-05-23 18:28:30.000000 bibmon-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 19:59:18.835799 bibmon-1.0.2/bibmon/
--rw-rw-rw-   0        0        0      647 2024-05-23 18:28:30.000000 bibmon-1.0.2/bibmon/__init__.py
--rw-rw-rw-   0        0        0     1357 2024-05-23 18:28:30.000000 bibmon-1.0.2/bibmon/_alarms.py
--rw-rw-rw-   0        0        0    26808 2024-05-23 18:28:30.000000 bibmon-1.0.2/bibmon/_bibmon_tools.py
--rw-rw-rw-   0        0        0    41603 2024-05-23 18:28:30.000000 bibmon-1.0.2/bibmon/_generic_model.py
--rw-rw-rw-   0        0        0     2953 2024-05-23 19:25:42.000000 bibmon-1.0.2/bibmon/_load_data.py
--rw-rw-rw-   0        0        0     3941 2024-05-23 18:28:30.000000 bibmon-1.0.2/bibmon/_pca.py
--rw-rw-rw-   0        0        0    12716 2024-05-23 18:28:30.000000 bibmon-1.0.2/bibmon/_preprocess.py
--rw-rw-rw-   0        0        0     5359 2024-05-23 18:28:30.000000 bibmon-1.0.2/bibmon/_sklearn_regressor.py
--rw-rw-rw-   0        0        0     2922 2024-05-23 18:28:30.000000 bibmon-1.0.2/bibmon/_template_generic_model_childs.py
-drwxrwxrwx   0        0        0        0 2024-05-23 19:59:18.882756 bibmon-1.0.2/bibmon/real_process_data/
--rw-rw-rw-   0        0        0        0 2024-05-23 19:26:32.000000 bibmon-1.0.2/bibmon/real_process_data/__init__.py
--rw-rw-rw-   0        0        0  2459724 2024-05-23 18:28:30.000000 bibmon-1.0.2/bibmon/real_process_data/real_process_data.csv
-drwxrwxrwx   0        0        0        0 2024-05-23 19:59:19.511623 bibmon-1.0.2/bibmon/tennessee_eastman/
--rw-rw-rw-   0        0        0        0 2024-05-23 19:26:32.000000 bibmon-1.0.2/bibmon/tennessee_eastman/__init__.py
--rw-rw-rw-   0        0        0   416101 2024-05-23 18:28:30.000000 bibmon-1.0.2/bibmon/tennessee_eastman/d00.dat
--rw-rw-rw-   0        0        0   800640 2024-05-23 18:28:30.000000 bibmon-1.0.2/bibmon/tennessee_eastman/d00_te.dat
--rw-rw-rw-   0        0        0   400320 2024-05-23 18:28:30.000000 bibmon-1.0.2/bibmon/tennessee_eastman/d01.dat
--rw-rw-rw-   0        0        0   800640 2024-05-23 18:28:30.000000 bibmon-1.0.2/bibmon/tennessee_eastman/d01_te.dat
--rw-rw-rw-   0        0        0   400320 2024-05-23 18:28:30.000000 bibmon-1.0.2/bibmon/tennessee_eastman/d02.dat
--rw-rw-rw-   0        0        0   800640 2024-05-23 18:28:30.000000 bibmon-1.0.2/bibmon/tennessee_eastman/d02_te.dat
--rw-rw-rw-   0        0        0   400320 2024-05-23 18:28:30.000000 bibmon-1.0.2/bibmon/tennessee_eastman/d03.dat
--rw-rw-rw-   0        0        0   800640 2024-05-23 18:28:30.000000 bibmon-1.0.2/bibmon/tennessee_eastman/d03_te.dat
--rw-rw-rw-   0        0        0   400320 2024-05-23 18:28:30.000000 bibmon-1.0.2/bibmon/tennessee_eastman/d04.dat
--rw-rw-rw-   0        0        0   800640 2024-05-23 18:28:30.000000 bibmon-1.0.2/bibmon/tennessee_eastman/d04_te.dat
--rw-rw-rw-   0        0        0   400320 2024-05-23 18:28:30.000000 bibmon-1.0.2/bibmon/tennessee_eastman/d05.dat
--rw-rw-rw-   0        0        0   800640 2024-05-23 18:28:30.000000 bibmon-1.0.2/bibmon/tennessee_eastman/d05_te.dat
--rw-rw-rw-   0        0        0   400320 2024-05-23 18:28:30.000000 bibmon-1.0.2/bibmon/tennessee_eastman/d06.dat
--rw-rw-rw-   0        0        0   800640 2024-05-23 18:28:30.000000 bibmon-1.0.2/bibmon/tennessee_eastman/d06_te.dat
--rw-rw-rw-   0        0        0   400320 2024-05-23 18:28:30.000000 bibmon-1.0.2/bibmon/tennessee_eastman/d07.dat
--rw-rw-rw-   0        0        0   800640 2024-05-23 18:28:30.000000 bibmon-1.0.2/bibmon/tennessee_eastman/d07_te.dat
--rw-rw-rw-   0        0        0   400320 2024-05-23 18:28:30.000000 bibmon-1.0.2/bibmon/tennessee_eastman/d08.dat
--rw-rw-rw-   0        0        0   800640 2024-05-23 18:28:30.000000 bibmon-1.0.2/bibmon/tennessee_eastman/d08_te.dat
--rw-rw-rw-   0        0        0   400320 2024-05-23 18:28:30.000000 bibmon-1.0.2/bibmon/tennessee_eastman/d09.dat
--rw-rw-rw-   0        0        0   800640 2024-05-23 18:28:30.000000 bibmon-1.0.2/bibmon/tennessee_eastman/d09_te.dat
--rw-rw-rw-   0        0        0   400320 2024-05-23 18:28:30.000000 bibmon-1.0.2/bibmon/tennessee_eastman/d10.dat
--rw-rw-rw-   0        0        0   800640 2024-05-23 18:28:30.000000 bibmon-1.0.2/bibmon/tennessee_eastman/d10_te.dat
--rw-rw-rw-   0        0        0   400320 2024-05-23 18:28:30.000000 bibmon-1.0.2/bibmon/tennessee_eastman/d11.dat
--rw-rw-rw-   0        0        0   800640 2024-05-23 18:28:30.000000 bibmon-1.0.2/bibmon/tennessee_eastman/d11_te.dat
--rw-rw-rw-   0        0        0   400320 2024-05-23 18:28:30.000000 bibmon-1.0.2/bibmon/tennessee_eastman/d12.dat
--rw-rw-rw-   0        0        0   800640 2024-05-23 18:28:30.000000 bibmon-1.0.2/bibmon/tennessee_eastman/d12_te.dat
--rw-rw-rw-   0        0        0   400320 2024-05-23 18:28:30.000000 bibmon-1.0.2/bibmon/tennessee_eastman/d13.dat
--rw-rw-rw-   0        0        0   800640 2024-05-23 18:28:30.000000 bibmon-1.0.2/bibmon/tennessee_eastman/d13_te.dat
--rw-rw-rw-   0        0        0   400320 2024-05-23 18:28:30.000000 bibmon-1.0.2/bibmon/tennessee_eastman/d14.dat
--rw-rw-rw-   0        0        0   800640 2024-05-23 18:28:30.000000 bibmon-1.0.2/bibmon/tennessee_eastman/d14_te.dat
--rw-rw-rw-   0        0        0   400320 2024-05-23 18:28:30.000000 bibmon-1.0.2/bibmon/tennessee_eastman/d15.dat
--rw-rw-rw-   0        0        0   800640 2024-05-23 18:28:30.000000 bibmon-1.0.2/bibmon/tennessee_eastman/d15_te.dat
--rw-rw-rw-   0        0        0   400320 2024-05-23 18:28:30.000000 bibmon-1.0.2/bibmon/tennessee_eastman/d16.dat
--rw-rw-rw-   0        0        0   800640 2024-05-23 18:28:30.000000 bibmon-1.0.2/bibmon/tennessee_eastman/d16_te.dat
--rw-rw-rw-   0        0        0   400320 2024-05-23 18:28:30.000000 bibmon-1.0.2/bibmon/tennessee_eastman/d17.dat
--rw-rw-rw-   0        0        0   800640 2024-05-23 18:28:30.000000 bibmon-1.0.2/bibmon/tennessee_eastman/d17_te.dat
--rw-rw-rw-   0        0        0   400320 2024-05-23 18:28:30.000000 bibmon-1.0.2/bibmon/tennessee_eastman/d18.dat
--rw-rw-rw-   0        0        0   800640 2024-05-23 18:28:30.000000 bibmon-1.0.2/bibmon/tennessee_eastman/d18_te.dat
--rw-rw-rw-   0        0        0   400320 2024-05-23 18:28:30.000000 bibmon-1.0.2/bibmon/tennessee_eastman/d19.dat
--rw-rw-rw-   0        0        0   800640 2024-05-23 18:28:30.000000 bibmon-1.0.2/bibmon/tennessee_eastman/d19_te.dat
--rw-rw-rw-   0        0        0   400320 2024-05-23 18:28:30.000000 bibmon-1.0.2/bibmon/tennessee_eastman/d20.dat
--rw-rw-rw-   0        0        0   800640 2024-05-23 18:28:30.000000 bibmon-1.0.2/bibmon/tennessee_eastman/d20_te.dat
--rw-rw-rw-   0        0        0   400320 2024-05-23 18:28:30.000000 bibmon-1.0.2/bibmon/tennessee_eastman/d21.dat
--rw-rw-rw-   0        0        0   800640 2024-05-23 18:28:30.000000 bibmon-1.0.2/bibmon/tennessee_eastman/d21_te.dat
-drwxrwxrwx   0        0        0        0 2024-05-23 19:59:18.882756 bibmon-1.0.2/bibmon.egg-info/
--rw-rw-rw-   0        0        0     3604 2024-05-23 19:59:18.000000 bibmon-1.0.2/bibmon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2094 2024-05-23 19:59:18.000000 bibmon-1.0.2/bibmon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 19:59:18.000000 bibmon-1.0.2/bibmon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      130 2024-05-23 19:59:18.000000 bibmon-1.0.2/bibmon.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-23 19:59:18.000000 bibmon-1.0.2/bibmon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 19:59:19.542899 bibmon-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1066 2024-05-23 19:54:03.000000 bibmon-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-23 19:59:19.542899 bibmon-1.0.2/test/
--rw-rw-rw-   0        0        0     8977 2024-05-23 18:28:30.000000 bibmon-1.0.2/test/test_models.py
--rw-rw-rw-   0        0        0     2160 2024-05-23 18:28:30.000000 bibmon-1.0.2/test/test_preprocess.py
--rw-rw-rw-   0        0        0     2340 2024-05-23 18:28:30.000000 bibmon-1.0.2/test/test_tools.py
+drwxrwxrwx   0        0        0        0 2024-05-28 18:02:25.962204 bibmon-1.0.3/
+-rw-rw-rw-   0        0        0    11554 2024-05-23 18:28:30.000000 bibmon-1.0.3/LICENSE.md
+-rw-rw-rw-   0        0        0     3704 2024-05-28 18:02:25.959653 bibmon-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3350 2024-05-28 18:01:12.000000 bibmon-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 18:02:25.018430 bibmon-1.0.3/bibmon/
+-rw-rw-rw-   0        0        0      647 2024-05-23 18:28:30.000000 bibmon-1.0.3/bibmon/__init__.py
+-rw-rw-rw-   0        0        0     1357 2024-05-23 18:28:30.000000 bibmon-1.0.3/bibmon/_alarms.py
+-rw-rw-rw-   0        0        0    26808 2024-05-23 18:28:30.000000 bibmon-1.0.3/bibmon/_bibmon_tools.py
+-rw-rw-rw-   0        0        0    41603 2024-05-23 18:28:30.000000 bibmon-1.0.3/bibmon/_generic_model.py
+-rw-rw-rw-   0        0        0     2953 2024-05-23 19:25:42.000000 bibmon-1.0.3/bibmon/_load_data.py
+-rw-rw-rw-   0        0        0     3941 2024-05-23 18:28:30.000000 bibmon-1.0.3/bibmon/_pca.py
+-rw-rw-rw-   0        0        0    12716 2024-05-23 18:28:30.000000 bibmon-1.0.3/bibmon/_preprocess.py
+-rw-rw-rw-   0        0        0     5359 2024-05-23 18:28:30.000000 bibmon-1.0.3/bibmon/_sklearn_regressor.py
+-rw-rw-rw-   0        0        0     2922 2024-05-23 18:28:30.000000 bibmon-1.0.3/bibmon/_template_generic_model_childs.py
+drwxrwxrwx   0        0        0        0 2024-05-28 18:02:25.081566 bibmon-1.0.3/bibmon/real_process_data/
+-rw-rw-rw-   0        0        0        0 2024-05-23 19:26:32.000000 bibmon-1.0.3/bibmon/real_process_data/__init__.py
+-rw-rw-rw-   0        0        0  2459724 2024-05-23 18:28:30.000000 bibmon-1.0.3/bibmon/real_process_data/real_process_data.csv
+drwxrwxrwx   0        0        0        0 2024-05-28 18:02:25.906519 bibmon-1.0.3/bibmon/tennessee_eastman/
+-rw-rw-rw-   0        0        0        0 2024-05-23 19:26:32.000000 bibmon-1.0.3/bibmon/tennessee_eastman/__init__.py
+-rw-rw-rw-   0        0        0   416101 2024-05-23 18:28:30.000000 bibmon-1.0.3/bibmon/tennessee_eastman/d00.dat
+-rw-rw-rw-   0        0        0   800640 2024-05-23 18:28:30.000000 bibmon-1.0.3/bibmon/tennessee_eastman/d00_te.dat
+-rw-rw-rw-   0        0        0   400320 2024-05-23 18:28:30.000000 bibmon-1.0.3/bibmon/tennessee_eastman/d01.dat
+-rw-rw-rw-   0        0        0   800640 2024-05-23 18:28:30.000000 bibmon-1.0.3/bibmon/tennessee_eastman/d01_te.dat
+-rw-rw-rw-   0        0        0   400320 2024-05-23 18:28:30.000000 bibmon-1.0.3/bibmon/tennessee_eastman/d02.dat
+-rw-rw-rw-   0        0        0   800640 2024-05-23 18:28:30.000000 bibmon-1.0.3/bibmon/tennessee_eastman/d02_te.dat
+-rw-rw-rw-   0        0        0   400320 2024-05-23 18:28:30.000000 bibmon-1.0.3/bibmon/tennessee_eastman/d03.dat
+-rw-rw-rw-   0        0        0   800640 2024-05-23 18:28:30.000000 bibmon-1.0.3/bibmon/tennessee_eastman/d03_te.dat
+-rw-rw-rw-   0        0        0   400320 2024-05-23 18:28:30.000000 bibmon-1.0.3/bibmon/tennessee_eastman/d04.dat
+-rw-rw-rw-   0        0        0   800640 2024-05-23 18:28:30.000000 bibmon-1.0.3/bibmon/tennessee_eastman/d04_te.dat
+-rw-rw-rw-   0        0        0   400320 2024-05-23 18:28:30.000000 bibmon-1.0.3/bibmon/tennessee_eastman/d05.dat
+-rw-rw-rw-   0        0        0   800640 2024-05-23 18:28:30.000000 bibmon-1.0.3/bibmon/tennessee_eastman/d05_te.dat
+-rw-rw-rw-   0        0        0   400320 2024-05-23 18:28:30.000000 bibmon-1.0.3/bibmon/tennessee_eastman/d06.dat
+-rw-rw-rw-   0        0        0   800640 2024-05-23 18:28:30.000000 bibmon-1.0.3/bibmon/tennessee_eastman/d06_te.dat
+-rw-rw-rw-   0        0        0   400320 2024-05-23 18:28:30.000000 bibmon-1.0.3/bibmon/tennessee_eastman/d07.dat
+-rw-rw-rw-   0        0        0   800640 2024-05-23 18:28:30.000000 bibmon-1.0.3/bibmon/tennessee_eastman/d07_te.dat
+-rw-rw-rw-   0        0        0   400320 2024-05-23 18:28:30.000000 bibmon-1.0.3/bibmon/tennessee_eastman/d08.dat
+-rw-rw-rw-   0        0        0   800640 2024-05-23 18:28:30.000000 bibmon-1.0.3/bibmon/tennessee_eastman/d08_te.dat
+-rw-rw-rw-   0        0        0   400320 2024-05-23 18:28:30.000000 bibmon-1.0.3/bibmon/tennessee_eastman/d09.dat
+-rw-rw-rw-   0        0        0   800640 2024-05-23 18:28:30.000000 bibmon-1.0.3/bibmon/tennessee_eastman/d09_te.dat
+-rw-rw-rw-   0        0        0   400320 2024-05-23 18:28:30.000000 bibmon-1.0.3/bibmon/tennessee_eastman/d10.dat
+-rw-rw-rw-   0        0        0   800640 2024-05-23 18:28:30.000000 bibmon-1.0.3/bibmon/tennessee_eastman/d10_te.dat
+-rw-rw-rw-   0        0        0   400320 2024-05-23 18:28:30.000000 bibmon-1.0.3/bibmon/tennessee_eastman/d11.dat
+-rw-rw-rw-   0        0        0   800640 2024-05-23 18:28:30.000000 bibmon-1.0.3/bibmon/tennessee_eastman/d11_te.dat
+-rw-rw-rw-   0        0        0   400320 2024-05-23 18:28:30.000000 bibmon-1.0.3/bibmon/tennessee_eastman/d12.dat
+-rw-rw-rw-   0        0        0   800640 2024-05-23 18:28:30.000000 bibmon-1.0.3/bibmon/tennessee_eastman/d12_te.dat
+-rw-rw-rw-   0        0        0   400320 2024-05-23 18:28:30.000000 bibmon-1.0.3/bibmon/tennessee_eastman/d13.dat
+-rw-rw-rw-   0        0        0   800640 2024-05-23 18:28:30.000000 bibmon-1.0.3/bibmon/tennessee_eastman/d13_te.dat
+-rw-rw-rw-   0        0        0   400320 2024-05-23 18:28:30.000000 bibmon-1.0.3/bibmon/tennessee_eastman/d14.dat
+-rw-rw-rw-   0        0        0   800640 2024-05-23 18:28:30.000000 bibmon-1.0.3/bibmon/tennessee_eastman/d14_te.dat
+-rw-rw-rw-   0        0        0   400320 2024-05-23 18:28:30.000000 bibmon-1.0.3/bibmon/tennessee_eastman/d15.dat
+-rw-rw-rw-   0        0        0   800640 2024-05-23 18:28:30.000000 bibmon-1.0.3/bibmon/tennessee_eastman/d15_te.dat
+-rw-rw-rw-   0        0        0   400320 2024-05-23 18:28:30.000000 bibmon-1.0.3/bibmon/tennessee_eastman/d16.dat
+-rw-rw-rw-   0        0        0   800640 2024-05-23 18:28:30.000000 bibmon-1.0.3/bibmon/tennessee_eastman/d16_te.dat
+-rw-rw-rw-   0        0        0   400320 2024-05-23 18:28:30.000000 bibmon-1.0.3/bibmon/tennessee_eastman/d17.dat
+-rw-rw-rw-   0        0        0   800640 2024-05-23 18:28:30.000000 bibmon-1.0.3/bibmon/tennessee_eastman/d17_te.dat
+-rw-rw-rw-   0        0        0   400320 2024-05-23 18:28:30.000000 bibmon-1.0.3/bibmon/tennessee_eastman/d18.dat
+-rw-rw-rw-   0        0        0   800640 2024-05-23 18:28:30.000000 bibmon-1.0.3/bibmon/tennessee_eastman/d18_te.dat
+-rw-rw-rw-   0        0        0   400320 2024-05-23 18:28:30.000000 bibmon-1.0.3/bibmon/tennessee_eastman/d19.dat
+-rw-rw-rw-   0        0        0   800640 2024-05-23 18:28:30.000000 bibmon-1.0.3/bibmon/tennessee_eastman/d19_te.dat
+-rw-rw-rw-   0        0        0   400320 2024-05-23 18:28:30.000000 bibmon-1.0.3/bibmon/tennessee_eastman/d20.dat
+-rw-rw-rw-   0        0        0   800640 2024-05-23 18:28:30.000000 bibmon-1.0.3/bibmon/tennessee_eastman/d20_te.dat
+-rw-rw-rw-   0        0        0   400320 2024-05-23 18:28:30.000000 bibmon-1.0.3/bibmon/tennessee_eastman/d21.dat
+-rw-rw-rw-   0        0        0   800640 2024-05-23 18:28:30.000000 bibmon-1.0.3/bibmon/tennessee_eastman/d21_te.dat
+drwxrwxrwx   0        0        0        0 2024-05-28 18:02:25.066373 bibmon-1.0.3/bibmon.egg-info/
+-rw-rw-rw-   0        0        0     3704 2024-05-28 18:02:24.000000 bibmon-1.0.3/bibmon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2094 2024-05-28 18:02:24.000000 bibmon-1.0.3/bibmon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 18:02:24.000000 bibmon-1.0.3/bibmon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      130 2024-05-28 18:02:24.000000 bibmon-1.0.3/bibmon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-28 18:02:24.000000 bibmon-1.0.3/bibmon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 18:02:25.962204 bibmon-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1093 2024-05-28 18:01:36.000000 bibmon-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 18:02:25.956222 bibmon-1.0.3/test/
+-rw-rw-rw-   0        0        0     8977 2024-05-23 18:28:30.000000 bibmon-1.0.3/test/test_models.py
+-rw-rw-rw-   0        0        0     2160 2024-05-23 18:28:30.000000 bibmon-1.0.3/test/test_preprocess.py
+-rw-rw-rw-   0        0        0     2340 2024-05-23 18:28:30.000000 bibmon-1.0.3/test/test_tools.py
```

### Comparing `bibmon-1.0.2/LICENSE.md` & `bibmon-1.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/PKG-INFO` & `bibmon-1.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: bibmon
-Version: 1.0.2
+Version: 1.0.3
 Summary: Library with routines for data-driven process monitoring.
 Home-page: https://github.com/petrobras/bibmon
 Author: BibMon developers
 Author-email: cc-bibmon@petrobras.com.br
 License: Apache 2.0
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/petrobras/BibMon/HEAD)
 [![Apache 2.0][apache-shield]][apache] 
 [![CC BY 4.0][cc-by-shield]][cc-by]
 
 [apache]: https://opensource.org/licenses/Apache-2.0
 [apache-shield]: https://img.shields.io/badge/License-Apache_2.0-blue.svg
 [cc-by]: http://creativecommons.org/licenses/by/4.0/
 [cc-by-shield]: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg
```

### Comparing `bibmon-1.0.2/README.md` & `bibmon-1.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/petrobras/BibMon/HEAD)
 [![Apache 2.0][apache-shield]][apache] 
 [![CC BY 4.0][cc-by-shield]][cc-by]
 
 [apache]: https://opensource.org/licenses/Apache-2.0
 [apache-shield]: https://img.shields.io/badge/License-Apache_2.0-blue.svg
 [cc-by]: http://creativecommons.org/licenses/by/4.0/
 [cc-by-shield]: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg
@@ -51,8 +52,8 @@
 * Automatic hyperparameter tuning.
 
 Contributing
 ----------------------
 
 BibMon is an open-source project driven by the community. If you would like to contribute to the project, please refer to the [CONTRIBUTING.md](https://github.com/petrobras/bibmon/blob/main/CONTRIBUTING.md) file.
 
-The package originated from research projects conducted in collaboration between the Chemical Engineering Program at COPPE/UFRJ and the Leopoldo Américo Miguez de Mello Research Center (CENPES/Petrobras).
+The package originated from research projects conducted in collaboration between the Chemical Engineering Program at COPPE/UFRJ and the Leopoldo Américo Miguez de Mello Research Center (CENPES/Petrobras).
```

### Comparing `bibmon-1.0.2/bibmon/__init__.py` & `bibmon-1.0.3/bibmon/__init__.py`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/bibmon/_alarms.py` & `bibmon-1.0.3/bibmon/_alarms.py`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/bibmon/_bibmon_tools.py` & `bibmon-1.0.3/bibmon/_bibmon_tools.py`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/bibmon/_generic_model.py` & `bibmon-1.0.3/bibmon/_generic_model.py`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/bibmon/_load_data.py` & `bibmon-1.0.3/bibmon/_load_data.py`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/bibmon/_pca.py` & `bibmon-1.0.3/bibmon/_pca.py`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/bibmon/_preprocess.py` & `bibmon-1.0.3/bibmon/_preprocess.py`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/bibmon/_sklearn_regressor.py` & `bibmon-1.0.3/bibmon/_sklearn_regressor.py`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/bibmon/_template_generic_model_childs.py` & `bibmon-1.0.3/bibmon/_template_generic_model_childs.py`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/bibmon/real_process_data/real_process_data.csv` & `bibmon-1.0.3/bibmon/real_process_data/real_process_data.csv`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/bibmon/tennessee_eastman/d00.dat` & `bibmon-1.0.3/bibmon/tennessee_eastman/d00.dat`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/bibmon/tennessee_eastman/d00_te.dat` & `bibmon-1.0.3/bibmon/tennessee_eastman/d00_te.dat`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/bibmon/tennessee_eastman/d01.dat` & `bibmon-1.0.3/bibmon/tennessee_eastman/d01.dat`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/bibmon/tennessee_eastman/d01_te.dat` & `bibmon-1.0.3/bibmon/tennessee_eastman/d01_te.dat`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/bibmon/tennessee_eastman/d02.dat` & `bibmon-1.0.3/bibmon/tennessee_eastman/d02.dat`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/bibmon/tennessee_eastman/d02_te.dat` & `bibmon-1.0.3/bibmon/tennessee_eastman/d02_te.dat`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/bibmon/tennessee_eastman/d03.dat` & `bibmon-1.0.3/bibmon/tennessee_eastman/d03.dat`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/bibmon/tennessee_eastman/d03_te.dat` & `bibmon-1.0.3/bibmon/tennessee_eastman/d03_te.dat`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/bibmon/tennessee_eastman/d04.dat` & `bibmon-1.0.3/bibmon/tennessee_eastman/d04.dat`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/bibmon/tennessee_eastman/d04_te.dat` & `bibmon-1.0.3/bibmon/tennessee_eastman/d04_te.dat`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/bibmon/tennessee_eastman/d05.dat` & `bibmon-1.0.3/bibmon/tennessee_eastman/d05.dat`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/bibmon/tennessee_eastman/d05_te.dat` & `bibmon-1.0.3/bibmon/tennessee_eastman/d05_te.dat`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/bibmon/tennessee_eastman/d06.dat` & `bibmon-1.0.3/bibmon/tennessee_eastman/d06.dat`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/bibmon/tennessee_eastman/d06_te.dat` & `bibmon-1.0.3/bibmon/tennessee_eastman/d06_te.dat`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/bibmon/tennessee_eastman/d07.dat` & `bibmon-1.0.3/bibmon/tennessee_eastman/d07.dat`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/bibmon/tennessee_eastman/d07_te.dat` & `bibmon-1.0.3/bibmon/tennessee_eastman/d07_te.dat`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/bibmon/tennessee_eastman/d08.dat` & `bibmon-1.0.3/bibmon/tennessee_eastman/d08.dat`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/bibmon/tennessee_eastman/d08_te.dat` & `bibmon-1.0.3/bibmon/tennessee_eastman/d08_te.dat`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/bibmon/tennessee_eastman/d09.dat` & `bibmon-1.0.3/bibmon/tennessee_eastman/d09.dat`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/bibmon/tennessee_eastman/d09_te.dat` & `bibmon-1.0.3/bibmon/tennessee_eastman/d09_te.dat`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/bibmon/tennessee_eastman/d10.dat` & `bibmon-1.0.3/bibmon/tennessee_eastman/d10.dat`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/bibmon/tennessee_eastman/d10_te.dat` & `bibmon-1.0.3/bibmon/tennessee_eastman/d10_te.dat`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/bibmon/tennessee_eastman/d11.dat` & `bibmon-1.0.3/bibmon/tennessee_eastman/d11.dat`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/bibmon/tennessee_eastman/d11_te.dat` & `bibmon-1.0.3/bibmon/tennessee_eastman/d11_te.dat`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/bibmon/tennessee_eastman/d12.dat` & `bibmon-1.0.3/bibmon/tennessee_eastman/d12.dat`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/bibmon/tennessee_eastman/d12_te.dat` & `bibmon-1.0.3/bibmon/tennessee_eastman/d12_te.dat`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/bibmon/tennessee_eastman/d13.dat` & `bibmon-1.0.3/bibmon/tennessee_eastman/d13.dat`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/bibmon/tennessee_eastman/d13_te.dat` & `bibmon-1.0.3/bibmon/tennessee_eastman/d13_te.dat`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/bibmon/tennessee_eastman/d14.dat` & `bibmon-1.0.3/bibmon/tennessee_eastman/d14.dat`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/bibmon/tennessee_eastman/d14_te.dat` & `bibmon-1.0.3/bibmon/tennessee_eastman/d14_te.dat`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/bibmon/tennessee_eastman/d15.dat` & `bibmon-1.0.3/bibmon/tennessee_eastman/d15.dat`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/bibmon/tennessee_eastman/d15_te.dat` & `bibmon-1.0.3/bibmon/tennessee_eastman/d15_te.dat`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/bibmon/tennessee_eastman/d16.dat` & `bibmon-1.0.3/bibmon/tennessee_eastman/d16.dat`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/bibmon/tennessee_eastman/d16_te.dat` & `bibmon-1.0.3/bibmon/tennessee_eastman/d16_te.dat`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/bibmon/tennessee_eastman/d17.dat` & `bibmon-1.0.3/bibmon/tennessee_eastman/d17.dat`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/bibmon/tennessee_eastman/d17_te.dat` & `bibmon-1.0.3/bibmon/tennessee_eastman/d17_te.dat`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/bibmon/tennessee_eastman/d18.dat` & `bibmon-1.0.3/bibmon/tennessee_eastman/d18.dat`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/bibmon/tennessee_eastman/d18_te.dat` & `bibmon-1.0.3/bibmon/tennessee_eastman/d18_te.dat`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/bibmon/tennessee_eastman/d19.dat` & `bibmon-1.0.3/bibmon/tennessee_eastman/d19.dat`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/bibmon/tennessee_eastman/d19_te.dat` & `bibmon-1.0.3/bibmon/tennessee_eastman/d19_te.dat`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/bibmon/tennessee_eastman/d20.dat` & `bibmon-1.0.3/bibmon/tennessee_eastman/d20.dat`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/bibmon/tennessee_eastman/d20_te.dat` & `bibmon-1.0.3/bibmon/tennessee_eastman/d20_te.dat`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/bibmon/tennessee_eastman/d21.dat` & `bibmon-1.0.3/bibmon/tennessee_eastman/d21.dat`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/bibmon/tennessee_eastman/d21_te.dat` & `bibmon-1.0.3/bibmon/tennessee_eastman/d21_te.dat`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/bibmon.egg-info/PKG-INFO` & `bibmon-1.0.3/bibmon.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: bibmon
-Version: 1.0.2
+Version: 1.0.3
 Summary: Library with routines for data-driven process monitoring.
 Home-page: https://github.com/petrobras/bibmon
 Author: BibMon developers
 Author-email: cc-bibmon@petrobras.com.br
 License: Apache 2.0
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/petrobras/BibMon/HEAD)
 [![Apache 2.0][apache-shield]][apache] 
 [![CC BY 4.0][cc-by-shield]][cc-by]
 
 [apache]: https://opensource.org/licenses/Apache-2.0
 [apache-shield]: https://img.shields.io/badge/License-Apache_2.0-blue.svg
 [cc-by]: http://creativecommons.org/licenses/by/4.0/
 [cc-by-shield]: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg
```

### Comparing `bibmon-1.0.2/bibmon.egg-info/SOURCES.txt` & `bibmon-1.0.3/bibmon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/setup.py` & `bibmon-1.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,27 +8,30 @@
 
 import setuptools
 import os
 
 with open('README.md') as f:
     README = f.read()
     
-requirements = os.path.dirname(os.path.realpath(__file__))+'/requirements.txt'
+requirements = os.path.join(
+    os.path.dirname(os.path.realpath(__file__)),
+    'requirements.txt'
+)
 
 if os.path.isfile(requirements):
     with open(requirements) as f:
         install_requires = f.read().splitlines()
 
 setuptools.setup(
     author="BibMon developers",
     author_email="cc-bibmon@petrobras.com.br",
     name='bibmon',
     description='Library with routines for data-driven process monitoring.',
     license='Apache 2.0',
-    version='1.0.2',
+    version='1.0.3',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://github.com/petrobras/bibmon',
     packages=setuptools.find_packages(include=['bibmon','bibmon.*']),
     include_package_data=True,
     package_data={
         'bibmon': ['real_process_data/*.csv','tennessee_eastman/*.dat'],
```

### Comparing `bibmon-1.0.2/test/test_models.py` & `bibmon-1.0.3/test/test_models.py`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/test/test_preprocess.py` & `bibmon-1.0.3/test/test_preprocess.py`

 * *Files identical despite different names*

### Comparing `bibmon-1.0.2/test/test_tools.py` & `bibmon-1.0.3/test/test_tools.py`

 * *Files identical despite different names*

