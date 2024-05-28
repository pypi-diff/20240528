# Comparing `tmp/netbox_reorder_rack-1.1.0.tar.gz` & `tmp/netbox_reorder_rack-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_reorder_rack-1.1.0.tar", last modified: Wed May  8 14:20:42 2024, max compression
+gzip compressed data, was "netbox_reorder_rack-1.1.1.tar", last modified: Tue May 28 14:52:42 2024, max compression
```

## Comparing `netbox_reorder_rack-1.1.0.tar` & `netbox_reorder_rack-1.1.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:20:42.888701 netbox_reorder_rack-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-08 14:20:38.000000 netbox_reorder_rack-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-08 14:20:38.000000 netbox_reorder_rack-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-05-08 14:20:42.888701 netbox_reorder_rack-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-08 14:20:38.000000 netbox_reorder_rack-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:20:42.884701 netbox_reorder_rack-1.1.0/netbox_reorder_rack/
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-08 14:20:38.000000 netbox_reorder_rack-1.1.0/netbox_reorder_rack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:20:42.884701 netbox_reorder_rack-1.1.0/netbox_reorder_rack/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 14:20:38.000000 netbox_reorder_rack-1.1.0/netbox_reorder_rack/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-08 14:20:38.000000 netbox_reorder_rack-1.1.0/netbox_reorder_rack/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-08 14:20:38.000000 netbox_reorder_rack-1.1.0/netbox_reorder_rack/api/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:20:42.880701 netbox_reorder_rack-1.1.0/netbox_reorder_rack/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:20:42.880701 netbox_reorder_rack-1.1.0/netbox_reorder_rack/static/netbox_reorder_rack/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:20:42.884701 netbox_reorder_rack-1.1.0/netbox_reorder_rack/static/netbox_reorder_rack/css/
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-08 14:20:38.000000 netbox_reorder_rack-1.1.0/netbox_reorder_rack/static/netbox_reorder_rack/css/rack.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:20:42.884701 netbox_reorder_rack-1.1.0/netbox_reorder_rack/static/netbox_reorder_rack/js/
--rw-r--r--   0 runner    (1001) docker     (127)    83425 2024-05-08 14:20:38.000000 netbox_reorder_rack-1.1.0/netbox_reorder_rack/static/netbox_reorder_rack/js/rack.js
--rw-r--r--   0 runner    (1001) docker     (127)   102233 2024-05-08 14:20:38.000000 netbox_reorder_rack-1.1.0/netbox_reorder_rack/static/netbox_reorder_rack/js/rack.js.map
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-08 14:20:38.000000 netbox_reorder_rack-1.1.0/netbox_reorder_rack/template_content.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:20:42.884701 netbox_reorder_rack-1.1.0/netbox_reorder_rack/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:20:42.884701 netbox_reorder_rack-1.1.0/netbox_reorder_rack/templates/netbox_reorder_rack/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:20:42.888701 netbox_reorder_rack-1.1.0/netbox_reorder_rack/templates/netbox_reorder_rack/inc/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-08 14:20:38.000000 netbox_reorder_rack-1.1.0/netbox_reorder_rack/templates/netbox_reorder_rack/inc/rack_button.html
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-08 14:20:38.000000 netbox_reorder_rack-1.1.0/netbox_reorder_rack/templates/netbox_reorder_rack/inc/rack_elevation.html
--rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-05-08 14:20:38.000000 netbox_reorder_rack-1.1.0/netbox_reorder_rack/templates/netbox_reorder_rack/rack.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:20:42.888701 netbox_reorder_rack-1.1.0/netbox_reorder_rack/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 14:20:38.000000 netbox_reorder_rack-1.1.0/netbox_reorder_rack/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-08 14:20:38.000000 netbox_reorder_rack-1.1.0/netbox_reorder_rack/templatetags/rack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:20:42.888701 netbox_reorder_rack-1.1.0/netbox_reorder_rack/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 14:20:38.000000 netbox_reorder_rack-1.1.0/netbox_reorder_rack/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6490 2024-05-08 14:20:38.000000 netbox_reorder_rack-1.1.0/netbox_reorder_rack/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-08 14:20:38.000000 netbox_reorder_rack-1.1.0/netbox_reorder_rack/tests/test_view.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-08 14:20:38.000000 netbox_reorder_rack-1.1.0/netbox_reorder_rack/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-08 14:20:38.000000 netbox_reorder_rack-1.1.0/netbox_reorder_rack/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:20:42.888701 netbox_reorder_rack-1.1.0/netbox_reorder_rack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-05-08 14:20:42.000000 netbox_reorder_rack-1.1.0/netbox_reorder_rack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-08 14:20:42.000000 netbox_reorder_rack-1.1.0/netbox_reorder_rack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 14:20:42.000000 netbox_reorder_rack-1.1.0/netbox_reorder_rack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 14:20:42.000000 netbox_reorder_rack-1.1.0/netbox_reorder_rack.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-08 14:20:42.000000 netbox_reorder_rack-1.1.0/netbox_reorder_rack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 14:20:42.888701 netbox_reorder_rack-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-08 14:20:38.000000 netbox_reorder_rack-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:52:42.220277 netbox_reorder_rack-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-28 14:52:32.000000 netbox_reorder_rack-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-28 14:52:32.000000 netbox_reorder_rack-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-05-28 14:52:42.220277 netbox_reorder_rack-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-05-28 14:52:32.000000 netbox_reorder_rack-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:52:42.216277 netbox_reorder_rack-1.1.1/netbox_reorder_rack/
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-28 14:52:32.000000 netbox_reorder_rack-1.1.1/netbox_reorder_rack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:52:42.216277 netbox_reorder_rack-1.1.1/netbox_reorder_rack/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 14:52:32.000000 netbox_reorder_rack-1.1.1/netbox_reorder_rack/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-28 14:52:32.000000 netbox_reorder_rack-1.1.1/netbox_reorder_rack/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-28 14:52:32.000000 netbox_reorder_rack-1.1.1/netbox_reorder_rack/api/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:52:42.212277 netbox_reorder_rack-1.1.1/netbox_reorder_rack/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:52:42.212277 netbox_reorder_rack-1.1.1/netbox_reorder_rack/static/netbox_reorder_rack/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:52:42.216277 netbox_reorder_rack-1.1.1/netbox_reorder_rack/static/netbox_reorder_rack/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-28 14:52:32.000000 netbox_reorder_rack-1.1.1/netbox_reorder_rack/static/netbox_reorder_rack/css/rack.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:52:42.216277 netbox_reorder_rack-1.1.1/netbox_reorder_rack/static/netbox_reorder_rack/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    83425 2024-05-28 14:52:32.000000 netbox_reorder_rack-1.1.1/netbox_reorder_rack/static/netbox_reorder_rack/js/rack.js
+-rw-r--r--   0 runner    (1001) docker     (127)   102233 2024-05-28 14:52:32.000000 netbox_reorder_rack-1.1.1/netbox_reorder_rack/static/netbox_reorder_rack/js/rack.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-28 14:52:32.000000 netbox_reorder_rack-1.1.1/netbox_reorder_rack/template_content.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:52:42.212277 netbox_reorder_rack-1.1.1/netbox_reorder_rack/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:52:42.216277 netbox_reorder_rack-1.1.1/netbox_reorder_rack/templates/netbox_reorder_rack/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:52:42.216277 netbox_reorder_rack-1.1.1/netbox_reorder_rack/templates/netbox_reorder_rack/inc/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-28 14:52:32.000000 netbox_reorder_rack-1.1.1/netbox_reorder_rack/templates/netbox_reorder_rack/inc/rack_button.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-28 14:52:32.000000 netbox_reorder_rack-1.1.1/netbox_reorder_rack/templates/netbox_reorder_rack/inc/rack_elevation.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-05-28 14:52:32.000000 netbox_reorder_rack-1.1.1/netbox_reorder_rack/templates/netbox_reorder_rack/rack.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:52:42.216277 netbox_reorder_rack-1.1.1/netbox_reorder_rack/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 14:52:32.000000 netbox_reorder_rack-1.1.1/netbox_reorder_rack/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-28 14:52:32.000000 netbox_reorder_rack-1.1.1/netbox_reorder_rack/templatetags/rack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:52:42.216277 netbox_reorder_rack-1.1.1/netbox_reorder_rack/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 14:52:32.000000 netbox_reorder_rack-1.1.1/netbox_reorder_rack/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6440 2024-05-28 14:52:32.000000 netbox_reorder_rack-1.1.1/netbox_reorder_rack/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-28 14:52:32.000000 netbox_reorder_rack-1.1.1/netbox_reorder_rack/tests/test_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-28 14:52:32.000000 netbox_reorder_rack-1.1.1/netbox_reorder_rack/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-28 14:52:32.000000 netbox_reorder_rack-1.1.1/netbox_reorder_rack/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:52:42.216277 netbox_reorder_rack-1.1.1/netbox_reorder_rack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-05-28 14:52:42.000000 netbox_reorder_rack-1.1.1/netbox_reorder_rack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-28 14:52:42.000000 netbox_reorder_rack-1.1.1/netbox_reorder_rack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 14:52:42.000000 netbox_reorder_rack-1.1.1/netbox_reorder_rack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 14:52:42.000000 netbox_reorder_rack-1.1.1/netbox_reorder_rack.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-28 14:52:42.000000 netbox_reorder_rack-1.1.1/netbox_reorder_rack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 14:52:42.220277 netbox_reorder_rack-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-28 14:52:32.000000 netbox_reorder_rack-1.1.1/setup.py
```

### Comparing `netbox_reorder_rack-1.1.0/LICENSE` & `netbox_reorder_rack-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_reorder_rack-1.1.0/PKG-INFO` & `netbox_reorder_rack-1.1.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,19 @@
-Metadata-Version: 2.1
-Name: netbox_reorder_rack
-Version: 1.1.0
-Summary: NetBox plugin to reorder rack layouts.
-Home-page: https://github.com/minitriga/netbox-reorder-rack/
-Author: Alex Gittings
-Author-email: agitting96@gmail.com
-Project-URL: Bug Tracker, https://github.com/minitriga/netbox-reorder-rack/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Framework :: Django
-Description-Content-Type: text/markdown
-License-File: LICENSE
+<p align="center"><img src="docs/img/reorder-rack.svg"></p>
 
-# Netbox Reorder Rack Plugin
+<h1 align="center">Netbox Reorder Rack Plugin</h1>
 
 ![Version](https://img.shields.io/pypi/v/netbox-reorder-rack) ![Downloads](https://img.shields.io/pypi/dm/netbox-reorder-rack)
 
 Allow the ability to reorder rack units in NetBox using a drag and drop interface.
 
 ![Reorder Rack](docs/img/netbox-reorder-rack.gif)
 
+> If there are any issues feel free to create an [Issue](https://github.com/minitriga/netbox-reorder-rack/issues) or feel free to contact me directly on Slack in the [NetDev](https://netdev.chat/) community.
+
 ## Installation
 
 **_NOTE:_** For docker please see: [Docker install](https://github.com/netbox-community/netbox-docker/wiki/Using-Netbox-Plugins)
 
 The plugin is available as a Python package and can be installed with pip.
 
 Run the following commands to install the required package after activating the virtual environment:
@@ -55,15 +45,23 @@
 
 
 ## Compatibility Matrix
 
 | netbox version | plugin version |
 | -------------- | ----------------------------- |
 | >= 4.0.0       | >= v1.1.0                     |
-| <= 4.0.0       | = v1.0.0                     |
+| <= 4.0.0       | = v1.0.0                      |
+
+## Dependencies
+Python:
+  - None
+
+Javascript:
+  - Gridstack (Currently running same versions as Netbox)
+  - Bootsrap (Currently running same versions as Netbox)
 
 ### Update
 
 To update the plugin, you need to update the package and restart NetBox.
 
 ```shell
 source /opt/netbox/venv/bin/activate
```

### Comparing `netbox_reorder_rack-1.1.0/netbox_reorder_rack/api/views.py` & `netbox_reorder_rack-1.1.1/netbox_reorder_rack/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox_reorder_rack-1.1.0/netbox_reorder_rack/static/netbox_reorder_rack/css/rack.css` & `netbox_reorder_rack-1.1.1/netbox_reorder_rack/static/netbox_reorder_rack/css/rack.css`

 * *Files identical despite different names*

### Comparing `netbox_reorder_rack-1.1.0/netbox_reorder_rack/static/netbox_reorder_rack/js/rack.js` & `netbox_reorder_rack-1.1.1/netbox_reorder_rack/static/netbox_reorder_rack/js/rack.js`

 * *Files identical despite different names*

### Comparing `netbox_reorder_rack-1.1.0/netbox_reorder_rack/static/netbox_reorder_rack/js/rack.js.map` & `netbox_reorder_rack-1.1.1/netbox_reorder_rack/static/netbox_reorder_rack/js/rack.js.map`

 * *Files identical despite different names*

### Comparing `netbox_reorder_rack-1.1.0/netbox_reorder_rack/templates/netbox_reorder_rack/inc/rack_elevation.html` & `netbox_reorder_rack-1.1.1/netbox_reorder_rack/templates/netbox_reorder_rack/inc/rack_elevation.html`

 * *Files identical despite different names*

### Comparing `netbox_reorder_rack-1.1.0/netbox_reorder_rack/templates/netbox_reorder_rack/rack.html` & `netbox_reorder_rack-1.1.1/netbox_reorder_rack/templates/netbox_reorder_rack/rack.html`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
 {% block content-wrapper %}
 <div class="tab-content">
   {% block content %}
   <div class="row">
     <div class="col col-12">
       <div class="row">
-        <div class="d-flex justify-content-end"><button class="btn btn-primary" id="saveButton" disabled>Save</button></div>
+        <div class="d-flex justify-content-end"><button class="btn btn-success" id="saveButton" disabled>Save</button></div>
       </div>
       <div class="row">
         <div class="col col-md-4 col-sm-4 col-xs-12 text-center">
           <h4>Front</h4>
           {% include 'netbox_reorder_rack/inc/rack_elevation.html' with units=front_units face='front' %}
         </div>
         <div class="col col-md-4 col-sm-4 col-xs-12 text-center">
```

### Comparing `netbox_reorder_rack-1.1.0/netbox_reorder_rack/templatetags/rack.py` & `netbox_reorder_rack-1.1.1/netbox_reorder_rack/templatetags/rack.py`

 * *Files identical despite different names*

### Comparing `netbox_reorder_rack-1.1.0/netbox_reorder_rack/tests/test_api.py` & `netbox_reorder_rack-1.1.1/netbox_reorder_rack/tests/test_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
+from core.models import ObjectType
 from dcim.models import Device
 from dcim.models import DeviceRole
 from dcim.models import DeviceType
 from dcim.models import Manufacturer
 from dcim.models import Rack
 from dcim.models import Site
-from django.contrib.contenttypes.models import ContentType
 from users.models import ObjectPermission
 from utilities.testing import TestCase
 
 
 class ReorderRackAPITest(TestCase):
     @classmethod
     def setUpTestData(cls):
@@ -140,16 +140,15 @@
         self.assertHttpStatus(resp, 500)
 
     def test_reorder_rack_view_with_permissions(self):
         # Add model-level permission
         obj_perm = ObjectPermission(name="Test permission", actions=["view", "change"])
         obj_perm.save()
         obj_perm.users.add(self.user)
-        ct = ContentType.objects.filter(model="device").first()
-        obj_perm.object_types.add(ct)
+        obj_perm.object_types.add(ObjectType.objects.get_for_model(Device))
 
         rack = Rack.objects.get(name="Test Rack 1")
         device1 = Device.objects.get(name="Device 1")
         device2 = Device.objects.get(name="Device 2")
         device3 = Device.objects.get(name="Device 3")
         device4 = Device.objects.get(name="Device 4")
```

### Comparing `netbox_reorder_rack-1.1.0/netbox_reorder_rack/tests/test_view.py` & `netbox_reorder_rack-1.1.1/netbox_reorder_rack/tests/test_view.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+from core.models import ObjectType
+from dcim.models import Device
 from dcim.models import Rack
 from dcim.models import Site
-from django.contrib.contenttypes.models import ContentType
 from users.models import ObjectPermission
 from utilities.testing import TestCase
 
 
 class ReorderRackTestCase(TestCase):
     @classmethod
     def setUpTestData(cls):
@@ -17,13 +18,12 @@
         self.assertHttpStatus(response, 403)
 
     def test_reorder_rack_view_with_permissions(self):
         # Add model-level permission
         obj_perm = ObjectPermission(name="Test permission", actions=["change", "view"])
         obj_perm.save()
         obj_perm.users.add(self.user)
-        ct = ContentType.objects.filter(model="device").first()
-        obj_perm.object_types.add(ct)
+        obj_perm.object_types.add(ObjectType.objects.get_for_model(Device))
         rack = Rack.objects.all().first()
 
         response = self.client.get(f"/dcim/racks/{rack.pk}/reorder/")
         self.assertHttpStatus(response, 200)
```

### Comparing `netbox_reorder_rack-1.1.0/netbox_reorder_rack/views.py` & `netbox_reorder_rack-1.1.1/netbox_reorder_rack/views.py`

 * *Files identical despite different names*

### Comparing `netbox_reorder_rack-1.1.0/netbox_reorder_rack.egg-info/PKG-INFO` & `netbox_reorder_rack-1.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 Metadata-Version: 2.1
 Name: netbox_reorder_rack
-Version: 1.1.0
+Version: 1.1.1
 Summary: NetBox plugin to reorder rack layouts.
 Home-page: https://github.com/minitriga/netbox-reorder-rack/
 Author: Alex Gittings
 Author-email: agitting96@gmail.com
 Project-URL: Bug Tracker, https://github.com/minitriga/netbox-reorder-rack/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Framework :: Django
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Netbox Reorder Rack Plugin
+<p align="center"><img src="docs/img/reorder-rack.svg"></p>
+
+<h1 align="center">Netbox Reorder Rack Plugin</h1>
 
 ![Version](https://img.shields.io/pypi/v/netbox-reorder-rack) ![Downloads](https://img.shields.io/pypi/dm/netbox-reorder-rack)
 
 Allow the ability to reorder rack units in NetBox using a drag and drop interface.
 
 ![Reorder Rack](docs/img/netbox-reorder-rack.gif)
 
+> If there are any issues feel free to create an [Issue](https://github.com/minitriga/netbox-reorder-rack/issues) or feel free to contact me directly on Slack in the [NetDev](https://netdev.chat/) community.
+
 ## Installation
 
 **_NOTE:_** For docker please see: [Docker install](https://github.com/netbox-community/netbox-docker/wiki/Using-Netbox-Plugins)
 
 The plugin is available as a Python package and can be installed with pip.
 
 Run the following commands to install the required package after activating the virtual environment:
@@ -55,15 +59,23 @@
 
 
 ## Compatibility Matrix
 
 | netbox version | plugin version |
 | -------------- | ----------------------------- |
 | >= 4.0.0       | >= v1.1.0                     |
-| <= 4.0.0       | = v1.0.0                     |
+| <= 4.0.0       | = v1.0.0                      |
+
+## Dependencies
+Python:
+  - None
+
+Javascript:
+  - Gridstack (Currently running same versions as Netbox)
+  - Bootsrap (Currently running same versions as Netbox)
 
 ### Update
 
 To update the plugin, you need to update the package and restart NetBox.
 
 ```shell
 source /opt/netbox/venv/bin/activate
```

### Comparing `netbox_reorder_rack-1.1.0/netbox_reorder_rack.egg-info/SOURCES.txt` & `netbox_reorder_rack-1.1.1/netbox_reorder_rack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox_reorder_rack-1.1.0/setup.py` & `netbox_reorder_rack-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="netbox_reorder_rack",
-    version="1.1.0",
+    version="1.1.1",
     author="Alex Gittings",
     author_email="agitting96@gmail.com",
     description="NetBox plugin to reorder rack layouts.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[],
     url="https://github.com/minitriga/netbox-reorder-rack/",
```

