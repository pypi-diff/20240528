# Comparing `tmp/research-task-0.1.0.tar.gz` & `tmp/research-task-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "research-task-0.1.0.tar", last modified: Tue May 28 11:48:41 2024, max compression
+gzip compressed data, was "research-task-0.1.1.tar", last modified: Tue May 28 12:25:03 2024, max compression
```

## Comparing `research-task-0.1.0.tar` & `research-task-0.1.1.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-28 11:48:41.063910 research-task-0.1.0/
--rw-r--r--   0 dan        (501) staff       (20)      155 2024-05-28 10:41:12.000000 research-task-0.1.0/MANIFEST.in
--rw-r--r--   0 dan        (501) staff       (20)     1184 2024-05-28 11:48:41.063684 research-task-0.1.0/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)       26 2024-05-16 15:47:54.000000 research-task-0.1.0/README.md
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-28 11:48:41.058951 research-task-0.1.0/llm_analyst/
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-28 11:48:41.060207 research-task-0.1.0/llm_analyst/resources/
--rw-r--r--   0 dan        (501) staff       (20)     1236 2024-05-25 16:35:56.000000 research-task-0.1.0/llm_analyst/resources/llm_analyst.config
--rw-r--r--   0 dan        (501) staff       (20)     1093 2024-05-21 17:28:03.000000 research-task-0.1.0/llm_analyst/resources/pdf_styles.css
--rw-r--r--   0 dan        (501) staff       (20)     9164 2024-05-23 21:57:26.000000 research-task-0.1.0/llm_analyst/resources/prompts.json
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-28 11:48:41.060984 research-task-0.1.0/research_task.egg-info/
--rw-r--r--   0 dan        (501) staff       (20)     1184 2024-05-28 11:48:41.000000 research-task-0.1.0/research_task.egg-info/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)      890 2024-05-28 11:48:41.000000 research-task-0.1.0/research_task.egg-info/SOURCES.txt
--rw-r--r--   0 dan        (501) staff       (20)        1 2024-05-28 11:48:41.000000 research-task-0.1.0/research_task.egg-info/dependency_links.txt
--rw-r--r--   0 dan        (501) staff       (20)        1 2024-05-28 11:48:41.000000 research-task-0.1.0/research_task.egg-info/not-zip-safe
--rw-r--r--   0 dan        (501) staff       (20)      392 2024-05-28 11:48:41.000000 research-task-0.1.0/research_task.egg-info/requires.txt
--rw-r--r--   0 dan        (501) staff       (20)        6 2024-05-28 11:48:41.000000 research-task-0.1.0/research_task.egg-info/top_level.txt
--rw-r--r--   0 dan        (501) staff       (20)       38 2024-05-28 11:48:41.064065 research-task-0.1.0/setup.cfg
--rw-r--r--   0 dan        (501) staff       (20)      930 2024-05-28 11:46:35.000000 research-task-0.1.0/setup.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-28 11:48:41.061324 research-task-0.1.0/tests/
--rw-r--r--   0 dan        (501) staff       (20)        0 2024-05-16 21:01:10.000000 research-task-0.1.0/tests/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)      133 2024-05-21 12:53:04.000000 research-task-0.1.0/tests/conftest.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-28 11:48:41.061471 research-task-0.1.0/tests/llm_analyst/
--rw-r--r--   0 dan        (501) staff       (20)        0 2024-05-16 20:41:40.000000 research-task-0.1.0/tests/llm_analyst/__init__.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-28 11:48:41.061671 research-task-0.1.0/tests/llm_analyst/chat_models/
--rw-r--r--   0 dan        (501) staff       (20)        0 2024-05-21 21:28:43.000000 research-task-0.1.0/tests/llm_analyst/chat_models/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)     1526 2024-05-26 12:16:58.000000 research-task-0.1.0/tests/llm_analyst/chat_models/test_groq.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-28 11:48:41.063216 research-task-0.1.0/tests/llm_analyst/core/
--rw-r--r--   0 dan        (501) staff       (20)        0 2024-05-16 23:13:43.000000 research-task-0.1.0/tests/llm_analyst/core/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)     1992 2024-05-26 19:09:15.000000 research-task-0.1.0/tests/llm_analyst/core/test_config.py
--rw-r--r--   0 dan        (501) staff       (20)     4100 2024-05-26 12:16:58.000000 research-task-0.1.0/tests/llm_analyst/core/test_prompts.py
--rw-r--r--   0 dan        (501) staff       (20)     5552 2024-05-26 23:10:06.000000 research-task-0.1.0/tests/llm_analyst/core/test_research_analyst.py
--rw-r--r--   0 dan        (501) staff       (20)     1793 2024-05-26 23:12:37.000000 research-task-0.1.0/tests/llm_analyst/core/test_research_editor.py
--rw-r--r--   0 dan        (501) staff       (20)     2397 2024-05-27 00:56:40.000000 research-task-0.1.0/tests/llm_analyst/core/test_research_publisher.py
--rw-r--r--   0 dan        (501) staff       (20)     4321 2024-05-26 12:51:49.000000 research-task-0.1.0/tests/llm_analyst/core/test_research_state.py
--rw-r--r--   0 dan        (501) staff       (20)     2533 2024-05-27 00:34:56.000000 research-task-0.1.0/tests/llm_analyst/core/test_research_writer.py
--rw-r--r--   0 dan        (501) staff       (20)      795 2024-05-26 12:16:58.000000 research-task-0.1.0/tests/utils_for_pytest.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-28 12:25:03.063628 research-task-0.1.1/
+-rw-r--r--   0 dan        (501) staff       (20)      180 2024-05-28 12:24:13.000000 research-task-0.1.1/MANIFEST.in
+-rw-r--r--   0 dan        (501) staff       (20)     1184 2024-05-28 12:25:03.063382 research-task-0.1.1/PKG-INFO
+-rw-r--r--   0 dan        (501) staff       (20)       26 2024-05-16 15:47:54.000000 research-task-0.1.1/README.md
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-28 12:25:03.058669 research-task-0.1.1/llm_analyst/
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-28 12:25:03.059973 research-task-0.1.1/llm_analyst/resources/
+-rw-r--r--   0 dan        (501) staff       (20)     1236 2024-05-25 16:35:56.000000 research-task-0.1.1/llm_analyst/resources/llm_analyst.config
+-rw-r--r--   0 dan        (501) staff       (20)     1093 2024-05-21 17:28:03.000000 research-task-0.1.1/llm_analyst/resources/pdf_styles.css
+-rw-r--r--   0 dan        (501) staff       (20)     9164 2024-05-23 21:57:26.000000 research-task-0.1.1/llm_analyst/resources/prompts.json
+-rw-r--r--   0 dan        (501) staff       (20)      406 2024-05-28 11:06:20.000000 research-task-0.1.1/requirements.txt
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-28 12:25:03.060748 research-task-0.1.1/research_task.egg-info/
+-rw-r--r--   0 dan        (501) staff       (20)     1184 2024-05-28 12:25:03.000000 research-task-0.1.1/research_task.egg-info/PKG-INFO
+-rw-r--r--   0 dan        (501) staff       (20)      907 2024-05-28 12:25:03.000000 research-task-0.1.1/research_task.egg-info/SOURCES.txt
+-rw-r--r--   0 dan        (501) staff       (20)        1 2024-05-28 12:25:03.000000 research-task-0.1.1/research_task.egg-info/dependency_links.txt
+-rw-r--r--   0 dan        (501) staff       (20)        1 2024-05-28 12:25:03.000000 research-task-0.1.1/research_task.egg-info/not-zip-safe
+-rw-r--r--   0 dan        (501) staff       (20)      392 2024-05-28 12:25:03.000000 research-task-0.1.1/research_task.egg-info/requires.txt
+-rw-r--r--   0 dan        (501) staff       (20)        6 2024-05-28 12:25:03.000000 research-task-0.1.1/research_task.egg-info/top_level.txt
+-rw-r--r--   0 dan        (501) staff       (20)       38 2024-05-28 12:25:03.063669 research-task-0.1.1/setup.cfg
+-rw-r--r--   0 dan        (501) staff       (20)      930 2024-05-28 12:24:53.000000 research-task-0.1.1/setup.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-28 12:25:03.061067 research-task-0.1.1/tests/
+-rw-r--r--   0 dan        (501) staff       (20)        0 2024-05-16 21:01:10.000000 research-task-0.1.1/tests/__init__.py
+-rw-r--r--   0 dan        (501) staff       (20)      133 2024-05-21 12:53:04.000000 research-task-0.1.1/tests/conftest.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-28 12:25:03.061203 research-task-0.1.1/tests/llm_analyst/
+-rw-r--r--   0 dan        (501) staff       (20)        0 2024-05-16 20:41:40.000000 research-task-0.1.1/tests/llm_analyst/__init__.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-28 12:25:03.061447 research-task-0.1.1/tests/llm_analyst/chat_models/
+-rw-r--r--   0 dan        (501) staff       (20)        0 2024-05-21 21:28:43.000000 research-task-0.1.1/tests/llm_analyst/chat_models/__init__.py
+-rw-r--r--   0 dan        (501) staff       (20)     1526 2024-05-26 12:16:58.000000 research-task-0.1.1/tests/llm_analyst/chat_models/test_groq.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-28 12:25:03.063101 research-task-0.1.1/tests/llm_analyst/core/
+-rw-r--r--   0 dan        (501) staff       (20)        0 2024-05-16 23:13:43.000000 research-task-0.1.1/tests/llm_analyst/core/__init__.py
+-rw-r--r--   0 dan        (501) staff       (20)     1992 2024-05-26 19:09:15.000000 research-task-0.1.1/tests/llm_analyst/core/test_config.py
+-rw-r--r--   0 dan        (501) staff       (20)     4100 2024-05-26 12:16:58.000000 research-task-0.1.1/tests/llm_analyst/core/test_prompts.py
+-rw-r--r--   0 dan        (501) staff       (20)     5552 2024-05-26 23:10:06.000000 research-task-0.1.1/tests/llm_analyst/core/test_research_analyst.py
+-rw-r--r--   0 dan        (501) staff       (20)     1793 2024-05-26 23:12:37.000000 research-task-0.1.1/tests/llm_analyst/core/test_research_editor.py
+-rw-r--r--   0 dan        (501) staff       (20)     2397 2024-05-27 00:56:40.000000 research-task-0.1.1/tests/llm_analyst/core/test_research_publisher.py
+-rw-r--r--   0 dan        (501) staff       (20)     4321 2024-05-26 12:51:49.000000 research-task-0.1.1/tests/llm_analyst/core/test_research_state.py
+-rw-r--r--   0 dan        (501) staff       (20)     2533 2024-05-27 00:34:56.000000 research-task-0.1.1/tests/llm_analyst/core/test_research_writer.py
+-rw-r--r--   0 dan        (501) staff       (20)      795 2024-05-26 12:16:58.000000 research-task-0.1.1/tests/utils_for_pytest.py
```

### Comparing `research-task-0.1.0/PKG-INFO` & `research-task-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: research-task
-Version: 0.1.0
+Version: 0.1.1
 Summary: LLM Research tool
 Home-page: https://github.com/DanHUMassMed/llm_analyst.git
 Author: Dan Higgins
 Author-email: daniel.higgins@yahoo.com
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: beautifulsoup4
```

### Comparing `research-task-0.1.0/llm_analyst/resources/llm_analyst.config` & `research-task-0.1.1/llm_analyst/resources/llm_analyst.config`

 * *Files identical despite different names*

### Comparing `research-task-0.1.0/llm_analyst/resources/pdf_styles.css` & `research-task-0.1.1/llm_analyst/resources/pdf_styles.css`

 * *Files identical despite different names*

### Comparing `research-task-0.1.0/llm_analyst/resources/prompts.json` & `research-task-0.1.1/llm_analyst/resources/prompts.json`

 * *Files identical despite different names*

### Comparing `research-task-0.1.0/research_task.egg-info/PKG-INFO` & `research-task-0.1.1/research_task.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: research-task
-Version: 0.1.0
+Version: 0.1.1
 Summary: LLM Research tool
 Home-page: https://github.com/DanHUMassMed/llm_analyst.git
 Author: Dan Higgins
 Author-email: daniel.higgins@yahoo.com
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: beautifulsoup4
```

### Comparing `research-task-0.1.0/research_task.egg-info/SOURCES.txt` & `research-task-0.1.1/research_task.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 MANIFEST.in
 README.md
+requirements.txt
 setup.py
 llm_analyst/resources/llm_analyst.config
 llm_analyst/resources/pdf_styles.css
 llm_analyst/resources/prompts.json
 research_task.egg-info/PKG-INFO
 research_task.egg-info/SOURCES.txt
 research_task.egg-info/dependency_links.txt
```

### Comparing `research-task-0.1.0/tests/llm_analyst/chat_models/test_groq.py` & `research-task-0.1.1/tests/llm_analyst/chat_models/test_groq.py`

 * *Files identical despite different names*

### Comparing `research-task-0.1.0/tests/llm_analyst/core/test_config.py` & `research-task-0.1.1/tests/llm_analyst/core/test_config.py`

 * *Files identical despite different names*

### Comparing `research-task-0.1.0/tests/llm_analyst/core/test_prompts.py` & `research-task-0.1.1/tests/llm_analyst/core/test_prompts.py`

 * *Files identical despite different names*

### Comparing `research-task-0.1.0/tests/llm_analyst/core/test_research_analyst.py` & `research-task-0.1.1/tests/llm_analyst/core/test_research_analyst.py`

 * *Files identical despite different names*

### Comparing `research-task-0.1.0/tests/llm_analyst/core/test_research_editor.py` & `research-task-0.1.1/tests/llm_analyst/core/test_research_editor.py`

 * *Files identical despite different names*

### Comparing `research-task-0.1.0/tests/llm_analyst/core/test_research_publisher.py` & `research-task-0.1.1/tests/llm_analyst/core/test_research_publisher.py`

 * *Files identical despite different names*

### Comparing `research-task-0.1.0/tests/llm_analyst/core/test_research_state.py` & `research-task-0.1.1/tests/llm_analyst/core/test_research_state.py`

 * *Files identical despite different names*

### Comparing `research-task-0.1.0/tests/llm_analyst/core/test_research_writer.py` & `research-task-0.1.1/tests/llm_analyst/core/test_research_writer.py`

 * *Files identical despite different names*

### Comparing `research-task-0.1.0/tests/utils_for_pytest.py` & `research-task-0.1.1/tests/utils_for_pytest.py`

 * *Files identical despite different names*

