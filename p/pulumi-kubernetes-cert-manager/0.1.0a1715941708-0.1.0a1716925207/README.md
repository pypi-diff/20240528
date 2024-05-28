# Comparing `tmp/pulumi_kubernetes_cert_manager-0.1.0a1715941708.tar.gz` & `tmp/pulumi_kubernetes_cert_manager-0.1.0a1716925207.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_kubernetes_cert_manager-0.1.0a1715941708.tar", last modified: Fri May 17 10:31:00 2024, max compression
+gzip compressed data, was "pulumi_kubernetes_cert_manager-0.1.0a1716925207.tar", last modified: Tue May 28 19:44:02 2024, max compression
```

## Comparing `pulumi_kubernetes_cert_manager-0.1.0a1715941708.tar` & `pulumi_kubernetes_cert_manager-0.1.0a1716925207.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-17 10:31:00.690595 pulumi_kubernetes_cert_manager-0.1.0a1715941708/
--rw-r--r--   0 runner    (1000) runner    (1000)     1951 2024-05-17 10:31:00.690595 pulumi_kubernetes_cert_manager-0.1.0a1715941708/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     1541 2024-05-17 10:31:00.000000 pulumi_kubernetes_cert_manager-0.1.0a1715941708/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-17 10:31:00.686595 pulumi_kubernetes_cert_manager-0.1.0a1715941708/pulumi_kubernetes_cert_manager/
--rw-------   0 runner    (1000) runner    (1000)      782 2024-05-17 10:31:00.000000 pulumi_kubernetes_cert_manager-0.1.0a1715941708/pulumi_kubernetes_cert_manager/__init__.py
--rw-------   0 runner    (1000) runner    (1000)    90893 2024-05-17 10:31:00.000000 pulumi_kubernetes_cert_manager-0.1.0a1715941708/pulumi_kubernetes_cert_manager/_inputs.py
--rw-------   0 runner    (1000) runner    (1000)     9228 2024-05-17 10:31:00.000000 pulumi_kubernetes_cert_manager-0.1.0a1715941708/pulumi_kubernetes_cert_manager/_utilities.py
--rw-------   0 runner    (1000) runner    (1000)    37520 2024-05-17 10:31:00.000000 pulumi_kubernetes_cert_manager-0.1.0a1715941708/pulumi_kubernetes_cert_manager/cert_manager.py
--rw-------   0 runner    (1000) runner    (1000)     3383 2024-05-17 10:31:00.000000 pulumi_kubernetes_cert_manager-0.1.0a1715941708/pulumi_kubernetes_cert_manager/outputs.py
--rw-------   0 runner    (1000) runner    (1000)     2781 2024-05-17 10:31:00.000000 pulumi_kubernetes_cert_manager-0.1.0a1715941708/pulumi_kubernetes_cert_manager/provider.py
--rw-------   0 runner    (1000) runner    (1000)       60 2024-05-17 10:31:00.000000 pulumi_kubernetes_cert_manager-0.1.0a1715941708/pulumi_kubernetes_cert_manager/pulumi-plugin.json
--rw-------   0 runner    (1000) runner    (1000)        0 2024-05-17 10:31:00.000000 pulumi_kubernetes_cert_manager-0.1.0a1715941708/pulumi_kubernetes_cert_manager/py.typed
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-17 10:31:00.690595 pulumi_kubernetes_cert_manager-0.1.0a1715941708/pulumi_kubernetes_cert_manager.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1951 2024-05-17 10:31:00.000000 pulumi_kubernetes_cert_manager-0.1.0a1715941708/pulumi_kubernetes_cert_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      692 2024-05-17 10:31:00.000000 pulumi_kubernetes_cert_manager-0.1.0a1715941708/pulumi_kubernetes_cert_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-05-17 10:31:00.000000 pulumi_kubernetes_cert_manager-0.1.0a1715941708/pulumi_kubernetes_cert_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-05-17 10:31:00.000000 pulumi_kubernetes_cert_manager-0.1.0a1715941708/pulumi_kubernetes_cert_manager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1000) runner    (1000)       81 2024-05-17 10:31:00.000000 pulumi_kubernetes_cert_manager-0.1.0a1715941708/pulumi_kubernetes_cert_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       31 2024-05-17 10:31:00.000000 pulumi_kubernetes_cert_manager-0.1.0a1715941708/pulumi_kubernetes_cert_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-05-17 10:31:00.690595 pulumi_kubernetes_cert_manager-0.1.0a1715941708/setup.cfg
--rw-------   0 runner    (1000) runner    (1000)     1427 2024-05-17 10:31:00.000000 pulumi_kubernetes_cert_manager-0.1.0a1715941708/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-28 19:44:02.247655 pulumi_kubernetes_cert_manager-0.1.0a1716925207/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2104 2024-05-28 19:44:02.247655 pulumi_kubernetes_cert_manager-0.1.0a1716925207/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     1541 2024-05-28 19:43:54.000000 pulumi_kubernetes_cert_manager-0.1.0a1716925207/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-28 19:44:02.247655 pulumi_kubernetes_cert_manager-0.1.0a1716925207/pulumi_kubernetes_cert_manager/
+-rw-------   0 runner    (1000) runner    (1000)      784 2024-05-28 19:43:54.000000 pulumi_kubernetes_cert_manager-0.1.0a1716925207/pulumi_kubernetes_cert_manager/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)    90895 2024-05-28 19:43:54.000000 pulumi_kubernetes_cert_manager-0.1.0a1716925207/pulumi_kubernetes_cert_manager/_inputs.py
+-rw-------   0 runner    (1000) runner    (1000)     9230 2024-05-28 19:43:54.000000 pulumi_kubernetes_cert_manager-0.1.0a1716925207/pulumi_kubernetes_cert_manager/_utilities.py
+-rw-------   0 runner    (1000) runner    (1000)    37522 2024-05-28 19:43:54.000000 pulumi_kubernetes_cert_manager-0.1.0a1716925207/pulumi_kubernetes_cert_manager/cert_manager.py
+-rw-------   0 runner    (1000) runner    (1000)     3385 2024-05-28 19:43:54.000000 pulumi_kubernetes_cert_manager-0.1.0a1716925207/pulumi_kubernetes_cert_manager/outputs.py
+-rw-------   0 runner    (1000) runner    (1000)     2783 2024-05-28 19:43:54.000000 pulumi_kubernetes_cert_manager-0.1.0a1716925207/pulumi_kubernetes_cert_manager/provider.py
+-rw-------   0 runner    (1000) runner    (1000)       99 2024-05-28 19:43:54.000000 pulumi_kubernetes_cert_manager-0.1.0a1716925207/pulumi_kubernetes_cert_manager/pulumi-plugin.json
+-rw-------   0 runner    (1000) runner    (1000)        0 2024-05-28 19:43:54.000000 pulumi_kubernetes_cert_manager-0.1.0a1716925207/pulumi_kubernetes_cert_manager/py.typed
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-28 19:44:02.247655 pulumi_kubernetes_cert_manager-0.1.0a1716925207/pulumi_kubernetes_cert_manager.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2104 2024-05-28 19:44:02.000000 pulumi_kubernetes_cert_manager-0.1.0a1716925207/pulumi_kubernetes_cert_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      645 2024-05-28 19:44:02.000000 pulumi_kubernetes_cert_manager-0.1.0a1716925207/pulumi_kubernetes_cert_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-05-28 19:44:02.000000 pulumi_kubernetes_cert_manager-0.1.0a1716925207/pulumi_kubernetes_cert_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       81 2024-05-28 19:44:02.000000 pulumi_kubernetes_cert_manager-0.1.0a1716925207/pulumi_kubernetes_cert_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       31 2024-05-28 19:44:02.000000 pulumi_kubernetes_cert_manager-0.1.0a1716925207/pulumi_kubernetes_cert_manager.egg-info/top_level.txt
+-rw-------   0 runner    (1000) runner    (1000)      804 2024-05-28 19:43:54.000000 pulumi_kubernetes_cert_manager-0.1.0a1716925207/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-05-28 19:44:02.247655 pulumi_kubernetes_cert_manager-0.1.0a1716925207/setup.cfg
```

### Comparing `pulumi_kubernetes_cert_manager-0.1.0a1715941708/PKG-INFO` & `pulumi_kubernetes_cert_manager-0.1.0a1716925207/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: pulumi_kubernetes_cert_manager
-Version: 0.1.0a1715941708
-Summary: Strongly-typed Cert Manager installation
-Home-page: https://pulumi.io
-License: Apache-2.0
-Project-URL: Repository, https://github.com/pulumi/pulumi-kubernetes-cert-manager
-Keywords: pulumi kubernetes cert-manager kind/component category/infrastructure
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
 # Pulumi Cert Manager Component
 
 This repo contains the Pulumi Cert Manager component for Kubernetes. This add-on automates the
 management and issuance of TLS certificates from various issuing sources. It ensures certificates
 are valid and up to date periodically, and attempts to renew certificates at an appropriate time
 before expiry.
```

### Comparing `pulumi_kubernetes_cert_manager-0.1.0a1715941708/README.md` & `pulumi_kubernetes_cert_manager-0.1.0a1716925207/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: pulumi_kubernetes_cert_manager
+Version: 0.1.0a1716925207
+Summary: Strongly-typed Cert Manager installation
+License: Apache-2.0
+Project-URL: Homepage, https://pulumi.io
+Project-URL: Repository, https://github.com/pulumi/pulumi-kubernetes-cert-manager
+Keywords: pulumi,kubernetes,cert-manager,kind/component,category/infrastructure
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Requires-Dist: parver>=0.2.1
+Requires-Dist: pulumi<4.0.0,>=3.0.0
+Requires-Dist: pulumi-kubernetes<5.0.0,>=3.7.1
+Requires-Dist: semver>=2.8.1
+
 # Pulumi Cert Manager Component
 
 This repo contains the Pulumi Cert Manager component for Kubernetes. This add-on automates the
 management and issuance of TLS certificates from various issuing sources. It ensures certificates
 are valid and up to date periodically, and attempts to renew certificates at an appropriate time
 before expiry.
```

### Comparing `pulumi_kubernetes_cert_manager-0.1.0a1715941708/pulumi_kubernetes_cert_manager/__init__.py` & `pulumi_kubernetes_cert_manager-0.1.0a1716925207/pulumi_kubernetes_cert_manager/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# *** WARNING: this file was generated by Pulumi SDK Generator. ***
+# *** WARNING: this file was generated by pulumi-language-python. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 from . import _utilities
 import typing
 # Export this package's modules as members:
 from .cert_manager import *
 from .provider import *
```

### Comparing `pulumi_kubernetes_cert_manager-0.1.0a1715941708/pulumi_kubernetes_cert_manager/_inputs.py` & `pulumi_kubernetes_cert_manager-0.1.0a1716925207/pulumi_kubernetes_cert_manager/_inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# *** WARNING: this file was generated by Pulumi SDK Generator. ***
+# *** WARNING: this file was generated by pulumi-language-python. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
```

### Comparing `pulumi_kubernetes_cert_manager-0.1.0a1715941708/pulumi_kubernetes_cert_manager/_utilities.py` & `pulumi_kubernetes_cert_manager-0.1.0a1716925207/pulumi_kubernetes_cert_manager/_utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# *** WARNING: this file was generated by Pulumi SDK Generator. ***
+# *** WARNING: this file was generated by pulumi-language-python. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 
 import asyncio
 import importlib.metadata
 import importlib.util
 import inspect
```

### Comparing `pulumi_kubernetes_cert_manager-0.1.0a1715941708/pulumi_kubernetes_cert_manager/cert_manager.py` & `pulumi_kubernetes_cert_manager-0.1.0a1716925207/pulumi_kubernetes_cert_manager/cert_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# *** WARNING: this file was generated by Pulumi SDK Generator. ***
+# *** WARNING: this file was generated by pulumi-language-python. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
```

### Comparing `pulumi_kubernetes_cert_manager-0.1.0a1715941708/pulumi_kubernetes_cert_manager/outputs.py` & `pulumi_kubernetes_cert_manager-0.1.0a1716925207/pulumi_kubernetes_cert_manager/outputs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# *** WARNING: this file was generated by Pulumi SDK Generator. ***
+# *** WARNING: this file was generated by pulumi-language-python. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
```

### Comparing `pulumi_kubernetes_cert_manager-0.1.0a1715941708/pulumi_kubernetes_cert_manager/provider.py` & `pulumi_kubernetes_cert_manager-0.1.0a1716925207/pulumi_kubernetes_cert_manager/provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# *** WARNING: this file was generated by Pulumi SDK Generator. ***
+# *** WARNING: this file was generated by pulumi-language-python. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
```

### Comparing `pulumi_kubernetes_cert_manager-0.1.0a1715941708/pulumi_kubernetes_cert_manager.egg-info/PKG-INFO` & `pulumi_kubernetes_cert_manager-0.1.0a1716925207/pulumi_kubernetes_cert_manager.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 Metadata-Version: 2.1
-Name: pulumi-kubernetes-cert-manager
-Version: 0.1.0a1715941708
+Name: pulumi_kubernetes_cert_manager
+Version: 0.1.0a1716925207
 Summary: Strongly-typed Cert Manager installation
-Home-page: https://pulumi.io
 License: Apache-2.0
+Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-kubernetes-cert-manager
-Keywords: pulumi kubernetes cert-manager kind/component category/infrastructure
+Keywords: pulumi,kubernetes,cert-manager,kind/component,category/infrastructure
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Requires-Dist: parver>=0.2.1
+Requires-Dist: pulumi<4.0.0,>=3.0.0
+Requires-Dist: pulumi-kubernetes<5.0.0,>=3.7.1
+Requires-Dist: semver>=2.8.1
 
 # Pulumi Cert Manager Component
 
 This repo contains the Pulumi Cert Manager component for Kubernetes. This add-on automates the
 management and issuance of TLS certificates from various issuing sources. It ensures certificates
 are valid and up to date periodically, and attempts to renew certificates at an appropriate time
 before expiry.
```

### Comparing `pulumi_kubernetes_cert_manager-0.1.0a1715941708/pulumi_kubernetes_cert_manager.egg-info/SOURCES.txt` & `pulumi_kubernetes_cert_manager-0.1.0a1716925207/pulumi_kubernetes_cert_manager.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 README.md
-setup.py
+pyproject.toml
 pulumi_kubernetes_cert_manager/__init__.py
 pulumi_kubernetes_cert_manager/_inputs.py
 pulumi_kubernetes_cert_manager/_utilities.py
 pulumi_kubernetes_cert_manager/cert_manager.py
 pulumi_kubernetes_cert_manager/outputs.py
 pulumi_kubernetes_cert_manager/provider.py
 pulumi_kubernetes_cert_manager/pulumi-plugin.json
 pulumi_kubernetes_cert_manager/py.typed
 pulumi_kubernetes_cert_manager.egg-info/PKG-INFO
 pulumi_kubernetes_cert_manager.egg-info/SOURCES.txt
 pulumi_kubernetes_cert_manager.egg-info/dependency_links.txt
-pulumi_kubernetes_cert_manager.egg-info/not-zip-safe
 pulumi_kubernetes_cert_manager.egg-info/requires.txt
 pulumi_kubernetes_cert_manager.egg-info/top_level.txt
```

