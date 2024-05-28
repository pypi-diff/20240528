# Comparing `tmp/niwatoko-1.2.5.tar.gz` & `tmp/niwatoko-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "niwatoko-1.2.5.tar", last modified: Tue May 28 19:10:43 2024, max compression
+gzip compressed data, was "niwatoko-1.2.6.tar", last modified: Tue May 28 19:13:39 2024, max compression
```

## Comparing `niwatoko-1.2.5.tar` & `niwatoko-1.2.6.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-28 19:10:43.143610 niwatoko-1.2.5/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    11356 2024-05-07 05:52:57.000000 niwatoko-1.2.5/LICENSE
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    16938 2024-05-28 19:10:43.143422 niwatoko-1.2.5/PKG-INFO
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    16052 2024-05-26 09:22:11.000000 niwatoko-1.2.5/README.md
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-28 19:10:43.137163 niwatoko-1.2.5/niwatoko/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)      166 2024-05-20 02:01:29.000000 niwatoko-1.2.5/niwatoko/__init__.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    25520 2024-05-28 19:09:01.000000 niwatoko-1.2.5/niwatoko/cli.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-28 19:10:43.135615 niwatoko-1.2.5/niwatoko/foundation_model/
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-28 19:10:43.135657 niwatoko-1.2.5/niwatoko/foundation_model/interpretation/
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-28 19:10:43.138283 niwatoko-1.2.5/niwatoko/foundation_model/interpretation/llm/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1346 2024-05-20 02:01:29.000000 niwatoko-1.2.5/niwatoko/foundation_model/interpretation/llm/claude.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2289 2024-05-26 09:22:11.000000 niwatoko-1.2.5/niwatoko/foundation_model/interpretation/llm/gpt.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-28 19:10:43.138503 niwatoko-1.2.5/niwatoko/grammar/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1509 2024-05-26 09:22:11.000000 niwatoko-1.2.5/niwatoko/grammar/system.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       33 2024-05-14 05:32:42.000000 niwatoko-1.2.5/niwatoko/temp.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-28 19:10:43.137910 niwatoko-1.2.5/niwatoko.egg-info/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    16938 2024-05-28 19:10:43.000000 niwatoko-1.2.5/niwatoko.egg-info/PKG-INFO
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1026 2024-05-28 19:10:43.000000 niwatoko-1.2.5/niwatoko.egg-info/SOURCES.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)        1 2024-05-28 19:10:43.000000 niwatoko-1.2.5/niwatoko.egg-info/dependency_links.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       47 2024-05-28 19:10:43.000000 niwatoko-1.2.5/niwatoko.egg-info/entry_points.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       80 2024-05-28 19:10:43.000000 niwatoko-1.2.5/niwatoko.egg-info/requires.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       15 2024-05-28 19:10:43.000000 niwatoko-1.2.5/niwatoko.egg-info/top_level.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       38 2024-05-28 19:10:43.143642 niwatoko-1.2.5/setup.cfg
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1775 2024-05-28 19:10:21.000000 niwatoko-1.2.5/setup.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-28 19:10:43.140180 niwatoko-1.2.5/tests/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     5897 2024-05-08 23:04:24.000000 niwatoko-1.2.5/tests/README.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2077 2024-05-07 02:46:41.000000 niwatoko-1.2.5/tests/__init__.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     3754 2024-05-08 23:03:26.000000 niwatoko-1.2.5/tests/test_compiler.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     4529 2024-05-08 23:03:26.000000 niwatoko-1.2.5/tests/test_compiler.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     3940 2024-05-08 23:04:26.000000 niwatoko-1.2.5/tests/test_compiler_v1_2.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-28 19:10:43.143106 niwatoko-1.2.5/tests/test_docs/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2747 2024-05-07 02:46:41.000000 niwatoko-1.2.5/tests/test_docs/__init__.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2030 2024-05-14 05:32:42.000000 niwatoko-1.2.5/tests/test_docs/output copy.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     3118 2024-05-14 05:32:42.000000 niwatoko-1.2.5/tests/test_docs/output.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     4172 2024-05-14 05:32:42.000000 niwatoko-1.2.5/tests/test_docs/output.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1733 2024-05-14 05:32:42.000000 niwatoko-1.2.5/tests/test_docs/output_.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2609 2024-05-07 05:48:44.000000 niwatoko-1.2.5/tests/test_docs/test_doc1.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2853 2024-05-07 05:48:44.000000 niwatoko-1.2.5/tests/test_docs/test_doc2.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2625 2024-05-07 05:48:44.000000 niwatoko-1.2.5/tests/test_docs/test_doc3.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1678 2024-05-07 22:46:07.000000 niwatoko-1.2.5/tests/test_docs/test_gen_github_issue.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1950 2024-05-07 22:46:07.000000 niwatoko-1.2.5/tests/test_docs/test_gen_grimoire.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1909 2024-05-07 22:46:07.000000 niwatoko-1.2.5/tests/test_docs/test_gen_grimoire2.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1850 2024-05-07 22:46:07.000000 niwatoko-1.2.5/tests/test_docs/test_gen_grimoire_en.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     5307 2024-05-07 05:52:23.000000 niwatoko-1.2.5/tests/test_docs/test_gen_zoltraak_pypi.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     6179 2024-05-14 05:32:42.000000 niwatoko-1.2.5/tests/test_docs/test_import_function.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2216 2024-05-07 02:46:41.000000 niwatoko-1.2.5/tests/test_interpreter.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2632 2024-05-07 02:46:41.000000 niwatoko-1.2.5/tests/test_parser.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-28 19:13:39.230672 niwatoko-1.2.6/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    11356 2024-05-07 05:52:57.000000 niwatoko-1.2.6/LICENSE
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    16938 2024-05-28 19:13:39.230485 niwatoko-1.2.6/PKG-INFO
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    16052 2024-05-26 09:22:11.000000 niwatoko-1.2.6/README.md
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-28 19:13:39.224560 niwatoko-1.2.6/niwatoko/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      166 2024-05-20 02:01:29.000000 niwatoko-1.2.6/niwatoko/__init__.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    25526 2024-05-28 19:13:06.000000 niwatoko-1.2.6/niwatoko/cli.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-28 19:13:39.223106 niwatoko-1.2.6/niwatoko/foundation_model/
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-28 19:13:39.223143 niwatoko-1.2.6/niwatoko/foundation_model/interpretation/
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-28 19:13:39.225712 niwatoko-1.2.6/niwatoko/foundation_model/interpretation/llm/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1346 2024-05-20 02:01:29.000000 niwatoko-1.2.6/niwatoko/foundation_model/interpretation/llm/claude.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2289 2024-05-26 09:22:11.000000 niwatoko-1.2.6/niwatoko/foundation_model/interpretation/llm/gpt.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-28 19:13:39.225825 niwatoko-1.2.6/niwatoko/grammar/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1509 2024-05-26 09:22:11.000000 niwatoko-1.2.6/niwatoko/grammar/system.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       33 2024-05-14 05:32:42.000000 niwatoko-1.2.6/niwatoko/temp.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-28 19:13:39.225348 niwatoko-1.2.6/niwatoko.egg-info/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    16938 2024-05-28 19:13:39.000000 niwatoko-1.2.6/niwatoko.egg-info/PKG-INFO
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1026 2024-05-28 19:13:39.000000 niwatoko-1.2.6/niwatoko.egg-info/SOURCES.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)        1 2024-05-28 19:13:39.000000 niwatoko-1.2.6/niwatoko.egg-info/dependency_links.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       47 2024-05-28 19:13:39.000000 niwatoko-1.2.6/niwatoko.egg-info/entry_points.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       80 2024-05-28 19:13:39.000000 niwatoko-1.2.6/niwatoko.egg-info/requires.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       15 2024-05-28 19:13:39.000000 niwatoko-1.2.6/niwatoko.egg-info/top_level.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       38 2024-05-28 19:13:39.230707 niwatoko-1.2.6/setup.cfg
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1775 2024-05-28 19:13:34.000000 niwatoko-1.2.6/setup.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-28 19:13:39.227326 niwatoko-1.2.6/tests/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     5897 2024-05-08 23:04:24.000000 niwatoko-1.2.6/tests/README.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2077 2024-05-07 02:46:41.000000 niwatoko-1.2.6/tests/__init__.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     3754 2024-05-08 23:03:26.000000 niwatoko-1.2.6/tests/test_compiler.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     4529 2024-05-08 23:03:26.000000 niwatoko-1.2.6/tests/test_compiler.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     3940 2024-05-08 23:04:26.000000 niwatoko-1.2.6/tests/test_compiler_v1_2.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-28 19:13:39.230174 niwatoko-1.2.6/tests/test_docs/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2747 2024-05-07 02:46:41.000000 niwatoko-1.2.6/tests/test_docs/__init__.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2030 2024-05-14 05:32:42.000000 niwatoko-1.2.6/tests/test_docs/output copy.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     3118 2024-05-14 05:32:42.000000 niwatoko-1.2.6/tests/test_docs/output.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     4172 2024-05-14 05:32:42.000000 niwatoko-1.2.6/tests/test_docs/output.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1733 2024-05-14 05:32:42.000000 niwatoko-1.2.6/tests/test_docs/output_.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2609 2024-05-07 05:48:44.000000 niwatoko-1.2.6/tests/test_docs/test_doc1.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2853 2024-05-07 05:48:44.000000 niwatoko-1.2.6/tests/test_docs/test_doc2.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2625 2024-05-07 05:48:44.000000 niwatoko-1.2.6/tests/test_docs/test_doc3.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1678 2024-05-07 22:46:07.000000 niwatoko-1.2.6/tests/test_docs/test_gen_github_issue.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1950 2024-05-07 22:46:07.000000 niwatoko-1.2.6/tests/test_docs/test_gen_grimoire.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1909 2024-05-07 22:46:07.000000 niwatoko-1.2.6/tests/test_docs/test_gen_grimoire2.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1850 2024-05-07 22:46:07.000000 niwatoko-1.2.6/tests/test_docs/test_gen_grimoire_en.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     5307 2024-05-07 05:52:23.000000 niwatoko-1.2.6/tests/test_docs/test_gen_zoltraak_pypi.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     6179 2024-05-14 05:32:42.000000 niwatoko-1.2.6/tests/test_docs/test_import_function.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2216 2024-05-07 02:46:41.000000 niwatoko-1.2.6/tests/test_interpreter.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2632 2024-05-07 02:46:41.000000 niwatoko-1.2.6/tests/test_parser.py
```

### Comparing `niwatoko-1.2.5/LICENSE` & `niwatoko-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.5/PKG-INFO` & `niwatoko-1.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niwatoko
-Version: 1.2.5
+Version: 1.2.6
 Summary: 自然言語でプログラミングを行うことができる新しいプログラミング言語
 Home-page: https://niwatoko2.vercel.app/
 Author: dai-motoki
 Author-email: dai.motoki1123@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Japanese
```

### Comparing `niwatoko-1.2.5/README.md` & `niwatoko-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.5/niwatoko/cli.py` & `niwatoko-1.2.6/niwatoko/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             print("バージョン情報がniwatokoモジュールに存在しません。")
         return
     if not file_path:
         print("ファイルパスが指定されていません。")
         return
 
     processed_content = process_imports(file_path, model_input_image)
-    print("processed_content:", processed_content)
+    # print("processed_content:", processed_content)
     print("実行中... (Processing...)")
 
     # ぐるぐるアニメーションを表示するスレッドを開始
     done = False
     spinner = threading.Thread(target=spin, args=(lambda: done,))
     spinner.start()
 
@@ -503,16 +503,16 @@
                 }
             ],
             "max_tokens": 4095
         }
         pbar.update(1)
     response = requests.post("https://api.openai.com/v1/chat/completions", headers=headers, json=payload)
     summary = response.json().get('choices', [{}])[0].get('message', {}).get('content', '')
-    print(summary)
-    print('')
+    # print(summary)
+    # print('')
 
     return summary
```

### Comparing `niwatoko-1.2.5/niwatoko/foundation_model/interpretation/llm/claude.py` & `niwatoko-1.2.6/niwatoko/foundation_model/interpretation/llm/claude.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.5/niwatoko/foundation_model/interpretation/llm/gpt.py` & `niwatoko-1.2.6/niwatoko/foundation_model/interpretation/llm/gpt.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.5/niwatoko/grammar/system.md` & `niwatoko-1.2.6/niwatoko/grammar/system.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.5/niwatoko.egg-info/PKG-INFO` & `niwatoko-1.2.6/niwatoko.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niwatoko
-Version: 1.2.5
+Version: 1.2.6
 Summary: 自然言語でプログラミングを行うことができる新しいプログラミング言語
 Home-page: https://niwatoko2.vercel.app/
 Author: dai-motoki
 Author-email: dai.motoki1123@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Japanese
```

### Comparing `niwatoko-1.2.5/niwatoko.egg-info/SOURCES.txt` & `niwatoko-1.2.6/niwatoko.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.5/setup.py` & `niwatoko-1.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # niwatoko - 自然言語プログラミング言語のPythonパッケージのsetup.pyファイルです。
 # このファイルはパッケージのインストールや配布に必要な情報を含んでいます。
 
 from setuptools import setup, find_packages
 
 setup(
     name='niwatoko',
-    version='1.2.5',
+    version='1.2.6',
     description='自然言語でプログラミングを行うことができる新しいプログラミング言語',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='dai-motoki',
     author_email='dai.motoki1123@gmail.com',
     url='https://niwatoko2.vercel.app/',
     packages=find_packages(),
```

### Comparing `niwatoko-1.2.5/tests/README.md` & `niwatoko-1.2.6/tests/README.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.5/tests/__init__.py` & `niwatoko-1.2.6/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.5/tests/test_compiler.md` & `niwatoko-1.2.6/tests/test_compiler.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.5/tests/test_compiler.py` & `niwatoko-1.2.6/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.5/tests/test_compiler_v1_2.py` & `niwatoko-1.2.6/tests/test_compiler_v1_2.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.5/tests/test_docs/__init__.py` & `niwatoko-1.2.6/tests/test_docs/__init__.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.5/tests/test_docs/output copy.md` & `niwatoko-1.2.6/tests/test_docs/output copy.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.5/tests/test_docs/output.md` & `niwatoko-1.2.6/tests/test_docs/output.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.5/tests/test_docs/output.py` & `niwatoko-1.2.6/tests/test_docs/output.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.5/tests/test_docs/output_.md` & `niwatoko-1.2.6/tests/test_docs/output_.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.5/tests/test_docs/test_doc1.md` & `niwatoko-1.2.6/tests/test_docs/test_doc1.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.5/tests/test_docs/test_doc2.md` & `niwatoko-1.2.6/tests/test_docs/test_doc2.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.5/tests/test_docs/test_doc3.md` & `niwatoko-1.2.6/tests/test_docs/test_doc3.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.5/tests/test_docs/test_gen_github_issue.md` & `niwatoko-1.2.6/tests/test_docs/test_gen_github_issue.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.5/tests/test_docs/test_gen_grimoire.md` & `niwatoko-1.2.6/tests/test_docs/test_gen_grimoire.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.5/tests/test_docs/test_gen_grimoire2.md` & `niwatoko-1.2.6/tests/test_docs/test_gen_grimoire2.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.5/tests/test_docs/test_gen_grimoire_en.md` & `niwatoko-1.2.6/tests/test_docs/test_gen_grimoire_en.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.5/tests/test_docs/test_gen_zoltraak_pypi.md` & `niwatoko-1.2.6/tests/test_docs/test_gen_zoltraak_pypi.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.5/tests/test_docs/test_import_function.md` & `niwatoko-1.2.6/tests/test_docs/test_import_function.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.5/tests/test_interpreter.py` & `niwatoko-1.2.6/tests/test_interpreter.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.2.5/tests/test_parser.py` & `niwatoko-1.2.6/tests/test_parser.py`

 * *Files identical despite different names*

