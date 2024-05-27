# Comparing `tmp/promptic-0.4.5.tar.gz` & `tmp/promptic-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptic-0.4.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "promptic-0.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `promptic-0.4.5.tar` & `promptic-0.5.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      555 2024-05-27 22:30:42.716118 promptic-0.4.5/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0     3156 2024-05-27 22:30:42.716118 promptic-0.4.5/.gitignore
--rw-r--r--   0        0        0     9161 2024-05-27 22:30:42.716118 promptic-0.4.5/LICENSE
--rw-r--r--   0        0        0     3017 2024-05-27 22:30:42.716118 promptic-0.4.5/README.md
--rw-r--r--   0        0        0     3767 2024-05-27 22:30:42.716118 promptic-0.4.5/promptic.py
--rw-r--r--   0        0        0      527 2024-05-27 22:30:42.716118 promptic-0.4.5/pyproject.toml
--rw-r--r--   0        0        0     3365 1970-01-01 00:00:00.000000 promptic-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0      487 2024-05-27 23:09:52.547532 promptic-0.5.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0     3156 2024-05-27 23:09:52.547532 promptic-0.5.0/.gitignore
+-rw-r--r--   0        0        0     9161 2024-05-27 23:09:52.547532 promptic-0.5.0/LICENSE
+-rw-r--r--   0        0        0     3525 2024-05-27 23:09:52.547532 promptic-0.5.0/README.md
+-rw-r--r--   0        0        0     4109 2024-05-27 23:09:52.547532 promptic-0.5.0/promptic.py
+-rw-r--r--   0        0        0      527 2024-05-27 23:09:52.547532 promptic-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3873 1970-01-01 00:00:00.000000 promptic-0.5.0/PKG-INFO
```

### Comparing `promptic-0.4.5/.gitignore` & `promptic-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `promptic-0.4.5/LICENSE` & `promptic-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `promptic-0.4.5/README.md` & `promptic-0.5.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -43,27 +43,43 @@
 
 ### Streaming Response (and [litellm][litellm] integration)
 
 ```python
 from promptic import llm
 
 @llm(
-    # keyword args are passed to litellm.completion
+    # most arguments are passed directly to litellm.completion
+    # see https://docs.litellm.ai/docs/completion
     stream=True,
     model="claude-3-haiku-20240307",
 )
-def haiku(subject, adjective, verb):
+def haiku(subject, adjective, verb="delights"):
     """Write a haiku about {subject} that is {adjective} and {verb}."""
 
-print("".join(haiku("programming", "witty", "delights")))
+print("".join(haiku("programming", adjective="witty")))
 # Bits and bytes abound,
 # Bugs and features intertwine,
 # Code, the poet's rhyme.
 ```
 
+### Customize System Prompt
+
+```python
+from promptic import llm
+
+@llm(system="you are a snarky chatbot")
+def answer(question):
+    """{question}"""
+
+print(answer("What's the best programming language?"))
+# Well, that's like asking what's the best flavor of ice cream. 
+# It really depends on what you're trying to accomplish and your personal preferences. 
+# But if you want to start a flame war, just bring up Python vs JavaScript.
+```
+
 ## Features
 
 - **Decorator-based API**: Easily define prompts using function docstrings and decorate them with `@promptic.llm`.
 - **Argument interpolation**: Automatically interpolate function arguments into the prompt using `{argument_name}` placeholders within docstrings.
 - **Pydantic model support**: Specify the expected output structure using Pydantic models, and `promptic` will ensure the LLM's response conforms to the defined schema.
 - **Streaming support**: Receive LLM responses in real-time by setting `stream=True` when calling the decorated function.
 - **Simplified LLM interaction**: No need to remember the exact shape of the OpenAPI response object or other LLM-specific details. `promptic` abstracts away the complexities, allowing you to focus on defining prompts and receiving structured outputs.
```

### Comparing `promptic-0.4.5/promptic.py` & `promptic-0.5.0/promptic.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,20 @@
 
 import litellm
 from pydantic import BaseModel
 
 logger = logging.getLogger(__name__)
 
 
-def promptic(fn=None, model="gpt-3.5-turbo", **litellm_kwargs):
+def promptic(
+    fn=None,
+    model="gpt-3.5-turbo",
+    system: str = None,
+    **litellm_kwargs,
+):
     logger.debug(f"{fn = }")
     logger.debug(f"{model = }")
     logger.debug(f"{litellm_kwargs = }")
 
     def decorator(func: Callable):
         @wraps(func)
         def wrapper(*args, **kwargs):
@@ -51,23 +56,37 @@
                 json_schema = json.dumps(schema, indent=2)
                 # Update the prompt to specify the expected JSON format
                 prompt_text += f"\n\nThe result should conform to the following JSON schema:\n```json\n{json_schema}\n```"
                 prompt_text += "\n\nPlease provide the result enclosed in triple backticks with 'json' on the first line."
 
             logger.debug(f"{prompt_text = }")
 
+            messages = []
+
+            if system:
+                messages.append(
+                    {
+                        "content": system,
+                        "role": "system",
+                    }
+                )
+            
+            messages.append(
+                {
+                    "content": prompt_text,
+                    "role": "user",
+                }
+            )
+
+            logger.debug(f"{messages = }")
+
             # Call the LLM with the prompt
             response = litellm.completion(
                 model=model,
-                messages=[
-                    {
-                        "content": prompt_text,
-                        "role": "user",
-                    },
-                ],
+                messages=messages,
                 **litellm_kwargs,
             )
 
             if litellm_kwargs.get("stream"):
                 return _stream_response(response)
             else:
                 # Get the generated text from the LLM response
```

### Comparing `promptic-0.4.5/pyproject.toml` & `promptic-0.5.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -8,12 +8,12 @@
 description = "A simple yet powerful abstraction for litellm and pydantic"
 license = {file = "LICENSE"}
 name = "promptic"
 requires = [
   "litellm~=1.38",
   "pydantic~=2.7",
 ]
-version = "0.4.5"
+version = "0.5.0"
 readme = "README.md"
 
 [project.urls]
 Home = "https://github.com/knowsuchagency/promptic"
```

### Comparing `promptic-0.4.5/PKG-INFO` & `promptic-0.5.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptic
-Version: 0.4.5
+Version: 0.5.0
 Summary: A simple yet powerful abstraction for litellm and pydantic
 Author-email: Stephan Fitzpatrick <knowsuchagency@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Project-URL: Home, https://github.com/knowsuchagency/promptic
 
 # promptic
@@ -52,27 +52,43 @@
 
 ### Streaming Response (and [litellm][litellm] integration)
 
 ```python
 from promptic import llm
 
 @llm(
-    # keyword args are passed to litellm.completion
+    # most arguments are passed directly to litellm.completion
+    # see https://docs.litellm.ai/docs/completion
     stream=True,
     model="claude-3-haiku-20240307",
 )
-def haiku(subject, adjective, verb):
+def haiku(subject, adjective, verb="delights"):
     """Write a haiku about {subject} that is {adjective} and {verb}."""
 
-print("".join(haiku("programming", "witty", "delights")))
+print("".join(haiku("programming", adjective="witty")))
 # Bits and bytes abound,
 # Bugs and features intertwine,
 # Code, the poet's rhyme.
 ```
 
+### Customize System Prompt
+
+```python
+from promptic import llm
+
+@llm(system="you are a snarky chatbot")
+def answer(question):
+    """{question}"""
+
+print(answer("What's the best programming language?"))
+# Well, that's like asking what's the best flavor of ice cream. 
+# It really depends on what you're trying to accomplish and your personal preferences. 
+# But if you want to start a flame war, just bring up Python vs JavaScript.
+```
+
 ## Features
 
 - **Decorator-based API**: Easily define prompts using function docstrings and decorate them with `@promptic.llm`.
 - **Argument interpolation**: Automatically interpolate function arguments into the prompt using `{argument_name}` placeholders within docstrings.
 - **Pydantic model support**: Specify the expected output structure using Pydantic models, and `promptic` will ensure the LLM's response conforms to the defined schema.
 - **Streaming support**: Receive LLM responses in real-time by setting `stream=True` when calling the decorated function.
 - **Simplified LLM interaction**: No need to remember the exact shape of the OpenAPI response object or other LLM-specific details. `promptic` abstracts away the complexities, allowing you to focus on defining prompts and receiving structured outputs.
```

