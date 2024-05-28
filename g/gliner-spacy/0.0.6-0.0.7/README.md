# Comparing `tmp/gliner-spacy-0.0.6.tar.gz` & `tmp/gliner-spacy-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gliner-spacy-0.0.6.tar", last modified: Thu Apr 25 03:57:02 2024, max compression
+gzip compressed data, was "gliner-spacy-0.0.7.tar", last modified: Tue May 28 13:10:14 2024, max compression
```

## Comparing `gliner-spacy-0.0.6.tar` & `gliner-spacy-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 wjbmattingly   (501) staff       (20)        0 2024-04-25 03:57:02.970188 gliner-spacy-0.0.6/
--rw-r--r--   0 wjbmattingly   (501) staff       (20)     1073 2024-04-08 09:18:42.000000 gliner-spacy-0.0.6/LICENSE
--rw-r--r--   0 wjbmattingly   (501) staff       (20)     3435 2024-04-25 03:57:02.970073 gliner-spacy-0.0.6/PKG-INFO
--rw-r--r--   0 wjbmattingly   (501) staff       (20)     2727 2024-04-25 03:43:07.000000 gliner-spacy-0.0.6/README.md
-drwxr-xr-x   0 wjbmattingly   (501) staff       (20)        0 2024-04-25 03:57:02.969331 gliner-spacy-0.0.6/gliner_spacy/
--rw-r--r--   0 wjbmattingly   (501) staff       (20)       60 2024-04-25 03:46:10.000000 gliner-spacy-0.0.6/gliner_spacy/__init__.py
--rw-r--r--   0 wjbmattingly   (501) staff       (20)     2895 2024-04-25 03:41:51.000000 gliner-spacy-0.0.6/gliner_spacy/pipeline.py
--rw-r--r--   0 wjbmattingly   (501) staff       (20)       22 2024-04-25 03:37:21.000000 gliner-spacy-0.0.6/gliner_spacy/version.py
-drwxr-xr-x   0 wjbmattingly   (501) staff       (20)        0 2024-04-25 03:57:02.969913 gliner-spacy-0.0.6/gliner_spacy.egg-info/
--rw-r--r--   0 wjbmattingly   (501) staff       (20)     3435 2024-04-25 03:57:02.000000 gliner-spacy-0.0.6/gliner_spacy.egg-info/PKG-INFO
--rw-r--r--   0 wjbmattingly   (501) staff       (20)      279 2024-04-25 03:57:02.000000 gliner-spacy-0.0.6/gliner_spacy.egg-info/SOURCES.txt
--rw-r--r--   0 wjbmattingly   (501) staff       (20)        1 2024-04-25 03:57:02.000000 gliner-spacy-0.0.6/gliner_spacy.egg-info/dependency_links.txt
--rw-r--r--   0 wjbmattingly   (501) staff       (20)       13 2024-04-25 03:57:02.000000 gliner-spacy-0.0.6/gliner_spacy.egg-info/requires.txt
--rw-r--r--   0 wjbmattingly   (501) staff       (20)       13 2024-04-25 03:57:02.000000 gliner-spacy-0.0.6/gliner_spacy.egg-info/top_level.txt
--rw-r--r--   0 wjbmattingly   (501) staff       (20)       38 2024-04-25 03:57:02.970231 gliner-spacy-0.0.6/setup.cfg
--rw-r--r--   0 wjbmattingly   (501) staff       (20)     1295 2024-04-25 03:43:39.000000 gliner-spacy-0.0.6/setup.py
+drwxr-xr-x   0 wjbmattingly   (501) staff       (20)        0 2024-05-28 13:10:14.588565 gliner-spacy-0.0.7/
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)     1073 2024-04-08 09:18:42.000000 gliner-spacy-0.0.7/LICENSE
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)     3506 2024-05-28 13:10:14.588458 gliner-spacy-0.0.7/PKG-INFO
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)     2798 2024-05-28 12:18:02.000000 gliner-spacy-0.0.7/README.md
+drwxr-xr-x   0 wjbmattingly   (501) staff       (20)        0 2024-05-28 13:10:14.587778 gliner-spacy-0.0.7/gliner_spacy/
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)       60 2024-04-25 03:46:10.000000 gliner-spacy-0.0.7/gliner_spacy/__init__.py
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)     3177 2024-05-28 12:57:57.000000 gliner-spacy-0.0.7/gliner_spacy/pipeline.py
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)       22 2024-05-28 13:07:17.000000 gliner-spacy-0.0.7/gliner_spacy/version.py
+drwxr-xr-x   0 wjbmattingly   (501) staff       (20)        0 2024-05-28 13:10:14.588298 gliner-spacy-0.0.7/gliner_spacy.egg-info/
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)     3506 2024-05-28 13:10:14.000000 gliner-spacy-0.0.7/gliner_spacy.egg-info/PKG-INFO
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)      279 2024-05-28 13:10:14.000000 gliner-spacy-0.0.7/gliner_spacy.egg-info/SOURCES.txt
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)        1 2024-05-28 13:10:14.000000 gliner-spacy-0.0.7/gliner_spacy.egg-info/dependency_links.txt
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)       27 2024-05-28 13:10:14.000000 gliner-spacy-0.0.7/gliner_spacy.egg-info/requires.txt
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)       13 2024-05-28 13:10:14.000000 gliner-spacy-0.0.7/gliner_spacy.egg-info/top_level.txt
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)       38 2024-05-28 13:10:14.588598 gliner-spacy-0.0.7/setup.cfg
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)     1309 2024-05-28 12:41:34.000000 gliner-spacy-0.0.7/setup.py
```

### Comparing `gliner-spacy-0.0.6/LICENSE` & `gliner-spacy-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gliner-spacy-0.0.6/PKG-INFO` & `gliner-spacy-0.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gliner-spacy
-Version: 0.0.6
+Version: 0.0.7
 Summary: A SpaCy wrapper for the GLiNER model for enhanced Named Entity Recognition capabilities
 Home-page: https://github.com/theirstory/gliner-spacy
 Author: William J. B. Mattingly
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
@@ -89,10 +89,11 @@
 ## Configuration
 The default configuration of the wrapper can be modified according to your requirements. The configurable parameters are:
 - `gliner_model`: The GLiNER model to be used.
 - `chunk_size`: Size of the text chunk to be processed at once.
 - `labels`: The entity labels to be recognized.
 - `style`: The style of output for the entities (either 'ent' or 'span').
 - `threshold`: The threshold of the GliNER model (controls the degree to which a hit is considered an entity)
+- `map_location`: The device on which to run the model: `cpu` or `gpu`
 
 ## Contributing
 Contributions to this project are welcome. Please ensure that your code adheres to the project's coding standards and include tests for new features.
```

### Comparing `gliner-spacy-0.0.6/README.md` & `gliner-spacy-0.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -71,10 +71,11 @@
 ## Configuration
 The default configuration of the wrapper can be modified according to your requirements. The configurable parameters are:
 - `gliner_model`: The GLiNER model to be used.
 - `chunk_size`: Size of the text chunk to be processed at once.
 - `labels`: The entity labels to be recognized.
 - `style`: The style of output for the entities (either 'ent' or 'span').
 - `threshold`: The threshold of the GliNER model (controls the degree to which a hit is considered an entity)
+- `map_location`: The device on which to run the model: `cpu` or `gpu`
 
 ## Contributing
 Contributions to this project are welcome. Please ensure that your code adheres to the project's coding standards and include tests for new features.
```

### Comparing `gliner-spacy-0.0.6/gliner_spacy/pipeline.py` & `gliner-spacy-0.0.7/gliner_spacy/pipeline.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,44 @@
 import spacy
 from gliner.model import GLiNER
 from spacy.language import Language
+from spacy.tokens import Span
 
+Span.set_extension("score", default=0, force=True)
 
 DEFAULT_SPACY_CONFIG = {
-        "gliner_model": "urchade/gliner_base",
-        "chunk_size": 250,
-        "labels": ["person", "organization"],
-        "style": "ent",
-        "threshold": .50
-    }
+    "gliner_model": "urchade/gliner_base",
+    "chunk_size": 250,
+    "labels": ["person", "organization"],
+    "style": "ent",
+    "threshold": .50,
+    "map_location": "cpu",
+}
 
 
 @Language.factory("gliner_spacy",
                   assigns=["doc.ents"],
                   default_config=DEFAULT_SPACY_CONFIG)
 class GlinerSpacy:
     def __init__(self,
                  nlp: Language,
                  name: str,
                  gliner_model: str,
                  chunk_size: int,
                  labels: list,
                  style: str,
-                 threshold: float
+                 threshold: float,
+                 map_location: str
                  ):
         
         self.nlp = nlp
-        self.model = GLiNER.from_pretrained(gliner_model)
+        self.model = GLiNER.from_pretrained(
+            gliner_model,
+            map_location=map_location
+        )
         self.labels = labels
         self.chunk_size = chunk_size
         self.style = style
         self.threshold = threshold
 
     def __call__(self, doc):
         # Tokenize the text
@@ -54,31 +61,34 @@
                 chunk_entities = self.model.predict_entities(chunk, self.labels,
                                                              flat_ner=False,
                                                              threshold=self.threshold)
             else:
                 chunk_entities = self.model.predict_entities(chunk, self.labels,
                                                              flat_ner=True,
                                                              threshold=self.threshold)
+             
             for entity in chunk_entities:
                 all_entities.append({
                     'start': offset + entity['start'],
                     'end': offset + entity['end'],
-                    'label': entity['label']
+                    'label': entity['label'],
+                    'score': entity['score']
                 })
             offset += len(chunk)
 
         # Create new spans for the entities and add them to the doc
         doc = self._create_entity_spans(doc, all_entities)
 
         return doc
 
     def _create_entity_spans(self, doc, all_entities):
         spans = []
         for ent in all_entities:
             span = doc.char_span(ent['start'], ent['end'], label=ent['label'])
+            span._.score = ent['score']
             if span:  # Only add span if it is valid
                 spans.append(span)
         if self.style == "span":
             doc.spans["sc"] = spans
         else:
             doc.ents = spans
         return doc
```

### Comparing `gliner-spacy-0.0.6/gliner_spacy.egg-info/PKG-INFO` & `gliner-spacy-0.0.7/gliner_spacy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gliner-spacy
-Version: 0.0.6
+Version: 0.0.7
 Summary: A SpaCy wrapper for the GLiNER model for enhanced Named Entity Recognition capabilities
 Home-page: https://github.com/theirstory/gliner-spacy
 Author: William J. B. Mattingly
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
@@ -89,10 +89,11 @@
 ## Configuration
 The default configuration of the wrapper can be modified according to your requirements. The configurable parameters are:
 - `gliner_model`: The GLiNER model to be used.
 - `chunk_size`: Size of the text chunk to be processed at once.
 - `labels`: The entity labels to be recognized.
 - `style`: The style of output for the entities (either 'ent' or 'span').
 - `threshold`: The threshold of the GliNER model (controls the degree to which a hit is considered an entity)
+- `map_location`: The device on which to run the model: `cpu` or `gpu`
 
 ## Contributing
 Contributions to this project are welcome. Please ensure that your code adheres to the project's coding standards and include tests for new features.
```

### Comparing `gliner-spacy-0.0.6/setup.py` & `gliner-spacy-0.0.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,16 +18,16 @@
     author='William J. B. Mattingly',
     description='A SpaCy wrapper for the GLiNER model for enhanced Named Entity Recognition capabilities',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/theirstory/gliner-spacy',
     packages=find_packages(),
     install_requires=[
-        'spacy',
-        'gliner',
+        'spacy>=3.0.0',
+        'gliner>=0.2.0',
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',  
         'Intended Audience :: Developers',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
```

