# Comparing `tmp/riogisoffline-0.0.26.tar.gz` & `tmp/riogisoffline-0.0.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "riogisoffline-0.0.26.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "riogisoffline-0.0.28.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `riogisoffline-0.0.26.tar` & `riogisoffline-0.0.28.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      717 2024-05-21 07:43:56.562218 riogisoffline-0.0.26/pyproject.toml
--rw-r--r--   0        0        0     1071 2024-05-21 07:43:56.562218 riogisoffline-0.0.26/riogisoffline/LICENSE
--rw-r--r--   0        0        0     7264 2024-05-21 07:43:56.562218 riogisoffline-0.0.26/riogisoffline/Makefile
--rw-r--r--   0        0        0      261 2024-05-21 07:43:56.562218 riogisoffline-0.0.26/riogisoffline/README.md
--rw-r--r--   0        0        0     2239 2024-05-21 07:43:56.562218 riogisoffline-0.0.26/riogisoffline/__init__.py
--rw-r--r--   0        0        0      158 2024-05-21 07:43:56.562218 riogisoffline-0.0.26/riogisoffline/compile.bat
--rw-r--r--   0        0        0     2810 2024-05-21 07:43:56.562218 riogisoffline-0.0.26/riogisoffline/dialog/riogis_dialog_settings.ui
--rw-r--r--   0        0        0     6345 2024-05-21 07:43:56.562218 riogisoffline-0.0.26/riogisoffline/dialog/riogis_dockwidget.ui
--rw-r--r--   0        0        0    30219 2024-05-21 07:43:56.562218 riogisoffline-0.0.26/riogisoffline/icon.png
--rw-r--r--   0        0        0     1505 2024-05-21 07:43:56.562218 riogisoffline-0.0.26/riogisoffline/metadata.txt
--rw-r--r--   0        0        0     1723 2024-05-21 07:43:56.562218 riogisoffline-0.0.26/riogisoffline/pb_tool.cfg
--rw-r--r--   0        0        0      195 2024-05-21 07:43:56.562218 riogisoffline-0.0.26/riogisoffline/plugin/__init__.py
--rw-r--r--   0        0        0     1283 2024-05-21 07:43:56.562218 riogisoffline-0.0.26/riogisoffline/plugin/azure_blob_storage_connection.py
--rw-r--r--   0        0        0      424 2024-05-21 07:43:56.562218 riogisoffline-0.0.26/riogisoffline/plugin/dependency_installer.py
--rw-r--r--   0        0        0    17046 2024-05-21 07:43:56.562218 riogisoffline-0.0.26/riogisoffline/plugin/refresh_map.py
--rw-r--r--   0        0        0   126345 2024-05-21 07:43:56.562218 riogisoffline-0.0.26/riogisoffline/plugin/resources.py
--rw-r--r--   0        0        0    14047 2024-05-21 07:43:56.562218 riogisoffline-0.0.26/riogisoffline/plugin/riogis.py
--rw-r--r--   0        0        0     1313 2024-05-21 07:43:56.562218 riogisoffline-0.0.26/riogisoffline/plugin/riogis_dockedwidget.py
--rw-r--r--   0        0        0     1310 2024-05-21 07:43:56.562218 riogisoffline-0.0.26/riogisoffline/plugin/settings_dialog.py
--rw-r--r--   0        0        0     7700 2024-05-21 07:43:56.562218 riogisoffline-0.0.26/riogisoffline/plugin/syncronizer.py
--rw-r--r--   0        0        0     2436 2024-05-21 07:43:56.562218 riogisoffline-0.0.26/riogisoffline/plugin/user_settings_generator.py
--rw-r--r--   0        0        0     2402 2024-05-21 07:43:56.562218 riogisoffline-0.0.26/riogisoffline/plugin/utils.py
--rw-r--r--   0        0        0      947 2024-05-21 07:43:56.562218 riogisoffline-0.0.26/riogisoffline/plugin/worker.py
--rw-r--r--   0        0        0     3559 2024-05-21 07:43:56.562218 riogisoffline-0.0.26/riogisoffline/plugin_upload.py
--rw-r--r--   0        0        0     8798 2024-05-21 07:43:56.562218 riogisoffline-0.0.26/riogisoffline/pylintrc
--rw-r--r--   0        0        0       18 2024-05-21 07:43:56.562218 riogisoffline-0.0.26/riogisoffline/requirements.txt
--rw-r--r--   0        0        0      102 2024-05-21 07:43:56.562218 riogisoffline-0.0.26/riogisoffline/resources.qrc
--rw-r--r--   0        0        0     2740 2024-05-21 07:43:56.562218 riogisoffline-0.0.26/riogisoffline/settings.json
--rw-r--r--   0        0        0      821 1970-01-01 00:00:00.000000 riogisoffline-0.0.26/PKG-INFO
+-rw-r--r--   0        0        0      717 2024-05-28 08:14:16.832396 riogisoffline-0.0.28/pyproject.toml
+-rw-r--r--   0        0        0     1071 2024-05-28 08:14:16.836396 riogisoffline-0.0.28/riogisoffline/LICENSE
+-rw-r--r--   0        0        0     7264 2024-05-28 08:14:16.836396 riogisoffline-0.0.28/riogisoffline/Makefile
+-rw-r--r--   0        0        0      261 2024-05-28 08:14:16.836396 riogisoffline-0.0.28/riogisoffline/README.md
+-rw-r--r--   0        0        0     2239 2024-05-28 08:14:16.836396 riogisoffline-0.0.28/riogisoffline/__init__.py
+-rw-r--r--   0        0        0      158 2024-05-28 08:14:16.836396 riogisoffline-0.0.28/riogisoffline/compile.bat
+-rw-r--r--   0        0        0     2810 2024-05-28 08:14:16.836396 riogisoffline-0.0.28/riogisoffline/dialog/riogis_dialog_settings.ui
+-rw-r--r--   0        0        0     6143 2024-05-28 08:14:16.836396 riogisoffline-0.0.28/riogisoffline/dialog/riogis_dockwidget.ui
+-rw-r--r--   0        0        0    30219 2024-05-28 08:14:16.836396 riogisoffline-0.0.28/riogisoffline/icon.png
+-rw-r--r--   0        0        0     1505 2024-05-28 08:14:16.836396 riogisoffline-0.0.28/riogisoffline/metadata.txt
+-rw-r--r--   0        0        0     1723 2024-05-28 08:14:16.836396 riogisoffline-0.0.28/riogisoffline/pb_tool.cfg
+-rw-r--r--   0        0        0      195 2024-05-28 08:14:16.836396 riogisoffline-0.0.28/riogisoffline/plugin/__init__.py
+-rw-r--r--   0        0        0     1283 2024-05-28 08:14:16.836396 riogisoffline-0.0.28/riogisoffline/plugin/azure_blob_storage_connection.py
+-rw-r--r--   0        0        0      424 2024-05-28 08:14:16.836396 riogisoffline-0.0.28/riogisoffline/plugin/dependency_installer.py
+-rw-r--r--   0        0        0    17046 2024-05-28 08:14:16.836396 riogisoffline-0.0.28/riogisoffline/plugin/refresh_map.py
+-rw-r--r--   0        0        0   126345 2024-05-28 08:14:16.836396 riogisoffline-0.0.28/riogisoffline/plugin/resources.py
+-rw-r--r--   0        0        0    14047 2024-05-28 08:14:16.836396 riogisoffline-0.0.28/riogisoffline/plugin/riogis.py
+-rw-r--r--   0        0        0     1313 2024-05-28 08:14:16.836396 riogisoffline-0.0.28/riogisoffline/plugin/riogis_dockedwidget.py
+-rw-r--r--   0        0        0     1310 2024-05-28 08:14:16.836396 riogisoffline-0.0.28/riogisoffline/plugin/settings_dialog.py
+-rw-r--r--   0        0        0     7700 2024-05-28 08:14:16.836396 riogisoffline-0.0.28/riogisoffline/plugin/syncronizer.py
+-rw-r--r--   0        0        0     2436 2024-05-28 08:14:16.836396 riogisoffline-0.0.28/riogisoffline/plugin/user_settings_generator.py
+-rw-r--r--   0        0        0     2635 2024-05-28 08:14:16.836396 riogisoffline-0.0.28/riogisoffline/plugin/utils.py
+-rw-r--r--   0        0        0      947 2024-05-28 08:14:16.836396 riogisoffline-0.0.28/riogisoffline/plugin/worker.py
+-rw-r--r--   0        0        0     3559 2024-05-28 08:14:16.836396 riogisoffline-0.0.28/riogisoffline/plugin_upload.py
+-rw-r--r--   0        0        0     8798 2024-05-28 08:14:16.836396 riogisoffline-0.0.28/riogisoffline/pylintrc
+-rw-r--r--   0        0        0       18 2024-05-28 08:14:16.836396 riogisoffline-0.0.28/riogisoffline/requirements.txt
+-rw-r--r--   0        0        0      102 2024-05-28 08:14:16.836396 riogisoffline-0.0.28/riogisoffline/resources.qrc
+-rw-r--r--   0        0        0     2740 2024-05-28 08:14:16.836396 riogisoffline-0.0.28/riogisoffline/settings.json
+-rw-r--r--   0        0        0      821 1970-01-01 00:00:00.000000 riogisoffline-0.0.28/PKG-INFO
```

### Comparing `riogisoffline-0.0.26/pyproject.toml` & `riogisoffline-0.0.28/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "riogisoffline"
-version = "0.0.26"
+version = "0.0.28"
 description = "This Exports attributes of a given feature to a Wincan consumable text file."
 authors = [
   { name = "Vann- og avløpsetaten Oslo kommune", email = "gis@vav.oslo.kommune.no" },
 ]
 license = { file = "riogisoffline/LICENSE" }
 readme = "riogisoffline/README.md"
 classifiers = [
```

### Comparing `riogisoffline-0.0.26/riogisoffline/LICENSE` & `riogisoffline-0.0.28/riogisoffline/LICENSE`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.26/riogisoffline/Makefile` & `riogisoffline-0.0.28/riogisoffline/Makefile`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.26/riogisoffline/__init__.py` & `riogisoffline-0.0.28/riogisoffline/__init__.py`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.26/riogisoffline/dialog/riogis_dialog_settings.ui` & `riogisoffline-0.0.28/riogisoffline/dialog/riogis_dialog_settings.ui`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.26/riogisoffline/dialog/riogis_dockwidget.ui` & `riogisoffline-0.0.28/riogisoffline/dialog/riogis_dockwidget.ui`

 * *Files 3% similar despite different names*

#### Comparing `riogisoffline-0.0.26/riogisoffline/dialog/riogis_dockwidget.ui` & `riogisoffline-0.0.28/riogisoffline/dialog/riogis_dockwidget.ui`

```diff
@@ -1,11 +1,11 @@
 <?xml version="1.0" encoding="utf-8"?>
 <ui version="4.0">
   <class>RioGIS2</class>
-  <widget class="QgsDockWidget" name="RioGIS2">
+  <widget class="QDockWidget" name="RioGIS2">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
         <width>296</width>
         <height>735</height>
       </rect>
@@ -189,18 +189,10 @@
               <string>Velg ledning i kart:</string>
             </property>
           </widget>
         </item>
       </layout>
     </widget>
   </widget>
-  <customwidgets>
-    <customwidget>
-      <class>QgsDockWidget</class>
-      <extends>QDockWidget</extends>
-      <header>qgsdockwidget.h</header>
-      <container>1</container>
-    </customwidget>
-  </customwidgets>
   <resources/>
   <connections/>
 </ui>
```

### Comparing `riogisoffline-0.0.26/riogisoffline/icon.png` & `riogisoffline-0.0.28/riogisoffline/icon.png`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.26/riogisoffline/metadata.txt` & `riogisoffline-0.0.28/riogisoffline/metadata.txt`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.26/riogisoffline/pb_tool.cfg` & `riogisoffline-0.0.28/riogisoffline/pb_tool.cfg`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.26/riogisoffline/plugin/azure_blob_storage_connection.py` & `riogisoffline-0.0.28/riogisoffline/plugin/azure_blob_storage_connection.py`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.26/riogisoffline/plugin/refresh_map.py` & `riogisoffline-0.0.28/riogisoffline/plugin/refresh_map.py`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.26/riogisoffline/plugin/resources.py` & `riogisoffline-0.0.28/riogisoffline/plugin/resources.py`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.26/riogisoffline/plugin/riogis.py` & `riogisoffline-0.0.28/riogisoffline/plugin/riogis.py`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.26/riogisoffline/plugin/riogis_dockedwidget.py` & `riogisoffline-0.0.28/riogisoffline/plugin/riogis_dockedwidget.py`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.26/riogisoffline/plugin/settings_dialog.py` & `riogisoffline-0.0.28/riogisoffline/plugin/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.26/riogisoffline/plugin/syncronizer.py` & `riogisoffline-0.0.28/riogisoffline/plugin/syncronizer.py`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.26/riogisoffline/plugin/user_settings_generator.py` & `riogisoffline-0.0.28/riogisoffline/plugin/user_settings_generator.py`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.26/riogisoffline/plugin/utils.py` & `riogisoffline-0.0.28/riogisoffline/plugin/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 
 default_message_duration = 3
 
 def get_plugin_dir(path_to_join=None):
 
     plugin_dir = os.getenv('PLUGIN_DIR')
 
+    if not plugin_dir:
+        # get parent of current dir if PLUGIN_DIR is not set
+        plugin_dir = os.path.dirname(os.path.dirname(__file__))
+
     if not path_to_join:
         return plugin_dir
 
     return os.path.join(plugin_dir, path_to_join)
 
 def load_json(path):
 
@@ -65,15 +69,16 @@
     """
 
     iface.messageBar().pushMessage(
             "", message, level=Qgis.Success, duration=message_duration
        )
 
 def get_user_settings_path():
-    return get_plugin_dir("bruker_settings.json")
+    # bruker_settings.json is placed in python-dir of qgis default profile
+    return get_plugin_dir("../../../bruker_settings.json")
 
 def get_settings_path():
     return get_plugin_dir("settings.json")
 
 def get_db_name():
     return "oslo_offline.db"
```

### Comparing `riogisoffline-0.0.26/riogisoffline/plugin/worker.py` & `riogisoffline-0.0.28/riogisoffline/plugin/worker.py`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.26/riogisoffline/plugin_upload.py` & `riogisoffline-0.0.28/riogisoffline/plugin_upload.py`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.26/riogisoffline/pylintrc` & `riogisoffline-0.0.28/riogisoffline/pylintrc`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.26/riogisoffline/settings.json` & `riogisoffline-0.0.28/riogisoffline/settings.json`

 * *Files identical despite different names*

### Comparing `riogisoffline-0.0.26/PKG-INFO` & `riogisoffline-0.0.28/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: riogisoffline
-Version: 0.0.26
+Version: 0.0.28
 Summary: This Exports attributes of a given feature to a Wincan consumable text file.
 Author-email: Vann- og avløpsetaten Oslo kommune <gis@vav.oslo.kommune.no>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

