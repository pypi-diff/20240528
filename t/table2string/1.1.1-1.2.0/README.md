# Comparing `tmp/table2string-1.1.1.tar.gz` & `tmp/table2string-1.2.0.tar.gz`

## Comparing `table2string-1.1.1.tar` & `table2string-1.2.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 table2string-1.1.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 table2string-1.1.1/.github/workflows/tests.yml
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 table2string-1.1.1/table2string/__init__.py
--rw-r--r--   0        0        0    10545 2020-02-02 00:00:00.000000 table2string-1.1.1/table2string/table2string.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 table2string-1.1.1/tests/__init__.py
--rw-r--r--   0        0        0    17959 2020-02-02 00:00:00.000000 table2string-1.1.1/tests/test_table2string.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 table2string-1.1.1/.gitignore
--rw-r--r--   0        0        0    18047 2020-02-02 00:00:00.000000 table2string-1.1.1/LICENSE
--rw-r--r--   0        0        0     5451 2020-02-02 00:00:00.000000 table2string-1.1.1/README.md
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 table2string-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     6447 2020-02-02 00:00:00.000000 table2string-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 table2string-1.2.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 table2string-1.2.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 table2string-1.2.0/table2string/__init__.py
+-rw-r--r--   0        0        0     5571 2020-02-02 00:00:00.000000 table2string-1.2.0/table2string/table2string.py
+-rw-r--r--   0        0        0     6466 2020-02-02 00:00:00.000000 table2string-1.2.0/table2string/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 table2string-1.2.0/tests/__init__.py
+-rw-r--r--   0        0        0    22042 2020-02-02 00:00:00.000000 table2string-1.2.0/tests/test_table2string.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 table2string-1.2.0/.gitignore
+-rw-r--r--   0        0        0    18047 2020-02-02 00:00:00.000000 table2string-1.2.0/LICENSE
+-rw-r--r--   0        0        0     7776 2020-02-02 00:00:00.000000 table2string-1.2.0/README.md
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 table2string-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     8921 2020-02-02 00:00:00.000000 table2string-1.2.0/PKG-INFO
```

### Comparing `table2string-1.1.1/.github/workflows/publish.yml` & `table2string-1.2.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `table2string-1.1.1/.github/workflows/tests.yml` & `table2string-1.2.0/.github/workflows/tests.yml`

 * *Files 13% similar despite different names*

```diff
@@ -11,15 +11,18 @@
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["3.10", "3.11", "3.12", "pypy-3.10"]
+        python-version: [
+          "3.7", "3.8", "3.9", "3.10", "3.11", "3.12",
+          "pypy-3.7", "pypy-3.8", "pypy-3.9", "pypy-3.10",
+        ]
 
     steps:
     - uses: actions/checkout@v4
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v3
       with:
         python-version: ${{ matrix.python-version }}
```

### Comparing `table2string-1.1.1/tests/test_table2string.py` & `table2string-1.2.0/tests/test_table2string.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from table2string.table2string import (
+from table2string.table2string import stringify_table
+from table2string.utils import (
     decrease_numbers,
     transform_align,
     transform_width,
-    stringify_table,
     line_spliter,
     fill_line,
 )
 
 
 def test_decrease_numbers():
     assert decrease_numbers([2, 2, 3], 10) == [3, 3, 4]
@@ -44,14 +44,32 @@
         ["1", "2", "3", " ", "4", "5", "6"],
         ["↩", "↩", " ", " ", "↩", "↩", " "],
     )
     assert line_spliter("123\n456", 2) == (["12", "3", "45", "6"], ["↩", " ", "↩", " "])
     assert line_spliter("123\n456", 3) == (["123", "456"], [" ", " "])
     assert line_spliter("123\n\n456", 3) == (["123", " ", "456"], [" ", " ", " "])
 
+    assert line_spliter(
+        text="123\n456\n789",
+        width=3,
+        height=2,
+    ) == (["123", "456"], [" ", "…"])
+
+    assert line_spliter(
+        text="123\n456\n789",
+        width=3,
+        height=3,
+    ) == (["123", "456", "789"], [" ", " ", " "])
+
+    assert line_spliter(
+        text="123\n456",
+        width=3,
+        height=3,
+    ) == (["123", "456"], [" ", " "])
+
 
 def test_fill_line():
     assert (
         fill_line(
             [["1", "2", "3", "4", "5", "6"]],
             [["↩", "↩", " ", "↩", "↩", " "]],
             [1],
@@ -735,7 +753,140 @@
 | 3 | 4 |
 | 5 | 6 |
 +---+---+
 | 7 | 8 |
 +---+---+
 """.strip()
     )
+    table_18 = [("123\n456\n789",)]
+    assert (
+        stringify_table(
+            table=table_18,
+            max_width=(3,),
+            max_height=3,
+        )
+        == stringify_table(
+            table=table_18,
+            max_width=(3,),
+            max_height=3,
+            maximize_height=True,
+        )
+        == """
++-----+
+| 123 |
+| 456 |
+| 789 |
++-----+
+""".strip()
+    )
+    assert (
+        stringify_table(
+            table=table_18,
+            max_width=(3,),
+            max_height=2,
+            maximize_height=True,
+        )
+        == """
++-----+
+| 123 |
+| 456…|
++-----+
+""".strip()
+    )
+    assert (
+        stringify_table(
+            table=table_18,
+            max_width=(3,),
+            max_height=4,
+            maximize_height=True,
+        )
+        == """
++-----+
+| 123 |
+| 456 |
+| 789 |
+|     |
++-----+
+""".strip()
+    )
+    assert (
+        stringify_table(
+            table=table_18,
+            max_width=(3,),
+            max_height=8,
+            maximize_height=True,
+        )
+        == """
++-----+
+| 123 |
+| 456 |
+| 789 |
+|     |
+|     |
+|     |
+|     |
+|     |
++-----+
+""".strip()
+    )
+    assert (
+        stringify_table(
+            table=[
+                ("City name", "Area", "Population", "Annual Rainfall"),
+                ("Adelaide", 1295, 1158259, 600.5),
+                ("Brisbane", 5905, 1857594, 1146.4),
+                ("Darwin", 112, 120900, 1714.7),
+                ("Hobart", 1357, 205556, 619.5),
+                ("Sydney", 2058, 4336374, 1214.8),
+                ("Melbourne", 1566, 3806092, 646.9),
+                ("Perth", 5386, 1554769, 869.4),
+            ],
+            sep=(1,),
+        )
+        == """
++-----------+------+------------+-----------------+
+| City name | Area | Population | Annual Rainfall |
++-----------+------+------------+-----------------+
+| Adelaide  | 1295 |    1158259 |           600.5 |
+| Brisbane  | 5905 |    1857594 |          1146.4 |
+| Darwin    |  112 |     120900 |          1714.7 |
+| Hobart    | 1357 |     205556 |           619.5 |
+| Sydney    | 2058 |    4336374 |          1214.8 |
+| Melbourne | 1566 |    3806092 |           646.9 |
+| Perth     | 5386 |    1554769 |           869.4 |
++-----------+------+------------+-----------------+
+""".strip()
+    )
+    assert (
+        stringify_table(
+            table=[
+                ("City name", "Area", "Population", "Annual Rainfall"),
+                *sorted(
+                    [
+                        ("Adelaide", 1295, 1158259, 600.5),
+                        ("Brisbane", 5905, 1857594, 1146.4),
+                        ("Darwin", 112, 120900, 1714.7),
+                        ("Hobart", 1357, 205556, 619.5),
+                        ("Sydney", 2058, 4336374, 1214.8),
+                        ("Melbourne", 1566, 3806092, 646.9),
+                        ("Perth", 5386, 1554769, 869.4),
+                    ],
+                    key=lambda x: x[3],
+                ),
+            ],
+            sep=(1, 5),
+        )
+        == """
++-----------+------+------------+-----------------+
+| City name | Area | Population | Annual Rainfall |
++-----------+------+------------+-----------------+
+| Adelaide  | 1295 |    1158259 |           600.5 |
+| Hobart    | 1357 |     205556 |           619.5 |
+| Melbourne | 1566 |    3806092 |           646.9 |
+| Perth     | 5386 |    1554769 |           869.4 |
++-----------+------+------------+-----------------+
+| Brisbane  | 5905 |    1857594 |          1146.4 |
+| Sydney    | 2058 |    4336374 |          1214.8 |
+| Darwin    |  112 |     120900 |          1714.7 |
++-----------+------+------------+-----------------+
+""".strip()
+    )
```

### Comparing `table2string-1.1.1/LICENSE` & `table2string-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `table2string-1.1.1/pyproject.toml` & `table2string-1.2.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "table2string"
-version = "1.1.1"
+version = "1.2.0"
 description = "A library to convert tables to string with full support for line breaks and formatting"
 authors = [{name = "EgorKhabarov", email = "not.a.fan.of.broccoli@gmail.com"}]
 license = {text = "GPL2"}
 readme = "README.md"
-requires-python = ">=3.10"
+requires-python = ">=3.7"
 keywords = ["table", "string", "tools"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Environment :: Console",
     "License :: OSI Approved :: GNU General Public License v2 (GPLv2)"
 ]
 dependencies = []
```

### Comparing `table2string-1.1.1/PKG-INFO` & `table2string-1.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 Metadata-Version: 2.3
 Name: table2string
-Version: 1.1.1
+Version: 1.2.0
 Summary: A library to convert tables to string with full support for line breaks and formatting
 Project-URL: Homepage, https://github.com/EgorKhabarov/table2string
 Project-URL: Documentation, https://github.com/EgorKhabarov/table2string
 Project-URL: Repository, https://github.com/EgorKhabarov/table2string
 Project-URL: Issues, https://github.com/EgorKhabarov/table2string/issues
 Author-email: EgorKhabarov <not.a.fan.of.broccoli@gmail.com>
 License: GPL2
 License-File: LICENSE
 Keywords: string,table,tools
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.10
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # table2string
 
 [![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/EgorKhabarov/table2string/tests.yml?style=flat&logo=GitHub&label=Tests)](https://github.com/EgorKhabarov/table2string/actions/workflows/tests.yml)
+[![Publish Python Package to PyPI](https://img.shields.io/github/actions/workflow/status/EgorKhabarov/table2string/publish.yml?style=flat&logo=GitHub&label=Publish%20to%20PyPI)](https://github.com/EgorKhabarov/table2string/actions/workflows/publish.yml)
 
 [![PyPi Package Version](https://img.shields.io/pypi/v/table2string.svg?style=flat&logo=pypi)](https://pypi.python.org/pypi/table2string)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/table2string.svg?style=flat&logo=pypi)](https://pypi.python.org/pypi/table2string)
 [![PyPi status](https://img.shields.io/pypi/status/table2string.svg?style=flat&logo=pypi)](https://pypi.python.org/pypi/table2string)
 [![PyPi downloads](https://img.shields.io/pypi/dm/table2string.svg?style=flat&logo=pypi)](https://pypi.org/project/table2string/)
 
 ## Convert table to string
@@ -63,15 +67,15 @@
 |  Table Name   |
 +-----+-----+---+
 |   1 |   2 | 3 |
 +-----+-----+---+
 | qwe | rty |   |
 |     | uio |   |
 +-----+-----+---+
->>> print(stringify_table([("1", "2", "3"), ("qwe", "rty\nuio", "")], name="Table Name"), end="")
+>>> print(stringify_table([("1", "2", "3"), ("qwe", "rty\nuio", "")], name="Table Name"))
 +---------------+
 |  Table Name   |
 +-----+-----+---+
 |   1 |   2 | 3 |
 +-----+-----+---+
 | qwe | rty |   |
 |     | uio |   |
@@ -108,50 +112,131 @@
 |     |      |
 | 789…|      |
 +-----+------+
 >>> print_table([("123456789",)], max_width=(1,), max_height=1)
 +---+
 | 1…|
 +---+
+>>> print_table(
+...     table=[("123\n456\n789",)],
+...     max_width=(3,),
+...     max_height=4,
+...     maximize_height=True,
+... )
++-----+
+| 123 |
+| 456 |
+| 789 |
+|     |
++-----+
+>>> print_table(
+...     table=[("123456789",)],
+...     max_width=(3,),
+...     max_height=4,
+...     maximize_height=True,
+... )
++-----+
+| 123↩|
+| 456↩|
+| 789 |
+|     |
++-----+
 
 ```
 
 ## Text alignment
 
 ```pycon
->>> print_table([("1", "example")], max_width=25, name="Table Name", align="<", name_align="<")
-+-----------------------+
-| Table Name            |
-+-----------+-----------+
-| 1         | example   |
-+-----------+-----------+
->>> print_table([("1", "example")], max_width=25, name="Table Name", align=">", name_align=">")
-+-----------------------+
-|            Table Name |
-+-----------+-----------+
-|         1 |   example |
-+-----------+-----------+
->>> print_table([("1", "example")], max_width=25, name="Table Name", align="^", name_align="^")
-+-----------------------+
-|      Table Name       |
-+-----------+-----------+
-|     1     |  example  |
-+-----------+-----------+
->>> print_table([("1", "example")], max_width=25, name="Table Name", align="*", name_align="*")
-+-----------------------+
-| Table Name            |
-+-----------+-----------+
-|         1 | example   |
-+-----------+-----------+
->>> print_table([("1", "example")], max_width=25, name="Table Name")
-+-----------------------+
-|      Table Name       |
-+-----------+-----------+
-|         1 | example   |
-+-----------+-----------+
+>>> kwargs_1 = {
+...     "table": [("1", "123456789\nqwerty\nasdfghjklzxcvb")],
+...     "name": "Table Name\nName\nNaaaaame",
+...     "max_width": (5, 15),
+... }
+>>> print_table(**kwargs_1)
++-------------------------+
+|       Table Name        |
+|          Name           |
+|        Naaaaame         |
++-------+-----------------+
+|     1 | 123456789       |
+|       | qwerty          |
+|       | asdfghjklzxcvb  |
++-------+-----------------+
+>>> print_table(**kwargs_1, align="*", name_align="*")  # align="**", name_align="**"
++-------------------------+
+| Table Name              |
+| Name                    |
+| Naaaaame                |
++-------+-----------------+
+|     1 | 123456789       |
+|       | qwerty          |
+|       | asdfghjklzxcvb  |
++-------+-----------------+
+>>> print_table(**kwargs_1, align="<", name_align="<")  # align="<<", name_align="<<"
++-------------------------+
+| Table Name              |
+| Name                    |
+| Naaaaame                |
++-------+-----------------+
+| 1     | 123456789       |
+|       | qwerty          |
+|       | asdfghjklzxcvb  |
++-------+-----------------+
+>>> print_table(**kwargs_1, align=">", name_align=">")  # align=">>", name_align=">>"
++-------------------------+
+|              Table Name |
+|                    Name |
+|                Naaaaame |
++-------+-----------------+
+|     1 |       123456789 |
+|       |          qwerty |
+|       |  asdfghjklzxcvb |
++-------+-----------------+
+>>> print_table(**kwargs_1, align="^", name_align="^")  # align="^^", name_align="^^"
++-------------------------+
+|       Table Name        |
+|          Name           |
+|        Naaaaame         |
++-------+-----------------+
+|   1   |    123456789    |
+|       |     qwerty      |
+|       | asdfghjklzxcvb  |
++-------+-----------------+
+>>> print_table(**kwargs_1, align="^<", name_align="^<")
++-------------------------+
+|       Table Name        |
+|       Name              |
+|       Naaaaame          |
++-------+-----------------+
+|   1   | 123456789       |
+|       | qwerty          |
+|       | asdfghjklzxcvb  |
++-------+-----------------+
+>>> print_table(**kwargs_1, align="^>", name_align="^>")
++-------------------------+
+|       Table Name        |
+|             Name        |
+|         Naaaaame        |
++-------+-----------------+
+|   1   |      123456789  |
+|       |         qwerty  |
+|       | asdfghjklzxcvb  |
++-------+-----------------+
+>>> print_table([("qwerty\n123456789\nasdfghjklzxcvb",)], max_width=(18,), align="^<")
++--------------------+
+|   qwerty           |
+|   123456789        |
+|   asdfghjklzxcvb   |
++--------------------+
+>>> print_table([("qwerty\n123456789\nasdfghjklzxcvb",)], max_width=(18,), align="^>")
++--------------------+
+|           qwerty   |
+|        123456789   |
+|   asdfghjklzxcvb   |
++--------------------+
 
 ```
 
 # Separator settings
 
 ```pycon
 >>> table_1 = [("qwe", "rty\nuio"), ("123456\n\n789000", "example")]
```

