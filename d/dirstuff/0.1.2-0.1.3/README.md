# Comparing `tmp/dirstuff-0.1.2.tar.gz` & `tmp/dirstuff-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dirstuff-0.1.2.tar", max compression
+gzip compressed data, was "dirstuff-0.1.3.tar", max compression
```

## Comparing `dirstuff-0.1.2.tar` & `dirstuff-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     9040 2023-11-11 22:58:09.584727 dirstuff-0.1.2/LICENSE.txt
--rw-r--r--   0        0        0     1840 2023-11-22 06:07:48.118000 dirstuff-0.1.2/README.md
--rw-r--r--   0        0        0       80 2023-11-22 06:07:48.118408 dirstuff-0.1.2/dirstuff/__init__.py
--rw-r--r--   0        0        0       19 2023-11-11 22:58:09.585317 dirstuff-0.1.2/dirstuff/cli/__init__.py
--rw-r--r--   0        0        0     1548 2023-11-21 17:48:47.581504 dirstuff-0.1.2/dirstuff/cli/cli.py
--rw-r--r--   0        0        0       19 2023-11-11 22:58:09.585604 dirstuff-0.1.2/dirstuff/lib/__init__.py
--rw-r--r--   0        0        0       88 2023-11-12 01:24:34.292729 dirstuff-0.1.2/dirstuff/lib/filter_criteria.py
--rw-r--r--   0        0        0     1273 2023-11-11 23:15:49.677121 dirstuff-0.1.2/dirstuff/lib/memory_utilities.py
--rw-r--r--   0        0        0     1146 2023-11-21 17:48:49.387185 dirstuff-0.1.2/dirstuff/lib/parser.py
--rw-r--r--   0        0        0     2226 2023-11-21 17:49:06.686850 dirstuff-0.1.2/dirstuff/lib/tree.py
--rw-r--r--   0        0        0       84 2023-11-22 06:07:48.192080 dirstuff-0.1.2/dirstuff/os/__init__.py
--rw-r--r--   0        0        0     4810 2023-12-21 01:14:30.445963 dirstuff-0.1.2/dirstuff/os/_filesystem.py
--rw-r--r--   0        0        0     1668 2023-12-21 01:14:37.464526 dirstuff-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2761 1970-01-01 00:00:00.000000 dirstuff-0.1.2/setup.py
--rw-r--r--   0        0        0     2978 1970-01-01 00:00:00.000000 dirstuff-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     9040 2023-11-11 22:58:09.584727 dirstuff-0.1.3/LICENSE.txt
+-rw-r--r--   0        0        0     2670 2024-05-28 05:11:31.661428 dirstuff-0.1.3/README.md
+-rw-r--r--   0        0        0       80 2023-11-22 06:07:48.118408 dirstuff-0.1.3/dirstuff/__init__.py
+-rw-r--r--   0        0        0       19 2023-11-11 22:58:09.585317 dirstuff-0.1.3/dirstuff/cli/__init__.py
+-rw-r--r--   0        0        0     1548 2023-11-21 17:48:47.581504 dirstuff-0.1.3/dirstuff/cli/cli.py
+-rw-r--r--   0        0        0       19 2023-11-11 22:58:09.585604 dirstuff-0.1.3/dirstuff/lib/__init__.py
+-rw-r--r--   0        0        0       88 2023-11-12 01:24:34.292729 dirstuff-0.1.3/dirstuff/lib/filter_criteria.py
+-rw-r--r--   0        0        0     1273 2023-11-11 23:15:49.677121 dirstuff-0.1.3/dirstuff/lib/memory_utilities.py
+-rw-r--r--   0        0        0     1146 2023-11-21 17:48:49.387185 dirstuff-0.1.3/dirstuff/lib/parser.py
+-rw-r--r--   0        0        0     2226 2023-11-21 17:49:06.686850 dirstuff-0.1.3/dirstuff/lib/tree.py
+-rw-r--r--   0        0        0       84 2023-11-22 06:07:48.192080 dirstuff-0.1.3/dirstuff/os/__init__.py
+-rw-r--r--   0        0        0     5450 2024-05-28 05:11:33.093631 dirstuff-0.1.3/dirstuff/os/_filesystem.py
+-rw-r--r--   0        0        0     1662 2024-05-28 05:07:02.231323 dirstuff-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3622 1970-01-01 00:00:00.000000 dirstuff-0.1.3/setup.py
+-rw-r--r--   0        0        0     3802 1970-01-01 00:00:00.000000 dirstuff-0.1.3/PKG-INFO
```

### Comparing `dirstuff-0.1.2/LICENSE.txt` & `dirstuff-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dirstuff-0.1.2/dirstuff/cli/cli.py` & `dirstuff-0.1.3/dirstuff/cli/cli.py`

 * *Files identical despite different names*

### Comparing `dirstuff-0.1.2/dirstuff/lib/memory_utilities.py` & `dirstuff-0.1.3/dirstuff/lib/memory_utilities.py`

 * *Files identical despite different names*

### Comparing `dirstuff-0.1.2/dirstuff/lib/parser.py` & `dirstuff-0.1.3/dirstuff/lib/parser.py`

 * *Files identical despite different names*

### Comparing `dirstuff-0.1.2/dirstuff/lib/tree.py` & `dirstuff-0.1.3/dirstuff/lib/tree.py`

 * *Files identical despite different names*

### Comparing `dirstuff-0.1.2/dirstuff/os/_filesystem.py` & `dirstuff-0.1.3/dirstuff/os/_filesystem.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,26 +33,26 @@
 
 class File(Path):
     def __init__(self, *args: Any, **kwargs: Any):
         super().__init__(*args, **kwargs)
         if self.libpath.exists() and not self.libpath.is_file():
             raise ValueError(f"Tried to create File from non-file path: {self.libpath}")
 
-    def rename(self, new_name: str) -> "File":
-        new_path = self.libpath.parent / new_name
-        if new_name == self.name:
+    def rename(self, new_name: str, same_name_ok: bool = False) -> "File":
+        if new_name == self.name and not same_name_ok:
             raise ValueError(f"No change made to file name: {self.name}")
         if not self.libpath.exists():
             raise FileNotFoundError(f"File does not exist: {self.libpath}")
+        new_path = self.libpath.parent / new_name
         self.libpath = self.libpath.rename(new_path)
         return self
 
-    def rename_regex(self, search: str, replace: str) -> "File":
-        new_name = re.sub(search, replace, self.name)
-        if new_name == self.name:
+    def rename_regex(self, pattern: str, replace: str, same_name_ok: bool = False) -> "File":
+        new_name = re.sub(pattern, replace, self.name)
+        if new_name == self.name and not same_name_ok:
             raise ValueError(f"No change made to file name: {self.name}")
         new_path = self.libpath.parent / new_name
         if not self.libpath.exists():
             raise FileNotFoundError(f"File does not exist: {self.libpath}")
         self.libpath = self.libpath.rename(new_path)
         return self
 
@@ -100,21 +100,29 @@
                 yield File(libpath)
 
     def iter_dirs(self) -> Iterator["Dir"]:
         for libpath in self.libpath.iterdir():
             if libpath.is_dir():
                 yield Dir(libpath)
 
-    def rename(self, new_name: str) -> "Dir":
+    def rename(self, new_name: str, same_name_ok: bool = False) -> "Dir":
+        if new_name == self.name and not same_name_ok:
+            raise ValueError(f"No change made to dir name: {self.name}")
+        if not self.libpath.exists():
+            raise FileNotFoundError(f"Dir does not exist: {self.libpath}")
         new_path = self.libpath.parent / new_name
         self.libpath = self.libpath.rename(new_path)
         return self
 
-    def rename_regex(self, search: str, replace: str) -> "Dir":
-        new_name = re.sub(search, replace, self.name)
+    def rename_regex(self, pattern: str, replace: str, same_name_ok: bool = False) -> "Dir":
+        new_name = re.sub(pattern, replace, self.name)
+        if new_name == self.name and not same_name_ok:
+            raise ValueError(f"No change made to dir name: {self.name}")
+        if not self.libpath.exists():
+            raise FileNotFoundError(f"Dir does not exist: {self.libpath}")
         new_path = self.libpath.parent / new_name
         self.libpath = self.libpath.rename(new_path)
         return self
 
     def move_into(self, dir: "Dir") -> "Dir":
         path = dir.libpath / self.libpath.name
         shutil.move(self.libpath, path)
```

### Comparing `dirstuff-0.1.2/pyproject.toml` & `dirstuff-0.1.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -12,30 +12,30 @@
 ]
 description = "Directory summary tool."
 keywords = ['directory', 'file', 'summary']
 license = "Apache Software License"
 name = "dirstuff"
 readme = "README.md"
 repository = "https://github.com/gregorybchris/dirstuff"
-version = "0.1.2"
+version = "0.1.3"
 
 [[tool.poetry.packages]]
 include = "dirstuff"
 
 [tool.poetry.dependencies]
 click = "^8.1.7"
-python = ">=3.9,<3.13"
+python = ">=3.9"
 colorama = "^0.4.6"
 
 [tool.poetry.group.dev.dependencies]
-black = "^23.9.1"
-mypy = "^1.6.0"
-pylint = "^3.0.1"
-pytest = "^7.1.2"
-semver = "^2.13.0"
+black = "^24.4.2"
+mypy = "^1.10.0"
+pylint = "^3.2.2"
+pytest = "^8.2.1"
+semver = "^3.0.2"
 
 [tool.poetry.scripts]
 dirsum = "dirstuff.cli.cli:main"
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `dirstuff-0.1.2/setup.py` & `dirstuff-0.1.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,173 +1,167 @@
-00000000: 2320 2d2a 2d20 636f 6469 6e67 3a20 7574  # -*- coding: ut
-00000010: 662d 3820 2d2a 2d0a 6672 6f6d 2073 6574  f-8 -*-.from set
-00000020: 7570 746f 6f6c 7320 696d 706f 7274 2073  uptools import s
-00000030: 6574 7570 0a0a 7061 636b 6167 6573 203d  etup..packages =
-00000040: 205c 0a5b 2764 6972 7374 7566 6627 2c20   \.['dirstuff', 
-00000050: 2764 6972 7374 7566 662e 636c 6927 2c20  'dirstuff.cli', 
-00000060: 2764 6972 7374 7566 662e 6c69 6227 2c20  'dirstuff.lib', 
-00000070: 2764 6972 7374 7566 662e 6f73 275d 0a0a  'dirstuff.os']..
-00000080: 7061 636b 6167 655f 6461 7461 203d 205c  package_data = \
-00000090: 0a7b 2727 3a20 5b27 2a27 5d7d 0a0a 696e  .{'': ['*']}..in
-000000a0: 7374 616c 6c5f 7265 7175 6972 6573 203d  stall_requires =
-000000b0: 205c 0a5b 2763 6c69 636b 3e3d 382e 312e   \.['click>=8.1.
-000000c0: 372c 3c39 2e30 2e30 272c 2027 636f 6c6f  7,<9.0.0', 'colo
-000000d0: 7261 6d61 3e3d 302e 342e 362c 3c30 2e35  rama>=0.4.6,<0.5
-000000e0: 2e30 275d 0a0a 656e 7472 795f 706f 696e  .0']..entry_poin
-000000f0: 7473 203d 205c 0a7b 2763 6f6e 736f 6c65  ts = \.{'console
-00000100: 5f73 6372 6970 7473 273a 205b 2764 6972  _scripts': ['dir
-00000110: 7375 6d20 3d20 6469 7273 7475 6666 2e63  sum = dirstuff.c
-00000120: 6c69 2e63 6c69 3a6d 6169 6e27 5d7d 0a0a  li.cli:main']}..
-00000130: 7365 7475 705f 6b77 6172 6773 203d 207b  setup_kwargs = {
-00000140: 0a20 2020 2027 6e61 6d65 273a 2027 6469  .    'name': 'di
-00000150: 7273 7475 6666 272c 0a20 2020 2027 7665  rstuff',.    've
-00000160: 7273 696f 6e27 3a20 2730 2e31 2e32 272c  rsion': '0.1.2',
-00000170: 0a20 2020 2027 6465 7363 7269 7074 696f  .    'descriptio
-00000180: 6e27 3a20 2744 6972 6563 746f 7279 2073  n': 'Directory s
-00000190: 756d 6d61 7279 2074 6f6f 6c2e 272c 0a20  ummary tool.',. 
-000001a0: 2020 2027 6c6f 6e67 5f64 6573 6372 6970     'long_descrip
-000001b0: 7469 6f6e 273a 2027 2320 4469 7253 7475  tion': '# DirStu
-000001c0: 6666 5c6e 5c6e 2323 2053 756d 6d61 7269  ff\n\n## Summari
-000001d0: 7a61 7469 6f6e 5c6e 5c6e 5375 6d6d 6172  zation\n\nSummar
-000001e0: 697a 6520 6120 6469 7265 6374 6f72 7920  ize a directory 
-000001f0: 7265 6375 7273 6976 656c 7920 6279 2066  recursively by f
-00000200: 696c 6520 7369 7a65 2e20 5468 6973 2074  ile size. This t
-00000210: 6f6f 6c20 6361 6e20 6265 2075 7365 6420  ool can be used 
-00000220: 746f 2071 7569 636b 6c79 2073 6561 7263  to quickly searc
-00000230: 6820 6120 6472 6976 6520 666f 7220 6c61  h a drive for la
-00000240: 7267 6520 6669 6c65 7320 7461 6b69 6e67  rge files taking
-00000250: 2075 7020 746f 6f20 6d75 6368 2073 7061   up too much spa
-00000260: 6365 2e5c 6e5c 6e23 2320 496e 7374 616c  ce.\n\n## Instal
-00000270: 6c61 7469 6f6e 5c6e 5c6e 496e 7374 616c  lation\n\nInstal
-00000280: 6c20 7468 6520 6375 7272 656e 7420 5079  l the current Py
-00000290: 5049 2072 656c 6561 7365 3a5c 6e5c 6e60  PI release:\n\n`
-000002a0: 6060 6261 7368 5c6e 7069 7020 696e 7374  ``bash\npip inst
-000002b0: 616c 6c20 6469 7273 7475 6666 5c6e 6060  all dirstuff\n``
-000002c0: 605c 6e5c 6e23 2320 5573 6167 655c 6e5c  `\n\n## Usage\n\
-000002d0: 6e60 6060 6261 7368 5c6e 2320 5275 6e20  n```bash\n# Run 
-000002e0: 7468 6520 7472 6565 2063 6f6d 6d61 6e64  the tree command
-000002f0: 2074 6f20 7375 6d6d 6172 697a 6520 6120   to summarize a 
-00000300: 6469 7265 6374 6f72 795c 6e24 2064 6972  directory\n$ dir
-00000310: 7374 7566 6620 7472 6565 203c 726f 6f74  stuff tree <root
-00000320: 2d64 6972 3e5c 6e5c 6e23 2053 7065 6369  -dir>\n\n# Speci
-00000330: 6679 2074 6865 206d 696e 696d 756d 2066  fy the minimum f
-00000340: 696c 6520 7369 7a65 2028 6465 6661 756c  ile size (defaul
-00000350: 7420 6973 2031 304d 4229 5c6e 2420 6469  t is 10MB)\n$ di
-00000360: 7273 7475 6666 2074 7265 6520 3c72 6f6f  rstuff tree <roo
-00000370: 742d 6469 723e 202d 2d73 697a 6520 3735  t-dir> --size 75
-00000380: 304d 425c 6e24 2064 6972 7374 7566 6620  0MB\n$ dirstuff 
-00000390: 7472 6565 203c 726f 6f74 2d64 6972 3e20  tree <root-dir> 
-000003a0: 2d2d 7369 7a65 2035 304b 425c 6e5c 6e23  --size 50KB\n\n#
-000003b0: 2050 7269 6e74 2066 756c 6c20 6162 736f   Print full abso
-000003c0: 6c75 7465 2070 6174 6873 2074 6f20 6469  lute paths to di
-000003d0: 7265 6374 6f72 6965 7320 696e 7374 6561  rectories instea
-000003e0: 6420 6f66 2064 6972 6563 746f 7279 206e  d of directory n
-000003f0: 616d 6573 5c6e 2420 6469 7273 7475 6666  ames\n$ dirstuff
-00000400: 2074 7265 6520 3c72 6f6f 742d 6469 723e   tree <root-dir>
-00000410: 202d 2d61 6273 6f6c 7574 655c 6e60 6060   --absolute\n```
-00000420: 5c6e 5c6e 6060 6062 6173 685c 6e23 2052  \n\n```bash\n# R
-00000430: 756e 2074 6865 206c 6973 7420 636f 6d6d  un the list comm
-00000440: 616e 6420 746f 2066 696e 6420 616c 6c20  and to find all 
-00000450: 6469 7265 6374 6f72 6965 7320 7769 7468  directories with
-00000460: 2061 206d 6174 6368 696e 6720 6e61 6d65   a matching name
-00000470: 5c6e 2420 6469 7273 7475 6666 206c 6973  \n$ dirstuff lis
-00000480: 7420 3c72 6f6f 742d 6469 723e 203c 6469  t <root-dir> <di
-00000490: 722d 6e61 6d65 3e5c 6e5c 6e23 2053 7065  r-name>\n\n# Spe
-000004a0: 6369 6679 2074 6865 206d 696e 696d 756d  cify the minimum
-000004b0: 2066 696c 6520 7369 7a65 2028 6465 6661   file size (defa
-000004c0: 756c 7420 6973 2031 304d 4229 5c6e 2420  ult is 10MB)\n$ 
-000004d0: 6469 7273 7475 6666 206c 6973 7420 3c72  dirstuff list <r
-000004e0: 6f6f 742d 6469 723e 203c 6469 722d 6e61  oot-dir> <dir-na
-000004f0: 6d65 3e20 2d2d 7369 7a65 2037 3530 4d42  me> --size 750MB
-00000500: 5c6e 2420 6469 7273 7475 6666 206c 6973  \n$ dirstuff lis
-00000510: 7420 3c72 6f6f 742d 6469 723e 203c 6469  t <root-dir> <di
-00000520: 722d 6e61 6d65 3e20 2d2d 7369 7a65 2035  r-name> --size 5
-00000530: 304b 425c 6e60 6060 5c6e 5c6e 6060 6062  0KB\n```\n\n```b
-00000540: 6173 685c 6e66 726f 6d20 6469 7273 7475  ash\nfrom dirstu
-00000550: 6666 2e6f 7320 696d 706f 7274 2050 6174  ff.os import Pat
-00000560: 685c 6e60 6060 5c6e 5c6e 2323 2045 7861  h\n```\n\n## Exa
-00000570: 6d70 6c65 735c 6e5c 6e23 2323 2054 7265  mples\n\n### Tre
-00000580: 655c 6e5c 6e60 6060 6261 7368 5c6e 2320  e\n\n```bash\n# 
-00000590: 5375 6d6d 6172 697a 6520 7468 6520 2f68  Summarize the /h
-000005a0: 6f6d 652f 7573 6572 2f6d 795f 646f 6375  ome/user/my_docu
-000005b0: 6d65 6e74 7320 6469 7265 6374 6f72 795c  ments directory\
-000005c0: 6e23 2073 686f 7769 6e67 206f 6e6c 7920  n# showing only 
-000005d0: 6469 7265 6374 6f72 6965 7320 6772 6561  directories grea
-000005e0: 7465 7220 7468 616e 2032 304d 4220 696e  ter than 20MB in
-000005f0: 2073 697a 655c 6e24 2064 6972 7374 7566   size\n$ dirstuf
-00000600: 6620 7472 6565 202f 686f 6d65 2f75 7365  f tree /home/use
-00000610: 722f 6d79 5f64 6f63 756d 656e 7473 202d  r/my_documents -
-00000620: 2d73 697a 6520 3230 4d42 5c6e 6060 605c  -size 20MB\n```\
-00000630: 6e5c 6e60 6060 7079 7468 6f6e 5c6e 7c2d  n\n```python\n|-
-00000640: 3e20 2036 392e 3020 4742 203e 206d 795f  >  69.0 GB > my_
-00000650: 646f 6375 6d65 6e74 735c 6e20 2020 207c  documents\n    |
-00000660: 2d3e 2020 3637 2e38 2047 4220 3e20 6d6f  ->  67.8 GB > mo
-00000670: 7669 6573 5c6e 2020 2020 2020 2020 7c2d  vies\n        |-
-00000680: 3e20 2036 322e 3020 4742 203e 2066 726f  >  62.0 GB > fro
-00000690: 6d5f 7468 655f 696e 7465 726e 6574 5c6e  m_the_internet\n
-000006a0: 2020 2020 2020 2020 7c2d 3e20 2020 352e          |->   5.
-000006b0: 3820 4742 203e 2068 6f6d 655f 6d6f 7669  8 GB > home_movi
-000006c0: 6573 5c6e 2020 2020 7c2d 3e20 3633 382e  es\n    |-> 638.
-000006d0: 3120 4d42 203e 2070 686f 746f 735c 6e20  1 MB > photos\n 
-000006e0: 2020 2020 2020 207c 2d3e 2033 3638 2e32         |-> 368.2
-000006f0: 204d 4220 3e20 726f 636b 5f63 6f6e 6365   MB > rock_conce
-00000700: 7274 5c6e 2020 2020 2020 2020 7c2d 3e20  rt\n        |-> 
-00000710: 3235 312e 3620 4d42 203e 2076 6163 6174  251.6 MB > vacat
-00000720: 696f 6e5f 3230 3139 5c6e 2020 2020 2020  ion_2019\n      
-00000730: 2020 7c2d 3e20 2031 382e 3420 4d42 203e    |->  18.4 MB >
-00000740: 2066 616d 696c 795f 7068 6f74 6f73 5c6e   family_photos\n
-00000750: 2020 2020 7c2d 3e20 3532 312e 3620 4d42      |-> 521.6 MB
-00000760: 203e 2077 6f72 6b5c 6e20 2020 2020 2020   > work\n       
-00000770: 207c 2d3e 2032 3633 2e38 204d 4220 3e20   |-> 263.8 MB > 
-00000780: 626f 7269 6e67 5f64 6f63 735c 6e20 2020  boring_docs\n   
-00000790: 2020 2020 207c 2d3e 2032 3537 2e37 204d       |-> 257.7 M
-000007a0: 4220 3e20 7265 706f 7274 735c 6e20 2020  B > reports\n   
-000007b0: 207c 2d3e 2020 3232 2e35 204d 4220 3e20   |->  22.5 MB > 
-000007c0: 6761 6d65 735c 6e60 6060 5c6e 5c6e 2323  games\n```\n\n##
-000007d0: 2320 4c69 7374 5c6e 5c6e 6060 6062 6173  # List\n\n```bas
-000007e0: 685c 6e23 204c 6973 7420 616c 6c20 6e6f  h\n# List all no
-000007f0: 6465 5f6d 6f64 756c 6573 2066 6f6c 6465  de_modules folde
-00000800: 7273 2075 6e64 6572 2074 6865 202f 686f  rs under the /ho
-00000810: 6d65 2f75 7365 722f 6d79 5f63 6f64 6520  me/user/my_code 
-00000820: 6469 7265 6374 6f72 795c 6e24 2064 6972  directory\n$ dir
-00000830: 7374 7566 6620 6c69 7374 207e 2f44 6f63  stuff list ~/Doc
-00000840: 756d 656e 7473 2f43 6f64 652f 5072 6f6a  uments/Code/Proj
-00000850: 6563 7473 2f43 7572 7265 6e74 206e 6f64  ects/Current nod
-00000860: 655f 6d6f 6475 6c65 735c 6e60 6060 5c6e  e_modules\n```\n
-00000870: 5c6e 6060 6070 7974 686f 6e5c 6e20 7c2d  \n```python\n |-
-00000880: 3e20 3431 392e 3620 4d42 203e 202f 7573  > 419.6 MB > /us
-00000890: 6572 2f6d 795f 636f 6465 2f70 6f72 7466  er/my_code/portf
-000008a0: 6f6c 696f 2f77 6562 2f6e 6f64 655f 6d6f  olio/web/node_mo
-000008b0: 6475 6c65 735c 6e20 7c2d 3e20 3332 302e  dules\n |-> 320.
-000008c0: 3320 4d42 203e 202f 7573 6572 2f6d 795f  3 MB > /user/my_
-000008d0: 636f 6465 2f66 756e 5f70 726f 6a65 6374  code/fun_project
-000008e0: 2f6e 6f64 655f 6d6f 6475 6c65 735c 6e20  /node_modules\n 
-000008f0: 7c2d 3e20 3239 382e 3120 4d42 203e 202f  |-> 298.1 MB > /
-00000900: 7573 6572 2f6d 795f 636f 6465 2f73 696d  user/my_code/sim
-00000910: 706c 655f 6761 6d65 2f76 6572 7369 6f6e  ple_game/version
-00000920: 5f32 2f6e 6f64 655f 6d6f 6475 6c65 735c  _2/node_modules\
-00000930: 6e60 6060 5c6e 272c 0a20 2020 2027 6175  n```\n',.    'au
-00000940: 7468 6f72 273a 2027 4368 7269 7320 4772  thor': 'Chris Gr
-00000950: 6567 6f72 7927 2c0a 2020 2020 2761 7574  egory',.    'aut
-00000960: 686f 725f 656d 6169 6c27 3a20 2763 6872  hor_email': 'chr
-00000970: 6973 746f 7068 6572 2e62 2e67 7265 676f  istopher.b.grego
-00000980: 7279 4067 6d61 696c 2e63 6f6d 272c 0a20  ry@gmail.com',. 
-00000990: 2020 2027 6d61 696e 7461 696e 6572 273a     'maintainer':
-000009a0: 2027 4e6f 6e65 272c 0a20 2020 2027 6d61   'None',.    'ma
-000009b0: 696e 7461 696e 6572 5f65 6d61 696c 273a  intainer_email':
-000009c0: 2027 4e6f 6e65 272c 0a20 2020 2027 7572   'None',.    'ur
-000009d0: 6c27 3a20 2768 7474 7073 3a2f 2f67 6974  l': 'https://git
-000009e0: 6875 622e 636f 6d2f 6772 6567 6f72 7962  hub.com/gregoryb
-000009f0: 6368 7269 732f 6469 7273 7475 6666 272c  chris/dirstuff',
-00000a00: 0a20 2020 2027 7061 636b 6167 6573 273a  .    'packages':
-00000a10: 2070 6163 6b61 6765 732c 0a20 2020 2027   packages,.    '
-00000a20: 7061 636b 6167 655f 6461 7461 273a 2070  package_data': p
-00000a30: 6163 6b61 6765 5f64 6174 612c 0a20 2020  ackage_data,.   
-00000a40: 2027 696e 7374 616c 6c5f 7265 7175 6972   'install_requir
-00000a50: 6573 273a 2069 6e73 7461 6c6c 5f72 6571  es': install_req
-00000a60: 7569 7265 732c 0a20 2020 2027 656e 7472  uires,.    'entr
-00000a70: 795f 706f 696e 7473 273a 2065 6e74 7279  y_points': entry
-00000a80: 5f70 6f69 6e74 732c 0a20 2020 2027 7079  _points,.    'py
-00000a90: 7468 6f6e 5f72 6571 7569 7265 7327 3a20  thon_requires': 
-00000aa0: 273e 3d33 2e39 2c3c 332e 3133 272c 0a7d  '>=3.9,<3.13',.}
-00000ab0: 0a0a 0a73 6574 7570 282a 2a73 6574 7570  ...setup(**setup
-00000ac0: 5f6b 7761 7267 7329 0a                   _kwargs).
+00000000: 3c64 6976 2061 6c69 676e 3d22 6365 6e74  <div align="cent
+00000010: 6572 223e 0a20 203c 696d 6720 7372 633d  er">.  <img src=
+00000020: 2261 7373 6574 732f 6469 7273 7475 6666  "assets/dirstuff
+00000030: 2d62 616e 6e65 722e 706e 6722 3e0a 2020  -banner.png">.  
+00000040: 3c68 313e 6469 7273 7475 6666 3c2f 6831  <h1>dirstuff</h1
+00000050: 3e0a 0a20 203c 703e 0a20 2020 203c 7374  >..  <p>.    <st
+00000060: 726f 6e67 3e75 7469 6c69 7469 6573 2066  rong>utilities f
+00000070: 6f72 2066 696c 6573 7973 7465 6d20 6f70  or filesystem op
+00000080: 6572 6174 696f 6e73 3c2f 7374 726f 6e67  erations</strong
+00000090: 3e0a 2020 3c2f 703e 0a0a 2020 3c62 723e  >.  </p>..  <br>
+000000a0: 0a20 203c 6469 763e 0a20 2020 203c 6120  .  <div>.    <a 
+000000b0: 6872 6566 3d22 6874 7470 733a 2f2f 6261  href="https://ba
+000000c0: 6467 652e 6675 7279 2e69 6f2f 7079 2f64  dge.fury.io/py/d
+000000d0: 6972 7374 7566 6622 3e3c 696d 6720 7372  irstuff"><img sr
+000000e0: 633d 2268 7474 7073 3a2f 2f62 6164 6765  c="https://badge
+000000f0: 2e66 7572 792e 696f 2f70 792f 6469 7273  .fury.io/py/dirs
+00000100: 7475 6666 2e73 7667 2220 616c 743d 2250  tuff.svg" alt="P
+00000110: 7950 4922 3e3c 2f61 3e0a 2020 2020 3c61  yPI"></a>.    <a
+00000120: 2068 7265 663d 2268 7474 7073 3a2f 2f70   href="https://p
+00000130: 6570 792e 7465 6368 2f70 726f 6a65 6374  epy.tech/project
+00000140: 2f64 6972 7374 7566 6622 3e3c 696d 6720  /dirstuff"><img 
+00000150: 7372 633d 2268 7474 7073 3a2f 2f70 6570  src="https://pep
+00000160: 792e 7465 6368 2f62 6164 6765 2f64 6972  y.tech/badge/dir
+00000170: 7374 7566 6622 2061 6c74 3d22 446f 776e  stuff" alt="Down
+00000180: 6c6f 6164 7322 3e3c 2f61 3e0a 2020 3c2f  loads"></a>.  </
+00000190: 6469 763e 0a20 203c 6272 3e0a 3c2f 6469  div>.  <br>.</di
+000001a0: 763e 0a0a 2323 2053 756d 6d61 7269 7a61  v>..## Summariza
+000001b0: 7469 6f6e 0a0a 5375 6d6d 6172 697a 6520  tion..Summarize 
+000001c0: 6120 6469 7265 6374 6f72 7920 7265 6375  a directory recu
+000001d0: 7273 6976 656c 7920 6279 2066 696c 6520  rsively by file 
+000001e0: 7369 7a65 2e20 5468 6973 2074 6f6f 6c20  size. This tool 
+000001f0: 6361 6e20 6265 2075 7365 6420 746f 2071  can be used to q
+00000200: 7569 636b 6c79 2073 6561 7263 6820 6120  uickly search a 
+00000210: 6472 6976 6520 666f 7220 6c61 7267 6520  drive for large 
+00000220: 6669 6c65 7320 7461 6b69 6e67 2075 7020  files taking up 
+00000230: 746f 6f20 6d75 6368 2073 7061 6365 2e0a  too much space..
+00000240: 0a23 2320 496e 7374 616c 6c61 7469 6f6e  .## Installation
+00000250: 0a0a 496e 7374 616c 6c20 7468 6520 6375  ..Install the cu
+00000260: 7272 656e 7420 5079 5049 2072 656c 6561  rrent PyPI relea
+00000270: 7365 3a0a 0a60 6060 6261 7368 0a70 6970  se:..```bash.pip
+00000280: 2069 6e73 7461 6c6c 2064 6972 7374 7566   install dirstuf
+00000290: 660a 6060 600a 0a23 2320 5573 6167 650a  f.```..## Usage.
+000002a0: 0a60 6060 6261 7368 0a23 2052 756e 2074  .```bash.# Run t
+000002b0: 6865 2074 7265 6520 636f 6d6d 616e 6420  he tree command 
+000002c0: 746f 2073 756d 6d61 7269 7a65 2061 2064  to summarize a d
+000002d0: 6972 6563 746f 7279 0a24 2064 6972 7374  irectory.$ dirst
+000002e0: 7566 6620 7472 6565 203c 726f 6f74 2d64  uff tree <root-d
+000002f0: 6972 3e0a 0a23 2053 7065 6369 6679 2074  ir>..# Specify t
+00000300: 6865 206d 696e 696d 756d 2066 696c 6520  he minimum file 
+00000310: 7369 7a65 2028 6465 6661 756c 7420 6973  size (default is
+00000320: 2031 304d 4229 0a24 2064 6972 7374 7566   10MB).$ dirstuf
+00000330: 6620 7472 6565 203c 726f 6f74 2d64 6972  f tree <root-dir
+00000340: 3e20 2d2d 7369 7a65 2037 3530 4d42 0a24  > --size 750MB.$
+00000350: 2064 6972 7374 7566 6620 7472 6565 203c   dirstuff tree <
+00000360: 726f 6f74 2d64 6972 3e20 2d2d 7369 7a65  root-dir> --size
+00000370: 2035 304b 420a 0a23 2050 7269 6e74 2066   50KB..# Print f
+00000380: 756c 6c20 6162 736f 6c75 7465 2070 6174  ull absolute pat
+00000390: 6873 2074 6f20 6469 7265 6374 6f72 6965  hs to directorie
+000003a0: 7320 696e 7374 6561 6420 6f66 2064 6972  s instead of dir
+000003b0: 6563 746f 7279 206e 616d 6573 0a24 2064  ectory names.$ d
+000003c0: 6972 7374 7566 6620 7472 6565 203c 726f  irstuff tree <ro
+000003d0: 6f74 2d64 6972 3e20 2d2d 6162 736f 6c75  ot-dir> --absolu
+000003e0: 7465 0a60 6060 0a0a 6060 6062 6173 680a  te.```..```bash.
+000003f0: 2320 5275 6e20 7468 6520 6c69 7374 2063  # Run the list c
+00000400: 6f6d 6d61 6e64 2074 6f20 6669 6e64 2061  ommand to find a
+00000410: 6c6c 2064 6972 6563 746f 7269 6573 2077  ll directories w
+00000420: 6974 6820 6120 6d61 7463 6869 6e67 206e  ith a matching n
+00000430: 616d 650a 2420 6469 7273 7475 6666 206c  ame.$ dirstuff l
+00000440: 6973 7420 3c72 6f6f 742d 6469 723e 203c  ist <root-dir> <
+00000450: 6469 722d 6e61 6d65 3e0a 0a23 2053 7065  dir-name>..# Spe
+00000460: 6369 6679 2074 6865 206d 696e 696d 756d  cify the minimum
+00000470: 2066 696c 6520 7369 7a65 2028 6465 6661   file size (defa
+00000480: 756c 7420 6973 2031 304d 4229 0a24 2064  ult is 10MB).$ d
+00000490: 6972 7374 7566 6620 6c69 7374 203c 726f  irstuff list <ro
+000004a0: 6f74 2d64 6972 3e20 3c64 6972 2d6e 616d  ot-dir> <dir-nam
+000004b0: 653e 202d 2d73 697a 6520 3735 304d 420a  e> --size 750MB.
+000004c0: 2420 6469 7273 7475 6666 206c 6973 7420  $ dirstuff list 
+000004d0: 3c72 6f6f 742d 6469 723e 203c 6469 722d  <root-dir> <dir-
+000004e0: 6e61 6d65 3e20 2d2d 7369 7a65 2035 304b  name> --size 50K
+000004f0: 420a 6060 600a 0a60 6060 6261 7368 0a66  B.```..```bash.f
+00000500: 726f 6d20 6469 7273 7475 6666 2e6f 7320  rom dirstuff.os 
+00000510: 696d 706f 7274 2050 6174 680a 6060 600a  import Path.```.
+00000520: 0a23 2320 4578 616d 706c 6573 0a0a 2323  .## Examples..##
+00000530: 2320 5472 6565 0a0a 6060 6062 6173 680a  # Tree..```bash.
+00000540: 2320 5375 6d6d 6172 697a 6520 7468 6520  # Summarize the 
+00000550: 2f68 6f6d 652f 7573 6572 2f6d 795f 646f  /home/user/my_do
+00000560: 6375 6d65 6e74 7320 6469 7265 6374 6f72  cuments director
+00000570: 790a 2320 7368 6f77 696e 6720 6f6e 6c79  y.# showing only
+00000580: 2064 6972 6563 746f 7269 6573 2067 7265   directories gre
+00000590: 6174 6572 2074 6861 6e20 3230 4d42 2069  ater than 20MB i
+000005a0: 6e20 7369 7a65 0a24 2064 6972 7374 7566  n size.$ dirstuf
+000005b0: 6620 7472 6565 202f 686f 6d65 2f75 7365  f tree /home/use
+000005c0: 722f 6d79 5f64 6f63 756d 656e 7473 202d  r/my_documents -
+000005d0: 2d73 697a 6520 3230 4d42 0a60 6060 0a0a  -size 20MB.```..
+000005e0: 6060 6070 7974 686f 6e0a 7c2d 3e20 2036  ```python.|->  6
+000005f0: 392e 3020 4742 203e 206d 795f 646f 6375  9.0 GB > my_docu
+00000600: 6d65 6e74 730a 2020 2020 7c2d 3e20 2036  ments.    |->  6
+00000610: 372e 3820 4742 203e 206d 6f76 6965 730a  7.8 GB > movies.
+00000620: 2020 2020 2020 2020 7c2d 3e20 2036 322e          |->  62.
+00000630: 3020 4742 203e 2066 726f 6d5f 7468 655f  0 GB > from_the_
+00000640: 696e 7465 726e 6574 0a20 2020 2020 2020  internet.       
+00000650: 207c 2d3e 2020 2035 2e38 2047 4220 3e20   |->   5.8 GB > 
+00000660: 686f 6d65 5f6d 6f76 6965 730a 2020 2020  home_movies.    
+00000670: 7c2d 3e20 3633 382e 3120 4d42 203e 2070  |-> 638.1 MB > p
+00000680: 686f 746f 730a 2020 2020 2020 2020 7c2d  hotos.        |-
+00000690: 3e20 3336 382e 3220 4d42 203e 2072 6f63  > 368.2 MB > roc
+000006a0: 6b5f 636f 6e63 6572 740a 2020 2020 2020  k_concert.      
+000006b0: 2020 7c2d 3e20 3235 312e 3620 4d42 203e    |-> 251.6 MB >
+000006c0: 2076 6163 6174 696f 6e5f 3230 3139 0a20   vacation_2019. 
+000006d0: 2020 2020 2020 207c 2d3e 2020 3138 2e34         |->  18.4
+000006e0: 204d 4220 3e20 6661 6d69 6c79 5f70 686f   MB > family_pho
+000006f0: 746f 730a 2020 2020 7c2d 3e20 3532 312e  tos.    |-> 521.
+00000700: 3620 4d42 203e 2077 6f72 6b0a 2020 2020  6 MB > work.    
+00000710: 2020 2020 7c2d 3e20 3236 332e 3820 4d42      |-> 263.8 MB
+00000720: 203e 2062 6f72 696e 675f 646f 6373 0a20   > boring_docs. 
+00000730: 2020 2020 2020 207c 2d3e 2032 3537 2e37         |-> 257.7
+00000740: 204d 4220 3e20 7265 706f 7274 730a 2020   MB > reports.  
+00000750: 2020 7c2d 3e20 2032 322e 3520 4d42 203e    |->  22.5 MB >
+00000760: 2067 616d 6573 0a60 6060 0a0a 2323 2320   games.```..### 
+00000770: 4c69 7374 0a0a 6060 6062 6173 680a 2320  List..```bash.# 
+00000780: 4c69 7374 2061 6c6c 206e 6f64 655f 6d6f  List all node_mo
+00000790: 6475 6c65 7320 666f 6c64 6572 7320 756e  dules folders un
+000007a0: 6465 7220 7468 6520 2f68 6f6d 652f 7573  der the /home/us
+000007b0: 6572 2f6d 795f 636f 6465 2064 6972 6563  er/my_code direc
+000007c0: 746f 7279 0a24 2064 6972 7374 7566 6620  tory.$ dirstuff 
+000007d0: 6c69 7374 207e 2f44 6f63 756d 656e 7473  list ~/Documents
+000007e0: 2f43 6f64 652f 5072 6f6a 6563 7473 2f43  /Code/Projects/C
+000007f0: 7572 7265 6e74 206e 6f64 655f 6d6f 6475  urrent node_modu
+00000800: 6c65 730a 6060 600a 0a60 6060 7079 7468  les.```..```pyth
+00000810: 6f6e 0a20 7c2d 3e20 3431 392e 3620 4d42  on. |-> 419.6 MB
+00000820: 203e 202f 7573 6572 2f6d 795f 636f 6465   > /user/my_code
+00000830: 2f70 6f72 7466 6f6c 696f 2f77 6562 2f6e  /portfolio/web/n
+00000840: 6f64 655f 6d6f 6475 6c65 730a 207c 2d3e  ode_modules. |->
+00000850: 2033 3230 2e33 204d 4220 3e20 2f75 7365   320.3 MB > /use
+00000860: 722f 6d79 5f63 6f64 652f 6675 6e5f 7072  r/my_code/fun_pr
+00000870: 6f6a 6563 742f 6e6f 6465 5f6d 6f64 756c  oject/node_modul
+00000880: 6573 0a20 7c2d 3e20 3239 382e 3120 4d42  es. |-> 298.1 MB
+00000890: 203e 202f 7573 6572 2f6d 795f 636f 6465   > /user/my_code
+000008a0: 2f73 696d 706c 655f 6761 6d65 2f76 6572  /simple_game/ver
+000008b0: 7369 6f6e 5f32 2f6e 6f64 655f 6d6f 6475  sion_2/node_modu
+000008c0: 6c65 730a 6060 600a 0a23 2320 5061 7468  les.```..## Path
+000008d0: 2075 7469 6c69 7469 6573 0a0a 6469 7273   utilities..dirs
+000008e0: 7475 6666 2070 726f 7669 6465 7320 736f  tuff provides so
+000008f0: 6d65 2050 7974 686f 6e20 7574 696c 6974  me Python utilit
+00000900: 6965 7320 666f 7220 696e 7465 7261 6374  ies for interact
+00000910: 696e 6720 7769 7468 2074 6865 2066 696c  ing with the fil
+00000920: 6573 7973 7465 6d2e 0a0a 2d20 7265 6e61  esystem...- rena
+00000930: 6d65 0a2d 206d 6f76 650a 2d20 636f 7079  me.- move.- copy
+00000940: 0a2d 2064 656c 6574 650a 2d20 7761 6c6b  .- delete.- walk
+00000950: 0a0a 496e 2074 6869 7320 6578 616d 706c  ..In this exampl
+00000960: 6520 7765 2069 7465 7261 7465 206f 7665  e we iterate ove
+00000970: 7220 6e65 7374 6564 2066 6f6c 6465 7273  r nested folders
+00000980: 2074 6861 7420 636f 6e74 6169 6e20 2e74   that contain .t
+00000990: 7874 2066 696c 6573 2061 6e64 2072 656e  xt files and ren
+000009a0: 616d 6520 7468 656d 2074 6f20 6861 7665  ame them to have
+000009b0: 202e 6d64 2065 7874 656e 7369 6f6e 732e   .md extensions.
+000009c0: 0a0a 6060 6070 7974 686f 6e0a 6672 6f6d  ..```python.from
+000009d0: 2064 6972 7374 7566 662e 6f73 2069 6d70   dirstuff.os imp
+000009e0: 6f72 7420 4469 720a 0a64 203d 2044 6972  ort Dir..d = Dir
+000009f0: 2822 6d79 5f66 6f6c 6465 7222 290a 666f  ("my_folder").fo
+00000a00: 7220 7375 6220 696e 2064 2e69 7465 725f  r sub in d.iter_
+00000a10: 6469 7273 2829 3a0a 2020 2020 666f 7220  dirs():.    for 
+00000a20: 6620 696e 2073 7562 2e69 7465 725f 6669  f in sub.iter_fi
+00000a30: 6c65 7328 293a 0a20 2020 2020 2020 2066  les():.        f
+00000a40: 2e72 656e 616d 655f 7265 6765 7828 7222  .rename_regex(r"
+00000a50: 285b 612d 7a5d 2a29 5c2e 7478 7422 2c20  ([a-z]*)\.txt", 
+00000a60: 7222 5c31 2e6d 6422 290a 6060 600a       r"\1.md").```.
```

