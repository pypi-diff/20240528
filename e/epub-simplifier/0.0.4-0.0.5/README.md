# Comparing `tmp/epub-simplifier-0.0.4.tar.gz` & `tmp/epub_simplifier-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epub-simplifier-0.0.4.tar", last modified: Wed Mar 20 11:21:07 2024, max compression
+gzip compressed data, was "epub_simplifier-0.0.5.tar", last modified: Tue May 28 11:42:35 2024, max compression
```

## Comparing `epub-simplifier-0.0.4.tar` & `epub_simplifier-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 11:21:07.390518 epub-simplifier-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-20 11:20:26.000000 epub-simplifier-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-03-20 11:21:07.390518 epub-simplifier-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-03-20 11:20:26.000000 epub-simplifier-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 11:21:07.386518 epub-simplifier-0.0.4/epub_simplifier/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 11:20:26.000000 epub-simplifier-0.0.4/epub_simplifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14397 2024-03-20 11:20:26.000000 epub-simplifier-0.0.4/epub_simplifier/simplifier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 11:21:07.390518 epub-simplifier-0.0.4/epub_simplifier.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-03-20 11:21:07.000000 epub-simplifier-0.0.4/epub_simplifier.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-03-20 11:21:07.000000 epub-simplifier-0.0.4/epub_simplifier.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 11:21:07.000000 epub-simplifier-0.0.4/epub_simplifier.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-20 11:21:07.000000 epub-simplifier-0.0.4/epub_simplifier.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-20 11:21:07.000000 epub-simplifier-0.0.4/epub_simplifier.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-20 11:21:07.000000 epub-simplifier-0.0.4/epub_simplifier.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-03-20 11:20:26.000000 epub-simplifier-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 11:21:07.390518 epub-simplifier-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 11:21:07.390518 epub-simplifier-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-03-20 11:20:26.000000 epub-simplifier-0.0.4/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:42:35.293862 epub_simplifier-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-28 11:41:55.000000 epub_simplifier-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-05-28 11:42:35.293862 epub_simplifier-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-28 11:41:55.000000 epub_simplifier-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:42:35.289862 epub_simplifier-0.0.5/epub_simplifier/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 11:41:55.000000 epub_simplifier-0.0.5/epub_simplifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14390 2024-05-28 11:41:55.000000 epub_simplifier-0.0.5/epub_simplifier/simplifier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:42:35.293862 epub_simplifier-0.0.5/epub_simplifier.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-05-28 11:42:35.000000 epub_simplifier-0.0.5/epub_simplifier.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-28 11:42:35.000000 epub_simplifier-0.0.5/epub_simplifier.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 11:42:35.000000 epub_simplifier-0.0.5/epub_simplifier.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-28 11:42:35.000000 epub_simplifier-0.0.5/epub_simplifier.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-28 11:42:35.000000 epub_simplifier-0.0.5/epub_simplifier.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-28 11:42:35.000000 epub_simplifier-0.0.5/epub_simplifier.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-05-28 11:41:55.000000 epub_simplifier-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 11:42:35.293862 epub_simplifier-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:42:35.289862 epub_simplifier-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-05-28 11:41:55.000000 epub_simplifier-0.0.5/tests/test_main.py
```

### Comparing `epub-simplifier-0.0.4/LICENSE` & `epub_simplifier-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `epub-simplifier-0.0.4/PKG-INFO` & `epub_simplifier-0.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epub-simplifier
-Version: 0.0.4
+Version: 0.0.5
 Summary: A command-line tool to simplify language in EPUB books
 Author-email: Anatolii Bubenkov <bubenkoff@gmail.com>
 Project-URL: Repository, https://github.com/bubenkoff/epub-simplifier.git
 Project-URL: Issues, https://github.com/bubenkoff/epub-simplifier/issues
 Keywords: epub,language,simplification,tool
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
@@ -36,14 +36,15 @@
 ![Test](https://github.com/bubenkoff/epub-simplifier/actions/workflows/test.yml/badge.svg)
 [![PyPI Version](https://img.shields.io/pypi/v/epub-simplifier.svg)
 ](https://pypi.python.org/pypi/epub-simplifier)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/epub-simplifier)
 ](https://pypi.python.org/pypi/epub-simplifier)
 [![Coverage](https://img.shields.io/coveralls/bubenkoff/epub-simplifier/main.svg)
 ](https://coveralls.io/r/bubenkoff/epub-simplifier)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 ## Description
 EPUB Simplifier is a command-line tool designed to convert text within EPUB files into a simplified language at a selected proficiency level. This tool aims to make literature more accessible to language learners by simplifying complex language structures and vocabulary.
 
 > [!WARNING]
 > It uses OpenAI API and requires an API key to work, which is not provided with the package. It can also be quite expensive to use, depending on the size of the book.
 
@@ -89,8 +90,8 @@
 ## Requirements
 The dependencies will be installed automatically during the package installation process.
 
 ## Feedback and Contributions
 Your feedback and contributions are welcome! If you encounter any issues or have suggestions for improvements, please feel free to open an issue on the GitHub repository or submit a pull request with your changes.
 
 ## License
-MIT 
+MIT
```

### Comparing `epub-simplifier-0.0.4/README.md` & `epub_simplifier-0.0.5/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 ![Test](https://github.com/bubenkoff/epub-simplifier/actions/workflows/test.yml/badge.svg)
 [![PyPI Version](https://img.shields.io/pypi/v/epub-simplifier.svg)
 ](https://pypi.python.org/pypi/epub-simplifier)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/epub-simplifier)
 ](https://pypi.python.org/pypi/epub-simplifier)
 [![Coverage](https://img.shields.io/coveralls/bubenkoff/epub-simplifier/main.svg)
 ](https://coveralls.io/r/bubenkoff/epub-simplifier)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 ## Description
 EPUB Simplifier is a command-line tool designed to convert text within EPUB files into a simplified language at a selected proficiency level. This tool aims to make literature more accessible to language learners by simplifying complex language structures and vocabulary.
 
 > [!WARNING]
 > It uses OpenAI API and requires an API key to work, which is not provided with the package. It can also be quite expensive to use, depending on the size of the book.
 
@@ -56,8 +57,8 @@
 ## Requirements
 The dependencies will be installed automatically during the package installation process.
 
 ## Feedback and Contributions
 Your feedback and contributions are welcome! If you encounter any issues or have suggestions for improvements, please feel free to open an issue on the GitHub repository or submit a pull request with your changes.
 
 ## License
-MIT 
+MIT
```

### Comparing `epub-simplifier-0.0.4/epub_simplifier/simplifier.py` & `epub_simplifier-0.0.5/epub_simplifier/simplifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,17 +18,15 @@
     # stop_after_attempt,
     wait_random_exponential,
     before_log,
 )  # for exponential backoff
 
 # require environment variables
 if "OPENAI_API_KEY" not in os.environ:
-    raise ValueError(
-        "OpenAI API key is not set. Please set the OPENAI_API_KEY environment variable."
-    )
+    raise ValueError("OpenAI API key is not set. Please set the OPENAI_API_KEY environment variable.")
 client = OpenAI()
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.StreamHandler())
 separator = "\n\n"
 
 wait_arguments = {
     "retry": retry_if_exception_type(IOError),
@@ -63,15 +61,15 @@
         "input": sum((usage["input"] for (_, usage) in chunks)),
         "output": sum((usage["output"] for (_, usage) in chunks)),
     }
     return separator.join((chunk for (chunk, _) in chunks)), usage
 
 
 @retry(**wait_arguments)
-async def simplify_chapter(title, text, language, level, max_tokens, model, dry_run):
+async def simplify_chapter(index, title, text, language, level, max_tokens, model, dry_run):
     """
     Simplify the text to a selected level using the latest OpenAI package.
     """
     result = []
     chunks = chunkify_text(text, separator, max_tokens)
     instructions = [
         {
@@ -80,23 +78,21 @@
         },
         {
             "role": "system",
             "content": f"Your student is a {level} student who wants to read {language} literature",
         },
     ]
     async with asyncio.TaskGroup() as group:
-        tasks = [
-            group.create_task(
-                process_chunk(title, chunk, language, instructions, model, dry_run)
-            )
-            for chunk in chunks
-        ]
+        tasks = [group.create_task(process_chunk(title, chunk, language, instructions, model, dry_run)) for chunk in chunks]
     result = [task.result() for task in tasks]
-    text, usage = dechunkify_text(result, separator)
-    logger.debug(f"\nSimplified text: {text}, usage: {usage}")
+    simplified_text, usage = dechunkify_text(result, separator)
+    logger.debug(
+        f"\nSimplified chapter: {index}, usage: {usage}, "
+        f"length ratio simplified / original: {len(simplified_text)/len(text):.2%}"
+    )
     # try:
     #     response = await client.chat.completions.create(
     #         model=model,  # Choose the best model for your needs. 'gpt-3.5-turbo' is suggested for efficiency and cost.
     #         messages=[
     #             *instructions,
     #             {
     #                 "role": "system",
@@ -117,15 +113,15 @@
     #     # Extracting and returning the completion text
     #     choice = response.choices[0]
     #     if choice.finish_reason == "length":
     #         logger.warning("Response was truncated.")
     #     text = choice.message.content.strip()
     # except Exception as e:
     #     logger.error(f"Error during API call: {e}")
-    return text, usage
+    return simplified_text, usage
 
 
 @retry(**wait_arguments)
 async def process_chunk(title, text, language, instructions, model, dry_run):
     logger.debug(f"\nProcessing chunk: {model}, dry_run: {dry_run}")
     # sleep for a while
     if dry_run:
@@ -215,19 +211,15 @@
     simplified_book = book
     # Process each item in the EPUB
     index = 1
     documents = list(book.get_items_of_type(ebooklib.ITEM_DOCUMENT))
     count = len(documents)
     if only_documents:
         only_documents = set(only_documents)
-    documents = [
-        document
-        for index, document in enumerate(documents)
-        if not only_documents or index in only_documents
-    ]
+    documents = [document for index, document in enumerate(documents) if not only_documents or index in only_documents]
     if max_documents:
         documents = documents[:max_documents]
     count = len(documents)
     # process documents in parallel using multiprocessing
     usage = {
         "input": 0,
         "output": 0,
@@ -290,110 +282,97 @@
     """Process a single document in the EPUB file."""
     # sleep for a while
     content = item.get_content().decode("utf-8")
     simplified_content = content
     logger.debug(f"\nProcessing item: {index}")
     soup = BeautifulSoup(content, "html.parser")
     # text = soup.get_text()
-    text = md(str(soup.body))
+    text = md(str(soup.body)).strip()
     if save_html:
         with open(os.path.join(html_path, f"{index}_input.html"), "w") as f:
             f.write(content)
         with open(os.path.join(html_path, f"{index}_input.md"), "w") as f:
             f.write(text)
-    simplified_text, usage = await simplify_chapter(
-        title, text, language, level, max_tokens, model, dry_run
-    )
-    if simplified_text:
-        logger.debug(f"\nSimplified: {index}")
-        simplified_content = markdown2.markdown(simplified_text)
-        soup.body.clear()
-        soup.body.append(BeautifulSoup(simplified_content, "html.parser"))
-        simplified_content = str(soup)
-        if save_html:
-            with open(os.path.join(html_path, f"{index}_output.html"), "w") as f:
-                f.write(simplified_content)
-            with open(os.path.join(html_path, f"{index}_output.md"), "w") as f:
-                f.write(simplified_text)
-        # simplified_book.add_item(item)
+    if text:
+        simplified_text, usage = await simplify_chapter(index, title, text, language, level, max_tokens, model, dry_run)
+        if simplified_text:
+            logger.debug(f"\nSimplified: {index}")
+            simplified_content = markdown2.markdown(simplified_text)
+            soup.body.clear()
+            soup.body.append(BeautifulSoup(simplified_content, "html.parser"))
+            simplified_content = str(soup)
+            if save_html:
+                with open(os.path.join(html_path, f"{index}_output.html"), "w") as f:
+                    f.write(simplified_content)
+                with open(os.path.join(html_path, f"{index}_output.md"), "w") as f:
+                    f.write(simplified_text)
+            # simplified_book.add_item(item)
     logger.debug(f"\nProcessed {index} document of {count}.")
     await result_queue.put(index)
     return simplified_content, usage
 
 
 def main():
     """Entry point for the command line interface."""
-    parser = argparse.ArgumentParser(
-        description="Simplify text in EPUB files to selected language level."
-    )
+    parser = argparse.ArgumentParser(description="Simplify text in EPUB files to selected language level.")
     parser.add_argument("input_path", type=str, help="Path to the original EPUB file.")
-    parser.add_argument(
-        "output_path", type=str, help="Path to save the simplified EPUB file."
-    )
+    parser.add_argument("output_path", type=str, help="Path to save the simplified EPUB file.")
     parser.add_argument("language", type=str, help="Language to simplify.")
     parser.add_argument("level", type=str, help="Language level to simplify to.")
     # max documents to process
     parser.add_argument("--max-documents", type=int, help="Max documents to process.")
     # save html documents to disk
-    parser.add_argument(
-        "--save-html", action="store_true", help="Save HTML documents to disk."
-    )
+    parser.add_argument("--save-html", action="store_true", help="Save HTML documents to disk.")
     # only process the selected documents, can be used for testing
     parser.add_argument(
         "--only-documents",
         type=lambda t: [int(s.strip()) for s in t.split(",")],
         help="Only process the selected documents. Comma-separated list of document numbers.",
     )
     # max tokens for the API call
     parser.add_argument(
         "--max-tokens",
         type=int,
         help="Max tokens for the API call. It's a total magic to select a proper value due to the OpenAI model behavior.",
         default=13000,
     )
     # dry run
-    parser.add_argument(
-        "--dry-run", action="store_true", help="Run without making any changes."
-    )
+    parser.add_argument("--dry-run", action="store_true", help="Run without making any changes.")
     # model
     parser.add_argument(
         "--model",
         type=str,
         help="OpenAI model to use. Default is gpt-4-turbo-preview.",
-        default="gpt-4-turbo-preview",
+        default="gpt-4o",
     )
     # price per input token
     parser.add_argument(
         "--pricing-input",
         type=float,
         help="Price per input token in USD",
-        default=10 / (10**6),
+        default=5 / (10**6),
     )
     # price per output token
     parser.add_argument(
         "--pricing-output",
         type=float,
         help="Price per output token in USD",
-        default=30 / (10**6),
+        default=15 / (10**6),
     )
     # answer yes to all questions
-    parser.add_argument(
-        "--yes", action="store_true", help="Answer yes to all questions."
-    )
+    parser.add_argument("--yes", action="store_true", help="Answer yes to all questions.")
     # log level
     parser.add_argument(
         "--log-level",
         type=str,
         help="Log level. Default is INFO.",
         default="INFO",
     )
     # version
-    parser.add_argument(
-        "--version", action="version", version=f"%(prog)s {version('epub-simplifier')}"
-    )
+    parser.add_argument("--version", action="version", version=f"%(prog)s {version('epub-simplifier')}")
 
     args = parser.parse_args()
     # set log level
     logger.setLevel(args.log_level)
     # check for input and output paths not being the same
     if args.input_path == args.output_path:
         raise ValueError("Input and output paths cannot be the same.")
```

### Comparing `epub-simplifier-0.0.4/epub_simplifier.egg-info/PKG-INFO` & `epub_simplifier-0.0.5/epub_simplifier.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epub-simplifier
-Version: 0.0.4
+Version: 0.0.5
 Summary: A command-line tool to simplify language in EPUB books
 Author-email: Anatolii Bubenkov <bubenkoff@gmail.com>
 Project-URL: Repository, https://github.com/bubenkoff/epub-simplifier.git
 Project-URL: Issues, https://github.com/bubenkoff/epub-simplifier/issues
 Keywords: epub,language,simplification,tool
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
@@ -36,14 +36,15 @@
 ![Test](https://github.com/bubenkoff/epub-simplifier/actions/workflows/test.yml/badge.svg)
 [![PyPI Version](https://img.shields.io/pypi/v/epub-simplifier.svg)
 ](https://pypi.python.org/pypi/epub-simplifier)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/epub-simplifier)
 ](https://pypi.python.org/pypi/epub-simplifier)
 [![Coverage](https://img.shields.io/coveralls/bubenkoff/epub-simplifier/main.svg)
 ](https://coveralls.io/r/bubenkoff/epub-simplifier)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 ## Description
 EPUB Simplifier is a command-line tool designed to convert text within EPUB files into a simplified language at a selected proficiency level. This tool aims to make literature more accessible to language learners by simplifying complex language structures and vocabulary.
 
 > [!WARNING]
 > It uses OpenAI API and requires an API key to work, which is not provided with the package. It can also be quite expensive to use, depending on the size of the book.
 
@@ -89,8 +90,8 @@
 ## Requirements
 The dependencies will be installed automatically during the package installation process.
 
 ## Feedback and Contributions
 Your feedback and contributions are welcome! If you encounter any issues or have suggestions for improvements, please feel free to open an issue on the GitHub repository or submit a pull request with your changes.
 
 ## License
-MIT 
+MIT
```

### Comparing `epub-simplifier-0.0.4/pyproject.toml` & `epub_simplifier-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 [project.urls]
 Repository = "https://github.com/bubenkoff/epub-simplifier.git"
 Issues = "https://github.com/bubenkoff/epub-simplifier/issues"
 
 [tool.black]
 line-length = 127
-target-version = ['py37']
+target-version = ['py38']
 include = '\.pyi?$'
 exclude = '''
 
 (
   /(
       \.eggs         # exclude a few common directories in the
     | \.git          # root of the project
```

### Comparing `epub-simplifier-0.0.4/tests/test_main.py` & `epub_simplifier-0.0.5/tests/test_main.py`

 * *Files 14% similar despite different names*

```diff
@@ -64,35 +64,39 @@
     original_book = epub.read_epub(input_path, {"ignore_ncx": True})
     original_documents = list(original_book.get_items_of_type(ebooklib.ITEM_DOCUMENT))
     original_title = original_book.get_metadata("DC", "title")[0][0]
     assert len(original_documents) == 1
     original_content = original_documents[0].get_content()
     original_soup = BeautifulSoup(original_content, "html.parser")
     original_text = md(str(original_soup.body)).strip()
-    assert original_text == """complicated text 1
+    assert (
+        original_text
+        == """complicated text 1
 
 
 complicated text 2"""
+    )
 
     if dry_run:
         # check that the output file is not created in dry-run mode
         assert not (tmp_path / "simplified_book.epub").exists()
         # and mock of the api is not called
         assert not patched.called
         return
     assert patched.call_count == 2
     # read the simplified book and check that it contains the expected text
     simplified_book = epub.read_epub(output_path, {"ignore_ncx": True})
-    simplified_documents = list(
-        simplified_book.get_items_of_type(ebooklib.ITEM_DOCUMENT)
-    )
+    simplified_documents = list(simplified_book.get_items_of_type(ebooklib.ITEM_DOCUMENT))
     simplified_title = simplified_book.get_metadata("DC", "title")[0][0]
 
     assert len(original_documents) == len(simplified_documents)
     assert original_title == simplified_title
     simplified_content = simplified_documents[0].get_content()
     simplified_soup = BeautifulSoup(simplified_content, "html.parser")
     simplified_text = md(str(simplified_soup.body)).strip()
-    assert simplified_text == """simplified text 1
+    assert (
+        simplified_text
+        == """simplified text 1
 
 
 simplified text 2"""
+    )
```

