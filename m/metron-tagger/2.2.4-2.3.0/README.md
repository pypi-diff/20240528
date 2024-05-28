# Comparing `tmp/metron_tagger-2.2.4.tar.gz` & `tmp/metron_tagger-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metron_tagger-2.2.4.tar", max compression
+gzip compressed data, was "metron_tagger-2.3.0.tar", max compression
```

## Comparing `metron_tagger-2.2.4.tar` & `metron_tagger-2.3.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    35149 2024-04-06 13:17:19.527556 metron_tagger-2.2.4/LICENSE
--rw-r--r--   0        0        0      897 2024-04-06 13:17:19.527556 metron_tagger-2.2.4/NEWS.md
--rw-r--r--   0        0        0     2845 2024-04-06 13:17:19.527556 metron_tagger-2.2.4/README.rst
--rw-r--r--   0        0        0       76 2024-04-06 13:17:19.527556 metron_tagger-2.2.4/metrontagger/__init__.py
--rw-r--r--   0        0        0     1413 2024-04-06 13:17:19.527556 metron_tagger-2.2.4/metrontagger/cli.py
--rw-r--r--   0        0        0     4936 2024-04-06 13:17:19.527556 metron_tagger-2.2.4/metrontagger/duplicates.py
--rw-r--r--   0        0        0     7573 2024-04-06 13:17:19.527556 metron_tagger-2.2.4/metrontagger/filerenamer.py
--rw-r--r--   0        0        0     3756 2024-04-06 13:17:19.527556 metron_tagger-2.2.4/metrontagger/filesorter.py
--rw-r--r--   0        0        0      577 2024-04-06 13:17:19.531556 metron_tagger-2.2.4/metrontagger/logging.py
--rw-r--r--   0        0        0     2787 2024-04-06 13:17:19.531556 metron_tagger-2.2.4/metrontagger/options.py
--rw-r--r--   0        0        0    13377 2024-04-06 13:17:19.531556 metron_tagger-2.2.4/metrontagger/run.py
--rw-r--r--   0        0        0     6443 2024-04-06 13:17:19.531556 metron_tagger-2.2.4/metrontagger/schema/v1/ComicInfo.xsd
--rw-r--r--   0        0        0     9518 2024-04-06 13:17:19.531556 metron_tagger-2.2.4/metrontagger/schema/v2/ComicInfo.xsd
--rw-r--r--   0        0        0     4030 2024-04-06 13:17:19.531556 metron_tagger-2.2.4/metrontagger/settings.py
--rw-r--r--   0        0        0      156 2024-04-06 13:17:19.531556 metron_tagger-2.2.4/metrontagger/styles.py
--rw-r--r--   0        0        0    15026 2024-04-06 13:17:19.531556 metron_tagger-2.2.4/metrontagger/talker.py
--rw-r--r--   0        0        0     1328 2024-04-06 13:17:19.531556 metron_tagger-2.2.4/metrontagger/utils.py
--rw-r--r--   0        0        0     1763 2024-04-06 13:17:19.531556 metron_tagger-2.2.4/metrontagger/validate_ci.py
--rw-r--r--   0        0        0     5171 2024-04-06 13:17:19.531556 metron_tagger-2.2.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-06 13:17:19.531556 metron_tagger-2.2.4/tests/__init__.py
--rw-r--r--   0        0        0     2534 2024-04-06 13:17:19.531556 metron_tagger-2.2.4/tests/conftest.py
--rw-r--r--   0        0        0     2567 2024-04-06 13:17:19.531556 metron_tagger-2.2.4/tests/test_filerenamer.py
--rw-r--r--   0        0        0     2693 2024-04-06 13:17:19.531556 metron_tagger-2.2.4/tests/test_filesorter.py
--rw-r--r--   0        0        0     6077 2024-04-06 13:17:19.531556 metron_tagger-2.2.4/tests/test_metron_tagger.py
--rw-r--r--   0        0        0     1431 2024-04-06 13:17:19.531556 metron_tagger-2.2.4/tests/test_options.py
--rw-r--r--   0        0        0     1336 2024-04-06 13:17:19.531556 metron_tagger-2.2.4/tests/test_settings.py
--rw-r--r--   0        0        0     9962 2024-04-06 13:17:19.531556 metron_tagger-2.2.4/tests/test_talker.py
--rw-r--r--   0        0        0     2314 2024-04-06 13:17:19.535556 metron_tagger-2.2.4/tests/test_utils.py
--rw-r--r--   0        0        0     4489 1970-01-01 00:00:00.000000 metron_tagger-2.2.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-28 15:10:07.997525 metron_tagger-2.3.0/LICENSE
+-rw-r--r--   0        0        0     1236 2024-05-28 15:10:07.997525 metron_tagger-2.3.0/NEWS.md
+-rw-r--r--   0        0        0     2961 2024-05-28 15:10:08.001525 metron_tagger-2.3.0/README.rst
+-rw-r--r--   0        0        0       76 2024-05-28 15:10:08.001525 metron_tagger-2.3.0/metrontagger/__init__.py
+-rw-r--r--   0        0        0     1500 2024-05-28 15:10:08.001525 metron_tagger-2.3.0/metrontagger/cli.py
+-rw-r--r--   0        0        0     4936 2024-05-28 15:10:08.001525 metron_tagger-2.3.0/metrontagger/duplicates.py
+-rw-r--r--   0        0        0     7737 2024-05-28 15:10:08.001525 metron_tagger-2.3.0/metrontagger/filerenamer.py
+-rw-r--r--   0        0        0     3938 2024-05-28 15:10:08.001525 metron_tagger-2.3.0/metrontagger/filesorter.py
+-rw-r--r--   0        0        0      577 2024-05-28 15:10:08.001525 metron_tagger-2.3.0/metrontagger/logging.py
+-rw-r--r--   0        0        0     2990 2024-05-28 15:10:08.001525 metron_tagger-2.3.0/metrontagger/options.py
+-rw-r--r--   0        0        0    13672 2024-05-28 15:10:08.001525 metron_tagger-2.3.0/metrontagger/run.py
+-rw-r--r--   0        0        0     6443 2024-05-28 15:10:08.001525 metron_tagger-2.3.0/metrontagger/schema/v1/ComicInfo.xsd
+-rw-r--r--   0        0        0     9518 2024-05-28 15:10:08.001525 metron_tagger-2.3.0/metrontagger/schema/v2/ComicInfo.xsd
+-rw-r--r--   0        0        0     4074 2024-05-28 15:10:08.001525 metron_tagger-2.3.0/metrontagger/settings.py
+-rw-r--r--   0        0        0      156 2024-05-28 15:10:08.001525 metron_tagger-2.3.0/metrontagger/styles.py
+-rw-r--r--   0        0        0    15026 2024-05-28 15:10:08.001525 metron_tagger-2.3.0/metrontagger/talker.py
+-rw-r--r--   0        0        0     1334 2024-05-28 15:10:08.001525 metron_tagger-2.3.0/metrontagger/utils.py
+-rw-r--r--   0        0        0     1763 2024-05-28 15:10:08.001525 metron_tagger-2.3.0/metrontagger/validate_ci.py
+-rw-r--r--   0        0        0     5171 2024-05-28 15:10:08.005525 metron_tagger-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-28 15:10:08.005525 metron_tagger-2.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     2534 2024-05-28 15:10:08.005525 metron_tagger-2.3.0/tests/conftest.py
+-rw-r--r--   0        0        0     2567 2024-05-28 15:10:08.005525 metron_tagger-2.3.0/tests/test_filerenamer.py
+-rw-r--r--   0        0        0     3246 2024-05-28 15:10:08.005525 metron_tagger-2.3.0/tests/test_filesorter.py
+-rw-r--r--   0        0        0     6077 2024-05-28 15:10:08.005525 metron_tagger-2.3.0/tests/test_metron_tagger.py
+-rw-r--r--   0        0        0     1431 2024-05-28 15:10:08.005525 metron_tagger-2.3.0/tests/test_options.py
+-rw-r--r--   0        0        0     1336 2024-05-28 15:10:08.005525 metron_tagger-2.3.0/tests/test_settings.py
+-rw-r--r--   0        0        0     9962 2024-05-28 15:10:08.005525 metron_tagger-2.3.0/tests/test_talker.py
+-rw-r--r--   0        0        0     2314 2024-05-28 15:10:08.005525 metron_tagger-2.3.0/tests/test_utils.py
+-rw-r--r--   0        0        0     4605 1970-01-01 00:00:00.000000 metron_tagger-2.3.0/PKG-INFO
```

### Comparing `metron_tagger-2.2.4/LICENSE` & `metron_tagger-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metron_tagger-2.2.4/NEWS.md` & `metron_tagger-2.3.0/NEWS.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,23 @@
 # 📰 Metron-Tagger News
 
+## v2.3.0
+
+## 🚀 Features
+
+- Handle Renaming of Digital Comics @bpepple (#122)
+- Remove Oddball Rename Tokens @bpepple (#120)
+- Remove Non-Valid Metadata @bpepple (#119)
+
+## 🧰 Maintenance
+
+- Type Annotation Fixes @bpepple (#118)
+- Bump requests from 2.31.0 to 2.32.0 @dependabot (#121)
+- Bump idna from 3.6 to 3.7 @dependabot (#117)
+
 ## v2.2.4
 
 ### 🐛 Bug Fixes
 
 - Fix Tagging Bug with Existing `ComicInfo.xml` @bpepple (#114)
 - Fix bug in duplicate image detection when attempting to hash a bad image.
   (#105)
```

### Comparing `metron_tagger-2.2.4/README.rst` & `metron_tagger-2.3.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -61,14 +61,15 @@
     -d, --delete         Delete the metadata tags from the file. (default: False)
     --ignore-existing    Ignore files that have existing metadata tag. (default: False)
     -i, --interactive    Interactively query the user when there are matches for an online search. (default: False)
     --missing            List files without metadata. (default: False)
     -s, --sort           Sort files that contain metadata tags. (default: False)
     -z, --export-to-cbz  Export a CBR (rar) archive to a CBZ (zip) archive. (default: False)
     --validate           Verify that comic archive has a valid ComicInfo.xml. (default: False)
+    --remove-non-valid   Remove ComicInfo.xml from comic if not valid. Used with --validate option (default: False)
     --delete-original    Delete the original archive after successful export to another format. (default: False)
     --duplicates         Identify and give the option to delete duplicate pages in a directory of comics. (Experimental) (default: False)
     --version            Show the version number and exit
 
 Bugs/Requests
 -------------
```

### Comparing `metron_tagger-2.2.4/metrontagger/cli.py` & `metron_tagger-2.3.0/metrontagger/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -46,14 +46,17 @@
 
     if opts.delete_original:
         config.delete_original = opts.delete_original
 
     if opts.validate:
         config.validate = opts.validate
 
+    if opts.remove_non_valid:
+        config.remove_non_valid = opts.remove_non_valid
+
     if opts.duplicates:
         config.duplicates = opts.duplicates
 
     return config
 
 
 def main() -> None:
```

### Comparing `metron_tagger-2.2.4/metrontagger/duplicates.py` & `metron_tagger-2.3.0/metrontagger/duplicates.py`

 * *Files identical despite different names*

### Comparing `metron_tagger-2.2.4/metrontagger/filerenamer.py` & `metron_tagger-2.3.0/metrontagger/filerenamer.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from darkseid.utils import unique_file
 
 from metrontagger.styles import Styles
 from metrontagger.utils import cleanup_string
 
 
 class FileRenamer:
-    """Class to rename a comic archive based on it's metadata tag"""
+    """Class to rename a comic archive based on its metadata tag"""
 
     def __init__(self: "FileRenamer", metadata: Metadata | None = None) -> None:
         self.metadata: Metadata | None = metadata
         self.template: str = "%series% v%volume% #%issue% (of %issuecount%) (%year%)"
         self.smart_cleanup: bool = True
         self.issue_zero_padding: int = 3
 
@@ -36,15 +36,17 @@
         """Method to set the padding for the issue's number"""
         self.issue_zero_padding = count
 
     def set_template(self: "FileRenamer", template: str) -> None:
         """Method to use a user's custom file naming template."""
         self.template = template
 
-    def replace_token(self: "FileRenamer", text: str, value: str | None, token: str) -> str:
+    def replace_token(
+        self: "FileRenamer", text: str, value: int | str | None, token: str
+    ) -> str:
         """Method to replace a value with another value"""
 
         # helper func
         def is_token(txt: str) -> bool:
             return txt[0] == "%" and txt.endswith("%")
 
         if value is not None:
@@ -66,16 +68,16 @@
             return " ".join(text_list)
 
         return text.replace(token, "")
 
     @staticmethod
     def _remove_empty_separators(value: str) -> str:
         value = re.sub(r"\(\s*[-:]*\s*\)", "", value)
-        value = re.sub(r"\[\s*[-:]*\s*\]", "", value)
-        return re.sub(r"\{\s*[-:]*\s*\}", "", value)
+        value = re.sub(r"\[\s*[-:]*\s*]", "", value)
+        return re.sub(r"\{\s*[-:]*\s*}", "", value)
 
     @staticmethod
     def _remove_duplicate_hyphen_underscore(value: str) -> str:
         value = re.sub(r"[-_]{2,}\s+", "-- ", value)
         value = re.sub(r"(\s--)+", " --", value)
         return re.sub(r"(\s-)+", " -", value)
 
@@ -86,84 +88,92 @@
         # remove duplicate spaces
         new_name = " ".join(new_name.split())
 
         # remove remove duplicate -, _,
         new_name = self._remove_duplicate_hyphen_underscore(new_name)
 
         # remove dash or double dash at end of line
-        new_name = re.sub(r"[-]{1,2}\s*$", "", new_name)
+        new_name = re.sub(r"-{1,2}\s*$", "", new_name)
 
         # remove duplicate spaces (again!)
         return " ".join(new_name.split())
 
     def determine_name(self: "FileRenamer", filename: Path) -> str | None:
         """Method to create the new filename based on the files metadata"""
         if not self.metadata:
             return None
         md = self.metadata
         new_name = self.template
 
-        new_name = self.replace_token(new_name, md.series.name, "%series%")
-        new_name = self.replace_token(new_name, md.series.volume, "%volume%")
+        new_name = self.replace_token(
+            new_name, md.series.name if md.series is not None else "Unknown", "%series%"
+        )
+        new_name = self.replace_token(
+            new_name, md.series.volume if md.series is not None else 0, "%volume%"
+        )
 
         if md.issue is None:
             issue_str = None
         elif md.issue == "½":
             issue_str = IssueString("0.5").as_string(pad=self.issue_zero_padding)
         else:
             issue_str = IssueString(md.issue).as_string(pad=self.issue_zero_padding)
         new_name = self.replace_token(new_name, issue_str, "%issue%")
 
         new_name = self.replace_token(new_name, md.issue_count, "%issuecount%")
-        new_name = self.replace_token(new_name, md.cover_date.year, "%year%")
-        new_name = self.replace_token(new_name, md.publisher, "%publisher%")
-        new_name = self.replace_token(new_name, md.stories, "%title%")
-        new_name = self.replace_token(new_name, md.cover_date.month, "%month%")
+        new_name = self.replace_token(
+            new_name, md.cover_date.year if md.cover_date is not None else "Unknown", "%year%"
+        )
+        new_name = self.replace_token(
+            new_name, "Unknown" if md.publisher is None else md.publisher.name, "%publisher%"
+        )
+        if md.cover_date is not None:
+            new_name = self.replace_token(new_name, md.cover_date.month, "%month%")
         month_name = None
-        if (
+        if md.cover_date is not None and (
             md.cover_date.month is not None
             and (
-                (isinstance(md.cover_date.month, str) and md.cover_date.month.isdigit())
+                (isinstance(md.cover_date.month, str) and str(md.cover_date.month).isdigit())
                 or isinstance(md.cover_date.month, int)
             )
             and int(md.cover_date.month) in range(1, 13)
         ):
             date_time = datetime.datetime(  # noqa: DTZ001
                 1970,
                 int(md.cover_date.month),
                 1,
                 0,
                 0,
             )
             month_name = date_time.strftime("%B")
         new_name = self.replace_token(new_name, month_name, "%month_name%")
 
-        new_name = self.replace_token(new_name, md.genres, "%genre%")
-        new_name = self.replace_token(new_name, md.series.language, "%language_code%")
-        new_name = self.replace_token(new_name, md.critical_rating, "%criticalrating%")
         new_name = self.replace_token(
             new_name,
             md.alternate_series,
             "%alternateseries%",
         )
         new_name = self.replace_token(
             new_name,
             md.alternate_number,
             "%alternatenumber%",
         )
         new_name = self.replace_token(new_name, md.alternate_count, "%alternatecount%")
         new_name = self.replace_token(new_name, md.imprint, "%imprint%")
-        if md.series.format == "Hard Cover":
-            new_name = self.replace_token(new_name, "HC", "%format%")
-        elif md.series.format == "Trade Paperback":
-            new_name = self.replace_token(new_name, "TPB", "%format%")
-        else:
-            new_name = self.replace_token(new_name, "", "%format%")
+        if md.series is not None:
+            match md.series.format:
+                case "Hard Cover":
+                    new_name = self.replace_token(new_name, "HC", "%format%")
+                case "Trade Paperback":
+                    new_name = self.replace_token(new_name, "TPB", "%format%")
+                case "Digital Chapters":
+                    new_name = self.replace_token(new_name, "Digital Chapter", "%format%")
+                case _:
+                    new_name = self.replace_token(new_name, "", "%format%")
         new_name = self.replace_token(new_name, md.age_rating, "%maturityrating%")
-        new_name = self.replace_token(new_name, md.stories, "%storyarc%")
         new_name = self.replace_token(new_name, md.series_group, "%seriesgroup%")
         new_name = self.replace_token(new_name, md.scan_info, "%scaninfo%")
 
         if self.smart_cleanup:
             new_name = self.smart_cleanup_string(new_name)
 
         ext = filename.suffix
```

### Comparing `metron_tagger-2.2.4/metrontagger/filesorter.py` & `metron_tagger-2.3.0/metrontagger/filesorter.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,17 +23,20 @@
         self.sort_directory = directory
 
     @staticmethod
     def _cleanup_metadata(
         meta_data: Metadata,
     ) -> tuple[str | None, str | None, str | None]:
         """Clean the metadata string."""
-        publisher = cleanup_string(meta_data.publisher.name)
-        series = cleanup_string(meta_data.series.name)
-        volume = cleanup_string(meta_data.series.volume)
+        publisher = cleanup_string(meta_data.publisher.name) if meta_data.publisher else None
+        if meta_data.series:
+            series = cleanup_string(meta_data.series.name)
+            volume = cleanup_string(meta_data.series.volume)
+        else:
+            series = volume = None
         return publisher, series, volume
 
     @staticmethod
     def _move_files(orig: Path, new: Path) -> bool:
         try:
             move(orig, new)
         except Error:
@@ -61,15 +64,17 @@
     def _get_new_path(
         self: "FileSorter",
         meta_data: Metadata,
         publisher: str,
         series: str,
         volume: str,
     ) -> Path:
-        tpb = meta_data.series.format == "Trade Paperback"
+        tpb = (
+            False if meta_data.series is None else meta_data.series.format == "Trade Paperback"
+        )
         return (
             Path(self.sort_directory)
             / publisher
             / f"{f'{series} TPB' if tpb else f'{series}'}"
             / f"v{volume}"
         )
```

### Comparing `metron_tagger-2.2.4/metrontagger/logging.py` & `metron_tagger-2.3.0/metrontagger/logging.py`

 * *Files identical despite different names*

### Comparing `metron_tagger-2.2.4/metrontagger/options.py` & `metron_tagger-2.3.0/metrontagger/options.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,14 +70,20 @@
     parser.add_argument(
         "--validate",
         help="Verify that comic archive has a valid ComicInfo.xml.",
         action="store_true",
         default=False,
     )
     parser.add_argument(
+        "--remove-non-valid",
+        help="Remove ComicInfo.xml from comic if not valid. Used with --validate option",
+        action="store_true",
+        default=False,
+    )
+    parser.add_argument(
         "--delete-original",
         help="Delete the original archive after successful export to another format.",
         action="store_true",
         default=False,
     )
     parser.add_argument(
         "--duplicates",
```

### Comparing `metron_tagger-2.2.4/metrontagger/run.py` & `metron_tagger-2.3.0/metrontagger/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
             else:
                 questionary.print(
                     f"'{comic.name}' is not a cbr archive. skipping...",
                     style=Styles.WARNING,
                 )
 
     @staticmethod
-    def _validate_comic_info(file_list: list[Path]) -> None:
+    def _validate_comic_info(file_list: list[Path], remove_ci: bool = False) -> None:
         questionary.print("\nValidating ComicInfo:\n---------------------", style=Styles.TITLE)
         for comic in file_list:
             ca = Comic(str(comic))
             if not ca.has_metadata():
                 questionary.print(
                     f"'{ca.path.name}' doesn't have a ComicInfo.xml file.",
                     style=Styles.WARNING,
@@ -111,14 +111,19 @@
             elif result == SchemaVersion.v1:
                 questionary.print(
                     f"'{ca.path.name}' is a valid ComicInfo Version 1",
                     style=Styles.SUCCESS,
                 )
             else:
                 questionary.print(f"'{ca.path.name}' is not valid", style=Styles.ERROR)
+                if remove_ci and ca.remove_metadata():
+                    questionary.print(
+                        f"Removed non-valid metadata from '{ca.path.name}'.",
+                        style=Styles.WARNING,
+                    )
 
     def _sort_comic_list(self: "Runner", file_list: list[Path]) -> None:
         if not self.config.sort_dir:
             questionary.print(
                 "\nUnable to sort files. No destination directory was provided.",
                 style=Styles.ERROR,
             )
@@ -327,8 +332,8 @@
         if self.config.sort:
             if not self.config.sort_dir and not self._get_sort_dir():
                 questionary.print("No sort directory given. Exiting...")
                 sys.exit(0)
             self._sort_comic_list(file_list)
 
         if self.config.validate:
-            self._validate_comic_info(file_list)
+            self._validate_comic_info(file_list, self.config.remove_non_valid)
```

### Comparing `metron_tagger-2.2.4/metrontagger/schema/v1/ComicInfo.xsd` & `metron_tagger-2.3.0/metrontagger/schema/v1/ComicInfo.xsd`

 * *Files identical despite different names*

### Comparing `metron_tagger-2.2.4/metrontagger/schema/v2/ComicInfo.xsd` & `metron_tagger-2.3.0/metrontagger/schema/v2/ComicInfo.xsd`

 * *Files identical despite different names*

### Comparing `metron_tagger-2.2.4/metrontagger/settings.py` & `metron_tagger-2.3.0/metrontagger/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
         self.rename: bool = False
         self.sort: bool = False
         self.interactive: bool = False
         self.ignore_existing: bool = False
         self.export_to_cbz: bool = False
         self.delete_original: bool = False
         self.validate: bool = False
+        self.remove_non_valid: bool = False
         self.duplicates: bool = False
 
         # Rename settings
         self.rename_template = "%series% v%volume% #%issue% (%year%)"
         self.rename_issue_number_padding = 3
         self.rename_use_smart_string_cleanup = True
```

### Comparing `metron_tagger-2.2.4/metrontagger/talker.py` & `metron_tagger-2.3.0/metrontagger/talker.py`

 * *Files identical despite different names*

### Comparing `metron_tagger-2.2.4/metrontagger/utils.py` & `metron_tagger-2.3.0/metrontagger/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Some miscellaneous functions"""
 
 from urllib.parse import quote_plus
 
 
-def cleanup_string(path_name: str | None) -> str | None:
+def cleanup_string(path_name: int | str | None) -> str | None:
     """Function to remove some characters that don't play nicely on Windows machines filesystem"""
     if path_name is None:
         return None
 
     if isinstance(path_name, int):
         path_name = str(path_name)
```

### Comparing `metron_tagger-2.2.4/metrontagger/validate_ci.py` & `metron_tagger-2.3.0/metrontagger/validate_ci.py`

 * *Files identical despite different names*

### Comparing `metron_tagger-2.2.4/pyproject.toml` & `metron_tagger-2.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.1.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "metron-tagger"
-version = "2.2.4"
+version = "2.3.0"
 description = "A program to write metadata from metron.cloud to a comic archive"
 authors = ["Brian Pepple <bpepple@metron.cloud>"]
 license = "GPL-3.0-or-later"
 maintainers = ["Brian Pepple <bpepple@metron.cloud>"]
 readme = "README.rst"
 packages = [{ include = "metrontagger" }]
 exclude = ["*/**/*~"]
```

### Comparing `metron_tagger-2.2.4/tests/conftest.py` & `metron_tagger-2.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `metron_tagger-2.2.4/tests/test_filerenamer.py` & `metron_tagger-2.3.0/tests/test_filerenamer.py`

 * *Files identical despite different names*

### Comparing `metron_tagger-2.2.4/tests/test_filesorter.py` & `metron_tagger-2.3.0/tests/test_filesorter.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,30 @@
     comic.write_metadata(fake_metadata)
     file_sorter = FileSorter(str(test_dir))
     res = file_sorter.sort_comics(Path(str(fake_comic)))
     assert res is False
 
 
 @pytest.mark.skipif(sys.platform in ["win32"], reason="Skip Windows.")
+def test_sort_comic_with_no_series_metadata(
+    fake_comic: ZipFile, fake_metadata: Metadata, tmp_path: Path
+) -> None:
+    test_dir = tmp_path / "sort2"
+    fake_metadata.series = None
+    comic = Comic(str(fake_comic))
+    if comic.has_metadata():
+        comic.remove_metadata()
+    comic.write_metadata(fake_metadata)
+    assert comic.has_metadata()
+    file_sorter = FileSorter(str(test_dir))
+    res = file_sorter.sort_comics(Path(str(fake_comic)))
+    assert res is False
+
+
+@pytest.mark.skipif(sys.platform in ["win32"], reason="Skip Windows.")
 def test_sort_comic(fake_comic: ZipFile, fake_metadata: Metadata, tmp_path: Path) -> None:
     test_dir = tmp_path / "sort1"
 
     test_dir.mkdir()
 
     result_dir = (
         test_dir
```

### Comparing `metron_tagger-2.2.4/tests/test_metron_tagger.py` & `metron_tagger-2.3.0/tests/test_metron_tagger.py`

 * *Files identical despite different names*

### Comparing `metron_tagger-2.2.4/tests/test_options.py` & `metron_tagger-2.3.0/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `metron_tagger-2.2.4/tests/test_settings.py` & `metron_tagger-2.3.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `metron_tagger-2.2.4/tests/test_talker.py` & `metron_tagger-2.3.0/tests/test_talker.py`

 * *Files identical despite different names*

### Comparing `metron_tagger-2.2.4/tests/test_utils.py` & `metron_tagger-2.3.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `metron_tagger-2.2.4/PKG-INFO` & `metron_tagger-2.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metron-tagger
-Version: 2.2.4
+Version: 2.3.0
 Summary: A program to write metadata from metron.cloud to a comic archive
 License: GPL-3.0-or-later
 Keywords: comics,comic,metadata,tagging,tagger
 Author: Brian Pepple
 Author-email: bpepple@metron.cloud
 Maintainer: Brian Pepple
 Maintainer-email: bpepple@metron.cloud
@@ -100,14 +100,15 @@
     -d, --delete         Delete the metadata tags from the file. (default: False)
     --ignore-existing    Ignore files that have existing metadata tag. (default: False)
     -i, --interactive    Interactively query the user when there are matches for an online search. (default: False)
     --missing            List files without metadata. (default: False)
     -s, --sort           Sort files that contain metadata tags. (default: False)
     -z, --export-to-cbz  Export a CBR (rar) archive to a CBZ (zip) archive. (default: False)
     --validate           Verify that comic archive has a valid ComicInfo.xml. (default: False)
+    --remove-non-valid   Remove ComicInfo.xml from comic if not valid. Used with --validate option (default: False)
     --delete-original    Delete the original archive after successful export to another format. (default: False)
     --duplicates         Identify and give the option to delete duplicate pages in a directory of comics. (Experimental) (default: False)
     --version            Show the version number and exit
 
 Bugs/Requests
 -------------
```

