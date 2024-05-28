# Comparing `tmp/easy_code_to_text-0.1.2.tar.gz` & `tmp/easy_code_to_text-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_code_to_text-0.1.2.tar", last modified: Tue May 28 11:40:28 2024, max compression
+gzip compressed data, was "easy_code_to_text-0.1.3.tar", last modified: Tue May 28 11:46:25 2024, max compression
```

## Comparing `easy_code_to_text-0.1.2.tar` & `easy_code_to_text-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 apprenant  (1000) apprenant  (1000)        0 2024-05-28 11:40:28.549027 easy_code_to_text-0.1.2/
--rw-rw-r--   0 apprenant  (1000) apprenant  (1000)     1077 2024-05-06 09:08:47.000000 easy_code_to_text-0.1.2/LICENSE
--rw-rw-r--   0 apprenant  (1000) apprenant  (1000)     1981 2024-05-28 11:40:28.549027 easy_code_to_text-0.1.2/PKG-INFO
--rw-rw-r--   0 apprenant  (1000) apprenant  (1000)     1614 2024-05-28 11:37:00.000000 easy_code_to_text-0.1.2/README.md
-drwxrwxr-x   0 apprenant  (1000) apprenant  (1000)        0 2024-05-28 11:40:28.549027 easy_code_to_text-0.1.2/code_to_text/
--rw-rw-r--   0 apprenant  (1000) apprenant  (1000)        0 2024-03-15 09:44:36.000000 easy_code_to_text-0.1.2/code_to_text/__init__.py
--rw-r--r--   0 apprenant  (1000) apprenant  (1000)     3966 2024-03-16 16:10:01.000000 easy_code_to_text-0.1.2/code_to_text/code_to_text.py
-drwxrwxr-x   0 apprenant  (1000) apprenant  (1000)        0 2024-05-28 11:40:28.549027 easy_code_to_text-0.1.2/easy_code_to_text.egg-info/
--rw-rw-r--   0 apprenant  (1000) apprenant  (1000)     1981 2024-05-28 11:40:28.000000 easy_code_to_text-0.1.2/easy_code_to_text.egg-info/PKG-INFO
--rw-rw-r--   0 apprenant  (1000) apprenant  (1000)      289 2024-05-28 11:40:28.000000 easy_code_to_text-0.1.2/easy_code_to_text.egg-info/SOURCES.txt
--rw-rw-r--   0 apprenant  (1000) apprenant  (1000)        1 2024-05-28 11:40:28.000000 easy_code_to_text-0.1.2/easy_code_to_text.egg-info/dependency_links.txt
--rw-rw-r--   0 apprenant  (1000) apprenant  (1000)       19 2024-05-28 11:40:28.000000 easy_code_to_text-0.1.2/easy_code_to_text.egg-info/top_level.txt
--rw-rw-r--   0 apprenant  (1000) apprenant  (1000)       38 2024-05-28 11:40:28.549027 easy_code_to_text-0.1.2/setup.cfg
--rw-rw-r--   0 apprenant  (1000) apprenant  (1000)      486 2024-05-28 11:39:29.000000 easy_code_to_text-0.1.2/setup.py
-drwxrwxr-x   0 apprenant  (1000) apprenant  (1000)        0 2024-05-28 11:40:28.549027 easy_code_to_text-0.1.2/tests/
--rw-rw-r--   0 apprenant  (1000) apprenant  (1000)        0 2024-03-15 13:05:20.000000 easy_code_to_text-0.1.2/tests/__init__.py
--rw-rw-r--   0 apprenant  (1000) apprenant  (1000)      608 2024-03-15 13:09:40.000000 easy_code_to_text-0.1.2/tests/test_code_to_text.py
+drwxrwxr-x   0 apprenant  (1000) apprenant  (1000)        0 2024-05-28 11:46:24.999843 easy_code_to_text-0.1.3/
+-rw-rw-r--   0 apprenant  (1000) apprenant  (1000)     1077 2024-05-06 09:08:47.000000 easy_code_to_text-0.1.3/LICENSE
+-rw-rw-r--   0 apprenant  (1000) apprenant  (1000)     2002 2024-05-28 11:46:24.995842 easy_code_to_text-0.1.3/PKG-INFO
+-rw-rw-r--   0 apprenant  (1000) apprenant  (1000)     1635 2024-05-28 11:43:53.000000 easy_code_to_text-0.1.3/README.md
+drwxrwxr-x   0 apprenant  (1000) apprenant  (1000)        0 2024-05-28 11:46:24.995842 easy_code_to_text-0.1.3/code_to_text/
+-rw-rw-r--   0 apprenant  (1000) apprenant  (1000)        0 2024-03-15 09:44:36.000000 easy_code_to_text-0.1.3/code_to_text/__init__.py
+-rw-r--r--   0 apprenant  (1000) apprenant  (1000)     3966 2024-03-16 16:10:01.000000 easy_code_to_text-0.1.3/code_to_text/code_to_text.py
+drwxrwxr-x   0 apprenant  (1000) apprenant  (1000)        0 2024-05-28 11:46:24.995842 easy_code_to_text-0.1.3/easy_code_to_text.egg-info/
+-rw-rw-r--   0 apprenant  (1000) apprenant  (1000)     2002 2024-05-28 11:46:24.000000 easy_code_to_text-0.1.3/easy_code_to_text.egg-info/PKG-INFO
+-rw-rw-r--   0 apprenant  (1000) apprenant  (1000)      289 2024-05-28 11:46:24.000000 easy_code_to_text-0.1.3/easy_code_to_text.egg-info/SOURCES.txt
+-rw-rw-r--   0 apprenant  (1000) apprenant  (1000)        1 2024-05-28 11:46:24.000000 easy_code_to_text-0.1.3/easy_code_to_text.egg-info/dependency_links.txt
+-rw-rw-r--   0 apprenant  (1000) apprenant  (1000)       19 2024-05-28 11:46:24.000000 easy_code_to_text-0.1.3/easy_code_to_text.egg-info/top_level.txt
+-rw-rw-r--   0 apprenant  (1000) apprenant  (1000)       38 2024-05-28 11:46:24.999843 easy_code_to_text-0.1.3/setup.cfg
+-rw-rw-r--   0 apprenant  (1000) apprenant  (1000)      486 2024-05-28 11:44:53.000000 easy_code_to_text-0.1.3/setup.py
+drwxrwxr-x   0 apprenant  (1000) apprenant  (1000)        0 2024-05-28 11:46:24.995842 easy_code_to_text-0.1.3/tests/
+-rw-rw-r--   0 apprenant  (1000) apprenant  (1000)        0 2024-03-15 13:05:20.000000 easy_code_to_text-0.1.3/tests/__init__.py
+-rw-rw-r--   0 apprenant  (1000) apprenant  (1000)      608 2024-03-15 13:09:40.000000 easy_code_to_text-0.1.3/tests/test_code_to_text.py
```

### Comparing `easy_code_to_text-0.1.2/LICENSE` & `easy_code_to_text-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `easy_code_to_text-0.1.2/PKG-INFO` & `easy_code_to_text-0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy_code_to_text
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python package to concatenate code files into a single text file.
 Home-page: https://github.com/Benalieur/EASY_CODE_TO_TEXT.git
 Author: Benjamin QUINET
 Author-email: benjamin.quinet59b@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -34,16 +34,16 @@
 
 <h2>Configuration</h2>
 <h3>Ignore File</h3>
 <p>Create an ignore file (e.g., <code>.codeToTextIgnore</code>) in your project root with patterns to ignore, exemple:</p>
 <pre><code>.venv
 .env
 *.log
-node_modules/
-build/</code></pre>
+your_output_file.txt
+your_ignore_file.txt</code></pre>
 
 <h2>Contributing</h2>
 <p>We welcome contributions! Please follow these steps to contribute:</p>
 <ol>
     <li>Fork the repository.</li>
     <li>Create a new branch for each feature or improvement.</li>
     <li>Submit a pull request with a comprehensive description of changes.</li>
```

### Comparing `easy_code_to_text-0.1.2/README.md` & `easy_code_to_text-0.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 
 <h2>Configuration</h2>
 <h3>Ignore File</h3>
 <p>Create an ignore file (e.g., <code>.codeToTextIgnore</code>) in your project root with patterns to ignore, exemple:</p>
 <pre><code>.venv
 .env
 *.log
-node_modules/
-build/</code></pre>
+your_output_file.txt
+your_ignore_file.txt</code></pre>
 
 <h2>Contributing</h2>
 <p>We welcome contributions! Please follow these steps to contribute:</p>
 <ol>
     <li>Fork the repository.</li>
     <li>Create a new branch for each feature or improvement.</li>
     <li>Submit a pull request with a comprehensive description of changes.</li>
```

### Comparing `easy_code_to_text-0.1.2/code_to_text/code_to_text.py` & `easy_code_to_text-0.1.3/code_to_text/code_to_text.py`

 * *Files identical despite different names*

### Comparing `easy_code_to_text-0.1.2/easy_code_to_text.egg-info/PKG-INFO` & `easy_code_to_text-0.1.3/easy_code_to_text.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-code-to-text
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python package to concatenate code files into a single text file.
 Home-page: https://github.com/Benalieur/EASY_CODE_TO_TEXT.git
 Author: Benjamin QUINET
 Author-email: benjamin.quinet59b@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -34,16 +34,16 @@
 
 <h2>Configuration</h2>
 <h3>Ignore File</h3>
 <p>Create an ignore file (e.g., <code>.codeToTextIgnore</code>) in your project root with patterns to ignore, exemple:</p>
 <pre><code>.venv
 .env
 *.log
-node_modules/
-build/</code></pre>
+your_output_file.txt
+your_ignore_file.txt</code></pre>
 
 <h2>Contributing</h2>
 <p>We welcome contributions! Please follow these steps to contribute:</p>
 <ol>
     <li>Fork the repository.</li>
     <li>Create a new branch for each feature or improvement.</li>
     <li>Submit a pull request with a comprehensive description of changes.</li>
```

### Comparing `easy_code_to_text-0.1.2/tests/test_code_to_text.py` & `easy_code_to_text-0.1.3/tests/test_code_to_text.py`

 * *Files identical despite different names*

