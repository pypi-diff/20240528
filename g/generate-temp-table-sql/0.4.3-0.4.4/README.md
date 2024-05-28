# Comparing `tmp/generate_temp_table_sql-0.4.3.tar.gz` & `tmp/generate_temp_table_sql-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "generate_temp_table_sql-0.4.3.tar", last modified: Tue May 28 12:02:06 2024, max compression
+gzip compressed data, was "generate_temp_table_sql-0.4.4.tar", last modified: Tue May 28 12:18:08 2024, max compression
```

## Comparing `generate_temp_table_sql-0.4.3.tar` & `generate_temp_table_sql-0.4.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 ryanwaldorf   (501) staff       (20)        0 2024-05-28 12:02:06.748697 generate_temp_table_sql-0.4.3/
--rw-r--r--   0 ryanwaldorf   (501) staff       (20)     1068 2024-05-26 15:44:57.000000 generate_temp_table_sql-0.4.3/LICENSE.txt
--rw-r--r--   0 ryanwaldorf   (501) staff       (20)       37 2024-05-26 15:46:01.000000 generate_temp_table_sql-0.4.3/MANIFEST.in
--rw-r--r--   0 ryanwaldorf   (501) staff       (20)     4184 2024-05-28 12:02:06.748606 generate_temp_table_sql-0.4.3/PKG-INFO
--rw-r--r--   0 ryanwaldorf   (501) staff       (20)     3661 2024-05-28 11:46:17.000000 generate_temp_table_sql-0.4.3/README.md
-drwxr-xr-x   0 ryanwaldorf   (501) staff       (20)        0 2024-05-28 12:02:06.747195 generate_temp_table_sql-0.4.3/generate_temp_table_sql/
--rw-r--r--   0 ryanwaldorf   (501) staff       (20)        0 2024-05-25 15:54:27.000000 generate_temp_table_sql-0.4.3/generate_temp_table_sql/__init__.py
--rw-r--r--   0 ryanwaldorf   (501) staff       (20)     2135 2024-05-28 12:00:45.000000 generate_temp_table_sql-0.4.3/generate_temp_table_sql/cli.py
--rw-r--r--   0 ryanwaldorf   (501) staff       (20)       88 2024-05-27 13:29:03.000000 generate_temp_table_sql-0.4.3/generate_temp_table_sql/constants.py
--rw-r--r--   0 ryanwaldorf   (501) staff       (20)     2559 2024-05-27 16:41:04.000000 generate_temp_table_sql-0.4.3/generate_temp_table_sql/sql_generator.py
-drwxr-xr-x   0 ryanwaldorf   (501) staff       (20)        0 2024-05-28 12:02:06.748004 generate_temp_table_sql-0.4.3/generate_temp_table_sql.egg-info/
--rw-r--r--   0 ryanwaldorf   (501) staff       (20)     4184 2024-05-28 12:02:06.000000 generate_temp_table_sql-0.4.3/generate_temp_table_sql.egg-info/PKG-INFO
--rw-r--r--   0 ryanwaldorf   (501) staff       (20)      517 2024-05-28 12:02:06.000000 generate_temp_table_sql-0.4.3/generate_temp_table_sql.egg-info/SOURCES.txt
--rw-r--r--   0 ryanwaldorf   (501) staff       (20)        1 2024-05-28 12:02:06.000000 generate_temp_table_sql-0.4.3/generate_temp_table_sql.egg-info/dependency_links.txt
--rw-r--r--   0 ryanwaldorf   (501) staff       (20)       70 2024-05-28 12:02:06.000000 generate_temp_table_sql-0.4.3/generate_temp_table_sql.egg-info/entry_points.txt
--rw-r--r--   0 ryanwaldorf   (501) staff       (20)        7 2024-05-28 12:02:06.000000 generate_temp_table_sql-0.4.3/generate_temp_table_sql.egg-info/requires.txt
--rw-r--r--   0 ryanwaldorf   (501) staff       (20)       30 2024-05-28 12:02:06.000000 generate_temp_table_sql-0.4.3/generate_temp_table_sql.egg-info/top_level.txt
--rw-r--r--   0 ryanwaldorf   (501) staff       (20)       38 2024-05-28 12:02:06.748734 generate_temp_table_sql-0.4.3/setup.cfg
--rw-r--r--   0 ryanwaldorf   (501) staff       (20)      819 2024-05-28 12:01:10.000000 generate_temp_table_sql-0.4.3/setup.py
-drwxr-xr-x   0 ryanwaldorf   (501) staff       (20)        0 2024-05-28 12:02:06.748287 generate_temp_table_sql-0.4.3/tests/
--rw-r--r--   0 ryanwaldorf   (501) staff       (20)        0 2024-05-25 16:57:00.000000 generate_temp_table_sql-0.4.3/tests/__init__.py
--rw-r--r--   0 ryanwaldorf   (501) staff       (20)     5435 2024-05-27 16:45:56.000000 generate_temp_table_sql-0.4.3/tests/test_sql_generator.py
+drwxr-xr-x   0 ryanwaldorf   (501) staff       (20)        0 2024-05-28 12:18:08.341174 generate_temp_table_sql-0.4.4/
+-rw-r--r--   0 ryanwaldorf   (501) staff       (20)     1068 2024-05-26 15:44:57.000000 generate_temp_table_sql-0.4.4/LICENSE.txt
+-rw-r--r--   0 ryanwaldorf   (501) staff       (20)       37 2024-05-26 15:46:01.000000 generate_temp_table_sql-0.4.4/MANIFEST.in
+-rw-r--r--   0 ryanwaldorf   (501) staff       (20)     4385 2024-05-28 12:18:08.341059 generate_temp_table_sql-0.4.4/PKG-INFO
+-rw-r--r--   0 ryanwaldorf   (501) staff       (20)     3862 2024-05-28 12:12:17.000000 generate_temp_table_sql-0.4.4/README.md
+drwxr-xr-x   0 ryanwaldorf   (501) staff       (20)        0 2024-05-28 12:18:08.339717 generate_temp_table_sql-0.4.4/generate_temp_table_sql/
+-rw-r--r--   0 ryanwaldorf   (501) staff       (20)        0 2024-05-25 15:54:27.000000 generate_temp_table_sql-0.4.4/generate_temp_table_sql/__init__.py
+-rw-r--r--   0 ryanwaldorf   (501) staff       (20)     2135 2024-05-28 12:00:45.000000 generate_temp_table_sql-0.4.4/generate_temp_table_sql/cli.py
+-rw-r--r--   0 ryanwaldorf   (501) staff       (20)       88 2024-05-27 13:29:03.000000 generate_temp_table_sql-0.4.4/generate_temp_table_sql/constants.py
+-rw-r--r--   0 ryanwaldorf   (501) staff       (20)     2559 2024-05-27 16:41:04.000000 generate_temp_table_sql-0.4.4/generate_temp_table_sql/sql_generator.py
+drwxr-xr-x   0 ryanwaldorf   (501) staff       (20)        0 2024-05-28 12:18:08.340696 generate_temp_table_sql-0.4.4/generate_temp_table_sql.egg-info/
+-rw-r--r--   0 ryanwaldorf   (501) staff       (20)     4385 2024-05-28 12:18:08.000000 generate_temp_table_sql-0.4.4/generate_temp_table_sql.egg-info/PKG-INFO
+-rw-r--r--   0 ryanwaldorf   (501) staff       (20)      517 2024-05-28 12:18:08.000000 generate_temp_table_sql-0.4.4/generate_temp_table_sql.egg-info/SOURCES.txt
+-rw-r--r--   0 ryanwaldorf   (501) staff       (20)        1 2024-05-28 12:18:08.000000 generate_temp_table_sql-0.4.4/generate_temp_table_sql.egg-info/dependency_links.txt
+-rw-r--r--   0 ryanwaldorf   (501) staff       (20)       70 2024-05-28 12:18:08.000000 generate_temp_table_sql-0.4.4/generate_temp_table_sql.egg-info/entry_points.txt
+-rw-r--r--   0 ryanwaldorf   (501) staff       (20)        7 2024-05-28 12:18:08.000000 generate_temp_table_sql-0.4.4/generate_temp_table_sql.egg-info/requires.txt
+-rw-r--r--   0 ryanwaldorf   (501) staff       (20)       30 2024-05-28 12:18:08.000000 generate_temp_table_sql-0.4.4/generate_temp_table_sql.egg-info/top_level.txt
+-rw-r--r--   0 ryanwaldorf   (501) staff       (20)       38 2024-05-28 12:18:08.341213 generate_temp_table_sql-0.4.4/setup.cfg
+-rw-r--r--   0 ryanwaldorf   (501) staff       (20)      819 2024-05-28 12:13:13.000000 generate_temp_table_sql-0.4.4/setup.py
+drwxr-xr-x   0 ryanwaldorf   (501) staff       (20)        0 2024-05-28 12:18:08.340890 generate_temp_table_sql-0.4.4/tests/
+-rw-r--r--   0 ryanwaldorf   (501) staff       (20)        0 2024-05-25 16:57:00.000000 generate_temp_table_sql-0.4.4/tests/__init__.py
+-rw-r--r--   0 ryanwaldorf   (501) staff       (20)     5435 2024-05-27 16:45:56.000000 generate_temp_table_sql-0.4.4/tests/test_sql_generator.py
```

### Comparing `generate_temp_table_sql-0.4.3/LICENSE.txt` & `generate_temp_table_sql-0.4.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `generate_temp_table_sql-0.4.3/PKG-INFO` & `generate_temp_table_sql-0.4.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6765 6e65  : 2.1.Name: gene
 00000020: 7261 7465 5f74 656d 705f 7461 626c 655f  rate_temp_table_
 00000030: 7371 6c0a 5665 7273 696f 6e3a 2030 2e34  sql.Version: 0.4
-00000040: 2e33 0a53 756d 6d61 7279 3a20 4120 7061  .3.Summary: A pa
+00000040: 2e34 0a53 756d 6d61 7279 3a20 4120 7061  .4.Summary: A pa
 00000050: 636b 6167 6520 746f 2067 656e 6572 6174  ckage to generat
 00000060: 6520 5351 4c20 7374 6174 656d 656e 7473  e SQL statements
 00000070: 2066 726f 6d20 4353 5620 6669 6c65 730a   from CSV files.
 00000080: 486f 6d65 2d70 6167 653a 2068 7474 7073  Home-page: https
 00000090: 3a2f 2f67 6974 6875 622e 636f 6d2f 7279  ://github.com/ry
 000000a0: 616e 7761 6c64 6f72 662f 6765 6e65 7261  anwaldorf/genera
 000000b0: 7465 5f74 656d 705f 7461 626c 655f 7371  te_temp_table_sq
@@ -175,88 +175,101 @@
 00000ae0: 6865 2063 6f6c 756d 6e73 2069 6e20 7468  he columns in th
 00000af0: 6520 7465 6d70 6f72 6172 7920 7461 626c  e temporary tabl
 00000b00: 652e 2044 6566 6175 6c74 7320 746f 2054  e. Defaults to T
 00000b10: 4558 5420 7768 6963 6820 776f 726b 7320  EXT which works 
 00000b20: 666f 7220 5265 6473 6869 6674 2061 6e64  for Redshift and
 00000b30: 2053 6e6f 7766 6c61 6b65 2e20 5573 6520   Snowflake. Use 
 00000b40: 5354 5249 4e47 2066 6f72 2042 6967 5175  STRING for BigQu
-00000b50: 6572 792e 0a60 6060 0a0a 2323 2323 2045  ery..```..#### E
-00000b60: 7861 6d70 6c65 0a41 7373 756d 6520 796f  xample.Assume yo
-00000b70: 7520 6861 7665 2061 2043 5356 2066 696c  u have a CSV fil
-00000b80: 6520 6578 616d 706c 652e 6373 7620 7769  e example.csv wi
-00000b90: 7468 2074 6865 2066 6f6c 6c6f 7769 6e67  th the following
-00000ba0: 2063 6f6e 7465 6e74 3a0a 0a60 6060 7368   content:..```sh
-00000bb0: 0a6e 616d 652c 6167 652c 6369 7479 0a4a  .name,age,city.J
-00000bc0: 6f68 6e2c 3330 2c4e 6577 2059 6f72 6b0a  ohn,30,New York.
-00000bd0: 4a61 6e65 2c32 352c 4c6f 7320 416e 6765  Jane,25,Los Ange
-00000be0: 6c65 730a 6060 600a 0a52 756e 2074 6865  les.```..Run the
-00000bf0: 2066 6f6c 6c6f 7769 6e67 2063 6f6d 6d61   following comma
-00000c00: 6e64 2074 6f20 6765 6e65 7261 7465 2053  nd to generate S
-00000c10: 514c 2073 7461 7465 6d65 6e74 733a 0a0a  QL statements:..
-00000c20: 6060 6073 680a 6765 6e65 7261 7465 2d74  ```sh.generate-t
-00000c30: 742d 7371 6c20 6578 616d 706c 652e 6373  t-sql example.cs
-00000c40: 7620 2d6f 206f 7574 7075 742e 7371 6c20  v -o output.sql 
-00000c50: 2d2d 7461 626c 655f 6e61 6d65 206d 795f  --table_name my_
-00000c60: 7465 6d70 5f74 6162 6c65 202d 2d63 6f6c  temp_table --col
-00000c70: 756d 6e5f 7479 7065 2053 5452 494e 470a  umn_type STRING.
-00000c80: 6060 600a 0a54 6865 206f 7574 7075 742e  ```..The output.
-00000c90: 7371 6c20 6669 6c65 2077 696c 6c20 636f  sql file will co
-00000ca0: 6e74 6169 6e3a 0a0a 6060 6073 680a 4352  ntain:..```sh.CR
-00000cb0: 4541 5445 2054 454d 5020 5441 424c 4520  EATE TEMP TABLE 
-00000cc0: 6d79 5f74 656d 705f 7461 626c 6520 280a  my_temp_table (.
-00000cd0: 2020 2020 6e61 6d65 2053 5452 494e 472c      name STRING,
-00000ce0: 0a20 2020 2061 6765 2053 5452 494e 472c  .    age STRING,
-00000cf0: 0a20 2020 2063 6974 7920 5354 5249 4e47  .    city STRING
-00000d00: 0a29 3b0a 0a2d 2d49 6e73 6572 7420 4461  .);..--Insert Da
-00000d10: 7461 2053 514c 3a0a 494e 5345 5254 2049  ta SQL:.INSERT I
-00000d20: 4e54 4f20 6d79 5f74 656d 705f 7461 626c  NTO my_temp_tabl
-00000d30: 6520 286e 616d 652c 2061 6765 2c20 6369  e (name, age, ci
-00000d40: 7479 2920 5641 4c55 4553 200a 2020 2020  ty) VALUES .    
-00000d50: 2827 4a6f 686e 272c 2027 3330 272c 2027  ('John', '30', '
-00000d60: 4e65 7720 596f 726b 2729 2c0a 2020 2020  New York'),.    
-00000d70: 2827 4a61 6e65 272c 2027 3235 272c 2027  ('Jane', '25', '
-00000d80: 4c6f 7320 416e 6765 6c65 7327 293b 0a60  Los Angeles');.`
-00000d90: 6060 0a0a 2323 2323 2052 756e 6e69 6e67  ``..#### Running
-00000da0: 2054 6573 7473 0a54 6f20 7275 6e20 7468   Tests.To run th
-00000db0: 6520 7465 7374 732c 2075 7365 2074 6865  e tests, use the
-00000dc0: 2066 6f6c 6c6f 7769 6e67 2063 6f6d 6d61   following comma
-00000dd0: 6e64 3a0a 0a60 6060 7368 0a70 7974 686f  nd:..```sh.pytho
-00000de0: 6e20 2d6d 2075 6e69 7474 6573 7420 6469  n -m unittest di
-00000df0: 7363 6f76 6572 202d 7320 7465 7374 730a  scover -s tests.
-00000e00: 6060 600a 0a23 2323 2320 436f 6e74 7269  ```..#### Contri
-00000e10: 6275 7469 6e67 0a43 6f6e 7472 6962 7574  buting.Contribut
-00000e20: 696f 6e73 2061 7265 2077 656c 636f 6d65  ions are welcome
-00000e30: 2120 506c 6561 7365 2066 6f6c 6c6f 7720  ! Please follow 
-00000e40: 7468 6573 6520 7374 6570 733a 0a0a 312e  these steps:..1.
-00000e50: 2046 6f72 6b20 7468 6520 7265 706f 7369   Fork the reposi
-00000e60: 746f 7279 0a32 2e20 4372 6561 7465 2061  tory.2. Create a
-00000e70: 206e 6577 2062 7261 6e63 6820 2867 6974   new branch (git
-00000e80: 2063 6865 636b 6f75 7420 2d62 2066 6561   checkout -b fea
-00000e90: 7475 7265 2d62 7261 6e63 6829 0a33 2e20  ture-branch).3. 
-00000ea0: 436f 6d6d 6974 2079 6f75 7220 6368 616e  Commit your chan
-00000eb0: 6765 7320 2867 6974 2063 6f6d 6d69 7420  ges (git commit 
-00000ec0: 2d61 6d20 2741 6464 206e 6577 2066 6561  -am 'Add new fea
-00000ed0: 7475 7265 2729 0a34 2e20 5075 7368 2074  ture').4. Push t
-00000ee0: 6f20 7468 6520 6272 616e 6368 2028 6769  o the branch (gi
-00000ef0: 7420 7075 7368 206f 7269 6769 6e20 6665  t push origin fe
-00000f00: 6174 7572 652d 6272 616e 6368 290a 352e  ature-branch).5.
-00000f10: 2043 7265 6174 6520 6120 6e65 7720 5075   Create a new Pu
-00000f20: 6c6c 2052 6571 7565 7374 0a0a 2323 2323  ll Request..####
-00000f30: 204c 6963 656e 7365 0a54 6869 7320 7072   License.This pr
-00000f40: 6f6a 6563 7420 6973 206c 6963 656e 7365  oject is license
-00000f50: 6420 756e 6465 7220 7468 6520 4d49 5420  d under the MIT 
-00000f60: 4c69 6365 6e73 6520 2d20 7365 6520 7468  License - see th
-00000f70: 6520 4c49 4345 4e53 4520 6669 6c65 2066  e LICENSE file f
-00000f80: 6f72 2064 6574 6169 6c73 2e0a 0a23 2323  or details...###
-00000f90: 2320 4175 7468 6f72 0a52 7961 6e20 5761  # Author.Ryan Wa
-00000fa0: 6c64 6f72 6620 2d20 7279 616e 4072 7961  ldorf - ryan@rya
-00000fb0: 6e77 616c 646f 7266 2e63 6f6d 3c62 722f  nwaldorf.com<br/
-00000fc0: 3e0a 3c61 2068 7265 663d 2268 7474 7073  >.<a href="https
-00000fd0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7279  ://github.com/ry
-00000fe0: 616e 7761 6c64 6f72 6622 2074 6172 6765  anwaldorf" targe
-00000ff0: 743d 225f 626c 616e 6b22 3e47 6974 4875  t="_blank">GitHu
-00001000: 623c 2f61 3e0a 3c61 2068 7265 663d 2268  b</a>.<a href="h
-00001010: 7474 7073 3a2f 2f77 7777 2e6c 696e 6b65  ttps://www.linke
-00001020: 6469 6e2e 636f 6d2f 696e 2f72 7961 6e2d  din.com/in/ryan-
-00001030: 7761 6c64 6f72 662f 2220 7461 7267 6574  waldorf/" target
-00001040: 3d22 5f62 6c61 6e6b 223e 4c69 6e6b 6564  ="_blank">Linked
-00001050: 496e 3c2f 613e 0a0a                      In</a>..
+00000b50: 6572 792e 0a2d 2d62 6174 6368 5f73 697a  ery..--batch_siz
+00000b60: 653a 2053 7065 6369 6679 2074 6865 206e  e: Specify the n
+00000b70: 756d 6265 7220 6f66 2072 6f77 7320 696e  umber of rows in
+00000b80: 7365 7274 6564 2070 6572 2069 6e73 6572  serted per inser
+00000b90: 7420 7374 6174 656d 656e 742e 2020 4966  t statement.  If
+00000ba0: 2070 7265 7365 6e74 2c20 6974 2063 7265   present, it cre
+00000bb0: 6174 6573 206d 756c 7469 706c 6520 696e  ates multiple in
+00000bc0: 7365 7274 2073 7461 7465 6d65 6e74 7320  sert statements 
+00000bd0: 6261 7365 6420 6f6e 2074 6865 2062 6174  based on the bat
+00000be0: 6368 2073 697a 6520 7370 6563 6966 6965  ch size specifie
+00000bf0: 642e 0a60 6060 0a0a 2323 2323 2045 7861  d..```..#### Exa
+00000c00: 6d70 6c65 0a41 7373 756d 6520 796f 7520  mple.Assume you 
+00000c10: 6861 7665 2061 2043 5356 2066 696c 6520  have a CSV file 
+00000c20: 6578 616d 706c 652e 6373 7620 7769 7468  example.csv with
+00000c30: 2074 6865 2066 6f6c 6c6f 7769 6e67 2063   the following c
+00000c40: 6f6e 7465 6e74 3a0a 0a60 6060 7368 0a6e  ontent:..```sh.n
+00000c50: 616d 652c 6167 652c 6369 7479 0a4a 6f68  ame,age,city.Joh
+00000c60: 6e2c 3330 2c4e 6577 2059 6f72 6b0a 4a61  n,30,New York.Ja
+00000c70: 6e65 2c32 352c 4c6f 7320 416e 6765 6c65  ne,25,Los Angele
+00000c80: 730a 6060 600a 0a52 756e 2074 6865 2066  s.```..Run the f
+00000c90: 6f6c 6c6f 7769 6e67 2063 6f6d 6d61 6e64  ollowing command
+00000ca0: 2074 6f20 6765 6e65 7261 7465 2053 514c   to generate SQL
+00000cb0: 2073 7461 7465 6d65 6e74 733a 0a0a 6060   statements:..``
+00000cc0: 6073 680a 6765 6e65 7261 7465 2d74 742d  `sh.generate-tt-
+00000cd0: 7371 6c20 6578 616d 706c 652e 6373 7620  sql example.csv 
+00000ce0: 2d6f 206f 7574 7075 742e 7371 6c20 2d2d  -o output.sql --
+00000cf0: 7461 626c 655f 6e61 6d65 206d 795f 7465  table_name my_te
+00000d00: 6d70 5f74 6162 6c65 202d 2d63 6f6c 756d  mp_table --colum
+00000d10: 6e5f 7479 7065 2053 5452 494e 470a 6060  n_type STRING.``
+00000d20: 600a 0a54 6865 206f 7574 7075 742e 7371  `..The output.sq
+00000d30: 6c20 6669 6c65 2077 696c 6c20 636f 6e74  l file will cont
+00000d40: 6169 6e3a 0a0a 6060 6073 680a 4352 4541  ain:..```sh.CREA
+00000d50: 5445 2054 454d 5020 5441 424c 4520 6d79  TE TEMP TABLE my
+00000d60: 5f74 656d 705f 7461 626c 6520 280a 2020  _temp_table (.  
+00000d70: 2020 6e61 6d65 2053 5452 494e 472c 0a20    name STRING,. 
+00000d80: 2020 2061 6765 2053 5452 494e 472c 0a20     age STRING,. 
+00000d90: 2020 2063 6974 7920 5354 5249 4e47 0a29     city STRING.)
+00000da0: 3b0a 0a2d 2d49 6e73 6572 7420 4461 7461  ;..--Insert Data
+00000db0: 2053 514c 3a0a 494e 5345 5254 2049 4e54   SQL:.INSERT INT
+00000dc0: 4f20 6d79 5f74 656d 705f 7461 626c 6520  O my_temp_table 
+00000dd0: 286e 616d 652c 2061 6765 2c20 6369 7479  (name, age, city
+00000de0: 2920 5641 4c55 4553 200a 2020 2020 2827  ) VALUES .    ('
+00000df0: 4a6f 686e 272c 2027 3330 272c 2027 4e65  John', '30', 'Ne
+00000e00: 7720 596f 726b 2729 2c0a 2020 2020 2827  w York'),.    ('
+00000e10: 4a61 6e65 272c 2027 3235 272c 2027 4c6f  Jane', '25', 'Lo
+00000e20: 7320 416e 6765 6c65 7327 293b 0a60 6060  s Angeles');.```
+00000e30: 0a0a 416c 6c20 6172 6775 6d65 6e74 7320  ..All arguments 
+00000e40: 6172 6520 6f70 7469 6f6e 616c 2065 7863  are optional exc
+00000e50: 6570 7420 7468 6520 6373 760a 0a23 2323  ept the csv..###
+00000e60: 2320 5275 6e6e 696e 6720 5465 7374 730a  # Running Tests.
+00000e70: 546f 2072 756e 2074 6865 2074 6573 7473  To run the tests
+00000e80: 2c20 7573 6520 7468 6520 666f 6c6c 6f77  , use the follow
+00000e90: 696e 6720 636f 6d6d 616e 643a 0a0a 6060  ing command:..``
+00000ea0: 6073 680a 7079 7468 6f6e 202d 6d20 756e  `sh.python -m un
+00000eb0: 6974 7465 7374 2064 6973 636f 7665 7220  ittest discover 
+00000ec0: 2d73 2074 6573 7473 0a60 6060 0a0a 2323  -s tests.```..##
+00000ed0: 2323 2043 6f6e 7472 6962 7574 696e 670a  ## Contributing.
+00000ee0: 436f 6e74 7269 6275 7469 6f6e 7320 6172  Contributions ar
+00000ef0: 6520 7765 6c63 6f6d 6521 2050 6c65 6173  e welcome! Pleas
+00000f00: 6520 666f 6c6c 6f77 2074 6865 7365 2073  e follow these s
+00000f10: 7465 7073 3a0a 0a31 2e20 466f 726b 2074  teps:..1. Fork t
+00000f20: 6865 2072 6570 6f73 6974 6f72 790a 322e  he repository.2.
+00000f30: 2043 7265 6174 6520 6120 6e65 7720 6272   Create a new br
+00000f40: 616e 6368 2028 6769 7420 6368 6563 6b6f  anch (git checko
+00000f50: 7574 202d 6220 6665 6174 7572 652d 6272  ut -b feature-br
+00000f60: 616e 6368 290a 332e 2043 6f6d 6d69 7420  anch).3. Commit 
+00000f70: 796f 7572 2063 6861 6e67 6573 2028 6769  your changes (gi
+00000f80: 7420 636f 6d6d 6974 202d 616d 2027 4164  t commit -am 'Ad
+00000f90: 6420 6e65 7720 6665 6174 7572 6527 290a  d new feature').
+00000fa0: 342e 2050 7573 6820 746f 2074 6865 2062  4. Push to the b
+00000fb0: 7261 6e63 6820 2867 6974 2070 7573 6820  ranch (git push 
+00000fc0: 6f72 6967 696e 2066 6561 7475 7265 2d62  origin feature-b
+00000fd0: 7261 6e63 6829 0a35 2e20 4372 6561 7465  ranch).5. Create
+00000fe0: 2061 206e 6577 2050 756c 6c20 5265 7175   a new Pull Requ
+00000ff0: 6573 740a 0a23 2323 2320 4c69 6365 6e73  est..#### Licens
+00001000: 650a 5468 6973 2070 726f 6a65 6374 2069  e.This project i
+00001010: 7320 6c69 6365 6e73 6564 2075 6e64 6572  s licensed under
+00001020: 2074 6865 204d 4954 204c 6963 656e 7365   the MIT License
+00001030: 202d 2073 6565 2074 6865 204c 4943 454e   - see the LICEN
+00001040: 5345 2066 696c 6520 666f 7220 6465 7461  SE file for deta
+00001050: 696c 732e 0a0a 2323 2323 2041 7574 686f  ils...#### Autho
+00001060: 720a 5279 616e 2057 616c 646f 7266 202d  r.Ryan Waldorf -
+00001070: 2072 7961 6e40 7279 616e 7761 6c64 6f72   ryan@ryanwaldor
+00001080: 662e 636f 6d3c 6272 2f3e 0a3c 6120 6872  f.com<br/>.<a hr
+00001090: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+000010a0: 7562 2e63 6f6d 2f72 7961 6e77 616c 646f  ub.com/ryanwaldo
+000010b0: 7266 2220 7461 7267 6574 3d22 5f62 6c61  rf" target="_bla
+000010c0: 6e6b 223e 4769 7448 7562 3c2f 613e 0a3c  nk">GitHub</a>.<
+000010d0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+000010e0: 7777 772e 6c69 6e6b 6564 696e 2e63 6f6d  www.linkedin.com
+000010f0: 2f69 6e2f 7279 616e 2d77 616c 646f 7266  /in/ryan-waldorf
+00001100: 2f22 2074 6172 6765 743d 225f 626c 616e  /" target="_blan
+00001110: 6b22 3e4c 696e 6b65 6449 6e3c 2f61 3e0a  k">LinkedIn</a>.
+00001120: 0a                                       .
```

### Comparing `generate_temp_table_sql-0.4.3/README.md` & `generate_temp_table_sql-0.4.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 #### Additional Options
 ```sh
 
 --o The path to the output SQL file.  Defaults to the director you call the command in.
 --overwrite: Allow overwriting the output file if it exists.
 --table_name: Specify the name of the temporary table to create.
 --column_type: Specify the data type of the columns in the temporary table. Defaults to TEXT which works for Redshift and Snowflake. Use STRING for BigQuery.
+--batch_size: Specify the number of rows inserted per insert statement.  If present, it creates multiple insert statements based on the batch size specified.
 ```
 
 #### Example
 Assume you have a CSV file example.csv with the following content:
 
 ```sh
 name,age,city
@@ -79,14 +80,16 @@
 
 --Insert Data SQL:
 INSERT INTO my_temp_table (name, age, city) VALUES 
     ('John', '30', 'New York'),
     ('Jane', '25', 'Los Angeles');
 ```
 
+All arguments are optional except the csv
+
 #### Running Tests
 To run the tests, use the following command:
 
 ```sh
 python -m unittest discover -s tests
 ```
```

#### html2text {}

```diff
@@ -23,24 +23,26 @@
 you can use the `generate-tt-sql` command to generate SQL statements from a CSV
 file. #### Basic Usage To generate SQL statements and save them to a file:
 ```sh generate-tt-sql path/to/your/file.csv ``` #### Additional Options ```sh -
 -o The path to the output SQL file. Defaults to the director you call the
 command in. --overwrite: Allow overwriting the output file if it exists. --
 table_name: Specify the name of the temporary table to create. --column_type:
 Specify the data type of the columns in the temporary table. Defaults to TEXT
-which works for Redshift and Snowflake. Use STRING for BigQuery. ``` ####
+which works for Redshift and Snowflake. Use STRING for BigQuery. --batch_size:
+Specify the number of rows inserted per insert statement. If present, it
+creates multiple insert statements based on the batch size specified. ``` ####
 Example Assume you have a CSV file example.csv with the following content:
 ```sh name,age,city John,30,New York Jane,25,Los Angeles ``` Run the following
 command to generate SQL statements: ```sh generate-tt-sql example.csv -
 o output.sql --table_name my_temp_table --column_type STRING ``` The output.sql
 file will contain: ```sh CREATE TEMP TABLE my_temp_table ( name STRING, age
 STRING, city STRING ); --Insert Data SQL: INSERT INTO my_temp_table (name, age,
-city) VALUES ('John', '30', 'New York'), ('Jane', '25', 'Los Angeles'); ```
-#### Running Tests To run the tests, use the following command: ```sh python -
-m unittest discover -s tests ``` #### Contributing Contributions are welcome!
-Please follow these steps: 1. Fork the repository 2. Create a new branch (git
-checkout -b feature-branch) 3. Commit your changes (git commit -am 'Add new
-feature') 4. Push to the branch (git push origin feature-branch) 5. Create a
-new Pull Request #### License This project is licensed under the MIT License -
-see the LICENSE file for details. #### Author Ryan Waldorf -
-ryan@ryanwaldorf.com
+city) VALUES ('John', '30', 'New York'), ('Jane', '25', 'Los Angeles'); ``` All
+arguments are optional except the csv #### Running Tests To run the tests, use
+the following command: ```sh python -m unittest discover -s tests ``` ####
+Contributing Contributions are welcome! Please follow these steps: 1. Fork the
+repository 2. Create a new branch (git checkout -b feature-branch) 3. Commit
+your changes (git commit -am 'Add new feature') 4. Push to the branch (git push
+origin feature-branch) 5. Create a new Pull Request #### License This project
+is licensed under the MIT License - see the LICENSE file for details. ####
+Author Ryan Waldorf - ryan@ryanwaldorf.com
 _G_i_t_H_u_b _L_i_n_k_e_d_I_n
```

### Comparing `generate_temp_table_sql-0.4.3/generate_temp_table_sql/cli.py` & `generate_temp_table_sql-0.4.4/generate_temp_table_sql/cli.py`

 * *Files identical despite different names*

### Comparing `generate_temp_table_sql-0.4.3/generate_temp_table_sql/sql_generator.py` & `generate_temp_table_sql-0.4.4/generate_temp_table_sql/sql_generator.py`

 * *Files identical despite different names*

### Comparing `generate_temp_table_sql-0.4.3/generate_temp_table_sql.egg-info/PKG-INFO` & `generate_temp_table_sql-0.4.4/generate_temp_table_sql.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6765 6e65  : 2.1.Name: gene
 00000020: 7261 7465 2d74 656d 702d 7461 626c 652d  rate-temp-table-
 00000030: 7371 6c0a 5665 7273 696f 6e3a 2030 2e34  sql.Version: 0.4
-00000040: 2e33 0a53 756d 6d61 7279 3a20 4120 7061  .3.Summary: A pa
+00000040: 2e34 0a53 756d 6d61 7279 3a20 4120 7061  .4.Summary: A pa
 00000050: 636b 6167 6520 746f 2067 656e 6572 6174  ckage to generat
 00000060: 6520 5351 4c20 7374 6174 656d 656e 7473  e SQL statements
 00000070: 2066 726f 6d20 4353 5620 6669 6c65 730a   from CSV files.
 00000080: 486f 6d65 2d70 6167 653a 2068 7474 7073  Home-page: https
 00000090: 3a2f 2f67 6974 6875 622e 636f 6d2f 7279  ://github.com/ry
 000000a0: 616e 7761 6c64 6f72 662f 6765 6e65 7261  anwaldorf/genera
 000000b0: 7465 5f74 656d 705f 7461 626c 655f 7371  te_temp_table_sq
@@ -175,88 +175,101 @@
 00000ae0: 6865 2063 6f6c 756d 6e73 2069 6e20 7468  he columns in th
 00000af0: 6520 7465 6d70 6f72 6172 7920 7461 626c  e temporary tabl
 00000b00: 652e 2044 6566 6175 6c74 7320 746f 2054  e. Defaults to T
 00000b10: 4558 5420 7768 6963 6820 776f 726b 7320  EXT which works 
 00000b20: 666f 7220 5265 6473 6869 6674 2061 6e64  for Redshift and
 00000b30: 2053 6e6f 7766 6c61 6b65 2e20 5573 6520   Snowflake. Use 
 00000b40: 5354 5249 4e47 2066 6f72 2042 6967 5175  STRING for BigQu
-00000b50: 6572 792e 0a60 6060 0a0a 2323 2323 2045  ery..```..#### E
-00000b60: 7861 6d70 6c65 0a41 7373 756d 6520 796f  xample.Assume yo
-00000b70: 7520 6861 7665 2061 2043 5356 2066 696c  u have a CSV fil
-00000b80: 6520 6578 616d 706c 652e 6373 7620 7769  e example.csv wi
-00000b90: 7468 2074 6865 2066 6f6c 6c6f 7769 6e67  th the following
-00000ba0: 2063 6f6e 7465 6e74 3a0a 0a60 6060 7368   content:..```sh
-00000bb0: 0a6e 616d 652c 6167 652c 6369 7479 0a4a  .name,age,city.J
-00000bc0: 6f68 6e2c 3330 2c4e 6577 2059 6f72 6b0a  ohn,30,New York.
-00000bd0: 4a61 6e65 2c32 352c 4c6f 7320 416e 6765  Jane,25,Los Ange
-00000be0: 6c65 730a 6060 600a 0a52 756e 2074 6865  les.```..Run the
-00000bf0: 2066 6f6c 6c6f 7769 6e67 2063 6f6d 6d61   following comma
-00000c00: 6e64 2074 6f20 6765 6e65 7261 7465 2053  nd to generate S
-00000c10: 514c 2073 7461 7465 6d65 6e74 733a 0a0a  QL statements:..
-00000c20: 6060 6073 680a 6765 6e65 7261 7465 2d74  ```sh.generate-t
-00000c30: 742d 7371 6c20 6578 616d 706c 652e 6373  t-sql example.cs
-00000c40: 7620 2d6f 206f 7574 7075 742e 7371 6c20  v -o output.sql 
-00000c50: 2d2d 7461 626c 655f 6e61 6d65 206d 795f  --table_name my_
-00000c60: 7465 6d70 5f74 6162 6c65 202d 2d63 6f6c  temp_table --col
-00000c70: 756d 6e5f 7479 7065 2053 5452 494e 470a  umn_type STRING.
-00000c80: 6060 600a 0a54 6865 206f 7574 7075 742e  ```..The output.
-00000c90: 7371 6c20 6669 6c65 2077 696c 6c20 636f  sql file will co
-00000ca0: 6e74 6169 6e3a 0a0a 6060 6073 680a 4352  ntain:..```sh.CR
-00000cb0: 4541 5445 2054 454d 5020 5441 424c 4520  EATE TEMP TABLE 
-00000cc0: 6d79 5f74 656d 705f 7461 626c 6520 280a  my_temp_table (.
-00000cd0: 2020 2020 6e61 6d65 2053 5452 494e 472c      name STRING,
-00000ce0: 0a20 2020 2061 6765 2053 5452 494e 472c  .    age STRING,
-00000cf0: 0a20 2020 2063 6974 7920 5354 5249 4e47  .    city STRING
-00000d00: 0a29 3b0a 0a2d 2d49 6e73 6572 7420 4461  .);..--Insert Da
-00000d10: 7461 2053 514c 3a0a 494e 5345 5254 2049  ta SQL:.INSERT I
-00000d20: 4e54 4f20 6d79 5f74 656d 705f 7461 626c  NTO my_temp_tabl
-00000d30: 6520 286e 616d 652c 2061 6765 2c20 6369  e (name, age, ci
-00000d40: 7479 2920 5641 4c55 4553 200a 2020 2020  ty) VALUES .    
-00000d50: 2827 4a6f 686e 272c 2027 3330 272c 2027  ('John', '30', '
-00000d60: 4e65 7720 596f 726b 2729 2c0a 2020 2020  New York'),.    
-00000d70: 2827 4a61 6e65 272c 2027 3235 272c 2027  ('Jane', '25', '
-00000d80: 4c6f 7320 416e 6765 6c65 7327 293b 0a60  Los Angeles');.`
-00000d90: 6060 0a0a 2323 2323 2052 756e 6e69 6e67  ``..#### Running
-00000da0: 2054 6573 7473 0a54 6f20 7275 6e20 7468   Tests.To run th
-00000db0: 6520 7465 7374 732c 2075 7365 2074 6865  e tests, use the
-00000dc0: 2066 6f6c 6c6f 7769 6e67 2063 6f6d 6d61   following comma
-00000dd0: 6e64 3a0a 0a60 6060 7368 0a70 7974 686f  nd:..```sh.pytho
-00000de0: 6e20 2d6d 2075 6e69 7474 6573 7420 6469  n -m unittest di
-00000df0: 7363 6f76 6572 202d 7320 7465 7374 730a  scover -s tests.
-00000e00: 6060 600a 0a23 2323 2320 436f 6e74 7269  ```..#### Contri
-00000e10: 6275 7469 6e67 0a43 6f6e 7472 6962 7574  buting.Contribut
-00000e20: 696f 6e73 2061 7265 2077 656c 636f 6d65  ions are welcome
-00000e30: 2120 506c 6561 7365 2066 6f6c 6c6f 7720  ! Please follow 
-00000e40: 7468 6573 6520 7374 6570 733a 0a0a 312e  these steps:..1.
-00000e50: 2046 6f72 6b20 7468 6520 7265 706f 7369   Fork the reposi
-00000e60: 746f 7279 0a32 2e20 4372 6561 7465 2061  tory.2. Create a
-00000e70: 206e 6577 2062 7261 6e63 6820 2867 6974   new branch (git
-00000e80: 2063 6865 636b 6f75 7420 2d62 2066 6561   checkout -b fea
-00000e90: 7475 7265 2d62 7261 6e63 6829 0a33 2e20  ture-branch).3. 
-00000ea0: 436f 6d6d 6974 2079 6f75 7220 6368 616e  Commit your chan
-00000eb0: 6765 7320 2867 6974 2063 6f6d 6d69 7420  ges (git commit 
-00000ec0: 2d61 6d20 2741 6464 206e 6577 2066 6561  -am 'Add new fea
-00000ed0: 7475 7265 2729 0a34 2e20 5075 7368 2074  ture').4. Push t
-00000ee0: 6f20 7468 6520 6272 616e 6368 2028 6769  o the branch (gi
-00000ef0: 7420 7075 7368 206f 7269 6769 6e20 6665  t push origin fe
-00000f00: 6174 7572 652d 6272 616e 6368 290a 352e  ature-branch).5.
-00000f10: 2043 7265 6174 6520 6120 6e65 7720 5075   Create a new Pu
-00000f20: 6c6c 2052 6571 7565 7374 0a0a 2323 2323  ll Request..####
-00000f30: 204c 6963 656e 7365 0a54 6869 7320 7072   License.This pr
-00000f40: 6f6a 6563 7420 6973 206c 6963 656e 7365  oject is license
-00000f50: 6420 756e 6465 7220 7468 6520 4d49 5420  d under the MIT 
-00000f60: 4c69 6365 6e73 6520 2d20 7365 6520 7468  License - see th
-00000f70: 6520 4c49 4345 4e53 4520 6669 6c65 2066  e LICENSE file f
-00000f80: 6f72 2064 6574 6169 6c73 2e0a 0a23 2323  or details...###
-00000f90: 2320 4175 7468 6f72 0a52 7961 6e20 5761  # Author.Ryan Wa
-00000fa0: 6c64 6f72 6620 2d20 7279 616e 4072 7961  ldorf - ryan@rya
-00000fb0: 6e77 616c 646f 7266 2e63 6f6d 3c62 722f  nwaldorf.com<br/
-00000fc0: 3e0a 3c61 2068 7265 663d 2268 7474 7073  >.<a href="https
-00000fd0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7279  ://github.com/ry
-00000fe0: 616e 7761 6c64 6f72 6622 2074 6172 6765  anwaldorf" targe
-00000ff0: 743d 225f 626c 616e 6b22 3e47 6974 4875  t="_blank">GitHu
-00001000: 623c 2f61 3e0a 3c61 2068 7265 663d 2268  b</a>.<a href="h
-00001010: 7474 7073 3a2f 2f77 7777 2e6c 696e 6b65  ttps://www.linke
-00001020: 6469 6e2e 636f 6d2f 696e 2f72 7961 6e2d  din.com/in/ryan-
-00001030: 7761 6c64 6f72 662f 2220 7461 7267 6574  waldorf/" target
-00001040: 3d22 5f62 6c61 6e6b 223e 4c69 6e6b 6564  ="_blank">Linked
-00001050: 496e 3c2f 613e 0a0a                      In</a>..
+00000b50: 6572 792e 0a2d 2d62 6174 6368 5f73 697a  ery..--batch_siz
+00000b60: 653a 2053 7065 6369 6679 2074 6865 206e  e: Specify the n
+00000b70: 756d 6265 7220 6f66 2072 6f77 7320 696e  umber of rows in
+00000b80: 7365 7274 6564 2070 6572 2069 6e73 6572  serted per inser
+00000b90: 7420 7374 6174 656d 656e 742e 2020 4966  t statement.  If
+00000ba0: 2070 7265 7365 6e74 2c20 6974 2063 7265   present, it cre
+00000bb0: 6174 6573 206d 756c 7469 706c 6520 696e  ates multiple in
+00000bc0: 7365 7274 2073 7461 7465 6d65 6e74 7320  sert statements 
+00000bd0: 6261 7365 6420 6f6e 2074 6865 2062 6174  based on the bat
+00000be0: 6368 2073 697a 6520 7370 6563 6966 6965  ch size specifie
+00000bf0: 642e 0a60 6060 0a0a 2323 2323 2045 7861  d..```..#### Exa
+00000c00: 6d70 6c65 0a41 7373 756d 6520 796f 7520  mple.Assume you 
+00000c10: 6861 7665 2061 2043 5356 2066 696c 6520  have a CSV file 
+00000c20: 6578 616d 706c 652e 6373 7620 7769 7468  example.csv with
+00000c30: 2074 6865 2066 6f6c 6c6f 7769 6e67 2063   the following c
+00000c40: 6f6e 7465 6e74 3a0a 0a60 6060 7368 0a6e  ontent:..```sh.n
+00000c50: 616d 652c 6167 652c 6369 7479 0a4a 6f68  ame,age,city.Joh
+00000c60: 6e2c 3330 2c4e 6577 2059 6f72 6b0a 4a61  n,30,New York.Ja
+00000c70: 6e65 2c32 352c 4c6f 7320 416e 6765 6c65  ne,25,Los Angele
+00000c80: 730a 6060 600a 0a52 756e 2074 6865 2066  s.```..Run the f
+00000c90: 6f6c 6c6f 7769 6e67 2063 6f6d 6d61 6e64  ollowing command
+00000ca0: 2074 6f20 6765 6e65 7261 7465 2053 514c   to generate SQL
+00000cb0: 2073 7461 7465 6d65 6e74 733a 0a0a 6060   statements:..``
+00000cc0: 6073 680a 6765 6e65 7261 7465 2d74 742d  `sh.generate-tt-
+00000cd0: 7371 6c20 6578 616d 706c 652e 6373 7620  sql example.csv 
+00000ce0: 2d6f 206f 7574 7075 742e 7371 6c20 2d2d  -o output.sql --
+00000cf0: 7461 626c 655f 6e61 6d65 206d 795f 7465  table_name my_te
+00000d00: 6d70 5f74 6162 6c65 202d 2d63 6f6c 756d  mp_table --colum
+00000d10: 6e5f 7479 7065 2053 5452 494e 470a 6060  n_type STRING.``
+00000d20: 600a 0a54 6865 206f 7574 7075 742e 7371  `..The output.sq
+00000d30: 6c20 6669 6c65 2077 696c 6c20 636f 6e74  l file will cont
+00000d40: 6169 6e3a 0a0a 6060 6073 680a 4352 4541  ain:..```sh.CREA
+00000d50: 5445 2054 454d 5020 5441 424c 4520 6d79  TE TEMP TABLE my
+00000d60: 5f74 656d 705f 7461 626c 6520 280a 2020  _temp_table (.  
+00000d70: 2020 6e61 6d65 2053 5452 494e 472c 0a20    name STRING,. 
+00000d80: 2020 2061 6765 2053 5452 494e 472c 0a20     age STRING,. 
+00000d90: 2020 2063 6974 7920 5354 5249 4e47 0a29     city STRING.)
+00000da0: 3b0a 0a2d 2d49 6e73 6572 7420 4461 7461  ;..--Insert Data
+00000db0: 2053 514c 3a0a 494e 5345 5254 2049 4e54   SQL:.INSERT INT
+00000dc0: 4f20 6d79 5f74 656d 705f 7461 626c 6520  O my_temp_table 
+00000dd0: 286e 616d 652c 2061 6765 2c20 6369 7479  (name, age, city
+00000de0: 2920 5641 4c55 4553 200a 2020 2020 2827  ) VALUES .    ('
+00000df0: 4a6f 686e 272c 2027 3330 272c 2027 4e65  John', '30', 'Ne
+00000e00: 7720 596f 726b 2729 2c0a 2020 2020 2827  w York'),.    ('
+00000e10: 4a61 6e65 272c 2027 3235 272c 2027 4c6f  Jane', '25', 'Lo
+00000e20: 7320 416e 6765 6c65 7327 293b 0a60 6060  s Angeles');.```
+00000e30: 0a0a 416c 6c20 6172 6775 6d65 6e74 7320  ..All arguments 
+00000e40: 6172 6520 6f70 7469 6f6e 616c 2065 7863  are optional exc
+00000e50: 6570 7420 7468 6520 6373 760a 0a23 2323  ept the csv..###
+00000e60: 2320 5275 6e6e 696e 6720 5465 7374 730a  # Running Tests.
+00000e70: 546f 2072 756e 2074 6865 2074 6573 7473  To run the tests
+00000e80: 2c20 7573 6520 7468 6520 666f 6c6c 6f77  , use the follow
+00000e90: 696e 6720 636f 6d6d 616e 643a 0a0a 6060  ing command:..``
+00000ea0: 6073 680a 7079 7468 6f6e 202d 6d20 756e  `sh.python -m un
+00000eb0: 6974 7465 7374 2064 6973 636f 7665 7220  ittest discover 
+00000ec0: 2d73 2074 6573 7473 0a60 6060 0a0a 2323  -s tests.```..##
+00000ed0: 2323 2043 6f6e 7472 6962 7574 696e 670a  ## Contributing.
+00000ee0: 436f 6e74 7269 6275 7469 6f6e 7320 6172  Contributions ar
+00000ef0: 6520 7765 6c63 6f6d 6521 2050 6c65 6173  e welcome! Pleas
+00000f00: 6520 666f 6c6c 6f77 2074 6865 7365 2073  e follow these s
+00000f10: 7465 7073 3a0a 0a31 2e20 466f 726b 2074  teps:..1. Fork t
+00000f20: 6865 2072 6570 6f73 6974 6f72 790a 322e  he repository.2.
+00000f30: 2043 7265 6174 6520 6120 6e65 7720 6272   Create a new br
+00000f40: 616e 6368 2028 6769 7420 6368 6563 6b6f  anch (git checko
+00000f50: 7574 202d 6220 6665 6174 7572 652d 6272  ut -b feature-br
+00000f60: 616e 6368 290a 332e 2043 6f6d 6d69 7420  anch).3. Commit 
+00000f70: 796f 7572 2063 6861 6e67 6573 2028 6769  your changes (gi
+00000f80: 7420 636f 6d6d 6974 202d 616d 2027 4164  t commit -am 'Ad
+00000f90: 6420 6e65 7720 6665 6174 7572 6527 290a  d new feature').
+00000fa0: 342e 2050 7573 6820 746f 2074 6865 2062  4. Push to the b
+00000fb0: 7261 6e63 6820 2867 6974 2070 7573 6820  ranch (git push 
+00000fc0: 6f72 6967 696e 2066 6561 7475 7265 2d62  origin feature-b
+00000fd0: 7261 6e63 6829 0a35 2e20 4372 6561 7465  ranch).5. Create
+00000fe0: 2061 206e 6577 2050 756c 6c20 5265 7175   a new Pull Requ
+00000ff0: 6573 740a 0a23 2323 2320 4c69 6365 6e73  est..#### Licens
+00001000: 650a 5468 6973 2070 726f 6a65 6374 2069  e.This project i
+00001010: 7320 6c69 6365 6e73 6564 2075 6e64 6572  s licensed under
+00001020: 2074 6865 204d 4954 204c 6963 656e 7365   the MIT License
+00001030: 202d 2073 6565 2074 6865 204c 4943 454e   - see the LICEN
+00001040: 5345 2066 696c 6520 666f 7220 6465 7461  SE file for deta
+00001050: 696c 732e 0a0a 2323 2323 2041 7574 686f  ils...#### Autho
+00001060: 720a 5279 616e 2057 616c 646f 7266 202d  r.Ryan Waldorf -
+00001070: 2072 7961 6e40 7279 616e 7761 6c64 6f72   ryan@ryanwaldor
+00001080: 662e 636f 6d3c 6272 2f3e 0a3c 6120 6872  f.com<br/>.<a hr
+00001090: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+000010a0: 7562 2e63 6f6d 2f72 7961 6e77 616c 646f  ub.com/ryanwaldo
+000010b0: 7266 2220 7461 7267 6574 3d22 5f62 6c61  rf" target="_bla
+000010c0: 6e6b 223e 4769 7448 7562 3c2f 613e 0a3c  nk">GitHub</a>.<
+000010d0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+000010e0: 7777 772e 6c69 6e6b 6564 696e 2e63 6f6d  www.linkedin.com
+000010f0: 2f69 6e2f 7279 616e 2d77 616c 646f 7266  /in/ryan-waldorf
+00001100: 2f22 2074 6172 6765 743d 225f 626c 616e  /" target="_blan
+00001110: 6b22 3e4c 696e 6b65 6449 6e3c 2f61 3e0a  k">LinkedIn</a>.
+00001120: 0a                                       .
```

### Comparing `generate_temp_table_sql-0.4.3/generate_temp_table_sql.egg-info/SOURCES.txt` & `generate_temp_table_sql-0.4.4/generate_temp_table_sql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `generate_temp_table_sql-0.4.3/setup.py` & `generate_temp_table_sql-0.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='generate_temp_table_sql',
-    version='0.4.3',
+    version='0.4.4',
     packages=find_packages(),
     install_requires=[
         'pandas',
     ],
     entry_points={
         'console_scripts': [
             'generate-tt-sql=generate_temp_table_sql.cli:main',
```

### Comparing `generate_temp_table_sql-0.4.3/tests/test_sql_generator.py` & `generate_temp_table_sql-0.4.4/tests/test_sql_generator.py`

 * *Files identical despite different names*

