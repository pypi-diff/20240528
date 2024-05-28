# Comparing `tmp/spdx_license_list-3.23.tar.gz` & `tmp/spdx_license_list-3.24.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spdx_license_list-3.23.tar", max compression
+gzip compressed data, was "spdx_license_list-3.24.0.tar", max compression
```

## Comparing `spdx_license_list-3.23.tar` & `spdx_license_list-3.24.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1063 2024-02-13 01:45:25.026625 spdx_license_list-3.23/LICENSE
--rw-r--r--   0        0        0     1869 2024-02-13 01:45:25.026625 spdx_license_list-3.23/README.md
--rw-r--r--   0        0        0     1012 2024-02-13 01:46:36.974160 spdx_license_list-3.23/pyproject.toml
--rw-r--r--   0        0        0   122736 2024-02-13 01:45:53.614444 spdx_license_list-3.23/src/spdx_license_list/__init__.py
--rw-r--r--   0        0        0        0 2024-02-13 01:45:25.026625 spdx_license_list-3.23/src/spdx_license_list/py.tpyed
--rw-r--r--   0        0        0     2724 1970-01-01 00:00:00.000000 spdx_license_list-3.23/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-28 02:32:57.376935 spdx_license_list-3.24.0/LICENSE
+-rw-r--r--   0        0        0     1869 2024-05-28 02:32:57.376935 spdx_license_list-3.24.0/README.md
+-rw-r--r--   0        0        0     1014 2024-05-28 02:34:12.580342 spdx_license_list-3.24.0/pyproject.toml
+-rw-r--r--   0        0        0   127066 2024-05-28 02:33:27.968696 spdx_license_list-3.24.0/src/spdx_license_list/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 02:32:57.380935 spdx_license_list-3.24.0/src/spdx_license_list/py.tpyed
+-rw-r--r--   0        0        0     2726 1970-01-01 00:00:00.000000 spdx_license_list-3.24.0/PKG-INFO
```

### Comparing `spdx_license_list-3.23/LICENSE` & `spdx_license_list-3.24.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spdx_license_list-3.23/README.md` & `spdx_license_list-3.24.0/README.md`

 * *Files identical despite different names*

### Comparing `spdx_license_list-3.23/pyproject.toml` & `spdx_license_list-3.24.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -38,11 +38,11 @@
     "Typing :: Typed",
 ]
 description = "SPDX License List as a Python dictionary"
 license = "MIT"
 name = "spdx-license-list"
 readme = "README.md"
 repository = "https://github.com/JJMC89/spdx-license-list"
-version = "3.23"
+version = "3.24.0"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `spdx_license_list-3.23/src/spdx_license_list/__init__.py` & `spdx_license_list-3.24.0/src/spdx_license_list/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,21 @@
     "0BSD": License(
         id="0BSD",
         name="BSD Zero Clause License",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=True,
     ),
+    "3D-Slicer-1.0": License(
+        id="3D-Slicer-1.0",
+        name="3D Slicer License v1.0",
+        deprecated_id=False,
+        fsf_libre=False,
+        osi_approved=False,
+    ),
     "AAL": License(
         id="AAL",
         name="Attribution Assurance License",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=True,
     ),
@@ -166,14 +173,21 @@
     "Aladdin": License(
         id="Aladdin",
         name="Aladdin Free Public License",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
+    "AMD-newlib": License(
+        id="AMD-newlib",
+        name="AMD newlib License",
+        deprecated_id=False,
+        fsf_libre=False,
+        osi_approved=False,
+    ),
     "AMDPLPA": License(
         id="AMDPLPA",
         name="AMD's plpa_map.c License",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
@@ -208,14 +222,21 @@
     "ANTLR-PD-fallback": License(
         id="ANTLR-PD-fallback",
         name="ANTLR Software Rights Notice with license fallback",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
+    "any-OSI": License(
+        id="any-OSI",
+        name="Any OSI License",
+        deprecated_id=False,
+        fsf_libre=False,
+        osi_approved=False,
+    ),
     "Apache-1.0": License(
         id="Apache-1.0",
         name="Apache License 1.0",
         deprecated_id=False,
         fsf_libre=True,
         osi_approved=False,
     ),
@@ -453,14 +474,21 @@
     "BSD-2-Clause-Darwin": License(
         id="BSD-2-Clause-Darwin",
         name="BSD 2-Clause - Ian Darwin variant",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
+    "BSD-2-Clause-first-lines": License(
+        id="BSD-2-Clause-first-lines",
+        name="BSD 2-Clause - first lines requirement",
+        deprecated_id=False,
+        fsf_libre=False,
+        osi_approved=False,
+    ),
     "BSD-2-Clause-FreeBSD": License(
         id="BSD-2-Clause-FreeBSD",
         name="BSD 2-Clause FreeBSD License",
         deprecated_id=True,
         fsf_libre=True,
         osi_approved=False,
     ),
@@ -733,14 +761,21 @@
     "Caldera-no-preamble": License(
         id="Caldera-no-preamble",
         name="Caldera License (without preamble)",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
+    "Catharon": License(
+        id="Catharon",
+        name="Catharon License",
+        deprecated_id=False,
+        fsf_libre=False,
+        osi_approved=False,
+    ),
     "CATOSL-1.1": License(
         id="CATOSL-1.1",
         name="Computer Associates Trusted Open Source License 1.1",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=True,
     ),
@@ -1405,14 +1440,21 @@
     "curl": License(
         id="curl",
         name="curl License",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
+    "cve-tou": License(
+        id="cve-tou",
+        name="Common Vulnerability Enumeration ToU License",
+        deprecated_id=False,
+        fsf_libre=False,
+        osi_approved=False,
+    ),
     "D-FSL-1.0": License(
         id="D-FSL-1.0",
         name="Deutsche Freie Software Lizenz",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
@@ -2077,14 +2119,21 @@
     "gtkbook": License(
         id="gtkbook",
         name="gtkbook License",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
+    "Gutmann": License(
+        id="Gutmann",
+        name="Gutmann License",
+        deprecated_id=False,
+        fsf_libre=False,
+        osi_approved=False,
+    ),
     "HaskellReport": License(
         id="HaskellReport",
         name="Haskell Language Report License",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
@@ -2147,49 +2196,77 @@
     "HPND-export-US": License(
         id="HPND-export-US",
         name="HPND with US Government export control warning",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
+    "HPND-export-US-acknowledgement": License(
+        id="HPND-export-US-acknowledgement",
+        name="HPND with US Government export control warning and acknowledgment",
+        deprecated_id=False,
+        fsf_libre=False,
+        osi_approved=False,
+    ),
     "HPND-export-US-modify": License(
         id="HPND-export-US-modify",
         name="HPND with US Government export control warning and modification rqmt",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
+    "HPND-export2-US": License(
+        id="HPND-export2-US",
+        name="HPND with US Government export control and 2 disclaimers",
+        deprecated_id=False,
+        fsf_libre=False,
+        osi_approved=False,
+    ),
     "HPND-Fenneberg-Livingston": License(
         id="HPND-Fenneberg-Livingston",
         name="Historical Permission Notice and Disclaimer - Fenneberg-Livingston variant",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
     "HPND-INRIA-IMAG": License(
         id="HPND-INRIA-IMAG",
         name="Historical Permission Notice and Disclaimer    - INRIA-IMAG variant",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
+    "HPND-Intel": License(
+        id="HPND-Intel",
+        name="Historical Permission Notice and Disclaimer - Intel variant",
+        deprecated_id=False,
+        fsf_libre=False,
+        osi_approved=False,
+    ),
     "HPND-Kevlin-Henney": License(
         id="HPND-Kevlin-Henney",
         name="Historical Permission Notice and Disclaimer - Kevlin Henney variant",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
     "HPND-Markus-Kuhn": License(
         id="HPND-Markus-Kuhn",
         name="Historical Permission Notice and Disclaimer - Markus Kuhn variant",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
+    "HPND-merchantability-variant": License(
+        id="HPND-merchantability-variant",
+        name="Historical Permission Notice and Disclaimer - merchantability variant",
+        deprecated_id=False,
+        fsf_libre=False,
+        osi_approved=False,
+    ),
     "HPND-MIT-disclaimer": License(
         id="HPND-MIT-disclaimer",
         name="Historical Permission Notice and Disclaimer with MIT disclaimer",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
@@ -2224,21 +2301,35 @@
     "HPND-sell-variant-MIT-disclaimer": License(
         id="HPND-sell-variant-MIT-disclaimer",
         name="HPND sell variant with MIT disclaimer",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
+    "HPND-sell-variant-MIT-disclaimer-rev": License(
+        id="HPND-sell-variant-MIT-disclaimer-rev",
+        name="HPND sell variant with MIT disclaimer - reverse",
+        deprecated_id=False,
+        fsf_libre=False,
+        osi_approved=False,
+    ),
     "HPND-UC": License(
         id="HPND-UC",
         name="Historical Permission Notice and Disclaimer - University of California variant",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
+    "HPND-UC-export-US": License(
+        id="HPND-UC-export-US",
+        name="Historical Permission Notice and Disclaimer - University of California, US export warning",
+        deprecated_id=False,
+        fsf_libre=False,
+        osi_approved=False,
+    ),
     "HTMLTIDY": License(
         id="HTMLTIDY",
         name="HTML Tidy License",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
@@ -2840,14 +2931,21 @@
     "MIT-Festival": License(
         id="MIT-Festival",
         name="MIT Festival Variant",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
+    "MIT-Khronos-old": License(
+        id="MIT-Khronos-old",
+        name="MIT Khronos - old variant",
+        deprecated_id=False,
+        fsf_libre=False,
+        osi_approved=False,
+    ),
     "MIT-Modern-Variant": License(
         id="MIT-Modern-Variant",
         name="MIT License Modern Variant",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=True,
     ),
@@ -3029,21 +3127,35 @@
     "NBPL-1.0": License(
         id="NBPL-1.0",
         name="Net Boolean Public License v1",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
+    "NCBI-PD": License(
+        id="NCBI-PD",
+        name="NCBI Public Domain Notice",
+        deprecated_id=False,
+        fsf_libre=False,
+        osi_approved=False,
+    ),
     "NCGL-UK-2.0": License(
         id="NCGL-UK-2.0",
         name="Non-Commercial Government Licence",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
+    "NCL": License(
+        id="NCL",
+        name="NCL Source Code License",
+        deprecated_id=False,
+        fsf_libre=False,
+        osi_approved=False,
+    ),
     "NCSA": License(
         id="NCSA",
         name="University of Illinois/NCSA Open Source License",
         deprecated_id=False,
         fsf_libre=True,
         osi_approved=True,
     ),
@@ -3197,14 +3309,21 @@
     "O-UDA-1.0": License(
         id="O-UDA-1.0",
         name="Open Use of Data Agreement v1.0",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
+    "OAR": License(
+        id="OAR",
+        name="OAR License",
+        deprecated_id=False,
+        fsf_libre=False,
+        osi_approved=False,
+    ),
     "OCCT-PL": License(
         id="OCCT-PL",
         name="Open CASCADE Technology Public License",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
@@ -3589,14 +3708,21 @@
     "Pixar": License(
         id="Pixar",
         name="Pixar License",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
+    "pkgconf": License(
+        id="pkgconf",
+        name="pkgconf License",
+        deprecated_id=False,
+        fsf_libre=False,
+        osi_approved=False,
+    ),
     "Plexus": License(
         id="Plexus",
         name="Plexus Classworlds License",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
@@ -3624,14 +3750,21 @@
     "PostgreSQL": License(
         id="PostgreSQL",
         name="PostgreSQL License",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=True,
     ),
+    "PPL": License(
+        id="PPL",
+        name="Peer Production License",
+        deprecated_id=False,
+        fsf_libre=False,
+        osi_approved=False,
+    ),
     "PSF-2.0": License(
         id="PSF-2.0",
         name="Python Software Foundation License 2.0",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
@@ -4009,14 +4142,21 @@
     "Sun-PPP": License(
         id="Sun-PPP",
         name="Sun PPP License",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
+    "Sun-PPP-2000": License(
+        id="Sun-PPP-2000",
+        name="Sun PPP License (2000)",
+        deprecated_id=False,
+        fsf_libre=False,
+        osi_approved=False,
+    ),
     "SunPro": License(
         id="SunPro",
         name="SunPro License",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
@@ -4072,14 +4212,21 @@
     "TGPPL-1.0": License(
         id="TGPPL-1.0",
         name="Transitive Grace Period Public Licence 1.0",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
+    "threeparttable": License(
+        id="threeparttable",
+        name="threeparttable License",
+        deprecated_id=False,
+        fsf_libre=False,
+        osi_approved=False,
+    ),
     "TMate": License(
         id="TMate",
         name="TMate Open Source License",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
@@ -4387,14 +4534,21 @@
     "XSkat": License(
         id="XSkat",
         name="XSkat License",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
+    "xzoom": License(
+        id="xzoom",
+        name="xzoom License",
+        deprecated_id=False,
+        fsf_libre=False,
+        osi_approved=False,
+    ),
     "YPL-1.0": License(
         id="YPL-1.0",
         name="Yahoo! Public License v1.0",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
```

### Comparing `spdx_license_list-3.23/PKG-INFO` & `spdx_license_list-3.24.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spdx-license-list
-Version: 3.23
+Version: 3.24.0
 Summary: SPDX License List as a Python dictionary
 Home-page: https://github.com/JJMC89/spdx-license-list
 License: MIT
 Author: JJMC89
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
```

