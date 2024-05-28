# Comparing `tmp/oaicli-0.2.2.tar.gz` & `tmp/oaicli-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oaicli-0.2.2.tar", last modified: Thu Nov 30 11:37:43 2023, max compression
+gzip compressed data, was "oaicli-0.2.4.tar", last modified: Tue May 28 20:23:28 2024, max compression
```

## Comparing `oaicli-0.2.2.tar` & `oaicli-0.2.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jonathan.hendler   (501) staff       (20)        0 2023-11-30 11:37:43.222971 oaicli-0.2.2/
--rw-r--r--   0 jonathan.hendler   (501) staff       (20)    11357 2023-11-10 11:25:42.000000 oaicli-0.2.2/LICENSE
--rw-r--r--   0 jonathan.hendler   (501) staff       (20)    16661 2023-11-30 11:37:43.222452 oaicli-0.2.2/PKG-INFO
--rw-r--r--   0 jonathan.hendler   (501) staff       (20)     3024 2023-11-24 10:23:48.000000 oaicli-0.2.2/README.md
-drwxr-xr-x   0 jonathan.hendler   (501) staff       (20)        0 2023-11-30 11:37:43.219560 oaicli-0.2.2/oaicli/
--rw-r--r--   0 jonathan.hendler   (501) staff       (20)     2479 2023-11-14 12:13:44.000000 oaicli-0.2.2/oaicli/__init__.py
--rw-r--r--   0 jonathan.hendler   (501) staff       (20)     5425 2023-11-30 11:36:39.000000 oaicli-0.2.2/oaicli/cli.py
--rw-r--r--   0 jonathan.hendler   (501) staff       (20)     7159 2023-11-30 11:36:39.000000 oaicli-0.2.2/oaicli/oai.py
--rw-r--r--   0 jonathan.hendler   (501) staff       (20)     7506 2023-11-30 11:36:39.000000 oaicli-0.2.2/oaicli/oai_wrappers.py
-drwxr-xr-x   0 jonathan.hendler   (501) staff       (20)        0 2023-11-30 11:37:43.221648 oaicli-0.2.2/oaicli.egg-info/
--rw-r--r--   0 jonathan.hendler   (501) staff       (20)    16661 2023-11-30 11:37:43.000000 oaicli-0.2.2/oaicli.egg-info/PKG-INFO
--rw-r--r--   0 jonathan.hendler   (501) staff       (20)      284 2023-11-30 11:37:43.000000 oaicli-0.2.2/oaicli.egg-info/SOURCES.txt
--rw-r--r--   0 jonathan.hendler   (501) staff       (20)        1 2023-11-30 11:37:43.000000 oaicli-0.2.2/oaicli.egg-info/dependency_links.txt
--rw-r--r--   0 jonathan.hendler   (501) staff       (20)       43 2023-11-30 11:37:43.000000 oaicli-0.2.2/oaicli.egg-info/entry_points.txt
--rw-r--r--   0 jonathan.hendler   (501) staff       (20)      122 2023-11-30 11:37:43.000000 oaicli-0.2.2/oaicli.egg-info/requires.txt
--rw-r--r--   0 jonathan.hendler   (501) staff       (20)        7 2023-11-30 11:37:43.000000 oaicli-0.2.2/oaicli.egg-info/top_level.txt
--rw-r--r--   0 jonathan.hendler   (501) staff       (20)      843 2023-11-30 11:36:39.000000 oaicli-0.2.2/pyproject.toml
--rw-r--r--   0 jonathan.hendler   (501) staff       (20)       38 2023-11-30 11:37:43.223057 oaicli-0.2.2/setup.cfg
+drwxr-xr-x   0 jonathan.hendler   (501) staff       (20)        0 2024-05-28 20:23:28.371744 oaicli-0.2.4/
+-rw-r--r--   0 jonathan.hendler   (501) staff       (20)    11357 2023-11-10 11:25:42.000000 oaicli-0.2.4/LICENSE
+-rw-r--r--   0 jonathan.hendler   (501) staff       (20)    16485 2024-05-28 20:23:28.371181 oaicli-0.2.4/PKG-INFO
+-rw-r--r--   0 jonathan.hendler   (501) staff       (20)     2847 2023-12-11 18:45:49.000000 oaicli-0.2.4/README.md
+drwxr-xr-x   0 jonathan.hendler   (501) staff       (20)        0 2024-05-28 20:23:28.368421 oaicli-0.2.4/oaicli/
+-rw-r--r--   0 jonathan.hendler   (501) staff       (20)     5561 2024-05-28 20:23:10.000000 oaicli-0.2.4/oaicli/__init__.py
+-rw-r--r--   0 jonathan.hendler   (501) staff       (20)     6184 2024-05-28 20:23:10.000000 oaicli-0.2.4/oaicli/cli.py
+-rw-r--r--   0 jonathan.hendler   (501) staff       (20)     7236 2024-05-28 20:23:10.000000 oaicli-0.2.4/oaicli/oai.py
+-rw-r--r--   0 jonathan.hendler   (501) staff       (20)     7899 2024-05-28 20:23:10.000000 oaicli-0.2.4/oaicli/oai_wrappers.py
+drwxr-xr-x   0 jonathan.hendler   (501) staff       (20)        0 2024-05-28 20:23:28.370479 oaicli-0.2.4/oaicli.egg-info/
+-rw-r--r--   0 jonathan.hendler   (501) staff       (20)    16485 2024-05-28 20:23:28.000000 oaicli-0.2.4/oaicli.egg-info/PKG-INFO
+-rw-r--r--   0 jonathan.hendler   (501) staff       (20)      284 2024-05-28 20:23:28.000000 oaicli-0.2.4/oaicli.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathan.hendler   (501) staff       (20)        1 2024-05-28 20:23:28.000000 oaicli-0.2.4/oaicli.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathan.hendler   (501) staff       (20)       43 2024-05-28 20:23:28.000000 oaicli-0.2.4/oaicli.egg-info/entry_points.txt
+-rw-r--r--   0 jonathan.hendler   (501) staff       (20)      123 2024-05-28 20:23:28.000000 oaicli-0.2.4/oaicli.egg-info/requires.txt
+-rw-r--r--   0 jonathan.hendler   (501) staff       (20)        7 2024-05-28 20:23:28.000000 oaicli-0.2.4/oaicli.egg-info/top_level.txt
+-rw-r--r--   0 jonathan.hendler   (501) staff       (20)      833 2024-05-28 20:23:10.000000 oaicli-0.2.4/pyproject.toml
+-rw-r--r--   0 jonathan.hendler   (501) staff       (20)       38 2024-05-28 20:23:28.371824 oaicli-0.2.4/setup.cfg
```

### Comparing `oaicli-0.2.2/LICENSE` & `oaicli-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `oaicli-0.2.2/PKG-INFO` & `oaicli-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oaicli
-Version: 0.2.2
+Version: 0.2.4
 Summary: A Command Line Interface to Open AI
 Author-email: Jonathan Hendler <jonathan@hai.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -208,15 +208,15 @@
 Keywords: cli,openai,api
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click>=8.1.7
-Requires-Dist: openai>=1.3.6
+Requires-Dist: openai>=1.29.0
 Requires-Dist: python-dotenv>=1.0.0
 Requires-Dist: appdirs>=1.4.4
 Requires-Dist: prompt-toolkit>=3.0.40
 Provides-Extra: dev
 Requires-Dist: black>=23.11.0; extra == "dev"
 Requires-Dist: flake8>=6.1.0; extra == "dev"
 
@@ -269,36 +269,26 @@
  Otherwise there is some agent and file maintenence.
 
     oaicli file upload
     oaicli file list
     oaicli file download-all
 
 
-
 ![Screenshot of running oaicli start](screenshot.png?raw=true "Running oaicli start")
 
-## experimental
-
-Probably broken. If you want autocompletion (useful for editing agents and uploading files)
-
-For Bash:
-
-    eval "$(_OAICLI_COMPLETE=source_bash oaicli)"
-
-For Zsh:
-
-    eval "$(_OAICLI_COMPLETE=source_zsh oaicli)"
 
 ## Roadmap
 
-### v0.3
+### v0.3-0.5
 
  - upload doc from url, or get web contents
  - cat a directory into a single file and upload
  - share publicically OAICLI help agent, uploading entire github repo. For example "what changes would you make to README.md based on the source code"
+ - pydantic refactor
+ - stream response to console
 
  ### v1.x
 
 Have agents select and talk to each other.
 
 Other:
```

### Comparing `oaicli-0.2.2/README.md` & `oaicli-0.2.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -47,36 +47,26 @@
  Otherwise there is some agent and file maintenence.
 
     oaicli file upload
     oaicli file list
     oaicli file download-all
 
 
-
 ![Screenshot of running oaicli start](screenshot.png?raw=true "Running oaicli start")
 
-## experimental
-
-Probably broken. If you want autocompletion (useful for editing agents and uploading files)
-
-For Bash:
-
-    eval "$(_OAICLI_COMPLETE=source_bash oaicli)"
-
-For Zsh:
-
-    eval "$(_OAICLI_COMPLETE=source_zsh oaicli)"
 
 ## Roadmap
 
-### v0.3
+### v0.3-0.5
 
  - upload doc from url, or get web contents
  - cat a directory into a single file and upload
  - share publicically OAICLI help agent, uploading entire github repo. For example "what changes would you make to README.md based on the source code"
+ - pydantic refactor
+ - stream response to console
 
  ### v1.x
 
 Have agents select and talk to each other.
 
 Other:
```

### Comparing `oaicli-0.2.2/oaicli/cli.py` & `oaicli-0.2.4/oaicli/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,25 +13,35 @@
     list_assistants,
     select_assistant,
     select_thread,
     update_agent,
     choose_or_create_file,
     run_thread,
     select_file_id,
+    session,
+    mutliline_toolbar,
 )
-from . import ASCII_ART, FilePathParamType
+from . import FILES_DIR, ASCII_ART, FilePathParamType, download_file, is_url
 from prompt_toolkit import prompt
+from prompt_toolkit.completion import PathCompleter
 
 
 @click.group()
 def cli():
     """Main entry point for oaicli."""
     pass
 
 
+@cli.command(name="version")
+def print_version():
+    import importlib.metadata
+
+    print(importlib.metadata.version("oaicli"))
+
+
 @cli.command(name="start")
 def start_up():
     """Get Started"""
     click.echo(ASCII_ART)
     assistants = []
     current_assistant = None
     current_assistant_id = None
@@ -57,15 +67,22 @@
 Inline commands:
  - Change agent by typing "change" (changes which agent runs the thread)
  - Add file to agent (or change prompt) with "agent"
  - Type 'exit' when done."""
     )
     while True:
         # user_query = click.prompt(f"oaicli ({current_thread_name}) >")
-        user_query = prompt(f"oaicli ({current_thread_name}) >")
+        # user_query = prompt(f"oaicli ({current_thread_name}) >")
+        user_query = session.prompt(
+            f"oaicli ({current_thread_name}) >",
+            multiline=True,
+            mouse_support=True,
+            bottom_toolbar=mutliline_toolbar,
+        )
+
         if user_query.strip() == "exit":
             exit("bye")
         elif user_query.strip() == "change":
             click.echo("changing agent")
             continue
         elif user_query.strip() == "agent":
             update_agent()
@@ -109,19 +126,30 @@
 def list_all():
     """List all files"""
     list_all_files()
 
 
 @file.command(name="upload")
 @click.option(
-    "-f", "--file-path", type=FilePathParamType(), help="Path to a file.", required=True
+    "-f",
+    "--file-path",
+    type=FilePathParamType(),
+    help="Path to a file or a URL.",
+    required=False,
 )
 def do_upload_file(file_path):
     """Upload file"""
-    if click.confirm(f"Are you sure you want to upload {file_path}?"):
+    if not file_path:
+        completer = PathCompleter()
+        file_path = session.prompt("Enter a file path or url: ", completer=completer)
+
+    filepath_is_url = is_url(file_path)
+    if filepath_is_url:
+        file_path, filename = download_file(file_path, FILES_DIR)
+    if click.confirm(f"Are you sure you want to upload {filename}?"):
         upload_file(file_path)
 
 
 @file.command(name="delete")
 def do_delete_file():
     """delete file"""
     file_id = select_file_id()
```

### Comparing `oaicli-0.2.2/oaicli/oai.py` & `oaicli-0.2.4/oaicli/oai.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from . import (
     OPEN_AI_MODEL_TYPE,
     DEFAULT_IMAGE_MODEL,
     agents_dir,
-    files_dir,
+    FILES_DIR,
     threads_dir,
 )
 from openai import OpenAI
 import os
 import logging
 import click
 import time
@@ -106,22 +106,24 @@
     file_object = open(local_path, "w")
     all_content = ""
     for _content in thread_message.content:
         all_content += _content.text.value
     file_object.write(all_content)
 
 
+# todo add back fileids
+# https://platform.openai.com/docs/api-reference/messages/createMessage
 def create_message(
     message_content: str, thread_name: str, thread_id: str, file_ids=None
 ):
     role = "user"
     if not file_ids:
         file_ids = []
     thread_message = client.beta.threads.messages.create(
-        thread_id, role=role, content=message_content, file_ids=file_ids
+        thread_id, role=role, content=message_content
     )
     save_local_message(thread_message, role=role)
     return thread_message
 
 
 def create_run(thread_id, assistant_id):
     return client.beta.threads.runs.create(
@@ -155,15 +157,15 @@
                 )
         elif run.status == "completed":
             return True
 
 
 def _get_local_filepath(file):
     new_filename = f"{file.id}{filename_separator}{file.filename}"
-    return f"{files_dir}/{new_filename}"
+    return f"{FILES_DIR}/{new_filename}"
 
 
 def delete_file(file_id: str):
     client.files.delete(file_id)
 
 
 def delete_assistant(assistant_id):
```

### Comparing `oaicli-0.2.2/oaicli/oai_wrappers.py` & `oaicli-0.2.4/oaicli/oai_wrappers.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     save_instructions,
     client,
 )
 
 from prompt_toolkit import PromptSession
 from prompt_toolkit.completion import PathCompleter
 from prompt_toolkit.formatted_text import HTML
-
+from . import is_url, download_file, copy_file
 
 import textwrap
 from datetime import datetime
 
 
 session = PromptSession()
 
@@ -52,15 +52,15 @@
         "Load an instructions file or enter instructions manually?",
         type=click.Choice(["f", "m"]),
         default="m",
     )
     if input_type == "m":
         # instructions = click.prompt("Instructions")
         instructions = session.prompt(
-            "Instructions",
+            "Instructions: ",
             multiline=True,
             mouse_support=True,
             bottom_toolbar=mutliline_toolbar,
         )
     else:
         completer = PathCompleter()
         file_path = session.prompt("Enter a file path: ", completer=completer)
@@ -94,15 +94,17 @@
     click.echo(f"current instructions:\n\n\t{formatted_instructions}\n")
     click.echo(f"current files:\n{current_assistant.file_ids}\n")
     if click.confirm(f"Update prompt?"):
         if click.confirm(f"did you update {current_assistant.id}/instructions.txt?"):
             new_instructions = None
         else:
             completer = PathCompleter()
-            file_path = session.prompt("Enter a file path: ", completer=completer)
+            file_path = session.prompt(
+                "Enter a file path or url: ", completer=completer
+            )
 
             click.echo(f"Loading filepath {file_path}")
             with open(file_path, "r") as filehandle:
                 new_instructions = filehandle.read()
         update_agent_instructions(
             current_assistant_id, new_instructions=new_instructions
         )
@@ -133,15 +135,21 @@
     return current_thread
 
 
 def choose_or_create_file():
     if click.confirm("Create new file?"):
         completer = PathCompleter()
         file_path = session.prompt("Enter a file path: ", completer=completer)
-
+        filepath_is_url = is_url(file_path)
+        if filepath_is_url:
+            file_path, filename = download_file(file_path)
+        else:
+            file_path, filename = copy_file(file_path)
+        if click.confirm(f"Are you sure you want to upload {filename}?"):
+            upload_file(file_path)
         if click.confirm(f"Are you sure you want to upload {file_path}?"):
             file = upload_file(file_path)
             file_id = file.id
     else:
         file_id = select_file_id()
     return file_id
```

### Comparing `oaicli-0.2.2/oaicli.egg-info/PKG-INFO` & `oaicli-0.2.4/oaicli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oaicli
-Version: 0.2.2
+Version: 0.2.4
 Summary: A Command Line Interface to Open AI
 Author-email: Jonathan Hendler <jonathan@hai.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -208,15 +208,15 @@
 Keywords: cli,openai,api
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click>=8.1.7
-Requires-Dist: openai>=1.3.6
+Requires-Dist: openai>=1.29.0
 Requires-Dist: python-dotenv>=1.0.0
 Requires-Dist: appdirs>=1.4.4
 Requires-Dist: prompt-toolkit>=3.0.40
 Provides-Extra: dev
 Requires-Dist: black>=23.11.0; extra == "dev"
 Requires-Dist: flake8>=6.1.0; extra == "dev"
 
@@ -269,36 +269,26 @@
  Otherwise there is some agent and file maintenence.
 
     oaicli file upload
     oaicli file list
     oaicli file download-all
 
 
-
 ![Screenshot of running oaicli start](screenshot.png?raw=true "Running oaicli start")
 
-## experimental
-
-Probably broken. If you want autocompletion (useful for editing agents and uploading files)
-
-For Bash:
-
-    eval "$(_OAICLI_COMPLETE=source_bash oaicli)"
-
-For Zsh:
-
-    eval "$(_OAICLI_COMPLETE=source_zsh oaicli)"
 
 ## Roadmap
 
-### v0.3
+### v0.3-0.5
 
  - upload doc from url, or get web contents
  - cat a directory into a single file and upload
  - share publicically OAICLI help agent, uploading entire github repo. For example "what changes would you make to README.md based on the source code"
+ - pydantic refactor
+ - stream response to console
 
  ### v1.x
 
 Have agents select and talk to each other.
 
 Other:
```

### Comparing `oaicli-0.2.2/pyproject.toml` & `oaicli-0.2.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [project]
 name = "oaicli"
-version = "0.2.2"
+version = "0.2.4"
 description = "A Command Line Interface to Open AI"
 authors = [{name = "Jonathan Hendler", email = "jonathan@hai.io"}]
 license = {file="LICENSE"}
 readme = "README.md"
-# repository = "https://github.com/HumanAssistedIntelligence/OAICLI"
+# repository = "https://github.com/HumanAssisted/OAICLI"
 keywords = ["cli", "openai", "api"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
     "click>=8.1.7",
-    "openai>=1.3.6",
+    "openai>=1.29.0",
     "python-dotenv>=1.0.0",
     "appdirs>=1.4.4",
-    "prompt-toolkit>=3.0.40"
+    "prompt-toolkit>=3.0.40",
 ]
 
 [project.optional-dependencies]
 dev = [
     "black>=23.11.0",
     "flake8>=6.1.0",
 ]
```

