# Comparing `tmp/mkdocs_ai_summary-0.2.3.tar.gz` & `tmp/mkdocs_ai_summary-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_ai_summary-0.2.3.tar", last modified: Sat May 25 02:05:45 2024, max compression
+gzip compressed data, was "mkdocs_ai_summary-0.2.4.tar", last modified: Tue May 28 13:28:34 2024, max compression
```

## Comparing `mkdocs_ai_summary-0.2.3.tar` & `mkdocs_ai_summary-0.2.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:05:45.001359 mkdocs_ai_summary-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-25 02:05:35.000000 mkdocs_ai_summary-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-05-25 02:05:45.001359 mkdocs_ai_summary-0.2.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:05:44.997359 mkdocs_ai_summary-0.2.3/mkdocs_ai_summary/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 02:05:35.000000 mkdocs_ai_summary-0.2.3/mkdocs_ai_summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-25 02:05:35.000000 mkdocs_ai_summary-0.2.3/mkdocs_ai_summary/chatgpt_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-05-25 02:05:35.000000 mkdocs_ai_summary-0.2.3/mkdocs_ai_summary/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-05-25 02:05:35.000000 mkdocs_ai_summary-0.2.3/mkdocs_ai_summary/tongyi_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:05:44.997359 mkdocs_ai_summary-0.2.3/mkdocs_ai_summary.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-05-25 02:05:44.000000 mkdocs_ai_summary-0.2.3/mkdocs_ai_summary.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-25 02:05:44.000000 mkdocs_ai_summary-0.2.3/mkdocs_ai_summary.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 02:05:44.000000 mkdocs_ai_summary-0.2.3/mkdocs_ai_summary.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-25 02:05:44.000000 mkdocs_ai_summary-0.2.3/mkdocs_ai_summary.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-25 02:05:44.000000 mkdocs_ai_summary-0.2.3/mkdocs_ai_summary.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-25 02:05:44.000000 mkdocs_ai_summary-0.2.3/mkdocs_ai_summary.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-25 02:05:35.000000 mkdocs_ai_summary-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-25 02:05:35.000000 mkdocs_ai_summary-0.2.3/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 02:05:45.001359 mkdocs_ai_summary-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:28:34.959824 mkdocs_ai_summary-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-28 13:28:25.000000 mkdocs_ai_summary-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-05-28 13:28:34.959824 mkdocs_ai_summary-0.2.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:28:34.959824 mkdocs_ai_summary-0.2.4/mkdocs_ai_summary/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 13:28:25.000000 mkdocs_ai_summary-0.2.4/mkdocs_ai_summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-05-28 13:28:25.000000 mkdocs_ai_summary-0.2.4/mkdocs_ai_summary/chatgpt_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-05-28 13:28:25.000000 mkdocs_ai_summary-0.2.4/mkdocs_ai_summary/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-28 13:28:25.000000 mkdocs_ai_summary-0.2.4/mkdocs_ai_summary/tongyi_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:28:34.959824 mkdocs_ai_summary-0.2.4/mkdocs_ai_summary.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-05-28 13:28:34.000000 mkdocs_ai_summary-0.2.4/mkdocs_ai_summary.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-28 13:28:34.000000 mkdocs_ai_summary-0.2.4/mkdocs_ai_summary.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 13:28:34.000000 mkdocs_ai_summary-0.2.4/mkdocs_ai_summary.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-28 13:28:34.000000 mkdocs_ai_summary-0.2.4/mkdocs_ai_summary.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-28 13:28:34.000000 mkdocs_ai_summary-0.2.4/mkdocs_ai_summary.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-28 13:28:34.000000 mkdocs_ai_summary-0.2.4/mkdocs_ai_summary.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-28 13:28:25.000000 mkdocs_ai_summary-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-28 13:28:25.000000 mkdocs_ai_summary-0.2.4/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 13:28:34.959824 mkdocs_ai_summary-0.2.4/setup.cfg
```

### Comparing `mkdocs_ai_summary-0.2.3/LICENSE` & `mkdocs_ai_summary-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_ai_summary-0.2.3/PKG-INFO` & `mkdocs_ai_summary-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-ai-summary
-Version: 0.2.3
+Version: 0.2.4
 Summary: A mkdocs plugin to generage summary with the help of AI.
 Author-email: Yang Zhang <mail@yangzhang.site>
 License: MIT License
         
         Copyright (c) 2024 Yang Zhang
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mkdocs_ai_summary-0.2.3/mkdocs_ai_summary/chatgpt_api.py` & `mkdocs_ai_summary-0.2.4/mkdocs_ai_summary/chatgpt_api.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,45 +17,58 @@
             {"role": "user", "content": prompt},
         ],
     )
 
     return completion.choices[0].message.content
 
 
+def get_cache_dict(cache_dir, file_suffix="_ai_summary_cache2"):
+    cache_file = cache_dir + file_suffix
+    if os.path.exists(cache_file):
+        with open(cache_file, "r+") as f:
+            cache_dict = json.load(f)
+    else:
+        cache_dict = {}
+    return cache_dict
+
+
+def ask_with_cache(question, page, content_md5, model, cache_dict, logger):
+    # asked before
+    if page in cache_dict:
+        if content_md5 == cache_dict[page]["content_md5"]:
+            ai_summary = cache_dict[page]["ai_summary"]
+            logger.info("Using cache.")
+        # asked before, but content changed
+        else:
+            ai_summary = ask(question, model=model)
+    # do not aksed before
+    else:
+        ai_summary = ask(question, model=model)
+    return ai_summary
+
+
 def get_summary_chatgpt(
     page,
     prompt,
     markdown,
     cache=True,
     cache_dir="./",
     model="gpt-3.5-turbo",
     logger=logging.Logger(""),
 ):
     question = prompt + markdown
     if cache:
         content_md5 = md5(markdown.encode("utf-8")).hexdigest()
-        cache_file = f"{cache_dir}_ai_summary_cache2.json"
-        if os.path.exists(cache_file):
-            with open(cache_file, "r+") as f:
-                cache_dict = json.load(f)
-        else:
-            cache_dict = {}
-
-        # asked before
-        if page in cache_dict:
-            if content_md5 == cache_dict[page]["content_md5"]:
-                ai_summary = cache_dict[page]["ai_summary"]
-                logger.info("Using cache.")
-            # asked before, but content changed
-            else:
-                ai_summary = ask(question, model=model)
-        # do not aksed before
-        else:
-            ai_summary = ask(question, model=model)
-            cache_dict[page] = {"content_md5": content_md5, "ai_summary": ai_summary}
-            with open(f"{cache_dir}/_ai_summary_cache2.json", "w+") as f:
-                cache_dict = json.dump(cache_dict, f)
+        cache_dict = get_cache_dict(cache_dir, file_suffix="_ai_summary_cache2.json")
+        ai_summary = ask_with_cache(
+            question, page, content_md5, model, cache_dict, logger
+        )
+        # always refresh the cache
+        cache_dict[page] = {"content_md5": content_md5, "ai_summary": ai_summary}
+        with open(f"{cache_dir}/_ai_summary_cache2.json", "w+") as f:
+            cache_dict = json.dump(cache_dict, f, indent=4)
     else:
         ai_summary = ask(question, model=model)
+    removed_line_break = ai_summary.replace(r"\n", "")
     return f"""!!! chatgpt-summary "AI Summary powered by [ChatGPT](https://chat.openai.com/)"
-    {ai_summary}
+    {removed_line_break}
 """
```

### Comparing `mkdocs_ai_summary-0.2.3/mkdocs_ai_summary/plugin.py` & `mkdocs_ai_summary-0.2.4/mkdocs_ai_summary/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_ai_summary-0.2.3/mkdocs_ai_summary/tongyi_api.py` & `mkdocs_ai_summary-0.2.4/mkdocs_ai_summary/tongyi_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import json
 import random
 from hashlib import md5
 from http import HTTPStatus
 from dashscope import Generation
 import logging
 
+from .chatgpt_api import get_cache_dict, ask_with_cache
+
 MAX_LENGTH = 6000
 
 
 class AiSummaryError(Exception):
 
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
@@ -48,33 +50,21 @@
     cache_dir="./",
     model="qwen-turbo",
     logger=logging.Logger(""),
 ):
     question = (prompt + markdown)[: MAX_LENGTH - 10]
     if cache:
         content_md5 = md5(markdown.encode("utf-8")).hexdigest()
-        cache_file = f"{cache_dir}_ai_summary_cache.json"
-        if os.path.exists(cache_file):
-            with open(cache_file, "r+") as f:
-                cache_dict = json.load(f)
-        else:
-            cache_dict = {}
-
-        # asked before
-        if page in cache_dict:
-            if content_md5 == cache_dict[page]["content_md5"]:
-                ai_summary = cache_dict[page]["ai_summary"]
-                logger.info("Using cache.")
-            # asked before, but content changed
-            else:
-                ai_summary = ask(question, model=model)
-        # do not aksed before
-        else:
-            ai_summary = ask(question, model=model)
-            cache_dict[page] = {"content_md5": content_md5, "ai_summary": ai_summary}
-            with open(f"{cache_dir}/_ai_summary_cache.json", "w+") as f:
-                cache_dict = json.dump(cache_dict, f)
+        cache_dict = get_cache_dict(cache_dir, file_suffix="_ai_summary_cache1.json")
+        ai_summary = ask_with_cache(
+            question, page, content_md5, model, cache_dict, logger
+        )
+        # always refresh the cache
+        cache_dict[page] = {"content_md5": content_md5, "ai_summary": ai_summary}
+        with open(f"{cache_dir}/_ai_summary_cache2.json", "w+") as f:
+            cache_dict = json.dump(cache_dict, f, indent=4)
     else:
         ai_summary = ask(question, model=model)
+    removed_line_break = ai_summary.replace(r"\n", "")
     return f"""!!! tongyiai-summary "AI Summary powered by [通义千问](https://tongyi.aliyun.com/)"
-    {ai_summary}
+    {removed_line_break}
 """
```

### Comparing `mkdocs_ai_summary-0.2.3/mkdocs_ai_summary.egg-info/PKG-INFO` & `mkdocs_ai_summary-0.2.4/mkdocs_ai_summary.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-ai-summary
-Version: 0.2.3
+Version: 0.2.4
 Summary: A mkdocs plugin to generage summary with the help of AI.
 Author-email: Yang Zhang <mail@yangzhang.site>
 License: MIT License
         
         Copyright (c) 2024 Yang Zhang
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mkdocs_ai_summary-0.2.3/pyproject.toml` & `mkdocs_ai_summary-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["."]
 
 [project]
 name = "mkdocs-ai-summary"
-version = "0.2.3"
+version = "0.2.4"
 requires-python = ">=3.10"
 dependencies = [
     "mkdocs>=1.5.3",
 ]
 authors = [
   { name="Yang Zhang", email="mail@yangzhang.site" },
 ]
```

### Comparing `mkdocs_ai_summary-0.2.3/readme.md` & `mkdocs_ai_summary-0.2.4/readme.md`

 * *Files identical despite different names*

