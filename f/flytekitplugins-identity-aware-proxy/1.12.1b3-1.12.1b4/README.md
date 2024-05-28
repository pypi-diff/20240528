# Comparing `tmp/flytekitplugins_identity_aware_proxy-1.12.1b3.tar.gz` & `tmp/flytekitplugins_identity_aware_proxy-1.12.1b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins_identity_aware_proxy-1.12.1b3.tar", last modified: Wed May 22 18:21:11 2024, max compression
+gzip compressed data, was "flytekitplugins_identity_aware_proxy-1.12.1b4.tar", last modified: Tue May 28 15:50:25 2024, max compression
```

## Comparing `flytekitplugins_identity_aware_proxy-1.12.1b3.tar` & `flytekitplugins_identity_aware_proxy-1.12.1b4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:11.074866 flytekitplugins_identity_aware_proxy-1.12.1b3/
--rw-r--r--   0 runner    (1001) docker     (127)    21942 2024-05-22 18:21:11.074866 flytekitplugins_identity_aware_proxy-1.12.1b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20805 2024-05-22 18:20:42.000000 flytekitplugins_identity_aware_proxy-1.12.1b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:11.070866 flytekitplugins_identity_aware_proxy-1.12.1b3/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:11.074866 flytekitplugins_identity_aware_proxy-1.12.1b3/flytekitplugins/identity_aware_proxy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:20:42.000000 flytekitplugins_identity_aware_proxy-1.12.1b3/flytekitplugins/identity_aware_proxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9491 2024-05-22 18:20:42.000000 flytekitplugins_identity_aware_proxy-1.12.1b3/flytekitplugins/identity_aware_proxy/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:11.074866 flytekitplugins_identity_aware_proxy-1.12.1b3/flytekitplugins_identity_aware_proxy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21942 2024-05-22 18:21:11.000000 flytekitplugins_identity_aware_proxy-1.12.1b3/flytekitplugins_identity_aware_proxy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-22 18:21:11.000000 flytekitplugins_identity_aware_proxy-1.12.1b3/flytekitplugins_identity_aware_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 18:21:11.000000 flytekitplugins_identity_aware_proxy-1.12.1b3/flytekitplugins_identity_aware_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-22 18:21:11.000000 flytekitplugins_identity_aware_proxy-1.12.1b3/flytekitplugins_identity_aware_proxy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-22 18:21:11.000000 flytekitplugins_identity_aware_proxy-1.12.1b3/flytekitplugins_identity_aware_proxy.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-22 18:21:11.000000 flytekitplugins_identity_aware_proxy-1.12.1b3/flytekitplugins_identity_aware_proxy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-22 18:21:11.000000 flytekitplugins_identity_aware_proxy-1.12.1b3/flytekitplugins_identity_aware_proxy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 18:21:11.074866 flytekitplugins_identity_aware_proxy-1.12.1b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-22 18:21:06.000000 flytekitplugins_identity_aware_proxy-1.12.1b3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:11.074866 flytekitplugins_identity_aware_proxy-1.12.1b3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6664 2024-05-22 18:20:42.000000 flytekitplugins_identity_aware_proxy-1.12.1b3/tests/test_flytekitplugins_iap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:50:25.687379 flytekitplugins_identity_aware_proxy-1.12.1b4/
+-rw-r--r--   0 runner    (1001) docker     (127)    21942 2024-05-28 15:50:25.687379 flytekitplugins_identity_aware_proxy-1.12.1b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20805 2024-05-28 15:49:57.000000 flytekitplugins_identity_aware_proxy-1.12.1b4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:50:25.683380 flytekitplugins_identity_aware_proxy-1.12.1b4/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:50:25.687379 flytekitplugins_identity_aware_proxy-1.12.1b4/flytekitplugins/identity_aware_proxy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 15:49:57.000000 flytekitplugins_identity_aware_proxy-1.12.1b4/flytekitplugins/identity_aware_proxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9491 2024-05-28 15:49:57.000000 flytekitplugins_identity_aware_proxy-1.12.1b4/flytekitplugins/identity_aware_proxy/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:50:25.687379 flytekitplugins_identity_aware_proxy-1.12.1b4/flytekitplugins_identity_aware_proxy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21942 2024-05-28 15:50:25.000000 flytekitplugins_identity_aware_proxy-1.12.1b4/flytekitplugins_identity_aware_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-28 15:50:25.000000 flytekitplugins_identity_aware_proxy-1.12.1b4/flytekitplugins_identity_aware_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 15:50:25.000000 flytekitplugins_identity_aware_proxy-1.12.1b4/flytekitplugins_identity_aware_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-28 15:50:25.000000 flytekitplugins_identity_aware_proxy-1.12.1b4/flytekitplugins_identity_aware_proxy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-28 15:50:25.000000 flytekitplugins_identity_aware_proxy-1.12.1b4/flytekitplugins_identity_aware_proxy.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-28 15:50:25.000000 flytekitplugins_identity_aware_proxy-1.12.1b4/flytekitplugins_identity_aware_proxy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-28 15:50:25.000000 flytekitplugins_identity_aware_proxy-1.12.1b4/flytekitplugins_identity_aware_proxy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 15:50:25.687379 flytekitplugins_identity_aware_proxy-1.12.1b4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-28 15:50:20.000000 flytekitplugins_identity_aware_proxy-1.12.1b4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:50:25.687379 flytekitplugins_identity_aware_proxy-1.12.1b4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6664 2024-05-28 15:49:57.000000 flytekitplugins_identity_aware_proxy-1.12.1b4/tests/test_flytekitplugins_iap.py
```

### Comparing `flytekitplugins_identity_aware_proxy-1.12.1b3/PKG-INFO` & `flytekitplugins_identity_aware_proxy-1.12.1b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-identity_aware_proxy
-Version: 1.12.1b3
+Version: 1.12.1b4
 Summary: External command plugin to generate ID tokens for GCP Identity Aware Proxy
 Home-page: https://github.com/flyteorg/flytekit/tree/master/plugins/flytekit-identity-aware-proxy
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `flytekitplugins_identity_aware_proxy-1.12.1b3/README.md` & `flytekitplugins_identity_aware_proxy-1.12.1b4/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins_identity_aware_proxy-1.12.1b3/flytekitplugins/identity_aware_proxy/cli.py` & `flytekitplugins_identity_aware_proxy-1.12.1b4/flytekitplugins/identity_aware_proxy/cli.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins_identity_aware_proxy-1.12.1b3/flytekitplugins_identity_aware_proxy.egg-info/PKG-INFO` & `flytekitplugins_identity_aware_proxy-1.12.1b4/flytekitplugins_identity_aware_proxy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-identity_aware_proxy
-Version: 1.12.1b3
+Version: 1.12.1b4
 Summary: External command plugin to generate ID tokens for GCP Identity Aware Proxy
 Home-page: https://github.com/flyteorg/flytekit/tree/master/plugins/flytekit-identity-aware-proxy
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `flytekitplugins_identity_aware_proxy-1.12.1b3/flytekitplugins_identity_aware_proxy.egg-info/SOURCES.txt` & `flytekitplugins_identity_aware_proxy-1.12.1b4/flytekitplugins_identity_aware_proxy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flytekitplugins_identity_aware_proxy-1.12.1b3/setup.py` & `flytekitplugins_identity_aware_proxy-1.12.1b4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "google-auth",
     "flytekit>=1.10",
     # https://github.com/grpc/grpc/issues/33935
     # https://github.com/grpc/grpc/issues/35323
     "grpcio>=1.62.0",
 ]
 
-__version__ = "1.12.1b3"
+__version__ = "1.12.1b4"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="External command plugin to generate ID tokens for GCP Identity Aware Proxy",
```

### Comparing `flytekitplugins_identity_aware_proxy-1.12.1b3/tests/test_flytekitplugins_iap.py` & `flytekitplugins_identity_aware_proxy-1.12.1b4/tests/test_flytekitplugins_iap.py`

 * *Files identical despite different names*

