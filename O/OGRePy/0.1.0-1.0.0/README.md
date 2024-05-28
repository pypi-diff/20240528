# Comparing `tmp/OGRePy-0.1.0.tar.gz` & `tmp/ogrepy-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OGRePy-0.1.0.tar", last modified: Sat Aug 20 00:47:10 2022, max compression
+gzip compressed data, was "ogrepy-1.0.0.tar", last modified: Tue May 28 02:22:55 2024, max compression
```

## Comparing `OGRePy-0.1.0.tar` & `ogrepy-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,13 @@
-drwxrwxrwx   0        0        0        0 2022-08-20 00:47:10.971004 OGRePy-0.1.0/
--rw-rw-rw-   0        0        0     1108 2022-08-19 21:19:10.000000 OGRePy-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0     1463 2022-08-20 00:47:10.971004 OGRePy-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      524 2022-08-20 00:46:21.000000 OGRePy-0.1.0/README.md
--rw-rw-rw-   0        0        0       96 2022-08-20 00:02:10.000000 OGRePy-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0     1009 2022-08-20 00:47:10.973003 OGRePy-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-08-20 00:47:10.951004 OGRePy-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2022-08-20 00:47:10.956004 OGRePy-0.1.0/src/OGRePy/
--rw-rw-rw-   0        0        0        0 2022-08-20 00:05:09.000000 OGRePy-0.1.0/src/OGRePy/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-20 00:47:10.970005 OGRePy-0.1.0/src/OGRePy.egg-info/
--rw-rw-rw-   0        0        0     1463 2022-08-20 00:47:10.000000 OGRePy-0.1.0/src/OGRePy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2022-08-20 00:47:10.000000 OGRePy-0.1.0/src/OGRePy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-20 00:47:10.000000 OGRePy-0.1.0/src/OGRePy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2022-08-20 00:47:10.000000 OGRePy-0.1.0/src/OGRePy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-08-20 00:47:10.000000 OGRePy-0.1.0/src/OGRePy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-28 02:22:55.614122 ogrepy-1.0.0/
+-rw-rw-rw-   0        0        0     1092 2024-05-28 02:16:22.000000 ogrepy-1.0.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     3060 2024-05-28 02:22:55.614122 ogrepy-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      536 2024-05-28 02:17:38.000000 ogrepy-1.0.0/README.md
+-rw-rw-rw-   0        0        0     1289 2024-05-28 02:17:06.000000 ogrepy-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1008 2024-05-28 02:22:55.620122 ogrepy-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-28 02:22:55.598123 ogrepy-1.0.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-28 02:22:55.613122 ogrepy-1.0.0/src/OGRePy.egg-info/
+-rw-rw-rw-   0        0        0     3060 2024-05-28 02:22:55.000000 ogrepy-1.0.0/src/OGRePy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      215 2024-05-28 02:22:55.000000 ogrepy-1.0.0/src/OGRePy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 02:22:55.000000 ogrepy-1.0.0/src/OGRePy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-28 02:22:55.000000 ogrepy-1.0.0/src/OGRePy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 02:22:55.000000 ogrepy-1.0.0/src/OGRePy.egg-info/top_level.txt
```

### Comparing `OGRePy-0.1.0/LICENSE.txt` & `ogrepy-1.0.0/LICENSE.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Barak Shoshany and Jared Wogan
+Copyright (c) 2024 Barak Shoshany
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `OGRePy-0.1.0/setup.cfg` & `ogrepy-1.0.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -7,58 +7,57 @@
 00000060: 5061 636b 6167 6520 666f 7220 5079 7468  Package for Pyth
 00000070: 6f6e 0d0a 6c6f 6e67 5f64 6573 6372 6970  on..long_descrip
 00000080: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
 00000090: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
 000000a0: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
 000000b0: 5f74 7970 6520 3d20 7465 7874 2f6d 6172  _type = text/mar
 000000c0: 6b64 6f77 6e0d 0a61 7574 686f 7220 3d20  kdown..author = 
-000000d0: 4261 7261 6b20 5368 6f73 6861 6e79 2061  Barak Shoshany a
-000000e0: 6e64 204a 6172 6564 2057 6f67 616e 0d0a  nd Jared Wogan..
-000000f0: 6175 7468 6f72 5f65 6d61 696c 203d 2062  author_email = b
-00000100: 6172 616b 7368 4067 6d61 696c 2e63 6f6d  araksh@gmail.com
-00000110: 0d0a 6c69 6365 6e73 6520 3d20 4d49 540d  ..license = MIT.
-00000120: 0a6c 6963 656e 7365 5f66 696c 6520 3d20  .license_file = 
-00000130: 4c49 4345 4e53 452e 7478 740d 0a75 726c  LICENSE.txt..url
-00000140: 203d 2068 7474 7073 3a2f 2f62 6172 616b   = https://barak
-00000150: 7368 2e63 6f6d 2f0d 0a70 6c61 7466 6f72  sh.com/..platfor
-00000160: 6d73 203d 2075 6e69 782c 206c 696e 7578  ms = unix, linux
-00000170: 2c20 6f73 782c 2063 7967 7769 6e2c 2077  , osx, cygwin, w
-00000180: 696e 3332 0d0a 6b65 7977 6f72 6473 203d  in32..keywords =
-00000190: 2073 6369 656e 7469 6669 632d 636f 6d70   scientific-comp
-000001a0: 7574 696e 672c 2064 6966 6665 7265 6e74  uting, different
-000001b0: 6961 6c2d 6765 6f6d 6574 7279 2c20 7465  ial-geometry, te
-000001c0: 6e73 6f72 2c20 7465 6e73 6f72 732c 2067  nsor, tensors, g
-000001d0: 656e 6572 616c 2d72 656c 6174 6976 6974  eneral-relativit
-000001e0: 790d 0a63 6c61 7373 6966 6965 7273 203d  y..classifiers =
-000001f0: 200d 0a09 5072 6f67 7261 6d6d 696e 6720   ...Programming 
-00000200: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000210: 6f6e 203a 3a20 330d 0a09 5072 6f67 7261  on :: 3...Progra
-00000220: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000230: 3a20 5079 7468 6f6e 203a 3a20 332e 380d  : Python :: 3.8.
-00000240: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-00000250: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000260: 203a 3a20 332e 390d 0a09 5072 6f67 7261   :: 3.9...Progra
-00000270: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000280: 3a20 5079 7468 6f6e 203a 3a20 332e 3130  : Python :: 3.10
-00000290: 0d0a 094c 6963 656e 7365 203a 3a20 4f53  ...License :: OS
-000002a0: 4920 4170 7072 6f76 6564 203a 3a20 4d49  I Approved :: MI
-000002b0: 5420 4c69 6365 6e73 650d 0a09 4f70 6572  T License...Oper
-000002c0: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
-000002d0: 4f53 2049 6e64 6570 656e 6465 6e74 0d0a  OS Independent..
-000002e0: 0954 6f70 6963 203a 3a20 5363 6965 6e74  .Topic :: Scient
-000002f0: 6966 6963 2f45 6e67 696e 6565 7269 6e67  ific/Engineering
-00000300: 203a 3a20 4d61 7468 656d 6174 6963 730d   :: Mathematics.
-00000310: 0a09 546f 7069 6320 3a3a 2053 6369 656e  ..Topic :: Scien
-00000320: 7469 6669 632f 456e 6769 6e65 6572 696e  tific/Engineerin
-00000330: 6720 3a3a 2050 6879 7369 6373 0d0a 0d0a  g :: Physics....
-00000340: 5b6f 7074 696f 6e73 5d0d 0a70 6163 6b61  [options]..packa
-00000350: 6765 7320 3d20 0d0a 094f 4752 6550 790d  ges = ...OGRePy.
-00000360: 0a69 6e73 7461 6c6c 5f72 6571 7569 7265  .install_require
-00000370: 7320 3d20 0d0a 0949 5079 7468 6f6e 3e3d  s = ...IPython>=
-00000380: 372e 3130 2e30 0d0a 0973 796d 7079 3e3d  7.10.0...sympy>=
-00000390: 312e 380d 0a70 7974 686f 6e5f 7265 7175  1.8..python_requ
-000003a0: 6972 6573 203d 203e 3d33 2e38 0d0a 7061  ires = >=3.8..pa
-000003b0: 636b 6167 655f 6469 7220 3d20 0d0a 093d  ckage_dir = ...=
-000003c0: 7372 630d 0a0d 0a5b 6567 675f 696e 666f  src....[egg_info
-000003d0: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
-000003e0: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
-000003f0: 0a                                       .
+000000d0: 4261 7261 6b20 5368 6f73 6861 6e79 0d0a  Barak Shoshany..
+000000e0: 6175 7468 6f72 5f65 6d61 696c 203d 2062  author_email = b
+000000f0: 6172 616b 7368 4067 6d61 696c 2e63 6f6d  araksh@gmail.com
+00000100: 0d0a 6c69 6365 6e73 6520 3d20 4d49 540d  ..license = MIT.
+00000110: 0a6c 6963 656e 7365 5f66 696c 6520 3d20  .license_file = 
+00000120: 4c49 4345 4e53 452e 7478 740d 0a75 726c  LICENSE.txt..url
+00000130: 203d 2068 7474 7073 3a2f 2f67 6974 6875   = https://githu
+00000140: 622e 636f 6d2f 6273 686f 7368 616e 792f  b.com/bshoshany/
+00000150: 4f47 5265 5079 0d0a 706c 6174 666f 726d  OGRePy..platform
+00000160: 7320 3d20 756e 6978 2c20 6c69 6e75 782c  s = unix, linux,
+00000170: 206f 7378 2c20 6379 6777 696e 2c20 7769   osx, cygwin, wi
+00000180: 6e33 320d 0a6b 6579 776f 7264 7320 3d20  n32..keywords = 
+00000190: 7363 6965 6e74 6966 6963 2d63 6f6d 7075  scientific-compu
+000001a0: 7469 6e67 2c20 6469 6666 6572 656e 7469  ting, differenti
+000001b0: 616c 2d67 656f 6d65 7472 792c 2074 656e  al-geometry, ten
+000001c0: 736f 722c 2074 656e 736f 7273 2c20 6765  sor, tensors, ge
+000001d0: 6e65 7261 6c2d 7265 6c61 7469 7669 7479  neral-relativity
+000001e0: 0d0a 636c 6173 7369 6669 6572 7320 3d20  ..classifiers = 
+000001f0: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
+00000200: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00000210: 6e20 3a3a 2033 0d0a 0950 726f 6772 616d  n :: 3...Program
+00000220: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000230: 2050 7974 686f 6e20 3a3a 2033 2e38 0d0a   Python :: 3.8..
+00000240: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
+00000250: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000260: 3a3a 2033 2e39 0d0a 0950 726f 6772 616d  :: 3.9...Program
+00000270: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000280: 2050 7974 686f 6e20 3a3a 2033 2e31 300d   Python :: 3.10.
+00000290: 0a09 4c69 6365 6e73 6520 3a3a 204f 5349  ..License :: OSI
+000002a0: 2041 7070 726f 7665 6420 3a3a 204d 4954   Approved :: MIT
+000002b0: 204c 6963 656e 7365 0d0a 094f 7065 7261   License...Opera
+000002c0: 7469 6e67 2053 7973 7465 6d20 3a3a 204f  ting System :: O
+000002d0: 5320 496e 6465 7065 6e64 656e 740d 0a09  S Independent...
+000002e0: 546f 7069 6320 3a3a 2053 6369 656e 7469  Topic :: Scienti
+000002f0: 6669 632f 456e 6769 6e65 6572 696e 6720  fic/Engineering 
+00000300: 3a3a 204d 6174 6865 6d61 7469 6373 0d0a  :: Mathematics..
+00000310: 0954 6f70 6963 203a 3a20 5363 6965 6e74  .Topic :: Scient
+00000320: 6966 6963 2f45 6e67 696e 6565 7269 6e67  ific/Engineering
+00000330: 203a 3a20 5068 7973 6963 730d 0a0d 0a5b   :: Physics....[
+00000340: 6f70 7469 6f6e 735d 0d0a 7061 636b 6167  options]..packag
+00000350: 6573 203d 200d 0a09 4f47 5265 5079 0d0a  es = ...OGRePy..
+00000360: 696e 7374 616c 6c5f 7265 7175 6972 6573  install_requires
+00000370: 203d 200d 0a09 4950 7974 686f 6e3e 3d37   = ...IPython>=7
+00000380: 2e31 302e 300d 0a09 7379 6d70 793e 3d31  .10.0...sympy>=1
+00000390: 2e38 0d0a 7079 7468 6f6e 5f72 6571 7569  .8..python_requi
+000003a0: 7265 7320 3d20 3e3d 332e 380d 0a70 6163  res = >=3.8..pac
+000003b0: 6b61 6765 5f64 6972 203d 200d 0a09 3d73  kage_dir = ...=s
+000003c0: 7263 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  rc....[egg_info]
+000003d0: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
+000003e0: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
```

