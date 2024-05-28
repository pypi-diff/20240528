# Comparing `tmp/pyresumeparser-0.0.6.tar.gz` & `tmp/pyresumeparser-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyresumeparser-0.0.6.tar", last modified: Tue May 28 11:39:35 2024, max compression
+gzip compressed data, was "pyresumeparser-0.0.7.tar", last modified: Tue May 28 12:36:24 2024, max compression
```

## Comparing `pyresumeparser-0.0.6.tar` & `pyresumeparser-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 pluto      (501) staff       (20)        0 2024-05-28 11:39:35.107604 pyresumeparser-0.0.6/
--rw-r--r--   0 pluto      (501) staff       (20)     2835 2024-05-28 11:39:35.106397 pyresumeparser-0.0.6/PKG-INFO
--rw-r--r--   0 pluto      (501) staff       (20)     2162 2024-05-28 11:38:04.000000 pyresumeparser-0.0.6/README.md
-drwxr-xr-x   0 pluto      (501) staff       (20)        0 2024-05-28 11:39:35.092551 pyresumeparser-0.0.6/pyresumeparser/
--rw-r--r--   0 pluto      (501) staff       (20)       44 2024-05-21 07:40:09.000000 pyresumeparser-0.0.6/pyresumeparser/__init__.py
--rw-r--r--   0 pluto      (501) staff       (20)     4716 2024-05-28 11:00:58.000000 pyresumeparser-0.0.6/pyresumeparser/main.py
-drwxr-xr-x   0 pluto      (501) staff       (20)        0 2024-05-28 11:39:35.099685 pyresumeparser-0.0.6/pyresumeparser.egg-info/
--rw-r--r--   0 pluto      (501) staff       (20)     2835 2024-05-28 11:39:34.000000 pyresumeparser-0.0.6/pyresumeparser.egg-info/PKG-INFO
--rw-r--r--   0 pluto      (501) staff       (20)      298 2024-05-28 11:39:34.000000 pyresumeparser-0.0.6/pyresumeparser.egg-info/SOURCES.txt
--rw-r--r--   0 pluto      (501) staff       (20)        1 2024-05-28 11:39:34.000000 pyresumeparser-0.0.6/pyresumeparser.egg-info/dependency_links.txt
--rw-r--r--   0 pluto      (501) staff       (20)       60 2024-05-28 11:39:34.000000 pyresumeparser-0.0.6/pyresumeparser.egg-info/entry_points.txt
--rw-r--r--   0 pluto      (501) staff       (20)       94 2024-05-28 11:39:34.000000 pyresumeparser-0.0.6/pyresumeparser.egg-info/requires.txt
--rw-r--r--   0 pluto      (501) staff       (20)       15 2024-05-28 11:39:34.000000 pyresumeparser-0.0.6/pyresumeparser.egg-info/top_level.txt
--rw-r--r--   0 pluto      (501) staff       (20)       38 2024-05-28 11:39:35.107761 pyresumeparser-0.0.6/setup.cfg
--rw-r--r--   0 pluto      (501) staff       (20)     1023 2024-05-28 11:38:15.000000 pyresumeparser-0.0.6/setup.py
+drwxr-xr-x   0 pluto      (501) staff       (20)        0 2024-05-28 12:36:24.776125 pyresumeparser-0.0.7/
+-rw-r--r--   0 pluto      (501) staff       (20)     3111 2024-05-28 12:36:24.774981 pyresumeparser-0.0.7/PKG-INFO
+-rw-r--r--   0 pluto      (501) staff       (20)     2435 2024-05-28 12:32:46.000000 pyresumeparser-0.0.7/README.md
+drwxr-xr-x   0 pluto      (501) staff       (20)        0 2024-05-28 12:36:24.767076 pyresumeparser-0.0.7/pyresumeparser/
+-rw-r--r--   0 pluto      (501) staff       (20)       44 2024-05-21 07:40:09.000000 pyresumeparser-0.0.7/pyresumeparser/__init__.py
+-rw-r--r--   0 pluto      (501) staff       (20)     4734 2024-05-28 12:33:59.000000 pyresumeparser-0.0.7/pyresumeparser/main.py
+drwxr-xr-x   0 pluto      (501) staff       (20)        0 2024-05-28 12:36:24.772648 pyresumeparser-0.0.7/pyresumeparser.egg-info/
+-rw-r--r--   0 pluto      (501) staff       (20)     3111 2024-05-28 12:36:24.000000 pyresumeparser-0.0.7/pyresumeparser.egg-info/PKG-INFO
+-rw-r--r--   0 pluto      (501) staff       (20)      298 2024-05-28 12:36:24.000000 pyresumeparser-0.0.7/pyresumeparser.egg-info/SOURCES.txt
+-rw-r--r--   0 pluto      (501) staff       (20)        1 2024-05-28 12:36:24.000000 pyresumeparser-0.0.7/pyresumeparser.egg-info/dependency_links.txt
+-rw-r--r--   0 pluto      (501) staff       (20)       60 2024-05-28 12:36:24.000000 pyresumeparser-0.0.7/pyresumeparser.egg-info/entry_points.txt
+-rw-r--r--   0 pluto      (501) staff       (20)       94 2024-05-28 12:36:24.000000 pyresumeparser-0.0.7/pyresumeparser.egg-info/requires.txt
+-rw-r--r--   0 pluto      (501) staff       (20)       15 2024-05-28 12:36:24.000000 pyresumeparser-0.0.7/pyresumeparser.egg-info/top_level.txt
+-rw-r--r--   0 pluto      (501) staff       (20)       38 2024-05-28 12:36:24.776394 pyresumeparser-0.0.7/setup.cfg
+-rw-r--r--   0 pluto      (501) staff       (20)     1016 2024-05-28 12:34:54.000000 pyresumeparser-0.0.7/setup.py
```

### Comparing `pyresumeparser-0.0.6/PKG-INFO` & `pyresumeparser-0.0.7/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,53 +1,45 @@
-Metadata-Version: 2.1
-Name: pyresumeparser
-Version: 0.0.6
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
 
-PyResumeParser is a Python package designed to parse resume PDF files and extract key entities such as names, emails, phone numbers, education details, skills, and more. It utilizes `spaCy` and `pdfminer.six` for natural language processing and PDF text extraction.
+PyResumeParser is a Python package designed to parse resume PDF files and extract key entities such as names, emails, phone numbers, education details, skills, and more. It utilizes `spaCy` and `pdfminer.six` for natural language processing and PDF text extraction. It requires Python version 3.10 or higher.
+
+
 
 ## Installation
 
 You can install PyResumeParser using pip:
 
-```bash
 pip install pyresumeparser
-Usage
+
+
+
+## Usage
+
 As a Python Module
+-------------------
 To use PyResumeParser in your Python code, you can import the package and call the parse_resume function:
 
 import pyresumeparser
-
 pdf_file = "resume.pdf"
 parsed_resume = pyresumeparser.parse_resume(pdf_file)
 print(parsed_resume)
+
+
 From the Terminal
+--------------------
 You can also use PyResumeParser directly from the terminal:
 
 pyresumeparser resume.pdf
+
 This command will parse the specified PDF file and print the extracted entities in JSON format.
 
-Example Output
+
+
+## Example Output
+
 Here is an example of the JSON output you might get from parsing a resume:
 
 
 {
     "first_name": ["John"],
     "last_name": ["Doe"],
     "email": ["johndoe@example.com"],
@@ -64,29 +56,46 @@
     "projects_worked": ["Project A", "Project B"],
     "skills": ["Python", "Machine Learning", "Data Analysis"],
     "total_experience": ["5 years"],
     "language": ["English"],
     "linkedin": ["https://linkedin.com/in/johndoe"],
     "github": ["https://github.com/johndoe"]
 }
-Requirements
-The following packages are required to use PyResumeParser:
+
+
+
+## Requirements
+
+Python version required: 3.10 or higher.
+
+The following packages are required to use PyResumeParser (required packages are automatically installed during the installation of the package pyresumeparser):
 
 spacy==3.7.4
 pdfminer.six==20231228
 spacy-transformers==1.3.5
 tqdm==4.66.4
-You can install these packages using pip:
 
 
+You can install these packages manually using pip:
+
 pip install -r requirements.txt
-Contributing
+
+
+
+## Contributing
+
 Contributions are welcome! Please feel free to submit a Pull Request or open an issue on GitHub.
 
-License
+
+
+## License
+
 This project is licensed under the MIT License.
 
-Author
+
+
+## Author
+
 Developed by Palash Khan.
 
 Feel free to reach out with any questions or feedback. Happy parsing!
```

### Comparing `pyresumeparser-0.0.6/README.md` & `pyresumeparser-0.0.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,65 @@
+Metadata-Version: 2.1
+Name: pyresumeparser
+Version: 0.0.7
+Summary: A package for parsing resume and extracting entities.
+Home-page: https://github.com/pkhan123/pyresumeparser
+Author: Palash Khan
+Author-email: palashkhan777@gmail.com
+Classifier: Programming Language :: Python :: 3.10
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
 
-PyResumeParser is a Python package designed to parse resume PDF files and extract key entities such as names, emails, phone numbers, education details, skills, and more. It utilizes `spaCy` and `pdfminer.six` for natural language processing and PDF text extraction.
+PyResumeParser is a Python package designed to parse resume PDF files and extract key entities such as names, emails, phone numbers, education details, skills, and more. It utilizes `spaCy` and `pdfminer.six` for natural language processing and PDF text extraction. It requires Python version 3.10 or higher.
+
+
 
 ## Installation
 
 You can install PyResumeParser using pip:
 
-```bash
 pip install pyresumeparser
-Usage
+
+
+
+## Usage
+
 As a Python Module
+-------------------
 To use PyResumeParser in your Python code, you can import the package and call the parse_resume function:
 
 import pyresumeparser
-
 pdf_file = "resume.pdf"
 parsed_resume = pyresumeparser.parse_resume(pdf_file)
 print(parsed_resume)
+
+
 From the Terminal
+--------------------
 You can also use PyResumeParser directly from the terminal:
 
 pyresumeparser resume.pdf
+
 This command will parse the specified PDF file and print the extracted entities in JSON format.
 
-Example Output
+
+
+## Example Output
+
 Here is an example of the JSON output you might get from parsing a resume:
 
 
 {
     "first_name": ["John"],
     "last_name": ["Doe"],
     "email": ["johndoe@example.com"],
@@ -44,29 +76,46 @@
     "projects_worked": ["Project A", "Project B"],
     "skills": ["Python", "Machine Learning", "Data Analysis"],
     "total_experience": ["5 years"],
     "language": ["English"],
     "linkedin": ["https://linkedin.com/in/johndoe"],
     "github": ["https://github.com/johndoe"]
 }
-Requirements
-The following packages are required to use PyResumeParser:
+
+
+
+## Requirements
+
+Python version required: 3.10 or higher.
+
+The following packages are required to use PyResumeParser (required packages are automatically installed during the installation of the package pyresumeparser):
 
 spacy==3.7.4
 pdfminer.six==20231228
 spacy-transformers==1.3.5
 tqdm==4.66.4
-You can install these packages using pip:
 
 
+You can install these packages manually using pip:
+
 pip install -r requirements.txt
-Contributing
+
+
+
+## Contributing
+
 Contributions are welcome! Please feel free to submit a Pull Request or open an issue on GitHub.
 
-License
+
+
+## License
+
 This project is licensed under the MIT License.
 
-Author
+
+
+## Author
+
 Developed by Palash Khan.
 
 Feel free to reach out with any questions or feedback. Happy parsing!
```

### Comparing `pyresumeparser-0.0.6/pyresumeparser/main.py` & `pyresumeparser-0.0.7/pyresumeparser/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,22 +121,23 @@
     
     # Remove duplicates by converting lists to sets and back to lists
     for key in entities:
         entities[key] = list(set(entities[key]))
     
     return entities
 
-def parse_resume(filepath, nlp):
+def parse_resume(filepath):
     """
     Converts a PDF file to a JSON object with extracted entities.
 
     :param filepath: Path to the PDF file
     :param nlp: spaCy NLP model
     :return: JSON object with extracted entities
     """
+    nlp = load_model()
     text = pdf_to_text(filepath)
     entities = extract_entities(text, nlp)
     entities_json = json.dumps(entities, indent=4)
     return entities_json
 
 def main():
     parser = argparse.ArgumentParser(description="Parse a resume PDF file and extract entities.")
```

### Comparing `pyresumeparser-0.0.6/pyresumeparser.egg-info/PKG-INFO` & `pyresumeparser-0.0.7/pyresumeparser.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,53 +1,65 @@
 Metadata-Version: 2.1
 Name: pyresumeparser
-Version: 0.0.6
+Version: 0.0.7
 Summary: A package for parsing resume and extracting entities.
 Home-page: https://github.com/pkhan123/pyresumeparser
 Author: Palash Khan
 Author-email: palashkhan777@gmail.com
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pdfminer.six==20231228
 Requires-Dist: spacy==3.7.4
 Requires-Dist: spacy-transformers==1.3.5
 Requires-Dist: tqdm==4.66.4
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 
 # PyResumeParser
 
-PyResumeParser is a Python package designed to parse resume PDF files and extract key entities such as names, emails, phone numbers, education details, skills, and more. It utilizes `spaCy` and `pdfminer.six` for natural language processing and PDF text extraction.
+PyResumeParser is a Python package designed to parse resume PDF files and extract key entities such as names, emails, phone numbers, education details, skills, and more. It utilizes `spaCy` and `pdfminer.six` for natural language processing and PDF text extraction. It requires Python version 3.10 or higher.
+
+
 
 ## Installation
 
 You can install PyResumeParser using pip:
 
-```bash
 pip install pyresumeparser
-Usage
+
+
+
+## Usage
+
 As a Python Module
+-------------------
 To use PyResumeParser in your Python code, you can import the package and call the parse_resume function:
 
 import pyresumeparser
-
 pdf_file = "resume.pdf"
 parsed_resume = pyresumeparser.parse_resume(pdf_file)
 print(parsed_resume)
+
+
 From the Terminal
+--------------------
 You can also use PyResumeParser directly from the terminal:
 
 pyresumeparser resume.pdf
+
 This command will parse the specified PDF file and print the extracted entities in JSON format.
 
-Example Output
+
+
+## Example Output
+
 Here is an example of the JSON output you might get from parsing a resume:
 
 
 {
     "first_name": ["John"],
     "last_name": ["Doe"],
     "email": ["johndoe@example.com"],
@@ -64,29 +76,46 @@
     "projects_worked": ["Project A", "Project B"],
     "skills": ["Python", "Machine Learning", "Data Analysis"],
     "total_experience": ["5 years"],
     "language": ["English"],
     "linkedin": ["https://linkedin.com/in/johndoe"],
     "github": ["https://github.com/johndoe"]
 }
-Requirements
-The following packages are required to use PyResumeParser:
+
+
+
+## Requirements
+
+Python version required: 3.10 or higher.
+
+The following packages are required to use PyResumeParser (required packages are automatically installed during the installation of the package pyresumeparser):
 
 spacy==3.7.4
 pdfminer.six==20231228
 spacy-transformers==1.3.5
 tqdm==4.66.4
-You can install these packages using pip:
 
 
+You can install these packages manually using pip:
+
 pip install -r requirements.txt
-Contributing
+
+
+
+## Contributing
+
 Contributions are welcome! Please feel free to submit a Pull Request or open an issue on GitHub.
 
-License
+
+
+## License
+
 This project is licensed under the MIT License.
 
-Author
+
+
+## Author
+
 Developed by Palash Khan.
 
 Feel free to reach out with any questions or feedback. Happy parsing!
```

### Comparing `pyresumeparser-0.0.6/setup.py` & `pyresumeparser-0.0.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-import os
 from setuptools import setup, find_packages
 
 setup(
     name='pyresumeparser',
-    version='0.0.6',
+    version='0.0.7',
     packages=find_packages(),
     install_requires=[
         'pdfminer.six==20231228',
         'spacy==3.7.4',
         'spacy-transformers==1.3.5',
         'tqdm==4.66.4'
     ],
@@ -25,13 +24,13 @@
     author='Palash Khan',
     author_email='palashkhan777@gmail.com',
     description='A package for parsing resume and extracting entities.',
     long_description=open('README.md', 'r', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/pkhan123/pyresumeparser',
     classifiers=[
-        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.10',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.10',
 )
```

