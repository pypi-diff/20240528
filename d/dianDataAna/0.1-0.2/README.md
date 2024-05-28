# Comparing `tmp/dianDataAna-0.1.tar.gz` & `tmp/dianDataAna-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dianDataAna-0.1.tar", last modified: Tue May 28 07:24:37 2024, max compression
+gzip compressed data, was "dianDataAna-0.2.tar", last modified: Tue May 28 08:24:30 2024, max compression
```

## Comparing `dianDataAna-0.1.tar` & `dianDataAna-0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 07:24:37.583163 dianDataAna-0.1/
--rw-rw-rw-   0        0        0      102 2024-05-28 07:24:37.567497 dianDataAna-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-28 07:24:37.567497 dianDataAna-0.1/dianDataAna/
--rw-rw-rw-   0        0        0       55 2024-05-28 07:18:50.000000 dianDataAna-0.1/dianDataAna/__init__.py
--rw-rw-rw-   0        0        0     1315 2024-05-28 07:18:50.000000 dianDataAna-0.1/dianDataAna/dianDataAna.py
-drwxrwxrwx   0        0        0        0 2024-05-28 07:24:37.567497 dianDataAna-0.1/dianDataAna.egg-info/
--rw-rw-rw-   0        0        0      102 2024-05-28 07:24:37.000000 dianDataAna-0.1/dianDataAna.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      211 2024-05-28 07:24:37.000000 dianDataAna-0.1/dianDataAna.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 07:24:37.000000 dianDataAna-0.1/dianDataAna.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-28 07:24:37.000000 dianDataAna-0.1/dianDataAna.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2024-05-28 07:23:06.000000 dianDataAna-0.1/license.txt
--rw-rw-rw-   0        0        0       42 2024-05-28 07:24:37.583163 dianDataAna-0.1/setup.cfg
--rw-rw-rw-   0        0        0      234 2024-05-28 07:22:51.000000 dianDataAna-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:24:30.582831 dianDataAna-0.2/
+-rw-rw-rw-   0        0        0      102 2024-05-28 08:24:30.582831 dianDataAna-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-28 08:24:30.567205 dianDataAna-0.2/dianDataAna/
+-rw-rw-rw-   0        0        0     1315 2024-05-28 07:18:50.000000 dianDataAna-0.2/dianDataAna/DataRead.py
+-rw-rw-rw-   0        0        0       48 2024-05-28 08:23:22.000000 dianDataAna-0.2/dianDataAna/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:24:30.582831 dianDataAna-0.2/dianDataAna.egg-info/
+-rw-rw-rw-   0        0        0      102 2024-05-28 08:24:30.000000 dianDataAna-0.2/dianDataAna.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      208 2024-05-28 08:24:30.000000 dianDataAna-0.2/dianDataAna.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 08:24:30.000000 dianDataAna-0.2/dianDataAna.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-28 08:24:30.000000 dianDataAna-0.2/dianDataAna.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2024-05-28 07:23:06.000000 dianDataAna-0.2/license.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 08:24:30.582831 dianDataAna-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      234 2024-05-28 08:23:25.000000 dianDataAna-0.2/setup.py
```

### Comparing `dianDataAna-0.1/dianDataAna/dianDataAna.py` & `dianDataAna-0.2/dianDataAna/DataRead.py`

 * *Files identical despite different names*

