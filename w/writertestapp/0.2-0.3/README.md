# Comparing `tmp/writertestapp-0.2.tar.gz` & `tmp/writertestapp-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "writertestapp-0.2.tar", last modified: Tue May 28 15:26:53 2024, max compression
+gzip compressed data, was "writertestapp-0.3.tar", last modified: Tue May 28 15:29:32 2024, max compression
```

## Comparing `writertestapp-0.2.tar` & `writertestapp-0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 alikus    (1000) alikus    (1000)        0 2024-05-28 15:26:53.886168 writertestapp-0.2/
--rw-r--r--   0 alikus    (1000) alikus    (1000)        0 2024-05-28 12:48:49.000000 writertestapp-0.2/LICENSE.txt
--rw-r--r--   0 alikus    (1000) alikus    (1000)      294 2024-05-28 15:26:53.886168 writertestapp-0.2/PKG-INFO
--rw-r--r--   0 alikus    (1000) alikus    (1000)       38 2024-05-28 15:26:53.886168 writertestapp-0.2/setup.cfg
--rw-r--r--   0 alikus    (1000) alikus    (1000)      407 2024-05-28 15:26:48.000000 writertestapp-0.2/setup.py
-drwxr-xr-x   0 alikus    (1000) alikus    (1000)        0 2024-05-28 15:26:53.876168 writertestapp-0.2/simple_writer_app/
-drwxr-xr-x   0 alikus    (1000) alikus    (1000)        0 2024-05-28 15:26:53.886168 writertestapp-0.2/simple_writer_app/writertestapp.egg-info/
--rw-r--r--   0 alikus    (1000) alikus    (1000)      294 2024-05-28 15:26:53.000000 writertestapp-0.2/simple_writer_app/writertestapp.egg-info/PKG-INFO
--rw-r--r--   0 alikus    (1000) alikus    (1000)      240 2024-05-28 15:26:53.000000 writertestapp-0.2/simple_writer_app/writertestapp.egg-info/SOURCES.txt
--rw-r--r--   0 alikus    (1000) alikus    (1000)        1 2024-05-28 15:26:53.000000 writertestapp-0.2/simple_writer_app/writertestapp.egg-info/dependency_links.txt
--rw-r--r--   0 alikus    (1000) alikus    (1000)        1 2024-05-28 15:26:53.000000 writertestapp-0.2/simple_writer_app/writertestapp.egg-info/top_level.txt
+drwxr-xr-x   0 alikus    (1000) alikus    (1000)        0 2024-05-28 15:29:32.266167 writertestapp-0.3/
+-rw-r--r--   0 alikus    (1000) alikus    (1000)        0 2024-05-28 12:48:49.000000 writertestapp-0.3/LICENSE.txt
+-rw-r--r--   0 alikus    (1000) alikus    (1000)      294 2024-05-28 15:29:32.266167 writertestapp-0.3/PKG-INFO
+-rw-r--r--   0 alikus    (1000) alikus    (1000)       38 2024-05-28 15:29:32.266167 writertestapp-0.3/setup.cfg
+-rw-r--r--   0 alikus    (1000) alikus    (1000)      407 2024-05-28 15:29:25.000000 writertestapp-0.3/setup.py
+drwxr-xr-x   0 alikus    (1000) alikus    (1000)        0 2024-05-28 15:29:32.266167 writertestapp-0.3/simple_writer_app/
+drwxr-xr-x   0 alikus    (1000) alikus    (1000)        0 2024-05-28 15:29:32.266167 writertestapp-0.3/simple_writer_app/writertestapp.egg-info/
+-rw-r--r--   0 alikus    (1000) alikus    (1000)      294 2024-05-28 15:29:32.000000 writertestapp-0.3/simple_writer_app/writertestapp.egg-info/PKG-INFO
+-rw-r--r--   0 alikus    (1000) alikus    (1000)      240 2024-05-28 15:29:32.000000 writertestapp-0.3/simple_writer_app/writertestapp.egg-info/SOURCES.txt
+-rw-r--r--   0 alikus    (1000) alikus    (1000)        1 2024-05-28 15:29:32.000000 writertestapp-0.3/simple_writer_app/writertestapp.egg-info/dependency_links.txt
+-rw-r--r--   0 alikus    (1000) alikus    (1000)        1 2024-05-28 15:29:32.000000 writertestapp-0.3/simple_writer_app/writertestapp.egg-info/top_level.txt
```

