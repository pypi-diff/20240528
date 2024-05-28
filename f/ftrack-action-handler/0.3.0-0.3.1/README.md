# Comparing `tmp/ftrack-action-handler-0.3.0.tar.gz` & `tmp/ftrack_action_handler-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ftrack-action-handler-0.3.0.tar", last modified: Wed May 11 10:20:42 2022, max compression
+gzip compressed data, was "ftrack_action_handler-0.3.1.tar", last modified: Tue May 28 10:45:00 2024, max compression
```

## Comparing `ftrack-action-handler-0.3.0.tar` & `ftrack_action_handler-0.3.1.tar`

### file list

```diff
@@ -1,46 +1,51 @@
-drwxrwxrwx   0        0        0        0 2022-05-11 10:20:42.000000 ftrack-action-handler-0.3.0/
--rw-rw-rw-   0        0        0      380 2022-05-06 13:17:02.000000 ftrack-action-handler-0.3.0/.gitignore
--rw-rw-rw-   0        0        0    10349 2022-05-06 13:17:02.000000 ftrack-action-handler-0.3.0/LICENSE.txt
--rw-rw-rw-   0        0        0       94 2022-05-06 13:17:02.000000 ftrack-action-handler-0.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1674 2022-05-11 10:20:42.000000 ftrack-action-handler-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     1013 2022-05-06 13:17:02.000000 ftrack-action-handler-0.3.0/README.rst
-drwxrwxrwx   0        0        0        0 2022-05-11 10:20:42.000000 ftrack-action-handler-0.3.0/doc/
-drwxrwxrwx   0        0        0        0 2022-05-11 10:20:42.000000 ftrack-action-handler-0.3.0/doc/_static/
--rw-rw-rw-   0        0        0        0 2022-05-06 13:17:02.000000 ftrack-action-handler-0.3.0/doc/_static/.gitkeep
-drwxrwxrwx   0        0        0        0 2022-05-11 10:20:42.000000 ftrack-action-handler-0.3.0/doc/api_reference/
--rw-rw-rw-   0        0        0      469 2022-05-06 14:29:45.000000 ftrack-action-handler-0.3.0/doc/api_reference/index.rst
--rw-rw-rw-   0        0        0     2796 2022-05-06 13:17:02.000000 ftrack-action-handler-0.3.0/doc/conf.py
--rw-rw-rw-   0        0        0      100 2022-05-06 13:17:02.000000 ftrack-action-handler-0.3.0/doc/glossary.rst
--rw-rw-rw-   0        0        0     1119 2022-05-06 13:17:02.000000 ftrack-action-handler-0.3.0/doc/index.rst
--rw-rw-rw-   0        0        0     1735 2022-05-06 13:17:02.000000 ftrack-action-handler-0.3.0/doc/installing.rst
-drwxrwxrwx   0        0        0        0 2022-05-11 10:20:42.000000 ftrack-action-handler-0.3.0/doc/release/
--rw-rw-rw-   0        0        0      369 2022-05-06 13:17:02.000000 ftrack-action-handler-0.3.0/doc/release/index.rst
--rw-rw-rw-   0        0        0     2230 2022-05-06 15:19:09.000000 ftrack-action-handler-0.3.0/doc/release/migration.rst
--rw-rw-rw-   0        0        0     1551 2022-05-11 10:18:08.000000 ftrack-action-handler-0.3.0/doc/release/release_notes.rst
--rw-rw-rw-   0        0        0       33 2022-03-09 20:55:54.000000 ftrack-action-handler-0.3.0/doc/requirements.txt
-drwxrwxrwx   0        0        0        0 2022-05-11 10:20:42.000000 ftrack-action-handler-0.3.0/doc/resources/
--rw-rw-rw-   0        0        0     1601 2022-05-06 15:15:59.000000 ftrack-action-handler-0.3.0/doc/resources/advanced_action.py
--rw-rw-rw-   0        0        0     4464 2022-05-06 15:21:00.000000 ftrack-action-handler-0.3.0/doc/resources/find_and_replace.py
--rw-rw-rw-   0        0        0     1935 2022-05-06 13:17:02.000000 ftrack-action-handler-0.3.0/doc/resources/my_custom_action.py
--rw-rw-rw-   0        0        0     1393 2022-05-06 15:18:13.000000 ftrack-action-handler-0.3.0/doc/using.rst
--rw-rw-rw-   0        0        0      150 2022-05-11 10:20:42.000000 ftrack-action-handler-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     2587 2022-05-06 13:17:02.000000 ftrack-action-handler-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-05-11 10:20:42.000000 ftrack-action-handler-0.3.0/source/
-drwxrwxrwx   0        0        0        0 2022-05-11 10:20:42.000000 ftrack-action-handler-0.3.0/source/ftrack_action_handler/
--rw-rw-rw-   0        0        0      101 2022-05-06 13:17:02.000000 ftrack-action-handler-0.3.0/source/ftrack_action_handler/__init__.py
--rw-rw-rw-   0        0        0       91 2022-05-11 10:20:41.000000 ftrack-action-handler-0.3.0/source/ftrack_action_handler/_version.py
-drwxrwxrwx   0        0        0        0 2022-05-11 10:20:42.000000 ftrack-action-handler-0.3.0/source/ftrack_action_handler/action/
--rw-rw-rw-   0        0        0      136 2022-05-06 13:17:02.000000 ftrack-action-handler-0.3.0/source/ftrack_action_handler/action/__init__.py
--rw-rw-rw-   0        0        0    14297 2022-05-06 13:17:02.000000 ftrack-action-handler-0.3.0/source/ftrack_action_handler/action/advanced.py
--rw-rw-rw-   0        0        0     7633 2022-05-06 13:17:02.000000 ftrack-action-handler-0.3.0/source/ftrack_action_handler/action/base.py
-drwxrwxrwx   0        0        0        0 2022-05-11 10:20:42.000000 ftrack-action-handler-0.3.0/source/ftrack_action_handler.egg-info/
--rw-rw-rw-   0        0        0     1674 2022-05-11 10:20:41.000000 ftrack-action-handler-0.3.0/source/ftrack_action_handler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      961 2022-05-11 10:20:42.000000 ftrack-action-handler-0.3.0/source/ftrack_action_handler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-05-11 10:20:41.000000 ftrack-action-handler-0.3.0/source/ftrack_action_handler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2022-05-11 10:20:42.000000 ftrack-action-handler-0.3.0/source/ftrack_action_handler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2022-05-11 10:20:42.000000 ftrack-action-handler-0.3.0/source/ftrack_action_handler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2022-05-11 10:20:41.000000 ftrack-action-handler-0.3.0/source/ftrack_action_handler.egg-info/zip-safe
-drwxrwxrwx   0        0        0        0 2022-05-11 10:20:42.000000 ftrack-action-handler-0.3.0/test/
-drwxrwxrwx   0        0        0        0 2022-05-11 10:20:42.000000 ftrack-action-handler-0.3.0/test/unit/
--rw-rw-rw-   0        0        0       59 2022-05-06 13:17:02.000000 ftrack-action-handler-0.3.0/test/unit/__init__.py
--rw-rw-rw-   0        0        0       59 2022-05-06 13:17:02.000000 ftrack-action-handler-0.3.0/test/unit/conftest.py
+drwxrwxrwx   0        0        0        0 2024-05-28 10:45:00.340876 ftrack_action_handler-0.3.1/
+drwxrwxrwx   0        0        0        0 2024-05-28 10:45:00.244780 ftrack_action_handler-0.3.1/.github/
+drwxrwxrwx   0        0        0        0 2024-05-28 10:45:00.265737 ftrack_action_handler-0.3.1/.github/workflows/
+-rw-rw-rw-   0        0        0      334 2024-05-28 10:28:27.000000 ftrack_action_handler-0.3.1/.github/workflows/pr-base.yml
+-rw-rw-rw-   0        0        0      380 2024-05-28 10:28:27.000000 ftrack_action_handler-0.3.1/.gitignore
+-rw-rw-rw-   0        0        0      192 2024-05-28 10:28:27.000000 ftrack_action_handler-0.3.1/CODEOWNERS
+-rw-rw-rw-   0        0        0     1228 2024-05-28 10:28:27.000000 ftrack_action_handler-0.3.1/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0    10349 2024-05-28 10:28:27.000000 ftrack_action_handler-0.3.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       94 2024-05-28 10:28:27.000000 ftrack_action_handler-0.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    12944 2024-05-28 10:45:00.338873 ftrack_action_handler-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2024-05-28 10:28:27.000000 ftrack_action_handler-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 10:45:00.278859 ftrack_action_handler-0.3.1/doc/
+drwxrwxrwx   0        0        0        0 2024-05-28 10:45:00.280858 ftrack_action_handler-0.3.1/doc/_static/
+-rw-rw-rw-   0        0        0        0 2024-05-28 10:28:27.000000 ftrack_action_handler-0.3.1/doc/_static/.gitkeep
+drwxrwxrwx   0        0        0        0 2024-05-28 10:45:00.282857 ftrack_action_handler-0.3.1/doc/api_reference/
+-rw-rw-rw-   0        0        0      469 2024-05-28 10:28:27.000000 ftrack_action_handler-0.3.1/doc/api_reference/index.rst
+-rw-rw-rw-   0        0        0     2588 2024-05-28 10:28:27.000000 ftrack_action_handler-0.3.1/doc/conf.py
+-rw-rw-rw-   0        0        0      100 2024-05-28 10:28:27.000000 ftrack_action_handler-0.3.1/doc/glossary.rst
+-rw-rw-rw-   0        0        0     1119 2024-05-28 10:28:27.000000 ftrack_action_handler-0.3.1/doc/index.rst
+-rw-rw-rw-   0        0        0     1735 2024-05-28 10:28:27.000000 ftrack_action_handler-0.3.1/doc/installing.rst
+drwxrwxrwx   0        0        0        0 2024-05-28 10:45:00.288858 ftrack_action_handler-0.3.1/doc/release/
+-rw-rw-rw-   0        0        0      369 2024-05-28 10:28:27.000000 ftrack_action_handler-0.3.1/doc/release/index.rst
+-rw-rw-rw-   0        0        0     2230 2024-05-28 10:28:27.000000 ftrack_action_handler-0.3.1/doc/release/migration.rst
+-rw-rw-rw-   0        0        0     2020 2024-05-28 10:28:27.000000 ftrack_action_handler-0.3.1/doc/release/release_notes.rst
+-rw-rw-rw-   0        0        0       33 2024-05-28 10:28:27.000000 ftrack_action_handler-0.3.1/doc/requirements.txt
+drwxrwxrwx   0        0        0        0 2024-05-28 10:45:00.298865 ftrack_action_handler-0.3.1/doc/resources/
+-rw-rw-rw-   0        0        0     1601 2024-05-28 10:28:27.000000 ftrack_action_handler-0.3.1/doc/resources/advanced_action.py
+-rw-rw-rw-   0        0        0     4464 2024-05-28 10:28:27.000000 ftrack_action_handler-0.3.1/doc/resources/find_and_replace.py
+-rw-rw-rw-   0        0        0     1935 2024-05-28 10:28:27.000000 ftrack_action_handler-0.3.1/doc/resources/my_custom_action.py
+-rw-rw-rw-   0        0        0     1315 2024-05-28 10:28:27.000000 ftrack_action_handler-0.3.1/doc/resources/user_run_action.py
+-rw-rw-rw-   0        0        0     1393 2024-05-28 10:28:27.000000 ftrack_action_handler-0.3.1/doc/using.rst
+-rw-rw-rw-   0        0        0     1651 2024-05-28 10:28:27.000000 ftrack_action_handler-0.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-28 10:45:00.341874 ftrack_action_handler-0.3.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-28 10:45:00.247778 ftrack_action_handler-0.3.1/source/
+drwxrwxrwx   0        0        0        0 2024-05-28 10:45:00.303867 ftrack_action_handler-0.3.1/source/ftrack_action_handler/
+-rw-rw-rw-   0        0        0      122 2024-05-28 10:28:27.000000 ftrack_action_handler-0.3.1/source/ftrack_action_handler/__init__.py
+-rw-rw-rw-   0        0        0       89 2024-05-28 10:44:59.000000 ftrack_action_handler-0.3.1/source/ftrack_action_handler/_version.py
+drwxrwxrwx   0        0        0        0 2024-05-28 10:45:00.326873 ftrack_action_handler-0.3.1/source/ftrack_action_handler/action/
+-rw-rw-rw-   0        0        0      136 2024-05-28 10:28:27.000000 ftrack_action_handler-0.3.1/source/ftrack_action_handler/action/__init__.py
+-rw-rw-rw-   0        0        0    14175 2024-05-28 10:28:27.000000 ftrack_action_handler-0.3.1/source/ftrack_action_handler/action/advanced.py
+-rw-rw-rw-   0        0        0     7633 2024-05-28 10:28:27.000000 ftrack_action_handler-0.3.1/source/ftrack_action_handler/action/base.py
+drwxrwxrwx   0        0        0        0 2024-05-28 10:45:00.335873 ftrack_action_handler-0.3.1/source/ftrack_action_handler.egg-info/
+-rw-rw-rw-   0        0        0    12944 2024-05-28 10:45:00.000000 ftrack_action_handler-0.3.1/source/ftrack_action_handler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      999 2024-05-28 10:45:00.000000 ftrack_action_handler-0.3.1/source/ftrack_action_handler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 10:45:00.000000 ftrack_action_handler-0.3.1/source/ftrack_action_handler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       99 2024-05-28 10:45:00.000000 ftrack_action_handler-0.3.1/source/ftrack_action_handler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-05-28 10:45:00.000000 ftrack_action_handler-0.3.1/source/ftrack_action_handler.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-28 10:45:00.248778 ftrack_action_handler-0.3.1/test/
+drwxrwxrwx   0        0        0        0 2024-05-28 10:45:00.332873 ftrack_action_handler-0.3.1/test/unit/
+-rw-rw-rw-   0        0        0       59 2024-05-28 10:28:27.000000 ftrack_action_handler-0.3.1/test/unit/__init__.py
+-rw-rw-rw-   0        0        0       59 2024-05-28 10:28:27.000000 ftrack_action_handler-0.3.1/test/unit/conftest.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ftrack-action-handler-0.3.0/LICENSE.txt` & `ftrack_action_handler-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ftrack-action-handler-0.3.0/README.rst` & `ftrack_action_handler-0.3.1/doc/index.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,32 @@
+..
+    :copyright: Copyright (c) 2017 ftrack
+
 ###############################
 ftrack-action-handler
 ###############################
 
-Simple example implementation of a BaseClass for handeling ftrack actions.
+Simple example implementation of a base class for handling ftrack actions.
 
-*************
-Documentation
-*************
+.. toctree::
+    :maxdepth: 1
 
-Full documentation, including installation and setup guides, can be found at
-http://ftrack-action-handler.rtd.ftrack.com/en/stable/
+    installing
+    using
+    api_reference/index
+    release/index
+    glossary
+
+******************
+Indices and tables
+******************
+
+* :ref:`genindex`
+* :ref:`modindex`
+* :ref:`search`
 
 *********************
 Copyright and license
 *********************
 
 Copyright (c) 2017 ftrack
```

### Comparing `ftrack-action-handler-0.3.0/doc/conf.py` & `ftrack_action_handler-0.3.1/doc/conf.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # :coding: utf-8
 # :copyright: Copyright (c) 2017 ftrack
 
 '''ftrack-action-handler documentation build configuration file.'''
 
 import os
 import sys
+from sphinx_pyproject import SphinxConfig
 
-from pkg_resources import DistributionNotFound, get_distribution
+from ftrack_action_handler import __version__ as _version
 
 # -- General ------------------------------------------------------------------
 # Inject source onto path so that autodoc can find it by default, but in such a
 # way as to allow overriding location.
 sys.path.append(
     os.path.abspath(os.path.join(os.path.dirname(__file__), '..', 'source'))
 )
@@ -31,25 +32,17 @@
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
 project = u'ftrack-action-handler'
 copyright = u'2017, ftrack'
 
-try:
-    release = get_distribution('ftrack-action-handler').version
-    # take major/minor/patch
-    VERSION = '.'.join(release.split('.')[:3])
-
-except DistributionNotFound:
-    # package is not installed
-    VERSION = 'Unknown version'
+version = _version
+release = _version
 
-version = VERSION
-release = VERSION
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 exclude_patterns = ['_template']
 
 # A list of prefixes to ignore for module listings.
 modindex_common_prefix = ['ftrack_action_handler.']
```

### Comparing `ftrack-action-handler-0.3.0/doc/installing.rst` & `ftrack_action_handler-0.3.1/doc/installing.rst`

 * *Files identical despite different names*

### Comparing `ftrack-action-handler-0.3.0/doc/release/migration.rst` & `ftrack_action_handler-0.3.1/doc/release/migration.rst`

 * *Files identical despite different names*

### Comparing `ftrack-action-handler-0.3.0/doc/release/release_notes.rst` & `ftrack_action_handler-0.3.1/doc/release/release_notes.rst`

 * *Files 26% similar despite different names*

```diff
@@ -3,14 +3,29 @@
 
 .. _release/release_notes:
 
 *************
 Release Notes
 *************
 
+.. release:: Upcoming
+    .. change:: changed
+        :tags: API
+
+        Provide run_as_user property in :ref:`AdvancedBaseAction <api_reference/AdvancedBaseAction>` to run the action as the user executing it.
+
+    .. change:: changed
+        :tags: Installer
+
+        Allow to install for ftrack-python-api 3.0.
+
+    .. change:: changed
+        :tags: API
+
+        Remove _get_entity_type from AdvancedBaseAction and rely on base class implementation.
 
 .. release:: 0.3.0
     :date: 2022-05-11
 
     .. change:: changed
         :tags: API
```

### Comparing `ftrack-action-handler-0.3.0/doc/resources/advanced_action.py` & `ftrack_action_handler-0.3.1/doc/resources/advanced_action.py`

 * *Files identical despite different names*

### Comparing `ftrack-action-handler-0.3.0/doc/resources/find_and_replace.py` & `ftrack_action_handler-0.3.1/doc/resources/find_and_replace.py`

 * *Files identical despite different names*

### Comparing `ftrack-action-handler-0.3.0/doc/resources/my_custom_action.py` & `ftrack_action_handler-0.3.1/doc/resources/my_custom_action.py`

 * *Files identical despite different names*

### Comparing `ftrack-action-handler-0.3.0/doc/using.rst` & `ftrack_action_handler-0.3.1/doc/using.rst`

 * *Files identical despite different names*

### Comparing `ftrack-action-handler-0.3.0/source/ftrack_action_handler/action/advanced.py` & `ftrack_action_handler-0.3.1/source/ftrack_action_handler/action/advanced.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # :coding: utf-8
 # :copyright: Copyright (c) 2017-2021 ftrack
 
 import json
 import logging
 import os
 import uuid
+import ftrack_api
 from ftrack_action_handler.action import BaseAction
 
 logging.basicConfig(level=logging.INFO)
 
 
 # --------------------------------------------------------------
 # Advanced Action Class.
@@ -35,14 +36,15 @@
 
     # Action filters
     allowed_roles = []  # Roles allowed for this action to run
     allowed_groups = []  # Groups allowed for this action to run
     ignored_types = []  # Types ignored for this action to run
     allowed_types = []  # Types allowed for this action to run
     limit_to_user = None  # Limit the action to the user which spans it
+    run_as_user = False # Run as the user running the action, not the one registering it.
     allow_empty_context = False  # Allow to run without a selection
 
     def __repr__(self):
         '''Action object representation.'''
         return '<{0}:{1}>'.format(self.__class__.__name__, self.identifier)
 
     def __init__(self, session, limit_to_user=None, make_unique=False):
@@ -246,38 +248,14 @@
         '''
         if self.limit_to_user is not None:
             if action_user['username'] != self.limit_to_user:
                 return False
             return True
         return True
 
-    def _get_entity_type(self, entity):
-        '''Return translated entity type that can be used with API.'''
-        # Get entity type and make sure it is lower cased. Most places except
-        # the component tab in the Sidebar will use lower case notation.
-        entity_type = entity.get('entityType').replace('_', '').lower()
-
-        for schema in self.session.schemas:
-            alias_for = schema.get('alias_for')
-
-            if (
-                    alias_for
-                    and isinstance(alias_for, str)
-                    and alias_for.lower() == entity_type
-            ):
-                return schema['id']
-
-        for schema in self.session.schemas:
-            if schema['id'].lower() == entity_type:
-                return schema['id']
-
-        raise ValueError(
-            'Unable to translate entity type: {0}.'.format(entity_type)
-        )
-
     # --------------------------------------------------------------
     # Default Action Method Overwrites
     # --------------------------------------------------------------
 
 
     def _discover(self, event):
         entities = self._translate_event(self.session, event)
@@ -394,7 +372,25 @@
     def mark_job_as_done(self, job_id, description):
         '''Mark a job as done.'''
 
         job = self.session.get('Job', job_id)
         job['data'] = json.dumps({'description': u'{}'.format(description)})
         job['status'] = 'done'
         self.session.commit()
+
+    def _launch(self, event):
+        if self.run_as_user:
+            user = event['source']['user']['username']
+            try:
+                new_session = ftrack_api.Session(
+                    server_url=self.session.server_url,
+                    api_key=self.session.api_key,
+                    api_user=user,
+                    auto_connect_event_hub=False
+                )
+            except Exception:
+                self.logger.warn('Please ensure your action has been registered with a Global API key.')
+                raise
+
+            self._session = new_session
+
+        return super(AdvancedBaseAction, self)._launch(event)
```

### Comparing `ftrack-action-handler-0.3.0/source/ftrack_action_handler/action/base.py` & `ftrack_action_handler-0.3.1/source/ftrack_action_handler/action/base.py`

 * *Files identical despite different names*

### Comparing `ftrack-action-handler-0.3.0/source/ftrack_action_handler.egg-info/SOURCES.txt` & `ftrack_action_handler-0.3.1/source/ftrack_action_handler.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 .gitignore
+CODEOWNERS
+CONTRIBUTING.md
 LICENSE.txt
 MANIFEST.in
-README.rst
-setup.cfg
-setup.py
+README.md
+pyproject.toml
+.github/workflows/pr-base.yml
 doc/conf.py
 doc/glossary.rst
 doc/index.rst
 doc/installing.rst
 doc/requirements.txt
 doc/using.rst
 doc/_static/.gitkeep
 doc/api_reference/index.rst
 doc/release/index.rst
 doc/release/migration.rst
 doc/release/release_notes.rst
 doc/resources/advanced_action.py
 doc/resources/find_and_replace.py
 doc/resources/my_custom_action.py
+doc/resources/user_run_action.py
 source/ftrack_action_handler/__init__.py
 source/ftrack_action_handler/_version.py
 source/ftrack_action_handler.egg-info/PKG-INFO
 source/ftrack_action_handler.egg-info/SOURCES.txt
 source/ftrack_action_handler.egg-info/dependency_links.txt
 source/ftrack_action_handler.egg-info/requires.txt
 source/ftrack_action_handler.egg-info/top_level.txt
-source/ftrack_action_handler.egg-info/zip-safe
 source/ftrack_action_handler/action/__init__.py
 source/ftrack_action_handler/action/advanced.py
 source/ftrack_action_handler/action/base.py
 test/unit/__init__.py
 test/unit/conftest.py
```

