# Comparing `tmp/language-practice-0.1.5.tar.gz` & `tmp/language_practice-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "language-practice-0.1.5.tar", last modified: Sat Mar  2 02:47:53 2024, max compression
+gzip compressed data, was "language_practice-0.2.0.tar", last modified: Mon May 27 23:39:20 2024, max compression
```

## Comparing `language-practice-0.1.5.tar` & `language_practice-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxr-xr-x   0 jbaublitz  (1000) jbaublitz  (1000)        0 2024-03-02 02:47:53.112593 language-practice-0.1.5/
--rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)     1500 2023-03-22 03:48:52.000000 language-practice-0.1.5/LICENSE
--rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)     3965 2024-03-02 02:47:53.112593 language-practice-0.1.5/PKG-INFO
--rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)     3526 2024-03-02 02:43:53.000000 language-practice-0.1.5/README.md
--rwxr-xr-x   0 jbaublitz  (1000) jbaublitz  (1000)     1188 2023-10-21 21:44:37.000000 language-practice-0.1.5/language-practice
-drwxr-xr-x   0 jbaublitz  (1000) jbaublitz  (1000)        0 2024-03-02 02:47:53.109593 language-practice-0.1.5/language_practice/
--rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)        0 2023-10-21 21:44:37.000000 language-practice-0.1.5/language_practice/__init__.py
--rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)      895 2024-03-01 04:53:15.000000 language-practice-0.1.5/language_practice/cache.py
--rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)     4050 2024-03-01 14:01:56.000000 language-practice-0.1.5/language_practice/repetition.py
--rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)     5303 2024-03-01 04:53:15.000000 language-practice-0.1.5/language_practice/terminal.py
--rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)     2875 2024-03-01 04:53:15.000000 language-practice-0.1.5/language_practice/toml.py
-drwxr-xr-x   0 jbaublitz  (1000) jbaublitz  (1000)        0 2024-03-02 02:47:53.111593 language-practice-0.1.5/language_practice/web/
--rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)     2231 2024-03-01 04:53:15.000000 language-practice-0.1.5/language_practice/web/__init__.py
--rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)     1007 2023-10-21 21:44:37.000000 language-practice-0.1.5/language_practice/web/fr.py
--rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)      748 2024-03-01 04:53:15.000000 language-practice-0.1.5/language_practice/web/ru.py
--rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)      798 2023-10-24 21:39:09.000000 language-practice-0.1.5/language_practice/web/shared.py
--rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)      434 2024-03-01 04:53:15.000000 language-practice-0.1.5/language_practice/web/uk.py
-drwxr-xr-x   0 jbaublitz  (1000) jbaublitz  (1000)        0 2024-03-02 02:47:53.111593 language-practice-0.1.5/language_practice.egg-info/
--rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)     3965 2024-03-02 02:47:53.000000 language-practice-0.1.5/language_practice.egg-info/PKG-INFO
--rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)      568 2024-03-02 02:47:53.000000 language-practice-0.1.5/language_practice.egg-info/SOURCES.txt
--rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)        1 2024-03-02 02:47:53.000000 language-practice-0.1.5/language_practice.egg-info/dependency_links.txt
--rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)       41 2024-03-02 02:47:53.000000 language-practice-0.1.5/language_practice.egg-info/requires.txt
--rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)       18 2024-03-02 02:47:53.000000 language-practice-0.1.5/language_practice.egg-info/top_level.txt
--rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)       81 2023-10-21 21:13:36.000000 language-practice-0.1.5/pyproject.toml
--rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)      549 2024-03-02 02:47:53.113592 language-practice-0.1.5/setup.cfg
--rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)       38 2023-10-21 21:44:37.000000 language-practice-0.1.5/setup.py
+drwxr-xr-x   0 jbaublitz  (1000) jbaublitz  (1000)        0 2024-05-27 23:39:20.558908 language_practice-0.2.0/
+-rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)     1500 2024-05-27 14:47:16.000000 language_practice-0.2.0/LICENSE
+-rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)     4160 2024-05-27 23:39:20.558908 language_practice-0.2.0/PKG-INFO
+-rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)     3721 2024-05-27 23:33:58.000000 language_practice-0.2.0/README.md
+-rwxr-xr-x   0 jbaublitz  (1000) jbaublitz  (1000)     1539 2024-05-27 23:33:58.000000 language_practice-0.2.0/language-practice
+drwxr-xr-x   0 jbaublitz  (1000) jbaublitz  (1000)        0 2024-05-27 23:39:20.557908 language_practice-0.2.0/language_practice/
+-rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)        0 2024-05-27 14:47:16.000000 language_practice-0.2.0/language_practice/__init__.py
+-rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)      895 2024-05-27 14:47:16.000000 language_practice-0.2.0/language_practice/cache.py
+-rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)     4050 2024-05-27 23:33:58.000000 language_practice-0.2.0/language_practice/repetition.py
+-rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)     5805 2024-05-27 23:33:58.000000 language_practice-0.2.0/language_practice/terminal.py
+-rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)     3245 2024-05-27 23:33:58.000000 language_practice-0.2.0/language_practice/toml.py
+drwxr-xr-x   0 jbaublitz  (1000) jbaublitz  (1000)        0 2024-05-27 23:39:20.558908 language_practice-0.2.0/language_practice/web/
+-rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)     2165 2024-05-27 23:33:58.000000 language_practice-0.2.0/language_practice/web/__init__.py
+-rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)     1007 2024-05-27 14:47:16.000000 language_practice-0.2.0/language_practice/web/fr.py
+-rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)      748 2024-05-27 14:47:16.000000 language_practice-0.2.0/language_practice/web/ru.py
+-rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)      798 2024-05-27 14:47:16.000000 language_practice-0.2.0/language_practice/web/shared.py
+-rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)      434 2024-05-27 14:47:16.000000 language_practice-0.2.0/language_practice/web/uk.py
+drwxr-xr-x   0 jbaublitz  (1000) jbaublitz  (1000)        0 2024-05-27 23:39:20.558908 language_practice-0.2.0/language_practice.egg-info/
+-rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)     4160 2024-05-27 23:39:20.000000 language_practice-0.2.0/language_practice.egg-info/PKG-INFO
+-rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)      553 2024-05-27 23:39:20.000000 language_practice-0.2.0/language_practice.egg-info/SOURCES.txt
+-rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)        1 2024-05-27 23:39:20.000000 language_practice-0.2.0/language_practice.egg-info/dependency_links.txt
+-rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)       41 2024-05-27 23:39:20.000000 language_practice-0.2.0/language_practice.egg-info/requires.txt
+-rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)       18 2024-05-27 23:39:20.000000 language_practice-0.2.0/language_practice.egg-info/top_level.txt
+-rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)      549 2024-05-27 23:39:20.559908 language_practice-0.2.0/setup.cfg
+-rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)       38 2024-05-27 14:47:16.000000 language_practice-0.2.0/setup.py
```

### Comparing `language-practice-0.1.5/LICENSE` & `language_practice-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `language-practice-0.1.5/PKG-INFO` & `language_practice-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: language-practice
-Version: 0.1.5
+Version: 0.2.0
 Summary: Flashcard app with support for downloading inflection tables
 Home-page: https://github.com/jbaublitz/language-practice
 Author: John Baublitz
 Author-email: "john.m.baublitz@gmail.com"
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -38,18 +38,21 @@
 
 Run `language-practice path/to/toml/file.toml` to start the program. This may take
 some time if you are using conjugation or declension charts as it will pull them in
 parallel from the internet. An internet connection is only required for this part
 of the execution.
 
 Command line options:
-* `--traceback`: useful for bug reporting, bubbles the Python exception up to the
+* `-t`/`--traceback`: useful for bug reporting, bubbles the Python exception up to the
 terminal
-* `--reset`: Redownload the entire cache and current information about what words you
+* `-r`/`--reset`: Redownload the entire cache and current information about what words you
 have guessed correctly/incorrectly
+* `-f`/`--file`: Path to the file containing the flashcard information
+* `-d`/`--dir`: File is a directory and all TOML files in the given directory should be loaded
+by the application
 
 Run ctrl-C to exit the program and save your progress
 
 ## File format
 
 The file format is TOML.
```

### Comparing `language-practice-0.1.5/README.md` & `language_practice-0.2.0/language_practice.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: language-practice
+Version: 0.2.0
+Summary: Flashcard app with support for downloading inflection tables
+Home-page: https://github.com/jbaublitz/language-practice
+Author: John Baublitz
+Author-email: "john.m.baublitz@gmail.com"
+License: BSD-3-Clause
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: aiohttp
+Requires-Dist: beautifulsoup4
+Requires-Dist: requests
+Requires-Dist: tabulate
+
 # `language_practice`
 
 Flashcard terminal app with spaced repetition
 
 ## Languages supported
 
 While any language with gender or verb aspect can be used, declension/verb conjugation
@@ -23,18 +38,21 @@
 
 Run `language-practice path/to/toml/file.toml` to start the program. This may take
 some time if you are using conjugation or declension charts as it will pull them in
 parallel from the internet. An internet connection is only required for this part
 of the execution.
 
 Command line options:
-* `--traceback`: useful for bug reporting, bubbles the Python exception up to the
+* `-t`/`--traceback`: useful for bug reporting, bubbles the Python exception up to the
 terminal
-* `--reset`: Redownload the entire cache and current information about what words you
+* `-r`/`--reset`: Redownload the entire cache and current information about what words you
 have guessed correctly/incorrectly
+* `-f`/`--file`: Path to the file containing the flashcard information
+* `-d`/`--dir`: File is a directory and all TOML files in the given directory should be loaded
+by the application
 
 Run ctrl-C to exit the program and save your progress
 
 ## File format
 
 The file format is TOML.
```

### Comparing `language-practice-0.1.5/language_practice/cache.py` & `language_practice-0.2.0/language_practice/cache.py`

 * *Files identical despite different names*

### Comparing `language-practice-0.1.5/language_practice/repetition.py` & `language_practice-0.2.0/language_practice/repetition.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Handles spaced repetition.
 """
 
-from collections import deque
 import json
+from collections import deque
 from random import shuffle
 
 
 class WordRepetition:
     """
     Information on a single word's repetition frequency.
     """
```

### Comparing `language-practice-0.1.5/language_practice/terminal.py` & `language_practice-0.2.0/language_practice/terminal.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,33 +2,48 @@
 Terminal application interface.
 """
 
 import os
 import sys
 import termios
 import tty
+from functools import reduce
 
 from tabulate import tabulate
 
 from language_practice.cache import Cache
 from language_practice.repetition import Repetition
 from language_practice.toml import TomlConfig
 from language_practice.web import refresh, scrape
 
 
 class Application:
     """
     Handles the interactive user input from the terminal.
     """
 
-    def __init__(self, word_path, reset):
-        if not word_path.endswith(".toml"):
-            raise RuntimeError("Word file needs to be a TOML file")
+    def __init__(self, word_path, is_dir, reset):
+        if is_dir:
+            (directory, _, files) = next(os.walk(word_path))
+            self.words = reduce(
+                lambda toml1, toml2: toml1.extend(toml2),
+                [
+                    TomlConfig(f"{directory}/{file}")
+                    for file in files
+                    if file.endswith(".toml")
+                ],
+            )
+            name = "directory"
+        else:
+            if not word_path.endswith(".toml"):
+                raise RuntimeError("Word file needs to be a TOML file")
+
+            (name, _) = os.path.splitext(word_path)
+            self.words = TomlConfig(word_path)
 
-        (name, _) = os.path.splitext(word_path)
         repetition_path = f"{name}-repetition.json"
         cache_path = f"{name}-cache.json"
 
         if reset:
             try:
                 os.remove(repetition_path)
                 os.remove(cache_path)
```

### Comparing `language-practice-0.1.5/language_practice/toml.py` & `language_practice-0.2.0/language_practice/toml.py`

 * *Files 7% similar despite different names*

```diff
@@ -102,7 +102,20 @@
         return self.lang
 
     def get_words(self):
         """
         Get a list of all words in the TOML file.
         """
         return list(self.words.keys())
+
+    def extend(self, toml):
+        """
+        Extend a TOML config with another TOML config.
+        """
+        if self.lang != toml.lang:
+            raise RuntimeError(
+                f"Attempted to join a TOML config with lang {self.lang} with \
+                one with lang {toml.lang}"
+            )
+
+        self.words.update(toml.words)
+        return self
```

### Comparing `language-practice-0.1.5/language_practice/web/__init__.py` & `language_practice-0.2.0/language_practice/web/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,17 +4,15 @@
 
 import asyncio
 
 import aiohttp
 from bs4 import BeautifulSoup
 from requests import get
 
-from language_practice.web import fr
-from language_practice.web import ru
-from language_practice.web import uk
+from language_practice.web import fr, ru, uk
 
 URL = "https://en.wiktionary.org/wiki/"
 
 
 def refresh(word, lang):
     """
     Refresh individual cache entry.
```

### Comparing `language-practice-0.1.5/language_practice/web/fr.py` & `language_practice-0.2.0/language_practice/web/fr.py`

 * *Files identical despite different names*

### Comparing `language-practice-0.1.5/language_practice/web/ru.py` & `language_practice-0.2.0/language_practice/web/ru.py`

 * *Files identical despite different names*

### Comparing `language-practice-0.1.5/language_practice/web/shared.py` & `language_practice-0.2.0/language_practice/web/shared.py`

 * *Files identical despite different names*

### Comparing `language-practice-0.1.5/language_practice.egg-info/PKG-INFO` & `language_practice-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: language-practice
-Version: 0.1.5
-Summary: Flashcard app with support for downloading inflection tables
-Home-page: https://github.com/jbaublitz/language-practice
-Author: John Baublitz
-Author-email: "john.m.baublitz@gmail.com"
-License: BSD-3-Clause
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: aiohttp
-Requires-Dist: beautifulsoup4
-Requires-Dist: requests
-Requires-Dist: tabulate
-
 # `language_practice`
 
 Flashcard terminal app with spaced repetition
 
 ## Languages supported
 
 While any language with gender or verb aspect can be used, declension/verb conjugation
@@ -38,18 +23,21 @@
 
 Run `language-practice path/to/toml/file.toml` to start the program. This may take
 some time if you are using conjugation or declension charts as it will pull them in
 parallel from the internet. An internet connection is only required for this part
 of the execution.
 
 Command line options:
-* `--traceback`: useful for bug reporting, bubbles the Python exception up to the
+* `-t`/`--traceback`: useful for bug reporting, bubbles the Python exception up to the
 terminal
-* `--reset`: Redownload the entire cache and current information about what words you
+* `-r`/`--reset`: Redownload the entire cache and current information about what words you
 have guessed correctly/incorrectly
+* `-f`/`--file`: Path to the file containing the flashcard information
+* `-d`/`--dir`: File is a directory and all TOML files in the given directory should be loaded
+by the application
 
 Run ctrl-C to exit the program and save your progress
 
 ## File format
 
 The file format is TOML.
```

### Comparing `language-practice-0.1.5/setup.cfg` & `language_practice-0.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 author = John Baublitz
 author_email = "john.m.baublitz@gmail.com"
 url = https://github.com/jbaublitz/language-practice
 description = Flashcard app with support for downloading inflection tables
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = BSD-3-Clause
-version = 0.1.5
+version = 0.2.0
 
 [options]
 install_requires = 
 	aiohttp
 	beautifulsoup4
 	requests
 	tabulate
```

