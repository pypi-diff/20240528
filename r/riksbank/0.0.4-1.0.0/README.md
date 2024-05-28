# Comparing `tmp/riksbank-0.0.4.tar.gz` & `tmp/riksbank-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/riksbank-0.0.4.tar", last modified: Sat Dec 15 17:28:34 2018, max compression
+gzip compressed data, was "riksbank-1.0.0.tar", last modified: Tue May 28 19:18:36 2024, max compression
```

## Comparing `riksbank-0.0.4.tar` & `riksbank-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2018-12-15 17:28:34.000000 riksbank-0.0.4/
--rw-r--r--   0 thomas    (1000) thomas    (1000)      481 2018-12-15 17:28:34.000000 riksbank-0.0.4/PKG-INFO
--rw-r--r--   0 thomas    (1000) thomas    (1000)       41 2018-12-11 20:15:33.000000 riksbank-0.0.4/README.md
-drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2018-12-15 17:28:34.000000 riksbank-0.0.4/riksbank/
--rw-r--r--   0 thomas    (1000) thomas    (1000)       18 2018-12-15 17:23:10.000000 riksbank-0.0.4/riksbank/__init__.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1611 2018-12-15 12:11:52.000000 riksbank-0.0.4/riksbank/riksbank.py
-drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2018-12-15 17:28:34.000000 riksbank-0.0.4/riksbank.egg-info/
--rw-r--r--   0 thomas    (1000) thomas    (1000)      481 2018-12-15 17:28:34.000000 riksbank-0.0.4/riksbank.egg-info/PKG-INFO
--rw-r--r--   0 thomas    (1000) thomas    (1000)      219 2018-12-15 17:28:34.000000 riksbank-0.0.4/riksbank.egg-info/SOURCES.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)        1 2018-12-15 17:28:34.000000 riksbank-0.0.4/riksbank.egg-info/dependency_links.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)       12 2018-12-15 17:28:34.000000 riksbank-0.0.4/riksbank.egg-info/requires.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)        9 2018-12-15 17:28:34.000000 riksbank-0.0.4/riksbank.egg-info/top_level.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)       38 2018-12-15 17:28:34.000000 riksbank-0.0.4/setup.cfg
--rw-r--r--   0 thomas    (1000) thomas    (1000)      658 2018-12-15 17:28:23.000000 riksbank-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:18:36.584016 riksbank-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-28 19:18:32.000000 riksbank-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-28 19:18:36.584016 riksbank-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-28 19:18:32.000000 riksbank-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:18:36.584016 riksbank-1.0.0/riksbank/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-28 19:18:32.000000 riksbank-1.0.0/riksbank/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-28 19:18:32.000000 riksbank-1.0.0/riksbank/riksbank.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:18:36.584016 riksbank-1.0.0/riksbank.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-28 19:18:36.000000 riksbank-1.0.0/riksbank.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-28 19:18:36.000000 riksbank-1.0.0/riksbank.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 19:18:36.000000 riksbank-1.0.0/riksbank.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-28 19:18:36.000000 riksbank-1.0.0/riksbank.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-28 19:18:36.000000 riksbank-1.0.0/riksbank.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 19:18:36.584016 riksbank-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-28 19:18:32.000000 riksbank-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:18:36.584016 riksbank-1.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-28 19:18:32.000000 riksbank-1.0.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-28 19:18:32.000000 riksbank-1.0.0/test/test_riksbank.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

