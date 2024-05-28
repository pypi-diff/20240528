# Comparing `tmp/atla-0.1.0a5.tar.gz` & `tmp/atla-0.1.0a6.tar.gz`

## Comparing `atla-0.1.0a5.tar` & `atla-0.1.0a6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 atla-0.1.0a5/src/atla/__init__.py
--rw-r--r--   0        0        0    64410 2020-02-02 00:00:00.000000 atla-0.1.0a5/src/atla/_base_client.py
--rw-r--r--   0        0        0    17710 2020-02-02 00:00:00.000000 atla-0.1.0a5/src/atla/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 atla-0.1.0a5/src/atla/_compat.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 atla-0.1.0a5/src/atla/_constants.py
--rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 atla-0.1.0a5/src/atla/_exceptions.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 atla-0.1.0a5/src/atla/_files.py
--rw-r--r--   0        0        0    26876 2020-02-02 00:00:00.000000 atla-0.1.0a5/src/atla/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 atla-0.1.0a5/src/atla/_qs.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 atla-0.1.0a5/src/atla/_resource.py
--rw-r--r--   0        0        0    28363 2020-02-02 00:00:00.000000 atla-0.1.0a5/src/atla/_response.py
--rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 atla-0.1.0a5/src/atla/_streaming.py
--rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 atla-0.1.0a5/src/atla/_types.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 atla-0.1.0a5/src/atla/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 atla-0.1.0a5/src/atla/py.typed
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 atla-0.1.0a5/src/atla/_utils/__init__.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 atla-0.1.0a5/src/atla/_utils/_logs.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 atla-0.1.0a5/src/atla/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 atla-0.1.0a5/src/atla/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 atla-0.1.0a5/src/atla/_utils/_sync.py
--rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 atla-0.1.0a5/src/atla/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 atla-0.1.0a5/src/atla/_utils/_typing.py
--rw-r--r--   0        0        0    11447 2020-02-02 00:00:00.000000 atla-0.1.0a5/src/atla/_utils/_utils.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 atla-0.1.0a5/src/atla/lib/.keep
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 atla-0.1.0a5/src/atla/resources/__init__.py
--rw-r--r--   0        0        0     6134 2020-02-02 00:00:00.000000 atla-0.1.0a5/src/atla/resources/evaluate.py
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 atla-0.1.0a5/src/atla/types/__init__.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 atla-0.1.0a5/src/atla/types/evaluate_create_params.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 atla-0.1.0a5/src/atla/types/evaluate_create_response.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 atla-0.1.0a5/.gitignore
--rw-r--r--   0        0        0    11334 2020-02-02 00:00:00.000000 atla-0.1.0a5/LICENSE
--rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 atla-0.1.0a5/pyproject.toml
--rw-r--r--   0        0        0    14608 2020-02-02 00:00:00.000000 atla-0.1.0a5/PKG-INFO
+-rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/__init__.py
+-rw-r--r--   0        0        0    64410 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/_base_client.py
+-rw-r--r--   0        0        0    17710 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/_compat.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/_constants.py
+-rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/_exceptions.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/_files.py
+-rw-r--r--   0        0        0    26876 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/_qs.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/_resource.py
+-rw-r--r--   0        0        0    28363 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/_response.py
+-rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/_streaming.py
+-rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/_types.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/py.typed
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/_utils/__init__.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/_utils/_logs.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/_utils/_sync.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/_utils/_typing.py
+-rw-r--r--   0        0        0    11447 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/lib/.keep
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/resources/__init__.py
+-rw-r--r--   0        0        0     6060 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/resources/evaluate.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/types/__init__.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/types/evaluate_create_params.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/types/evaluation.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 atla-0.1.0a6/.gitignore
+-rw-r--r--   0        0        0    11334 2020-02-02 00:00:00.000000 atla-0.1.0a6/LICENSE
+-rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 atla-0.1.0a6/pyproject.toml
+-rw-r--r--   0        0        0    14571 2020-02-02 00:00:00.000000 atla-0.1.0a6/PKG-INFO
```

### Comparing `atla-0.1.0a5/src/atla/__init__.py` & `atla-0.1.0a6/src/atla/__init__.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a5/src/atla/_base_client.py` & `atla-0.1.0a6/src/atla/_base_client.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a5/src/atla/_client.py` & `atla-0.1.0a6/src/atla/_client.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a5/src/atla/_compat.py` & `atla-0.1.0a6/src/atla/_compat.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a5/src/atla/_exceptions.py` & `atla-0.1.0a6/src/atla/_exceptions.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a5/src/atla/_files.py` & `atla-0.1.0a6/src/atla/_files.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a5/src/atla/_models.py` & `atla-0.1.0a6/src/atla/_models.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a5/src/atla/_qs.py` & `atla-0.1.0a6/src/atla/_qs.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a5/src/atla/_resource.py` & `atla-0.1.0a6/src/atla/_resource.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a5/src/atla/_response.py` & `atla-0.1.0a6/src/atla/_response.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a5/src/atla/_streaming.py` & `atla-0.1.0a6/src/atla/_streaming.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a5/src/atla/_types.py` & `atla-0.1.0a6/src/atla/_types.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a5/src/atla/_utils/__init__.py` & `atla-0.1.0a6/src/atla/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a5/src/atla/_utils/_logs.py` & `atla-0.1.0a6/src/atla/_utils/_logs.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a5/src/atla/_utils/_proxy.py` & `atla-0.1.0a6/src/atla/_utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a5/src/atla/_utils/_sync.py` & `atla-0.1.0a6/src/atla/_utils/_sync.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a5/src/atla/_utils/_transform.py` & `atla-0.1.0a6/src/atla/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a5/src/atla/_utils/_typing.py` & `atla-0.1.0a6/src/atla/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a5/src/atla/_utils/_utils.py` & `atla-0.1.0a6/src/atla/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a5/src/atla/resources/__init__.py` & `atla-0.1.0a6/src/atla/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a5/src/atla/resources/evaluate.py` & `atla-0.1.0a6/src/atla/resources/evaluate.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     to_streamed_response_wrapper,
     async_to_raw_response_wrapper,
     async_to_streamed_response_wrapper,
 )
 from .._base_client import (
     make_request_options,
 )
-from ..types.evaluate_create_response import EvaluateCreateResponse
+from ..types.evaluation import Evaluation
 
 __all__ = ["EvaluateResource", "AsyncEvaluateResource"]
 
 
 class EvaluateResource(SyncAPIResource):
     @cached_property
     def with_raw_response(self) -> EvaluateResourceWithRawResponse:
@@ -48,15 +48,15 @@
         reference: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> EvaluateCreateResponse:
+    ) -> Evaluation:
         """
         Creates a model evaluation for a given LLM input and response.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
@@ -77,15 +77,15 @@
                     "reference": reference,
                 },
                 evaluate_create_params.EvaluateCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=EvaluateCreateResponse,
+            cast_to=Evaluation,
         )
 
 
 class AsyncEvaluateResource(AsyncAPIResource):
     @cached_property
     def with_raw_response(self) -> AsyncEvaluateResourceWithRawResponse:
         return AsyncEvaluateResourceWithRawResponse(self)
@@ -105,15 +105,15 @@
         reference: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> EvaluateCreateResponse:
+    ) -> Evaluation:
         """
         Creates a model evaluation for a given LLM input and response.
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
@@ -134,15 +134,15 @@
                     "reference": reference,
                 },
                 evaluate_create_params.EvaluateCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=EvaluateCreateResponse,
+            cast_to=Evaluation,
         )
 
 
 class EvaluateResourceWithRawResponse:
     def __init__(self, evaluate: EvaluateResource) -> None:
         self._evaluate = evaluate
```

### Comparing `atla-0.1.0a5/src/atla/types/evaluate_create_params.py` & `atla-0.1.0a6/src/atla/types/evaluate_create_params.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a5/src/atla/types/evaluate_create_response.py` & `atla-0.1.0a6/src/atla/types/evaluation.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from typing import Dict, Optional
 
 from .._models import BaseModel
 
-__all__ = ["EvaluateCreateResponse", "Evaluations", "Usage"]
+__all__ = ["Evaluation", "Evaluations", "Usage"]
 
 
 class Evaluations(BaseModel):
     critique: object
 
     score: int
 
@@ -17,15 +17,15 @@
     evaluation_tokens: int
 
     prompt_tokens: int
 
     total_tokens: int
 
 
-class EvaluateCreateResponse(BaseModel):
+class Evaluation(BaseModel):
     evaluations: Dict[str, Evaluations]
 
     model: str
 
     usage: Usage
 
     id: Optional[str] = None
```

### Comparing `atla-0.1.0a5/LICENSE` & `atla-0.1.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a5/pyproject.toml` & `atla-0.1.0a6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "atla"
-version = "0.1.0-alpha.5"
+version = "0.1.0-alpha.6"
 description = "The official Python library for the atla API"
 dynamic = ["readme"]
 license = "Apache-2.0"
 authors = [
 { name = "Atla", email = "support@atla.com" },
 ]
 dependencies = [
```

### Comparing `atla-0.1.0a5/PKG-INFO` & `atla-0.1.0a6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: atla
-Version: 0.1.0a5
+Version: 0.1.0a6
 Summary: The official Python library for the atla API
 Project-URL: Homepage, https://github.com/atla-ai/atla-sdk-python
 Project-URL: Repository, https://github.com/atla-ai/atla-sdk-python
 Author-email: Atla <support@atla.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
@@ -65,20 +65,20 @@
 client = Atla(
     # This is the default and can be omitted
     api_key=os.environ.get("ATLA_API_KEY"),
     # defaults to "production".
     environment="development",
 )
 
-evaluate_create_response = client.evaluate.create(
+score = client.evaluate.create(
     input="The sentence you are given might be too wordy, complicated, or unclear. Rewrite the sentence and make your writing clearer by keeping it concise. Whenever possible, break complex sentences into multiple sentences and eliminate unnecessary words.",
     metrics=["precision", "recall"],
     response="If you have any questions about my rate, please let me know.",
 )
-print(evaluate_create_response.evaluations)
+print(score.evaluations.recall.score)
 ```
 
 While you can provide an `api_key` keyword argument,
 we recommend using [python-dotenv](https://pypi.org/project/python-dotenv/)
 to add `ATLA_API_KEY="My API Key"` to your `.env` file
 so that your API Key is not stored in source control.
 
@@ -96,20 +96,20 @@
     api_key=os.environ.get("ATLA_API_KEY"),
     # defaults to "production".
     environment="development",
 )
 
 
 async def main() -> None:
-    evaluate_create_response = await client.evaluate.create(
+    score = await client.evaluate.create(
         input="The sentence you are given might be too wordy, complicated, or unclear. Rewrite the sentence and make your writing clearer by keeping it concise. Whenever possible, break complex sentences into multiple sentences and eliminate unnecessary words.",
         metrics=["precision", "recall"],
         response="If you have any questions about my rate, please let me know.",
     )
-    print(evaluate_create_response.evaluations)
+    print(score.evaluations.recall.score)
 
 
 asyncio.run(main())
 ```
 
 Functionality between the synchronous and asynchronous clients is otherwise identical.
 
@@ -259,15 +259,15 @@
     input="The sentence you are given might be too wordy, complicated, or unclear. Rewrite the sentence and make your writing clearer by keeping it concise. Whenever possible, break complex sentences into multiple sentences and eliminate unnecessary words.",
     metrics=["precision", "recall"],
     response="If you have any questions about my rate, please let me know.",
 )
 print(response.headers.get('X-My-Header'))
 
 evaluate = response.parse()  # get the object that `evaluate.create()` would have returned
-print(evaluate.evaluations)
+print(evaluate.evaluations_recall_score)
 ```
 
 These methods return an [`APIResponse`](https://github.com/atla-ai/atla-sdk-python/tree/main/src/atla/_response.py) object.
 
 The async client returns an [`AsyncAPIResponse`](https://github.com/atla-ai/atla-sdk-python/tree/main/src/atla/_response.py) with the same structure, the only difference being `await`able methods for reading the response content.
 
 #### `.with_streaming_response`
```

