# Comparing `tmp/dde-agent-lib-1.0.0a3.tar.gz` & `tmp/dde-agent-lib-1.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dde-agent-lib-1.0.0a3.tar", last modified: Tue May 28 06:16:12 2024, max compression
+gzip compressed data, was "dist/dde-agent-lib-1.0.0a4.tar", last modified: Tue May 28 06:27:42 2024, max compression
```

## Comparing `dde-agent-lib-1.0.0a3.tar` & `dde-agent-lib-1.0.0a4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:16:12.000000 dde-agent-lib-1.0.0a3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:16:12.000000 dde-agent-lib-1.0.0a3/dde_agent_lib.egg-info/
--rw-r--r--   0 root         (0) root         (0)        6 2024-05-28 06:16:12.000000 dde-agent-lib-1.0.0a3/dde_agent_lib.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      435 2024-05-28 06:16:12.000000 dde-agent-lib-1.0.0a3/dde_agent_lib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 06:16:12.000000 dde-agent-lib-1.0.0a3/dde_agent_lib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      385 2024-05-28 06:16:12.000000 dde-agent-lib-1.0.0a3/dde_agent_lib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      399 2024-05-28 06:16:11.000000 dde-agent-lib-1.0.0a3/setup.py
--rw-r--r--   0 root         (0) root         (0)      119 2024-05-28 06:16:11.000000 dde-agent-lib-1.0.0a3/README.md
--rw-r--r--   0 root         (0) root         (0)      385 2024-05-28 06:16:12.000000 dde-agent-lib-1.0.0a3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 06:16:12.000000 dde-agent-lib-1.0.0a3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:16:12.000000 dde-agent-lib-1.0.0a3/agent/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:16:12.000000 dde-agent-lib-1.0.0a3/agent/wapper/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 06:16:11.000000 dde-agent-lib-1.0.0a3/agent/wapper/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:16:12.000000 dde-agent-lib-1.0.0a3/agent/service/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:16:12.000000 dde-agent-lib-1.0.0a3/agent/service/memory/
--rw-r--r--   0 root         (0) root         (0)     5101 2024-05-28 06:16:11.000000 dde-agent-lib-1.0.0a3/agent/service/memory/memorytool.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 06:16:11.000000 dde-agent-lib-1.0.0a3/agent/service/memory/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 06:16:11.000000 dde-agent-lib-1.0.0a3/agent/service/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:16:12.000000 dde-agent-lib-1.0.0a3/agent/service/llm/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 06:16:11.000000 dde-agent-lib-1.0.0a3/agent/service/llm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:16:12.000000 dde-agent-lib-1.0.0a3/agent/utils/
--rw-r--r--   0 root         (0) root         (0)     1744 2024-05-28 06:16:11.000000 dde-agent-lib-1.0.0a3/agent/utils/http_util.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 06:16:11.000000 dde-agent-lib-1.0.0a3/agent/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:16:12.000000 dde-agent-lib-1.0.0a3/agent/fegin/
--rw-r--r--   0 root         (0) root         (0)     1881 2024-05-28 06:16:11.000000 dde-agent-lib-1.0.0a3/agent/fegin/portal_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 06:16:11.000000 dde-agent-lib-1.0.0a3/agent/fegin/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 06:16:11.000000 dde-agent-lib-1.0.0a3/agent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:27:42.000000 dde-agent-lib-1.0.0a4/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:27:42.000000 dde-agent-lib-1.0.0a4/dde_agent_lib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        6 2024-05-28 06:27:42.000000 dde-agent-lib-1.0.0a4/dde_agent_lib.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      435 2024-05-28 06:27:42.000000 dde-agent-lib-1.0.0a4/dde_agent_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 06:27:42.000000 dde-agent-lib-1.0.0a4/dde_agent_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      385 2024-05-28 06:27:42.000000 dde-agent-lib-1.0.0a4/dde_agent_lib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      399 2024-05-28 06:27:41.000000 dde-agent-lib-1.0.0a4/setup.py
+-rw-r--r--   0 root         (0) root         (0)      119 2024-05-28 06:27:41.000000 dde-agent-lib-1.0.0a4/README.md
+-rw-r--r--   0 root         (0) root         (0)      385 2024-05-28 06:27:42.000000 dde-agent-lib-1.0.0a4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 06:27:42.000000 dde-agent-lib-1.0.0a4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:27:42.000000 dde-agent-lib-1.0.0a4/agent/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:27:42.000000 dde-agent-lib-1.0.0a4/agent/wapper/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 06:27:41.000000 dde-agent-lib-1.0.0a4/agent/wapper/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:27:42.000000 dde-agent-lib-1.0.0a4/agent/service/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:27:42.000000 dde-agent-lib-1.0.0a4/agent/service/memory/
+-rw-r--r--   0 root         (0) root         (0)     5115 2024-05-28 06:27:41.000000 dde-agent-lib-1.0.0a4/agent/service/memory/memorytool.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 06:27:41.000000 dde-agent-lib-1.0.0a4/agent/service/memory/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 06:27:41.000000 dde-agent-lib-1.0.0a4/agent/service/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:27:42.000000 dde-agent-lib-1.0.0a4/agent/service/llm/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 06:27:41.000000 dde-agent-lib-1.0.0a4/agent/service/llm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:27:42.000000 dde-agent-lib-1.0.0a4/agent/utils/
+-rw-r--r--   0 root         (0) root         (0)     1744 2024-05-28 06:27:41.000000 dde-agent-lib-1.0.0a4/agent/utils/http_util.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 06:27:41.000000 dde-agent-lib-1.0.0a4/agent/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 06:27:42.000000 dde-agent-lib-1.0.0a4/agent/fegin/
+-rw-r--r--   0 root         (0) root         (0)     1881 2024-05-28 06:27:41.000000 dde-agent-lib-1.0.0a4/agent/fegin/portal_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 06:27:41.000000 dde-agent-lib-1.0.0a4/agent/fegin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 06:27:41.000000 dde-agent-lib-1.0.0a4/agent/__init__.py
```

### Comparing `dde-agent-lib-1.0.0a3/agent/service/memory/memorytool.py` & `dde-agent-lib-1.0.0a4/agent/service/memory/memorytool.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
                 break
         return last_pdf_order_index
 
     def retrieve_memory(self,session_id: str, split_pdf: bool = False):
         self.logger.info(f'根据session_id[%s]从portal后端查询历史消息, split_pdf=[%s]', session_id, split_pdf)
         memories = []
         try:
-            memory_resp = self.get_chat_detail(session_id)
+            memory_resp = self.portal_client.get_chat_detail(session_id)
             if memory_resp is None or memory_resp.get("data") is None or memory_resp.get("data").get("conversation") is None:
                 self.logger.info(f'根据session_id[%s]从portal后端查询历史消息为空，请检查参数', session_id)
                 self.logger.info(f'retrieve_memory,session_id[{session_id}],return[]')
                 return []
             chat_info_list = memory_resp.get('data').get('conversation')
             if len(chat_info_list) < 2:
                 self.logger.info(f"retrieve_memory,len(chat_info_list) < 2, return[],session_id={session_id}")
```

### Comparing `dde-agent-lib-1.0.0a3/agent/utils/http_util.py` & `dde-agent-lib-1.0.0a4/agent/utils/http_util.py`

 * *Files identical despite different names*

### Comparing `dde-agent-lib-1.0.0a3/agent/fegin/portal_client.py` & `dde-agent-lib-1.0.0a4/agent/fegin/portal_client.py`

 * *Files identical despite different names*

