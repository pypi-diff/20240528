# Comparing `tmp/pyoload-1.0.2.tar.gz` & `tmp/pyoload-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyoload-1.0.2.tar", last modified: Wed May 22 16:20:16 2024, max compression
+gzip compressed data, was "pyoload-1.1.0.tar", last modified: Tue May 28 14:42:39 2024, max compression
```

## Comparing `pyoload-1.0.2.tar` & `pyoload-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:20:16.066493 pyoload-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-22 16:20:13.000000 pyoload-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-05-22 16:20:16.066493 pyoload-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-05-22 16:20:13.000000 pyoload-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:20:16.062493 pyoload-1.0.2/pyoload/
--rw-r--r--   0 runner    (1001) docker     (127)    10243 2024-05-22 16:20:11.000000 pyoload-1.0.2/pyoload/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:20:16.066493 pyoload-1.0.2/pyoload.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-05-22 16:20:16.000000 pyoload-1.0.2/pyoload.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-22 16:20:16.000000 pyoload-1.0.2/pyoload.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 16:20:16.000000 pyoload-1.0.2/pyoload.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-22 16:20:16.000000 pyoload-1.0.2/pyoload.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-22 16:20:16.000000 pyoload-1.0.2/pyoload.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 16:20:16.066493 pyoload-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-05-22 16:20:11.000000 pyoload-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:20:16.066493 pyoload-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-22 16:20:11.000000 pyoload-1.0.2/tests/test_placeholder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:42:39.721882 pyoload-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-28 14:42:37.000000 pyoload-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8623 2024-05-28 14:42:39.721882 pyoload-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7096 2024-05-28 14:42:37.000000 pyoload-1.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:42:39.717882 pyoload-1.1.0/pyoload/
+-rw-r--r--   0 runner    (1001) docker     (127)    13001 2024-05-28 14:42:32.000000 pyoload-1.1.0/pyoload/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:42:39.721882 pyoload-1.1.0/pyoload.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8623 2024-05-28 14:42:39.000000 pyoload-1.1.0/pyoload.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-28 14:42:39.000000 pyoload-1.1.0/pyoload.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 14:42:39.000000 pyoload-1.1.0/pyoload.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-28 14:42:39.000000 pyoload-1.1.0/pyoload.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-28 14:42:39.000000 pyoload-1.1.0/pyoload.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 14:42:39.721882 pyoload-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-05-28 14:42:32.000000 pyoload-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:42:39.721882 pyoload-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-28 14:42:32.000000 pyoload-1.1.0/tests/test_placeholder.py
```

### Comparing `pyoload-1.0.2/LICENSE` & `pyoload-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyoload-1.0.2/pyoload/__init__.py` & `pyoload-1.1.0/pyoload/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, GenericAlias, Union
+from typing import Any, GenericAlias
 from types import UnionType
 from functools import wraps, partial
 from inspect import isclass
 
 import sys
 
 
@@ -45,46 +45,130 @@
 Vs = Values
 
 
 def get_name(funcOrCls):
     return funcOrCls.__module__ + '.' + funcOrCls.__qualname__
 
 
-g_n = get_name
+class Check:
+    checks_list = {}
 
+    def __init_subclass__(cls, subclass):
+        cls.register(cls.name, cls.__call__)
 
-class Validator:
-    def __init__(self, func):
-        if not callable(func):
-            raise TypeError(self.__class__.__init__.__qualname__)
-        self.func = func
+    @classmethod
+    def register(cls, name):
+        if name in cls.checks_list:
+            raise Check.CheckNameAlreadyExistsError(name)
+
+        def inner(func):
+            cls.checks_list[name] = func
+        return inner
+
+    @classmethod
+    def check(cls, name, params, val):
+        print(cls, name, params, val)
+        check = cls.checks_list.get(name)
+        if check is None:
+            raise Check.CheckDoesNotExistError(name)
+        check(params, val)
+
+    class CheckNameAlreadyExistsError(ValueError):
+        pass
+
+    class CheckDoesNotExistError(ValueError):
+        pass
+
+    class CheckError(Exception):
+        pass
+
+
+@Check.register('len')
+def len_check(params, val):
+    print(params, val)
+    if isinstance(params, int):
+        if not len(val) == params:
+            raise Check.CheckError(f'length of {val!r} not eq {params!r}')
+    elif isinstance(params, tuple) and len(params) > 0:
+        mi = ma = None
+        mi, ma = params
+        if mi is not None:
+            if not len(val) > mi:
+                raise Check.CheckError(f'length of {val!r} not gt {mi!r}')
+        if ma is not None:
+            if not len(val) < ma:
+                raise Check.CheckError(f'length of {val!r} not lt {mi!r}')
+
+
+@Check.register('lt')
+def lt_check(param, val):
+    if not val < param:
+        raise Check.CheckError()
+
+
+@Check.register('le')
+def le_check(param, val):
+    if not val <= param:
+        raise Check.CheckError()
+
+
+@Check.register('ge')
+def ge_check(param, val):
+    if not val >= param:
+        raise Check.CheckError()
+
+
+@Check.register('gt')
+def gt_check(param, val):
+    if not val > param:
+        raise Check.CheckError()
+
+
+@Check.register('func')
+def func_check(param, val):
+    if not param(val):
+        raise Check.CheckError()
+
+
+@Check.register('match_')
+def matches_check(param, val):
+    if not typeMatch(val, param):
+        raise Check.CheckError()
+
+
+class Checks:
+    def __init__(self, **checks):
+        self.checks = checks
+        print(f'{checks=}')
 
     def __call__(self, val):
-        try:
-            return self.func()
-        except Exception as e:
-            raise AnnotationError(
-                f'{type(e)} while using validator method: {get_name(self.func)}' +
-                f'\n{e!s}',
-            ) from e
+        print(self.checks, val)
+        for name, params in self.checks.items():
+            Check.check(name, params, val)
 
+    def __str__(self):
+        ret = '<Checks('
+        for k, v in self.checks.items():
+            ret += f'{k}={v!r}, '
+        ret = ret[:-2] + ')>'
+        return ret
 
-Vf = Validator
+    __repr__ = __str__
 
 
 class Cast:
     @staticmethod
     def cast(val, totype):
         if isinstance(totype, GenericAlias):
             if totype.__origin__ == dict:
                 if len(totype.__args__) == 2:
                     kt, vt = totype.__args__
                 elif len(totype.__args__) == 1:
                     kt, vt = Any, totype.__args__[1]
-                print(f"{totype=} {kt=} {vt=}")
+                print(f'{totype=} {kt=} {vt=}')
                 return {
                     Cast.cast(k, kt): Cast.cast(v, vt) for k, v in val.items()
                 }
             else:
                 sub = totype.__args__[0]
                 return totype.__origin__([
                     Cast.cast(v, sub) for v in val
@@ -93,54 +177,60 @@
             errors = []
             for subtype in totype.__args__:
                 try:
                     return Cast.cast(val, subtype)
                 except Exception as e:
                     errors.append(e)
             else:
-                raise e
+                raise errors
         else:
             return totype(val) if not isinstance(val, totype) else val
 
     def __init__(self, type):
         """
         creates a casting object for the specified type
         """
         self.type = type
 
-    def __call__(self:'Cast', val: Any):
-        '''
+    def __call__(self: 'Cast', val: Any):
+        """
         Calls to the type specified in the object `.type` attribute
         :param self: The cast onject
         :param val: the value to be casted
 
         :return: The casted value
-        '''
+        """
         try:
             return Cast.cast(val, self.type)
         except Exception as e:
             raise CastingError(
                 f'Exception({e}) while casting: {val!r} to {self.type}',
             ) from e
 
 
-def typeMatch(val: Any, spec:type) -> bool:
-    '''
+def typeMatch(val: Any, spec: type) -> bool:
+    """
     recursively checks if type matches
     :param val: The value to typecheck
     :param spec: The type specifier
 
     :return: A boolean
-    '''
+    """
     if spec == Any or spec is None or val is None:
         return True
     if isinstance(spec, Values):
         return spec(val)
-    elif isinstance(spec, Validator):
-        return spec(val)
+    elif isinstance(spec, Checks):
+        print(val)
+        try:
+            spec(val)
+        except Check.CheckError:
+            return False
+        else:
+            return True
     elif isinstance(spec, GenericAlias):
         if not isinstance(val, spec.__origin__):
             return False
 
         if spec.__origin__ == dict:
             if len(spec.__args__) == 2:
                 kt, vt = spec.__args__
@@ -161,129 +251,144 @@
                     return False
             else:
                 return True
     else:
         return isinstance(val, spec)
 
 
-
 def get_module(obj: Any):
-    '''
+    """
     gets the module to which an object, function or class belongs
     :param obj: the object
     :returns: the module
-    '''
+    """
     return sys.modules[obj.__module__]
 
 
 def resolveAnnotations(obj: Any) -> None:
-    '''
+    """
     Evaluates all the stringized annotations of the argument
 
     :param obj: The object
     :returns: None
-    '''
+    """
     if isclass(obj) or hasattr(obj, '__class__'):
         for k, v in obj.__annotations__.items():
             if isinstance(v, str):
                 try:
-                    obj.__annotations__[k] = eval(v, dict(vars(get_module(obj))), dict(vars(obj)))
+                    obj.__annotations__[k] = eval(
+                        v,
+                        dict(vars(get_module(obj))), dict(vars(obj)),
+                    )
                 except Exception as e:
                     raise AnnotationResolutionError(
-                        f'Exception: {e!s} while resolving'
-                        f' annotation {e}={v!r} of object {obj!r}',
+                        (
+                            f'Exception: {e!s} while resolving'
+                            f' annotation {e}={v!r} of object {obj!r}'
+                        ),
                     ) from e
     elif callable(obj):
         for k, v in obj.__annotations__.items():
             if isinstance(v, str):
                 try:
                     obj.__annotations__[k] = eval(v, obj.__globals__)
                 except Exception as e:
                     raise AnnotationResolutionError(
                         f'Exception: {k!s} while resolving'
                         f' annotation {v!r} of function {obj!r}',
-                        f'globals: {obj.__globals__}'
+                        f'globals: {obj.__globals__}',
                     ) from e
 
 
-def annotate(func:callable, oload:bool=False) -> callable:
-    '''
+def annotate(func: callable, oload: bool = False) -> callable:
+    """
     returns a wrapper over the passed function
     which typechecks arguments on each call
     :param func: the function to annotate
     :param oload: internal
 
-    :return: the wrapper function
-    '''
+    :returns: the wrapper function
+    """
     if isclass(func):
         return annotateClass(func)
-    anno = func.__annotations__
-    if len(anno) == 0:
+    if len(func.__annotations__) == 0:
+        raise Warning(f'function {get_name(func)} is not annotated')
         return func
 
     @wraps(func)
     def wrapper(*args, **kw):
-        names = tuple(anno.keys())
-        if any(isinstance(x, str) for x in anno.values()):
+        i = 0
+        while str in map(type, func.__annotations__.values()) and i < 10:
             resolveAnnotations(func)
+            i += 1
+        else:
+            if i == 10:
+                raise AnnotationResolutionError(func.__annotations__)
+        anno = func.__annotations__.copy()
+        if 'return' in anno:
+            anno.pop('return')
+        names = list(anno.keys())
         vals = {}
         try:
             if func.__defaults__:
                 for i, v in enumerate(reversed(func.__defaults__)):
                     vals[names[-1 - i]] = v
             for i, v in enumerate(args):
                 vals[names[i]] = v
             vals.update(kw)
         except IndexError as e:
             raise AnnotationError(
-                f'Was function {get_name(func)} properly annotated?',
+                f'Was function {get_name(func)} properly annotated?, has'
+                f' {len(anno)} annotations but {len(args)} arguments passed',
             ) from e
 
         errors = []
         for k, v in vals.items():
             if isinstance(anno[k], Cast):
                 vals[k] = anno[k](v)
                 continue
             if not typeMatch(v, anno[k]):
                 if oload:
                     raise InternalAnnotationError()
                 errors.append(
                     AnnotationError(
-                        f'Value: {v!r} does not match annotation: {anno[k]!r}' +
+                        f'Value: {v!r} does not match annotation: {anno[k]!r}'
                         f' for argument {k!r} of function {get_name(func)}',
                     ),
                 )
         if len(errors) > 0:
             raise AnnotationErrors(errors)
 
         ret = func(**vals)
-        if 'return' in anno:
-            if not typeMatch(ret, anno['return']):
+        if 'return' in func.__annotations__:
+            ann = func.__annotations__['return']
+            if not typeMatch(ret, ann):
                 raise AnnotationError(
-                    f"return value {ret!r} does not match annotation: {anno['return']} of function {get_name(func)}",
+                    f'return value {ret!r} does not match annotation: '
+                    f'{ann} of function {get_name(func)}',
                 )
         return ret
     wrapper.__pyod_annotate__ = func
     return wrapper
 
 
 __overloads__ = {}
 
 
-def overload(func:callable, name:str|None=None):
-    '''
+def overload(func: callable, name: str | None = None):
+    """
     returns a wrapper over the passed function
     which typechecks arguments on each call
     and finds the function instance with same name which does not raise
     an `InternalAnnotationError` exception
     :param func: the function to annotate
     :param oload: internal
 
     :return: the wrapper function
-    '''
+    """
     if isinstance(func, str):
         return partial(overload, name=func)
     if name is None or not isinstance(name, str):
         name = get_name(func)
     if name not in __overloads__:
         __overloads__[name] = []
     __overloads__[name].append(annotate(func, True))
@@ -295,30 +400,31 @@
                 val = f(*args, **kw)
             except InternalAnnotationError:
                 continue
             else:
                 break
         else:
             raise OverloadError(
-                f'No overload of function: {get_name(func)} matches types of arguments',
+                f'No overload of function: {get_name(func)}'
+                ' matches types of arguments',
             )
         return val
 
     wrapper.__pyo_overloads__ = __overloads__[name]
     wrapper.__pyo_overloads_name__ = name
 
     return wrapper
 
 
 def annotateClass(cls):
-    '''
+    """
     Annotates a class object, wrapping and replacing over it's __setattr__
     and typechecking over each attribute assignment.
     If no annotation for the passed object found it sets it to `type(val)`
-    '''
+    """
     if not hasattr(cls, '__annotations__'):
         cls.__annotations__ = {}
     if isinstance(cls, bool):
         return partial(annotate, recur=cls)
     recur = not hasattr(cls, '__annotate_norecur__')
     setter = cls.__setattr__
     if recur:
@@ -340,17 +446,17 @@
             resolveAnnotations(self)
 
         if name not in self.__annotations__:
             if value is not None:
                 self.__annotations__[name] = type(value)
         elif not typeMatch(value, self.__annotations__[name]):
             raise AnnotationError(
-                f'value {value!r} does not match annotation' +
-                f'of attribute: {name!r}:{self.__annotations__[name]!r} of object of class {get_name(cls)}',
+                f'value {value!r} does not match annotation'
+                f'of attribute: {name!r}:{self.__annotations__[name]!r}'
+                f' of object of class {get_name(cls)}',
             )
-        
         return setter(self, name, value)
     cls.__setattr__ = new_setter
     return cls
 
 
-__version__ = '1.0.2'
+__version__ = '1.1.0'
```

### Comparing `pyoload-1.0.2/setup.py` & `pyoload-1.1.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 from pathlib import Path
 
 from setuptools import setup, find_packages
 
 from pyoload import __version__
 
 project_dir = Path(__file__).parent
+
 try:
-    long_description = (project_dir / 'README.md').read_text()
+    long_description = (project_dir / 'README.rst').read_text()
 except FileNotFoundError:
-    long_description = ''
+    try:
+        long_description = Path('README.rst').read_text()
+    except FileNotFoundError:
+        long_description = Path('/src/README.rst').read_text()
 
 deps = ()
 
 extra_flake8 = (
     'flake8',
     'flake8-commas',
     'flake8-quotes',
@@ -39,17 +43,22 @@
     name='pyoload',
     version=__version__,
     packages=find_packages(exclude=['tests', 'tests.*']),
     url='https://github.com/ken-morel/pyoload',
     license='MIT',
     author='ken-morel',
     author_email='engonken8@gmail.com',
-    description='Python package for function argument overload, typechecking and casting',
+    maintainer='ken-morel',
+    maintainer_email='engonken8@gmail.com',
+    description=(
+        'Python package for function argument overload,'
+        ' typechecking and casting'
+    ),
     long_description=long_description,
-    long_description_content_type='text/markdown',
+    long_description_content_type='text/x-rst',
 
     install_requires=deps,
     extras_require={
         'dev': extra_dev,
         'ci': extra_ci,
     },
```

