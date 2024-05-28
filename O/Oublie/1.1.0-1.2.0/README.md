# Comparing `tmp/oublie-1.1.0.tar.gz` & `tmp/oublie-1.2.0.tar.gz`

## Comparing `oublie-1.1.0.tar` & `oublie-1.2.0.tar`

### file list

```diff
@@ -1,48 +1,52 @@
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 oublie-1.1.0/.idea/.gitignore
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 oublie-1.1.0/.idea/.name
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 oublie-1.1.0/.idea/Oublie-Python.iml
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 oublie-1.1.0/.idea/misc.xml
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 oublie-1.1.0/.idea/modules.xml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 oublie-1.1.0/.idea/vcs.xml
--rw-r--r--   0        0        0    10919 2020-02-02 00:00:00.000000 oublie-1.1.0/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 oublie-1.1.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 oublie-1.1.0/docs/Makefile
--rwxr-xr-x   0        0        0      804 2020-02-02 00:00:00.000000 oublie-1.1.0/docs/make.bat
--rw-r--r--   0        0        0    16993 2020-02-02 00:00:00.000000 oublie-1.1.0/docs/build/doctrees/environment.pickle
--rw-r--r--   0        0        0     4935 2020-02-02 00:00:00.000000 oublie-1.1.0/docs/build/doctrees/index.doctree
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 oublie-1.1.0/docs/build/html/.buildinfo
--rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 oublie-1.1.0/docs/build/html/genindex.html
--rw-r--r--   0        0        0     3359 2020-02-02 00:00:00.000000 oublie-1.1.0/docs/build/html/index.html
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 oublie-1.1.0/docs/build/html/objects.inv
--rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 oublie-1.1.0/docs/build/html/search.html
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 oublie-1.1.0/docs/build/html/searchindex.js
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 oublie-1.1.0/docs/build/html/_sources/index.rst.txt
--rw-r--r--   0        0        0    11932 2020-02-02 00:00:00.000000 oublie-1.1.0/docs/build/html/_static/alabaster.css
--rw-r--r--   0        0        0    15715 2020-02-02 00:00:00.000000 oublie-1.1.0/docs/build/html/_static/basic.css
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 oublie-1.1.0/docs/build/html/_static/custom.css
--rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 oublie-1.1.0/docs/build/html/_static/doctools.js
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 oublie-1.1.0/docs/build/html/_static/documentation_options.js
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 oublie-1.1.0/docs/build/html/_static/file.png
--rw-r--r--   0        0        0     4957 2020-02-02 00:00:00.000000 oublie-1.1.0/docs/build/html/_static/language_data.js
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 oublie-1.1.0/docs/build/html/_static/minus.png
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 oublie-1.1.0/docs/build/html/_static/plus.png
--rw-r--r--   0        0        0     5409 2020-02-02 00:00:00.000000 oublie-1.1.0/docs/build/html/_static/pygments.css
--rw-r--r--   0        0        0    18215 2020-02-02 00:00:00.000000 oublie-1.1.0/docs/build/html/_static/searchtools.js
--rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 oublie-1.1.0/docs/build/html/_static/sphinx_highlight.js
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 oublie-1.1.0/docs/source/conf.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 oublie-1.1.0/docs/source/index.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 oublie-1.1.0/src/Oublie/__init__.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 oublie-1.1.0/src/Oublie/example.py
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 oublie-1.1.0/src/Oublie/huatu.py
--rw-r--r--   0        0        0     5256 2020-02-02 00:00:00.000000 oublie-1.1.0/src/Oublie/netop.py
--rw-r--r--   0        0        0    18796 2020-02-02 00:00:00.000000 oublie-1.1.0/tests/AttMpls.graphml
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 oublie-1.1.0/tests/a.py
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 oublie-1.1.0/tests/aaa.py
--rw-r--r--   0        0        0    69478 2020-02-02 00:00:00.000000 oublie-1.1.0/tests/condensed_west_europe_delete.graphml
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 oublie-1.1.0/tests/test_huatu.py
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 oublie-1.1.0/tests/test_netop.py
--rw-r--r--   0        0        0    11046 2020-02-02 00:00:00.000000 oublie-1.1.0/tests/新建 DOCX 文档.docx
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 oublie-1.1.0/LICENSE
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 oublie-1.1.0/README.md
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 oublie-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 oublie-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 oublie-1.2.0/.idea/.gitignore
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 oublie-1.2.0/.idea/.name
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 oublie-1.2.0/.idea/Oublie-Python.iml
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 oublie-1.2.0/.idea/misc.xml
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 oublie-1.2.0/.idea/modules.xml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 oublie-1.2.0/.idea/vcs.xml
+-rw-r--r--   0        0        0    12693 2020-02-02 00:00:00.000000 oublie-1.2.0/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 oublie-1.2.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 oublie-1.2.0/docs/Makefile
+-rwxr-xr-x   0        0        0      804 2020-02-02 00:00:00.000000 oublie-1.2.0/docs/make.bat
+-rw-r--r--   0        0        0    16993 2020-02-02 00:00:00.000000 oublie-1.2.0/docs/build/doctrees/environment.pickle
+-rw-r--r--   0        0        0     4935 2020-02-02 00:00:00.000000 oublie-1.2.0/docs/build/doctrees/index.doctree
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 oublie-1.2.0/docs/build/html/.buildinfo
+-rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 oublie-1.2.0/docs/build/html/genindex.html
+-rw-r--r--   0        0        0     3359 2020-02-02 00:00:00.000000 oublie-1.2.0/docs/build/html/index.html
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 oublie-1.2.0/docs/build/html/objects.inv
+-rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 oublie-1.2.0/docs/build/html/search.html
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 oublie-1.2.0/docs/build/html/searchindex.js
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 oublie-1.2.0/docs/build/html/_sources/index.rst.txt
+-rw-r--r--   0        0        0    11932 2020-02-02 00:00:00.000000 oublie-1.2.0/docs/build/html/_static/alabaster.css
+-rw-r--r--   0        0        0    15715 2020-02-02 00:00:00.000000 oublie-1.2.0/docs/build/html/_static/basic.css
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 oublie-1.2.0/docs/build/html/_static/custom.css
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 oublie-1.2.0/docs/build/html/_static/doctools.js
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 oublie-1.2.0/docs/build/html/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 oublie-1.2.0/docs/build/html/_static/file.png
+-rw-r--r--   0        0        0     4957 2020-02-02 00:00:00.000000 oublie-1.2.0/docs/build/html/_static/language_data.js
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 oublie-1.2.0/docs/build/html/_static/minus.png
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 oublie-1.2.0/docs/build/html/_static/plus.png
+-rw-r--r--   0        0        0     5409 2020-02-02 00:00:00.000000 oublie-1.2.0/docs/build/html/_static/pygments.css
+-rw-r--r--   0        0        0    18215 2020-02-02 00:00:00.000000 oublie-1.2.0/docs/build/html/_static/searchtools.js
+-rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 oublie-1.2.0/docs/build/html/_static/sphinx_highlight.js
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 oublie-1.2.0/docs/source/conf.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 oublie-1.2.0/docs/source/index.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 oublie-1.2.0/src/Oublie/__init__.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 oublie-1.2.0/src/Oublie/example.py
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 oublie-1.2.0/src/Oublie/huatu.py
+-rw-r--r--   0        0        0     7473 2020-02-02 00:00:00.000000 oublie-1.2.0/src/Oublie/netop.py
+-rw-r--r--   0        0        0    24697 2020-02-02 00:00:00.000000 oublie-1.2.0/src/Oublie/netsss.py
+-rw-r--r--   0        0        0    18796 2020-02-02 00:00:00.000000 oublie-1.2.0/tests/AttMpls.graphml
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 oublie-1.2.0/tests/a.py
+-rw-r--r--   0        0        0    69478 2020-02-02 00:00:00.000000 oublie-1.2.0/tests/condensed_west_europe_delete.graphml
+-rw-r--r--   0        0        0     4800 2020-02-02 00:00:00.000000 oublie-1.2.0/tests/graph.svg
+-rw-r--r--   0        0        0    25443 2020-02-02 00:00:00.000000 oublie-1.2.0/tests/scapyyg6ed49h.svg
+-rw-r--r--   0        0        0   268262 2020-02-02 00:00:00.000000 oublie-1.2.0/tests/shixubuchang.png
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 oublie-1.2.0/tests/test_huatu.py
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 oublie-1.2.0/tests/test_netop.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 oublie-1.2.0/tests/test_netsss.py
+-rw-r--r--   0        0        0    11046 2020-02-02 00:00:00.000000 oublie-1.2.0/tests/新建 DOCX 文档.docx
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 oublie-1.2.0/LICENSE
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 oublie-1.2.0/README.md
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 oublie-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 oublie-1.2.0/PKG-INFO
```

### Comparing `oublie-1.1.0/.idea/workspace.xml` & `oublie-1.2.0/.idea/workspace.xml`

 * *Files 4% similar despite different names*

#### Comparing `oublie-1.1.0/.idea/workspace.xml` & `oublie-1.2.0/.idea/workspace.xml`

```diff
@@ -2,17 +2,23 @@
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
     <list default="true" id="5aff02c1-806c-496b-9b25-ca1b95b2d14c" name="变更" comment="完全搭好">
       <change afterPath="$PROJECT_DIR$/src/Oublie/netop.py" afterDir="false"/>
-      <change afterPath="$PROJECT_DIR$/tests/aaa.py" afterDir="false"/>
+      <change afterPath="$PROJECT_DIR$/src/Oublie/netsss.py" afterDir="false"/>
+      <change afterPath="$PROJECT_DIR$/tests/graph.svg" afterDir="false"/>
+      <change afterPath="$PROJECT_DIR$/tests/scapyyg6ed49h.svg" afterDir="false"/>
+      <change afterPath="$PROJECT_DIR$/tests/shixubuchang.png" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/tests/test_netop.py" afterDir="false"/>
+      <change afterPath="$PROJECT_DIR$/tests/test_netsss.py" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/tests/新建 DOCX 文档.docx" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/dist/oublie-1.0.0-py3-none-any.whl" beforeDir="false"/>
+      <change beforePath="$PROJECT_DIR$/dist/oublie-1.0.0.tar.gz" beforeDir="false"/>
       <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/src/Oublie/huatu.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/Oublie/huatu.py" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/tests/test.py" beforeDir="false"/>
       <change beforePath="$PROJECT_DIR$/tests/test_network.py" beforeDir="false" afterPath="$PROJECT_DIR$/tests/test_huatu.py" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
@@ -44,27 +50,30 @@
     <option name="showLibraryContents" value="true"/>
   </component>
   <component name="PropertiesComponent">{
   &quot;keyToString&quot;: {
     &quot;ASKED_ADD_EXTERNAL_FILES&quot;: &quot;true&quot;,
     &quot;RunOnceActivity.OpenProjectViewOnStart&quot;: &quot;true&quot;,
     &quot;RunOnceActivity.ShowReadmeOnStart&quot;: &quot;true&quot;,
-    &quot;last_opened_file_path&quot;: &quot;E:/31316/Documents/PycharmProject/Oublie-Python&quot;,
+    &quot;last_opened_file_path&quot;: &quot;E:/31316/Documents/PycharmProject/Oublie-Python/tests&quot;,
     &quot;settings.editor.selected.configurable&quot;: &quot;actions.on.save&quot;
   }
 }</component>
   <component name="RecentsManager">
+    <key name="CopyFile.RECENT_KEYS">
+      <recent name="E:\31316\Documents\PycharmProject\Oublie-Python\tests"/>
+    </key>
     <key name="MoveFile.RECENT_KEYS">
       <recent name="E:\31316\Documents\PycharmProject\Oublie-Python\tests"/>
       <recent name="E:\31316\Documents\PycharmProject\Oublie\tests"/>
       <recent name="E:\31316\Documents\PycharmProject\Oublie"/>
       <recent name="E:\31316\Documents\PycharmProject\Oublie\src\aaa"/>
     </key>
   </component>
-  <component name="RunManager" selected="Python.test_netop">
+  <component name="RunManager" selected="Python.test_netsss">
     <configuration name="a" type="PythonConfigurationType" factoryName="Python" temporary="true" nameIsGenerated="true">
       <module name="Oublie-Python"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <envs>
         <env name="PYTHONUNBUFFERED" value="1"/>
       </envs>
@@ -141,16 +150,38 @@
       <option name="SHOW_COMMAND_LINE" value="false"/>
       <option name="EMULATE_TERMINAL" value="false"/>
       <option name="MODULE_MODE" value="false"/>
       <option name="REDIRECT_INPUT" value="false"/>
       <option name="INPUT_FILE" value=""/>
       <method v="2"/>
     </configuration>
+    <configuration name="test_netsss" type="PythonConfigurationType" factoryName="Python" temporary="true" nameIsGenerated="true">
+      <module name="Oublie-Python"/>
+      <option name="INTERPRETER_OPTIONS" value=""/>
+      <option name="PARENT_ENVS" value="true"/>
+      <envs>
+        <env name="PYTHONUNBUFFERED" value="1"/>
+      </envs>
+      <option name="SDK_HOME" value=""/>
+      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/tests"/>
+      <option name="IS_MODULE_SDK" value="true"/>
+      <option name="ADD_CONTENT_ROOTS" value="true"/>
+      <option name="ADD_SOURCE_ROOTS" value="true"/>
+      <option name="SCRIPT_NAME" value="$PROJECT_DIR$/tests/test_netsss.py"/>
+      <option name="PARAMETERS" value=""/>
+      <option name="SHOW_COMMAND_LINE" value="false"/>
+      <option name="EMULATE_TERMINAL" value="false"/>
+      <option name="MODULE_MODE" value="false"/>
+      <option name="REDIRECT_INPUT" value="false"/>
+      <option name="INPUT_FILE" value=""/>
+      <method v="2"/>
+    </configuration>
     <recent_temporary>
       <list>
+        <item itemvalue="Python.test_netsss"/>
         <item itemvalue="Python.test_netop"/>
         <item itemvalue="Python.netop"/>
         <item itemvalue="Python.test_huatu"/>
         <item itemvalue="Python.a"/>
       </list>
     </recent_temporary>
   </component>
```

### Comparing `oublie-1.1.0/docs/Makefile` & `oublie-1.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `oublie-1.1.0/docs/make.bat` & `oublie-1.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `oublie-1.1.0/docs/build/doctrees/environment.pickle` & `oublie-1.2.0/docs/build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `oublie-1.1.0/docs/build/doctrees/index.doctree` & `oublie-1.2.0/docs/build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `oublie-1.1.0/docs/build/html/genindex.html` & `oublie-1.2.0/docs/build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `oublie-1.1.0/docs/build/html/index.html` & `oublie-1.2.0/docs/build/html/index.html`

 * *Files identical despite different names*

### Comparing `oublie-1.1.0/docs/build/html/search.html` & `oublie-1.2.0/docs/build/html/search.html`

 * *Files identical despite different names*

### Comparing `oublie-1.1.0/docs/build/html/searchindex.js` & `oublie-1.2.0/docs/build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `oublie-1.1.0/docs/build/html/_static/alabaster.css` & `oublie-1.2.0/docs/build/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `oublie-1.1.0/docs/build/html/_static/basic.css` & `oublie-1.2.0/docs/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `oublie-1.1.0/docs/build/html/_static/doctools.js` & `oublie-1.2.0/docs/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `oublie-1.1.0/docs/build/html/_static/language_data.js` & `oublie-1.2.0/docs/build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `oublie-1.1.0/docs/build/html/_static/pygments.css` & `oublie-1.2.0/docs/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `oublie-1.1.0/docs/build/html/_static/searchtools.js` & `oublie-1.2.0/docs/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `oublie-1.1.0/docs/build/html/_static/sphinx_highlight.js` & `oublie-1.2.0/docs/build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `oublie-1.1.0/docs/source/conf.py` & `oublie-1.2.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `oublie-1.1.0/src/Oublie/huatu.py` & `oublie-1.2.0/src/Oublie/huatu.py`

 * *Files identical despite different names*

### Comparing `oublie-1.1.0/tests/AttMpls.graphml` & `oublie-1.2.0/tests/AttMpls.graphml`

 * *Files identical despite different names*

### Comparing `oublie-1.1.0/tests/condensed_west_europe_delete.graphml` & `oublie-1.2.0/tests/condensed_west_europe_delete.graphml`

 * *Files identical despite different names*

### Comparing `oublie-1.1.0/tests/test_netop.py` & `oublie-1.2.0/tests/test_netop.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,81 @@
 from _socket import gethostbyaddr
 
+import scapy.route
+from scapy.layers.l2 import arping
+
 from src.Oublie.netop import *
 
-ans, unans = None, None
+# ans, unans = None, None
 
-# ans,unans=synSCAN("172.16.14.87",80)
+# ans, unans = synScan("172.16.14.0/27")
 
-# ans, unans = sr(IP(dst="127.0.0.1")/ICMP(), timeout=3)
+# ans, unans = icmpScanHost("172.16.14.0/24", timeout=3)
 # ans.summary(lambda s,r: r.sprintf("%IP.src% is alive") )
 
+# res = icmpScanHost("172.16.14.0/24", timeout=3)
+
 # ans, unans = xmasScan("172.16.76.91")
 
 # ans, unans = sr(IP(dst="127.0.0.1",proto=80)/"SCAPY",retry=2)
 
 # ans.summary(lambda s,r:(s.summary(),r.summary()))
 
 # ans, unans = ackScan("172.16.76.91",(80,90))
 
 # ans, unans = arpPing("172.16.76.0/24", iface="以太网")
 
-ans, unans = icmpPing("172.16.76.1", timeout=5, iface='以太网')
+# res = arpScanHost("172.16.76.0/27", "以太网", timeout=10)
 
-# ans, unans = tcpTraceroute("172.16.14.1", 3, )
+# ans, unans = icmpPing("172.16.14.87", timeout=5, iface='以太网', count=1)
 
 # ans, unans = icmpPing("172.16.76.1", 10, iface='以太网')
 
-# ans, unans = udpTraceroute("172.16.76.1", 3, 3)
+# ans = udpTraceroute("172.16.14.1", 3, 5)
+
+# ans = tcpSynTraceroute("172.16.14.1", 3, 5)
+
+# res, _ = traceroute("www.baidu.com", maxttl=17, timeout=5)
+
+# res = dnsTraceroute("172.16.14.87", maxttl=5)
+
+# for s, r in res:
+#     print(s.ttl)
+
+# res.graph()
 
-# res = arpScanHost("172.16.76.0/27", "以太网")
-# print(res)
+# ans.summary()
 
-# for i in ans:
-#     i.show()
+# for i in res:
+#     print(i)
 
-ans.summary()
-print("----")
-if unans != None:
-    unans.summary()
+# for s, r in ans:
+#     print(s["IP"].ttl, r["IP"].sip)
+
+# ans.summary()
+# print("----")
+# if unans != None:
+#     unans.summary()
+#
+# print("---")
+# print(ans.res[0])
 
 # if ans:
 #     print(ans.summary)
 # else:
 #     print("没有响应")
 
 # print(conf.route.route("172.16.14.1"))
 # ifa = IFACES.dev_from_name('以太网')
 # print(ifa.name, ifa.index, ifa.network_name, ifa.description)
+
+
+# arpingans.summary(lambda s, r: r.sprintf("%IP.src%\t{ICMP:%ICMP.type%}\t{TCP:%TCP.flags%}"))
+# ans, unans = arping("172.16.76.0/27")
+# k = arpScanHost(ans)
+# print(k)
+
+lfa = LFA("H1", "172.16.14.87", "")
+
+lfa.traceroute_target()
+
+scapy.route.Route
```

### Comparing `oublie-1.1.0/tests/新建 DOCX 文档.docx` & `oublie-1.2.0/tests/新建 DOCX 文档.docx`

 * *Files identical despite different names*

### Comparing `oublie-1.1.0/LICENSE` & `oublie-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oublie-1.1.0/PKG-INFO` & `oublie-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: Oublie
-Version: 1.1.0
+Version: 1.2.0
 Summary: Oublie的个人Python模块
 Project-URL: Homepage, https://github.com/oublie6/Oublie-Python
 Project-URL: Bug Tracker, https://github.com/oublie6/Oublie-Python/issues
 Author-email: Oublie <313166062@qq.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Requires-Dist: matplotlib
 Requires-Dist: networkx
 Description-Content-Type: text/markdown
 
 # Oublie的个人仓库
 
 这是Oublie的个人仓库
```

