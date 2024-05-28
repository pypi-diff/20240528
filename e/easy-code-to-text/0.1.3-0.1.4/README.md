# Comparing `tmp/easy_code_to_text-0.1.3.tar.gz` & `tmp/easy_code_to_text-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_code_to_text-0.1.3.tar", last modified: Tue May 28 11:46:25 2024, max compression
+gzip compressed data, was "easy_code_to_text-0.1.4.tar", last modified: Tue May 28 11:59:41 2024, max compression
```

## Comparing `easy_code_to_text-0.1.3.tar` & `easy_code_to_text-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 apprenant  (1000) apprenant  (1000)        0 2024-05-28 11:46:24.999843 easy_code_to_text-0.1.3/
--rw-rw-r--   0 apprenant  (1000) apprenant  (1000)     1077 2024-05-06 09:08:47.000000 easy_code_to_text-0.1.3/LICENSE
--rw-rw-r--   0 apprenant  (1000) apprenant  (1000)     2002 2024-05-28 11:46:24.995842 easy_code_to_text-0.1.3/PKG-INFO
--rw-rw-r--   0 apprenant  (1000) apprenant  (1000)     1635 2024-05-28 11:43:53.000000 easy_code_to_text-0.1.3/README.md
-drwxrwxr-x   0 apprenant  (1000) apprenant  (1000)        0 2024-05-28 11:46:24.995842 easy_code_to_text-0.1.3/code_to_text/
--rw-rw-r--   0 apprenant  (1000) apprenant  (1000)        0 2024-03-15 09:44:36.000000 easy_code_to_text-0.1.3/code_to_text/__init__.py
--rw-r--r--   0 apprenant  (1000) apprenant  (1000)     3966 2024-03-16 16:10:01.000000 easy_code_to_text-0.1.3/code_to_text/code_to_text.py
-drwxrwxr-x   0 apprenant  (1000) apprenant  (1000)        0 2024-05-28 11:46:24.995842 easy_code_to_text-0.1.3/easy_code_to_text.egg-info/
--rw-rw-r--   0 apprenant  (1000) apprenant  (1000)     2002 2024-05-28 11:46:24.000000 easy_code_to_text-0.1.3/easy_code_to_text.egg-info/PKG-INFO
--rw-rw-r--   0 apprenant  (1000) apprenant  (1000)      289 2024-05-28 11:46:24.000000 easy_code_to_text-0.1.3/easy_code_to_text.egg-info/SOURCES.txt
--rw-rw-r--   0 apprenant  (1000) apprenant  (1000)        1 2024-05-28 11:46:24.000000 easy_code_to_text-0.1.3/easy_code_to_text.egg-info/dependency_links.txt
--rw-rw-r--   0 apprenant  (1000) apprenant  (1000)       19 2024-05-28 11:46:24.000000 easy_code_to_text-0.1.3/easy_code_to_text.egg-info/top_level.txt
--rw-rw-r--   0 apprenant  (1000) apprenant  (1000)       38 2024-05-28 11:46:24.999843 easy_code_to_text-0.1.3/setup.cfg
--rw-rw-r--   0 apprenant  (1000) apprenant  (1000)      486 2024-05-28 11:44:53.000000 easy_code_to_text-0.1.3/setup.py
-drwxrwxr-x   0 apprenant  (1000) apprenant  (1000)        0 2024-05-28 11:46:24.995842 easy_code_to_text-0.1.3/tests/
--rw-rw-r--   0 apprenant  (1000) apprenant  (1000)        0 2024-03-15 13:05:20.000000 easy_code_to_text-0.1.3/tests/__init__.py
--rw-rw-r--   0 apprenant  (1000) apprenant  (1000)      608 2024-03-15 13:09:40.000000 easy_code_to_text-0.1.3/tests/test_code_to_text.py
+drwxrwxr-x   0 apprenant  (1000) apprenant  (1000)        0 2024-05-28 11:59:41.009113 easy_code_to_text-0.1.4/
+-rw-rw-r--   0 apprenant  (1000) apprenant  (1000)     1077 2024-05-06 09:08:47.000000 easy_code_to_text-0.1.4/LICENSE
+-rw-rw-r--   0 apprenant  (1000) apprenant  (1000)     1903 2024-05-28 11:59:41.009113 easy_code_to_text-0.1.4/PKG-INFO
+-rw-rw-r--   0 apprenant  (1000) apprenant  (1000)     1536 2024-05-28 11:57:36.000000 easy_code_to_text-0.1.4/README.md
+drwxrwxr-x   0 apprenant  (1000) apprenant  (1000)        0 2024-05-28 11:59:41.009113 easy_code_to_text-0.1.4/code_to_text/
+-rw-rw-r--   0 apprenant  (1000) apprenant  (1000)        0 2024-03-15 09:44:36.000000 easy_code_to_text-0.1.4/code_to_text/__init__.py
+-rw-r--r--   0 apprenant  (1000) apprenant  (1000)     3966 2024-03-16 16:10:01.000000 easy_code_to_text-0.1.4/code_to_text/code_to_text.py
+drwxrwxr-x   0 apprenant  (1000) apprenant  (1000)        0 2024-05-28 11:59:41.009113 easy_code_to_text-0.1.4/easy_code_to_text.egg-info/
+-rw-rw-r--   0 apprenant  (1000) apprenant  (1000)     1903 2024-05-28 11:59:40.000000 easy_code_to_text-0.1.4/easy_code_to_text.egg-info/PKG-INFO
+-rw-rw-r--   0 apprenant  (1000) apprenant  (1000)      289 2024-05-28 11:59:40.000000 easy_code_to_text-0.1.4/easy_code_to_text.egg-info/SOURCES.txt
+-rw-rw-r--   0 apprenant  (1000) apprenant  (1000)        1 2024-05-28 11:59:40.000000 easy_code_to_text-0.1.4/easy_code_to_text.egg-info/dependency_links.txt
+-rw-rw-r--   0 apprenant  (1000) apprenant  (1000)       19 2024-05-28 11:59:40.000000 easy_code_to_text-0.1.4/easy_code_to_text.egg-info/top_level.txt
+-rw-rw-r--   0 apprenant  (1000) apprenant  (1000)       38 2024-05-28 11:59:41.009113 easy_code_to_text-0.1.4/setup.cfg
+-rw-rw-r--   0 apprenant  (1000) apprenant  (1000)      486 2024-05-28 11:58:12.000000 easy_code_to_text-0.1.4/setup.py
+drwxrwxr-x   0 apprenant  (1000) apprenant  (1000)        0 2024-05-28 11:59:41.009113 easy_code_to_text-0.1.4/tests/
+-rw-rw-r--   0 apprenant  (1000) apprenant  (1000)        0 2024-03-15 13:05:20.000000 easy_code_to_text-0.1.4/tests/__init__.py
+-rw-rw-r--   0 apprenant  (1000) apprenant  (1000)      608 2024-03-15 13:09:40.000000 easy_code_to_text-0.1.4/tests/test_code_to_text.py
```

### Comparing `easy_code_to_text-0.1.3/LICENSE` & `easy_code_to_text-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `easy_code_to_text-0.1.3/PKG-INFO` & `easy_code_to_text-0.1.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,55 +1,77 @@
 Metadata-Version: 2.1
 Name: easy_code_to_text
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python package to concatenate code files into a single text file.
 Home-page: https://github.com/Benalieur/EASY_CODE_TO_TEXT.git
 Author: Benjamin QUINET
 Author-email: benjamin.quinet59b@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<h1>easy_code_to_text Project</h1>
-<p>A Python package to concatenate code files into a single document, with support for multiple programming languages and customizable ignore patterns.</p>
 
-<h2>Features</h2>
-<ul>
-    <li>Support for multiple programming languages including Python, JavaScript, HTML, CSS, Java, and YAML.</li>
-    <li>Customizable ignore patterns to exclude specific files or directories.</li>
-    <li>Generates a single document with clear demarcation for each file's path and language.</li>
-</ul>
-
-<h2>Installation</h2>
-<p>The package can be installed via pip:</p>
-<pre><code>pip install easy-code-to-text</code></pre>
-
-<h2>Usage</h2>
-<p>After installation, you can use the package as follows:</p>
-<pre><code>from code_to_text.code_to_text import read_and_combine_files
+# easy_code_to_text Project
 
-read_and_combine_files(input_directory='your_code_directory',
-                       output_file='your_output_file.txt',
-                       ignore_file_path='your_ignore_file.txt')</code></pre>
+A Python package to concatenate code files into a single document, with support for multiple programming languages and customizable ignore patterns.
+
+## Features
+
+- Support for multiple programming languages including Python, JavaScript, HTML, CSS, Java, and YAML.
+- Customizable ignore patterns to exclude specific files or directories.
+- Generates a single document with clear demarcation for each file's path and language.
+
+## Installation
+
+The package can be installed via pip:
+
+```
+pip install easy-code-to-text
+```
+
+## Configuration
+
+### Ignore File
+
+Create an ignore file (e.g., `.codeToTextIgnore`) in your project root with patterns to ignore, example:
+
+```
+# Your environment files
+.venv
 
-<h2>Configuration</h2>
-<h3>Ignore File</h3>
-<p>Create an ignore file (e.g., <code>.codeToTextIgnore</code>) in your project root with patterns to ignore, exemple:</p>
-<pre><code>.venv
+# Your private files
 .env
+
+# Python cache and logs files
+__pycache__
 *.log
+
+# Your output and ignore file
 your_output_file.txt
-your_ignore_file.txt</code></pre>
+your_ignore_file.txt
+```
+
+## Usage
+
+After installation, you can use the package as follows:
+
+```py
+from code_to_text.code_to_text import read_and_combine_files
+
+read_and_combine_files(input_directory='your_code_directory',
+                       output_file='your_output_file.txt',
+                       ignore_file_path='your_ignore_file.txt')
+```
+
+## Contributing
+
+We welcome contributions! Please follow these steps to contribute:
 
-<h2>Contributing</h2>
-<p>We welcome contributions! Please follow these steps to contribute:</p>
-<ol>
-    <li>Fork the repository.</li>
-    <li>Create a new branch for each feature or improvement.</li>
-    <li>Submit a pull request with a comprehensive description of changes.</li>
-</ol>
+1. Fork the repository.
+2. Create a new branch for each feature or improvement.
+3. Submit a pull request with a comprehensive description of changes.
 
-<h2>License</h2>
-<p>This project is open source and available under the MIT License. Benjamin QUINET.</p>
+## License
 
+This project is open source and available under the MIT License. Benjamin QUINET.
```

### Comparing `easy_code_to_text-0.1.3/README.md` & `easy_code_to_text-0.1.4/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,64 @@
-<h1>easy_code_to_text Project</h1>
-<p>A Python package to concatenate code files into a single document, with support for multiple programming languages and customizable ignore patterns.</p>
 
-<h2>Features</h2>
-<ul>
-    <li>Support for multiple programming languages including Python, JavaScript, HTML, CSS, Java, and YAML.</li>
-    <li>Customizable ignore patterns to exclude specific files or directories.</li>
-    <li>Generates a single document with clear demarcation for each file's path and language.</li>
-</ul>
-
-<h2>Installation</h2>
-<p>The package can be installed via pip:</p>
-<pre><code>pip install easy-code-to-text</code></pre>
-
-<h2>Usage</h2>
-<p>After installation, you can use the package as follows:</p>
-<pre><code>from code_to_text.code_to_text import read_and_combine_files
+# easy_code_to_text Project
 
-read_and_combine_files(input_directory='your_code_directory',
-                       output_file='your_output_file.txt',
-                       ignore_file_path='your_ignore_file.txt')</code></pre>
+A Python package to concatenate code files into a single document, with support for multiple programming languages and customizable ignore patterns.
+
+## Features
+
+- Support for multiple programming languages including Python, JavaScript, HTML, CSS, Java, and YAML.
+- Customizable ignore patterns to exclude specific files or directories.
+- Generates a single document with clear demarcation for each file's path and language.
+
+## Installation
+
+The package can be installed via pip:
+
+```
+pip install easy-code-to-text
+```
+
+## Configuration
+
+### Ignore File
+
+Create an ignore file (e.g., `.codeToTextIgnore`) in your project root with patterns to ignore, example:
+
+```
+# Your environment files
+.venv
 
-<h2>Configuration</h2>
-<h3>Ignore File</h3>
-<p>Create an ignore file (e.g., <code>.codeToTextIgnore</code>) in your project root with patterns to ignore, exemple:</p>
-<pre><code>.venv
+# Your private files
 .env
+
+# Python cache and logs files
+__pycache__
 *.log
+
+# Your output and ignore file
 your_output_file.txt
-your_ignore_file.txt</code></pre>
+your_ignore_file.txt
+```
+
+## Usage
+
+After installation, you can use the package as follows:
+
+```py
+from code_to_text.code_to_text import read_and_combine_files
+
+read_and_combine_files(input_directory='your_code_directory',
+                       output_file='your_output_file.txt',
+                       ignore_file_path='your_ignore_file.txt')
+```
+
+## Contributing
+
+We welcome contributions! Please follow these steps to contribute:
+
+1. Fork the repository.
+2. Create a new branch for each feature or improvement.
+3. Submit a pull request with a comprehensive description of changes.
 
-<h2>Contributing</h2>
-<p>We welcome contributions! Please follow these steps to contribute:</p>
-<ol>
-    <li>Fork the repository.</li>
-    <li>Create a new branch for each feature or improvement.</li>
-    <li>Submit a pull request with a comprehensive description of changes.</li>
-</ol>
+## License
 
-<h2>License</h2>
-<p>This project is open source and available under the MIT License. Benjamin QUINET.</p>
+This project is open source and available under the MIT License. Benjamin QUINET.
```

### Comparing `easy_code_to_text-0.1.3/code_to_text/code_to_text.py` & `easy_code_to_text-0.1.4/code_to_text/code_to_text.py`

 * *Files identical despite different names*

### Comparing `easy_code_to_text-0.1.3/easy_code_to_text.egg-info/PKG-INFO` & `easy_code_to_text-0.1.4/easy_code_to_text.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,55 +1,77 @@
 Metadata-Version: 2.1
 Name: easy-code-to-text
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python package to concatenate code files into a single text file.
 Home-page: https://github.com/Benalieur/EASY_CODE_TO_TEXT.git
 Author: Benjamin QUINET
 Author-email: benjamin.quinet59b@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<h1>easy_code_to_text Project</h1>
-<p>A Python package to concatenate code files into a single document, with support for multiple programming languages and customizable ignore patterns.</p>
 
-<h2>Features</h2>
-<ul>
-    <li>Support for multiple programming languages including Python, JavaScript, HTML, CSS, Java, and YAML.</li>
-    <li>Customizable ignore patterns to exclude specific files or directories.</li>
-    <li>Generates a single document with clear demarcation for each file's path and language.</li>
-</ul>
-
-<h2>Installation</h2>
-<p>The package can be installed via pip:</p>
-<pre><code>pip install easy-code-to-text</code></pre>
-
-<h2>Usage</h2>
-<p>After installation, you can use the package as follows:</p>
-<pre><code>from code_to_text.code_to_text import read_and_combine_files
+# easy_code_to_text Project
 
-read_and_combine_files(input_directory='your_code_directory',
-                       output_file='your_output_file.txt',
-                       ignore_file_path='your_ignore_file.txt')</code></pre>
+A Python package to concatenate code files into a single document, with support for multiple programming languages and customizable ignore patterns.
+
+## Features
+
+- Support for multiple programming languages including Python, JavaScript, HTML, CSS, Java, and YAML.
+- Customizable ignore patterns to exclude specific files or directories.
+- Generates a single document with clear demarcation for each file's path and language.
+
+## Installation
+
+The package can be installed via pip:
+
+```
+pip install easy-code-to-text
+```
+
+## Configuration
+
+### Ignore File
+
+Create an ignore file (e.g., `.codeToTextIgnore`) in your project root with patterns to ignore, example:
+
+```
+# Your environment files
+.venv
 
-<h2>Configuration</h2>
-<h3>Ignore File</h3>
-<p>Create an ignore file (e.g., <code>.codeToTextIgnore</code>) in your project root with patterns to ignore, exemple:</p>
-<pre><code>.venv
+# Your private files
 .env
+
+# Python cache and logs files
+__pycache__
 *.log
+
+# Your output and ignore file
 your_output_file.txt
-your_ignore_file.txt</code></pre>
+your_ignore_file.txt
+```
+
+## Usage
+
+After installation, you can use the package as follows:
+
+```py
+from code_to_text.code_to_text import read_and_combine_files
+
+read_and_combine_files(input_directory='your_code_directory',
+                       output_file='your_output_file.txt',
+                       ignore_file_path='your_ignore_file.txt')
+```
+
+## Contributing
+
+We welcome contributions! Please follow these steps to contribute:
 
-<h2>Contributing</h2>
-<p>We welcome contributions! Please follow these steps to contribute:</p>
-<ol>
-    <li>Fork the repository.</li>
-    <li>Create a new branch for each feature or improvement.</li>
-    <li>Submit a pull request with a comprehensive description of changes.</li>
-</ol>
+1. Fork the repository.
+2. Create a new branch for each feature or improvement.
+3. Submit a pull request with a comprehensive description of changes.
 
-<h2>License</h2>
-<p>This project is open source and available under the MIT License. Benjamin QUINET.</p>
+## License
 
+This project is open source and available under the MIT License. Benjamin QUINET.
```

### Comparing `easy_code_to_text-0.1.3/tests/test_code_to_text.py` & `easy_code_to_text-0.1.4/tests/test_code_to_text.py`

 * *Files identical despite different names*

