# Comparing `tmp/poppy-pop-0.8.3.tar.gz` & `tmp/poppy-pop-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poppy-pop-0.8.3.tar", max compression
+gzip compressed data, was "poppy-pop-0.9.0.tar", max compression
```

## Comparing `poppy-pop-0.8.3.tar` & `poppy-pop-0.9.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0    21863 2022-12-06 18:42:09.358659 poppy-pop-0.8.3/LICENSE
--rw-r--r--   0        0        0      915 2022-12-06 18:42:09.358659 poppy-pop-0.8.3/README.md
--rw-r--r--   0        0        0       64 2022-12-06 18:42:09.358659 poppy-pop-0.8.3/poppy/__init__.py
--rw-r--r--   0        0        0      374 2022-12-06 18:42:09.358659 poppy-pop-0.8.3/poppy/pop/__init__.py
--rw-r--r--   0        0        0       70 2022-12-06 18:42:09.358659 poppy-pop-0.8.3/poppy/pop/alembic/__init__.py
--rw-r--r--   0        0        0     2934 2022-12-06 18:42:09.358659 poppy-pop-0.8.3/poppy/pop/alembic/env.py
--rw-r--r--   0        0        0     2102 2022-12-06 18:42:09.358659 poppy-pop-0.8.3/poppy/pop/alembic/helpers.py
--rw-r--r--   0        0        0      494 2022-12-06 18:42:09.358659 poppy-pop-0.8.3/poppy/pop/alembic/script.py.mako
--rw-r--r--   0        0        0      165 2022-12-06 18:42:09.358659 poppy-pop-0.8.3/poppy/pop/commands/__init__.py
--rw-r--r--   0        0        0     2514 2022-12-06 18:42:09.358659 poppy-pop-0.8.3/poppy/pop/commands/db.py
--rw-r--r--   0        0        0     3814 2022-12-06 18:42:09.358659 poppy-pop-0.8.3/poppy/pop/commands/master.py
--rw-r--r--   0        0        0     6227 2022-12-06 18:42:09.358659 poppy-pop-0.8.3/poppy/pop/commands/migration.py
--rw-r--r--   0        0        0     3666 2022-12-06 18:42:09.358659 poppy-pop-0.8.3/poppy/pop/commands/test.py
--rw-r--r--   0        0        0      642 2022-12-06 18:42:09.358659 poppy-pop-0.8.3/poppy/pop/commands/web_admin.py
--rw-r--r--   0        0        0     1122 2022-12-06 18:42:09.358659 poppy-pop-0.8.3/poppy/pop/db_connector.py
--rw-r--r--   0        0        0     2038 2022-12-06 18:42:09.358659 poppy-pop-0.8.3/poppy/pop/descriptor.json
--rw-r--r--   0        0        0       69 2022-12-06 18:42:09.362659 poppy-pop-0.8.3/poppy/pop/json_schemas/__init__.py
--rw-r--r--   0        0        0     1861 2022-12-06 18:42:09.362659 poppy-pop-0.8.3/poppy/pop/json_schemas/config-schema.json
--rw-r--r--   0        0        0     2590 2022-12-06 18:42:09.362659 poppy-pop-0.8.3/poppy/pop/json_schemas/pipeline-descriptor-schema.json
--rw-r--r--   0        0        0     4659 2022-12-06 18:42:09.362659 poppy-pop-0.8.3/poppy/pop/json_schemas/plugin-descriptor-schema.json
--rw-r--r--   0        0        0      343 2022-12-06 18:42:09.362659 poppy-pop-0.8.3/poppy/pop/loop.py
--rw-r--r--   0        0        0      158 2022-12-06 18:42:09.362659 poppy-pop-0.8.3/poppy/pop/migration.py
--rw-r--r--   0        0        0      782 2022-12-06 18:42:09.362659 poppy-pop-0.8.3/poppy/pop/models/__init__.py
--rw-r--r--   0        0        0     1294 2022-12-06 18:42:09.362659 poppy-pop-0.8.3/poppy/pop/models/alembic_script_extra.py
--rw-r--r--   0        0        0     4665 2022-12-06 18:42:09.362659 poppy-pop-0.8.3/poppy/pop/models/job.py
--rw-r--r--   0        0        0     3353 2022-12-06 18:42:09.362659 poppy-pop-0.8.3/poppy/pop/models/versions/poppy_pop_0001_initial_.py
--rw-r--r--   0        0        0      882 2022-12-06 18:42:09.362659 poppy-pop-0.8.3/poppy/pop/models/versions/poppy_pop_0002_version_num_.py
--rw-r--r--   0        0        0      656 2022-12-06 18:42:09.362659 poppy-pop-0.8.3/poppy/pop/plugins.py
--rw-r--r--   0        0        0     2280 2022-12-06 18:42:09.362659 poppy-pop-0.8.3/poppy/pop/pop.py
--rw-r--r--   0        0        0       91 2022-12-06 18:42:09.362659 poppy-pop-0.8.3/poppy/pop/scripts/__init__.py
--rw-r--r--   0        0        0      478 2022-12-06 18:42:09.362659 poppy-pop-0.8.3/poppy/pop/scripts/create_migrator.sql
--rw-r--r--   0        0        0      108 2022-12-06 18:42:09.362659 poppy-pop-0.8.3/poppy/pop/scripts/drop_migrator.sql
--rw-r--r--   0        0        0     7777 2022-12-06 18:42:09.362659 poppy-pop-0.8.3/poppy/pop/scripts/scripts.py
--rw-r--r--   0        0        0    10273 2022-12-06 18:42:09.362659 poppy-pop-0.8.3/poppy/pop/tasks.py
--rw-r--r--   0        0        0     1176 2022-12-06 18:42:09.362659 poppy-pop-0.8.3/poppy/pop/tests.py
--rw-r--r--   0        0        0      579 2022-12-06 18:42:09.362659 poppy-pop-0.8.3/poppy/pop/tools.py
--rw-r--r--   0        0        0      977 2022-12-06 18:42:09.362659 poppy-pop-0.8.3/pyproject.toml
--rw-r--r--   0        0        0     1851 2022-12-06 18:42:43.382408 poppy-pop-0.8.3/setup.py
--rw-r--r--   0        0        0     1513 2022-12-06 18:42:43.383076 poppy-pop-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0    21863 2022-12-14 16:46:19.122214 poppy-pop-0.9.0/LICENSE
+-rw-r--r--   0        0        0      915 2022-12-14 16:46:19.122214 poppy-pop-0.9.0/README.md
+-rw-r--r--   0        0        0       64 2022-12-14 16:46:19.122214 poppy-pop-0.9.0/poppy/__init__.py
+-rw-r--r--   0        0        0      374 2022-12-14 16:46:19.122214 poppy-pop-0.9.0/poppy/pop/__init__.py
+-rw-r--r--   0        0        0       70 2022-12-14 16:46:19.122214 poppy-pop-0.9.0/poppy/pop/alembic/__init__.py
+-rw-r--r--   0        0        0     2934 2022-12-14 16:46:19.122214 poppy-pop-0.9.0/poppy/pop/alembic/env.py
+-rw-r--r--   0        0        0     2102 2022-12-14 16:46:19.122214 poppy-pop-0.9.0/poppy/pop/alembic/helpers.py
+-rw-r--r--   0        0        0      494 2022-12-14 16:46:19.122214 poppy-pop-0.9.0/poppy/pop/alembic/script.py.mako
+-rw-r--r--   0        0        0      165 2022-12-14 16:46:19.122214 poppy-pop-0.9.0/poppy/pop/commands/__init__.py
+-rw-r--r--   0        0        0     2514 2022-12-14 16:46:19.122214 poppy-pop-0.9.0/poppy/pop/commands/db.py
+-rw-r--r--   0        0        0     3814 2022-12-14 16:46:19.122214 poppy-pop-0.9.0/poppy/pop/commands/master.py
+-rw-r--r--   0        0        0     6859 2022-12-14 16:46:19.122214 poppy-pop-0.9.0/poppy/pop/commands/migration.py
+-rw-r--r--   0        0        0     3666 2022-12-14 16:46:19.122214 poppy-pop-0.9.0/poppy/pop/commands/test.py
+-rw-r--r--   0        0        0      642 2022-12-14 16:46:19.122214 poppy-pop-0.9.0/poppy/pop/commands/web_admin.py
+-rw-r--r--   0        0        0     1122 2022-12-14 16:46:19.122214 poppy-pop-0.9.0/poppy/pop/db_connector.py
+-rw-r--r--   0        0        0     2247 2022-12-14 16:46:19.122214 poppy-pop-0.9.0/poppy/pop/descriptor.json
+-rw-r--r--   0        0        0       69 2022-12-14 16:46:19.122214 poppy-pop-0.9.0/poppy/pop/json_schemas/__init__.py
+-rw-r--r--   0        0        0     1861 2022-12-14 16:46:19.122214 poppy-pop-0.9.0/poppy/pop/json_schemas/config-schema.json
+-rw-r--r--   0        0        0     2590 2022-12-14 16:46:19.122214 poppy-pop-0.9.0/poppy/pop/json_schemas/pipeline-descriptor-schema.json
+-rw-r--r--   0        0        0     4659 2022-12-14 16:46:19.122214 poppy-pop-0.9.0/poppy/pop/json_schemas/plugin-descriptor-schema.json
+-rw-r--r--   0        0        0      343 2022-12-14 16:46:19.122214 poppy-pop-0.9.0/poppy/pop/loop.py
+-rw-r--r--   0        0        0      158 2022-12-14 16:46:19.122214 poppy-pop-0.9.0/poppy/pop/migration.py
+-rw-r--r--   0        0        0      782 2022-12-14 16:46:19.122214 poppy-pop-0.9.0/poppy/pop/models/__init__.py
+-rw-r--r--   0        0        0     1294 2022-12-14 16:46:19.122214 poppy-pop-0.9.0/poppy/pop/models/alembic_script_extra.py
+-rw-r--r--   0        0        0     4665 2022-12-14 16:46:19.122214 poppy-pop-0.9.0/poppy/pop/models/job.py
+-rw-r--r--   0        0        0     3353 2022-12-14 16:46:19.122214 poppy-pop-0.9.0/poppy/pop/models/versions/poppy_pop_0001_initial_.py
+-rw-r--r--   0        0        0      882 2022-12-14 16:46:19.122214 poppy-pop-0.9.0/poppy/pop/models/versions/poppy_pop_0002_version_num_.py
+-rw-r--r--   0        0        0      656 2022-12-14 16:46:19.122214 poppy-pop-0.9.0/poppy/pop/plugins.py
+-rw-r--r--   0        0        0     2280 2022-12-14 16:46:19.122214 poppy-pop-0.9.0/poppy/pop/pop.py
+-rw-r--r--   0        0        0       91 2022-12-14 16:46:19.122214 poppy-pop-0.9.0/poppy/pop/scripts/__init__.py
+-rw-r--r--   0        0        0      478 2022-12-14 16:46:19.122214 poppy-pop-0.9.0/poppy/pop/scripts/create_migrator.sql
+-rw-r--r--   0        0        0      108 2022-12-14 16:46:19.122214 poppy-pop-0.9.0/poppy/pop/scripts/drop_migrator.sql
+-rw-r--r--   0        0        0     7777 2022-12-14 16:46:19.122214 poppy-pop-0.9.0/poppy/pop/scripts/scripts.py
+-rw-r--r--   0        0        0    11664 2022-12-14 16:46:19.122214 poppy-pop-0.9.0/poppy/pop/tasks.py
+-rw-r--r--   0        0        0     1176 2022-12-14 16:46:19.122214 poppy-pop-0.9.0/poppy/pop/tests.py
+-rw-r--r--   0        0        0      579 2022-12-14 16:46:19.122214 poppy-pop-0.9.0/poppy/pop/tools.py
+-rw-r--r--   0        0        0     1026 2022-12-14 16:46:19.122214 poppy-pop-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1851 2022-12-14 17:08:30.525842 poppy-pop-0.9.0/setup.py
+-rw-r--r--   0        0        0     1513 2022-12-14 17:08:30.526152 poppy-pop-0.9.0/PKG-INFO
```

### Comparing `poppy-pop-0.8.3/LICENSE` & `poppy-pop-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `poppy-pop-0.8.3/README.md` & `poppy-pop-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `poppy-pop-0.8.3/poppy/pop/alembic/env.py` & `poppy-pop-0.9.0/poppy/pop/alembic/env.py`

 * *Files identical despite different names*

### Comparing `poppy-pop-0.8.3/poppy/pop/alembic/helpers.py` & `poppy-pop-0.9.0/poppy/pop/alembic/helpers.py`

 * *Files identical despite different names*

### Comparing `poppy-pop-0.8.3/poppy/pop/commands/db.py` & `poppy-pop-0.9.0/poppy/pop/commands/db.py`

 * *Files identical despite different names*

### Comparing `poppy-pop-0.8.3/poppy/pop/commands/master.py` & `poppy-pop-0.9.0/poppy/pop/commands/master.py`

 * *Files identical despite different names*

### Comparing `poppy-pop-0.8.3/poppy/pop/commands/migration.py` & `poppy-pop-0.9.0/poppy/pop/commands/migration.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 from poppy.core.command import Command
 from poppy.pop.tasks import Downgrade
+from poppy.pop.tasks import DowngradeAll
 from poppy.pop.tasks import Upgrade
 #from poppy.pop.tasks import set_current
 from poppy.pop.tasks import ShowCurrent
 from poppy.pop.tasks import Makemigrations
 
 __all__ = []
 
 
 class MigratorUpgradeCommand(Command):
     """
     Commands relative to the migrator for the pipeline database.
     """
-    __command__ = "migrator_upgrade"
-    __command_name__ = "upgrade"
-    __parent__ = "db"
-    __parent_arguments__ = ["base"]
-    __help__ = "Upgrade the pipeline database to the specified revision"
+    __command__ = 'migrator_upgrade'
+    __command_name__ = 'upgrade'
+    __parent__ = 'db'
+    __parent_arguments__ = ['base']
+    __help__ = 'Upgrade the pipeline database to the specified revision'
 
     def add_arguments(self, parser):
         """
         Add arguments for the migration of the database for a given plugin and
         to a given revision.
         """
 
         # and an argument for the revision to move on
         parser.add_argument(
-            "revision",
+            'revision',
             type=str,
             default=None,
-            nargs="?",
+            nargs='?',
             help="""
             The revision of the database to switch on. Can be either 'head' for
-            the last revision, or an unique identifier of the revision (for 
-            example 'ae1' for the revision 'ae1027a6acf'), or a decimal value 
+            the last revision, or an unique identifier of the revision (for
+            example 'ae1' for the revision 'ae1027a6acf'), or a decimal value
             '+N' N being the number of revisions to execute from the current one.
             """
         )
 
     def setup_tasks(self, pipeline):
         """
         Executed to update the database.
@@ -54,36 +55,36 @@
         pipeline.start = task
 
 
 class MigratorDowngradeCommand(Command):
     """
     Commands relative to the migrator for the poppy database.
     """
-    __command__ = "migrator_downgrade"
-    __command_name__ = "downgrade"
-    __parent__ = "db"
-    __parent_arguments__ = ["base"]
-    __help__ = "Downgrade the POPPy database to the specified revision"
+    __command__ = 'migrator_downgrade'
+    __command_name__ = 'downgrade'
+    __parent__ = 'db'
+    __parent_arguments__ = ['base']
+    __help__ = 'Downgrade the POPPy database to the specified revision'
 
     def add_arguments(self, parser):
         """
         Add arguments for the migration of the database for a given plugin and
         to a given revision.
         """
 
         # and an argument for the revision to move on
         parser.add_argument(
-            "revision",
+            'revision',
             type=str,
             default=None,
-            nargs="?",
+            nargs='?',
             help="""
-            The revision of the database to switch on. Can be a unique 
-            identifier of the revision (for example 'ae1' for the revision 
-            'ae1027a6acf'), or a decimal value '-N' N being the number of 
+            The revision of the database to switch on. Can be a unique
+            identifier of the revision (for example 'ae1' for the revision
+            'ae1027a6acf'), or a decimal value '-N' N being the number of
             revisions to downgrade from the current one.
             one.
         """
         )
 
     def setup_tasks(self, pipeline):
         """
@@ -98,19 +99,19 @@
         pipeline.start = task
 
 
 class MigratorCurrentCommand(Command):
     """
     Commands relative to the migrator for the poppy database.
     """
-    __command__ = "migrator_current"
-    __command_name__ = "current"
-    __parent__ = "db"
-    __parent_arguments__ = ["base"]
-    __help__ = "Show information on the current revision of the POPPy database"
+    __command__ = 'migrator_current'
+    __command_name__ = 'current'
+    __parent__ = 'db'
+    __parent_arguments__ = ['base']
+    __help__ = 'Show information on the current revision of the POPPy database'
 
     def setup_tasks(self, pipeline):
         """
         Show information on the current revision of the POPPy database.
         """
 
         # the task
@@ -121,27 +122,27 @@
         pipeline.start = task
 
 
 class MigratorMakemigrationsCommand(Command):
     """
     Commands to call the generation of migrations
     """
-    __command__ = "migrator_makemigrations"
-    __command_name__ = "makemigrations"
-    __parent__ = "db"
-    __parent_arguments__ = ["base"]
-    __help__ = "Show information on the current revision of the POPPy database"
+    __command__ = 'migrator_makemigrations'
+    __command_name__ = 'makemigrations'
+    __parent__ = 'db'
+    __parent_arguments__ = ['base']
+    __help__ = 'Show information on the current revision of the POPPy database'
 
     def add_arguments(self, parser):
         """
         Add arguments for the migration of the database for a given plugin
         """
         # argument for the plugin to use
         parser.add_argument(
-            "plugin",
+            'plugin',
             type=str,
             help="""
             The name of the plugin for which the migration will be applied.
             """,
         )
 
     def setup_tasks(self, pipeline):
@@ -152,14 +153,38 @@
         # the task
         task = Makemigrations()
 
         # create the topology of tasks
         pipeline | task
         pipeline.start = task
 
+
+class MigratorDowngradeAllCommand(Command):
+    """
+    Commands relative to the migrator for the poppy database.
+    """
+    __command__ = 'migrator_downgrade_all'
+    __command_name__ = 'downgrade_all'
+    __parent__ = 'db'
+    __parent_arguments__ = ['base']
+    __help__ = 'Downgrade the POPPy database to the first initial revision'
+
+    def setup_tasks(self, pipeline):
+        """
+        Executed to fully downgrade the database.
+        """
+
+        # the task
+        task = DowngradeAll()
+
+        # create the topology of tasks
+        pipeline | task
+        pipeline.start = task
+
+
 # TODO - Make this command functional (not set_current() method in poppy.pop.tasks)
 # class MigratorSetCurrentCommand(Command):
 #     """
 #     Commands relative to the migrator for the poppy database.
 #     """
 #     __command__ = "migrator_current_set"
 #     __command_name__ = "set"
@@ -208,8 +233,7 @@
 #
 #         # create the topology of tasks
 #         pipeline | task
 #         pipeline.start = task
 #
 #         # run the pipeline
 #         pipeline.run()
-
```

### Comparing `poppy-pop-0.8.3/poppy/pop/commands/test.py` & `poppy-pop-0.9.0/poppy/pop/commands/test.py`

 * *Files identical despite different names*

### Comparing `poppy-pop-0.8.3/poppy/pop/commands/web_admin.py` & `poppy-pop-0.9.0/poppy/pop/commands/web_admin.py`

 * *Files identical despite different names*

### Comparing `poppy-pop-0.8.3/poppy/pop/db_connector.py` & `poppy-pop-0.9.0/poppy/pop/db_connector.py`

 * *Files identical despite different names*

### Comparing `poppy-pop-0.8.3/poppy/pop/descriptor.json` & `poppy-pop-0.9.0/poppy/pop/descriptor.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9457671957671957%*

 * *Differences: {"'release'": "{'version': '0.9.0', 'date': '2022-12-14', 'modification': 'Add downgrade_all "*

 * *              "task/command'}",*

 * * "'tasks'": "{insert: [(5, OrderedDict([('name', 'downgrade_all'), ('category', 'Software "*

 * *            "execution'), ('description', 'A task to fully reverse the migrations of the POPPy "*

 * *            "database'), ('inputs', OrderedDict()), ('outputs', OrderedDict())]))]}"}*

```diff
@@ -4,19 +4,19 @@
         "identifier": "poppy.pop",
         "name": "POPPY Operation Plugin (POP)",
         "project": "POPPY"
     },
     "release": {
         "author": "Xavier Bonnin <xavier.bonnin@obspm.fr>, ROC Team <roc.support@sympa.obspm.fr>",
         "contact": "roc.support@sympa.obspm.fr",
-        "date": "2022-12-06",
+        "date": "2022-12-14",
         "institute": "LESIA",
-        "modification": "Add port in config-schema.json",
+        "modification": "Add downgrade_all task/command",
         "url": "https://gitlab.obspm.fr/POPPy/POP",
-        "version": "0.8.3"
+        "version": "0.9.0"
     },
     "tasks": [
         {
             "category": "Software execution",
             "description": "To execute a script on the POPPy database",
             "inputs": {},
             "name": "execute",
@@ -48,14 +48,21 @@
             "description": "A task to reverse the migration of the POPPy database",
             "inputs": {},
             "name": "downgrade",
             "outputs": {}
         },
         {
             "category": "Software execution",
+            "description": "A task to fully reverse the migrations of the POPPy database",
+            "inputs": {},
+            "name": "downgrade_all",
+            "outputs": {}
+        },
+        {
+            "category": "Software execution",
             "description": "Show the status of the current revision",
             "inputs": {},
             "name": "show_current",
             "outputs": {}
         },
         {
             "category": "Software execution",
```

### Comparing `poppy-pop-0.8.3/poppy/pop/json_schemas/config-schema.json` & `poppy-pop-0.9.0/poppy/pop/json_schemas/config-schema.json`

 * *Files identical despite different names*

### Comparing `poppy-pop-0.8.3/poppy/pop/json_schemas/pipeline-descriptor-schema.json` & `poppy-pop-0.9.0/poppy/pop/json_schemas/pipeline-descriptor-schema.json`

 * *Files identical despite different names*

### Comparing `poppy-pop-0.8.3/poppy/pop/json_schemas/plugin-descriptor-schema.json` & `poppy-pop-0.9.0/poppy/pop/json_schemas/plugin-descriptor-schema.json`

 * *Files identical despite different names*

### Comparing `poppy-pop-0.8.3/poppy/pop/models/__init__.py` & `poppy-pop-0.9.0/poppy/pop/models/__init__.py`

 * *Files identical despite different names*

### Comparing `poppy-pop-0.8.3/poppy/pop/models/alembic_script_extra.py` & `poppy-pop-0.9.0/poppy/pop/models/alembic_script_extra.py`

 * *Files identical despite different names*

### Comparing `poppy-pop-0.8.3/poppy/pop/models/job.py` & `poppy-pop-0.9.0/poppy/pop/models/job.py`

 * *Files identical despite different names*

### Comparing `poppy-pop-0.8.3/poppy/pop/models/versions/poppy_pop_0001_initial_.py` & `poppy-pop-0.9.0/poppy/pop/models/versions/poppy_pop_0001_initial_.py`

 * *Files identical despite different names*

### Comparing `poppy-pop-0.8.3/poppy/pop/models/versions/poppy_pop_0002_version_num_.py` & `poppy-pop-0.9.0/poppy/pop/models/versions/poppy_pop_0002_version_num_.py`

 * *Files identical despite different names*

### Comparing `poppy-pop-0.8.3/poppy/pop/plugins.py` & `poppy-pop-0.9.0/poppy/pop/plugins.py`

 * *Files identical despite different names*

### Comparing `poppy-pop-0.8.3/poppy/pop/pop.py` & `poppy-pop-0.9.0/poppy/pop/pop.py`

 * *Files identical despite different names*

### Comparing `poppy-pop-0.8.3/poppy/pop/scripts/scripts.py` & `poppy-pop-0.9.0/poppy/pop/scripts/scripts.py`

 * *Files identical despite different names*

### Comparing `poppy-pop-0.8.3/poppy/pop/tasks.py` & `poppy-pop-0.9.0/poppy/pop/tasks.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,35 +14,36 @@
 from poppy.pop.plugins import Plugin
 from poppy.pop.migration import MigrateError
 from poppy.pop.tools import paths
 from poppy.core.conf import settings
 from poppy.core.logger import logger
 
 __all__ = [
-    "Execute",
-    "ExecuteCli",
-    "Makemigrations",
-    "Upgrade",
-    "Downgrade",
-    "ShowCurrent",
-    "CallAlembic",
-    "RunAdminWebServer",
+    'Execute',
+    'ExecuteCli',
+    'Makemigrations',
+    'Upgrade',
+    'Downgrade',
+    'DowngradeAll',
+    'ShowCurrent',
+    'CallAlembic',
+    'RunAdminWebServer',
 ]
 
 
 class DryRunTask(Task):
     def __init__(self):
         # init as usual but without related information on the database
         super().__init__()
 
         # force dry run
         DryRunner().activate()
 
 
-@DryRunTask.as_task(plugin_name="poppy.pop", name="execute")
+@DryRunTask.as_task(plugin_name='poppy.pop', name='execute')
 @Connector.if_connected(settings.MAIN_DATABASE)
 def Execute(self):
     """
     To execute a script on the POPPy database.
     """
     # get the database objects for the POPPy
     database = self.pipeline.db.get_database()
@@ -53,26 +54,26 @@
         database.scoped_session.close_all()
     except Exception as e:
         logger.error("Can't close sessions on sqlalchemy")
         logger.error(e)
         return
 
     # read the script
-    with open(self.pipeline.properties.script, "r") as f:
+    with open(self.pipeline.properties.script, 'r') as f:
         script = f.read()
 
     # execute the script
     try:
         database.engine.execute(script)
     except Exception as e:
         logger.error(e)
         return
 
 
-@DryRunTask.as_task(plugin_name="poppy.pop", name="execute_cli")
+@DryRunTask.as_task(plugin_name='poppy.pop', name='execute_cli')
 @Connector.if_connected(settings.MAIN_DATABASE)
 def ExecuteCli(self):
     """
     To execute a script on the POPPy database from the command line.
     """
     # get the database objects for the POPPy
     database = self.pipeline.db.get_database()
@@ -87,229 +88,270 @@
         return
 
     # execute the script if present or the command in argument
     if self.pipeline.properties.execute is None:
         script = self.pipeline.properties.input.read()
     else:
         script = self.pipeline.properties.execute
-    logger.debug("Running command(s):\n{0}".format(script))
+    logger.debug('Running command(s):\n{0}'.format(script))
     try:
         database.engine.execute(script)
     except Exception as e:
         logger.error(e)
         return
 
 
-@DryRunTask.as_task(plugin_name="poppy.pop", name="makemigrations")
+@DryRunTask.as_task(plugin_name='poppy.pop', name='makemigrations')
 def Makemigrations(task):
     """A task to automatically generate migrations
     'alembic revision --autogenerate' is used to generate migrations.
     You have to manually edit the migration after being generated, because
     alembic cannot detect changes of table/column name etc, or does not
     generate the schema creation. More info :
     http://alembic.zzzcomputing.com/en/latest/autogenerate.html#what-does-autog
     enerate-detect-and-what-does-it-not-detect
     """
     # get the plugin to use
     plugin = task.pipeline.properties.plugin
 
     # check that it is valid
     if plugin not in Plugin.manager:
-        raise MigrateError("{0} is not a valid registered plugin name".format(plugin))
+        raise MigrateError('{0} is not a valid registered plugin name'.format(plugin))
 
     database = task.pipeline.db.get_database()
     version_locations = list()
     for plugin_name in settings.PLUGINS:
         plug = Plugin.manager[plugin_name]
-        location = os.path.join(plug.module.__path__[0], "models", "versions")
+        location = os.path.join(plug.module.__path__[0], 'models', 'versions')
         if os.path.isdir(location):
             version_locations.append(location)
 
     cfg = Config()
 
-    cfg.set_main_option("version_locations", " ".join(version_locations))
-    cfg.set_main_option("script_location", paths.from_root("alembic"))
-    cfg.set_main_option("output_encoding", "utf-8")
+    cfg.set_main_option('version_locations', ' '.join(version_locations))
+    cfg.set_main_option('script_location', paths.from_root('alembic'))
+    cfg.set_main_option('output_encoding', 'utf-8')
 
     database.create_engine(admin=True)
     database.create_connection()
 
-    cfg.attributes["connection"] = database.db_connection
-    cfg.attributes["plugin"] = plugin
+    cfg.attributes['connection'] = database.db_connection
+    cfg.attributes['plugin'] = plugin
 
-    logger.info("Calling alembic revision")
+    logger.info('Calling alembic revision')
 
     # used to pass arguments to alembic revision command
     # http://alembic.zzzcomputing.com/en/latest/api/commands.html#alembic.command.revision
     args = dict()
     for arg in sys.argv[4:]:
         try:
             # Only parse keyword of the form (-)-key=val
-            if "=" in arg:
-                s = arg.split("=")
+            if '=' in arg:
+                s = arg.split('=')
             else:
                 logger.error(
-                    f"Input keyword {arg} can not be parsed and will be ignored, "
+                    f'Input keyword {arg} can not be parsed and will be ignored, '
                     "please call extra alembic keywords using '='!"
                 )
                 continue
 
             # Replace any hyphen "-" by underscore "_" in keyword argument name
             # (including "-" or "--" prefix)
-            s[0] = s[0].replace("-", "_")
+            s[0] = s[0].replace('-', '_')
 
             # Remove "_" or "__" prefix
-            if s[0].startswith("__"):
+            if s[0].startswith('__'):
                 args.update({s[0][2:]: s[1]})
-            elif s[0].startswith("_"):
+            elif s[0].startswith('_'):
                 args.update({s[0][1:]: s[1]})
         except IndexError:
-            logger.error(f"Unknown argument: {arg}, skipping!")
+            logger.error(f'Unknown argument: {arg}, skipping!')
 
     command.revision(
         cfg,
         autogenerate=True,
         version_path=os.path.join(
-            Plugin.manager[plugin].module.__path__[0], "models", "versions"
+            Plugin.manager[plugin].module.__path__[0], 'models', 'versions'
         ),
         **args,
     )
 
     # TODO have poppy.pop as dependency for any first migration of a plugin ?
 
 
-@DryRunTask.as_task(plugin_name="poppy.pop", name="upgrade")
+@DryRunTask.as_task(plugin_name='poppy.pop', name='upgrade')
 def Upgrade(task):
     """
     A task to do the migration of the POPPy database.
     """
     revision = task.pipeline.properties.revision
 
     database = task.pipeline.db.get_database()
     version_locations = list()
     for plugin_name in settings.PLUGINS:
         plug = Plugin.manager[plugin_name]
-        location = os.path.join(plug.module.__path__[0], "models", "versions")
+        location = os.path.join(plug.module.__path__[0], 'models', 'versions')
         if os.path.isdir(location):
             version_locations.append(location)
 
     cfg = Config()
 
-    cfg.set_main_option("version_locations", " ".join(version_locations))
-    cfg.set_main_option("script_location", paths.from_root("alembic"))
-    cfg.set_main_option("output_encoding", "utf-8")
+    cfg.set_main_option('version_locations', ' '.join(version_locations))
+    cfg.set_main_option('script_location', paths.from_root('alembic'))
+    cfg.set_main_option('output_encoding', 'utf-8')
 
     database.create_engine(admin=True)
     database.create_connection()
 
-    cfg.attributes["connection"] = database.db_connection
-    logger.info("Calling alembic")
+    cfg.attributes['connection'] = database.db_connection
+    logger.info('Calling alembic')
 
     command.upgrade(cfg, revision)
 
 
-@DryRunTask.as_task(plugin_name="poppy.pop", name="downgrade")
+@DryRunTask.as_task(plugin_name='poppy.pop', name='downgrade')
 def Downgrade(task):
     """
     A task to do the migration of the POPPy database.
     """
     # get the plugin to use
     revision = task.pipeline.properties.revision
 
     database = task.pipeline.db.get_database()
     version_locations = list()
     for plugin_name in settings.PLUGINS:
         plug = Plugin.manager[plugin_name]
-        location = os.path.join(plug.module.__path__[0], "models", "versions")
+        location = os.path.join(plug.module.__path__[0], 'models', 'versions')
         if os.path.isdir(location):
             version_locations.append(location)
 
     cfg = Config()
 
-    cfg.set_main_option("version_locations", " ".join(version_locations))
-    cfg.set_main_option("script_location", paths.from_root("alembic"))
-    cfg.set_main_option("output_encoding", "utf-8")
+    cfg.set_main_option('version_locations', ' '.join(version_locations))
+    cfg.set_main_option('script_location', paths.from_root('alembic'))
+    cfg.set_main_option('output_encoding', 'utf-8')
 
     database.create_engine(admin=True)
     database.create_connection()
 
-    cfg.attributes["connection"] = database.db_connection
+    cfg.attributes['connection'] = database.db_connection
 
-    logger.info("Calling alembic")
+    logger.info('Calling alembic')
 
     command.downgrade(cfg, revision)
 
 
-@DryRunTask.as_task(plugin_name="poppy.pop", name="show_current")
+@DryRunTask.as_task(plugin_name='poppy.pop', name='downgrade_all')
+def DowngradeAll(task):
+    """
+    A task to do the migration of the POPPy database.
+    """
+    database = task.pipeline.db.get_database()
+    version_locations = list()
+    for plugin_name in settings.PLUGINS:
+        plug = Plugin.manager[plugin_name]
+        location = os.path.join(plug.module.__path__[0], 'models', 'versions')
+        if os.path.isdir(location):
+            version_locations.append(location)
+
+    cfg = Config()
+
+    cfg.set_main_option('version_locations', ' '.join(version_locations))
+    cfg.set_main_option('script_location', paths.from_root('alembic'))
+    cfg.set_main_option('output_encoding', 'utf-8')
+
+    database.create_engine(admin=True)
+    database.create_connection()
+
+    cfg.attributes['connection'] = database.db_connection
+
+    logger.info('Calling alembic')
+
+    # Define a maximum number of possible downgrade migrations
+    # (To avoid infinite loop)
+    max_rev_iter = 10000
+    for i in range(max_rev_iter):
+        revision = '-1'
+        try:
+            command.downgrade(cfg, revision)
+        except alembic.script.revision.RevisionError:
+            break
+        except alembic.util.exc.CommandError as e:
+            if str(e) == "Relative revision -1 didn't produce 1 migrations":
+                break
+            else:
+                raise e
+
+@DryRunTask.as_task(plugin_name='poppy.pop', name='show_current')
 def ShowCurrent(task):
     """
     Show the status of the current revision.
     """
 
     database = task.pipeline.db.get_database()
     version_locations = list()
     for plugin_name in settings.PLUGINS:
         plug = Plugin.manager[plugin_name]
-        location = os.path.join(plug.module.__path__[0], "models", "versions")
+        location = os.path.join(plug.module.__path__[0], 'models', 'versions')
         if os.path.isdir(location):
             version_locations.append(location)
 
     cfg = Config()
 
-    cfg.set_main_option("version_locations", " ".join(version_locations))
-    cfg.set_main_option("script_location", paths.from_root("alembic"))
-    cfg.set_main_option("output_encoding", "utf-8")
+    cfg.set_main_option('version_locations', ' '.join(version_locations))
+    cfg.set_main_option('script_location', paths.from_root('alembic'))
+    cfg.set_main_option('output_encoding', 'utf-8')
 
     database.create_engine(admin=True)
     database.create_connection()
 
-    cfg.attributes["connection"] = database.db_connection
+    cfg.attributes['connection'] = database.db_connection
 
-    logger.info("Calling alembic")
+    logger.info('Calling alembic')
 
     command.current(cfg)
 
 
-@DryRunTask.as_task(plugin_name="poppy.pop", name="call_alembic")
+@DryRunTask.as_task(plugin_name='poppy.pop', name='call_alembic')
 def CallAlembic(task):
     """
     Call alembic directly
     """
     import tempfile
 
     TEMP_DIR = tempfile.gettempdir()
 
     version_locations = list()
     for plugin_name in settings.PLUGINS:
         plug = Plugin.manager[plugin_name]
-        location = os.path.join(plug.module.__path__[0], "models", "versions")
+        location = os.path.join(plug.module.__path__[0], 'models', 'versions')
         if os.path.isdir(location):
             version_locations.append(location)
 
-    with open(os.path.join(TEMP_DIR, "alembic.ini"), "w") as f:
+    with open(os.path.join(TEMP_DIR, 'alembic.ini'), 'w') as f:
         f.truncate()
-        f.write("[alembic]\n")
+        f.write('[alembic]\n')
         f.write(f'script_location = {paths.from_root("alembic")}\n')
         f.write(f'version_locations = {" ".join(version_locations)}\n')
         f.write(
-            f"sqlalchemy.url = {task.pipeline.db.get_database().generate_url_admin()}\n"
+            f'sqlalchemy.url = {task.pipeline.db.get_database().generate_url_admin()}\n'
         )
-        f.write("output_encoding = utf-8\n")
+        f.write('output_encoding = utf-8\n')
 
     alembicArgs = [
-        "-c",
-        os.path.join(TEMP_DIR, "alembic.ini"),
+        '-c',
+        os.path.join(TEMP_DIR, 'alembic.ini'),
         sys.argv[3],
         *sys.argv[4:],
     ]
 
     alembic.config.main(argv=alembicArgs)
 
 
-@Task.as_task(plugin_name="poppy.pop", name="run_admin_web_server")
+@Task.as_task(plugin_name='poppy.pop', name='run_admin_web_server')
 def RunAdminWebServer():
     from flask import Flask
     from flask_admin import Admin
     from flask_admin.contrib.sqla import ModelView
     from poppy.pop.models.job import JobLog
 
     # get the meb connector and get the database
@@ -321,17 +363,16 @@
 
     # get a database session
     session = database.session_factory()
 
     app = Flask(__name__)
 
     # set optional bootswatch theme
-    app.config["FLASK_ADMIN_SWATCH"] = "slate"
+    app.config['FLASK_ADMIN_SWATCH'] = 'slate'
 
     # Flask and Flask-SQLAlchemy initialization here
-    admin = Admin(app, name="Poppy", template_mode="bootstrap3")
+    admin = Admin(app, name='Poppy', template_mode='bootstrap3')
 
     # add a model to demonstrate the usage of the admin web page
     admin.add_view(ModelView(JobLog, session))
 
-    app.run(host="0.0.0.0")
-
+    app.run(host='0.0.0.0')
```

### Comparing `poppy-pop-0.8.3/poppy/pop/tests.py` & `poppy-pop-0.9.0/poppy/pop/tests.py`

 * *Files identical despite different names*

### Comparing `poppy-pop-0.8.3/poppy/pop/tools.py` & `poppy-pop-0.9.0/poppy/pop/tools.py`

 * *Files identical despite different names*

### Comparing `poppy-pop-0.8.3/pyproject.toml` & `poppy-pop-0.9.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 skip-string-normalization = true
 line-length = 79
 include = "\\.pyi?$"
 exclude = "/(\n    \\.git\n  | \\.hg\n  | \\.mypy_cache\n  | \\.tox\n  | \\.venv\n  | _build\n  | buck-out\n  | build\n  | dist\n)/\n"
 
 [tool.poetry]
 name = "poppy-pop"
-version = "0.8.3"
+version = "0.9.0"
 readme = "README.md"
 license = "CeCILL-C"
 repository = "https://gitlab.obspm.fr/POPPy/POP"
 description = "POPPY Operation Plugin (POP)"
 authors = [ "Xavier Bonnin <xavier.bonnin@obspm.fr>", "ROC Team <roc.support@sympa.obspm.fr>",]
 exclude = [ "bump_version.py",]
 [[tool.poetry.packages]]
@@ -23,11 +23,12 @@
 [tool.poetry.dependencies]
 python = ">=3.8,<4"
 poppy-core = {version = ">=0.10"}
 
 [tool.poetry.dev-dependencies]
 pytest = {version="^5.2", optional=true}
 pytest-cov = {version="^2.10.1", optional=true}
+pytest-timeout = {version="^1.4", optional=true}
 pre-commit = "^2.8"
 
 [tool.poetry.scripts]
 pop = "poppy.pop.scripts:main"
```

### Comparing `poppy-pop-0.8.3/setup.py` & `poppy-pop-0.9.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ['poppy-core>=0.10']
 
 entry_points = \
 {'console_scripts': ['pop = poppy.pop.scripts:main']}
 
 setup_kwargs = {
     'name': 'poppy-pop',
-    'version': '0.8.3',
+    'version': '0.9.0',
     'description': 'POPPY Operation Plugin (POP)',
     'long_description': 'poppy.pop\n=========\n\n[![pipeline status](https://gitlab.obspm.fr/POPPY/POP/badges/develop/pipeline.svg)](https://gitlab.obspm.fr/POPPY/POP/pipelines)\n\n\nIntroduction\n------------\n\nThis directory contains the source code of the POPPY Operation Plugin (POP), the main plugin to be used with the POPPY framework.\n\nSee "POPPY User Manual" for more details.\n\nLicense\n-------\nPOPPY is under GPL license.\n\nAcknowledgement\n-----------\nPOPPY is project developed by the RPW Operations Centre (ROC) team based at LESIA (Meudon, France).\nThe ROC is funded by the Centre National d\'Etudes Spatiale (CNES) in the framework of the European Space Agency (ESA) Solar Orbiter mission.\n\nContact\n-------\nxavier.bonnin@obspm.fr (project manager)\nsonny.lion@obspm.fr (software designer)\nquynh-nhu.nguyen@obspm.fr (software developer)\n\ncontributors\n------------\nGregoire Duvauchelle (software developer)\nManual Duarte (software designer)\n',
     'author': 'Xavier Bonnin',
     'author_email': 'xavier.bonnin@obspm.fr',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://gitlab.obspm.fr/POPPy/POP',
```

### Comparing `poppy-pop-0.8.3/PKG-INFO` & `poppy-pop-0.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poppy-pop
-Version: 0.8.3
+Version: 0.9.0
 Summary: POPPY Operation Plugin (POP)
 Home-page: https://gitlab.obspm.fr/POPPy/POP
 License: CECILL-C
 Author: Xavier Bonnin
 Author-email: xavier.bonnin@obspm.fr
 Requires-Python: >=3.8,<4
 Classifier: License :: CeCILL-C Free Software License Agreement (CECILL-C)
```

