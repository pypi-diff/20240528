# Comparing `tmp/openai_hacker-0.1.3.tar.gz` & `tmp/openai_hacker-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_hacker-0.1.3.tar", last modified: Fri Mar 29 05:56:44 2024, max compression
+gzip compressed data, was "openai_hacker-0.1.4.tar", last modified: Tue May 28 01:46:46 2024, max compression
```

## Comparing `openai_hacker-0.1.3.tar` & `openai_hacker-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 lixf       (501) staff       (20)        0 2024-03-29 05:56:44.983764 openai_hacker-0.1.3/
--rw-r--r--   0 lixf       (501) staff       (20)    10142 2024-03-13 10:35:19.000000 openai_hacker-0.1.3/LICENSE
--rw-r--r--   0 lixf       (501) staff       (20)     2044 2024-03-29 05:56:44.983914 openai_hacker-0.1.3/PKG-INFO
--rw-r--r--   0 lixf       (501) staff       (20)     1012 2024-03-29 05:54:10.000000 openai_hacker-0.1.3/README.md
-drwxr-xr-x   0 lixf       (501) staff       (20)        0 2024-03-29 05:56:44.980817 openai_hacker-0.1.3/openai_hacker/
--rw-r--r--   0 lixf       (501) staff       (20)       47 2024-03-28 02:12:13.000000 openai_hacker-0.1.3/openai_hacker/__init__.py
--rw-r--r--   0 lixf       (501) staff       (20)     5091 2024-03-28 02:27:02.000000 openai_hacker-0.1.3/openai_hacker/_hack.py
--rw-r--r--   0 lixf       (501) staff       (20)      220 2024-03-28 02:11:55.000000 openai_hacker-0.1.3/openai_hacker/conf.py
-drwxr-xr-x   0 lixf       (501) staff       (20)        0 2024-03-29 05:56:44.983421 openai_hacker-0.1.3/openai_hacker.egg-info/
--rw-r--r--   0 lixf       (501) staff       (20)     2044 2024-03-29 05:56:44.000000 openai_hacker-0.1.3/openai_hacker.egg-info/PKG-INFO
--rw-r--r--   0 lixf       (501) staff       (20)      327 2024-03-29 05:56:44.000000 openai_hacker-0.1.3/openai_hacker.egg-info/SOURCES.txt
--rw-r--r--   0 lixf       (501) staff       (20)        1 2024-03-29 05:56:44.000000 openai_hacker-0.1.3/openai_hacker.egg-info/dependency_links.txt
--rw-r--r--   0 lixf       (501) staff       (20)        1 2024-03-13 10:04:07.000000 openai_hacker-0.1.3/openai_hacker.egg-info/not-zip-safe
--rw-r--r--   0 lixf       (501) staff       (20)       21 2024-03-29 05:56:44.000000 openai_hacker-0.1.3/openai_hacker.egg-info/requires.txt
--rw-r--r--   0 lixf       (501) staff       (20)       14 2024-03-29 05:56:44.000000 openai_hacker-0.1.3/openai_hacker.egg-info/top_level.txt
--rw-r--r--   0 lixf       (501) staff       (20)       38 2024-03-29 05:56:44.984435 openai_hacker-0.1.3/setup.cfg
--rw-r--r--   0 lixf       (501) staff       (20)     2255 2024-03-14 07:07:15.000000 openai_hacker-0.1.3/setup.py
+drwxr-xr-x   0 lixf       (501) staff       (20)        0 2024-05-28 01:46:46.351805 openai_hacker-0.1.4/
+-rw-r--r--   0 lixf       (501) staff       (20)    10142 2024-03-13 10:35:19.000000 openai_hacker-0.1.4/LICENSE
+-rw-r--r--   0 lixf       (501) staff       (20)     2044 2024-05-28 01:46:46.351964 openai_hacker-0.1.4/PKG-INFO
+-rw-r--r--   0 lixf       (501) staff       (20)     1012 2024-03-29 05:54:10.000000 openai_hacker-0.1.4/README.md
+drwxr-xr-x   0 lixf       (501) staff       (20)        0 2024-05-28 01:46:46.348167 openai_hacker-0.1.4/openai_hacker/
+-rw-r--r--   0 lixf       (501) staff       (20)       47 2024-05-28 01:44:19.000000 openai_hacker-0.1.4/openai_hacker/__init__.py
+-rw-r--r--   0 lixf       (501) staff       (20)     5463 2024-05-11 10:46:04.000000 openai_hacker-0.1.4/openai_hacker/_hack.py
+-rw-r--r--   0 lixf       (501) staff       (20)      220 2024-03-28 02:11:55.000000 openai_hacker-0.1.4/openai_hacker/conf.py
+drwxr-xr-x   0 lixf       (501) staff       (20)        0 2024-05-28 01:46:46.351404 openai_hacker-0.1.4/openai_hacker.egg-info/
+-rw-r--r--   0 lixf       (501) staff       (20)     2044 2024-05-28 01:46:46.000000 openai_hacker-0.1.4/openai_hacker.egg-info/PKG-INFO
+-rw-r--r--   0 lixf       (501) staff       (20)      327 2024-05-28 01:46:46.000000 openai_hacker-0.1.4/openai_hacker.egg-info/SOURCES.txt
+-rw-r--r--   0 lixf       (501) staff       (20)        1 2024-05-28 01:46:46.000000 openai_hacker-0.1.4/openai_hacker.egg-info/dependency_links.txt
+-rw-r--r--   0 lixf       (501) staff       (20)        1 2024-03-13 10:04:07.000000 openai_hacker-0.1.4/openai_hacker.egg-info/not-zip-safe
+-rw-r--r--   0 lixf       (501) staff       (20)       21 2024-05-28 01:46:46.000000 openai_hacker-0.1.4/openai_hacker.egg-info/requires.txt
+-rw-r--r--   0 lixf       (501) staff       (20)       14 2024-05-28 01:46:46.000000 openai_hacker-0.1.4/openai_hacker.egg-info/top_level.txt
+-rw-r--r--   0 lixf       (501) staff       (20)       38 2024-05-28 01:46:46.352442 openai_hacker-0.1.4/setup.cfg
+-rw-r--r--   0 lixf       (501) staff       (20)     2255 2024-03-14 07:07:15.000000 openai_hacker-0.1.4/setup.py
```

### Comparing `openai_hacker-0.1.3/LICENSE` & `openai_hacker-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_hacker-0.1.3/PKG-INFO` & `openai_hacker-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_hacker
-Version: 0.1.3
+Version: 0.1.4
 Summary: hacker of openai python client
 Home-page: https://github.com/lixf/openai-hacker
 Author: DataCanvas Community
 Author-email: lixf@sovon.net
 License: Apache License 2.0
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
```

### Comparing `openai_hacker-0.1.3/README.md` & `openai_hacker-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `openai_hacker-0.1.3/openai_hacker/_hack.py` & `openai_hacker-0.1.4/openai_hacker/_hack.py`

 * *Files 12% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         fn_text_create_cached = None
 
 
 def get_next_dump_file(chat: bool):
     counters[conf.stage] += 1
     n_counter = counters[conf.stage]
     suffix = conf.suffix_chat if chat else conf.suffix_completion
-    dump_file = f'{conf.stage}_{n_counter:03d}{suffix}'
+    dump_file = f'{conf.stage}_{n_counter:06d}{suffix}'
     return dump_file
 
 
 def dump_data(file_name: str, data):
     if file_name.endswith('.json'):
         content = json.dumps(data, ensure_ascii=False, indent=2, default=json_default)
     else:  # default as yaml
@@ -123,15 +123,25 @@
     r = None
     try:
         if fn_chat_create_cached is not None:
             r = fn_chat_create_cached(*args, **kwargs)
         else:
             r = fn_chat_create_original(*args, **kwargs)
 
-        log_data = dict(request=kwargs, response=r.__dict__)
+        log_data = dict(request=kwargs, response=dict(
+            choices=[dict(
+                content=m['message']['content'],
+                role=m['message']['role']
+            ) for m in r['choices']],
+            model=r.get('model'),
+            created=r.get('created'),
+        ))
+        if 'usage' in r.keys():
+            log_data['response']['usage'] = {k: v for k, v in r['usage'].items() if k.find('token') >= 0}
+
         dump_data(log_file, log_data)
         return r
     except KeyboardInterrupt:
         raise
     except AttributeError:
         return r  # ignore
     except Exception as e:
```

### Comparing `openai_hacker-0.1.3/openai_hacker.egg-info/PKG-INFO` & `openai_hacker-0.1.4/openai_hacker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-hacker
-Version: 0.1.3
+Version: 0.1.4
 Summary: hacker of openai python client
 Home-page: https://github.com/lixf/openai-hacker
 Author: DataCanvas Community
 Author-email: lixf@sovon.net
 License: Apache License 2.0
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
```

### Comparing `openai_hacker-0.1.3/setup.py` & `openai_hacker-0.1.4/setup.py`

 * *Files identical despite different names*

