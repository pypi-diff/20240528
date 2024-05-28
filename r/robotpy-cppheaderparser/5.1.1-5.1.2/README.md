# Comparing `tmp/robotpy-cppheaderparser-5.1.1.tar.gz` & `tmp/robotpy-cppheaderparser-5.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotpy-cppheaderparser-5.1.1.tar", last modified: Thu Oct  5 08:05:28 2023, max compression
+gzip compressed data, was "robotpy-cppheaderparser-5.1.2.tar", last modified: Tue May 28 03:07:44 2024, max compression
```

## Comparing `robotpy-cppheaderparser-5.1.1.tar` & `robotpy-cppheaderparser-5.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 08:05:28.842305 robotpy-cppheaderparser-5.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 08:05:28.842305 robotpy-cppheaderparser-5.1.1/CppHeaderParser/
--rw-r--r--   0 runner    (1001) docker     (127)   139054 2023-10-05 08:05:21.000000 robotpy-cppheaderparser-5.1.1/CppHeaderParser/CppHeaderParser.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2023-10-05 08:05:21.000000 robotpy-cppheaderparser-5.1.1/CppHeaderParser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2023-10-05 08:05:21.000000 robotpy-cppheaderparser-5.1.1/CppHeaderParser/doxygen.py
--rw-r--r--   0 runner    (1001) docker     (127)     6144 2023-10-05 08:05:21.000000 robotpy-cppheaderparser-5.1.1/CppHeaderParser/lexer.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2023-10-05 08:05:21.000000 robotpy-cppheaderparser-5.1.1/CppHeaderParser/tojson.py
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-10-05 08:05:28.000000 robotpy-cppheaderparser-5.1.1/CppHeaderParser/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2023-10-05 08:05:21.000000 robotpy-cppheaderparser-5.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2023-10-05 08:05:21.000000 robotpy-cppheaderparser-5.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4175 2023-10-05 08:05:28.842305 robotpy-cppheaderparser-5.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2531 2023-10-05 08:05:21.000000 robotpy-cppheaderparser-5.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 08:05:28.842305 robotpy-cppheaderparser-5.1.1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2023-10-05 08:05:21.000000 robotpy-cppheaderparser-5.1.1/examples/SampleClass.h
--rwxr-xr-x   0 runner    (1001) docker     (127)     2215 2023-10-05 08:05:21.000000 robotpy-cppheaderparser-5.1.1/examples/readSampleClass.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 08:05:28.842305 robotpy-cppheaderparser-5.1.1/robotpy_cppheaderparser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4175 2023-10-05 08:05:28.000000 robotpy-cppheaderparser-5.1.1/robotpy_cppheaderparser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      535 2023-10-05 08:05:28.000000 robotpy-cppheaderparser-5.1.1/robotpy_cppheaderparser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-05 08:05:28.000000 robotpy-cppheaderparser-5.1.1/robotpy_cppheaderparser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2023-10-05 08:05:28.000000 robotpy-cppheaderparser-5.1.1/robotpy_cppheaderparser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-10-05 08:05:28.000000 robotpy-cppheaderparser-5.1.1/robotpy_cppheaderparser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2023-10-05 08:05:28.842305 robotpy-cppheaderparser-5.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2023-10-05 08:05:21.000000 robotpy-cppheaderparser-5.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 08:05:28.842305 robotpy-cppheaderparser-5.1.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)   124226 2023-10-05 08:05:21.000000 robotpy-cppheaderparser-5.1.1/test/test_CppHeaderParser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 03:07:44.798989 robotpy-cppheaderparser-5.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 03:07:44.794989 robotpy-cppheaderparser-5.1.2/CppHeaderParser/
+-rw-r--r--   0 runner    (1001) docker     (127)   140801 2024-05-28 03:07:39.000000 robotpy-cppheaderparser-5.1.2/CppHeaderParser/CppHeaderParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-28 03:07:39.000000 robotpy-cppheaderparser-5.1.2/CppHeaderParser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-28 03:07:39.000000 robotpy-cppheaderparser-5.1.2/CppHeaderParser/doxygen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6144 2024-05-28 03:07:39.000000 robotpy-cppheaderparser-5.1.2/CppHeaderParser/lexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-28 03:07:39.000000 robotpy-cppheaderparser-5.1.2/CppHeaderParser/tojson.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-28 03:07:44.000000 robotpy-cppheaderparser-5.1.2/CppHeaderParser/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-28 03:07:39.000000 robotpy-cppheaderparser-5.1.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-28 03:07:39.000000 robotpy-cppheaderparser-5.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-05-28 03:07:44.798989 robotpy-cppheaderparser-5.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-05-28 03:07:39.000000 robotpy-cppheaderparser-5.1.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 03:07:44.794989 robotpy-cppheaderparser-5.1.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-28 03:07:39.000000 robotpy-cppheaderparser-5.1.2/examples/SampleClass.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2215 2024-05-28 03:07:39.000000 robotpy-cppheaderparser-5.1.2/examples/readSampleClass.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 03:07:44.794989 robotpy-cppheaderparser-5.1.2/robotpy_cppheaderparser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-05-28 03:07:44.000000 robotpy-cppheaderparser-5.1.2/robotpy_cppheaderparser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-28 03:07:44.000000 robotpy-cppheaderparser-5.1.2/robotpy_cppheaderparser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 03:07:44.000000 robotpy-cppheaderparser-5.1.2/robotpy_cppheaderparser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-28 03:07:44.000000 robotpy-cppheaderparser-5.1.2/robotpy_cppheaderparser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-28 03:07:44.000000 robotpy-cppheaderparser-5.1.2/robotpy_cppheaderparser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-28 03:07:44.798989 robotpy-cppheaderparser-5.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-05-28 03:07:39.000000 robotpy-cppheaderparser-5.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 03:07:44.798989 robotpy-cppheaderparser-5.1.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)   126372 2024-05-28 03:07:39.000000 robotpy-cppheaderparser-5.1.2/test/test_CppHeaderParser.py
```

### Comparing `robotpy-cppheaderparser-5.1.1/CppHeaderParser/CppHeaderParser.py` & `robotpy-cppheaderparser-5.1.2/CppHeaderParser/CppHeaderParser.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,14 +137,15 @@
 
 #: Symbols to ignore, usually special macros
 ignoreSymbols = ["Q_OBJECT"]
 
 _BRACE_REASON_OTHER = 0
 _BRACE_REASON_NS = 1
 _BRACE_REASON_EXTERN = 2
+_BRACE_REASON_VARIABLE = 3
 
 # Track what was added in what order and at what depth
 parseHistory = []
 
 
 def is_namespace(nameStack):
     """Determines if a namespace is being specified"""
@@ -235,18 +236,21 @@
     return r
 
 
 def is_property_namestack(nameStack):
     r = False
     if "(" not in nameStack and ")" not in nameStack:
         r = True
-    elif (
-        "(" in nameStack
-        and "=" in nameStack
-        and nameStack.index("=") < nameStack.index("(")
+    elif "(" in nameStack and (
+        (  # = initialization
+            "=" in nameStack and nameStack.index("=") < nameStack.index("(")
+        )
+        or (  # {} initialization
+            "{" in nameStack and nameStack.index("{") < nameStack.index("(")
+        )
     ):
         r = True
     # See if we are a function pointer
     if not r and is_function_pointer_stack(nameStack):
         r = True
     return r
 
@@ -1213,37 +1217,56 @@
         debug_print("var trace %s", nameStack)
         if len(nameStack) and nameStack[0] == "extern":
             self["extern"] = True
             del nameStack[0]
         else:
             self["extern"] = False
 
+        if "=" in nameStack:
+            self["type"] = " ".join(nameStack[: nameStack.index("=") - 1])
+            self["name"] = nameStack[nameStack.index("=") - 1]
+            default = " ".join(nameStack[nameStack.index("=") + 1 :])
+            nameStack = nameStack[: nameStack.index("=")]
+            default = self._filter_name(default)
+            self["default"] = default
+            # backwards compat; deprecate camelCase in dicts
+            self["defaultValue"] = default
+        elif "{" in nameStack and "}" in nameStack:
+            posBracket = nameStack.index("{")
+            self["type"] = " ".join(nameStack[: posBracket - 1])
+            self["name"] = nameStack[posBracket - 1]
+            default = " ".join(nameStack[posBracket + 1 : -1])
+            nameStack = nameStack[:posBracket]
+            default = self._filter_name(default)
+            self["default"] = default
+            # backwards compat; deprecate camelCase in dicts
+            self["defaultValue"] = default
+
         _stack_ = nameStack
-        if "[" in nameStack:  # strip off array informatin
-            arrayStack = nameStack[nameStack.index("[") :]
-            if nameStack.count("[") > 1:
+        self["array"] = 0
+        while "]" in nameStack[-1]:  # strip off array information
+            arrayPos = len(nameStack) - 1 - nameStack[::-1].index("[")
+            arrayStack = nameStack[arrayPos:]
+            if self["array"] == 1:
                 debug_print("Multi dimensional array")
                 debug_print("arrayStack=%s", arrayStack)
-                nums = [x for x in arrayStack if x.isdigit()]
-                # Calculate size by multiplying all dimensions
-                p = 1
-                for n in nums:
-                    p *= int(n)
+                if len(arrayStack) == 3:
+                    n = arrayStack[1]
                 # Multi dimensional array
-                self["array_size"] = p
+                if not "multi_dimensional_array_size" in self:
+                    self["multi_dimensional_array_size"] = self["array_size"]
+                self["multi_dimensional_array_size"] += "x" + n
+                self["array_size"] = str(int(self["array_size"]) * int(n))
                 self["multi_dimensional_array"] = 1
-                self["multi_dimensional_array_size"] = "x".join(nums)
             else:
                 debug_print("Array")
                 if len(arrayStack) == 3:
                     self["array_size"] = arrayStack[1]
-            nameStack = nameStack[: nameStack.index("[")]
+            nameStack = nameStack[:arrayPos]
             self["array"] = 1
-        else:
-            self["array"] = 0
         nameStack = self._name_stack_helper(nameStack)
 
         if doxygen:
             self["doxygen"] = doxygen
 
         debug_print("Variable: %s", nameStack)
 
@@ -1264,23 +1287,14 @@
                 + nameStack[nameStack.index(")") :]
             )
             self["name"] = " ".join(
                 nameStack[nameStack.index("(") + 2 : nameStack.index(")")]
             )
             self["function_pointer"] = 1
 
-        elif "=" in nameStack:
-            self["type"] = " ".join(nameStack[: nameStack.index("=") - 1])
-            self["name"] = nameStack[nameStack.index("=") - 1]
-            default = " ".join(nameStack[nameStack.index("=") + 1 :])
-            default = self._filter_name(default)
-            self["default"] = default
-            # backwards compat; deprecate camelCase in dicts
-            self["defaultValue"] = default
-
         elif (
             is_fundamental(nameStack[-1])
             or nameStack[-1] in [">", "<", ":", "."]
             or (len(nameStack) > 2 and nameStack[-2] == "::")
         ):
             # Un named parameter
             self["type"] = " ".join(nameStack)
@@ -1875,17 +1889,17 @@
                         elif "::" in var:
                             var["ctypes_type"] = "ctypes.c_void_p"
                             var["unresolved"] = True
 
                         elif tag in self._template_typenames:
                             var["typename"] = tag
                             var["ctypes_type"] = "ctypes.c_void_p"
-                            var[
-                                "unresolved"
-                            ] = True  # TODO, how to deal with templates?
+                            var["unresolved"] = (
+                                True  # TODO, how to deal with templates?
+                            )
 
                         elif tag.startswith(
                             "_"
                         ):  # assume starting with underscore is not important for wrapping
                             warning_print("WARN unresolved %s", _tag)
                             var["ctypes_type"] = "ctypes.c_void_p"
                             var["unresolved"] = True
@@ -2927,15 +2941,31 @@
                     self._precomp_macro_buf.append((tok.value, tok.location))
                     self.stack = []
                     self.stmtTokens = []
                     self.nameStack = []
                     continue
 
                 if parenDepth == 0 and tok.type == "{":
-                    self.lastBraceReason = _BRACE_REASON_OTHER
+                    if self.nameStack[0] in (
+                        "class",
+                        "struct",
+                        "union",
+                        "namespace",
+                        "enum",
+                        "extern",
+                        "typedef",
+                    ) or (is_method_namestack(self.stack) or (not self.curClass)):
+                        self.lastBraceReason = _BRACE_REASON_OTHER
+                    else:
+                        # Case : type variable {init};
+                        self.lastBraceReason = _BRACE_REASON_VARIABLE
+                        self.braceDepth += 1
+                        self.braceReason.append(self.lastBraceReason)
+                        self.nameStack.append(tok.value)
+                        continue
                     if len(self.nameStack) >= 2 and is_namespace(
                         self.nameStack
                     ):  # namespace {} with no name used in boost, this sets default?
                         self.nameSpaces.append("".join(self.nameStack[1:]))
                         ns = self.cur_namespace()
                         self.stack = []
                         self.stmtTokens = []
@@ -2987,14 +3017,18 @@
                         self.nameSpaces.pop()
                         self.stack = []  # clear stack when namespace ends?
                         self.stmtTokens = []
                     elif reason == _BRACE_REASON_EXTERN:
                         self.linkage_stack.pop()
                         self.stack = []  # clear stack when linkage ends?
                         self.stmtTokens = []
+                    # Case : type variable {init};
+                    elif reason == _BRACE_REASON_VARIABLE:
+                        self.nameStack.append(tok.value)
+                        continue
                     else:
                         self._evaluate_stack()
                     self.braceDepth -= 1
 
                     # if self.curClass:
                     #     debug_print(
                     #         "CURBD %s", self._classes_brace_level[self.curClass]
```

### Comparing `robotpy-cppheaderparser-5.1.1/CppHeaderParser/doxygen.py` & `robotpy-cppheaderparser-5.1.2/CppHeaderParser/doxygen.py`

 * *Files identical despite different names*

### Comparing `robotpy-cppheaderparser-5.1.1/CppHeaderParser/lexer.py` & `robotpy-cppheaderparser-5.1.2/CppHeaderParser/lexer.py`

 * *Files identical despite different names*

### Comparing `robotpy-cppheaderparser-5.1.1/LICENSE.txt` & `robotpy-cppheaderparser-5.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotpy-cppheaderparser-5.1.1/PKG-INFO` & `robotpy-cppheaderparser-5.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: robotpy-cppheaderparser
-Version: 5.1.1
+Version: 5.1.2
 Summary: Parse C++ header files and generate a data structure representing the class
 Home-page: https://github.com/robotpy/robotpy-cppheaderparser
 Author: Jashua Cloutier
 Author-email: jashuac@bellsouth.net
 Maintainer: RobotPy Development Team
 Maintainer-email: robotpy@googlegroups.com
 License: BSD
```

### Comparing `robotpy-cppheaderparser-5.1.1/README.rst` & `robotpy-cppheaderparser-5.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `robotpy-cppheaderparser-5.1.1/examples/SampleClass.h` & `robotpy-cppheaderparser-5.1.2/examples/SampleClass.h`

 * *Files identical despite different names*

### Comparing `robotpy-cppheaderparser-5.1.1/examples/readSampleClass.py` & `robotpy-cppheaderparser-5.1.2/examples/readSampleClass.py`

 * *Files identical despite different names*

### Comparing `robotpy-cppheaderparser-5.1.1/robotpy_cppheaderparser.egg-info/PKG-INFO` & `robotpy-cppheaderparser-5.1.2/robotpy_cppheaderparser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: robotpy-cppheaderparser
-Version: 5.1.1
+Version: 5.1.2
 Summary: Parse C++ header files and generate a data structure representing the class
 Home-page: https://github.com/robotpy/robotpy-cppheaderparser
 Author: Jashua Cloutier
 Author-email: jashuac@bellsouth.net
 Maintainer: RobotPy Development Team
 Maintainer-email: robotpy@googlegroups.com
 License: BSD
```

### Comparing `robotpy-cppheaderparser-5.1.1/robotpy_cppheaderparser.egg-info/SOURCES.txt` & `robotpy-cppheaderparser-5.1.2/robotpy_cppheaderparser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robotpy-cppheaderparser-5.1.1/setup.py` & `robotpy-cppheaderparser-5.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `robotpy-cppheaderparser-5.1.1/test/test_CppHeaderParser.py` & `robotpy-cppheaderparser-5.1.2/test/test_CppHeaderParser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1158,22 +1158,17 @@
                 self.cppHeader.classes["CarrotClass"]["methods"]["private"][0][
                     "parameters"
                 ]
             ),
             [],
         )
 
-    def test_class_template(self):
-        self.assertEqual(
-            self.cppHeader.classes["CarrotClass"]["template"], "template<class T>"
-        )
-
 
 # Bug 3517289
-class CarrotClass_TestCase(unittest.TestCase):
+class ExternClass_TestCase(unittest.TestCase):
     def setUp(self):
         self.cppHeader = CppHeaderParser.CppHeader("TestSampleClass.h")
 
     def test_num_private_methods(self):
         self.assertEqual(
             len(self.cppHeader.classes["ExternClass"]["methods"]["private"]), 1
         )
@@ -2360,15 +2355,15 @@
 class Picture_TestCase(unittest.TestCase):
     def setUp(self):
         self.cppHeader = CppHeaderParser.CppHeader("TestSampleClass.h")
 
     def test_array_size(self):
         self.assertEqual(
             self.cppHeader.classes["Picture"]["properties"]["public"][1]["array_size"],
-            16384,
+            "16384",
         )
 
     def test_multi_dimensional_array_size(self):
         self.assertEqual(
             self.cppHeader.classes["Picture"]["properties"]["public"][1][
                 "multi_dimensional_array_size"
             ],
@@ -4223,9 +4218,92 @@
         # FnNotCS should not in namespace cs nor extern C
         fn = self.cppHeader.functions[1]
         self.assertEqual(fn["name"], "FnNotInCSOrExtern")
         self.assertEqual(fn["namespace"], "")
         self.assertEqual(fn["linkage"], "")
 
 
+# Github PR 85
+class ContainerOfArray_TestCase(unittest.TestCase):
+    def setUp(self):
+        self.cppHeader = CppHeaderParser.CppHeader(
+            """
+class ContainerOfArray {
+public:
+    std::unique_ptr<int[]> variable;
+    std::unique_ptr<int[]> function(std::unique_ptr<int[]> param1);
+};
+""",
+            "string",
+        )
+
+    def test_rtntype(self):
+        self.assertEqual(
+            self.cppHeader.classes["ContainerOfArray"]["methods"]["public"][0][
+                "rtnType"
+            ],
+            "std::unique_ptr<int [ ] >",
+        )
+
+    def test_parameters(self):
+        self.assertEqual(
+            filter_pameters(
+                self.cppHeader.classes["ContainerOfArray"]["methods"]["public"][0][
+                    "parameters"
+                ]
+            ),
+            [{"name": "param1", "desc": None, "type": "std::unique_ptr<int [ ] >"}],
+        )
+
+    def test_member(self):
+        self.assertEqual(
+            self.cppHeader.classes["ContainerOfArray"]["properties"]["public"][0][
+                "name"
+            ],
+            "variable",
+        )
+        self.assertEqual(
+            self.cppHeader.classes["ContainerOfArray"]["properties"]["public"][0][
+                "type"
+            ],
+            "std::unique_ptr<int [ ] >",
+        )
+
+
+class InitBracket_TestCase(unittest.TestCase):
+    def setUp(self):
+        self.cppHeader = CppHeaderParser.CppHeader(
+            """
+class InitBracket {
+public:
+    int variable{10};
+    std::shared_ptr<int> variable2 {std::make_shared<int>(150)};
+};
+""",
+            "string",
+        )
+
+    def test_member(self):
+        self.assertEqual(
+            self.cppHeader.classes["InitBracket"]["properties"]["public"][0]["name"],
+            "variable",
+        )
+        self.assertEqual(
+            self.cppHeader.classes["InitBracket"]["properties"]["public"][0][
+                "defaultValue"
+            ],
+            "10",
+        )
+        self.assertEqual(
+            self.cppHeader.classes["InitBracket"]["properties"]["public"][1]["name"],
+            "variable2",
+        )
+        self.assertEqual(
+            self.cppHeader.classes["InitBracket"]["properties"]["public"][1][
+                "defaultValue"
+            ],
+            "std::make_shared<int> ( 150 )",
+        )
+
+
 if __name__ == "__main__":
     unittest.main()
```

