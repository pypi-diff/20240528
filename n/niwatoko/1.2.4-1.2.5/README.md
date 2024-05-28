# Comparing `tmp/niwatoko-1.2.4.tar.gz` & `tmp/niwatoko-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "niwatoko-1.2.4.tar", last modified: Sat May 25 04:20:22 2024, max compression
+gzip compressed data, was "niwatoko-1.2.5.tar", last modified: Tue May 28 19:10:43 2024, max compression
```

## Comparing `niwatoko-1.2.4.tar` & `niwatoko-1.2.5.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-25 04:20:22.215102 niwatoko-1.2.4/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    11356 2024-05-07 05:52:57.000000 niwatoko-1.2.4/LICENSE
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    16858 2024-05-25 04:20:22.214732 niwatoko-1.2.4/PKG-INFO
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    15972 2024-05-14 05:32:42.000000 niwatoko-1.2.4/README.md
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-25 04:20:22.209612 niwatoko-1.2.4/niwatoko/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)      166 2024-05-20 02:01:29.000000 niwatoko-1.2.4/niwatoko/__init__.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    25194 2024-05-24 20:49:42.000000 niwatoko-1.2.4/niwatoko/cli.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-25 04:20:22.208166 niwatoko-1.2.4/niwatoko/foundation_model/
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-25 04:20:22.208202 niwatoko-1.2.4/niwatoko/foundation_model/interpretation/
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-25 04:20:22.211258 niwatoko-1.2.4/niwatoko/foundation_model/interpretation/llm/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1346 2024-05-20 02:01:29.000000 niwatoko-1.2.4/niwatoko/foundation_model/interpretation/llm/claude.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2289 2024-05-20 03:04:54.000000 niwatoko-1.2.4/niwatoko/foundation_model/interpretation/llm/gpt.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-25 04:20:22.211533 niwatoko-1.2.4/niwatoko/grammar/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1509 2024-05-20 02:55:54.000000 niwatoko-1.2.4/niwatoko/grammar/system.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       33 2024-05-14 05:32:42.000000 niwatoko-1.2.4/niwatoko/temp.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-25 04:20:22.210996 niwatoko-1.2.4/niwatoko.egg-info/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    16858 2024-05-25 04:20:22.000000 niwatoko-1.2.4/niwatoko.egg-info/PKG-INFO
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1026 2024-05-25 04:20:22.000000 niwatoko-1.2.4/niwatoko.egg-info/SOURCES.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)        1 2024-05-25 04:20:22.000000 niwatoko-1.2.4/niwatoko.egg-info/dependency_links.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       47 2024-05-25 04:20:22.000000 niwatoko-1.2.4/niwatoko.egg-info/entry_points.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       80 2024-05-25 04:20:22.000000 niwatoko-1.2.4/niwatoko.egg-info/requires.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       15 2024-05-25 04:20:22.000000 niwatoko-1.2.4/niwatoko.egg-info/top_level.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       38 2024-05-25 04:20:22.215152 niwatoko-1.2.4/setup.cfg
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1775 2024-05-25 04:20:03.000000 niwatoko-1.2.4/setup.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-25 04:20:22.212662 niwatoko-1.2.4/tests/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     5897 2024-05-08 23:04:24.000000 niwatoko-1.2.4/tests/README.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2077 2024-05-07 02:46:41.000000 niwatoko-1.2.4/tests/__init__.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     3754 2024-05-08 23:03:26.000000 niwatoko-1.2.4/tests/test_compiler.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     4529 2024-05-08 23:03:26.000000 niwatoko-1.2.4/tests/test_compiler.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     3940 2024-05-08 23:04:26.000000 niwatoko-1.2.4/tests/test_compiler_v1_2.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-25 04:20:22.214505 niwatoko-1.2.4/tests/test_docs/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2747 2024-05-07 02:46:41.000000 niwatoko-1.2.4/tests/test_docs/__init__.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2030 2024-05-14 05:32:42.000000 niwatoko-1.2.4/tests/test_docs/output copy.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     3118 2024-05-14 05:32:42.000000 niwatoko-1.2.4/tests/test_docs/output.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     4172 2024-05-14 05:32:42.000000 niwatoko-1.2.4/tests/test_docs/output.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1733 2024-05-14 05:32:42.000000 niwatoko-1.2.4/tests/test_docs/output_.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2609 2024-05-07 05:48:44.000000 niwatoko-1.2.4/tests/test_docs/test_doc1.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2853 2024-05-07 05:48:44.000000 niwatoko-1.2.4/tests/test_docs/test_doc2.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2625 2024-05-07 05:48:44.000000 niwatoko-1.2.4/tests/test_docs/test_doc3.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1678 2024-05-07 22:46:07.000000 niwatoko-1.2.4/tests/test_docs/test_gen_github_issue.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1950 2024-05-07 22:46:07.000000 niwatoko-1.2.4/tests/test_docs/test_gen_grimoire.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1909 2024-05-07 22:46:07.000000 niwatoko-1.2.4/tests/test_docs/test_gen_grimoire2.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1850 2024-05-07 22:46:07.000000 niwatoko-1.2.4/tests/test_docs/test_gen_grimoire_en.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     5307 2024-05-07 05:52:23.000000 niwatoko-1.2.4/tests/test_docs/test_gen_zoltraak_pypi.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     6179 2024-05-14 05:32:42.000000 niwatoko-1.2.4/tests/test_docs/test_import_function.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2216 2024-05-07 02:46:41.000000 niwatoko-1.2.4/tests/test_interpreter.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2632 2024-05-07 02:46:41.000000 niwatoko-1.2.4/tests/test_parser.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-28 19:10:43.143610 niwatoko-1.2.5/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    11356 2024-05-07 05:52:57.000000 niwatoko-1.2.5/LICENSE
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    16938 2024-05-28 19:10:43.143422 niwatoko-1.2.5/PKG-INFO
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    16052 2024-05-26 09:22:11.000000 niwatoko-1.2.5/README.md
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-28 19:10:43.137163 niwatoko-1.2.5/niwatoko/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      166 2024-05-20 02:01:29.000000 niwatoko-1.2.5/niwatoko/__init__.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    25520 2024-05-28 19:09:01.000000 niwatoko-1.2.5/niwatoko/cli.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-28 19:10:43.135615 niwatoko-1.2.5/niwatoko/foundation_model/
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-28 19:10:43.135657 niwatoko-1.2.5/niwatoko/foundation_model/interpretation/
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-28 19:10:43.138283 niwatoko-1.2.5/niwatoko/foundation_model/interpretation/llm/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1346 2024-05-20 02:01:29.000000 niwatoko-1.2.5/niwatoko/foundation_model/interpretation/llm/claude.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2289 2024-05-26 09:22:11.000000 niwatoko-1.2.5/niwatoko/foundation_model/interpretation/llm/gpt.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-28 19:10:43.138503 niwatoko-1.2.5/niwatoko/grammar/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1509 2024-05-26 09:22:11.000000 niwatoko-1.2.5/niwatoko/grammar/system.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       33 2024-05-14 05:32:42.000000 niwatoko-1.2.5/niwatoko/temp.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-28 19:10:43.137910 niwatoko-1.2.5/niwatoko.egg-info/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    16938 2024-05-28 19:10:43.000000 niwatoko-1.2.5/niwatoko.egg-info/PKG-INFO
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1026 2024-05-28 19:10:43.000000 niwatoko-1.2.5/niwatoko.egg-info/SOURCES.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)        1 2024-05-28 19:10:43.000000 niwatoko-1.2.5/niwatoko.egg-info/dependency_links.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       47 2024-05-28 19:10:43.000000 niwatoko-1.2.5/niwatoko.egg-info/entry_points.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       80 2024-05-28 19:10:43.000000 niwatoko-1.2.5/niwatoko.egg-info/requires.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       15 2024-05-28 19:10:43.000000 niwatoko-1.2.5/niwatoko.egg-info/top_level.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       38 2024-05-28 19:10:43.143642 niwatoko-1.2.5/setup.cfg
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1775 2024-05-28 19:10:21.000000 niwatoko-1.2.5/setup.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-28 19:10:43.140180 niwatoko-1.2.5/tests/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     5897 2024-05-08 23:04:24.000000 niwatoko-1.2.5/tests/README.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2077 2024-05-07 02:46:41.000000 niwatoko-1.2.5/tests/__init__.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     3754 2024-05-08 23:03:26.000000 niwatoko-1.2.5/tests/test_compiler.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     4529 2024-05-08 23:03:26.000000 niwatoko-1.2.5/tests/test_compiler.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     3940 2024-05-08 23:04:26.000000 niwatoko-1.2.5/tests/test_compiler_v1_2.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-28 19:10:43.143106 niwatoko-1.2.5/tests/test_docs/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2747 2024-05-07 02:46:41.000000 niwatoko-1.2.5/tests/test_docs/__init__.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2030 2024-05-14 05:32:42.000000 niwatoko-1.2.5/tests/test_docs/output copy.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     3118 2024-05-14 05:32:42.000000 niwatoko-1.2.5/tests/test_docs/output.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     4172 2024-05-14 05:32:42.000000 niwatoko-1.2.5/tests/test_docs/output.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1733 2024-05-14 05:32:42.000000 niwatoko-1.2.5/tests/test_docs/output_.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2609 2024-05-07 05:48:44.000000 niwatoko-1.2.5/tests/test_docs/test_doc1.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2853 2024-05-07 05:48:44.000000 niwatoko-1.2.5/tests/test_docs/test_doc2.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2625 2024-05-07 05:48:44.000000 niwatoko-1.2.5/tests/test_docs/test_doc3.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1678 2024-05-07 22:46:07.000000 niwatoko-1.2.5/tests/test_docs/test_gen_github_issue.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1950 2024-05-07 22:46:07.000000 niwatoko-1.2.5/tests/test_docs/test_gen_grimoire.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1909 2024-05-07 22:46:07.000000 niwatoko-1.2.5/tests/test_docs/test_gen_grimoire2.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1850 2024-05-07 22:46:07.000000 niwatoko-1.2.5/tests/test_docs/test_gen_grimoire_en.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     5307 2024-05-07 05:52:23.000000 niwatoko-1.2.5/tests/test_docs/test_gen_zoltraak_pypi.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     6179 2024-05-14 05:32:42.000000 niwatoko-1.2.5/tests/test_docs/test_import_function.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2216 2024-05-07 02:46:41.000000 niwatoko-1.2.5/tests/test_interpreter.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2632 2024-05-07 02:46:41.000000 niwatoko-1.2.5/tests/test_parser.py
```

### Comparing `niwatoko-1.2.4/LICENSE` & `niwatoko-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.4/PKG-INFO` & `niwatoko-1.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niwatoko
-Version: 1.2.4
+Version: 1.2.5
 Summary: 自然言語でプログラミングを行うことができる新しいプログラミング言語
 Home-page: https://niwatoko2.vercel.app/
 Author: dai-motoki
 Author-email: dai.motoki1123@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Japanese
@@ -16,15 +16,21 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# 要件定義書: niwatoko - 自然言語プログラミング言語のPythonパッケージ
+# 抽象プログラミング言語 にわとこ
+
+## 利用方法は以下URLをチェックしてください。
+https://niwatoko2.vercel.app/
+
+
+## 以下は開発者向け
 
 ## 1. 目的
 niwatoko は、自然言語でプログラミングを行うことができる新しいプログラミング言語です。このプロジェクトの目的は、niwatoko のPythonパッケージを開発し、ユーザーが自然言語を使ってプログラムを記述し、実行できるようにすることです。パッケージには、自然言語処理のための認識系AIと、プログラムの出力を生成するための生成AI（テキスト生成や画像生成）が組み込まれます。
 
 ## 2. パッケージの基本構造
 ```
 niwatoko/
```

### Comparing `niwatoko-1.2.4/README.md` & `niwatoko-1.2.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,14 @@
-# 要件定義書: niwatoko - 自然言語プログラミング言語のPythonパッケージ
+# 抽象プログラミング言語 にわとこ
+
+## 利用方法は以下URLをチェックしてください。
+https://niwatoko2.vercel.app/
+
+
+## 以下は開発者向け
 
 ## 1. 目的
 niwatoko は、自然言語でプログラミングを行うことができる新しいプログラミング言語です。このプロジェクトの目的は、niwatoko のPythonパッケージを開発し、ユーザーが自然言語を使ってプログラムを記述し、実行できるようにすることです。パッケージには、自然言語処理のための認識系AIと、プログラムの出力を生成するための生成AI（テキスト生成や画像生成）が組み込まれます。
 
 ## 2. パッケージの基本構造
 ```
 niwatoko/
```

### Comparing `niwatoko-1.2.4/niwatoko/cli.py` & `niwatoko-1.2.5/niwatoko/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,47 +52,15 @@
 
     # ぐるぐるアニメーションを表示するスレッドを開始
     done = False
     spinner = threading.Thread(target=spin, args=(lambda: done,))
     spinner.start()
 
     while True:
-        if model == 'openai' or model == 'openai-gpt-turbo':
-            generated_code = gpt_generate_response(
-                model="gpt-4-turbo-2024-04-09",
-                prompt=processed_content,
-                max_tokens=1000,
-                temperature=0.5,
-            )
-        elif model == 'openai-gpt4o':
-            generated_code = gpt_generate_response_gpt4o(
-                prompt=processed_content,
-                max_tokens=2048,
-                temperature=0.5,
-            )
-        elif model in ['gemini-1.5-pro', 'gemini-1.5-flash']:
-            generated_code = generate_gemini_response(
-                model=model,
-                prompt=processed_content,
-            )
-        else:
-            if model == 'claude-sonnet':
-                claude_model = 'claude-3-sonnet-20240229'
-            elif model == 'claude-opus':
-                claude_model = 'claude-3-opus-20240229'
-            else:
-                claude_model = 'claude-3-haiku-20240307'  # デフォルトはhaiku
-            
-            print("model:", claude_model)
-            generated_code = generate_response(
-                model=claude_model,
-                prompt=processed_content,
-                max_tokens=4000,
-                temperature=0.2,
-            )
+        generated_code = generate_code(model, processed_content)
         
         # ぐるぐるアニメーションを停止
         done = True
         spinner.join()
 
         if output:
             with open(output, 'w', encoding = "utf-8") as file:
@@ -101,26 +69,70 @@
                 code_content = generated_code[code_block_start:code_block_end]    # コードブロックの内容を抽出する
                 file.write(code_content)                                          # 抽出したコードをファイルに書き込む
                 print(f"生成されたコードを {output} に書き出しました。")
                 print(f"Generated code has been written to {output}.")
                 print("生成されたコードを実行します。")                             # 生成されたコードを実行する旨を表示
                 exec_globals = {}                                                 # 実行環境のグローバル変数を初期化
                 exec_locals = {}                                                  # 実行環境のローカル変数を初期化
-                try:
-                    exec(code_content, exec_globals, exec_locals)                 # execを使用して生成されたコードを実行
-                    print("生成されたコードの実行が成功しました。")                 # 実行成功のメッセージを表示
-                    break  # 成功した場合、ループを抜ける
-                except Exception as e:
-                    print("生成されたコードの実行に失敗しました。")                 # 実行失敗のメッセージを表示
-                    print("エラー:", str(e))                                      # エラーメッセージを表示
-                    user_input = input("エラーが発生しました。自動修正を試みますか？ (y/n): ")  # 自動修正を試みるかユーザーに確認
-                    if user_input.lower() == 'y':
-                        processed_content += f"\n# エラーが出ました。修正してください: {str(e)}"  # エラーをプロンプトに追加
-                    else:
-                        print("自動修正をスキップします。")                         # 自動修正をスキップする旨を表示
+            try:
+                exec(code_content, exec_globals, exec_locals)                 # execを使用して生成されたコードを実行
+                print("生成されたコードの実行が成功しました。")                 # 実行成功のメッセージを表示
+                break  # 成功した場合、ループを抜ける
+            except Exception as e:
+                print("生成されたコードの実行に失敗しました。")                 # 実行失敗のメッセージを表示
+                print("エラー:", str(e))                                      # エラーメッセージを表示
+                # エラー要因を想定してテキストで出力
+                error_analysis = generate_code(
+                    model=model,
+                    content=f"以下のエラーが発生しました。考えられる要因を分析してください。\n\nエラー: {str(e)}"
+                )
+                print("エラー要因の分析結果:", error_analysis)
+                user_input = input("エラーが発生しました。自動修正を試みますか？ (y/n): ")  # 自動修正を試みるかユーザーに確認
+                if user_input.lower() == 'y':
+                    # エラー要因の分析結果をプロンプトに追加
+                    processed_content += f"\n# エラーが出ました。修正してください: {str(e)}\n# エラー要因の分析:\n{error_analysis}"
+                else:
+                    print("自動修正をスキップします。")                         # 自動修正をスキップする旨を表示
+
+
+
+def generate_code(model, content):
+    if model == 'openai' or model == 'openai-gpt-turbo':
+        return gpt_generate_response(
+            model="gpt-4-turbo-2024-04-09",
+            prompt=content,
+            max_tokens=1000,
+            temperature=0.5,
+        )
+    elif model == 'openai-gpt4o':
+        return gpt_generate_response_gpt4o(
+            prompt=content,
+            max_tokens=2048,
+            temperature=0.5,
+        )
+    elif model in ['gemini-1.5-pro', 'gemini-1.5-flash']:
+        return generate_gemini_response(
+            model=model,
+            prompt=content,
+        )
+    else:
+        if model == 'claude-sonnet':
+            claude_model = 'claude-3-sonnet-20240229'
+        elif model == 'claude-opus':
+            claude_model = 'claude-3-opus-20240229'
+        else:
+            claude_model = 'claude-3-haiku-20240307'  # デフォルトはhaiku
+        
+        print("model:", claude_model)
+        return generate_response(
+            model=claude_model,
+            prompt=content,
+            max_tokens=4000,
+            temperature=0.2,
+        )
 
 def spin(done):
     """
     ぐるぐるアニメーションを表示する関数
     Args:
         done (function): アニメーションを停止するかどうかを判定する関数
     """
@@ -234,15 +246,15 @@
         import_path (str): インポートするファイルのパス
         line (str): インポート文の行
 
     Returns:
         list: 処理後の出力行のリスト
     """
     import_path = import_path[4:-1] + '.md'  # 拡張子を追加
-    print(import_path)
+    # print(import_path)
     import_content = get_file_content(import_path)
     return [line, '```\n', import_content, '```\n']
 
 def process_py_import(import_path, line):
     """
     Pythonファイルのインポートを処理する関数
 
@@ -403,16 +415,16 @@
             }
         ],
         "max_tokens": 100
     }
 
     response = requests.post("https://api.openai.com/v1/chat/completions", headers=headers, json=payload)
     content = response.json().get('choices', [{}])[0].get('message', {}).get('content', '')
-    print(content)
-    print('')
+    # print(content)
+    # print('')
 
     return content
 
 import cv2
 from moviepy.editor import VideoFileClip
 import time
 import base64
```

### Comparing `niwatoko-1.2.4/niwatoko/foundation_model/interpretation/llm/claude.py` & `niwatoko-1.2.5/niwatoko/foundation_model/interpretation/llm/claude.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.4/niwatoko/foundation_model/interpretation/llm/gpt.py` & `niwatoko-1.2.5/niwatoko/foundation_model/interpretation/llm/gpt.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.4/niwatoko/grammar/system.md` & `niwatoko-1.2.5/niwatoko/grammar/system.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.4/niwatoko.egg-info/PKG-INFO` & `niwatoko-1.2.5/niwatoko.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niwatoko
-Version: 1.2.4
+Version: 1.2.5
 Summary: 自然言語でプログラミングを行うことができる新しいプログラミング言語
 Home-page: https://niwatoko2.vercel.app/
 Author: dai-motoki
 Author-email: dai.motoki1123@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Japanese
@@ -16,15 +16,21 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# 要件定義書: niwatoko - 自然言語プログラミング言語のPythonパッケージ
+# 抽象プログラミング言語 にわとこ
+
+## 利用方法は以下URLをチェックしてください。
+https://niwatoko2.vercel.app/
+
+
+## 以下は開発者向け
 
 ## 1. 目的
 niwatoko は、自然言語でプログラミングを行うことができる新しいプログラミング言語です。このプロジェクトの目的は、niwatoko のPythonパッケージを開発し、ユーザーが自然言語を使ってプログラムを記述し、実行できるようにすることです。パッケージには、自然言語処理のための認識系AIと、プログラムの出力を生成するための生成AI（テキスト生成や画像生成）が組み込まれます。
 
 ## 2. パッケージの基本構造
 ```
 niwatoko/
```

### Comparing `niwatoko-1.2.4/niwatoko.egg-info/SOURCES.txt` & `niwatoko-1.2.5/niwatoko.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.4/setup.py` & `niwatoko-1.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # niwatoko - 自然言語プログラミング言語のPythonパッケージのsetup.pyファイルです。
 # このファイルはパッケージのインストールや配布に必要な情報を含んでいます。
 
 from setuptools import setup, find_packages
 
 setup(
     name='niwatoko',
-    version='1.2.4',
+    version='1.2.5',
     description='自然言語でプログラミングを行うことができる新しいプログラミング言語',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='dai-motoki',
     author_email='dai.motoki1123@gmail.com',
     url='https://niwatoko2.vercel.app/',
     packages=find_packages(),
```

### Comparing `niwatoko-1.2.4/tests/README.md` & `niwatoko-1.2.5/tests/README.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.4/tests/__init__.py` & `niwatoko-1.2.5/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.4/tests/test_compiler.md` & `niwatoko-1.2.5/tests/test_compiler.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.4/tests/test_compiler.py` & `niwatoko-1.2.5/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.4/tests/test_compiler_v1_2.py` & `niwatoko-1.2.5/tests/test_compiler_v1_2.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.4/tests/test_docs/__init__.py` & `niwatoko-1.2.5/tests/test_docs/__init__.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.4/tests/test_docs/output copy.md` & `niwatoko-1.2.5/tests/test_docs/output copy.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.4/tests/test_docs/output.md` & `niwatoko-1.2.5/tests/test_docs/output.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.4/tests/test_docs/output.py` & `niwatoko-1.2.5/tests/test_docs/output.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.4/tests/test_docs/output_.md` & `niwatoko-1.2.5/tests/test_docs/output_.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.4/tests/test_docs/test_doc1.md` & `niwatoko-1.2.5/tests/test_docs/test_doc1.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.4/tests/test_docs/test_doc2.md` & `niwatoko-1.2.5/tests/test_docs/test_doc2.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.4/tests/test_docs/test_doc3.md` & `niwatoko-1.2.5/tests/test_docs/test_doc3.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.4/tests/test_docs/test_gen_github_issue.md` & `niwatoko-1.2.5/tests/test_docs/test_gen_github_issue.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.4/tests/test_docs/test_gen_grimoire.md` & `niwatoko-1.2.5/tests/test_docs/test_gen_grimoire.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.4/tests/test_docs/test_gen_grimoire2.md` & `niwatoko-1.2.5/tests/test_docs/test_gen_grimoire2.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.4/tests/test_docs/test_gen_grimoire_en.md` & `niwatoko-1.2.5/tests/test_docs/test_gen_grimoire_en.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.4/tests/test_docs/test_gen_zoltraak_pypi.md` & `niwatoko-1.2.5/tests/test_docs/test_gen_zoltraak_pypi.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.4/tests/test_docs/test_import_function.md` & `niwatoko-1.2.5/tests/test_docs/test_import_function.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.4/tests/test_interpreter.py` & `niwatoko-1.2.5/tests/test_interpreter.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.4/tests/test_parser.py` & `niwatoko-1.2.5/tests/test_parser.py`

 * *Files identical despite different names*

