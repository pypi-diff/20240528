# Comparing `tmp/schemafunc-0.2.0.tar.gz` & `tmp/schemafunc-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schemafunc-0.2.0.tar", max compression
+gzip compressed data, was "schemafunc-0.3.0.tar", max compression
```

## Comparing `schemafunc-0.2.0.tar` & `schemafunc-0.3.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1069 2024-04-11 16:31:26.401239 schemafunc-0.2.0/LICENSE
--rw-r--r--   0        0        0     1139 2024-04-14 16:09:41.782786 schemafunc-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     6278 2024-04-12 20:52:00.845243 schemafunc-0.2.0/README.md
--rw-r--r--   0        0        0    12127 2024-04-14 16:04:13.480496 schemafunc-0.2.0/src/schemafunc.py
--rw-r--r--   0        0        0     7289 1970-01-01 00:00:00.000000 schemafunc-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-11 16:31:26.401239 schemafunc-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1139 2024-05-28 18:48:29.945819 schemafunc-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6614 2024-04-14 16:41:56.673792 schemafunc-0.3.0/README.md
+-rw-r--r--   0        0        0    19796 2024-05-28 18:46:08.076593 schemafunc-0.3.0/src/schemafunc.py
+-rw-r--r--   0        0        0     7625 1970-01-01 00:00:00.000000 schemafunc-0.3.0/PKG-INFO
```

### Comparing `schemafunc-0.2.0/LICENSE` & `schemafunc-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `schemafunc-0.2.0/pyproject.toml` & `schemafunc-0.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "schemafunc"
-version = "0.2.0"
+version = "0.3.0"
 description = "Python function-to-LLM tool maker."
 authors = ["Dustin Wyatt <dustin.wyatt@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/dmwyatt/schemafunc"
 
 keywords = ["python", "openai", "llm", "language-model", "schema", "function", "tool"]
```

### Comparing `schemafunc-0.2.0/README.md` & `schemafunc-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 signature.
 
 The intended use case is for LLM tool usage and output constraints.
 
 Future updates should include explicit support for other LLMs, though the current 
 functionality probably works with most or can be easily adapted.
 
+Supports Python 3.8+.
+
 ## Output constraints?
 
 You don't actually have to *really* want the LLM to "use a tool". You might just want 
 to ensure it always returns valid JSON in a specific format.  "Function calling" or 
 "tool usage" actually ends up being a great way to enforce that.  Just create a 
 function whose arguments match the output you want. You don't actually have to use the 
 function, but when you tell the LLM the function is available, it will constrain its 
@@ -23,25 +25,35 @@
 * Manually keeping the JSON description of a python function up-to-date is 
   error-prone. Even if you use something like `pydantic` to build and enforce the 
   schema, you still end up with two sources of truth that you have to keep in sync.
 * It's tedious and irritating to have to write the same information twice.
 * In my experience, writing a Python function is more ergonomic, natural, and less 
   error-prone than writing a JSON schema by hand. Even if you were to use `pydantic` 
   and create a model that models the expected schema, I still find that it's not a 
-  great mental model to map from a `BaseModel` to a function signature.
+  great mental model to map from a `BaseModel` to the type of "tool call" that OpenAI 
+  and others expect.
 
 ## Key features
 
 * **Automatic**: The schema is generated from the function.
   * Add `@add_schemafunc` to your function and your schema is done.
 * Tool schema available as a property of the function, so you can access it easily.
   * `your_own_function.schemafunc.schema` 
 * Easy tool kwargs for `openai` chat completions API.
   * `your_own_function.schemafunc.openai_tool_kwargs`
   * Use by unpacking the kwargs into the `openai` API call.
+* Extracts the function description from the first line of the docstring.
+* Extracts parameter descriptions from the docstring parameter list.
+* Supports Numpy-style, Google-style, and RestructuredText-style docstrings.
+
+## Installation
+    
+```bash
+pip install schemafunc
+```
 
 ## Example
 
 ### Quick Example
 
 ```python
 import openai
```

### Comparing `schemafunc-0.2.0/src/schemafunc.py` & `schemafunc-0.3.0/src/schemafunc.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import inspect
 import typing
 from collections.abc import Sequence, Set
 from functools import cached_property, wraps
+from types import MappingProxyType
 
 from docstring_parser import Docstring, parse
 
 
 class FunctionMetadata:
     def __init__(self, func, **schema_kwargs):
         self.func = func
@@ -50,84 +51,203 @@
 
 class NoDocstringError(Exception):
     pass
 
 
 def function_to_schema(
     func: typing.Callable,
-    require_param_descriptions: bool = True,
-    allow_bare_generic_types: bool = False,
-    ignore_undocumented_params: bool = False,
-    ignore_no_docstring: bool = False,
+    require_all_params_in_doc: bool = True,
+    require_descriptions_for_params: bool = True,
+    allow_bare_generic_types: bool = True,
+    require_short_description: bool = True,
 ) -> dict:
+    """
+    Generates a JSON schema from a given function.
+
+    The function's parameters and their types, as well as the descriptions provided
+    in the function's docstring, are included in the resulting schema. This provides
+    a machine-readable definition of the function's expected inputs and behaviors.
+
+    Parameters:
+        func (typing.Callable): The function to be converted into a schema.
+        require_all_params_in_doc (bool, optional): If True, an exception is raised
+            if not all parameters are documented. Defaults to True.
+        require_descriptions_for_params (bool, optional): If True, an exception is
+            raised if a documented parameter lacks a description. Defaults to True.
+        allow_bare_generic_types (bool, optional): If True, bare generic types such
+            as List, Dict are allowed. Defaults to True.
+        require_short_description (bool, optional): If True, an exception is raised
+            if the function docstring lacks a short description. Defaults to True.
+
+    Returns:
+        dict: A representation of the function as a JSON schema.
+
+    Raises:
+        NoDocstringError: Raised if the function lacks a docstring and
+            require_all_params_in_doc is True.
+        NoShortDescriptionError: Raised if function docstring lacks a short
+            description and require_short_description is True.
+        ValueError: Raised if a parameter lacks a type annotation.
+        BareGenericTypeError: Raised if a parameter has a bare generic type and
+            allow_bare_generic_types is False.
+        ParameterNotDocumentedError: Raised if a parameter is not documented in the
+            docstring and require_all_params_in_doc is True.
+        ParameterMissingDescriptionError: Raised if a parameter is documented but
+            lacks a description and require_descriptions_for_params is True.
+
+    Examples:
+        >>> def example_function(param1: int):
+        ...    '''
+        ...    Simple example function.
+        ...    Args:
+        ...        param1 (int): The first parameter.
+        ...    '''
+        ...    pass
+
+
+        >>> function_to_schema(example_function)
+        {'type': 'function', 'function': {'name': 'example_function', 'description': 'Simple example function.', 'parameters': {'type': 'object', 'properties': {'param1': {'type': 'integer', 'description': 'The first parameter.'}}, 'required': ['param1']}}}
+    """
     signature = inspect.signature(func)
-    docstring = parse(func.__doc__)
+    docstring = parse(func.__doc__) if func.__doc__ else None
+
+    if (
+        require_all_params_in_doc
+        or require_descriptions_for_params
+        or require_short_description
+    ) and docstring is None:
+        raise NoDocstringError("The function must have a docstring")
+
+    if require_short_description and not docstring.short_description:
+        raise NoShortDescriptionError(
+            "The function must have a short description in the docstring"
+        )
 
-    if not docstring.short_description:
-        if not ignore_no_docstring:
-            raise NoDocstringError("The function must have a docstring")
+    if require_all_params_in_doc and signature.parameters:
+        # list of missing parameters. Missing if not in docstring
+        missing_params = [
+            param_name
+            for param_name in signature.parameters
+            if param_name not in [p.arg_name for p in getattr(docstring, "params", [])]
+        ]
+        if missing_params:
+            raise ParameterNotDocumentedError(
+                "The following parameters are not documented in the docstring: "
+                + ", ".join(missing_params)
+            )
+
+    if require_descriptions_for_params:
+        # list of parameters with missing descriptions
+        missing_desc_params = [
+            param.arg_name for param in docstring.params if not param.description
+        ]
+
+        if missing_desc_params:
+            raise ParameterMissingDescriptionError(
+                f"The following parameters are missing descriptions in the docstring: {', '.join(missing_desc_params)}"
+            )
 
     parameters = process_parameters(
         signature,
         docstring,
-        require_param_descriptions,
         allow_bare_generic_types,
-        ignore_undocumented_params,
-        ignore_no_docstring,
     )
-    return generate_schema(func, docstring, parameters, ignore_no_docstring)
+    return generate_schema(func, docstring, parameters)
 
 
 class ParameterNotDocumentedError(Exception):
     pass
 
 
 class ParameterMissingDescriptionError(Exception):
     pass
 
 
 def process_parameters(
     signature: inspect.Signature,
     docstring: Docstring,
-    require_param_descriptions: bool,
     allow_bare_generic_types: bool,
-    ignore_undocumented_params: bool,
-    ignore_no_docstring: bool,
-) -> dict:
+) -> typing.Dict[str, typing.Any]:
+    """
+    Generates JSON schema representation of the parameters of a function.
+
+    This function systematically processes the parameters of a given function,
+    guided by their type annotations and any related documentation provided
+    within the function's docstring, and constructs a comprehensive JSON schema
+    representation.
+
+    Parameters:
+        signature (inspect.Signature): A Signature object of the function
+            to process.
+        docstring (Docstring): A parsed docstring object which includes
+            parameter's documentation.
+        allow_bare_generic_types (bool): A boolean parameter that indicates
+            whether to allow bare generic types (like List, Dict) without a
+            specific item type. If True, it will instantiate the item type
+            as an empty object. If False, it will raise a BareGenericTypeError
+            for any parameter having a bare generic type.
+
+    Returns:
+        dict: A dictionary object that represents the JSON schema of the
+            parameters of the function. Each entry represents a parameter,
+            with its name as the key and the associated JSON schema as the
+            value.
+
+    Raises:
+        ValueError: If a parameter lacks a type annotation.
+        BareGenericTypeError: If allow_bare_generic_types is False and a
+            parameter has a bare generic type.
+
+    Example:
+        >>> from inspect import signature
+        >>> from docstring_parser import parse
+
+        >>> def example_function(param: int):
+        ...     '''
+        ...     Example function.
+        ...
+        ...     Args:
+        ...         param: The first parameter.
+        ...     '''
+        ...     pass
+        >>> sig = signature(example_function)
+        >>> doc = parse(example_function.__doc__)
+        >>> process_parameters(sig, doc, allow_bare_generic_types=False)
+        {'param': {'type': 'integer', 'description': 'The first parameter.'}}
+
+    Note:
+        Always provide type annotations for parameters in the function's
+        signature. The function relies on these annotations to accurately define
+        the JSON schema. The function also leverages the related documentation
+        within the function's docstring to enhance the precision of the results,
+        providing expanded context when required.
+    """
     parameters = {}
 
     for name, param in signature.parameters.items():
         if param.annotation == inspect.Parameter.empty:
             raise ValueError(f"Parameter {name} must have a type annotation")
 
         param_type = param.annotation
-        param_docstring = next(
-            (p for p in docstring.params if p.arg_name == name), None
+        param_docstring = (
+            next((p for p in docstring.params if p.arg_name == name), None)
+            if docstring
+            else None
         )
 
         try:
             param_schema = resolve_type(param_type)
         except BareGenericTypeError:
             if allow_bare_generic_types:
                 param_schema = {"type": "array", "items": {}}  # Unspecified item type
             else:
                 raise
 
-        if param_docstring is None:
-            if not ignore_undocumented_params and not ignore_no_docstring:
-                raise ParameterNotDocumentedError(
-                    f"Parameter {name} is not documented in the docstring"
-                )
-        else:
-            if require_param_descriptions and not param_docstring.description:
-                raise ParameterMissingDescriptionError(
-                    f"Parameter {name} is missing a description in the docstring"
-                )
-            if param_docstring.description:
-                param_schema["description"] = param_docstring.description
+        if param_docstring and param_docstring.description:
+            param_schema["description"] = param_docstring.description
 
         if param.default != inspect.Parameter.empty and param.default is not None:
             param_schema["default"] = param.default
 
         parameters[name] = param_schema
 
     return parameters
@@ -137,28 +257,20 @@
     pass
 
 
 def generate_schema(
     func: typing.Callable,
     docstring: Docstring,
     parameters: dict,
-    ignore_no_docstring: bool,
 ) -> dict:
-    if not docstring.short_description and not ignore_no_docstring:
-        raise NoShortDescriptionError(
-            "The function must have a short description in the docstring"
-        )
-
     schema = {
         "type": "function",
         "function": {
             "name": func.__name__,
-            "description": docstring.short_description
-            if docstring.short_description
-            else "",
+            "description": getattr(docstring, "description", "").strip(),
             "parameters": {
                 "type": "object",
                 "properties": parameters,
                 "required": [
                     name
                     for name, param in inspect.signature(func).parameters.items()
                     if param.default == inspect.Parameter.empty
@@ -166,56 +278,104 @@
             },
         },
     }
 
     return schema
 
 
-json_schema_types = {
-    int: "integer",
-    float: "number",
-    str: "string",
-    bool: "boolean",
-    None: "null",
-    type(None): "null",
-    # Include both None and type(None) in the dictionary to handle two scenarios:
-    #
-    # 1. When a function parameter is annotated with None directly, such as:
-    #      def func(param: None):
-    #    The None key is used to map the type to the JSON Schema type "null".
-    #
-    # 2. When a function parameter is part of a union type with None, such as:
-    #      def func(param: typing.Union[int, None]):
-    #    The type(None) key is used when resolving the union type to map the None type
-    #    to the JSON Schema type "null".
-    #
-    # By including both None and type(None), the code can handle both scenarios
-    # correctly and avoid raising a ValueError for unsupported types.
-}
+JSON_SCHEMA_TYPES = MappingProxyType(
+    {
+        int: "integer",
+        float: "number",
+        str: "string",
+        bool: "boolean",
+        # Include both None and type(None) in the dictionary to handle two scenarios:
+        #
+        # 1. When a function parameter is annotated with None directly, such as:
+        #      def func(param: None):
+        #    The None key is used to map the type to the JSON Schema type "null".
+        #
+        # 2. When a function parameter is part of a union type with None, such as:
+        #      def func(param: typing.Union[int, None]):
+        #    The type(None) key is used when resolving the union type to map the None type
+        #    to the JSON Schema type "null".
+        #
+        # By including both None and type(None), the code can handle both scenarios
+        # correctly and avoid raising a ValueError for unsupported types.
+        None: "null",
+        type(None): "null",
+    }
+)
+
+
+class UnsupportedTypeError(Exception):
+    pass
 
 
 def resolve_type(param_type: typing.Type) -> dict:
+    """
+    Resolves a Python type into a JSON Schema dictionary.
+
+    This function takes a Python type (such as `int`, `str`, `typing.Union`,
+    `typing.List`, etc.) and returns a dictionary representing the equivalent
+    JSON Schema type.
+
+    Args:
+        param_type (typing.Type): The Python type to resolve.
+
+    Returns:
+        dict: A dictionary representing the JSON Schema equivalent of the input type.
+
+    Raises:
+        UnsupportedTypeError: If the input type is not supported by the function.
+
+    Examples:
+        >>> resolve_type(int)
+        {'type': 'integer'}
+
+        >>> resolve_type(typing.List[str])
+        {'type': 'array', 'items': {'type': 'string'}}
+
+        >>> resolve_type(typing.Union[int, str])
+        {'type': ['integer', 'string']}
+
+    The function supports the following types:
+
+    - Basic types (`int`, `float`, `str`, `bool`, `None`): These are converted to the
+      corresponding JSON Schema types (`'integer'`, `'number'`, `'string'`,
+      `'boolean'`, `'null'`).
+
+    - Union types (`typing.Union`): These are converted to a JSON Schema type array,
+      where each element represents one of the types in the union.
+
+    - Array types (`typing.List`, `typing.Tuple`, `typing.Set`, etc.): These are
+      converted to a JSON Schema `'array'` type, with the `items` property
+      representing the type of the array elements.
+
+    - Literal types (`typing.Literal`): These are converted to a JSON Schema
+      `'string'` type, with an `enum` property listing the permitted literal values.
+    """
     if is_basic_type(param_type):
         return resolve_basic_type(param_type)
     elif is_union_type(param_type):
         return resolve_union_type(param_type)
     elif is_array_type(param_type):
         return resolve_array_type(param_type)
     elif is_literal_type(param_type):
         return resolve_literal_type(param_type)
     else:
-        raise ValueError(f"Unsupported type: {param_type}")
+        raise UnsupportedTypeError(f"Unsupported type: {param_type}")
 
 
 def is_basic_type(param_type: typing.Type) -> bool:
-    return param_type in json_schema_types
+    return param_type in JSON_SCHEMA_TYPES
 
 
 def resolve_basic_type(param_type: typing.Type) -> dict:
-    return {"type": json_schema_types[param_type]}
+    return {"type": JSON_SCHEMA_TYPES[param_type]}
 
 
 def is_union_type(param_type: typing.Type) -> bool:
     return typing.get_origin(param_type) == typing.Union
 
 
 def resolve_union_type(param_type: typing.Type) -> dict:
@@ -259,14 +419,41 @@
         else:
             schema["type"].append(resolved_type["type"])
 
     return schema
 
 
 def is_array_type(param_type: typing.Type) -> bool:
+    """
+    Determines if the given type is representable as a JavaScript array.
+
+    This function handles both generic types and non-generic types. It uses
+    `typing.get_origin` to get the original generic type for generic types,
+    and falls back to the input type itself for non-generic types.
+
+    Args:
+        param_type (typing.Type): The type to check.
+
+    Returns:
+        bool: True if the type is representable as a JavaScript array, False otherwise.
+
+    Examples:
+        >>> is_array_type(typing.List[int])
+        True
+        >>> is_array_type(typing.Tuple[int, str, bool])
+        True
+        >>> is_array_type(list)
+        True
+        >>> is_array_type(tuple)
+        True
+        >>> is_array_type(dict)
+        False
+        >>> is_array_type(str)
+        False
+    """
     return is_representable_as_js_array(typing.get_origin(param_type) or param_type)
 
 
 class BareGenericTypeError(ValueError):
     pass
```

### Comparing `schemafunc-0.2.0/PKG-INFO` & `schemafunc-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schemafunc
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python function-to-LLM tool maker.
 Home-page: https://github.com/dmwyatt/schemafunc
 License: MIT
 Keywords: python,openai,llm,language-model,schema,function,tool
 Author: Dustin Wyatt
 Author-email: dustin.wyatt@gmail.com
 Requires-Python: >=3.8.10,<4.0.0
@@ -29,14 +29,16 @@
 signature.
 
 The intended use case is for LLM tool usage and output constraints.
 
 Future updates should include explicit support for other LLMs, though the current 
 functionality probably works with most or can be easily adapted.
 
+Supports Python 3.8+.
+
 ## Output constraints?
 
 You don't actually have to *really* want the LLM to "use a tool". You might just want 
 to ensure it always returns valid JSON in a specific format.  "Function calling" or 
 "tool usage" actually ends up being a great way to enforce that.  Just create a 
 function whose arguments match the output you want. You don't actually have to use the 
 function, but when you tell the LLM the function is available, it will constrain its 
@@ -48,25 +50,35 @@
 * Manually keeping the JSON description of a python function up-to-date is 
   error-prone. Even if you use something like `pydantic` to build and enforce the 
   schema, you still end up with two sources of truth that you have to keep in sync.
 * It's tedious and irritating to have to write the same information twice.
 * In my experience, writing a Python function is more ergonomic, natural, and less 
   error-prone than writing a JSON schema by hand. Even if you were to use `pydantic` 
   and create a model that models the expected schema, I still find that it's not a 
-  great mental model to map from a `BaseModel` to a function signature.
+  great mental model to map from a `BaseModel` to the type of "tool call" that OpenAI 
+  and others expect.
 
 ## Key features
 
 * **Automatic**: The schema is generated from the function.
   * Add `@add_schemafunc` to your function and your schema is done.
 * Tool schema available as a property of the function, so you can access it easily.
   * `your_own_function.schemafunc.schema` 
 * Easy tool kwargs for `openai` chat completions API.
   * `your_own_function.schemafunc.openai_tool_kwargs`
   * Use by unpacking the kwargs into the `openai` API call.
+* Extracts the function description from the first line of the docstring.
+* Extracts parameter descriptions from the docstring parameter list.
+* Supports Numpy-style, Google-style, and RestructuredText-style docstrings.
+
+## Installation
+    
+```bash
+pip install schemafunc
+```
 
 ## Example
 
 ### Quick Example
 
 ```python
 import openai
```

