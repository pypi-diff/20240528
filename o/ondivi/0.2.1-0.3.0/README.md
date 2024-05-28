# Comparing `tmp/ondivi-0.2.1.tar.gz` & `tmp/ondivi-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ondivi-0.2.1.tar", max compression
+gzip compressed data, was "ondivi-0.3.0.tar", max compression
```

## Comparing `ondivi-0.2.1.tar` & `ondivi-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1109 2024-05-27 12:11:26.056879 ondivi-0.2.1/LICENSE
--rw-r--r--   0        0        0     1624 2024-05-27 12:11:26.056879 ondivi-0.2.1/README.md
--rw-r--r--   0        0        0      151 2024-05-27 12:11:26.056879 ondivi-0.2.1/ondivi/__init__.py
--rw-r--r--   0        0        0     4448 2024-05-27 12:11:26.056879 ondivi-0.2.1/ondivi/__main__.py
--rw-r--r--   0        0        0     3770 2024-05-27 12:11:26.368882 ondivi-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2108 1970-01-01 00:00:00.000000 ondivi-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1109 2024-05-28 12:20:53.382493 ondivi-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1624 2024-05-28 12:20:53.382493 ondivi-0.3.0/README.md
+-rw-r--r--   0        0        0      151 2024-05-28 12:20:53.382493 ondivi-0.3.0/ondivi/__init__.py
+-rw-r--r--   0        0        0     5821 2024-05-28 12:20:53.382493 ondivi-0.3.0/ondivi/__main__.py
+-rw-r--r--   0        0        0     3772 2024-05-28 12:20:53.882498 ondivi-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2104 1970-01-01 00:00:00.000000 ondivi-0.3.0/PKG-INFO
```

### Comparing `ondivi-0.2.1/LICENSE` & `ondivi-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ondivi-0.2.1/README.md` & `ondivi-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ondivi-0.2.1/ondivi/__main__.py` & `ondivi-0.3.0/ondivi/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -32,42 +32,77 @@
 
 from git import Repo
 
 Diff = str
 FileName = str
 
 
-def define_changed_lines(diff: Diff) -> dict[FileName, list[int]]:  # noqa: WPS210. TODO: too many local variables
+def define_changed_lines(diff: Diff) -> dict[FileName, list[int]]:
     """Define changed lines in file.
 
+    Example of diff:
+
+    +---------------------------------------------------------------------+
+    │ diff --git a/ondivi/__main__.py b/ondivi/__main__.py                | <- filename
+    | index 669d0ff..7a518fa 100644                                       |
+    | --- a/ondivi/__main__.py                                            |
+    | +++ b/ondivi/__main__.py                                            |
+    | @@ -26,0 +27,2 @@ from git import Repo                              | <- Changed lines = [27, 28]
+    | +Diff = str                                                         |
+    | +FileName = str                                                     |
+    | @@ -28 +30,2 @@ from git import Repo                                | <- Changed lines = [27, 28, 30, 31]
+    | -def define_changed_lines(diff):                                    |
+    | +                                                                   |
+    | +def define_changed_lines(diff: Diff) -> dict[FileName, list[int]]: |
+    +---------------------------------------------------------------------+
+
     :param diff: Diff
     :return: dict[FileName, list[int]]
     """
     res: dict[FileName, list[int]] = {}
     current_file = ''
     for line in diff.splitlines():
-        if line.startswith('diff --git'):
+        if _line_contain_filename(line):
             current_file = line.split(' b/')[-1].strip()
             res[current_file] = []
-        elif line.startswith('@@'):
-            splitted_line = line.split('@@')[1].strip()
-            added_lines = splitted_line.split('+')[1]
-            start_line = int(
-                added_lines.split(',')[0],
-            )
-            if ',' not in added_lines:  # noqa: SIM108. Too complexity line
-                num_lines = 0
-            else:
-                num_lines = int(added_lines.split(',')[1]) - 1
-            res[current_file].extend(list(range(
-                start_line, start_line + num_lines + 1,
-            )))
+        elif _diff_line_contain_changed_lines(line):
+            res[current_file].extend(_changed_lines(line))
     return res
 
 
+def _line_contain_filename(diff_line: str) -> bool:
+    return diff_line.startswith('diff --git')
+
+
+def _diff_line_contain_changed_lines(diff_line: str) -> bool:
+    return diff_line.startswith('@@')
+
+
+def _changed_lines(diff_line: str) -> list[int]:
+    """Changed lines.
+
+    >>> _changed_lines('@@ -28 +30,2 @@ from git import Repo')
+    [30, 31]
+
+    :param diff_line: str
+    :return: list[int]
+    """
+    splitted_line = diff_line.split('@@')[1].strip()
+    added_lines = splitted_line.split('+')[1]
+    start_line = int(
+        added_lines.split(',')[0],
+    )
+    num_lines = 0
+    if ',' in added_lines:
+        num_lines = int(added_lines.split(',')[1]) - 1
+    return list(range(
+        start_line, start_line + num_lines + 1,
+    ))
+
+
 def filter_out_violations(
     changed_lines: dict[FileName, list[int]],
     violations: list[str],
 ) -> list[str]:
     """Collect target violations.
 
     :param changed_lines: dict[FileName, list[int]], violations: list[str]
@@ -118,19 +153,19 @@
         help=' '.join([
             'Commit or branch which will contain legacy code.',
             'Program filter out violations on baseline',
             '(default: "master")',
         ]),
     )
     args = parser.parse_args()
-    violations = sys.stdin.read().strip().splitlines()
-    sys.stdout.write('\n'.join(
-        controller(
-            Repo('.').git.diff('--unified=0', args.baseline),
-            violations,
-        ),
-    ))
+    violations = controller(
+        Repo('.').git.diff('--unified=0', args.baseline),
+        sys.stdin.read().strip().splitlines(),
+    )
+    sys.stdout.write('\n'.join(violations))
     sys.stdout.write('\n')
+    if violations:
+        sys.exit(1)
 
 
 if __name__ == '__main__':
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ondivi-0.2.1/pyproject.toml` & `ondivi-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -18,22 +18,22 @@
 # IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 # DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 # OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 # OR OTHER DEALINGS IN THE SOFTWARE.
 
 [tool.poetry]
 name = "ondivi"
-version = "0.2.1"
+version = "0.3.0"
 description = ""
 authors = ["Almaz Ilaletdinov <a.ilaletdinov@yandex.ru>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
-gitpython = "^3.0"
+gitpython = ">=2,<4"
 
 [tool.poetry.scripts]
 ondivi = "ondivi.__main__:main"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "0.4.5"
 wemake-python-styleguide = "0.19.2"
```

### Comparing `ondivi-0.2.1/PKG-INFO` & `ondivi-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: ondivi
-Version: 0.2.1
+Version: 0.3.0
 Summary: 
 Author: Almaz Ilaletdinov
 Author-email: a.ilaletdinov@yandex.ru
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: gitpython (>=3.0,<4.0)
+Requires-Dist: gitpython (>=2,<4)
 Description-Content-Type: text/markdown
 
 # Ondivi (Only diff violations)
 
 [![wemake-python-styleguide](https://img.shields.io/badge/style-wemake-000000.svg)](https://github.com/wemake-services/wemake-python-styleguide)
 [![Lines of code](https://tokei.rs/b1/github/blablatdinov/ondivi)](https://github.com/XAMPPRocky/tokei)
 [![Hits-of-Code](https://hitsofcode.com/github/blablatdinov/ondivi)](https://hitsofcode.com/github/blablatdinov/quranbot-aiogram/view)
```

