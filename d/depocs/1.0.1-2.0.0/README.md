# Comparing `tmp/depocs-1.0.1.tar.gz` & `tmp/depocs-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/depocs-1.0.1.tar", last modified: Thu Jan 31 20:55:54 2019, max compression
+gzip compressed data, was "depocs-2.0.0.tar", max compression
```

## Comparing `depocs-1.0.1.tar` & `depocs-2.0.0.tar`

### file list

```diff
@@ -1,14 +1,5 @@
-drwxr-xr-x   0 kchan      (501) staff       (20)        0 2019-01-31 20:55:54.000000 depocs-1.0.1/
--rw-r--r--   0 kchan      (501) staff       (20)     6620 2019-01-31 20:55:54.000000 depocs-1.0.1/PKG-INFO
-drwxr-xr-x   0 kchan      (501) staff       (20)        0 2019-01-31 20:55:54.000000 depocs-1.0.1/depocs/
--rw-r--r--   0 kchan      (501) staff       (20)    10495 2019-01-31 20:51:56.000000 depocs-1.0.1/depocs/__init__.py
--rw-r--r--   0 kchan      (501) staff       (20)       24 2019-01-31 17:02:00.000000 depocs-1.0.1/MANIFEST.in
--rw-r--r--   0 kchan      (501) staff       (20)     2243 2019-01-31 20:51:56.000000 depocs-1.0.1/setup.py
--rw-r--r--   0 kchan      (501) staff       (20)       67 2019-01-31 20:55:54.000000 depocs-1.0.1/setup.cfg
--rw-r--r--   0 kchan      (501) staff       (20)     4563 2019-01-31 17:02:00.000000 depocs-1.0.1/README.rst
-drwxr-xr-x   0 kchan      (501) staff       (20)        0 2019-01-31 20:55:54.000000 depocs-1.0.1/depocs.egg-info/
--rw-r--r--   0 kchan      (501) staff       (20)     6620 2019-01-31 20:55:54.000000 depocs-1.0.1/depocs.egg-info/PKG-INFO
--rw-r--r--   0 kchan      (501) staff       (20)      209 2019-01-31 20:55:54.000000 depocs-1.0.1/depocs.egg-info/SOURCES.txt
--rw-r--r--   0 kchan      (501) staff       (20)       12 2019-01-31 20:55:54.000000 depocs-1.0.1/depocs.egg-info/requires.txt
--rw-r--r--   0 kchan      (501) staff       (20)        7 2019-01-31 20:55:54.000000 depocs-1.0.1/depocs.egg-info/top_level.txt
--rw-r--r--   0 kchan      (501) staff       (20)        1 2019-01-31 20:55:54.000000 depocs-1.0.1/depocs.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0     4563 2024-05-27 22:45:01.489681 depocs-2.0.0/README.rst
+-rw-r--r--   0        0        0    11845 2024-05-27 22:45:01.489681 depocs-2.0.0/depocs/__init__.py
+-rw-r--r--   0        0        0     1391 2024-05-27 22:45:01.489681 depocs-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     8449 2024-05-27 22:45:01.489681 depocs-2.0.0/tests/__init__.py
+-rw-r--r--   0        0        0     5201 1970-01-01 00:00:00.000000 depocs-2.0.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `depocs-1.0.1/PKG-INFO` & `depocs-2.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,169 +1,165 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: depocs
-Version: 1.0.1
+Version: 2.0.0
 Summary: Scoped thread-local mixin class
 Home-page: https://github.com/sdelements/depocs
-Author: Security Compass
-Author-email: jed@securitycompass.com
 License: MIT
-Description: Scoped Objects
-        ==============
-        
-        ``Scoped`` is a mixin class that creates a thread-local stack for each of its
-        subclasses. Instances of the subclass can be pushed and popped on this stack,
-        and the instance at the top of the stack is always available as a property of
-        the class. ``Scoped`` classes are typically used to make parameters implicitly
-        available within a (dynamic) scope, without having to pass them around as
-        function arguments. ``Scoped`` helps you do this in a safe and convenient way,
-        and provides very informative error messages when you do something wrong.
-        
-        
-        Examples
-        --------
-        
-        A ``Scoped`` class can be used to pass around contextual data:
-        
-        .. code-block:: python
-        
-            class Session(Scoped):
-                def __init__(self, user):
-                    self.user = user
-        
-            def print_current_user():
-                print(Session.current.user)
-        
-            with Session(some_guy):
-                print_current_user()
-        
-        
-        It can also be used to provide dependencies:
-        
-        .. code-block:: python
-        
-            class Clock(Scoped):
-                def __init__(self, now=None):
-                    self._now = now
-        
-                def now(self):
-                    return self._now or datetime.now()
-        
-            Clock.default = Clock()
-        
-            def print_time()
-                print(Clock.current.now())
-        
-            print_time() # Prints the real time
-        
-            def test_print_fake_time(self):
-                with Clock(datetime(2000, 1, 1)):
-                    print_time() # Prints a fake time
-        
-        
-        Opening and Closing
-        -------------------
-        
-        ``Scoped`` objects are best used as context managers (i.e. using the ``with``
-        statement), but for situations where this isn't possible, you can also open
-        and close them "manually":
-        
-        .. code-block:: python
-        
-            class Transaction(Scoped):
-                ...
-        
-            transaction = Transaction().open()
-            try:
-                ...
-            finally:
-                transaction.close()
-        
-        Obviously, you will need to do whatever is necessary to ensure that every
-        call to ``open`` is matched by a call to ``close``.
-        
-        
-        Options
-        -------
-        
-        The behavior of ``Scoped`` subclasses can be customized by declaring
-        options in a nested class named ``ScopedOptions``. Except where noted,
-        options are automatically inherited by subclasses that do not override
-        them:
-        
-        .. code-block:: python
-        
-            class Thingy(Scoped):
-                class ScopedOptions:
-        
-                    # If True, instances will share the stack of their parent class.
-                    # If False, this class will have its own stack independent of any
-                    # ancestors. The default is to inherit the stack, unless subclassing
-                    # Scoped directly. This option is NOT inherited by subclasses.
-                    inherit_stack = False
-        
-                    # Maximum number of scopes that can be nested on this stack.
-                    # This cannot be overridden if inheriting the parent stack.
-                    max_nesting = 16
-        
-                    # If True, instances can be re-opened after being closed.
-                    # If False, instances can only be opened and closed once, and will
-                    # raise a LifecycleError on any attempt to reopen them.
-                    allow_reuse = False
-        
-        
-        Default Instance
-        ----------------
-        
-        An instance of a Scoped subclass can be assigned to the ``default`` property
-        of the class. This instance will be the value of the ``current`` property
-        when the stack is empty i.e. when no other instances are open. The default
-        instance itself is not opened by virtue of being the default. Opening it
-        will push it onto the stack like any other instance.
-        
-        
-        Errors
-        ------
-        
-        ``Scoped`` has three inner exception classes that it will raise for various
-        error conditions: ``Scoped.Error`` is the base class for the other two, which
-        are ``Scoped.Missing`` and ``Scoped.Lifecycle``.
-        
-        ``Scoped.Missing`` is raised when an attempt is made to access a scoped object
-        that is not available, i.e. when accessing ``Scoped.current`` with an empty
-        stack and no default instance.
-        
-        ``Scoped.Lifecycle`` is raised on any attempt to open or close a scoped object
-        at the wrong time e.g. opening an object that is already open, closing an object
-        that is not at the top of the stack, and various other cases.
-        
-        Both of these exceptions are automatically subclassed along with their containing
-        class. Each subclass of ``Scoped`` gets its own exception classes that inherit
-        from the base exceptions. This allows you to easily handle errors from particular
-        scoped classes without worrying about catching unrelated errors from other scoped
-        classes.
-        
-        Docs
-        ----
-        
-        `The complete documentation for depocs can be found on readthedocs.org <http://depocs.readthedocs.org/en/latest/>`_
-        
-        FAQ
-        ---
-        
-        Q: What does the name "depocs" mean?
-        
-        A: It's "scoped" spelled backwards. :smile:
-        
-Keywords: development thread-local
-Platform: UNKNOWN
+Author: Security Compass
+Author-email: contact@securitycompass.com
+Requires-Python: >=3.12,<3.13
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
+Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.2
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/x-rst
+
+Scoped Objects
+==============
+
+``Scoped`` is a mixin class that creates a thread-local stack for each of its
+subclasses. Instances of the subclass can be pushed and popped on this stack,
+and the instance at the top of the stack is always available as a property of
+the class. ``Scoped`` classes are typically used to make parameters implicitly
+available within a (dynamic) scope, without having to pass them around as
+function arguments. ``Scoped`` helps you do this in a safe and convenient way,
+and provides very informative error messages when you do something wrong.
+
+
+Examples
+--------
+
+A ``Scoped`` class can be used to pass around contextual data:
+
+.. code-block:: python
+
+    class Session(Scoped):
+        def __init__(self, user):
+            self.user = user
+
+    def print_current_user():
+        print(Session.current.user)
+
+    with Session(some_guy):
+        print_current_user()
+
+
+It can also be used to provide dependencies:
+
+.. code-block:: python
+
+    class Clock(Scoped):
+        def __init__(self, now=None):
+            self._now = now
+
+        def now(self):
+            return self._now or datetime.now()
+
+    Clock.default = Clock()
+
+    def print_time()
+        print(Clock.current.now())
+
+    print_time() # Prints the real time
+
+    def test_print_fake_time(self):
+        with Clock(datetime(2000, 1, 1)):
+            print_time() # Prints a fake time
+
+
+Opening and Closing
+-------------------
+
+``Scoped`` objects are best used as context managers (i.e. using the ``with``
+statement), but for situations where this isn't possible, you can also open
+and close them "manually":
+
+.. code-block:: python
+
+    class Transaction(Scoped):
+        ...
+
+    transaction = Transaction().open()
+    try:
+        ...
+    finally:
+        transaction.close()
+
+Obviously, you will need to do whatever is necessary to ensure that every
+call to ``open`` is matched by a call to ``close``.
+
+
+Options
+-------
+
+The behavior of ``Scoped`` subclasses can be customized by declaring
+options in a nested class named ``ScopedOptions``. Except where noted,
+options are automatically inherited by subclasses that do not override
+them:
+
+.. code-block:: python
+
+    class Thingy(Scoped):
+        class ScopedOptions:
+
+            # If True, instances will share the stack of their parent class.
+            # If False, this class will have its own stack independent of any
+            # ancestors. The default is to inherit the stack, unless subclassing
+            # Scoped directly. This option is NOT inherited by subclasses.
+            inherit_stack = False
+
+            # Maximum number of scopes that can be nested on this stack.
+            # This cannot be overridden if inheriting the parent stack.
+            max_nesting = 16
+
+            # If True, instances can be re-opened after being closed.
+            # If False, instances can only be opened and closed once, and will
+            # raise a LifecycleError on any attempt to reopen them.
+            allow_reuse = False
+
+
+Default Instance
+----------------
+
+An instance of a Scoped subclass can be assigned to the ``default`` property
+of the class. This instance will be the value of the ``current`` property
+when the stack is empty i.e. when no other instances are open. The default
+instance itself is not opened by virtue of being the default. Opening it
+will push it onto the stack like any other instance.
+
+
+Errors
+------
+
+``Scoped`` has three inner exception classes that it will raise for various
+error conditions: ``Scoped.Error`` is the base class for the other two, which
+are ``Scoped.Missing`` and ``Scoped.Lifecycle``.
+
+``Scoped.Missing`` is raised when an attempt is made to access a scoped object
+that is not available, i.e. when accessing ``Scoped.current`` with an empty
+stack and no default instance.
+
+``Scoped.Lifecycle`` is raised on any attempt to open or close a scoped object
+at the wrong time e.g. opening an object that is already open, closing an object
+that is not at the top of the stack, and various other cases.
+
+Both of these exceptions are automatically subclassed along with their containing
+class. Each subclass of ``Scoped`` gets its own exception classes that inherit
+from the base exceptions. This allows you to easily handle errors from particular
+scoped classes without worrying about catching unrelated errors from other scoped
+classes.
+
+Docs
+----
+
+`The complete documentation for depocs can be found on readthedocs.org <http://depocs.readthedocs.org/en/latest/>`_
+
+FAQ
+---
+
+Q: What does the name "depocs" mean?
+
+A: It's "scoped" spelled backwards. :smile:
+
```

### Comparing `depocs-1.0.1/depocs/__init__.py` & `depocs-2.0.0/depocs/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,69 +5,105 @@
 the class.
 
 Scoped classes are typically used to make parameters implicitly
 available within a (dynamic) scope, without having to pass them around as
 function arguments. Scoped helps you do this in a safe and convenient way, and
 provides very informative error messages when you do something wrong.
 """
-from six import with_metaclass
 
 import inspect
 import threading
 
 
+# Copied from six
+def with_metaclass(meta, *bases):
+    """Create a base class with a metaclass."""
+
+    # This requires a bit of explanation: the basic idea is to make a dummy
+    # metaclass for one level of class instantiation that replaces itself with
+    # the actual metaclass.
+    class metaclass(type):
+
+        def __new__(cls, name, this_bases, d):
+            return meta(name, bases, d)
+
+        @classmethod
+        def __prepare__(cls, name, this_bases):
+            return meta.__prepare__(name, bases)
+
+    return type.__new__(metaclass, "temporary_class", (), {})
+
+
 class classproperty(property):
     """
     Marries ``@property`` and ``@classmethod``. Why doesn't python have this?
     Grr..
     """
+
     def __new__(cls, fget, *args):
         return super(classproperty, cls).__new__(cls, classmethod(fget), *args)
 
     def __get__(self, obj, type=None):
         return self.fget(type)
 
 
 class ScopedClass(type):
     def __init__(cls, clsname, bases=None, attrs=None):
         super(ScopedClass, cls).__init__(clsname, bases, attrs)
 
-        if not hasattr(cls, '_Scoped__thread_local'):
+        if not hasattr(cls, "_Scoped__thread_local"):
             # ScopedBase
             return
-        elif '_Scoped__thread_local' in attrs:
+        elif "_Scoped__thread_local" in attrs:
             # Scoped
             return
         else:
             # subclass of Scoped
-            scoped_bases = tuple(base for base in bases if isinstance(base, ScopedClass))
-            immediate_subclass = len(scoped_bases) == 0 or scoped_bases[0]._Scoped__thread_local is None
-
-            if 'ScopedOptions' in attrs:
-                meta = dict((name, getattr(attrs['ScopedOptions'], name))
-                            for name in dir(attrs['ScopedOptions']) if name[:2] != '__')
+            scoped_bases = tuple(
+                base for base in bases if isinstance(base, ScopedClass)
+            )
+            immediate_subclass = (
+                len(scoped_bases) == 0 or scoped_bases[0]._Scoped__thread_local is None
+            )
+
+            if "ScopedOptions" in attrs:
+                meta = dict(
+                    (name, getattr(attrs["ScopedOptions"], name))
+                    for name in dir(attrs["ScopedOptions"])
+                    if name[:2] != "__"
+                )
             else:
                 meta = {}
 
-            if 'inherit_stack' not in meta:
-                meta['inherit_stack'] = not immediate_subclass
+            if "inherit_stack" not in meta:
+                meta["inherit_stack"] = not immediate_subclass
 
-            if meta['inherit_stack'] and immediate_subclass:
+            if meta["inherit_stack"] and immediate_subclass:
                 raise TypeError("Base class does not have a stack to inherit")
 
-            if not meta['inherit_stack']:
+            if not meta["inherit_stack"]:
                 cls._Scoped__thread_local = threading.local()
 
-            if 'max_nesting' in meta and meta['inherit_stack']:
+            if "max_nesting" in meta and meta["inherit_stack"]:
                 raise TypeError("Can't override max_nesting if inheriting the stack")
 
             if scoped_bases:
-                cls.ScopedOptions = type('ScopedOptions', tuple(base.ScopedOptions for base in scoped_bases), meta)
-                cls.Missing = type('Missing', tuple(base.Missing for base in scoped_bases), {})
-                cls.LifecycleError = type('LifecycleError', tuple(base.LifecycleError for base in scoped_bases), {})
+                cls.ScopedOptions = type(
+                    "ScopedOptions",
+                    tuple(base.ScopedOptions for base in scoped_bases),
+                    meta,
+                )
+                cls.Missing = type(
+                    "Missing", tuple(base.Missing for base in scoped_bases), {}
+                )
+                cls.LifecycleError = type(
+                    "LifecycleError",
+                    tuple(base.LifecycleError for base in scoped_bases),
+                    {},
+                )
 
 
 class Scoped(ScopedClass("ScopedBase", (object,), {})):
     """
     Abstract base class for an object representing a scope that can be entered and left
     by explicitly opening and closing the object. Instances can only be accessed from
     the thread they were opened in. Scopes can optionally be nested, and the inner-most
@@ -118,15 +154,15 @@
         pass
 
     class Missing(Error):
         """
         A current scope is expected and there isn't one
         """
 
-    class LifecycleError(with_metaclass(ScopedClass, Error)):
+    class LifecycleError(with_metaclass(ScopedClass, Exception)):
         """
         A scope was opened/closed at the wrong time
         """
 
     class ScopedOptions(object):
         """
         Subclasses can use an inner class named 'ScopedOptions' to set some
@@ -169,27 +205,38 @@
 
         ``call_site_level`` is the number of stack frames to skip when
         determining where the scope was opened from.  The default value of 1
         will record the site of the actual call to this method.
         """
         if self.is_open:
             if self.open_site:
-                raise self.LifecycleError("{0}({1}) is already open\n{2}".format(
-                    self.__class__.__name__, id(self), self.format_trace("  ")))
+                raise self.LifecycleError(
+                    "{0}({1}) is already open\n{2}".format(
+                        self.__class__.__name__, id(self), self.format_trace("  ")
+                    )
+                )
 
         if not self.ScopedOptions.allow_reuse and self.is_used:
-            raise self.LifecycleError("{0}({1}) cannot be reused\n{2}".format(
-                self.__class__.__name__, id(self), self.format_trace("  ")))
+            raise self.LifecycleError(
+                "{0}({1}) cannot be reused\n{2}".format(
+                    self.__class__.__name__, id(self), self.format_trace("  ")
+                )
+            )
 
-        if not hasattr(self._Scoped__thread_local, 'stack'):
+        if not hasattr(self._Scoped__thread_local, "stack"):
             self._Scoped__thread_local.stack = []
 
         if len(self._Scoped__thread_local.stack) >= self.ScopedOptions.max_nesting:
-            raise self.LifecycleError("Cannot nest {0} more than {1} levels\n{2}".format(
-                self.__class__.__name__, self.ScopedOptions.max_nesting, self.format_trace("  ")))
+            raise self.LifecycleError(
+                "Cannot nest {0} more than {1} levels\n{2}".format(
+                    self.__class__.__name__,
+                    self.ScopedOptions.max_nesting,
+                    self.format_trace("  "),
+                )
+            )
 
         self._Scoped__thread_local.stack.append(self)
         self._Scoped__is_open = True
         self._Scoped__is_used = True
 
         stack = inspect.stack()
         if len(stack) > call_site_level:
@@ -200,23 +247,32 @@
     def close(self):
         """
         Closes the current scoped context, removing it from the stack of
         contexts.
         """
         if not self.is_open:
             if not self.ScopedOptions.allow_reuse and self.is_used:
-                raise self.LifecycleError("This {0} has already been closed\n{1}".format(
-                    self.__class__.__name__, self.format_trace("  ")))
+                raise self.LifecycleError(
+                    "This {0} has already been closed\n{1}".format(
+                        self.__class__.__name__, self.format_trace("  ")
+                    )
+                )
             else:
-                raise self.LifecycleError("This {0} is not open\n{1}".format(
-                    self.__class__.__name__, self.format_trace("  ")))
+                raise self.LifecycleError(
+                    "This {0} is not open\n{1}".format(
+                        self.__class__.__name__, self.format_trace("  ")
+                    )
+                )
 
         if not self.is_current:
-            raise self.LifecycleError("This {0} is not at the top of the stack\n{1}".format(
-                self.__class__.__name__, self.format_trace("  ")))
+            raise self.LifecycleError(
+                "This {0} is not at the top of the stack\n{1}".format(
+                    self.__class__.__name__, self.format_trace("  ")
+                )
+            )
 
         self._Scoped__thread_local.stack.pop()
         self._Scoped__is_open = False
 
         return self
 
     def __enter__(self):
@@ -251,15 +307,18 @@
 
     @classproperty
     def default(cls):
         return None
 
     @classproperty
     def has_topmost(cls):
-        return hasattr(cls._Scoped__thread_local, 'stack') and len(cls._Scoped__thread_local.stack) > 0
+        return (
+            hasattr(cls._Scoped__thread_local, "stack")
+            and len(cls._Scoped__thread_local.stack) > 0
+        )
 
     @classproperty
     def topmost(cls):
         if not cls.has_topmost:
             raise cls.Missing("No {0} on the stack".format(cls.__name__))
         return cls._Scoped__thread_local.stack[-1]
 
@@ -287,21 +346,25 @@
             del cls._Scoped__thread_local.stack
         except AttributeError:
             pass
 
     def format_trace_entry(self):
         if self.open_site:
             return "{0}({1}) opened at {2}:{3}\n".format(
-                self.__class__.__name__,
-                id(self),
-                self.open_site[1],
-                self.open_site[2])
+                self.__class__.__name__, id(self), self.open_site[1], self.open_site[2]
+            )
         else:
             return "{0}({1}) opened somewhere\n".format(
-                self.__class__.__name__, id(self))
+                self.__class__.__name__, id(self)
+            )
 
     @classmethod
     def format_trace(cls, prefix=""):
-        if hasattr(cls._Scoped__thread_local, 'stack'):
-            return "".join([prefix + so.format_trace_entry() for so in cls._Scoped__thread_local.stack])
+        if hasattr(cls._Scoped__thread_local, "stack"):
+            return "".join(
+                [
+                    prefix + so.format_trace_entry()
+                    for so in cls._Scoped__thread_local.stack
+                ]
+            )
         else:
             return ""
```

### Comparing `depocs-1.0.1/README.rst` & `depocs-2.0.0/README.rst`

 * *Files identical despite different names*

