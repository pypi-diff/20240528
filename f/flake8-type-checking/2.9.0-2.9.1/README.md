# Comparing `tmp/flake8_type_checking-2.9.0.tar.gz` & `tmp/flake8_type_checking-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8_type_checking-2.9.0.tar", max compression
+gzip compressed data, was "flake8_type_checking-2.9.1.tar", max compression
```

## Comparing `flake8_type_checking-2.9.0.tar` & `flake8_type_checking-2.9.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1520 2024-01-29 08:56:33.949797 flake8_type_checking-2.9.0/LICENSE
--rw-r--r--   0        0        0    14875 2024-01-29 08:56:33.949797 flake8_type_checking-2.9.0/README.md
--rw-r--r--   0        0        0        0 2024-01-29 08:56:33.949797 flake8_type_checking-2.9.0/flake8_type_checking/__init__.py
--rw-r--r--   0        0        0    83838 2024-01-29 08:56:33.949797 flake8_type_checking-2.9.0/flake8_type_checking/checker.py
--rw-r--r--   0        0        0     2088 2024-01-29 08:56:33.949797 flake8_type_checking-2.9.0/flake8_type_checking/constants.py
--rw-r--r--   0        0        0     6127 2024-01-29 08:56:33.949797 flake8_type_checking-2.9.0/flake8_type_checking/plugin.py
--rw-r--r--   0        0        0        0 2024-01-29 08:56:33.949797 flake8_type_checking-2.9.0/flake8_type_checking/py.typed
--rw-r--r--   0        0        0      789 2024-01-29 08:56:33.949797 flake8_type_checking-2.9.0/flake8_type_checking/types.py
--rw-r--r--   0        0        0     2009 2024-01-29 08:56:33.949797 flake8_type_checking-2.9.0/pyproject.toml
--rw-r--r--   0        0        0    16179 1970-01-01 00:00:00.000000 flake8_type_checking-2.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1520 2024-05-28 12:01:48.098991 flake8_type_checking-2.9.1/LICENSE
+-rw-r--r--   0        0        0    14875 2024-05-28 12:01:48.098991 flake8_type_checking-2.9.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-28 12:01:48.098991 flake8_type_checking-2.9.1/flake8_type_checking/__init__.py
+-rw-r--r--   0        0        0    85497 2024-05-28 12:01:48.098991 flake8_type_checking-2.9.1/flake8_type_checking/checker.py
+-rw-r--r--   0        0        0     2088 2024-05-28 12:01:48.098991 flake8_type_checking-2.9.1/flake8_type_checking/constants.py
+-rw-r--r--   0        0        0     6127 2024-05-28 12:01:48.098991 flake8_type_checking-2.9.1/flake8_type_checking/plugin.py
+-rw-r--r--   0        0        0        0 2024-05-28 12:01:48.098991 flake8_type_checking-2.9.1/flake8_type_checking/py.typed
+-rw-r--r--   0        0        0      789 2024-05-28 12:01:48.098991 flake8_type_checking-2.9.1/flake8_type_checking/types.py
+-rw-r--r--   0        0        0     2009 2024-05-28 12:01:48.098991 flake8_type_checking-2.9.1/pyproject.toml
+-rw-r--r--   0        0        0    16179 1970-01-01 00:00:00.000000 flake8_type_checking-2.9.1/PKG-INFO
```

### Comparing `flake8_type_checking-2.9.0/LICENSE` & `flake8_type_checking-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8_type_checking-2.9.0/README.md` & `flake8_type_checking-2.9.1/README.md`

 * *Files identical despite different names*

### Comparing `flake8_type_checking-2.9.0/flake8_type_checking/checker.py` & `flake8_type_checking-2.9.1/flake8_type_checking/checker.py`

 * *Files 2% similar despite different names*

```diff
@@ -750,14 +750,17 @@
         # classes are not real scopes, i.e. they don't propagate symbols
         # to inner-scopes, so we need to treat them differently in lookup
         # the class name itself is also special, since it's available in methods
         # but not in the class body itself, so we record it, so we can special-case
         # it in symbol lookups
         self.class_name = node.name if isinstance(node, ast.ClassDef) else None
 
+        #: Whether or not annotation assignments never get evaluated in this scope
+        self.ann_assign_never_evaluates = not is_head and isinstance(node, (ast.FunctionDef, ast.AsyncFunctionDef))
+
     def lookup(self, symbol_name: str, use: HasPosition | None = None, runtime_only: bool = True) -> Symbol | None:
         """
         Simulate a symbol lookup.
 
         If a symbol is redefined multiple times in the same block we don't try
         to return the symbol closest to the use-site, we just return the first
         one we find, since we don't really care what symbol we find currently.
@@ -820,42 +823,58 @@
     def __init__(self) -> None:
         #: All type annotations in the file, without quotes around them
         self.unwrapped_annotations: list[UnwrappedAnnotation] = []
 
         #: All type annotations in the file, with quotes around them
         self.wrapped_annotations: list[WrappedAnnotation] = []
 
+        #: All type annotations in the file with unnecessary quotes around them
+        self.excess_wrapped_annotations: list[WrappedAnnotation] = []
+
         #: All the invalid uses of string literals inside ast.BinOp
         self.invalid_binop_literals: list[ast.Constant] = []
 
+        #: Whether or not this annotation ever gets evaluated
+        # e.g. AnnAssign.annotation within a function body will never evaluate
+        self.never_evaluates = False
+
     def visit(
-        self, node: ast.AST, scope: Scope | None = None, type: Literal['annotation', 'alias', 'new-alias'] | None = None
+        self,
+        node: ast.AST,
+        scope: Scope | None = None,
+        type: Literal['annotation', 'alias', 'new-alias'] | None = None,
+        never_evaluates: bool | None = None,
     ) -> None:
         """Visit the node with the given scope and annotation type."""
         if scope is not None:
             self.scope = scope
         if type is not None:
             self.type = type
+        if never_evaluates is not None:
+            self.never_evaluates = never_evaluates
         super().visit(node)
 
     def visit_annotation_name(self, node: ast.Name) -> None:
         """Register unwrapped annotation."""
         setattr(node, ANNOTATION_PROPERTY, True)
+        if self.never_evaluates:
+            return
+
         self.unwrapped_annotations.append(
             UnwrappedAnnotation(node.lineno, node.col_offset, node.id, self.scope, self.type)
         )
 
     def visit_annotation_string(self, node: ast.Constant) -> None:
         """Register wrapped annotation and invalid binop literals."""
         setattr(node, ANNOTATION_PROPERTY, True)
         # we don't want to register them as both so we don't emit redundant errors
         if getattr(node, BINOP_OPERAND_PROPERTY, False):
             self.invalid_binop_literals.append(node)
         else:
-            self.wrapped_annotations.append(
+            (self.excess_wrapped_annotations if self.never_evaluates else self.wrapped_annotations).append(
                 WrappedAnnotation(
                     node.lineno, node.col_offset, node.value, set(NAME_RE.findall(node.value)), self.scope, self.type
                 )
             )
 
 
 class ImportVisitor(
@@ -968,14 +987,19 @@
 
     @property
     def wrapped_annotations(self) -> list[WrappedAnnotation]:
         """All type annotations in the file, with quotes around them."""
         return self.annotation_visitor.wrapped_annotations
 
     @property
+    def excess_wrapped_annotations(self) -> list[WrappedAnnotation]:
+        """All type annotations in the file, with excess quotes around them."""
+        return self.annotation_visitor.excess_wrapped_annotations
+
+    @property
     def invalid_binop_literals(self) -> list[ast.Constant]:
         """All invalid uses of binop literals."""
         return self.annotation_visitor.invalid_binop_literals
 
     @property
     def typing_module_name(self) -> str:
         """
@@ -1326,18 +1350,22 @@
 
     def visit_Constant(self, node: ast.Constant) -> ast.Constant:
         """Map constants."""
         super().visit_Constant(node)
         return node
 
     def add_annotation(
-        self, node: ast.AST, scope: Scope, type: Literal['annotation', 'alias', 'new-alias'] = 'annotation'
+        self,
+        node: ast.AST,
+        scope: Scope,
+        type: Literal['annotation', 'alias', 'new-alias'] = 'annotation',
+        never_evaluates: bool = False,
     ) -> None:
         """Map all annotations on an AST node."""
-        self.annotation_visitor.visit(node, scope, type)
+        self.annotation_visitor.visit(node, scope, type, never_evaluates)
 
     @staticmethod
     def set_child_node_attribute(node: Any, attr: str, val: Any) -> Any:
         """Set the parent attribute on the current node children."""
         for key, value in node.__dict__.items():
             if type(value) not in [int, str, list, bool] and value is not None and not key.startswith('_'):
                 setattr(node.__dict__[key], attr, val)
@@ -1359,15 +1387,18 @@
         Remove all annotation assignments.
 
         But also keep track of any explicit `TypeAlias` assignments, we should treat the RHS like
         an annotation as well, but we have to keep in mind that the RHS will not automatically become
         a ForwardRef with a future import, like a true annotation would.
         """
         super().visit_AnnAssign(node)
-        self.add_annotation(node.annotation, self.current_scope)
+
+        self.add_annotation(
+            node.annotation, self.current_scope, never_evaluates=self.current_scope.ann_assign_never_evaluates
+        )
 
         if node.value is None:
             return
 
         if isinstance(node.target, ast.Name):
             self.current_scope.symbols[node.target.id].append(
                 Symbol(
@@ -1835,17 +1866,19 @@
             Classified.THIRD_PARTY: (self.visitor.third_party_imports, TC002),
             Classified.BUILTIN: (self.visitor.built_in_imports, TC003),
         }
 
         unused_imports = set(self.visitor.imports) - self.visitor.names - self.visitor.mapped_names
         used_imports = set(self.visitor.imports) - unused_imports
         already_imported_modules = [self.visitor.imports[name].module for name in used_imports]
-        annotation_names = [n for i in self.visitor.wrapped_annotations for n in i.names] + [
-            i.annotation for i in self.visitor.unwrapped_annotations
-        ]
+        annotation_names = (
+            [n for i in self.visitor.wrapped_annotations for n in i.names]
+            + [i.annotation for i in self.visitor.unwrapped_annotations]
+            + [n for i in self.visitor.excess_wrapped_annotations for n in i.names]
+        )
 
         for name in unused_imports:
             if name not in annotation_names:
                 # The import seems to be completely unused.
                 # Prevent flagging these, as they're already covered by F401
                 continue
 
@@ -2042,14 +2075,20 @@
                 error = TC201.format(annotation=item.annotation)
 
                 if not self.visitor.futures_annotation:
                     yield item.lineno, item.col_offset, TC101.format(annotation=item.annotation), None
 
             yield item.lineno, item.col_offset, error, None
 
+        for item in self.visitor.excess_wrapped_annotations:
+            assert item.type == 'annotation'
+            # This always generates an error in either case
+            yield item.lineno, item.col_offset, TC101.format(annotation=item.annotation), None
+            yield item.lineno, item.col_offset, TC201.format(annotation=item.annotation), None
+
     @property
     def errors(self) -> Flake8Generator:
         """
         Return relevant errors in the required flake8-defined format.
 
         Flake8 plugins must return generators in this format: https://flake8.pycqa.org/en/latest/plugin-development/
         """
```

### Comparing `flake8_type_checking-2.9.0/flake8_type_checking/constants.py` & `flake8_type_checking-2.9.1/flake8_type_checking/constants.py`

 * *Files identical despite different names*

### Comparing `flake8_type_checking-2.9.0/flake8_type_checking/plugin.py` & `flake8_type_checking-2.9.1/flake8_type_checking/plugin.py`

 * *Files identical despite different names*

### Comparing `flake8_type_checking-2.9.0/flake8_type_checking/types.py` & `flake8_type_checking-2.9.1/flake8_type_checking/types.py`

 * *Files identical despite different names*

### Comparing `flake8_type_checking-2.9.0/pyproject.toml` & `flake8_type_checking-2.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = 'flake8-type-checking'
-version = "2.9.0"
+version = "2.9.1"
 description = 'A flake8 plugin for managing type-checking imports & forward references'
 homepage = 'https://github.com/snok'
 repository = 'https://github.com/snok/flake8-type-checking'
 authors = ['Sondre Lillebø Gundersen <sondrelg@live.no>']
 license = 'BSD-3-Clause'
 readme = 'README.md'
 keywords = ['flake8', 'plugin', 'linting', 'type hint', 'typing', 'imports']
```

### Comparing `flake8_type_checking-2.9.0/PKG-INFO` & `flake8_type_checking-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-type-checking
-Version: 2.9.0
+Version: 2.9.1
 Summary: A flake8 plugin for managing type-checking imports & forward references
 Home-page: https://github.com/snok
 License: BSD-3-Clause
 Keywords: flake8,plugin,linting,type hint,typing,imports
 Author: Sondre Lillebø Gundersen
 Author-email: sondrelg@live.no
 Requires-Python: >=3.8
```

