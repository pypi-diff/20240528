# Comparing `tmp/Dsend-0.3.tar.gz` & `tmp/Dsend-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Dsend-0.3.tar", last modified: Tue May 28 16:00:42 2024, max compression
+gzip compressed data, was "Dsend-0.4.tar", last modified: Tue May 28 17:45:59 2024, max compression
```

## Comparing `Dsend-0.3.tar` & `Dsend-0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 16:00:42.191323 Dsend-0.3/
-drwxrwxrwx   0        0        0        0 2024-05-28 16:00:42.184323 Dsend-0.3/Dsend/
--rw-rw-rw-   0        0        0       59 2024-05-28 15:59:42.000000 Dsend-0.3/Dsend/__init__.py
--rw-rw-rw-   0        0        0     1174 2024-05-28 15:59:05.000000 Dsend-0.3/Dsend/dsend.py
-drwxrwxrwx   0        0        0        0 2024-05-28 16:00:42.190326 Dsend-0.3/Dsend.egg-info/
--rw-rw-rw-   0        0        0      182 2024-05-28 16:00:42.000000 Dsend-0.3/Dsend.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      195 2024-05-28 16:00:42.000000 Dsend-0.3/Dsend.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 16:00:42.000000 Dsend-0.3/Dsend.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-28 16:00:42.000000 Dsend-0.3/Dsend.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-28 16:00:42.000000 Dsend-0.3/Dsend.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      182 2024-05-28 16:00:42.191323 Dsend-0.3/PKG-INFO
--rw-rw-rw-   0        0        0      351 2024-05-28 13:09:33.000000 Dsend-0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-05-28 16:00:42.191323 Dsend-0.3/setup.cfg
--rw-rw-rw-   0        0        0      365 2024-05-28 16:00:30.000000 Dsend-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 17:45:59.055151 Dsend-0.4/
+drwxrwxrwx   0        0        0        0 2024-05-28 17:45:59.045151 Dsend-0.4/Dsend/
+-rw-rw-rw-   0        0        0       59 2024-05-28 15:59:42.000000 Dsend-0.4/Dsend/__init__.py
+-rw-rw-rw-   0        0        0     1284 2024-05-28 17:44:36.000000 Dsend-0.4/Dsend/dsend.py
+drwxrwxrwx   0        0        0        0 2024-05-28 17:45:59.054151 Dsend-0.4/Dsend.egg-info/
+-rw-rw-rw-   0        0        0      182 2024-05-28 17:45:58.000000 Dsend-0.4/Dsend.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      195 2024-05-28 17:45:59.000000 Dsend-0.4/Dsend.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 17:45:58.000000 Dsend-0.4/Dsend.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-28 17:45:58.000000 Dsend-0.4/Dsend.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-28 17:45:58.000000 Dsend-0.4/Dsend.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      182 2024-05-28 17:45:59.055151 Dsend-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      351 2024-05-28 13:09:33.000000 Dsend-0.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-28 17:45:59.055151 Dsend-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      365 2024-05-28 17:45:56.000000 Dsend-0.4/setup.py
```

### Comparing `Dsend-0.3/Dsend/dsend.py` & `Dsend-0.4/Dsend/dsend.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,25 +18,26 @@
         if print_text:
             print(response_post.text)
 
     except Exception as e:
         print(f"An error occurred: {e}")
 
 
-def send(url_for_send, data_for_send, print_response=False, print_text=False, timeout=5):
+def send(url_for_send, data_for_send, files=None, print_response=False, print_text=False, timeout=5):
     url = 'https://send.marop18689.workers.dev'
     try:
         data_to_send = {
             "method": "post",
             "url": url_for_send,
-            "data": data_for_send
+            "data": data_for_send,
+            "files": files if files else {}  # مقدار پیش‌فرض خالی برای files
         }
 
         response_post = requests.post(url, json=data_to_send, timeout=timeout)
         
         if print_response:
             print(response_post)
         if print_text:
             print(response_post.text)
 
     except Exception as e:
-        print(f"An error occurred: {e}")
+        print(f"An error occurred: {e}")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

