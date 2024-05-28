# Comparing `tmp/blint-2.1.6.tar.gz` & `tmp/blint-2.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blint-2.1.6.tar", max compression
+gzip compressed data, was "blint-2.1.7.tar", max compression
```

## Comparing `blint-2.1.6.tar` & `blint-2.1.7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1068 2024-05-19 15:19:11.846203 blint-2.1.6/LICENSE
--rw-r--r--   0        0        0     6233 2024-05-19 15:19:11.846203 blint-2.1.6/README.md
--rw-r--r--   0        0        0        0 2024-05-19 15:19:11.850203 blint-2.1.6/blint/__init__.py
--rw-r--r--   0        0        0    24648 2024-05-19 15:19:11.850203 blint-2.1.6/blint/analysis.py
--rw-r--r--   0        0        0    13915 2024-05-19 15:19:11.850203 blint-2.1.6/blint/android.py
--rw-r--r--   0        0        0    59632 2024-05-19 15:19:11.850203 blint-2.1.6/blint/binary.py
--rw-r--r--   0        0        0     2785 2024-05-19 15:19:11.850203 blint-2.1.6/blint/checks.py
--rw-r--r--   0        0        0     6198 2024-05-19 15:19:11.850203 blint-2.1.6/blint/cli.py
--rw-r--r--   0        0        0    20192 2024-05-19 15:19:11.850203 blint-2.1.6/blint/config.py
--rw-r--r--   0        0        0      324 2024-05-19 15:19:11.850203 blint-2.1.6/blint/cyclonedx/README.md
--rw-r--r--   0        0        0        0 2024-05-19 15:19:11.850203 blint-2.1.6/blint/cyclonedx/__init__.py
--rw-r--r--   0        0        0    20843 2024-05-19 15:19:11.850203 blint-2.1.6/blint/cyclonedx/spdx.py
--rw-r--r--   0        0        0   169203 2024-05-19 15:19:11.850203 blint-2.1.6/blint/cyclonedx/spec.py
--rw-r--r--   0        0        0        0 2024-05-19 15:19:11.850203 blint-2.1.6/blint/data/__init__.py
--rw-r--r--   0        0        0        0 2024-05-19 15:19:11.850203 blint-2.1.6/blint/data/annotations/__init__.py
--rw-r--r--   0        0        0     1498 2024-05-19 15:19:11.850203 blint-2.1.6/blint/data/annotations/review_entries_generic.yml
--rw-r--r--   0        0        0     2358 2024-05-19 15:19:11.850203 blint-2.1.6/blint/data/annotations/review_entries_pe.yml
--rw-r--r--   0        0        0    15418 2024-05-19 15:19:11.850203 blint-2.1.6/blint/data/annotations/review_exe_go.yml
--rw-r--r--   0        0        0   124932 2024-05-19 15:19:11.850203 blint-2.1.6/blint/data/annotations/review_imports_pe.yml
--rw-r--r--   0        0        0     8155 2024-05-19 15:19:11.854203 blint-2.1.6/blint/data/annotations/review_methods_generic.yml
--rw-r--r--   0        0        0     5764 2024-05-19 15:19:11.854203 blint-2.1.6/blint/data/annotations/review_methods_mips.yml
--rw-r--r--   0        0        0     2409 2024-05-19 15:19:11.854203 blint-2.1.6/blint/data/annotations/review_monero_generic.yml
--rw-r--r--   0        0        0     1522 2024-05-19 15:19:11.854203 blint-2.1.6/blint/data/annotations/review_monero_go.yml
--rw-r--r--   0        0        0      994 2024-05-19 15:19:11.854203 blint-2.1.6/blint/data/annotations/review_monero_rust
--rw-r--r--   0        0        0      994 2024-05-19 15:19:11.854203 blint-2.1.6/blint/data/annotations/review_monero_rust.yml
--rw-r--r--   0        0        0     5646 2024-05-19 15:19:11.854203 blint-2.1.6/blint/data/annotations/review_rootkits_win.yml
--rw-r--r--   0        0        0     3507 2024-05-19 15:19:11.854203 blint-2.1.6/blint/data/annotations/review_symbols_antiforensic.yml
--rw-r--r--   0        0        0     2943 2024-05-19 15:19:11.854203 blint-2.1.6/blint/data/annotations/review_symbols_generic.yml
--rw-r--r--   0        0        0     1277 2024-05-19 15:19:11.854203 blint-2.1.6/blint/data/annotations/review_symbols_hooka.yml
--rw-r--r--   0        0        0    23537 2024-05-19 15:19:11.854203 blint-2.1.6/blint/data/annotations/review_symbols_macho.yml
--rw-r--r--   0        0        0    10425 2024-05-19 15:19:11.854203 blint-2.1.6/blint/data/annotations/review_symbols_rust.yml
--rw-r--r--   0        0        0    11038 2024-05-19 15:19:11.854203 blint-2.1.6/blint/data/rules.yml
--rw-r--r--   0        0        0      936 2024-05-19 15:19:11.854203 blint-2.1.6/blint/logger.py
--rw-r--r--   0        0        0    24832 2024-05-19 15:19:11.854203 blint-2.1.6/blint/sbom.py
--rw-r--r--   0        0        0    15610 2024-05-19 15:19:11.854203 blint-2.1.6/blint/utils.py
--rw-r--r--   0        0        0     1884 2024-05-19 15:19:11.854203 blint-2.1.6/pyproject.toml
--rw-r--r--   0        0        0     7525 1970-01-01 00:00:00.000000 blint-2.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-28 15:15:51.594902 blint-2.1.7/LICENSE
+-rw-r--r--   0        0        0     6233 2024-05-28 15:15:51.594902 blint-2.1.7/README.md
+-rw-r--r--   0        0        0        0 2024-05-28 15:15:51.594902 blint-2.1.7/blint/__init__.py
+-rw-r--r--   0        0        0    24648 2024-05-28 15:15:51.594902 blint-2.1.7/blint/analysis.py
+-rw-r--r--   0        0        0    13915 2024-05-28 15:15:51.594902 blint-2.1.7/blint/android.py
+-rw-r--r--   0        0        0    59632 2024-05-28 15:15:51.598902 blint-2.1.7/blint/binary.py
+-rw-r--r--   0        0        0     2785 2024-05-28 15:15:51.598902 blint-2.1.7/blint/checks.py
+-rw-r--r--   0        0        0     6447 2024-05-28 15:15:51.598902 blint-2.1.7/blint/cli.py
+-rw-r--r--   0        0        0    20192 2024-05-28 15:15:51.598902 blint-2.1.7/blint/config.py
+-rw-r--r--   0        0        0      324 2024-05-28 15:15:51.598902 blint-2.1.7/blint/cyclonedx/README.md
+-rw-r--r--   0        0        0        0 2024-05-28 15:15:51.598902 blint-2.1.7/blint/cyclonedx/__init__.py
+-rw-r--r--   0        0        0    20843 2024-05-28 15:15:51.598902 blint-2.1.7/blint/cyclonedx/spdx.py
+-rw-r--r--   0        0        0   169203 2024-05-28 15:15:51.598902 blint-2.1.7/blint/cyclonedx/spec.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:15:51.598902 blint-2.1.7/blint/data/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:15:51.598902 blint-2.1.7/blint/data/annotations/__init__.py
+-rw-r--r--   0        0        0     1498 2024-05-28 15:15:51.598902 blint-2.1.7/blint/data/annotations/review_entries_generic.yml
+-rw-r--r--   0        0        0     2358 2024-05-28 15:15:51.598902 blint-2.1.7/blint/data/annotations/review_entries_pe.yml
+-rw-r--r--   0        0        0    15418 2024-05-28 15:15:51.598902 blint-2.1.7/blint/data/annotations/review_exe_go.yml
+-rw-r--r--   0        0        0   124932 2024-05-28 15:15:51.598902 blint-2.1.7/blint/data/annotations/review_imports_pe.yml
+-rw-r--r--   0        0        0     8155 2024-05-28 15:15:51.598902 blint-2.1.7/blint/data/annotations/review_methods_generic.yml
+-rw-r--r--   0        0        0     5764 2024-05-28 15:15:51.598902 blint-2.1.7/blint/data/annotations/review_methods_mips.yml
+-rw-r--r--   0        0        0     2409 2024-05-28 15:15:51.598902 blint-2.1.7/blint/data/annotations/review_monero_generic.yml
+-rw-r--r--   0        0        0     1522 2024-05-28 15:15:51.598902 blint-2.1.7/blint/data/annotations/review_monero_go.yml
+-rw-r--r--   0        0        0      994 2024-05-28 15:15:51.598902 blint-2.1.7/blint/data/annotations/review_monero_rust
+-rw-r--r--   0        0        0      994 2024-05-28 15:15:51.598902 blint-2.1.7/blint/data/annotations/review_monero_rust.yml
+-rw-r--r--   0        0        0     5646 2024-05-28 15:15:51.598902 blint-2.1.7/blint/data/annotations/review_rootkits_win.yml
+-rw-r--r--   0        0        0     3507 2024-05-28 15:15:51.598902 blint-2.1.7/blint/data/annotations/review_symbols_antiforensic.yml
+-rw-r--r--   0        0        0     2943 2024-05-28 15:15:51.598902 blint-2.1.7/blint/data/annotations/review_symbols_generic.yml
+-rw-r--r--   0        0        0     1277 2024-05-28 15:15:51.598902 blint-2.1.7/blint/data/annotations/review_symbols_hooka.yml
+-rw-r--r--   0        0        0    23537 2024-05-28 15:15:51.598902 blint-2.1.7/blint/data/annotations/review_symbols_macho.yml
+-rw-r--r--   0        0        0    10425 2024-05-28 15:15:51.598902 blint-2.1.7/blint/data/annotations/review_symbols_rust.yml
+-rw-r--r--   0        0        0    11038 2024-05-28 15:15:51.598902 blint-2.1.7/blint/data/rules.yml
+-rw-r--r--   0        0        0      936 2024-05-28 15:15:51.598902 blint-2.1.7/blint/logger.py
+-rw-r--r--   0        0        0    26828 2024-05-28 15:15:51.602902 blint-2.1.7/blint/sbom.py
+-rw-r--r--   0        0        0    15610 2024-05-28 15:15:51.602902 blint-2.1.7/blint/utils.py
+-rw-r--r--   0        0        0     1886 2024-05-28 15:15:51.602902 blint-2.1.7/pyproject.toml
+-rw-r--r--   0        0        0     7530 1970-01-01 00:00:00.000000 blint-2.1.7/PKG-INFO
```

### Comparing `blint-2.1.6/LICENSE` & `blint-2.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `blint-2.1.6/README.md` & `blint-2.1.7/README.md`

 * *Files identical despite different names*

### Comparing `blint-2.1.6/blint/analysis.py` & `blint-2.1.7/blint/analysis.py`

 * *Files identical despite different names*

### Comparing `blint-2.1.6/blint/android.py` & `blint-2.1.7/blint/android.py`

 * *Files identical despite different names*

### Comparing `blint-2.1.6/blint/binary.py` & `blint-2.1.7/blint/binary.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
                 .replace("$RF$", "&")
                 .replace("$LP$", "(")
                 .replace("$RP$", ")")
                 .replace("$C$", ",")
                 .replace("$u27$", "'")
             )
         # In case of rust symbols, try and trim the hash part from the end of the symbols
-        if demangled_symbol.count("::") > 3:
+        if demangled_symbol.count("::") > 2:
             last_part = demangled_symbol.split("::")[-1]
             if len(last_part) == 17:
                 demangled_symbol = demangled_symbol.removesuffix(f"::{last_part}")
         return demangled_symbol
     except AttributeError:
         return symbol
```

### Comparing `blint-2.1.6/blint/checks.py` & `blint-2.1.7/blint/checks.py`

 * *Files identical despite different names*

### Comparing `blint-2.1.6/blint/cli.py` & `blint-2.1.7/blint/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -108,14 +108,22 @@
     sbom_parser.add_argument(
         "--stdout",
         action="store_true",
         default=False,
         dest="stdout_mode",
         help="Print the SBOM to stdout instead of a file.",
     )
+    sbom_parser.add_argument(
+        "--exports-prefix",
+        default=[],
+        action="extend",
+        nargs="+",
+        dest="exports_prefix",
+        help="prefixes for the exports to be included in the SBOM.",
+    )
     return parser.parse_args()
 
 
 def parse_input(src):
     """Parses the input source.
 
     This function takes the input source as a list and parses it to extract the
@@ -178,15 +186,15 @@
             if args.sbom_output:
                 sbom_output = args.sbom_output
             else:
                 sbom_output = os.path.join(os.getcwd(), "bom.json")
             sbom_output_dir = os.path.dirname(sbom_output)
             if sbom_output_dir and not os.path.exists(sbom_output_dir):
                 os.makedirs(sbom_output_dir)
-        generate(src_dirs, sbom_output, args.deep_mode)
+        generate(src_dirs, sbom_output, args.deep_mode, args.exports_prefix)
     # Default case
     else:
         if reports_dir and not os.path.exists(reports_dir):
             os.makedirs(reports_dir)
         files = gen_file_list(src_dirs)
         analyzer = AnalysisRunner()
         findings, reviews, fuzzables = analyzer.start(
```

### Comparing `blint-2.1.6/blint/config.py` & `blint-2.1.7/blint/config.py`

 * *Files identical despite different names*

### Comparing `blint-2.1.6/blint/cyclonedx/spdx.py` & `blint-2.1.7/blint/cyclonedx/spdx.py`

 * *Files identical despite different names*

### Comparing `blint-2.1.6/blint/cyclonedx/spec.py` & `blint-2.1.7/blint/cyclonedx/spec.py`

 * *Files identical despite different names*

### Comparing `blint-2.1.6/blint/data/annotations/review_entries_generic.yml` & `blint-2.1.7/blint/data/annotations/review_entries_generic.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.6/blint/data/annotations/review_entries_pe.yml` & `blint-2.1.7/blint/data/annotations/review_entries_pe.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.6/blint/data/annotations/review_exe_go.yml` & `blint-2.1.7/blint/data/annotations/review_exe_go.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.6/blint/data/annotations/review_imports_pe.yml` & `blint-2.1.7/blint/data/annotations/review_imports_pe.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.6/blint/data/annotations/review_methods_generic.yml` & `blint-2.1.7/blint/data/annotations/review_methods_generic.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.6/blint/data/annotations/review_methods_mips.yml` & `blint-2.1.7/blint/data/annotations/review_methods_mips.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.6/blint/data/annotations/review_monero_generic.yml` & `blint-2.1.7/blint/data/annotations/review_monero_generic.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.6/blint/data/annotations/review_monero_go.yml` & `blint-2.1.7/blint/data/annotations/review_monero_go.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.6/blint/data/annotations/review_monero_rust` & `blint-2.1.7/blint/data/annotations/review_monero_rust`

 * *Files identical despite different names*

### Comparing `blint-2.1.6/blint/data/annotations/review_monero_rust.yml` & `blint-2.1.7/blint/data/annotations/review_monero_rust.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.6/blint/data/annotations/review_rootkits_win.yml` & `blint-2.1.7/blint/data/annotations/review_rootkits_win.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.6/blint/data/annotations/review_symbols_antiforensic.yml` & `blint-2.1.7/blint/data/annotations/review_symbols_antiforensic.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.6/blint/data/annotations/review_symbols_generic.yml` & `blint-2.1.7/blint/data/annotations/review_symbols_generic.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.6/blint/data/annotations/review_symbols_hooka.yml` & `blint-2.1.7/blint/data/annotations/review_symbols_hooka.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.6/blint/data/annotations/review_symbols_macho.yml` & `blint-2.1.7/blint/data/annotations/review_symbols_macho.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.6/blint/data/annotations/review_symbols_rust.yml` & `blint-2.1.7/blint/data/annotations/review_symbols_rust.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.6/blint/data/rules.yml` & `blint-2.1.7/blint/data/rules.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.6/blint/logger.py` & `blint-2.1.7/blint/logger.py`

 * *Files identical despite different names*

### Comparing `blint-2.1.6/blint/sbom.py` & `blint-2.1.7/blint/sbom.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,15 +84,15 @@
             )
         ]
     )
     metadata.lifecycles = [Lifecycles(phase=Phase.post_build)]
     return metadata
 
 
-def generate(src_dirs: list[str], output_file: str, deep_mode: bool) -> bool:
+def generate(src_dirs: list[str], output_file: str, deep_mode: bool, export_prefixes: list[str]) -> bool:
     """
     Generates an SBOM for the given source directories.
 
     Args:
         src_dirs (list): A list of source directories.
         output_file (str): The path to the output file.
         deep_mode (bool): Flag indicating whether to perform deep analysis.
@@ -127,15 +127,15 @@
             task = progress.add_task(
                 f"[green] Parsing {len(exe_files)} binaries",
                 total=len(exe_files),
                 start=True,
             )
         for exe in exe_files:
             progress.update(task, description=f"Processing [bold]{exe}[/bold]", advance=1)
-            components += process_exe_file(dependencies_dict, deep_mode, exe, sbom)
+            components += process_exe_file(dependencies_dict, deep_mode, exe, sbom, export_prefixes)
         if android_files:
             task = progress.add_task(
                 f"[green] Parsing {len(android_files)} android apps",
                 total=len(android_files),
                 start=True,
             )
         for f in android_files:
@@ -262,14 +262,15 @@
 
 
 def process_exe_file(
     dependencies_dict: dict[str, set],
     deep_mode: bool,
     exe: str,
     sbom: CycloneDX,
+    export_prefixes: list[str] = None,
 ) -> list[Component]:
     """
     Processes an executable file, extracts metadata, and generates a Software Bill of Materials.
 
     Args:
         dependencies_dict (dict[str, set]): A dictionary of dependencies.
         deep_mode: A flag indicating whether to include deep analysis of the executable.
@@ -342,51 +343,89 @@
             parent_component.properties.append(
                 Property(
                     name="internal:symbols_version",
                     value=", ".join([f["name"] for f in symbols_version]),
                 )
             )
         internal_functions = sorted(
-            {f["name"] for f in metadata.get("functions", []) if f["name"]}
+            {f["name"] for f in metadata.get("functions", []) if not any(f["name"].startswith(p) for p in export_prefixes)}
         )
         if internal_functions:
             parent_component.properties.append(
                 Property(
                     name="internal:functions",
                     value=SYMBOL_DELIMITER.join(internal_functions),
                 )
             )
+        export_functions = sorted(
+            {f["name"] for f in metadata.get("functions", []) if any(f["name"].startswith(p) for p in export_prefixes)}
+        )
+        if export_functions:
+            parent_component.properties.append(
+                Property(
+                    name="internal:export_functions",
+                    value=SYMBOL_DELIMITER.join(export_functions),
+                )
+            )
         symtab_symbols = sorted(
-            {f["name"] for f in metadata.get("symtab_symbols", []) if f["name"]}
+            {f["name"] for f in metadata.get("symtab_symbols", []) if not any(f["name"].startswith(p) for p in export_prefixes)}
         )
         if symtab_symbols:
             parent_component.properties.append(
                 Property(
                     name="internal:symtab_symbols",
                     value=SYMBOL_DELIMITER.join(symtab_symbols),
                 )
             )
-        all_imports = sorted({f["name"] for f in metadata.get("imports", [])})
+        exported_symtab_symbols = sorted(
+            {f["name"] for f in metadata.get("symtab_symbols", []) if any(f["name"].startswith(p) for p in export_prefixes)}
+        )
+        if exported_symtab_symbols:
+            parent_component.properties.append(
+                Property(
+                    name="internal:exported_symtab_symbols",
+                    value=SYMBOL_DELIMITER.join(exported_symtab_symbols),
+                )
+            )
+        all_imports = sorted({f["name"] for f in metadata.get("imports", []) if not any(f["name"].startswith(p) for p in export_prefixes)})
         if all_imports:
             parent_component.properties.append(
                 Property(
                     name="internal:imports",
                     value=SYMBOL_DELIMITER.join(all_imports),
                 )
             )
+        all_exports = sorted({f["name"] for f in metadata.get("imports", []) if any(f["name"].startswith(p) for p in export_prefixes)})
+        if all_imports:
+            parent_component.properties.append(
+                Property(
+                    name="internal:exports",
+                    value=SYMBOL_DELIMITER.join(all_exports),
+                )
+            )
         dynamic_symbols = sorted(
-            {f["name"] for f in metadata.get("dynamic_symbols", []) if f["name"]}
+            {f["name"] for f in metadata.get("dynamic_symbols", []) if not any(f["name"].startswith(p) for p in export_prefixes)}
         )
         if dynamic_symbols:
             parent_component.properties.append(
                 Property(
                     name="internal:dynamic_symbols",
                     value=SYMBOL_DELIMITER.join(dynamic_symbols),
                 )
             )
+        exported_dynamic_symbols = sorted(
+            {f["name"] for f in metadata.get("dynamic_symbols", []) if any(f["name"].startswith(p) for p in export_prefixes)}
+        )
+        if exported_dynamic_symbols:
+            parent_component.properties.append(
+                Property(
+                    name="internal:exported_dynamic_symbols",
+                    value=SYMBOL_DELIMITER.join(exported_dynamic_symbols),
+                )
+            )
     if not sbom.metadata.component.components:
         sbom.metadata.component.components = []
     _add_to_parent_component(sbom.metadata.component.components, parent_component)
     if metadata.get("libraries"):
         for entry in metadata.get("libraries"):
             comp = create_library_component(entry, exe)
             lib_components.append(comp)
```

### Comparing `blint-2.1.6/blint/utils.py` & `blint-2.1.7/blint/utils.py`

 * *Files identical despite different names*

### Comparing `blint-2.1.6/pyproject.toml` & `blint-2.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "blint"
-version = "2.1.6"
+version = "2.1.7"
 description = "Linter and SBOM generator for binary files."
 authors = ["Prabhu Subramanian <prabhu@appthreat.com>", "Caroline Russell <caroline@appthreat.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/OWASP-dep-scan/blint"
 repository = "https://github.com/OWASP-dep-scan/blint"
 keywords = ["linter", "binary", "security", "sast"]
@@ -32,15 +32,15 @@
 lief = "^0.14.0"
 rich = "^13.7.0"
 PyYAML = "^6.0.1"
 defusedxml = "^0.7.1"
 pydantic = {version = "^2.6.0", extras = ["email"]}
 orjson = "^3.10.1"
 symbolic = "10.2.1"
-ar = "^0.8"
+ar = "^0.9.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0.0"
 black = "^24.0.0"
 flake8 = "^7.0.0"
 pylint = "^3.0.0"
 pytest-cov = "^4.0.0"
```

### Comparing `blint-2.1.6/PKG-INFO` & `blint-2.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blint
-Version: 2.1.6
+Version: 2.1.7
 Summary: Linter and SBOM generator for binary files.
 Home-page: https://github.com/OWASP-dep-scan/blint
 License: MIT
 Keywords: linter,binary,security,sast
 Author: Prabhu Subramanian
 Author-email: prabhu@appthreat.com
 Requires-Python: >=3.10,<3.13
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Requires-Dist: PyYAML (>=6.0.1,<7.0.0)
-Requires-Dist: ar (>=0.8,<0.9)
+Requires-Dist: ar (>=0.9.1,<0.10.0)
 Requires-Dist: defusedxml (>=0.7.1,<0.8.0)
 Requires-Dist: lief (>=0.14.0,<0.15.0)
 Requires-Dist: orjson (>=3.10.1,<4.0.0)
 Requires-Dist: pydantic[email] (>=2.6.0,<3.0.0)
 Requires-Dist: rich (>=13.7.0,<14.0.0)
 Requires-Dist: symbolic (==10.2.1)
 Project-URL: CI, https://github.com/AppThreat/blint/actions
```

