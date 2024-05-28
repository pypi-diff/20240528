# Comparing `tmp/easy_code_to_text-0.1.1.tar.gz` & `tmp/easy_code_to_text-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_code_to_text-0.1.1.tar", last modified: Mon May  6 09:10:46 2024, max compression
+gzip compressed data, was "easy_code_to_text-0.1.2.tar", last modified: Tue May 28 11:40:28 2024, max compression
```

## Comparing `easy_code_to_text-0.1.1.tar` & `easy_code_to_text-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 apprenant  (1000) apprenant  (1000)        0 2024-05-06 09:10:45.996527 easy_code_to_text-0.1.1/
--rw-rw-r--   0 apprenant  (1000) apprenant  (1000)     1077 2024-05-06 09:08:47.000000 easy_code_to_text-0.1.1/LICENSE
--rw-rw-r--   0 apprenant  (1000) apprenant  (1000)     1943 2024-05-06 09:10:45.996527 easy_code_to_text-0.1.1/PKG-INFO
--rw-rw-r--   0 apprenant  (1000) apprenant  (1000)     1576 2024-05-06 08:54:43.000000 easy_code_to_text-0.1.1/README.md
-drwxrwxr-x   0 apprenant  (1000) apprenant  (1000)        0 2024-05-06 09:10:45.996527 easy_code_to_text-0.1.1/code_to_text/
--rw-rw-r--   0 apprenant  (1000) apprenant  (1000)        0 2024-03-15 09:44:36.000000 easy_code_to_text-0.1.1/code_to_text/__init__.py
--rw-r--r--   0 apprenant  (1000) apprenant  (1000)     3966 2024-03-16 16:10:01.000000 easy_code_to_text-0.1.1/code_to_text/code_to_text.py
-drwxrwxr-x   0 apprenant  (1000) apprenant  (1000)        0 2024-05-06 09:10:45.996527 easy_code_to_text-0.1.1/easy_code_to_text.egg-info/
--rw-rw-r--   0 apprenant  (1000) apprenant  (1000)     1943 2024-05-06 09:10:45.000000 easy_code_to_text-0.1.1/easy_code_to_text.egg-info/PKG-INFO
--rw-rw-r--   0 apprenant  (1000) apprenant  (1000)      289 2024-05-06 09:10:45.000000 easy_code_to_text-0.1.1/easy_code_to_text.egg-info/SOURCES.txt
--rw-rw-r--   0 apprenant  (1000) apprenant  (1000)        1 2024-05-06 09:10:45.000000 easy_code_to_text-0.1.1/easy_code_to_text.egg-info/dependency_links.txt
--rw-rw-r--   0 apprenant  (1000) apprenant  (1000)       19 2024-05-06 09:10:45.000000 easy_code_to_text-0.1.1/easy_code_to_text.egg-info/top_level.txt
--rw-rw-r--   0 apprenant  (1000) apprenant  (1000)       38 2024-05-06 09:10:45.996527 easy_code_to_text-0.1.1/setup.cfg
--rw-rw-r--   0 apprenant  (1000) apprenant  (1000)      486 2024-05-06 09:10:13.000000 easy_code_to_text-0.1.1/setup.py
-drwxrwxr-x   0 apprenant  (1000) apprenant  (1000)        0 2024-05-06 09:10:45.996527 easy_code_to_text-0.1.1/tests/
--rw-rw-r--   0 apprenant  (1000) apprenant  (1000)        0 2024-03-15 13:05:20.000000 easy_code_to_text-0.1.1/tests/__init__.py
--rw-rw-r--   0 apprenant  (1000) apprenant  (1000)      608 2024-03-15 13:09:40.000000 easy_code_to_text-0.1.1/tests/test_code_to_text.py
+drwxrwxr-x   0 apprenant  (1000) apprenant  (1000)        0 2024-05-28 11:40:28.549027 easy_code_to_text-0.1.2/
+-rw-rw-r--   0 apprenant  (1000) apprenant  (1000)     1077 2024-05-06 09:08:47.000000 easy_code_to_text-0.1.2/LICENSE
+-rw-rw-r--   0 apprenant  (1000) apprenant  (1000)     1981 2024-05-28 11:40:28.549027 easy_code_to_text-0.1.2/PKG-INFO
+-rw-rw-r--   0 apprenant  (1000) apprenant  (1000)     1614 2024-05-28 11:37:00.000000 easy_code_to_text-0.1.2/README.md
+drwxrwxr-x   0 apprenant  (1000) apprenant  (1000)        0 2024-05-28 11:40:28.549027 easy_code_to_text-0.1.2/code_to_text/
+-rw-rw-r--   0 apprenant  (1000) apprenant  (1000)        0 2024-03-15 09:44:36.000000 easy_code_to_text-0.1.2/code_to_text/__init__.py
+-rw-r--r--   0 apprenant  (1000) apprenant  (1000)     3966 2024-03-16 16:10:01.000000 easy_code_to_text-0.1.2/code_to_text/code_to_text.py
+drwxrwxr-x   0 apprenant  (1000) apprenant  (1000)        0 2024-05-28 11:40:28.549027 easy_code_to_text-0.1.2/easy_code_to_text.egg-info/
+-rw-rw-r--   0 apprenant  (1000) apprenant  (1000)     1981 2024-05-28 11:40:28.000000 easy_code_to_text-0.1.2/easy_code_to_text.egg-info/PKG-INFO
+-rw-rw-r--   0 apprenant  (1000) apprenant  (1000)      289 2024-05-28 11:40:28.000000 easy_code_to_text-0.1.2/easy_code_to_text.egg-info/SOURCES.txt
+-rw-rw-r--   0 apprenant  (1000) apprenant  (1000)        1 2024-05-28 11:40:28.000000 easy_code_to_text-0.1.2/easy_code_to_text.egg-info/dependency_links.txt
+-rw-rw-r--   0 apprenant  (1000) apprenant  (1000)       19 2024-05-28 11:40:28.000000 easy_code_to_text-0.1.2/easy_code_to_text.egg-info/top_level.txt
+-rw-rw-r--   0 apprenant  (1000) apprenant  (1000)       38 2024-05-28 11:40:28.549027 easy_code_to_text-0.1.2/setup.cfg
+-rw-rw-r--   0 apprenant  (1000) apprenant  (1000)      486 2024-05-28 11:39:29.000000 easy_code_to_text-0.1.2/setup.py
+drwxrwxr-x   0 apprenant  (1000) apprenant  (1000)        0 2024-05-28 11:40:28.549027 easy_code_to_text-0.1.2/tests/
+-rw-rw-r--   0 apprenant  (1000) apprenant  (1000)        0 2024-03-15 13:05:20.000000 easy_code_to_text-0.1.2/tests/__init__.py
+-rw-rw-r--   0 apprenant  (1000) apprenant  (1000)      608 2024-03-15 13:09:40.000000 easy_code_to_text-0.1.2/tests/test_code_to_text.py
```

### Comparing `easy_code_to_text-0.1.1/LICENSE` & `easy_code_to_text-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `easy_code_to_text-0.1.1/PKG-INFO` & `easy_code_to_text-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy_code_to_text
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python package to concatenate code files into a single text file.
 Home-page: https://github.com/Benalieur/EASY_CODE_TO_TEXT.git
 Author: Benjamin QUINET
 Author-email: benjamin.quinet59b@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -18,28 +18,30 @@
     <li>Support for multiple programming languages including Python, JavaScript, HTML, CSS, Java, and YAML.</li>
     <li>Customizable ignore patterns to exclude specific files or directories.</li>
     <li>Generates a single document with clear demarcation for each file's path and language.</li>
 </ul>
 
 <h2>Installation</h2>
 <p>The package can be installed via pip:</p>
-<pre><code>pip install code_to_text</code></pre>
+<pre><code>pip install easy-code-to-text</code></pre>
 
 <h2>Usage</h2>
 <p>After installation, you can use the package as follows:</p>
-<pre><code>from code_to_text import read_and_combine_files
+<pre><code>from code_to_text.code_to_text import read_and_combine_files
 
 read_and_combine_files(input_directory='your_code_directory',
                        output_file='your_output_file.txt',
                        ignore_file_path='your_ignore_file.txt')</code></pre>
 
 <h2>Configuration</h2>
 <h3>Ignore File</h3>
-<p>Create an ignore file (e.g., <code>.codeToTextIgnore</code>) in your project root with patterns to ignore:</p>
-<pre><code>*.log
+<p>Create an ignore file (e.g., <code>.codeToTextIgnore</code>) in your project root with patterns to ignore, exemple:</p>
+<pre><code>.venv
+.env
+*.log
 node_modules/
 build/</code></pre>
 
 <h2>Contributing</h2>
 <p>We welcome contributions! Please follow these steps to contribute:</p>
 <ol>
     <li>Fork the repository.</li>
```

### Comparing `easy_code_to_text-0.1.1/README.md` & `easy_code_to_text-0.1.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -6,28 +6,30 @@
     <li>Support for multiple programming languages including Python, JavaScript, HTML, CSS, Java, and YAML.</li>
     <li>Customizable ignore patterns to exclude specific files or directories.</li>
     <li>Generates a single document with clear demarcation for each file's path and language.</li>
 </ul>
 
 <h2>Installation</h2>
 <p>The package can be installed via pip:</p>
-<pre><code>pip install code_to_text</code></pre>
+<pre><code>pip install easy-code-to-text</code></pre>
 
 <h2>Usage</h2>
 <p>After installation, you can use the package as follows:</p>
-<pre><code>from code_to_text import read_and_combine_files
+<pre><code>from code_to_text.code_to_text import read_and_combine_files
 
 read_and_combine_files(input_directory='your_code_directory',
                        output_file='your_output_file.txt',
                        ignore_file_path='your_ignore_file.txt')</code></pre>
 
 <h2>Configuration</h2>
 <h3>Ignore File</h3>
-<p>Create an ignore file (e.g., <code>.codeToTextIgnore</code>) in your project root with patterns to ignore:</p>
-<pre><code>*.log
+<p>Create an ignore file (e.g., <code>.codeToTextIgnore</code>) in your project root with patterns to ignore, exemple:</p>
+<pre><code>.venv
+.env
+*.log
 node_modules/
 build/</code></pre>
 
 <h2>Contributing</h2>
 <p>We welcome contributions! Please follow these steps to contribute:</p>
 <ol>
     <li>Fork the repository.</li>
```

### Comparing `easy_code_to_text-0.1.1/code_to_text/code_to_text.py` & `easy_code_to_text-0.1.2/code_to_text/code_to_text.py`

 * *Files identical despite different names*

### Comparing `easy_code_to_text-0.1.1/easy_code_to_text.egg-info/PKG-INFO` & `easy_code_to_text-0.1.2/easy_code_to_text.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-code-to-text
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python package to concatenate code files into a single text file.
 Home-page: https://github.com/Benalieur/EASY_CODE_TO_TEXT.git
 Author: Benjamin QUINET
 Author-email: benjamin.quinet59b@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -18,28 +18,30 @@
     <li>Support for multiple programming languages including Python, JavaScript, HTML, CSS, Java, and YAML.</li>
     <li>Customizable ignore patterns to exclude specific files or directories.</li>
     <li>Generates a single document with clear demarcation for each file's path and language.</li>
 </ul>
 
 <h2>Installation</h2>
 <p>The package can be installed via pip:</p>
-<pre><code>pip install code_to_text</code></pre>
+<pre><code>pip install easy-code-to-text</code></pre>
 
 <h2>Usage</h2>
 <p>After installation, you can use the package as follows:</p>
-<pre><code>from code_to_text import read_and_combine_files
+<pre><code>from code_to_text.code_to_text import read_and_combine_files
 
 read_and_combine_files(input_directory='your_code_directory',
                        output_file='your_output_file.txt',
                        ignore_file_path='your_ignore_file.txt')</code></pre>
 
 <h2>Configuration</h2>
 <h3>Ignore File</h3>
-<p>Create an ignore file (e.g., <code>.codeToTextIgnore</code>) in your project root with patterns to ignore:</p>
-<pre><code>*.log
+<p>Create an ignore file (e.g., <code>.codeToTextIgnore</code>) in your project root with patterns to ignore, exemple:</p>
+<pre><code>.venv
+.env
+*.log
 node_modules/
 build/</code></pre>
 
 <h2>Contributing</h2>
 <p>We welcome contributions! Please follow these steps to contribute:</p>
 <ol>
     <li>Fork the repository.</li>
```

### Comparing `easy_code_to_text-0.1.1/tests/test_code_to_text.py` & `easy_code_to_text-0.1.2/tests/test_code_to_text.py`

 * *Files identical despite different names*

