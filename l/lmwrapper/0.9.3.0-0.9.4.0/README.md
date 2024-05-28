# Comparing `tmp/lmwrapper-0.9.3.0.tar.gz` & `tmp/lmwrapper-0.9.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmwrapper-0.9.3.0.tar", last modified: Tue May 28 06:26:55 2024, max compression
+gzip compressed data, was "lmwrapper-0.9.4.0.tar", last modified: Tue May 28 14:34:14 2024, max compression
```

## Comparing `lmwrapper-0.9.3.0.tar` & `lmwrapper-0.9.4.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-05-28 06:26:55.861950 lmwrapper-0.9.3.0/
--rw-r--r--   0 dgros      (501) staff       (20)     6653 2024-05-28 06:26:55.861658 lmwrapper-0.9.3.0/PKG-INFO
--rw-r--r--   0 dgros      (501) staff       (20)     5312 2024-04-06 05:06:05.000000 lmwrapper-0.9.3.0/README.md
-drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-05-28 06:26:55.852758 lmwrapper-0.9.3.0/lmwrapper/
--rw-r--r--   0 dgros      (501) staff       (20)     2416 2024-03-28 22:03:47.000000 lmwrapper-0.9.3.0/lmwrapper/_TokenStoppingCriteria.py
--rw-r--r--   0 dgros      (501) staff       (20)        0 2024-03-28 22:03:47.000000 lmwrapper-0.9.3.0/lmwrapper/__init__.py
--rw-r--r--   0 dgros      (501) staff       (20)     4461 2024-04-29 22:31:00.000000 lmwrapper-0.9.3.0/lmwrapper/abstract_predictor.py
--rw-r--r--   0 dgros      (501) staff       (20)     1654 2024-03-28 22:03:47.000000 lmwrapper-0.9.3.0/lmwrapper/caching.py
--rw-r--r--   0 dgros      (501) staff       (20)      294 2024-03-28 22:03:47.000000 lmwrapper-0.9.3.0/lmwrapper/env.py
-drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-05-28 06:26:55.855634 lmwrapper-0.9.3.0/lmwrapper/huggingface_wrapper/
--rw-r--r--   0 dgros      (501) staff       (20)       90 2024-04-29 23:28:16.000000 lmwrapper-0.9.3.0/lmwrapper/huggingface_wrapper/__init__.py
--rw-r--r--   0 dgros      (501) staff       (20)     1712 2024-03-30 04:33:51.000000 lmwrapper-0.9.3.0/lmwrapper/huggingface_wrapper/prediction.py
--rw-r--r--   0 dgros      (501) staff       (20)    41718 2024-05-11 01:30:32.000000 lmwrapper-0.9.3.0/lmwrapper/huggingface_wrapper/predictor.py
--rw-r--r--   0 dgros      (501) staff       (20)      305 2024-04-29 22:31:00.000000 lmwrapper-0.9.3.0/lmwrapper/huggingface_wrapper/utilstorch.py
--rw-r--r--   0 dgros      (501) staff       (20)    27146 2024-04-29 22:31:00.000000 lmwrapper-0.9.3.0/lmwrapper/huggingface_wrapper/wrapper.py
--rw-r--r--   0 dgros      (501) staff       (20)     3920 2024-04-29 22:31:00.000000 lmwrapper-0.9.3.0/lmwrapper/interals.py
-drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-05-28 06:26:55.856501 lmwrapper-0.9.3.0/lmwrapper/openai_wrapper/
--rw-r--r--   0 dgros      (501) staff       (20)       74 2024-05-01 22:58:02.000000 lmwrapper-0.9.3.0/lmwrapper/openai_wrapper/__init__.py
--rw-r--r--   0 dgros      (501) staff       (20)    19242 2024-05-28 06:20:50.000000 lmwrapper-0.9.3.0/lmwrapper/openai_wrapper/wrapper.py
--rw-r--r--   0 dgros      (501) staff       (20)     3646 2024-03-28 22:03:47.000000 lmwrapper-0.9.3.0/lmwrapper/prompt_trimming.py
--rw-r--r--   0 dgros      (501) staff       (20)      583 2024-03-28 22:03:47.000000 lmwrapper-0.9.3.0/lmwrapper/runtime.py
--rw-r--r--   0 dgros      (501) staff       (20)     1149 2024-03-28 22:03:47.000000 lmwrapper-0.9.3.0/lmwrapper/secrets_manager.py
--rw-r--r--   0 dgros      (501) staff       (20)    16344 2024-05-11 01:22:44.000000 lmwrapper-0.9.3.0/lmwrapper/structs.py
--rw-r--r--   0 dgros      (501) staff       (20)      710 2024-03-19 21:15:58.000000 lmwrapper-0.9.3.0/lmwrapper/togethertoy.py
--rw-r--r--   0 dgros      (501) staff       (20)     2227 2024-04-06 06:54:30.000000 lmwrapper-0.9.3.0/lmwrapper/utils.py
--rw-r--r--   0 dgros      (501) staff       (20)     1098 2024-03-28 22:03:47.000000 lmwrapper-0.9.3.0/lmwrapper/wrapping_config.py
-drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-05-28 06:26:55.860360 lmwrapper-0.9.3.0/lmwrapper.egg-info/
--rw-r--r--   0 dgros      (501) staff       (20)     6653 2024-05-28 06:26:55.000000 lmwrapper-0.9.3.0/lmwrapper.egg-info/PKG-INFO
--rw-r--r--   0 dgros      (501) staff       (20)     1044 2024-05-28 06:26:55.000000 lmwrapper-0.9.3.0/lmwrapper.egg-info/SOURCES.txt
--rw-r--r--   0 dgros      (501) staff       (20)        1 2024-05-28 06:26:55.000000 lmwrapper-0.9.3.0/lmwrapper.egg-info/dependency_links.txt
--rw-r--r--   0 dgros      (501) staff       (20)      402 2024-05-28 06:26:55.000000 lmwrapper-0.9.3.0/lmwrapper.egg-info/requires.txt
--rw-r--r--   0 dgros      (501) staff       (20)       10 2024-05-28 06:26:55.000000 lmwrapper-0.9.3.0/lmwrapper.egg-info/top_level.txt
--rw-r--r--   0 dgros      (501) staff       (20)     4823 2024-05-28 06:26:08.000000 lmwrapper-0.9.3.0/pyproject.toml
--rw-r--r--   0 dgros      (501) staff       (20)       38 2024-05-28 06:26:55.862002 lmwrapper-0.9.3.0/setup.cfg
-drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-05-28 06:26:55.859890 lmwrapper-0.9.3.0/test/
--rw-r--r--   0 dgros      (501) staff       (20)     1244 2024-03-30 04:33:51.000000 lmwrapper-0.9.3.0/test/test_caching.py
--rw-r--r--   0 dgros      (501) staff       (20)      547 2024-03-28 22:03:47.000000 lmwrapper-0.9.3.0/test/test_docs.py
--rw-r--r--   0 dgros      (501) staff       (20)    31215 2024-05-02 00:01:14.000000 lmwrapper-0.9.3.0/test/test_huggingface.py
--rw-r--r--   0 dgros      (501) staff       (20)     6266 2024-05-11 01:59:20.000000 lmwrapper-0.9.3.0/test/test_huggingface_internals.py
--rw-r--r--   0 dgros      (501) staff       (20)     6534 2024-03-30 04:33:51.000000 lmwrapper-0.9.3.0/test/test_huggingface_memory.py
--rw-r--r--   0 dgros      (501) staff       (20)    18789 2024-05-11 01:40:49.000000 lmwrapper-0.9.3.0/test/test_models_common.py
--rw-r--r--   0 dgros      (501) staff       (20)    10516 2024-05-28 06:24:33.000000 lmwrapper-0.9.3.0/test/test_openai.py
--rw-r--r--   0 dgros      (501) staff       (20)      512 2024-03-28 22:03:47.000000 lmwrapper-0.9.3.0/test/test_prompt_trimming.py
--rw-r--r--   0 dgros      (501) staff       (20)     2080 2024-02-10 07:57:44.000000 lmwrapper-0.9.3.0/test/test_structs.py
--rw-r--r--   0 dgros      (501) staff       (20)      237 2024-02-10 00:21:07.000000 lmwrapper-0.9.3.0/test/test_util.py
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-05-28 14:34:14.244995 lmwrapper-0.9.4.0/
+-rw-r--r--   0 dgros      (501) staff       (20)     6653 2024-05-28 14:34:14.244654 lmwrapper-0.9.4.0/PKG-INFO
+-rw-r--r--   0 dgros      (501) staff       (20)     5312 2024-04-06 05:06:05.000000 lmwrapper-0.9.4.0/README.md
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-05-28 14:34:14.236933 lmwrapper-0.9.4.0/lmwrapper/
+-rw-r--r--   0 dgros      (501) staff       (20)     2416 2024-03-28 22:03:47.000000 lmwrapper-0.9.4.0/lmwrapper/_TokenStoppingCriteria.py
+-rw-r--r--   0 dgros      (501) staff       (20)        0 2024-03-28 22:03:47.000000 lmwrapper-0.9.4.0/lmwrapper/__init__.py
+-rw-r--r--   0 dgros      (501) staff       (20)     4461 2024-04-29 22:31:00.000000 lmwrapper-0.9.4.0/lmwrapper/abstract_predictor.py
+-rw-r--r--   0 dgros      (501) staff       (20)     1654 2024-03-28 22:03:47.000000 lmwrapper-0.9.4.0/lmwrapper/caching.py
+-rw-r--r--   0 dgros      (501) staff       (20)      294 2024-03-28 22:03:47.000000 lmwrapper-0.9.4.0/lmwrapper/env.py
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-05-28 14:34:14.239344 lmwrapper-0.9.4.0/lmwrapper/huggingface_wrapper/
+-rw-r--r--   0 dgros      (501) staff       (20)       90 2024-04-29 23:28:16.000000 lmwrapper-0.9.4.0/lmwrapper/huggingface_wrapper/__init__.py
+-rw-r--r--   0 dgros      (501) staff       (20)     1712 2024-03-30 04:33:51.000000 lmwrapper-0.9.4.0/lmwrapper/huggingface_wrapper/prediction.py
+-rw-r--r--   0 dgros      (501) staff       (20)    41718 2024-05-11 01:30:32.000000 lmwrapper-0.9.4.0/lmwrapper/huggingface_wrapper/predictor.py
+-rw-r--r--   0 dgros      (501) staff       (20)      305 2024-04-29 22:31:00.000000 lmwrapper-0.9.4.0/lmwrapper/huggingface_wrapper/utilstorch.py
+-rw-r--r--   0 dgros      (501) staff       (20)    27146 2024-04-29 22:31:00.000000 lmwrapper-0.9.4.0/lmwrapper/huggingface_wrapper/wrapper.py
+-rw-r--r--   0 dgros      (501) staff       (20)     3920 2024-04-29 22:31:00.000000 lmwrapper-0.9.4.0/lmwrapper/interals.py
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-05-28 14:34:14.240043 lmwrapper-0.9.4.0/lmwrapper/openai_wrapper/
+-rw-r--r--   0 dgros      (501) staff       (20)       74 2024-05-01 22:58:02.000000 lmwrapper-0.9.4.0/lmwrapper/openai_wrapper/__init__.py
+-rw-r--r--   0 dgros      (501) staff       (20)    19696 2024-05-28 13:38:36.000000 lmwrapper-0.9.4.0/lmwrapper/openai_wrapper/wrapper.py
+-rw-r--r--   0 dgros      (501) staff       (20)     3646 2024-03-28 22:03:47.000000 lmwrapper-0.9.4.0/lmwrapper/prompt_trimming.py
+-rw-r--r--   0 dgros      (501) staff       (20)      583 2024-03-28 22:03:47.000000 lmwrapper-0.9.4.0/lmwrapper/runtime.py
+-rw-r--r--   0 dgros      (501) staff       (20)     1149 2024-03-28 22:03:47.000000 lmwrapper-0.9.4.0/lmwrapper/secrets_manager.py
+-rw-r--r--   0 dgros      (501) staff       (20)    17296 2024-05-28 14:20:43.000000 lmwrapper-0.9.4.0/lmwrapper/structs.py
+-rw-r--r--   0 dgros      (501) staff       (20)      710 2024-03-19 21:15:58.000000 lmwrapper-0.9.4.0/lmwrapper/togethertoy.py
+-rw-r--r--   0 dgros      (501) staff       (20)     2227 2024-04-06 06:54:30.000000 lmwrapper-0.9.4.0/lmwrapper/utils.py
+-rw-r--r--   0 dgros      (501) staff       (20)     1098 2024-03-28 22:03:47.000000 lmwrapper-0.9.4.0/lmwrapper/wrapping_config.py
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-05-28 14:34:14.243365 lmwrapper-0.9.4.0/lmwrapper.egg-info/
+-rw-r--r--   0 dgros      (501) staff       (20)     6653 2024-05-28 14:34:14.000000 lmwrapper-0.9.4.0/lmwrapper.egg-info/PKG-INFO
+-rw-r--r--   0 dgros      (501) staff       (20)     1044 2024-05-28 14:34:14.000000 lmwrapper-0.9.4.0/lmwrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 dgros      (501) staff       (20)        1 2024-05-28 14:34:14.000000 lmwrapper-0.9.4.0/lmwrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 dgros      (501) staff       (20)      402 2024-05-28 14:34:14.000000 lmwrapper-0.9.4.0/lmwrapper.egg-info/requires.txt
+-rw-r--r--   0 dgros      (501) staff       (20)       10 2024-05-28 14:34:14.000000 lmwrapper-0.9.4.0/lmwrapper.egg-info/top_level.txt
+-rw-r--r--   0 dgros      (501) staff       (20)     4823 2024-05-28 14:28:42.000000 lmwrapper-0.9.4.0/pyproject.toml
+-rw-r--r--   0 dgros      (501) staff       (20)       38 2024-05-28 14:34:14.245053 lmwrapper-0.9.4.0/setup.cfg
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-05-28 14:34:14.242944 lmwrapper-0.9.4.0/test/
+-rw-r--r--   0 dgros      (501) staff       (20)     1244 2024-03-30 04:33:51.000000 lmwrapper-0.9.4.0/test/test_caching.py
+-rw-r--r--   0 dgros      (501) staff       (20)      547 2024-03-28 22:03:47.000000 lmwrapper-0.9.4.0/test/test_docs.py
+-rw-r--r--   0 dgros      (501) staff       (20)    31215 2024-05-02 00:01:14.000000 lmwrapper-0.9.4.0/test/test_huggingface.py
+-rw-r--r--   0 dgros      (501) staff       (20)     6266 2024-05-11 01:59:20.000000 lmwrapper-0.9.4.0/test/test_huggingface_internals.py
+-rw-r--r--   0 dgros      (501) staff       (20)     6534 2024-03-30 04:33:51.000000 lmwrapper-0.9.4.0/test/test_huggingface_memory.py
+-rw-r--r--   0 dgros      (501) staff       (20)    20390 2024-05-28 14:27:31.000000 lmwrapper-0.9.4.0/test/test_models_common.py
+-rw-r--r--   0 dgros      (501) staff       (20)    10516 2024-05-28 06:24:33.000000 lmwrapper-0.9.4.0/test/test_openai.py
+-rw-r--r--   0 dgros      (501) staff       (20)      512 2024-03-28 22:03:47.000000 lmwrapper-0.9.4.0/test/test_prompt_trimming.py
+-rw-r--r--   0 dgros      (501) staff       (20)     2080 2024-02-10 07:57:44.000000 lmwrapper-0.9.4.0/test/test_structs.py
+-rw-r--r--   0 dgros      (501) staff       (20)      237 2024-02-10 00:21:07.000000 lmwrapper-0.9.4.0/test/test_util.py
```

### Comparing `lmwrapper-0.9.3.0/PKG-INFO` & `lmwrapper-0.9.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmwrapper
-Version: 0.9.3.0
+Version: 0.9.4.0
 Summary: Wrapper around language model APIs
 Author: David Gros, Claudio Spiess
 Project-URL: Homepage, https://github.com/DaiseyCode/lmwrapper
 Keywords: large language models,openai
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `lmwrapper-0.9.3.0/README.md` & `lmwrapper-0.9.4.0/README.md`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.9.3.0/lmwrapper/_TokenStoppingCriteria.py` & `lmwrapper-0.9.4.0/lmwrapper/_TokenStoppingCriteria.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.9.3.0/lmwrapper/abstract_predictor.py` & `lmwrapper-0.9.4.0/lmwrapper/abstract_predictor.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.9.3.0/lmwrapper/caching.py` & `lmwrapper-0.9.4.0/lmwrapper/caching.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.9.3.0/lmwrapper/huggingface_wrapper/prediction.py` & `lmwrapper-0.9.4.0/lmwrapper/huggingface_wrapper/prediction.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.9.3.0/lmwrapper/huggingface_wrapper/predictor.py` & `lmwrapper-0.9.4.0/lmwrapper/huggingface_wrapper/predictor.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.9.3.0/lmwrapper/huggingface_wrapper/wrapper.py` & `lmwrapper-0.9.4.0/lmwrapper/huggingface_wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.9.3.0/lmwrapper/interals.py` & `lmwrapper-0.9.4.0/lmwrapper/interals.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.9.3.0/lmwrapper/openai_wrapper/wrapper.py` & `lmwrapper-0.9.4.0/lmwrapper/openai_wrapper/wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,24 +43,38 @@
             msg = (
                 "This property is only available when the prompt `logprobs` flag is set"
                 " (openai endpoint only will return tokens when logprobs is set)"
             )
             raise ValueError(
                 msg,
             )
-        return self.metad.logprobs.tokens
+        probably_chat = hasattr(self.metad.logprobs, "content")
+        if not probably_chat:
+            return self.metad.logprobs.tokens
+        else:
+            return [
+                lp.token
+                for lp in self.metad.logprobs.content
+            ]
 
     def _all_toks_offsets(self):
         return self.metad.logprobs.text_offset
 
     def _all_logprobs(self):
         if self.metad.logprobs is None:
             assert self.prompt.logprobs is None or self.prompt.logprobs == 0
             return None
-        return self.metad.logprobs.token_logprobs
+        probably_chat = hasattr(self.metad.logprobs, "content")
+        if not probably_chat:
+            return self.metad.logprobs.token_logprobs
+        else:
+            return [
+                lp.logprob
+                for lp in self.metad.logprobs.content
+            ]
 
     @property
     def completion_tokens(self):
         return self._all_toks()[self._get_completion_token_index() :]
 
     @property
     def completion_token_offsets(self):
```

### Comparing `lmwrapper-0.9.3.0/lmwrapper/prompt_trimming.py` & `lmwrapper-0.9.4.0/lmwrapper/prompt_trimming.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.9.3.0/lmwrapper/runtime.py` & `lmwrapper-0.9.4.0/lmwrapper/runtime.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.9.3.0/lmwrapper/secrets_manager.py` & `lmwrapper-0.9.4.0/lmwrapper/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.9.3.0/lmwrapper/structs.py` & `lmwrapper-0.9.4.0/lmwrapper/structs.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,31 @@
 LM_CHAT_DIALOG_COERCIBLE_TYPES = Union[
     str,
     list[Union["LmChatTurn", tuple[str, str], dict, str]],
     "LmChatDialog",
 ]  # Defines a set of types that can be converted into a LmChatDialog
 
 
+class StopMode(StrEnum):
+    """Determines how to try to handle stop tokens"""
+    WILL_NOT_CONTAIN = "WILL_NOT_CONTAIN"
+    """This emulates the classic openai completion API. This makes
+    sure the returned sequence will not contain the stop token.
+    Even though the completion text will not include the stop sequence,
+    it is possible for the returned tokens to have it in cases where the stop sequence
+    is a prefix of the next token."""
+    ONLY_STOP_GENERATING = "ONLY_STOP_GENERATING"
+    """This is the style of the openai chat API. This stops generating once
+    the sequence is seen. However, the output might contain the stop sequence."""
+    AUTO = "AUTO"
+    """This chooses a mode that is the default for the style of model. This
+    means the behavior is somewhat undefined and unpredictable, but is more
+    likely to work for more models."""
+
+
 @dataclass(frozen=True)
 class LmPrompt:
     text: str | LM_CHAT_DIALOG_COERCIBLE_TYPES
     """The actual text of the prompt. If it is a LM_CHAT_DIALOG_COERCIBLE_TYPES
     which can become a LmChatDialog (such as a list of strings) it will be converted
     into a LmChatDialog."""
     max_tokens: int | None = None
@@ -27,18 +44,21 @@
     It recommended that you specify a limit yourself to have more predictable
     behaviour."""
     stop: list[str] = None
     """Sequences where the model will stop generating further tokens.
     The returned text will not contain the stop sequence. This sequence might span
     accross tokens and does not have to be an actual token in the vocabulary.
     For example could make a stop token of 'I like pie' even if that's not actually
-    a token. Even though the completion text will not include the stop sequence,
-    it is possible for the returned tokens to have it in cases where the stop sequence
-    is a prefix of the next token.
+    a token.
     """
+    stop_mode: StopMode = StopMode.AUTO
+    """Different models/providers handle stopping in different ways. You can
+    either leave that as-is ("auto") or try to change the mode to try
+    to emulate another mode (which may or may not work depending on
+    the model)."""
     logprobs: int = 1
     """Include the log probabilities on the logprobs most likely tokens,
     as well the chosen tokens. For example, if logprobs is 5, the
     API will return a list of the 5 most likely tokens.
     The model will always return the logprob of the sampled token,
     so there may be up to logprobs+1 elements in the response.
```

### Comparing `lmwrapper-0.9.3.0/lmwrapper/togethertoy.py` & `lmwrapper-0.9.4.0/lmwrapper/togethertoy.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.9.3.0/lmwrapper/utils.py` & `lmwrapper-0.9.4.0/lmwrapper/utils.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.9.3.0/lmwrapper/wrapping_config.py` & `lmwrapper-0.9.4.0/lmwrapper/wrapping_config.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.9.3.0/lmwrapper.egg-info/PKG-INFO` & `lmwrapper-0.9.4.0/lmwrapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmwrapper
-Version: 0.9.3.0
+Version: 0.9.4.0
 Summary: Wrapper around language model APIs
 Author: David Gros, Claudio Spiess
 Project-URL: Homepage, https://github.com/DaiseyCode/lmwrapper
 Keywords: large language models,openai
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `lmwrapper-0.9.3.0/lmwrapper.egg-info/SOURCES.txt` & `lmwrapper-0.9.4.0/lmwrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.9.3.0/pyproject.toml` & `lmwrapper-0.9.4.0/pyproject.toml`

 * *Files identical despite different names*

```diff
@@ -13,15 +13,15 @@
 
 [tool.setuptools.packages.find]
 where = ["."]
 include = ["lmwrapper*"]
 
 [project]
 name = "lmwrapper"
-version = "0.9.3.0"
+version = "0.9.4.0"
 authors = [
     { name = "David Gros" },
     { name = "Claudio Spiess" },
 ]
 description = "Wrapper around language model APIs"
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `lmwrapper-0.9.3.0/test/test_caching.py` & `lmwrapper-0.9.4.0/test/test_caching.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.9.3.0/test/test_docs.py` & `lmwrapper-0.9.4.0/test/test_docs.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.9.3.0/test/test_huggingface.py` & `lmwrapper-0.9.4.0/test/test_huggingface.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.9.3.0/test/test_huggingface_internals.py` & `lmwrapper-0.9.4.0/test/test_huggingface_internals.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.9.3.0/test/test_huggingface_memory.py` & `lmwrapper-0.9.4.0/test/test_huggingface_memory.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.9.3.0/test/test_models_common.py` & `lmwrapper-0.9.4.0/test/test_models_common.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,19 @@
 from lmwrapper.huggingface_wrapper.wrapper import get_huggingface_lm
 from lmwrapper.openai_wrapper.wrapper import OpenAiModelNames, get_open_ai_lm
 from lmwrapper.structs import LmPrompt
 
 ALL_MODELS = [
     get_open_ai_lm(OpenAiModelNames.gpt_3_5_turbo_instruct),
     get_huggingface_lm("gpt2"),
+    get_open_ai_lm(OpenAiModelNames.gpt_3_5_turbo),
 ]
 
+COMPLETION_MODELS = ALL_MODELS[:-1]
+
 
 ECHOABLE_MODELS = [
     # get_open_ai_lm(OpenAiModelNames.gpt_3_5_turbo_instruct),
     # Won't work with now that echo disabled
     get_huggingface_lm("gpt2"),
 ]
 
@@ -243,15 +246,15 @@
             temperature=0,
             cache=False,
         ),
     )
     assert len(new_line.completion_tokens) == 4
 
 
-@pytest.mark.parametrize("lm", ALL_MODELS)
+@pytest.mark.parametrize("lm", COMPLETION_MODELS)
 def test_no_stopping_program(lm):
     prompt_text = "# Functions\ndef double(x):\n"
     resp = lm.predict(
         LmPrompt(
             prompt_text,
             max_tokens=50,
             logprobs=1,
@@ -271,14 +274,50 @@
             cache=False,
         ),
     )
     assert "\ndef" not in resp.completion_text
 
 
 @pytest.mark.parametrize("lm", ALL_MODELS)
+def test_stopping_begin_tok_full_tok(lm):
+    val_normal = lm.predict(
+        LmPrompt(
+            capital_prompt,
+            max_tokens=4,
+            logprobs=1,
+            temperature=0,
+            cache=False,
+        ),
+    )
+    print(val_normal.completion_text)
+    assert "is the city Paris" in val_normal.completion_text
+    assert len(val_normal.completion_tokens) == 4
+    assert (
+            lm.remove_special_chars_from_tokens(val_normal.completion_tokens)[-1]
+            == " Paris"
+    )
+    val_no_pa = lm.predict(
+        LmPrompt(
+            capital_prompt,
+            max_tokens=4,
+            logprobs=1,
+            temperature=0,
+            cache=False,
+            stop=[" Paris"],
+        ),
+    )
+    print(val_no_pa.completion_text)
+    assert val_no_pa.completion_text == " is the city"
+    assert len(val_no_pa.completion_tokens) == 3
+    assert val_no_pa.completion_tokens[0] == val_normal.completion_tokens[0]
+    assert val_no_pa.completion_tokens[1] == val_normal.completion_tokens[1]
+    assert val_no_pa.completion_tokens[2] == val_normal.completion_tokens[2]
+
+
+@pytest.mark.parametrize("lm", COMPLETION_MODELS)
 def test_stopping_begin_tok(lm):
     val_normal = lm.predict(
         LmPrompt(
             capital_prompt,
             max_tokens=4,
             logprobs=1,
             temperature=0,
@@ -302,23 +341,24 @@
             cache=False,
             stop=[" Pa"],
         ),
     )
     print(val_no_pa.completion_text)
     assert val_no_pa.completion_text == " is the city"
     assert len(val_no_pa.completion_tokens) == 3
+    assert val_no_pa.completion_tokens[0] == val_normal.completion_tokens[0]
     assert np.allclose(
         val_no_pa.completion_logprobs,
         val_normal.completion_logprobs[:-1],
         atol=0.001,
         rtol=0.001,
     )
 
 
-@pytest.mark.parametrize("lm", ALL_MODELS)
+@pytest.mark.parametrize("lm", COMPLETION_MODELS)
 def test_stopping_middle_tok(lm):
     val_normal = lm.predict(
         LmPrompt(
             capital_prompt,
             max_tokens=4,
             logprobs=1,
             temperature=0,
@@ -346,15 +386,15 @@
     )
     assert (
         lm.remove_special_chars_from_tokens(val_no_ari.completion_tokens)[-1]
         == " Paris"
     )
 
 
-@pytest.mark.parametrize("lm", ALL_MODELS)
+@pytest.mark.parametrize("lm", COMPLETION_MODELS)
 def test_stopping_end_tok(lm):
     val_normal = lm.predict(
         LmPrompt(
             capital_prompt,
             max_tokens=4,
             logprobs=1,
             temperature=0,
@@ -382,15 +422,15 @@
     )
     assert (
         lm.remove_special_chars_from_tokens(val_no_ris.completion_tokens)[-1]
         == " Paris"
     )
 
 
-@pytest.mark.parametrize("lm", ALL_MODELS)
+@pytest.mark.parametrize("lm", COMPLETION_MODELS)
 def test_stopping_span_subtoks(lm):
     val_normal = lm.predict(
         LmPrompt(
             capital_prompt,
             max_tokens=4,
             logprobs=1,
             temperature=0,
@@ -417,15 +457,15 @@
         rtol=0.001,
     )
     assert (
         lm.remove_special_chars_from_tokens(val_no_ris.completion_tokens)[-1] == " city"
     )
 
 
-@pytest.mark.parametrize("lm", ALL_MODELS)
+@pytest.mark.parametrize("lm", COMPLETION_MODELS)
 def test_stopping_span_subtoks2(lm):
     val_normal = lm.predict(
         LmPrompt(
             capital_prompt,
             max_tokens=4,
             logprobs=1,
             temperature=0,
@@ -452,15 +492,15 @@
         rtol=0.001,
     )
     assert (
         lm.remove_special_chars_from_tokens(val_no_ris.completion_tokens)[-1] == " city"
     )
 
 
-@pytest.mark.parametrize("lm", ALL_MODELS)
+@pytest.mark.parametrize("lm", COMPLETION_MODELS)
 def test_stopping_span_subtoks_multiple(lm):
     val_normal = lm.predict(
         LmPrompt(
             capital_prompt,
             max_tokens=4,
             logprobs=1,
             temperature=0,
@@ -636,30 +676,36 @@
     assert pred.completion_text == " I J K"
     assert pred.completion_tokens == [" I", " J", " K"]
     base_len = len(prompt)
     assert pred.completion_token_offsets == [base_len + 0, base_len + 2, base_len + 4]
 
 
 @pytest.mark.parametrize("lm", ALL_MODELS)
-def test_token_offsets(lm):
+def test_token_seq_probs(lm):
     prompt = "A B C D E F G H"
     pred = lm.predict(
         LmPrompt(
             prompt,
             max_tokens=3,
             cache=False,
             temperature=0,
             logprobs=1,
         ),
     )
-    assert pred.completion_text == " I J K"
-    assert pred.completion_tokens == [" I", " J", " K"]
+    is_chat = lm not in COMPLETION_MODELS
+    if not is_chat:
+        expected_tokens = [" I", " J", " K"]
+    else:
+        # When in chat the next turn doesn't start with a space
+        expected_tokens = ["I", " J", " K"]
+    assert pred.completion_text == "".join(expected_tokens)
+    assert pred.completion_tokens == expected_tokens
     top_probs = pred.top_token_logprobs
     assert len(top_probs) == 3
-    for i, expected in enumerate([" I", " J", " K"]):
+    for i, expected in enumerate(expected_tokens):
         assert isinstance(top_probs[i][expected], float)
         assert top_probs[i][expected] == pred.completion_logprobs[i]
         assert top_probs[i][expected] < 0
 
 
 @pytest.mark.parametrize("lm", ECHOABLE_MODELS)
 def test_echo_many_toks(lm):
```

### Comparing `lmwrapper-0.9.3.0/test/test_openai.py` & `lmwrapper-0.9.4.0/test/test_openai.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.9.3.0/test/test_prompt_trimming.py` & `lmwrapper-0.9.4.0/test/test_prompt_trimming.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.9.3.0/test/test_structs.py` & `lmwrapper-0.9.4.0/test/test_structs.py`

 * *Files identical despite different names*

