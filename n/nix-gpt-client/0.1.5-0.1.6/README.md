# Comparing `tmp/nix_gpt_client-0.1.5.tar.gz` & `tmp/nix_gpt_client-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nix_gpt_client-0.1.5.tar", last modified: Tue May 28 10:27:06 2024, max compression
+gzip compressed data, was "nix_gpt_client-0.1.6.tar", last modified: Tue May 28 10:55:44 2024, max compression
```

## Comparing `nix_gpt_client-0.1.5.tar` & `nix_gpt_client-0.1.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 nix       (1000) nix       (1000)        0 2024-05-28 10:27:06.177603 nix_gpt_client-0.1.5/
--rw-r--r--   0 nix       (1000) nix       (1000)     1063 2024-05-06 15:30:22.000000 nix_gpt_client-0.1.5/LICENCE
--rw-r--r--   0 nix       (1000) nix       (1000)     4187 2024-05-28 10:27:06.177603 nix_gpt_client-0.1.5/PKG-INFO
--rw-r--r--   0 nix       (1000) nix       (1000)     3470 2024-05-06 15:30:22.000000 nix_gpt_client-0.1.5/README.md
--rw-r--r--   0 nix       (1000) nix       (1000)      848 2024-05-28 10:26:54.000000 nix_gpt_client-0.1.5/pyproject.toml
--rw-r--r--   0 nix       (1000) nix       (1000)       38 2024-05-28 10:27:06.177603 nix_gpt_client-0.1.5/setup.cfg
-drwxr-xr-x   0 nix       (1000) nix       (1000)        0 2024-05-28 10:27:06.174270 nix_gpt_client-0.1.5/src/
--rw-r--r--   0 nix       (1000) nix       (1000)        0 2024-05-06 15:30:22.000000 nix_gpt_client-0.1.5/src/__init__.py
-drwxr-xr-x   0 nix       (1000) nix       (1000)        0 2024-05-28 10:27:06.174270 nix_gpt_client-0.1.5/src/nix/
--rw-r--r--   0 nix       (1000) nix       (1000)        0 2024-05-17 12:27:48.000000 nix_gpt_client-0.1.5/src/nix/__init__.py
-drwxr-xr-x   0 nix       (1000) nix       (1000)        0 2024-05-28 10:27:06.174270 nix_gpt_client-0.1.5/src/nix/gptclient/
--rw-r--r--   0 nix       (1000) nix       (1000)      169 2024-05-24 10:22:41.000000 nix_gpt_client-0.1.5/src/nix/gptclient/__init__.py
--rw-r--r--   0 nix       (1000) nix       (1000)     2509 2024-05-28 10:25:42.000000 nix_gpt_client-0.1.5/src/nix/gptclient/_gpt_client.py
--rw-r--r--   0 nix       (1000) nix       (1000)      483 2024-05-24 10:59:30.000000 nix_gpt_client-0.1.5/src/nix/gptclient/_tokens_count.py
--rw-r--r--   0 nix       (1000) nix       (1000)      681 2024-05-24 11:02:33.000000 nix_gpt_client-0.1.5/src/nix/gptclient/_types.py
--rw-r--r--   0 nix       (1000) nix       (1000)      654 2024-05-06 15:30:22.000000 nix_gpt_client-0.1.5/src/nix/gptclient/_validate.py
-drwxr-xr-x   0 nix       (1000) nix       (1000)        0 2024-05-28 10:27:06.177603 nix_gpt_client-0.1.5/src/nix_gpt_client.egg-info/
--rw-r--r--   0 nix       (1000) nix       (1000)     4187 2024-05-28 10:27:06.000000 nix_gpt_client-0.1.5/src/nix_gpt_client.egg-info/PKG-INFO
--rw-r--r--   0 nix       (1000) nix       (1000)      434 2024-05-28 10:27:06.000000 nix_gpt_client-0.1.5/src/nix_gpt_client.egg-info/SOURCES.txt
--rw-r--r--   0 nix       (1000) nix       (1000)        1 2024-05-28 10:27:06.000000 nix_gpt_client-0.1.5/src/nix_gpt_client.egg-info/dependency_links.txt
--rw-r--r--   0 nix       (1000) nix       (1000)       16 2024-05-28 10:27:06.000000 nix_gpt_client-0.1.5/src/nix_gpt_client.egg-info/requires.txt
--rw-r--r--   0 nix       (1000) nix       (1000)       13 2024-05-28 10:27:06.000000 nix_gpt_client-0.1.5/src/nix_gpt_client.egg-info/top_level.txt
+drwxr-xr-x   0 nix       (1000) nix       (1000)        0 2024-05-28 10:55:44.564840 nix_gpt_client-0.1.6/
+-rw-r--r--   0 nix       (1000) nix       (1000)     1063 2024-05-06 15:30:22.000000 nix_gpt_client-0.1.6/LICENCE
+-rw-r--r--   0 nix       (1000) nix       (1000)     4187 2024-05-28 10:55:44.564840 nix_gpt_client-0.1.6/PKG-INFO
+-rw-r--r--   0 nix       (1000) nix       (1000)     3470 2024-05-06 15:30:22.000000 nix_gpt_client-0.1.6/README.md
+-rw-r--r--   0 nix       (1000) nix       (1000)      848 2024-05-28 10:55:38.000000 nix_gpt_client-0.1.6/pyproject.toml
+-rw-r--r--   0 nix       (1000) nix       (1000)       38 2024-05-28 10:55:44.564840 nix_gpt_client-0.1.6/setup.cfg
+drwxr-xr-x   0 nix       (1000) nix       (1000)        0 2024-05-28 10:55:44.564840 nix_gpt_client-0.1.6/src/
+-rw-r--r--   0 nix       (1000) nix       (1000)        0 2024-05-06 15:30:22.000000 nix_gpt_client-0.1.6/src/__init__.py
+drwxr-xr-x   0 nix       (1000) nix       (1000)        0 2024-05-28 10:55:44.564840 nix_gpt_client-0.1.6/src/nix/
+-rw-r--r--   0 nix       (1000) nix       (1000)        0 2024-05-17 12:27:48.000000 nix_gpt_client-0.1.6/src/nix/__init__.py
+drwxr-xr-x   0 nix       (1000) nix       (1000)        0 2024-05-28 10:55:44.564840 nix_gpt_client-0.1.6/src/nix/gptclient/
+-rw-r--r--   0 nix       (1000) nix       (1000)      169 2024-05-24 10:22:41.000000 nix_gpt_client-0.1.6/src/nix/gptclient/__init__.py
+-rw-r--r--   0 nix       (1000) nix       (1000)     2511 2024-05-28 10:34:17.000000 nix_gpt_client-0.1.6/src/nix/gptclient/_gpt_client.py
+-rw-r--r--   0 nix       (1000) nix       (1000)      483 2024-05-24 10:59:30.000000 nix_gpt_client-0.1.6/src/nix/gptclient/_tokens_count.py
+-rw-r--r--   0 nix       (1000) nix       (1000)      681 2024-05-24 11:02:33.000000 nix_gpt_client-0.1.6/src/nix/gptclient/_types.py
+-rw-r--r--   0 nix       (1000) nix       (1000)      654 2024-05-06 15:30:22.000000 nix_gpt_client-0.1.6/src/nix/gptclient/_validate.py
+drwxr-xr-x   0 nix       (1000) nix       (1000)        0 2024-05-28 10:55:44.564840 nix_gpt_client-0.1.6/src/nix_gpt_client.egg-info/
+-rw-r--r--   0 nix       (1000) nix       (1000)     4187 2024-05-28 10:55:44.000000 nix_gpt_client-0.1.6/src/nix_gpt_client.egg-info/PKG-INFO
+-rw-r--r--   0 nix       (1000) nix       (1000)      434 2024-05-28 10:55:44.000000 nix_gpt_client-0.1.6/src/nix_gpt_client.egg-info/SOURCES.txt
+-rw-r--r--   0 nix       (1000) nix       (1000)        1 2024-05-28 10:55:44.000000 nix_gpt_client-0.1.6/src/nix_gpt_client.egg-info/dependency_links.txt
+-rw-r--r--   0 nix       (1000) nix       (1000)       16 2024-05-28 10:55:44.000000 nix_gpt_client-0.1.6/src/nix_gpt_client.egg-info/requires.txt
+-rw-r--r--   0 nix       (1000) nix       (1000)       13 2024-05-28 10:55:44.000000 nix_gpt_client-0.1.6/src/nix_gpt_client.egg-info/top_level.txt
```

### Comparing `nix_gpt_client-0.1.5/LICENCE` & `nix_gpt_client-0.1.6/LICENCE`

 * *Files identical despite different names*

### Comparing `nix_gpt_client-0.1.5/PKG-INFO` & `nix_gpt_client-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nix-gpt-client
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Python library for easy interaction with the GPT API, featuring typed requests and responses.
 Author-email: nks_nix <nikusunix@gmail.com>
 Maintainer-email: nks_nix <nikusunix@gmail.com>
 Project-URL: Homepage, https://github.com/nixnks/nix-gpt-client
 Project-URL: Documentation, https://readthedocs.org
 Project-URL: Repository, https://github.com/nixnks/nix-gpt-client.git
 Project-URL: Changelog, https://github.com/nixnks/nix-gpt-client/CHANGELOG.md
```

### Comparing `nix_gpt_client-0.1.5/README.md` & `nix_gpt_client-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `nix_gpt_client-0.1.5/pyproject.toml` & `nix_gpt_client-0.1.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nix-gpt-client"
-version = "0.1.5"
+version = "0.1.6"
 dependencies = [
     "openai",
     "tiktoken"
 ]
 requires-python = ">=3.11"
 authors = [
     { name = "nks_nix", email = "nikusunix@gmail.com" },
```

### Comparing `nix_gpt_client-0.1.5/src/nix/gptclient/_gpt_client.py` & `nix_gpt_client-0.1.6/src/nix/gptclient/_gpt_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,14 +58,14 @@
                 model=self._model,
                 temperature=self._temperature,
                 top_p=self._top_p,
                 presence_penalty=self._presence_penalty,
                 frequency_penalty=self._frequency_penalty,
                 response_format=self.response_format
             )
-            self.last_cost = response['cost']['total']
+            self.last_cost = response.usage.total_tokens
             if response.choices:
                 return response.choices[0].message.content
             else:
                 return None
         except openai.OpenAIError as error:
             raise error
```

### Comparing `nix_gpt_client-0.1.5/src/nix/gptclient/_types.py` & `nix_gpt_client-0.1.6/src/nix/gptclient/_types.py`

 * *Files identical despite different names*

### Comparing `nix_gpt_client-0.1.5/src/nix/gptclient/_validate.py` & `nix_gpt_client-0.1.6/src/nix/gptclient/_validate.py`

 * *Files identical despite different names*

### Comparing `nix_gpt_client-0.1.5/src/nix_gpt_client.egg-info/PKG-INFO` & `nix_gpt_client-0.1.6/src/nix_gpt_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nix-gpt-client
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Python library for easy interaction with the GPT API, featuring typed requests and responses.
 Author-email: nks_nix <nikusunix@gmail.com>
 Maintainer-email: nks_nix <nikusunix@gmail.com>
 Project-URL: Homepage, https://github.com/nixnks/nix-gpt-client
 Project-URL: Documentation, https://readthedocs.org
 Project-URL: Repository, https://github.com/nixnks/nix-gpt-client.git
 Project-URL: Changelog, https://github.com/nixnks/nix-gpt-client/CHANGELOG.md
```

