# Comparing `tmp/llama_index_readers_feishu_wiki-0.1.0.tar.gz` & `tmp/llama_index_readers_feishu_wiki-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_readers_feishu_wiki-0.1.0.tar", max compression
+gzip compressed data, was "llama_index_readers_feishu_wiki-0.1.1.tar", max compression
```

## Comparing `llama_index_readers_feishu_wiki-0.1.0.tar` & `llama_index_readers_feishu_wiki-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      982 2024-03-01 03:06:17.853972 llama_index_readers_feishu_wiki-0.1.0/README.md
--rw-r--r--   0        0        0       98 2024-03-01 03:06:17.853972 llama_index_readers_feishu_wiki-0.1.0/llama_index/readers/feishu_wiki/__init__.py
--rw-r--r--   0        0        0     5411 2024-03-01 03:06:17.853972 llama_index_readers_feishu_wiki-0.1.0/llama_index/readers/feishu_wiki/base.py
--rw-r--r--   0        0        0     1504 2024-03-01 03:06:17.853972 llama_index_readers_feishu_wiki-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1610 1970-01-01 00:00:00.000000 llama_index_readers_feishu_wiki-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      746 2024-05-28 16:46:24.949751 llama_index_readers_feishu_wiki-0.1.1/README.md
+-rw-r--r--   0        0        0       98 2024-05-28 16:46:24.949751 llama_index_readers_feishu_wiki-0.1.1/llama_index/readers/feishu_wiki/__init__.py
+-rw-r--r--   0        0        0     5410 2024-05-28 16:46:24.949751 llama_index_readers_feishu_wiki-0.1.1/llama_index/readers/feishu_wiki/base.py
+-rw-r--r--   0        0        0     1504 2024-05-28 16:46:24.949751 llama_index_readers_feishu_wiki-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1374 1970-01-01 00:00:00.000000 llama_index_readers_feishu_wiki-0.1.1/PKG-INFO
```

### Comparing `llama_index_readers_feishu_wiki-0.1.0/llama_index/readers/feishu_wiki/base.py` & `llama_index_readers_feishu_wiki-0.1.1/llama_index/readers/feishu_wiki/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         if self.tenant_access_token == "" or self.expire < time.time():
             self._update_tenant_access_token()
         headers = {
             "Authorization": f"Bearer {self.tenant_access_token}",
             "Content-Type": "application/json; charset=utf-8",
         }
 
-        url = self.host + self.wiki_spaces_url_path.format(space_id)
+        url = self.host + self.wiki_nodes_url_path.format(space_id)
         if parent_node_token:
             url += f"?parent_node_token={parent_node_token}"
         try:
             response = requests.get(url, headers=headers)
             result = response.json()
         except Exception:
             return []
```

### Comparing `llama_index_readers_feishu_wiki-0.1.0/pyproject.toml` & `llama_index_readers_feishu_wiki-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 authors = ["Your Name <you@example.com>"]
 description = "llama-index readers feishu_wiki integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 maintainers = ["zhourunlai"]
 name = "llama-index-readers-feishu-wiki"
 readme = "README.md"
-version = "0.1.0"
+version = "0.1.1"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 requests = "^2.31.0"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `llama_index_readers_feishu_wiki-0.1.0/PKG-INFO` & `llama_index_readers_feishu_wiki-0.1.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-readers-feishu-wiki
-Version: 0.1.0
+Version: 0.1.1
 Summary: llama-index readers feishu_wiki integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Maintainer: zhourunlai
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -25,19 +25,17 @@
 To use this loader, you need to:
 
 1. apply the permission(`wiki:wiki:readonly`) of the feishu app
 2. add the feishu app as the admin of your feishu space, see [here](https://open.feishu.cn/document/server-docs/docs/wiki-v2/wiki-qa#b5da330b) for more help
 3. finally, pass your feishu space id to this loader
 
 ```python
-from llama_index import download_loader
-
 app_id = "xxx"
 app_secret = "xxx"
 space_id = "xxx"
 FeishuWikiReader = download_loader("FeishuWikiReader")
 loader = FeishuWikiReader(app_id, app_secret)
 documents = loader.load_data(space_id=space_id)
 ```
 
-This loader is designed to be used as a way to load data into [LlamaIndex](https://github.com/run-llama/llama_index/tree/main/llama_index) and/or subsequently used as a Tool in a [LangChain](https://github.com/hwchase17/langchain) Agent. See [here](https://github.com/emptycrown/llama-hub/tree/main) for examples.
+This loader is designed to be used as a way to load data into [LlamaIndex](https://github.com/run-llama/llama_index/).
```

