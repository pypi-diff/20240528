# Comparing `tmp/ru_text_cleaner-2.0.1.tar.gz` & `tmp/ru_text_cleaner-2.0.2.tar.gz`

## Comparing `ru_text_cleaner-2.0.1.tar` & `ru_text_cleaner-2.0.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.1/requirements.txt
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.1/test.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.1/.idea/.gitignore
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.1/.idea/TextCleaner.iml
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.1/.idea/misc.xml
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.1/.idea/modules.xml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.1/.idea/vcs.xml
--rw-r--r--   0        0        0    10856 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.1/.idea/workspace.xml
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.1/src/ru_text_cleaner/__init__.py
--rw-r--r--   0        0        0     3576 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.1/src/ru_text_cleaner/simple_cleaner/TextCleaner.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.1/src/ru_text_cleaner/simple_cleaner/__init__.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.1/src/ru_text_cleaner/simple_cleaner/_clean_stopwords.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.1/src/ru_text_cleaner/simple_cleaner/_emoji_cleaner.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.1/src/ru_text_cleaner/simple_cleaner/_html_cleaner.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.1/src/ru_text_cleaner/simple_cleaner/_punctuation_cleaner.py
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.1/src/ru_text_cleaner/simple_cleaner/_spaces_cleaner.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.1/src/ru_text_cleaner/simple_cleaner/_to_lower.py
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.1/src/ru_text_cleaner/simple_cleaner/_to_morpheme.py
--rw-r--r--   0        0        0     3801 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.1/src/ru_text_cleaner/tensor_cleaner/TextCleaner.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.1/src/ru_text_cleaner/tensor_cleaner/__init__.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.1/src/ru_text_cleaner/tensor_cleaner/_clean_stopwords.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.1/src/ru_text_cleaner/tensor_cleaner/_emoji_cleaner.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.1/src/ru_text_cleaner/tensor_cleaner/_html_cleaner.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.1/src/ru_text_cleaner/tensor_cleaner/_punctuation_cleaner.py
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.1/src/ru_text_cleaner/tensor_cleaner/_spaces_cleaner.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.1/src/ru_text_cleaner/tensor_cleaner/_to_lower.py
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.1/src/ru_text_cleaner/tensor_cleaner/_to_morpheme.py
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.1/LICENSE
--rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.1/README.md
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/requirements.txt
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/test.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/.idea/.gitignore
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/.idea/TextCleaner.iml
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/.idea/misc.xml
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/.idea/vcs.xml
+-rw-r--r--   0        0        0    11204 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/.idea/workspace.xml
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/src/ru_text_cleaner/__init__.py
+-rw-r--r--   0        0        0     3576 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/src/ru_text_cleaner/simple_cleaner/TextCleaner.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/src/ru_text_cleaner/simple_cleaner/__init__.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/src/ru_text_cleaner/simple_cleaner/_clean_stopwords.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/src/ru_text_cleaner/simple_cleaner/_emoji_cleaner.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/src/ru_text_cleaner/simple_cleaner/_html_cleaner.py
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/src/ru_text_cleaner/simple_cleaner/_punctuation_cleaner.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/src/ru_text_cleaner/simple_cleaner/_spaces_cleaner.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/src/ru_text_cleaner/simple_cleaner/_to_lower.py
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/src/ru_text_cleaner/simple_cleaner/_to_morpheme.py
+-rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/src/ru_text_cleaner/tensor_cleaner/TextCleaner.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/src/ru_text_cleaner/tensor_cleaner/__init__.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/src/ru_text_cleaner/tensor_cleaner/_clean_stopwords.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/src/ru_text_cleaner/tensor_cleaner/_emoji_cleaner.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/src/ru_text_cleaner/tensor_cleaner/_html_cleaner.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/src/ru_text_cleaner/tensor_cleaner/_punctuation_cleaner.py
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/src/ru_text_cleaner/tensor_cleaner/_spaces_cleaner.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/src/ru_text_cleaner/tensor_cleaner/_to_lower.py
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/src/ru_text_cleaner/tensor_cleaner/_to_morpheme.py
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/LICENSE
+-rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/README.md
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/PKG-INFO
```

### Comparing `ru_text_cleaner-2.0.1/.idea/workspace.xml` & `ru_text_cleaner-2.0.2/.idea/workspace.xml`

 * *Files 16% similar despite different names*

#### Comparing `ru_text_cleaner-2.0.1/.idea/workspace.xml` & `ru_text_cleaner-2.0.2/.idea/workspace.xml`

```diff
@@ -1,17 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
-    <list default="true" id="1e7c1d4a-6db9-4bec-b8db-c44acb60056e" name="Changes" comment="Adapted for tensforflow strings">
-      <change beforePath="$PROJECT_DIR$/README.md" beforeDir="false" afterPath="$PROJECT_DIR$/README.md" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/ru_text_cleaner/simple_cleaner/_punctuation_cleaner.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/ru_text_cleaner/simple_cleaner/_punctuation_cleaner.py" afterDir="false"/>
-    </list>
+    <list default="true" id="1e7c1d4a-6db9-4bec-b8db-c44acb60056e" name="Changes" comment="Adapted for tensforflow strings"/>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
     <option name="RECENT_TEMPLATES">
@@ -227,15 +224,31 @@
       <option name="closed" value="true"/>
       <created>1716486527377</created>
       <option name="number" value="00018"/>
       <option name="presentableId" value="LOCAL-00018"/>
       <option name="project" value="LOCAL"/>
       <updated>1716486527377</updated>
     </task>
-    <option name="localTasksCounter" value="19"/>
+    <task id="LOCAL-00019" summary="Adapted for tensforflow strings">
+      <option name="closed" value="true"/>
+      <created>1716486793625</created>
+      <option name="number" value="00019"/>
+      <option name="presentableId" value="LOCAL-00019"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1716486793625</updated>
+    </task>
+    <task id="LOCAL-00020" summary="Adapted for tensforflow strings">
+      <option name="closed" value="true"/>
+      <created>1716486939290</created>
+      <option name="number" value="00020"/>
+      <option name="presentableId" value="LOCAL-00020"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1716486939290</updated>
+    </task>
+    <option name="localTasksCounter" value="21"/>
     <servers/>
   </component>
   <component name="VcsManagerConfiguration">
     <MESSAGE value="More functions v1.0"/>
     <MESSAGE value="Support only russian language"/>
     <MESSAGE value="README.md"/>
     <MESSAGE value="File configuration"/>
```

### Comparing `ru_text_cleaner-2.0.1/.idea/inspectionProfiles/Project_Default.xml` & `ru_text_cleaner-2.0.2/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `ru_text_cleaner-2.0.1/src/ru_text_cleaner/simple_cleaner/TextCleaner.py` & `ru_text_cleaner-2.0.2/src/ru_text_cleaner/simple_cleaner/TextCleaner.py`

 * *Files identical despite different names*

### Comparing `ru_text_cleaner-2.0.1/src/ru_text_cleaner/simple_cleaner/_clean_stopwords.py` & `ru_text_cleaner-2.0.2/src/ru_text_cleaner/simple_cleaner/_clean_stopwords.py`

 * *Files identical despite different names*

### Comparing `ru_text_cleaner-2.0.1/src/ru_text_cleaner/simple_cleaner/_spaces_cleaner.py` & `ru_text_cleaner-2.0.2/src/ru_text_cleaner/simple_cleaner/_spaces_cleaner.py`

 * *Files identical despite different names*

### Comparing `ru_text_cleaner-2.0.1/src/ru_text_cleaner/simple_cleaner/_to_morpheme.py` & `ru_text_cleaner-2.0.2/src/ru_text_cleaner/simple_cleaner/_to_morpheme.py`

 * *Files identical despite different names*

### Comparing `ru_text_cleaner-2.0.1/src/ru_text_cleaner/tensor_cleaner/TextCleaner.py` & `ru_text_cleaner-2.0.2/src/ru_text_cleaner/tensor_cleaner/TextCleaner.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import tensorflow
-
+import warnings
 from ._html_cleaner import clean_html
 from ._spaces_cleaner import clean_spaces
 from ._to_morpheme import text_to_morphems
 from ._to_lower import to_lower_text
 from ._emoji_cleaner import clean_emoji
 from ._clean_stopwords import clean_stopwords
 from ._punctuation_cleaner import clean_punctuation
 
-
 class TextCleaner:
     def __init__(self, spaces=True, punctuation=True, html=True, emoji=True, lower=True,
                  stop_words=True, morpheme=True):
 
+        warnings.warn("Tensor cleaners is deprecated. It will be overwritten in next versions", DeprecationWarning)
+
         """
         Метод __init__ инциализирует экземпляр класса TextCleaner
 
         self.spaces = spaces - Необходимо ли удалять пробелы
         self.punctuation = punctuation - Необходимо ли удалять пунктуацию
         self.html = html - Необходимо ли удалять теги HTML
         self.emoji = emoji - Необходимо ли удалять Emoji
```

### Comparing `ru_text_cleaner-2.0.1/src/ru_text_cleaner/tensor_cleaner/_clean_stopwords.py` & `ru_text_cleaner-2.0.2/src/ru_text_cleaner/tensor_cleaner/_clean_stopwords.py`

 * *Files identical despite different names*

### Comparing `ru_text_cleaner-2.0.1/src/ru_text_cleaner/tensor_cleaner/_spaces_cleaner.py` & `ru_text_cleaner-2.0.2/src/ru_text_cleaner/tensor_cleaner/_spaces_cleaner.py`

 * *Files identical despite different names*

### Comparing `ru_text_cleaner-2.0.1/src/ru_text_cleaner/tensor_cleaner/_to_morpheme.py` & `ru_text_cleaner-2.0.2/src/ru_text_cleaner/tensor_cleaner/_to_morpheme.py`

 * *Files identical despite different names*

### Comparing `ru_text_cleaner-2.0.1/LICENSE` & `ru_text_cleaner-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ru_text_cleaner-2.0.1/README.md` & `ru_text_cleaner-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ru_text_cleaner-2.0.1/pyproject.toml` & `ru_text_cleaner-2.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['pymorphy2>=0.9.1', 'nltk>=3.8.1', 'hatchling', 'emoji>=2.11.1', 'tensorflow>=2.16.1']
 build-backend = "hatchling.build"
 
 [project]
 name = "ru-text-cleaner"
-version = "2.0.1"
+version = "2.0.2"
 authors = [
     { name="Vildan Nasyrov", email="" },
     { name="Artem Gafarov", email="a.m.gafarov@ya.ru" },
 ]
 description = "Cleans russian text and preparing for NLP"
 requires-python = ">=3.10.4"
 readme = "README.md"
```

### Comparing `ru_text_cleaner-2.0.1/PKG-INFO` & `ru_text_cleaner-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ru-text-cleaner
-Version: 2.0.1
+Version: 2.0.2
 Summary: Cleans russian text and preparing for NLP
 Project-URL: Homepage, https://github.com/rvneural/TextCleaner
 Project-URL: Issues, https://github.com/rvneural/TextCleaner/issues
 Author: Vildan Nasyrov
 Author-email: Artem Gafarov <a.m.gafarov@ya.ru>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

