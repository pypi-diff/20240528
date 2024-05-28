# Comparing `tmp/easy_code_to_text-0.1.1.tar.gz` & `tmp/easy_code_to_text-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_code_to_text-0.1.1.tar", last modified: Mon May  6 09:10:46 2024, max compression
+gzip compressed data, was "easy_code_to_text-0.1.6.tar", last modified: Tue May 28 12:14:51 2024, max compression
```

## Comparing `easy_code_to_text-0.1.1.tar` & `easy_code_to_text-0.1.6.tar`

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
+drwxrwxr-x   0 apprenant  (1000) apprenant  (1000)        0 2024-05-28 12:14:51.203421 easy_code_to_text-0.1.6/
+-rw-rw-r--   0 apprenant  (1000) apprenant  (1000)     1077 2024-05-06 09:08:47.000000 easy_code_to_text-0.1.6/LICENSE
+-rw-rw-r--   0 apprenant  (1000) apprenant  (1000)     1901 2024-05-28 12:14:51.203421 easy_code_to_text-0.1.6/PKG-INFO
+-rw-rw-r--   0 apprenant  (1000) apprenant  (1000)     1534 2024-05-28 12:02:21.000000 easy_code_to_text-0.1.6/README.md
+drwxrwxr-x   0 apprenant  (1000) apprenant  (1000)        0 2024-05-28 12:14:51.203421 easy_code_to_text-0.1.6/code_to_text/
+-rw-rw-r--   0 apprenant  (1000) apprenant  (1000)        0 2024-03-15 09:44:36.000000 easy_code_to_text-0.1.6/code_to_text/__init__.py
+-rw-r--r--   0 apprenant  (1000) apprenant  (1000)     3584 2024-05-28 12:09:20.000000 easy_code_to_text-0.1.6/code_to_text/code_to_text.py
+drwxrwxr-x   0 apprenant  (1000) apprenant  (1000)        0 2024-05-28 12:14:51.203421 easy_code_to_text-0.1.6/easy_code_to_text.egg-info/
+-rw-rw-r--   0 apprenant  (1000) apprenant  (1000)     1901 2024-05-28 12:14:51.000000 easy_code_to_text-0.1.6/easy_code_to_text.egg-info/PKG-INFO
+-rw-rw-r--   0 apprenant  (1000) apprenant  (1000)      289 2024-05-28 12:14:51.000000 easy_code_to_text-0.1.6/easy_code_to_text.egg-info/SOURCES.txt
+-rw-rw-r--   0 apprenant  (1000) apprenant  (1000)        1 2024-05-28 12:14:51.000000 easy_code_to_text-0.1.6/easy_code_to_text.egg-info/dependency_links.txt
+-rw-rw-r--   0 apprenant  (1000) apprenant  (1000)       19 2024-05-28 12:14:51.000000 easy_code_to_text-0.1.6/easy_code_to_text.egg-info/top_level.txt
+-rw-rw-r--   0 apprenant  (1000) apprenant  (1000)       38 2024-05-28 12:14:51.203421 easy_code_to_text-0.1.6/setup.cfg
+-rw-rw-r--   0 apprenant  (1000) apprenant  (1000)      486 2024-05-28 12:14:40.000000 easy_code_to_text-0.1.6/setup.py
+drwxrwxr-x   0 apprenant  (1000) apprenant  (1000)        0 2024-05-28 12:14:51.203421 easy_code_to_text-0.1.6/tests/
+-rw-rw-r--   0 apprenant  (1000) apprenant  (1000)        0 2024-03-15 13:05:20.000000 easy_code_to_text-0.1.6/tests/__init__.py
+-rw-rw-r--   0 apprenant  (1000) apprenant  (1000)      608 2024-03-15 13:09:40.000000 easy_code_to_text-0.1.6/tests/test_code_to_text.py
```

### Comparing `easy_code_to_text-0.1.1/LICENSE` & `easy_code_to_text-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `easy_code_to_text-0.1.1/PKG-INFO` & `easy_code_to_text-0.1.6/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,64 @@
-Metadata-Version: 2.1
-Name: easy_code_to_text
-Version: 0.1.1
-Summary: A Python package to concatenate code files into a single text file.
-Home-page: https://github.com/Benalieur/EASY_CODE_TO_TEXT.git
-Author: Benjamin QUINET
-Author-email: benjamin.quinet59b@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<h1>easy_code_to_text Project</h1>
-<p>A Python package to concatenate code files into a single document, with support for multiple programming languages and customizable ignore patterns.</p>
-
-<h2>Features</h2>
-<ul>
-    <li>Support for multiple programming languages including Python, JavaScript, HTML, CSS, Java, and YAML.</li>
-    <li>Customizable ignore patterns to exclude specific files or directories.</li>
-    <li>Generates a single document with clear demarcation for each file's path and language.</li>
-</ul>
-
-<h2>Installation</h2>
-<p>The package can be installed via pip:</p>
-<pre><code>pip install code_to_text</code></pre>
-
-<h2>Usage</h2>
-<p>After installation, you can use the package as follows:</p>
-<pre><code>from code_to_text import read_and_combine_files
+
+# easy_code_to_text Project
+
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
+
+# Your private files
+.env
+
+# Python cache and logs files
+__pycache__
+*.log
+
+# Your output and ignore file
+my_project_output.txt
+.codeToTextIgnore
+```
+
+## Usage
+
+After installation, you can use the package as follows:
+
+```py
+from code_to_text.code_to_text import read_and_combine_files
 
 read_and_combine_files(input_directory='your_code_directory',
                        output_file='your_output_file.txt',
-                       ignore_file_path='your_ignore_file.txt')</code></pre>
+                       ignore_file_path='your_ignore_file.txt')
+```
+
+## Contributing
 
-<h2>Configuration</h2>
-<h3>Ignore File</h3>
-<p>Create an ignore file (e.g., <code>.codeToTextIgnore</code>) in your project root with patterns to ignore:</p>
-<pre><code>*.log
-node_modules/
-build/</code></pre>
-
-<h2>Contributing</h2>
-<p>We welcome contributions! Please follow these steps to contribute:</p>
-<ol>
-    <li>Fork the repository.</li>
-    <li>Create a new branch for each feature or improvement.</li>
-    <li>Submit a pull request with a comprehensive description of changes.</li>
-</ol>
+We welcome contributions! Please follow these steps to contribute:
 
-<h2>License</h2>
-<p>This project is open source and available under the MIT License. Benjamin QUINET.</p>
+1. Fork the repository.
+2. Create a new branch for each feature or improvement.
+3. Submit a pull request with a comprehensive description of changes.
 
+## License
 
+This project is open source and available under the MIT License. Benjamin QUINET.
```

### Comparing `easy_code_to_text-0.1.1/code_to_text/code_to_text.py` & `easy_code_to_text-0.1.6/code_to_text/code_to_text.py`

 * *Files 16% similar despite different names*

```diff
@@ -84,17 +84,8 @@
                         content = infile.read()
                         # Write metadata and content to the output file
                         outfile.write(f"---\nPath: {relative_path}\nLanguage: {language}\n---\n")
                         outfile.write(f"```{language}\n")
                         outfile.write(content)
                         outfile.write("\n```\n\n")
                 except Exception as e:
-                    print(f"Unable to read file {file_path}: {e}")
-
-
-if __name__ == '__main__':
-
-    project_path = '/home/apprenant/Documents/Programmation/le_prix_demain_app'
-    output_file = '/home/apprenant/Documents/Programmation/le_prix_demain_app/code_to_text_project.txt'
-    ignore_file = '/home/apprenant/Documents/Programmation/le_prix_demain_app/text_ignore'
-
-    read_and_combine_files(project_path, output_file, ignore_file)
+                    print(f"Unable to read file {file_path}: {e}")
```

### Comparing `easy_code_to_text-0.1.1/easy_code_to_text.egg-info/PKG-INFO` & `easy_code_to_text-0.1.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,77 @@
 Metadata-Version: 2.1
-Name: easy-code-to-text
-Version: 0.1.1
+Name: easy_code_to_text
+Version: 0.1.6
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
-<pre><code>pip install code_to_text</code></pre>
-
-<h2>Usage</h2>
-<p>After installation, you can use the package as follows:</p>
-<pre><code>from code_to_text import read_and_combine_files
+# easy_code_to_text Project
+
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
+
+# Your private files
+.env
+
+# Python cache and logs files
+__pycache__
+*.log
+
+# Your output and ignore file
+my_project_output.txt
+.codeToTextIgnore
+```
+
+## Usage
+
+After installation, you can use the package as follows:
+
+```py
+from code_to_text.code_to_text import read_and_combine_files
 
 read_and_combine_files(input_directory='your_code_directory',
                        output_file='your_output_file.txt',
-                       ignore_file_path='your_ignore_file.txt')</code></pre>
+                       ignore_file_path='your_ignore_file.txt')
+```
+
+## Contributing
+
+We welcome contributions! Please follow these steps to contribute:
 
-<h2>Configuration</h2>
-<h3>Ignore File</h3>
-<p>Create an ignore file (e.g., <code>.codeToTextIgnore</code>) in your project root with patterns to ignore:</p>
-<pre><code>*.log
-node_modules/
-build/</code></pre>
-
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

### Comparing `easy_code_to_text-0.1.1/tests/test_code_to_text.py` & `easy_code_to_text-0.1.6/tests/test_code_to_text.py`

 * *Files identical despite different names*

