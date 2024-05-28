# Comparing `tmp/pyresumeparser-0.0.3.tar.gz` & `tmp/pyresumeparser-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyresumeparser-0.0.3.tar", last modified: Tue May 21 09:14:20 2024, max compression
+gzip compressed data, was "pyresumeparser-0.0.5.tar", last modified: Tue May 28 11:22:17 2024, max compression
```

## Comparing `pyresumeparser-0.0.3.tar` & `pyresumeparser-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,15 @@
-drwxr-xr-x   0 pluto      (501) staff       (20)        0 2024-05-21 09:14:20.273957 pyresumeparser-0.0.3/
--rw-r--r--   0 pluto      (501) staff       (20)       35 2024-05-21 08:12:01.000000 pyresumeparser-0.0.3/MANIFEST.in
--rw-r--r--   0 pluto      (501) staff       (20)     2723 2024-05-21 09:14:20.272801 pyresumeparser-0.0.3/PKG-INFO
--rw-r--r--   0 pluto      (501) staff       (20)     2172 2024-05-21 08:41:25.000000 pyresumeparser-0.0.3/README.md
-drwxr-xr-x   0 pluto      (501) staff       (20)        0 2024-05-21 09:14:20.271500 pyresumeparser-0.0.3/pyresumeparser.egg-info/
--rw-r--r--   0 pluto      (501) staff       (20)     2723 2024-05-21 09:14:20.000000 pyresumeparser-0.0.3/pyresumeparser.egg-info/PKG-INFO
--rw-r--r--   0 pluto      (501) staff       (20)      414 2024-05-21 09:14:20.000000 pyresumeparser-0.0.3/pyresumeparser.egg-info/SOURCES.txt
--rw-r--r--   0 pluto      (501) staff       (20)        1 2024-05-21 09:14:20.000000 pyresumeparser-0.0.3/pyresumeparser.egg-info/dependency_links.txt
--rw-r--r--   0 pluto      (501) staff       (20)       59 2024-05-21 09:14:20.000000 pyresumeparser-0.0.3/pyresumeparser.egg-info/entry_points.txt
--rw-r--r--   0 pluto      (501) staff       (20)       62 2024-05-21 09:14:20.000000 pyresumeparser-0.0.3/pyresumeparser.egg-info/requires.txt
--rw-r--r--   0 pluto      (501) staff       (20)       14 2024-05-21 09:14:20.000000 pyresumeparser-0.0.3/pyresumeparser.egg-info/top_level.txt
-drwxr-xr-x   0 pluto      (501) staff       (20)        0 2024-05-21 09:14:20.267179 pyresumeparser-0.0.3/resume_parser/
--rw-r--r--   0 pluto      (501) staff       (20)       44 2024-05-21 07:40:09.000000 pyresumeparser-0.0.3/resume_parser/__init__.py
--rw-r--r--   0 pluto      (501) staff       (20)     2914 2024-05-21 09:04:27.000000 pyresumeparser-0.0.3/resume_parser/main.py
-drwxr-xr-x   0 pluto      (501) staff       (20)        0 2024-05-21 09:14:20.270121 pyresumeparser-0.0.3/resume_parser/model-best/
--rw-r--r--   0 pluto      (501) staff       (20)     2885 2024-05-15 13:00:41.000000 pyresumeparser-0.0.3/resume_parser/model-best/config.cfg
--rw-r--r--   0 pluto      (501) staff       (20)     2499 2024-05-15 13:00:41.000000 pyresumeparser-0.0.3/resume_parser/model-best/meta.json
--rw-r--r--   0 pluto      (501) staff       (20)    77066 2024-05-15 13:00:40.000000 pyresumeparser-0.0.3/resume_parser/model-best/tokenizer
--rw-r--r--   0 pluto      (501) staff       (20)       38 2024-05-21 09:14:20.274150 pyresumeparser-0.0.3/setup.cfg
--rw-r--r--   0 pluto      (501) staff       (20)     1046 2024-05-21 09:03:44.000000 pyresumeparser-0.0.3/setup.py
+drwxr-xr-x   0 pluto      (501) staff       (20)        0 2024-05-28 11:22:17.509692 pyresumeparser-0.0.5/
+-rw-r--r--   0 pluto      (501) staff       (20)     2895 2024-05-28 11:22:17.508765 pyresumeparser-0.0.5/PKG-INFO
+-rw-r--r--   0 pluto      (501) staff       (20)     2222 2024-05-28 11:13:33.000000 pyresumeparser-0.0.5/README.md
+drwxr-xr-x   0 pluto      (501) staff       (20)        0 2024-05-28 11:22:17.482152 pyresumeparser-0.0.5/pyresumeparser/
+-rw-r--r--   0 pluto      (501) staff       (20)       44 2024-05-21 07:40:09.000000 pyresumeparser-0.0.5/pyresumeparser/__init__.py
+-rw-r--r--   0 pluto      (501) staff       (20)     4716 2024-05-28 11:00:58.000000 pyresumeparser-0.0.5/pyresumeparser/main.py
+drwxr-xr-x   0 pluto      (501) staff       (20)        0 2024-05-28 11:22:17.501070 pyresumeparser-0.0.5/pyresumeparser.egg-info/
+-rw-r--r--   0 pluto      (501) staff       (20)     2895 2024-05-28 11:22:17.000000 pyresumeparser-0.0.5/pyresumeparser.egg-info/PKG-INFO
+-rw-r--r--   0 pluto      (501) staff       (20)      298 2024-05-28 11:22:17.000000 pyresumeparser-0.0.5/pyresumeparser.egg-info/SOURCES.txt
+-rw-r--r--   0 pluto      (501) staff       (20)        1 2024-05-28 11:22:17.000000 pyresumeparser-0.0.5/pyresumeparser.egg-info/dependency_links.txt
+-rw-r--r--   0 pluto      (501) staff       (20)       60 2024-05-28 11:22:17.000000 pyresumeparser-0.0.5/pyresumeparser.egg-info/entry_points.txt
+-rw-r--r--   0 pluto      (501) staff       (20)       94 2024-05-28 11:22:17.000000 pyresumeparser-0.0.5/pyresumeparser.egg-info/requires.txt
+-rw-r--r--   0 pluto      (501) staff       (20)       15 2024-05-28 11:22:17.000000 pyresumeparser-0.0.5/pyresumeparser.egg-info/top_level.txt
+-rw-r--r--   0 pluto      (501) staff       (20)       38 2024-05-28 11:22:17.509885 pyresumeparser-0.0.5/setup.cfg
+-rw-r--r--   0 pluto      (501) staff       (20)     1023 2024-05-28 11:08:58.000000 pyresumeparser-0.0.5/setup.py
```

### Comparing `pyresumeparser-0.0.3/PKG-INFO` & `pyresumeparser-0.0.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,58 +1,61 @@
 Metadata-Version: 2.1
 Name: pyresumeparser
-Version: 0.0.3
+Version: 0.0.5
 Summary: A package for parsing resume and extracting entities.
-Home-page: https://github.com/pkhan123/resume_parser
+Home-page: https://github.com/pkhan123/pyresumeparser
 Author: Palash Khan
 Author-email: palashkhan777@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pdfminer.six==20231228
 Requires-Dist: spacy==3.7.4
 Requires-Dist: spacy-transformers==1.3.5
+Requires-Dist: tqdm==4.66.4
+Provides-Extra: dev
+Requires-Dist: build; extra == "dev"
+Requires-Dist: twine; extra == "dev"
 
-# ResumeParser
+# PyResumeParser
 
-ResumeParser is a Python package designed to parse resume PDF files and extract key entities such as names, emails, phone numbers, education details, skills, and more. It utilizes `spaCy` and `pdfminer.six` for natural language processing and PDF text extraction.
+PyResumeParser is a Python package designed to parse resume PDF files and extract key entities such as names, emails, phone numbers, education details, skills, and more. It utilizes `spaCy` and `pdfminer.six` for natural language processing and PDF text extraction.
 
 ## Installation
 
-You can install ResumeParser using pip:
+You can install PyResumeParser using pip:
 
 ```bash
-pip install resumeparser
-
-
+pip install pyresumeparser
 Usage
 As a Python Module
-To use ResumeParser in your Python code, you can import the package and call the parse_resume function:
+To use PyResumeParser in your Python code, you can import the package and call the parse_resume function:
 
-import resumeparser
+python
+Copy code
+import pyresumeparser
 
 pdf_file = "resume.pdf"
-parsed_resume = resumeparser.parse_resume(pdf_file)
+parsed_resume = pyresumeparser.parse_resume(pdf_file)
 print(parsed_resume)
-
-
 From the Terminal
-You can also use ResumeParser directly from the terminal:
+You can also use PyResumeParser directly from the terminal:
 
+bash
+Copy code
 pyresumeparser resume.pdf
-
-
 This command will parse the specified PDF file and print the extracted entities in JSON format.
 
-
 Example Output
 Here is an example of the JSON output you might get from parsing a resume:
 
+json
+Copy code
 {
     "first_name": ["John"],
     "last_name": ["Doe"],
     "email": ["johndoe@example.com"],
     "phone": ["+1 234 567 890"],
     "country": ["USA"],
     "state": ["California"],
@@ -66,29 +69,30 @@
     "projects_worked": ["Project A", "Project B"],
     "skills": ["Python", "Machine Learning", "Data Analysis"],
     "total_experience": ["5 years"],
     "language": ["English"],
     "linkedin": ["https://linkedin.com/in/johndoe"],
     "github": ["https://github.com/johndoe"]
 }
-
 Requirements
-The following packages are required to use ResumeParser:
+The following packages are required to use PyResumeParser:
 
 spacy==3.7.4
 pdfminer.six==20231228
 spacy-transformers==1.3.5
+tqdm==4.66.4
 You can install these packages using pip:
 
+bash
+Copy code
 pip install -r requirements.txt
-
-
 Contributing
 Contributions are welcome! Please feel free to submit a Pull Request or open an issue on GitHub.
 
 License
-This project is licensed under the MIT License - see the LICENSE file for details.
+This project is licensed under the MIT License.
 
 Author
 Developed by Palash Khan.
 
 Feel free to reach out with any questions or feedback. Happy parsing!
+
```

### Comparing `pyresumeparser-0.0.3/pyresumeparser.egg-info/PKG-INFO` & `pyresumeparser-0.0.5/pyresumeparser.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,58 +1,61 @@
 Metadata-Version: 2.1
 Name: pyresumeparser
-Version: 0.0.3
+Version: 0.0.5
 Summary: A package for parsing resume and extracting entities.
-Home-page: https://github.com/pkhan123/resume_parser
+Home-page: https://github.com/pkhan123/pyresumeparser
 Author: Palash Khan
 Author-email: palashkhan777@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pdfminer.six==20231228
 Requires-Dist: spacy==3.7.4
 Requires-Dist: spacy-transformers==1.3.5
+Requires-Dist: tqdm==4.66.4
+Provides-Extra: dev
+Requires-Dist: build; extra == "dev"
+Requires-Dist: twine; extra == "dev"
 
-# ResumeParser
+# PyResumeParser
 
-ResumeParser is a Python package designed to parse resume PDF files and extract key entities such as names, emails, phone numbers, education details, skills, and more. It utilizes `spaCy` and `pdfminer.six` for natural language processing and PDF text extraction.
+PyResumeParser is a Python package designed to parse resume PDF files and extract key entities such as names, emails, phone numbers, education details, skills, and more. It utilizes `spaCy` and `pdfminer.six` for natural language processing and PDF text extraction.
 
 ## Installation
 
-You can install ResumeParser using pip:
+You can install PyResumeParser using pip:
 
 ```bash
-pip install resumeparser
-
-
+pip install pyresumeparser
 Usage
 As a Python Module
-To use ResumeParser in your Python code, you can import the package and call the parse_resume function:
+To use PyResumeParser in your Python code, you can import the package and call the parse_resume function:
 
-import resumeparser
+python
+Copy code
+import pyresumeparser
 
 pdf_file = "resume.pdf"
-parsed_resume = resumeparser.parse_resume(pdf_file)
+parsed_resume = pyresumeparser.parse_resume(pdf_file)
 print(parsed_resume)
-
-
 From the Terminal
-You can also use ResumeParser directly from the terminal:
+You can also use PyResumeParser directly from the terminal:
 
+bash
+Copy code
 pyresumeparser resume.pdf
-
-
 This command will parse the specified PDF file and print the extracted entities in JSON format.
 
-
 Example Output
 Here is an example of the JSON output you might get from parsing a resume:
 
+json
+Copy code
 {
     "first_name": ["John"],
     "last_name": ["Doe"],
     "email": ["johndoe@example.com"],
     "phone": ["+1 234 567 890"],
     "country": ["USA"],
     "state": ["California"],
@@ -66,29 +69,30 @@
     "projects_worked": ["Project A", "Project B"],
     "skills": ["Python", "Machine Learning", "Data Analysis"],
     "total_experience": ["5 years"],
     "language": ["English"],
     "linkedin": ["https://linkedin.com/in/johndoe"],
     "github": ["https://github.com/johndoe"]
 }
-
 Requirements
-The following packages are required to use ResumeParser:
+The following packages are required to use PyResumeParser:
 
 spacy==3.7.4
 pdfminer.six==20231228
 spacy-transformers==1.3.5
+tqdm==4.66.4
 You can install these packages using pip:
 
+bash
+Copy code
 pip install -r requirements.txt
-
-
 Contributing
 Contributions are welcome! Please feel free to submit a Pull Request or open an issue on GitHub.
 
 License
-This project is licensed under the MIT License - see the LICENSE file for details.
+This project is licensed under the MIT License.
 
 Author
 Developed by Palash Khan.
 
 Feel free to reach out with any questions or feedback. Happy parsing!
+
```

