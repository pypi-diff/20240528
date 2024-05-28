# Comparing `tmp/UnitMatchPy-1.5b0.tar.gz` & `tmp/UnitMatchPy-1.5rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UnitMatchPy-1.5b0.tar", last modified: Fri May 17 15:35:29 2024, max compression
+gzip compressed data, was "UnitMatchPy-1.5rc0.tar", last modified: Tue May 28 11:43:58 2024, max compression
```

## Comparing `UnitMatchPy-1.5b0.tar` & `UnitMatchPy-1.5rc0.tar`

### file list

```diff
@@ -1,378 +1,378 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.840255 UnitMatchPy-1.5b0/
--rw-rw-rw-   0        0        0    21281 2023-12-13 15:09:14.000000 UnitMatchPy-1.5b0/LICENSE
--rw-rw-rw-   0        0        0       31 2024-05-17 15:23:47.000000 UnitMatchPy-1.5b0/MANIFEST.in
--rw-rw-rw-   0        0        0     2327 2024-05-17 15:35:29.839219 UnitMatchPy-1.5b0/PKG-INFO
--rw-rw-rw-   0        0        0     2053 2024-05-01 10:16:34.000000 UnitMatchPy-1.5b0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.350176 UnitMatchPy-1.5b0/UnitMatchPy/
--rw-rw-rw-   0        0        0     7288 2024-05-17 14:46:04.000000 UnitMatchPy-1.5b0/UnitMatchPy/AssignUniqueID.py
--rw-rw-rw-   0        0        0     2600 2024-05-01 13:35:22.000000 UnitMatchPy-1.5b0/UnitMatchPy/Bayes_fun.py
--rw-rw-rw-   0        0        0     8209 2024-05-01 13:35:20.000000 UnitMatchPy-1.5b0/UnitMatchPy/Extract_raw_data.py
--rw-rw-rw-   0        0        0    50507 2024-05-17 15:28:42.000000 UnitMatchPy-1.5b0/UnitMatchPy/GUI.py
--rw-rw-rw-   0        0        0    23396 2024-05-01 13:35:11.000000 UnitMatchPy-1.5b0/UnitMatchPy/Metrics_fun.py
--rw-rw-rw-   0        0        0     5258 2024-05-01 13:35:07.000000 UnitMatchPy-1.5b0/UnitMatchPy/Overlord.py
--rw-rw-rw-   0        0        0    13809 2024-05-01 13:35:03.000000 UnitMatchPy-1.5b0/UnitMatchPy/Param_fun.py
--rw-rw-rw-   0        0        0    13419 2024-05-01 13:34:57.000000 UnitMatchPy-1.5b0/UnitMatchPy/Save_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.294785 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.390803 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/
--rw-rw-rw-   0        0        0     2263 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/LICENSE
--rw-rw-rw-   0        0        0    15818 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/README.txt
--rw-rw-rw-   0        0        0     2097 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/awdark.tcl
--rw-rw-rw-   0        0        0     1881 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/awlight.tcl
--rw-rw-rw-   0        0        0     6815 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/awtemplate.tcl
--rw-rw-rw-   0        0        0     5137 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/awthemes.n7
--rw-rw-rw-   0        0        0   170232 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/awthemes.tcl
--rw-rw-rw-   0        0        0     3562 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/awwinxpblue.tcl
--rw-rw-rw-   0        0        0    10425 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/colorutils.tcl
--rw-rw-rw-   0        0        0     7022 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/demoscaled.tcl
--rw-rw-rw-   0        0        0     5311 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/demoscaledb.tcl
--rw-rw-rw-   0        0        0    42639 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/demottk.tcl
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.294785 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.392802 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/
--rw-rw-rw-   0        0        0     3066 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/README.txt
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.297370 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.400831 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/chevron/
--rw-rw-rw-   0        0        0     2614 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/chevron/arrow-down-d.svg
--rw-rw-rw-   0        0        0     2596 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/chevron/arrow-down-n-base.svg
--rw-rw-rw-   0        0        0     2608 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/chevron/arrow-down-n.svg
--rw-rw-rw-   0        0        0     2608 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/chevron/arrow-down-sn.svg
--rw-rw-rw-   0        0        0     2699 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/chevron/arrow-left-n.svg
--rw-rw-rw-   0        0        0     2703 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/chevron/arrow-right-n.svg
--rw-rw-rw-   0        0        0     2704 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/chevron/arrow-right-sn.svg
--rw-rw-rw-   0        0        0     2711 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/chevron/arrow-up-d.svg
--rw-rw-rw-   0        0        0     2703 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/chevron/arrow-up-n.svg
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.414919 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/open/
--rw-rw-rw-   0        0        0     2593 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/open/arrow-down-n-base.svg
--rw-rw-rw-   0        0        0     2686 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/open/arrow-down-n.svg
--rw-rw-rw-   0        0        0     2687 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/open/arrow-down-sn.svg
--rw-rw-rw-   0        0        0     2755 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/open/arrow-left-n.svg
--rw-rw-rw-   0        0        0     2757 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/open/arrow-right-n.svg
--rw-rw-rw-   0        0        0     2757 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/open/arrow-right-sn.svg
--rw-rw-rw-   0        0        0     2755 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/open/arrow-up-n.svg
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.425084 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid/
--rw-rw-rw-   0        0        0     2506 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid/arrow-down-n-base.svg
--rw-rw-rw-   0        0        0     2590 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid/arrow-down-n.svg
--rw-rw-rw-   0        0        0     2590 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid/arrow-down-sn.svg
--rw-rw-rw-   0        0        0     2660 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid/arrow-left-n.svg
--rw-rw-rw-   0        0        0     2662 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid/arrow-right-n.svg
--rw-rw-rw-   0        0        0     2636 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid/arrow-right-sn.svg
--rw-rw-rw-   0        0        0     2636 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid/arrow-up-n.svg
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.438429 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid-bg/
--rw-rw-rw-   0        0        0     2972 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid-bg/arrow-down-d.svg
--rw-rw-rw-   0        0        0     2966 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid-bg/arrow-down-n-base.svg
--rw-rw-rw-   0        0        0     2964 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid-bg/arrow-down-n.svg
--rw-rw-rw-   0        0        0     2969 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid-bg/arrow-left-d.svg
--rw-rw-rw-   0        0        0     2961 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid-bg/arrow-left-n.svg
--rw-rw-rw-   0        0        0     2968 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid-bg/arrow-right-d.svg
--rw-rw-rw-   0        0        0     2960 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid-bg/arrow-right-n.svg
--rw-rw-rw-   0        0        0     2967 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid-bg/arrow-up-d.svg
--rw-rw-rw-   0        0        0     2959 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid-bg/arrow-up-n.svg
--rw-rw-rw-   0        0        0       77 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid-bg/settings.tcl
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.302149 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.446768 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-accent-gradient/
--rw-rw-rw-   0        0        0     4016 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-accent-gradient/button-a.svg
--rw-rw-rw-   0        0        0     2984 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-accent-gradient/button-d.svg
--rw-rw-rw-   0        0        0     2993 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-accent-gradient/button-n.svg
--rw-rw-rw-   0        0        0     3013 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-accent-gradient/button-p.svg
--rw-rw-rw-   0        0        0       79 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-accent-gradient/settings.tcl
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.459028 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-flat/
--rw-rw-rw-   0        0        0     2161 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-flat/button-a.svg
--rw-rw-rw-   0        0        0     2195 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-flat/button-af-base.svg
--rw-rw-rw-   0        0        0     2160 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-flat/button-af.svg
--rw-rw-rw-   0        0        0     2169 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-flat/button-d.svg
--rw-rw-rw-   0        0        0     2160 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-flat/button-f.svg
--rw-rw-rw-   0        0        0     2197 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-flat/button-n.svg
--rw-rw-rw-   0        0        0     2160 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-flat/button-p.svg
--rw-rw-rw-   0        0        0      117 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-flat/settings.tcl
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.460603 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-gradient/
--rw-rw-rw-   0        0        0     3596 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-gradient/button-d.svg
--rw-rw-rw-   0        0        0     3573 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-gradient/button-n-base.svg
--rw-rw-rw-   0        0        0     3590 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-gradient/button-n.svg
--rw-rw-rw-   0        0        0       79 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-gradient/settings.tcl
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.305204 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.472602 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check/
--rw-rw-rw-   0        0        0     3260 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check/cb-sa-base.svg
--rw-rw-rw-   0        0        0     3244 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check/cb-sa.svg
--rw-rw-rw-   0        0        0     3198 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check/cb-sd.svg
--rw-rw-rw-   0        0        0     2772 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check/cb-sn-base.svg
--rw-rw-rw-   0        0        0     3203 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check/cb-sn.svg
--rw-rw-rw-   0        0        0     2199 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check/cb-ua.svg
--rw-rw-rw-   0        0        0     2200 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check/cb-ud.svg
--rw-rw-rw-   0        0        0     2202 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check/cb-un.svg
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.488618 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check-rev/
--rw-rw-rw-   0        0        0     3260 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check-rev/cb-sa-base.svg
--rw-rw-rw-   0        0        0     3243 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check-rev/cb-sa.svg
--rw-rw-rw-   0        0        0     3195 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check-rev/cb-sd.svg
--rw-rw-rw-   0        0        0     2772 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check-rev/cb-sn-base.svg
--rw-rw-rw-   0        0        0     3200 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check-rev/cb-sn.svg
--rw-rw-rw-   0        0        0     2199 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check-rev/cb-ua.svg
--rw-rw-rw-   0        0        0     2200 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check-rev/cb-ud.svg
--rw-rw-rw-   0        0        0     2202 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check-rev/cb-un.svg
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.500285 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-square/
--rw-rw-rw-   0        0        0     2460 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-square/cb-sa.svg
--rw-rw-rw-   0        0        0     2458 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-square/cb-sd.svg
--rw-rw-rw-   0        0        0     2443 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-square/cb-sn-base.svg
--rw-rw-rw-   0        0        0     2457 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-square/cb-sn.svg
--rw-rw-rw-   0        0        0     2187 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-square/cb-ua.svg
--rw-rw-rw-   0        0        0     2190 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-square/cb-ud.svg
--rw-rw-rw-   0        0        0     2186 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-square/cb-un.svg
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.506920 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/square-check-gradient/
--rw-rw-rw-   0        0        0     3929 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/square-check-gradient/cb-sd.svg
--rw-rw-rw-   0        0        0     3531 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/square-check-gradient/cb-sn-base.svg
--rw-rw-rw-   0        0        0     3930 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/square-check-gradient/cb-sn.svg
--rw-rw-rw-   0        0        0     2963 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/square-check-gradient/cb-ud.svg
--rw-rw-rw-   0        0        0     2957 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/square-check-gradient/cb-un.svg
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.514869 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/square-x/
--rw-rw-rw-   0        0        0     3079 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/square-x/cb-sd.svg
--rw-rw-rw-   0        0        0     2965 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/square-x/cb-sn-base.svg
--rw-rw-rw-   0        0        0     3073 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/square-x/cb-sn.svg
--rw-rw-rw-   0        0        0     2169 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/square-x/cb-ud.svg
--rw-rw-rw-   0        0        0     2165 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/square-x/cb-un.svg
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.307197 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.527780 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/rounded/
--rw-rw-rw-   0        0        0     3113 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/rounded/combo-arrow-down-d.svg
--rw-rw-rw-   0        0        0     3109 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/rounded/combo-arrow-down-n-base.svg
--rw-rw-rw-   0        0        0     3107 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/rounded/combo-arrow-down-n.svg
--rw-rw-rw-   0        0        0     2754 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/rounded/combo-entry-a.svg
--rw-rw-rw-   0        0        0     2756 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/rounded/combo-entry-d.svg
--rw-rw-rw-   0        0        0     2753 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/rounded/combo-entry-f.svg
--rw-rw-rw-   0        0        0     2760 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/rounded/combo-entry-n-base.svg
--rw-rw-rw-   0        0        0     2752 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/rounded/combo-entry-n.svg
--rw-rw-rw-   0        0        0       95 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/rounded/settings.tcl
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.535587 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/solid-bg/
--rw-rw-rw-   0        0        0     2861 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/solid-bg/combo-arrow-down-a.svg
--rw-rw-rw-   0        0        0     2796 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/solid-bg/combo-arrow-down-d-base.svg
--rw-rw-rw-   0        0        0     2882 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/solid-bg/combo-arrow-down-d.svg
--rw-rw-rw-   0        0        0     2890 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/solid-bg/combo-arrow-down-n-base.svg
--rw-rw-rw-   0        0        0     2870 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/solid-bg/combo-arrow-down-n.svg
--rw-rw-rw-   0        0        0       79 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/solid-bg/settings.tcl
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.308404 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/empty/
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.536587 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/empty/empty/
--rw-rw-rw-   0        0        0     1898 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/empty/empty/empty.svg
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.309424 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/entry/
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.545294 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/entry/roundedrect/
--rw-rw-rw-   0        0        0     2254 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/entry/roundedrect/entry-a.svg
--rw-rw-rw-   0        0        0     2256 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/entry/roundedrect/entry-d.svg
--rw-rw-rw-   0        0        0     2253 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/entry/roundedrect/entry-f.svg
--rw-rw-rw-   0        0        0     2283 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/entry/roundedrect/entry-n-base.svg
--rw-rw-rw-   0        0        0     2252 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/entry/roundedrect/entry-n.svg
--rw-rw-rw-   0        0        0       38 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/entry/roundedrect/settings.tcl
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.309424 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/labelframe/
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.547294 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/labelframe/square/
--rw-rw-rw-   0        0        0     2083 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/labelframe/square/labelframe-d.svg
--rw-rw-rw-   0        0        0     2081 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/labelframe/square/labelframe-n.svg
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.309424 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/menubutton/
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.554620 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/menubutton/chevron/
--rw-rw-rw-   0        0        0     2938 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/menubutton/chevron/mb-arrow-down-a.svg
--rw-rw-rw-   0        0        0     2933 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/menubutton/chevron/mb-arrow-down-d.svg
--rw-rw-rw-   0        0        0     2930 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/menubutton/chevron/mb-arrow-down-n-base.svg
--rw-rw-rw-   0        0        0     2923 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/menubutton/chevron/mb-arrow-down-n.svg
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.559407 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/menubutton/solid/
--rw-rw-rw-   0        0        0     2486 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/menubutton/solid/mb-arrow-down-d-base.svg
--rw-rw-rw-   0        0        0     2578 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/menubutton/solid/mb-arrow-down-d.svg
--rw-rw-rw-   0        0        0     2480 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/menubutton/solid/mb-arrow-down-n-base.svg
--rw-rw-rw-   0        0        0     2567 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/menubutton/solid/mb-arrow-down-n.svg
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.313812 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.569079 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-dark/
--rw-rw-rw-   0        0        0     2762 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-dark/notebook-tab-a.svg
--rw-rw-rw-   0        0        0     2768 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-dark/notebook-tab-d.svg
--rw-rw-rw-   0        0        0     2773 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-dark/notebook-tab-h.svg
--rw-rw-rw-   0        0        0     2773 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-dark/notebook-tab-i-base.svg
--rw-rw-rw-   0        0        0     2768 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-dark/notebook-tab-i.svg
--rw-rw-rw-   0        0        0       71 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-dark/settings.tcl
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.578172 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light/
--rw-rw-rw-   0        0        0     2762 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light/notebook-tab-a.svg
--rw-rw-rw-   0        0        0     2771 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light/notebook-tab-d.svg
--rw-rw-rw-   0        0        0     2773 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light/notebook-tab-h.svg
--rw-rw-rw-   0        0        0     2773 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light/notebook-tab-i-base.svg
--rw-rw-rw-   0        0        0     2764 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light/notebook-tab-i.svg
--rw-rw-rw-   0        0        0       71 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light/settings.tcl
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.590002 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light-accent/
--rw-rw-rw-   0        0        0     2762 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light-accent/notebook-tab-a.svg
--rw-rw-rw-   0        0        0     2771 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light-accent/notebook-tab-d.svg
--rw-rw-rw-   0        0        0     2764 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light-accent/notebook-tab-h.svg
--rw-rw-rw-   0        0        0     2773 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light-accent/notebook-tab-i-base.svg
--rw-rw-rw-   0        0        0     2764 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light-accent/notebook-tab-i.svg
--rw-rw-rw-   0        0        0       71 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light-accent/settings.tcl
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.592412 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.612642 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect/
--rw-rw-rw-   0        0        0       78 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect/settings.tcl
--rw-rw-rw-   0        0        0     2252 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect/slider-hd.svg
--rw-rw-rw-   0        0        0     2249 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect/slider-hn-base.svg
--rw-rw-rw-   0        0        0     2250 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect/slider-hn.svg
--rw-rw-rw-   0        0        0     2256 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect/slider-vd.svg
--rw-rw-rw-   0        0        0     2254 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect/slider-vn.svg
--rw-rw-rw-   0        0        0     2256 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect/trough-hd.svg
--rw-rw-rw-   0        0        0     2249 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect/trough-hn-base.svg
--rw-rw-rw-   0        0        0     2254 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect/trough-hn.svg
--rw-rw-rw-   0        0        0     2260 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect/trough-vd.svg
--rw-rw-rw-   0        0        0     2258 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect/trough-vn.svg
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.624306 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-bord/
--rw-rw-rw-   0        0        0       78 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-bord/settings.tcl
--rw-rw-rw-   0        0        0     2268 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-bord/slider-hd.svg
--rw-rw-rw-   0        0        0     2309 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-bord/slider-hn-base.svg
--rw-rw-rw-   0        0        0     2264 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-bord/slider-hn.svg
--rw-rw-rw-   0        0        0     2267 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-bord/slider-vd.svg
--rw-rw-rw-   0        0        0     2263 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-bord/slider-vn.svg
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.639226 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-diag/
--rw-rw-rw-   0        0        0    16071 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-diag/diag-mask.svg
--rw-rw-rw-   0        0        0       41 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-diag/settings.tcl
--rw-rw-rw-   0        0        0    16122 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-diag/slider-hd.svg
--rw-rw-rw-   0        0        0    16122 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-diag/slider-hn-base.svg
--rw-rw-rw-   0        0        0    16118 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-diag/slider-hn.svg
--rw-rw-rw-   0        0        0    16147 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-diag/slider-vd.svg
--rw-rw-rw-   0        0        0    16147 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-diag/slider-vn-base.svg
--rw-rw-rw-   0        0        0    16143 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-diag/slider-vn.svg
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.659700 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rounded-line/
--rw-rw-rw-   0        0        0       78 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rounded-line/settings.tcl
--rw-rw-rw-   0        0        0     2264 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rounded-line/slider-hd.svg
--rw-rw-rw-   0        0        0     2262 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rounded-line/slider-hn.svg
--rw-rw-rw-   0        0        0     2257 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rounded-line/slider-vd.svg
--rw-rw-rw-   0        0        0     2255 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rounded-line/slider-vn.svg
--rw-rw-rw-   0        0        0     2268 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rounded-line/trough-hd.svg
--rw-rw-rw-   0        0        0     2263 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rounded-line/trough-hn-base.svg
--rw-rw-rw-   0        0        0     2266 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rounded-line/trough-hn.svg
--rw-rw-rw-   0        0        0     2261 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rounded-line/trough-vd.svg
--rw-rw-rw-   0        0        0     2263 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rounded-line/trough-vn-base.svg
--rw-rw-rw-   0        0        0     2259 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rounded-line/trough-vn.svg
--rw-rw-rw-   0        0        0       78 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/settings.tcl
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.319584 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.676540 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle/
--rw-rw-rw-   0        0        0     2300 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle/rb-sa.svg
--rw-rw-rw-   0        0        0     2297 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle/rb-sd.svg
--rw-rw-rw-   0        0        0     2340 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle/rb-sn-base.svg
--rw-rw-rw-   0        0        0     2311 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle/rb-sn.svg
--rw-rw-rw-   0        0        0     2139 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle/rb-ua.svg
--rw-rw-rw-   0        0        0     2138 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle/rb-ud.svg
--rw-rw-rw-   0        0        0     2152 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle/rb-un.svg
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.686216 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-gradient/
--rw-rw-rw-   0        0        0     3198 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-gradient/rb-sd.svg
--rw-rw-rw-   0        0        0     3178 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-gradient/rb-sn-base.svg
--rw-rw-rw-   0        0        0     3204 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-gradient/rb-sn.svg
--rw-rw-rw-   0        0        0     2950 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-gradient/rb-ud.svg
--rw-rw-rw-   0        0        0     2960 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-gradient/rb-un.svg
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.697323 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-hlbg/
--rw-rw-rw-   0        0        0     2313 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-hlbg/rb-sa.svg
--rw-rw-rw-   0        0        0     2321 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-hlbg/rb-sd.svg
--rw-rw-rw-   0        0        0     2288 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-hlbg/rb-sn-base.svg
--rw-rw-rw-   0        0        0     2306 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-hlbg/rb-sn.svg
--rw-rw-rw-   0        0        0     2120 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-hlbg/rb-ua.svg
--rw-rw-rw-   0        0        0     2126 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-hlbg/rb-ud.svg
--rw-rw-rw-   0        0        0     2138 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-hlbg/rb-un.svg
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.708715 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-rev/
--rw-rw-rw-   0        0        0     2336 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-rev/rb-sa.svg
--rw-rw-rw-   0        0        0     2333 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-rev/rb-sd.svg
--rw-rw-rw-   0        0        0     2342 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-rev/rb-sn-base.svg
--rw-rw-rw-   0        0        0     2327 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-rev/rb-sn.svg
--rw-rw-rw-   0        0        0     2155 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-rev/rb-ua.svg
--rw-rw-rw-   0        0        0     2138 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-rev/rb-ud.svg
--rw-rw-rw-   0        0        0     2152 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-rev/rb-un.svg
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.717938 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/octagon-circle/
--rw-rw-rw-   0        0        0     2796 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/octagon-circle/rb-sd.svg
--rw-rw-rw-   0        0        0     3133 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/octagon-circle/rb-sn-base.svg
--rw-rw-rw-   0        0        0     2806 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/octagon-circle/rb-sn.svg
--rw-rw-rw-   0        0        0     2543 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/octagon-circle/rb-ud.svg
--rw-rw-rw-   0        0        0     2557 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/octagon-circle/rb-un.svg
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.323027 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.722620 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/circle/
--rw-rw-rw-   0        0        0     2163 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/circle/scale-ha.svg
--rw-rw-rw-   0        0        0     2164 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/circle/scale-hd.svg
--rw-rw-rw-   0        0        0     2162 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/circle/scale-hn.svg
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.727376 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/circle-rev/
--rw-rw-rw-   0        0        0     2160 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/circle-rev/scale-ha.svg
--rw-rw-rw-   0        0        0     2164 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/circle-rev/scale-hd.svg
--rw-rw-rw-   0        0        0     2162 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/circle-rev/scale-hn.svg
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.733581 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-bord-grip/
--rw-rw-rw-   0        0        0     7806 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-bord-grip/scale-hd.svg
--rw-rw-rw-   0        0        0     7808 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-bord-grip/scale-hn-base.svg
--rw-rw-rw-   0        0        0     7778 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-bord-grip/scale-hn.svg
--rw-rw-rw-   0        0        0     7812 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-bord-grip/scale-vd.svg
--rw-rw-rw-   0        0        0     7784 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-bord-grip/scale-vn.svg
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.760189 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/
--rw-rw-rw-   0        0        0     3369 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/scale-hd.svg
--rw-rw-rw-   0        0        0     3364 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/scale-hn-base.svg
--rw-rw-rw-   0        0        0     3359 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/scale-hn.svg
--rw-rw-rw-   0        0        0     2258 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/scale-trough-hd.svg
--rw-rw-rw-   0        0        0     2269 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/scale-trough-hn-base.svg
--rw-rw-rw-   0        0        0     2254 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/scale-trough-hn.svg
--rw-rw-rw-   0        0        0     2246 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/scale-trough-vd.svg
--rw-rw-rw-   0        0        0     2257 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/scale-trough-vn-base.svg
--rw-rw-rw-   0        0        0     2242 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/scale-trough-vn.svg
--rw-rw-rw-   0        0        0     3423 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/scale-vd.svg
--rw-rw-rw-   0        0        0     3413 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/scale-vn.svg
--rw-rw-rw-   0        0        0       90 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/settings.tcl
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.324028 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scrollbar-grip/
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.766416 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scrollbar-grip/circle/
--rw-rw-rw-   0        0        0     7495 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scrollbar-grip/circle/sb-slider-h-grip-base.svg
--rw-rw-rw-   0        0        0     7453 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scrollbar-grip/circle/sb-slider-h-grip.svg
--rw-rw-rw-   0        0        0     7520 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scrollbar-grip/circle/sb-slider-v-grip-base.svg
--rw-rw-rw-   0        0        0     7500 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scrollbar-grip/circle/sb-slider-v-grip.svg
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.325029 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/sizegrip/
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.769298 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/sizegrip/circle/
--rw-rw-rw-   0        0        0     5046 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/sizegrip/circle/sizegrip-base.svg
--rw-rw-rw-   0        0        0     5058 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/sizegrip/circle/sizegrip.svg
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.327030 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.776263 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/chevron/
--rw-rw-rw-   0        0        0     3000 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/chevron/tree-arrow-down-base.svg
--rw-rw-rw-   0        0        0     3000 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/chevron/tree-arrow-down-n.svg
--rw-rw-rw-   0        0        0     3000 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/chevron/tree-arrow-down-sn.svg
--rw-rw-rw-   0        0        0     2993 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/chevron/tree-arrow-right-n.svg
--rw-rw-rw-   0        0        0     2993 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/chevron/tree-arrow-right-sn.svg
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.785959 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/open/
--rw-rw-rw-   0        0        0     2593 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/open/tree-arrow-down-n-base.svg
--rw-rw-rw-   0        0        0     2685 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/open/tree-arrow-down-n.svg
--rw-rw-rw-   0        0        0     2685 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/open/tree-arrow-down-sn.svg
--rw-rw-rw-   0        0        0     2627 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/open/tree-arrow-right-n-base.svg
--rw-rw-rw-   0        0        0     2716 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/open/tree-arrow-right-n.svg
--rw-rw-rw-   0        0        0     2716 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/open/tree-arrow-right-sn.svg
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.791381 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/plusminus-box/
--rw-rw-rw-   0        0        0     3068 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/plusminus-box/tree-arrow-down-n-base.svg
--rw-rw-rw-   0        0        0     3005 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/plusminus-box/tree-arrow-down-n.svg
--rw-rw-rw-   0        0        0     3005 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/plusminus-box/tree-arrow-down-sn.svg
--rw-rw-rw-   0        0        0     3035 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/plusminus-box/tree-arrow-right-n-base.svg
--rw-rw-rw-   0        0        0     3055 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/plusminus-box/tree-arrow-right-n.svg
--rw-rw-rw-   0        0        0     3056 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/plusminus-box/tree-arrow-right-sn.svg
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.801470 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/solid/
--rw-rw-rw-   0        0        0     2475 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/solid/tree-arrow-down-n-base.svg
--rw-rw-rw-   0        0        0     2578 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/solid/tree-arrow-down-n.svg
--rw-rw-rw-   0        0        0     2578 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/solid/tree-arrow-down-sn.svg
--rw-rw-rw-   0        0        0     2461 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/solid/tree-arrow-right-n-base.svg
--rw-rw-rw-   0        0        0     2570 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/solid/tree-arrow-right-n.svg
--rw-rw-rw-   0        0        0     2570 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/solid/tree-arrow-right-sn.svg
--rw-rw-rw-   0        0        0     1811 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/pkgIndex.tcl
--rw-rw-rw-   0        0        0    14872 2024-04-23 13:36:45.000000 UnitMatchPy-1.5b0/UnitMatchPy/UM Logo.ico
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.806128 UnitMatchPy-1.5b0/UnitMatchPy/UnitMatchPy.egg-info/
--rw-rw-rw-   0        0        0     2325 2024-05-17 15:16:39.000000 UnitMatchPy-1.5b0/UnitMatchPy/UnitMatchPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-17 15:16:39.000000 UnitMatchPy-1.5b0/UnitMatchPy/UnitMatchPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 15:16:39.000000 UnitMatchPy-1.5b0/UnitMatchPy/UnitMatchPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-05-17 15:16:39.000000 UnitMatchPy-1.5b0/UnitMatchPy/UnitMatchPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-17 15:16:39.000000 UnitMatchPy-1.5b0/UnitMatchPy/UnitMatchPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      228 2024-05-01 13:35:33.000000 UnitMatchPy-1.5b0/UnitMatchPy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.838222 UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/
--rw-rw-rw-   0        0        0     9564 2024-04-30 12:55:34.000000 UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/AssignUniqueID.cpython-311.pyc
--rw-rw-rw-   0        0        0     4322 2024-04-23 13:42:01.000000 UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/Bayes_fun.cpython-311.pyc
--rw-rw-rw-   0        0        0     4066 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/Bayes_fun.cpython-312.pyc
--rw-rw-rw-   0        0        0     9387 2024-04-23 13:42:07.000000 UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/Extract_raw_data.cpython-311.pyc
--rw-rw-rw-   0        0        0     8483 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/Extract_raw_data.cpython-312.pyc
--rw-rw-rw-   0        0        0    81032 2024-04-30 12:42:43.000000 UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/GUI.cpython-311.pyc
--rw-rw-rw-   0        0        0    68574 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/GUI.cpython-312.pyc
--rw-rw-rw-   0        0        0    32875 2024-04-23 13:42:07.000000 UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/Metrics_fun.cpython-311.pyc
--rw-rw-rw-   0        0        0    29945 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/Metrics_fun.cpython-312.pyc
--rw-rw-rw-   0        0        0     5735 2024-04-23 13:42:07.000000 UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/Overlord.cpython-311.pyc
--rw-rw-rw-   0        0        0     5433 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/Overlord.cpython-312.pyc
--rw-rw-rw-   0        0        0    17495 2024-04-23 13:42:01.000000 UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/Param_fun.cpython-311.pyc
--rw-rw-rw-   0        0        0    16071 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/Param_fun.cpython-312.pyc
--rw-rw-rw-   0        0        0    16462 2024-04-30 12:57:43.000000 UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/Save_utils.cpython-311.pyc
--rw-rw-rw-   0        0        0    13859 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/Save_utils.cpython-312.pyc
--rw-rw-rw-   0        0        0      558 2024-04-23 13:42:01.000000 UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0      431 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0    17825 2024-04-30 09:18:28.000000 UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/utils.cpython-311.pyc
--rw-rw-rw-   0        0        0    14691 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/utils.cpython-312.pyc
--rw-rw-rw-   0        0        0    20911 2024-05-02 10:52:32.000000 UnitMatchPy-1.5b0/UnitMatchPy/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.371899 UnitMatchPy-1.5b0/UnitMatchPy.egg-info/
--rw-rw-rw-   0        0        0     2327 2024-05-17 15:35:28.000000 UnitMatchPy-1.5b0/UnitMatchPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    25269 2024-05-17 15:35:29.000000 UnitMatchPy-1.5b0/UnitMatchPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 15:35:28.000000 UnitMatchPy-1.5b0/UnitMatchPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-05-17 15:35:28.000000 UnitMatchPy-1.5b0/UnitMatchPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-17 15:35:28.000000 UnitMatchPy-1.5b0/UnitMatchPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-17 15:35:29.840255 UnitMatchPy-1.5b0/setup.cfg
--rw-rw-rw-   0        0        0      677 2024-05-17 15:35:16.000000 UnitMatchPy-1.5b0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:58.168676 UnitMatchPy-1.5rc0/
+-rw-rw-rw-   0        0        0    21281 2023-12-13 15:09:14.000000 UnitMatchPy-1.5rc0/LICENSE
+-rw-rw-rw-   0        0        0       31 2024-05-17 15:23:47.000000 UnitMatchPy-1.5rc0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2328 2024-05-28 11:43:58.167676 UnitMatchPy-1.5rc0/PKG-INFO
+-rw-rw-rw-   0        0        0     2053 2024-05-01 10:16:34.000000 UnitMatchPy-1.5rc0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:55.370015 UnitMatchPy-1.5rc0/UnitMatchPy/
+-rw-rw-rw-   0        0        0     7288 2024-05-17 14:46:04.000000 UnitMatchPy-1.5rc0/UnitMatchPy/AssignUniqueID.py
+-rw-rw-rw-   0        0        0     2600 2024-05-01 13:35:22.000000 UnitMatchPy-1.5rc0/UnitMatchPy/Bayes_fun.py
+-rw-rw-rw-   0        0        0     8209 2024-05-01 13:35:20.000000 UnitMatchPy-1.5rc0/UnitMatchPy/Extract_raw_data.py
+-rw-rw-rw-   0        0        0    50507 2024-05-17 15:28:42.000000 UnitMatchPy-1.5rc0/UnitMatchPy/GUI.py
+-rw-rw-rw-   0        0        0    23396 2024-05-01 13:35:11.000000 UnitMatchPy-1.5rc0/UnitMatchPy/Metrics_fun.py
+-rw-rw-rw-   0        0        0     5258 2024-05-01 13:35:07.000000 UnitMatchPy-1.5rc0/UnitMatchPy/Overlord.py
+-rw-rw-rw-   0        0        0    13809 2024-05-01 13:35:03.000000 UnitMatchPy-1.5rc0/UnitMatchPy/Param_fun.py
+-rw-rw-rw-   0        0        0    13419 2024-05-01 13:34:57.000000 UnitMatchPy-1.5rc0/UnitMatchPy/Save_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:55.284606 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:55.534410 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/
+-rw-rw-rw-   0        0        0     2263 2024-04-23 13:37:49.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/LICENSE
+-rw-rw-rw-   0        0        0    15818 2024-04-23 13:37:49.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/README.txt
+-rw-rw-rw-   0        0        0     2097 2024-04-23 13:37:49.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/awdark.tcl
+-rw-rw-rw-   0        0        0     1881 2024-04-23 13:37:49.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/awlight.tcl
+-rw-rw-rw-   0        0        0     6815 2024-04-23 13:37:49.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/awtemplate.tcl
+-rw-rw-rw-   0        0        0     5137 2024-04-23 13:37:49.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/awthemes.n7
+-rw-rw-rw-   0        0        0   170232 2024-04-23 13:37:49.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/awthemes.tcl
+-rw-rw-rw-   0        0        0     3562 2024-04-23 13:37:49.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/awwinxpblue.tcl
+-rw-rw-rw-   0        0        0    10425 2024-04-23 13:37:49.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/colorutils.tcl
+-rw-rw-rw-   0        0        0     7022 2024-04-23 13:37:49.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/demoscaled.tcl
+-rw-rw-rw-   0        0        0     5311 2024-04-23 13:37:49.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/demoscaledb.tcl
+-rw-rw-rw-   0        0        0    42639 2024-04-23 13:37:49.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/demottk.tcl
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:55.284606 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:55.537462 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/
+-rw-rw-rw-   0        0        0     3066 2024-04-23 13:37:49.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/README.txt
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:55.290591 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:55.637959 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/chevron/
+-rw-rw-rw-   0        0        0     2614 2024-04-23 13:37:49.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/chevron/arrow-down-d.svg
+-rw-rw-rw-   0        0        0     2596 2024-04-23 13:37:49.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/chevron/arrow-down-n-base.svg
+-rw-rw-rw-   0        0        0     2608 2024-04-23 13:37:49.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/chevron/arrow-down-n.svg
+-rw-rw-rw-   0        0        0     2608 2024-04-23 13:37:49.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/chevron/arrow-down-sn.svg
+-rw-rw-rw-   0        0        0     2699 2024-04-23 13:37:49.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/chevron/arrow-left-n.svg
+-rw-rw-rw-   0        0        0     2703 2024-04-23 13:37:49.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/chevron/arrow-right-n.svg
+-rw-rw-rw-   0        0        0     2704 2024-04-23 13:37:49.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/chevron/arrow-right-sn.svg
+-rw-rw-rw-   0        0        0     2711 2024-04-23 13:37:49.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/chevron/arrow-up-d.svg
+-rw-rw-rw-   0        0        0     2703 2024-04-23 13:37:49.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/chevron/arrow-up-n.svg
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:55.704274 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/open/
+-rw-rw-rw-   0        0        0     2593 2024-04-23 13:37:49.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/open/arrow-down-n-base.svg
+-rw-rw-rw-   0        0        0     2686 2024-04-23 13:37:49.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/open/arrow-down-n.svg
+-rw-rw-rw-   0        0        0     2687 2024-04-23 13:37:49.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/open/arrow-down-sn.svg
+-rw-rw-rw-   0        0        0     2755 2024-04-23 13:37:49.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/open/arrow-left-n.svg
+-rw-rw-rw-   0        0        0     2757 2024-04-23 13:37:49.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/open/arrow-right-n.svg
+-rw-rw-rw-   0        0        0     2757 2024-04-23 13:37:49.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/open/arrow-right-sn.svg
+-rw-rw-rw-   0        0        0     2755 2024-04-23 13:37:49.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/open/arrow-up-n.svg
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:55.762076 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid/
+-rw-rw-rw-   0        0        0     2506 2024-04-23 13:37:49.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid/arrow-down-n-base.svg
+-rw-rw-rw-   0        0        0     2590 2024-04-23 13:37:49.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid/arrow-down-n.svg
+-rw-rw-rw-   0        0        0     2590 2024-04-23 13:37:49.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid/arrow-down-sn.svg
+-rw-rw-rw-   0        0        0     2660 2024-04-23 13:37:49.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid/arrow-left-n.svg
+-rw-rw-rw-   0        0        0     2662 2024-04-23 13:37:49.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid/arrow-right-n.svg
+-rw-rw-rw-   0        0        0     2636 2024-04-23 13:37:49.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid/arrow-right-sn.svg
+-rw-rw-rw-   0        0        0     2636 2024-04-23 13:37:49.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid/arrow-up-n.svg
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:55.856189 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid-bg/
+-rw-rw-rw-   0        0        0     2972 2024-04-23 13:37:49.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid-bg/arrow-down-d.svg
+-rw-rw-rw-   0        0        0     2966 2024-04-23 13:37:49.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid-bg/arrow-down-n-base.svg
+-rw-rw-rw-   0        0        0     2964 2024-04-23 13:37:49.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid-bg/arrow-down-n.svg
+-rw-rw-rw-   0        0        0     2969 2024-04-23 13:37:49.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid-bg/arrow-left-d.svg
+-rw-rw-rw-   0        0        0     2961 2024-04-23 13:37:49.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid-bg/arrow-left-n.svg
+-rw-rw-rw-   0        0        0     2968 2024-04-23 13:37:49.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid-bg/arrow-right-d.svg
+-rw-rw-rw-   0        0        0     2960 2024-04-23 13:37:49.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid-bg/arrow-right-n.svg
+-rw-rw-rw-   0        0        0     2967 2024-04-23 13:37:49.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid-bg/arrow-up-d.svg
+-rw-rw-rw-   0        0        0     2959 2024-04-23 13:37:49.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid-bg/arrow-up-n.svg
+-rw-rw-rw-   0        0        0       77 2024-04-23 13:37:49.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid-bg/settings.tcl
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:55.292800 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:55.897304 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-accent-gradient/
+-rw-rw-rw-   0        0        0     4016 2024-04-23 13:37:49.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-accent-gradient/button-a.svg
+-rw-rw-rw-   0        0        0     2984 2024-04-23 13:37:49.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-accent-gradient/button-d.svg
+-rw-rw-rw-   0        0        0     2993 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-accent-gradient/button-n.svg
+-rw-rw-rw-   0        0        0     3013 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-accent-gradient/button-p.svg
+-rw-rw-rw-   0        0        0       79 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-accent-gradient/settings.tcl
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:55.958081 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-flat/
+-rw-rw-rw-   0        0        0     2161 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-flat/button-a.svg
+-rw-rw-rw-   0        0        0     2195 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-flat/button-af-base.svg
+-rw-rw-rw-   0        0        0     2160 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-flat/button-af.svg
+-rw-rw-rw-   0        0        0     2169 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-flat/button-d.svg
+-rw-rw-rw-   0        0        0     2160 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-flat/button-f.svg
+-rw-rw-rw-   0        0        0     2197 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-flat/button-n.svg
+-rw-rw-rw-   0        0        0     2160 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-flat/button-p.svg
+-rw-rw-rw-   0        0        0      117 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-flat/settings.tcl
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:55.992023 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-gradient/
+-rw-rw-rw-   0        0        0     3596 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-gradient/button-d.svg
+-rw-rw-rw-   0        0        0     3573 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-gradient/button-n-base.svg
+-rw-rw-rw-   0        0        0     3590 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-gradient/button-n.svg
+-rw-rw-rw-   0        0        0       79 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-gradient/settings.tcl
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:55.292800 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:56.074468 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check/
+-rw-rw-rw-   0        0        0     3260 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check/cb-sa-base.svg
+-rw-rw-rw-   0        0        0     3244 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check/cb-sa.svg
+-rw-rw-rw-   0        0        0     3198 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check/cb-sd.svg
+-rw-rw-rw-   0        0        0     2772 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check/cb-sn-base.svg
+-rw-rw-rw-   0        0        0     3203 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check/cb-sn.svg
+-rw-rw-rw-   0        0        0     2199 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check/cb-ua.svg
+-rw-rw-rw-   0        0        0     2200 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check/cb-ud.svg
+-rw-rw-rw-   0        0        0     2202 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check/cb-un.svg
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:56.122479 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check-rev/
+-rw-rw-rw-   0        0        0     3260 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check-rev/cb-sa-base.svg
+-rw-rw-rw-   0        0        0     3243 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check-rev/cb-sa.svg
+-rw-rw-rw-   0        0        0     3195 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check-rev/cb-sd.svg
+-rw-rw-rw-   0        0        0     2772 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check-rev/cb-sn-base.svg
+-rw-rw-rw-   0        0        0     3200 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check-rev/cb-sn.svg
+-rw-rw-rw-   0        0        0     2199 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check-rev/cb-ua.svg
+-rw-rw-rw-   0        0        0     2200 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check-rev/cb-ud.svg
+-rw-rw-rw-   0        0        0     2202 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check-rev/cb-un.svg
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:56.216129 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-square/
+-rw-rw-rw-   0        0        0     2460 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-square/cb-sa.svg
+-rw-rw-rw-   0        0        0     2458 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-square/cb-sd.svg
+-rw-rw-rw-   0        0        0     2443 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-square/cb-sn-base.svg
+-rw-rw-rw-   0        0        0     2457 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-square/cb-sn.svg
+-rw-rw-rw-   0        0        0     2187 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-square/cb-ua.svg
+-rw-rw-rw-   0        0        0     2190 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-square/cb-ud.svg
+-rw-rw-rw-   0        0        0     2186 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-square/cb-un.svg
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:56.282474 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/square-check-gradient/
+-rw-rw-rw-   0        0        0     3929 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/square-check-gradient/cb-sd.svg
+-rw-rw-rw-   0        0        0     3531 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/square-check-gradient/cb-sn-base.svg
+-rw-rw-rw-   0        0        0     3930 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/square-check-gradient/cb-sn.svg
+-rw-rw-rw-   0        0        0     2963 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/square-check-gradient/cb-ud.svg
+-rw-rw-rw-   0        0        0     2957 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/square-check-gradient/cb-un.svg
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:56.337629 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/square-x/
+-rw-rw-rw-   0        0        0     3079 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/square-x/cb-sd.svg
+-rw-rw-rw-   0        0        0     2965 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/square-x/cb-sn-base.svg
+-rw-rw-rw-   0        0        0     3073 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/square-x/cb-sn.svg
+-rw-rw-rw-   0        0        0     2169 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/square-x/cb-ud.svg
+-rw-rw-rw-   0        0        0     2165 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/square-x/cb-un.svg
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:55.300011 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:56.479273 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/rounded/
+-rw-rw-rw-   0        0        0     3113 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/rounded/combo-arrow-down-d.svg
+-rw-rw-rw-   0        0        0     3109 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/rounded/combo-arrow-down-n-base.svg
+-rw-rw-rw-   0        0        0     3107 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/rounded/combo-arrow-down-n.svg
+-rw-rw-rw-   0        0        0     2754 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/rounded/combo-entry-a.svg
+-rw-rw-rw-   0        0        0     2756 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/rounded/combo-entry-d.svg
+-rw-rw-rw-   0        0        0     2753 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/rounded/combo-entry-f.svg
+-rw-rw-rw-   0        0        0     2760 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/rounded/combo-entry-n-base.svg
+-rw-rw-rw-   0        0        0     2752 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/rounded/combo-entry-n.svg
+-rw-rw-rw-   0        0        0       95 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/rounded/settings.tcl
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:56.545832 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/solid-bg/
+-rw-rw-rw-   0        0        0     2861 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/solid-bg/combo-arrow-down-a.svg
+-rw-rw-rw-   0        0        0     2796 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/solid-bg/combo-arrow-down-d-base.svg
+-rw-rw-rw-   0        0        0     2882 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/solid-bg/combo-arrow-down-d.svg
+-rw-rw-rw-   0        0        0     2890 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/solid-bg/combo-arrow-down-n-base.svg
+-rw-rw-rw-   0        0        0     2870 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/solid-bg/combo-arrow-down-n.svg
+-rw-rw-rw-   0        0        0       79 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/solid-bg/settings.tcl
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:55.301012 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/empty/
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:56.553303 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/empty/empty/
+-rw-rw-rw-   0        0        0     1898 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/empty/empty/empty.svg
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:55.302533 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/entry/
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:56.616347 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/entry/roundedrect/
+-rw-rw-rw-   0        0        0     2254 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/entry/roundedrect/entry-a.svg
+-rw-rw-rw-   0        0        0     2256 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/entry/roundedrect/entry-d.svg
+-rw-rw-rw-   0        0        0     2253 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/entry/roundedrect/entry-f.svg
+-rw-rw-rw-   0        0        0     2283 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/entry/roundedrect/entry-n-base.svg
+-rw-rw-rw-   0        0        0     2252 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/entry/roundedrect/entry-n.svg
+-rw-rw-rw-   0        0        0       38 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/entry/roundedrect/settings.tcl
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:55.302533 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/labelframe/
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:56.634672 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/labelframe/square/
+-rw-rw-rw-   0        0        0     2083 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/labelframe/square/labelframe-d.svg
+-rw-rw-rw-   0        0        0     2081 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/labelframe/square/labelframe-n.svg
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:55.302533 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/menubutton/
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:56.676708 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/menubutton/chevron/
+-rw-rw-rw-   0        0        0     2938 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/menubutton/chevron/mb-arrow-down-a.svg
+-rw-rw-rw-   0        0        0     2933 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/menubutton/chevron/mb-arrow-down-d.svg
+-rw-rw-rw-   0        0        0     2930 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/menubutton/chevron/mb-arrow-down-n-base.svg
+-rw-rw-rw-   0        0        0     2923 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/menubutton/chevron/mb-arrow-down-n.svg
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:56.712530 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/menubutton/solid/
+-rw-rw-rw-   0        0        0     2486 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/menubutton/solid/mb-arrow-down-d-base.svg
+-rw-rw-rw-   0        0        0     2578 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/menubutton/solid/mb-arrow-down-d.svg
+-rw-rw-rw-   0        0        0     2480 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/menubutton/solid/mb-arrow-down-n-base.svg
+-rw-rw-rw-   0        0        0     2567 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/menubutton/solid/mb-arrow-down-n.svg
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:55.310397 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:56.789546 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-dark/
+-rw-rw-rw-   0        0        0     2762 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-dark/notebook-tab-a.svg
+-rw-rw-rw-   0        0        0     2768 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-dark/notebook-tab-d.svg
+-rw-rw-rw-   0        0        0     2773 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-dark/notebook-tab-h.svg
+-rw-rw-rw-   0        0        0     2773 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-dark/notebook-tab-i-base.svg
+-rw-rw-rw-   0        0        0     2768 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-dark/notebook-tab-i.svg
+-rw-rw-rw-   0        0        0       71 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-dark/settings.tcl
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:56.831682 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light/
+-rw-rw-rw-   0        0        0     2762 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light/notebook-tab-a.svg
+-rw-rw-rw-   0        0        0     2771 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light/notebook-tab-d.svg
+-rw-rw-rw-   0        0        0     2773 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light/notebook-tab-h.svg
+-rw-rw-rw-   0        0        0     2773 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light/notebook-tab-i-base.svg
+-rw-rw-rw-   0        0        0     2764 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light/notebook-tab-i.svg
+-rw-rw-rw-   0        0        0       71 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light/settings.tcl
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:56.860587 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light-accent/
+-rw-rw-rw-   0        0        0     2762 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light-accent/notebook-tab-a.svg
+-rw-rw-rw-   0        0        0     2771 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light-accent/notebook-tab-d.svg
+-rw-rw-rw-   0        0        0     2764 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light-accent/notebook-tab-h.svg
+-rw-rw-rw-   0        0        0     2773 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light-accent/notebook-tab-i-base.svg
+-rw-rw-rw-   0        0        0     2764 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light-accent/notebook-tab-i.svg
+-rw-rw-rw-   0        0        0       71 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light-accent/settings.tcl
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:56.870696 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:56.996499 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect/
+-rw-rw-rw-   0        0        0       78 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect/settings.tcl
+-rw-rw-rw-   0        0        0     2252 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect/slider-hd.svg
+-rw-rw-rw-   0        0        0     2249 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect/slider-hn-base.svg
+-rw-rw-rw-   0        0        0     2250 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect/slider-hn.svg
+-rw-rw-rw-   0        0        0     2256 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect/slider-vd.svg
+-rw-rw-rw-   0        0        0     2254 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect/slider-vn.svg
+-rw-rw-rw-   0        0        0     2256 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect/trough-hd.svg
+-rw-rw-rw-   0        0        0     2249 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect/trough-hn-base.svg
+-rw-rw-rw-   0        0        0     2254 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect/trough-hn.svg
+-rw-rw-rw-   0        0        0     2260 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect/trough-vd.svg
+-rw-rw-rw-   0        0        0     2258 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect/trough-vn.svg
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:57.047200 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-bord/
+-rw-rw-rw-   0        0        0       78 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-bord/settings.tcl
+-rw-rw-rw-   0        0        0     2268 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-bord/slider-hd.svg
+-rw-rw-rw-   0        0        0     2309 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-bord/slider-hn-base.svg
+-rw-rw-rw-   0        0        0     2264 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-bord/slider-hn.svg
+-rw-rw-rw-   0        0        0     2267 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-bord/slider-vd.svg
+-rw-rw-rw-   0        0        0     2263 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-bord/slider-vn.svg
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:57.132574 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-diag/
+-rw-rw-rw-   0        0        0    16071 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-diag/diag-mask.svg
+-rw-rw-rw-   0        0        0       41 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-diag/settings.tcl
+-rw-rw-rw-   0        0        0    16122 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-diag/slider-hd.svg
+-rw-rw-rw-   0        0        0    16122 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-diag/slider-hn-base.svg
+-rw-rw-rw-   0        0        0    16118 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-diag/slider-hn.svg
+-rw-rw-rw-   0        0        0    16147 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-diag/slider-vd.svg
+-rw-rw-rw-   0        0        0    16147 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-diag/slider-vn-base.svg
+-rw-rw-rw-   0        0        0    16143 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-diag/slider-vn.svg
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:57.238261 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rounded-line/
+-rw-rw-rw-   0        0        0       78 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rounded-line/settings.tcl
+-rw-rw-rw-   0        0        0     2264 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rounded-line/slider-hd.svg
+-rw-rw-rw-   0        0        0     2262 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rounded-line/slider-hn.svg
+-rw-rw-rw-   0        0        0     2257 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rounded-line/slider-vd.svg
+-rw-rw-rw-   0        0        0     2255 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rounded-line/slider-vn.svg
+-rw-rw-rw-   0        0        0     2268 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rounded-line/trough-hd.svg
+-rw-rw-rw-   0        0        0     2263 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rounded-line/trough-hn-base.svg
+-rw-rw-rw-   0        0        0     2266 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rounded-line/trough-hn.svg
+-rw-rw-rw-   0        0        0     2261 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rounded-line/trough-vd.svg
+-rw-rw-rw-   0        0        0     2263 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rounded-line/trough-vn-base.svg
+-rw-rw-rw-   0        0        0     2259 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rounded-line/trough-vn.svg
+-rw-rw-rw-   0        0        0       78 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/settings.tcl
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:55.315806 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:57.348237 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle/
+-rw-rw-rw-   0        0        0     2300 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle/rb-sa.svg
+-rw-rw-rw-   0        0        0     2297 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle/rb-sd.svg
+-rw-rw-rw-   0        0        0     2340 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle/rb-sn-base.svg
+-rw-rw-rw-   0        0        0     2311 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle/rb-sn.svg
+-rw-rw-rw-   0        0        0     2139 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle/rb-ua.svg
+-rw-rw-rw-   0        0        0     2138 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle/rb-ud.svg
+-rw-rw-rw-   0        0        0     2152 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle/rb-un.svg
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:57.425265 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-gradient/
+-rw-rw-rw-   0        0        0     3198 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-gradient/rb-sd.svg
+-rw-rw-rw-   0        0        0     3178 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-gradient/rb-sn-base.svg
+-rw-rw-rw-   0        0        0     3204 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-gradient/rb-sn.svg
+-rw-rw-rw-   0        0        0     2950 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-gradient/rb-ud.svg
+-rw-rw-rw-   0        0        0     2960 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-gradient/rb-un.svg
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:57.515805 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-hlbg/
+-rw-rw-rw-   0        0        0     2313 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-hlbg/rb-sa.svg
+-rw-rw-rw-   0        0        0     2321 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-hlbg/rb-sd.svg
+-rw-rw-rw-   0        0        0     2288 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-hlbg/rb-sn-base.svg
+-rw-rw-rw-   0        0        0     2306 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-hlbg/rb-sn.svg
+-rw-rw-rw-   0        0        0     2120 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-hlbg/rb-ua.svg
+-rw-rw-rw-   0        0        0     2126 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-hlbg/rb-ud.svg
+-rw-rw-rw-   0        0        0     2138 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-hlbg/rb-un.svg
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:57.586834 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-rev/
+-rw-rw-rw-   0        0        0     2336 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-rev/rb-sa.svg
+-rw-rw-rw-   0        0        0     2333 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-rev/rb-sd.svg
+-rw-rw-rw-   0        0        0     2342 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-rev/rb-sn-base.svg
+-rw-rw-rw-   0        0        0     2327 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-rev/rb-sn.svg
+-rw-rw-rw-   0        0        0     2155 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-rev/rb-ua.svg
+-rw-rw-rw-   0        0        0     2138 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-rev/rb-ud.svg
+-rw-rw-rw-   0        0        0     2152 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-rev/rb-un.svg
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:57.635068 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/octagon-circle/
+-rw-rw-rw-   0        0        0     2796 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/octagon-circle/rb-sd.svg
+-rw-rw-rw-   0        0        0     3133 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/octagon-circle/rb-sn-base.svg
+-rw-rw-rw-   0        0        0     2806 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/octagon-circle/rb-sn.svg
+-rw-rw-rw-   0        0        0     2543 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/octagon-circle/rb-ud.svg
+-rw-rw-rw-   0        0        0     2557 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/octagon-circle/rb-un.svg
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:55.315806 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:57.677847 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/circle/
+-rw-rw-rw-   0        0        0     2163 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/circle/scale-ha.svg
+-rw-rw-rw-   0        0        0     2164 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/circle/scale-hd.svg
+-rw-rw-rw-   0        0        0     2162 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/circle/scale-hn.svg
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:57.689571 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/circle-rev/
+-rw-rw-rw-   0        0        0     2160 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/circle-rev/scale-ha.svg
+-rw-rw-rw-   0        0        0     2164 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/circle-rev/scale-hd.svg
+-rw-rw-rw-   0        0        0     2162 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/circle-rev/scale-hn.svg
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:57.741810 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-bord-grip/
+-rw-rw-rw-   0        0        0     7806 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-bord-grip/scale-hd.svg
+-rw-rw-rw-   0        0        0     7808 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-bord-grip/scale-hn-base.svg
+-rw-rw-rw-   0        0        0     7778 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-bord-grip/scale-hn.svg
+-rw-rw-rw-   0        0        0     7812 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-bord-grip/scale-vd.svg
+-rw-rw-rw-   0        0        0     7784 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-bord-grip/scale-vn.svg
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:57.866225 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/
+-rw-rw-rw-   0        0        0     3369 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/scale-hd.svg
+-rw-rw-rw-   0        0        0     3364 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/scale-hn-base.svg
+-rw-rw-rw-   0        0        0     3359 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/scale-hn.svg
+-rw-rw-rw-   0        0        0     2258 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/scale-trough-hd.svg
+-rw-rw-rw-   0        0        0     2269 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/scale-trough-hn-base.svg
+-rw-rw-rw-   0        0        0     2254 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/scale-trough-hn.svg
+-rw-rw-rw-   0        0        0     2246 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/scale-trough-vd.svg
+-rw-rw-rw-   0        0        0     2257 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/scale-trough-vn-base.svg
+-rw-rw-rw-   0        0        0     2242 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/scale-trough-vn.svg
+-rw-rw-rw-   0        0        0     3423 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/scale-vd.svg
+-rw-rw-rw-   0        0        0     3413 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/scale-vn.svg
+-rw-rw-rw-   0        0        0       90 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/settings.tcl
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:55.315806 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scrollbar-grip/
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:57.908949 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scrollbar-grip/circle/
+-rw-rw-rw-   0        0        0     7495 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scrollbar-grip/circle/sb-slider-h-grip-base.svg
+-rw-rw-rw-   0        0        0     7453 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scrollbar-grip/circle/sb-slider-h-grip.svg
+-rw-rw-rw-   0        0        0     7520 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scrollbar-grip/circle/sb-slider-v-grip-base.svg
+-rw-rw-rw-   0        0        0     7500 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scrollbar-grip/circle/sb-slider-v-grip.svg
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:55.315806 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/sizegrip/
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:57.929943 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/sizegrip/circle/
+-rw-rw-rw-   0        0        0     5046 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/sizegrip/circle/sizegrip-base.svg
+-rw-rw-rw-   0        0        0     5058 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/sizegrip/circle/sizegrip.svg
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:55.326425 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:57.966587 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/chevron/
+-rw-rw-rw-   0        0        0     3000 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/chevron/tree-arrow-down-base.svg
+-rw-rw-rw-   0        0        0     3000 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/chevron/tree-arrow-down-n.svg
+-rw-rw-rw-   0        0        0     3000 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/chevron/tree-arrow-down-sn.svg
+-rw-rw-rw-   0        0        0     2993 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/chevron/tree-arrow-right-n.svg
+-rw-rw-rw-   0        0        0     2993 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/chevron/tree-arrow-right-sn.svg
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:58.006541 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/open/
+-rw-rw-rw-   0        0        0     2593 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/open/tree-arrow-down-n-base.svg
+-rw-rw-rw-   0        0        0     2685 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/open/tree-arrow-down-n.svg
+-rw-rw-rw-   0        0        0     2685 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/open/tree-arrow-down-sn.svg
+-rw-rw-rw-   0        0        0     2627 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/open/tree-arrow-right-n-base.svg
+-rw-rw-rw-   0        0        0     2716 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/open/tree-arrow-right-n.svg
+-rw-rw-rw-   0        0        0     2716 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/open/tree-arrow-right-sn.svg
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:58.056452 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/plusminus-box/
+-rw-rw-rw-   0        0        0     3068 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/plusminus-box/tree-arrow-down-n-base.svg
+-rw-rw-rw-   0        0        0     3005 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/plusminus-box/tree-arrow-down-n.svg
+-rw-rw-rw-   0        0        0     3005 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/plusminus-box/tree-arrow-down-sn.svg
+-rw-rw-rw-   0        0        0     3035 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/plusminus-box/tree-arrow-right-n-base.svg
+-rw-rw-rw-   0        0        0     3055 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/plusminus-box/tree-arrow-right-n.svg
+-rw-rw-rw-   0        0        0     3056 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/plusminus-box/tree-arrow-right-sn.svg
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:58.105994 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/solid/
+-rw-rw-rw-   0        0        0     2475 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/solid/tree-arrow-down-n-base.svg
+-rw-rw-rw-   0        0        0     2578 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/solid/tree-arrow-down-n.svg
+-rw-rw-rw-   0        0        0     2578 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/solid/tree-arrow-down-sn.svg
+-rw-rw-rw-   0        0        0     2461 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/solid/tree-arrow-right-n-base.svg
+-rw-rw-rw-   0        0        0     2570 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/solid/tree-arrow-right-n.svg
+-rw-rw-rw-   0        0        0     2570 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/solid/tree-arrow-right-sn.svg
+-rw-rw-rw-   0        0        0     1811 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/pkgIndex.tcl
+-rw-rw-rw-   0        0        0    14872 2024-04-23 13:36:45.000000 UnitMatchPy-1.5rc0/UnitMatchPy/UM Logo.ico
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:58.123051 UnitMatchPy-1.5rc0/UnitMatchPy/UnitMatchPy.egg-info/
+-rw-rw-rw-   0        0        0     2325 2024-05-17 15:16:39.000000 UnitMatchPy-1.5rc0/UnitMatchPy/UnitMatchPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-17 15:16:39.000000 UnitMatchPy-1.5rc0/UnitMatchPy/UnitMatchPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 15:16:39.000000 UnitMatchPy-1.5rc0/UnitMatchPy/UnitMatchPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-05-17 15:16:39.000000 UnitMatchPy-1.5rc0/UnitMatchPy/UnitMatchPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-17 15:16:39.000000 UnitMatchPy-1.5rc0/UnitMatchPy/UnitMatchPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      228 2024-05-01 13:35:33.000000 UnitMatchPy-1.5rc0/UnitMatchPy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:58.158944 UnitMatchPy-1.5rc0/UnitMatchPy/__pycache__/
+-rw-rw-rw-   0        0        0     9564 2024-04-30 12:55:34.000000 UnitMatchPy-1.5rc0/UnitMatchPy/__pycache__/AssignUniqueID.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4322 2024-04-23 13:42:01.000000 UnitMatchPy-1.5rc0/UnitMatchPy/__pycache__/Bayes_fun.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4066 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/__pycache__/Bayes_fun.cpython-312.pyc
+-rw-rw-rw-   0        0        0     9387 2024-04-23 13:42:07.000000 UnitMatchPy-1.5rc0/UnitMatchPy/__pycache__/Extract_raw_data.cpython-311.pyc
+-rw-rw-rw-   0        0        0     8483 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/__pycache__/Extract_raw_data.cpython-312.pyc
+-rw-rw-rw-   0        0        0    81032 2024-04-30 12:42:43.000000 UnitMatchPy-1.5rc0/UnitMatchPy/__pycache__/GUI.cpython-311.pyc
+-rw-rw-rw-   0        0        0    68574 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/__pycache__/GUI.cpython-312.pyc
+-rw-rw-rw-   0        0        0    32875 2024-04-23 13:42:07.000000 UnitMatchPy-1.5rc0/UnitMatchPy/__pycache__/Metrics_fun.cpython-311.pyc
+-rw-rw-rw-   0        0        0    29945 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/__pycache__/Metrics_fun.cpython-312.pyc
+-rw-rw-rw-   0        0        0     5735 2024-04-23 13:42:07.000000 UnitMatchPy-1.5rc0/UnitMatchPy/__pycache__/Overlord.cpython-311.pyc
+-rw-rw-rw-   0        0        0     5433 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/__pycache__/Overlord.cpython-312.pyc
+-rw-rw-rw-   0        0        0    17495 2024-04-23 13:42:01.000000 UnitMatchPy-1.5rc0/UnitMatchPy/__pycache__/Param_fun.cpython-311.pyc
+-rw-rw-rw-   0        0        0    16071 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/__pycache__/Param_fun.cpython-312.pyc
+-rw-rw-rw-   0        0        0    16462 2024-04-30 12:57:43.000000 UnitMatchPy-1.5rc0/UnitMatchPy/__pycache__/Save_utils.cpython-311.pyc
+-rw-rw-rw-   0        0        0    13859 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/__pycache__/Save_utils.cpython-312.pyc
+-rw-rw-rw-   0        0        0      558 2024-04-23 13:42:01.000000 UnitMatchPy-1.5rc0/UnitMatchPy/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      431 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0    17825 2024-04-30 09:18:28.000000 UnitMatchPy-1.5rc0/UnitMatchPy/__pycache__/utils.cpython-311.pyc
+-rw-rw-rw-   0        0        0    14691 2024-04-23 13:37:50.000000 UnitMatchPy-1.5rc0/UnitMatchPy/__pycache__/utils.cpython-312.pyc
+-rw-rw-rw-   0        0        0    20990 2024-05-28 11:42:20.000000 UnitMatchPy-1.5rc0/UnitMatchPy/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-28 11:43:55.413476 UnitMatchPy-1.5rc0/UnitMatchPy.egg-info/
+-rw-rw-rw-   0        0        0     2328 2024-05-28 11:43:54.000000 UnitMatchPy-1.5rc0/UnitMatchPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    25269 2024-05-28 11:43:55.000000 UnitMatchPy-1.5rc0/UnitMatchPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 11:43:54.000000 UnitMatchPy-1.5rc0/UnitMatchPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-05-28 11:43:54.000000 UnitMatchPy-1.5rc0/UnitMatchPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-28 11:43:54.000000 UnitMatchPy-1.5rc0/UnitMatchPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 11:43:58.168676 UnitMatchPy-1.5rc0/setup.cfg
+-rw-rw-rw-   0        0        0      677 2024-05-28 11:43:22.000000 UnitMatchPy-1.5rc0/setup.py
```

### Comparing `UnitMatchPy-1.5b0/LICENSE` & `UnitMatchPy-1.5rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/PKG-INFO` & `UnitMatchPy-1.5rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UnitMatchPy
-Version: 1.5b0
+Version: 1.5rc0
 Summary: Description of the package
 Author: Enny van Beest, Celian Bimbard and Sam Dodgson
 Author-email: e.beest@ucl.ac.uk
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `UnitMatchPy-1.5b0/README.md` & `UnitMatchPy-1.5rc0/README.md`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/AssignUniqueID.py` & `UnitMatchPy-1.5rc0/UnitMatchPy/AssignUniqueID.py`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/Bayes_fun.py` & `UnitMatchPy-1.5rc0/UnitMatchPy/Bayes_fun.py`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/Extract_raw_data.py` & `UnitMatchPy-1.5rc0/UnitMatchPy/Extract_raw_data.py`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/GUI.py` & `UnitMatchPy-1.5rc0/UnitMatchPy/GUI.py`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/Metrics_fun.py` & `UnitMatchPy-1.5rc0/UnitMatchPy/Metrics_fun.py`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/Overlord.py` & `UnitMatchPy-1.5rc0/UnitMatchPy/Overlord.py`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/Param_fun.py` & `UnitMatchPy-1.5rc0/UnitMatchPy/Param_fun.py`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/Save_utils.py` & `UnitMatchPy-1.5rc0/UnitMatchPy/Save_utils.py`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/LICENSE` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/README.txt` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/README.txt`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/awdark.tcl` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/awdark.tcl`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/awlight.tcl` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/awlight.tcl`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/awtemplate.tcl` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/awtemplate.tcl`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/awthemes.n7` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/awthemes.n7`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/awthemes.tcl` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/awthemes.tcl`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/awwinxpblue.tcl` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/awwinxpblue.tcl`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/colorutils.tcl` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/colorutils.tcl`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/demoscaled.tcl` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/demoscaled.tcl`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/demoscaledb.tcl` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/demoscaledb.tcl`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/demottk.tcl` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/demottk.tcl`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/README.txt` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/README.txt`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/chevron/arrow-down-d.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/chevron/arrow-down-d.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/chevron/arrow-down-n-base.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/chevron/arrow-down-n-base.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/chevron/arrow-down-n.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/chevron/arrow-down-n.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/chevron/arrow-down-sn.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/chevron/arrow-down-sn.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/chevron/arrow-left-n.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/chevron/arrow-left-n.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/chevron/arrow-right-n.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/chevron/arrow-right-n.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/chevron/arrow-right-sn.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/chevron/arrow-right-sn.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/chevron/arrow-up-d.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/chevron/arrow-up-d.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/chevron/arrow-up-n.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/chevron/arrow-up-n.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/open/arrow-down-n-base.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/open/arrow-down-n-base.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/open/arrow-down-n.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/open/arrow-down-n.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/open/arrow-down-sn.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/open/arrow-down-sn.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/open/arrow-left-n.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/open/arrow-left-n.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/open/arrow-right-n.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/open/arrow-right-n.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/open/arrow-right-sn.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/open/arrow-right-sn.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/open/arrow-up-n.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/open/arrow-up-n.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid/arrow-down-n-base.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid/arrow-down-n-base.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid/arrow-down-n.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid/arrow-down-n.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid/arrow-down-sn.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid/arrow-down-sn.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid/arrow-left-n.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid/arrow-left-n.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid/arrow-right-n.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid/arrow-right-n.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid/arrow-right-sn.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid/arrow-right-sn.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid/arrow-up-n.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid/arrow-up-n.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid-bg/arrow-down-d.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid-bg/arrow-down-d.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid-bg/arrow-down-n-base.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid-bg/arrow-down-n-base.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid-bg/arrow-down-n.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid-bg/arrow-down-n.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid-bg/arrow-left-d.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid-bg/arrow-left-d.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid-bg/arrow-left-n.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid-bg/arrow-left-n.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid-bg/arrow-right-d.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid-bg/arrow-right-d.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid-bg/arrow-right-n.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid-bg/arrow-right-n.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid-bg/arrow-up-d.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid-bg/arrow-up-d.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid-bg/arrow-up-n.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid-bg/arrow-up-n.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-accent-gradient/button-a.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-accent-gradient/button-a.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-accent-gradient/button-d.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-accent-gradient/button-d.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-accent-gradient/button-n.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-accent-gradient/button-n.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-accent-gradient/button-p.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-accent-gradient/button-p.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-flat/button-a.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-flat/button-a.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-flat/button-af-base.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-flat/button-af-base.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-flat/button-af.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-flat/button-af.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-flat/button-d.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-flat/button-d.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-flat/button-f.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-flat/button-f.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-flat/button-n.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-flat/button-n.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-flat/button-p.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-flat/button-p.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-gradient/button-d.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-gradient/button-d.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-gradient/button-n-base.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-gradient/button-n-base.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-gradient/button-n.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-gradient/button-n.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check/cb-sa-base.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check/cb-sa-base.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check/cb-sa.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check/cb-sa.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check/cb-sd.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check/cb-sd.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check/cb-sn-base.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check/cb-sn-base.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check/cb-sn.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check/cb-sn.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check/cb-ua.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check/cb-ua.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check/cb-ud.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check/cb-ud.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check/cb-un.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check/cb-un.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check-rev/cb-sa-base.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check-rev/cb-sa-base.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check-rev/cb-sa.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check-rev/cb-sa.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check-rev/cb-sd.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check-rev/cb-sd.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check-rev/cb-sn-base.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check-rev/cb-sn-base.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check-rev/cb-sn.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check-rev/cb-sn.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check-rev/cb-ua.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check-rev/cb-ua.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check-rev/cb-ud.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check-rev/cb-ud.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check-rev/cb-un.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check-rev/cb-un.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-square/cb-sa.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-square/cb-sa.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-square/cb-sd.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-square/cb-sd.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-square/cb-sn-base.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-square/cb-sn-base.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-square/cb-sn.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-square/cb-sn.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-square/cb-ua.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-square/cb-ua.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-square/cb-ud.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-square/cb-ud.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-square/cb-un.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-square/cb-un.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/square-check-gradient/cb-sd.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/square-check-gradient/cb-sd.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/square-check-gradient/cb-sn-base.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/square-check-gradient/cb-sn-base.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/square-check-gradient/cb-sn.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/square-check-gradient/cb-sn.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/square-check-gradient/cb-ud.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/square-check-gradient/cb-ud.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/square-check-gradient/cb-un.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/square-check-gradient/cb-un.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/square-x/cb-sd.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/square-x/cb-sd.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/square-x/cb-sn-base.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/square-x/cb-sn-base.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/square-x/cb-sn.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/square-x/cb-sn.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/square-x/cb-ud.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/square-x/cb-ud.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/square-x/cb-un.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/square-x/cb-un.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/rounded/combo-arrow-down-d.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/rounded/combo-arrow-down-d.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/rounded/combo-arrow-down-n-base.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/rounded/combo-arrow-down-n-base.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/rounded/combo-arrow-down-n.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/rounded/combo-arrow-down-n.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/rounded/combo-entry-a.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/rounded/combo-entry-a.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/rounded/combo-entry-d.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/rounded/combo-entry-d.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/rounded/combo-entry-f.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/rounded/combo-entry-f.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/rounded/combo-entry-n-base.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/rounded/combo-entry-n-base.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/rounded/combo-entry-n.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/rounded/combo-entry-n.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/solid-bg/combo-arrow-down-a.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/solid-bg/combo-arrow-down-a.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/solid-bg/combo-arrow-down-d-base.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/solid-bg/combo-arrow-down-d-base.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/solid-bg/combo-arrow-down-d.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/solid-bg/combo-arrow-down-d.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/solid-bg/combo-arrow-down-n-base.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/solid-bg/combo-arrow-down-n-base.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/solid-bg/combo-arrow-down-n.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/solid-bg/combo-arrow-down-n.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/empty/empty/empty.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/empty/empty/empty.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/entry/roundedrect/entry-a.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/entry/roundedrect/entry-a.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/entry/roundedrect/entry-d.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/entry/roundedrect/entry-d.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/entry/roundedrect/entry-f.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/entry/roundedrect/entry-f.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/entry/roundedrect/entry-n-base.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/entry/roundedrect/entry-n-base.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/entry/roundedrect/entry-n.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/entry/roundedrect/entry-n.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/labelframe/square/labelframe-d.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/labelframe/square/labelframe-d.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/labelframe/square/labelframe-n.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/labelframe/square/labelframe-n.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/menubutton/chevron/mb-arrow-down-a.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/menubutton/chevron/mb-arrow-down-a.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/menubutton/chevron/mb-arrow-down-d.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/menubutton/chevron/mb-arrow-down-d.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/menubutton/chevron/mb-arrow-down-n-base.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/menubutton/chevron/mb-arrow-down-n-base.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/menubutton/chevron/mb-arrow-down-n.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/menubutton/chevron/mb-arrow-down-n.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/menubutton/solid/mb-arrow-down-d-base.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/menubutton/solid/mb-arrow-down-d-base.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/menubutton/solid/mb-arrow-down-d.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/menubutton/solid/mb-arrow-down-d.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/menubutton/solid/mb-arrow-down-n-base.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/menubutton/solid/mb-arrow-down-n-base.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/menubutton/solid/mb-arrow-down-n.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/menubutton/solid/mb-arrow-down-n.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-dark/notebook-tab-a.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-dark/notebook-tab-a.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-dark/notebook-tab-d.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-dark/notebook-tab-d.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-dark/notebook-tab-h.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-dark/notebook-tab-h.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-dark/notebook-tab-i-base.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-dark/notebook-tab-i-base.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-dark/notebook-tab-i.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-dark/notebook-tab-i.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light/notebook-tab-a.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light/notebook-tab-a.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light/notebook-tab-d.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light/notebook-tab-d.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light/notebook-tab-h.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light/notebook-tab-h.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light/notebook-tab-i-base.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light/notebook-tab-i-base.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light/notebook-tab-i.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light/notebook-tab-i.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light-accent/notebook-tab-a.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light-accent/notebook-tab-a.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light-accent/notebook-tab-d.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light-accent/notebook-tab-d.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light-accent/notebook-tab-h.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light-accent/notebook-tab-h.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light-accent/notebook-tab-i-base.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light-accent/notebook-tab-i-base.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light-accent/notebook-tab-i.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light-accent/notebook-tab-i.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect/slider-hd.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect/slider-hd.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect/slider-hn-base.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect/slider-hn-base.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect/slider-hn.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect/slider-hn.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect/slider-vd.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect/slider-vd.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect/slider-vn.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect/slider-vn.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect/trough-hd.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect/trough-hd.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect/trough-hn-base.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect/trough-hn-base.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect/trough-hn.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect/trough-hn.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect/trough-vd.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect/trough-vd.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect/trough-vn.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect/trough-vn.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-bord/slider-hd.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-bord/slider-hd.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-bord/slider-hn-base.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-bord/slider-hn-base.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-bord/slider-hn.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-bord/slider-hn.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-bord/slider-vd.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-bord/slider-vd.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-bord/slider-vn.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-bord/slider-vn.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-diag/diag-mask.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-diag/diag-mask.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-diag/slider-hd.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-diag/slider-hd.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-diag/slider-hn-base.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-diag/slider-hn-base.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-diag/slider-hn.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-diag/slider-hn.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-diag/slider-vd.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-diag/slider-vd.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-diag/slider-vn-base.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-diag/slider-vn-base.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-diag/slider-vn.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-diag/slider-vn.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rounded-line/slider-hd.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rounded-line/slider-hd.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rounded-line/slider-hn.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rounded-line/slider-hn.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rounded-line/slider-vd.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rounded-line/slider-vd.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rounded-line/slider-vn.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rounded-line/slider-vn.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rounded-line/trough-hd.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rounded-line/trough-hd.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rounded-line/trough-hn-base.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rounded-line/trough-hn-base.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rounded-line/trough-hn.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rounded-line/trough-hn.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rounded-line/trough-vd.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rounded-line/trough-vd.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rounded-line/trough-vn-base.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rounded-line/trough-vn-base.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rounded-line/trough-vn.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rounded-line/trough-vn.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle/rb-sa.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle/rb-sa.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle/rb-sd.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle/rb-sd.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle/rb-sn-base.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle/rb-sn-base.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle/rb-sn.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle/rb-sn.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle/rb-ua.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle/rb-ua.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle/rb-ud.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle/rb-ud.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle/rb-un.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle/rb-un.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-gradient/rb-sd.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-gradient/rb-sd.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-gradient/rb-sn-base.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-gradient/rb-sn-base.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-gradient/rb-sn.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-gradient/rb-sn.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-gradient/rb-ud.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-gradient/rb-ud.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-gradient/rb-un.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-gradient/rb-un.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-hlbg/rb-sa.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-hlbg/rb-sa.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-hlbg/rb-sd.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-hlbg/rb-sd.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-hlbg/rb-sn-base.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-hlbg/rb-sn-base.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-hlbg/rb-sn.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-hlbg/rb-sn.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-hlbg/rb-ua.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-hlbg/rb-ua.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-hlbg/rb-ud.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-hlbg/rb-ud.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-hlbg/rb-un.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-hlbg/rb-un.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-rev/rb-sa.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-rev/rb-sa.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-rev/rb-sd.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-rev/rb-sd.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-rev/rb-sn-base.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-rev/rb-sn-base.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-rev/rb-sn.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-rev/rb-sn.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-rev/rb-ua.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-rev/rb-ua.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-rev/rb-ud.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-rev/rb-ud.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-rev/rb-un.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-rev/rb-un.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/octagon-circle/rb-sd.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/octagon-circle/rb-sd.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/octagon-circle/rb-sn-base.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/octagon-circle/rb-sn-base.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/octagon-circle/rb-sn.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/octagon-circle/rb-sn.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/octagon-circle/rb-ud.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/octagon-circle/rb-ud.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/octagon-circle/rb-un.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/octagon-circle/rb-un.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/circle/scale-ha.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/circle/scale-ha.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/circle/scale-hd.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/circle/scale-hd.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/circle/scale-hn.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/circle/scale-hn.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/circle-rev/scale-ha.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/circle-rev/scale-ha.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/circle-rev/scale-hd.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/circle-rev/scale-hd.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/circle-rev/scale-hn.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/circle-rev/scale-hn.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-bord-grip/scale-hd.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-bord-grip/scale-hd.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-bord-grip/scale-hn-base.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-bord-grip/scale-hn-base.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-bord-grip/scale-hn.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-bord-grip/scale-hn.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-bord-grip/scale-vd.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-bord-grip/scale-vd.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-bord-grip/scale-vn.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-bord-grip/scale-vn.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/scale-hd.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/scale-hd.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/scale-hn-base.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/scale-hn-base.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/scale-hn.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/scale-hn.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/scale-trough-hd.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/scale-trough-hd.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/scale-trough-hn-base.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/scale-trough-hn-base.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/scale-trough-hn.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/scale-trough-hn.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/scale-trough-vd.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/scale-trough-vd.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/scale-trough-vn-base.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/scale-trough-vn-base.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/scale-trough-vn.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/scale-trough-vn.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/scale-vd.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/scale-vd.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/scale-vn.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/scale-vn.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scrollbar-grip/circle/sb-slider-h-grip-base.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scrollbar-grip/circle/sb-slider-h-grip-base.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scrollbar-grip/circle/sb-slider-h-grip.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scrollbar-grip/circle/sb-slider-h-grip.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scrollbar-grip/circle/sb-slider-v-grip-base.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scrollbar-grip/circle/sb-slider-v-grip-base.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scrollbar-grip/circle/sb-slider-v-grip.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scrollbar-grip/circle/sb-slider-v-grip.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/sizegrip/circle/sizegrip-base.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/sizegrip/circle/sizegrip-base.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/sizegrip/circle/sizegrip.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/sizegrip/circle/sizegrip.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/chevron/tree-arrow-down-base.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/chevron/tree-arrow-down-base.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/chevron/tree-arrow-down-n.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/chevron/tree-arrow-down-n.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/chevron/tree-arrow-down-sn.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/chevron/tree-arrow-down-sn.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/chevron/tree-arrow-right-n.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/chevron/tree-arrow-right-n.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/chevron/tree-arrow-right-sn.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/chevron/tree-arrow-right-sn.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/open/tree-arrow-down-n-base.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/open/tree-arrow-down-n-base.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/open/tree-arrow-down-n.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/open/tree-arrow-down-n.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/open/tree-arrow-down-sn.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/open/tree-arrow-down-sn.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/open/tree-arrow-right-n-base.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/open/tree-arrow-right-n-base.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/open/tree-arrow-right-n.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/open/tree-arrow-right-n.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/open/tree-arrow-right-sn.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/open/tree-arrow-right-sn.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/plusminus-box/tree-arrow-down-n-base.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/plusminus-box/tree-arrow-down-n-base.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/plusminus-box/tree-arrow-down-n.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/plusminus-box/tree-arrow-down-n.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/plusminus-box/tree-arrow-down-sn.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/plusminus-box/tree-arrow-down-sn.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/plusminus-box/tree-arrow-right-n-base.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/plusminus-box/tree-arrow-right-n-base.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/plusminus-box/tree-arrow-right-n.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/plusminus-box/tree-arrow-right-n.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/plusminus-box/tree-arrow-right-sn.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/plusminus-box/tree-arrow-right-sn.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/solid/tree-arrow-down-n-base.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/solid/tree-arrow-down-n-base.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/solid/tree-arrow-down-n.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/solid/tree-arrow-down-n.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/solid/tree-arrow-down-sn.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/solid/tree-arrow-down-sn.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/solid/tree-arrow-right-n-base.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/solid/tree-arrow-right-n-base.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/solid/tree-arrow-right-n.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/solid/tree-arrow-right-n.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/solid/tree-arrow-right-sn.svg` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/solid/tree-arrow-right-sn.svg`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/pkgIndex.tcl` & `UnitMatchPy-1.5rc0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/UM Logo.ico` & `UnitMatchPy-1.5rc0/UnitMatchPy/UM Logo.ico`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/UnitMatchPy.egg-info/PKG-INFO` & `UnitMatchPy-1.5rc0/UnitMatchPy/UnitMatchPy.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/AssignUniqueID.cpython-311.pyc` & `UnitMatchPy-1.5rc0/UnitMatchPy/__pycache__/AssignUniqueID.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/Bayes_fun.cpython-311.pyc` & `UnitMatchPy-1.5rc0/UnitMatchPy/__pycache__/Bayes_fun.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/Bayes_fun.cpython-312.pyc` & `UnitMatchPy-1.5rc0/UnitMatchPy/__pycache__/Bayes_fun.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/Extract_raw_data.cpython-311.pyc` & `UnitMatchPy-1.5rc0/UnitMatchPy/__pycache__/Extract_raw_data.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/Extract_raw_data.cpython-312.pyc` & `UnitMatchPy-1.5rc0/UnitMatchPy/__pycache__/Extract_raw_data.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/GUI.cpython-311.pyc` & `UnitMatchPy-1.5rc0/UnitMatchPy/__pycache__/GUI.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/GUI.cpython-312.pyc` & `UnitMatchPy-1.5rc0/UnitMatchPy/__pycache__/GUI.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/Metrics_fun.cpython-311.pyc` & `UnitMatchPy-1.5rc0/UnitMatchPy/__pycache__/Metrics_fun.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/Metrics_fun.cpython-312.pyc` & `UnitMatchPy-1.5rc0/UnitMatchPy/__pycache__/Metrics_fun.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/Overlord.cpython-311.pyc` & `UnitMatchPy-1.5rc0/UnitMatchPy/__pycache__/Overlord.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/Overlord.cpython-312.pyc` & `UnitMatchPy-1.5rc0/UnitMatchPy/__pycache__/Overlord.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/Param_fun.cpython-311.pyc` & `UnitMatchPy-1.5rc0/UnitMatchPy/__pycache__/Param_fun.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/Param_fun.cpython-312.pyc` & `UnitMatchPy-1.5rc0/UnitMatchPy/__pycache__/Param_fun.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/Save_utils.cpython-311.pyc` & `UnitMatchPy-1.5rc0/UnitMatchPy/__pycache__/Save_utils.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/Save_utils.cpython-312.pyc` & `UnitMatchPy-1.5rc0/UnitMatchPy/__pycache__/Save_utils.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/__init__.cpython-311.pyc` & `UnitMatchPy-1.5rc0/UnitMatchPy/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/utils.cpython-311.pyc` & `UnitMatchPy-1.5rc0/UnitMatchPy/__pycache__/utils.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/utils.cpython-312.pyc` & `UnitMatchPy-1.5rc0/UnitMatchPy/__pycache__/utils.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy/utils.py` & `UnitMatchPy-1.5rc0/UnitMatchPy/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -358,20 +358,22 @@
 
 
 def paths_fromKS(KSdirs):
     nSessions = len(KSdirs)
 
     #load in the number of channels
     tmp = os.getcwd()
+    #load in a waveform from each session to get the number of channels!
     nChannels = []
     for i in range(nSessions):
-        pathtmp = os.path.join(KSdirs[0], 'params.py')#
-        os.chdir(KSdirs[0])
-        from params import n_channels_dat
-        nChannels.append(n_channels_dat - 1) #subtract the sync channel
+        pathtmp = os.path.join(KSdirs[i], 'RawWaveforms')
+        file = os.listdir(pathtmp)
+        WaveformTmp = np.load(os.path.join(pathtmp,file[0]))
+        nChannels.append(WaveformTmp.shape[1])
+
     os.chdir(tmp)
 
     #Load ChannelPos
     ChannelPos = []
     for i in range(nSessions):
         PathTmp = os.path.join(KSdirs[i], 'channel_positions.npy')
         PosTmp = np.load(PathTmp)
```

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy.egg-info/PKG-INFO` & `UnitMatchPy-1.5rc0/UnitMatchPy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UnitMatchPy
-Version: 1.5b0
+Version: 1.5rc0
 Summary: Description of the package
 Author: Enny van Beest, Celian Bimbard and Sam Dodgson
 Author-email: e.beest@ucl.ac.uk
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `UnitMatchPy-1.5b0/UnitMatchPy.egg-info/SOURCES.txt` & `UnitMatchPy-1.5rc0/UnitMatchPy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.5b0/setup.py` & `UnitMatchPy-1.5rc0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     description = f.read()
 
 setup(
     name="UnitMatchPy",
-    version="1.5b",
+    version="1.5c",
     description="Description of the package",
     author="Enny van Beest, Celian Bimbard and Sam Dodgson",
     author_email="e.beest@ucl.ac.uk",
     packages=find_packages(),  
     include_package_data=True,
     python_requires=">=3.7",
     install_requires=[
```

