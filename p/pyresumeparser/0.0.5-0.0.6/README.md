# Comparing `tmp/pyresumeparser-0.0.5.tar.gz` & `tmp/pyresumeparser-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyresumeparser-0.0.5.tar", last modified: Tue May 28 11:22:17 2024, max compression
+gzip compressed data, was "pyresumeparser-0.0.6.tar", last modified: Tue May 28 11:39:35 2024, max compression
```

## Comparing `pyresumeparser-0.0.5.tar` & `pyresumeparser-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 pluto      (501) staff       (20)        0 2024-05-28 11:22:17.509692 pyresumeparser-0.0.5/
--rw-r--r--   0 pluto      (501) staff       (20)     2895 2024-05-28 11:22:17.508765 pyresumeparser-0.0.5/PKG-INFO
--rw-r--r--   0 pluto      (501) staff       (20)     2222 2024-05-28 11:13:33.000000 pyresumeparser-0.0.5/README.md
-drwxr-xr-x   0 pluto      (501) staff       (20)        0 2024-05-28 11:22:17.482152 pyresumeparser-0.0.5/pyresumeparser/
--rw-r--r--   0 pluto      (501) staff       (20)       44 2024-05-21 07:40:09.000000 pyresumeparser-0.0.5/pyresumeparser/__init__.py
--rw-r--r--   0 pluto      (501) staff       (20)     4716 2024-05-28 11:00:58.000000 pyresumeparser-0.0.5/pyresumeparser/main.py
-drwxr-xr-x   0 pluto      (501) staff       (20)        0 2024-05-28 11:22:17.501070 pyresumeparser-0.0.5/pyresumeparser.egg-info/
--rw-r--r--   0 pluto      (501) staff       (20)     2895 2024-05-28 11:22:17.000000 pyresumeparser-0.0.5/pyresumeparser.egg-info/PKG-INFO
--rw-r--r--   0 pluto      (501) staff       (20)      298 2024-05-28 11:22:17.000000 pyresumeparser-0.0.5/pyresumeparser.egg-info/SOURCES.txt
--rw-r--r--   0 pluto      (501) staff       (20)        1 2024-05-28 11:22:17.000000 pyresumeparser-0.0.5/pyresumeparser.egg-info/dependency_links.txt
--rw-r--r--   0 pluto      (501) staff       (20)       60 2024-05-28 11:22:17.000000 pyresumeparser-0.0.5/pyresumeparser.egg-info/entry_points.txt
--rw-r--r--   0 pluto      (501) staff       (20)       94 2024-05-28 11:22:17.000000 pyresumeparser-0.0.5/pyresumeparser.egg-info/requires.txt
--rw-r--r--   0 pluto      (501) staff       (20)       15 2024-05-28 11:22:17.000000 pyresumeparser-0.0.5/pyresumeparser.egg-info/top_level.txt
--rw-r--r--   0 pluto      (501) staff       (20)       38 2024-05-28 11:22:17.509885 pyresumeparser-0.0.5/setup.cfg
--rw-r--r--   0 pluto      (501) staff       (20)     1023 2024-05-28 11:08:58.000000 pyresumeparser-0.0.5/setup.py
+drwxr-xr-x   0 pluto      (501) staff       (20)        0 2024-05-28 11:39:35.107604 pyresumeparser-0.0.6/
+-rw-r--r--   0 pluto      (501) staff       (20)     2835 2024-05-28 11:39:35.106397 pyresumeparser-0.0.6/PKG-INFO
+-rw-r--r--   0 pluto      (501) staff       (20)     2162 2024-05-28 11:38:04.000000 pyresumeparser-0.0.6/README.md
+drwxr-xr-x   0 pluto      (501) staff       (20)        0 2024-05-28 11:39:35.092551 pyresumeparser-0.0.6/pyresumeparser/
+-rw-r--r--   0 pluto      (501) staff       (20)       44 2024-05-21 07:40:09.000000 pyresumeparser-0.0.6/pyresumeparser/__init__.py
+-rw-r--r--   0 pluto      (501) staff       (20)     4716 2024-05-28 11:00:58.000000 pyresumeparser-0.0.6/pyresumeparser/main.py
+drwxr-xr-x   0 pluto      (501) staff       (20)        0 2024-05-28 11:39:35.099685 pyresumeparser-0.0.6/pyresumeparser.egg-info/
+-rw-r--r--   0 pluto      (501) staff       (20)     2835 2024-05-28 11:39:34.000000 pyresumeparser-0.0.6/pyresumeparser.egg-info/PKG-INFO
+-rw-r--r--   0 pluto      (501) staff       (20)      298 2024-05-28 11:39:34.000000 pyresumeparser-0.0.6/pyresumeparser.egg-info/SOURCES.txt
+-rw-r--r--   0 pluto      (501) staff       (20)        1 2024-05-28 11:39:34.000000 pyresumeparser-0.0.6/pyresumeparser.egg-info/dependency_links.txt
+-rw-r--r--   0 pluto      (501) staff       (20)       60 2024-05-28 11:39:34.000000 pyresumeparser-0.0.6/pyresumeparser.egg-info/entry_points.txt
+-rw-r--r--   0 pluto      (501) staff       (20)       94 2024-05-28 11:39:34.000000 pyresumeparser-0.0.6/pyresumeparser.egg-info/requires.txt
+-rw-r--r--   0 pluto      (501) staff       (20)       15 2024-05-28 11:39:34.000000 pyresumeparser-0.0.6/pyresumeparser.egg-info/top_level.txt
+-rw-r--r--   0 pluto      (501) staff       (20)       38 2024-05-28 11:39:35.107761 pyresumeparser-0.0.6/setup.cfg
+-rw-r--r--   0 pluto      (501) staff       (20)     1023 2024-05-28 11:38:15.000000 pyresumeparser-0.0.6/setup.py
```

### Comparing `pyresumeparser-0.0.5/PKG-INFO` & `pyresumeparser-0.0.6/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,61 +1,36 @@
-Metadata-Version: 2.1
-Name: pyresumeparser
-Version: 0.0.5
-Summary: A package for parsing resume and extracting entities.
-Home-page: https://github.com/pkhan123/pyresumeparser
-Author: Palash Khan
-Author-email: palashkhan777@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Requires-Dist: pdfminer.six==20231228
-Requires-Dist: spacy==3.7.4
-Requires-Dist: spacy-transformers==1.3.5
-Requires-Dist: tqdm==4.66.4
-Provides-Extra: dev
-Requires-Dist: build; extra == "dev"
-Requires-Dist: twine; extra == "dev"
-
 # PyResumeParser
 
 PyResumeParser is a Python package designed to parse resume PDF files and extract key entities such as names, emails, phone numbers, education details, skills, and more. It utilizes `spaCy` and `pdfminer.six` for natural language processing and PDF text extraction.
 
 ## Installation
 
 You can install PyResumeParser using pip:
 
 ```bash
 pip install pyresumeparser
 Usage
 As a Python Module
 To use PyResumeParser in your Python code, you can import the package and call the parse_resume function:
 
-python
-Copy code
 import pyresumeparser
 
 pdf_file = "resume.pdf"
 parsed_resume = pyresumeparser.parse_resume(pdf_file)
 print(parsed_resume)
 From the Terminal
 You can also use PyResumeParser directly from the terminal:
 
-bash
-Copy code
 pyresumeparser resume.pdf
 This command will parse the specified PDF file and print the extracted entities in JSON format.
 
 Example Output
 Here is an example of the JSON output you might get from parsing a resume:
 
-json
-Copy code
+
 {
     "first_name": ["John"],
     "last_name": ["Doe"],
     "email": ["johndoe@example.com"],
     "phone": ["+1 234 567 890"],
     "country": ["USA"],
     "state": ["California"],
@@ -78,16 +53,15 @@
 
 spacy==3.7.4
 pdfminer.six==20231228
 spacy-transformers==1.3.5
 tqdm==4.66.4
 You can install these packages using pip:
 
-bash
-Copy code
+
 pip install -r requirements.txt
 Contributing
 Contributions are welcome! Please feel free to submit a Pull Request or open an issue on GitHub.
 
 License
 This project is licensed under the MIT License.
```

### Comparing `pyresumeparser-0.0.5/README.md` & `pyresumeparser-0.0.6/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,41 +1,56 @@
+Metadata-Version: 2.1
+Name: pyresumeparser
+Version: 0.0.6
+Summary: A package for parsing resume and extracting entities.
+Home-page: https://github.com/pkhan123/pyresumeparser
+Author: Palash Khan
+Author-email: palashkhan777@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Requires-Dist: pdfminer.six==20231228
+Requires-Dist: spacy==3.7.4
+Requires-Dist: spacy-transformers==1.3.5
+Requires-Dist: tqdm==4.66.4
+Provides-Extra: dev
+Requires-Dist: build; extra == "dev"
+Requires-Dist: twine; extra == "dev"
+
 # PyResumeParser
 
 PyResumeParser is a Python package designed to parse resume PDF files and extract key entities such as names, emails, phone numbers, education details, skills, and more. It utilizes `spaCy` and `pdfminer.six` for natural language processing and PDF text extraction.
 
 ## Installation
 
 You can install PyResumeParser using pip:
 
 ```bash
 pip install pyresumeparser
 Usage
 As a Python Module
 To use PyResumeParser in your Python code, you can import the package and call the parse_resume function:
 
-python
-Copy code
 import pyresumeparser
 
 pdf_file = "resume.pdf"
 parsed_resume = pyresumeparser.parse_resume(pdf_file)
 print(parsed_resume)
 From the Terminal
 You can also use PyResumeParser directly from the terminal:
 
-bash
-Copy code
 pyresumeparser resume.pdf
 This command will parse the specified PDF file and print the extracted entities in JSON format.
 
 Example Output
 Here is an example of the JSON output you might get from parsing a resume:
 
-json
-Copy code
+
 {
     "first_name": ["John"],
     "last_name": ["Doe"],
     "email": ["johndoe@example.com"],
     "phone": ["+1 234 567 890"],
     "country": ["USA"],
     "state": ["California"],
@@ -58,16 +73,15 @@
 
 spacy==3.7.4
 pdfminer.six==20231228
 spacy-transformers==1.3.5
 tqdm==4.66.4
 You can install these packages using pip:
 
-bash
-Copy code
+
 pip install -r requirements.txt
 Contributing
 Contributions are welcome! Please feel free to submit a Pull Request or open an issue on GitHub.
 
 License
 This project is licensed under the MIT License.
```

### Comparing `pyresumeparser-0.0.5/pyresumeparser/main.py` & `pyresumeparser-0.0.6/pyresumeparser/main.py`

 * *Files identical despite different names*

### Comparing `pyresumeparser-0.0.5/pyresumeparser.egg-info/PKG-INFO` & `pyresumeparser-0.0.6/pyresumeparser.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyresumeparser
-Version: 0.0.5
+Version: 0.0.6
 Summary: A package for parsing resume and extracting entities.
 Home-page: https://github.com/pkhan123/pyresumeparser
 Author: Palash Khan
 Author-email: palashkhan777@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -28,34 +28,29 @@
 
 ```bash
 pip install pyresumeparser
 Usage
 As a Python Module
 To use PyResumeParser in your Python code, you can import the package and call the parse_resume function:
 
-python
-Copy code
 import pyresumeparser
 
 pdf_file = "resume.pdf"
 parsed_resume = pyresumeparser.parse_resume(pdf_file)
 print(parsed_resume)
 From the Terminal
 You can also use PyResumeParser directly from the terminal:
 
-bash
-Copy code
 pyresumeparser resume.pdf
 This command will parse the specified PDF file and print the extracted entities in JSON format.
 
 Example Output
 Here is an example of the JSON output you might get from parsing a resume:
 
-json
-Copy code
+
 {
     "first_name": ["John"],
     "last_name": ["Doe"],
     "email": ["johndoe@example.com"],
     "phone": ["+1 234 567 890"],
     "country": ["USA"],
     "state": ["California"],
@@ -78,16 +73,15 @@
 
 spacy==3.7.4
 pdfminer.six==20231228
 spacy-transformers==1.3.5
 tqdm==4.66.4
 You can install these packages using pip:
 
-bash
-Copy code
+
 pip install -r requirements.txt
 Contributing
 Contributions are welcome! Please feel free to submit a Pull Request or open an issue on GitHub.
 
 License
 This project is licensed under the MIT License.
```

### Comparing `pyresumeparser-0.0.5/setup.py` & `pyresumeparser-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from setuptools import setup, find_packages
 
 setup(
     name='pyresumeparser',
-    version='0.0.5',
+    version='0.0.6',
     packages=find_packages(),
     install_requires=[
         'pdfminer.six==20231228',
         'spacy==3.7.4',
         'spacy-transformers==1.3.5',
         'tqdm==4.66.4'
     ],
```

