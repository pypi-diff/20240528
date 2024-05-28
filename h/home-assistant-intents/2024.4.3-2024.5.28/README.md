# Comparing `tmp/home-assistant-intents-2024.4.3.tar.gz` & `tmp/home-assistant-intents-2024.5.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "home-assistant-intents-2024.4.3.tar", last modified: Mon Apr 22 17:29:26 2024, max compression
+gzip compressed data, was "home-assistant-intents-2024.5.28.tar", last modified: Tue May 28 14:58:04 2024, max compression
```

## Comparing `home-assistant-intents-2024.4.3.tar` & `home-assistant-intents-2024.5.28.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2024-04-22 17:29:26.205138 home-assistant-intents-2024.4.3/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    18657 2023-02-15 17:17:10.000000 home-assistant-intents-2024.4.3/LICENSE.md
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       72 2023-01-11 16:06:16.000000 home-assistant-intents-2024.4.3/MANIFEST.in
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1337 2024-04-22 17:29:26.205138 home-assistant-intents-2024.4.3/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      523 2023-05-30 16:59:24.000000 home-assistant-intents-2024.4.3/README.md
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2024-04-22 17:29:26.201138 home-assistant-intents-2024.4.3/home_assistant_intents/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3368 2024-03-29 16:20:36.000000 home-assistant-intents-2024.4.3/home_assistant_intents/__init__.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2024-04-22 17:29:26.205138 home-assistant-intents-2024.4.3/home_assistant_intents/data/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3391 2024-04-22 17:29:21.000000 home-assistant-intents-2024.4.3/home_assistant_intents/data/af.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    19745 2024-04-22 17:29:21.000000 home-assistant-intents-2024.4.3/home_assistant_intents/data/ar.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    60407 2024-04-22 17:29:21.000000 home-assistant-intents-2024.4.3/home_assistant_intents/data/bg.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2362 2024-04-22 17:29:21.000000 home-assistant-intents-2024.4.3/home_assistant_intents/data/bn.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    20718 2024-04-22 17:29:21.000000 home-assistant-intents-2024.4.3/home_assistant_intents/data/ca.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    66715 2024-04-22 17:29:21.000000 home-assistant-intents-2024.4.3/home_assistant_intents/data/cs.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    22955 2024-04-22 17:29:21.000000 home-assistant-intents-2024.4.3/home_assistant_intents/data/da.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    30623 2024-04-22 17:29:21.000000 home-assistant-intents-2024.4.3/home_assistant_intents/data/de-CH.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    65003 2024-04-22 17:29:21.000000 home-assistant-intents-2024.4.3/home_assistant_intents/data/de.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    67879 2024-04-22 17:29:21.000000 home-assistant-intents-2024.4.3/home_assistant_intents/data/el.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)   101806 2024-04-22 17:29:21.000000 home-assistant-intents-2024.4.3/home_assistant_intents/data/en.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)   116685 2024-04-22 17:29:21.000000 home-assistant-intents-2024.4.3/home_assistant_intents/data/es.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1005 2024-04-22 17:29:21.000000 home-assistant-intents-2024.4.3/home_assistant_intents/data/et.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     6407 2024-04-22 17:29:21.000000 home-assistant-intents-2024.4.3/home_assistant_intents/data/eu.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3344 2024-04-22 17:29:21.000000 home-assistant-intents-2024.4.3/home_assistant_intents/data/fa.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    68674 2024-04-22 17:29:21.000000 home-assistant-intents-2024.4.3/home_assistant_intents/data/fi.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     9009 2024-04-22 17:29:21.000000 home-assistant-intents-2024.4.3/home_assistant_intents/data/fr-CA.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)   137454 2024-04-22 17:29:21.000000 home-assistant-intents-2024.4.3/home_assistant_intents/data/fr.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    36322 2024-04-22 17:29:21.000000 home-assistant-intents-2024.4.3/home_assistant_intents/data/gl.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1832 2024-04-22 17:29:21.000000 home-assistant-intents-2024.4.3/home_assistant_intents/data/gu.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    17909 2024-04-22 17:29:21.000000 home-assistant-intents-2024.4.3/home_assistant_intents/data/he.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1984 2024-04-22 17:29:21.000000 home-assistant-intents-2024.4.3/home_assistant_intents/data/hi.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    45624 2024-04-22 17:29:22.000000 home-assistant-intents-2024.4.3/home_assistant_intents/data/hr.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)   115891 2024-04-22 17:29:22.000000 home-assistant-intents-2024.4.3/home_assistant_intents/data/hu.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4885 2024-04-22 17:29:22.000000 home-assistant-intents-2024.4.3/home_assistant_intents/data/id.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    20852 2024-04-22 17:29:22.000000 home-assistant-intents-2024.4.3/home_assistant_intents/data/is.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    34883 2024-04-22 17:29:22.000000 home-assistant-intents-2024.4.3/home_assistant_intents/data/it.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3989 2024-04-22 17:29:22.000000 home-assistant-intents-2024.4.3/home_assistant_intents/data/ka.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1656 2024-04-22 17:29:22.000000 home-assistant-intents-2024.4.3/home_assistant_intents/data/kn.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    63797 2024-04-22 17:29:22.000000 home-assistant-intents-2024.4.3/home_assistant_intents/data/ko.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14734 2024-04-22 17:29:22.000000 home-assistant-intents-2024.4.3/home_assistant_intents/data/lb.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    13713 2024-04-22 17:29:22.000000 home-assistant-intents-2024.4.3/home_assistant_intents/data/lt.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    10475 2024-04-22 17:29:22.000000 home-assistant-intents-2024.4.3/home_assistant_intents/data/lv.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14734 2024-04-22 17:29:22.000000 home-assistant-intents-2024.4.3/home_assistant_intents/data/ml.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1825 2024-04-22 17:29:22.000000 home-assistant-intents-2024.4.3/home_assistant_intents/data/mn.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     6416 2024-04-22 17:29:22.000000 home-assistant-intents-2024.4.3/home_assistant_intents/data/ms.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    72078 2024-04-22 17:29:22.000000 home-assistant-intents-2024.4.3/home_assistant_intents/data/nb.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)   117660 2024-04-22 17:29:22.000000 home-assistant-intents-2024.4.3/home_assistant_intents/data/nl.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    80016 2024-04-22 17:29:22.000000 home-assistant-intents-2024.4.3/home_assistant_intents/data/pl.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    19196 2024-04-22 17:29:22.000000 home-assistant-intents-2024.4.3/home_assistant_intents/data/pt-br.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    18077 2024-04-22 17:29:22.000000 home-assistant-intents-2024.4.3/home_assistant_intents/data/pt.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)   107508 2024-04-22 17:29:22.000000 home-assistant-intents-2024.4.3/home_assistant_intents/data/ro.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)   103994 2024-04-22 17:29:22.000000 home-assistant-intents-2024.4.3/home_assistant_intents/data/ru.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    18266 2024-04-22 17:29:22.000000 home-assistant-intents-2024.4.3/home_assistant_intents/data/sk.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)   110627 2024-04-22 17:29:22.000000 home-assistant-intents-2024.4.3/home_assistant_intents/data/sl.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    29113 2024-04-22 17:29:22.000000 home-assistant-intents-2024.4.3/home_assistant_intents/data/sr.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    22734 2024-04-22 17:29:22.000000 home-assistant-intents-2024.4.3/home_assistant_intents/data/sv.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11284 2024-04-22 17:29:23.000000 home-assistant-intents-2024.4.3/home_assistant_intents/data/sw.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2219 2024-04-22 17:29:23.000000 home-assistant-intents-2024.4.3/home_assistant_intents/data/te.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     6456 2024-04-22 17:29:23.000000 home-assistant-intents-2024.4.3/home_assistant_intents/data/tr.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    32039 2024-04-22 17:29:23.000000 home-assistant-intents-2024.4.3/home_assistant_intents/data/uk.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    16432 2024-04-22 17:29:23.000000 home-assistant-intents-2024.4.3/home_assistant_intents/data/ur.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    82818 2024-04-22 17:29:23.000000 home-assistant-intents-2024.4.3/home_assistant_intents/data/vi.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    19297 2024-04-22 17:29:23.000000 home-assistant-intents-2024.4.3/home_assistant_intents/data/zh-cn.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    15749 2024-04-22 17:29:23.000000 home-assistant-intents-2024.4.3/home_assistant_intents/data/zh-hk.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    40899 2024-04-22 17:29:23.000000 home-assistant-intents-2024.4.3/home_assistant_intents/data/zh-tw.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      594 2024-04-22 17:29:23.000000 home-assistant-intents-2024.4.3/home_assistant_intents/languages.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2024-04-22 17:29:26.201138 home-assistant-intents-2024.4.3/home_assistant_intents.egg-info/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1337 2024-04-22 17:29:25.000000 home-assistant-intents-2024.4.3/home_assistant_intents.egg-info/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2377 2024-04-22 17:29:26.000000 home-assistant-intents-2024.4.3/home_assistant_intents.egg-info/SOURCES.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2024-04-22 17:29:25.000000 home-assistant-intents-2024.4.3/home_assistant_intents.egg-info/dependency_links.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       23 2024-04-22 17:29:26.000000 home-assistant-intents-2024.4.3/home_assistant_intents.egg-info/top_level.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-05-30 16:35:50.000000 home-assistant-intents-2024.4.3/home_assistant_intents.egg-info/zip-safe
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1081 2024-04-03 15:00:05.000000 home-assistant-intents-2024.4.3/pyproject.toml
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       38 2024-04-22 17:29:26.205138 home-assistant-intents-2024.4.3/setup.cfg
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2024-05-28 14:58:04.221718 home-assistant-intents-2024.5.28/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    18657 2023-02-15 17:17:10.000000 home-assistant-intents-2024.5.28/LICENSE.md
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       72 2023-01-11 16:06:16.000000 home-assistant-intents-2024.5.28/MANIFEST.in
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1338 2024-05-28 14:58:04.221718 home-assistant-intents-2024.5.28/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      523 2023-05-30 16:59:24.000000 home-assistant-intents-2024.5.28/README.md
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2024-05-28 14:58:04.213718 home-assistant-intents-2024.5.28/home_assistant_intents/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3891 2024-05-28 14:06:33.000000 home-assistant-intents-2024.5.28/home_assistant_intents/__init__.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2024-05-28 14:58:04.221718 home-assistant-intents-2024.5.28/home_assistant_intents/data/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3391 2024-05-28 14:57:59.000000 home-assistant-intents-2024.5.28/home_assistant_intents/data/af.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    19955 2024-05-28 14:57:59.000000 home-assistant-intents-2024.5.28/home_assistant_intents/data/ar.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    61231 2024-05-28 14:57:59.000000 home-assistant-intents-2024.5.28/home_assistant_intents/data/bg.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2362 2024-05-28 14:57:59.000000 home-assistant-intents-2024.5.28/home_assistant_intents/data/bn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    20781 2024-05-28 14:57:59.000000 home-assistant-intents-2024.5.28/home_assistant_intents/data/ca.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    66715 2024-05-28 14:57:59.000000 home-assistant-intents-2024.5.28/home_assistant_intents/data/cs.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    22955 2024-05-28 14:57:59.000000 home-assistant-intents-2024.5.28/home_assistant_intents/data/da.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    30623 2024-05-28 14:57:59.000000 home-assistant-intents-2024.5.28/home_assistant_intents/data/de-CH.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    67458 2024-05-28 14:57:59.000000 home-assistant-intents-2024.5.28/home_assistant_intents/data/de.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    67879 2024-05-28 14:57:59.000000 home-assistant-intents-2024.5.28/home_assistant_intents/data/el.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)   115213 2024-05-28 14:57:59.000000 home-assistant-intents-2024.5.28/home_assistant_intents/data/en.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)   120565 2024-05-28 14:57:59.000000 home-assistant-intents-2024.5.28/home_assistant_intents/data/es.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1005 2024-05-28 14:57:59.000000 home-assistant-intents-2024.5.28/home_assistant_intents/data/et.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     6407 2024-05-28 14:57:59.000000 home-assistant-intents-2024.5.28/home_assistant_intents/data/eu.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3344 2024-05-28 14:57:59.000000 home-assistant-intents-2024.5.28/home_assistant_intents/data/fa.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    69080 2024-05-28 14:57:59.000000 home-assistant-intents-2024.5.28/home_assistant_intents/data/fi.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     9009 2024-05-28 14:57:59.000000 home-assistant-intents-2024.5.28/home_assistant_intents/data/fr-CA.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)   141130 2024-05-28 14:57:59.000000 home-assistant-intents-2024.5.28/home_assistant_intents/data/fr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    36322 2024-05-28 14:57:59.000000 home-assistant-intents-2024.5.28/home_assistant_intents/data/gl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1832 2024-05-28 14:57:59.000000 home-assistant-intents-2024.5.28/home_assistant_intents/data/gu.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    18301 2024-05-28 14:58:00.000000 home-assistant-intents-2024.5.28/home_assistant_intents/data/he.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1984 2024-05-28 14:58:00.000000 home-assistant-intents-2024.5.28/home_assistant_intents/data/hi.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    45624 2024-05-28 14:58:00.000000 home-assistant-intents-2024.5.28/home_assistant_intents/data/hr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)   115891 2024-05-28 14:58:00.000000 home-assistant-intents-2024.5.28/home_assistant_intents/data/hu.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4885 2024-05-28 14:58:00.000000 home-assistant-intents-2024.5.28/home_assistant_intents/data/id.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    20852 2024-05-28 14:58:00.000000 home-assistant-intents-2024.5.28/home_assistant_intents/data/is.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    37507 2024-05-28 14:58:00.000000 home-assistant-intents-2024.5.28/home_assistant_intents/data/it.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3989 2024-05-28 14:58:00.000000 home-assistant-intents-2024.5.28/home_assistant_intents/data/ka.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1656 2024-05-28 14:58:00.000000 home-assistant-intents-2024.5.28/home_assistant_intents/data/kn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    63797 2024-05-28 14:58:00.000000 home-assistant-intents-2024.5.28/home_assistant_intents/data/ko.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14734 2024-05-28 14:58:00.000000 home-assistant-intents-2024.5.28/home_assistant_intents/data/lb.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    13713 2024-05-28 14:58:00.000000 home-assistant-intents-2024.5.28/home_assistant_intents/data/lt.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11790 2024-05-28 14:58:00.000000 home-assistant-intents-2024.5.28/home_assistant_intents/data/lv.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14734 2024-05-28 14:58:00.000000 home-assistant-intents-2024.5.28/home_assistant_intents/data/ml.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1825 2024-05-28 14:58:00.000000 home-assistant-intents-2024.5.28/home_assistant_intents/data/mn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     6416 2024-05-28 14:58:00.000000 home-assistant-intents-2024.5.28/home_assistant_intents/data/ms.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    73076 2024-05-28 14:58:00.000000 home-assistant-intents-2024.5.28/home_assistant_intents/data/nb.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)   117660 2024-05-28 14:58:00.000000 home-assistant-intents-2024.5.28/home_assistant_intents/data/nl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    80016 2024-05-28 14:58:00.000000 home-assistant-intents-2024.5.28/home_assistant_intents/data/pl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    20655 2024-05-28 14:58:00.000000 home-assistant-intents-2024.5.28/home_assistant_intents/data/pt-br.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    19639 2024-05-28 14:58:00.000000 home-assistant-intents-2024.5.28/home_assistant_intents/data/pt.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)   107508 2024-05-28 14:58:00.000000 home-assistant-intents-2024.5.28/home_assistant_intents/data/ro.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)   107156 2024-05-28 14:58:00.000000 home-assistant-intents-2024.5.28/home_assistant_intents/data/ru.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    18266 2024-05-28 14:58:00.000000 home-assistant-intents-2024.5.28/home_assistant_intents/data/sk.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)   110627 2024-05-28 14:58:01.000000 home-assistant-intents-2024.5.28/home_assistant_intents/data/sl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    29113 2024-05-28 14:58:01.000000 home-assistant-intents-2024.5.28/home_assistant_intents/data/sr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    25291 2024-05-28 14:58:01.000000 home-assistant-intents-2024.5.28/home_assistant_intents/data/sv.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11284 2024-05-28 14:58:01.000000 home-assistant-intents-2024.5.28/home_assistant_intents/data/sw.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2219 2024-05-28 14:58:01.000000 home-assistant-intents-2024.5.28/home_assistant_intents/data/te.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     6456 2024-05-28 14:58:01.000000 home-assistant-intents-2024.5.28/home_assistant_intents/data/tr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    33881 2024-05-28 14:58:01.000000 home-assistant-intents-2024.5.28/home_assistant_intents/data/uk.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    16432 2024-05-28 14:58:01.000000 home-assistant-intents-2024.5.28/home_assistant_intents/data/ur.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    82818 2024-05-28 14:58:01.000000 home-assistant-intents-2024.5.28/home_assistant_intents/data/vi.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    19297 2024-05-28 14:58:01.000000 home-assistant-intents-2024.5.28/home_assistant_intents/data/zh-cn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    15749 2024-05-28 14:58:01.000000 home-assistant-intents-2024.5.28/home_assistant_intents/data/zh-hk.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    40899 2024-05-28 14:58:01.000000 home-assistant-intents-2024.5.28/home_assistant_intents/data/zh-tw.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      594 2024-05-28 14:58:01.000000 home-assistant-intents-2024.5.28/home_assistant_intents/languages.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2024-05-28 14:58:04.213718 home-assistant-intents-2024.5.28/home_assistant_intents.egg-info/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1338 2024-05-28 14:58:03.000000 home-assistant-intents-2024.5.28/home_assistant_intents.egg-info/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2377 2024-05-28 14:58:04.000000 home-assistant-intents-2024.5.28/home_assistant_intents.egg-info/SOURCES.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2024-05-28 14:58:03.000000 home-assistant-intents-2024.5.28/home_assistant_intents.egg-info/dependency_links.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       23 2024-05-28 14:58:04.000000 home-assistant-intents-2024.5.28/home_assistant_intents.egg-info/top_level.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-05-30 16:35:50.000000 home-assistant-intents-2024.5.28/home_assistant_intents.egg-info/zip-safe
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1082 2024-05-28 14:48:24.000000 home-assistant-intents-2024.5.28/pyproject.toml
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       38 2024-05-28 14:58:04.221718 home-assistant-intents-2024.5.28/setup.cfg
```

### Comparing `home-assistant-intents-2024.4.3/LICENSE.md` & `home-assistant-intents-2024.5.28/LICENSE.md`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2024.4.3/PKG-INFO` & `home-assistant-intents-2024.5.28/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: home-assistant-intents
-Version: 2024.4.3
+Version: 2024.5.28
 Summary: Intents for Home Assistant
 Author-email: The Home Assistant Authors <hello@home-assistant.io>
 License: Apache-2.0
 Project-URL: Source Code, https://github.com/home-assistant/intents
 Keywords: home,assistant,intent,recognition
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `home-assistant-intents-2024.4.3/README.md` & `home-assistant-intents-2024.5.28/README.md`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/__init__.py` & `home-assistant-intents-2024.5.28/home_assistant_intents/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -88,14 +88,29 @@
 
     DUPLICATE_ENTITIES_IN_AREA = "duplicate_entities_in_area"
     """More than one entity in an area matched with the same name."""
 
     DUPLICATE_ENTITIES_IN_FLOOR = "duplicate_entities_in_floor"
     """More than one entity in an floor matched with the same name."""
 
+    FEATURE_NOT_SUPPORTED = "feature_not_supported"
+    """Entity does not support a required feature."""
+
+    ENTITY_WRONG_STATE = "entity_wrong_state"
+    """Entity is not in the correct state."""
+
+    TIMER_NOT_FOUND = "timer_not_found"
+    """No timer matched the provided constraints."""
+
+    MULTIPLE_TIMERS_MATCHED = "multiple_timers_matched"
+    """More than one timer targeted for an action matched the constraints."""
+
+    NO_TIMER_SUPPORT = "no_timer_support"
+    """Vocie satellite does not support timers."""
+
 
 def get_intents(
     language: str,
     json_load: Callable[[IO[str]], Dict[str, Any]] = json.load,
 ) -> Optional[Dict[str, Any]]:
     """Load intents by language."""
     intents_path = _DATA_DIR / f"{language}.json"
```

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/data/af.json` & `home-assistant-intents-2024.5.28/home_assistant_intents/data/af.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/data/ar.json` & `home-assistant-intents-2024.5.28/home_assistant_intents/data/ar.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9826871141975309%*

 * *Differences: {"'expansion_rules'": "{'turn': '(غير|اضبط|أضبط|إضبط|ضبط)', 'turn_on': "*

 * *                      "'(افتح|إفتح|شغل|اشعل|أشعل|اشغل|أشغل|ابدأ|إبدأ|شعل|فعل|تفعيل|تشغيل|فعل)', "*

 * *                      "'turn_off': '(أغلق|اغلق|اطفئ|أطفئ|طفي)', 'open': '(افتح|إفتح|إرفع|ارفع)', "*

 * *                      "'close': '(أغلق|اغلق|اقفل|اخفض|انزل|نزل)'}",*

 * * "'lists'": "{'color': {'values': {0: {'in': '(ابيض|أبيض)'}, 1: {'in': '(اسود|أسود)'}, 2: {'in': "*

 * *            "'(احمر|أحمر)'}, 4: {'in': '(اصفر|أصفر)'}, 5: {'in': '(اخضر|أخض […]*

```diff
@@ -1,39 +1,39 @@
 {
     "expansion_rules": {
         "all": "(\u0643\u0644|\u062c\u0645\u064a\u0639)",
         "any": "(\u0623\u064a)",
         "area": "[\u0627\u0644]{area}",
         "awning": "[\u0627\u0644](\u0645\u0638\u0644\u0629|\u0645\u0638\u0644\u0627\u062a)",
         "brightness": "{brightness}[% | \u0628\u0627\u0644\u0645\u0627\u0626\u0629]",
-        "close": "(\u0627\u063a\u0644\u0642|\u0627\u0642\u0641\u0644|\u0627\u062e\u0641\u0636|\u0627\u0646\u0632\u0644|\u0646\u0632\u0644)",
+        "close": "(\u0623\u063a\u0644\u0642|\u0627\u063a\u0644\u0642|\u0627\u0642\u0641\u0644|\u0627\u062e\u0641\u0636|\u0627\u0646\u0632\u0644|\u0646\u0632\u0644)",
         "color": "[\u0627\u0644](\u0644\u0648\u0646|\u0627\u0644\u0648\u0627\u0646)",
         "colors": "[\u0627\u0644]{color}",
         "curtain": "[\u0627\u0644](\u0633\u062a\u0627\u0626\u0631|\u0633\u062a\u0627\u0631\u0629|\u0633\u062a\u0627\u0631\u0627\u062a)",
         "door": "[\u0627\u0644](\u0628\u0627\u0628|\u0627\u0628\u0648\u0627\u0628)",
         "fan": "[\u0627\u0644](\u0645\u0631\u0648\u062d\u0629|\u0645\u0631\u0627\u0648\u062d|\u0645\u0631\u0648\u062d\u0627\u062a)",
         "garage": "[\u0627\u0644](\u0628\u0627\u0628|\u0627\u0628\u0648\u0627\u0628|\u0628\u0648\u0627\u0628\u0629|\u0628\u0648\u0627\u0628\u0627\u062a) [\u0627\u0644]\u062c\u0631\u0627\u062c",
         "gate": "[\u0627\u0644](\u0628\u0648\u0627\u0628\u0629|\u0628\u0648\u0627\u0628\u0627\u062a)",
         "how_many": "\u0643\u0645 \u0639\u062f\u062f",
         "in": "(\u0641\u064a|\u062f\u0627\u062e\u0644)",
         "intensity": "[\u0627\u0644](\u062f\u0631\u062c\u0629 [\u0627\u0644]\u0633\u0637\u0648\u0639|[\u0634\u062f\u0629] [\u0627\u0644]\u0633\u0637\u0648\u0639|\u0642\u0648\u0629|\u0634\u062f\u0629)",
         "is_it": "(\u0647\u0644 [\u0647\u064a]|\u0647\u0644 [\u0647\u0648]|\u0647\u0644 \u0647\u0646\u0627\u0643)",
         "light": "[\u0627\u0644](\u0627\u0636\u0648\u0627\u0621|\u0627\u0636\u0627\u0621\u0629|\u0636\u0648\u0621|\u0645\u0635\u0627\u0628\u064a\u062d|\u0645\u0635\u0628\u0627\u062d|\u0627\u0646\u0648\u0627\u0631|\u0646\u0648\u0631|\u0644\u0645\u0628\u0629|\u0644\u0645\u0628\u0627\u062a|\u0627\u0646\u0648\u0627\u0631)",
         "lock": "[\u0627\u0644](\u0627\u0642\u0641\u0627\u0644|\u0642\u0641\u0644)",
         "name": "[\u0627\u0644]{name}",
-        "open": "(\u0627\u0641\u062a\u062d|\u0627\u0631\u0641\u0639)",
+        "open": "(\u0627\u0641\u062a\u062d|\u0625\u0641\u062a\u062d|\u0625\u0631\u0641\u0639|\u0627\u0631\u0641\u0639)",
         "scene": "[\u0627\u0644](\u0645\u0634\u0647\u062f|\u0645\u0634\u0627\u0647\u062f|\u0627\u0639\u062f\u0627\u062f\u0627\u062a)",
         "script": "[\u0627\u0644](\u0628\u0631\u0646\u0627\u0645\u062c|\u0628\u0631\u0627\u0645\u062c|\u0645\u0633\u0627\u0631|\u0645\u0633\u0627\u0631\u0627\u062a|\u0633\u064a\u0646\u0627\u0631\u064a\u0648)",
         "switch": "[\u0627\u0644](\u0645\u0641\u062a\u0627\u062d|\u0645\u0641\u0627\u062a\u064a\u062d)",
         "temp": "(\u0628\u0627\u0631\u062f\u0629|\u062f\u0627\u0641\u0626\u0629|\u0644\u0637\u064a\u0641\u0629|\u062d\u0627\u0631\u0629|\u062f\u0631\u062c\u0629 [\u0627\u0644]\u062d\u0631\u0627\u0631\u0629)",
         "temperature": "{temperature}[\u00b0| \u062f\u0631\u062c\u0629] [{temperature_unit}]",
         "to": "(\u0639\u0644\u0649|\u0627\u0644\u0649)",
-        "turn": "(\u063a\u064a\u0631|\u0627\u0636\u0628\u0637|\u0636\u0628\u0637)",
-        "turn_off": "(\u0627\u063a\u0644\u0642|\u0627\u0637\u0641\u0626|\u0637\u0641\u064a)",
-        "turn_on": "(\u0627\u0641\u062a\u062d|\u0634\u063a\u0644|\u0627\u0634\u0639\u0644|\u0627\u0634\u063a\u0644|\u0627\u0628\u062f\u0623|\u0634\u0639\u0644|\u0641\u0639\u0644|\u062a\u0641\u0639\u064a\u0644|\u062a\u0634\u063a\u064a\u0644|\u0641\u0639\u0644)",
+        "turn": "(\u063a\u064a\u0631|\u0627\u0636\u0628\u0637|\u0623\u0636\u0628\u0637|\u0625\u0636\u0628\u0637|\u0636\u0628\u0637)",
+        "turn_off": "(\u0623\u063a\u0644\u0642|\u0627\u063a\u0644\u0642|\u0627\u0637\u0641\u0626|\u0623\u0637\u0641\u0626|\u0637\u0641\u064a)",
+        "turn_on": "(\u0627\u0641\u062a\u062d|\u0625\u0641\u062a\u062d|\u0634\u063a\u0644|\u0627\u0634\u0639\u0644|\u0623\u0634\u0639\u0644|\u0627\u0634\u063a\u0644|\u0623\u0634\u063a\u0644|\u0627\u0628\u062f\u0623|\u0625\u0628\u062f\u0623|\u0634\u0639\u0644|\u0641\u0639\u0644|\u062a\u0641\u0639\u064a\u0644|\u062a\u0634\u063a\u064a\u0644|\u0641\u0639\u0644)",
         "what_is": "(\u0645\u0627 \u0647\u0648|\u0645\u0627 \u0647\u064a|\u0645\u0627\u0630\u0627 \u064a\u0643\u0648\u0646|\u0645\u0627\u0630\u0627 \u062a\u0643\u0648\u0646|\u0643\u0645 \u0647\u064a|\u0643\u0645 \u0647\u0648)",
         "window": "[\u0627\u0644](\u0646\u0627\u0641\u0630\u0629|\u0646\u0648\u0627\u0641\u0630|\u0646\u0627\u0641\u0630\u0627\u062a|\u0634\u0628\u0627\u0643|\u0634\u0628\u0627\u0628\u064a\u0643)"
     },
     "intents": {
         "HassClimateGetTemperature": {
             "data": [
                 {
@@ -485,39 +485,39 @@
                     "out": 1
                 }
             ]
         },
         "color": {
             "values": [
                 {
-                    "in": "\u0627\u0628\u064a\u0636",
+                    "in": "(\u0627\u0628\u064a\u0636|\u0623\u0628\u064a\u0636)",
                     "out": "white"
                 },
                 {
-                    "in": "\u0627\u0633\u0648\u062f",
+                    "in": "(\u0627\u0633\u0648\u062f|\u0623\u0633\u0648\u062f)",
                     "out": "black"
                 },
                 {
-                    "in": "\u0627\u062d\u0645\u0631",
+                    "in": "(\u0627\u062d\u0645\u0631|\u0623\u062d\u0645\u0631)",
                     "out": "red"
                 },
                 {
                     "in": "\u0628\u0631\u062a\u0642\u0627\u0644\u064a",
                     "out": "orange"
                 },
                 {
-                    "in": "\u0627\u0635\u0641\u0631",
+                    "in": "(\u0627\u0635\u0641\u0631|\u0623\u0635\u0641\u0631)",
                     "out": "yellow"
                 },
                 {
-                    "in": "\u0627\u062e\u0636\u0631",
+                    "in": "(\u0627\u062e\u0636\u0631|\u0623\u062e\u0636\u0631)",
                     "out": "green"
                 },
                 {
-                    "in": "\u0627\u0632\u0631\u0642",
+                    "in": "(\u0627\u0632\u0631\u0642|\u0623\u0632\u0631\u0642)",
                     "out": "blue"
                 },
                 {
                     "in": "\u0628\u0646\u0641\u0633\u062c\u064a",
                     "out": "purple"
                 },
                 {
@@ -622,20 +622,20 @@
                     "out": "fahrenheit"
                 }
             ]
         }
     },
     "responses": {
         "errors": {
-            "handle_error": "\u062d\u062f\u062b \u062e\u0637\u0623 \u0627\u062b\u0646\u0627\u0621 \u0645\u0639\u0627\u0644\u062c\u0629 \u0627\u0644\u0646\u0635",
-            "no_area": "\u0644\u0627 \u062a\u0648\u062c\u062f \u0645\u0646\u0637\u0642\u0629 \u0628\u0627\u0644\u0623\u0633\u0645 {{ area }}",
-            "no_device_class_in_area": "\u0627\u0644\u0645\u0646\u0637\u0642\u0629 {{ area }} \u0644\u0627 \u062a\u062d\u062a\u0648\u0649 \u0639\u0644\u0649 \u0641\u0626\u0629 \u0627\u0644\u0623\u062c\u0647\u0632\u0629 {{ device_class }}",
-            "no_domain_in_area": "\u0627\u0644\u0646\u0637\u0627\u0642 {{ domain }} \u063a\u064a\u0631 \u0645\u0648\u062c\u0648\u062f \u0628\u0627\u0644\u0645\u0646\u0637\u0642\u0629 {{ area }}",
-            "no_entity": "\u0644\u0627 \u064a\u0648\u062c\u062f \u062c\u0647\u0627\u0632 \u0627\u0648 \u062e\u0627\u0635\u064a\u0629 \u0628\u0627\u0644\u0623\u0633\u0645 {{ entity }}",
-            "no_intent": "\u0639\u0641\u0648\u0627, \u0644\u0645 \u0627\u0641\u0647\u0645 \u0647\u0630\u0627"
+            "handle_error": "\u062d\u062f\u062b \u062e\u0637\u0623 \u0623\u062b\u0646\u0627\u0621 \u0645\u0639\u0627\u0644\u062c\u0629 \u0627\u0644\u0646\u0635",
+            "no_area": "\u0639\u0641\u0648\u0627\u060c \u0644\u0627 \u062a\u0648\u062c\u062f \u0645\u0646\u0637\u0642\u0629 \u0628\u0627\u0644\u0625\u0633\u0645 {{ area }}",
+            "no_device_class_in_area": "\u0639\u0641\u0648\u0627\u060c \u0627\u0644\u0645\u0646\u0637\u0642\u0629 {{ area }} \u0644\u0627 \u062a\u062d\u062a\u0648\u0649 \u0639\u0644\u0649 \u0641\u0626\u0629 \u0627\u0644\u0623\u062c\u0647\u0632\u0629 {{ device_class }}",
+            "no_domain_in_area": "\u0639\u0641\u0648\u0627\u060c \u0627\u0644\u0646\u0637\u0627\u0642 {{ domain }} \u063a\u064a\u0631 \u0645\u0648\u062c\u0648\u062f \u0628\u0627\u0644\u0645\u0646\u0637\u0642\u0629 {{ area }}",
+            "no_entity": "\u0639\u0641\u0648\u0627\u060c \u0644\u0627 \u064a\u0648\u062c\u062f \u062c\u0647\u0627\u0632 \u0627\u0648 \u062e\u0627\u0635\u064a\u0629 \u0628\u0627\u0644\u0625\u0633\u0645 {{ entity }}",
+            "no_intent": "\u0639\u0641\u0648\u0627\u060c \u0644\u0645 \u0623\u0641\u0647\u0645 \u0647\u0630\u0627"
         },
         "intents": {
             "HassClimateGetTemperature": {
                 "default": "{{ state_attr(state.entity_id, 'current_temperature') }}"
             },
             "HassGetState": {
                 "all": "{% if not query.unmatched: %}\n  \u0627\u062c\u0644\n{% else %}\n  {% set no_match = query.unmatched | map(attribute=\"name\") | sort | list %}\n  {% if no_match | length > 4 %}\n    \u0644\u0627, {{ no_match[:3] | join(\", \") }} \u0648 {{ (no_match | length - 3) }} \u0627\u064a\u0636\u0627\n  {%- else -%}\n    \u0644\u0627,\n    {% for name in no_match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} \u0648 {% endif -%}\n      {{ name }}\n    {%- endfor %} \u0644\u064a\u0633\u062a\n  {% endif %}\n{% endif %}\n",
```

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/data/bg.json` & `home-assistant-intents-2024.5.28/home_assistant_intents/data/bg.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9843548906048906%*

 * *Differences: {"'intents'": "{'HassListAddItem': OrderedDict([('data', [OrderedDict([('sentences', ['добави "*

 * *              "<item> (в|към) <my_list>', 'сложи <item> (в|към) <my_list>', 'прибави <item> "*

 * *              "(в|към) <my_list>', 'запиши <item> (в|към) <my_list>']), ('response', "*

 * *              "'item_added'), ('requires_context', OrderedDict([('domain', 'todo')])), "*

 * *              "('expansion_rules', OrderedDict([('my_list', '[ моя| моите] [ списък| списъка| "*

 * *              "списъка ми] [с|със|за] {name} [ми]' […]*

```diff
@@ -839,14 +839,34 @@
                     "slots": {
                         "brightness": 1,
                         "name": "all"
                     }
                 }
             ]
         },
+        "HassListAddItem": {
+            "data": [
+                {
+                    "expansion_rules": {
+                        "item": "{shopping_list_item:item}",
+                        "my_list": "[ \u043c\u043e\u044f| \u043c\u043e\u0438\u0442\u0435] [ \u0441\u043f\u0438\u0441\u044a\u043a| \u0441\u043f\u0438\u0441\u044a\u043a\u0430| \u0441\u043f\u0438\u0441\u044a\u043a\u0430 \u043c\u0438] [\u0441|\u0441\u044a\u0441|\u0437\u0430] {name} [\u043c\u0438]"
+                    },
+                    "requires_context": {
+                        "domain": "todo"
+                    },
+                    "response": "item_added",
+                    "sentences": [
+                        "\u0434\u043e\u0431\u0430\u0432\u0438 <item> (\u0432|\u043a\u044a\u043c) <my_list>",
+                        "\u0441\u043b\u043e\u0436\u0438 <item> (\u0432|\u043a\u044a\u043c) <my_list>",
+                        "\u043f\u0440\u0438\u0431\u0430\u0432\u0438 <item> (\u0432|\u043a\u044a\u043c) <my_list>",
+                        "\u0437\u0430\u043f\u0438\u0448\u0438 <item> (\u0432|\u043a\u044a\u043c) <my_list>"
+                    ]
+                }
+            ]
+        },
         "HassNevermind": {
             "data": [
                 {
                     "sentences": [
                         "\u0437\u0430\u0431\u0440\u0430\u0432\u0438",
                         "\u043e\u0442\u043a\u0430\u0436\u0438",
                         "\u043d\u044f\u043c\u0430 \u043d\u0438\u0449\u043e",
@@ -1487,14 +1507,17 @@
                 },
                 {
                     "in": "\u0438\u0437\u043a\u043b\u044e\u0447\u0435\u043d[\u0430|\u043e|\u0438|\u0438\u044f\u0442|\u0438\u0442\u0435|\u043e\u0442\u043e|\u0430\u0442\u0430]",
                     "out": "off"
                 }
             ]
         },
+        "shopping_list_item": {
+            "wildcard": true
+        },
         "temperature": {
             "range": {
                 "from": 0,
                 "to": 100,
                 "type": "temperature"
             }
         },
@@ -1537,14 +1560,17 @@
             },
             "HassLightSet": {
                 "brightness": "\u042f\u0440\u043a\u043e\u0441\u0442\u0442\u0430 \u043d\u0430 {{ slots.name }} \u0435 \u043d\u0430\u0441\u0442\u0440\u043e\u0435\u043d\u0430 \u043d\u0430 {{ slots.brightness }}",
                 "brightness_area": "\u042f\u0440\u043a\u043e\u0441\u0442\u0442\u0430 \u0432 {{ slots.area }} \u0435 \u043d\u0430\u0441\u0442\u0440\u043e\u0435\u043d\u0430 \u043d\u0430 {{ slots.brightness }}",
                 "color": "\u0426\u0432\u0435\u0442\u044a\u0442 \u043d\u0430 {{ slots.name }} \u0435 \u043d\u0430\u0441\u0442\u0440\u043e\u0435\u043d \u043d\u0430 {{ slots.color }}",
                 "color_area": "\u0426\u0432\u0435\u0442\u044a\u0442 \u0432 {{ slots.area }} \u0435 \u043d\u0430\u0441\u0442\u0440\u043e\u0435\u043d \u043d\u0430 {{ slots.color }}"
             },
+            "HassListAddItem": {
+                "item_added": "\u0414\u043e\u0431\u0430\u0432\u0438\u0445 {{ slots.item }}"
+            },
             "HassTurnOff": {
                 "cover": "\u0417\u0430\u0442\u0432\u043e\u0440\u0438\u0445 {{ slots.name }}",
                 "cover_area": "\u0417\u0430\u0442\u0432\u043e\u0440\u0438\u0445 {{ slots.area }}",
                 "cover_device_class": "\u0417\u0430\u0442\u0432\u043e\u0440\u0438\u0445 {{ slots.device_class }}",
                 "default": "\u0418\u0437\u043a\u043b\u044e\u0447\u0438\u0445 {{ slots.name }}",
                 "fans_area": "\u0418\u0437\u043a\u043b\u044e\u0447\u0438\u0445 \u0432\u0435\u043d\u0442\u0438\u043b\u0430\u0442\u043e\u0440\u0438\u0442\u0435 \u0432 {{ slots.area }}",
                 "light": "\u0418\u0437\u0433\u0430\u0441\u0438\u0445 {{ slots.name }}",
```

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/data/bn.json` & `home-assistant-intents-2024.5.28/home_assistant_intents/data/bn.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/data/ca.json` & `home-assistant-intents-2024.5.28/home_assistant_intents/data/ca.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998597081930415%*

 * *Differences: {"'intents'": "{'HassTurnOff': {'data': {4: {'sentences': ['(<tanca>|<baixar>) [(la|les)] "*

 * *              "port(a|es) [del] garatge']}, 5: {'sentences': ['(<tanca>|<baixar>) [(la|les)] "*

 * *              "persian(a|es) <area>']}, 6: {'sentences': ['(<tanca>|<baixar>) [(la|les)] "*

 * *              "cortin(a|es) <area>']}}}, 'HassTurnOn': {'data': {8: {'sentences': "*

 * *              "['(<obre>|<pujar>) [(la|les)] port(a|es) [del] garatge']}, 9: {'sentences': "*

 * *              "['(<obre>|<pujar>) [(la|les)] persian(a|es […]*

```diff
@@ -264,38 +264,38 @@
                     "slots": {
                         "domain": "light"
                     }
                 },
                 {
                     "response": "cover_device_class",
                     "sentences": [
-                        "<tanca> [(la|les)] port(a|es) [del] garatge"
+                        "(<tanca>|<baixar>) [(la|les)] port(a|es) [del] garatge"
                     ],
                     "slots": {
                         "device_class": "garage",
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "cover_area",
                     "sentences": [
-                        "<tanca> [(la|les)] persian(a|es) <area>"
+                        "(<tanca>|<baixar>) [(la|les)] persian(a|es) <area>"
                     ],
                     "slots": {
                         "device_class": [
                             "blind",
                             "shutter"
                         ],
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "cover_area",
                     "sentences": [
-                        "<tanca> [(la|les)] cortin(a|es) <area>"
+                        "(<tanca>|<baixar>) [(la|les)] cortin(a|es) <area>"
                     ],
                     "slots": {
                         "device_class": "curtain",
                         "domain": "cover"
                     }
                 },
                 {
@@ -396,38 +396,38 @@
                     "sentences": [
                         "<obre> <name> [<area>]"
                     ]
                 },
                 {
                     "response": "cover_device_class",
                     "sentences": [
-                        "<obre> [(la|les)] port(a|es) [del] garatge"
+                        "(<obre>|<pujar>) [(la|les)] port(a|es) [del] garatge"
                     ],
                     "slots": {
                         "device_class": "garage",
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "cover_area",
                     "sentences": [
-                        "<obre> [(la|les)] persian(a|es) <area>"
+                        "(<obre>|<pujar>) [(la|les)] persian(a|es) <area>"
                     ],
                     "slots": {
                         "device_class": [
                             "blind",
                             "shutter"
                         ],
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "cover_area",
                     "sentences": [
-                        "<obre> [(la|les)] cortin(a|es) <area>"
+                        "(<obre>|<pujar>) [(la|les)] cortin(a|es) <area>"
                     ],
                     "slots": {
                         "device_class": "curtain",
                         "domain": "cover"
                     }
                 }
             ]
```

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/data/cs.json` & `home-assistant-intents-2024.5.28/home_assistant_intents/data/cs.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/data/da.json` & `home-assistant-intents-2024.5.28/home_assistant_intents/data/da.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/data/de-CH.json` & `home-assistant-intents-2024.5.28/home_assistant_intents/data/de-CH.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/data/de.json` & `home-assistant-intents-2024.5.28/home_assistant_intents/data/de.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9916338609307359%*

 * *Differences: {"'expansion_rules'": "{'floor': '[in|auf] [<artikel>|im|<von_dem>] {floor} [Geschoss]'}",*

 * * "'intents'": "{'HassTurnOff': {'data': {insert: [(3, OrderedDict([('sentences', ['<schalten> "*

 * *              "(<licht>|<lichter>|<alle_lichter>) <floor> <aus>', '<schalten> <floor> "*

 * *              "(<licht>|<lichter>|<alle_lichter>) <aus>', '(<licht>|<lichter>|<alle_lichter>) "*

 * *              "<floor> <aus>[<schalten>]', '(<licht>|<lichter>|<alle_lichter>) <aus>[<schalten>] "*

 * *              "<floor>', '<floor> (<licht> […]*

```diff
@@ -22,14 +22,15 @@
         "co": "Kohlen[stoff]monoxid",
         "co_sensor": "<co>[-]Sensor[en]",
         "deaktivieren": "de<aktivieren>",
         "ding": "((Ding|Ger\u00e4t)[e|en]|Sensor[en]|Gegenstand|Gegenst\u00e4nde[n])",
         "entsperren": "((ent|auf)<sperren>|\u00f6ffne|entrieg(el|le))[n]",
         "erkannt": "(entdeckt|ausgel\u00f6st|erkannt|an)",
         "etwas": "[irgend][et]was",
+        "floor": "[in|auf] [<artikel>|im|<von_dem>] {floor} [Geschoss]",
         "garage": "<artikel> (Garage[n]|Garagentor[e])",
         "gas_sensor": "Gas[-]Sensor[en]",
         "irgend": "(irgend(<artikel_unbestimmt>[s]|welche[s]|wo)|(einige|manche)[s]|<artikel_unbestimmt>[s]) <artikel_bestimmt>",
         "ist_wurde": "(ist|wurde)",
         "ladestand": "<artikel> [Lade][zu]Stand",
         "leuchten_lassen": "([er]leuchten lassen|[ein]f\u00e4rben)",
         "licht": "<artikel> (Licht|Lampe|Beleuchtung)",
@@ -1123,14 +1124,31 @@
                         "(<licht>|<lichter>) [hier] <aus><machen>"
                     ],
                     "slots": {
                         "domain": "light"
                     }
                 },
                 {
+                    "response": "light",
+                    "sentences": [
+                        "<schalten> (<licht>|<lichter>|<alle_lichter>) <floor> <aus>",
+                        "<schalten> <floor> (<licht>|<lichter>|<alle_lichter>) <aus>",
+                        "(<licht>|<lichter>|<alle_lichter>) <floor> <aus>[<schalten>]",
+                        "(<licht>|<lichter>|<alle_lichter>) <aus>[<schalten>] <floor>",
+                        "<floor> (<licht>|<lichter>|<alle_lichter>) <aus>[<schalten>]",
+                        "<machen> <floor> (<licht>|<lichter>|<alle_lichter>) <aus>",
+                        "<machen> (<licht>|<lichter>|<alle_lichter>) <floor> <aus>",
+                        "(<licht>|<lichter>|<alle_lichter>) <floor> <aus><machen>",
+                        "<floor> (<licht>|<lichter>|<alle_lichter>) <aus><machen>"
+                    ],
+                    "slots": {
+                        "domain": "light"
+                    }
+                },
+                {
                     "requires_context": {
                         "domain": "cover"
                     },
                     "response": "cover",
                     "sentences": [
                         "<schliessen> <name>",
                         "<name> <schliessen>",
@@ -1282,14 +1300,31 @@
                         "(<licht>|<lichter>) [hier] <an><machen>"
                     ],
                     "slots": {
                         "domain": "light"
                     }
                 },
                 {
+                    "response": "light",
+                    "sentences": [
+                        "<schalten> (<licht>|<lichter>|<alle_lichter>) <floor> <an>",
+                        "<schalten> <floor> (<licht>|<lichter>|<alle_lichter>) <an>",
+                        "(<licht>|<lichter>|<alle_lichter>) <floor> <an>[<schalten>]",
+                        "(<licht>|<lichter>|<alle_lichter>) <an>[<schalten>] <floor>",
+                        "<floor> (<licht>|<lichter>|<alle_lichter>) <an>[<schalten>]",
+                        "<machen> <floor> (<licht>|<lichter>|<alle_lichter>) <an>",
+                        "<machen> (<licht>|<lichter>|<alle_lichter>) <floor> <an>",
+                        "(<licht>|<lichter>|<alle_lichter>) <floor> <an><machen>",
+                        "<floor> (<licht>|<lichter>|<alle_lichter>) <an><machen>"
+                    ],
+                    "slots": {
+                        "domain": "light"
+                    }
+                },
+                {
                     "response": "fan_all",
                     "sentences": [
                         "<schalten> <luefter> <area> <an>",
                         "<schalten> <area> <luefter> <an>",
                         "starte <luefter> <area> [<an>]",
                         "starte <area> <luefter> [<an>]",
                         "<machen> <luefter> <area> <an>",
@@ -1872,28 +1907,36 @@
             ]
         }
     },
     "responses": {
         "errors": {
             "duplicate_entities": "Es wurden mehrere {{ entity }} gefunden",
             "duplicate_entities_in_area": "Im Bereich {{ area }} wurden mehrere {{ entity }} gefunden",
+            "duplicate_entities_in_floor": "In der Etage {{ floor }} wurden mehrere {{ entity }} gefunden",
             "handle_error": "Es ist ein unerwarteter Fehler aufgetreten",
             "no_area": "Kein Bereich mit dem Namen {{ area }} vorhanden",
             "no_device_class": "Kein {{ device_class }} vorhanden",
             "no_device_class_exposed": "Es ist kein {{ device_class }} freigegeben",
             "no_device_class_in_area": "Im Bereich {{ area }} ist kein {{ device_class }} vorhanden",
             "no_device_class_in_area_exposed": "Im Bereich {{ area }} ist kein {{ device_class }} freigegeben",
+            "no_device_class_in_floor": "In der Etage {{ floor }} ist kein {{ device_class }} vorhanden",
+            "no_device_class_in_floor_exposed": "In der Etage {{ floor }} ist kein {{ device_class }} freigegeben",
             "no_domain": "Kein {{ domain }} vorhanden",
             "no_domain_exposed": "Es ist kein {{ domain }} freigegeben",
             "no_domain_in_area": "Im Bereich {{ area }} ist kein {{ domain }} vorhanden",
             "no_domain_in_area_exposed": "Im Bereich {{ area }} ist kein {{ domain }} freigegeben",
+            "no_domain_in_floor": "In der Etage {{ floor }} ist kein {{ domain }} vorhanden",
+            "no_domain_in_floor_exposed": "In der Etage {{ floor }} ist kein {{ domain }} freigegeben",
             "no_entity": "{{ entity }} existiert nicht",
             "no_entity_exposed": "{{ entity }} ist nicht freigegeben",
             "no_entity_in_area": "{{ entity }} ist im Bereich {{ area }} nicht vorhanden",
             "no_entity_in_area_exposed": "{{ entity }} ist im Bereich {{ area }} nicht freigegeben",
+            "no_entity_in_floor": "{{ entity }} ist in der Etage {{ floor }} nicht vorhanden",
+            "no_entity_in_floor_exposed": "{{ entity }} ist in der Etage {{ floor }} nicht freigegeben",
+            "no_floor": "Keine Etage mit dem Namen {{ floor }} vorhanden",
             "no_intent": "Entschuldigung, das habe ich nicht verstanden"
         },
         "intents": {
             "HassClimateGetTemperature": {
                 "default": "{{ state_attr(state.entity_id, 'current_temperature') }}"
             },
             "HassGetState": {
```

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/data/el.json` & `home-assistant-intents-2024.5.28/home_assistant_intents/data/el.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/data/en.json` & `home-assistant-intents-2024.5.28/home_assistant_intents/data/en.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9284353956228957%*

 * *Differences: {"'expansion_rules'": "{'timer_set': '(start|set|create)', 'timer_cancel': '(cancel|stop)', "*

 * *                      "'timer_duration_seconds': '{timer_seconds:seconds} second[s]', "*

 * *                      "'timer_duration_minutes': '{timer_minutes:minutes} minute[s][ [and "*

 * *                      "]{timer_seconds:seconds} second[s]]', 'timer_duration_hours': "*

 * *                      "'{timer_hours:hours} hour[s][ [and ]{timer_minutes:minutes} minute[s]][ "*

 * *                      "[and ]{timer_seconds:seconds} s […]*

```diff
@@ -13,21 +13,46 @@
         "name": "[the] {name}",
         "numeric_value_set": "(set|change|turn|increase|decrease|make)",
         "open": "(open|raise)",
         "position": "{position}[[ ]%| percent]",
         "set": "(set|make|change|turn)",
         "temp": "(temp|temperature)",
         "temperature": "{temperature}[ ][\u00b0|degrees][ ][{temperature_unit}]",
+        "timer_cancel": "(cancel|stop)",
+        "timer_duration": "<timer_duration_seconds>|<timer_duration_minutes>|<timer_duration_hours>",
+        "timer_duration_hours": "{timer_hours:hours} hour[s][ [and ]{timer_minutes:minutes} minute[s]][ [and ]{timer_seconds:seconds} second[s]]",
+        "timer_duration_minutes": "{timer_minutes:minutes} minute[s][ [and ]{timer_seconds:seconds} second[s]]",
+        "timer_duration_seconds": "{timer_seconds:seconds} second[s]",
+        "timer_set": "(start|set|create)",
+        "timer_start": "<timer_start_seconds>|<timer_start_minutes>|<timer_start_hours>",
+        "timer_start_hours": "{timer_hours:start_hours} hour[s][ [and ]{timer_minutes:start_minutes} minute[s]][ [and ]{timer_seconds:start_seconds} second[s]]",
+        "timer_start_minutes": "{timer_minutes:start_minutes} minute[s][ [and ]{timer_seconds:start_seconds} second[s]]",
+        "timer_start_seconds": "{timer_seconds:start_seconds} second[s]",
         "turn": "(turn|switch|change)",
         "volume": "{volume:volume_level}[[ ]%| percent]",
         "what_is": "(what's|whats|what is)",
         "what_is_the_class_of_name": "(<what_is> the <class> (of|in|from|(indicated|measured) by) <name> [in <area>]|<what_is> <name>['s] <class> [in <area>]|<what_is> <area> <name>['s] <class>)",
         "where_is": "(where's|wheres|where is)"
     },
     "intents": {
+        "HassCancelTimer": {
+            "data": [
+                {
+                    "sentences": [
+                        "<timer_cancel>[ the| my] timer",
+                        "<timer_cancel>[ the| my] <timer_start> timer",
+                        "<timer_cancel>[ the| my] timer for <timer_start>",
+                        "<timer_cancel>[ the| my] {area} timer",
+                        "<timer_cancel>[ the| my] timer in <area>",
+                        "<timer_cancel>[ the| my] {timer_name:name} timer",
+                        "<timer_cancel>[ the| my] timer for {timer_name:name}"
+                    ]
+                }
+            ]
+        },
         "HassClimateGetTemperature": {
             "data": [
                 {
                     "sentences": [
                         "<what_is> [the][ current] <temp> [in <area>]",
                         "how (hot | cold | warm | cool) is it [in <area>]",
                         "is it (hot | cold | warm | cool) [in <area>]",
@@ -42,14 +67,40 @@
                         "<what_is> <name>[ current] <temp>",
                         "<what_is>[ the][ current] <temp>[ of] <name>",
                         "how (hot | cold | warm | cool) is <name>"
                     ]
                 }
             ]
         },
+        "HassDecreaseTimer": {
+            "data": [
+                {
+                    "sentences": [
+                        "remove <timer_duration> from[ the| my] timer",
+                        "remove <timer_duration> from[ the| my] <timer_start> timer",
+                        "remove <timer_duration> from[ the| my] timer for <timer_start>",
+                        "remove <timer_duration> from[ the| my] {area} timer",
+                        "remove <timer_duration> from[ the| my] timer in <area>",
+                        "remove <timer_duration> from[ the| my] {timer_name:name} timer",
+                        "remove <timer_duration> from[ the| my] timer (named|called|for) {timer_name:name}"
+                    ]
+                },
+                {
+                    "sentences": [
+                        "decrease[ the| my] timer by <timer_duration>",
+                        "decrease[ the| my] <timer_start> timer by <timer_duration>",
+                        "decrease[ the| my] timer for <timer_start> by <timer_duration>",
+                        "decrease[ the| my] {area} timer by <timer_duration>",
+                        "decrease[ the| my] timer in <area> by <timer_duration>",
+                        "decrease[ the| my] {timer_name:name} timer by <timer_duration>",
+                        "decrease[ the| my] timer (named|called|for) {timer_name:name} by <timer_duration>"
+                    ]
+                }
+            ]
+        },
         "HassGetState": {
             "data": [
                 {
                     "requires_context": {
                         "domain": "person"
                     },
                     "response": "where",
@@ -2288,14 +2339,40 @@
                         "<what_is>[ the] weather[ like] (for|in|at) <name>",
                         "<what_is>[ the] weather (for|in|at) <name>[ like]",
                         "<what_is>[ the] <name> weather[ like]"
                     ]
                 }
             ]
         },
+        "HassIncreaseTimer": {
+            "data": [
+                {
+                    "sentences": [
+                        "add <timer_duration> to[ the| my] timer",
+                        "add <timer_duration> to[ the| my] <timer_start> timer",
+                        "add <timer_duration> to[ the| my] timer for <timer_start>",
+                        "add <timer_duration> to[ the| my] {area} timer",
+                        "add <timer_duration> to[ the| my] timer in <area>",
+                        "add <timer_duration> to[ the| my] {timer_name:name} timer",
+                        "add <timer_duration> to[ the| my] timer (named|called|for) {timer_name:name}"
+                    ]
+                },
+                {
+                    "sentences": [
+                        "increase[ the| my] timer by <timer_duration>",
+                        "increase[ the| my] <timer_start> timer by <timer_duration>",
+                        "increase[ the| my] timer for <timer_start> by <timer_duration>",
+                        "increase[ the| my] {area} timer by <timer_duration>",
+                        "increase[ the| my] timer in <area> by <timer_duration>",
+                        "increase[ the| my] {timer_name:name} timer by <timer_duration>",
+                        "increase[ the| my] timer (named|called|for) {timer_name:name} by <timer_duration>"
+                    ]
+                }
+            ]
+        },
         "HassLightSet": {
             "data": [
                 {
                     "requires_context": {
                         "domain": "light"
                     },
                     "response": "brightness",
@@ -2451,51 +2528,115 @@
                     "requires_context": {
                         "domain": "media_player"
                     },
                     "sentences": [
                         "next [track|item] [on|for] <name>",
                         "(skip [(to [the ]next [(song|track)]|([the ](song|track)|this [(song|track)]) )];[on ]<name>)"
                     ]
+                },
+                {
+                    "requires_context": {
+                        "area": {
+                            "slot": true
+                        }
+                    },
+                    "sentences": [
+                        "next [track|item]",
+                        "(skip [(to [the ]next [(song|track)]|([the ](song|track)|this [(song|track)]))])"
+                    ]
+                },
+                {
+                    "sentences": [
+                        "next [track|item] [in ]<area>",
+                        "(skip [(to [the ]next [(song|track)]|([the ](song|track)|this [(song|track)]) )];[in ]<area>)"
+                    ]
                 }
             ]
         },
         "HassMediaPause": {
             "data": [
                 {
                     "requires_context": {
                         "domain": "media_player"
                     },
                     "sentences": [
                         "(pause;<name>)"
                     ]
+                },
+                {
+                    "requires_context": {
+                        "area": {
+                            "slot": true
+                        }
+                    },
+                    "sentences": [
+                        "pause"
+                    ]
+                },
+                {
+                    "sentences": [
+                        "pause[ [the |my ](music|[tv ]show[s]|media[ player[s]]) ][ in] <area>",
+                        "pause <area> (music|[tv ]show[s]|media[ player[s]])"
+                    ]
                 }
             ]
         },
         "HassMediaUnpause": {
             "data": [
                 {
                     "requires_context": {
                         "domain": "media_player"
                     },
                     "sentences": [
                         "((unpause|resume);<name>)"
                     ]
+                },
+                {
+                    "requires_context": {
+                        "area": {
+                            "slot": true
+                        }
+                    },
+                    "sentences": [
+                        "(unpause|resume)"
+                    ]
+                },
+                {
+                    "sentences": [
+                        "(unpause|resume)[ [the |my ](music|[tv ]show[s]|media[ player[s]]) ][ in] <area>",
+                        "(unpause|resume) <area> (music|[tv ]show[s]|media[ player[s]])"
+                    ]
                 }
             ]
         },
         "HassNevermind": {
             "data": [
                 {
                     "sentences": [
                         "nevermind",
                         "never mind"
                     ]
                 }
             ]
         },
+        "HassPauseTimer": {
+            "data": [
+                {
+                    "sentences": [
+                        "pause[ the| my] timer",
+                        "pause[ the| my] <timer_start> timer",
+                        "pause[ the| my] timer for <timer_start>",
+                        "pause[ the| my] {area} timer",
+                        "pause[ the| my] timer in <area>",
+                        "pause[ the| my] {timer_name:name} timer",
+                        "pause[ the| my] timer (named|called|for) {timer_name:name}"
+                    ]
+                }
+            ]
+        },
         "HassSetPosition": {
             "data": [
                 {
                     "requires_context": {
                         "domain": "valve"
                     },
                     "sentences": [
@@ -2535,14 +2676,37 @@
                     },
                     "sentences": [
                         "<numeric_value_set> <name> volume to <volume> [percent]",
                         "turn <name> [volume] (up|down) to <volume> [percent]",
                         "(<numeric_value_set> the volume to <volume> [percent];[on ]<name>)",
                         "(turn (the volume;(up|down)) to <volume> [percent];[on ]<name>)"
                     ]
+                },
+                {
+                    "requires_context": {
+                        "area": {
+                            "slot": true
+                        }
+                    },
+                    "sentences": [
+                        "<numeric_value_set> volume to <volume> [percent]",
+                        "turn volume (up|down) to <volume> [percent]",
+                        "<numeric_value_set> the volume to <volume> [percent]",
+                        "turn (the volume;(up|down)) to <volume> [percent]"
+                    ]
+                },
+                {
+                    "sentences": [
+                        "<numeric_value_set> <area> volume to <volume> [percent]",
+                        "turn <area> [volume] (up|down) to <volume> [percent]",
+                        "turn [volume] (up|down) to <volume> [percent][in ]<area>",
+                        "(<numeric_value_set> the volume to <volume> [percent];[in ]<area>)",
+                        "<numeric_value_set> the volume [in ]<area> to <volume> [percent]",
+                        "(turn (the volume;(up|down)) to <volume> [percent];[in ]<area>)"
+                    ]
                 }
             ]
         },
         "HassShoppingListAddItem": {
             "data": [
                 {
                     "expansion_rules": {
@@ -2553,14 +2717,58 @@
                     "sentences": [
                         "add <item> to<my_list>",
                         "put <item> (on|in)<my_list>"
                     ]
                 }
             ]
         },
+        "HassStartTimer": {
+            "data": [
+                {
+                    "requires_context": {
+                        "area": {
+                            "slot": false
+                        }
+                    },
+                    "sentences": [
+                        "<timer_duration> timer",
+                        "timer for <timer_duration>",
+                        "<timer_duration> timer for {timer_name:name}",
+                        "timer for <timer_duration> (named|called) {timer_name:name}",
+                        "<timer_set>[ a] <timer_duration> timer",
+                        "<timer_set>[ a] timer for <timer_duration>",
+                        "<timer_set>[ a] <timer_duration> timer (named|called|for) {timer_name:name}",
+                        "<timer_set>[ a] timer (named|called) {timer_name:name} for <timer_duration>",
+                        "<timer_set>[ a] timer for <timer_duration> (named|called) {timer_name:name}"
+                    ]
+                }
+            ]
+        },
+        "HassTimerStatus": {
+            "data": [
+                {
+                    "sentences": [
+                        "timer[s] status",
+                        "status of[ the| my] timer[s]",
+                        "[how much ]time[ is] left on[ the| my] timer[s]",
+                        "<timer_start> timer status",
+                        "status of[ the| my] <timer_start> timer",
+                        "[how much ]time[ is] left on[ the| my] <timer_start> timer",
+                        "{area} timer status",
+                        "status of[ the| my] {area} timer[s]",
+                        "status of[ the| my] timer[s] in <area>",
+                        "[how much ]time[ is] left on[ the| my] {area} timer",
+                        "[how much ]time[ is] left on[ the| my] timer[s] in <area>",
+                        "{timer_name:name} timer status",
+                        "status of[ the| my] {timer_name:name} timer[s]",
+                        "[how much ]time[ is] left on[ the| my] {timer_name:name} timer"
+                    ]
+                }
+            ]
+        },
         "HassTurnOff": {
             "data": [
                 {
                     "excludes_context": {
                         "domain": [
                             "binary_sensor",
                             "cover",
@@ -3041,14 +3249,29 @@
                     ],
                     "slots": {
                         "domain": "cover"
                     }
                 }
             ]
         },
+        "HassUnpauseTimer": {
+            "data": [
+                {
+                    "sentences": [
+                        "(resume|continue)[ the| my] timer",
+                        "(resume|continue)[ the| my] <timer_start> timer",
+                        "(resume|continue)[ the| my] timer for <timer_start>",
+                        "(resume|continue)[ the| my] {area} timer",
+                        "(resume|continue)[ the| my] timer in <area>",
+                        "(resume|continue)[ the| my] timer (named|called|for) {timer_name:name}",
+                        "(resume|continue)[ the| my] {timer_name:name} timer"
+                    ]
+                }
+            ]
+        },
         "HassVacuumReturnToBase": {
             "data": [
                 {
                     "requires_context": {
                         "domain": "vacuum"
                     },
                     "sentences": [
@@ -3557,14 +3780,35 @@
                 "fahrenheit",
                 {
                     "in": "f",
                     "out": "fahrenheit"
                 }
             ]
         },
+        "timer_hours": {
+            "range": {
+                "from": 1,
+                "to": 100
+            }
+        },
+        "timer_minutes": {
+            "range": {
+                "from": 1,
+                "to": 100
+            }
+        },
+        "timer_name": {
+            "wildcard": true
+        },
+        "timer_seconds": {
+            "range": {
+                "from": 1,
+                "to": 100
+            }
+        },
         "volume": {
             "range": {
                 "from": 0,
                 "to": 100,
                 "type": "percentage"
             }
         },
@@ -3573,15 +3817,18 @@
         }
     },
     "responses": {
         "errors": {
             "duplicate_entities": "Sorry, there are multiple devices called {{ entity }}",
             "duplicate_entities_in_area": "Sorry, there are multiple devices called {{ entity }} in the {{ area }} area",
             "duplicate_entities_in_floor": "Sorry, there are multiple devices called {{ entity }} in the {{ floor }} floor",
+            "entity_wrong_state": "Sorry, no device is {{ state | lower }}",
+            "feature_not_supported": "Sorry, no device supports the required features",
             "handle_error": "An unexpected error occurred",
+            "multiple_timers_matched": "Sorry, I am unable to target multiple timers",
             "no_area": "Sorry, I am not aware of any area called {{ area }}",
             "no_device_class": "Sorry, I am not aware of any {{ device_class }}",
             "no_device_class_exposed": "Sorry, no {{ device_class }} is exposed",
             "no_device_class_in_area": "Sorry, I am not aware of any {{ device_class }} in the {{ area }} area",
             "no_device_class_in_area_exposed": "Sorry, no {{ device_class }} in the {{ area }} area is exposed",
             "no_device_class_in_floor": "Sorry, I am not aware of any {{ device_class }} in the {{ floor }} floor",
             "no_device_class_in_floor_exposed": "Sorry, no {{ device_class }} in the {{ floor }} floor is exposed",
@@ -3594,58 +3841,78 @@
             "no_entity": "Sorry, I am not aware of any device called {{ entity }}",
             "no_entity_exposed": "Sorry, {{ entity }} is not exposed",
             "no_entity_in_area": "Sorry, I am not aware of any device called {{ entity }} in the {{ area }} area",
             "no_entity_in_area_exposed": "Sorry, {{ entity }} in the {{ area }} area is not exposed",
             "no_entity_in_floor": "Sorry, I am not aware of any device called {{ entity }} in the {{ floor }} floor",
             "no_entity_in_floor_exposed": "Sorry, {{ entity }} in the {{ floor }} floor is not exposed",
             "no_floor": "Sorry, I am not aware of any floor called {{ floor }}",
-            "no_intent": "Sorry, I couldn't understand that"
+            "no_intent": "Sorry, I couldn't understand that",
+            "no_timer_support": "Sorry, timers are not supported on this device",
+            "timer_not_found": "Sorry, I couldn't find that timer"
         },
         "intents": {
+            "HassCancelTimer": {
+                "default": "Timer cancelled"
+            },
             "HassClimateGetTemperature": {
                 "default": "{% set temperature = state_attr(state.entity_id, 'current_temperature') %} {% if temperature == 1: %} {{ temperature }} degree {% else: %} {{ temperature }} degrees {% endif %}\n"
             },
+            "HassDecreaseTimer": {
+                "default": "Timer updated"
+            },
             "HassGetState": {
                 "all": "{% if not query.unmatched: %}\n  Yes\n{% else %}\n  {% set no_match = query.unmatched | map(attribute=\"name\") | sort | list %}\n  {% if no_match | length > 4 %}\n    No, {{ no_match[:3] | join(\", \") }} and {{ (no_match | length - 3) }} more are not {{ slots.state }}\n  {%- else -%}\n    No,\n    {% for name in no_match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} and {% endif -%}\n      {{ name }}\n    {%- endfor %} {% if no_match | length > 1 %}are{% else %}is{% endif %} not {{ slots.state }}\n  {% endif %}\n{% endif %}\n",
                 "any": "{% if query.matched %}\n  {% set match = query.matched | map(attribute=\"name\") | sort | list %}\n  {% if match | length > 4 %}\n    Yes, {{ match[:3] | join(\", \") }} and {{ (match | length - 3) }} more\n  {%- else -%}\n    Yes,\n    {% for name in match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} and {% endif -%}\n      {{ name }}\n    {%- endfor -%}\n  {% endif %}\n{% else %}\n  No\n{% endif %}\n",
                 "default": "{{ state.state_with_unit }}",
                 "how_many": "{{ query.matched | length }}\n",
                 "one": "{{ slots.name | capitalize }} is {{ state.state_with_unit }}\n",
                 "one_yesno": "{% if query.matched %}\n  Yes\n{% else %}\n  No, {{ state.state_with_unit }}\n{% endif %}\n",
                 "where": "{% if state == \"not_home\" %}\n  {{ slots.name | capitalize }} is away\n{% else %}\n  {{ slots.name | capitalize }} is at {{ state.state }}\n{% endif %}\n",
                 "which": "{% if not query.matched %}\n  Not any\n{% else: %}\n  {% set match = query.matched | map(attribute=\"name\") | sort | list %}\n  {% if match | length > 4 %}\n    {{ match[:3] | join(\", \") }} and {{ (match | length - 3) }} more\n  {% else %}\n    {%- for name in match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} and {% endif -%}\n      {{ name }}\n    {%- endfor -%}\n  {% endif %}\n{% endif %}\n"
             },
             "HassGetWeather": {
                 "default": "{% set weather_condition = {\n  'clear': 'and clear',\n  'clear-night': 'and clear',\n  'cloudy': 'and cloudy',\n  'exceptional': 'and exceptional',\n  'fog': 'with fog',\n  'hail': 'with hail',\n  'lightning': 'with lightning',\n  'lightning-rainy': 'with lightning and rain',\n  'partlycloudy': 'and partly cloudy',\n  'pouring': 'and pouring rain',\n  'rainy': 'and raining',\n  'snowy': 'and snowing',\n  'snowy-rainy': 'with snow and rain',\n  'sunny': 'and sunny',\n  'windy': 'and windy',\n  'windy-variant': 'with wind and clouds'\n} %} {{ state.attributes.get('temperature') }} {{ state.attributes.get('temperature_unit') }} {{ weather_condition.get((state.state | string).lower(), \"\") }}\n"
             },
+            "HassIncreaseTimer": {
+                "default": "Timer updated"
+            },
             "HassLightSet": {
                 "brightness": "Brightness set",
                 "color": "Color set"
             },
             "HassListAddItem": {
                 "item_added": "Added {{ slots.item }}"
             },
             "HassMediaNext": {
                 "default": "Playing next"
             },
             "HassMediaPause": {
                 "default": "Paused"
             },
             "HassMediaUnpause": {
-                "default": "Unpaused"
+                "default": "Resumed"
+            },
+            "HassPauseTimer": {
+                "default": "Timer paused"
             },
             "HassSetPosition": {
                 "default": "Position set"
             },
             "HassSetVolume": {
                 "default": "Volume set"
             },
             "HassShoppingListAddItem": {
                 "item_added": "Added {{ slots.item }}"
             },
+            "HassStartTimer": {
+                "default": "Timer started"
+            },
+            "HassTimerStatus": {
+                "default": "{% set num_timers = slots.timers | length %}\n{% set active_timers = slots.timers | selectattr('is_active') | list %}\n{% set num_active_timers = active_timers | length %}\n{% set paused_timers = slots.timers | rejectattr('is_active') | list %}\n{% set num_paused_timers = paused_timers | length %}\n{% set next_timer = None %}\n\n{% if num_timers == 0: %}\n  No timers.\n{% elif num_active_timers == 0: %}\n  {# No active timers #}\n  {% if num_paused_timers == 1: %}\n    {% set next_timer = paused_timers[0] %}\n    Timer is paused.\n  {% else: %}\n    {{ num_paused_timers }} paused timers.\n  {% endif %}\n{% else: %}\n  {# At least one active timer #}\n  {% if num_active_timers == 1: %}\n    {% set next_timer = active_timers[0] %}\n  {% else: %}\n    {# Get active timer that will finish soonest #}\n    {% set sorted_timers = active_timers | sort(attribute='total_seconds_left') %}\n    {% set next_timer = sorted_timers[0] %}\n    {{ num_active_timers }} running timers.\n  {% endif %}\n\n  {% if num_paused_timers == 1: %}\n    1 paused timer.\n  {% elif num_paused_timers > 0: %}\n    {{ num_paused_timers }} paused timers.\n  {% endif %}\n{% endif %}\n\n{% if next_timer: %}\n  {# At least one active timer #}\n  {% if (next_timer.rounded_hours_left == 1) and (next_timer.rounded_minutes_left > 0): %}\n    1 hour and {{ next_timer.rounded_minutes_left }} minutes\n  {% elif (next_timer.rounded_hours_left == 1): %}\n    1 hour\n  {% elif (next_timer.rounded_hours_left > 1) and (next_timer.rounded_minutes_left > 0): %}\n    {{ next_timer.rounded_hours_left }} hours and {{ next_timer.rounded_minutes_left }} minutes\n  {% elif (next_timer.rounded_hours_left > 1): %}\n    {{ next_timer.rounded_hours_left }} hours\n  {% elif (next_timer.rounded_minutes_left == 1) and (next_timer.rounded_seconds_left > 0): %}\n    1 minute and {{ next_timer.rounded_seconds_left }} seconds\n  {% elif (next_timer.rounded_minutes_left == 1): %}\n    1 minute\n  {% elif (next_timer.rounded_minutes_left > 1) and (next_timer.rounded_seconds_left > 0): %}\n    {{ next_timer.rounded_minutes_left }} minutes and {{ next_timer.rounded_seconds_left }} seconds\n  {% elif (next_timer.rounded_minutes_left > 1): %}\n    {{ next_timer.rounded_minutes_left }} minutes\n  {% elif (next_timer.rounded_seconds_left == 1): %}\n    1 second\n  {% elif (next_timer.rounded_seconds_left > 1): %}\n    {{ next_timer.rounded_seconds_left }} seconds\n  {% endif %}\n\n  {% if num_timers > 1: %}\n    {# Give some extra information to disambiguate #}\n    left on\n    {% if (next_timer.start_hours > 0) and (next_timer.start_minutes > 0): %}\n      {{ next_timer.start_hours }} hour and {{ next_timer.start_minutes }} minute\n    {% elif (next_timer.start_hours > 0): %}\n      {{ next_timer.start_hours }} hour\n    {% elif (next_timer.start_minutes > 0) and (next_timer.start_seconds > 0): %}\n      {{ next_timer.start_minutes }} minute and {{ next_timer.start_seconds }} second\n    {% elif (next_timer.start_minutes > 0): %}\n      {{ next_timer.start_minutes }} minute\n    {% elif (next_timer.start_seconds > 0): %}\n      {{ next_timer.start_seconds }} second\n    {% endif %}\n\n    {% if next_timer.name: %}\n      {{ next_timer.name }}\n    {% elif next_timer.area: %}\n      {{ next_timer.area }}\n    {% endif %}\n\n    timer.\n  {% else: %}\n    left.\n  {% endif %}\n{% endif %}\n"
+            },
             "HassTurnOff": {
                 "cover": "Closed",
                 "cover_device_class": "Closed the {{ slots.device_class }}",
                 "default": "Turned off the {{ state.domain }}",
                 "fan_all": "Turned off all of the fans",
                 "fans_area": "Turned off the fans",
                 "light_all": "Turned off all of the lights",
@@ -3663,14 +3930,17 @@
                 "lights_area": "Turned on the lights",
                 "lights_floor": "Turned on the lights",
                 "lock": "Locked",
                 "scene": "Activated",
                 "script": "Started",
                 "valve": "Opened"
             },
+            "HassUnpauseTimer": {
+                "default": "Timer resumed"
+            },
             "HassVacuumReturnToBase": {
                 "default": "Returning"
             },
             "HassVacuumStart": {
                 "default": "Started"
             }
         }
```

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/data/es.json` & `home-assistant-intents-2024.5.28/home_assistant_intents/data/es.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9785051255513189%*

 * *Differences: {"'expansion_rules'": "{'de_aqui': '[ (de|en)] (aquí|acá|(el|la) <habitación>)', 'luces': "*

 * *                      "'[el|la|l(a|o)s] "*

 * *                      '(luz|luces|lámpara[s]|bombill(a|o)[s]|ampolleta[s]|luminaria[s]|lamparilla[s]|foco[s]|interruptor[es]|llave[s][ '*

 * *                      "de la luz])', 'planta': '[en|del|de] [el|la] ([planta|piso] {floor}|{floor} "*

 * *                      "(planta|piso))', 'habitación': "*

 * *                      "'(habitaci(ón|ones)|pieza[s]|cuarto[s]|aposento[s]|sala[s]|[r […]*

```diff
@@ -1,41 +1,48 @@
 {
     "expansion_rules": {
         "abre": "(abr(a|e|ir|\u00ed)|<sube>)",
         "ahora": "[ahora [mismo]|actual[mente]|en este momento]",
         "apaga": "(apag(a|ue|ar|\u00e1)|desconect(a|e|ar|\u00e1)|desactiv(a|e|ar|\u00e1))",
+        "aqu\u00ed": "[en |de ](aqu\u00ed|est(a|e) (habitaci\u00f3n|pieza|cuarto))",
         "area": "[en|del|de] [el|la] {area}",
         "a\u00f1adir": "(a\u00f1ad(a|e|ir|\u00ed)|apunt[a|e|ar|\u00e1]|pon[ga|er|\u00e9])",
         "baja": "(baj(a|e|ar|\u00e1)|redu(ce|zca|cir|c\u00ed)|decrement(a|e|ar|\u00e1))",
         "brightness": "{brightness} [%|porcien[to]|por cien[to]]",
         "cambia": "(cambi(a[r]|\u00e1|e|o)|(muev[a|e]|mov[er|\u00e9]))",
         "cancela": "cancel(a[r]|\u00e1|e|aci\u00f3n)",
+        "casa": "(casa|apartamento|departamento|piso)",
         "cierra": "(cierr(a|e)|cerr(ar|\u00e1)|<baja>)",
         "cual_es": "(Cu\u00e1l es [el|la]|Cu\u00e1les son [los|las])",
         "cual_es_la_medida_del_sensor": "(<cual_es>|Qu\u00e9|Cu\u00e1nt(a|o)[s]) [(la (cantidad|medida)|el nivel) de ][<class> (de|del|en|desde|por|<mide>)] [[el ](sensor |medidor )[de ]]<name> [<area>]",
-        "de_aqui": "[ (de|en)] (aqu\u00ed|ac\u00e1|la habitaci\u00f3n|la pieza)",
+        "de_aqui": "[ (de|en)] (aqu\u00ed|ac\u00e1|(el|la) <habitaci\u00f3n>)",
         "dime": "(sab(es|\u00e9)|dime|dec(ir|\u00ed|id)[me]|ind(i|\u00ed)(ca|que|car|c\u00e1)[me])",
         "dime_si": "<dime> si",
         "donde_se_encuentra": "d\u00f3nde <se_encuentra>",
         "ejecuta": "(<enciende>|ejecut(a|e|ar|\u00e1)|inici(a|e|ar|\u00e1))",
         "enciende": "(enc[i]end(a|e|er|\u00e9)|conect(a|e|ar|\u00e1)|activ(a|e|ar|\u00e1)|prend(a|e|er|\u00e9))",
         "establece": "(pon[ga|er|\u00e9]|estable[z]c(a|e|er|\u00e9)|ajust(a|e|ar|\u00e1)|configur(a|e|ar|\u00e1)|cambi(a[r]|\u00e1|e))",
         "establece_abre_cierra": "(<establece>|<abre>|<cierra>)",
         "establece_sube_baja": "(<establece>|<enciende>|<sube>|<baja>)",
+        "habitaci\u00f3n": "(habitaci(\u00f3n|ones)|pieza[s]|cuarto[s]|aposento[s]|sala[s]|[re]c\u00e1mara[s])",
+        "luces": "[el|la|l(a|o)s] (luz|luces|l\u00e1mpara[s]|bombill(a|o)[s]|ampolleta[s]|luminaria[s]|lamparilla[s]|foco[s]|interruptor[es]|llave[s][ de la luz])",
         "mide": "[que] ([es|est\u00e1] (mid(e|ie)|medi|indica|marca)[ndo|d(a|o)]|tiene|hay) [por|en]",
         "name": "[el|la|los|las] {name}",
         "pausa": "(paus(a|ar|e|\u00e1)|par(a|ar|e|\u00e1))|det(\u00e9n|ener|enga|en\u00e9)",
         "pista": "(pista|canci\u00f3n|medio|v\u00eddeo|video|elemento)",
+        "planta": "[en|del|de] [el|la] ([planta|piso] {floor}|{floor} (planta|piso))",
         "posici\u00f3n": "{position}[ ][%|por[ ]cien[to]]",
         "puerta": "[el|la] (puerta|port\u00f3n|cancela|verja|reja|compuerta|portillo)",
         "reproduce": "(reprodu(ce|cir|c\u00ed|zca)|escuchar|oir|ver|visualizar)",
         "se_encuentra": "(se (encuentra|localiza|ubica)|est\u00e1|mora)",
         "sube": "(sub(a|e|ir|\u00ed)|levant(a|e|ar|\u00e1)|aument(a|e|ar|\u00e1)|increment(a|e|ar|\u00e1))",
         "temp": "[el|la] (temperatura|calor|grados)",
         "temperature": "{temperature} [grados] [{temperature_unit}]",
+        "todas_partes": "[en |de[l] ](todas [las ]partes|todos los sitios|todos [los ]lados|<todos> <habitaci\u00f3n>|[<todos> <habitaci\u00f3n> [de[l]|en] ][el |la ]<casa>)",
+        "todos": "(tod(a|o)s [l(a|o)s]|cada [un(a|o) de l(a|o)s]|tod(a|o)s y cada un(a|o) de l(a|o)s)",
         "volumen": "{volume:volume_level}[ ][%|por[ ]cien[to]]"
     },
     "intents": {
         "HassClimateGetTemperature": {
             "data": [
                 {
                     "sentences": [
@@ -2664,41 +2671,52 @@
                     "sentences": [
                         "<apaga> [[el|la|los|las] (luz|luces|(interruptor[es]|llave[s] de [la luz]))] [de|del] <name>"
                     ]
                 },
                 {
                     "response": "lights_area",
                     "sentences": [
-                        "<apaga> [(la|las)] (luz | luces) <area>",
-                        "<apaga> todas las luces <area>",
+                        "<apaga> [<todos>] <luces> <area>",
                         "<apaga> <area>"
                     ],
                     "slots": {
                         "domain": "light"
                     }
                 },
                 {
                     "response": "light_all",
                     "sentences": [
-                        "<apaga> todas las luces"
+                        "<apaga> [<todos>] <luces> <todas_partes>",
+                        "<apaga> <todos> <luces>"
                     ],
                     "slots": {
                         "domain": "light",
                         "name": "all"
                     }
                 },
                 {
                     "requires_context": {
                         "area": {
                             "slot": true
                         }
                     },
                     "response": "lights_area",
                     "sentences": [
-                        "<apaga> ((la luz|las luces)[<de_aqui>]|todas las luces <de_aqui>)"
+                        "<apaga> [<todos>] <luces> <de_aqui>",
+                        "<apaga> <luces>"
+                    ],
+                    "slots": {
+                        "domain": "light"
+                    }
+                },
+                {
+                    "response": "lights_floor",
+                    "sentences": [
+                        "<apaga> [<todos>] <luces> <planta>",
+                        "<apaga> <planta>"
                     ],
                     "slots": {
                         "domain": "light"
                     }
                 },
                 {
                     "requires_context": {
@@ -2816,36 +2834,57 @@
             "data": [
                 {
                     "requires_context": {
                         "domain": "light"
                     },
                     "response": "light",
                     "sentences": [
-                        "<enciende> [[(el|la|los|las)] (luz|luces|(interruptor[es]|llave[s] de [la luz]))] [de|del] <name>"
+                        "<enciende> <luces> [de [l(a|o)[s]]|del] <name>"
                     ]
                 },
                 {
                     "response": "lights_area",
                     "sentences": [
-                        "<enciende> [toda[s]] ([la] luz | [las] luces) <area>",
+                        "<enciende> [<todos>] <luces> <area>",
                         "<enciende> <area>"
                     ],
                     "slots": {
                         "domain": "light"
                     }
                 },
                 {
+                    "response": "light_all",
+                    "sentences": [
+                        "<enciende> [<todos>] <luces> <todas_partes>",
+                        "<enciende> <todos> <luces>"
+                    ],
+                    "slots": {
+                        "domain": "light"
+                    }
+                },
+                {
                     "requires_context": {
                         "area": {
                             "slot": true
                         }
                     },
                     "response": "lights_area",
                     "sentences": [
-                        "<enciende> [todas] la[s] lu(z|ces)[<de_aqui>]"
+                        "<enciende> [<todos>] <luces> <de_aqui>",
+                        "<enciende> <luces>"
+                    ],
+                    "slots": {
+                        "domain": "light"
+                    }
+                },
+                {
+                    "response": "lights_floor",
+                    "sentences": [
+                        "<enciende> [<todos>] <luces> <planta>",
+                        "<enciende> <planta>"
                     ],
                     "slots": {
                         "domain": "light"
                     }
                 },
                 {
                     "response": "fans_area",
@@ -3569,22 +3608,28 @@
             "duplicate_entities_in_area": "Lo siento, hay varios dispositivos denominados {{ entity }} en el \u00e1rea {{ area }}",
             "handle_error": "Se ha producido un error inesperado al procesar la instrucci\u00f3n",
             "no_area": "Lo siento, no conozco ning\u00fan \u00e1rea llamada {{ area }}",
             "no_device_class": "{% set translations = {\n  \"awning\": \"ning\u00fan toldo\",\n  \"blind\": \"ninguna persiana\",\n  \"curtain\": \"ninguna cortina\",\n  \"door\": \"ninguna puerta\",\n  \"garage\": \"ninguna puerta de garaje\",\n  \"gate\": \"ninguna puerta\",\n  \"shade\": \"ning\u00fan estor\",\n  \"shutter\": \"ninguna contraventana\",\n  \"window\": \"ninguna ventana\"\n  } %}\n{% if device_class in translations -%}\n  Lo siento, no conozco {{ translations[device_class] }}\n{%- else -%}\n  Lo siento, no conozco ning\u00fan elemento de la clase {{ device_class }}\n{%- endif %}\n",
             "no_device_class_exposed": "Lo siento, no se expone al asistente ning\u00fan elemento de clase {{ device_class }}",
             "no_device_class_in_area": "{% set translations = {\n  \"awning\": \"ning\u00fan toldo\",\n  \"blind\": \"ninguna persiana\",\n  \"curtain\": \"ninguna cortina\",\n  \"door\": \"ninguna puerta\",\n  \"garage\": \"ninguna puerta de garaje\",\n  \"gate\": \"ninguna puerta\",\n  \"shade\": \"ning\u00fan estor\",\n  \"shutter\": \"ninguna contraventana\",\n  \"window\": \"ninguna ventana\"\n  } %}\n{% if device_class in translations -%}\n  Lo siento, no conozco {{ translations[device_class] }} en el \u00e1rea {{ area }}\n{%- else -%}\n  Lo siento, no conozco ning\u00fan elemento de la clase {{ device_class }} en el \u00e1rea {{ area }}\n{%- endif %}\n",
             "no_device_class_in_area_exposed": "Lo siento, no se expone al asistente ning\u00fan elemento de clase {{ device_class }} en el \u00e1rea {{ area }}",
+            "no_device_class_in_floor": "{% set translations = {\n  \"awning\": \"ning\u00fan toldo\",\n  \"blind\": \"ninguna persiana\",\n  \"curtain\": \"ninguna cortina\",\n  \"door\": \"ninguna puerta\",\n  \"garage\": \"ninguna puerta de garaje\",\n  \"gate\": \"ninguna puerta\",\n  \"shade\": \"ning\u00fan estor\",\n  \"shutter\": \"ninguna contraventana\",\n  \"window\": \"ninguna ventana\"\n  } %}\n{% if device_class in translations -%}\n  Lo siento, no conozco {{ translations[device_class] }} en la planta {{ floor }}\n{%- else -%}\n  Lo siento, no conozco ning\u00fan elemento de la clase {{ device_class }} en la planta {{ floor }}\n{%- endif %}\n",
+            "no_device_class_in_floor_exposed": "Lo siento, no se expone al asistente ning\u00fan elemento de clase {{ device_class }} en la planta {{ floor }}",
             "no_domain": "{% set translations = {\n  \"button\": \"ning\u00fan bot\u00f3n\",\n  \"camera\": \"ninguna c\u00e1mara\",\n  \"input_button\": \"ning\u00fan bot\u00f3n de entrada\",\n  \"alarm_control_panel\": \"ninguna alarma\",\n  \"automation\": \"ninguna automatizaci\u00f3n\",\n  \"fan\": \"ning\u00fan ventilador\",\n  \"climate\": \"ning\u00fan termostato\",\n  \"humidifier\": \"ning\u00fan humidificador\",\n  \"input_boolean\": \"ning\u00fan interruptor\",\n  \"siren\": \"ninguna sirena\",\n  \"water_heater\": \"ning\u00fan calentador de agua\",\n  \"light\": \"ninguna luz\",\n  \"switch\": \"ning\u00fan interruptor\",\n  \"script\": \"ning\u00fan script\",\n  \"remote\": \"ning\u00fan control remoto\",\n  \"lock\": \"ninguna cerradura\",\n  \"vacuum\": \"ning\u00fan aspirador\",\n  \"scene\": \"ninguna escena\",\n  \"media_player\": \"ning\u00fan reproductor multimedia\",\n  \"lawn_mower\": \"ning\u00fan cortac\u00e9sped\",\n  \"valve\": \"ninguna v\u00e1lvula\"\n  } %}\n{% if domain in translations -%}\n  Lo siento, no conozco {{ translations[domain] }}\n{%- else -%}\n  Lo siento, no conozco ning\u00fan elemento del tipo indicado\n{%- endif %}\n",
             "no_domain_exposed": "Lo siento, no se expone al asistente ning\u00fan elemento de tipo {{ domain }}",
             "no_domain_in_area": "{% set translations = {\n  \"button\": \"ning\u00fan bot\u00f3n\",\n  \"camera\": \"ninguna c\u00e1mara\",\n  \"input_button\": \"ning\u00fan bot\u00f3n de entrada\",\n  \"alarm_control_panel\": \"ninguna alarma\",\n  \"automation\": \"ninguna automatizaci\u00f3n\",\n  \"fan\": \"ning\u00fan ventilador\",\n  \"climate\": \"ning\u00fan termostato\",\n  \"humidifier\": \"ning\u00fan humidificador\",\n  \"input_boolean\": \"ning\u00fan interruptor\",\n  \"siren\": \"ninguna sirena\",\n  \"water_heater\": \"ning\u00fan calentador de agua\",\n  \"light\": \"ninguna luz\",\n  \"switch\": \"ning\u00fan interruptor\",\n  \"script\": \"ning\u00fan script\",\n  \"remote\": \"ning\u00fan control remoto\",\n  \"lock\": \"ninguna cerradura\",\n  \"vacuum\": \"ning\u00fan aspirador\",\n  \"scene\": \"ninguna escena\",\n  \"media_player\": \"ning\u00fan reproductor multimedia\",\n  \"lawn_mower\": \"ning\u00fan cortac\u00e9sped\",\n  \"valve\": \"ninguna v\u00e1lvula\"\n  } %}\n{% if domain in translations -%}\n  Lo siento, no conozco {{ translations[domain] }} en el \u00e1rea {{ area }}\n{%- else -%}\n  Lo siento, no conozco ning\u00fan elemento del tipo {{ domain }} en el \u00e1rea {{ area }}\n{%- endif %}\n",
             "no_domain_in_area_exposed": "Lo siento, no se expone al asistente ning\u00fan elemento de tipo {{ domain }} en el \u00e1rea {{ area }}",
+            "no_domain_in_floor": "{% set translations = {\n  \"button\": \"ning\u00fan bot\u00f3n\",\n  \"camera\": \"ninguna c\u00e1mara\",\n  \"input_button\": \"ning\u00fan bot\u00f3n de entrada\",\n  \"alarm_control_panel\": \"ninguna alarma\",\n  \"automation\": \"ninguna automatizaci\u00f3n\",\n  \"fan\": \"ning\u00fan ventilador\",\n  \"climate\": \"ning\u00fan termostato\",\n  \"humidifier\": \"ning\u00fan humidificador\",\n  \"input_boolean\": \"ning\u00fan interruptor\",\n  \"siren\": \"ninguna sirena\",\n  \"water_heater\": \"ning\u00fan calentador de agua\",\n  \"light\": \"ninguna luz\",\n  \"switch\": \"ning\u00fan interruptor\",\n  \"script\": \"ning\u00fan script\",\n  \"remote\": \"ning\u00fan control remoto\",\n  \"lock\": \"ninguna cerradura\",\n  \"vacuum\": \"ning\u00fan aspirador\",\n  \"scene\": \"ninguna escena\",\n  \"media_player\": \"ning\u00fan reproductor multimedia\",\n  \"lawn_mower\": \"ning\u00fan cortac\u00e9sped\",\n  \"valve\": \"ninguna v\u00e1lvula\"\n  } %}\n{% if domain in translations -%}\n  Lo siento, no conozco {{ translations[domain] }} en la planta {{ floor }}\n{%- else -%}\n  Lo siento, no conozco ning\u00fan elemento del tipo {{ domain }} en la planta {{ floor }}\n{%- endif %}\n",
+            "no_domain_in_floor_exposed": "Lo siento, no se expone al asistente ning\u00fan elemento de tipo {{ domain }} en la planta {{ floor }}",
             "no_entity": "Lo siento, no conozco ning\u00fan dispositivo llamado {{ entity }}",
             "no_entity_exposed": "Lo siento, el dispositivo {{ entity }} no se expone al asistente",
             "no_entity_in_area": "Lo siento, no conozco ning\u00fan dispositivo llamado {{ entity }} en el \u00e1rea {{ area }}",
             "no_entity_in_area_exposed": "Lo siento, el dispositivo {{ entity }} en el \u00e1rea {{ area }} no se expone al asistente",
+            "no_entity_in_floor_exposed": "Lo siento, el dispositivo {{ entity }} en la planta {{ floor }} no se expone al asistente",
+            "no_floor": "Lo siento, no conozco ninguna planta llamada {{ floor }}",
             "no_intent": "Lo siento, no he entendido"
         },
         "intents": {
             "HassClimateGetTemperature": {
                 "default": "{% set temperature = state_attr(state.entity_id, 'current_temperature') %} {{ temperature | float | abs | round(1) | replace('.0', '') | replace('.',',') }} {{ 'grado' if temperature | float | abs == 1 else 'grados' }} {{ 'bajo cero' if temperature | float < 0 else '' }}\n"
             },
             "HassGetState": {
@@ -3632,27 +3677,30 @@
                 "cover": "{{ slots.name }} se ha cerrado",
                 "cover_device_class": "Cierre completado",
                 "default": "{{ slots.name }} se ha desconectado",
                 "fans_area": "Ventiladores apagados",
                 "light": "{{ slots.name }} se ha apagado",
                 "light_all": "Todas las luces apagadas",
                 "lights_area": "Luces apagadas",
+                "lights_floor": "Luces apagadas",
                 "lock": "{{ slots.name }} se ha abierto",
                 "lock_area": "Apertura completada",
                 "valve": "{{ slots.name }} se ha cerrado"
             },
             "HassTurnOn": {
                 "cover": "{{ slots.name }} se ha abierto",
                 "cover_area": "Apertura completada",
                 "cover_device_class": "Apertura completada",
                 "default": "{{ slots.name }} se ha activado",
                 "fan": "{{ slots.name }} se ha encendido",
                 "fans_area": "Ventiladores encendidos",
                 "light": "{{ slots.name }} se ha encendido",
+                "light_all": "Se han encendido todas las luces",
                 "lights_area": "Luces encendidas",
+                "lights_floor": "Luces encendidas",
                 "lock": "{{ slots.name }} se ha cerrado",
                 "lock_area": "Cierre efectuado",
                 "scene": "Escena {{ slots.name }} activada",
                 "script": "Script iniciado",
                 "valve": "{{ slots.name }} se ha abierto"
             },
             "HassVacuumReturnToBase": {
```

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/data/et.json` & `home-assistant-intents-2024.5.28/home_assistant_intents/data/et.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/data/eu.json` & `home-assistant-intents-2024.5.28/home_assistant_intents/data/eu.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/data/fa.json` & `home-assistant-intents-2024.5.28/home_assistant_intents/data/fa.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/data/fi.json` & `home-assistant-intents-2024.5.28/home_assistant_intents/data/fi.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9993100979691788%*

 * *Differences: {"'expansion_rules'": "{'käynnistä': '(käynnistä|starttaa|aja)'}",*

 * * "'intents'": "{'HassTurnOn': {'data': {9: {'excludes_context': {'domain': {insert: [(6, "*

 * *              "'script')], delete: [4]}}}, insert: [(5, OrderedDict([('sentences', ['<käynnistä> "*

 * *              "<nimi>', '<laita> <nimi> <päälle>', '<laita> <päälle> <nimi>']), "*

 * *              "('requires_context', OrderedDict([('domain', 'script')])), ('slots', "*

 * *              "OrderedDict([('domain', 'script')])), ('response', 'script')]))]}}}",*

 * * " […]*

```diff
@@ -40,15 +40,15 @@
         "kylm\u00e4ksi": "(kylm\u00e4ksi|viile\u00e4ksi|vilpoiseksi)",
         "kylm\u00e4n": "(kylm\u00e4n|viile\u00e4n|vilpoisen)",
         "kylm\u00e4n\u00e4": "(kylm\u00e4n\u00e4|viile\u00e4n\u00e4|vilpoisena)",
         "kylm\u00e4\u00e4": "(kylm\u00e4\u00e4|viile\u00e4\u00e4|vilpoista)",
         "kytke": "(kytke|laita|aseta)",
         "kytkimet": "(kytkimet|vivut)",
         "kytkin": "(kytkin|vipu)",
-        "k\u00e4ynnist\u00e4": "(k\u00e4ynnist\u00e4|starttaa)",
+        "k\u00e4ynnist\u00e4": "(k\u00e4ynnist\u00e4|starttaa|aja)",
         "laita": "(kytke|aseta|k\u00e4\u00e4nn\u00e4|s\u00e4\u00e4d\u00e4|pist\u00e4|muuta|laita|siirr\u00e4)",
         "laite": "[\u00e4ly]laite",
         "laitteelle": "[\u00e4ly]laitteelle",
         "laitteelta": "[\u00e4ly]laitteelta",
         "laitteen": "[\u00e4ly]laitteen",
         "laitteeseen": "[\u00e4ly]laitteeseen",
         "laitteessa": "[\u00e4ly]laitteessa",
@@ -908,14 +908,28 @@
                     "slots": {
                         "domain": "fan",
                         "name": "all"
                     }
                 },
                 {
                     "requires_context": {
+                        "domain": "script"
+                    },
+                    "response": "script",
+                    "sentences": [
+                        "<k\u00e4ynnist\u00e4> <nimi>",
+                        "<laita> <nimi> <p\u00e4\u00e4lle>",
+                        "<laita> <p\u00e4\u00e4lle> <nimi>"
+                    ],
+                    "slots": {
+                        "domain": "script"
+                    }
+                },
+                {
+                    "requires_context": {
                         "domain": "valve"
                     },
                     "response": "valve",
                     "sentences": [
                         "<avaa> <nimi>"
                     ],
                     "slots": {
@@ -946,17 +960,17 @@
                 {
                     "excludes_context": {
                         "domain": [
                             "binary_sensor",
                             "cover",
                             "lock",
                             "scene",
-                            "script",
                             "sensor",
-                            "valve"
+                            "valve",
+                            "script"
                         ]
                     },
                     "sentences": [
                         "<laita> <p\u00e4\u00e4lle> {name} [(<alueessa>|<alueesta>|<alueelta>|<alueella>) {area}]",
                         "<laita> <p\u00e4\u00e4lle> (<alueessa>|<alueesta>|<alueen>|<alueelta>|<alueella>) {area} {name}",
                         "[<laita>] {name} <p\u00e4\u00e4lle> [(<alueessa>|<alueesta>|<alueelta>|<alueella>) {area}]",
                         "[<laita>] {name} (<alueessa>|<alueesta>|<alueelta>|<alueella>) {area} <p\u00e4\u00e4lle>",
@@ -1307,14 +1321,15 @@
                 "default": "Kytkettiin p\u00e4\u00e4lle {{ slots.name }}",
                 "fans_area_plural": "Tuulettimet ovat nyt p\u00e4\u00e4ll\u00e4",
                 "fans_area_singular": "Tuuletin on nyt p\u00e4\u00e4ll\u00e4",
                 "lights_area_plural": "Laitettiin valot p\u00e4\u00e4lle",
                 "lights_area_singular": "Laitettiin valo p\u00e4\u00e4lle",
                 "lights_area_uncountable": "Valaistiin",
                 "lock": "Lukittu",
+                "script": "K\u00e4ynnistettiin {{ slots.name }}",
                 "valve": "Avattiin"
             },
             "HassVacuumReturnToBase": {
                 "default": "Palaamassa"
             },
             "HassVacuumStart": {
                 "default": "K\u00e4ynnistettiin"
```

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/data/fr-CA.json` & `home-assistant-intents-2024.5.28/home_assistant_intents/data/fr-CA.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/data/fr.json` & `home-assistant-intents-2024.5.28/home_assistant_intents/data/fr.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9833208033647486%*

 * *Differences: {"'expansion_rules'": "{'lis': '(lis|lire)', 'mets': '(mets|mettre|passe|passer|mets_dirty)', "*

 * *                      "'regle': "*

 * *                      "'(règle|régler|met|mets|mettre|ajuste|ajuster|change|changer|mets_dirty)', "*

 * *                      "'reprends': "*

 * *                      "'(remets|remettre|reprends|reprend|reprendre|reprise|relance|relancer)', "*

 * *                      "'media': "*

 * *                      "'(morceau|chanson|musique|son|élément|podcast|film|vidéo|épisode|radio|média)', "*

 * *         […]*

```diff
@@ -8,38 +8,42 @@
         "capteur": "(capteur|sonde|d\u00e9tecteur)[s]",
         "dans": "(dans|du|de|des|\u00e0|au|aux|sur)",
         "de": "(du|de|des)",
         "degres": "(\u00b0| \u00b0| degr\u00e9| degr\u00e9s)",
         "demarre": "(d\u00e9marre|d\u00e9marrer|lance|lancer)",
         "diminue": "(diminue|diminuer|baisse|baisser)",
         "eclaire": "(\u00e9claire|\u00e9clairer|illumine|illuminer)",
+        "en_route": "(en route)|(en marche)",
         "estil": "(est|sont)[-][ ][(il[s]|elle[s])]",
         "eteins": "(\u00e9teint|eteint|\u00e9teins|eteins|\u00e9teindre|eteindre|d\u00e9sactive|d\u00e9sactiver|stoppe|stopper|arr\u00eate|arr\u00eater|coupe|couper|<eteins_dirty>)",
         "eteins_dirty": "(\u00e9tant|\u00e9tends|\u00e9tend|\u00e9tendre|\u00e9tat|et tant|et teins|et teint|et teints|et t'as|\u00e9t\u00e9|\u00e9tais|\u00e9tait)",
         "fenetre": "(fenetre[s]|fen\u00eatre[s]|baie[s]|velux|v\u00e9lux|lucarne[s])",
         "ferme": "(ferme|fermer|baisse|baisser)",
         "ici": "(<dans> (cette|la) pi\u00e8ce)|(ici)",
         "le": "(le |la |les |l')",
-        "lis": "(lis|lire|lecture)",
+        "lecture": "(lecture|visionnage)",
+        "lis": "(lis|lire)",
         "lumiere": "(lumi\u00e8re|lampe|ampoule)",
         "lumieres": "(lumi\u00e8res|lampes|ampoules)",
         "maison": "maison|domicile|appartement|appart|logement",
-        "media": "(morceau|chanson|\u00e9l\u00e9ment|podcast|film|vid\u00e9o|\u00e9pisode|m\u00e9dia)",
-        "mets": "(mets|mettre|passe|passer)",
+        "media": "(morceau|chanson|musique|son|\u00e9l\u00e9ment|podcast|film|vid\u00e9o|\u00e9pisode|radio|m\u00e9dia)",
+        "mets": "(mets|mettre|passe|passer|mets_dirty)",
+        "mets_dirty": "(mais|ma\u00eetre)",
         "ouvre": "(ouvre|ouvrir|monte|monter)",
         "partout": "([de] partout)|(<dans> [<tous>] [<le>]<maison>)|(<dans> toutes les pi\u00e8ces)",
         "pourcent": "(%| %| pourcent| pour cent)",
         "quel": "quel[le][s]",
         "quelest": "<quel> (est|sont)",
-        "regle": "(r\u00e8gle|r\u00e9gler|met|mets|mettre|ajuste|ajuster|change|changer)",
+        "regle": "(r\u00e8gle|r\u00e9gler|met|mets|mettre|ajuste|ajuster|change|changer|mets_dirty)",
         "renvoie": "(renvoie|renvoyer|arr\u00eate|arr\u00eater|stop[pe]|stopper)",
-        "reprends": "(reprends|reprendre|reprise)",
+        "reprends": "(remets|remettre|reprends|reprend|reprendre|reprise|relance|relancer)",
         "tous": "(tout|tous|toute[s])",
         "ventilateur": "[le ](ventilateur|brasseur d'air)",
         "ventilateurs": "[les ](ventilateurs|brasseurs d'air)",
+        "volume": "(volume|son|watt[s])",
         "what_is_the_class_of_name": "<quelest> (le |la |l'|les )<class> [(indiqu\u00e9[e][s]|mesur\u00e9[e][s]|renvoy\u00e9[e][s]|restant[e][s]|retourn\u00e9[e][s]|utilis\u00e9[e][s]|produit[e][s]|consomm\u00e9[e][s]|donn\u00e9[e][s]) ][(par|<dans>|sur)] [<le>]{name} [<dans> [<le>]{area}]",
         "yatil": "(y a[-][ ]t[-][']il|il y a)"
     },
     "intents": {
         "HassClimateGetTemperature": {
             "data": [
                 {
@@ -2662,42 +2666,123 @@
             "data": [
                 {
                     "requires_context": {
                         "domain": "media_player"
                     },
                     "sentences": [
                         "<media> suivant[e] sur [<le>]{name}",
-                        "<mets> (<le>|au|\u00e0 la) <media> suivant[e] [sur] [<le>]{name}"
+                        "<mets> (<le>|au |\u00e0 la )<media> suivant[e] [sur] [<le>]{name}"
+                    ]
+                },
+                {
+                    "requires_context": {
+                        "area": {
+                            "slot": true
+                        }
+                    },
+                    "sentences": [
+                        "suivant[e]",
+                        "<media> suivant[e]",
+                        "<mets> (<le>|au |\u00e0 la )<media> suivant[e]"
+                    ]
+                },
+                {
+                    "sentences": [
+                        "suivant[e] <dans> [<le>]{area}",
+                        "<media> suivant[e] <dans> [<le>]{area}",
+                        "<mets> (<le>|au |\u00e0 la )<media> suivant[e] <dans> [<le>]{area}"
                     ]
                 }
             ]
         },
         "HassMediaPause": {
             "data": [
                 {
                     "requires_context": {
                         "domain": "media_player"
                     },
                     "sentences": [
                         "<mets> [<le>]{name} (sur|en) pause",
                         "<mets> (sur|en) pause [<le>]{name} ",
-                        "Pause sur [<le>]{name}"
+                        "<mets> [<le>]<media> (sur|en) pause sur [<le>]{name} ",
+                        "Pause sur [<le>]{name}",
+                        "[<le>]{name} en pause",
+                        "<eteins>  [<le>]<media> sur [<le>]{name}",
+                        "<eteins> <le> <lecture> <de> [<le>]<media> sur [<le>]{name}",
+                        "<eteins> <le> <lecture> sur [<le>]{name}"
+                    ]
+                },
+                {
+                    "requires_context": {
+                        "area": {
+                            "slot": true
+                        }
+                    },
+                    "sentences": [
+                        "<eteins> [<le>]<media>",
+                        "<eteins> <le> <lecture> <de> [<le>]<media>",
+                        "<eteins> <le> <lecture>",
+                        "pause",
+                        "<mets> [<le>]<media> (sur|en) pause"
+                    ]
+                },
+                {
+                    "sentences": [
+                        "<eteins> [<le>]<media> <dans> [<le>]{area}",
+                        "<eteins> <le> <lecture> <de> [<le>]<media> <dans> [<le>]{area}",
+                        "<eteins> <le> <lecture> <dans> [<le>]{area}",
+                        "pause <dans> [<le>]{area}",
+                        "<mets> [<le>]<media> (sur|en) pause <dans> [<le>]{area}"
                     ]
                 }
             ]
         },
         "HassMediaUnpause": {
             "data": [
                 {
                     "requires_context": {
                         "domain": "media_player"
                     },
                     "sentences": [
                         "<lis> sur [<le>]{name}",
-                        "<reprends> [la lecture] sur [<le>]{name}"
+                        "<lecture> sur [<le>]{name}",
+                        "<reprends> [<le>]<media> sur [<le>]{name}",
+                        "<reprends> [<le>]<media> <en_route> sur [<le>]{name}",
+                        "<reprends> <le> <lecture> <de> [<le>]<media> sur [<le>]{name}",
+                        "<reprends> <le> <lecture> <de> [<le>]<media> <en_route> sur [<le>]{name}",
+                        "<reprends> <le> <lecture> sur [<le>]{name}",
+                        "<reprends> <le> <lecture> <en_route> sur [<le>]{name}",
+                        "<reprends> [<le>]{name} <en_route>"
+                    ]
+                },
+                {
+                    "requires_context": {
+                        "area": {
+                            "slot": true
+                        }
+                    },
+                    "sentences": [
+                        "<lecture>",
+                        "<reprends> [<le>]<media>",
+                        "<reprends> [<le>]<media> <en_route>",
+                        "<reprends> <le> <lecture> <de> [<le>]<media>",
+                        "<reprends> <le> <lecture> <de> [<le>]<media> <en_route>",
+                        "<reprends> <le> <lecture>",
+                        "<reprends> <le> <lecture> <en_route>"
+                    ]
+                },
+                {
+                    "sentences": [
+                        "<lecture> <dans> [<le>]{area}",
+                        "<reprends> [<le>]<media> <dans> [<le>]{area}",
+                        "<reprends> [<le>]<media> <en_route> <dans> [<le>]{area}",
+                        "<reprends> <le> <lecture> <de> [<le>]<media> <dans> [<le>]{area}",
+                        "<reprends> <le> <lecture> <de> [<le>]<media> <en_route> <dans> [<le>]{area}",
+                        "<reprends> <le> <lecture> <dans> [<le>]{area}",
+                        "<reprends> <le> <lecture> <en_route> <dans> [<le>]{area}"
                     ]
                 }
             ]
         },
         "HassNevermind": {
             "data": [
                 {
@@ -2783,15 +2868,30 @@
             "data": [
                 {
                     "requires_context": {
                         "domain": "media_player"
                     },
                     "sentences": [
                         "<regle> [<le>]{name} [\u00e0|sur] {volume:volume_level}<pourcent>",
-                        "<regle> le volume [<de>] [<le>]{name} [\u00e0|sur] {volume:volume_level}<pourcent>"
+                        "<regle> [<le>]<volume> [<de>] [<le>]{name} [\u00e0|sur] {volume:volume_level}<pourcent>"
+                    ]
+                },
+                {
+                    "requires_context": {
+                        "area": {
+                            "slot": true
+                        }
+                    },
+                    "sentences": [
+                        "<regle> [<le>]<volume> [\u00e0|sur] {volume:volume_level}<pourcent>"
+                    ]
+                },
+                {
+                    "sentences": [
+                        "<regle> [<le>]<volume> [\u00e0|sur] {volume:volume_level}<pourcent> <dans> [<le>]{area}"
                     ]
                 }
             ]
         },
         "HassShoppingListAddItem": {
             "data": [
                 {
```

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/data/gl.json` & `home-assistant-intents-2024.5.28/home_assistant_intents/data/gl.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/data/gu.json` & `home-assistant-intents-2024.5.28/home_assistant_intents/data/gu.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/data/he.json` & `home-assistant-intents-2024.5.28/home_assistant_intents/data/he.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9469907407407407%*

 * *Differences: {"'expansion_rules'": "{'open': '(פתח[י] | לפתוח | תפתח[י] | תעל[ה|י] | העל[ה|י] | הרם | הרימי | "*

 * *                      "להרים | תרים | תרימי)', 'close': '(סגור | סגרי | סיגרי | לסגור | תסגור | "*

 * *                      'תסגרי | הנמך | הנמיכי | תנמיך | תנמיכי | הורד | הורידי | להוריד | '*

 * *                      "תוריד[י])'}",*

 * * "'intents'": "{'HassTurnOff': {'data': {0: {'sentences': {insert: [(0, 'כב[ה|י] [את] [ה]<name>'), "*

 * *              "(3, 'תכב[ה|י] [את] [ה]<name>')], delete: [3, 0]}}, 1: {'sentences': "*

 * *  […]*

```diff
@@ -1,14 +1,14 @@
 {
     "expansion_rules": {
         "area": "[\u05d4][\u05d1]{area}",
         "brightness": "{brightness}[%| \u05d0\u05d7\u05d5\u05d6 | \u05d0\u05d7\u05d5\u05d6\u05d9\u05dd]",
-        "close": "(\u05e1\u05d2\u05d5\u05e8 | \u05dc\u05e1\u05d2\u05d5\u05e8 | \u05ea\u05e1\u05d2\u05d5\u05e8 | \u05d4\u05e0\u05de\u05da | \u05ea\u05e0\u05de\u05d9\u05da | \u05d4\u05d5\u05e8\u05d3 | \u05dc\u05d4\u05d5\u05e8\u05d9\u05d3 | \u05ea\u05d5\u05e8\u05d9\u05d3)",
+        "close": "(\u05e1\u05d2\u05d5\u05e8 | \u05e1\u05d2\u05e8\u05d9 | \u05e1\u05d9\u05d2\u05e8\u05d9 | \u05dc\u05e1\u05d2\u05d5\u05e8 | \u05ea\u05e1\u05d2\u05d5\u05e8 | \u05ea\u05e1\u05d2\u05e8\u05d9 | \u05d4\u05e0\u05de\u05da | \u05d4\u05e0\u05de\u05d9\u05db\u05d9 | \u05ea\u05e0\u05de\u05d9\u05da | \u05ea\u05e0\u05de\u05d9\u05db\u05d9 | \u05d4\u05d5\u05e8\u05d3 | \u05d4\u05d5\u05e8\u05d9\u05d3\u05d9 | \u05dc\u05d4\u05d5\u05e8\u05d9\u05d3 | \u05ea\u05d5\u05e8\u05d9\u05d3[\u05d9])",
         "name": "[\u05d4]{name}",
-        "open": "(\u05e4\u05ea\u05d7 | \u05dc\u05e4\u05ea\u05d5\u05d7 | \u05ea\u05e4\u05ea\u05d7 | \u05ea\u05e2\u05dc\u05d4 | \u05d4\u05e2\u05dc\u05d4 | \u05d4\u05e8\u05dd | \u05dc\u05d4\u05e8\u05d9\u05dd | \u05ea\u05e8\u05d9\u05dd)",
+        "open": "(\u05e4\u05ea\u05d7[\u05d9] | \u05dc\u05e4\u05ea\u05d5\u05d7 | \u05ea\u05e4\u05ea\u05d7[\u05d9] | \u05ea\u05e2\u05dc[\u05d4|\u05d9] | \u05d4\u05e2\u05dc[\u05d4|\u05d9] | \u05d4\u05e8\u05dd | \u05d4\u05e8\u05d9\u05de\u05d9 | \u05dc\u05d4\u05e8\u05d9\u05dd | \u05ea\u05e8\u05d9\u05dd | \u05ea\u05e8\u05d9\u05de\u05d9)",
         "set": "(\u05db\u05d5\u05d5\u05df|\u05e9\u05e0\u05d4|\u05e7\u05d1\u05e2)",
         "temp": "(\u05de\u05e2\u05dc\u05d5\u05ea|\u05d8\u05de\u05e4\u05e8\u05d8\u05d5\u05e8\u05d4|\u05d8\u05de\u05e4\u05e8\u05d8\u05d5\u05e8\u05ea)",
         "temperature": "{temperature} [{temperature_unit}] [\u00b0| \u05de\u05e2\u05dc\u05d5\u05ea]",
         "what_is": "(\u05de\u05d4|\u05de\u05d4\u05d5|\u05de\u05d4\u05d9|\u05de\u05d4\u05dd|\u05de\u05d4\u05df)",
         "window": "(\u05d7\u05dc\u05d5\u05df | \u05d7\u05dc\u05d5\u05e0\u05d5\u05ea | \u05ea\u05e8\u05d9\u05e1 | \u05ea\u05e8\u05d9\u05e1\u05d9\u05dd | \u05d5\u05d9\u05dc\u05d5\u05df | \u05d5\u05d9\u05dc\u05d5\u05e0\u05d5\u05ea | \u05e1\u05d5\u05db\u05da | \u05e1\u05d5\u05db\u05d7\u05d9\u05dd)"
     },
     "intents": {
@@ -114,154 +114,154 @@
             ]
         },
         "HassLightSet": {
             "data": [
                 {
                     "response": "brightness",
                     "sentences": [
-                        "\u05e7\u05d1\u05e2 [\u05d0\u05ea] [\u05d4]\u05d1\u05d4\u05d9\u05e8\u05d5\u05ea \u05d4<name> \u05dc<brightness>",
-                        "\u05e9\u05e0\u05d4 [\u05d0\u05ea] [\u05d4]\u05d1\u05d4\u05d9\u05e8\u05d5\u05ea \u05d4<name> \u05dc<brightness>",
-                        "\u05d4\u05d2\u05d3\u05e8 [\u05d0\u05ea] [\u05d4]\u05d1\u05d4\u05d9\u05e8\u05d5\u05ea \u05d4<name> \u05dc<brightness>"
+                        "\u05e7\u05d1\u05e2[\u05d9] [\u05d0\u05ea] [\u05d4]\u05d1\u05d4\u05d9\u05e8\u05d5\u05ea \u05d4<name> \u05dc<brightness>",
+                        "\u05e9\u05e0[\u05d4|\u05d9] [\u05d0\u05ea] [\u05d4]\u05d1\u05d4\u05d9\u05e8\u05d5\u05ea \u05d4<name> \u05dc<brightness>",
+                        "(\u05d4\u05d2\u05d3\u05e8|\u05d4\u05d2\u05d3\u05d9\u05e8\u05d9) [\u05d0\u05ea] [\u05d4]\u05d1\u05d4\u05d9\u05e8\u05d5\u05ea \u05d4<name> \u05dc<brightness>"
                     ]
                 },
                 {
                     "response": "brightness_area",
                     "sentences": [
-                        "\u05e7\u05d1\u05e2 [\u05d0\u05ea] [\u05d4]\u05d1\u05d4\u05d9\u05e8\u05d5\u05ea \u05d4<name> \u05dc<brightness> \u05d1<area>",
-                        "\u05e9\u05e0\u05d4 [\u05d0\u05ea] [\u05d4]\u05d1\u05d4\u05d9\u05e8\u05d5\u05ea \u05d4<name> \u05dc<brightness> \u05d1<area>",
-                        "\u05d4\u05d2\u05d3\u05e8 [\u05d0\u05ea] [\u05d4]\u05d1\u05d4\u05d9\u05e8\u05d5\u05ea \u05d4<name> \u05dc<brightness> \u05d1<area>"
+                        "\u05e7\u05d1\u05e2[\u05d9] [\u05d0\u05ea] [\u05d4]\u05d1\u05d4\u05d9\u05e8\u05d5\u05ea \u05d4<name> \u05dc<brightness> \u05d1<area>",
+                        "\u05e9\u05e0[\u05d4|\u05d9] [\u05d0\u05ea] [\u05d4]\u05d1\u05d4\u05d9\u05e8\u05d5\u05ea \u05d4<name> \u05dc<brightness> \u05d1<area>",
+                        "(\u05d4\u05d2\u05d3\u05e8|\u05d4\u05d2\u05d3\u05d9\u05e8\u05d9) [\u05d0\u05ea] [\u05d4]\u05d1\u05d4\u05d9\u05e8\u05d5\u05ea \u05d4<name> \u05dc<brightness> \u05d1<area>"
                     ]
                 }
             ]
         },
         "HassTurnOff": {
             "data": [
                 {
                     "sentences": [
-                        "\u05db\u05d1\u05d4 [\u05d0\u05ea] [\u05d4]<name>",
+                        "\u05db\u05d1[\u05d4|\u05d9] [\u05d0\u05ea] [\u05d4]<name>",
                         "\u05db\u05d9\u05d1\u05d5\u05d9 [\u05e9\u05dc] [\u05d4]<name>",
                         "\u05dc\u05db\u05d1\u05d5\u05ea [\u05d0\u05ea] [\u05d4]<name>",
-                        "\u05ea\u05db\u05d1\u05d4 [\u05d0\u05ea] [\u05d4]<name>"
+                        "\u05ea\u05db\u05d1[\u05d4|\u05d9] [\u05d0\u05ea] [\u05d4]<name>"
                     ]
                 },
                 {
                     "sentences": [
-                        "(\u05db\u05d1\u05d4|\u05db\u05d9\u05d1\u05d5\u05d9|\u05dc\u05db\u05d1\u05d5\u05ea|\u05ea\u05db\u05d1\u05d4) [\u05e9\u05dc] [\u05db\u05dc] [\u05d0\u05ea] [\u05d4](\u05d0\u05d5\u05e8|\u05d0\u05d5\u05e8\u05d5\u05ea) \u05d1<area>"
+                        "(\u05db\u05d1[\u05d4|\u05d9]|\u05db\u05d9\u05d1\u05d5\u05d9|\u05dc\u05db\u05d1\u05d5\u05ea|\u05ea\u05db\u05d1[\u05d4|\u05d9]) [\u05e9\u05dc] [\u05db\u05dc] [\u05d0\u05ea] [\u05d4](\u05d0\u05d5\u05e8|\u05d0\u05d5\u05e8\u05d5\u05ea) \u05d1<area>"
                     ],
                     "slots": {
                         "domain": "light"
                     }
                 },
                 {
                     "response": "cover_device_class",
                     "sentences": [
-                        "\u05e1\u05d2\u05d5\u05e8 [\u05d0\u05ea] [\u05d4]<name>",
-                        "\u05ea\u05e1\u05d2\u05d5\u05e8 [\u05d0\u05ea] [\u05d4]<name>"
+                        "(\u05e1\u05d2\u05d5\u05e8 | \u05e1[\u05d9]\u05d2\u05e8\u05d9) [\u05d0\u05ea] [\u05d4]<name>",
+                        "(\u05ea\u05e1\u05d2\u05d5\u05e8 | \u05ea\u05e1\u05d2\u05e8\u05d9) [\u05d0\u05ea] [\u05d4]<name>"
                     ],
                     "slots": {
                         "device_class": [
                             "garage",
                             "blind",
                             "curtain",
                             "shutter"
                         ],
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "cover_area",
                     "sentences": [
-                        "\u05e1\u05d2\u05d5\u05e8 [\u05d0\u05ea] [\u05d4]{cover_classes:device_class} \u05d1<area>",
-                        "\u05ea\u05e1\u05d2\u05d5\u05e8 [\u05d0\u05ea] [\u05d4]{cover_classes:device_class} \u05d1<area>"
+                        "(\u05e1\u05d2\u05d5\u05e8 | \u05e1[\u05d9]\u05d2\u05e8\u05d9) [\u05d0\u05ea] [\u05d4]{cover_classes:device_class} \u05d1<area>",
+                        "(\u05ea\u05e1\u05d2\u05d5\u05e8 | \u05ea\u05e1\u05d2\u05e8\u05d9) [\u05d0\u05ea] [\u05d4]{cover_classes:device_class} \u05d1<area>"
                     ],
                     "slots": {
                         "device_class": [
                             "blind",
                             "curtain",
                             "shutter",
                             "garage"
                         ],
                         "domain": "cover"
                     }
                 },
                 {
                     "sentences": [
-                        "(\u05db\u05d1\u05d4|\u05db\u05d9\u05d1\u05d5\u05d9|\u05dc\u05db\u05d1\u05d5\u05ea|\u05ea\u05db\u05d1\u05d4) [\u05e9\u05dc] [\u05db\u05dc] [\u05d0\u05ea] [\u05d4](\u05de\u05d0\u05d5\u05d5\u05e8\u05e8|\u05de\u05d0\u05d5\u05e8\u05e8) \u05d1<area>"
+                        "(\u05db\u05d1[\u05d4|\u05d9] | \u05db\u05d9\u05d1\u05d5\u05d9 | \u05dc\u05db\u05d1\u05d5\u05ea | \u05ea\u05db\u05d1[\u05d4|\u05d9]) [\u05e9\u05dc] [\u05db\u05dc] [\u05d0\u05ea] [\u05d4](\u05de\u05d0\u05d5\u05d5\u05e8\u05e8|\u05de\u05d0\u05d5\u05e8\u05e8) \u05d1<area>"
                     ],
                     "slots": {
                         "domain": "fan"
                     }
                 },
                 {
                     "sentences": [
-                        "(\u05db\u05d1\u05d4|\u05db\u05d9\u05d1\u05d5\u05d9|\u05dc\u05db\u05d1\u05d5\u05ea|\u05ea\u05db\u05d1\u05d4) [\u05e9\u05dc] [\u05db\u05dc] [\u05d0\u05ea] [\u05d4](\u05de\u05d0\u05d5\u05d5\u05e8\u05e8\u05d9\u05dd|\u05de\u05d0\u05d5\u05e8\u05e8\u05d9\u05dd) \u05d1<area>"
+                        "(\u05db\u05d1[\u05d4|\u05d9] | \u05db\u05d9\u05d1\u05d5\u05d9 | \u05dc\u05db\u05d1\u05d5\u05ea | \u05ea\u05db\u05d1[\u05d4|\u05d9]) [\u05e9\u05dc] [\u05db\u05dc] [\u05d0\u05ea] [\u05d4](\u05de\u05d0\u05d5\u05d5\u05e8\u05e8\u05d9\u05dd|\u05de\u05d0\u05d5\u05e8\u05e8\u05d9\u05dd) \u05d1<area>"
                     ],
                     "slots": {
                         "domain": "fan",
                         "name": "all"
                     }
                 }
             ]
         },
         "HassTurnOn": {
             "data": [
                 {
                     "sentences": [
-                        "(\u05d4\u05d3\u05dc\u05e7|\u05d4\u05d3\u05dc\u05e7\u05d4|\u05dc\u05d4\u05d3\u05dc\u05d9\u05e7|\u05ea\u05d3\u05dc\u05d9\u05e7) [\u05e9\u05dc] [\u05db\u05dc] [\u05d0\u05ea] [\u05d4](\u05d0\u05d5\u05e8|\u05d0\u05d5\u05e8\u05d5\u05ea) \u05d1<area>"
+                        "(\u05d4\u05d3\u05dc\u05e7|\u05d4\u05d3\u05dc\u05d9\u05e7\u05d9|\u05d4\u05d3\u05dc\u05e7\u05d4|\u05dc\u05d4\u05d3\u05dc\u05d9\u05e7|\u05ea\u05d3\u05dc\u05d9\u05e7[\u05d9]) [\u05e9\u05dc] [\u05db\u05dc] [\u05d0\u05ea] [\u05d4](\u05d0\u05d5\u05e8|\u05d0\u05d5\u05e8\u05d5\u05ea) \u05d1<area>"
                     ],
                     "slots": {
                         "domain": "light"
                     }
                 },
                 {
                     "sentences": [
-                        "(\u05d4\u05d3\u05dc\u05e7|\u05d4\u05d3\u05dc\u05e7\u05d4|\u05dc\u05d4\u05d3\u05dc\u05d9\u05e7|\u05ea\u05d3\u05dc\u05d9\u05e7) [\u05e9\u05dc] [\u05db\u05dc] [\u05d0\u05ea] [\u05d4](\u05de\u05d0\u05d5\u05d5\u05e8\u05e8|\u05de\u05d0\u05d5\u05e8\u05e8) \u05d1<area>"
+                        "(\u05d4\u05d3\u05dc\u05e7|\u05d4\u05d3\u05dc\u05d9\u05e7\u05d9|\u05d4\u05d3\u05dc\u05e7\u05d4|\u05dc\u05d4\u05d3\u05dc\u05d9\u05e7|\u05ea\u05d3\u05dc\u05d9\u05e7[\u05d9]) [\u05e9\u05dc] [\u05db\u05dc] [\u05d0\u05ea] [\u05d4](\u05de\u05d0\u05d5\u05d5\u05e8\u05e8|\u05de\u05d0\u05d5\u05e8\u05e8) \u05d1<area>"
                     ],
                     "slots": {
                         "domain": "fan"
                     }
                 },
                 {
                     "sentences": [
-                        "(\u05d4\u05d3\u05dc\u05e7|\u05d4\u05d3\u05dc\u05e7\u05d4|\u05dc\u05d4\u05d3\u05dc\u05d9\u05e7|\u05ea\u05d3\u05dc\u05d9\u05e7) [\u05e9\u05dc] [\u05db\u05dc] [\u05d0\u05ea] [\u05d4](\u05de\u05d0\u05d5\u05d5\u05e8\u05e8\u05d9\u05dd|\u05de\u05d0\u05d5\u05e8\u05e8\u05d9\u05dd) \u05d1<area>"
+                        "(\u05d4\u05d3\u05dc\u05e7|\u05d4\u05d3\u05dc\u05d9\u05e7\u05d9|\u05d4\u05d3\u05dc\u05e7\u05d4|\u05dc\u05d4\u05d3\u05dc\u05d9\u05e7|\u05ea\u05d3\u05dc\u05d9\u05e7[\u05d9]) [\u05e9\u05dc] [\u05db\u05dc] [\u05d0\u05ea] [\u05d4](\u05de\u05d0\u05d5\u05d5\u05e8\u05e8\u05d9\u05dd|\u05de\u05d0\u05d5\u05e8\u05e8\u05d9\u05dd) \u05d1<area>"
                     ],
                     "slots": {
                         "domain": "fan",
                         "name": "all"
                     }
                 },
                 {
                     "sentences": [
-                        "\u05d4\u05d3\u05dc\u05e7 [\u05d0\u05ea] [\u05d4]<name>",
+                        "(\u05d4\u05d3\u05dc\u05e7 | \u05d4\u05d3\u05dc\u05d9\u05e7\u05d9) [\u05d0\u05ea] [\u05d4]<name>",
                         "\u05d4\u05d3\u05dc\u05e7\u05d4 [\u05e9\u05dc] [\u05d4]<name>",
                         "\u05dc\u05d4\u05d3\u05dc\u05d9\u05e7 [\u05d0\u05ea] [\u05d4]<name>",
-                        "\u05ea\u05d3\u05dc\u05d9\u05e7 [\u05d0\u05ea] [\u05d4]<name>"
+                        "\u05ea\u05d3\u05dc\u05d9\u05e7[\u05d9] [\u05d0\u05ea] [\u05d4]<name>"
                     ]
                 },
                 {
                     "response": "cover_device_class",
                     "sentences": [
-                        "\u05e4\u05ea\u05d7 [\u05d0\u05ea] [\u05d4]<name>",
-                        "\u05ea\u05e4\u05ea\u05d7 [\u05d0\u05ea] [\u05d4]<name>"
+                        "\u05e4\u05ea\u05d7[\u05d9] [\u05d0\u05ea] [\u05d4]<name>",
+                        "\u05ea\u05e4\u05ea\u05d7[\u05d9] [\u05d0\u05ea] [\u05d4]<name>"
                     ],
                     "slots": {
                         "device_class": [
                             "garage",
                             "blind",
                             "curtain",
                             "shutter"
                         ],
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "cover_area",
                     "sentences": [
-                        "\u05e4\u05ea\u05d7 [\u05d0\u05ea] [\u05d4]{cover_classes:device_class} \u05d1<area>",
-                        "\u05ea\u05e4\u05ea\u05d7 [\u05d0\u05ea] [\u05d4]{cover_classes:device_class} \u05d1<area>"
+                        "\u05e4\u05ea\u05d7[\u05d9] [\u05d0\u05ea] [\u05d4]{cover_classes:device_class} \u05d1<area>",
+                        "\u05ea\u05e4\u05ea\u05d7[\u05d9] [\u05d0\u05ea] [\u05d4]{cover_classes:device_class} \u05d1<area>"
                     ],
                     "slots": {
                         "device_class": [
                             "blind",
                             "curtain",
                             "shutter",
                             "garage"
@@ -610,12 +610,12 @@
             }
         }
     },
     "skip_words": [
         "\u05d0\u05e0\u05d0",
         "\u05e0\u05d0",
         "\u05d1\u05d1\u05e7\u05e9\u05d4",
-        "\u05d0\u05ea\u05d4 \u05d9\u05db\u05d5\u05dc",
-        "\u05ea\u05d5\u05db\u05dc",
+        "\u05d0\u05ea[\u05d4] \u05d9\u05db\u05d5\u05dc[\u05d4]",
+        "\u05ea\u05d5\u05db\u05dc[\u05d9]",
         "\u05d0\u05e4\u05e9\u05e8"
     ]
 }
```

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/data/hi.json` & `home-assistant-intents-2024.5.28/home_assistant_intents/data/hi.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/data/hr.json` & `home-assistant-intents-2024.5.28/home_assistant_intents/data/hr.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/data/hu.json` & `home-assistant-intents-2024.5.28/home_assistant_intents/data/hu.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/data/id.json` & `home-assistant-intents-2024.5.28/home_assistant_intents/data/id.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/data/is.json` & `home-assistant-intents-2024.5.28/home_assistant_intents/data/is.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/data/it.json` & `home-assistant-intents-2024.5.28/home_assistant_intents/data/it.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9334446519774264%*

 * *Differences: {"'expansion_rules'": '{\'the\': "(l(o |a |e )|i[l] |gli |l(`|’|\')[ ]|in |a |(a|ne)(l |llo |lla '*

 * *                      '|lle |ll(`|’|\')[ ]|gli ))", \'in\': "(all\'interno |dentro |in | ne[l |i '*

 * *                      '|gli |llo |lla |lle |ll(`|’|\')[ ]])", \'of\': "(de[l |llo |lla |lle '*

 * *                      '|ll(`|’|\')[ ]|i |gli ]|di )", \'to\': "(a[l |llo |lla |lle |ll(`|’|\')[ '*

 * *                      ']|gli ])", \'name\': \'[<the>]{name}\', \'area\': \'[<the>][area ]{area}\', '*

 * *                      […]*

```diff
@@ -1,31 +1,48 @@
 {
     "expansion_rules": {
         "all": "(tutt(o|e|i|a) [quant(i|e)] | ogni)",
-        "area": "{area}",
-        "brightness": "{brightness}[%| percento]",
+        "area": "[<the>][area ]{area}",
+        "brightness": "{brightness}[[ ]<percent>]",
         "climate": "(clima|climatizzator(e|i)|condizionator(e|i)|aria condizionata)",
         "close": "(chiud(i|ere) | abbass(a|are))",
+        "closed": "chius(o|a|e|i)",
         "cover": "(tend(a|e)[ da sole]|serrand(a|e)|tapparell(a|e)|persian(a|e)|port(a|e)|saracinesc(a|he)|venezian(a|e)|cancell(o|i)|finestr(a|e)|oscurant(e|i))",
         "fan": "(ventol(a|e) | ventilator(e|i) | ventilazione | climatizzator(e|i) | condizionator(e|i))",
+        "floor": "[<the>][floor ]{floor}",
         "garage": "(serrand(a|e) | port(a|e) [basculant(e|i)|de(l|i) garage] | saracinesc(a|he))",
         "home": "(casa|appartamento)",
-        "in": "(in | ne[i |gli |l[lo |la |le |l'| ]])",
+        "how_many": "quant(i|e) [sono]",
+        "in": "(all'interno |dentro |in | ne[l |i |gli |llo |lla |lle |ll(`|\u2019|')[ ]])",
         "in_here": "(qu(a|i)|in questa (stanza|camera))",
-        "light": "luc(e|i)",
-        "name": "{name}",
-        "of": "(de[l[lo |la |le |l'| ]]|i |gli |di )",
+        "light": "( [punt(o|i)] luce | luci | lampad[in](a|e) | lampadari[o])",
+        "lock": "(port(a|e) | blocch(o|hi) | serratur(a|e) | lucchett(o|i))",
+        "locked": "(chius|serrat|sbarrat|bloccat)(o|a|e|i)",
+        "name": "[<the>]{name}",
+        "numeric_value_set": "(<set> | [fa(`|\u2019|'|i|re) ]((alz|aument|increment|abbass)(a|are) | ridu(ci|rre)) | fa(`|\u2019|'|i|re) (salire|scendere))",
+        "of": "(de[l |llo |lla |lle |ll(`|\u2019|')[ ]|i |gli ]|di )",
         "open": "(apr(i|ire) | alz(a|are))",
-        "set": "(impost(a|are) | cambi(a|are) | mett(i|ere) | modific(a|are))",
-        "temperature": "{temperature}[\u00b0| gradi] [{temperature_unit}]",
-        "the": "(l(o|a|e) | i[l] | gli | l'| in | ne(l|llo|lla|lle|ll'|gli) | a[(l|llo|lla|lle|ll'|gli)])",
-        "to": "a[l[lo |la |le |l'] | gli ]",
+        "opened": "(apert|spalancat)(o|a|e|i)",
+        "percent": "(%|percento|per cento|su cento)",
+        "position": "{position}[[ ]<percent>]",
+        "set": "( (impost|mett|modific|cambi|sett)(a|are) | rend(i|ere) )",
+        "some": "(qualche | qualcun(o|a) | un[(o |a |(`|\u2019|')[ ])] | de[i |gli |lle ] | alcun(o|a) | nessun(o|a))",
+        "temperature": "{temperature}[ ][{temperature_unit}]",
+        "the": "(l(o |a |e )|i[l] |gli |l(`|\u2019|')[ ]|in |a |(a|ne)(l |llo |lla |lle |ll(`|\u2019|')[ ]|gli ))",
+        "there_is": "(c'\u00e8|c(`|\u2019|')e(`|\u2019|')|ci sta[nno]|ci sono)",
+        "to": "(a[l |llo |lla |lle |ll(`|\u2019|')[ ]|gli ])",
+        "to_lock": "(chiud[i|ere]|blocca[re])",
+        "triggered": "(rilevat|attiv[at])(o|a|e|i)",
         "turn_off": "((spegn|speng)(i|ere) | disattiv(a|are))",
-        "turn_on": "(accend(i|ere) | attiv(a|are))",
-        "what_is": "(qual[e] \u00e8|quant(o |')\u00e8|com(e |')\u00e8|che)"
+        "turn_on": "[fa(`|\u2019|'|i|re)](accend(i|ere) | attiv(a|are))",
+        "unlock": "(apri[re]|sblocca[re]|schiud[i|ere])",
+        "unlocked": "(apert|sbloccat)(o|a|e|i)",
+        "volume": "{volume:volume_level}[[ ]<percent>]",
+        "what_is": "(qual[e] \u00e8 | quant(o |(`|\u2019|'))\u00e8 | com(e |(`|\u2019|'))\u00e8 | che)",
+        "which": "(qual[e|i] sono | che)"
     },
     "intents": {
         "HassClimateGetTemperature": {
             "data": [
                 {
                     "sentences": [
                         "[<what_is>] [la] temperatura [c'\u00e8] [(<in> | <of> | <the>)] [<area>]",
@@ -237,21 +254,21 @@
                 }
             ]
         },
         "HassShoppingListAddItem": {
             "data": [
                 {
                     "expansion_rules": {
+                        "add": "((mett|aggiung)[i|ere]|inseri[sci|re])",
                         "item": "{shopping_list_item:item}",
-                        "my_list": "[mia ]lista[ della spesa]"
+                        "my_list": " [(mio|mia|mie|miei|nostra|nostre)] (lista [della spesa]|shopping list)"
                     },
                     "response": "item_added",
                     "sentences": [
-                        "aggiungi <item>[ alla <my_list>]",
-                        "metti <item> nella <my_list>"
+                        "<add> <item> [(<in>|sulla|alla) <my_list>]"
                     ]
                 }
             ]
         },
         "HassTurnOff": {
             "data": [
                 {
@@ -505,42 +522,41 @@
                             "lock",
                             "scene",
                             "script",
                             "sensor"
                         ]
                     },
                     "sentences": [
-                        "<turn_on> [<the>]<name> [<in><area>]",
-                        "[<the>]<name> <turn_on> [<in><area>]"
+                        "<turn_on> <name> [<in><area>]"
                     ]
                 },
                 {
                     "requires_context": {
                         "domain": "cover"
                     },
                     "response": "cover",
                     "sentences": [
-                        "<open> [<the>] {name} [[<in>|<of>]{area}]"
+                        "<open> <name> [[<in>|<of>]{area}]"
                     ]
                 },
                 {
                     "response": "cover_area",
                     "sentences": [
-                        "<open> [<all>] [<in>|<the>] {area}"
+                        "<open> [<all>] [<in>|<the>]{area}"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "cover_device_class",
                     "sentences": [
                         "<open> <all> [<the>]{cover_classes:device_class}",
                         "<open> [<all>] [<the>]{cover_classes:device_class} [<in>|<of>]<home>",
-                        "<open> (<in>|<of>)<home> [<all>] [<the>] {cover_classes:device_class}"
+                        "<open> (<in>|<of>)<home> [<all>] [<the>]{cover_classes:device_class}"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
                 },
                 {
                     "requires_context": {
@@ -551,16 +567,16 @@
                         "<open> [<all>] [<the>]{cover_classes:device_class} [[<in>|<of>]{area}]",
                         "<open> [[<in>|<of>]{area}] [<all>] [<the>]{cover_classes:device_class}"
                     ]
                 },
                 {
                     "response": "cover_garage",
                     "sentences": [
-                        "<open> <the> <garage> [del garage]",
-                        "<open> [[<in>] garage] <the> <garage>"
+                        "<open> <the><garage> [del garage]",
+                        "<open> [[<in>]garage] <the><garage>"
                     ],
                     "slots": {
                         "device_class": "garage",
                         "domain": "cover"
                     }
                 },
                 {
@@ -588,59 +604,59 @@
                 "to": 100,
                 "type": "percentage"
             }
         },
         "brightness_level": {
             "values": [
                 {
-                    "in": "massimo",
+                    "in": "[al] massimo",
                     "out": 100
                 },
                 {
-                    "in": "minimo",
+                    "in": "[al] minimo",
                     "out": 1
                 },
                 {
-                    "in": "met\u00e0",
+                    "in": "[a] met\u00e0",
                     "out": 50
                 }
             ]
         },
         "bs_battery_charging_states": {
             "values": [
                 {
-                    "in": "[in] carica",
+                    "in": "(in carica|caricando)",
                     "out": "on"
                 },
                 {
                     "in": "non in carica",
                     "out": "off"
                 }
             ]
         },
         "bs_battery_states": {
             "values": [
                 {
-                    "in": "bass(o|a|e|i)",
+                    "in": "bass(o|a|e|i)|scaric(o|a|he|hi)|per scaricar(e|si)",
                     "out": "on"
                 },
                 {
-                    "in": "normale",
+                    "in": "normale|caric(o|a|he|hi)",
                     "out": "off"
                 }
             ]
         },
         "bs_carbon_monoxide_states": {
             "values": [
                 {
-                    "in": "(rilevat|attiv[at])(o|a|e|i)",
+                    "in": "<triggered>",
                     "out": "on"
                 },
                 {
-                    "in": "non rilevat(o|a|e|i)",
+                    "in": "non <triggered>",
                     "out": "off"
                 }
             ]
         },
         "bs_cold_states": {
             "values": [
                 {
@@ -664,43 +680,43 @@
                     "out": "off"
                 }
             ]
         },
         "bs_door_states": {
             "values": [
                 {
-                    "in": "apert(o|a|e|i)",
+                    "in": "<opened>",
                     "out": "on"
                 },
                 {
-                    "in": "chius(o|a|e|i)",
+                    "in": "<closed>",
                     "out": "off"
                 }
             ]
         },
         "bs_garage_door_states": {
             "values": [
                 {
-                    "in": "apert(o|a|e|i)",
+                    "in": "<opened>",
                     "out": "on"
                 },
                 {
-                    "in": "chus(o|a|e|i)",
+                    "in": "<closed>",
                     "out": "off"
                 }
             ]
         },
         "bs_gas_states": {
             "values": [
                 {
-                    "in": "(rilevat|attiv[at])(o|a|e|i)",
+                    "in": "<triggered>",
                     "out": "on"
                 },
                 {
-                    "in": "non rilevat(o|a|e|i)",
+                    "in": "non <triggered>",
                     "out": "off"
                 }
             ]
         },
         "bs_heat_states": {
             "values": [
                 {
@@ -712,31 +728,31 @@
                     "out": "off"
                 }
             ]
         },
         "bs_light_states": {
             "values": [
                 {
-                    "in": "(rilevat|attiv[at]|acces)(o|a|e|i)",
+                    "in": "<triggered>|acces(o|a|e|i)",
                     "out": "on"
                 },
                 {
                     "in": "no luce",
                     "out": "off"
                 }
             ]
         },
         "bs_lock_states": {
             "values": [
                 {
-                    "in": "apert(o|a|e|i)",
+                    "in": "<unlocked>",
                     "out": "on"
                 },
                 {
-                    "in": "chius(o|a|e|i)",
+                    "in": "<locked>",
                     "out": "off"
                 }
             ]
         },
         "bs_moisture_states": {
             "values": [
                 {
@@ -748,67 +764,67 @@
                     "out": "off"
                 }
             ]
         },
         "bs_motion_states": {
             "values": [
                 {
-                    "in": "(rilevat|attiv[at])(o|a|e|i)",
+                    "in": "<triggered>",
                     "out": "on"
                 },
                 {
                     "in": "liber(o|a|e|i)",
                     "out": "off"
                 }
             ]
         },
         "bs_occupancy_states": {
             "values": [
                 {
-                    "in": "(rilevat|attiv[at])(o|a|e|i)",
+                    "in": "<triggered>",
                     "out": "on"
                 },
                 {
                     "in": "(liber|sgombr)(o|a|e|i)",
                     "out": "off"
                 }
             ]
         },
         "bs_opening_states": {
             "values": [
                 {
-                    "in": "apert(o|a|e|i)",
+                    "in": "<opened>",
                     "out": "on"
                 },
                 {
-                    "in": "chius(o|a|e|i)",
+                    "in": "<closed>",
                     "out": "off"
                 }
             ]
         },
         "bs_plug_states": {
             "values": [
                 {
-                    "in": "(attaccat|collegat)(o|a|e|i)",
+                    "in": "(attaccat|collegat|alimentat)(o|a|e|i)",
                     "out": "on"
                 },
                 {
-                    "in": "(staccat|non attaccat|scollegat|non collegat)(o|a|e|i)",
+                    "in": "(staccat|scollegat|non (attaccat|collegat|alimentat)(o|a|e|i))",
                     "out": "off"
                 }
             ]
         },
         "bs_power_states": {
             "values": [
                 {
-                    "in": "(attaccat|collegat)(o|a|e|i)",
+                    "in": "(attaccat|collegat|alimentat)(o|a|e|i)",
                     "out": "on"
                 },
                 {
-                    "in": "(staccat|non attaccat|scollegat|non collegat)(o|a|e|i)",
+                    "in": "(staccat|scollegat|non (attaccat|collegat|alimentat)(o|a|e|i))",
                     "out": "off"
                 }
             ]
         },
         "bs_presence_states": {
             "values": [
                 {
@@ -824,15 +840,15 @@
         "bs_problem_states": {
             "values": [
                 {
                     "in": "rilevat(o|i)",
                     "out": "on"
                 },
                 {
-                    "in": "ok",
+                    "in": "ok|a posto",
                     "out": "off"
                 }
             ]
         },
         "bs_running_states": {
             "values": [
                 {
@@ -856,79 +872,79 @@
                     "out": "off"
                 }
             ]
         },
         "bs_smoke_states": {
             "values": [
                 {
-                    "in": "(rilevat|attiv[at])(o|a|e|i)",
+                    "in": "<triggered>",
                     "out": "on"
                 },
                 {
-                    "in": "liber(o|a|e|i)",
+                    "in": "non <triggered>",
                     "out": "off"
                 }
             ]
         },
         "bs_sound_states": {
             "values": [
                 {
-                    "in": "(rilevat|attiv[at])(o|a|e|i)",
+                    "in": "<triggered>",
                     "out": "on"
                 },
                 {
-                    "in": "liber(o|a|e|i)",
+                    "in": "non <triggered>",
                     "out": "off"
                 }
             ]
         },
         "bs_tamper_states": {
             "values": [
                 {
-                    "in": "(rilevat|attiv[at]|manomess|alterat)(o|a|e|i)",
+                    "in": "<triggered>|(manomess|alterat)(o|a|e|i)",
                     "out": "on"
                 },
                 {
-                    "in": "liber(o|a|e|i)",
+                    "in": "non (<triggered>|(manomess|alterat)(o|a|e|i))",
                     "out": "off"
                 }
             ]
         },
         "bs_update_states": {
             "values": [
                 {
-                    "in": "aggiornamento disponibile",
+                    "in": "aggiornamento disponibile|da aggiornare|non aggiornato",
                     "out": "on"
                 },
                 {
-                    "in": "aggornato",
+                    "in": "aggiornato",
                     "out": "off"
                 }
             ]
         },
         "bs_vibration_states": {
             "values": [
                 {
-                    "in": "(rilevat(a|a|e|i)|[in ]vibrazione)",
+                    "in": "(<triggered>|[in ]vibrazione|[sta[nno]] vibrando)",
                     "out": "on"
                 },
                 {
-                    "in": "(liber(a|a|e|i)|non [in ]vibrazione)",
+                    "in": "(liber(a|a|e|i)|non (<triggered>|[in ]vibrazione|[sta[nno] vibrando]))",
                     "out": "off"
                 }
             ]
         },
         "bs_window_states": {
             "values": [
                 {
-                    "in": "apert(o|a|e|i)",
+                    "in": "<opened>",
                     "out": "on"
                 },
                 {
-                    "in": "chius(o|a|e|i)",
+                    "in": "<closed>",
                     "out": "closed"
                 }
             ]
         },
         "color": {
             "values": [
                 {
@@ -1016,51 +1032,51 @@
                     "out": "window"
                 }
             ]
         },
         "cover_states": {
             "values": [
                 {
-                    "in": "apert(a|o|e|i)",
+                    "in": "<opened>|alzat(a|o|e|i)|tirat(a|o|e|i) su",
                     "out": "open"
                 },
                 {
-                    "in": "chius(a|o|e|i)",
+                    "in": "<closed>|abbassat(a|o|e|i)|tirat(a|o|e|i) gi\u00f9",
                     "out": "closed"
                 },
                 {
-                    "in": "in apertura",
+                    "in": "(in apertura | [si sta[nno]] (aprendo | alzando | tirando su))",
                     "out": "opening"
                 },
                 {
-                    "in": "in chiusura",
+                    "in": "(in chiusura | [si sta[nno]] (chiudendo | abbassando | tirando gi\u00f9))",
                     "out": "closing"
                 }
             ]
         },
         "lock_states": {
             "values": [
                 {
-                    "in": "chius(o|a|e|i)",
+                    "in": "<locked>",
                     "out": "locked"
                 },
                 {
-                    "in": "apert(o|a|e|i)",
+                    "in": "<unlocked>",
                     "out": "unlocked"
                 }
             ]
         },
         "on_off_domains": {
             "values": [
                 {
-                    "in": "luc(e|i)",
+                    "in": "<light>",
                     "out": "light"
                 },
                 {
-                    "in": "(ventol(a|e)|ventilator(e|i)|ventilazione|climatizzator(e|i)|condizionator(e|i))",
+                    "in": "<fan>",
                     "out": "fan"
                 },
                 {
                     "in": "(interruttor(e|i)|pres(a|e))",
                     "out": "switch"
                 }
             ]
@@ -1073,57 +1089,80 @@
                 },
                 {
                     "in": "(spent|disattiv[at])(o|i|a|e)",
                     "out": "off"
                 }
             ]
         },
+        "position": {
+            "range": {
+                "from": 0,
+                "to": 100,
+                "type": "percentage"
+            }
+        },
         "shopping_list_item": {
             "wildcard": true
         },
         "temperature": {
             "range": {
                 "from": 0,
                 "to": 100,
                 "type": "temperature"
             }
         },
         "temperature_unit": {
             "values": [
-                "(celsius | centigradi)",
                 {
-                    "in": "c",
+                    "in": "([ ]\u00b0|[ ][\u00b0][ ](C|c|celsius|Celsius)| [gradi] centigradi)",
                     "out": "celsius"
                 },
-                "fahrenheit",
                 {
-                    "in": "f",
+                    "in": "([ ][\u00b0][ ](F|f|Fahreneit|fahreneit)| [gradi] fahrenheit)",
                     "out": "fahrenheit"
                 }
             ]
+        },
+        "volume": {
+            "range": {
+                "from": 0,
+                "to": 100,
+                "type": "percentage"
+            }
+        },
+        "zone": {
+            "wildcard": true
         }
     },
     "responses": {
         "errors": {
             "duplicate_entities": "Mi dispiace, esistono pi\u00f9 dispositivi chiamati {{ entity }}",
             "duplicate_entities_in_area": "Mi dispiace, nell'area {{ area }} esistono pi\u00f9 dispositivi chiamati {{ entity }}",
+            "duplicate_entities_in_floor": "Mi dispiace, nel piano {{ floor }} esistono pi\u00f9 dispositivi chiamati {{ entity }}",
             "handle_error": "Si \u00e8 verificato un errore inatteso durante l'elaborazione",
             "no_area": "Non conosco nessuna area chiamata {{ area }}",
             "no_device_class": "Mi dispiace, non conosco nessun dispositivo appartenente alla classe {{ device_class }}",
             "no_device_class_exposed": "Mi dispiace, nessun dispositivo appartenente alla classe {{ device_class }} \u00e8 stato esposto",
             "no_device_class_in_area": "Mi dispiace, nell'area {{ area }} non conosco nessun dispositivo appartenente alla classe {{ device_class }}",
             "no_device_class_in_area_exposed": "Mi dispiace, nell'area {{ area }} nessun dispositivo appartenente alla classe {{ device_class }} \u00e8 stato esposto",
+            "no_device_class_in_floor": "Mi dispiace, nel piano {{ floor }} non conosco nessun dispositivo appartenente alla classe {{ device_class }}",
+            "no_device_class_in_floor_exposed": "Mi dispiace, nel piano {{ floor }} nessun dispositivo appartenente alla classe {{ device_class }} \u00e8 stato esposto",
             "no_domain": "Mi dispiace, non conosco nessun dispositivo appartenente al dominio {{ domain }}",
             "no_domain_exposed": "Mi dispiace, il dominio {{ domain }} non \u00e8 stato esposto",
             "no_domain_in_area": "Mi dispiace, nell'area {{ area }} non conosco nessun dispositivo appartenente al dominio {{ domain }}",
             "no_domain_in_area_exposed": "Mi dispiace, nell'area {{ area }} il dominio {{ domain }} non \u00e8 stato esposto",
-            "no_entity": "Mi dispiace, non sconosco nessun dispositivo chiamato {{ entity }}",
+            "no_domain_in_floor": "Mi dispiace, nel piano {{ floor }} non conosco nessun dispositivo appartenente al dominio {{ domain }}",
+            "no_domain_in_floor_exposed": "Mi dispiace, nel piano {{ floor }} il dominio {{ domain }} non \u00e8 stato esposto",
+            "no_entity": "Mi dispiace, non conosco nessun dispositivo chiamato {{ entity }}",
             "no_entity_exposed": "Mi dispiace, il dispositivo {{ entity }} non \u00e8 stato esposto",
-            "no_entity_in_area": "Mi dispiace, nell'area {{ area }} non sconosco nessun dispositivo chiamato {{ entity }}",
+            "no_entity_in_area": "Mi dispiace, nell'area {{ area }} non conosco nessun dispositivo chiamato {{ entity }}",
             "no_entity_in_area_exposed": "Mi dispiace, il dispositivo {{ entity }} nell'area {{ area }} non \u00e8 stato esposto",
+            "no_entity_in_floor": "Mi dispiace, nel piano {{ floor }} non conosco nessun dispositivo chiamato {{ entity }}",
+            "no_entity_in_floor_exposed": "Mi dispiace, il dispositivo {{ entity }} nel piano {{ floor }} non \u00e8 stato esposto",
+            "no_floor": "Mi dispiace, non conosco nessun piano chiamato {{ floor }}",
             "no_intent": "Mi dispiace, non ho capito"
         },
         "intents": {
             "HassClimateGetTemperature": {
                 "default": "{% set temperature = state_attr(state.entity_id, 'current_temperature') %} {% if temperature == 1: %} {{ temperature }} grado {% else: %} {{ temperature }} gradi {% endif %}\n"
             },
             "HassGetState": {
```

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/data/ka.json` & `home-assistant-intents-2024.5.28/home_assistant_intents/data/ka.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/data/kn.json` & `home-assistant-intents-2024.5.28/home_assistant_intents/data/kn.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/data/ko.json` & `home-assistant-intents-2024.5.28/home_assistant_intents/data/ko.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/data/lb.json` & `home-assistant-intents-2024.5.28/home_assistant_intents/data/lb.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/data/lt.json` & `home-assistant-intents-2024.5.28/home_assistant_intents/data/lt.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/data/lv.json` & `home-assistant-intents-2024.5.28/home_assistant_intents/data/lv.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9772569444444444%*

 * *Differences: {"'intents'": "{'HassGetWeather': OrderedDict([('data', [OrderedDict([('sentences', ['kād[s|i|as] "*

 * *              "[šobrīd|ārā|ir] (laiks|laikapstākļi|laika apstākļi|laika ziņas)'])]), "*

 * *              "OrderedDict([('sentences', ['kād[s|i|as] [šobrīd|ārā|ir] (laiks|laikapstākļi|laika "*

 * *              "apstākļi|laika ziņas) <name>', 'kād[s|i|as] (laiks|laikapstākļi|laika "*

 * *              "apstākļi|laika ziņas) [šobrīd|ir] <name>']), ('requires_context', "*

 * *              "OrderedDict([('domain', 'weather')]))])] […]*

```diff
@@ -21,14 +21,32 @@
                         "k\u0101da temperat\u016bra [<area>]",
                         "cik <area> (karst(i|s|a) | aukst(i|s|a) | silt(i|s|a) | v\u0113si)",
                         "cik (karst(i|s|a) | aukst(i|s|a) | silt(i|s|a) | v\u0113si) [<area>]"
                     ]
                 }
             ]
         },
+        "HassGetWeather": {
+            "data": [
+                {
+                    "sentences": [
+                        "k\u0101d[s|i|as] [\u0161obr\u012bd|\u0101r\u0101|ir] (laiks|laikapst\u0101k\u013ci|laika apst\u0101k\u013ci|laika zi\u0146as)"
+                    ]
+                },
+                {
+                    "requires_context": {
+                        "domain": "weather"
+                    },
+                    "sentences": [
+                        "k\u0101d[s|i|as] [\u0161obr\u012bd|\u0101r\u0101|ir] (laiks|laikapst\u0101k\u013ci|laika apst\u0101k\u013ci|laika zi\u0146as) <name>",
+                        "k\u0101d[s|i|as] (laiks|laikapst\u0101k\u013ci|laika apst\u0101k\u013ci|laika zi\u0146as) [\u0161obr\u012bd|ir] <name>"
+                    ]
+                }
+            ]
+        },
         "HassLightSet": {
             "data": [
                 {
                     "response": "brightness",
                     "sentences": [
                         "<set> <name> [gaismas] (spilgtumu | spo\u017eumu) [uz] <brightness>",
                         "<set> <name> uz <brightness> [spilgtuma]"
@@ -329,35 +347,38 @@
             "no_intent": "Atvainojiet, es nevar\u0113ju to saprast"
         },
         "intents": {
             "HassClimateGetTemperature": {
                 "default": "{{ state.state }} gr\u0101du"
             },
             "HassGetState": {},
+            "HassGetWeather": {
+                "default": "{% set weather_condition = {\n  'clear': 'skaidrs laiks',\n  'clear-night': 'skaidrs laiks',\n  'cloudy': 'm\u0101ko\u0146ains',\n  'exceptional': '\u0101rk\u0101rt\u0113js',\n  'fog': 'migla',\n  'hail': 'krusa',\n  'lightning': 'p\u0113rkons',\n  'lightning-rainy': 'p\u0113\u0157kons un lietus',\n  'partlycloudy': 'da\u013c\u0113ji m\u0101ko\u0146ains',\n  'pouring': 'lietusg\u0101zes',\n  'rainy': 'l\u012bst',\n  'snowy': 'snieg',\n  'snowy-rainy': 'slapj\u0161 sniegs',\n  'sunny': 'saulains',\n  'windy': 'v\u0113jains',\n  'windy-variant': 'ar v\u0113ju un lietu'\n} %} {{ state.attributes.get('temperature') }} {{ state.attributes.get('temperature_unit') }} {{ weather_condition.get((state.state | string).lower(), \"\") }}\n"
+            },
             "HassLightSet": {
-                "brightness": "{{ slots.name }} brightness set to {{ slots.brightness }}",
-                "brightness_area": "Brightness in {{ slots.area }} set to {{ slots.brightness }}",
-                "color": "{{ slots.name }} color set to {{ slots.color }}",
-                "color_area": "Color in {{ slots.area }} set to {{ slots.color }}"
+                "brightness": "{{ slots.name }} spilgtums nomain\u012bts uz {{ slots.brightness }}",
+                "brightness_area": "Spilgtums {{ slots.area }} nomain\u012bts uz {{ slots.brightness }}",
+                "color": "{{ slots.name }} kr\u0101sa nomain\u012bta uz {{ slots.color }}",
+                "color_area": "Kr\u0101sa {{ slots.area }} nomain\u012bta uz {{ slots.color }}"
             },
             "HassTurnOff": {
-                "cover": "Closed {{ slots.name }}",
-                "cover_area": "Closed {{ slots.area }}",
-                "cover_device_class": "Closed {{ slots.device_class }}",
-                "default": "Turned off {{ slots.name }}",
-                "fans_area": "Turned off fans in {{ slots.area }}",
-                "lights_area": "Turned off lights in {{ slots.area }}"
+                "cover": "Aizv\u0113ru {{ slots.name }}",
+                "cover_area": "Aizv\u0113ru {{ slots.area }}",
+                "cover_device_class": "Aizv\u0113ru {{ slots.device_class }}",
+                "default": "Izsl\u0113dzu {{ slots.name }}",
+                "fans_area": "Izsl\u0113dzu ventilatorus {{ slots.area }}",
+                "lights_area": "Izsl\u0113dzu gaismas {{ slots.area }}"
             },
             "HassTurnOn": {
-                "cover": "Opened {{ slots.name }}",
-                "cover_area": "Opened {{ slots.area }}",
-                "cover_device_class": "Opened {{ slots.device_class }}",
-                "default": "Turned on {{ slots.name }}",
-                "fans_area": "Turned on fans in {{ slots.area }}",
-                "lights_area": "Turned on lights in {{ slots.area }}"
+                "cover": "Atv\u0113ru {{ slots.name }}",
+                "cover_area": "Atv\u0113ru {{ slots.area }}",
+                "cover_device_class": "Atv\u0113ru {{ slots.device_class }}",
+                "default": "Iesl\u0113dzu {{ slots.name }}",
+                "fans_area": "Iesl\u0113dzu ventilatorus {{ slots.area }}",
+                "lights_area": "Iesl\u0113dzu gaismas {{ slots.area }}"
             }
         }
     },
     "skip_words": [
         "l\u016bdzu",
         "paldies",
         "[vai] vari",
```

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/data/ml.json` & `home-assistant-intents-2024.5.28/home_assistant_intents/data/ml.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/data/mn.json` & `home-assistant-intents-2024.5.28/home_assistant_intents/data/mn.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/data/ms.json` & `home-assistant-intents-2024.5.28/home_assistant_intents/data/ms.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/data/nb.json` & `home-assistant-intents-2024.5.28/home_assistant_intents/data/nb.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9891304347826088%*

 * *Differences: {"'responses'": "{'errors': {'no_entity_exposed': '{{ entity }} er ikke eksponert', "*

 * *                "'no_entity_in_area_exposed': '{{ entity }} i {{ area }} er ikke eksponert', "*

 * *                "'no_entity_in_floor_exposed': '{{ entity }} i {{ floor }} er ikke eksponert', "*

 * *                "'no_domain_exposed': '{{ domain }} er ikke eksponert', "*

 * *                "'no_domain_in_area_exposed': '{{ domain }} i {{ area }} er ikke eksponert', "*

 * *                "'no_domain_in_floor_exposed': '{{ domain }} i {{ […]*

```diff
@@ -2568,23 +2568,35 @@
                 "to": 100,
                 "type": "percentage"
             }
         }
     },
     "responses": {
         "errors": {
+            "duplicate_entities": "Det finnes flere enheter som heter {{ entity }}",
+            "duplicate_entities_in_area": "Det finnes flere enheter som heter {{ entity }} i {{ area }}",
+            "duplicate_entities_in_floor": "Det finnes flere enheter som heter {{ entity }} i {{ floor }}",
             "handle_error": "Det oppsto en uventet feil",
             "no_area": "Det er ingen omr\u00e5der som heter {{ area }}",
+            "no_device_class_exposed": "{{ device_class }} er ikke eksponert",
             "no_device_class_in_area": "{{ area }} har ingen {{ device_class }}",
+            "no_device_class_in_area_exposed": "{{ device_class }} i {{ area }} er ikke eksponert",
             "no_device_class_in_floor": "{{ floor }} har ingen {{ device_class }}",
+            "no_device_class_in_floor_exposed": "{{ device_class }} i {{ floor }} er ikke eksponert",
+            "no_domain_exposed": "{{ domain }} er ikke eksponert",
             "no_domain_in_area": "{{ area }} har ingen {{ domain }}",
+            "no_domain_in_area_exposed": "{{ domain }} i {{ area }} er ikke eksponert",
             "no_domain_in_floor": "{{ floor }} har ingen {{ domain }}",
+            "no_domain_in_floor_exposed": "{{ domain }} i {{ floor }} er ikke eksponert",
             "no_entity": "Finner ingen enhet som heter {{ entity }}",
+            "no_entity_exposed": "{{ entity }} er ikke eksponert",
             "no_entity_in_area": "Finner ingen enhet som heter {{ entity }} i {{ area }}",
+            "no_entity_in_area_exposed": "{{ entity }} i {{ area }} er ikke eksponert",
             "no_entity_in_floor": "Finner ingen enhet som heter {{ entity }} i {{ floor }}",
+            "no_entity_in_floor_exposed": "{{ entity }} i {{ floor }} er ikke eksponert",
             "no_floor": "Det er ingen etasje som heter {{ floor }}",
             "no_intent": "Jeg skj\u00f8nte dessverre ikke det"
         },
         "intents": {
             "HassClimateGetTemperature": {
                 "default": "{{ state_attr(state.entity_id, 'current_temperature') }}"
             },
```

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/data/nl.json` & `home-assistant-intents-2024.5.28/home_assistant_intents/data/nl.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/data/pl.json` & `home-assistant-intents-2024.5.28/home_assistant_intents/data/pl.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/data/pt-br.json` & `home-assistant-intents-2024.5.28/home_assistant_intents/data/pt-br.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9886921296296296%*

 * *Differences: {"'expansion_rules'": "{'piso': '[do] [(piso|andar)] [de] {floor}'}",*

 * * "'intents'": "{'HassTurnOff': {'data': {insert: [(3, OrderedDict([('sentences', ['<desligar> "*

 * *              "[tod[a|o]s] [(o[s]| a[s])] (luz[es]| lâmpada[s]) <piso>']), ('response', "*

 * *              "'lights_floor'), ('slots', OrderedDict([('domain', 'light')]))]))]}}, 'HassTurnOn': "*

 * *              "{'data': {insert: [(2, OrderedDict([('sentences', ['<ligar> [tod[a|o]s] [(o[s]| "*

 * *              "a[s])] (luz[es]| lâmpada[s]) <piso>']), ('s […]*

```diff
@@ -9,14 +9,15 @@
         "esta": "(est\u00e1|est\u00e3o|existe|existem)",
         "fecha": "(fecha|feche|fechar)",
         "juntar": "(junte|junta[r])",
         "ligar": "(liga[r]|ligue|acende[r]|acenda|ativa[r]|ative)",
         "muda": "(p\u00f5e|ponha|muda|mude|altera|coloca|deixa|p\u00f4r|mudar|alterar|colocar|deixar|definir|defina|setar)",
         "na_zona": "(n[o|a]|d[a|o]) {area}",
         "nome": "[(o[s]|a[s])] {name}",
+        "piso": "[do] [(piso|andar)] [de] {floor}",
         "por": "(p\u00f4r|p\u00f5e|ponha|definir|defina|setar)",
         "position": "{position}[[ ]%| por cento]",
         "qual": "(que|qual|qual \u00e9|quais)",
         "temperatura": "{temperature}[\u00b0| graus] [{temperature_unit}]",
         "volume": "{volume:volume_level}[[ ]%| por cento]",
         "zona": "[(o|os|a|as)] {area}"
     },
@@ -239,14 +240,23 @@
                     "slots": {
                         "area": "all",
                         "domain": "light",
                         "name": "all"
                     }
                 },
                 {
+                    "response": "lights_floor",
+                    "sentences": [
+                        "<desligar> [tod[a|o]s] [(o[s]| a[s])] (luz[es]| l\u00e2mpada[s]) <piso>"
+                    ],
+                    "slots": {
+                        "domain": "light"
+                    }
+                },
+                {
                     "response": "cover",
                     "sentences": [
                         "<fecha> [(o | a)] [(porta | port\u00e3o) da] garagem"
                     ],
                     "slots": {
                         "device_class": "garage",
                         "domain": "cover"
@@ -309,14 +319,23 @@
                     "slots": {
                         "area": "all",
                         "domain": "light",
                         "name": "all"
                     }
                 },
                 {
+                    "response": "lights_floor",
+                    "sentences": [
+                        "<ligar> [tod[a|o]s] [(o[s]| a[s])] (luz[es]| l\u00e2mpada[s]) <piso>"
+                    ],
+                    "slots": {
+                        "domain": "light"
+                    }
+                },
+                {
                     "response": "fans_area",
                     "sentences": [
                         "<ligar> todos os ventiladores <na_zona>"
                     ],
                     "slots": {
                         "domain": "fan",
                         "name": "all"
@@ -628,28 +647,36 @@
             }
         }
     },
     "responses": {
         "errors": {
             "duplicate_entities": "Desculpe, h\u00e1 v\u00e1rios dispositivos chamados {{ entity }}",
             "duplicate_entities_in_area": "Desculpe, h\u00e1 v\u00e1rios dispositivos chamados {{ entity }} na \u00e1rea {{ area }}",
+            "duplicate_entities_in_floor": "Desculpe, existem v\u00e1rios dispositivos chamados {{ entity }} no piso {{ floor }}.",
             "handle_error": "Um erro inesperado ocorreu ao processar o pedido",
             "no_area": "N\u00e3o existe nenhuma \u00e1rea chamada {{ area }}",
             "no_device_class": "Desculpe, eu n\u00e3o conhe\u00e7o nenhuma {{ device_class }}",
             "no_device_class_exposed": "Desculpe, nenhuma {{ device_class }} est\u00e1 exposta",
             "no_device_class_in_area": "{{ area }} n\u00e3o cont\u00e9m {{ device_class }}",
             "no_device_class_in_area_exposed": "Desculpe, nenhuma {{ device_class }} na \u00e1rea {{ area }} est\u00e1 exposta",
+            "no_device_class_in_floor": "Desculpe, n\u00e3o existe nenhum(a) {{ device_class }} no piso {{ floor }}.",
+            "no_device_class_in_floor_exposed": "Desculpe, nenhum(a) {{ device_class }} no piso {{ floor }} est\u00e1 exposto.",
             "no_domain": "Desculpe, eu n\u00e3o conhe\u00e7o nenhum {{ domain }}",
             "no_domain_exposed": "Desculpe, nenhum {{ domain }} est\u00e1 exposto",
             "no_domain_in_area": "{{ area }} n\u00e3o contem {{ domain }}",
             "no_domain_in_area_exposed": "Desculpe, nenhum {{ domain }} na \u00e1rea {{ area }} est\u00e1 exposto",
+            "no_domain_in_floor": "Desculpe, n\u00e3o existe nenhum(a) {{ domain }} no piso {{ floor }}.",
+            "no_domain_in_floor_exposed": "Desculpe, nenhum(a) {{ domain }} no piso {{ floor }} est\u00e1 exposto.",
             "no_entity": "N\u00e3o existe nenhum dispositivo ou entidade com o nome {{ entity }}",
             "no_entity_exposed": "Desculpe, {{ entity }} n\u00e3o est\u00e1 exposto",
             "no_entity_in_area": "Desculpe, eu n\u00e3o conhe\u00e7o nenhum dispositivo chamado {{ entity }} na \u00e1rea {{ area }}",
             "no_entity_in_area_exposed": "Desculpe, {{ entity }} na \u00e1rea {{ area }} n\u00e3o est\u00e1 exposto",
+            "no_entity_in_floor": "Desculpe, n\u00e3o existe nenhum dispositivo chamado {{ entity }} no piso {{ floor }}.",
+            "no_entity_in_floor_exposed": "Desculpe, {{ entity }} no piso {{ floor }} n\u00e3o est\u00e1 exposto.",
+            "no_floor": "Desculpe, n\u00e3o existe nenhum piso chamado {{ floor }}",
             "no_intent": "Desculpe, n\u00e3o consegui entender seu pedido"
         },
         "intents": {
             "HassClimateGetTemperature": {
                 "default": "{% set temperature = state_attr(state.entity_id, 'current_temperature') %} {% if (temperature | float) >= -1 and (temperature | float) <= 1  %} {{ temperature }} grau {% else: %} {{ temperature }} graus {% endif %}\n"
             },
             "HassGetState": {},
@@ -687,25 +714,27 @@
                 "cover": "Fechado",
                 "cover_device_class": "Fechado {{ slots.device_class }}",
                 "default": "{{ slots.name }} desligado",
                 "fan_all": "Todos ventiladores desligados",
                 "fans_area": "Ventiladores desligados",
                 "light_all": "Todas luzes apagadas",
                 "lights_area": "Luzes apagadas",
+                "lights_floor": "Luzes apagadas",
                 "lock": "Destrancado",
                 "valve": "Fechada"
             },
             "HassTurnOn": {
                 "cover": "Aberto",
                 "cover_device_class": "{{ slots.device_class }} aberto",
                 "default": "{{ slots.name }} ligado",
                 "fans_all": "Ligando todos ventiladores",
                 "fans_area": "Ligando ventiladores",
                 "light_all": "Acendendo todas luzes",
                 "lights_area": "Acendendo luzes",
+                "lights_floor": "Acendendo luzes",
                 "lock": "Trancado",
                 "scene": "Ativando cena {{slots.name}}",
                 "script": "Iniciado {{slots.name}}",
                 "valve": "Aberta"
             },
             "HassVacuumReturnToBase": {
                 "default": "Retornando"
```

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/data/pt.json` & `home-assistant-intents-2024.5.28/home_assistant_intents/data/pt.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9799396494708995%*

 * *Differences: {"'intents'": "{'HassTurnOff': {'data': {4: {'sentences': ['<fecha>  [as|os|a|o] "*

 * *              '[(cortina|cortinas|cortinado|cortinados|estore|estores|persiana|persianas)] '*

 * *              "<na_zona>']}, insert: [(2, OrderedDict([('sentences', ['<desliga> [(o | os | a | "*

 * *              "as)] (luz | luzes | candeeiro | candeeiros)', '<desliga> [(todas | todos)] [(o | os "*

 * *              "| a | as)] (luz | luzes | candeeiro | candeeiros) aqui']), ('slots', "*

 * *              "OrderedDict([('domain', 'light')])), […]*

```diff
@@ -261,27 +261,41 @@
                         "<desliga> [(todas | todos)] [(o | os | a | as)] (luz | luzes | candeeiro | candeeiros) <na_zona>"
                     ],
                     "slots": {
                         "domain": "light"
                     }
                 },
                 {
+                    "requires_context": {
+                        "area": {
+                            "slot": true
+                        }
+                    },
+                    "sentences": [
+                        "<desliga> [(o | os | a | as)] (luz | luzes | candeeiro | candeeiros)",
+                        "<desliga> [(todas | todos)] [(o | os | a | as)] (luz | luzes | candeeiro | candeeiros) aqui"
+                    ],
+                    "slots": {
+                        "domain": "light"
+                    }
+                },
+                {
                     "response": "cover",
                     "sentences": [
                         "<fecha> [(o | a)] [(porta | port\u00e3o) da] garagem"
                     ],
                     "slots": {
                         "device_class": "garage",
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "cover",
                     "sentences": [
-                        "<fecha> [as | os] [(cortinas | cortinados | estores | persianas)] <na_zona>"
+                        "<fecha>  [as|os|a|o] [(cortina|cortinas|cortinado|cortinados|estore|estores|persiana|persianas)] <na_zona>"
                     ],
                     "slots": {
                         "device_class": [
                             "blind",
                             "curtain",
                             "shutter"
                         ],
@@ -307,14 +321,28 @@
                         "<liga> [(todas | todos)] [(o | os | a | as)] (luz | luzes | candeeiro | candeeiros) <na_zona>"
                     ],
                     "slots": {
                         "domain": "light"
                     }
                 },
                 {
+                    "requires_context": {
+                        "area": {
+                            "slot": true
+                        }
+                    },
+                    "sentences": [
+                        "<liga> [(o | os | a | as)] (luz | luzes | candeeiro | candeeiros)",
+                        "<liga> [(todas | todos)] [(o | os | a | as)] (luz | luzes | candeeiro | candeeiros) aqui"
+                    ],
+                    "slots": {
+                        "domain": "light"
+                    }
+                },
+                {
                     "response": "fans_area",
                     "sentences": [
                         "(liga | ligue | ligar) [todas] as ventoinhas <na_zona>"
                     ],
                     "slots": {
                         "domain": "fan",
                         "name": "all"
@@ -324,15 +352,16 @@
                     "excludes_context": {
                         "domain": [
                             "binary_sensor",
                             "cover",
                             "lock",
                             "scene",
                             "script",
-                            "sensor"
+                            "sensor",
+                            "vacuum"
                         ]
                     },
                     "sentences": [
                         "<liga> [a[s]|o[s]] [luz[es]|interruptor[es]] [do|da] <nome>"
                     ]
                 },
                 {
@@ -344,26 +373,50 @@
                         "device_class": "garage",
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "cover",
                     "sentences": [
-                        "<abre>  [as|os] [(cortinas | cortinados | estores | persianas)] <na_zona>"
+                        "<abre>  [as|os|a|o] [(cortina|cortinas|cortinado|cortinados|estore|estores|persiana|persianas)] <na_zona>"
                     ],
                     "slots": {
                         "device_class": [
                             "blind",
                             "curtain",
                             "shutter"
                         ],
                         "domain": "cover"
                     }
                 }
             ]
+        },
+        "HassVacuumReturnToBase": {
+            "data": [
+                {
+                    "requires_context": {
+                        "domain": "vacuum"
+                    },
+                    "sentences": [
+                        "(retornar|voltar) <nome> [(a|\u00e0|para a) base]"
+                    ]
+                }
+            ]
+        },
+        "HassVacuumStart": {
+            "data": [
+                {
+                    "requires_context": {
+                        "domain": "vacuum"
+                    },
+                    "sentences": [
+                        "(come\u00e7ar|iniciar|ligar) <nome>"
+                    ]
+                }
+            ]
         }
     },
     "language": "pt",
     "lists": {
         "brightness": {
             "range": {
                 "from": 0,
@@ -622,14 +675,20 @@
                 "cover": "Aberto",
                 "cover_device_class": "{{ slots.device_class }} aberto",
                 "default": "Ligado",
                 "fans_area": "Ventoinhas ligadas",
                 "lights_area": "Luzes ligados",
                 "scene": "Ativado",
                 "script": "Iniciado"
+            },
+            "HassVacuumReturnToBase": {
+                "default": "A regressar"
+            },
+            "HassVacuumStart": {
+                "default": "Limpeza iniciada"
             }
         }
     },
     "skip_words": [
         "por favor",
         "se faz favor",
         "pode",
```

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/data/ro.json` & `home-assistant-intents-2024.5.28/home_assistant_intents/data/ro.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/data/ru.json` & `home-assistant-intents-2024.5.28/home_assistant_intents/data/ru.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9979974934402017%*

 * *Differences: {"'intents'": "{'HassTurnOff': {'data': {3: {'sentences': {delete: [3, 2]}}, 4: {'sentences': "*

 * *              "['<turn_off> [весь] свет [здесь|в (комнате|помещении)]', '<turn_off> [здесь|в "*

 * *              "(комнате|помещении)] [весь] свет']}, insert: [(2, OrderedDict([('sentences', "*

 * *              "['<turn_off> (<area> <name>|<name> <area>)']), ('requires_context', "*

 * *              "OrderedDict([('domain', 'light')]))])), (5, OrderedDict([('sentences', ['<turn_off> "*

 * *              "[весь] свет (дома|в (доме| […]*

```diff
@@ -2200,15 +2200,15 @@
                 }
             ]
         },
         "HassGetWeather": {
             "data": [
                 {
                     "sentences": [
-                        "[\u041a\u0430\u043a\u0430\u044f] \u043f\u043e\u0433\u043e\u0434\u0430"
+                        "[\u041a\u0430\u043a\u0430\u044f ][\u0441\u0435\u0439\u0447\u0430\u0441 ] \u043f\u043e\u0433\u043e\u0434\u0430"
                     ]
                 },
                 {
                     "requires_context": {
                         "domain": "weather"
                     },
                     "sentences": [
@@ -2366,36 +2366,51 @@
                     "response": "cover",
                     "sentences": [
                         "<close> <name>",
                         "<close> <name> <area>"
                     ]
                 },
                 {
+                    "requires_context": {
+                        "domain": "light"
+                    },
+                    "sentences": [
+                        "<turn_off> (<area> <name>|<name> <area>)"
+                    ]
+                },
+                {
                     "response": "lights_area",
                     "sentences": [
                         "<turn_off> [\u0432\u0435\u0441\u044c] \u0441\u0432\u0435\u0442 <area>",
-                        "<turn_off> <area> [\u0432\u0435\u0441\u044c] \u0441\u0432\u0435\u0442",
-                        "<turn_off> <area> <name>",
-                        "<turn_off> <name> <area>"
+                        "<turn_off> <area> [\u0432\u0435\u0441\u044c] \u0441\u0432\u0435\u0442"
                     ],
                     "slots": {
                         "domain": "light"
                     }
                 },
                 {
                     "requires_context": {
                         "area": {
                             "slot": true
                         }
                     },
                     "response": "lights_area",
                     "sentences": [
-                        "<turn_off> \u0432\u0435\u0441\u044c \u0441\u0432\u0435\u0442",
-                        "<turn_off> [\u0432\u0435\u0441\u044c] \u0441\u0432\u0435\u0442 \u0437\u0434\u0435\u0441\u044c",
-                        "<turn_off> \u0437\u0434\u0435\u0441\u044c [\u0432\u0435\u0441\u044c] \u0441\u0432\u0435\u0442"
+                        "<turn_off> [\u0432\u0435\u0441\u044c] \u0441\u0432\u0435\u0442 [\u0437\u0434\u0435\u0441\u044c|\u0432 (\u043a\u043e\u043c\u043d\u0430\u0442\u0435|\u043f\u043e\u043c\u0435\u0449\u0435\u043d\u0438\u0438)]",
+                        "<turn_off> [\u0437\u0434\u0435\u0441\u044c|\u0432 (\u043a\u043e\u043c\u043d\u0430\u0442\u0435|\u043f\u043e\u043c\u0435\u0449\u0435\u043d\u0438\u0438)] [\u0432\u0435\u0441\u044c] \u0441\u0432\u0435\u0442"
+                    ],
+                    "slots": {
+                        "domain": "light"
+                    }
+                },
+                {
+                    "response": "light_all",
+                    "sentences": [
+                        "<turn_off> [\u0432\u0435\u0441\u044c] \u0441\u0432\u0435\u0442 (\u0434\u043e\u043c\u0430|\u0432 (\u0434\u043e\u043c\u0435|\u043a\u0432\u0430\u0440\u0442\u0438\u0440\u0435))",
+                        "<turn_off> (\u0434\u043e\u043c\u0430|\u0432 (\u0434\u043e\u043c\u0435|\u043a\u0432\u0430\u0440\u0442\u0438\u0440\u0435)) [\u0432\u0435\u0441\u044c] \u0441\u0432\u0435\u0442"
                     ],
                     "slots": {
                         "domain": "light"
                     }
                 },
                 {
                     "response": "cover_device_class",
@@ -2435,14 +2450,22 @@
                     }
                 }
             ]
         },
         "HassTurnOn": {
             "data": [
                 {
+                    "requires_context": {
+                        "domain": "light"
+                    },
+                    "sentences": [
+                        "<turn_on> (<area> <name>|<name> <area>)"
+                    ]
+                },
+                {
                     "response": "lights_area",
                     "sentences": [
                         "<turn_on> [\u0432\u0435\u0441\u044c] \u0441\u0432\u0435\u0442 <area>",
                         "<turn_on> <area> [\u0432\u0435\u0441\u044c] \u0441\u0432\u0435\u0442"
                     ],
                     "slots": {
                         "domain": "light"
@@ -2452,16 +2475,26 @@
                     "requires_context": {
                         "area": {
                             "slot": true
                         }
                     },
                     "response": "lights_area",
                     "sentences": [
-                        "<turn_on> \u0441\u0432\u0435\u0442 [\u0437\u0434\u0435\u0441\u044c]",
-                        "<turn_on> [\u0437\u0434\u0435\u0441\u044c] \u0441\u0432\u0435\u0442"
+                        "<turn_on> [\u0432\u0435\u0441\u044c] \u0441\u0432\u0435\u0442 [\u0437\u0434\u0435\u0441\u044c|\u0432 (\u043a\u043e\u043c\u043d\u0430\u0442\u0435|\u043f\u043e\u043c\u0435\u0449\u0435\u043d\u0438\u0438)]",
+                        "<turn_on> [\u0437\u0434\u0435\u0441\u044c|\u0432 (\u043a\u043e\u043c\u043d\u0430\u0442\u0435|\u043f\u043e\u043c\u0435\u0449\u0435\u043d\u0438\u0438)] [\u0432\u0435\u0441\u044c] \u0441\u0432\u0435\u0442"
+                    ],
+                    "slots": {
+                        "domain": "light"
+                    }
+                },
+                {
+                    "response": "light_all",
+                    "sentences": [
+                        "<turn_on> [\u0432\u0435\u0441\u044c] \u0441\u0432\u0435\u0442 (\u0434\u043e\u043c\u0430|\u0432 (\u0434\u043e\u043c\u0435|\u043a\u0432\u0430\u0440\u0442\u0438\u0440\u0435))",
+                        "<turn_on> (\u0434\u043e\u043c\u0430|\u0432 (\u0434\u043e\u043c\u0435|\u043a\u0432\u0430\u0440\u0442\u0438\u0440\u0435)) [\u0432\u0435\u0441\u044c] \u0441\u0432\u0435\u0442"
                     ],
                     "slots": {
                         "domain": "light"
                     }
                 },
                 {
                     "response": "fans_area",
@@ -3055,15 +3088,15 @@
                 "one": "{{ slots.name | capitalize }} {{ state.state_with_unit }}\n",
                 "one_yesno": "{% if query.matched %}\n  \u0414\u0430\n{% else %}\n  \u041d\u0435\u0442, {{ state.state_with_unit }}\n{% endif %}\n",
                 "sensor_value": "\u0422\u0435\u043a\u0443\u0449\u0435\u0435 \u0437\u043d\u0430\u0447\u0435\u043d\u0438\u0435: {{ state.state_with_unit }}\n",
                 "sensor_value_temperature": "\u0422\u0435\u043c\u043f\u0435\u0440\u0430\u0442\u0443\u0440\u0430 {{ state.state_with_unit }}\n",
                 "which": "{% if not query.matched %}\n  \u041d\u0438\u043a\u0430\u043a\u0438\u0435\n{% else: %}\n  {% set match = query.matched | map(attribute=\"name\") | sort | list %}\n  {% if match | length > 4 %}\n    {{ match[:3] | join(\", \") }} \u0438 \u0435\u0449\u0451 {{ (match | length - 3) }}\n  {% else %}\n    {%- for name in match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} \u0438 {% endif -%}\n      {{ name }}\n    {%- endfor -%}\n  {% endif %}\n{% endif %}\n"
             },
             "HassGetWeather": {
-                "default": "{% set weather_condition = {\n  'clear': ', \u044f\u0441\u043d\u043e',\n  'clear-night': ', \u044f\u0441\u043d\u0430\u044f \u043d\u043e\u0447\u044c',\n  'cloudy': ', \u043e\u0431\u043b\u0430\u0447\u043d\u043e',\n  'exceptional': ', \u044d\u043a\u0441\u0442\u0440\u0435\u043c\u0430\u043b\u044c\u043d\u044b\u0435 \u043f\u043e\u0433\u043e\u0434\u043d\u044b\u0435 \u044f\u0432\u043b\u0435\u043d\u0438\u044f',\n  'fog': ', \u0442\u0443\u043c\u0430\u043d',\n  'hail': ', \u0433\u0440\u0430\u0434',\n  'lightning': ', \u0433\u0440\u043e\u0437\u0430',\n  'lightning-rainy': ', \u0434\u043e\u0436\u0434\u044c \u0441 \u0433\u0440\u043e\u0437\u043e\u0439',\n  'partlycloudy': ', \u0447\u0430\u0441\u0442\u0438\u0447\u043d\u0430\u044f \u043e\u0431\u043b\u0430\u0447\u043d\u043e\u0441\u0442\u044c',\n  'pouring': ', \u043b\u0438\u0432\u0435\u043d\u044c',\n  'rainy': ', \u0434\u043e\u0436\u0434\u044c',\n  'snowy': ', \u0441\u043d\u0435\u0433',\n  'snowy-rainy': ', \u043c\u043e\u043a\u0440\u044b\u0439 \u0441\u043d\u0435\u0433',\n  'sunny': ', \u0441\u043e\u043b\u043d\u0435\u0447\u043d\u043e',\n  'windy': ', \u0432\u0435\u0442\u0440\u0435\u043d\u043d\u043e',\n  'windy-variant': ', \u0432\u0435\u0442\u0440\u0435\u043d\u043d\u043e \u0438 \u043e\u0431\u043b\u0430\u0447\u043d\u043e'\n} %}\n\n\n{% set temperature = state.attributes.get('temperature') | float %} {% if temperature < 0 %}\n  {% set temperature_string = '\u043c\u0438\u043d\u0443\u0441 ' ~ (temperature * -1) | string | replace('.', ',') %}\n{% else %}\n  {% set temperature_string = temperature | string | replace('.', ',') %}\n{% endif %} {{ temperature_string }} {{ state.attributes.get('temperature_unit') }}{{ weather_condition.get((state.state | string).lower(), state.state | string) }}\n"
+                "default": "{% set weather_condition = {\n  'clear': ', \u044f\u0441\u043d\u043e',\n  'clear-night': ', \u044f\u0441\u043d\u0430\u044f \u043d\u043e\u0447\u044c',\n  'cloudy': ', \u043e\u0431\u043b\u0430\u0447\u043d\u043e',\n  'exceptional': ', \u044d\u043a\u0441\u0442\u0440\u0435\u043c\u0430\u043b\u044c\u043d\u044b\u0435 \u043f\u043e\u0433\u043e\u0434\u043d\u044b\u0435 \u044f\u0432\u043b\u0435\u043d\u0438\u044f',\n  'fog': ', \u0442\u0443\u043c\u0430\u043d',\n  'hail': ', \u0433\u0440\u0430\u0434',\n  'lightning': ', \u0433\u0440\u043e\u0437\u0430',\n  'lightning-rainy': ', \u0434\u043e\u0436\u0434\u044c \u0441 \u0433\u0440\u043e\u0437\u043e\u0439',\n  'partlycloudy': ', \u0447\u0430\u0441\u0442\u0438\u0447\u043d\u0430\u044f \u043e\u0431\u043b\u0430\u0447\u043d\u043e\u0441\u0442\u044c',\n  'pouring': ', \u043b\u0438\u0432\u0435\u043d\u044c',\n  'rainy': ', \u0434\u043e\u0436\u0434\u044c',\n  'snowy': ', \u0441\u043d\u0435\u0433',\n  'snowy-rainy': ', \u043c\u043e\u043a\u0440\u044b\u0439 \u0441\u043d\u0435\u0433',\n  'sunny': ', \u0441\u043e\u043b\u043d\u0435\u0447\u043d\u043e',\n  'windy': ', \u0432\u0435\u0442\u0440\u0435\u043d\u043d\u043e',\n  'windy-variant': ', \u0432\u0435\u0442\u0440\u0435\u043d\u043d\u043e \u0438 \u043e\u0431\u043b\u0430\u0447\u043d\u043e'\n} %}\n\n  {% set temperature = state.attributes.get('temperature') | float %}\n  {% if temperature.is_integer() %}\n      {% if temperature == 0 %}\n        {% set temperature_string = 0 | string %}\n      {% elif temperature < 0 %}\n        {% set temperature_string = '\u043c\u0438\u043d\u0443\u0441 ' ~ (temperature | abs | int ) | string %}\n      {% else %}\n        {% set temperature_string = '\u043f\u043b\u044e\u0441 ' ~ (temperature | int) | string %}\n      {% endif %}\n  {% else %}\n      {% if temperature < 0 %}\n        {% set temperature_string = '\u043c\u0438\u043d\u0443\u0441 ' ~ (temperature | abs) | string | replace('.', ',') %}\n      {% else %}\n        {% set temperature_string = '\u043f\u043b\u044e\u0441 ' ~ temperature | string | replace('.', ',') %}\n      {% endif %}\n  {% endif %}\n\n{{ \"\u0421\u0435\u0439\u0447\u0430\u0441 \" ~ temperature_string}}{{ weather_condition.get((state.state | string).lower(), state.state | string) }}\n"
             },
             "HassLightSet": {
                 "brightness": "\u042f\u0440\u043a\u043e\u0441\u0442\u044c {{ slots.name }} \u0443\u0441\u0442\u0430\u043d\u043e\u0432\u043b\u0435\u043d\u0430 \u043d\u0430 {{ slots.brightness }}",
                 "brightness_area": "\u042f\u0440\u043a\u043e\u0441\u0442\u044c \u0432 {{ slots.area }} \u0443\u0441\u0442\u0430\u043d\u043e\u0432\u043b\u0435\u043d\u0430 \u043d\u0430 {{ slots.brightness }}",
                 "color": "\u0426\u0432\u0435\u0442 {{ slots.name }} \u0443\u0441\u0442\u0430\u043d\u043e\u0432\u043b\u0435\u043d \u043d\u0430 {{ slots.color }}",
                 "color_area": "\u0426\u0432\u0435\u0442 \u0432 {{ slots.area }} \u0443\u0441\u0442\u0430\u043d\u043e\u0432\u043b\u0435\u043d \u043d\u0430 {{ slots.color }}"
             },
@@ -3082,27 +3115,29 @@
             "HassSetVolume": {
                 "default": "\u0413\u0440\u043e\u043c\u043a\u043e\u0441\u0442\u044c \u0437\u0430\u0434\u0430\u043d\u0430"
             },
             "HassShoppingListAddItem": {
                 "item_added": "\u0414\u043e\u0431\u0430\u0432\u043b\u044f\u044e {{ slots.item }}"
             },
             "HassTurnOff": {
-                "cover": "{% set Female_ending = \"\u0430\u0443\u044f\u044c\" %}\n{% set Neuter_ending = \"\u043e\u0435\" %}\n{% set Plural_ending = \"\u044b\u0438\" %}\n{% set last_letter = slots.name[-1].lower() %}\n{% if slots.name.lower() == \"\u0432\u043e\u0440\u043e\u0442\u0430\" %}\n  {% set ender = \"\u044b\" %}\n{% elif last_letter in Female_ending %}\n  {% set ender = \"\u0430\" %}\n{% elif last_letter in Neuter_ending%}\n  {% set ender = \"\u043e\" %}\n{% elif last_letter in Plural_ending%}\n  {% set ender = \"\u044b\" %}\n{% else %}\n  {% set ender = \"\" %}\n{% endif %}\n{{ slots.name }} \u0437\u0430\u043a\u0440\u044b\u0442{{ ender }}\n",
+                "cover": "{% set female_ending = \"\u0430\" %}\n{% set neuter_ending = \"\u043e\" %}\n{% set male_ending = \"\" %}\n{% set plural_ending = \"\u044b\" %}\n{% if slots.name.lower() == \"\u0432\u043e\u0440\u043e\u0442\u0430\" %}\n  {% set ender = plural_ending %}\n{% elif slots.name[-1].lower() in \"\u044c\" %}\n  {% if (slots.name.lower() in \"\u0432\u044b\u043a\u043b\u044e\u0447\u0430\u0442\u0435\u043b\u044c, \u043f\u043e\u043b\u044c\u0437\u043e\u0432\u0430\u0442\u0435\u043b\u044c, \u0434\u0435\u043d\u044c, \u0434\u043e\u0436\u0434\u044c, \u0434\u0432\u0438\u0433\u0430\u0442\u0435\u043b\u044c, \u043f\u0443\u0442\u044c\") or\n        (slots.name[-2].lower() in \"\u0440\u044c\") %}\n    {% set ending = male_ending %}\n  {% else %}\n    {% set ending = female_ending %}\n  {% endif %}\n{% elif slots.name[-1].lower() in \"\u0430, \u0443, \u044f\" %}\n  {% set ending = female_ending %}\n{% elif slots.name[-1].lower() in \"\u043e, \u0435\" %}\n  {% set ending = neuter_ending %}\n{% elif slots.name[-1].lower() in \"\u044b, \u0438\"%}\n  {% set ending = plural_ending %}\n{% else %}\n  {% set ending = male_ending %}\n{% endif %}\n{{ slots.name ~ \" \u0437\u0430\u043a\u0440\u044b\u0442\" ~ ending }}\n",
                 "cover_area": "\u0417\u0430\u043a\u0440\u044b\u0442\u0438\u0435 \u0432 {{ slots.area }} \u0432\u044b\u043f\u043e\u043b\u043d\u0435\u043d\u043e",
                 "cover_device_class": "\u0417\u0430\u043a\u0440\u044b\u0442\u0438\u0435 \u0432\u044b\u043f\u043e\u043b\u043d\u0435\u043d\u043e",
-                "default": "{% set Female_ending = \"\u0430\u0443\u044f\u044c\" %}\n{% set Neuter_ending = \"\u043e\u0435\" %}\n{% set Plural_ending = \"\u044b\u0438\" %}\n{% set last_letter = slots.name[-1].lower() %}\n{% if last_letter in Female_ending %}\n  {% set ender = \"\u0430\" %}\n{% elif last_letter in Neuter_ending%}\n  {% set ender = \"\u043e\" %}\n{% elif last_letter in Plural_ending%}\n  {% set ender = \"\u044b\" %}\n{% else %}\n  {% set ender = \"\" %}\n{% endif %}\n{{ slots.name }} \u0432\u044b\u043a\u043b\u044e\u0447\u0435\u043d{{ ender }}\n",
+                "default": "{% set female_ending = \"\u0430\" %}\n{% set neuter_ending = \"\u043e\" %}\n{% set male_ending = \"\" %}\n{% set plural_ending = \"\u044b\" %}\n{% if slots.name[-1].lower() in \"\u044c\" %}\n  {% if (slots.name.lower() in \"\u0432\u044b\u043a\u043b\u044e\u0447\u0430\u0442\u0435\u043b\u044c, \u043f\u043e\u043b\u044c\u0437\u043e\u0432\u0430\u0442\u0435\u043b\u044c, \u0434\u0435\u043d\u044c, \u0434\u043e\u0436\u0434\u044c, \u0434\u0432\u0438\u0433\u0430\u0442\u0435\u043b\u044c, \u043f\u0443\u0442\u044c\") or\n        (slots.name[-2].lower() in \"\u0440\u044c\") %}\n    {% set ending = male_ending %}\n  {% else %}\n    {% set ending = female_ending %}\n  {% endif %}\n{% elif slots.name[-1].lower() in \"\u0430, \u0443, \u044f\" %}\n  {% set ending = female_ending %}\n{% elif slots.name[-1].lower() in \"\u043e, \u0435\" %}\n  {% set ending = neuter_ending %}\n{% elif slots.name[-1].lower() in \"\u044b, \u0438\"%}\n  {% set ending = plural_ending %}\n{% else %}\n  {% set ending = male_ending %}\n{% endif %}\n{{ slots.name ~ \" \u0432\u044b\u043a\u043b\u044e\u0447\u0435\u043d\" ~ ending }}\n",
                 "fans_area": "\u0412\u0435\u043d\u0442\u0438\u043b\u044f\u0442\u043e\u0440\u044b \u0432\u044b\u043a\u043b\u044e\u0447\u0435\u043d\u044b \u0432 {{ slots.area }}",
+                "light_all": "\u0412\u0435\u0441\u044c \u0441\u0432\u0435\u0442 \u0432\u044b\u043a\u043b\u044e\u0447\u0435\u043d",
                 "lights_area": "\u0421\u0432\u0435\u0442 \u0432 {{ slots.area }} \u0432\u044b\u043a\u043b\u044e\u0447\u0435\u043d"
             },
             "HassTurnOn": {
-                "cover": "{% set Female_ending = \"\u0430\u0443\u044f\u044c\" %}\n{% set Neuter_ending = \"\u043e\u0435\" %}\n{% set Plural_ending = \"\u044b\u0438\" %}\n{% set last_letter = slots.name[-1].lower() %}\n{% if slots.name.lower() == \"\u0432\u043e\u0440\u043e\u0442\u0430\" %}\n  {% set ender = \"\u044b\" %}\n{% elif last_letter in Female_ending %}\n  {% set ender = \"\u0430\" %}\n{% elif last_letter in Neuter_ending%}\n  {% set ender = \"\u043e\" %}\n{% elif last_letter in Plural_ending%}\n  {% set ender = \"\u044b\" %}\n{% else %}\n  {% set ender = \"\" %}\n{% endif %}\n{{ slots.name }} \u043e\u0442\u043a\u0440\u044b\u0442{{ ender }}\n",
+                "cover": "{% set female_ending = \"\u0430\" %}\n{% set neuter_ending = \"\u043e\" %}\n{% set male_ending = \"\" %}\n{% set plural_ending = \"\u044b\" %}\n{% if slots.name.lower() == \"\u0432\u043e\u0440\u043e\u0442\u0430\" %}\n  {% set ender = plural_ending %}\n{% elif slots.name[-1].lower() in \"\u044c\" %}\n  {% if (slots.name.lower() in \"\u0432\u044b\u043a\u043b\u044e\u0447\u0430\u0442\u0435\u043b\u044c, \u043f\u043e\u043b\u044c\u0437\u043e\u0432\u0430\u0442\u0435\u043b\u044c, \u0434\u0435\u043d\u044c, \u0434\u043e\u0436\u0434\u044c, \u0434\u0432\u0438\u0433\u0430\u0442\u0435\u043b\u044c, \u043f\u0443\u0442\u044c\") or\n        (slots.name[-2].lower() in \"\u0440\u044c\") %}\n    {% set ending = male_ending %}\n  {% else %}\n    {% set ending = female_ending %}\n  {% endif %}\n{% elif slots.name[-1].lower() in \"\u0430, \u0443, \u044f\" %}\n  {% set ending = female_ending %}\n{% elif slots.name[-1].lower() in \"\u043e, \u0435\" %}\n  {% set ending = neuter_ending %}\n{% elif slots.name[-1].lower() in \"\u044b, \u0438\"%}\n  {% set ending = plural_ending %}\n{% else %}\n  {% set ending = male_ending %}\n{% endif %}\n{{ slots.name ~ \" \u043e\u0442\u043a\u0440\u044b\u0442\" ~ ending }}\n",
                 "cover_area": "\u041e\u0442\u043a\u0440\u044b\u0442\u0438\u0435 \u0432 {{ slots.area }} \u0432\u044b\u043f\u043e\u043b\u043d\u0435\u043d\u043e",
                 "cover_device_class": "\u041e\u0442\u043a\u0440\u044b\u0442\u0438\u0435 \u0432\u044b\u043f\u043e\u043b\u043d\u0435\u043d\u043e",
-                "default": "{% set Female_ending = \"\u0430\u0443\u044f\u044c\" %}\n{% set Neuter_ending = \"\u043e\u0435\" %}\n{% set Plural_ending = \"\u044b\u0438\" %}\n{% set last_letter = slots.name[-1].lower() %}\n{% if last_letter in Female_ending %}\n  {% set ender = \"\u0430\" %}\n{% elif last_letter in Neuter_ending%}\n  {% set ender = \"\u043e\" %}\n{% elif last_letter in Plural_ending%}\n  {% set ender = \"\u044b\" %}\n{% else %}\n  {% set ender = \"\" %}\n{% endif %}\n{{ slots.name }} \u0432\u043a\u043b\u044e\u0447\u0435\u043d{{ ender }}\n",
+                "default": "{% set female_ending = \"\u0430\" %}\n{% set neuter_ending = \"\u043e\" %}\n{% set male_ending = \"\" %}\n{% set plural_ending = \"\u044b\" %}\n{% if slots.name[-1].lower() in \"\u044c\" %}\n  {% if (slots.name.lower() in \"\u0432\u044b\u043a\u043b\u044e\u0447\u0430\u0442\u0435\u043b\u044c, \u043f\u043e\u043b\u044c\u0437\u043e\u0432\u0430\u0442\u0435\u043b\u044c, \u0434\u0435\u043d\u044c, \u0434\u043e\u0436\u0434\u044c, \u0434\u0432\u0438\u0433\u0430\u0442\u0435\u043b\u044c, \u043f\u0443\u0442\u044c\") or\n        (slots.name[-2].lower() in \"\u0440\u044c\") %}\n    {% set ending = male_ending %}\n  {% else %}\n    {% set ending = female_ending %}\n  {% endif %}\n{% elif slots.name[-1].lower() in \"\u0430, \u0443, \u044f\" %}\n  {% set ending = female_ending %}\n{% elif slots.name[-1].lower() in \"\u043e, \u0435\" %}\n  {% set ending = neuter_ending %}\n{% elif slots.name[-1].lower() in \"\u044b, \u0438\"%}\n  {% set ending = plural_ending %}\n{% else %}\n  {% set ending = male_ending %}\n{% endif %}\n{{ slots.name ~ \" \u0432\u043a\u043b\u044e\u0447\u0435\u043d\" ~ ending }}\n",
                 "fans_area": "\u0412\u043a\u043b\u044e\u0447\u0435\u043d\u044b \u0432\u0435\u043d\u0442\u0438\u043b\u044f\u0442\u043e\u0440\u044b \u0432 {{ slots.area }}",
+                "light_all": "\u0412\u0435\u0441\u044c \u0441\u0432\u0435\u0442 \u0432\u043a\u043b\u044e\u0447\u0435\u043d",
                 "lights_area": "\u0421\u0432\u0435\u0442 \u0432 {{ slots.area }} \u0432\u043a\u043b\u044e\u0447\u0435\u043d",
                 "script": "\u0412\u044b\u043f\u043e\u043b\u043d\u0435\u043d\u043e"
             }
         }
     },
     "skip_words": [
         "\u043f\u043e\u0436\u0430\u043b\u0443\u0439\u0441\u0442\u0430",
```

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/data/sk.json` & `home-assistant-intents-2024.5.28/home_assistant_intents/data/sk.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/data/sl.json` & `home-assistant-intents-2024.5.28/home_assistant_intents/data/sl.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/data/sr.json` & `home-assistant-intents-2024.5.28/home_assistant_intents/data/sr.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/data/sv.json` & `home-assistant-intents-2024.5.28/home_assistant_intents/data/sv.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9500210437710438%*

 * *Differences: {"'expansion_rules'": "{'volym': '{volume:volume_level}[[ ]%| procent]'}",*

 * * "'intents'": "{'HassGetWeather': OrderedDict([('data', [OrderedDict([('sentences', ['hur (är|ser) "*

 * *              "vädret [ut]'])]), OrderedDict([('sentences', ['hur (är|ser) vädret [ut] i "*

 * *              "{name}']), ('requires_context', OrderedDict([('domain', 'weather')]))])])]), "*

 * *              "'HassMediaUnpause': OrderedDict([('data', [OrderedDict([('sentences', ['återuppta "*

 * *              "[på] <name>', 'fortsätt på <name>']), […]*

```diff
@@ -16,14 +16,15 @@
         "sl\u00e5_av": "(sl\u00e5 (av | fr\u00e5n | ifr\u00e5n) | sl\u00e4ck | st\u00e4ng [av] | stoppa)",
         "sl\u00e5_p\u00e5": "(t\u00e4nd | s\u00e4tt (p\u00e5 | ig\u00e5ng | fart p\u00e5) | sl\u00e5 (p\u00e5 | till) | starta)",
         "st\u00e4ng_gardiner": "(st\u00e4ng [igen | till]| dra (ner | igen | f\u00f6r | till ) | hissa ner | veckla (ner | igen) | tillslut) | sl\u00e5 (igen |ihop | f\u00f6r) | rulla ner",
         "temp": "(temperatur[en])",
         "temperature": "{temperature}[\u00b0| grader] [{temperature_unit}]",
         "vad": "(vad \u00e4r | vad \u00e4r det | vad \u00e4r det f\u00f6r | vilken)",
         "varmt_kallt": "(varmt | varm | kallt | kall | het | svalt )",
+        "volym": "{volume:volume_level}[[ ]%| procent]",
         "\u00e4ndra": "(st\u00e4ll in | s\u00e4tt | justera | \u00e4ndra | vrid (upp | ner))",
         "\u00e4r": "(\u00e4r det | \u00e4r)",
         "\u00f6ppna_gardiner": "(\u00f6ppna [upp] | dra (upp | bort | is\u00e4r | undan) | hissa upp | veckla upp | rulla upp)"
     },
     "intents": {
         "HassClimateGetTemperature": {
             "data": [
@@ -81,14 +82,31 @@
                     "response": "how_many",
                     "sentences": [
                         "hur m\u00e5nga {on_off_domains:domain} \u00e4r {on_off_states:state} [<i_p\u00e5> <area>]"
                     ]
                 }
             ]
         },
+        "HassGetWeather": {
+            "data": [
+                {
+                    "sentences": [
+                        "hur (\u00e4r|ser) v\u00e4dret [ut]"
+                    ]
+                },
+                {
+                    "requires_context": {
+                        "domain": "weather"
+                    },
+                    "sentences": [
+                        "hur (\u00e4r|ser) v\u00e4dret [ut] i {name}"
+                    ]
+                }
+            ]
+        },
         "HassLightSet": {
             "data": [
                 {
                     "response": "brightness",
                     "sentences": [
                         "[<dimra>] [upp | ner] <name> [<ljusintensitet>] till <brightness>",
                         "[<dimra>] [upp | ner] <name> till <brightness> [<ljusintensitet>]",
@@ -138,23 +156,73 @@
                     ],
                     "slots": {
                         "name": "all"
                     }
                 }
             ]
         },
+        "HassMediaNext": {
+            "data": [
+                {
+                    "requires_context": {
+                        "domain": "media_player"
+                    },
+                    "sentences": [
+                        "[spela ]n\u00e4sta [sp\u00e5r ] p\u00e5 <name>"
+                    ]
+                }
+            ]
+        },
+        "HassMediaPause": {
+            "data": [
+                {
+                    "requires_context": {
+                        "domain": "media_player"
+                    },
+                    "sentences": [
+                        "pausa <name>"
+                    ]
+                }
+            ]
+        },
+        "HassMediaUnpause": {
+            "data": [
+                {
+                    "requires_context": {
+                        "domain": "media_player"
+                    },
+                    "sentences": [
+                        "\u00e5teruppta [p\u00e5] <name>",
+                        "forts\u00e4tt p\u00e5 <name>"
+                    ]
+                }
+            ]
+        },
         "HassNevermind": {
             "data": [
                 {
                     "sentences": [
                         "gl\u00f6m det"
                     ]
                 }
             ]
         },
+        "HassSetVolume": {
+            "data": [
+                {
+                    "requires_context": {
+                        "domain": "media_player"
+                    },
+                    "sentences": [
+                        "s\u00e4tt volymen till <volym> p\u00e5 <name>",
+                        "(s\u00e4nk|\u00f6ka) volymen p\u00e5 <name> till <volym>"
+                    ]
+                }
+            ]
+        },
         "HassShoppingListAddItem": {
             "data": [
                 {
                     "expansion_rules": {
                         "item": "{shopping_list_item:item}",
                         "my_list": "[min ][ink\u00f6ps]lista[n]"
                     },
@@ -770,14 +838,21 @@
                 },
                 "fahrenheit",
                 {
                     "in": "f",
                     "out": "fahrenheit"
                 }
             ]
+        },
+        "volume": {
+            "range": {
+                "from": 0,
+                "to": 100,
+                "type": "percentage"
+            }
         }
     },
     "responses": {
         "errors": {
             "duplicate_entities": "Det finns flera enheter med namnet {{ entity }}",
             "duplicate_entities_in_area": "Det finns flera enheter med namnet {{ entity }} i {{ area }}",
             "handle_error": "Ett ov\u00e4ntat fel intr\u00e4ffade under utf\u00f6randet av avsikten",
@@ -804,20 +879,35 @@
                 "all": "{% if not query.unmatched: %}\n  Ja\n{% else %}\n  {% set no_match = query.unmatched | map(attribute=\"name\") | sort | list %}\n  {% if no_match | length > 4 %}\n    Nej, inte {{ no_match[:3] | join(\", \") }} och {{ (no_match | length - 3) }} fler\n  {%- else -%}\n    Nej, inte\n    {% for name in no_match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} och {% endif -%}\n      {{ name }}\n    {%- endfor %}\n  {% endif %}\n{% endif %}\n",
                 "any": "{% if query.matched %}\n  {% set match = query.matched | map(attribute=\"name\") | sort | list %}\n  {% if match | length > 4 %}\n    Ja, {{ match[:3] | join(\", \") }} och {{ (match | length - 3) }} fler\n  {%- else -%}\n    Ja,\n    {% for name in match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} och {% endif -%}\n      {{ name }}\n    {%- endfor -%}\n  {% endif %}\n{% else %}\n  Nej\n{% endif %}\n",
                 "how_many": "{{ query.matched | length }}\n",
                 "one": "{{ slots.name | capitalize }} \u00e4r {{ state.state_with_unit }}\n",
                 "one_yesno": "{% if query.matched %}\n  Ja\n{% else %}\n  Nej, den \u00e4r {{ state.state_with_unit }}\n{% endif %}\n",
                 "which": "{% if not query.matched %}\n  Inte n\u00e5gon\n{% else: %}\n  {% set match = query.matched | map(attribute=\"name\") | sort | list %}\n  {% if match | length > 4 %}\n    {{ match[:3] | join(\", \") }} och {{ (match | length - 3) }} fler\n  {% else %}\n    {%- for name in match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} och {% endif -%}\n      {{ name }}\n    {%- endfor -%}\n  {% endif %}\n{% endif %}\n"
             },
+            "HassGetWeather": {
+                "default": "{% set weather_condition = {\n  'clear': 'och klart',\n  'clear-night': 'och klart',\n  'cloudy': 'och mulet',\n  'exceptional': 'och str\u00e5lande solsken', \n  'fog': 'och dimma',\n  'hail': 'och hagel',\n  'lightning': 'och \u00e5ska',\n  'lightning-rainy': 'och \u00e5ska med regn',\n  'partlycloudy': 'och delvis mulet',\n  'pouring': 'och skyfall',\n  'rainy': 'och regn',\n  'snowy': 'och sn\u00f6',\n  'snowy-rainy': 'och sn\u00f6blandat regn',\n  'sunny': 'och sol',\n  'windy': 'och bl\u00e5st',\n  'windy-variant': 'och mulet med bl\u00e5st'\n} %} {{ state.attributes.get('temperature') }} {{ state.attributes.get('temperature_unit') }} {{ weather_condition.get((state.state | string).lower(), \"\") }}\n"
+            },
             "HassLightSet": {
                 "brightness": "{{ slots.name }} ljusstyrka sattes till {{ slots.brightness }}",
                 "brightness_area": "Ljusstyrkan i {{ slots.area }} sattes till {{ slots.brightness }}",
                 "color": "{{ slots.name }} f\u00e4rg sattes till {{ slots.color }}",
                 "color_area": "F\u00e4rgen p\u00e5 belysningen i {{ slots.area }} sattes till {{ slots.color }}"
             },
+            "HassMediaNext": {
+                "default": "Spelar n\u00e4sta"
+            },
+            "HassMediaPause": {
+                "default": "Pausad"
+            },
+            "HassMediaUnpause": {
+                "default": "\u00c5terupptar"
+            },
+            "HassSetVolume": {
+                "default": "Volym satt"
+            },
             "HassShoppingListAddItem": {
                 "item_added": "{{ slots.item | title }} tillagt"
             },
             "HassTurnOff": {
                 "cover": "St\u00e4ngde {{ slots.name }}",
                 "cover_area": "St\u00e4ngde i {{ slots.area }}",
                 "cover_device_class": "St\u00e4ngde {{ slots.device_class }}",
```

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/data/sw.json` & `home-assistant-intents-2024.5.28/home_assistant_intents/data/sw.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/data/te.json` & `home-assistant-intents-2024.5.28/home_assistant_intents/data/te.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/data/tr.json` & `home-assistant-intents-2024.5.28/home_assistant_intents/data/tr.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/data/uk.json` & `home-assistant-intents-2024.5.28/home_assistant_intents/data/uk.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9858761505180776%*

 * *Differences: {"'expansion_rules'": "{'floor': '[в|у|на] {floor}'}",*

 * * "'intents'": "{'HassTurnOff': {'data': {insert: [(2, OrderedDict([('sentences', ['<вимкни> [все] "*

 * *              "світло <floor>', '<вимкни> <floor> [все] світло']), ('response', 'lights_floor'), "*

 * *              "('slots', OrderedDict([('domain', 'light')]))]))]}}, 'HassTurnOn': {'data': "*

 * *              "{insert: [(1, OrderedDict([('sentences', ['<ввімкни> [все] світло <floor>', "*

 * *              "'<ввімкни> <floor> [все] світло']), ('response', 'lights_ […]*

```diff
@@ -1,11 +1,12 @@
 {
     "expansion_rules": {
         "area": "[\u0432|\u0443|\u043d\u0430] {area}",
         "brightness": "{brightness}[%| \u0432\u0456\u0434\u0441\u043e\u0442\u043a(\u0456\u0432|\u0430|\u0438)]",
+        "floor": "[\u0432|\u0443|\u043d\u0430] {floor}",
         "name": "{name}",
         "position": "{position}[[ ]%| \u0432\u0456\u0434\u0441\u043e\u0442\u043a(\u0456\u0432|\u0430|\u0438)]",
         "temperature": "{temperature} [\u0433\u0440\u0430\u0434\u0443\u0441(\u0456\u0432|\u0438|\u0430)] [{temperature_unit}]",
         "volume": "{volume:volume_level}[[ ]%| \u0432\u0456\u0434\u0441\u043e\u0442\u043a(\u0456\u0432|\u0430|\u0438)]",
         "\u0432\u0432\u0456\u043c\u043a\u043d\u0438": "(\u0432|\u0443)\u0432\u0456\u043c\u043a\u043d\u0438 | \u0432\u043a\u043b\u044e\u0447\u0438",
         "\u0432\u0438\u043c\u043a\u043d\u0438": "\u0432\u0438\u043c\u043a\u043d\u0438 | \u0432\u0438\u043a\u043b\u044e\u0447\u0438",
         "\u0432\u0456\u0434\u043a\u0440\u0438\u0439": "\u0432\u0456\u0434\u043a\u0440\u0438\u0439 | \u0440\u043e\u0437\u043a\u0440\u0438\u0439 | \u043f\u0456\u0434\u043d\u0456\u043c\u0438 | \u0432\u0456\u0434\u0447\u0438\u043d\u0438",
@@ -309,14 +310,24 @@
                         "<\u0432\u0438\u043c\u043a\u043d\u0438> <area> [\u0432\u0441\u0435] \u0441\u0432\u0456\u0442\u043b\u043e"
                     ],
                     "slots": {
                         "domain": "light"
                     }
                 },
                 {
+                    "response": "lights_floor",
+                    "sentences": [
+                        "<\u0432\u0438\u043c\u043a\u043d\u0438> [\u0432\u0441\u0435] \u0441\u0432\u0456\u0442\u043b\u043e <floor>",
+                        "<\u0432\u0438\u043c\u043a\u043d\u0438> <floor> [\u0432\u0441\u0435] \u0441\u0432\u0456\u0442\u043b\u043e"
+                    ],
+                    "slots": {
+                        "domain": "light"
+                    }
+                },
+                {
                     "response": "cover_device_class",
                     "sentences": [
                         "<\u0437\u0430\u043a\u0440\u0438\u0439> [\u0434\u0432\u0435\u0440\u0456] [\u0443|\u0432] \u0433\u0430\u0440\u0430\u0436[\u0430|\u0443|\u0456]",
                         "<\u0437\u0430\u043a\u0440\u0438\u0439> \u0433\u0430\u0440\u0430\u0436\u043d\u0456 \u0434\u0432\u0435\u0440\u0456"
                     ],
                     "slots": {
                         "device_class": "garage",
@@ -375,14 +386,24 @@
                         "<\u0432\u0432\u0456\u043c\u043a\u043d\u0438> <area> [\u0432\u0441\u0435] \u0441\u0432\u0456\u0442\u043b\u043e"
                     ],
                     "slots": {
                         "domain": "light"
                     }
                 },
                 {
+                    "response": "lights_floor",
+                    "sentences": [
+                        "<\u0432\u0432\u0456\u043c\u043a\u043d\u0438> [\u0432\u0441\u0435] \u0441\u0432\u0456\u0442\u043b\u043e <floor>",
+                        "<\u0432\u0432\u0456\u043c\u043a\u043d\u0438> <floor> [\u0432\u0441\u0435] \u0441\u0432\u0456\u0442\u043b\u043e"
+                    ],
+                    "slots": {
+                        "domain": "light"
+                    }
+                },
+                {
                     "response": "fans_area",
                     "sentences": [
                         "<\u0432\u0432\u0456\u043c\u043a\u043d\u0438> [\u0432\u0441\u0456] \u0432\u0435\u043d\u0442\u0438\u043b\u044f\u0442\u043e\u0440[\u0438] <area>",
                         "<\u0432\u0432\u0456\u043c\u043a\u043d\u0438> <area> [\u0432\u0441\u0456] \u0432\u0435\u043d\u0442\u0438\u043b\u044f\u0442\u043e\u0440[\u0438]",
                         "<\u0432\u0432\u0456\u043c\u043a\u043d\u0438> \u0432\u0435\u043d\u0442\u0438\u043b\u044f\u0446\u0456\u044e <area>",
                         "<\u0432\u0432\u0456\u043c\u043a\u043d\u0438> <area> \u0432\u0435\u043d\u0442\u0438\u043b\u044f\u0446\u0456\u044e"
                     ],
@@ -1028,28 +1049,36 @@
             }
         }
     },
     "responses": {
         "errors": {
             "duplicate_entities": "\u0412\u0438\u0431\u0430\u0447\u0442\u0435, \u0454 \u0434\u0435\u043a\u0456\u043b\u044c\u043a\u0430 \u043f\u0440\u0438\u0441\u0442\u0440\u043e\u0457\u0432 \u0437 \u043d\u0430\u0437\u0432\u043e\u044e {{ entity }}",
             "duplicate_entities_in_area": "\u0412\u0438\u0431\u0430\u0447\u0442\u0435, \u0454 \u0434\u0435\u043a\u0456\u043b\u044c\u043a\u0430 \u043f\u0440\u0438\u0441\u0442\u0440\u043e\u0457\u0432 \u0437 \u043d\u0430\u0437\u0432\u043e\u044e {{ entity }} \u0432 \u043f\u0440\u0438\u043c\u0456\u0449\u0435\u043d\u043d\u0456 {{ area }}",
+            "duplicate_entities_in_floor": "\u0412\u0438\u0431\u0430\u0447\u0442\u0435, \u0454 \u0434\u0435\u043a\u0456\u043b\u044c\u043a\u0430 \u043f\u0440\u0438\u0441\u0442\u0440\u043e\u0457\u0432 \u0437 \u043d\u0430\u0437\u0432\u043e\u044e {{ entity }} \u043d\u0430 {{ floor }} \u043f\u043e\u0432\u0435\u0440\u0441\u0456",
             "handle_error": "\u0412\u0438\u0431\u0430\u0447\u0442\u0435, \u043f\u0456\u0434 \u0447\u0430\u0441 \u0432\u0438\u043a\u043e\u043d\u0430\u043d\u043d\u044f \u0437\u0430\u043f\u0438\u0442\u0443 \u0432\u0438\u043d\u0438\u043a\u043b\u0430 \u043d\u0435\u043e\u0447\u0456\u043a\u0443\u0432\u0430\u043d\u0430 \u043f\u043e\u043c\u0438\u043b\u043a\u0430",
             "no_area": "\u0412\u0438\u0431\u0430\u0447\u0442\u0435, \u043c\u0435\u043d\u0456 \u043d\u0435 \u0432\u0456\u0434\u043e\u043c\u0435 \u043f\u0440\u0438\u043c\u0456\u0449\u0435\u043d\u043d\u044f \u0437 \u043d\u0430\u0437\u0432\u043e\u044e {{ area }}",
             "no_device_class": "\u0412\u0438\u0431\u0430\u0447\u0442\u0435, \u043c\u0435\u043d\u0456 \u043d\u0435 \u0432\u0456\u0434\u043e\u043c\u043e \u0436\u043e\u0434\u043d\u043e\u0433\u043e {{ device_class }}",
             "no_device_class_exposed": "\u0412\u0438\u0431\u0430\u0447\u0442\u0435, \u043d\u0435\u043c\u0430\u0454 \u0436\u043e\u0434\u043d\u043e\u0433\u043e \u0434\u043e\u0441\u0442\u0443\u043f\u043d\u043e\u0433\u043e {{ device_class }}",
             "no_device_class_in_area": "\u0412\u0438\u0431\u0430\u0447\u0442\u0435, \u043c\u0435\u043d\u0456 \u043d\u0435 \u0432\u0456\u0434\u043e\u043c\u043e \u0436\u043e\u0434\u043d\u043e\u0433\u043e {{ device_class }} \u0432 \u043f\u0440\u0438\u043c\u0456\u0449\u0435\u043d\u043d\u0456 {{ area }}",
             "no_device_class_in_area_exposed": "\u0412\u0438\u0431\u0430\u0447\u0442\u0435, \u043d\u0435\u043c\u0430\u0454 \u0436\u043e\u0434\u043d\u043e\u0433\u043e \u0434\u043e\u0441\u0442\u0443\u043f\u043d\u043e\u0433\u043e {{ device_class }} \u0432 \u043f\u0440\u0438\u043c\u0456\u0449\u0435\u043d\u043d\u0456 {{ area }}",
+            "no_device_class_in_floor": "\u0412\u0438\u0431\u0430\u0447\u0442\u0435, \u043c\u0435\u043d\u0456 \u043d\u0435 \u0432\u0456\u0434\u043e\u043c\u043e \u0436\u043e\u0434\u043d\u043e\u0433\u043e {{ device_class }} \u043d\u0430 {{ floor }} \u043f\u043e\u0432\u0435\u0440\u0441\u0456",
+            "no_device_class_in_floor_exposed": "\u0412\u0438\u0431\u0430\u0447\u0442\u0435, \u043d\u0435\u043c\u0430\u0454 \u0436\u043e\u0434\u043d\u043e\u0433\u043e \u0434\u043e\u0441\u0442\u0443\u043f\u043d\u043e\u0433\u043e {{ device_class }} \u043d\u0430 {{ floor }} \u043f\u043e\u0432\u0435\u0440\u0441\u0456",
             "no_domain": "\u0412\u0438\u0431\u0430\u0447\u0442\u0435, \u043c\u0435\u043d\u0456 \u043d\u0435 \u0432\u0456\u0434\u043e\u043c\u043e \u0436\u043e\u0434\u043d\u043e\u0433\u043e {{ domain }}",
             "no_domain_exposed": "\u0412\u0438\u0431\u0430\u0447\u0442\u0435, \u043d\u0435\u043c\u0430\u0454 \u0436\u043e\u0434\u043d\u043e\u0433\u043e \u0434\u043e\u0441\u0442\u0443\u043f\u043d\u043e\u0433\u043e {{ domain }}",
             "no_domain_in_area": "\u0412\u0438\u0431\u0430\u0447\u0442\u0435, \u043c\u0435\u043d\u0456 \u043d\u0435 \u0432\u0456\u0434\u043e\u043c\u043e \u0436\u043e\u0434\u043d\u043e\u0433\u043e {{ domain }} \u0432 \u043f\u0440\u0438\u043c\u0456\u0449\u0435\u043d\u043d\u0456 {{ area }}",
             "no_domain_in_area_exposed": "\u0412\u0438\u0431\u0430\u0447\u0442\u0435, \u043d\u0435\u043c\u0430\u0454 \u0436\u043e\u0434\u043d\u043e\u0433\u043e \u0434\u043e\u0441\u0442\u0443\u043f\u043d\u043e\u0433\u043e {{ domain }} \u0432 \u043f\u0440\u0438\u043c\u0456\u0449\u0435\u043d\u043d\u0456 {{ area }}",
+            "no_domain_in_floor": "\u0412\u0438\u0431\u0430\u0447\u0442\u0435, \u043c\u0435\u043d\u0456 \u043d\u0435 \u0432\u0456\u0434\u043e\u043c\u043e \u0436\u043e\u0434\u043d\u043e\u0433\u043e {{ domain }} \u043d\u0430 {{ floor }} \u043f\u043e\u0432\u0435\u0440\u0441\u0456",
+            "no_domain_in_floor_exposed": "\u0412\u0438\u0431\u0430\u0447\u0442\u0435, \u043d\u0435\u043c\u0430\u0454 \u0436\u043e\u0434\u043d\u043e\u0433\u043e \u0434\u043e\u0441\u0442\u0443\u043f\u043d\u043e\u0433\u043e {{ domain }} \u043d\u0430 {{ floor }} \u043f\u043e\u0432\u0435\u0440\u0441\u0456",
             "no_entity": "\u0412\u0438\u0431\u0430\u0447\u0442\u0435, \u043c\u0435\u043d\u0456 \u043d\u0435 \u0432\u0456\u0434\u043e\u043c\u043e \u043f\u0440\u0438\u0441\u0442\u0440\u043e\u044e \u0437 \u043d\u0430\u0437\u0432\u043e\u044e {{ entity }}",
             "no_entity_exposed": "\u0412\u0438\u0431\u0430\u0447\u0442\u0435, {{ entity }} \u043d\u0435 \u0454 \u0434\u043e\u0441\u0442\u0443\u043f\u043d\u0438\u043c",
             "no_entity_in_area": "\u0412\u0438\u0431\u0430\u0447\u0442\u0435, \u043c\u0435\u043d\u0456 \u043d\u0435 \u0432\u0456\u0434\u043e\u043c\u043e \u043f\u0440\u0438\u0441\u0442\u0440\u043e\u044e \u0437 \u043d\u0430\u0437\u0432\u043e\u044e {{ entity }} \u0432 \u043f\u0440\u0438\u043c\u0456\u0449\u0435\u043d\u043d\u0456 {{ area }}",
             "no_entity_in_area_exposed": "\u0412\u0438\u0431\u0430\u0447\u0442\u0435, {{ entity }} \u0432 \u043f\u0440\u0438\u043c\u0456\u0449\u0435\u043d\u043d\u0456 {{ area }} \u043d\u0435 \u0454 \u0434\u043e\u0441\u0442\u0443\u043f\u043d\u0438\u043c",
+            "no_entity_in_floor": "\u0412\u0438\u0431\u0430\u0447\u0442\u0435, \u043c\u0435\u043d\u0456 \u043d\u0435 \u0432\u0456\u0434\u043e\u043c\u043e \u043f\u0440\u0438\u0441\u0442\u0440\u043e\u044e \u0437 \u043d\u0430\u0437\u0432\u043e\u044e {{ entity }} \u043d\u0430 {{ floor }} \u043f\u043e\u0432\u0435\u0440\u0441\u0456",
+            "no_entity_in_floor_exposed": "\u0412\u0438\u0431\u0430\u0447\u0442\u0435, {{ entity }} \u043d\u0430 {{ floor }} \u043f\u043e\u0432\u0435\u0440\u0441\u0456 \u043d\u0435 \u0454 \u0434\u043e\u0441\u0442\u0443\u043f\u043d\u0438\u043c",
+            "no_floor": "\u0412\u0438\u0431\u0430\u0447\u0442\u0435, \u043c\u0435\u043d\u0456 \u043d\u0435 \u0432\u0456\u0434\u043e\u043c\u0438\u0439 \u043f\u043e\u0432\u0435\u0440\u0445 \u0437 \u043d\u0430\u0437\u0432\u043e\u044e {{ area }}",
             "no_intent": "\u0412\u0438\u0431\u0430\u0447\u0442\u0435, \u044f \u0446\u044c\u043e\u0433\u043e \u043d\u0435 \u0440\u043e\u0437\u0443\u043c\u0456\u044e"
         },
         "intents": {
             "HassClimateGetTemperature": {
                 "default": "{{ state.state }} \u0433\u0440\u0430\u0434\u0443\u0441\u0456\u0432"
             },
             "HassGetState": {
@@ -1093,23 +1122,25 @@
             "HassTurnOff": {
                 "cover": "{{ slots.name }} \u0437\u0430\u043a\u0440\u0438\u0442\u043e",
                 "cover_area": "{{ slots.area }} \u0432\u0456\u0434\u043a\u0440\u0438\u0442\u043e",
                 "cover_device_class": "{{ slots.device_class }} \u0437\u0430\u043a\u0440\u0438\u0442\u043e",
                 "default": "{{ slots.name }} \u0432\u0438\u043c\u043a\u043d\u0435\u043d\u043e",
                 "fans_area": "\u0412\u0435\u043d\u0442\u0438\u043b\u044f\u0442\u043e\u0440\u0438 \u0432 {{ slots.area }} \u0432\u0438\u043c\u043a\u043d\u0435\u043d\u043e",
                 "lights_area": "\u0421\u0432\u0456\u0442\u043b\u043e \u0432 {{ slots.area }} \u0432\u0438\u043c\u043a\u043d\u0435\u043d\u043e",
+                "lights_floor": "\u0421\u0432\u0456\u0442\u043b\u043e \u0432\u0438\u043c\u043a\u043d\u0435\u043d\u043e",
                 "valve": "\u0417\u0430\u043a\u0440\u0438\u0442\u043e"
             },
             "HassTurnOn": {
                 "cover": "{{ slots.name }} \u0432\u0456\u0434\u043a\u0440\u0438\u0442\u043e",
                 "cover_area": "{{ slots.area }} \u0432\u0456\u0434\u043a\u0440\u0438\u0442\u043e",
                 "cover_device_class": "{{ slots.device_class }} \u0432\u0456\u0434\u043a\u0440\u0438\u0442\u043e",
                 "default": "{{ slots.name }} \u0432\u0432\u0456\u043c\u043a\u043d\u0435\u043d\u043e",
                 "fans_area": "\u0412\u0435\u043d\u0442\u0438\u043b\u044f\u0442\u043e\u0440\u0438 \u0432 {{ slots.area }} \u0432\u0432\u0456\u043c\u043a\u043d\u0435\u043d\u043e",
                 "lights_area": "\u0421\u0432\u0456\u0442\u043b\u043e \u0432 {{ slots.area }} \u0432\u0432\u0456\u043c\u043a\u043d\u0435\u043d\u043e",
+                "lights_floor": "\u0421\u0432\u0456\u0442\u043b\u043e \u0432\u0432\u0456\u043c\u043a\u043d\u0435\u043d\u043e",
                 "script": "\u0420\u043e\u0437\u043f\u043e\u0447\u0430\u0442\u043e",
                 "valve": "\u0412\u0456\u0434\u043a\u0440\u0438\u0442\u043e"
             },
             "HassVacuumReturnToBase": {
                 "default": "{{ slots.name }} \u043f\u043e\u0432\u0435\u0440\u0442\u0430\u0454\u0442\u044c\u0441\u044f"
             },
             "HassVacuumStart": {
```

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/data/ur.json` & `home-assistant-intents-2024.5.28/home_assistant_intents/data/ur.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/data/vi.json` & `home-assistant-intents-2024.5.28/home_assistant_intents/data/vi.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/data/zh-cn.json` & `home-assistant-intents-2024.5.28/home_assistant_intents/data/zh-cn.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/data/zh-hk.json` & `home-assistant-intents-2024.5.28/home_assistant_intents/data/zh-hk.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/data/zh-tw.json` & `home-assistant-intents-2024.5.28/home_assistant_intents/data/zh-tw.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents/languages.py` & `home-assistant-intents-2024.5.28/home_assistant_intents/languages.py`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents.egg-info/PKG-INFO` & `home-assistant-intents-2024.5.28/home_assistant_intents.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: home-assistant-intents
-Version: 2024.4.3
+Version: 2024.5.28
 Summary: Intents for Home Assistant
 Author-email: The Home Assistant Authors <hello@home-assistant.io>
 License: Apache-2.0
 Project-URL: Source Code, https://github.com/home-assistant/intents
 Keywords: home,assistant,intent,recognition
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `home-assistant-intents-2024.4.3/home_assistant_intents.egg-info/SOURCES.txt` & `home-assistant-intents-2024.5.28/home_assistant_intents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2024.4.3/pyproject.toml` & `home-assistant-intents-2024.5.28/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=62.3", "wheel~=0.37.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name        = "home-assistant-intents"
-version     = "2024.4.3"
+version     = "2024.5.28"
 license     = {text = "Apache-2.0"}
 description = "Intents for Home Assistant"
 readme      = "README.md"
 authors     = [
     {name = "The Home Assistant Authors", email = "hello@home-assistant.io"}
 ]
 keywords    = ["home", "assistant", "intent", "recognition"]
```

