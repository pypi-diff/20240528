# Comparing `tmp/research-task-0.1.1.tar.gz` & `tmp/research-task-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "research-task-0.1.1.tar", last modified: Tue May 28 12:25:03 2024, max compression
+gzip compressed data, was "research-task-0.1.2.tar", last modified: Tue May 28 13:57:00 2024, max compression
```

## Comparing `research-task-0.1.1.tar` & `research-task-0.1.2.tar`

### file list

```diff
@@ -1,37 +1,45 @@
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-28 12:25:03.063628 research-task-0.1.1/
--rw-r--r--   0 dan        (501) staff       (20)      180 2024-05-28 12:24:13.000000 research-task-0.1.1/MANIFEST.in
--rw-r--r--   0 dan        (501) staff       (20)     1184 2024-05-28 12:25:03.063382 research-task-0.1.1/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)       26 2024-05-16 15:47:54.000000 research-task-0.1.1/README.md
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-28 12:25:03.058669 research-task-0.1.1/llm_analyst/
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-28 12:25:03.059973 research-task-0.1.1/llm_analyst/resources/
--rw-r--r--   0 dan        (501) staff       (20)     1236 2024-05-25 16:35:56.000000 research-task-0.1.1/llm_analyst/resources/llm_analyst.config
--rw-r--r--   0 dan        (501) staff       (20)     1093 2024-05-21 17:28:03.000000 research-task-0.1.1/llm_analyst/resources/pdf_styles.css
--rw-r--r--   0 dan        (501) staff       (20)     9164 2024-05-23 21:57:26.000000 research-task-0.1.1/llm_analyst/resources/prompts.json
--rw-r--r--   0 dan        (501) staff       (20)      406 2024-05-28 11:06:20.000000 research-task-0.1.1/requirements.txt
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-28 12:25:03.060748 research-task-0.1.1/research_task.egg-info/
--rw-r--r--   0 dan        (501) staff       (20)     1184 2024-05-28 12:25:03.000000 research-task-0.1.1/research_task.egg-info/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)      907 2024-05-28 12:25:03.000000 research-task-0.1.1/research_task.egg-info/SOURCES.txt
--rw-r--r--   0 dan        (501) staff       (20)        1 2024-05-28 12:25:03.000000 research-task-0.1.1/research_task.egg-info/dependency_links.txt
--rw-r--r--   0 dan        (501) staff       (20)        1 2024-05-28 12:25:03.000000 research-task-0.1.1/research_task.egg-info/not-zip-safe
--rw-r--r--   0 dan        (501) staff       (20)      392 2024-05-28 12:25:03.000000 research-task-0.1.1/research_task.egg-info/requires.txt
--rw-r--r--   0 dan        (501) staff       (20)        6 2024-05-28 12:25:03.000000 research-task-0.1.1/research_task.egg-info/top_level.txt
--rw-r--r--   0 dan        (501) staff       (20)       38 2024-05-28 12:25:03.063669 research-task-0.1.1/setup.cfg
--rw-r--r--   0 dan        (501) staff       (20)      930 2024-05-28 12:24:53.000000 research-task-0.1.1/setup.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-28 12:25:03.061067 research-task-0.1.1/tests/
--rw-r--r--   0 dan        (501) staff       (20)        0 2024-05-16 21:01:10.000000 research-task-0.1.1/tests/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)      133 2024-05-21 12:53:04.000000 research-task-0.1.1/tests/conftest.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-28 12:25:03.061203 research-task-0.1.1/tests/llm_analyst/
--rw-r--r--   0 dan        (501) staff       (20)        0 2024-05-16 20:41:40.000000 research-task-0.1.1/tests/llm_analyst/__init__.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-28 12:25:03.061447 research-task-0.1.1/tests/llm_analyst/chat_models/
--rw-r--r--   0 dan        (501) staff       (20)        0 2024-05-21 21:28:43.000000 research-task-0.1.1/tests/llm_analyst/chat_models/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)     1526 2024-05-26 12:16:58.000000 research-task-0.1.1/tests/llm_analyst/chat_models/test_groq.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-28 12:25:03.063101 research-task-0.1.1/tests/llm_analyst/core/
--rw-r--r--   0 dan        (501) staff       (20)        0 2024-05-16 23:13:43.000000 research-task-0.1.1/tests/llm_analyst/core/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)     1992 2024-05-26 19:09:15.000000 research-task-0.1.1/tests/llm_analyst/core/test_config.py
--rw-r--r--   0 dan        (501) staff       (20)     4100 2024-05-26 12:16:58.000000 research-task-0.1.1/tests/llm_analyst/core/test_prompts.py
--rw-r--r--   0 dan        (501) staff       (20)     5552 2024-05-26 23:10:06.000000 research-task-0.1.1/tests/llm_analyst/core/test_research_analyst.py
--rw-r--r--   0 dan        (501) staff       (20)     1793 2024-05-26 23:12:37.000000 research-task-0.1.1/tests/llm_analyst/core/test_research_editor.py
--rw-r--r--   0 dan        (501) staff       (20)     2397 2024-05-27 00:56:40.000000 research-task-0.1.1/tests/llm_analyst/core/test_research_publisher.py
--rw-r--r--   0 dan        (501) staff       (20)     4321 2024-05-26 12:51:49.000000 research-task-0.1.1/tests/llm_analyst/core/test_research_state.py
--rw-r--r--   0 dan        (501) staff       (20)     2533 2024-05-27 00:34:56.000000 research-task-0.1.1/tests/llm_analyst/core/test_research_writer.py
--rw-r--r--   0 dan        (501) staff       (20)      795 2024-05-26 12:16:58.000000 research-task-0.1.1/tests/utils_for_pytest.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-28 13:57:00.950497 research-task-0.1.2/
+-rw-r--r--   0 dan        (501) staff       (20)       42 2024-05-28 13:46:14.000000 research-task-0.1.2/MANIFEST.in
+-rw-r--r--   0 dan        (501) staff       (20)     1184 2024-05-28 13:57:00.950269 research-task-0.1.2/PKG-INFO
+-rw-r--r--   0 dan        (501) staff       (20)       26 2024-05-16 15:47:54.000000 research-task-0.1.2/README.md
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-28 13:57:00.945669 research-task-0.1.2/llm_analyst/
+-rw-r--r--   0 dan        (501) staff       (20)        0 2024-05-28 13:55:52.000000 research-task-0.1.2/llm_analyst/__init__.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-28 13:57:00.945991 research-task-0.1.2/llm_analyst/chat_models/
+-rw-r--r--   0 dan        (501) staff       (20)        0 2024-05-16 23:23:22.000000 research-task-0.1.2/llm_analyst/chat_models/__init__.py
+-rw-r--r--   0 dan        (501) staff       (20)     1609 2024-05-23 14:05:24.000000 research-task-0.1.2/llm_analyst/chat_models/groq.py
+-rw-r--r--   0 dan        (501) staff       (20)     1624 2024-05-23 14:04:58.000000 research-task-0.1.2/llm_analyst/chat_models/openai.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-28 13:57:00.947825 research-task-0.1.2/llm_analyst/core/
+-rw-r--r--   0 dan        (501) staff       (20)        0 2024-05-16 23:12:03.000000 research-task-0.1.2/llm_analyst/core/__init__.py
+-rw-r--r--   0 dan        (501) staff       (20)     6576 2024-05-25 17:34:28.000000 research-task-0.1.2/llm_analyst/core/config.py
+-rw-r--r--   0 dan        (501) staff       (20)      130 2024-05-16 18:02:15.000000 research-task-0.1.2/llm_analyst/core/exceptions.py
+-rw-r--r--   0 dan        (501) staff       (20)     3033 2024-05-25 17:24:59.000000 research-task-0.1.2/llm_analyst/core/prompts.py
+-rw-r--r--   0 dan        (501) staff       (20)    14786 2024-05-26 22:05:51.000000 research-task-0.1.2/llm_analyst/core/research_analyst.py
+-rw-r--r--   0 dan        (501) staff       (20)     4650 2024-05-26 21:51:33.000000 research-task-0.1.2/llm_analyst/core/research_editor.py
+-rw-r--r--   0 dan        (501) staff       (20)     5990 2024-05-27 00:56:26.000000 research-task-0.1.2/llm_analyst/core/research_publisher.py
+-rw-r--r--   0 dan        (501) staff       (20)     5120 2024-05-26 12:43:01.000000 research-task-0.1.2/llm_analyst/core/research_state.py
+-rw-r--r--   0 dan        (501) staff       (20)     6655 2024-05-27 00:16:06.000000 research-task-0.1.2/llm_analyst/core/research_writer.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-28 13:57:00.948175 research-task-0.1.2/llm_analyst/embedding_methods/
+-rw-r--r--   0 dan        (501) staff       (20)        0 2024-05-17 16:18:10.000000 research-task-0.1.2/llm_analyst/embedding_methods/__init__.py
+-rw-r--r--   0 dan        (501) staff       (20)     2604 2024-05-23 20:11:10.000000 research-task-0.1.2/llm_analyst/embedding_methods/compressor.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-28 13:57:00.948305 research-task-0.1.2/llm_analyst/resources/
+-rw-r--r--   0 dan        (501) staff       (20)        0 2024-05-17 10:10:32.000000 research-task-0.1.2/llm_analyst/resources/__init__.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-28 13:57:00.948521 research-task-0.1.2/llm_analyst/scrapers/
+-rw-r--r--   0 dan        (501) staff       (20)        0 2024-05-20 16:23:04.000000 research-task-0.1.2/llm_analyst/scrapers/__init__.py
+-rw-r--r--   0 dan        (501) staff       (20)     1546 2024-05-20 19:38:22.000000 research-task-0.1.2/llm_analyst/scrapers/scraper_methods.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-28 13:57:00.948744 research-task-0.1.2/llm_analyst/search_methods/
+-rw-r--r--   0 dan        (501) staff       (20)        0 2024-05-17 11:24:03.000000 research-task-0.1.2/llm_analyst/search_methods/__init__.py
+-rw-r--r--   0 dan        (501) staff       (20)     8593 2024-05-27 19:48:47.000000 research-task-0.1.2/llm_analyst/search_methods/internet_search.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-28 13:57:00.949202 research-task-0.1.2/llm_analyst/utils/
+-rw-r--r--   0 dan        (501) staff       (20)        0 2024-05-21 18:11:23.000000 research-task-0.1.2/llm_analyst/utils/__init__.py
+-rw-r--r--   0 dan        (501) staff       (20)      976 2024-05-27 11:56:10.000000 research-task-0.1.2/llm_analyst/utils/app_logging.py
+-rw-r--r--   0 dan        (501) staff       (20)      228 2024-05-21 18:16:55.000000 research-task-0.1.2/llm_analyst/utils/utilities.py
+-rw-r--r--   0 dan        (501) staff       (20)      406 2024-05-28 11:06:20.000000 research-task-0.1.2/requirements.txt
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-28 13:57:00.949990 research-task-0.1.2/research_task.egg-info/
+-rw-r--r--   0 dan        (501) staff       (20)     1184 2024-05-28 13:57:00.000000 research-task-0.1.2/research_task.egg-info/PKG-INFO
+-rw-r--r--   0 dan        (501) staff       (20)     1063 2024-05-28 13:57:00.000000 research-task-0.1.2/research_task.egg-info/SOURCES.txt
+-rw-r--r--   0 dan        (501) staff       (20)        1 2024-05-28 13:57:00.000000 research-task-0.1.2/research_task.egg-info/dependency_links.txt
+-rw-r--r--   0 dan        (501) staff       (20)        1 2024-05-28 13:57:00.000000 research-task-0.1.2/research_task.egg-info/not-zip-safe
+-rw-r--r--   0 dan        (501) staff       (20)      392 2024-05-28 13:57:00.000000 research-task-0.1.2/research_task.egg-info/requires.txt
+-rw-r--r--   0 dan        (501) staff       (20)       12 2024-05-28 13:57:00.000000 research-task-0.1.2/research_task.egg-info/top_level.txt
+-rw-r--r--   0 dan        (501) staff       (20)       38 2024-05-28 13:57:00.950545 research-task-0.1.2/setup.cfg
+-rw-r--r--   0 dan        (501) staff       (20)     1060 2024-05-28 13:41:03.000000 research-task-0.1.2/setup.py
```

### Comparing `research-task-0.1.1/PKG-INFO` & `research-task-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: research-task
-Version: 0.1.1
+Version: 0.1.2
 Summary: LLM Research tool
 Home-page: https://github.com/DanHUMassMed/llm_analyst.git
 Author: Dan Higgins
 Author-email: daniel.higgins@yahoo.com
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: beautifulsoup4
```

### Comparing `research-task-0.1.1/research_task.egg-info/PKG-INFO` & `research-task-0.1.2/research_task.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: research-task
-Version: 0.1.1
+Version: 0.1.2
 Summary: LLM Research tool
 Home-page: https://github.com/DanHUMassMed/llm_analyst.git
 Author: Dan Higgins
 Author-email: daniel.higgins@yahoo.com
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: beautifulsoup4
```

