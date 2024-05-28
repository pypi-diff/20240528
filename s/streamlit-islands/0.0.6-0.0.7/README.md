# Comparing `tmp/streamlit-islands-0.0.6.tar.gz` & `tmp/streamlit-islands-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-islands-0.0.6.tar", last modified: Sun May 26 14:08:16 2024, max compression
+gzip compressed data, was "streamlit-islands-0.0.7.tar", last modified: Tue May 28 10:40:42 2024, max compression
```

## Comparing `streamlit-islands-0.0.6.tar` & `streamlit-islands-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 anasb     (1000) anasb     (1000)        0 2024-05-26 14:08:16.303913 streamlit-islands-0.0.6/
--rw-r--r--   0 anasb     (1000) anasb     (1000)     1067 2024-03-04 22:49:07.000000 streamlit-islands-0.0.6/LICENSE.txt
--rw-r--r--   0 anasb     (1000) anasb     (1000)     5089 2024-05-26 14:08:16.303913 streamlit-islands-0.0.6/PKG-INFO
--rw-r--r--   0 anasb     (1000) anasb     (1000)     4720 2024-05-26 14:06:17.000000 streamlit-islands-0.0.6/README.md
--rw-r--r--   0 anasb     (1000) anasb     (1000)       38 2024-05-26 14:08:16.303913 streamlit-islands-0.0.6/setup.cfg
--rw-r--r--   0 anasb     (1000) anasb     (1000)      845 2024-05-26 14:08:05.000000 streamlit-islands-0.0.6/setup.py
-drwxr-xr-x   0 anasb     (1000) anasb     (1000)        0 2024-05-26 14:08:16.303913 streamlit-islands-0.0.6/streamlit_islands/
--rw-r--r--   0 anasb     (1000) anasb     (1000)     4753 2024-05-26 14:06:02.000000 streamlit-islands-0.0.6/streamlit_islands/__init__.py
--rw-r--r--   0 anasb     (1000) anasb     (1000)      325 2024-05-26 12:30:40.000000 streamlit-islands-0.0.6/streamlit_islands/demo.py
--rw-r--r--   0 anasb     (1000) anasb     (1000)        0 2024-05-25 05:53:34.000000 streamlit-islands-0.0.6/streamlit_islands/test.py
-drwxr-xr-x   0 anasb     (1000) anasb     (1000)        0 2024-05-26 14:08:16.303913 streamlit-islands-0.0.6/streamlit_islands.egg-info/
--rw-r--r--   0 anasb     (1000) anasb     (1000)     5089 2024-05-26 14:08:15.000000 streamlit-islands-0.0.6/streamlit_islands.egg-info/PKG-INFO
--rw-r--r--   0 anasb     (1000) anasb     (1000)      329 2024-05-26 14:08:16.000000 streamlit-islands-0.0.6/streamlit_islands.egg-info/SOURCES.txt
--rw-r--r--   0 anasb     (1000) anasb     (1000)        1 2024-05-26 14:08:15.000000 streamlit-islands-0.0.6/streamlit_islands.egg-info/dependency_links.txt
--rw-r--r--   0 anasb     (1000) anasb     (1000)       16 2024-05-26 14:08:16.000000 streamlit-islands-0.0.6/streamlit_islands.egg-info/requires.txt
--rw-r--r--   0 anasb     (1000) anasb     (1000)       18 2024-05-26 14:08:16.000000 streamlit-islands-0.0.6/streamlit_islands.egg-info/top_level.txt
-drwxr-xr-x   0 anasb     (1000) anasb     (1000)        0 2024-05-26 14:08:16.303913 streamlit-islands-0.0.6/test/
--rw-r--r--   0 anasb     (1000) anasb     (1000)      441 2024-05-26 12:52:00.000000 streamlit-islands-0.0.6/test/test.py
+drwxr-xr-x   0 anasb     (1000) anasb     (1000)        0 2024-05-28 10:40:42.762274 streamlit-islands-0.0.7/
+-rw-r--r--   0 anasb     (1000) anasb     (1000)     1067 2024-03-04 22:49:07.000000 streamlit-islands-0.0.7/LICENSE.txt
+-rw-r--r--   0 anasb     (1000) anasb     (1000)     6656 2024-05-28 10:40:42.762274 streamlit-islands-0.0.7/PKG-INFO
+-rw-r--r--   0 anasb     (1000) anasb     (1000)     6287 2024-05-27 09:35:50.000000 streamlit-islands-0.0.7/README.md
+-rw-r--r--   0 anasb     (1000) anasb     (1000)       38 2024-05-28 10:40:42.762274 streamlit-islands-0.0.7/setup.cfg
+-rw-r--r--   0 anasb     (1000) anasb     (1000)      845 2024-05-28 10:40:38.000000 streamlit-islands-0.0.7/setup.py
+drwxr-xr-x   0 anasb     (1000) anasb     (1000)        0 2024-05-28 10:40:42.762274 streamlit-islands-0.0.7/streamlit_islands/
+-rw-r--r--   0 anasb     (1000) anasb     (1000)     4825 2024-05-28 10:38:57.000000 streamlit-islands-0.0.7/streamlit_islands/__init__.py
+-rw-r--r--   0 anasb     (1000) anasb     (1000)      325 2024-05-26 12:30:40.000000 streamlit-islands-0.0.7/streamlit_islands/demo.py
+-rw-r--r--   0 anasb     (1000) anasb     (1000)        0 2024-05-25 05:53:34.000000 streamlit-islands-0.0.7/streamlit_islands/test.py
+drwxr-xr-x   0 anasb     (1000) anasb     (1000)        0 2024-05-28 10:40:42.762274 streamlit-islands-0.0.7/streamlit_islands.egg-info/
+-rw-r--r--   0 anasb     (1000) anasb     (1000)     6656 2024-05-28 10:40:42.000000 streamlit-islands-0.0.7/streamlit_islands.egg-info/PKG-INFO
+-rw-r--r--   0 anasb     (1000) anasb     (1000)      329 2024-05-28 10:40:42.000000 streamlit-islands-0.0.7/streamlit_islands.egg-info/SOURCES.txt
+-rw-r--r--   0 anasb     (1000) anasb     (1000)        1 2024-05-28 10:40:42.000000 streamlit-islands-0.0.7/streamlit_islands.egg-info/dependency_links.txt
+-rw-r--r--   0 anasb     (1000) anasb     (1000)       16 2024-05-28 10:40:42.000000 streamlit-islands-0.0.7/streamlit_islands.egg-info/requires.txt
+-rw-r--r--   0 anasb     (1000) anasb     (1000)       18 2024-05-28 10:40:42.000000 streamlit-islands-0.0.7/streamlit_islands.egg-info/top_level.txt
+drwxr-xr-x   0 anasb     (1000) anasb     (1000)        0 2024-05-28 10:40:42.762274 streamlit-islands-0.0.7/test/
+-rw-r--r--   0 anasb     (1000) anasb     (1000)      483 2024-05-28 02:20:23.000000 streamlit-islands-0.0.7/test/test.py
```

### Comparing `streamlit-islands-0.0.6/LICENSE.txt` & `streamlit-islands-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-islands-0.0.6/PKG-INFO` & `streamlit-islands-0.0.7/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,38 @@
-Metadata-Version: 2.1
-Name: streamlit-islands
-Version: 0.0.6
-Summary: Separate static content from dynamic content in Streamlit
-Home-page: https://github.com/bouzidanas/streamlit-islands
-Author: Anas Bouzid
-Author-email: anasbouzid@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 streamlit-islands  [![Version](https://img.shields.io/pypi/v/streamlit-islands)](https://pypi.org/project/streamlit-islands/#history) 
 [![PyPi - Downloads](https://img.shields.io/pypi/dm/streamlit-islands)](https://pypi.org/project/streamlit-islands/#files)[![Component Demo](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://islands-demo.streamlit.app/)
 ============
 
 Separate static content from dynamic content in Streamlit
 
-## Overview
-For content heavy Streamlit applications, it can be useful to separate static content from dynamic/interactive content. This package provides a way to do that by allowing you to define static content in markdown files which then leaves you to focus on the logic heavy parts of your application in your Streamlit script. 
-
-To use this package, you define your static content in markdown files and insert special placeholders within the markdown in the locations where you want to insert dynamic content. The package then reads the markdown file and splits it at the placeholders. The static content is passed to `st.markdown` or `st.write` and the placeholders are replaced with calls to functions you define in your Streamlit script that contain the dynamic or interactive parts of the app.
-
 ## Installation
 Install [streamlit-islands](https://pypi.org/project/streamlit-islands/) with pip:
 ```bash
 pip install streamlit-islands
 ```
 
+## Overview
+For content heavy Streamlit applications, it can be useful to separate static content from dynamic/interactive content. This package provides a way to do that by allowing you to define static content in markdown files which then leaves you to focus on the logic heavy parts of your application in your Streamlit script. 
+
+To use this package, you define your static content in markdown files and insert special placeholders within the markdown in the locations where you want to insert dynamic content. The package then reads the markdown file and splits it at the placeholders. The static content is passed to `st.markdown` or `st.write` and the placeholders are replaced with calls to functions you define in your Streamlit script that contain the dynamic or interactive parts of the app.
+
+### Why 'islands'?
+The general idea here can be achieved in other ways but this package is designed to make it easy and to encourage a separation of concerns. Inspiration for the name comes from [Astro Islands](https://docs.astro.build/en/concepts/islands/).
+
+While the concept of 'islands' architecture is not the same as what this package does, the idea of separating static and dynamic regions of the app is similar.
+
+It might be useful to think of the dynamic parts of the app as 'islands' in a sea of static content. These islands are where the user interacts with the app and where the logic of the app is executed. Islands in the same app share the same global scope and thus can share data (variables, functions. etc) and state (`session_state`, etc).
+
+>[!NOTE]
+>*You can achieve something even closer to 'component islands' if you decorate the functions (that add dynamic parts of the script) with the `@st.experimental_fragment` decorator. This turns those dynamic parts of the script into fragments which can rerun independently of the full script!*
+
 ## Usage
 To use this package, you need to have a markdown file that contains the static content of your Streamlit app and a Streamlit script that contains the dynamic content.
 
-## Markdown file
+### Markdown file
 The markdown file should contain the static content of your Streamlit app. Use placeholders to indicate where functions that add dynamic content should be called.
 
 #### Placeholder format
 The placeholders in the markdown file must be formatted as follows:
 
 ```
 (empty line)
@@ -44,59 +41,76 @@
 (empty line)
 ```
 The `function_name` should be the name of the function you define in your Streamlit script that contains the dynamic content. The args should be the arguments you want to pass to the function (seperated by commas). The arguments should what the function expects. For example, if the function expects a list of strings, the args should be in the format `['arg1', 'arg2']`. 
 
 This special format is specifically designed to be ignored by markdown parsers so that the markdown file can still be rendered as expected. 
 
 >[!NOTE]
->The `args` inside the parentheses can span multiple lines.
+>*The `args` inside the parentheses can span multiple lines.*
 
 There is one additional requirement for the placeholders. There must be an empty line ***before AND after*** the placeholder. Anything that comes directly after (not separated by an empty line) will be removed before the markdown is added to the Streamlit app. This is to allow you to add backup content, comments, or other content to the markdown file that you don't want to be rendered in the app but you ***DO*** want to be rendered by markdown parsers.
 
-## Streamlit script
+#### Example: `my-markdown-file.md`
+```markdown
+# My header
+
+This is a test of the markdown content for the `streamlit-islands` package.
+This is a paragraph. It contains a few sentences. 
+
+[add]: # (1, 2)
+
+We start another paragraph here. This is a test of the markdown content for the `streamlit-islands` package.
+This is a paragraph. It contains a few sentences.
+
+[say_hello]: # ("Bob")
+
+## A subheader
+A new section of the document.
+```
+
+### Streamlit script
 To load the static content and add the dynamic content, you can use the `load_content` function from the `streamlit_islands` package. 
 
 ```python
 import streamlit as st
 import streamlit_islands as sti
 import os.path
 
 def say_hello(name):
-    st.write(name*10)
+    st.write("Hello, " + name)
 
 def add(a, b):
     if st.button('Show the result'):
         st.toast("The result is: " + str(a + b)) 
 
-# Test the function
+# Load the content of the markdown file
 file_path = os.path.join(os.path.dirname(__file__), "my-markdown-file.md")
 content = sti.load_content(file_path)
 ```
 
 The dynamic/interactive sections of the app are added by the functions you define in your Streamlit script. The functions that you want to be seen by `load_content` must be placed above where `load_content` is called. The function names must also match the names in the placeholders in the markdown file. The arguments passed to the functions should match the arguments in those placeholders as well. 
 
 >[!NOTE]
-> For organization purposes, you might want to have functions that are defined above `load_content` that you want to be ignored. You can do this using the `exclude` function from the `streamlit_islands` package.
+> *For organization purposes, you might want to have functions that are defined above `load_content` that you want to be ignored. You can do this using the `exclude` function from the `streamlit_islands` package.*
 
 ```python
 import streamlit as st
 import streamlit_islands as sti
 import os.path
 
 def say_hello(name):
-    st.write(name*10)
+    st.write("Hello, " + name)
 
 def add(a, b):
     if st.button('Show the result'):
         st.toast("The result is: " + str(a + b)) 
 
 # Exclude the function from being used by load_content
 sti.exclude("say_hello")
 
-# Test the function
+# Load the content of the markdown file
 file_path = os.path.join(os.path.dirname(__file__), "my-markdown-file.md")
 content = sti.load_content(file_path)
 ```
 
 ## License
-This project is licensed under the [MIT License](LICENSE.txt)
-
+This project is licensed under the [MIT License](LICENSE.txt)
```

### Comparing `streamlit-islands-0.0.6/setup.py` & `streamlit-islands-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "PROJECT.md").read_text()
 
 setup(
     name='streamlit-islands',
-    version='0.0.6',
+    version='0.0.7',
     author='Anas Bouzid',
     author_email='anasbouzid@gmail.com',
     description='Separate static content from dynamic content in Streamlit',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/bouzidanas/streamlit-islands",
     packages=find_packages(),
```

### Comparing `streamlit-islands-0.0.6/streamlit_islands/__init__.py` & `streamlit-islands-0.0.7/streamlit_islands/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
                 dynamic_content.append([temp_call_name, temp_call_args])
             else:
                 temp_call_args += line.split("]: # (")[1][-1]
                 in_dynamic_content = True
 
             if len(static_content) > 0:
                 for index in range(len(temp_content)):
-                    if temp_content[index].strip() == "":
+                    if temp_content[index] == "":
                         static_content.append("\n".join(temp_content[index:]))
                         break
             else:
                 static_content.append("\n".join(temp_content))
             temp_content = []
         elif in_dynamic_content and line.strip().endswith(")"):
             temp_call_args += line[:-1].strip()
@@ -68,15 +68,15 @@
             temp_call_args += line.strip()
         else:
             temp_content.append(line)
 
     # Make sure to add the last bit of static content        
     if len(temp_content) > 0:
         for index in range(len(temp_content)):
-            if temp_content[index].strip() == "":
+            if temp_content[index] == "":
                 static_content.append("\n".join(temp_content[index:]))
                 break
 
     return static_content, dynamic_content
 
 def call_local_function(function_name, arguments, function):
     try:
@@ -90,15 +90,15 @@
 
     for index in range(len(static_content)):
         if use_write:
             st.write(static_content[index], **kwargs)
         else:
             st.markdown(static_content[index], **kwargs)
         if len(dynamic_content) > index:
-            caller_globals = dict(inspect.getmembers(inspect.stack()[1][0]))["f_locals"]
+            caller_globals = dict(inspect.getmembers(inspect.stack()[1][0]))["f_locals"]  # This must be in a function called in the streamlit script to get the correct globals
             function_name = dynamic_content[index][0]
             function_args = "[" + dynamic_content[index][1] + "]"
             if function_name in caller_globals and callable(caller_globals[function_name]) and function_name not in excluded_functions:
                 call_local_function(function_name, function_args, caller_globals[function_name])
             else:
                 st.error('**ERROR!** `streamlit-islands` could not find a function called `<' + function_name + ">` in the streamlit script. Make sure the function is defined above the call to `load_content` and is not excluded.")
```

### Comparing `streamlit-islands-0.0.6/streamlit_islands.egg-info/PKG-INFO` & `streamlit-islands-0.0.7/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-islands
-Version: 0.0.6
+Version: 0.0.7
 Summary: Separate static content from dynamic content in Streamlit
 Home-page: https://github.com/bouzidanas/streamlit-islands
 Author: Anas Bouzid
 Author-email: anasbouzid@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
@@ -13,29 +13,39 @@
 
 streamlit-islands  [![Version](https://img.shields.io/pypi/v/streamlit-islands)](https://pypi.org/project/streamlit-islands/#history) 
 [![PyPi - Downloads](https://img.shields.io/pypi/dm/streamlit-islands)](https://pypi.org/project/streamlit-islands/#files)[![Component Demo](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://islands-demo.streamlit.app/)
 ============
 
 Separate static content from dynamic content in Streamlit
 
-## Overview
-For content heavy Streamlit applications, it can be useful to separate static content from dynamic/interactive content. This package provides a way to do that by allowing you to define static content in markdown files which then leaves you to focus on the logic heavy parts of your application in your Streamlit script. 
-
-To use this package, you define your static content in markdown files and insert special placeholders within the markdown in the locations where you want to insert dynamic content. The package then reads the markdown file and splits it at the placeholders. The static content is passed to `st.markdown` or `st.write` and the placeholders are replaced with calls to functions you define in your Streamlit script that contain the dynamic or interactive parts of the app.
-
 ## Installation
 Install [streamlit-islands](https://pypi.org/project/streamlit-islands/) with pip:
 ```bash
 pip install streamlit-islands
 ```
 
+## Overview
+For content heavy Streamlit applications, it can be useful to separate static content from dynamic/interactive content. This package provides a way to do that by allowing you to define static content in markdown files which then leaves you to focus on the logic heavy parts of your application in your Streamlit script. 
+
+To use this package, you define your static content in markdown files and insert special placeholders within the markdown in the locations where you want to insert dynamic content. The package then reads the markdown file and splits it at the placeholders. The static content is passed to `st.markdown` or `st.write` and the placeholders are replaced with calls to functions you define in your Streamlit script that contain the dynamic or interactive parts of the app.
+
+### Why 'islands'?
+The general idea here can be achieved in other ways but this package is designed to make it easy and to encourage a separation of concerns. Inspiration for the name comes from [Astro Islands](https://docs.astro.build/en/concepts/islands/).
+
+While the concept of 'islands' architecture is not the same as what this package does, the idea of separating static and dynamic regions of the app is similar.
+
+It might be useful to think of the dynamic parts of the app as 'islands' in a sea of static content. These islands are where the user interacts with the app and where the logic of the app is executed. Islands in the same app share the same global scope and thus can share data (variables, functions. etc) and state (`session_state`, etc).
+
+>[!NOTE]
+>*You can achieve something even closer to 'component islands' if you decorate the functions (that add dynamic parts of the script) with the `@st.experimental_fragment` decorator. This turns those dynamic parts of the script into fragments which can rerun independently of the full script!*
+
 ## Usage
 To use this package, you need to have a markdown file that contains the static content of your Streamlit app and a Streamlit script that contains the dynamic content.
 
-## Markdown file
+### Markdown file
 The markdown file should contain the static content of your Streamlit app. Use placeholders to indicate where functions that add dynamic content should be called.
 
 #### Placeholder format
 The placeholders in the markdown file must be formatted as follows:
 
 ```
 (empty line)
@@ -44,59 +54,77 @@
 (empty line)
 ```
 The `function_name` should be the name of the function you define in your Streamlit script that contains the dynamic content. The args should be the arguments you want to pass to the function (seperated by commas). The arguments should what the function expects. For example, if the function expects a list of strings, the args should be in the format `['arg1', 'arg2']`. 
 
 This special format is specifically designed to be ignored by markdown parsers so that the markdown file can still be rendered as expected. 
 
 >[!NOTE]
->The `args` inside the parentheses can span multiple lines.
+>*The `args` inside the parentheses can span multiple lines.*
 
 There is one additional requirement for the placeholders. There must be an empty line ***before AND after*** the placeholder. Anything that comes directly after (not separated by an empty line) will be removed before the markdown is added to the Streamlit app. This is to allow you to add backup content, comments, or other content to the markdown file that you don't want to be rendered in the app but you ***DO*** want to be rendered by markdown parsers.
 
-## Streamlit script
+#### Example: `my-markdown-file.md`
+```markdown
+# My header
+
+This is a test of the markdown content for the `streamlit-islands` package.
+This is a paragraph. It contains a few sentences. 
+
+[add]: # (1, 2)
+
+We start another paragraph here. This is a test of the markdown content for the `streamlit-islands` package.
+This is a paragraph. It contains a few sentences.
+
+[say_hello]: # ("Bob")
+
+## A subheader
+A new section of the document.
+```
+
+### Streamlit script
 To load the static content and add the dynamic content, you can use the `load_content` function from the `streamlit_islands` package. 
 
 ```python
 import streamlit as st
 import streamlit_islands as sti
 import os.path
 
 def say_hello(name):
-    st.write(name*10)
+    st.write("Hello, " + name)
 
 def add(a, b):
     if st.button('Show the result'):
         st.toast("The result is: " + str(a + b)) 
 
-# Test the function
+# Load the content of the markdown file
 file_path = os.path.join(os.path.dirname(__file__), "my-markdown-file.md")
 content = sti.load_content(file_path)
 ```
 
 The dynamic/interactive sections of the app are added by the functions you define in your Streamlit script. The functions that you want to be seen by `load_content` must be placed above where `load_content` is called. The function names must also match the names in the placeholders in the markdown file. The arguments passed to the functions should match the arguments in those placeholders as well. 
 
 >[!NOTE]
-> For organization purposes, you might want to have functions that are defined above `load_content` that you want to be ignored. You can do this using the `exclude` function from the `streamlit_islands` package.
+> *For organization purposes, you might want to have functions that are defined above `load_content` that you want to be ignored. You can do this using the `exclude` function from the `streamlit_islands` package.*
 
 ```python
 import streamlit as st
 import streamlit_islands as sti
 import os.path
 
 def say_hello(name):
-    st.write(name*10)
+    st.write("Hello, " + name)
 
 def add(a, b):
     if st.button('Show the result'):
         st.toast("The result is: " + str(a + b)) 
 
 # Exclude the function from being used by load_content
 sti.exclude("say_hello")
 
-# Test the function
+# Load the content of the markdown file
 file_path = os.path.join(os.path.dirname(__file__), "my-markdown-file.md")
 content = sti.load_content(file_path)
 ```
 
 ## License
 This project is licensed under the [MIT License](LICENSE.txt)
```

