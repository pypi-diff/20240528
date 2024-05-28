# Comparing `tmp/mobile_strings_converter-0.1.1.tar.gz` & `tmp/mobile_strings_converter-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mobile_strings_converter-0.1.1.tar", max compression
+gzip compressed data, was "mobile_strings_converter-0.1.3.tar", max compression
```

## Comparing `mobile_strings_converter-0.1.1.tar` & `mobile_strings_converter-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1074 2023-03-19 12:35:02.146893 mobile_strings_converter-0.1.1/LICENSE
--rw-r--r--   0        0        0    16720 2023-03-19 12:35:02.146893 mobile_strings_converter-0.1.1/README.md
--rw-r--r--   0        0        0     1504 2023-03-19 12:35:02.146893 mobile_strings_converter-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      462 2023-03-19 12:35:02.146893 mobile_strings_converter-0.1.1/src/mobile_strings_converter/__init__.py
--rw-r--r--   0        0        0     2636 2023-03-19 12:35:02.146893 mobile_strings_converter-0.1.1/src/mobile_strings_converter/__main__.py
--rw-r--r--   0        0        0    77096 2023-03-19 12:35:02.146893 mobile_strings_converter-0.1.1/src/mobile_strings_converter/assets/fonts/Aakar.ttf
--rw-r--r--   0        0        0  1796568 2023-03-19 12:35:02.162893 mobile_strings_converter-0.1.1/src/mobile_strings_converter/assets/fonts/AnekTelugu-VariableFont_wdth,wght.ttf
--rw-r--r--   0        0        0   680264 2023-03-19 12:35:02.166893 mobile_strings_converter-0.1.1/src/mobile_strings_converter/assets/fonts/DejaVuSansCondensed.ttf
--rw-r--r--   0        0        0   584324 2023-03-19 12:35:02.170893 mobile_strings_converter-0.1.1/src/mobile_strings_converter/assets/fonts/Eunjin.ttf
--rw-r--r--   0        0        0    28568 2023-03-19 12:35:02.170893 mobile_strings_converter-0.1.1/src/mobile_strings_converter/assets/fonts/Gurvetica_a8_Heavy.ttf
--rw-r--r--   0        0        0    73292 2023-03-19 12:35:02.170893 mobile_strings_converter-0.1.1/src/mobile_strings_converter/assets/fonts/Latha.ttf
--rw-r--r--   0        0        0    86820 2023-03-19 12:35:02.170893 mobile_strings_converter-0.1.1/src/mobile_strings_converter/assets/fonts/Waree.ttf
--rw-r--r--   0        0        0 15443432 2023-03-19 12:35:02.294893 mobile_strings_converter-0.1.1/src/mobile_strings_converter/assets/fonts/fireflysung.ttf
--rw-r--r--   0        0        0    72500 2023-03-19 12:35:02.294893 mobile_strings_converter-0.1.1/src/mobile_strings_converter/assets/fonts/gargi.ttf
--rw-r--r--   0        0        0      108 2023-03-19 12:35:02.294893 mobile_strings_converter-0.1.1/src/mobile_strings_converter/console_style.py
--rw-r--r--   0        0        0    15839 2023-03-19 12:35:02.294893 mobile_strings_converter-0.1.1/src/mobile_strings_converter/converter.py
--rw-r--r--   0        0        0    18369 1970-01-01 00:00:00.000000 mobile_strings_converter-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-05-28 16:25:47.967559 mobile_strings_converter-0.1.3/LICENSE
+-rw-r--r--   0        0        0    17753 2024-05-28 16:25:47.967559 mobile_strings_converter-0.1.3/README.md
+-rw-r--r--   0        0        0     1530 2024-05-28 16:25:47.967559 mobile_strings_converter-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      460 2024-05-28 16:25:47.967559 mobile_strings_converter-0.1.3/src/mobile_strings_converter/__init__.py
+-rw-r--r--   0        0        0     2378 2024-05-28 16:25:47.967559 mobile_strings_converter-0.1.3/src/mobile_strings_converter/__main__.py
+-rw-r--r--   0        0        0    77096 2024-05-28 16:25:47.967559 mobile_strings_converter-0.1.3/src/mobile_strings_converter/assets/fonts/Aakar.ttf
+-rw-r--r--   0        0        0  1796568 2024-05-28 16:25:47.979559 mobile_strings_converter-0.1.3/src/mobile_strings_converter/assets/fonts/AnekTelugu-VariableFont_wdth,wght.ttf
+-rw-r--r--   0        0        0   680264 2024-05-28 16:25:47.983559 mobile_strings_converter-0.1.3/src/mobile_strings_converter/assets/fonts/DejaVuSansCondensed.ttf
+-rw-r--r--   0        0        0   584324 2024-05-28 16:25:47.987559 mobile_strings_converter-0.1.3/src/mobile_strings_converter/assets/fonts/Eunjin.ttf
+-rw-r--r--   0        0        0    28568 2024-05-28 16:25:47.987559 mobile_strings_converter-0.1.3/src/mobile_strings_converter/assets/fonts/Gurvetica_a8_Heavy.ttf
+-rw-r--r--   0        0        0    73292 2024-05-28 16:25:47.987559 mobile_strings_converter-0.1.3/src/mobile_strings_converter/assets/fonts/Latha.ttf
+-rw-r--r--   0        0        0    86820 2024-05-28 16:25:47.987559 mobile_strings_converter-0.1.3/src/mobile_strings_converter/assets/fonts/Waree.ttf
+-rw-r--r--   0        0        0 15443432 2024-05-28 16:25:48.079559 mobile_strings_converter-0.1.3/src/mobile_strings_converter/assets/fonts/fireflysung.ttf
+-rw-r--r--   0        0        0    72500 2024-05-28 16:25:48.079559 mobile_strings_converter-0.1.3/src/mobile_strings_converter/assets/fonts/gargi.ttf
+-rw-r--r--   0        0        0      108 2024-05-28 16:25:48.079559 mobile_strings_converter-0.1.3/src/mobile_strings_converter/console_style.py
+-rw-r--r--   0        0        0    26425 2024-05-28 16:25:48.079559 mobile_strings_converter-0.1.3/src/mobile_strings_converter/converter.py
+-rw-r--r--   0        0        0    19474 1970-01-01 00:00:00.000000 mobile_strings_converter-0.1.3/PKG-INFO
```

### Comparing `mobile_strings_converter-0.1.1/LICENSE` & `mobile_strings_converter-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mobile_strings_converter-0.1.1/README.md` & `mobile_strings_converter-0.1.3/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -9,83 +9,91 @@
 *** https://www.markdownguide.org/basic-syntax/#reference-style-links
 -->
 
 <!-- PROJECT LOGO -->
 <br />
 <div align="center">
     <img src="docs/icon.png" alt="Logo" width="156" height="156" style="margin-bottom:-40px">
-    <h2 align="center">Mobile strings converter</h2>
+    <h1 align="center">Mobile Strings Converter</h1>
     <p align="center">
         A Python package that converts Android & iOS strings files to any supported file type.
         <br />
         <br />
         <a href="https://pypi.org/project/mobile-strings-converter/">
           <img alt="PyPI version" src="https://img.shields.io/pypi/v/mobile-strings-converter" />
         </a>
         <a href="https://pypi.org/project/mobile-strings-converter/">
           <img alt="Python versions support" src="https://img.shields.io/pypi/pyversions/mobile-strings-converter" />
         </a>
         <br />
-        <a href="https://github.com/HenestrosaConH/mobile-strings-converter/actions/workflows/build.yaml">
-          <img alt="GitHub action: Build" src="https://github.com/HenestrosaConH/mobile-strings-converter/actions/workflows/build.yaml/badge.svg" />
+        <a href="https://github.com/HenestrosaDev/mobile-strings-converter/actions/workflows/build.yaml">
+          <img alt="GitHub action: Build" src="https://github.com/HenestrosaDev/mobile-strings-converter/actions/workflows/build.yaml/badge.svg" />
         </a>
-        <a href="https://codecov.io/gh/HenestrosaConH/mobile-strings-converter/">
-          <img alt="Codecov" src="https://codecov.io/gh/HenestrosaConH/mobile-strings-converter/branch/main/graph/badge.svg" />
+        <a href="https://codecov.io/gh/HenestrosaDev/mobile-strings-converter/">
+          <img alt="Codecov" src="https://codecov.io/gh/HenestrosaDev/mobile-strings-converter/branch/main/graph/badge.svg" />
         </a>
-        <a href="https://github.com/HenestrosaConH/mobile-strings-converter/blob/main/LICENSE">
-          <img alt="License" src="https://img.shields.io/github/license/HenestrosaConH/mobile-strings-converter" />
+        <a href="https://github.com/HenestrosaDev/mobile-strings-converter/blob/main/LICENSE">
+          <img alt="License" src="https://img.shields.io/github/license/HenestrosaDev/mobile-strings-converter" />
         </a>
         <br />
-        <a href="https://github.com/HenestrosaConH/mobile-strings-converter/graphs/contributors">
-          <img alt="GitHub Contributors" src="https://img.shields.io/github/contributors/HenestrosaConH/mobile-strings-converter" />
+        <a href="https://github.com/HenestrosaDev/mobile-strings-converter/graphs/contributors">
+          <img alt="GitHub Contributors" src="https://img.shields.io/github/contributors/HenestrosaDev/mobile-strings-converter" />
         </a>
-        <a href="https://github.com/HenestrosaConH/mobile-strings-converter/issues">
-          <img alt="Issues" src="https://img.shields.io/github/issues/HenestrosaConH/mobile-strings-converter" />
+        <a href="https://github.com/HenestrosaDev/mobile-strings-converter/issues">
+          <img alt="Issues" src="https://img.shields.io/github/issues/HenestrosaDev/mobile-strings-converter" />
         </a>
-        <a href="https://github.com/HenestrosaConH/mobile-strings-converter/pulls">
-          <img alt="GitHub pull requests" src="https://img.shields.io/github/issues-pr/HenestrosaConH/mobile-strings-converter" />
+        <a href="https://github.com/HenestrosaDev/mobile-strings-converter/pulls">
+          <img alt="GitHub pull requests" src="https://img.shields.io/github/issues-pr/HenestrosaDev/mobile-strings-converter" />
         </a>
         <br />
         <br />
-        <a href="https://github.com/HenestrosaConH/mobile-strings-converter/issues/new/choose">Report Bug</a> · <a href="https://github.com/HenestrosaConH/mobile-strings-converter/issues/new/choose">Request Feature</a> · <a href="https://github.com/HenestrosaConH/mobile-strings-converter/discussions">Ask Question</a>
+        <a href="https://github.com/HenestrosaDev/mobile-strings-converter/issues/new/choose">Report Bug</a> · <a href="https://github.com/HenestrosaDev/mobile-strings-converter/issues/new/choose">Request Feature</a> · <a href="https://github.com/HenestrosaDev/mobile-strings-converter/discussions">Ask Question</a>
     </p>
 </div>
 
 <!-- TABLE OF CONTENTS -->
 
 ## Table of Contents
 
 - [About the Project](#about-the-project)
+  - [File Types Supported](#file-types-supported) 
   - [Project Structure](#project-structure)
   - [Built With](#built-with)
 - [Release Files](#release-files)
+- [Getting Started](#getting-started)
+  - [Script Installation](#script-installation)
+  - [Package Installation](#package-installation)
 - [Usage](#usage)
-  - [To Execute the Script](#to-execute-the-script)
-  - [To Import the Package Into Your Project](#to-import-the-package-into-your-project)
-  - [To Open the Code](#to-open-the-code)
+  - [Run the Program](#run-the-program)
+    - [Script Flags](#script-flags)
+  - [Using the Package in Your Project](#using-the-package-in-your-project)
+  - [Generate a Spreadsheet in Google Sheets](#generate-a-spreadsheet-in-google-sheets)
 - [Notes](#notes)
-  - [List of Indic Languages Supported by PDF files](#list-of-indic-languages-supported-by-pdf-files)
-  - [List of Languages Not Supported by PDF files](#list-of-languages-not-supported-by-pdf-files)
+  - [Indic Languages Supported by PDF files](#indic-languages-supported-by-pdf-files)
+  - [Languages Not Supported by PDF files](#languages-not-supported-by-pdf-files)
 - [Roadmap](#roadmap)
 - [Contributing](#contributing)
 - [License](#license)
 - [Authors](#authors)
 - [Acknowledgments](#acknowledgments)
 - [Support](#support)
 
 <!-- ABOUT THE PROJECT -->
 
 ## About the Project
 
 I tried to do the whole process of converting a strings resource file into a spreadsheet in Google Sheets by hand and, even though you can do it with the option **Data > Split text to columns**, 
 it involves wasting your time generating the spreadsheet manually. Due to that, I decided to build a time-efficient solution, which consists on running a Python script in order to achieve that with any file type.
 
-Moreover, not only this script can be executed on its own, it also can be installed as a package via **PyPI** (more information [here](#to-import-the-package-into-your-project) about how to install it).
+Moreover, not only this script can be executed on its own, it also can be installed as a package via **PyPI** (more information [here](#using-the-package-in-your-project) about how to install it).
+
+<!-- FILE TYPES SUPPORTED -->
+
+### File Types Supported
 
-The file types supported by the package are the following:
 - Android strings format (`*.xml`)
 - CSV
 - Google Sheets support
 - HTML
 - iOS strings format (`*.strings`)
 - JSON
 - MD
@@ -94,203 +102,324 @@
 - XLSX
 - YAML
 
 <!-- PROJECT STRUCTURE -->
 
 ### Project Structure
 
-#### Root directories:
-
-- `.github/workflows`: GitHub workflows. It also includes the templates for issues and pull requests, as well as the `depandabot.yml` file for Dependabot configuration.
-- `docs`: Contains files related to the documentation of the project.
-- `src/mobile_strings_converter`:  Contains the source code files.
-- `tests`: Contains unit tests to ensure the correct functionality of the package. It also includes the `files` directory, which contains a few demo files in different formats to use in the unit tests.
-
-#### Root files:
-
-- `.gitignore`: File used by the version control system Git to specify files or directories that should be ignored by Git when tracking changes to a project.
-- `.pre-commit-config.yaml`: Configuration file used by **pre-commit**, a tool that runs checks (such as linting, testing, or formatting) on the code before you commit changes to version control. The file specifies which checks pre-commit should run and how it should run them.
-- `LICENSE`: Project license, which is [MIT](https://opensource.org/license/mit/).
-- `poetry.lock`: File generated by **Poetry**, a package manager for Python, that contains the exact versions of all packages used by a project. The file is used to ensure that all members of a development team are using the same versions of packages, even if different versions are available in the package repository.
-- `pyproject.toml`: Configuration file used by **Poetry**. It specifies the metadata for a Python project, including the project name, version, description, author, license and dependencies.
-- `README.md`: What you are reading right now.
-- `requirements.txt`: Lists the names and versions of each package used to build this project. To install the requirements, execute `pip install -r requirements.txt`.
-- `requirements-dev.txt`: Lists the names and versions of each package used in the development stage of this project. To install the requirements, execute `pip install -r requirements-dev.txt`.
+<details>
+  <summary>ASCII folder structure</summary>
 
+```
+│   .gitignore
+│   .pre-commit-config.yaml
+│   LICENSE
+│   poetry.lock 
+│   pyproject.toml
+│   README.md
+│   requirements.txt
+│   requirements-dev.txt
+│
+├───.github
+│   │   CONTRIBUTING.md
+│   │
+│   ├───ISSUE_TEMPLATE
+│   │       bug_report_template.md
+│   │       feature_request_template.md
+│   │
+│   └───PULL_REQUEST_TEMPLATE
+│           pull_request_template.md
+│
+├───docs
+│       icon.png
+│
+├───src
+│   ├───mobile_strings_converter
+│   │       console_style.py
+│   │       converter.py
+│   │       __init__.py
+│   │       __main__.py
+│   │
+│   ├───assets
+│   │       └───fonts
+│   │               Aakar.ttf
+│   │               AnekTelugu-VariableFont_wdth,wght.ttf
+│   │               DejaVuSansCondensed.ttf
+│   │               Eunjin.ttf
+│   │               fireflysung.ttf
+│   │               gargi.ttf
+│   │               Gurvetica_a8_Heavy.ttf
+│   │               Latha.ttf
+│   │               Waree.ttf
+│   │
+│   ├───controller
+│   │       main_controller.py
+│   │       __init__.py
+│   │
+│   ├───model
+│   │       transcription.py
+│   │       __init__.py
+│   │
+│   ├───utils
+│   │       constants.py
+│   │       i18n.py
+│   │       path_helper.py
+│   │       __init__.py
+│   │
+│   └───view
+│           main_window.py
+│           __init__.py
+│
+└───tests   
+    │   base_tests.py
+    │   test_get_strings.py
+    │   test_to_android.py
+    │   test_to_csv.py
+    │   test_to_html.py
+    │   test_to_ios.py
+    │   test_to_json.py
+    │   test_to_md.py
+    │   test_to_ods.py
+    │   test_to_pdf.py
+    │   test_to_xlsx.py
+    │   test_to_yaml.py
+    │
+    └───files
+        ├───input
+        │       Localizable.strings
+        │       strings.xml
+        │
+        ├───template-with-comments
+        │       Localizable.strings
+        │       strings.csv
+        │       strings.html
+        │       strings.json
+        │       strings.md
+        │       strings.ods
+        │       strings.pdf
+        │       strings.xlsx
+        │       strings.xml
+        │       strings.yaml
+        │
+        └───template-without-comments
+                Localizable.strings
+                strings.csv
+                strings.html
+                strings.json
+                strings.md
+                strings.ods
+                strings.pdf
+                strings.xlsx
+                strings.xml
+                strings.yaml
+```
+</details>
 
 <!-- BUILT WITH -->
 
 ### Built With
 
-- [openpyxl](https://pypi.org/project/openpyxl/): To generate ODS and XLSX files.
-- [gspread](https://pypi.org/project/gspread/): To generate spreadsheets in Google Sheets.
-- [protobuf](https://pypi.org/project/oauth2client/): Used by `google.oauth2.credentials` to authenticate to the user's Google account in order to create the spreadsheet in Google Sheets. 
-- [PyYAML](https://pypi.org/project/PyYAML/): To generate YAML files.
-- [arabic-reshaper](https://pypi.org/project/arabic-reshaper/) and [python-bidi](https://pypi.org/project/python-bidi/): To add arabic characters support for PDF files.
-- [fpdf2](https://pypi.org/project/fpdf2/): To generate PDF files.
-- [lingua-language-detector](https://pypi.org/project/lingua-language-detector/): To recognize the **value** language when writing a PDF in order to know what font to use.  
+- [openpyxl](https://pypi.org/project/openpyxl/) to generate ODS and XLSX files.
+- [gspread](https://pypi.org/project/gspread/) to generate spreadsheets in Google Sheets.
+- [protobuf](https://pypi.org/project/oauth2client/) is used by `google.oauth2.credentials` to authenticate to the user's Google account in order to create the spreadsheet in Google Sheets. 
+- [PyYAML](https://pypi.org/project/PyYAML/) to generate YAML files.
+- [arabic-reshaper](https://pypi.org/project/arabic-reshaper/) and [python-bidi](https://pypi.org/project/python-bidi/) to add arabic characters support for PDF files.
+- [fpdf2](https://pypi.org/project/fpdf2/) to generate PDF files.
+- [lingua-language-detector](https://pypi.org/project/lingua-language-detector/) to recognize the **value** language when writing a PDF in order to know what font to use.  
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 <!-- RELEASE FILES -->
 
 ## Release Files
 
-| File                                                                                                                                                         | Description                                                                                                 | Size      |
-|:-------------------------------------------------------------------------------------------------------------------------------------------------------------|:------------------------------------------------------------------------------------------------------------|:----------|
-| [mobile-strings-converter.zip](https://github.com/HenestrosaConH/mobile-strings-converter/releases/latest/download/mobile-strings-converter.zip)             | Standard language support for PDF files (over 100 languages, including RTL)                                 | 0.32 MB   |
-| [mobile-strings-converter-indic.zip](https://github.com/HenestrosaConH/mobile-strings-converter/releases/latest/download/mobile-strings-converter-indic.zip) | PDF file support for Indic languages ([see list](#list-of-indic-languages-supported-by-pdf-files))          | 1.40 MB   |
-| [mobile-strings-converter-zh-ja.zip](https://github.com/HenestrosaConH/mobile-strings-converter/releases/latest/download/mobile-strings-converter-zh-ja.zip) | PDF file support for Japanese and Chinese (simplified and traditional)                                      | 7.17 MB   |
-| [mobile-strings-converter-ko.zip](https://github.com/HenestrosaConH/mobile-strings-converter/releases/latest/download/mobile-strings-converter-ko.zip)       | PDF file support for Korean                                                                                 | 0.46 MB   |
-| [mobile-strings-converter-th.zip](https://github.com/HenestrosaConH/mobile-strings-converter/releases/latest/download/mobile-strings-converter-th.zip)       | PDF file support for Thai                                                                                   | 0.37 MB   |
-| [mobile-strings-converter-all.zip](https://github.com/HenestrosaConH/mobile-strings-converter/releases/latest/download/mobile-strings-converter-all.zip)     | PDF file support for almost all languages ([see exceptions](#list-of-languages-not-supported-by-pdf-files)) | 8.43 MB   |
+| File                                                                                                                                            | Description                                                                                         | Size    |
+|:------------------------------------------------------------------------------------------------------------------------------------------------|:----------------------------------------------------------------------------------------------------|:--------|
+| [mobile-strings-converter.zip](https://github.com/HenestrosaDev/mobile-strings-converter/releases/latest/download/mobile-strings-converter.zip) | PDF file support for almost all languages ([see exceptions](#languages-not-supported-by-pdf-files)) | 8.43 MB |
+
+<p align="right">(<a href="#top">back to top</a>)</p>
+
+<!-- GETTING STARTED -->
+
+## Getting Started
+
+### Script Installation
+
+1. Download the [release](#release-files) that is best suited to your needs.
+2. (Optional but recommended) Create a Python virtual environment in the project root. If you're using `virtualenv`, you would run `virtualenv venv`.
+3. (Optional but recommended) Activate the virtual environment:
+   ```bash
+   # on Windows
+   . venv/Scripts/activate
+   # if you get the error `FullyQualifiedErrorId : UnauthorizedAccess`, run this:
+   Set-ExecutionPolicy Unrestricted -Scope Process
+   # and then . venv/Scripts/activate
+   
+   # on macOS and Linux
+   source venv/Scripts/activate
+   ```
+4. Open the command line and run `pip install -r path/to/requirements.txt` to install the required packages to run the script.
+
+### Package Installation
+
+Install the PyPI package by running `pip install mobile-strings-converter`.
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 <!-- USAGE -->
 
 ## Usage
 
-### To Execute The Script
+### Run the Program
 
-1. Download the [release](#release-files) that is best suited to your needs.
-2. Open the command line and run `pip install -r path/to/requirements.txt` to install the required packages to execute the script.
-3. Example of a basic command to convert a `.xml` or `.strings` file to another file type: 
-    ```
-    path/to/python path/to/mobile_strings_converter.py path/to/<*.xml | *.strings> -o path/to/*.<SUPPORTED FILE TYPE EXTENSION>
-    ```
+For a basic usage, you can run the following command:
+
+```
+python path/to/mobile_strings_converter.py *.[SUPPORTED_FILE_TYPE] -o *.[SUPPORTED_FILE_TYPE]
+```
+
+See [Generate a Spreadsheet in Google Sheets](#generate-a-spreadsheet-in-google-sheets) to create a spreadsheet.
+
+#### Script Flags
+
+| Flag                        | Description                                                                                                                                                         |
+|:----------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| `-h` or `--help`            | Displays help text for the program                                                                                                                                  |
+| `-o` or `--output-filepath` | Specifies the filepath for storing the converted file. The file extension can be chosen from the list of supported file types mentioned [here](#about-the-project). |
+| `-g` or `--google-sheets`   | Followed by the name of the sheet, creates a new Google Sheets spreadsheet with the specified name.                                                                 |
+| `-c` or `--credentials`     | Followed by the path to your `service_account.json` file is mandatory if you want to generate a spreadsheet in your Google account.                                 |
+| `-p` or `--print-comments`  | The output file will include any commented strings present in the original file.                                                                                    |
 
-#### To Generate a Spreadsheet in Google Sheets
+<p align="right">(<a href="#top">back to top</a>)</p>
+
+### Using the Package in Your Project
+
+Once you have followed the steps of the [Getting Started](#getting-started) section, import the package and the wrapper function(s) you want to use: 
+```python
+# Using the `get_strings` function
+from mobile_strings_converter import get_strings  
+
+get_strings(
+   input_filepath=Path("strings.xml"), 
+   should_print_comments=True
+)
+```
+
+### Generate a Spreadsheet in Google Sheets
+
+#### Set Up Google Account
 
 Before going further into running the commands to do so, please note that you will have to generate a `service_account.json` file. You can do the following to get one:
 
 1. Go to the [Google Cloud Console](https://console.cloud.google.com/).
 2. Create a new project or select an existing project.
 3. Go to the **APIs & Services** page, click on **Dashboard** and then click on **Enable APIs and Services**.
 4. Search for **Google Sheets API** and enable it.
 5. Go to the **Credentials** page, click on **Create credentials**, and then choose **Service account**.
 6. Give your service account a name and select a role. For this purpose, you can select **Project -> Editor**.
 7. Click on the **Create key** button, select the JSON format and download the `service_account.json` file.
 8. Share your Google Sheets file with the email address that is specified in the **client_email** field in the `service_account.json` file.
 
-Alternatively, you can create an XLSX file and open it in Google Sheets if you do not want to go through the hassle of generating the `service_account.json` file.
+Alternatively, you can create a `.xlsx` file and open it in Google Sheets if you do not want to go through the hassle of generating the `service_account.json` file.
 
 Once you have generated the `service_account.json` file, you can generate a spreadsheet in Google Sheets by running the following command:
 ```
-path/to/python path/to/mobile_strings_converter.py path/to/<strings.xml | Localizable.strings> -gs <SHEET NAME> -c path/to/service_account.json 
+python path/to/mobile_strings_converter.py <*.xml | *.strings> -g <SHEET_NAME> -c path/to/service_account.json 
 ```
 
 If you want to generate an output file along with the spreadsheet, run this:
 ```
-path/to/python path/to/mobile_strings_converter.py path/to/<strings.xml | Localizable.strings> -gs <SHEET NAME> -c path/to/service_account.json -o path/to/strings.<SUPPORTED FILE TYPE EXTENSION>
+python path/to/mobile_strings_converter.py *.[SUPPORTED_FILE_TYPE -g <SHEET_NAME> -c path/to/service_account.json -o *.[SUPPORTED_FILE_TYPE]
 ```
 
-#### Script flags
+#### Using the `to_google_sheets` Function in Your Project
 
-- `-h`, `--help`: Show help
-- `-o`, `--output-filepath`: Output filepath where you want to store the converted file. Its extension can be any of the file types listed [here](#about-the-project).
-- `-g`, `--google-sheets` <spreadsheet name>: Creates a spreadsheet in Google Sheets with the name passed as argument.
-- `-c`, `--credentials` <`service_account.json` filepath>: Mandatory if you want to generate a spreadsheet in your Google account.
-- `-p`, `--print-comments`: If present, indicates that commented strings will be printed in the output file.
+```python
+from mobile_strings_converter import to_google_sheets
 
-### To Import the Package Into Your Project
-
-1. Run `pip install mobile-strings-converter`
-2. Import the package and the wrapper function with this line of code: `from mobile_strings_converter import convert_strings`.
-
-### To Open the Code
-
-1. Clone the project with the `git clone https://github.com/HenestrosaConH/mobile-strings-converter.git` command.
-2. Open it in your favourite IDE (mine is [PyCharm](https://www.jetbrains.com/pycharm/))
-
-<p align="right">(<a href="#top">back to top</a>)</p>
+to_google_sheets(
+    input_filepath=Path("path/to/strings-file"),
+    sheet_name="MyProject strings",
+    credentials_filepath=Path("path/to/service_account.json"),
+    should_print_comments=True,
+)
+```
 
 <!-- NOTES -->
 
 ## Notes
 
-### List of Indic Languages Supported by PDF files
+### Indic Languages Supported by PDF files
 
 - Hindi
 - Marathu
 - Oriya
 - Tibetan
 - Gujarati
 - Telugu
 - Tamil
 - Punjabi
 
-### List of Languages Not Supported by PDF files
+### Languages Not Supported by PDF files
 
-- **Bengali** (not possible to print correctly using [fpdf2](https://pypi.org/project/fpdf2/))
-- **Dhivehi** (not recognized by [lingua-language-detector](https://pypi.org/project/lingua-language-detector/))
-- **Kannada** (not recognized by [lingua-language-detector](https://pypi.org/project/lingua-language-detector/))
-- **Khmer** (not recognized by [lingua-language-detector](https://pypi.org/project/lingua-language-detector/))
-- **Lao** (not recognized by [lingua-language-detector](https://pypi.org/project/lingua-language-detector/))
-- **Malayalam** (not recognized by [lingua-language-detector](https://pypi.org/project/lingua-language-detector/))
-- **Meiteilon (manipuri)** (not recognized by [lingua-language-detector](https://pypi.org/project/lingua-language-detector/))
-- **Myanmar burmese** (not possible to print correctly using [fpdf2](https://pypi.org/project/fpdf2/))
-- **Odia (Oriya)** (not recognized by [lingua-language-detector](https://pypi.org/project/lingua-language-detector/))
-- **Sinhala** (not recognized by [lingua-language-detector](https://pypi.org/project/lingua-language-detector/))
-- **Tigrinya** (not recognized by [lingua-language-detector](https://pypi.org/project/lingua-language-detector/))
+- Bengali <sub>(not possible to print correctly using [fpdf2](https://pypi.org/project/fpdf2/))</sub>
+- Dhivehi <sub>(not recognized by [lingua-language-detector](https://pypi.org/project/lingua-language-detector/))</sub>
+- Kannada <sub>(not recognized by [lingua-language-detector](https://pypi.org/project/lingua-language-detector/))</sub>
+- Khmer <sub>(not recognized by [lingua-language-detector](https://pypi.org/project/lingua-language-detector/))</sub>
+- Lao <sub>(not recognized by [lingua-language-detector](https://pypi.org/project/lingua-language-detector/))</sub>
+- Malayalam <sub>(not recognized by [lingua-language-detector](https://pypi.org/project/lingua-language-detector/))</sub>
+- Meiteilon (manipuri) <sub>(not recognized by [lingua-language-detector](https://pypi.org/project/lingua-language-detector/))</sub>
+- Myanmar burmese <sub>(not possible to print correctly using [fpdf2](https://pypi.org/project/fpdf2/))</sub>
+- Odia (Oriya) <sub>(not recognized by [lingua-language-detector](https://pypi.org/project/lingua-language-detector/))</sub></sub>
+- Sinhala <sub>(not recognized by [lingua-language-detector](https://pypi.org/project/lingua-language-detector/))</sub>
+- Tigrinya <sub>(not recognized by [lingua-language-detector](https://pypi.org/project/lingua-language-detector/))</sub>
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 <!-- ROADMAP -->
 
 ## Roadmap
 
+- [x] Add support for converting a file (not `.xml` or `.strings`) into a strings resource file (`.xml` or `.strings`).
 - [ ] Add support for multiple `.xml`/`.strings` files input.
-- [ ] Add support for converting a file (not `.xml` nor `.strings`) to a strings resource file.
 - [ ] Make a web version.
 
-You can propose a new feature creating an [issue](https://github.com/HenestrosaConH/mobile-strings-converter/new/choose).
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
+You can propose a new feature creating an [issue](https://github.com/HenestrosaDev/mobile-strings-converter/new/choose).
 
 <!-- CONTRIBUTING -->
 
 ## Contributing
 
 Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.
-Please, read the [CONTRIBUTING.md](https://github.com/HenestrosaConH/mobile-strings-converter/blob/main/.github/CONTRIBUTING.md) file, where you can find more detailed information about how to contribute to the project.
-
-<p align="right">(<a href="#top">back to top</a>)</p>
+Please, read the [CONTRIBUTING.md](https://github.com/HenestrosaDev/mobile-strings-converter/blob/main/.github/CONTRIBUTING.md) file, where you can find more detailed information about how to contribute to the project.
 
 <!-- LICENSE -->
 
 ## License
 
 Distributed under the MIT License. See `LICENSE` for more information.
 
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
 <!-- AUTHORS -->
 
 ## Authors
 
-- HenestrosaConH <henestrosaconh@gmail.com> (José Carlos López Henestrosa)
+- HenestrosaDev <henestrosadev@gmail.com> (José Carlos López Henestrosa)
 
-See also the list of [contributors](https://github.com/HenestrosaConH/mobile-strings-converter/contributors) who participated in this project.
-
-<p align="right">(<a href="#top">back to top</a>)</p>
+See also the list of [contributors](https://github.com/HenestrosaDev/mobile-strings-converter/contributors) who participated in this project.
 
 <!-- ACKNOWLEDGMENTS -->
 
 ## Acknowledgments
 
 I have made use of the following resources to make this project:
 
-- [Best-README-Template](https://github.com/othneildrew/Best-README-Template/)
-- [Img Shields](https://shields.io)
 - [How to create a Python package](https://mathspp.com/blog/how-to-create-a-python-package-in-2022#how-to-create-a-python-package)
-- [Icon created by Midjourney](https://www.midjourney.com/app/)
-
-<p align="right">(<a href="#top">back to top</a>)</p>
 
 <!-- SUPPORT -->
 
 ## Support
 
-[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/U7U5J6COZ)
+Would you like to support the project? That's very kind of you! You can go to my Ko-Fi profile by clicking on the button down below.
+
+[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/henestrosadev)
 
 <p align="right">(<a href="#top">back to top</a>)</p>
```

#### html2text {}

```diff
@@ -1,189 +1,182 @@
 
                                     [Logo]
-                     ********** MMoobbiillee ssttrriinnggss ccoonnvveerrtteerr **********
+                    ************ MMoobbiillee SSttrriinnggss CCoonnvveerrtteerr ************
   A Python package that converts Android & iOS strings files to any supported
                                   file type.
 
                     _[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_ _s_u_p_p_o_r_t_]
                    _[_G_i_t_H_u_b_ _a_c_t_i_o_n_:_ _B_u_i_l_d_]_[_C_o_d_e_c_o_v_]_[_L_i_c_e_n_s_e_]
               _[_G_i_t_H_u_b_ _C_o_n_t_r_i_b_u_t_o_r_s_]_[_I_s_s_u_e_s_]_[_G_i_t_H_u_b_ _p_u_l_l_ _r_e_q_u_e_s_t_s_]
 
                  _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e Â· _A_s_k_ _Q_u_e_s_t_i_o_n
-## Table of Contents - [About the Project](#about-the-project) - [Project
-Structure](#project-structure) - [Built With](#built-with) - [Release Files]
-(#release-files) - [Usage](#usage) - [To Execute the Script](#to-execute-the-
-script) - [To Import the Package Into Your Project](#to-import-the-package-
-into-your-project) - [To Open the Code](#to-open-the-code) - [Notes](#notes) -
-[List of Indic Languages Supported by PDF files](#list-of-indic-languages-
-supported-by-pdf-files) - [List of Languages Not Supported by PDF files](#list-
-of-languages-not-supported-by-pdf-files) - [Roadmap](#roadmap) - [Contributing]
-(#contributing) - [License](#license) - [Authors](#authors) - [Acknowledgments]
-(#acknowledgments) - [Support](#support) ## About the Project I tried to do the
-whole process of converting a strings resource file into a spreadsheet in
-Google Sheets by hand and, even though you can do it with the option **Data >
-Split text to columns**, it involves wasting your time generating the
-spreadsheet manually. Due to that, I decided to build a time-efficient
-solution, which consists on running a Python script in order to achieve that
-with any file type. Moreover, not only this script can be executed on its own,
-it also can be installed as a package via **PyPI** (more information [here]
-(#to-import-the-package-into-your-project) about how to install it). The file
-types supported by the package are the following: - Android strings format
-(`*.xml`) - CSV - Google Sheets support - HTML - iOS strings format
-(`*.strings`) - JSON - MD - ODS - PDF - XLSX - YAML ### Project Structure ####
-Root directories: - `.github/workflows`: GitHub workflows. It also includes the
-templates for issues and pull requests, as well as the `depandabot.yml` file
-for Dependabot configuration. - `docs`: Contains files related to the
-documentation of the project. - `src/mobile_strings_converter`: Contains the
-source code files. - `tests`: Contains unit tests to ensure the correct
-functionality of the package. It also includes the `files` directory, which
-contains a few demo files in different formats to use in the unit tests. ####
-Root files: - `.gitignore`: File used by the version control system Git to
-specify files or directories that should be ignored by Git when tracking
-changes to a project. - `.pre-commit-config.yaml`: Configuration file used by
-**pre-commit**, a tool that runs checks (such as linting, testing, or
-formatting) on the code before you commit changes to version control. The file
-specifies which checks pre-commit should run and how it should run them. -
-`LICENSE`: Project license, which is [MIT](https://opensource.org/license/mit/
-). - `poetry.lock`: File generated by **Poetry**, a package manager for Python,
-that contains the exact versions of all packages used by a project. The file is
-used to ensure that all members of a development team are using the same
-versions of packages, even if different versions are available in the package
-repository. - `pyproject.toml`: Configuration file used by **Poetry**. It
-specifies the metadata for a Python project, including the project name,
-version, description, author, license and dependencies. - `README.md`: What you
-are reading right now. - `requirements.txt`: Lists the names and versions of
-each package used to build this project. To install the requirements, execute
-`pip install -r requirements.txt`. - `requirements-dev.txt`: Lists the names
-and versions of each package used in the development stage of this project. To
-install the requirements, execute `pip install -r requirements-dev.txt`. ###
-Built With - [openpyxl](https://pypi.org/project/openpyxl/): To generate ODS
-and XLSX files. - [gspread](https://pypi.org/project/gspread/): To generate
-spreadsheets in Google Sheets. - [protobuf](https://pypi.org/project/
-oauth2client/): Used by `google.oauth2.credentials` to authenticate to the
-user's Google account in order to create the spreadsheet in Google Sheets. -
-[PyYAML](https://pypi.org/project/PyYAML/): To generate YAML files. - [arabic-
-reshaper](https://pypi.org/project/arabic-reshaper/) and [python-bidi](https://
-pypi.org/project/python-bidi/): To add arabic characters support for PDF files.
-- [fpdf2](https://pypi.org/project/fpdf2/): To generate PDF files. - [lingua-
-language-detector](https://pypi.org/project/lingua-language-detector/): To
-recognize the **value** language when writing a PDF in order to know what font
-to use.
+## Table of Contents - [About the Project](#about-the-project) - [File Types
+Supported](#file-types-supported) - [Project Structure](#project-structure) -
+[Built With](#built-with) - [Release Files](#release-files) - [Getting Started]
+(#getting-started) - [Script Installation](#script-installation) - [Package
+Installation](#package-installation) - [Usage](#usage) - [Run the Program]
+(#run-the-program) - [Script Flags](#script-flags) - [Using the Package in Your
+Project](#using-the-package-in-your-project) - [Generate a Spreadsheet in
+Google Sheets](#generate-a-spreadsheet-in-google-sheets) - [Notes](#notes) -
+[Indic Languages Supported by PDF files](#indic-languages-supported-by-pdf-
+files) - [Languages Not Supported by PDF files](#languages-not-supported-by-
+pdf-files) - [Roadmap](#roadmap) - [Contributing](#contributing) - [License]
+(#license) - [Authors](#authors) - [Acknowledgments](#acknowledgments) -
+[Support](#support) ## About the Project I tried to do the whole process of
+converting a strings resource file into a spreadsheet in Google Sheets by hand
+and, even though you can do it with the option **Data > Split text to
+columns**, it involves wasting your time generating the spreadsheet manually.
+Due to that, I decided to build a time-efficient solution, which consists on
+running a Python script in order to achieve that with any file type. Moreover,
+not only this script can be executed on its own, it also can be installed as a
+package via **PyPI** (more information [here](#using-the-package-in-your-
+project) about how to install it). ### File Types Supported - Android strings
+format (`*.xml`) - CSV - Google Sheets support - HTML - iOS strings format
+(`*.strings`) - JSON - MD - ODS - PDF - XLSX - YAML ### Project Structure ASCII
+folder structure ``` â .gitignore â .pre-commit-config.yaml â LICENSE â
+poetry.lock â pyproject.toml â README.md â requirements.txt â
+requirements-dev.txt â ââââ.github â â CONTRIBUTING.md â â
+â ââââISSUE_TEMPLATE â â bug_report_template.md â â
+feature_request_template.md â â â ââââPULL_REQUEST_TEMPLATE â
+pull_request_template.md â ââââdocs â icon.png â ââââsrc
+â ââââmobile_strings_converter â â console_style.py â â
+converter.py â â __init__.py â â __main__.py â â â
+ââââassets â â ââââfonts â â Aakar.ttf â â
+AnekTelugu-VariableFont_wdth,wght.ttf â â DejaVuSansCondensed.ttf â â
+Eunjin.ttf â â fireflysung.ttf â â gargi.ttf â â
+Gurvetica_a8_Heavy.ttf â â Latha.ttf â â Waree.ttf â â â
+ââââcontroller â â main_controller.py â â __init__.py â â
+â ââââmodel â â transcription.py â â __init__.py â â â
+ââââutils â â constants.py â â i18n.py â â path_helper.py
+â â __init__.py â â â ââââview â main_window.py â
+__init__.py â ââââtests â base_tests.py â test_get_strings.py â
+test_to_android.py â test_to_csv.py â test_to_html.py â test_to_ios.py
+â test_to_json.py â test_to_md.py â test_to_ods.py â test_to_pdf.py â
+test_to_xlsx.py â test_to_yaml.py â ââââfiles ââââinput â
+Localizable.strings â strings.xml â ââââtemplate-with-comments â
+Localizable.strings â strings.csv â strings.html â strings.json â
+strings.md â strings.ods â strings.pdf â strings.xlsx â strings.xml â
+strings.yaml â ââââtemplate-without-comments Localizable.strings
+strings.csv strings.html strings.json strings.md strings.ods strings.pdf
+strings.xlsx strings.xml strings.yaml ``` ### Built With - [openpyxl](https://
+pypi.org/project/openpyxl/) to generate ODS and XLSX files. - [gspread](https:/
+/pypi.org/project/gspread/) to generate spreadsheets in Google Sheets. -
+[protobuf](https://pypi.org/project/oauth2client/) is used by
+`google.oauth2.credentials` to authenticate to the user's Google account in
+order to create the spreadsheet in Google Sheets. - [PyYAML](https://pypi.org/
+project/PyYAML/) to generate YAML files. - [arabic-reshaper](https://pypi.org/
+project/arabic-reshaper/) and [python-bidi](https://pypi.org/project/python-
+bidi/) to add arabic characters support for PDF files. - [fpdf2](https://
+pypi.org/project/fpdf2/) to generate PDF files. - [lingua-language-detector]
+(https://pypi.org/project/lingua-language-detector/) to recognize the **value**
+language when writing a PDF in order to know what font to use.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Release Files | File | Description | Size | |:------------------------------
 -------------------------------------------------------------------------------
-------------------------------------------------|:-----------------------------
+-----------------------------------|:------------------------------------------
+----------------------------------------------------------|:--------| |
+[mobile-strings-converter.zip](https://github.com/HenestrosaDev/mobile-strings-
+converter/releases/latest/download/mobile-strings-converter.zip) | PDF file
+support for almost all languages ([see exceptions](#languages-not-supported-by-
+pdf-files)) | 8.43 MB |
+                                                                  (_b_a_c_k_ _t_o_ _t_o_p)
+## Getting Started ### Script Installation 1. Download the [release](#release-
+files) that is best suited to your needs. 2. (Optional but recommended) Create
+a Python virtual environment in the project root. If you're using `virtualenv`,
+you would run `virtualenv venv`. 3. (Optional but recommended) Activate the
+virtual environment: ```bash # on Windows . venv/Scripts/activate # if you get
+the error `FullyQualifiedErrorId : UnauthorizedAccess`, run this: Set-
+ExecutionPolicy Unrestricted -Scope Process # and then . venv/Scripts/activate
+# on macOS and Linux source venv/Scripts/activate ``` 4. Open the command line
+and run `pip install -r path/to/requirements.txt` to install the required
+packages to run the script. ### Package Installation Install the PyPI package
+by running `pip install mobile-strings-converter`.
+                                                                  (_b_a_c_k_ _t_o_ _t_o_p)
+## Usage ### Run the Program For a basic usage, you can run the following
+command: ``` python path/to/mobile_strings_converter.py *.[SUPPORTED_FILE_TYPE]
+-o *.[SUPPORTED_FILE_TYPE] ``` See [Generate a Spreadsheet in Google Sheets]
+(#generate-a-spreadsheet-in-google-sheets) to create a spreadsheet. #### Script
+Flags | Flag | Description | |:----------------------------|:------------------
 -------------------------------------------------------------------------------
-|:----------| | [mobile-strings-converter.zip](https://github.com/
-HenestrosaConH/mobile-strings-converter/releases/latest/download/mobile-
-strings-converter.zip) | Standard language support for PDF files (over 100
-languages, including RTL) | 0.32 MB | | [mobile-strings-converter-indic.zip]
-(https://github.com/HenestrosaConH/mobile-strings-converter/releases/latest/
-download/mobile-strings-converter-indic.zip) | PDF file support for Indic
-languages ([see list](#list-of-indic-languages-supported-by-pdf-files)) | 1.40
-MB | | [mobile-strings-converter-zh-ja.zip](https://github.com/HenestrosaConH/
-mobile-strings-converter/releases/latest/download/mobile-strings-converter-zh-
-ja.zip) | PDF file support for Japanese and Chinese (simplified and
-traditional) | 7.17 MB | | [mobile-strings-converter-ko.zip](https://
-github.com/HenestrosaConH/mobile-strings-converter/releases/latest/download/
-mobile-strings-converter-ko.zip) | PDF file support for Korean | 0.46 MB | |
-[mobile-strings-converter-th.zip](https://github.com/HenestrosaConH/mobile-
-strings-converter/releases/latest/download/mobile-strings-converter-th.zip) |
-PDF file support for Thai | 0.37 MB | | [mobile-strings-converter-all.zip]
-(https://github.com/HenestrosaConH/mobile-strings-converter/releases/latest/
-download/mobile-strings-converter-all.zip) | PDF file support for almost all
-languages ([see exceptions](#list-of-languages-not-supported-by-pdf-files)) |
-8.43 MB |
-                                                                  (_b_a_c_k_ _t_o_ _t_o_p)
-## Usage ### To Execute The Script 1. Download the [release](#release-files)
-that is best suited to your needs. 2. Open the command line and run `pip
-install -r path/to/requirements.txt` to install the required packages to
-execute the script. 3. Example of a basic command to convert a `.xml` or
-`.strings` file to another file type: ``` path/to/python path/to/
-mobile_strings_converter.py path/to/<*.xml | *.strings> -o path/to/*. ``` ####
-To Generate a Spreadsheet in Google Sheets Before going further into running
-the commands to do so, please note that you will have to generate a
+-------------------------------------------------------------------| | `-h` or
+`--help` | Displays help text for the program | | `-o` or `--output-filepath` |
+Specifies the filepath for storing the converted file. The file extension can
+be chosen from the list of supported file types mentioned [here](#about-the-
+project). | | `-g` or `--google-sheets` | Followed by the name of the sheet,
+creates a new Google Sheets spreadsheet with the specified name. | | `-c` or `-
+-credentials` | Followed by the path to your `service_account.json` file is
+mandatory if you want to generate a spreadsheet in your Google account. | | `-
+p` or `--print-comments` | The output file will include any commented strings
+present in the original file. |
+                                                                  (_b_a_c_k_ _t_o_ _t_o_p)
+### Using the Package in Your Project Once you have followed the steps of the
+[Getting Started](#getting-started) section, import the package and the wrapper
+function(s) you want to use: ```python # Using the `get_strings` function from
+mobile_strings_converter import get_strings get_strings( input_filepath=Path
+("strings.xml"), should_print_comments=True ) ``` ### Generate a Spreadsheet in
+Google Sheets #### Set Up Google Account Before going further into running the
+commands to do so, please note that you will have to generate a
 `service_account.json` file. You can do the following to get one: 1. Go to the
 [Google Cloud Console](https://console.cloud.google.com/). 2. Create a new
 project or select an existing project. 3. Go to the **APIs & Services** page,
 click on **Dashboard** and then click on **Enable APIs and Services**. 4.
 Search for **Google Sheets API** and enable it. 5. Go to the **Credentials**
 page, click on **Create credentials**, and then choose **Service account**. 6.
 Give your service account a name and select a role. For this purpose, you can
 select **Project -> Editor**. 7. Click on the **Create key** button, select the
 JSON format and download the `service_account.json` file. 8. Share your Google
 Sheets file with the email address that is specified in the **client_email**
-field in the `service_account.json` file. Alternatively, you can create an XLSX
-file and open it in Google Sheets if you do not want to go through the hassle
-of generating the `service_account.json` file. Once you have generated the
-`service_account.json` file, you can generate a spreadsheet in Google Sheets by
-running the following command: ``` path/to/python path/to/
-mobile_strings_converter.py path/to/
- Localizable.strings> -gs -c path/to/service_account.json ``` If you want to
-generate an output file along with the spreadsheet, run this: ``` path/to/
-python path/to/mobile_strings_converter.py path/to/
- Localizable.strings> -gs -c path/to/service_account.json -o path/to/strings.
-``` #### Script flags - `-h`, `--help`: Show help - `-o`, `--output-filepath`:
-Output filepath where you want to store the converted file. Its extension can
-be any of the file types listed [here](#about-the-project). - `-g`, `--google-
-sheets` : Creates a spreadsheet in Google Sheets with the name passed as
-argument. - `-c`, `--credentials` <`service_account.json` filepath>: Mandatory
-if you want to generate a spreadsheet in your Google account. - `-p`, `--print-
-comments`: If present, indicates that commented strings will be printed in the
-output file. ### To Import the Package Into Your Project 1. Run `pip install
-mobile-strings-converter` 2. Import the package and the wrapper function with
-this line of code: `from mobile_strings_converter import convert_strings`. ###
-To Open the Code 1. Clone the project with the `git clone https://github.com/
-HenestrosaConH/mobile-strings-converter.git` command. 2. Open it in your
-favourite IDE (mine is [PyCharm](https://www.jetbrains.com/pycharm/))
-                                                                  (_b_a_c_k_ _t_o_ _t_o_p)
-## Notes ### List of Indic Languages Supported by PDF files - Hindi - Marathu -
-Oriya - Tibetan - Gujarati - Telugu - Tamil - Punjabi ### List of Languages Not
-Supported by PDF files - **Bengali** (not possible to print correctly using
-[fpdf2](https://pypi.org/project/fpdf2/)) - **Dhivehi** (not recognized by
+field in the `service_account.json` file. Alternatively, you can create a
+`.xlsx` file and open it in Google Sheets if you do not want to go through the
+hassle of generating the `service_account.json` file. Once you have generated
+the `service_account.json` file, you can generate a spreadsheet in Google
+Sheets by running the following command: ``` python path/to/
+mobile_strings_converter.py <*.xml | *.strings> -g -c path/to/
+service_account.json ``` If you want to generate an output file along with the
+spreadsheet, run this: ``` python path/to/mobile_strings_converter.py *.
+[SUPPORTED_FILE_TYPE -g -c path/to/service_account.json -o *.
+[SUPPORTED_FILE_TYPE] ``` #### Using the `to_google_sheets` Function in Your
+Project ```python from mobile_strings_converter import to_google_sheets
+to_google_sheets( input_filepath=Path("path/to/strings-file"),
+sheet_name="MyProject strings", credentials_filepath=Path("path/to/
+service_account.json"), should_print_comments=True, ) ``` ## Notes ### Indic
+Languages Supported by PDF files - Hindi - Marathu - Oriya - Tibetan - Gujarati
+- Telugu - Tamil - Punjabi ### Languages Not Supported by PDF files - Bengali
+(not possible to print correctly using [fpdf2](https://pypi.org/project/fpdf2/
+)) - Dhivehi (not recognized by [lingua-language-detector](https://pypi.org/
+project/lingua-language-detector/)) - Kannada (not recognized by [lingua-
+language-detector](https://pypi.org/project/lingua-language-detector/)) - Khmer
+(not recognized by [lingua-language-detector](https://pypi.org/project/lingua-
+language-detector/)) - Lao (not recognized by [lingua-language-detector](https:
+//pypi.org/project/lingua-language-detector/)) - Malayalam (not recognized by
 [lingua-language-detector](https://pypi.org/project/lingua-language-detector/))
-- **Kannada** (not recognized by [lingua-language-detector](https://pypi.org/
-project/lingua-language-detector/)) - **Khmer** (not recognized by [lingua-
-language-detector](https://pypi.org/project/lingua-language-detector/)) -
-**Lao** (not recognized by [lingua-language-detector](https://pypi.org/project/
-lingua-language-detector/)) - **Malayalam** (not recognized by [lingua-
-language-detector](https://pypi.org/project/lingua-language-detector/)) -
-**Meiteilon (manipuri)** (not recognized by [lingua-language-detector](https://
-pypi.org/project/lingua-language-detector/)) - **Myanmar burmese** (not
-possible to print correctly using [fpdf2](https://pypi.org/project/fpdf2/)) -
-**Odia (Oriya)** (not recognized by [lingua-language-detector](https://
-pypi.org/project/lingua-language-detector/)) - **Sinhala** (not recognized by
-[lingua-language-detector](https://pypi.org/project/lingua-language-detector/))
-- **Tigrinya** (not recognized by [lingua-language-detector](https://pypi.org/
-project/lingua-language-detector/))
-                                                                  (_b_a_c_k_ _t_o_ _t_o_p)
-## Roadmap - [ ] Add support for multiple `.xml`/`.strings` files input. - [ ]
-Add support for converting a file (not `.xml` nor `.strings`) to a strings
-resource file. - [ ] Make a web version. You can propose a new feature creating
-an [issue](https://github.com/HenestrosaConH/mobile-strings-converter/new/
-choose).
-                                                                  (_b_a_c_k_ _t_o_ _t_o_p)
-## Contributing Contributions are what make the open source community such an
-amazing place to learn, inspire, and create. Any contributions you make are
-**greatly appreciated**. Please, read the [CONTRIBUTING.md](https://github.com/
-HenestrosaConH/mobile-strings-converter/blob/main/.github/CONTRIBUTING.md)
-file, where you can find more detailed information about how to contribute to
-the project.
-                                                                  (_b_a_c_k_ _t_o_ _t_o_p)
-## License Distributed under the MIT License. See `LICENSE` for more
-information.
-                                                                  (_b_a_c_k_ _t_o_ _t_o_p)
-## Authors - HenestrosaConH
+- Meiteilon (manipuri) (not recognized by [lingua-language-detector](https://
+pypi.org/project/lingua-language-detector/)) - Myanmar burmese (not possible to
+print correctly using [fpdf2](https://pypi.org/project/fpdf2/)) - Odia (Oriya)
+(not recognized by [lingua-language-detector](https://pypi.org/project/lingua-
+language-detector/))
+ - Sinhala (not recognized by [lingua-language-detector](https://pypi.org/
+project/lingua-language-detector/)) - Tigrinya (not recognized by [lingua-
+language-detector](https://pypi.org/project/lingua-language-detector/))
+                                                                  (_b_a_c_k_ _t_o_ _t_o_p)
+## Roadmap - [x] Add support for converting a file (not `.xml` or `.strings`)
+into a strings resource file (`.xml` or `.strings`). - [ ] Add support for
+multiple `.xml`/`.strings` files input. - [ ] Make a web version. You can
+propose a new feature creating an [issue](https://github.com/HenestrosaDev/
+mobile-strings-converter/new/choose). ## Contributing Contributions are what
+make the open source community such an amazing place to learn, inspire, and
+create. Any contributions you make are **greatly appreciated**. Please, read
+the [CONTRIBUTING.md](https://github.com/HenestrosaDev/mobile-strings-
+converter/blob/main/.github/CONTRIBUTING.md) file, where you can find more
+detailed information about how to contribute to the project. ## License
+Distributed under the MIT License. See `LICENSE` for more information. ##
+Authors - HenestrosaDev
 gmail.com> (JosÃ© Carlos LÃ³pez Henestrosa) See also the list of [contributors]
-(https://github.com/HenestrosaConH/mobile-strings-converter/contributors) who
-participated in this project.
-                                                                  (_b_a_c_k_ _t_o_ _t_o_p)
-## Acknowledgments I have made use of the following resources to make this
-project: - [Best-README-Template](https://github.com/othneildrew/Best-README-
-Template/) - [Img Shields](https://shields.io) - [How to create a Python
-package](https://mathspp.com/blog/how-to-create-a-python-package-in-2022#how-
-to-create-a-python-package) - [Icon created by Midjourney](https://
-www.midjourney.com/app/)
-                                                                  (_b_a_c_k_ _t_o_ _t_o_p)
-## Support [![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-
-fi.com/U7U5J6COZ)
+(https://github.com/HenestrosaDev/mobile-strings-converter/contributors) who
+participated in this project. ## Acknowledgments I have made use of the
+following resources to make this project: - [How to create a Python package]
+(https://mathspp.com/blog/how-to-create-a-python-package-in-2022#how-to-create-
+a-python-package) ## Support Would you like to support the project? That's very
+kind of you! You can go to my Ko-Fi profile by clicking on the button down
+below. [![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/
+henestrosadev)
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
```

### Comparing `mobile_strings_converter-0.1.1/pyproject.toml` & `mobile_strings_converter-0.1.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "mobile-strings-converter"
-version = "0.1.1"
-description = "A Python package that converts Android & iOS strings files to any supported file type."
-authors = ["José Carlos López <henestrosaconh@gmail.com>"]
+version = "0.1.3"
+description = "Convert Android & iOS strings files to any supported file type and vice versa."
+authors = ["José Carlos López <henestrosadev@gmail.com>"]
 license = "MIT"
 classifiers=[
     "Intended Audience :: Developers",
     "Environment :: Console",
     "Topic :: Text Processing :: General",
     "Topic :: Utilities",
     "Operating System :: OS Independent",
@@ -29,32 +29,34 @@
     "json",
     "ods",
     "pdf",
     "md",
     "ios",
     "Localizable.strings"
 ]
-repository="https://github.com/HenestrosaConH/mobile-strings-converter"
+repository="https://github.com/HenestrosaDev/mobile-strings-converter"
 readme = "README.md"
 packages = [{include = "mobile_strings_converter", from = "src"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
-pyyaml = "^6.0"
-protobuf = "^4.21.12"
-gspread = "^5.7.2"
-openpyxl = "^3.1.0"
-fpdf2 = "^2.6.1"
-lingua-language-detector = "^1.3.2"
+pyyaml = "^6.0.1"
+protobuf = "^5.26.1"
+gspread = "^6.1.0"
+openpyxl = "^3.1.2"
+fpdf2 = "^2.7.8"
+lingua-language-detector = "^2.0.2"
 python-bidi = "^0.4.2"
 arabic-reshaper = "^3.0.0"
+ezodf = "^0.3.2"
+pypdf2 = "^3.0.1"
 
 
 [tool.poetry.group.dev.dependencies]
-pre-commit = "^3.0.4"
+pre-commit = "^3.5.0"
 codecov = "^2.1.12"
 
 [tool.poetry.group.test.dependencies]
 pandas = "^1.5.3"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `mobile_strings_converter-0.1.1/src/mobile_strings_converter/__main__.py` & `mobile_strings_converter-0.1.3/src/mobile_strings_converter/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -46,21 +46,14 @@
         help="If called, indicates that commented strings will be printed in the "
         "output file.",
     )
     args = parser.parse_args()
 
     input_filepath = Path(args.input_filepath)
 
-    if input_filepath.suffix not in [".strings", ".xml"]:
-        print(
-            f"{ConsoleStyle.RED}Invalid input file. Its extension must be .strings "
-            f"for iOS strings or .xml for Android strings.{ConsoleStyle.RED}"
-        )
-        return
-
     if args.google_sheets and not args.credentials:
         print(
             f"{ConsoleStyle.RED}Error: You need to pass the path of the "
             f"`service_account.json` file to generate a Sheet.{ConsoleStyle.END}"
         )
         return
     elif not args.google_sheets and args.credentials:
@@ -73,12 +66,12 @@
         to_google_sheets(
             input_filepath,
             sheet_name=args.google_sheets,
             credentials_filepath=Path(args.credentials),
             should_print_comments=args.print_comments,
         )
 
-    convert_strings(input_filepath, Path(args.output_path), args.print_comments)
+    convert_strings(input_filepath, Path(args.output_filepath), args.print_comments)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `mobile_strings_converter-0.1.1/src/mobile_strings_converter/assets/fonts/Aakar.ttf` & `mobile_strings_converter-0.1.3/src/mobile_strings_converter/assets/fonts/Aakar.ttf`

 * *Files identical despite different names*

### Comparing `mobile_strings_converter-0.1.1/src/mobile_strings_converter/assets/fonts/AnekTelugu-VariableFont_wdth,wght.ttf` & `mobile_strings_converter-0.1.3/src/mobile_strings_converter/assets/fonts/AnekTelugu-VariableFont_wdth,wght.ttf`

 * *Files identical despite different names*

### Comparing `mobile_strings_converter-0.1.1/src/mobile_strings_converter/assets/fonts/DejaVuSansCondensed.ttf` & `mobile_strings_converter-0.1.3/src/mobile_strings_converter/assets/fonts/DejaVuSansCondensed.ttf`

 * *Files identical despite different names*

### Comparing `mobile_strings_converter-0.1.1/src/mobile_strings_converter/assets/fonts/Eunjin.ttf` & `mobile_strings_converter-0.1.3/src/mobile_strings_converter/assets/fonts/Eunjin.ttf`

 * *Files identical despite different names*

### Comparing `mobile_strings_converter-0.1.1/src/mobile_strings_converter/assets/fonts/Gurvetica_a8_Heavy.ttf` & `mobile_strings_converter-0.1.3/src/mobile_strings_converter/assets/fonts/Gurvetica_a8_Heavy.ttf`

 * *Files identical despite different names*

### Comparing `mobile_strings_converter-0.1.1/src/mobile_strings_converter/assets/fonts/Latha.ttf` & `mobile_strings_converter-0.1.3/src/mobile_strings_converter/assets/fonts/Latha.ttf`

 * *Files identical despite different names*

### Comparing `mobile_strings_converter-0.1.1/src/mobile_strings_converter/assets/fonts/Waree.ttf` & `mobile_strings_converter-0.1.3/src/mobile_strings_converter/assets/fonts/Waree.ttf`

 * *Files identical despite different names*

### Comparing `mobile_strings_converter-0.1.1/src/mobile_strings_converter/assets/fonts/fireflysung.ttf` & `mobile_strings_converter-0.1.3/src/mobile_strings_converter/assets/fonts/fireflysung.ttf`

 * *Files identical despite different names*

### Comparing `mobile_strings_converter-0.1.1/src/mobile_strings_converter/assets/fonts/gargi.ttf` & `mobile_strings_converter-0.1.3/src/mobile_strings_converter/assets/fonts/gargi.ttf`

 * *Files identical despite different names*

### Comparing `mobile_strings_converter-0.1.1/PKG-INFO` & `mobile_strings_converter-0.1.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 Metadata-Version: 2.1
 Name: mobile-strings-converter
-Version: 0.1.1
-Summary: A Python package that converts Android & iOS strings files to any supported file type.
-Home-page: https://github.com/HenestrosaConH/mobile-strings-converter
+Version: 0.1.3
+Summary: Convert Android & iOS strings files to any supported file type and vice versa.
+Home-page: https://github.com/HenestrosaDev/mobile-strings-converter
 License: MIT
 Keywords: android,strings.xml,strings,converter,csv,xlsx,yaml,html,json,ods,pdf,md,ios,Localizable.strings
 Author: José Carlos López
-Author-email: henestrosaconh@gmail.com
+Author-email: henestrosadev@gmail.com
 Requires-Python: >=3.8
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: Other OS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Text Processing :: General
 Classifier: Topic :: Utilities
 Requires-Dist: arabic-reshaper (>=3.0.0,<4.0.0)
-Requires-Dist: fpdf2 (>=2.6.1,<3.0.0)
-Requires-Dist: gspread (>=5.7.2,<6.0.0)
-Requires-Dist: lingua-language-detector (>=1.3.2,<2.0.0)
-Requires-Dist: openpyxl (>=3.1.0,<4.0.0)
-Requires-Dist: protobuf (>=4.21.12,<5.0.0)
+Requires-Dist: ezodf (>=0.3.2,<0.4.0)
+Requires-Dist: fpdf2 (>=2.7.8,<3.0.0)
+Requires-Dist: gspread (>=6.1.0,<7.0.0)
+Requires-Dist: lingua-language-detector (>=2.0.2,<3.0.0)
+Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
+Requires-Dist: protobuf (>=5.26.1,<6.0.0)
+Requires-Dist: pypdf2 (>=3.0.1,<4.0.0)
 Requires-Dist: python-bidi (>=0.4.2,<0.5.0)
-Requires-Dist: pyyaml (>=6.0,<7.0)
-Project-URL: Repository, https://github.com/HenestrosaConH/mobile-strings-converter
+Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
+Project-URL: Repository, https://github.com/HenestrosaDev/mobile-strings-converter
 Description-Content-Type: text/markdown
 
 <div id="top"></div>
 
 <!-- PROJECT SHIELDS -->
 <!--
 *** I am using markdown "reference style" links for readability.
@@ -46,83 +48,91 @@
 *** https://www.markdownguide.org/basic-syntax/#reference-style-links
 -->
 
 <!-- PROJECT LOGO -->
 <br />
 <div align="center">
     <img src="docs/icon.png" alt="Logo" width="156" height="156" style="margin-bottom:-40px">
-    <h2 align="center">Mobile strings converter</h2>
+    <h1 align="center">Mobile Strings Converter</h1>
     <p align="center">
         A Python package that converts Android & iOS strings files to any supported file type.
         <br />
         <br />
         <a href="https://pypi.org/project/mobile-strings-converter/">
           <img alt="PyPI version" src="https://img.shields.io/pypi/v/mobile-strings-converter" />
         </a>
         <a href="https://pypi.org/project/mobile-strings-converter/">
           <img alt="Python versions support" src="https://img.shields.io/pypi/pyversions/mobile-strings-converter" />
         </a>
         <br />
-        <a href="https://github.com/HenestrosaConH/mobile-strings-converter/actions/workflows/build.yaml">
-          <img alt="GitHub action: Build" src="https://github.com/HenestrosaConH/mobile-strings-converter/actions/workflows/build.yaml/badge.svg" />
+        <a href="https://github.com/HenestrosaDev/mobile-strings-converter/actions/workflows/build.yaml">
+          <img alt="GitHub action: Build" src="https://github.com/HenestrosaDev/mobile-strings-converter/actions/workflows/build.yaml/badge.svg" />
         </a>
-        <a href="https://codecov.io/gh/HenestrosaConH/mobile-strings-converter/">
-          <img alt="Codecov" src="https://codecov.io/gh/HenestrosaConH/mobile-strings-converter/branch/main/graph/badge.svg" />
+        <a href="https://codecov.io/gh/HenestrosaDev/mobile-strings-converter/">
+          <img alt="Codecov" src="https://codecov.io/gh/HenestrosaDev/mobile-strings-converter/branch/main/graph/badge.svg" />
         </a>
-        <a href="https://github.com/HenestrosaConH/mobile-strings-converter/blob/main/LICENSE">
-          <img alt="License" src="https://img.shields.io/github/license/HenestrosaConH/mobile-strings-converter" />
+        <a href="https://github.com/HenestrosaDev/mobile-strings-converter/blob/main/LICENSE">
+          <img alt="License" src="https://img.shields.io/github/license/HenestrosaDev/mobile-strings-converter" />
         </a>
         <br />
-        <a href="https://github.com/HenestrosaConH/mobile-strings-converter/graphs/contributors">
-          <img alt="GitHub Contributors" src="https://img.shields.io/github/contributors/HenestrosaConH/mobile-strings-converter" />
+        <a href="https://github.com/HenestrosaDev/mobile-strings-converter/graphs/contributors">
+          <img alt="GitHub Contributors" src="https://img.shields.io/github/contributors/HenestrosaDev/mobile-strings-converter" />
         </a>
-        <a href="https://github.com/HenestrosaConH/mobile-strings-converter/issues">
-          <img alt="Issues" src="https://img.shields.io/github/issues/HenestrosaConH/mobile-strings-converter" />
+        <a href="https://github.com/HenestrosaDev/mobile-strings-converter/issues">
+          <img alt="Issues" src="https://img.shields.io/github/issues/HenestrosaDev/mobile-strings-converter" />
         </a>
-        <a href="https://github.com/HenestrosaConH/mobile-strings-converter/pulls">
-          <img alt="GitHub pull requests" src="https://img.shields.io/github/issues-pr/HenestrosaConH/mobile-strings-converter" />
+        <a href="https://github.com/HenestrosaDev/mobile-strings-converter/pulls">
+          <img alt="GitHub pull requests" src="https://img.shields.io/github/issues-pr/HenestrosaDev/mobile-strings-converter" />
         </a>
         <br />
         <br />
-        <a href="https://github.com/HenestrosaConH/mobile-strings-converter/issues/new/choose">Report Bug</a> · <a href="https://github.com/HenestrosaConH/mobile-strings-converter/issues/new/choose">Request Feature</a> · <a href="https://github.com/HenestrosaConH/mobile-strings-converter/discussions">Ask Question</a>
+        <a href="https://github.com/HenestrosaDev/mobile-strings-converter/issues/new/choose">Report Bug</a> · <a href="https://github.com/HenestrosaDev/mobile-strings-converter/issues/new/choose">Request Feature</a> · <a href="https://github.com/HenestrosaDev/mobile-strings-converter/discussions">Ask Question</a>
     </p>
 </div>
 
 <!-- TABLE OF CONTENTS -->
 
 ## Table of Contents
 
 - [About the Project](#about-the-project)
+  - [File Types Supported](#file-types-supported) 
   - [Project Structure](#project-structure)
   - [Built With](#built-with)
 - [Release Files](#release-files)
+- [Getting Started](#getting-started)
+  - [Script Installation](#script-installation)
+  - [Package Installation](#package-installation)
 - [Usage](#usage)
-  - [To Execute the Script](#to-execute-the-script)
-  - [To Import the Package Into Your Project](#to-import-the-package-into-your-project)
-  - [To Open the Code](#to-open-the-code)
+  - [Run the Program](#run-the-program)
+    - [Script Flags](#script-flags)
+  - [Using the Package in Your Project](#using-the-package-in-your-project)
+  - [Generate a Spreadsheet in Google Sheets](#generate-a-spreadsheet-in-google-sheets)
 - [Notes](#notes)
-  - [List of Indic Languages Supported by PDF files](#list-of-indic-languages-supported-by-pdf-files)
-  - [List of Languages Not Supported by PDF files](#list-of-languages-not-supported-by-pdf-files)
+  - [Indic Languages Supported by PDF files](#indic-languages-supported-by-pdf-files)
+  - [Languages Not Supported by PDF files](#languages-not-supported-by-pdf-files)
 - [Roadmap](#roadmap)
 - [Contributing](#contributing)
 - [License](#license)
 - [Authors](#authors)
 - [Acknowledgments](#acknowledgments)
 - [Support](#support)
 
 <!-- ABOUT THE PROJECT -->
 
 ## About the Project
 
 I tried to do the whole process of converting a strings resource file into a spreadsheet in Google Sheets by hand and, even though you can do it with the option **Data > Split text to columns**, 
 it involves wasting your time generating the spreadsheet manually. Due to that, I decided to build a time-efficient solution, which consists on running a Python script in order to achieve that with any file type.
 
-Moreover, not only this script can be executed on its own, it also can be installed as a package via **PyPI** (more information [here](#to-import-the-package-into-your-project) about how to install it).
+Moreover, not only this script can be executed on its own, it also can be installed as a package via **PyPI** (more information [here](#using-the-package-in-your-project) about how to install it).
+
+<!-- FILE TYPES SUPPORTED -->
+
+### File Types Supported
 
-The file types supported by the package are the following:
 - Android strings format (`*.xml`)
 - CSV
 - Google Sheets support
 - HTML
 - iOS strings format (`*.strings`)
 - JSON
 - MD
@@ -131,204 +141,325 @@
 - XLSX
 - YAML
 
 <!-- PROJECT STRUCTURE -->
 
 ### Project Structure
 
-#### Root directories:
-
-- `.github/workflows`: GitHub workflows. It also includes the templates for issues and pull requests, as well as the `depandabot.yml` file for Dependabot configuration.
-- `docs`: Contains files related to the documentation of the project.
-- `src/mobile_strings_converter`:  Contains the source code files.
-- `tests`: Contains unit tests to ensure the correct functionality of the package. It also includes the `files` directory, which contains a few demo files in different formats to use in the unit tests.
-
-#### Root files:
-
-- `.gitignore`: File used by the version control system Git to specify files or directories that should be ignored by Git when tracking changes to a project.
-- `.pre-commit-config.yaml`: Configuration file used by **pre-commit**, a tool that runs checks (such as linting, testing, or formatting) on the code before you commit changes to version control. The file specifies which checks pre-commit should run and how it should run them.
-- `LICENSE`: Project license, which is [MIT](https://opensource.org/license/mit/).
-- `poetry.lock`: File generated by **Poetry**, a package manager for Python, that contains the exact versions of all packages used by a project. The file is used to ensure that all members of a development team are using the same versions of packages, even if different versions are available in the package repository.
-- `pyproject.toml`: Configuration file used by **Poetry**. It specifies the metadata for a Python project, including the project name, version, description, author, license and dependencies.
-- `README.md`: What you are reading right now.
-- `requirements.txt`: Lists the names and versions of each package used to build this project. To install the requirements, execute `pip install -r requirements.txt`.
-- `requirements-dev.txt`: Lists the names and versions of each package used in the development stage of this project. To install the requirements, execute `pip install -r requirements-dev.txt`.
+<details>
+  <summary>ASCII folder structure</summary>
 
+```
+│   .gitignore
+│   .pre-commit-config.yaml
+│   LICENSE
+│   poetry.lock 
+│   pyproject.toml
+│   README.md
+│   requirements.txt
+│   requirements-dev.txt
+│
+├───.github
+│   │   CONTRIBUTING.md
+│   │
+│   ├───ISSUE_TEMPLATE
+│   │       bug_report_template.md
+│   │       feature_request_template.md
+│   │
+│   └───PULL_REQUEST_TEMPLATE
+│           pull_request_template.md
+│
+├───docs
+│       icon.png
+│
+├───src
+│   ├───mobile_strings_converter
+│   │       console_style.py
+│   │       converter.py
+│   │       __init__.py
+│   │       __main__.py
+│   │
+│   ├───assets
+│   │       └───fonts
+│   │               Aakar.ttf
+│   │               AnekTelugu-VariableFont_wdth,wght.ttf
+│   │               DejaVuSansCondensed.ttf
+│   │               Eunjin.ttf
+│   │               fireflysung.ttf
+│   │               gargi.ttf
+│   │               Gurvetica_a8_Heavy.ttf
+│   │               Latha.ttf
+│   │               Waree.ttf
+│   │
+│   ├───controller
+│   │       main_controller.py
+│   │       __init__.py
+│   │
+│   ├───model
+│   │       transcription.py
+│   │       __init__.py
+│   │
+│   ├───utils
+│   │       constants.py
+│   │       i18n.py
+│   │       path_helper.py
+│   │       __init__.py
+│   │
+│   └───view
+│           main_window.py
+│           __init__.py
+│
+└───tests   
+    │   base_tests.py
+    │   test_get_strings.py
+    │   test_to_android.py
+    │   test_to_csv.py
+    │   test_to_html.py
+    │   test_to_ios.py
+    │   test_to_json.py
+    │   test_to_md.py
+    │   test_to_ods.py
+    │   test_to_pdf.py
+    │   test_to_xlsx.py
+    │   test_to_yaml.py
+    │
+    └───files
+        ├───input
+        │       Localizable.strings
+        │       strings.xml
+        │
+        ├───template-with-comments
+        │       Localizable.strings
+        │       strings.csv
+        │       strings.html
+        │       strings.json
+        │       strings.md
+        │       strings.ods
+        │       strings.pdf
+        │       strings.xlsx
+        │       strings.xml
+        │       strings.yaml
+        │
+        └───template-without-comments
+                Localizable.strings
+                strings.csv
+                strings.html
+                strings.json
+                strings.md
+                strings.ods
+                strings.pdf
+                strings.xlsx
+                strings.xml
+                strings.yaml
+```
+</details>
 
 <!-- BUILT WITH -->
 
 ### Built With
 
-- [openpyxl](https://pypi.org/project/openpyxl/): To generate ODS and XLSX files.
-- [gspread](https://pypi.org/project/gspread/): To generate spreadsheets in Google Sheets.
-- [protobuf](https://pypi.org/project/oauth2client/): Used by `google.oauth2.credentials` to authenticate to the user's Google account in order to create the spreadsheet in Google Sheets. 
-- [PyYAML](https://pypi.org/project/PyYAML/): To generate YAML files.
-- [arabic-reshaper](https://pypi.org/project/arabic-reshaper/) and [python-bidi](https://pypi.org/project/python-bidi/): To add arabic characters support for PDF files.
-- [fpdf2](https://pypi.org/project/fpdf2/): To generate PDF files.
-- [lingua-language-detector](https://pypi.org/project/lingua-language-detector/): To recognize the **value** language when writing a PDF in order to know what font to use.  
+- [openpyxl](https://pypi.org/project/openpyxl/) to generate ODS and XLSX files.
+- [gspread](https://pypi.org/project/gspread/) to generate spreadsheets in Google Sheets.
+- [protobuf](https://pypi.org/project/oauth2client/) is used by `google.oauth2.credentials` to authenticate to the user's Google account in order to create the spreadsheet in Google Sheets. 
+- [PyYAML](https://pypi.org/project/PyYAML/) to generate YAML files.
+- [arabic-reshaper](https://pypi.org/project/arabic-reshaper/) and [python-bidi](https://pypi.org/project/python-bidi/) to add arabic characters support for PDF files.
+- [fpdf2](https://pypi.org/project/fpdf2/) to generate PDF files.
+- [lingua-language-detector](https://pypi.org/project/lingua-language-detector/) to recognize the **value** language when writing a PDF in order to know what font to use.  
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 <!-- RELEASE FILES -->
 
 ## Release Files
 
-| File                                                                                                                                                         | Description                                                                                                 | Size      |
-|:-------------------------------------------------------------------------------------------------------------------------------------------------------------|:------------------------------------------------------------------------------------------------------------|:----------|
-| [mobile-strings-converter.zip](https://github.com/HenestrosaConH/mobile-strings-converter/releases/latest/download/mobile-strings-converter.zip)             | Standard language support for PDF files (over 100 languages, including RTL)                                 | 0.32 MB   |
-| [mobile-strings-converter-indic.zip](https://github.com/HenestrosaConH/mobile-strings-converter/releases/latest/download/mobile-strings-converter-indic.zip) | PDF file support for Indic languages ([see list](#list-of-indic-languages-supported-by-pdf-files))          | 1.40 MB   |
-| [mobile-strings-converter-zh-ja.zip](https://github.com/HenestrosaConH/mobile-strings-converter/releases/latest/download/mobile-strings-converter-zh-ja.zip) | PDF file support for Japanese and Chinese (simplified and traditional)                                      | 7.17 MB   |
-| [mobile-strings-converter-ko.zip](https://github.com/HenestrosaConH/mobile-strings-converter/releases/latest/download/mobile-strings-converter-ko.zip)       | PDF file support for Korean                                                                                 | 0.46 MB   |
-| [mobile-strings-converter-th.zip](https://github.com/HenestrosaConH/mobile-strings-converter/releases/latest/download/mobile-strings-converter-th.zip)       | PDF file support for Thai                                                                                   | 0.37 MB   |
-| [mobile-strings-converter-all.zip](https://github.com/HenestrosaConH/mobile-strings-converter/releases/latest/download/mobile-strings-converter-all.zip)     | PDF file support for almost all languages ([see exceptions](#list-of-languages-not-supported-by-pdf-files)) | 8.43 MB   |
+| File                                                                                                                                            | Description                                                                                         | Size    |
+|:------------------------------------------------------------------------------------------------------------------------------------------------|:----------------------------------------------------------------------------------------------------|:--------|
+| [mobile-strings-converter.zip](https://github.com/HenestrosaDev/mobile-strings-converter/releases/latest/download/mobile-strings-converter.zip) | PDF file support for almost all languages ([see exceptions](#languages-not-supported-by-pdf-files)) | 8.43 MB |
+
+<p align="right">(<a href="#top">back to top</a>)</p>
+
+<!-- GETTING STARTED -->
+
+## Getting Started
+
+### Script Installation
+
+1. Download the [release](#release-files) that is best suited to your needs.
+2. (Optional but recommended) Create a Python virtual environment in the project root. If you're using `virtualenv`, you would run `virtualenv venv`.
+3. (Optional but recommended) Activate the virtual environment:
+   ```bash
+   # on Windows
+   . venv/Scripts/activate
+   # if you get the error `FullyQualifiedErrorId : UnauthorizedAccess`, run this:
+   Set-ExecutionPolicy Unrestricted -Scope Process
+   # and then . venv/Scripts/activate
+   
+   # on macOS and Linux
+   source venv/Scripts/activate
+   ```
+4. Open the command line and run `pip install -r path/to/requirements.txt` to install the required packages to run the script.
+
+### Package Installation
+
+Install the PyPI package by running `pip install mobile-strings-converter`.
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 <!-- USAGE -->
 
 ## Usage
 
-### To Execute The Script
+### Run the Program
 
-1. Download the [release](#release-files) that is best suited to your needs.
-2. Open the command line and run `pip install -r path/to/requirements.txt` to install the required packages to execute the script.
-3. Example of a basic command to convert a `.xml` or `.strings` file to another file type: 
-    ```
-    path/to/python path/to/mobile_strings_converter.py path/to/<*.xml | *.strings> -o path/to/*.<SUPPORTED FILE TYPE EXTENSION>
-    ```
+For a basic usage, you can run the following command:
 
-#### To Generate a Spreadsheet in Google Sheets
+```
+python path/to/mobile_strings_converter.py *.[SUPPORTED_FILE_TYPE] -o *.[SUPPORTED_FILE_TYPE]
+```
+
+See [Generate a Spreadsheet in Google Sheets](#generate-a-spreadsheet-in-google-sheets) to create a spreadsheet.
+
+#### Script Flags
+
+| Flag                        | Description                                                                                                                                                         |
+|:----------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| `-h` or `--help`            | Displays help text for the program                                                                                                                                  |
+| `-o` or `--output-filepath` | Specifies the filepath for storing the converted file. The file extension can be chosen from the list of supported file types mentioned [here](#about-the-project). |
+| `-g` or `--google-sheets`   | Followed by the name of the sheet, creates a new Google Sheets spreadsheet with the specified name.                                                                 |
+| `-c` or `--credentials`     | Followed by the path to your `service_account.json` file is mandatory if you want to generate a spreadsheet in your Google account.                                 |
+| `-p` or `--print-comments`  | The output file will include any commented strings present in the original file.                                                                                    |
+
+<p align="right">(<a href="#top">back to top</a>)</p>
+
+### Using the Package in Your Project
+
+Once you have followed the steps of the [Getting Started](#getting-started) section, import the package and the wrapper function(s) you want to use: 
+```python
+# Using the `get_strings` function
+from mobile_strings_converter import get_strings  
+
+get_strings(
+   input_filepath=Path("strings.xml"), 
+   should_print_comments=True
+)
+```
+
+### Generate a Spreadsheet in Google Sheets
+
+#### Set Up Google Account
 
 Before going further into running the commands to do so, please note that you will have to generate a `service_account.json` file. You can do the following to get one:
 
 1. Go to the [Google Cloud Console](https://console.cloud.google.com/).
 2. Create a new project or select an existing project.
 3. Go to the **APIs & Services** page, click on **Dashboard** and then click on **Enable APIs and Services**.
 4. Search for **Google Sheets API** and enable it.
 5. Go to the **Credentials** page, click on **Create credentials**, and then choose **Service account**.
 6. Give your service account a name and select a role. For this purpose, you can select **Project -> Editor**.
 7. Click on the **Create key** button, select the JSON format and download the `service_account.json` file.
 8. Share your Google Sheets file with the email address that is specified in the **client_email** field in the `service_account.json` file.
 
-Alternatively, you can create an XLSX file and open it in Google Sheets if you do not want to go through the hassle of generating the `service_account.json` file.
+Alternatively, you can create a `.xlsx` file and open it in Google Sheets if you do not want to go through the hassle of generating the `service_account.json` file.
 
 Once you have generated the `service_account.json` file, you can generate a spreadsheet in Google Sheets by running the following command:
 ```
-path/to/python path/to/mobile_strings_converter.py path/to/<strings.xml | Localizable.strings> -gs <SHEET NAME> -c path/to/service_account.json 
+python path/to/mobile_strings_converter.py <*.xml | *.strings> -g <SHEET_NAME> -c path/to/service_account.json 
 ```
 
 If you want to generate an output file along with the spreadsheet, run this:
 ```
-path/to/python path/to/mobile_strings_converter.py path/to/<strings.xml | Localizable.strings> -gs <SHEET NAME> -c path/to/service_account.json -o path/to/strings.<SUPPORTED FILE TYPE EXTENSION>
+python path/to/mobile_strings_converter.py *.[SUPPORTED_FILE_TYPE -g <SHEET_NAME> -c path/to/service_account.json -o *.[SUPPORTED_FILE_TYPE]
 ```
 
-#### Script flags
+#### Using the `to_google_sheets` Function in Your Project
 
-- `-h`, `--help`: Show help
-- `-o`, `--output-filepath`: Output filepath where you want to store the converted file. Its extension can be any of the file types listed [here](#about-the-project).
-- `-g`, `--google-sheets` <spreadsheet name>: Creates a spreadsheet in Google Sheets with the name passed as argument.
-- `-c`, `--credentials` <`service_account.json` filepath>: Mandatory if you want to generate a spreadsheet in your Google account.
-- `-p`, `--print-comments`: If present, indicates that commented strings will be printed in the output file.
+```python
+from mobile_strings_converter import to_google_sheets
 
-### To Import the Package Into Your Project
-
-1. Run `pip install mobile-strings-converter`
-2. Import the package and the wrapper function with this line of code: `from mobile_strings_converter import convert_strings`.
-
-### To Open the Code
-
-1. Clone the project with the `git clone https://github.com/HenestrosaConH/mobile-strings-converter.git` command.
-2. Open it in your favourite IDE (mine is [PyCharm](https://www.jetbrains.com/pycharm/))
-
-<p align="right">(<a href="#top">back to top</a>)</p>
+to_google_sheets(
+    input_filepath=Path("path/to/strings-file"),
+    sheet_name="MyProject strings",
+    credentials_filepath=Path("path/to/service_account.json"),
+    should_print_comments=True,
+)
+```
 
 <!-- NOTES -->
 
 ## Notes
 
-### List of Indic Languages Supported by PDF files
+### Indic Languages Supported by PDF files
 
 - Hindi
 - Marathu
 - Oriya
 - Tibetan
 - Gujarati
 - Telugu
 - Tamil
 - Punjabi
 
-### List of Languages Not Supported by PDF files
+### Languages Not Supported by PDF files
 
-- **Bengali** (not possible to print correctly using [fpdf2](https://pypi.org/project/fpdf2/))
-- **Dhivehi** (not recognized by [lingua-language-detector](https://pypi.org/project/lingua-language-detector/))
-- **Kannada** (not recognized by [lingua-language-detector](https://pypi.org/project/lingua-language-detector/))
-- **Khmer** (not recognized by [lingua-language-detector](https://pypi.org/project/lingua-language-detector/))
-- **Lao** (not recognized by [lingua-language-detector](https://pypi.org/project/lingua-language-detector/))
-- **Malayalam** (not recognized by [lingua-language-detector](https://pypi.org/project/lingua-language-detector/))
-- **Meiteilon (manipuri)** (not recognized by [lingua-language-detector](https://pypi.org/project/lingua-language-detector/))
-- **Myanmar burmese** (not possible to print correctly using [fpdf2](https://pypi.org/project/fpdf2/))
-- **Odia (Oriya)** (not recognized by [lingua-language-detector](https://pypi.org/project/lingua-language-detector/))
-- **Sinhala** (not recognized by [lingua-language-detector](https://pypi.org/project/lingua-language-detector/))
-- **Tigrinya** (not recognized by [lingua-language-detector](https://pypi.org/project/lingua-language-detector/))
+- Bengali <sub>(not possible to print correctly using [fpdf2](https://pypi.org/project/fpdf2/))</sub>
+- Dhivehi <sub>(not recognized by [lingua-language-detector](https://pypi.org/project/lingua-language-detector/))</sub>
+- Kannada <sub>(not recognized by [lingua-language-detector](https://pypi.org/project/lingua-language-detector/))</sub>
+- Khmer <sub>(not recognized by [lingua-language-detector](https://pypi.org/project/lingua-language-detector/))</sub>
+- Lao <sub>(not recognized by [lingua-language-detector](https://pypi.org/project/lingua-language-detector/))</sub>
+- Malayalam <sub>(not recognized by [lingua-language-detector](https://pypi.org/project/lingua-language-detector/))</sub>
+- Meiteilon (manipuri) <sub>(not recognized by [lingua-language-detector](https://pypi.org/project/lingua-language-detector/))</sub>
+- Myanmar burmese <sub>(not possible to print correctly using [fpdf2](https://pypi.org/project/fpdf2/))</sub>
+- Odia (Oriya) <sub>(not recognized by [lingua-language-detector](https://pypi.org/project/lingua-language-detector/))</sub></sub>
+- Sinhala <sub>(not recognized by [lingua-language-detector](https://pypi.org/project/lingua-language-detector/))</sub>
+- Tigrinya <sub>(not recognized by [lingua-language-detector](https://pypi.org/project/lingua-language-detector/))</sub>
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 <!-- ROADMAP -->
 
 ## Roadmap
 
+- [x] Add support for converting a file (not `.xml` or `.strings`) into a strings resource file (`.xml` or `.strings`).
 - [ ] Add support for multiple `.xml`/`.strings` files input.
-- [ ] Add support for converting a file (not `.xml` nor `.strings`) to a strings resource file.
 - [ ] Make a web version.
 
-You can propose a new feature creating an [issue](https://github.com/HenestrosaConH/mobile-strings-converter/new/choose).
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
+You can propose a new feature creating an [issue](https://github.com/HenestrosaDev/mobile-strings-converter/new/choose).
 
 <!-- CONTRIBUTING -->
 
 ## Contributing
 
 Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.
-Please, read the [CONTRIBUTING.md](https://github.com/HenestrosaConH/mobile-strings-converter/blob/main/.github/CONTRIBUTING.md) file, where you can find more detailed information about how to contribute to the project.
-
-<p align="right">(<a href="#top">back to top</a>)</p>
+Please, read the [CONTRIBUTING.md](https://github.com/HenestrosaDev/mobile-strings-converter/blob/main/.github/CONTRIBUTING.md) file, where you can find more detailed information about how to contribute to the project.
 
 <!-- LICENSE -->
 
 ## License
 
 Distributed under the MIT License. See `LICENSE` for more information.
 
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
 <!-- AUTHORS -->
 
 ## Authors
 
-- HenestrosaConH <henestrosaconh@gmail.com> (José Carlos López Henestrosa)
+- HenestrosaDev <henestrosadev@gmail.com> (José Carlos López Henestrosa)
 
-See also the list of [contributors](https://github.com/HenestrosaConH/mobile-strings-converter/contributors) who participated in this project.
-
-<p align="right">(<a href="#top">back to top</a>)</p>
+See also the list of [contributors](https://github.com/HenestrosaDev/mobile-strings-converter/contributors) who participated in this project.
 
 <!-- ACKNOWLEDGMENTS -->
 
 ## Acknowledgments
 
 I have made use of the following resources to make this project:
 
-- [Best-README-Template](https://github.com/othneildrew/Best-README-Template/)
-- [Img Shields](https://shields.io)
 - [How to create a Python package](https://mathspp.com/blog/how-to-create-a-python-package-in-2022#how-to-create-a-python-package)
-- [Icon created by Midjourney](https://www.midjourney.com/app/)
-
-<p align="right">(<a href="#top">back to top</a>)</p>
 
 <!-- SUPPORT -->
 
 ## Support
 
-[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/U7U5J6COZ)
+Would you like to support the project? That's very kind of you! You can go to my Ko-Fi profile by clicking on the button down below.
+
+[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/henestrosadev)
 
 <p align="right">(<a href="#top">back to top</a>)</p>
```

#### html2text {}

```diff
@@ -1,211 +1,205 @@
-Metadata-Version: 2.1 Name: mobile-strings-converter Version: 0.1.1 Summary: A
-Python package that converts Android & iOS strings files to any supported file
-type. Home-page: https://github.com/HenestrosaConH/mobile-strings-converter
-License: MIT Keywords:
+Metadata-Version: 2.1 Name: mobile-strings-converter Version: 0.1.3 Summary:
+Convert Android & iOS strings files to any supported file type and vice versa.
+Home-page: https://github.com/HenestrosaDev/mobile-strings-converter License:
+MIT Keywords:
 android,strings.xml,strings,converter,csv,xlsx,yaml,html,json,ods,pdf,md,ios,Localizable.strings
-Author: JosÃ© Carlos LÃ³pez Author-email: henestrosaconh@gmail.com Requires-
+Author: JosÃ© Carlos LÃ³pez Author-email: henestrosadev@gmail.com Requires-
 Python: >=3.8 Classifier: Environment :: Console Classifier: Intended Audience
 :: Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: MacOS Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: OS Independent Classifier: Operating System ::
 Other OS Classifier: Operating System :: POSIX :: Linux Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 Classifier: Topic :: Text
+Classifier: Programming Language :: Python :: 3.12 Classifier: Topic :: Text
 Processing :: General Classifier: Topic :: Utilities Requires-Dist: arabic-
-reshaper (>=3.0.0,<4.0.0) Requires-Dist: fpdf2 (>=2.6.1,<3.0.0) Requires-Dist:
-gspread (>=5.7.2,<6.0.0) Requires-Dist: lingua-language-detector
-(>=1.3.2,<2.0.0) Requires-Dist: openpyxl (>=3.1.0,<4.0.0) Requires-Dist:
-protobuf (>=4.21.12,<5.0.0) Requires-Dist: python-bidi (>=0.4.2,<0.5.0)
-Requires-Dist: pyyaml (>=6.0,<7.0) Project-URL: Repository, https://github.com/
-HenestrosaConH/mobile-strings-converter Description-Content-Type: text/markdown
+reshaper (>=3.0.0,<4.0.0) Requires-Dist: ezodf (>=0.3.2,<0.4.0) Requires-Dist:
+fpdf2 (>=2.7.8,<3.0.0) Requires-Dist: gspread (>=6.1.0,<7.0.0) Requires-Dist:
+lingua-language-detector (>=2.0.2,<3.0.0) Requires-Dist: openpyxl
+(>=3.1.2,<4.0.0) Requires-Dist: protobuf (>=5.26.1,<6.0.0) Requires-Dist:
+pypdf2 (>=3.0.1,<4.0.0) Requires-Dist: python-bidi (>=0.4.2,<0.5.0) Requires-
+Dist: pyyaml (>=6.0.1,<7.0.0) Project-URL: Repository, https://github.com/
+HenestrosaDev/mobile-strings-converter Description-Content-Type: text/markdown
 
                                     [Logo]
-                     ********** MMoobbiillee ssttrriinnggss ccoonnvveerrtteerr **********
+                    ************ MMoobbiillee SSttrriinnggss CCoonnvveerrtteerr ************
   A Python package that converts Android & iOS strings files to any supported
                                   file type.
 
                     _[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_ _s_u_p_p_o_r_t_]
                    _[_G_i_t_H_u_b_ _a_c_t_i_o_n_:_ _B_u_i_l_d_]_[_C_o_d_e_c_o_v_]_[_L_i_c_e_n_s_e_]
               _[_G_i_t_H_u_b_ _C_o_n_t_r_i_b_u_t_o_r_s_]_[_I_s_s_u_e_s_]_[_G_i_t_H_u_b_ _p_u_l_l_ _r_e_q_u_e_s_t_s_]
 
                  _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e Â· _A_s_k_ _Q_u_e_s_t_i_o_n
-## Table of Contents - [About the Project](#about-the-project) - [Project
-Structure](#project-structure) - [Built With](#built-with) - [Release Files]
-(#release-files) - [Usage](#usage) - [To Execute the Script](#to-execute-the-
-script) - [To Import the Package Into Your Project](#to-import-the-package-
-into-your-project) - [To Open the Code](#to-open-the-code) - [Notes](#notes) -
-[List of Indic Languages Supported by PDF files](#list-of-indic-languages-
-supported-by-pdf-files) - [List of Languages Not Supported by PDF files](#list-
-of-languages-not-supported-by-pdf-files) - [Roadmap](#roadmap) - [Contributing]
-(#contributing) - [License](#license) - [Authors](#authors) - [Acknowledgments]
-(#acknowledgments) - [Support](#support) ## About the Project I tried to do the
-whole process of converting a strings resource file into a spreadsheet in
-Google Sheets by hand and, even though you can do it with the option **Data >
-Split text to columns**, it involves wasting your time generating the
-spreadsheet manually. Due to that, I decided to build a time-efficient
-solution, which consists on running a Python script in order to achieve that
-with any file type. Moreover, not only this script can be executed on its own,
-it also can be installed as a package via **PyPI** (more information [here]
-(#to-import-the-package-into-your-project) about how to install it). The file
-types supported by the package are the following: - Android strings format
-(`*.xml`) - CSV - Google Sheets support - HTML - iOS strings format
-(`*.strings`) - JSON - MD - ODS - PDF - XLSX - YAML ### Project Structure ####
-Root directories: - `.github/workflows`: GitHub workflows. It also includes the
-templates for issues and pull requests, as well as the `depandabot.yml` file
-for Dependabot configuration. - `docs`: Contains files related to the
-documentation of the project. - `src/mobile_strings_converter`: Contains the
-source code files. - `tests`: Contains unit tests to ensure the correct
-functionality of the package. It also includes the `files` directory, which
-contains a few demo files in different formats to use in the unit tests. ####
-Root files: - `.gitignore`: File used by the version control system Git to
-specify files or directories that should be ignored by Git when tracking
-changes to a project. - `.pre-commit-config.yaml`: Configuration file used by
-**pre-commit**, a tool that runs checks (such as linting, testing, or
-formatting) on the code before you commit changes to version control. The file
-specifies which checks pre-commit should run and how it should run them. -
-`LICENSE`: Project license, which is [MIT](https://opensource.org/license/mit/
-). - `poetry.lock`: File generated by **Poetry**, a package manager for Python,
-that contains the exact versions of all packages used by a project. The file is
-used to ensure that all members of a development team are using the same
-versions of packages, even if different versions are available in the package
-repository. - `pyproject.toml`: Configuration file used by **Poetry**. It
-specifies the metadata for a Python project, including the project name,
-version, description, author, license and dependencies. - `README.md`: What you
-are reading right now. - `requirements.txt`: Lists the names and versions of
-each package used to build this project. To install the requirements, execute
-`pip install -r requirements.txt`. - `requirements-dev.txt`: Lists the names
-and versions of each package used in the development stage of this project. To
-install the requirements, execute `pip install -r requirements-dev.txt`. ###
-Built With - [openpyxl](https://pypi.org/project/openpyxl/): To generate ODS
-and XLSX files. - [gspread](https://pypi.org/project/gspread/): To generate
-spreadsheets in Google Sheets. - [protobuf](https://pypi.org/project/
-oauth2client/): Used by `google.oauth2.credentials` to authenticate to the
-user's Google account in order to create the spreadsheet in Google Sheets. -
-[PyYAML](https://pypi.org/project/PyYAML/): To generate YAML files. - [arabic-
-reshaper](https://pypi.org/project/arabic-reshaper/) and [python-bidi](https://
-pypi.org/project/python-bidi/): To add arabic characters support for PDF files.
-- [fpdf2](https://pypi.org/project/fpdf2/): To generate PDF files. - [lingua-
-language-detector](https://pypi.org/project/lingua-language-detector/): To
-recognize the **value** language when writing a PDF in order to know what font
-to use.
+## Table of Contents - [About the Project](#about-the-project) - [File Types
+Supported](#file-types-supported) - [Project Structure](#project-structure) -
+[Built With](#built-with) - [Release Files](#release-files) - [Getting Started]
+(#getting-started) - [Script Installation](#script-installation) - [Package
+Installation](#package-installation) - [Usage](#usage) - [Run the Program]
+(#run-the-program) - [Script Flags](#script-flags) - [Using the Package in Your
+Project](#using-the-package-in-your-project) - [Generate a Spreadsheet in
+Google Sheets](#generate-a-spreadsheet-in-google-sheets) - [Notes](#notes) -
+[Indic Languages Supported by PDF files](#indic-languages-supported-by-pdf-
+files) - [Languages Not Supported by PDF files](#languages-not-supported-by-
+pdf-files) - [Roadmap](#roadmap) - [Contributing](#contributing) - [License]
+(#license) - [Authors](#authors) - [Acknowledgments](#acknowledgments) -
+[Support](#support) ## About the Project I tried to do the whole process of
+converting a strings resource file into a spreadsheet in Google Sheets by hand
+and, even though you can do it with the option **Data > Split text to
+columns**, it involves wasting your time generating the spreadsheet manually.
+Due to that, I decided to build a time-efficient solution, which consists on
+running a Python script in order to achieve that with any file type. Moreover,
+not only this script can be executed on its own, it also can be installed as a
+package via **PyPI** (more information [here](#using-the-package-in-your-
+project) about how to install it). ### File Types Supported - Android strings
+format (`*.xml`) - CSV - Google Sheets support - HTML - iOS strings format
+(`*.strings`) - JSON - MD - ODS - PDF - XLSX - YAML ### Project Structure ASCII
+folder structure ``` â .gitignore â .pre-commit-config.yaml â LICENSE â
+poetry.lock â pyproject.toml â README.md â requirements.txt â
+requirements-dev.txt â ââââ.github â â CONTRIBUTING.md â â
+â ââââISSUE_TEMPLATE â â bug_report_template.md â â
+feature_request_template.md â â â ââââPULL_REQUEST_TEMPLATE â
+pull_request_template.md â ââââdocs â icon.png â ââââsrc
+â ââââmobile_strings_converter â â console_style.py â â
+converter.py â â __init__.py â â __main__.py â â â
+ââââassets â â ââââfonts â â Aakar.ttf â â
+AnekTelugu-VariableFont_wdth,wght.ttf â â DejaVuSansCondensed.ttf â â
+Eunjin.ttf â â fireflysung.ttf â â gargi.ttf â â
+Gurvetica_a8_Heavy.ttf â â Latha.ttf â â Waree.ttf â â â
+ââââcontroller â â main_controller.py â â __init__.py â â
+â ââââmodel â â transcription.py â â __init__.py â â â
+ââââutils â â constants.py â â i18n.py â â path_helper.py
+â â __init__.py â â â ââââview â main_window.py â
+__init__.py â ââââtests â base_tests.py â test_get_strings.py â
+test_to_android.py â test_to_csv.py â test_to_html.py â test_to_ios.py
+â test_to_json.py â test_to_md.py â test_to_ods.py â test_to_pdf.py â
+test_to_xlsx.py â test_to_yaml.py â ââââfiles ââââinput â
+Localizable.strings â strings.xml â ââââtemplate-with-comments â
+Localizable.strings â strings.csv â strings.html â strings.json â
+strings.md â strings.ods â strings.pdf â strings.xlsx â strings.xml â
+strings.yaml â ââââtemplate-without-comments Localizable.strings
+strings.csv strings.html strings.json strings.md strings.ods strings.pdf
+strings.xlsx strings.xml strings.yaml ``` ### Built With - [openpyxl](https://
+pypi.org/project/openpyxl/) to generate ODS and XLSX files. - [gspread](https:/
+/pypi.org/project/gspread/) to generate spreadsheets in Google Sheets. -
+[protobuf](https://pypi.org/project/oauth2client/) is used by
+`google.oauth2.credentials` to authenticate to the user's Google account in
+order to create the spreadsheet in Google Sheets. - [PyYAML](https://pypi.org/
+project/PyYAML/) to generate YAML files. - [arabic-reshaper](https://pypi.org/
+project/arabic-reshaper/) and [python-bidi](https://pypi.org/project/python-
+bidi/) to add arabic characters support for PDF files. - [fpdf2](https://
+pypi.org/project/fpdf2/) to generate PDF files. - [lingua-language-detector]
+(https://pypi.org/project/lingua-language-detector/) to recognize the **value**
+language when writing a PDF in order to know what font to use.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Release Files | File | Description | Size | |:------------------------------
 -------------------------------------------------------------------------------
-------------------------------------------------|:-----------------------------
+-----------------------------------|:------------------------------------------
+----------------------------------------------------------|:--------| |
+[mobile-strings-converter.zip](https://github.com/HenestrosaDev/mobile-strings-
+converter/releases/latest/download/mobile-strings-converter.zip) | PDF file
+support for almost all languages ([see exceptions](#languages-not-supported-by-
+pdf-files)) | 8.43 MB |
+                                                                  (_b_a_c_k_ _t_o_ _t_o_p)
+## Getting Started ### Script Installation 1. Download the [release](#release-
+files) that is best suited to your needs. 2. (Optional but recommended) Create
+a Python virtual environment in the project root. If you're using `virtualenv`,
+you would run `virtualenv venv`. 3. (Optional but recommended) Activate the
+virtual environment: ```bash # on Windows . venv/Scripts/activate # if you get
+the error `FullyQualifiedErrorId : UnauthorizedAccess`, run this: Set-
+ExecutionPolicy Unrestricted -Scope Process # and then . venv/Scripts/activate
+# on macOS and Linux source venv/Scripts/activate ``` 4. Open the command line
+and run `pip install -r path/to/requirements.txt` to install the required
+packages to run the script. ### Package Installation Install the PyPI package
+by running `pip install mobile-strings-converter`.
+                                                                  (_b_a_c_k_ _t_o_ _t_o_p)
+## Usage ### Run the Program For a basic usage, you can run the following
+command: ``` python path/to/mobile_strings_converter.py *.[SUPPORTED_FILE_TYPE]
+-o *.[SUPPORTED_FILE_TYPE] ``` See [Generate a Spreadsheet in Google Sheets]
+(#generate-a-spreadsheet-in-google-sheets) to create a spreadsheet. #### Script
+Flags | Flag | Description | |:----------------------------|:------------------
 -------------------------------------------------------------------------------
-|:----------| | [mobile-strings-converter.zip](https://github.com/
-HenestrosaConH/mobile-strings-converter/releases/latest/download/mobile-
-strings-converter.zip) | Standard language support for PDF files (over 100
-languages, including RTL) | 0.32 MB | | [mobile-strings-converter-indic.zip]
-(https://github.com/HenestrosaConH/mobile-strings-converter/releases/latest/
-download/mobile-strings-converter-indic.zip) | PDF file support for Indic
-languages ([see list](#list-of-indic-languages-supported-by-pdf-files)) | 1.40
-MB | | [mobile-strings-converter-zh-ja.zip](https://github.com/HenestrosaConH/
-mobile-strings-converter/releases/latest/download/mobile-strings-converter-zh-
-ja.zip) | PDF file support for Japanese and Chinese (simplified and
-traditional) | 7.17 MB | | [mobile-strings-converter-ko.zip](https://
-github.com/HenestrosaConH/mobile-strings-converter/releases/latest/download/
-mobile-strings-converter-ko.zip) | PDF file support for Korean | 0.46 MB | |
-[mobile-strings-converter-th.zip](https://github.com/HenestrosaConH/mobile-
-strings-converter/releases/latest/download/mobile-strings-converter-th.zip) |
-PDF file support for Thai | 0.37 MB | | [mobile-strings-converter-all.zip]
-(https://github.com/HenestrosaConH/mobile-strings-converter/releases/latest/
-download/mobile-strings-converter-all.zip) | PDF file support for almost all
-languages ([see exceptions](#list-of-languages-not-supported-by-pdf-files)) |
-8.43 MB |
-                                                                  (_b_a_c_k_ _t_o_ _t_o_p)
-## Usage ### To Execute The Script 1. Download the [release](#release-files)
-that is best suited to your needs. 2. Open the command line and run `pip
-install -r path/to/requirements.txt` to install the required packages to
-execute the script. 3. Example of a basic command to convert a `.xml` or
-`.strings` file to another file type: ``` path/to/python path/to/
-mobile_strings_converter.py path/to/<*.xml | *.strings> -o path/to/*. ``` ####
-To Generate a Spreadsheet in Google Sheets Before going further into running
-the commands to do so, please note that you will have to generate a
+-------------------------------------------------------------------| | `-h` or
+`--help` | Displays help text for the program | | `-o` or `--output-filepath` |
+Specifies the filepath for storing the converted file. The file extension can
+be chosen from the list of supported file types mentioned [here](#about-the-
+project). | | `-g` or `--google-sheets` | Followed by the name of the sheet,
+creates a new Google Sheets spreadsheet with the specified name. | | `-c` or `-
+-credentials` | Followed by the path to your `service_account.json` file is
+mandatory if you want to generate a spreadsheet in your Google account. | | `-
+p` or `--print-comments` | The output file will include any commented strings
+present in the original file. |
+                                                                  (_b_a_c_k_ _t_o_ _t_o_p)
+### Using the Package in Your Project Once you have followed the steps of the
+[Getting Started](#getting-started) section, import the package and the wrapper
+function(s) you want to use: ```python # Using the `get_strings` function from
+mobile_strings_converter import get_strings get_strings( input_filepath=Path
+("strings.xml"), should_print_comments=True ) ``` ### Generate a Spreadsheet in
+Google Sheets #### Set Up Google Account Before going further into running the
+commands to do so, please note that you will have to generate a
 `service_account.json` file. You can do the following to get one: 1. Go to the
 [Google Cloud Console](https://console.cloud.google.com/). 2. Create a new
 project or select an existing project. 3. Go to the **APIs & Services** page,
 click on **Dashboard** and then click on **Enable APIs and Services**. 4.
 Search for **Google Sheets API** and enable it. 5. Go to the **Credentials**
 page, click on **Create credentials**, and then choose **Service account**. 6.
 Give your service account a name and select a role. For this purpose, you can
 select **Project -> Editor**. 7. Click on the **Create key** button, select the
 JSON format and download the `service_account.json` file. 8. Share your Google
 Sheets file with the email address that is specified in the **client_email**
-field in the `service_account.json` file. Alternatively, you can create an XLSX
-file and open it in Google Sheets if you do not want to go through the hassle
-of generating the `service_account.json` file. Once you have generated the
-`service_account.json` file, you can generate a spreadsheet in Google Sheets by
-running the following command: ``` path/to/python path/to/
-mobile_strings_converter.py path/to/
- Localizable.strings> -gs -c path/to/service_account.json ``` If you want to
-generate an output file along with the spreadsheet, run this: ``` path/to/
-python path/to/mobile_strings_converter.py path/to/
- Localizable.strings> -gs -c path/to/service_account.json -o path/to/strings.
-``` #### Script flags - `-h`, `--help`: Show help - `-o`, `--output-filepath`:
-Output filepath where you want to store the converted file. Its extension can
-be any of the file types listed [here](#about-the-project). - `-g`, `--google-
-sheets` : Creates a spreadsheet in Google Sheets with the name passed as
-argument. - `-c`, `--credentials` <`service_account.json` filepath>: Mandatory
-if you want to generate a spreadsheet in your Google account. - `-p`, `--print-
-comments`: If present, indicates that commented strings will be printed in the
-output file. ### To Import the Package Into Your Project 1. Run `pip install
-mobile-strings-converter` 2. Import the package and the wrapper function with
-this line of code: `from mobile_strings_converter import convert_strings`. ###
-To Open the Code 1. Clone the project with the `git clone https://github.com/
-HenestrosaConH/mobile-strings-converter.git` command. 2. Open it in your
-favourite IDE (mine is [PyCharm](https://www.jetbrains.com/pycharm/))
-                                                                  (_b_a_c_k_ _t_o_ _t_o_p)
-## Notes ### List of Indic Languages Supported by PDF files - Hindi - Marathu -
-Oriya - Tibetan - Gujarati - Telugu - Tamil - Punjabi ### List of Languages Not
-Supported by PDF files - **Bengali** (not possible to print correctly using
-[fpdf2](https://pypi.org/project/fpdf2/)) - **Dhivehi** (not recognized by
+field in the `service_account.json` file. Alternatively, you can create a
+`.xlsx` file and open it in Google Sheets if you do not want to go through the
+hassle of generating the `service_account.json` file. Once you have generated
+the `service_account.json` file, you can generate a spreadsheet in Google
+Sheets by running the following command: ``` python path/to/
+mobile_strings_converter.py <*.xml | *.strings> -g -c path/to/
+service_account.json ``` If you want to generate an output file along with the
+spreadsheet, run this: ``` python path/to/mobile_strings_converter.py *.
+[SUPPORTED_FILE_TYPE -g -c path/to/service_account.json -o *.
+[SUPPORTED_FILE_TYPE] ``` #### Using the `to_google_sheets` Function in Your
+Project ```python from mobile_strings_converter import to_google_sheets
+to_google_sheets( input_filepath=Path("path/to/strings-file"),
+sheet_name="MyProject strings", credentials_filepath=Path("path/to/
+service_account.json"), should_print_comments=True, ) ``` ## Notes ### Indic
+Languages Supported by PDF files - Hindi - Marathu - Oriya - Tibetan - Gujarati
+- Telugu - Tamil - Punjabi ### Languages Not Supported by PDF files - Bengali
+(not possible to print correctly using [fpdf2](https://pypi.org/project/fpdf2/
+)) - Dhivehi (not recognized by [lingua-language-detector](https://pypi.org/
+project/lingua-language-detector/)) - Kannada (not recognized by [lingua-
+language-detector](https://pypi.org/project/lingua-language-detector/)) - Khmer
+(not recognized by [lingua-language-detector](https://pypi.org/project/lingua-
+language-detector/)) - Lao (not recognized by [lingua-language-detector](https:
+//pypi.org/project/lingua-language-detector/)) - Malayalam (not recognized by
 [lingua-language-detector](https://pypi.org/project/lingua-language-detector/))
-- **Kannada** (not recognized by [lingua-language-detector](https://pypi.org/
-project/lingua-language-detector/)) - **Khmer** (not recognized by [lingua-
-language-detector](https://pypi.org/project/lingua-language-detector/)) -
-**Lao** (not recognized by [lingua-language-detector](https://pypi.org/project/
-lingua-language-detector/)) - **Malayalam** (not recognized by [lingua-
-language-detector](https://pypi.org/project/lingua-language-detector/)) -
-**Meiteilon (manipuri)** (not recognized by [lingua-language-detector](https://
-pypi.org/project/lingua-language-detector/)) - **Myanmar burmese** (not
-possible to print correctly using [fpdf2](https://pypi.org/project/fpdf2/)) -
-**Odia (Oriya)** (not recognized by [lingua-language-detector](https://
-pypi.org/project/lingua-language-detector/)) - **Sinhala** (not recognized by
-[lingua-language-detector](https://pypi.org/project/lingua-language-detector/))
-- **Tigrinya** (not recognized by [lingua-language-detector](https://pypi.org/
-project/lingua-language-detector/))
-                                                                  (_b_a_c_k_ _t_o_ _t_o_p)
-## Roadmap - [ ] Add support for multiple `.xml`/`.strings` files input. - [ ]
-Add support for converting a file (not `.xml` nor `.strings`) to a strings
-resource file. - [ ] Make a web version. You can propose a new feature creating
-an [issue](https://github.com/HenestrosaConH/mobile-strings-converter/new/
-choose).
-                                                                  (_b_a_c_k_ _t_o_ _t_o_p)
-## Contributing Contributions are what make the open source community such an
-amazing place to learn, inspire, and create. Any contributions you make are
-**greatly appreciated**. Please, read the [CONTRIBUTING.md](https://github.com/
-HenestrosaConH/mobile-strings-converter/blob/main/.github/CONTRIBUTING.md)
-file, where you can find more detailed information about how to contribute to
-the project.
-                                                                  (_b_a_c_k_ _t_o_ _t_o_p)
-## License Distributed under the MIT License. See `LICENSE` for more
-information.
-                                                                  (_b_a_c_k_ _t_o_ _t_o_p)
-## Authors - HenestrosaConH
+- Meiteilon (manipuri) (not recognized by [lingua-language-detector](https://
+pypi.org/project/lingua-language-detector/)) - Myanmar burmese (not possible to
+print correctly using [fpdf2](https://pypi.org/project/fpdf2/)) - Odia (Oriya)
+(not recognized by [lingua-language-detector](https://pypi.org/project/lingua-
+language-detector/))
+ - Sinhala (not recognized by [lingua-language-detector](https://pypi.org/
+project/lingua-language-detector/)) - Tigrinya (not recognized by [lingua-
+language-detector](https://pypi.org/project/lingua-language-detector/))
+                                                                  (_b_a_c_k_ _t_o_ _t_o_p)
+## Roadmap - [x] Add support for converting a file (not `.xml` or `.strings`)
+into a strings resource file (`.xml` or `.strings`). - [ ] Add support for
+multiple `.xml`/`.strings` files input. - [ ] Make a web version. You can
+propose a new feature creating an [issue](https://github.com/HenestrosaDev/
+mobile-strings-converter/new/choose). ## Contributing Contributions are what
+make the open source community such an amazing place to learn, inspire, and
+create. Any contributions you make are **greatly appreciated**. Please, read
+the [CONTRIBUTING.md](https://github.com/HenestrosaDev/mobile-strings-
+converter/blob/main/.github/CONTRIBUTING.md) file, where you can find more
+detailed information about how to contribute to the project. ## License
+Distributed under the MIT License. See `LICENSE` for more information. ##
+Authors - HenestrosaDev
 gmail.com> (JosÃ© Carlos LÃ³pez Henestrosa) See also the list of [contributors]
-(https://github.com/HenestrosaConH/mobile-strings-converter/contributors) who
-participated in this project.
-                                                                  (_b_a_c_k_ _t_o_ _t_o_p)
-## Acknowledgments I have made use of the following resources to make this
-project: - [Best-README-Template](https://github.com/othneildrew/Best-README-
-Template/) - [Img Shields](https://shields.io) - [How to create a Python
-package](https://mathspp.com/blog/how-to-create-a-python-package-in-2022#how-
-to-create-a-python-package) - [Icon created by Midjourney](https://
-www.midjourney.com/app/)
-                                                                  (_b_a_c_k_ _t_o_ _t_o_p)
-## Support [![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-
-fi.com/U7U5J6COZ)
+(https://github.com/HenestrosaDev/mobile-strings-converter/contributors) who
+participated in this project. ## Acknowledgments I have made use of the
+following resources to make this project: - [How to create a Python package]
+(https://mathspp.com/blog/how-to-create-a-python-package-in-2022#how-to-create-
+a-python-package) ## Support Would you like to support the project? That's very
+kind of you! You can go to my Ko-Fi profile by clicking on the button down
+below. [![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/
+henestrosadev)
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
```

