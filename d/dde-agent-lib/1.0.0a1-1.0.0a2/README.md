# Comparing `tmp/dde-agent-lib-1.0.0a1.tar.gz` & `tmp/dde-agent-lib-1.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dde-agent-lib-1.0.0a1.tar", last modified: Fri May 17 08:28:50 2024, max compression
+gzip compressed data, was "dist/dde-agent-lib-1.0.0a2.tar", last modified: Tue May 28 04:11:41 2024, max compression
```

## Comparing `dde-agent-lib-1.0.0a1.tar` & `dde-agent-lib-1.0.0a2.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 08:28:50.000000 dde-agent-lib-1.0.0a1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 08:28:50.000000 dde-agent-lib-1.0.0a1/wapper/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-17 08:28:50.000000 dde-agent-lib-1.0.0a1/wapper/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 08:28:50.000000 dde-agent-lib-1.0.0a1/dde_agent_lib.egg-info/
--rw-r--r--   0 root         (0) root         (0)       27 2024-05-17 08:28:50.000000 dde-agent-lib-1.0.0a1/dde_agent_lib.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      363 2024-05-17 08:28:50.000000 dde-agent-lib-1.0.0a1/dde_agent_lib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 08:28:50.000000 dde-agent-lib-1.0.0a1/dde_agent_lib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      385 2024-05-17 08:28:50.000000 dde-agent-lib-1.0.0a1/dde_agent_lib.egg-info/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 08:28:50.000000 dde-agent-lib-1.0.0a1/service/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 08:28:50.000000 dde-agent-lib-1.0.0a1/service/memory/
--rw-r--r--   0 root         (0) root         (0)     5088 2024-05-17 08:28:50.000000 dde-agent-lib-1.0.0a1/service/memory/memorytool.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-17 08:28:50.000000 dde-agent-lib-1.0.0a1/service/memory/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-17 08:28:50.000000 dde-agent-lib-1.0.0a1/service/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 08:28:50.000000 dde-agent-lib-1.0.0a1/service/llm/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-17 08:28:50.000000 dde-agent-lib-1.0.0a1/service/llm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 08:28:50.000000 dde-agent-lib-1.0.0a1/utils/
--rw-r--r--   0 root         (0) root         (0)     1744 2024-05-17 08:28:50.000000 dde-agent-lib-1.0.0a1/utils/http_util.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-17 08:28:50.000000 dde-agent-lib-1.0.0a1/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      399 2024-05-17 08:28:50.000000 dde-agent-lib-1.0.0a1/setup.py
--rw-r--r--   0 root         (0) root         (0)      119 2024-05-17 08:28:50.000000 dde-agent-lib-1.0.0a1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 08:28:50.000000 dde-agent-lib-1.0.0a1/fegin/
--rw-r--r--   0 root         (0) root         (0)     1881 2024-05-17 08:28:50.000000 dde-agent-lib-1.0.0a1/fegin/portal_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-17 08:28:50.000000 dde-agent-lib-1.0.0a1/fegin/__init__.py
--rw-r--r--   0 root         (0) root         (0)      385 2024-05-17 08:28:50.000000 dde-agent-lib-1.0.0a1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-17 08:28:50.000000 dde-agent-lib-1.0.0a1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 04:11:41.000000 dde-agent-lib-1.0.0a2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 04:11:41.000000 dde-agent-lib-1.0.0a2/dde_agent_lib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        6 2024-05-28 04:11:40.000000 dde-agent-lib-1.0.0a2/dde_agent_lib.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      435 2024-05-28 04:11:40.000000 dde-agent-lib-1.0.0a2/dde_agent_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 04:11:40.000000 dde-agent-lib-1.0.0a2/dde_agent_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      385 2024-05-28 04:11:40.000000 dde-agent-lib-1.0.0a2/dde_agent_lib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      399 2024-05-28 04:11:40.000000 dde-agent-lib-1.0.0a2/setup.py
+-rw-r--r--   0 root         (0) root         (0)      119 2024-05-28 04:11:40.000000 dde-agent-lib-1.0.0a2/README.md
+-rw-r--r--   0 root         (0) root         (0)      385 2024-05-28 04:11:41.000000 dde-agent-lib-1.0.0a2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 04:11:41.000000 dde-agent-lib-1.0.0a2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 04:11:41.000000 dde-agent-lib-1.0.0a2/agent/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 04:11:41.000000 dde-agent-lib-1.0.0a2/agent/wapper/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 04:11:40.000000 dde-agent-lib-1.0.0a2/agent/wapper/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 04:11:41.000000 dde-agent-lib-1.0.0a2/agent/service/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 04:11:41.000000 dde-agent-lib-1.0.0a2/agent/service/memory/
+-rw-r--r--   0 root         (0) root         (0)     5094 2024-05-28 04:11:40.000000 dde-agent-lib-1.0.0a2/agent/service/memory/memorytool.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 04:11:40.000000 dde-agent-lib-1.0.0a2/agent/service/memory/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 04:11:40.000000 dde-agent-lib-1.0.0a2/agent/service/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 04:11:41.000000 dde-agent-lib-1.0.0a2/agent/service/llm/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 04:11:40.000000 dde-agent-lib-1.0.0a2/agent/service/llm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 04:11:41.000000 dde-agent-lib-1.0.0a2/agent/utils/
+-rw-r--r--   0 root         (0) root         (0)     1744 2024-05-28 04:11:40.000000 dde-agent-lib-1.0.0a2/agent/utils/http_util.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 04:11:40.000000 dde-agent-lib-1.0.0a2/agent/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 04:11:41.000000 dde-agent-lib-1.0.0a2/agent/fegin/
+-rw-r--r--   0 root         (0) root         (0)     1881 2024-05-28 04:11:40.000000 dde-agent-lib-1.0.0a2/agent/fegin/portal_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 04:11:40.000000 dde-agent-lib-1.0.0a2/agent/fegin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 04:11:40.000000 dde-agent-lib-1.0.0a2/agent/__init__.py
```

### Comparing `dde-agent-lib-1.0.0a1/service/memory/memorytool.py` & `dde-agent-lib-1.0.0a2/agent/service/memory/memorytool.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 from urllib.parse import unquote
-from fegin.portal_client import PortalClient
+from agent.fegin.portal_client import PortalClient
 
 class MemoryService:
     def __init__(self, logger, portal_address, system_config):
         self.logger = logger
         self.portal_client = PortalClient(portal_address,system_config)
 
     #检查当前轮对话是否上传pdf文档
```

### Comparing `dde-agent-lib-1.0.0a1/utils/http_util.py` & `dde-agent-lib-1.0.0a2/agent/utils/http_util.py`

 * *Files identical despite different names*

### Comparing `dde-agent-lib-1.0.0a1/fegin/portal_client.py` & `dde-agent-lib-1.0.0a2/agent/fegin/portal_client.py`

 * *Files identical despite different names*

