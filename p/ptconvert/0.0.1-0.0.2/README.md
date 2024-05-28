# Comparing `tmp/ptconvert-0.0.1.tar.gz` & `tmp/ptconvert-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptconvert-0.0.1.tar", last modified: Thu May  9 12:27:02 2024, max compression
+gzip compressed data, was "ptconvert-0.0.2.tar", last modified: Tue May 28 10:11:03 2024, max compression
```

## Comparing `ptconvert-0.0.1.tar` & `ptconvert-0.0.2.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 12:27:02.002390 ptconvert-0.0.1/
--rwxr-xr-x   0 kali      (1000) kali      (1000)    35823 2024-04-29 08:26:36.000000 ptconvert-0.0.1/LICENSE
--rwxr-xr-x   0 kali      (1000) kali      (1000)       38 2024-04-29 08:26:36.000000 ptconvert-0.0.1/MANIFEST.in
--rw-r--r--   0 kali      (1000) kali      (1000)     2726 2024-05-09 12:27:02.002390 ptconvert-0.0.1/PKG-INFO
--rwxr-xr-x   0 kali      (1000) kali      (1000)     2265 2024-04-29 08:26:36.000000 ptconvert-0.0.1/README.md
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 12:27:02.002390 ptconvert-0.0.1/ptconvert/
--rwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-29 08:26:36.000000 ptconvert-0.0.1/ptconvert/__init__.py
--rwxr-xr-x   0 kali      (1000) kali      (1000)       21 2024-04-29 08:26:36.000000 ptconvert-0.0.1/ptconvert/_version.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 12:27:02.002390 ptconvert-0.0.1/ptconvert/modules/
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 12:27:02.002390 ptconvert-0.0.1/ptconvert/modules/__pycache__/
--rw-r--r--   0 kali      (1000) kali      (1000)     2322 2024-05-02 07:42:18.000000 ptconvert-0.0.1/ptconvert/modules/__pycache__/_baseclass.cpython-311.pyc
--rw-r--r--   0 kali      (1000) kali      (1000)     7781 2024-05-06 12:18:52.000000 ptconvert-0.0.1/ptconvert/modules/__pycache__/burp_report.cpython-311.pyc
--rw-r--r--   0 kali      (1000) kali      (1000)     5819 2024-05-02 11:23:24.000000 ptconvert-0.0.1/ptconvert/modules/__pycache__/csv.cpython-311.pyc
--rwxr-xr-x   0 kali      (1000) kali      (1000)      920 2024-05-02 07:42:16.000000 ptconvert-0.0.1/ptconvert/modules/_baseclass.py
--rw-r--r--   0 kali      (1000) kali      (1000)     6689 2024-05-06 12:17:14.000000 ptconvert-0.0.1/ptconvert/modules/burp_report.py
--rwxr-xr-x   0 kali      (1000) kali      (1000)     1739 2024-05-09 09:49:27.000000 ptconvert-0.0.1/ptconvert/modules/swagger.py
--rwxr-xr-x   0 kali      (1000) kali      (1000)     5288 2024-05-06 11:24:26.000000 ptconvert-0.0.1/ptconvert/ptconvert.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 12:27:02.002390 ptconvert-0.0.1/ptconvert.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     2726 2024-05-09 12:27:01.000000 ptconvert-0.0.1/ptconvert.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      564 2024-05-09 12:27:01.000000 ptconvert-0.0.1/ptconvert.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2024-05-09 12:27:01.000000 ptconvert-0.0.1/ptconvert.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       55 2024-05-09 12:27:01.000000 ptconvert-0.0.1/ptconvert.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       17 2024-05-09 12:27:01.000000 ptconvert-0.0.1/ptconvert.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       10 2024-05-09 12:27:01.000000 ptconvert-0.0.1/ptconvert.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2024-05-09 12:27:02.002390 ptconvert-0.0.1/setup.cfg
--rwxr-xr-x   0 kali      (1000) kali      (1000)      964 2024-05-09 12:25:07.000000 ptconvert-0.0.1/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-28 10:11:03.852159 ptconvert-0.0.2/
+-rw-r--r--   0 kali      (1000) kali      (1000)    35823 2024-04-29 08:26:36.000000 ptconvert-0.0.2/LICENSE
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2024-04-29 08:26:36.000000 ptconvert-0.0.2/MANIFEST.in
+-rw-r--r--   0 kali      (1000) kali      (1000)     3239 2024-05-28 10:11:03.852159 ptconvert-0.0.2/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)     2519 2024-05-28 10:08:17.000000 ptconvert-0.0.2/README.md
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-28 10:11:03.852159 ptconvert-0.0.2/ptconvert/
+-rw-r--r--   0 kali      (1000) kali      (1000)        0 2024-04-29 08:26:36.000000 ptconvert-0.0.2/ptconvert/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       21 2024-05-28 10:02:00.000000 ptconvert-0.0.2/ptconvert/_version.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-28 10:11:03.852159 ptconvert-0.0.2/ptconvert/modules/
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-28 10:11:03.852159 ptconvert-0.0.2/ptconvert/modules/__pycache__/
+-rw-r--r--   0 kali      (1000) kali      (1000)     2322 2024-05-02 07:42:18.000000 ptconvert-0.0.2/ptconvert/modules/__pycache__/_baseclass.cpython-311.pyc
+-rw-r--r--   0 kali      (1000) kali      (1000)     7789 2024-05-28 07:42:00.000000 ptconvert-0.0.2/ptconvert/modules/__pycache__/burp_report.cpython-311.pyc
+-rw-r--r--   0 kali      (1000) kali      (1000)     5819 2024-05-02 11:23:24.000000 ptconvert-0.0.2/ptconvert/modules/__pycache__/csv.cpython-311.pyc
+-rw-r--r--   0 kali      (1000) kali      (1000)     3059 2024-05-28 07:42:04.000000 ptconvert-0.0.2/ptconvert/modules/__pycache__/swagger.cpython-311.pyc
+-rw-r--r--   0 kali      (1000) kali      (1000)      920 2024-05-02 07:42:16.000000 ptconvert-0.0.2/ptconvert/modules/_baseclass.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     5624 2024-05-09 11:23:44.000000 ptconvert-0.0.2/ptconvert/modules/burp_report.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1064 2024-05-09 11:23:51.000000 ptconvert-0.0.2/ptconvert/modules/burp_report.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)     1739 2024-05-09 09:49:27.000000 ptconvert-0.0.2/ptconvert/modules/swagger.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     5444 2024-05-28 10:01:47.000000 ptconvert-0.0.2/ptconvert/ptconvert.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-28 10:11:03.852159 ptconvert-0.0.2/ptconvert.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     3239 2024-05-28 10:11:03.000000 ptconvert-0.0.2/ptconvert.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      652 2024-05-28 10:11:03.000000 ptconvert-0.0.2/ptconvert.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2024-05-28 10:11:03.000000 ptconvert-0.0.2/ptconvert.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       55 2024-05-28 10:11:03.000000 ptconvert-0.0.2/ptconvert.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       17 2024-05-28 10:11:03.000000 ptconvert-0.0.2/ptconvert.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       10 2024-05-28 10:11:03.000000 ptconvert-0.0.2/ptconvert.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2024-05-28 10:11:03.852159 ptconvert-0.0.2/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)     1267 2024-05-28 10:07:55.000000 ptconvert-0.0.2/setup.py
```

### Comparing `ptconvert-0.0.1/LICENSE` & `ptconvert-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ptconvert-0.0.1/PKG-INFO` & `ptconvert-0.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 Metadata-Version: 2.1
 Name: ptconvert
-Version: 0.0.1
+Version: 0.0.2
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
 License: GPLv3
+Project-URL: homepage, https://www.penterep.com/
+Project-URL: repository, https://github.com/penterep/ptconvert
+Project-URL: tracker, https://github.com/penterep/ptconvert/issues
+Project-URL: changelog, https://github.com/penterep/ptconvert/blob/main/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Environment :: Console
 Classifier: Topic :: Security
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ptlibs<2,>=1.0.7
 
 [![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)](https://www.penterep.com/)
 
 
-## PTCONVERT - Penterep Data Format Converter
+## PTCONVERT - Penterep Data Format Convertor
 
 ptconvert is a tool that transforms various data formats into Penterep-compatible JSON.
 
 ## Installation
 
 ```
 pip install ptconvert
@@ -46,21 +50,26 @@
 ## Usage examples
 ```
 ptconvert -f swagger -i swagger_file.json -o penterep.json
 ```
 
 ## Options
 ```
-   -i  --input    <file>    Set input file
-   -o  --output   <output>  Set output file
-   -f  --format   <format>  Set input file format to:
-                   swagger      Swagger format
+-i  --input      <file>         Set input file
+-o  --output     <output>       Set output file
+-f  --format     <format>       Set input file format to:
+                  burp-report    BurpReport format
+                  swagger        Swagger format
+
+      --csv        <path-to-csv>  Set path to CSV file
+      --use-texts                 Use texts from Burp Report
+      --parse-url                 Parse URLs in Burp Report
 
-   -v  --version            Show script version and exit
-   -h  --help               Show this help message and exit
+-v  --version                   Show script version and exit
+-h  --help                      Show this help message and exit
 ```
 
 ## Dependencies
 ```
 ptlibs
 ```
```

### Comparing `ptconvert-0.0.1/README.md` & `ptconvert-0.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)](https://www.penterep.com/)
 
 
-## PTCONVERT - Penterep Data Format Converter
+## PTCONVERT - Penterep Data Format Convertor
 
 ptconvert is a tool that transforms various data formats into Penterep-compatible JSON.
 
 ## Installation
 
 ```
 pip install ptconvert
@@ -29,21 +29,26 @@
 ## Usage examples
 ```
 ptconvert -f swagger -i swagger_file.json -o penterep.json
 ```
 
 ## Options
 ```
-   -i  --input    <file>    Set input file
-   -o  --output   <output>  Set output file
-   -f  --format   <format>  Set input file format to:
-                   swagger      Swagger format
+-i  --input      <file>         Set input file
+-o  --output     <output>       Set output file
+-f  --format     <format>       Set input file format to:
+                  burp-report    BurpReport format
+                  swagger        Swagger format
+
+      --csv        <path-to-csv>  Set path to CSV file
+      --use-texts                 Use texts from Burp Report
+      --parse-url                 Parse URLs in Burp Report
 
-   -v  --version            Show script version and exit
-   -h  --help               Show this help message and exit
+-v  --version                   Show script version and exit
+-h  --help                      Show this help message and exit
 ```
 
 ## Dependencies
 ```
 ptlibs
 ```
```

### Comparing `ptconvert-0.0.1/ptconvert/modules/__pycache__/_baseclass.cpython-311.pyc` & `ptconvert-0.0.2/ptconvert/modules/__pycache__/_baseclass.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ptconvert-0.0.1/ptconvert/modules/__pycache__/burp_report.cpython-311.pyc` & `ptconvert-0.0.2/ptconvert/modules/__pycache__/burp_report.cpython-311.pyc`

 * *Files 6% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x4aca3866 (Mon May  6 12:17:14 2024 UTC)
-files sz: 6689
+moddate:  0x40b23c66 (Thu May  9 11:23:44 2024 UTC)
+files sz: 5624
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c006d015a010100640264036c025a02640264036c035a
@@ -45,15 +45,15 @@
                 54 IMPORT_NAME              7 (ptlibs.ptpathtypedetector)
                 56 IMPORT_FROM              8 (PtPathTypeDetector)
                 58 STORE_NAME               8 (PtPathTypeDetector)
                 60 POP_TOP
    
      8          62 PUSH_NULL
                 64 LOAD_BUILD_CLASS
-                66 LOAD_CONST               6 (<code object BurpReportParser, file "/home/kali/penterep/dkummel/ptconvert/ptconvert/modules/burp_report.py", line 8>)
+                66 LOAD_CONST               6 (<code object BurpReportParser, file "/home/kali/penterep/penterep-public/ptconvert/ptconvert/modules/burp_report.py", line 8>)
                 68 MAKE_FUNCTION            0
                 70 LOAD_CONST               7 ('BurpReportParser')
                 72 LOAD_NAME                1 (BaseClass)
                 74 PRECALL                  3
                 78 CALL                     3
                 88 STORE_NAME               9 (BurpReportParser)
                 90 LOAD_CONST               3 (None)
@@ -79,35 +79,35 @@
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('BurpReportParser')
                        8 STORE_NAME               2 (__qualname__)
          
            9          10 LOAD_CONST               1 ('ptjsonlib')
                       12 LOAD_NAME                3 (object)
                       14 BUILD_TUPLE              2
-                      16 LOAD_CONST               2 (<code object __init__, file "/home/kali/penterep/dkummel/ptconvert/ptconvert/modules/burp_report.py", line 9>)
+                      16 LOAD_CONST               2 (<code object __init__, file "/home/kali/penterep/penterep-public/ptconvert/ptconvert/modules/burp_report.py", line 9>)
                       18 MAKE_FUNCTION            4 (annotations)
                       20 STORE_NAME               4 (__init__)
          
           12          22 LOAD_CONST               3 ('return')
                       24 LOAD_NAME                5 (list)
                       26 BUILD_TUPLE              2
-                      28 LOAD_CONST               4 (<code object convert, file "/home/kali/penterep/dkummel/ptconvert/ptconvert/modules/burp_report.py", line 12>)
+                      28 LOAD_CONST               4 (<code object convert, file "/home/kali/penterep/penterep-public/ptconvert/ptconvert/modules/burp_report.py", line 12>)
                       30 MAKE_FUNCTION            4 (annotations)
                       32 STORE_NAME               6 (convert)
          
-         129          34 LOAD_CONST               5 (<code object get_text_safely, file "/home/kali/penterep/dkummel/ptconvert/ptconvert/modules/burp_report.py", line 129>)
+         106          34 LOAD_CONST               5 (<code object get_text_safely, file "/home/kali/penterep/penterep-public/ptconvert/ptconvert/modules/burp_report.py", line 106>)
                       36 MAKE_FUNCTION            0
                       38 STORE_NAME               7 (get_text_safely)
          
-         132          40 LOAD_CONST               6 ('vulnerability_classification')
+         109          40 LOAD_CONST               6 ('vulnerability_classification')
                       42 LOAD_NAME                8 (str)
                       44 LOAD_CONST               3 ('return')
                       46 LOAD_NAME                8 (str)
                       48 BUILD_TUPLE              4
-                      50 LOAD_CONST               7 (<code object get_cwe_from_vulnerability_classifications, file "/home/kali/penterep/dkummel/ptconvert/ptconvert/modules/burp_report.py", line 132>)
+                      50 LOAD_CONST               7 (<code object get_cwe_from_vulnerability_classifications, file "/home/kali/penterep/penterep-public/ptconvert/ptconvert/modules/burp_report.py", line 109>)
                       52 MAKE_FUNCTION            4 (annotations)
                       54 STORE_NAME               9 (get_cwe_from_vulnerability_classifications)
                       56 LOAD_CONST               8 (None)
                       58 RETURN_VALUE
          consts
             'BurpReportParser'
             'ptjsonlib'
@@ -126,15 +126,15 @@
                             18 RETURN_VALUE
                consts
                   None
                names      ('ptjsonlib',)
                varnames   ('self', 'ptjsonlib')
                freevars   ()
                cellvars   ()
-               filename   '/home/kali/penterep/dkummel/ptconvert/ptconvert/modules/burp_report.py'
+               filename   '/home/kali/penterep/penterep-public/ptconvert/ptconvert/modules/burp_report.py'
                name       '__init__'
                firstlineno 9
                lnotab 0x0201
             'return'
             code
                argcount  : 2
                nlocals   : 37
@@ -148,15 +148,15 @@
                   00000000007d027c02a00500000000000000000000000000000000000000
                   00a6000000ab0000000000000000007d036e132300740c00000000000000
                   000000240072067d04820064007d047e047701770078035900770167007d
                   05740f000000000000000000007c016a0000000000000000006403a60200
                   00ab02000000000000000035007d067401000000000000000000006a0800
                   000000000000007c06a6010000ab0100000000000000007d077c03a00900
                   000000000000000000000000000000000000006404a6010000ab01000000
-                  0000000000440090045dba7d088900a00a00000000000000000000000000
+                  0000000000440090045dbb7d088900a00a00000000000000000000000000
                   000000000000007c08a00b00000000000000000000000000000000000000
                   006405a6010000ab010000000000000000a6010000ab0100000000000000
                   007d098900a00a00000000000000000000000000000000000000007c08a0
                   0b00000000000000000000000000000000000000006406a6010000ab0100
                   00000000000000a6010000ab0100000000000000007d0a8900a00a000000
                   00000000000000000000000000000000007c08a00b000000000000000000
                   00000000000000000000006407a6010000ab010000000000000000a60100
@@ -216,29 +216,29 @@
                   0078017d1f78017d207d1e64207c1e69017d217c016a0c00000000000000
                   0072537c21a01300000000000000000000000000000000000000007c0c7c
                   0b7c0f7429000000000000000000006a1500000000000000007c10a60100
                   00ab0100000000000000007429000000000000000000006a150000000000
                   0000007c11a6010000ab0100000000000000007429000000000000000000
                   006a1500000000000000007c12a6010000ab0100000000000000007c1a64
                   219c07a6010000ab01000000000000000001007c016a1600000000000000
-                  00726689006a010000000000000000a01700000000000000000000000000
+                  00726789006a010000000000000000a01700000000000000000000000000
                   000000000000007c0a7c0b7a000000a6010000ab0100000000000000007d
                   227c2272467c1f7c22641b1900000000000000000064223c0000007c2264
                   2319000000000000000000642419000000000000000000a0180000000000
                   0000000000000000000000000000007c21a6010000ab0100000000000000
                   0001007c2244005d177d237c05a018000000000000000000000000000000
-                  00000000007c23a6010000ab01000000000000000001008c186e5a89006a
-                  010000000000000000a01900000000000000000000000000000000000000
-                  0064257c1f7c0a7c0b7a0000007c0b743500000000000000000000a60000
-                  00ab000000000000000000a01b0000000000000000000000000000000000
-                  0000007c0ba6010000ab01000000000000000064269c037c216701ac27a6
-                  040000ab0400000000000000007d247c05a0180000000000000000000000
-                  0000000000000000007c24a6010000ab010000000000000000010090048c
-                  bc0900640064006400a6020000ab02000000000000000001006e0b230031
-                  007304770278035900770101005900010001007c055300
+                  00000000007c23a6010000ab01000000000000000001008c1890048c6189
+                  006a010000000000000000a0190000000000000000000000000000000000
+                  00000064257c1f7c0a7c0b7a0000007c0b743500000000000000000000a6
+                  000000ab000000000000000000a01b000000000000000000000000000000
+                  00000000007c0ba6010000ab01000000000000000064269c037c216701ac
+                  27a6040000ab0400000000000000007d247c05a018000000000000000000
+                  00000000000000000000007c24a6010000ab010000000000000000010090
+                  048cbd0900640064006400a6020000ab02000000000000000001006e0b23
+                  0031007304770278035900770101005900010001007c055300
                              0 MAKE_CELL                0 (self)
                
                 12           2 RESUME                   0
                
                 13           4 LOAD_FAST                1 (args)
                              6 LOAD_ATTR                0 (csv)
                             16 POP_JUMP_FORWARD_IF_TRUE    27 (to 72)
@@ -308,15 +308,15 @@
                 26         294 LOAD_FAST                3 (root_element)
                            296 LOAD_METHOD              9 (findall)
                            318 LOAD_CONST               4 ('issue')
                            320 PRECALL                  1
                            324 CALL                     1
                            334 GET_ITER
                        >>  336 EXTENDED_ARG             4
-                           338 FOR_ITER              1210 (to 2760)
+                           338 FOR_ITER              1211 (to 2762)
                            340 STORE_FAST               8 (issue)
                
                 27         342 LOAD_DEREF               0 (self)
                            344 LOAD_METHOD             10 (get_text_safely)
                            366 LOAD_FAST                8 (issue)
                            368 LOAD_METHOD             11 (find)
                            390 LOAD_CONST               5 ('type')
@@ -445,15 +445,15 @@
                           1210 LOAD_METHOD             11 (find)
                           1232 LOAD_CONST              16 ('issueDetailItems')
                           1234 PRECALL                  1
                           1238 CALL                     1
                           1248 POP_JUMP_FORWARD_IF_NONE    52 (to 1354)
                           1250 LOAD_CLOSURE             0 (self)
                           1252 BUILD_TUPLE              1
-                          1254 LOAD_CONST              17 (<code object <listcomp>, file "/home/kali/penterep/dkummel/ptconvert/ptconvert/modules/burp_report.py", line 41>)
+                          1254 LOAD_CONST              17 (<code object <listcomp>, file "/home/kali/penterep/penterep-public/ptconvert/ptconvert/modules/burp_report.py", line 41>)
                           1256 MAKE_FUNCTION            8 (closure)
                           1258 LOAD_FAST                8 (issue)
                           1260 LOAD_METHOD             11 (find)
                           1282 LOAD_CONST              16 ('issueDetailItems')
                           1284 PRECALL                  1
                           1288 CALL                     1
                           1298 LOAD_METHOD              9 (findall)
@@ -671,15 +671,15 @@
                
                 73        2342 PRECALL                  1
                           2346 CALL                     1
                           2356 POP_TOP
                
                 84     >> 2358 LOAD_FAST                1 (args)
                           2360 LOAD_ATTR               22 (parse_url)
-                          2370 POP_JUMP_FORWARD_IF_FALSE   102 (to 2576)
+                          2370 POP_JUMP_FORWARD_IF_FALSE   103 (to 2578)
                
                 85        2372 LOAD_DEREF               0 (self)
                           2374 LOAD_ATTR                1 (ptjsonlib)
                           2384 LOAD_METHOD             23 (parse_url2nodes)
                           2406 LOAD_FAST               10 (issue_host)
                           2408 LOAD_FAST               11 (issue_location)
                           2410 BINARY_OP                0 (+)
@@ -716,90 +716,90 @@
                 90        2530 LOAD_FAST                5 (result_node_list)
                           2532 LOAD_METHOD             24 (append)
                           2554 LOAD_FAST               35 (n)
                           2556 PRECALL                  1
                           2560 CALL                     1
                           2570 POP_TOP
                           2572 JUMP_BACKWARD           24 (to 2526)
-                       >> 2574 JUMP_FORWARD            90 (to 2756)
+                       >> 2574 EXTENDED_ARG             4
+                          2576 JUMP_BACKWARD         1121 (to 336)
                
-                92     >> 2576 LOAD_DEREF               0 (self)
-                          2578 LOAD_ATTR                1 (ptjsonlib)
-                          2588 LOAD_METHOD             25 (create_node_object)
+                92     >> 2578 LOAD_DEREF               0 (self)
+                          2580 LOAD_ATTR                1 (ptjsonlib)
+                          2590 LOAD_METHOD             25 (create_node_object)
+               
+                93        2612 LOAD_CONST              37 ('webSource')
+               
+                94        2614 LOAD_FAST               31 (penterep_root_node)
+               
+                96        2616 LOAD_FAST               10 (issue_host)
+                          2618 LOAD_FAST               11 (issue_location)
+                          2620 BINARY_OP                0 (+)
+               
+                97        2624 LOAD_FAST               11 (issue_location)
+               
+                98        2626 LOAD_GLOBAL             53 (NULL + PtPathTypeDetector)
+                          2638 PRECALL                  0
+                          2642 CALL                     0
+                          2652 LOAD_METHOD             27 (get_type)
+                          2674 LOAD_FAST               11 (issue_location)
+                          2676 PRECALL                  1
+                          2680 CALL                     1
+               
+                95        2690 LOAD_CONST              38 (('url', 'name', 'webSourceType'))
+                          2692 BUILD_CONST_KEY_MAP      3
+               
+               100        2694 LOAD_FAST               33 (vulnerability)
+                          2696 BUILD_LIST               1
+               
+                92        2698 KW_NAMES                39
+                          2700 PRECALL                  4
+                          2704 CALL                     4
+                          2714 STORE_FAST              36 (node)
+               
+               102        2716 LOAD_FAST                5 (result_node_list)
+                          2718 LOAD_METHOD             24 (append)
+                          2740 LOAD_FAST               36 (node)
+                          2742 PRECALL                  1
+                          2746 CALL                     1
+                          2756 POP_TOP
+                          2758 EXTENDED_ARG             4
+                          2760 JUMP_BACKWARD         1213 (to 336)
                
-                93        2610 LOAD_CONST              37 ('webSource')
+                26     >> 2762 NOP
                
-                94        2612 LOAD_FAST               31 (penterep_root_node)
-               
-                96        2614 LOAD_FAST               10 (issue_host)
-                          2616 LOAD_FAST               11 (issue_location)
-                          2618 BINARY_OP                0 (+)
-               
-                97        2622 LOAD_FAST               11 (issue_location)
-               
-                98        2624 LOAD_GLOBAL             53 (NULL + PtPathTypeDetector)
-                          2636 PRECALL                  0
-                          2640 CALL                     0
-                          2650 LOAD_METHOD             27 (get_type)
-                          2672 LOAD_FAST               11 (issue_location)
-                          2674 PRECALL                  1
-                          2678 CALL                     1
-               
-                95        2688 LOAD_CONST              38 (('url', 'name', 'webSourceType'))
-                          2690 BUILD_CONST_KEY_MAP      3
-               
-               100        2692 LOAD_FAST               33 (vulnerability)
-                          2694 BUILD_LIST               1
-               
-                92        2696 KW_NAMES                39
-                          2698 PRECALL                  4
-                          2702 CALL                     4
-                          2712 STORE_FAST              36 (node)
-               
-               102        2714 LOAD_FAST                5 (result_node_list)
-                          2716 LOAD_METHOD             24 (append)
-                          2738 LOAD_FAST               36 (node)
-                          2740 PRECALL                  1
-                          2744 CALL                     1
-                          2754 POP_TOP
-               
-               104     >> 2756 EXTENDED_ARG             4
-                          2758 JUMP_BACKWARD         1212 (to 336)
-               
-                26     >> 2760 NOP
-               
-                23        2762 LOAD_CONST               0 (None)
-                          2764 LOAD_CONST               0 (None)
+                23        2764 LOAD_CONST               0 (None)
                           2766 LOAD_CONST               0 (None)
-                          2768 PRECALL                  2
-                          2772 CALL                     2
-                          2782 POP_TOP
-                          2784 JUMP_FORWARD            11 (to 2808)
-                       >> 2786 PUSH_EXC_INFO
-                          2788 WITH_EXCEPT_START
-                          2790 POP_JUMP_FORWARD_IF_TRUE     4 (to 2800)
-                          2792 RERAISE                  2
-                       >> 2794 COPY                     3
-                          2796 POP_EXCEPT
-                          2798 RERAISE                  1
-                       >> 2800 POP_TOP
-                          2802 POP_EXCEPT
-                          2804 POP_TOP
+                          2768 LOAD_CONST               0 (None)
+                          2770 PRECALL                  2
+                          2774 CALL                     2
+                          2784 POP_TOP
+                          2786 JUMP_FORWARD            11 (to 2810)
+                       >> 2788 PUSH_EXC_INFO
+                          2790 WITH_EXCEPT_START
+                          2792 POP_JUMP_FORWARD_IF_TRUE     4 (to 2802)
+                          2794 RERAISE                  2
+                       >> 2796 COPY                     3
+                          2798 POP_EXCEPT
+                          2800 RERAISE                  1
+                       >> 2802 POP_TOP
+                          2804 POP_EXCEPT
                           2806 POP_TOP
+                          2808 POP_TOP
                
-               127     >> 2808 LOAD_FAST                5 (result_node_list)
-                          2810 RETURN_VALUE
+               104     >> 2810 LOAD_FAST                5 (result_node_list)
+                          2812 RETURN_VALUE
                ExceptionTable:
                  74 to 164 -> 168 [0]
                  168 to 186 -> 200 [1] lasti
                  188 to 188 -> 190 [1] lasti
                  190 to 198 -> 200 [1] lasti
-                 252 to 2758 -> 2786 [1] lasti
-                 2786 to 2792 -> 2794 [3] lasti
-                 2800 to 2800 -> 2794 [3] lasti
+                 252 to 2760 -> 2788 [1] lasti
+                 2788 to 2794 -> 2796 [3] lasti
+                 2802 to 2802 -> 2796 [3] lasti
                consts
                   None
                   '--csv parameter is required for BurpReportParser module'
                   True
                   'r'
                   'issue'
                   'type'
@@ -838,15 +838,15 @@
                                   54 JUMP_BACKWARD           24 (to 8)
                              >>   56 RETURN_VALUE
                      consts
                      names      ('get_text_safely',)
                      varnames   ('.0', 'item')
                      freevars   ('self',)
                      cellvars   ()
-                     filename   '/home/kali/penterep/dkummel/ptconvert/ptconvert/modules/burp_report.py'
+                     filename   '/home/kali/penterep/penterep-public/ptconvert/ptconvert/modules/burp_report.py'
                      name       '<listcomp>'
                      firstlineno 41
                      lnotab 0x
                   'issueDetailItem'
                   'requestresponse'
                   'request'
                   'response'
@@ -868,35 +868,35 @@
                   'webSource'
                   ('url', 'name', 'webSourceType')
                   ('node_type', 'parent_type', 'properties', 'vulnerabilities')
                names      ('csv', 'ptjsonlib', 'end_error', 'load_xml', 'input', 'getroot', 'Exception', 'open', 'reader', 'findall', 'get_text_safely', 'find', 'use_texts', 'get', 'get_cwe_from_vulnerability_classifications', 'hex', 'int', 'lstrip', 'seek', 'update', 'ptmisclib', 'clean_html', 'parse_url', 'parse_url2nodes', 'append', 'create_node_object', 'PtPathTypeDetector', 'get_type')
                varnames   ('self', 'args', 'tree', 'root_element', 'e', 'result_node_list', 'file', 'csv_reader', 'issue', 'issue_type', 'issue_host', 'issue_location', 'issue_name', 'issue_path', 'issue_host_ip', 'issue_severity', 'issue_background', 'issue_remediation', 'issue_detail', 'issue_detail_items', 'request_response', 'issue_request', 'issue_response', 'issue_request_method', 'issue_references', 'issue_vulnerability_classifications', 'issue_cwe', 'found_record', 'row', 'hex_issue_type', 'penterep_vuln_code', 'penterep_root_node', 'penterep_target_node', 'vulnerability', 'node_list', 'n', 'node')
                freevars   ()
                cellvars   ('self',)
-               filename   '/home/kali/penterep/dkummel/ptconvert/ptconvert/modules/burp_report.py'
+               filename   '/home/kali/penterep/penterep-public/ptconvert/ptconvert/modules/burp_report.py'
                name       'convert'
                firstlineno 12
                lnotab
                   0x04010e013602020134012c0112010aff080304012c0128023001500150
                   015002100150015001580150015001500150022a01980204022a01040150
                   01500152020c02500250012a030401080148013e01300104012a0104fc02
                   0504012a010c0208010e01180202010201020126012601260102f904ff10
-                  0b0e013a0104011601420108012e022201020102020801020140fd040504
-                  f8120a2a0204b202fd2e68
+                  0b0e013a01040116014201080130022201020102020801020140fd040504
+                  f8120a2eb402fd2e51
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 1
                flags     : 3
                code
                   0x97007c01810e7c016a00000000000000000081077c016a000000000000
                   0000006e0164015300
-               129           0 RESUME                   0
+               106           0 RESUME                   0
                
-               130           2 LOAD_FAST                1 (element)
+               107           2 LOAD_FAST                1 (element)
                              4 POP_JUMP_FORWARD_IF_NONE    14 (to 34)
                              6 LOAD_FAST                1 (element)
                              8 LOAD_ATTR                0 (text)
                             18 POP_JUMP_FORWARD_IF_NONE     7 (to 34)
                             20 LOAD_FAST                1 (element)
                             22 LOAD_ATTR                0 (text)
                             32 JUMP_FORWARD             1 (to 36)
@@ -905,30 +905,30 @@
                consts
                   None
                   ''
                names      ('text',)
                varnames   ('self', 'element')
                freevars   ()
                cellvars   ()
-               filename   '/home/kali/penterep/dkummel/ptconvert/ptconvert/modules/burp_report.py'
+               filename   '/home/kali/penterep/penterep-public/ptconvert/ptconvert/modules/burp_report.py'
                name       'get_text_safely'
-               firstlineno 129
+               firstlineno 106
                lnotab 0x0201
             'vulnerability_classification'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 4
                flags     : 3
                code
                   0x97007401000000000000000000006a01000000000000000064017c01a6
                   020000ab0200000000000000006402190000000000000000005300
-               132           0 RESUME                   0
+               109           0 RESUME                   0
                
-               135           2 LOAD_GLOBAL              1 (NULL + re)
+               112           2 LOAD_GLOBAL              1 (NULL + re)
                             14 LOAD_ATTR                1 (findall)
                             24 LOAD_CONST               1 ('CWE-(\\d*)')
                             26 LOAD_FAST                1 (vulnerability_classification)
                             28 PRECALL                  2
                             32 CALL                     2
                             42 LOAD_CONST               2 (0)
                             44 BINARY_SUBSCR
@@ -937,29 +937,29 @@
                   'Retrieve CWE from provided <vulnerability_classification> element'
                   'CWE-(\\d*)'
                   0
                names      ('re', 'findall')
                varnames   ('self', 'vulnerability_classification')
                freevars   ()
                cellvars   ()
-               filename   '/home/kali/penterep/dkummel/ptconvert/ptconvert/modules/burp_report.py'
+               filename   '/home/kali/penterep/penterep-public/ptconvert/ptconvert/modules/burp_report.py'
                name       'get_cwe_from_vulnerability_classifications'
-               firstlineno 132
+               firstlineno 109
                lnotab 0x0203
             None
          names      ('__name__', '__module__', '__qualname__', 'object', '__init__', 'list', 'convert', 'get_text_safely', 'str', 'get_cwe_from_vulnerability_classifications')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/kali/penterep/dkummel/ptconvert/ptconvert/modules/burp_report.py'
+         filename   '/home/kali/penterep/penterep-public/ptconvert/ptconvert/modules/burp_report.py'
          name       'BurpReportParser'
          firstlineno 8
-         lnotab 0x0a010c030c750603
+         lnotab 0x0a010c030c5e0603
       'BurpReportParser'
    names      ('_baseclass', 'BaseClass', 'csv', 're', 'json', 'ptlibs', 'ptmisclib', 'ptlibs.ptpathtypedetector', 'PtPathTypeDetector', 'BurpReportParser')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/home/kali/penterep/dkummel/ptconvert/ptconvert/modules/burp_report.py'
+   filename   '/home/kali/penterep/penterep-public/ptconvert/ptconvert/modules/burp_report.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff02010c0218020c010c02
```

### Comparing `ptconvert-0.0.1/ptconvert/modules/__pycache__/csv.cpython-311.pyc` & `ptconvert-0.0.2/ptconvert/modules/__pycache__/csv.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ptconvert-0.0.1/ptconvert/modules/_baseclass.py` & `ptconvert-0.0.2/ptconvert/modules/_baseclass.py`

 * *Files identical despite different names*

### Comparing `ptconvert-0.0.1/ptconvert/modules/burp_report.py` & `ptconvert-0.0.2/ptconvert/modules/burp_report.py`

 * *Files 20% similar despite different names*

```diff
@@ -97,37 +97,14 @@
                             "name": issue_location,
                             "webSourceType": PtPathTypeDetector().get_type(issue_location)
                         },
                         vulnerabilities=[vulnerability]
                     )
                     result_node_list.append(node)
 
-                """
-                print(
-                    f"TYPE: {issue_type}",
-                    f"PT-VULN-CODE: {penterep_vuln_code}",
-                    f"PT-ROOT-NODE: {penterep_root_node}",
-                    f"PT-TARGET-NODE: {penterep_target_node}",
-                    f"NAME: {issue_name}",
-                    f"PATH: {issue_path}",
-                    f"LOCATION: {issue_location}",
-                    f"SEVERITY: {issue_severity}",
-                    f"BACKGROUND: {issue_background}",
-                    f"REMEDIATION: {issue_remediation}",
-                    f"DETAIL: {issue_detail}",
-                    f"DETAIL_ITEMS: {issue_detail_items}",
-                    f"REQUEST: ...",
-                    f"REQUEST METHOD: {issue_request_method}",
-                    f"RESPONSE: ...",
-                    f"REFERENCES: {issue_references}",
-                    f"VULN CLASSIFICATION: {issue_vulnerability_classifications}",
-                    sep="\n",
-                    end="\n---------------\n\n"
-                )
-                """
         return result_node_list
 
     def get_text_safely(self, element):
         return element.text if element is not None and element.text is not None else ""
 
     def get_cwe_from_vulnerability_classifications(self, vulnerability_classification: str) -> str:
         """Retrieve CWE from provided <vulnerability_classification> element"""
```

### Comparing `ptconvert-0.0.1/ptconvert/modules/swagger.py` & `ptconvert-0.0.2/ptconvert/modules/swagger.py`

 * *Files identical despite different names*

### Comparing `ptconvert-0.0.1/ptconvert/ptconvert.py` & `ptconvert-0.0.2/ptconvert/ptconvert.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 
 class PtConvert:
     def __init__(self):
         self.ptjsonlib = ptjsonlib.PtJsonLib()
 
     def run(self, args):
         parser_class = getattr(self.load_and_get_module(args.format.replace('-', "_")), f"{format_string(args.format.capitalize())}Parser")
-        #nodes_list = parser_class(self.ptjsonlib).convert(args)
         try:
             nodes_list = parser_class(self.ptjsonlib).convert(args)
         except Exception as e:
             print(e)
             self.ptjsonlib.end_error(f"Error occured inside {parser_class}", True)
 
         self.ptjsonlib.add_nodes(nodes_list)
@@ -99,17 +98,23 @@
     parser.add_argument("-f",  "--format",     type=lambda s: s.lower(), required=True, choices=([module[2].lstrip() for module in get_modules_help()]))
 
     parser.add_argument("--csv",               type=str)
     parser.add_argument("--parse-url",         action="store_true")
     parser.add_argument("--use-texts",         action="store_true")
     parser.add_argument("-v",  "--version",    action="version", version=f"%(prog)s {__version__}")
 
+    parser.add_argument("--socket-address",    type=str, default=None)
+    parser.add_argument("--socket-port",       type=str, default=None)
+    parser.add_argument("--process-ident",     type=str, default=None)
+
+
     if len(sys.argv) == 1 or "-h" in sys.argv or "--help" in sys.argv:
         ptprinthelper.help_print(get_help(), SCRIPTNAME, __version__)
         sys.exit(0)
+
     args = parser.parse_args()
     ptprinthelper.print_banner(SCRIPTNAME, __version__, False)
     return args
 
 
 def main():
     global SCRIPTNAME
```

### Comparing `ptconvert-0.0.1/ptconvert.egg-info/PKG-INFO` & `ptconvert-0.0.2/ptconvert.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 Metadata-Version: 2.1
 Name: ptconvert
-Version: 0.0.1
+Version: 0.0.2
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
 License: GPLv3
+Project-URL: homepage, https://www.penterep.com/
+Project-URL: repository, https://github.com/penterep/ptconvert
+Project-URL: tracker, https://github.com/penterep/ptconvert/issues
+Project-URL: changelog, https://github.com/penterep/ptconvert/blob/main/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Environment :: Console
 Classifier: Topic :: Security
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ptlibs<2,>=1.0.7
 
 [![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)](https://www.penterep.com/)
 
 
-## PTCONVERT - Penterep Data Format Converter
+## PTCONVERT - Penterep Data Format Convertor
 
 ptconvert is a tool that transforms various data formats into Penterep-compatible JSON.
 
 ## Installation
 
 ```
 pip install ptconvert
@@ -46,21 +50,26 @@
 ## Usage examples
 ```
 ptconvert -f swagger -i swagger_file.json -o penterep.json
 ```
 
 ## Options
 ```
-   -i  --input    <file>    Set input file
-   -o  --output   <output>  Set output file
-   -f  --format   <format>  Set input file format to:
-                   swagger      Swagger format
+-i  --input      <file>         Set input file
+-o  --output     <output>       Set output file
+-f  --format     <format>       Set input file format to:
+                  burp-report    BurpReport format
+                  swagger        Swagger format
+
+      --csv        <path-to-csv>  Set path to CSV file
+      --use-texts                 Use texts from Burp Report
+      --parse-url                 Parse URLs in Burp Report
 
-   -v  --version            Show script version and exit
-   -h  --help               Show this help message and exit
+-v  --version                   Show script version and exit
+-h  --help                      Show this help message and exit
 ```
 
 ## Dependencies
 ```
 ptlibs
 ```
```

### Comparing `ptconvert-0.0.1/ptconvert.egg-info/SOURCES.txt` & `ptconvert-0.0.2/ptconvert.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,11 +9,13 @@
 ptconvert.egg-info/SOURCES.txt
 ptconvert.egg-info/dependency_links.txt
 ptconvert.egg-info/entry_points.txt
 ptconvert.egg-info/requires.txt
 ptconvert.egg-info/top_level.txt
 ptconvert/modules/_baseclass.py
 ptconvert/modules/burp_report.py
+ptconvert/modules/burp_report.txt
 ptconvert/modules/swagger.py
 ptconvert/modules/__pycache__/_baseclass.cpython-311.pyc
 ptconvert/modules/__pycache__/burp_report.cpython-311.pyc
-ptconvert/modules/__pycache__/csv.cpython-311.pyc
+ptconvert/modules/__pycache__/csv.cpython-311.pyc
+ptconvert/modules/__pycache__/swagger.cpython-311.pyc
```

