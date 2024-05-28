# Comparing `tmp/anoteai-0.6.tar.gz` & `tmp/anoteai-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anoteai-0.6.tar", last modified: Tue May 28 15:52:22 2024, max compression
+gzip compressed data, was "anoteai-0.7.tar", last modified: Tue May 28 16:34:26 2024, max compression
```

## Comparing `anoteai-0.6.tar` & `anoteai-0.7.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 natanvidra   (501) staff       (20)        0 2024-05-28 15:52:22.381186 anoteai-0.6/
--rw-r--r--   0 natanvidra   (501) staff       (20)      232 2024-05-28 15:52:22.381071 anoteai-0.6/PKG-INFO
-drwxr-xr-x   0 natanvidra   (501) staff       (20)        0 2024-05-28 15:52:22.380156 anoteai-0.6/anoteai/
--rw-r--r--   0 natanvidra   (501) staff       (20)       23 2024-02-23 01:34:13.000000 anoteai-0.6/anoteai/__init__.py
--rw-r--r--   0 natanvidra   (501) staff       (20)    15495 2024-05-28 15:51:11.000000 anoteai-0.6/anoteai/core.py
--rw-r--r--   0 natanvidra   (501) staff       (20)     2328 2024-05-28 15:44:20.000000 anoteai-0.6/anoteai/testing.py
-drwxr-xr-x   0 natanvidra   (501) staff       (20)        0 2024-05-28 15:52:22.380798 anoteai-0.6/anoteai.egg-info/
--rw-r--r--   0 natanvidra   (501) staff       (20)      232 2024-05-28 15:52:22.000000 anoteai-0.6/anoteai.egg-info/PKG-INFO
--rw-r--r--   0 natanvidra   (501) staff       (20)      217 2024-05-28 15:52:22.000000 anoteai-0.6/anoteai.egg-info/SOURCES.txt
--rw-r--r--   0 natanvidra   (501) staff       (20)        1 2024-05-28 15:52:22.000000 anoteai-0.6/anoteai.egg-info/dependency_links.txt
--rw-r--r--   0 natanvidra   (501) staff       (20)        9 2024-05-28 15:52:22.000000 anoteai-0.6/anoteai.egg-info/requires.txt
--rw-r--r--   0 natanvidra   (501) staff       (20)        8 2024-05-28 15:52:22.000000 anoteai-0.6/anoteai.egg-info/top_level.txt
--rw-r--r--   0 natanvidra   (501) staff       (20)       38 2024-05-28 15:52:22.381224 anoteai-0.6/setup.cfg
--rw-r--r--   0 natanvidra   (501) staff       (20)      340 2024-05-28 15:52:19.000000 anoteai-0.6/setup.py
+drwxr-xr-x   0 natanvidra   (501) staff       (20)        0 2024-05-28 16:34:26.578305 anoteai-0.7/
+-rw-r--r--   0 natanvidra   (501) staff       (20)      232 2024-05-28 16:34:26.578156 anoteai-0.7/PKG-INFO
+drwxr-xr-x   0 natanvidra   (501) staff       (20)        0 2024-05-28 16:34:26.577078 anoteai-0.7/anoteai/
+-rw-r--r--   0 natanvidra   (501) staff       (20)       23 2024-02-23 01:34:13.000000 anoteai-0.7/anoteai/__init__.py
+-rw-r--r--   0 natanvidra   (501) staff       (20)    34331 2024-05-28 16:31:27.000000 anoteai-0.7/anoteai/core.py
+-rw-r--r--   0 natanvidra   (501) staff       (20)      610 2024-05-28 16:27:12.000000 anoteai-0.7/anoteai/pop_quiz.py
+-rw-r--r--   0 natanvidra   (501) staff       (20)     2384 2024-05-28 16:32:52.000000 anoteai-0.7/anoteai/testing.py
+drwxr-xr-x   0 natanvidra   (501) staff       (20)        0 2024-05-28 16:34:26.577962 anoteai-0.7/anoteai.egg-info/
+-rw-r--r--   0 natanvidra   (501) staff       (20)      232 2024-05-28 16:34:26.000000 anoteai-0.7/anoteai.egg-info/PKG-INFO
+-rw-r--r--   0 natanvidra   (501) staff       (20)      237 2024-05-28 16:34:26.000000 anoteai-0.7/anoteai.egg-info/SOURCES.txt
+-rw-r--r--   0 natanvidra   (501) staff       (20)        1 2024-05-28 16:34:26.000000 anoteai-0.7/anoteai.egg-info/dependency_links.txt
+-rw-r--r--   0 natanvidra   (501) staff       (20)        9 2024-05-28 16:34:26.000000 anoteai-0.7/anoteai.egg-info/requires.txt
+-rw-r--r--   0 natanvidra   (501) staff       (20)        8 2024-05-28 16:34:26.000000 anoteai-0.7/anoteai.egg-info/top_level.txt
+-rw-r--r--   0 natanvidra   (501) staff       (20)       38 2024-05-28 16:34:26.578352 anoteai-0.7/setup.cfg
+-rw-r--r--   0 natanvidra   (501) staff       (20)      340 2024-05-28 16:34:09.000000 anoteai-0.7/setup.py
```

### Comparing `anoteai-0.6/anoteai/testing.py` & `anoteai-0.7/anoteai/testing.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import time
-#from anoteai import anote
+#from anoteai import Anote
 from core import Anote
 
 
 if __name__ == "__main__":
-    api_key = '56bf88500d3622b97a1210844457bf32'
+    api_key = 'd0cf6bcde6e936424d89f8980884e470'
 
     anote = Anote(api_key, is_private=False)
     # anote = anote(api_key, is_private=True)
 
-    file_paths = ['sample_docs/doc1.pdf', 'sample_docs/doc2.pdf']
+    file_paths = ['sample_docs/doc1.pdf', 'sample_docs/doc2.pdf', "https://docs.anote.ai/", "https://anote.ai/"]
 
     upload_result = anote.upload(task_type="documents", model_type="gpt", file_paths=file_paths)
     print("output from upload: ", upload_result)
     chat_id = upload_result['id']
-    chat_result = anote.chat(chat_id, "What is this paper classification performance about?")
+    chat_result = anote.chat(chat_id, "Given what you know about Anote, generate 10 quiz questions")
     print("output from chat: ", chat_result)
     message_id = chat_result['message_id']
-    print("output from evaluate:", anote.evaluate(message_id))
+    # print("output from evaluate:", anote.evaluate(message_id))
 
     #PUBLIC
     # file_paths = ['sample_docs/doc1.pdf', 'sample_docs/doc2.pdf', 'https://docs.anote.ai/']
     # chat_id = anote.upload(task_type="documents", model_type="gpt", file_paths=file_paths)['id']
 
     # response1 = anote.chat(chat_id, "Who wrote the paper on Improving Classification performance?")
     # print("Answer:", response1['answer'])
```

