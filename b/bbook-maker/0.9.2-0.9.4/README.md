# Comparing `tmp/bbook_maker-0.9.2.tar.gz` & `tmp/bbook_maker-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbook_maker-0.9.2.tar", last modified: Thu May  2 00:33:57 2024, max compression
+gzip compressed data, was "bbook_maker-0.9.4.tar", last modified: Tue May 28 02:58:50 2024, max compression
```

## Comparing `bbook_maker-0.9.2.tar` & `bbook_maker-0.9.4.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0     1063 2024-05-02 00:33:54.058906 bbook_maker-0.9.2/LICENSE
--rw-r--r--   0        0        0    13660 2024-05-02 00:33:54.058906 bbook_maker-0.9.2/README.md
--rw-r--r--   0        0        0        0 2024-05-02 00:33:54.058906 bbook_maker-0.9.2/book_maker/__init__.py
--rw-r--r--   0        0        0       60 2024-05-02 00:33:54.058906 bbook_maker-0.9.2/book_maker/__main__.py
--rw-r--r--   0        0        0    15907 2024-05-02 00:33:54.058906 bbook_maker-0.9.2/book_maker/cli.py
--rw-r--r--   0        0        0      296 2024-05-02 00:33:54.058906 bbook_maker-0.9.2/book_maker/loader/__init__.py
--rw-r--r--   0        0        0      491 2024-05-02 00:33:54.058906 bbook_maker-0.9.2/book_maker/loader/base_loader.py
--rw-r--r--   0        0        0    20061 2024-05-02 00:33:54.058906 bbook_maker-0.9.2/book_maker/loader/epub_loader.py
--rw-r--r--   0        0        0     3641 2024-05-02 00:33:54.058906 bbook_maker-0.9.2/book_maker/loader/helper.py
--rw-r--r--   0        0        0    10383 2024-05-02 00:33:54.058906 bbook_maker-0.9.2/book_maker/loader/srt_loader.py
--rw-r--r--   0        0        0     4558 2024-05-02 00:33:54.058906 bbook_maker-0.9.2/book_maker/loader/txt_loader.py
--rw-r--r--   0        0        0    30290 2024-05-02 00:33:54.058906 bbook_maker-0.9.2/book_maker/obok.py
--rw-r--r--   0        0        0      895 2024-05-02 00:33:54.058906 bbook_maker-0.9.2/book_maker/translator/__init__.py
--rw-r--r--   0        0        0      391 2024-05-02 00:33:54.058906 bbook_maker-0.9.2/book_maker/translator/base_translator.py
--rw-r--r--   0        0        0     2115 2024-05-02 00:33:54.058906 bbook_maker-0.9.2/book_maker/translator/caiyun_translator.py
--rw-r--r--   0        0        0    10987 2024-05-02 00:33:54.058906 bbook_maker-0.9.2/book_maker/translator/chatgptapi_translator.py
--rw-r--r--   0        0        0     1445 2024-05-02 00:33:54.058906 bbook_maker-0.9.2/book_maker/translator/claude_translator.py
--rw-r--r--   0        0        0      846 2024-05-02 00:33:54.058906 bbook_maker-0.9.2/book_maker/translator/custom_api_translator.py
--rw-r--r--   0        0        0     1525 2024-05-02 00:33:54.058906 bbook_maker-0.9.2/book_maker/translator/deepl_free_translator.py
--rw-r--r--   0        0        0     2227 2024-05-02 00:33:54.058906 bbook_maker-0.9.2/book_maker/translator/deepl_translator.py
--rw-r--r--   0        0        0     2810 2024-05-02 00:33:54.058906 bbook_maker-0.9.2/book_maker/translator/gemini_translator.py
--rw-r--r--   0        0        0     1843 2024-05-02 00:33:54.058906 bbook_maker-0.9.2/book_maker/translator/google_translator.py
--rw-r--r--   0        0        0     2472 2024-05-02 00:33:54.058906 bbook_maker-0.9.2/book_maker/translator/litellm_translator.py
--rw-r--r--   0        0        0     2839 2024-05-02 00:33:54.058906 bbook_maker-0.9.2/book_maker/translator/tencent_transmart_translator.py
--rw-r--r--   0        0        0     4246 2024-05-02 00:33:54.058906 bbook_maker-0.9.2/book_maker/utils.py
--rw-r--r--   0        0        0     1146 2024-05-02 00:33:57.714899 bbook_maker-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     9507 2024-05-02 00:33:54.066906 bbook_maker-0.9.2/tests/test_integration.py
--rw-r--r--   0        0        0    14535 1970-01-01 00:00:00.000000 bbook_maker-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-28 02:58:41.176322 bbook_maker-0.9.4/LICENSE
+-rw-r--r--   0        0        0    13660 2024-05-28 02:58:41.176322 bbook_maker-0.9.4/README.md
+-rw-r--r--   0        0        0        0 2024-05-28 02:58:41.176322 bbook_maker-0.9.4/book_maker/__init__.py
+-rw-r--r--   0        0        0       60 2024-05-28 02:58:41.176322 bbook_maker-0.9.4/book_maker/__main__.py
+-rw-r--r--   0        0        0    16190 2024-05-28 02:58:41.176322 bbook_maker-0.9.4/book_maker/cli.py
+-rw-r--r--   0        0        0      296 2024-05-28 02:58:41.176322 bbook_maker-0.9.4/book_maker/loader/__init__.py
+-rw-r--r--   0        0        0      491 2024-05-28 02:58:41.176322 bbook_maker-0.9.4/book_maker/loader/base_loader.py
+-rw-r--r--   0        0        0    20061 2024-05-28 02:58:41.176322 bbook_maker-0.9.4/book_maker/loader/epub_loader.py
+-rw-r--r--   0        0        0     3641 2024-05-28 02:58:41.176322 bbook_maker-0.9.4/book_maker/loader/helper.py
+-rw-r--r--   0        0        0    10383 2024-05-28 02:58:41.176322 bbook_maker-0.9.4/book_maker/loader/srt_loader.py
+-rw-r--r--   0        0        0     4558 2024-05-28 02:58:41.176322 bbook_maker-0.9.4/book_maker/loader/txt_loader.py
+-rw-r--r--   0        0        0    30290 2024-05-28 02:58:41.176322 bbook_maker-0.9.4/book_maker/obok.py
+-rw-r--r--   0        0        0      980 2024-05-28 02:58:41.176322 bbook_maker-0.9.4/book_maker/translator/__init__.py
+-rw-r--r--   0        0        0      391 2024-05-28 02:58:41.176322 bbook_maker-0.9.4/book_maker/translator/base_translator.py
+-rw-r--r--   0        0        0     2115 2024-05-28 02:58:41.176322 bbook_maker-0.9.4/book_maker/translator/caiyun_translator.py
+-rw-r--r--   0        0        0    11012 2024-05-28 02:58:41.176322 bbook_maker-0.9.4/book_maker/translator/chatgptapi_translator.py
+-rw-r--r--   0        0        0     1445 2024-05-28 02:58:41.176322 bbook_maker-0.9.4/book_maker/translator/claude_translator.py
+-rw-r--r--   0        0        0      846 2024-05-28 02:58:41.176322 bbook_maker-0.9.4/book_maker/translator/custom_api_translator.py
+-rw-r--r--   0        0        0     1525 2024-05-28 02:58:41.176322 bbook_maker-0.9.4/book_maker/translator/deepl_free_translator.py
+-rw-r--r--   0        0        0     2227 2024-05-28 02:58:41.176322 bbook_maker-0.9.4/book_maker/translator/deepl_translator.py
+-rw-r--r--   0        0        0     2810 2024-05-28 02:58:41.176322 bbook_maker-0.9.4/book_maker/translator/gemini_translator.py
+-rw-r--r--   0        0        0     1843 2024-05-28 02:58:41.176322 bbook_maker-0.9.4/book_maker/translator/google_translator.py
+-rw-r--r--   0        0        0     1373 2024-05-28 02:58:41.176322 bbook_maker-0.9.4/book_maker/translator/groq_translator.py
+-rw-r--r--   0        0        0     2472 2024-05-28 02:58:41.176322 bbook_maker-0.9.4/book_maker/translator/litellm_translator.py
+-rw-r--r--   0        0        0     2839 2024-05-28 02:58:41.176322 bbook_maker-0.9.4/book_maker/translator/tencent_transmart_translator.py
+-rw-r--r--   0        0        0     4246 2024-05-28 02:58:41.176322 bbook_maker-0.9.4/book_maker/utils.py
+-rw-r--r--   0        0        0     1165 2024-05-28 02:58:50.392311 bbook_maker-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0     9507 2024-05-28 02:58:41.184322 bbook_maker-0.9.4/tests/test_integration.py
+-rw-r--r--   0        0        0    14562 1970-01-01 00:00:00.000000 bbook_maker-0.9.4/PKG-INFO
```

### Comparing `bbook_maker-0.9.2/LICENSE` & `bbook_maker-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bbook_maker-0.9.2/README.md` & `bbook_maker-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `bbook_maker-0.9.2/book_maker/cli.py` & `bbook_maker-0.9.4/book_maker/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,14 +110,22 @@
     parser.add_argument(
         "--gemini_key",
         dest="gemini_key",
         type=str,
         help="You can get Gemini Key from  https://makersuite.google.com/app/apikey",
     )
 
+    # for Groq
+    parser.add_argument(
+        "--groq_key",
+        dest="groq_key",
+        type=str,
+        help="You can get Groq Key from  https://console.groq.com/keys",
+    )
+
     parser.add_argument(
         "--test",
         dest="test",
         action="store_true",
         help="only the first 10 paragraphs will be translated, for testing",
     )
     parser.add_argument(
@@ -137,15 +145,15 @@
         metavar="MODEL",
         help="model to use, available: {%(choices)s}",
     )
     parser.add_argument(
         "--ollama_model",
         dest="ollama_model",
         type=str,
-        default="ollama_model",
+        default="",
         metavar="MODEL",
         help="use ollama",
     )
     parser.add_argument(
         "--language",
         type=str,
         choices=sorted(LANGUAGES.keys())
@@ -337,14 +345,16 @@
             raise Exception("Please provide claude key")
     elif options.model == "customapi":
         API_KEY = options.custom_api or env.get("BBM_CUSTOM_API")
         if not API_KEY:
             raise Exception("Please provide custom translate api")
     elif options.model == "gemini":
         API_KEY = options.gemini_key or env.get("BBM_GOOGLE_GEMINI_KEY")
+    elif options.model == "groq":
+        API_KEY = options.groq_key or env.get("BBM_GROQ_API_KEY")
     else:
         API_KEY = ""
 
     if options.book_from == "kobo":
         from book_maker import obok
 
         device_path = options.device_path
@@ -419,15 +429,15 @@
         assert options.model in [
             "chatgptapi",
             "gpt4",
         ], "only support chatgptapi for deployment_id"
         if not options.api_base:
             raise ValueError("`api_base` must be provided when using `deployment_id`")
         e.translate_model.set_deployment_id(options.deployment_id)
-    if options.model == "openai":
+    if options.model in ("openai", "groq"):
         # Currently only supports `openai` when you also have --model_list set
         if options.model_list:
             e.translate_model.set_model_list(options.model_list.split(","))
         else:
             raise ValueError(
                 "When using `openai` model, you must also provide `--model_list`. For default model sets use `--model chatgptapi` or `--model gpt4`",
             )
```

### Comparing `bbook_maker-0.9.2/book_maker/loader/epub_loader.py` & `bbook_maker-0.9.4/book_maker/loader/epub_loader.py`

 * *Files identical despite different names*

### Comparing `bbook_maker-0.9.2/book_maker/loader/helper.py` & `bbook_maker-0.9.4/book_maker/loader/helper.py`

 * *Files identical despite different names*

### Comparing `bbook_maker-0.9.2/book_maker/loader/srt_loader.py` & `bbook_maker-0.9.4/book_maker/loader/srt_loader.py`

 * *Files identical despite different names*

### Comparing `bbook_maker-0.9.2/book_maker/loader/txt_loader.py` & `bbook_maker-0.9.4/book_maker/loader/txt_loader.py`

 * *Files identical despite different names*

### Comparing `bbook_maker-0.9.2/book_maker/obok.py` & `bbook_maker-0.9.4/book_maker/obok.py`

 * *Files identical despite different names*

### Comparing `bbook_maker-0.9.2/book_maker/translator/__init__.py` & `bbook_maker-0.9.4/book_maker/translator/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from book_maker.translator.caiyun_translator import Caiyun
 from book_maker.translator.chatgptapi_translator import ChatGPTAPI
 from book_maker.translator.deepl_translator import DeepL
 from book_maker.translator.deepl_free_translator import DeepLFree
 from book_maker.translator.google_translator import Google
 from book_maker.translator.claude_translator import Claude
 from book_maker.translator.gemini_translator import Gemini
+from book_maker.translator.groq_translator import GroqClient
 from book_maker.translator.tencent_transmart_translator import TencentTranSmart
 from book_maker.translator.custom_api_translator import CustomAPI
 
 MODEL_DICT = {
     "openai": ChatGPTAPI,
     "chatgptapi": ChatGPTAPI,
     "gpt4": ChatGPTAPI,
     "google": Google,
     "caiyun": Caiyun,
     "deepl": DeepL,
     "deeplfree": DeepLFree,
     "claude": Claude,
     "gemini": Gemini,
+    "groq": GroqClient,
     "tencentransmart": TencentTranSmart,
     "customapi": CustomAPI,
     # add more here
 }
```

### Comparing `bbook_maker-0.9.2/book_maker/translator/caiyun_translator.py` & `bbook_maker-0.9.4/book_maker/translator/caiyun_translator.py`

 * *Files identical despite different names*

### Comparing `bbook_maker-0.9.2/book_maker/translator/chatgptapi_translator.py` & `bbook_maker-0.9.4/book_maker/translator/chatgptapi_translator.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     "gpt-3.5-turbo-0301",
     "gpt-3.5-turbo-0125",
 ]
 GPT4_MODEL_LIST = [
     "gpt-4-1106-preview",
     "gpt-4",
     "gpt-4-32k",
+    "gpt-4o-2024-05-13",
     "gpt-4-0613",
     "gpt-4-32k-0613",
 ]
 
 
 class ChatGPTAPI(Base):
     DEFAULT_PROMPT = "Please help me to translate,`{text}` to {language}, please return only translated content not include the origin text"
```

### Comparing `bbook_maker-0.9.2/book_maker/translator/claude_translator.py` & `bbook_maker-0.9.4/book_maker/translator/claude_translator.py`

 * *Files identical despite different names*

### Comparing `bbook_maker-0.9.2/book_maker/translator/custom_api_translator.py` & `bbook_maker-0.9.4/book_maker/translator/custom_api_translator.py`

 * *Files identical despite different names*

### Comparing `bbook_maker-0.9.2/book_maker/translator/deepl_free_translator.py` & `bbook_maker-0.9.4/book_maker/translator/deepl_free_translator.py`

 * *Files identical despite different names*

### Comparing `bbook_maker-0.9.2/book_maker/translator/deepl_translator.py` & `bbook_maker-0.9.4/book_maker/translator/deepl_translator.py`

 * *Files identical despite different names*

### Comparing `bbook_maker-0.9.2/book_maker/translator/gemini_translator.py` & `bbook_maker-0.9.4/book_maker/translator/gemini_translator.py`

 * *Files identical despite different names*

### Comparing `bbook_maker-0.9.2/book_maker/translator/google_translator.py` & `bbook_maker-0.9.4/book_maker/translator/google_translator.py`

 * *Files identical despite different names*

### Comparing `bbook_maker-0.9.2/book_maker/translator/litellm_translator.py` & `bbook_maker-0.9.4/book_maker/translator/litellm_translator.py`

 * *Files identical despite different names*

### Comparing `bbook_maker-0.9.2/book_maker/translator/tencent_transmart_translator.py` & `bbook_maker-0.9.4/book_maker/translator/tencent_transmart_translator.py`

 * *Files identical despite different names*

### Comparing `bbook_maker-0.9.2/book_maker/utils.py` & `bbook_maker-0.9.4/book_maker/utils.py`

 * *Files identical despite different names*

### Comparing `bbook_maker-0.9.2/pyproject.toml` & `bbook_maker-0.9.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -22,16 +22,17 @@
     "litellm",
     "openai>=1.1.1",
     "PyDeepLX",
     "requests",
     "rich",
     "tiktoken",
     "tqdm",
+    "groq>=0.5.0",
 ]
-version = "0.9.2"
+version = "0.9.4"
 
 [project.license]
 text = "MIT"
 
 [project.scripts]
 bbook_maker = "book_maker.cli:main"
```

### Comparing `bbook_maker-0.9.2/tests/test_integration.py` & `bbook_maker-0.9.4/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `bbook_maker-0.9.2/PKG-INFO` & `bbook_maker-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbook-maker
-Version: 0.9.2
+Version: 0.9.4
 Summary: The bilingual_book_maker is an AI translation tool that uses ChatGPT to assist users in creating multi-language versions of epub/txt files and books.
 Author-Email: yihong0618 <zouzou0208@gmail.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Project-URL: Homepage, https://github.com/yihong0618/bilingual_book_maker
@@ -18,14 +18,15 @@
 Requires-Dist: litellm
 Requires-Dist: openai>=1.1.1
 Requires-Dist: PyDeepLX
 Requires-Dist: requests
 Requires-Dist: rich
 Requires-Dist: tiktoken
 Requires-Dist: tqdm
+Requires-Dist: groq>=0.5.0
 Description-Content-Type: text/markdown
 
 **[中文](./README-CN.md) | English**
 [![litellm](https://img.shields.io/badge/%20%F0%9F%9A%85%20liteLLM-OpenAI%7CAzure%7CAnthropic%7CPalm%7CCohere%7CReplicate%7CHugging%20Face-blue?color=green)](https://github.com/BerriAI/litellm)
 
 # bilingual_book_maker
 The bilingual_book_maker is an AI translation tool that uses ChatGPT to assist users in creating multi-language versions of epub/txt/srt files and books. This tool is exclusively designed for translating epub books that have entered the public domain and is not intended for copyrighted works. Before using this tool, please review the project's **[disclaimer](./disclaimer.md)**.
```

