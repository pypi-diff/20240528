# Comparing `tmp/generate_temp_table_sql-0.4.2.tar.gz` & `tmp/generate_temp_table_sql-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "generate_temp_table_sql-0.4.2.tar", last modified: Mon May 27 17:01:08 2024, max compression
+gzip compressed data, was "generate_temp_table_sql-0.4.3.tar", last modified: Tue May 28 12:02:06 2024, max compression
```

## Comparing `generate_temp_table_sql-0.4.2.tar` & `generate_temp_table_sql-0.4.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 ryanwaldorf   (501) staff       (20)        0 2024-05-27 17:01:08.456885 generate_temp_table_sql-0.4.2/
--rw-r--r--   0 ryanwaldorf   (501) staff       (20)     1068 2024-05-26 15:44:57.000000 generate_temp_table_sql-0.4.2/LICENSE.txt
--rw-r--r--   0 ryanwaldorf   (501) staff       (20)       37 2024-05-26 15:46:01.000000 generate_temp_table_sql-0.4.2/MANIFEST.in
--rw-r--r--   0 ryanwaldorf   (501) staff       (20)     3206 2024-05-27 17:01:08.456797 generate_temp_table_sql-0.4.2/PKG-INFO
--rw-r--r--   0 ryanwaldorf   (501) staff       (20)     2683 2024-05-27 13:31:42.000000 generate_temp_table_sql-0.4.2/README.md
-drwxr-xr-x   0 ryanwaldorf   (501) staff       (20)        0 2024-05-27 17:01:08.455696 generate_temp_table_sql-0.4.2/generate_temp_table_sql/
--rw-r--r--   0 ryanwaldorf   (501) staff       (20)        0 2024-05-25 15:54:27.000000 generate_temp_table_sql-0.4.2/generate_temp_table_sql/__init__.py
--rw-r--r--   0 ryanwaldorf   (501) staff       (20)     2127 2024-05-27 16:33:51.000000 generate_temp_table_sql-0.4.2/generate_temp_table_sql/cli.py
--rw-r--r--   0 ryanwaldorf   (501) staff       (20)       88 2024-05-27 13:29:03.000000 generate_temp_table_sql-0.4.2/generate_temp_table_sql/constants.py
--rw-r--r--   0 ryanwaldorf   (501) staff       (20)     2559 2024-05-27 16:41:04.000000 generate_temp_table_sql-0.4.2/generate_temp_table_sql/sql_generator.py
-drwxr-xr-x   0 ryanwaldorf   (501) staff       (20)        0 2024-05-27 17:01:08.456361 generate_temp_table_sql-0.4.2/generate_temp_table_sql.egg-info/
--rw-r--r--   0 ryanwaldorf   (501) staff       (20)     3206 2024-05-27 17:01:08.000000 generate_temp_table_sql-0.4.2/generate_temp_table_sql.egg-info/PKG-INFO
--rw-r--r--   0 ryanwaldorf   (501) staff       (20)      517 2024-05-27 17:01:08.000000 generate_temp_table_sql-0.4.2/generate_temp_table_sql.egg-info/SOURCES.txt
--rw-r--r--   0 ryanwaldorf   (501) staff       (20)        1 2024-05-27 17:01:08.000000 generate_temp_table_sql-0.4.2/generate_temp_table_sql.egg-info/dependency_links.txt
--rw-r--r--   0 ryanwaldorf   (501) staff       (20)       70 2024-05-27 17:01:08.000000 generate_temp_table_sql-0.4.2/generate_temp_table_sql.egg-info/entry_points.txt
--rw-r--r--   0 ryanwaldorf   (501) staff       (20)        7 2024-05-27 17:01:08.000000 generate_temp_table_sql-0.4.2/generate_temp_table_sql.egg-info/requires.txt
--rw-r--r--   0 ryanwaldorf   (501) staff       (20)       30 2024-05-27 17:01:08.000000 generate_temp_table_sql-0.4.2/generate_temp_table_sql.egg-info/top_level.txt
--rw-r--r--   0 ryanwaldorf   (501) staff       (20)       38 2024-05-27 17:01:08.456930 generate_temp_table_sql-0.4.2/setup.cfg
--rw-r--r--   0 ryanwaldorf   (501) staff       (20)      819 2024-05-27 16:58:47.000000 generate_temp_table_sql-0.4.2/setup.py
-drwxr-xr-x   0 ryanwaldorf   (501) staff       (20)        0 2024-05-27 17:01:08.456550 generate_temp_table_sql-0.4.2/tests/
--rw-r--r--   0 ryanwaldorf   (501) staff       (20)        0 2024-05-25 16:57:00.000000 generate_temp_table_sql-0.4.2/tests/__init__.py
--rw-r--r--   0 ryanwaldorf   (501) staff       (20)     5435 2024-05-27 16:45:56.000000 generate_temp_table_sql-0.4.2/tests/test_sql_generator.py
+drwxr-xr-x   0 ryanwaldorf   (501) staff       (20)        0 2024-05-28 12:02:06.748697 generate_temp_table_sql-0.4.3/
+-rw-r--r--   0 ryanwaldorf   (501) staff       (20)     1068 2024-05-26 15:44:57.000000 generate_temp_table_sql-0.4.3/LICENSE.txt
+-rw-r--r--   0 ryanwaldorf   (501) staff       (20)       37 2024-05-26 15:46:01.000000 generate_temp_table_sql-0.4.3/MANIFEST.in
+-rw-r--r--   0 ryanwaldorf   (501) staff       (20)     4184 2024-05-28 12:02:06.748606 generate_temp_table_sql-0.4.3/PKG-INFO
+-rw-r--r--   0 ryanwaldorf   (501) staff       (20)     3661 2024-05-28 11:46:17.000000 generate_temp_table_sql-0.4.3/README.md
+drwxr-xr-x   0 ryanwaldorf   (501) staff       (20)        0 2024-05-28 12:02:06.747195 generate_temp_table_sql-0.4.3/generate_temp_table_sql/
+-rw-r--r--   0 ryanwaldorf   (501) staff       (20)        0 2024-05-25 15:54:27.000000 generate_temp_table_sql-0.4.3/generate_temp_table_sql/__init__.py
+-rw-r--r--   0 ryanwaldorf   (501) staff       (20)     2135 2024-05-28 12:00:45.000000 generate_temp_table_sql-0.4.3/generate_temp_table_sql/cli.py
+-rw-r--r--   0 ryanwaldorf   (501) staff       (20)       88 2024-05-27 13:29:03.000000 generate_temp_table_sql-0.4.3/generate_temp_table_sql/constants.py
+-rw-r--r--   0 ryanwaldorf   (501) staff       (20)     2559 2024-05-27 16:41:04.000000 generate_temp_table_sql-0.4.3/generate_temp_table_sql/sql_generator.py
+drwxr-xr-x   0 ryanwaldorf   (501) staff       (20)        0 2024-05-28 12:02:06.748004 generate_temp_table_sql-0.4.3/generate_temp_table_sql.egg-info/
+-rw-r--r--   0 ryanwaldorf   (501) staff       (20)     4184 2024-05-28 12:02:06.000000 generate_temp_table_sql-0.4.3/generate_temp_table_sql.egg-info/PKG-INFO
+-rw-r--r--   0 ryanwaldorf   (501) staff       (20)      517 2024-05-28 12:02:06.000000 generate_temp_table_sql-0.4.3/generate_temp_table_sql.egg-info/SOURCES.txt
+-rw-r--r--   0 ryanwaldorf   (501) staff       (20)        1 2024-05-28 12:02:06.000000 generate_temp_table_sql-0.4.3/generate_temp_table_sql.egg-info/dependency_links.txt
+-rw-r--r--   0 ryanwaldorf   (501) staff       (20)       70 2024-05-28 12:02:06.000000 generate_temp_table_sql-0.4.3/generate_temp_table_sql.egg-info/entry_points.txt
+-rw-r--r--   0 ryanwaldorf   (501) staff       (20)        7 2024-05-28 12:02:06.000000 generate_temp_table_sql-0.4.3/generate_temp_table_sql.egg-info/requires.txt
+-rw-r--r--   0 ryanwaldorf   (501) staff       (20)       30 2024-05-28 12:02:06.000000 generate_temp_table_sql-0.4.3/generate_temp_table_sql.egg-info/top_level.txt
+-rw-r--r--   0 ryanwaldorf   (501) staff       (20)       38 2024-05-28 12:02:06.748734 generate_temp_table_sql-0.4.3/setup.cfg
+-rw-r--r--   0 ryanwaldorf   (501) staff       (20)      819 2024-05-28 12:01:10.000000 generate_temp_table_sql-0.4.3/setup.py
+drwxr-xr-x   0 ryanwaldorf   (501) staff       (20)        0 2024-05-28 12:02:06.748287 generate_temp_table_sql-0.4.3/tests/
+-rw-r--r--   0 ryanwaldorf   (501) staff       (20)        0 2024-05-25 16:57:00.000000 generate_temp_table_sql-0.4.3/tests/__init__.py
+-rw-r--r--   0 ryanwaldorf   (501) staff       (20)     5435 2024-05-27 16:45:56.000000 generate_temp_table_sql-0.4.3/tests/test_sql_generator.py
```

### Comparing `generate_temp_table_sql-0.4.2/LICENSE.txt` & `generate_temp_table_sql-0.4.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `generate_temp_table_sql-0.4.2/PKG-INFO` & `generate_temp_table_sql-0.4.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,201 +1,229 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 6765 6e65  : 2.1.Name: gene
-00000020: 7261 7465 5f74 656d 705f 7461 626c 655f  rate_temp_table_
-00000030: 7371 6c0a 5665 7273 696f 6e3a 2030 2e34  sql.Version: 0.4
-00000040: 2e32 0a53 756d 6d61 7279 3a20 4120 7061  .2.Summary: A pa
-00000050: 636b 6167 6520 746f 2067 656e 6572 6174  ckage to generat
-00000060: 6520 5351 4c20 7374 6174 656d 656e 7473  e SQL statements
-00000070: 2066 726f 6d20 4353 5620 6669 6c65 730a   from CSV files.
-00000080: 486f 6d65 2d70 6167 653a 2068 7474 7073  Home-page: https
-00000090: 3a2f 2f67 6974 6875 622e 636f 6d2f 7279  ://github.com/ry
-000000a0: 616e 7761 6c64 6f72 662f 6765 6e65 7261  anwaldorf/genera
-000000b0: 7465 5f74 656d 705f 7461 626c 655f 7371  te_temp_table_sq
-000000c0: 6c0a 4175 7468 6f72 3a20 5279 616e 2057  l.Author: Ryan W
-000000d0: 616c 646f 7266 0a41 7574 686f 722d 656d  aldorf.Author-em
-000000e0: 6169 6c3a 2072 7961 6e40 7279 616e 7761  ail: ryan@ryanwa
-000000f0: 6c64 6f72 662e 636f 6d0a 4c69 6365 6e73  ldorf.com.Licens
-00000100: 653a 2055 4e4b 4e4f 574e 0a50 6c61 7466  e: UNKNOWN.Platf
-00000110: 6f72 6d3a 2055 4e4b 4e4f 574e 0a43 6c61  orm: UNKNOWN.Cla
-00000120: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
-00000130: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000140: 2050 7974 686f 6e20 3a3a 2033 0a43 6c61   Python :: 3.Cla
-00000150: 7373 6966 6965 723a 204c 6963 656e 7365  ssifier: License
-00000160: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
-00000170: 203a 3a20 4d49 5420 4c69 6365 6e73 650a   :: MIT License.
-00000180: 436c 6173 7369 6669 6572 3a20 4f70 6572  Classifier: Oper
-00000190: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
-000001a0: 4f53 2049 6e64 6570 656e 6465 6e74 0a52  OS Independent.R
-000001b0: 6571 7569 7265 732d 5079 7468 6f6e 3a20  equires-Python: 
-000001c0: 3e3d 332e 360a 4465 7363 7269 7074 696f  >=3.6.Descriptio
-000001d0: 6e2d 436f 6e74 656e 742d 5479 7065 3a20  n-Content-Type: 
-000001e0: 7465 7874 2f6d 6172 6b64 6f77 6e0a 4c69  text/markdown.Li
-000001f0: 6365 6e73 652d 4669 6c65 3a20 4c49 4345  cense-File: LICE
-00000200: 4e53 452e 7478 740a 0a23 2047 656e 6572  NSE.txt..# Gener
-00000210: 6174 6520 5465 6d70 2054 6162 6c65 2053  ate Temp Table S
-00000220: 514c 0a0a 4765 6e65 7261 7465 2054 656d  QL..Generate Tem
-00000230: 7020 5461 626c 6520 5351 4c20 6973 2061  p Table SQL is a
-00000240: 2050 7974 686f 6e20 7061 636b 6167 6520   Python package 
-00000250: 7468 6174 2067 656e 6572 6174 6573 2053  that generates S
-00000260: 514c 2073 7461 7465 6d65 6e74 7320 666f  QL statements fo
-00000270: 7220 6372 6561 7469 6e67 2061 2074 656d  r creating a tem
-00000280: 706f 7261 7279 2074 6162 6c65 2061 6e64  porary table and
-00000290: 2069 6e73 6572 7469 6e67 2064 6174 6120   inserting data 
-000002a0: 6672 6f6d 2061 2043 5356 2066 696c 652e  from a CSV file.
-000002b0: 2020 4974 2773 2075 7365 6675 6c20 7768    It's useful wh
-000002c0: 656e 2079 6f75 206e 6565 6420 746f 206d  en you need to m
-000002d0: 6f76 6520 6461 7461 2062 6574 7765 656e  ove data between
-000002e0: 2064 6174 6120 7761 7265 686f 7573 6573   data warehouses
-000002f0: 2074 6861 7420 6172 6520 6f74 6865 7277   that are otherw
-00000300: 6973 6520 6e6f 7420 636f 6e6e 6563 7465  ise not connecte
-00000310: 642c 2073 6f20 796f 7520 6361 6e20 646f  d, so you can do
-00000320: 776e 6c6f 6164 2061 2043 5356 2061 6e64  wnload a CSV and
-00000330: 2072 6563 7265 6174 6520 7468 6520 6461   recreate the da
-00000340: 7461 2069 6e20 7468 6520 6f74 6865 7220  ta in the other 
-00000350: 7761 7265 686f 7573 6520 6173 2061 2074  warehouse as a t
-00000360: 656d 706f 7261 7279 2074 6162 6c65 2066  emporary table f
-00000370: 726f 6d20 7468 6520 4353 562e 0a0a 2323  rom the CSV...##
-00000380: 2046 6561 7475 7265 730a 0a2d 204c 6f61   Features..- Loa
-00000390: 6420 6461 7461 2066 726f 6d20 6120 4353  d data from a CS
-000003a0: 5620 6669 6c65 0a2d 2047 656e 6572 6174  V file.- Generat
-000003b0: 6520 6120 6043 5245 4154 4520 5445 4d50  e a `CREATE TEMP
-000003c0: 2054 4142 4c45 6020 5351 4c20 7374 6174   TABLE` SQL stat
-000003d0: 656d 656e 740a 2d20 4765 6e65 7261 7465  ement.- Generate
-000003e0: 2060 494e 5345 5254 2049 4e54 4f60 2053   `INSERT INTO` S
-000003f0: 514c 2073 7461 7465 6d65 6e74 7320 666f  QL statements fo
-00000400: 7220 7468 6520 6461 7461 0a2d 2043 6f6d  r the data.- Com
-00000410: 6d61 6e64 2d6c 696e 6520 696e 7465 7266  mand-line interf
-00000420: 6163 6520 2843 4c49 2920 666f 7220 6561  ace (CLI) for ea
-00000430: 7379 2075 7361 6765 0a0a 2323 2049 6e73  sy usage..## Ins
-00000440: 7461 6c6c 6174 696f 6e0a 0a23 2323 2050  tallation..### P
-00000450: 7265 7265 7175 6973 6974 6573 0a0a 2d20  rerequisites..- 
-00000460: 5079 7468 6f6e 2033 2e36 206f 7220 6869  Python 3.6 or hi
-00000470: 6768 6572 0a2d 2060 7061 6e64 6173 6020  gher.- `pandas` 
-00000480: 6c69 6272 6172 790a 0a23 2323 2049 6e73  library..### Ins
-00000490: 7461 6c6c 696e 670a 0a31 2e20 436c 6f6e  talling..1. Clon
-000004a0: 6520 7468 6520 7265 706f 7369 746f 7279  e the repository
-000004b0: 3a0a 2020 2020 6060 6073 680a 2020 2020  :.    ```sh.    
-000004c0: 6769 7420 636c 6f6e 6520 6874 7470 733a  git clone https:
-000004d0: 2f2f 6769 7468 7562 2e63 6f6d 2f72 7977  //github.com/ryw
-000004e0: 616c 646f 722f 6765 6e65 7261 7465 5f74  aldor/generate_t
-000004f0: 656d 705f 7461 626c 655f 7371 6c2e 6769  emp_table_sql.gi
-00000500: 740a 2020 2020 6364 2067 656e 6572 6174  t.    cd generat
-00000510: 655f 7465 6d70 5f74 6162 6c65 5f73 716c  e_temp_table_sql
-00000520: 0a20 2020 2060 6060 0a0a 322e 2049 6e73  .    ```..2. Ins
-00000530: 7461 6c6c 2074 6865 2070 6163 6b61 6765  tall the package
-00000540: 206c 6f63 616c 6c79 3a0a 2020 2020 6060   locally:.    ``
-00000550: 6073 680a 2020 2020 7069 7020 696e 7374  `sh.    pip inst
-00000560: 616c 6c20 2d65 202e 0a20 2020 2060 6060  all -e ..    ```
-00000570: 0a0a 2323 2055 7361 6765 0a0a 2323 2320  ..## Usage..### 
-00000580: 436f 6d6d 616e 642d 4c69 6e65 2049 6e74  Command-Line Int
-00000590: 6572 6661 6365 2028 434c 4929 0a0a 4166  erface (CLI)..Af
-000005a0: 7465 7220 696e 7374 616c 6c69 6e67 2074  ter installing t
-000005b0: 6865 2070 6163 6b61 6765 2c20 796f 7520  he package, you 
-000005c0: 6361 6e20 7573 6520 7468 6520 6067 656e  can use the `gen
-000005d0: 6572 6174 652d 7474 2d73 716c 6020 636f  erate-tt-sql` co
-000005e0: 6d6d 616e 6420 746f 2067 656e 6572 6174  mmand to generat
-000005f0: 6520 5351 4c20 7374 6174 656d 656e 7473  e SQL statements
-00000600: 2066 726f 6d20 6120 4353 5620 6669 6c65   from a CSV file
-00000610: 2e0a 0a23 2323 2320 4261 7369 6320 5573  ...#### Basic Us
-00000620: 6167 650a 0a54 6f20 6765 6e65 7261 7465  age..To generate
-00000630: 2053 514c 2073 7461 7465 6d65 6e74 7320   SQL statements 
-00000640: 616e 6420 7361 7665 2074 6865 6d20 746f  and save them to
-00000650: 2061 2066 696c 653a 0a60 6060 7368 0a67   a file:.```sh.g
-00000660: 656e 6572 6174 652d 7474 2d73 716c 2070  enerate-tt-sql p
-00000670: 6174 682f 746f 2f79 6f75 722f 6669 6c65  ath/to/your/file
-00000680: 2e63 7376 0a60 6060 0a0a 2323 2323 2041  .csv.```..#### A
-00000690: 6464 6974 696f 6e61 6c20 4f70 7469 6f6e  dditional Option
-000006a0: 730a 6060 6073 680a 0a2d 2d6f 2054 6865  s.```sh..--o The
-000006b0: 2070 6174 6820 746f 2074 6865 206f 7574   path to the out
-000006c0: 7075 7420 5351 4c20 6669 6c65 2e20 2044  put SQL file.  D
-000006d0: 6566 6175 6c74 7320 746f 2074 6865 2064  efaults to the d
-000006e0: 6972 6563 746f 7220 796f 7520 6361 6c6c  irector you call
-000006f0: 2074 6865 2063 6f6d 6d61 6e64 2069 6e2e   the command in.
-00000700: 0a2d 2d6f 7665 7277 7269 7465 3a20 416c  .--overwrite: Al
-00000710: 6c6f 7720 6f76 6572 7772 6974 696e 6720  low overwriting 
-00000720: 7468 6520 6f75 7470 7574 2066 696c 6520  the output file 
-00000730: 6966 2069 7420 6578 6973 7473 2e0a 2d2d  if it exists..--
-00000740: 7461 626c 655f 6e61 6d65 3a20 5370 6563  table_name: Spec
-00000750: 6966 7920 7468 6520 6e61 6d65 206f 6620  ify the name of 
-00000760: 7468 6520 7465 6d70 6f72 6172 7920 7461  the temporary ta
-00000770: 626c 6520 746f 2063 7265 6174 652e 0a2d  ble to create..-
-00000780: 2d63 6f6c 756d 6e5f 7479 7065 3a20 5370  -column_type: Sp
-00000790: 6563 6966 7920 7468 6520 6461 7461 2074  ecify the data t
-000007a0: 7970 6520 6f66 2074 6865 2063 6f6c 756d  ype of the colum
-000007b0: 6e73 2069 6e20 7468 6520 7465 6d70 6f72  ns in the tempor
-000007c0: 6172 7920 7461 626c 652e 2044 6566 6175  ary table. Defau
-000007d0: 6c74 7320 746f 2054 4558 5420 7768 6963  lts to TEXT whic
-000007e0: 6820 776f 726b 7320 666f 7220 5265 6473  h works for Reds
-000007f0: 6869 6674 2061 6e64 2053 6e6f 7766 6c61  hift and Snowfla
-00000800: 6b65 2e20 5573 6520 5354 5249 4e47 2066  ke. Use STRING f
-00000810: 6f72 2042 6967 5175 6572 792e 0a60 6060  or BigQuery..```
-00000820: 0a0a 2323 2323 2045 7861 6d70 6c65 0a41  ..#### Example.A
-00000830: 7373 756d 6520 796f 7520 6861 7665 2061  ssume you have a
-00000840: 2043 5356 2066 696c 6520 6578 616d 706c   CSV file exampl
-00000850: 652e 6373 7620 7769 7468 2074 6865 2066  e.csv with the f
-00000860: 6f6c 6c6f 7769 6e67 2063 6f6e 7465 6e74  ollowing content
-00000870: 3a0a 0a60 6060 7368 0a6e 616d 652c 6167  :..```sh.name,ag
-00000880: 652c 6369 7479 0a4a 6f68 6e2c 3330 2c4e  e,city.John,30,N
-00000890: 6577 2059 6f72 6b0a 4a61 6e65 2c32 352c  ew York.Jane,25,
-000008a0: 4c6f 7320 416e 6765 6c65 730a 6060 600a  Los Angeles.```.
-000008b0: 0a52 756e 2074 6865 2066 6f6c 6c6f 7769  .Run the followi
-000008c0: 6e67 2063 6f6d 6d61 6e64 2074 6f20 6765  ng command to ge
-000008d0: 6e65 7261 7465 2053 514c 2073 7461 7465  nerate SQL state
-000008e0: 6d65 6e74 733a 0a0a 6060 6073 680a 6765  ments:..```sh.ge
-000008f0: 6e65 7261 7465 2d74 742d 7371 6c20 6578  nerate-tt-sql ex
-00000900: 616d 706c 652e 6373 7620 2d6f 206f 7574  ample.csv -o out
-00000910: 7075 742e 7371 6c20 2d2d 7461 626c 655f  put.sql --table_
-00000920: 6e61 6d65 206d 795f 7465 6d70 5f74 6162  name my_temp_tab
-00000930: 6c65 202d 2d63 6f6c 756d 6e5f 7479 7065  le --column_type
-00000940: 2053 5452 494e 470a 6060 600a 0a54 6865   STRING.```..The
-00000950: 206f 7574 7075 742e 7371 6c20 6669 6c65   output.sql file
-00000960: 2077 696c 6c20 636f 6e74 6169 6e3a 0a0a   will contain:..
-00000970: 6060 6073 680a 4352 4541 5445 2054 454d  ```sh.CREATE TEM
-00000980: 5020 5441 424c 4520 6d79 5f74 656d 705f  P TABLE my_temp_
-00000990: 7461 626c 6520 280a 2020 2020 6e61 6d65  table (.    name
-000009a0: 2053 5452 494e 472c 0a20 2020 2061 6765   STRING,.    age
-000009b0: 2053 5452 494e 472c 0a20 2020 2063 6974   STRING,.    cit
-000009c0: 7920 5354 5249 4e47 0a29 3b0a 0a2d 2d49  y STRING.);..--I
-000009d0: 6e73 6572 7420 4461 7461 2053 514c 3a0a  nsert Data SQL:.
-000009e0: 494e 5345 5254 2049 4e54 4f20 6d79 5f74  INSERT INTO my_t
-000009f0: 656d 705f 7461 626c 6520 286e 616d 652c  emp_table (name,
-00000a00: 2061 6765 2c20 6369 7479 2920 5641 4c55   age, city) VALU
-00000a10: 4553 200a 2020 2020 2827 4a6f 686e 272c  ES .    ('John',
-00000a20: 2027 3330 272c 2027 4e65 7720 596f 726b   '30', 'New York
-00000a30: 2729 2c0a 2020 2020 2827 4a61 6e65 272c  '),.    ('Jane',
-00000a40: 2027 3235 272c 2027 4c6f 7320 416e 6765   '25', 'Los Ange
-00000a50: 6c65 7327 293b 0a60 6060 0a0a 2323 2323  les');.```..####
-00000a60: 2052 756e 6e69 6e67 2054 6573 7473 0a54   Running Tests.T
-00000a70: 6f20 7275 6e20 7468 6520 7465 7374 732c  o run the tests,
-00000a80: 2075 7365 2074 6865 2066 6f6c 6c6f 7769   use the followi
-00000a90: 6e67 2063 6f6d 6d61 6e64 3a0a 0a60 6060  ng command:..```
-00000aa0: 7368 0a70 7974 686f 6e20 2d6d 2075 6e69  sh.python -m uni
-00000ab0: 7474 6573 7420 6469 7363 6f76 6572 202d  ttest discover -
-00000ac0: 7320 7465 7374 730a 6060 600a 0a23 2323  s tests.```..###
-00000ad0: 2320 436f 6e74 7269 6275 7469 6e67 0a43  # Contributing.C
-00000ae0: 6f6e 7472 6962 7574 696f 6e73 2061 7265  ontributions are
-00000af0: 2077 656c 636f 6d65 2120 506c 6561 7365   welcome! Please
-00000b00: 2066 6f6c 6c6f 7720 7468 6573 6520 7374   follow these st
-00000b10: 6570 733a 0a0a 312e 2046 6f72 6b20 7468  eps:..1. Fork th
-00000b20: 6520 7265 706f 7369 746f 7279 0a32 2e20  e repository.2. 
-00000b30: 4372 6561 7465 2061 206e 6577 2062 7261  Create a new bra
-00000b40: 6e63 6820 2867 6974 2063 6865 636b 6f75  nch (git checkou
-00000b50: 7420 2d62 2066 6561 7475 7265 2d62 7261  t -b feature-bra
-00000b60: 6e63 6829 0a33 2e20 436f 6d6d 6974 2079  nch).3. Commit y
-00000b70: 6f75 7220 6368 616e 6765 7320 2867 6974  our changes (git
-00000b80: 2063 6f6d 6d69 7420 2d61 6d20 2741 6464   commit -am 'Add
-00000b90: 206e 6577 2066 6561 7475 7265 2729 0a34   new feature').4
-00000ba0: 2e20 5075 7368 2074 6f20 7468 6520 6272  . Push to the br
-00000bb0: 616e 6368 2028 6769 7420 7075 7368 206f  anch (git push o
-00000bc0: 7269 6769 6e20 6665 6174 7572 652d 6272  rigin feature-br
-00000bd0: 616e 6368 290a 352e 2043 7265 6174 6520  anch).5. Create 
-00000be0: 6120 6e65 7720 5075 6c6c 2052 6571 7565  a new Pull Reque
-00000bf0: 7374 0a0a 2323 2323 204c 6963 656e 7365  st..#### License
-00000c00: 0a54 6869 7320 7072 6f6a 6563 7420 6973  .This project is
-00000c10: 206c 6963 656e 7365 6420 756e 6465 7220   licensed under 
-00000c20: 7468 6520 4d49 5420 4c69 6365 6e73 6520  the MIT License 
-00000c30: 2d20 7365 6520 7468 6520 4c49 4345 4e53  - see the LICENS
-00000c40: 4520 6669 6c65 2066 6f72 2064 6574 6169  E file for detai
-00000c50: 6c73 2e0a 0a23 2323 2320 4175 7468 6f72  ls...#### Author
-00000c60: 0a52 7961 6e20 5761 6c64 6f72 6620 2d20  .Ryan Waldorf - 
-00000c70: 7279 616e 4072 7961 6e77 616c 646f 7266  ryan@ryanwaldorf
-00000c80: 2e63 6f6d 0a0a                           .com..
+00000000: 2320 4765 6e65 7261 7465 2054 656d 7020  # Generate Temp 
+00000010: 5461 626c 6520 5351 4c0a 0a47 656e 6572  Table SQL..Gener
+00000020: 6174 6520 5465 6d70 2054 6162 6c65 2053  ate Temp Table S
+00000030: 514c 2069 7320 6120 5079 7468 6f6e 2070  QL is a Python p
+00000040: 6163 6b61 6765 2074 6861 7420 6765 6e65  ackage that gene
+00000050: 7261 7465 7320 5351 4c20 7374 6174 656d  rates SQL statem
+00000060: 656e 7473 2066 6f72 2063 7265 6174 696e  ents for creatin
+00000070: 6720 6120 7465 6d70 6f72 6172 7920 7461  g a temporary ta
+00000080: 626c 6520 616e 6420 696e 7365 7274 696e  ble and insertin
+00000090: 6720 6461 7461 2066 726f 6d20 6120 4353  g data from a CS
+000000a0: 5620 6669 6c65 2e20 2049 7427 7320 7573  V file.  It's us
+000000b0: 6566 756c 2077 6865 6e20 796f 7520 6e65  eful when you ne
+000000c0: 6564 2074 6f20 6d6f 7665 2064 6174 6120  ed to move data 
+000000d0: 6265 7477 6565 6e20 6469 7363 6f6e 6e65  between disconne
+000000e0: 6374 6564 2064 6174 6162 6173 6573 2061  cted databases a
+000000f0: 6e64 2064 6174 6120 7761 7265 686f 7573  nd data warehous
+00000100: 6573 2e20 2059 6f75 2063 616e 206e 6f77  es.  You can now
+00000110: 2073 696d 706c 7920 756e 6c6f 6164 2061   simply unload a
+00000120: 2043 5356 2c20 7475 726e 2074 6861 7420   CSV, turn that 
+00000130: 4353 5620 696e 746f 2053 514c 2073 7461  CSV into SQL sta
+00000140: 7465 6d65 6e74 7320 6372 6561 7469 6e67  tements creating
+00000150: 2061 2074 656d 7020 7461 626c 6520 616e   a temp table an
+00000160: 6420 696e 7365 7274 696e 6720 6461 7461  d inserting data
+00000170: 2077 6974 6820 6120 434c 4920 636f 6d6d   with a CLI comm
+00000180: 616e 642c 2061 6e64 2063 6f70 7920 7468  and, and copy th
+00000190: 6f73 6520 5351 4c20 7374 6174 656d 656e  ose SQL statemen
+000001a0: 7473 2069 6e74 6f20 796f 7572 2071 7565  ts into your que
+000001b0: 7279 2065 6469 746f 7220 736f 2079 6f75  ry editor so you
+000001c0: 2063 616e 2073 7461 7274 2075 7369 6e67   can start using
+000001d0: 2074 6865 2064 6174 6120 696e 2061 2064   the data in a d
+000001e0: 6966 6665 7265 6e74 2077 6172 6568 6f75  ifferent warehou
+000001f0: 7365 2e0a 0a3c 623e 5768 7920 6469 6420  se...<b>Why did 
+00000200: 4920 6275 696c 6420 7468 6973 3f3c 2f62  I build this?</b
+00000210: 3e20 2049 276d 206f 6674 656e 2077 6f6e  >  I'm often won
+00000220: 6465 7269 6e67 2068 6f77 2061 2070 726f  dering how a pro
+00000230: 6475 6374 2049 276d 2077 6f72 6b69 6e67  duct I'm working
+00000240: 206f 6e20 6973 206c 696e 6b65 6420 746f   on is linked to
+00000250: 2063 7573 746f 6d65 7220 7370 656e 642e   customer spend.
+00000260: 2020 486f 7765 7665 722c 206d 7920 6f70    However, my op
+00000270: 6572 6174 696f 6e61 6c20 7761 7265 686f  erational wareho
+00000280: 7573 6520 7468 6174 2069 6e63 6c75 6465  use that include
+00000290: 7320 6461 7461 206c 696b 6520 7468 6520  s data like the 
+000002a0: 6461 7465 7320 616e 6420 7469 6d65 7320  dates and times 
+000002b0: 6375 7374 6f6d 6572 7320 7573 6564 2061  customers used a
+000002c0: 2070 726f 6475 6374 2069 7320 7365 7061   product is sepa
+000002d0: 7261 7465 2066 726f 6d20 6d79 2066 696e  rate from my fin
+000002e0: 616e 6369 616c 2077 6172 6568 6f75 7365  ancial warehouse
+000002f0: 2077 6869 6368 2068 6173 2074 6865 2062   which has the b
+00000300: 696c 6c69 6e67 2064 6174 612e 2020 4920  illing data.  I 
+00000310: 6e65 6564 2074 6f20 6d6f 7665 2064 6174  need to move dat
+00000320: 6120 6672 6f6d 206f 6e65 2074 6f20 7468  a from one to th
+00000330: 6520 6f74 6865 7220 736f 2049 2063 616e  e other so I can
+00000340: 206a 6f69 6e20 7468 6520 6669 6e61 6e63   join the financ
+00000350: 6520 616e 6420 7072 6f64 7563 7420 6461  e and product da
+00000360: 7461 2074 6f67 6574 6865 7220 746f 2064  ta together to d
+00000370: 6f20 616e 2061 6e61 6c79 7369 732e 2e2e  o an analysis...
+00000380: 616e 6420 7475 726e 696e 6720 7468 6520  and turning the 
+00000390: 4353 5620 696e 746f 2053 514c 2062 7920  CSV into SQL by 
+000003a0: 6861 6e64 2069 6e20 6578 6365 6c20 6973  hand in excel is
+000003b0: 2061 2050 4954 412e 2020 5769 7468 2074   a PITA.  With t
+000003c0: 6869 732c 2049 2063 616e 206e 6f77 206d  his, I can now m
+000003d0: 6f76 6520 7468 6520 6461 7461 2069 6e20  ove the data in 
+000003e0: 7365 636f 6e64 732e 2020 4920 7369 6d70  seconds.  I simp
+000003f0: 6c79 2064 6f77 6e6c 6f61 6420 7468 6520  ly download the 
+00000400: 4353 562c 2072 756e 203c 636f 6465 3e67  CSV, run <code>g
+00000410: 656e 6572 6174 652d 7474 2d73 716c 2063  enerate-tt-sql c
+00000420: 7376 5f6e 616d 652e 6373 763c 2f63 6f64  sv_name.csv</cod
+00000430: 653e 2069 6e20 6d79 2074 6572 6d69 6e61  e> in my termina
+00000440: 6c2c 2061 6e64 2063 6f70 7920 6974 2069  l, and copy it i
+00000450: 6e74 6f20 6d79 2071 7565 7279 2065 6469  nto my query edi
+00000460: 746f 722e 2020 4974 2773 2069 6d6d 6564  tor.  It's immed
+00000470: 6961 7465 6c79 2061 7661 696c 6162 6c65  iately available
+00000480: 2074 6f20 7175 6572 7920 736f 2049 2063   to query so I c
+00000490: 616e 2067 6f20 7374 7261 6967 6874 2074  an go straight t
+000004a0: 6f20 616e 616c 7973 6973 2e0a 0a23 2320  o analysis...## 
+000004b0: 4665 6174 7572 6573 0a0a 2d20 4c6f 6164  Features..- Load
+000004c0: 2064 6174 6120 6672 6f6d 2061 2043 5356   data from a CSV
+000004d0: 2066 696c 650a 2d20 4765 6e65 7261 7465   file.- Generate
+000004e0: 2061 2060 4352 4541 5445 2054 454d 5020   a `CREATE TEMP 
+000004f0: 5441 424c 4560 2053 514c 2073 7461 7465  TABLE` SQL state
+00000500: 6d65 6e74 0a2d 2047 656e 6572 6174 6520  ment.- Generate 
+00000510: 6049 4e53 4552 5420 494e 544f 6020 5351  `INSERT INTO` SQ
+00000520: 4c20 7374 6174 656d 656e 7473 2066 6f72  L statements for
+00000530: 2074 6865 2064 6174 610a 2d20 436f 6d6d   the data.- Comm
+00000540: 616e 642d 6c69 6e65 2069 6e74 6572 6661  and-line interfa
+00000550: 6365 2028 434c 4929 2066 6f72 2065 6173  ce (CLI) for eas
+00000560: 7920 7573 6167 650a 0a23 2320 496e 7374  y usage..## Inst
+00000570: 616c 6c61 7469 6f6e 0a0a 2323 2320 5072  allation..### Pr
+00000580: 6572 6571 7569 7369 7465 730a 0a2d 2050  erequisites..- P
+00000590: 7974 686f 6e20 332e 3620 6f72 2068 6967  ython 3.6 or hig
+000005a0: 6865 720a 2d20 6070 616e 6461 7360 206c  her.- `pandas` l
+000005b0: 6962 7261 7279 0a0a 2323 2320 496e 7374  ibrary..### Inst
+000005c0: 616c 6c69 6e67 0a0a 312e 2043 6c6f 6e65  alling..1. Clone
+000005d0: 2074 6865 2072 6570 6f73 6974 6f72 793a   the repository:
+000005e0: 0a20 2020 2060 6060 7368 0a20 2020 2067  .    ```sh.    g
+000005f0: 6974 2063 6c6f 6e65 2068 7474 7073 3a2f  it clone https:/
+00000600: 2f67 6974 6875 622e 636f 6d2f 7279 7761  /github.com/rywa
+00000610: 6c64 6f72 2f67 656e 6572 6174 655f 7465  ldor/generate_te
+00000620: 6d70 5f74 6162 6c65 5f73 716c 2e67 6974  mp_table_sql.git
+00000630: 0a20 2020 2063 6420 6765 6e65 7261 7465  .    cd generate
+00000640: 5f74 656d 705f 7461 626c 655f 7371 6c0a  _temp_table_sql.
+00000650: 2020 2020 6060 600a 0a32 2e20 496e 7374      ```..2. Inst
+00000660: 616c 6c20 7468 6520 7061 636b 6167 6520  all the package 
+00000670: 6c6f 6361 6c6c 793a 0a20 2020 2060 6060  locally:.    ```
+00000680: 7368 0a20 2020 2070 6970 2069 6e73 7461  sh.    pip insta
+00000690: 6c6c 202d 6520 2e0a 2020 2020 6060 600a  ll -e ..    ```.
+000006a0: 0a23 2320 5573 6167 650a 0a23 2323 2043  .## Usage..### C
+000006b0: 6f6d 6d61 6e64 2d4c 696e 6520 496e 7465  ommand-Line Inte
+000006c0: 7266 6163 6520 2843 4c49 290a 0a41 6674  rface (CLI)..Aft
+000006d0: 6572 2069 6e73 7461 6c6c 696e 6720 7468  er installing th
+000006e0: 6520 7061 636b 6167 652c 2079 6f75 2063  e package, you c
+000006f0: 616e 2075 7365 2074 6865 2060 6765 6e65  an use the `gene
+00000700: 7261 7465 2d74 742d 7371 6c60 2063 6f6d  rate-tt-sql` com
+00000710: 6d61 6e64 2074 6f20 6765 6e65 7261 7465  mand to generate
+00000720: 2053 514c 2073 7461 7465 6d65 6e74 7320   SQL statements 
+00000730: 6672 6f6d 2061 2043 5356 2066 696c 652e  from a CSV file.
+00000740: 0a0a 2323 2323 2042 6173 6963 2055 7361  ..#### Basic Usa
+00000750: 6765 0a0a 546f 2067 656e 6572 6174 6520  ge..To generate 
+00000760: 5351 4c20 7374 6174 656d 656e 7473 2061  SQL statements a
+00000770: 6e64 2073 6176 6520 7468 656d 2074 6f20  nd save them to 
+00000780: 6120 6669 6c65 3a0a 6060 6073 680a 6765  a file:.```sh.ge
+00000790: 6e65 7261 7465 2d74 742d 7371 6c20 7061  nerate-tt-sql pa
+000007a0: 7468 2f74 6f2f 796f 7572 2f66 696c 652e  th/to/your/file.
+000007b0: 6373 760a 6060 600a 0a23 2323 2320 4164  csv.```..#### Ad
+000007c0: 6469 7469 6f6e 616c 204f 7074 696f 6e73  ditional Options
+000007d0: 0a60 6060 7368 0a0a 2d2d 6f20 5468 6520  .```sh..--o The 
+000007e0: 7061 7468 2074 6f20 7468 6520 6f75 7470  path to the outp
+000007f0: 7574 2053 514c 2066 696c 652e 2020 4465  ut SQL file.  De
+00000800: 6661 756c 7473 2074 6f20 7468 6520 6469  faults to the di
+00000810: 7265 6374 6f72 2079 6f75 2063 616c 6c20  rector you call 
+00000820: 7468 6520 636f 6d6d 616e 6420 696e 2e0a  the command in..
+00000830: 2d2d 6f76 6572 7772 6974 653a 2041 6c6c  --overwrite: All
+00000840: 6f77 206f 7665 7277 7269 7469 6e67 2074  ow overwriting t
+00000850: 6865 206f 7574 7075 7420 6669 6c65 2069  he output file i
+00000860: 6620 6974 2065 7869 7374 732e 0a2d 2d74  f it exists..--t
+00000870: 6162 6c65 5f6e 616d 653a 2053 7065 6369  able_name: Speci
+00000880: 6679 2074 6865 206e 616d 6520 6f66 2074  fy the name of t
+00000890: 6865 2074 656d 706f 7261 7279 2074 6162  he temporary tab
+000008a0: 6c65 2074 6f20 6372 6561 7465 2e0a 2d2d  le to create..--
+000008b0: 636f 6c75 6d6e 5f74 7970 653a 2053 7065  column_type: Spe
+000008c0: 6369 6679 2074 6865 2064 6174 6120 7479  cify the data ty
+000008d0: 7065 206f 6620 7468 6520 636f 6c75 6d6e  pe of the column
+000008e0: 7320 696e 2074 6865 2074 656d 706f 7261  s in the tempora
+000008f0: 7279 2074 6162 6c65 2e20 4465 6661 756c  ry table. Defaul
+00000900: 7473 2074 6f20 5445 5854 2077 6869 6368  ts to TEXT which
+00000910: 2077 6f72 6b73 2066 6f72 2052 6564 7368   works for Redsh
+00000920: 6966 7420 616e 6420 536e 6f77 666c 616b  ift and Snowflak
+00000930: 652e 2055 7365 2053 5452 494e 4720 666f  e. Use STRING fo
+00000940: 7220 4269 6751 7565 7279 2e0a 6060 600a  r BigQuery..```.
+00000950: 0a23 2323 2320 4578 616d 706c 650a 4173  .#### Example.As
+00000960: 7375 6d65 2079 6f75 2068 6176 6520 6120  sume you have a 
+00000970: 4353 5620 6669 6c65 2065 7861 6d70 6c65  CSV file example
+00000980: 2e63 7376 2077 6974 6820 7468 6520 666f  .csv with the fo
+00000990: 6c6c 6f77 696e 6720 636f 6e74 656e 743a  llowing content:
+000009a0: 0a0a 6060 6073 680a 6e61 6d65 2c61 6765  ..```sh.name,age
+000009b0: 2c63 6974 790a 4a6f 686e 2c33 302c 4e65  ,city.John,30,Ne
+000009c0: 7720 596f 726b 0a4a 616e 652c 3235 2c4c  w York.Jane,25,L
+000009d0: 6f73 2041 6e67 656c 6573 0a60 6060 0a0a  os Angeles.```..
+000009e0: 5275 6e20 7468 6520 666f 6c6c 6f77 696e  Run the followin
+000009f0: 6720 636f 6d6d 616e 6420 746f 2067 656e  g command to gen
+00000a00: 6572 6174 6520 5351 4c20 7374 6174 656d  erate SQL statem
+00000a10: 656e 7473 3a0a 0a60 6060 7368 0a67 656e  ents:..```sh.gen
+00000a20: 6572 6174 652d 7474 2d73 716c 2065 7861  erate-tt-sql exa
+00000a30: 6d70 6c65 2e63 7376 202d 6f20 6f75 7470  mple.csv -o outp
+00000a40: 7574 2e73 716c 202d 2d74 6162 6c65 5f6e  ut.sql --table_n
+00000a50: 616d 6520 6d79 5f74 656d 705f 7461 626c  ame my_temp_tabl
+00000a60: 6520 2d2d 636f 6c75 6d6e 5f74 7970 6520  e --column_type 
+00000a70: 5354 5249 4e47 0a60 6060 0a0a 5468 6520  STRING.```..The 
+00000a80: 6f75 7470 7574 2e73 716c 2066 696c 6520  output.sql file 
+00000a90: 7769 6c6c 2063 6f6e 7461 696e 3a0a 0a60  will contain:..`
+00000aa0: 6060 7368 0a43 5245 4154 4520 5445 4d50  ``sh.CREATE TEMP
+00000ab0: 2054 4142 4c45 206d 795f 7465 6d70 5f74   TABLE my_temp_t
+00000ac0: 6162 6c65 2028 0a20 2020 206e 616d 6520  able (.    name 
+00000ad0: 5354 5249 4e47 2c0a 2020 2020 6167 6520  STRING,.    age 
+00000ae0: 5354 5249 4e47 2c0a 2020 2020 6369 7479  STRING,.    city
+00000af0: 2053 5452 494e 470a 293b 0a0a 2d2d 496e   STRING.);..--In
+00000b00: 7365 7274 2044 6174 6120 5351 4c3a 0a49  sert Data SQL:.I
+00000b10: 4e53 4552 5420 494e 544f 206d 795f 7465  NSERT INTO my_te
+00000b20: 6d70 5f74 6162 6c65 2028 6e61 6d65 2c20  mp_table (name, 
+00000b30: 6167 652c 2063 6974 7929 2056 414c 5545  age, city) VALUE
+00000b40: 5320 0a20 2020 2028 274a 6f68 6e27 2c20  S .    ('John', 
+00000b50: 2733 3027 2c20 274e 6577 2059 6f72 6b27  '30', 'New York'
+00000b60: 292c 0a20 2020 2028 274a 616e 6527 2c20  ),.    ('Jane', 
+00000b70: 2732 3527 2c20 274c 6f73 2041 6e67 656c  '25', 'Los Angel
+00000b80: 6573 2729 3b0a 6060 600a 0a23 2323 2320  es');.```..#### 
+00000b90: 5275 6e6e 696e 6720 5465 7374 730a 546f  Running Tests.To
+00000ba0: 2072 756e 2074 6865 2074 6573 7473 2c20   run the tests, 
+00000bb0: 7573 6520 7468 6520 666f 6c6c 6f77 696e  use the followin
+00000bc0: 6720 636f 6d6d 616e 643a 0a0a 6060 6073  g command:..```s
+00000bd0: 680a 7079 7468 6f6e 202d 6d20 756e 6974  h.python -m unit
+00000be0: 7465 7374 2064 6973 636f 7665 7220 2d73  test discover -s
+00000bf0: 2074 6573 7473 0a60 6060 0a0a 2323 2323   tests.```..####
+00000c00: 2043 6f6e 7472 6962 7574 696e 670a 436f   Contributing.Co
+00000c10: 6e74 7269 6275 7469 6f6e 7320 6172 6520  ntributions are 
+00000c20: 7765 6c63 6f6d 6521 2050 6c65 6173 6520  welcome! Please 
+00000c30: 666f 6c6c 6f77 2074 6865 7365 2073 7465  follow these ste
+00000c40: 7073 3a0a 0a31 2e20 466f 726b 2074 6865  ps:..1. Fork the
+00000c50: 2072 6570 6f73 6974 6f72 790a 322e 2043   repository.2. C
+00000c60: 7265 6174 6520 6120 6e65 7720 6272 616e  reate a new bran
+00000c70: 6368 2028 6769 7420 6368 6563 6b6f 7574  ch (git checkout
+00000c80: 202d 6220 6665 6174 7572 652d 6272 616e   -b feature-bran
+00000c90: 6368 290a 332e 2043 6f6d 6d69 7420 796f  ch).3. Commit yo
+00000ca0: 7572 2063 6861 6e67 6573 2028 6769 7420  ur changes (git 
+00000cb0: 636f 6d6d 6974 202d 616d 2027 4164 6420  commit -am 'Add 
+00000cc0: 6e65 7720 6665 6174 7572 6527 290a 342e  new feature').4.
+00000cd0: 2050 7573 6820 746f 2074 6865 2062 7261   Push to the bra
+00000ce0: 6e63 6820 2867 6974 2070 7573 6820 6f72  nch (git push or
+00000cf0: 6967 696e 2066 6561 7475 7265 2d62 7261  igin feature-bra
+00000d00: 6e63 6829 0a35 2e20 4372 6561 7465 2061  nch).5. Create a
+00000d10: 206e 6577 2050 756c 6c20 5265 7175 6573   new Pull Reques
+00000d20: 740a 0a23 2323 2320 4c69 6365 6e73 650a  t..#### License.
+00000d30: 5468 6973 2070 726f 6a65 6374 2069 7320  This project is 
+00000d40: 6c69 6365 6e73 6564 2075 6e64 6572 2074  licensed under t
+00000d50: 6865 204d 4954 204c 6963 656e 7365 202d  he MIT License -
+00000d60: 2073 6565 2074 6865 204c 4943 454e 5345   see the LICENSE
+00000d70: 2066 696c 6520 666f 7220 6465 7461 696c   file for detail
+00000d80: 732e 0a0a 2323 2323 2041 7574 686f 720a  s...#### Author.
+00000d90: 5279 616e 2057 616c 646f 7266 202d 2072  Ryan Waldorf - r
+00000da0: 7961 6e40 7279 616e 7761 6c64 6f72 662e  yan@ryanwaldorf.
+00000db0: 636f 6d3c 6272 2f3e 0a3c 6120 6872 6566  com<br/>.<a href
+00000dc0: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
+00000dd0: 2e63 6f6d 2f72 7961 6e77 616c 646f 7266  .com/ryanwaldorf
+00000de0: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
+00000df0: 223e 4769 7448 7562 3c2f 613e 0a3c 6120  ">GitHub</a>.<a 
+00000e00: 6872 6566 3d22 6874 7470 733a 2f2f 7777  href="https://ww
+00000e10: 772e 6c69 6e6b 6564 696e 2e63 6f6d 2f69  w.linkedin.com/i
+00000e20: 6e2f 7279 616e 2d77 616c 646f 7266 2f22  n/ryan-waldorf/"
+00000e30: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
+00000e40: 3e4c 696e 6b65 6449 6e3c 2f61 3e         >LinkedIn</a>
```

### Comparing `generate_temp_table_sql-0.4.2/generate_temp_table_sql/cli.py` & `generate_temp_table_sql-0.4.3/generate_temp_table_sql/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 def main():
     parser = argparse.ArgumentParser(description='Process a CSV file to generate SQL statements.')
     parser.add_argument('csv_file', type=str, help='The path to the CSV file')
     parser.add_argument('-o', '--output_file', type=str, help='The path to the output SQL file.  Defaults to the director you call the command in.')
     parser.add_argument('--overwrite', action='store_true', help='Allow overwriting the output file if it exists')
     parser.add_argument('--table_name', type=str, help='The name of the temp table you will create')
     parser.add_argument('--column_type', type=str, help='The data type of the columns in the temp table.  Defaults to TEXT which works for Redshift and Snowflake.  BigQuery requires STRING.')
-    parser.add_argument('--batch_size', type=int, help='The number of rows inserted per insert statement.  If present, it creates multiple insert statements based on the batch size specified.')
+    parser.add_argument('--batch_size', type=int, help='Specify the number of rows inserted per insert statement.  If present, it creates multiple insert statements based on the batch size specified.')
 
     args = parser.parse_args()
     
     # Use specified output file name or generate a default one
     if args.output_file is None:
         base_name = os.path.splitext(os.path.basename(args.csv_file))[0]
         args.output_file = os.path.join(os.getcwd(), base_name + '_temp_table.sql')
```

### Comparing `generate_temp_table_sql-0.4.2/generate_temp_table_sql/sql_generator.py` & `generate_temp_table_sql-0.4.3/generate_temp_table_sql/sql_generator.py`

 * *Files identical despite different names*

### Comparing `generate_temp_table_sql-0.4.2/generate_temp_table_sql.egg-info/PKG-INFO` & `generate_temp_table_sql-0.4.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6765 6e65  : 2.1.Name: gene
-00000020: 7261 7465 2d74 656d 702d 7461 626c 652d  rate-temp-table-
+00000020: 7261 7465 5f74 656d 705f 7461 626c 655f  rate_temp_table_
 00000030: 7371 6c0a 5665 7273 696f 6e3a 2030 2e34  sql.Version: 0.4
-00000040: 2e32 0a53 756d 6d61 7279 3a20 4120 7061  .2.Summary: A pa
+00000040: 2e33 0a53 756d 6d61 7279 3a20 4120 7061  .3.Summary: A pa
 00000050: 636b 6167 6520 746f 2067 656e 6572 6174  ckage to generat
 00000060: 6520 5351 4c20 7374 6174 656d 656e 7473  e SQL statements
 00000070: 2066 726f 6d20 4353 5620 6669 6c65 730a   from CSV files.
 00000080: 486f 6d65 2d70 6167 653a 2068 7474 7073  Home-page: https
 00000090: 3a2f 2f67 6974 6875 622e 636f 6d2f 7279  ://github.com/ry
 000000a0: 616e 7761 6c64 6f72 662f 6765 6e65 7261  anwaldorf/genera
 000000b0: 7465 5f74 656d 705f 7461 626c 655f 7371  te_temp_table_sq
@@ -40,162 +40,223 @@
 00000270: 7220 6372 6561 7469 6e67 2061 2074 656d  r creating a tem
 00000280: 706f 7261 7279 2074 6162 6c65 2061 6e64  porary table and
 00000290: 2069 6e73 6572 7469 6e67 2064 6174 6120   inserting data 
 000002a0: 6672 6f6d 2061 2043 5356 2066 696c 652e  from a CSV file.
 000002b0: 2020 4974 2773 2075 7365 6675 6c20 7768    It's useful wh
 000002c0: 656e 2079 6f75 206e 6565 6420 746f 206d  en you need to m
 000002d0: 6f76 6520 6461 7461 2062 6574 7765 656e  ove data between
-000002e0: 2064 6174 6120 7761 7265 686f 7573 6573   data warehouses
-000002f0: 2074 6861 7420 6172 6520 6f74 6865 7277   that are otherw
-00000300: 6973 6520 6e6f 7420 636f 6e6e 6563 7465  ise not connecte
-00000310: 642c 2073 6f20 796f 7520 6361 6e20 646f  d, so you can do
-00000320: 776e 6c6f 6164 2061 2043 5356 2061 6e64  wnload a CSV and
-00000330: 2072 6563 7265 6174 6520 7468 6520 6461   recreate the da
-00000340: 7461 2069 6e20 7468 6520 6f74 6865 7220  ta in the other 
-00000350: 7761 7265 686f 7573 6520 6173 2061 2074  warehouse as a t
-00000360: 656d 706f 7261 7279 2074 6162 6c65 2066  emporary table f
-00000370: 726f 6d20 7468 6520 4353 562e 0a0a 2323  rom the CSV...##
-00000380: 2046 6561 7475 7265 730a 0a2d 204c 6f61   Features..- Loa
-00000390: 6420 6461 7461 2066 726f 6d20 6120 4353  d data from a CS
-000003a0: 5620 6669 6c65 0a2d 2047 656e 6572 6174  V file.- Generat
-000003b0: 6520 6120 6043 5245 4154 4520 5445 4d50  e a `CREATE TEMP
-000003c0: 2054 4142 4c45 6020 5351 4c20 7374 6174   TABLE` SQL stat
-000003d0: 656d 656e 740a 2d20 4765 6e65 7261 7465  ement.- Generate
-000003e0: 2060 494e 5345 5254 2049 4e54 4f60 2053   `INSERT INTO` S
-000003f0: 514c 2073 7461 7465 6d65 6e74 7320 666f  QL statements fo
-00000400: 7220 7468 6520 6461 7461 0a2d 2043 6f6d  r the data.- Com
-00000410: 6d61 6e64 2d6c 696e 6520 696e 7465 7266  mand-line interf
-00000420: 6163 6520 2843 4c49 2920 666f 7220 6561  ace (CLI) for ea
-00000430: 7379 2075 7361 6765 0a0a 2323 2049 6e73  sy usage..## Ins
-00000440: 7461 6c6c 6174 696f 6e0a 0a23 2323 2050  tallation..### P
-00000450: 7265 7265 7175 6973 6974 6573 0a0a 2d20  rerequisites..- 
-00000460: 5079 7468 6f6e 2033 2e36 206f 7220 6869  Python 3.6 or hi
-00000470: 6768 6572 0a2d 2060 7061 6e64 6173 6020  gher.- `pandas` 
-00000480: 6c69 6272 6172 790a 0a23 2323 2049 6e73  library..### Ins
-00000490: 7461 6c6c 696e 670a 0a31 2e20 436c 6f6e  talling..1. Clon
-000004a0: 6520 7468 6520 7265 706f 7369 746f 7279  e the repository
-000004b0: 3a0a 2020 2020 6060 6073 680a 2020 2020  :.    ```sh.    
-000004c0: 6769 7420 636c 6f6e 6520 6874 7470 733a  git clone https:
-000004d0: 2f2f 6769 7468 7562 2e63 6f6d 2f72 7977  //github.com/ryw
-000004e0: 616c 646f 722f 6765 6e65 7261 7465 5f74  aldor/generate_t
-000004f0: 656d 705f 7461 626c 655f 7371 6c2e 6769  emp_table_sql.gi
-00000500: 740a 2020 2020 6364 2067 656e 6572 6174  t.    cd generat
-00000510: 655f 7465 6d70 5f74 6162 6c65 5f73 716c  e_temp_table_sql
-00000520: 0a20 2020 2060 6060 0a0a 322e 2049 6e73  .    ```..2. Ins
-00000530: 7461 6c6c 2074 6865 2070 6163 6b61 6765  tall the package
-00000540: 206c 6f63 616c 6c79 3a0a 2020 2020 6060   locally:.    ``
-00000550: 6073 680a 2020 2020 7069 7020 696e 7374  `sh.    pip inst
-00000560: 616c 6c20 2d65 202e 0a20 2020 2060 6060  all -e ..    ```
-00000570: 0a0a 2323 2055 7361 6765 0a0a 2323 2320  ..## Usage..### 
-00000580: 436f 6d6d 616e 642d 4c69 6e65 2049 6e74  Command-Line Int
-00000590: 6572 6661 6365 2028 434c 4929 0a0a 4166  erface (CLI)..Af
-000005a0: 7465 7220 696e 7374 616c 6c69 6e67 2074  ter installing t
-000005b0: 6865 2070 6163 6b61 6765 2c20 796f 7520  he package, you 
-000005c0: 6361 6e20 7573 6520 7468 6520 6067 656e  can use the `gen
-000005d0: 6572 6174 652d 7474 2d73 716c 6020 636f  erate-tt-sql` co
-000005e0: 6d6d 616e 6420 746f 2067 656e 6572 6174  mmand to generat
-000005f0: 6520 5351 4c20 7374 6174 656d 656e 7473  e SQL statements
-00000600: 2066 726f 6d20 6120 4353 5620 6669 6c65   from a CSV file
-00000610: 2e0a 0a23 2323 2320 4261 7369 6320 5573  ...#### Basic Us
-00000620: 6167 650a 0a54 6f20 6765 6e65 7261 7465  age..To generate
-00000630: 2053 514c 2073 7461 7465 6d65 6e74 7320   SQL statements 
-00000640: 616e 6420 7361 7665 2074 6865 6d20 746f  and save them to
-00000650: 2061 2066 696c 653a 0a60 6060 7368 0a67   a file:.```sh.g
-00000660: 656e 6572 6174 652d 7474 2d73 716c 2070  enerate-tt-sql p
-00000670: 6174 682f 746f 2f79 6f75 722f 6669 6c65  ath/to/your/file
-00000680: 2e63 7376 0a60 6060 0a0a 2323 2323 2041  .csv.```..#### A
-00000690: 6464 6974 696f 6e61 6c20 4f70 7469 6f6e  dditional Option
-000006a0: 730a 6060 6073 680a 0a2d 2d6f 2054 6865  s.```sh..--o The
-000006b0: 2070 6174 6820 746f 2074 6865 206f 7574   path to the out
-000006c0: 7075 7420 5351 4c20 6669 6c65 2e20 2044  put SQL file.  D
-000006d0: 6566 6175 6c74 7320 746f 2074 6865 2064  efaults to the d
-000006e0: 6972 6563 746f 7220 796f 7520 6361 6c6c  irector you call
-000006f0: 2074 6865 2063 6f6d 6d61 6e64 2069 6e2e   the command in.
-00000700: 0a2d 2d6f 7665 7277 7269 7465 3a20 416c  .--overwrite: Al
-00000710: 6c6f 7720 6f76 6572 7772 6974 696e 6720  low overwriting 
-00000720: 7468 6520 6f75 7470 7574 2066 696c 6520  the output file 
-00000730: 6966 2069 7420 6578 6973 7473 2e0a 2d2d  if it exists..--
-00000740: 7461 626c 655f 6e61 6d65 3a20 5370 6563  table_name: Spec
-00000750: 6966 7920 7468 6520 6e61 6d65 206f 6620  ify the name of 
-00000760: 7468 6520 7465 6d70 6f72 6172 7920 7461  the temporary ta
-00000770: 626c 6520 746f 2063 7265 6174 652e 0a2d  ble to create..-
-00000780: 2d63 6f6c 756d 6e5f 7479 7065 3a20 5370  -column_type: Sp
-00000790: 6563 6966 7920 7468 6520 6461 7461 2074  ecify the data t
-000007a0: 7970 6520 6f66 2074 6865 2063 6f6c 756d  ype of the colum
-000007b0: 6e73 2069 6e20 7468 6520 7465 6d70 6f72  ns in the tempor
-000007c0: 6172 7920 7461 626c 652e 2044 6566 6175  ary table. Defau
-000007d0: 6c74 7320 746f 2054 4558 5420 7768 6963  lts to TEXT whic
-000007e0: 6820 776f 726b 7320 666f 7220 5265 6473  h works for Reds
-000007f0: 6869 6674 2061 6e64 2053 6e6f 7766 6c61  hift and Snowfla
-00000800: 6b65 2e20 5573 6520 5354 5249 4e47 2066  ke. Use STRING f
-00000810: 6f72 2042 6967 5175 6572 792e 0a60 6060  or BigQuery..```
-00000820: 0a0a 2323 2323 2045 7861 6d70 6c65 0a41  ..#### Example.A
-00000830: 7373 756d 6520 796f 7520 6861 7665 2061  ssume you have a
-00000840: 2043 5356 2066 696c 6520 6578 616d 706c   CSV file exampl
-00000850: 652e 6373 7620 7769 7468 2074 6865 2066  e.csv with the f
-00000860: 6f6c 6c6f 7769 6e67 2063 6f6e 7465 6e74  ollowing content
-00000870: 3a0a 0a60 6060 7368 0a6e 616d 652c 6167  :..```sh.name,ag
-00000880: 652c 6369 7479 0a4a 6f68 6e2c 3330 2c4e  e,city.John,30,N
-00000890: 6577 2059 6f72 6b0a 4a61 6e65 2c32 352c  ew York.Jane,25,
-000008a0: 4c6f 7320 416e 6765 6c65 730a 6060 600a  Los Angeles.```.
-000008b0: 0a52 756e 2074 6865 2066 6f6c 6c6f 7769  .Run the followi
-000008c0: 6e67 2063 6f6d 6d61 6e64 2074 6f20 6765  ng command to ge
-000008d0: 6e65 7261 7465 2053 514c 2073 7461 7465  nerate SQL state
-000008e0: 6d65 6e74 733a 0a0a 6060 6073 680a 6765  ments:..```sh.ge
-000008f0: 6e65 7261 7465 2d74 742d 7371 6c20 6578  nerate-tt-sql ex
-00000900: 616d 706c 652e 6373 7620 2d6f 206f 7574  ample.csv -o out
-00000910: 7075 742e 7371 6c20 2d2d 7461 626c 655f  put.sql --table_
-00000920: 6e61 6d65 206d 795f 7465 6d70 5f74 6162  name my_temp_tab
-00000930: 6c65 202d 2d63 6f6c 756d 6e5f 7479 7065  le --column_type
-00000940: 2053 5452 494e 470a 6060 600a 0a54 6865   STRING.```..The
-00000950: 206f 7574 7075 742e 7371 6c20 6669 6c65   output.sql file
-00000960: 2077 696c 6c20 636f 6e74 6169 6e3a 0a0a   will contain:..
-00000970: 6060 6073 680a 4352 4541 5445 2054 454d  ```sh.CREATE TEM
-00000980: 5020 5441 424c 4520 6d79 5f74 656d 705f  P TABLE my_temp_
-00000990: 7461 626c 6520 280a 2020 2020 6e61 6d65  table (.    name
-000009a0: 2053 5452 494e 472c 0a20 2020 2061 6765   STRING,.    age
-000009b0: 2053 5452 494e 472c 0a20 2020 2063 6974   STRING,.    cit
-000009c0: 7920 5354 5249 4e47 0a29 3b0a 0a2d 2d49  y STRING.);..--I
-000009d0: 6e73 6572 7420 4461 7461 2053 514c 3a0a  nsert Data SQL:.
-000009e0: 494e 5345 5254 2049 4e54 4f20 6d79 5f74  INSERT INTO my_t
-000009f0: 656d 705f 7461 626c 6520 286e 616d 652c  emp_table (name,
-00000a00: 2061 6765 2c20 6369 7479 2920 5641 4c55   age, city) VALU
-00000a10: 4553 200a 2020 2020 2827 4a6f 686e 272c  ES .    ('John',
-00000a20: 2027 3330 272c 2027 4e65 7720 596f 726b   '30', 'New York
-00000a30: 2729 2c0a 2020 2020 2827 4a61 6e65 272c  '),.    ('Jane',
-00000a40: 2027 3235 272c 2027 4c6f 7320 416e 6765   '25', 'Los Ange
-00000a50: 6c65 7327 293b 0a60 6060 0a0a 2323 2323  les');.```..####
-00000a60: 2052 756e 6e69 6e67 2054 6573 7473 0a54   Running Tests.T
-00000a70: 6f20 7275 6e20 7468 6520 7465 7374 732c  o run the tests,
-00000a80: 2075 7365 2074 6865 2066 6f6c 6c6f 7769   use the followi
-00000a90: 6e67 2063 6f6d 6d61 6e64 3a0a 0a60 6060  ng command:..```
-00000aa0: 7368 0a70 7974 686f 6e20 2d6d 2075 6e69  sh.python -m uni
-00000ab0: 7474 6573 7420 6469 7363 6f76 6572 202d  ttest discover -
-00000ac0: 7320 7465 7374 730a 6060 600a 0a23 2323  s tests.```..###
-00000ad0: 2320 436f 6e74 7269 6275 7469 6e67 0a43  # Contributing.C
-00000ae0: 6f6e 7472 6962 7574 696f 6e73 2061 7265  ontributions are
-00000af0: 2077 656c 636f 6d65 2120 506c 6561 7365   welcome! Please
-00000b00: 2066 6f6c 6c6f 7720 7468 6573 6520 7374   follow these st
-00000b10: 6570 733a 0a0a 312e 2046 6f72 6b20 7468  eps:..1. Fork th
-00000b20: 6520 7265 706f 7369 746f 7279 0a32 2e20  e repository.2. 
-00000b30: 4372 6561 7465 2061 206e 6577 2062 7261  Create a new bra
-00000b40: 6e63 6820 2867 6974 2063 6865 636b 6f75  nch (git checkou
-00000b50: 7420 2d62 2066 6561 7475 7265 2d62 7261  t -b feature-bra
-00000b60: 6e63 6829 0a33 2e20 436f 6d6d 6974 2079  nch).3. Commit y
-00000b70: 6f75 7220 6368 616e 6765 7320 2867 6974  our changes (git
-00000b80: 2063 6f6d 6d69 7420 2d61 6d20 2741 6464   commit -am 'Add
-00000b90: 206e 6577 2066 6561 7475 7265 2729 0a34   new feature').4
-00000ba0: 2e20 5075 7368 2074 6f20 7468 6520 6272  . Push to the br
-00000bb0: 616e 6368 2028 6769 7420 7075 7368 206f  anch (git push o
-00000bc0: 7269 6769 6e20 6665 6174 7572 652d 6272  rigin feature-br
-00000bd0: 616e 6368 290a 352e 2043 7265 6174 6520  anch).5. Create 
-00000be0: 6120 6e65 7720 5075 6c6c 2052 6571 7565  a new Pull Reque
-00000bf0: 7374 0a0a 2323 2323 204c 6963 656e 7365  st..#### License
-00000c00: 0a54 6869 7320 7072 6f6a 6563 7420 6973  .This project is
-00000c10: 206c 6963 656e 7365 6420 756e 6465 7220   licensed under 
-00000c20: 7468 6520 4d49 5420 4c69 6365 6e73 6520  the MIT License 
-00000c30: 2d20 7365 6520 7468 6520 4c49 4345 4e53  - see the LICENS
-00000c40: 4520 6669 6c65 2066 6f72 2064 6574 6169  E file for detai
-00000c50: 6c73 2e0a 0a23 2323 2320 4175 7468 6f72  ls...#### Author
-00000c60: 0a52 7961 6e20 5761 6c64 6f72 6620 2d20  .Ryan Waldorf - 
-00000c70: 7279 616e 4072 7961 6e77 616c 646f 7266  ryan@ryanwaldorf
-00000c80: 2e63 6f6d 0a0a                           .com..
+000002e0: 2064 6973 636f 6e6e 6563 7465 6420 6461   disconnected da
+000002f0: 7461 6261 7365 7320 616e 6420 6461 7461  tabases and data
+00000300: 2077 6172 6568 6f75 7365 732e 2020 596f   warehouses.  Yo
+00000310: 7520 6361 6e20 6e6f 7720 7369 6d70 6c79  u can now simply
+00000320: 2075 6e6c 6f61 6420 6120 4353 562c 2074   unload a CSV, t
+00000330: 7572 6e20 7468 6174 2043 5356 2069 6e74  urn that CSV int
+00000340: 6f20 5351 4c20 7374 6174 656d 656e 7473  o SQL statements
+00000350: 2063 7265 6174 696e 6720 6120 7465 6d70   creating a temp
+00000360: 2074 6162 6c65 2061 6e64 2069 6e73 6572   table and inser
+00000370: 7469 6e67 2064 6174 6120 7769 7468 2061  ting data with a
+00000380: 2043 4c49 2063 6f6d 6d61 6e64 2c20 616e   CLI command, an
+00000390: 6420 636f 7079 2074 686f 7365 2053 514c  d copy those SQL
+000003a0: 2073 7461 7465 6d65 6e74 7320 696e 746f   statements into
+000003b0: 2079 6f75 7220 7175 6572 7920 6564 6974   your query edit
+000003c0: 6f72 2073 6f20 796f 7520 6361 6e20 7374  or so you can st
+000003d0: 6172 7420 7573 696e 6720 7468 6520 6461  art using the da
+000003e0: 7461 2069 6e20 6120 6469 6666 6572 656e  ta in a differen
+000003f0: 7420 7761 7265 686f 7573 652e 0a0a 3c62  t warehouse...<b
+00000400: 3e57 6879 2064 6964 2049 2062 7569 6c64  >Why did I build
+00000410: 2074 6869 733f 3c2f 623e 2020 4927 6d20   this?</b>  I'm 
+00000420: 6f66 7465 6e20 776f 6e64 6572 696e 6720  often wondering 
+00000430: 686f 7720 6120 7072 6f64 7563 7420 4927  how a product I'
+00000440: 6d20 776f 726b 696e 6720 6f6e 2069 7320  m working on is 
+00000450: 6c69 6e6b 6564 2074 6f20 6375 7374 6f6d  linked to custom
+00000460: 6572 2073 7065 6e64 2e20 2048 6f77 6576  er spend.  Howev
+00000470: 6572 2c20 6d79 206f 7065 7261 7469 6f6e  er, my operation
+00000480: 616c 2077 6172 6568 6f75 7365 2074 6861  al warehouse tha
+00000490: 7420 696e 636c 7564 6573 2064 6174 6120  t includes data 
+000004a0: 6c69 6b65 2074 6865 2064 6174 6573 2061  like the dates a
+000004b0: 6e64 2074 696d 6573 2063 7573 746f 6d65  nd times custome
+000004c0: 7273 2075 7365 6420 6120 7072 6f64 7563  rs used a produc
+000004d0: 7420 6973 2073 6570 6172 6174 6520 6672  t is separate fr
+000004e0: 6f6d 206d 7920 6669 6e61 6e63 6961 6c20  om my financial 
+000004f0: 7761 7265 686f 7573 6520 7768 6963 6820  warehouse which 
+00000500: 6861 7320 7468 6520 6269 6c6c 696e 6720  has the billing 
+00000510: 6461 7461 2e20 2049 206e 6565 6420 746f  data.  I need to
+00000520: 206d 6f76 6520 6461 7461 2066 726f 6d20   move data from 
+00000530: 6f6e 6520 746f 2074 6865 206f 7468 6572  one to the other
+00000540: 2073 6f20 4920 6361 6e20 6a6f 696e 2074   so I can join t
+00000550: 6865 2066 696e 616e 6365 2061 6e64 2070  he finance and p
+00000560: 726f 6475 6374 2064 6174 6120 746f 6765  roduct data toge
+00000570: 7468 6572 2074 6f20 646f 2061 6e20 616e  ther to do an an
+00000580: 616c 7973 6973 2e2e 2e61 6e64 2074 7572  alysis...and tur
+00000590: 6e69 6e67 2074 6865 2043 5356 2069 6e74  ning the CSV int
+000005a0: 6f20 5351 4c20 6279 2068 616e 6420 696e  o SQL by hand in
+000005b0: 2065 7863 656c 2069 7320 6120 5049 5441   excel is a PITA
+000005c0: 2e20 2057 6974 6820 7468 6973 2c20 4920  .  With this, I 
+000005d0: 6361 6e20 6e6f 7720 6d6f 7665 2074 6865  can now move the
+000005e0: 2064 6174 6120 696e 2073 6563 6f6e 6473   data in seconds
+000005f0: 2e20 2049 2073 696d 706c 7920 646f 776e  .  I simply down
+00000600: 6c6f 6164 2074 6865 2043 5356 2c20 7275  load the CSV, ru
+00000610: 6e20 3c63 6f64 653e 6765 6e65 7261 7465  n <code>generate
+00000620: 2d74 742d 7371 6c20 6373 765f 6e61 6d65  -tt-sql csv_name
+00000630: 2e63 7376 3c2f 636f 6465 3e20 696e 206d  .csv</code> in m
+00000640: 7920 7465 726d 696e 616c 2c20 616e 6420  y terminal, and 
+00000650: 636f 7079 2069 7420 696e 746f 206d 7920  copy it into my 
+00000660: 7175 6572 7920 6564 6974 6f72 2e20 2049  query editor.  I
+00000670: 7427 7320 696d 6d65 6469 6174 656c 7920  t's immediately 
+00000680: 6176 6169 6c61 626c 6520 746f 2071 7565  available to que
+00000690: 7279 2073 6f20 4920 6361 6e20 676f 2073  ry so I can go s
+000006a0: 7472 6169 6768 7420 746f 2061 6e61 6c79  traight to analy
+000006b0: 7369 732e 0a0a 2323 2046 6561 7475 7265  sis...## Feature
+000006c0: 730a 0a2d 204c 6f61 6420 6461 7461 2066  s..- Load data f
+000006d0: 726f 6d20 6120 4353 5620 6669 6c65 0a2d  rom a CSV file.-
+000006e0: 2047 656e 6572 6174 6520 6120 6043 5245   Generate a `CRE
+000006f0: 4154 4520 5445 4d50 2054 4142 4c45 6020  ATE TEMP TABLE` 
+00000700: 5351 4c20 7374 6174 656d 656e 740a 2d20  SQL statement.- 
+00000710: 4765 6e65 7261 7465 2060 494e 5345 5254  Generate `INSERT
+00000720: 2049 4e54 4f60 2053 514c 2073 7461 7465   INTO` SQL state
+00000730: 6d65 6e74 7320 666f 7220 7468 6520 6461  ments for the da
+00000740: 7461 0a2d 2043 6f6d 6d61 6e64 2d6c 696e  ta.- Command-lin
+00000750: 6520 696e 7465 7266 6163 6520 2843 4c49  e interface (CLI
+00000760: 2920 666f 7220 6561 7379 2075 7361 6765  ) for easy usage
+00000770: 0a0a 2323 2049 6e73 7461 6c6c 6174 696f  ..## Installatio
+00000780: 6e0a 0a23 2323 2050 7265 7265 7175 6973  n..### Prerequis
+00000790: 6974 6573 0a0a 2d20 5079 7468 6f6e 2033  ites..- Python 3
+000007a0: 2e36 206f 7220 6869 6768 6572 0a2d 2060  .6 or higher.- `
+000007b0: 7061 6e64 6173 6020 6c69 6272 6172 790a  pandas` library.
+000007c0: 0a23 2323 2049 6e73 7461 6c6c 696e 670a  .### Installing.
+000007d0: 0a31 2e20 436c 6f6e 6520 7468 6520 7265  .1. Clone the re
+000007e0: 706f 7369 746f 7279 3a0a 2020 2020 6060  pository:.    ``
+000007f0: 6073 680a 2020 2020 6769 7420 636c 6f6e  `sh.    git clon
+00000800: 6520 6874 7470 733a 2f2f 6769 7468 7562  e https://github
+00000810: 2e63 6f6d 2f72 7977 616c 646f 722f 6765  .com/rywaldor/ge
+00000820: 6e65 7261 7465 5f74 656d 705f 7461 626c  nerate_temp_tabl
+00000830: 655f 7371 6c2e 6769 740a 2020 2020 6364  e_sql.git.    cd
+00000840: 2067 656e 6572 6174 655f 7465 6d70 5f74   generate_temp_t
+00000850: 6162 6c65 5f73 716c 0a20 2020 2060 6060  able_sql.    ```
+00000860: 0a0a 322e 2049 6e73 7461 6c6c 2074 6865  ..2. Install the
+00000870: 2070 6163 6b61 6765 206c 6f63 616c 6c79   package locally
+00000880: 3a0a 2020 2020 6060 6073 680a 2020 2020  :.    ```sh.    
+00000890: 7069 7020 696e 7374 616c 6c20 2d65 202e  pip install -e .
+000008a0: 0a20 2020 2060 6060 0a0a 2323 2055 7361  .    ```..## Usa
+000008b0: 6765 0a0a 2323 2320 436f 6d6d 616e 642d  ge..### Command-
+000008c0: 4c69 6e65 2049 6e74 6572 6661 6365 2028  Line Interface (
+000008d0: 434c 4929 0a0a 4166 7465 7220 696e 7374  CLI)..After inst
+000008e0: 616c 6c69 6e67 2074 6865 2070 6163 6b61  alling the packa
+000008f0: 6765 2c20 796f 7520 6361 6e20 7573 6520  ge, you can use 
+00000900: 7468 6520 6067 656e 6572 6174 652d 7474  the `generate-tt
+00000910: 2d73 716c 6020 636f 6d6d 616e 6420 746f  -sql` command to
+00000920: 2067 656e 6572 6174 6520 5351 4c20 7374   generate SQL st
+00000930: 6174 656d 656e 7473 2066 726f 6d20 6120  atements from a 
+00000940: 4353 5620 6669 6c65 2e0a 0a23 2323 2320  CSV file...#### 
+00000950: 4261 7369 6320 5573 6167 650a 0a54 6f20  Basic Usage..To 
+00000960: 6765 6e65 7261 7465 2053 514c 2073 7461  generate SQL sta
+00000970: 7465 6d65 6e74 7320 616e 6420 7361 7665  tements and save
+00000980: 2074 6865 6d20 746f 2061 2066 696c 653a   them to a file:
+00000990: 0a60 6060 7368 0a67 656e 6572 6174 652d  .```sh.generate-
+000009a0: 7474 2d73 716c 2070 6174 682f 746f 2f79  tt-sql path/to/y
+000009b0: 6f75 722f 6669 6c65 2e63 7376 0a60 6060  our/file.csv.```
+000009c0: 0a0a 2323 2323 2041 6464 6974 696f 6e61  ..#### Additiona
+000009d0: 6c20 4f70 7469 6f6e 730a 6060 6073 680a  l Options.```sh.
+000009e0: 0a2d 2d6f 2054 6865 2070 6174 6820 746f  .--o The path to
+000009f0: 2074 6865 206f 7574 7075 7420 5351 4c20   the output SQL 
+00000a00: 6669 6c65 2e20 2044 6566 6175 6c74 7320  file.  Defaults 
+00000a10: 746f 2074 6865 2064 6972 6563 746f 7220  to the director 
+00000a20: 796f 7520 6361 6c6c 2074 6865 2063 6f6d  you call the com
+00000a30: 6d61 6e64 2069 6e2e 0a2d 2d6f 7665 7277  mand in..--overw
+00000a40: 7269 7465 3a20 416c 6c6f 7720 6f76 6572  rite: Allow over
+00000a50: 7772 6974 696e 6720 7468 6520 6f75 7470  writing the outp
+00000a60: 7574 2066 696c 6520 6966 2069 7420 6578  ut file if it ex
+00000a70: 6973 7473 2e0a 2d2d 7461 626c 655f 6e61  ists..--table_na
+00000a80: 6d65 3a20 5370 6563 6966 7920 7468 6520  me: Specify the 
+00000a90: 6e61 6d65 206f 6620 7468 6520 7465 6d70  name of the temp
+00000aa0: 6f72 6172 7920 7461 626c 6520 746f 2063  orary table to c
+00000ab0: 7265 6174 652e 0a2d 2d63 6f6c 756d 6e5f  reate..--column_
+00000ac0: 7479 7065 3a20 5370 6563 6966 7920 7468  type: Specify th
+00000ad0: 6520 6461 7461 2074 7970 6520 6f66 2074  e data type of t
+00000ae0: 6865 2063 6f6c 756d 6e73 2069 6e20 7468  he columns in th
+00000af0: 6520 7465 6d70 6f72 6172 7920 7461 626c  e temporary tabl
+00000b00: 652e 2044 6566 6175 6c74 7320 746f 2054  e. Defaults to T
+00000b10: 4558 5420 7768 6963 6820 776f 726b 7320  EXT which works 
+00000b20: 666f 7220 5265 6473 6869 6674 2061 6e64  for Redshift and
+00000b30: 2053 6e6f 7766 6c61 6b65 2e20 5573 6520   Snowflake. Use 
+00000b40: 5354 5249 4e47 2066 6f72 2042 6967 5175  STRING for BigQu
+00000b50: 6572 792e 0a60 6060 0a0a 2323 2323 2045  ery..```..#### E
+00000b60: 7861 6d70 6c65 0a41 7373 756d 6520 796f  xample.Assume yo
+00000b70: 7520 6861 7665 2061 2043 5356 2066 696c  u have a CSV fil
+00000b80: 6520 6578 616d 706c 652e 6373 7620 7769  e example.csv wi
+00000b90: 7468 2074 6865 2066 6f6c 6c6f 7769 6e67  th the following
+00000ba0: 2063 6f6e 7465 6e74 3a0a 0a60 6060 7368   content:..```sh
+00000bb0: 0a6e 616d 652c 6167 652c 6369 7479 0a4a  .name,age,city.J
+00000bc0: 6f68 6e2c 3330 2c4e 6577 2059 6f72 6b0a  ohn,30,New York.
+00000bd0: 4a61 6e65 2c32 352c 4c6f 7320 416e 6765  Jane,25,Los Ange
+00000be0: 6c65 730a 6060 600a 0a52 756e 2074 6865  les.```..Run the
+00000bf0: 2066 6f6c 6c6f 7769 6e67 2063 6f6d 6d61   following comma
+00000c00: 6e64 2074 6f20 6765 6e65 7261 7465 2053  nd to generate S
+00000c10: 514c 2073 7461 7465 6d65 6e74 733a 0a0a  QL statements:..
+00000c20: 6060 6073 680a 6765 6e65 7261 7465 2d74  ```sh.generate-t
+00000c30: 742d 7371 6c20 6578 616d 706c 652e 6373  t-sql example.cs
+00000c40: 7620 2d6f 206f 7574 7075 742e 7371 6c20  v -o output.sql 
+00000c50: 2d2d 7461 626c 655f 6e61 6d65 206d 795f  --table_name my_
+00000c60: 7465 6d70 5f74 6162 6c65 202d 2d63 6f6c  temp_table --col
+00000c70: 756d 6e5f 7479 7065 2053 5452 494e 470a  umn_type STRING.
+00000c80: 6060 600a 0a54 6865 206f 7574 7075 742e  ```..The output.
+00000c90: 7371 6c20 6669 6c65 2077 696c 6c20 636f  sql file will co
+00000ca0: 6e74 6169 6e3a 0a0a 6060 6073 680a 4352  ntain:..```sh.CR
+00000cb0: 4541 5445 2054 454d 5020 5441 424c 4520  EATE TEMP TABLE 
+00000cc0: 6d79 5f74 656d 705f 7461 626c 6520 280a  my_temp_table (.
+00000cd0: 2020 2020 6e61 6d65 2053 5452 494e 472c      name STRING,
+00000ce0: 0a20 2020 2061 6765 2053 5452 494e 472c  .    age STRING,
+00000cf0: 0a20 2020 2063 6974 7920 5354 5249 4e47  .    city STRING
+00000d00: 0a29 3b0a 0a2d 2d49 6e73 6572 7420 4461  .);..--Insert Da
+00000d10: 7461 2053 514c 3a0a 494e 5345 5254 2049  ta SQL:.INSERT I
+00000d20: 4e54 4f20 6d79 5f74 656d 705f 7461 626c  NTO my_temp_tabl
+00000d30: 6520 286e 616d 652c 2061 6765 2c20 6369  e (name, age, ci
+00000d40: 7479 2920 5641 4c55 4553 200a 2020 2020  ty) VALUES .    
+00000d50: 2827 4a6f 686e 272c 2027 3330 272c 2027  ('John', '30', '
+00000d60: 4e65 7720 596f 726b 2729 2c0a 2020 2020  New York'),.    
+00000d70: 2827 4a61 6e65 272c 2027 3235 272c 2027  ('Jane', '25', '
+00000d80: 4c6f 7320 416e 6765 6c65 7327 293b 0a60  Los Angeles');.`
+00000d90: 6060 0a0a 2323 2323 2052 756e 6e69 6e67  ``..#### Running
+00000da0: 2054 6573 7473 0a54 6f20 7275 6e20 7468   Tests.To run th
+00000db0: 6520 7465 7374 732c 2075 7365 2074 6865  e tests, use the
+00000dc0: 2066 6f6c 6c6f 7769 6e67 2063 6f6d 6d61   following comma
+00000dd0: 6e64 3a0a 0a60 6060 7368 0a70 7974 686f  nd:..```sh.pytho
+00000de0: 6e20 2d6d 2075 6e69 7474 6573 7420 6469  n -m unittest di
+00000df0: 7363 6f76 6572 202d 7320 7465 7374 730a  scover -s tests.
+00000e00: 6060 600a 0a23 2323 2320 436f 6e74 7269  ```..#### Contri
+00000e10: 6275 7469 6e67 0a43 6f6e 7472 6962 7574  buting.Contribut
+00000e20: 696f 6e73 2061 7265 2077 656c 636f 6d65  ions are welcome
+00000e30: 2120 506c 6561 7365 2066 6f6c 6c6f 7720  ! Please follow 
+00000e40: 7468 6573 6520 7374 6570 733a 0a0a 312e  these steps:..1.
+00000e50: 2046 6f72 6b20 7468 6520 7265 706f 7369   Fork the reposi
+00000e60: 746f 7279 0a32 2e20 4372 6561 7465 2061  tory.2. Create a
+00000e70: 206e 6577 2062 7261 6e63 6820 2867 6974   new branch (git
+00000e80: 2063 6865 636b 6f75 7420 2d62 2066 6561   checkout -b fea
+00000e90: 7475 7265 2d62 7261 6e63 6829 0a33 2e20  ture-branch).3. 
+00000ea0: 436f 6d6d 6974 2079 6f75 7220 6368 616e  Commit your chan
+00000eb0: 6765 7320 2867 6974 2063 6f6d 6d69 7420  ges (git commit 
+00000ec0: 2d61 6d20 2741 6464 206e 6577 2066 6561  -am 'Add new fea
+00000ed0: 7475 7265 2729 0a34 2e20 5075 7368 2074  ture').4. Push t
+00000ee0: 6f20 7468 6520 6272 616e 6368 2028 6769  o the branch (gi
+00000ef0: 7420 7075 7368 206f 7269 6769 6e20 6665  t push origin fe
+00000f00: 6174 7572 652d 6272 616e 6368 290a 352e  ature-branch).5.
+00000f10: 2043 7265 6174 6520 6120 6e65 7720 5075   Create a new Pu
+00000f20: 6c6c 2052 6571 7565 7374 0a0a 2323 2323  ll Request..####
+00000f30: 204c 6963 656e 7365 0a54 6869 7320 7072   License.This pr
+00000f40: 6f6a 6563 7420 6973 206c 6963 656e 7365  oject is license
+00000f50: 6420 756e 6465 7220 7468 6520 4d49 5420  d under the MIT 
+00000f60: 4c69 6365 6e73 6520 2d20 7365 6520 7468  License - see th
+00000f70: 6520 4c49 4345 4e53 4520 6669 6c65 2066  e LICENSE file f
+00000f80: 6f72 2064 6574 6169 6c73 2e0a 0a23 2323  or details...###
+00000f90: 2320 4175 7468 6f72 0a52 7961 6e20 5761  # Author.Ryan Wa
+00000fa0: 6c64 6f72 6620 2d20 7279 616e 4072 7961  ldorf - ryan@rya
+00000fb0: 6e77 616c 646f 7266 2e63 6f6d 3c62 722f  nwaldorf.com<br/
+00000fc0: 3e0a 3c61 2068 7265 663d 2268 7474 7073  >.<a href="https
+00000fd0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7279  ://github.com/ry
+00000fe0: 616e 7761 6c64 6f72 6622 2074 6172 6765  anwaldorf" targe
+00000ff0: 743d 225f 626c 616e 6b22 3e47 6974 4875  t="_blank">GitHu
+00001000: 623c 2f61 3e0a 3c61 2068 7265 663d 2268  b</a>.<a href="h
+00001010: 7474 7073 3a2f 2f77 7777 2e6c 696e 6b65  ttps://www.linke
+00001020: 6469 6e2e 636f 6d2f 696e 2f72 7961 6e2d  din.com/in/ryan-
+00001030: 7761 6c64 6f72 662f 2220 7461 7267 6574  waldorf/" target
+00001040: 3d22 5f62 6c61 6e6b 223e 4c69 6e6b 6564  ="_blank">Linked
+00001050: 496e 3c2f 613e 0a0a                      In</a>..
```

### Comparing `generate_temp_table_sql-0.4.2/generate_temp_table_sql.egg-info/SOURCES.txt` & `generate_temp_table_sql-0.4.3/generate_temp_table_sql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `generate_temp_table_sql-0.4.2/setup.py` & `generate_temp_table_sql-0.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='generate_temp_table_sql',
-    version='0.4.2',
+    version='0.4.3',
     packages=find_packages(),
     install_requires=[
         'pandas',
     ],
     entry_points={
         'console_scripts': [
             'generate-tt-sql=generate_temp_table_sql.cli:main',
```

### Comparing `generate_temp_table_sql-0.4.2/tests/test_sql_generator.py` & `generate_temp_table_sql-0.4.3/tests/test_sql_generator.py`

 * *Files identical despite different names*

