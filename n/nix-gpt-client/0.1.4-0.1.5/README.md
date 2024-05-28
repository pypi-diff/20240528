# Comparing `tmp/nix_gpt_client-0.1.4.tar.gz` & `tmp/nix_gpt_client-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nix_gpt_client-0.1.4.tar", last modified: Fri May 24 10:32:37 2024, max compression
+gzip compressed data, was "nix_gpt_client-0.1.5.tar", last modified: Tue May 28 10:27:06 2024, max compression
```

## Comparing `nix_gpt_client-0.1.4.tar` & `nix_gpt_client-0.1.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 nix       (1000) nix       (1000)        0 2024-05-24 10:32:37.251190 nix_gpt_client-0.1.4/
--rw-r--r--   0 nix       (1000) nix       (1000)     1063 2024-05-06 15:30:22.000000 nix_gpt_client-0.1.4/LICENCE
--rw-r--r--   0 nix       (1000) nix       (1000)     4187 2024-05-24 10:32:37.251190 nix_gpt_client-0.1.4/PKG-INFO
--rw-r--r--   0 nix       (1000) nix       (1000)     3470 2024-05-06 15:30:22.000000 nix_gpt_client-0.1.4/README.md
--rw-r--r--   0 nix       (1000) nix       (1000)      848 2024-05-24 10:32:04.000000 nix_gpt_client-0.1.4/pyproject.toml
--rw-r--r--   0 nix       (1000) nix       (1000)       38 2024-05-24 10:32:37.251190 nix_gpt_client-0.1.4/setup.cfg
-drwxr-xr-x   0 nix       (1000) nix       (1000)        0 2024-05-24 10:32:37.244523 nix_gpt_client-0.1.4/src/
--rw-r--r--   0 nix       (1000) nix       (1000)        0 2024-05-06 15:30:22.000000 nix_gpt_client-0.1.4/src/__init__.py
-drwxr-xr-x   0 nix       (1000) nix       (1000)        0 2024-05-24 10:32:37.244523 nix_gpt_client-0.1.4/src/nix/
--rw-r--r--   0 nix       (1000) nix       (1000)        0 2024-05-17 12:27:48.000000 nix_gpt_client-0.1.4/src/nix/__init__.py
-drwxr-xr-x   0 nix       (1000) nix       (1000)        0 2024-05-24 10:32:37.247857 nix_gpt_client-0.1.4/src/nix/gptclient/
--rw-r--r--   0 nix       (1000) nix       (1000)      169 2024-05-24 10:22:41.000000 nix_gpt_client-0.1.4/src/nix/gptclient/__init__.py
--rw-r--r--   0 nix       (1000) nix       (1000)     2360 2024-05-24 10:31:21.000000 nix_gpt_client-0.1.4/src/nix/gptclient/_gpt_client.py
--rw-r--r--   0 nix       (1000) nix       (1000)      483 2024-05-24 10:30:22.000000 nix_gpt_client-0.1.4/src/nix/gptclient/_tokens_count.py
--rw-r--r--   0 nix       (1000) nix       (1000)      680 2024-05-17 12:09:50.000000 nix_gpt_client-0.1.4/src/nix/gptclient/_types.py
--rw-r--r--   0 nix       (1000) nix       (1000)      654 2024-05-06 15:30:22.000000 nix_gpt_client-0.1.4/src/nix/gptclient/_validate.py
-drwxr-xr-x   0 nix       (1000) nix       (1000)        0 2024-05-24 10:32:37.251190 nix_gpt_client-0.1.4/src/nix_gpt_client.egg-info/
--rw-r--r--   0 nix       (1000) nix       (1000)     4187 2024-05-24 10:32:37.000000 nix_gpt_client-0.1.4/src/nix_gpt_client.egg-info/PKG-INFO
--rw-r--r--   0 nix       (1000) nix       (1000)      434 2024-05-24 10:32:37.000000 nix_gpt_client-0.1.4/src/nix_gpt_client.egg-info/SOURCES.txt
--rw-r--r--   0 nix       (1000) nix       (1000)        1 2024-05-24 10:32:37.000000 nix_gpt_client-0.1.4/src/nix_gpt_client.egg-info/dependency_links.txt
--rw-r--r--   0 nix       (1000) nix       (1000)       16 2024-05-24 10:32:37.000000 nix_gpt_client-0.1.4/src/nix_gpt_client.egg-info/requires.txt
--rw-r--r--   0 nix       (1000) nix       (1000)       13 2024-05-24 10:32:37.000000 nix_gpt_client-0.1.4/src/nix_gpt_client.egg-info/top_level.txt
+drwxr-xr-x   0 nix       (1000) nix       (1000)        0 2024-05-28 10:27:06.177603 nix_gpt_client-0.1.5/
+-rw-r--r--   0 nix       (1000) nix       (1000)     1063 2024-05-06 15:30:22.000000 nix_gpt_client-0.1.5/LICENCE
+-rw-r--r--   0 nix       (1000) nix       (1000)     4187 2024-05-28 10:27:06.177603 nix_gpt_client-0.1.5/PKG-INFO
+-rw-r--r--   0 nix       (1000) nix       (1000)     3470 2024-05-06 15:30:22.000000 nix_gpt_client-0.1.5/README.md
+-rw-r--r--   0 nix       (1000) nix       (1000)      848 2024-05-28 10:26:54.000000 nix_gpt_client-0.1.5/pyproject.toml
+-rw-r--r--   0 nix       (1000) nix       (1000)       38 2024-05-28 10:27:06.177603 nix_gpt_client-0.1.5/setup.cfg
+drwxr-xr-x   0 nix       (1000) nix       (1000)        0 2024-05-28 10:27:06.174270 nix_gpt_client-0.1.5/src/
+-rw-r--r--   0 nix       (1000) nix       (1000)        0 2024-05-06 15:30:22.000000 nix_gpt_client-0.1.5/src/__init__.py
+drwxr-xr-x   0 nix       (1000) nix       (1000)        0 2024-05-28 10:27:06.174270 nix_gpt_client-0.1.5/src/nix/
+-rw-r--r--   0 nix       (1000) nix       (1000)        0 2024-05-17 12:27:48.000000 nix_gpt_client-0.1.5/src/nix/__init__.py
+drwxr-xr-x   0 nix       (1000) nix       (1000)        0 2024-05-28 10:27:06.174270 nix_gpt_client-0.1.5/src/nix/gptclient/
+-rw-r--r--   0 nix       (1000) nix       (1000)      169 2024-05-24 10:22:41.000000 nix_gpt_client-0.1.5/src/nix/gptclient/__init__.py
+-rw-r--r--   0 nix       (1000) nix       (1000)     2509 2024-05-28 10:25:42.000000 nix_gpt_client-0.1.5/src/nix/gptclient/_gpt_client.py
+-rw-r--r--   0 nix       (1000) nix       (1000)      483 2024-05-24 10:59:30.000000 nix_gpt_client-0.1.5/src/nix/gptclient/_tokens_count.py
+-rw-r--r--   0 nix       (1000) nix       (1000)      681 2024-05-24 11:02:33.000000 nix_gpt_client-0.1.5/src/nix/gptclient/_types.py
+-rw-r--r--   0 nix       (1000) nix       (1000)      654 2024-05-06 15:30:22.000000 nix_gpt_client-0.1.5/src/nix/gptclient/_validate.py
+drwxr-xr-x   0 nix       (1000) nix       (1000)        0 2024-05-28 10:27:06.177603 nix_gpt_client-0.1.5/src/nix_gpt_client.egg-info/
+-rw-r--r--   0 nix       (1000) nix       (1000)     4187 2024-05-28 10:27:06.000000 nix_gpt_client-0.1.5/src/nix_gpt_client.egg-info/PKG-INFO
+-rw-r--r--   0 nix       (1000) nix       (1000)      434 2024-05-28 10:27:06.000000 nix_gpt_client-0.1.5/src/nix_gpt_client.egg-info/SOURCES.txt
+-rw-r--r--   0 nix       (1000) nix       (1000)        1 2024-05-28 10:27:06.000000 nix_gpt_client-0.1.5/src/nix_gpt_client.egg-info/dependency_links.txt
+-rw-r--r--   0 nix       (1000) nix       (1000)       16 2024-05-28 10:27:06.000000 nix_gpt_client-0.1.5/src/nix_gpt_client.egg-info/requires.txt
+-rw-r--r--   0 nix       (1000) nix       (1000)       13 2024-05-28 10:27:06.000000 nix_gpt_client-0.1.5/src/nix_gpt_client.egg-info/top_level.txt
```

### Comparing `nix_gpt_client-0.1.4/LICENCE` & `nix_gpt_client-0.1.5/LICENCE`

 * *Files identical despite different names*

### Comparing `nix_gpt_client-0.1.4/PKG-INFO` & `nix_gpt_client-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nix-gpt-client
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python library for easy interaction with the GPT API, featuring typed requests and responses.
 Author-email: nks_nix <nikusunix@gmail.com>
 Maintainer-email: nks_nix <nikusunix@gmail.com>
 Project-URL: Homepage, https://github.com/nixnks/nix-gpt-client
 Project-URL: Documentation, https://readthedocs.org
 Project-URL: Repository, https://github.com/nixnks/nix-gpt-client.git
 Project-URL: Changelog, https://github.com/nixnks/nix-gpt-client/CHANGELOG.md
```

### Comparing `nix_gpt_client-0.1.4/README.md` & `nix_gpt_client-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `nix_gpt_client-0.1.4/pyproject.toml` & `nix_gpt_client-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nix-gpt-client"
-version = "0.1.4"
+version = "0.1.5"
 dependencies = [
     "openai",
     "tiktoken"
 ]
 requires-python = ">=3.11"
 authors = [
     { name = "nks_nix", email = "nikusunix@gmail.com" },
```

### Comparing `nix_gpt_client-0.1.4/src/nix/gptclient/_gpt_client.py` & `nix_gpt_client-0.1.5/src/nix/gptclient/_gpt_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
         self._presence_penalty = presence_penalty
         self._frequency_penalty = frequency_penalty
         self._temperature = temperature
         self.response_format = response_format
 
         self._messages: dict = []
         self._ai_client: openai.OpenAI = openai.OpenAI()
+        self.last_cost = 0
 
     def add_message(self, role: GPTMessageRole, data: str | dict | list):
         data_in_json = json.dumps(data)
         self._messages.append({
             "role": role,
             "content": data_in_json
         })
@@ -43,24 +44,28 @@
             "content": f"{schema_type} JSON schema: {json_schema}"
         })
 
     def get_messages_token_count(self) -> int:
         from ._tokens_count import num_token_from_message
         return sum([num_token_from_message(message, self._model) for message in self._messages])
 
+    def get_messages(self) -> list:
+        return self._messages
+
     def run(self):
         try:
             response = self._ai_client.chat.completions.create(
                 messages=self._messages,
                 model=self._model,
                 temperature=self._temperature,
                 top_p=self._top_p,
                 presence_penalty=self._presence_penalty,
                 frequency_penalty=self._frequency_penalty,
                 response_format=self.response_format
             )
+            self.last_cost = response['cost']['total']
             if response.choices:
                 return response.choices[0].message.content
             else:
                 return None
         except openai.OpenAIError as error:
             raise error
```

### Comparing `nix_gpt_client-0.1.4/src/nix/gptclient/_types.py` & `nix_gpt_client-0.1.5/src/nix/gptclient/_types.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     user = "user"
 
 
 class GPTSchemaType(str, Enum):
     input = "Input"
     output = "Output"
 
+
 class GPTModel(str, Enum):
     GPT_4o = "gpt-4o"
     GPT_4o_2024_05_13 = "gpt-4o-2024-05-13"
     GPT_4_TURBO = "gpt-4-turbo"
     GPT_4_TURBO_2024_04_09 = "gpt-4-turbo-2024-04-09"
     GPT_4_TURBO_PREVIEW = "gpt-4-turbo-preview"
     GPT_4_0125_PREVIEW = "gpt-4-0125-preview"
```

### Comparing `nix_gpt_client-0.1.4/src/nix/gptclient/_validate.py` & `nix_gpt_client-0.1.5/src/nix/gptclient/_validate.py`

 * *Files identical despite different names*

### Comparing `nix_gpt_client-0.1.4/src/nix_gpt_client.egg-info/PKG-INFO` & `nix_gpt_client-0.1.5/src/nix_gpt_client.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nix-gpt-client
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python library for easy interaction with the GPT API, featuring typed requests and responses.
 Author-email: nks_nix <nikusunix@gmail.com>
 Maintainer-email: nks_nix <nikusunix@gmail.com>
 Project-URL: Homepage, https://github.com/nixnks/nix-gpt-client
 Project-URL: Documentation, https://readthedocs.org
 Project-URL: Repository, https://github.com/nixnks/nix-gpt-client.git
 Project-URL: Changelog, https://github.com/nixnks/nix-gpt-client/CHANGELOG.md
```

