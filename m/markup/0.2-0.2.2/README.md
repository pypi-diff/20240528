# Comparing `tmp/markup-0.2.tar.gz` & `tmp/markup-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markup-0.2.tar", last modified: Wed Mar  3 15:11:20 2010, max compression, from Unix
+gzip compressed data, was "markup-0.2.2.tar", last modified: Mon May 27 23:56:14 2024, max compression
```

## Comparing `markup-0.2.tar` & `markup-0.2.2.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxr-xr-x   0 jhammel   (1000) jhammel   (1000)        0 2010-03-03 15:11:20.000000 markup-0.2/
-drwxr-xr-x   0 jhammel   (1000) jhammel   (1000)        0 2010-03-03 15:11:20.000000 markup-0.2/markup/
--rw-r--r--   0 jhammel   (1000) jhammel   (1000)       21 2010-03-03 15:09:35.000000 markup-0.2/markup/__init__.py
--rw-r--r--   0 jhammel   (1000) jhammel   (1000)     8289 2010-03-03 15:09:35.000000 markup-0.2/markup/form.py
--rw-r--r--   0 jhammel   (1000) jhammel   (1000)     4865 2010-03-03 15:09:35.000000 markup-0.2/markup/markup.py
-drwxr-xr-x   0 jhammel   (1000) jhammel   (1000)        0 2010-03-03 15:11:20.000000 markup-0.2/markup.egg-info/
--rw-r--r--   0 jhammel   (1000) jhammel   (1000)      251 2010-03-03 15:11:20.000000 markup-0.2/markup.egg-info/PKG-INFO
--rw-r--r--   0 jhammel   (1000) jhammel   (1000)      256 2010-03-03 15:11:20.000000 markup-0.2/markup.egg-info/SOURCES.txt
--rw-r--r--   0 jhammel   (1000) jhammel   (1000)        1 2010-03-03 15:11:20.000000 markup-0.2/markup.egg-info/dependency_links.txt
--rw-r--r--   0 jhammel   (1000) jhammel   (1000)       37 2010-03-03 15:11:20.000000 markup-0.2/markup.egg-info/entry_points.txt
--rw-r--r--   0 jhammel   (1000) jhammel   (1000)        1 2010-03-03 15:10:10.000000 markup-0.2/markup.egg-info/not-zip-safe
--rw-r--r--   0 jhammel   (1000) jhammel   (1000)        7 2010-03-03 15:11:20.000000 markup-0.2/markup.egg-info/top_level.txt
--rw-r--r--   0 jhammel   (1000) jhammel   (1000)      285 2010-03-03 15:09:35.000000 markup-0.2/TODO
--rw-r--r--   0 jhammel   (1000) jhammel   (1000)       59 2010-03-03 15:11:20.000000 markup-0.2/setup.cfg
--rw-r--r--   0 jhammel   (1000) jhammel   (1000)      745 2010-03-03 15:09:35.000000 markup-0.2/setup.py
--rw-r--r--   0 jhammel   (1000) jhammel   (1000)      251 2010-03-03 15:11:20.000000 markup-0.2/PKG-INFO
+drwxrwxr-x   0 jhammel   (1000) jhammel   (1000)        0 2024-05-27 23:56:14.692192 markup-0.2.2/
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      217 2024-05-27 23:56:14.692192 markup-0.2.2/PKG-INFO
+drwxrwxr-x   0 jhammel   (1000) jhammel   (1000)        0 2024-05-27 23:56:14.692192 markup-0.2.2/markup/
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)       22 2024-05-27 23:55:12.000000 markup-0.2.2/markup/__init__.py
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)     8519 2024-05-27 23:55:12.000000 markup-0.2.2/markup/form.py
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)     4978 2024-05-27 23:55:12.000000 markup-0.2.2/markup/markup.py
+drwxrwxr-x   0 jhammel   (1000) jhammel   (1000)        0 2024-05-27 23:56:14.692192 markup-0.2.2/markup.egg-info/
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      217 2024-05-27 23:56:14.000000 markup-0.2.2/markup.egg-info/PKG-INFO
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      251 2024-05-27 23:56:14.000000 markup-0.2.2/markup.egg-info/SOURCES.txt
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)        1 2024-05-27 23:56:14.000000 markup-0.2.2/markup.egg-info/dependency_links.txt
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)       37 2024-05-27 23:56:14.000000 markup-0.2.2/markup.egg-info/entry_points.txt
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)        1 2024-05-27 23:55:16.000000 markup-0.2.2/markup.egg-info/not-zip-safe
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)        7 2024-05-27 23:56:14.000000 markup-0.2.2/markup.egg-info/top_level.txt
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)       59 2024-05-27 23:56:14.692192 markup-0.2.2/setup.cfg
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      663 2024-05-27 23:56:06.000000 markup-0.2.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `markup-0.2/markup/form.py` & `markup-0.2.2/markup/form.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,20 @@
-import markup
-from cStringIO import StringIO
+from . import markup
+
+try:
+    from cStringIO import StringIO
+except ModuleNotFoundError:
+    try:
+        from StringIO import StringIO
+    except ModuleNotFoundError:
+        from io import StringIO
+
+# python3 only
+string = (str,)
+
 
 class Form(object):
     """a simple class for HTML forms"""
 
     type_validators = {} # validators inherit to type
 
     def __init__(self, method='post', action=None, submit='Submit', post_html=''):
@@ -16,47 +27,49 @@
         self.post_html = post_html
         self.elements = []
         self.validators = {} # keys=tuples of names; values=validators
 
     def __call__(self, errors=None):
         """render the form"""
         retval = StringIO()
-        print >> retval
+        retval.write('\n')
 
         def name_field(element):
             if not element['name']:
                 return ''
             title={}
             help = element.get('help')
             if help:
                 title['title'] = help
             return markup.span(markup.strong('%s:' % element['name']), **title)
 
         # print the form as a table
-        table = [ [ name_field(element), element['html'] ]
-                  for element in self.elements ]
+        table = [[name_field(element), element['html']]
+                 for element in self.elements]
         if errors:
             for row, element in zip(table, self.elements):
                 error = errors.get(element['name'], '')
                 if error:
-                    if not isinstance(error, basestring):
+                    if not isinstance(error, string):
                         if len(error) == 1:
                             error = error[0]
                         else:
                             error = markup.listify(error)
                     error = markup.div(error, **{ 'class': 'error' })
                 row.append(error)
-            
-        print >> retval, markup.tablify(table)
-        print >> retval, self.post_html
+
+        retval.write('{}\n'.format(markup.tablify(table)))
+        retval.write('{}\n'.format(self.post_html))
 
         # each form has a submit button
         # XXX this should probably be more customizable
-        print >> retval, markup.input(None, type='submit', name='submit',
-                                      value=self.submit),
+        retval.write('{}\n'.format(markup.input(None,
+                                                type='submit',
+                                                name='submit',
+                                                value=self.submit)))
 
         args = { 'method': self.method,
                  'enctype': 'multipart/form-data'}
         if self.action is not None:
             args['action'] = self.action
         return markup.form(retval.getvalue(), **args)
 
@@ -82,25 +95,25 @@
         for names, validators in self.validators.items():
             args = [ post.get(arg) for arg in names ]
             error = None
 
             for validator in validators:
                 try:
                     validation = validator(*args)
-                except Exception, e: # horrible!
+                except Exception as e:
                     error = str(e)
                 else:
-                    if isinstance(validation, basestring):
+                    if isinstance(validation, string):
                         error = validation # error string
                     elif validation == False:
                         error = "Illegal value for %s" % name
                 if error:
                     for name in names:
                         add_error(name, error)
-                    
+
         return errors
 
     ### functions to add form elements
     # each of these should be decorated to have:
     # * a name/label
     # * a validator (optional)
     # (depending on type, an additional validator may be implied)
@@ -133,15 +146,15 @@
         for item in items:
             kw = { 'name': name, 'value': item, 'type': 'checkbox' }
             if item in checked:
                 kw['checked'] = 'checked'
 
             # XXX hacky;  ideally, one would use a list with no bullets
             retval.append('%s%s<br/>' % (markup.input(None, **kw), item))
-            
+
         return '\n'.join(retval)
 
     def radiobuttons(self, name, items, checked=None, joiner='<br/>'):
         if checked is None:
             checked = items[0]
         joiner = "%s\n" % joiner
         retval = []
@@ -154,18 +167,18 @@
                 kw['checked'] = None
 
             # display contextual help
             if title:
                 title = dict(title=title)
             else:
                 title = {}
-                
+
             retval.append(markup.span('%s%s' % (item, markup.input(**kw)),
                           **title))
-            
+
         return joiner.join(retval)
 
     def add_password_confirmation(self, password='Password',
                                   confirmation='Confirm password',
                                   validators=None):
         """add password and confirm password fields"""
         if validators is None:
@@ -173,60 +186,56 @@
         validators.append(lambda x: bool(x.strip()) or "Please provide a password")
         self.add_element('password', password)
         self.add_element('password', confirmation)
         self.validators[(password,)] = validators
         match = lambda x, y: (x == y) or "Fields don't match"
         self.validators[(password, confirmation)] = [ match ]
 
-    
     def add_element(self, func, name, *args, **kwargs):
 
-        if isinstance(func, basestring):
+        if isinstance(func, string):
             func_name = func
             func = getattr(self, func)
         else:
             func_name = func.func_name
 
         # form validators
         validators = self.type_validators.get(func_name, [])
         validators.extend(kwargs.pop('validators', []))
         self.validators[(name, )] = validators
 
         # don't diplay hidden elements
         if func_name == 'hidden':
-            self.elements.append(dict(name='', 
+            self.elements.append(dict(name='',
                                       html=func(name, *args, **kwargs)))
             return
 
         # allow contextual help
         help = kwargs.pop('help', None)
 
         # allow alternate input names
         # XXX breaks validation?
         input_name = kwargs.pop('input_name', name)
 
-        self.elements.append(dict(name=name, 
+        self.elements.append(dict(name=name,
                                   html=func(input_name, *args, **kwargs),
                                   help=help))
 
     # TODO: add validation
     def add_elements(self, name, funcs, args, kwargs, help=None):
         """add multiple elements to the form
         * name: master name; element names will be derived from this
         * funcs: list of html-returning functions to add
         * args: list of positional args: [ [ args1 ], [ args2], ... ]
         * kwargs: dictionary of kwargs: [ { kwargs1 }, { kwargs2 }, ... ]
         """
         html = StringIO()
-        
+
         for func, index in zip(funcs, range(len(funcs))):
             # no validation (yet)
-            if isinstance(func, basestring):
+            if isinstance(func, string):
                 func = getattr(self, func)
-            print >> html, func('%s-%d' % (name, index), *args[index],
-                                **kwargs[index])
+            html.write('{}\n'.format(func('%s-%d' % (name, index), *args[index],
+                                          **kwargs[index])))
         self.elements.append(dict(name=name,
                                   html=html.getvalue(),
                                   help=help))
-
-
-
```

### Comparing `markup-0.2/markup/markup.py` & `markup-0.2.2/markup/markup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,27 @@
-from cStringIO import StringIO
+try:
+    from cStringIO import StringIO
+except ImportError:
+    try:
+        # python2
+        from StringIO import StringIO
+    except ImportError:
+        # python3
+        from io import StringIO
+
 
 def HTMLmarkup(tag, text=None, **attributes):
     """
     markups the text with the tag and
     attributes
     """
 
     # ideally, this woulod be cached for cascading calls
     s = StringIO()
-    
+
     s.write('<%s' % tag)
     for attribute, value in attributes.items():
         if value is None:
             s.write(' %s' % attribute)
         else:
             s.write(' %s="%s"' % (attribute, value))
 
@@ -105,23 +114,22 @@
     if header is None:
         header = '',
     else:
         header = '%s\n' % lh(header)
 
     # convert dicts to lists of 2-tuples
     if hasattr(items, 'items'):
-        items = items.items() 
+        items = items.items()
 
     items = [ dt(term) + dd(definition) for term, definition in items ]
     return dl(('\n%s%s\n' % ( header, '\n'.join(items))), **attributes)
 
-def tablify(rows, header=False, item_attributes=None, 
-            **attributes):
+def tablify(rows, header=False, item_attributes=None, **attributes):
     """return an HTML table from a iterable of iterable rows"""
-    
+
     if item_attributes is None:
         item_attributes = {}
 
     retval = []
     if header:
         markup = th
     else:
@@ -137,16 +145,15 @@
     """wrap a string in a webpage"""
 
     _head = ''
     if pagetitle:
         _head += title(pagetitle)
     rel = 'stylesheet'
     for i in stylesheets:
-        attributes = dict(rel=rel,
-                          type='text/css')        
+        attributes = dict(rel=rel, type='text/css')
         if hasattr(i, '__iter__'):
             # assume a 2-tuple
             attributes['href'] = i[0]
             attributes['title'] = i[1]
         else:
             attributes['href'] = i
         _head += '\n' + HTMLmarkup('link', None, **attributes)
```

### Comparing `markup-0.2/setup.py` & `markup-0.2.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 from setuptools import setup, find_packages
 import sys, os
 
-version = '0.2'
+version = '0.2.2'
 
 setup(name='markup',
       version=version,
       description="generate HTML markup programmatically",
-      long_description="""\
-""",
+      long_description="",
       classifiers=[], # Get strings from http://pypi.python.org/pypi?%3Aaction=list_classifiers
       keywords='',
       author='Jeff Hammel',
-      author_email='jhammel@openplans.org',
-      url='http://www.openplans.org/people/k0s/',
+      author_email='k0scist@gmail.com',
+      url='http://k0s.org/',
       license='GPL',
       packages=find_packages(exclude=['ez_setup', 'examples', 'tests']),
       include_package_data=True,
       zip_safe=False,
-      install_requires=[
-          # -*- Extra requirements: -*-
-      ],
+      install_requires=[],
       entry_points="""
       # -*- Entry points: -*-
       """,
-      )
+)
```

