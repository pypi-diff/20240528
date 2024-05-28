# Comparing `tmp/yedextended-1.0.9.tar.gz` & `tmp/yedextended-2.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yedextended-1.0.9.tar", last modified: Wed May  1 12:49:04 2024, max compression
+gzip compressed data, was "yedextended-2.0.0a0.tar", last modified: Tue May 28 12:26:01 2024, max compression
```

## Comparing `yedextended-1.0.9.tar` & `yedextended-2.0.0a0.tar`

### file list

```diff
@@ -1,52 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:49:04.388076 yedextended-1.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-01 12:48:58.000000 yedextended-1.0.9/.deepsource.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:49:04.380076 yedextended-1.0.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:49:04.380076 yedextended-1.0.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-01 12:48:58.000000 yedextended-1.0.9/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-01 12:48:58.000000 yedextended-1.0.9/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-01 12:48:58.000000 yedextended-1.0.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-01 12:48:58.000000 yedextended-1.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7975 2024-05-01 12:49:04.388076 yedextended-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7171 2024-05-01 12:48:58.000000 yedextended-1.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:49:04.384076 yedextended-1.0.9/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-01 12:48:58.000000 yedextended-1.0.9/examples/demo-basic-create-and-open.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-01 12:48:58.000000 yedextended-1.0.9/examples/demo-basic-formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-01 12:48:58.000000 yedextended-1.0.9/examples/demo-basic_bulk_manage1.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-01 12:48:58.000000 yedextended-1.0.9/examples/demo-basic_bulk_manage2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-01 12:48:58.000000 yedextended-1.0.9/examples/demo-custom-properties-nodes-edges.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-01 12:48:58.000000 yedextended-1.0.9/examples/demo-multilabels.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-01 12:48:58.000000 yedextended-1.0.9/examples/demo-round-robin_read_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-01 12:48:58.000000 yedextended-1.0.9/examples/demo-uml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-01 12:48:58.000000 yedextended-1.0.9/examples/demo-url-description-groups-nodes-edges.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-01 12:48:58.000000 yedextended-1.0.9/examples/readme-1.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-01 12:48:58.000000 yedextended-1.0.9/examples/readme-2.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-01 12:48:58.000000 yedextended-1.0.9/examples/readme-3.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-01 12:48:58.000000 yedextended-1.0.9/examples/test.csv
--rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-05-01 12:48:58.000000 yedextended-1.0.9/examples/test.graphml
--rw-r--r--   0 runner    (1001) docker     (127)    12020 2024-05-01 12:48:58.000000 yedextended-1.0.9/examples/yed_created_edges.graphml
--rw-r--r--   0 runner    (1001) docker     (127)     5078 2024-05-01 12:48:58.000000 yedextended-1.0.9/examples/yed_modified_app_created.graphml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:49:04.384076 yedextended-1.0.9/images/
--rw-r--r--   0 runner    (1001) docker     (127)    10876 2024-05-01 12:48:58.000000 yedextended-1.0.9/images/demo_multilabel.png
--rw-r--r--   0 runner    (1001) docker     (127)    14894 2024-05-01 12:48:58.000000 yedextended-1.0.9/images/example-UML.png
--rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-05-01 12:48:58.000000 yedextended-1.0.9/images/example.png
--rw-r--r--   0 runner    (1001) docker     (127)    10047 2024-05-01 12:48:58.000000 yedextended-1.0.9/images/excel_obj_entry.gif
--rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-05-01 12:48:58.000000 yedextended-1.0.9/images/excel_rel_entry.gif
--rw-r--r--   0 runner    (1001) docker     (127)    14361 2024-05-01 12:48:58.000000 yedextended-1.0.9/images/graph.gif
--rw-r--r--   0 runner    (1001) docker     (127)     7257 2024-05-01 12:48:58.000000 yedextended-1.0.9/images/graph_from_excel_obj.gif
--rw-r--r--   0 runner    (1001) docker     (127)     8913 2024-05-01 12:48:58.000000 yedextended-1.0.9/images/graph_from_excel_rel.gif
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-05-01 12:48:58.000000 yedextended-1.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-01 12:48:58.000000 yedextended-1.0.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 12:49:04.388076 yedextended-1.0.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:49:04.380076 yedextended-1.0.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:49:04.384076 yedextended-1.0.9/src/yedextended/
--rw-r--r--   0 runner    (1001) docker     (127)    73127 2024-05-01 12:48:58.000000 yedextended-1.0.9/src/yedextended/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:49:04.388076 yedextended-1.0.9/src/yedextended.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7975 2024-05-01 12:49:04.000000 yedextended-1.0.9/src/yedextended.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-01 12:49:04.000000 yedextended-1.0.9/src/yedextended.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 12:49:04.000000 yedextended-1.0.9/src/yedextended.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-01 12:49:04.000000 yedextended-1.0.9/src/yedextended.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-01 12:49:04.000000 yedextended-1.0.9/src/yedextended.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-01 12:48:58.000000 yedextended-1.0.9/test_coverage.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:49:04.384076 yedextended-1.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:48:58.000000 yedextended-1.0.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-05-01 12:48:58.000000 yedextended-1.0.9/tests/test_yedextended.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:26:01.496098 yedextended-2.0.0a0/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-28 12:25:35.000000 yedextended-2.0.0a0/.deepsource.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:26:01.488098 yedextended-2.0.0a0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:26:01.488098 yedextended-2.0.0a0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-28 12:25:35.000000 yedextended-2.0.0a0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-28 12:25:35.000000 yedextended-2.0.0a0/.github/workflows/ci.yml.bak
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-28 12:25:35.000000 yedextended-2.0.0a0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-28 12:25:35.000000 yedextended-2.0.0a0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-28 12:25:35.000000 yedextended-2.0.0a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8322 2024-05-28 12:26:01.496098 yedextended-2.0.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-05-28 12:25:35.000000 yedextended-2.0.0a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-28 12:25:35.000000 yedextended-2.0.0a0/ci.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-28 12:25:35.000000 yedextended-2.0.0a0/coverage_sticker.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:26:01.492098 yedextended-2.0.0a0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-28 12:25:35.000000 yedextended-2.0.0a0/examples/demo-basic-create-and-open.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-28 12:25:35.000000 yedextended-2.0.0a0/examples/demo-basic-formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-28 12:25:35.000000 yedextended-2.0.0a0/examples/demo-basic_bulk_manage1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-28 12:25:35.000000 yedextended-2.0.0a0/examples/demo-basic_bulk_manage2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-28 12:25:35.000000 yedextended-2.0.0a0/examples/demo-custom-properties-nodes-edges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-05-28 12:25:35.000000 yedextended-2.0.0a0/examples/demo-multilabels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-28 12:25:35.000000 yedextended-2.0.0a0/examples/demo-round-robin_read_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-28 12:25:35.000000 yedextended-2.0.0a0/examples/demo-some-props.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-28 12:25:35.000000 yedextended-2.0.0a0/examples/demo-uml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-28 12:25:35.000000 yedextended-2.0.0a0/examples/demo-url-description-groups-nodes-edges.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-28 12:25:35.000000 yedextended-2.0.0a0/examples/readme-1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-28 12:25:35.000000 yedextended-2.0.0a0/examples/readme-2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-28 12:25:35.000000 yedextended-2.0.0a0/examples/readme-3.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-28 12:25:35.000000 yedextended-2.0.0a0/examples/test.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-05-28 12:25:35.000000 yedextended-2.0.0a0/examples/test.graphml
+-rw-r--r--   0 runner    (1001) docker     (127)    10564 2024-05-28 12:25:35.000000 yedextended-2.0.0a0/examples/yed_created_edges.graphml
+-rw-r--r--   0 runner    (1001) docker     (127)    14842 2024-05-28 12:25:35.000000 yedextended-2.0.0a0/examples/yed_created_edges_deeper.graphml
+-rw-r--r--   0 runner    (1001) docker     (127)     7852 2024-05-28 12:25:35.000000 yedextended-2.0.0a0/examples/yed_created_edges_obj.graphml
+-rw-r--r--   0 runner    (1001) docker     (127)     9055 2024-05-28 12:25:35.000000 yedextended-2.0.0a0/examples/yed_created_edges_simplified.graphml
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-28 12:25:35.000000 yedextended-2.0.0a0/examples/yed_created_empty_graph.graphml
+-rw-r--r--   0 runner    (1001) docker     (127)     5078 2024-05-28 12:25:35.000000 yedextended-2.0.0a0/examples/yed_modified_app_created.graphml
+-rw-r--r--   0 runner    (1001) docker     (127)     8510 2024-05-28 12:25:35.000000 yedextended-2.0.0a0/examples/yed_test_to_excel1.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)     9381 2024-05-28 12:25:35.000000 yedextended-2.0.0a0/examples/yed_test_to_excel2.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)     9379 2024-05-28 12:25:35.000000 yedextended-2.0.0a0/examples/yed_test_to_excel3.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:26:01.496098 yedextended-2.0.0a0/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    10876 2024-05-28 12:25:35.000000 yedextended-2.0.0a0/images/demo_multilabel.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14894 2024-05-28 12:25:35.000000 yedextended-2.0.0a0/images/example-UML.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-05-28 12:25:35.000000 yedextended-2.0.0a0/images/example.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10047 2024-05-28 12:25:35.000000 yedextended-2.0.0a0/images/excel_obj_entry.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-05-28 12:25:35.000000 yedextended-2.0.0a0/images/excel_rel_entry.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    14361 2024-05-28 12:25:35.000000 yedextended-2.0.0a0/images/graph.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     7257 2024-05-28 12:25:35.000000 yedextended-2.0.0a0/images/graph_from_excel_obj.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     8913 2024-05-28 12:25:35.000000 yedextended-2.0.0a0/images/graph_from_excel_rel.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-05-28 12:25:35.000000 yedextended-2.0.0a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-28 12:25:35.000000 yedextended-2.0.0a0/requirements.dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-28 12:25:35.000000 yedextended-2.0.0a0/run_tests_simple.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 12:26:01.496098 yedextended-2.0.0a0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:26:01.488098 yedextended-2.0.0a0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:26:01.496098 yedextended-2.0.0a0/src/yedextended/
+-rw-r--r--   0 runner    (1001) docker     (127)    89865 2024-05-28 12:25:35.000000 yedextended-2.0.0a0/src/yedextended/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:26:01.496098 yedextended-2.0.0a0/src/yedextended.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8322 2024-05-28 12:26:01.000000 yedextended-2.0.0a0/src/yedextended.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-28 12:26:01.000000 yedextended-2.0.0a0/src/yedextended.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 12:26:01.000000 yedextended-2.0.0a0/src/yedextended.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-28 12:26:01.000000 yedextended-2.0.0a0/src/yedextended.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-28 12:26:01.000000 yedextended-2.0.0a0/src/yedextended.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-28 12:25:35.000000 yedextended-2.0.0a0/test_coverage.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:26:01.496098 yedextended-2.0.0a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:25:35.000000 yedextended-2.0.0a0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24494 2024-05-28 12:25:35.000000 yedextended-2.0.0a0/tests/test_yedextended.py
```

### Comparing `yedextended-1.0.9/.github/workflows/ci.yml` & `yedextended-2.0.0a0/.github/workflows/ci.yml.bak`

 * *Files 10% similar despite different names*

```diff
@@ -27,46 +27,44 @@
       uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
         
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        python -m pip install flake8 pytest coverage coverage-badge
+        python -m pip install flake8 pytest coverage coverage-badge setuptools
         python -m pip install -e .
-        if (Test-Path requirements.txt){ python -m pip install -r requirements.txt}
+        if (Test-Path requirements.dev.txt){ python -m pip install -r requirements.dev.txt}
         
     - name: Lint with flake8
       run: |
-        # stop the build if there are Python syntax errors or undefined names
+        # Stop the build if there are Python syntax errors or undefined names
         flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
-        # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
+        # Exit-zero treats all errors as warnings (you may want to adjust this)
         flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
         
-    - name: Run tests with pytest and with coverage information
+    - name: Run tests with pytest and coverage information
       run: |
         coverage run -m pytest .
-
+    
     - name: Generate and commit coverage report
       id: coverage-report
       if: matrix.python-version == '3.12'  # Execute only if Python version is 3.12
       run: |
-        # Run coverage report and capture the output
-        $coverage_output = coverage report -m
-        # Generate the SVG coverage badge
+        $coverage_output= coverage report -m
         coverage-badge -o test_coverage.svg -f
         
         # Configure Git with the author information
         git config --global user.email "info@colestjohn.com"
         git config --global user.name "cole-st-john"
         
         # Add the test_coverage.svg file to the repository
         git add test_coverage.svg
         
         # Commit the file with a message that includes the coverage output
-        git commit -m "Update test coverage badge -  ${coverage_output}"
+        git commit -m "Updated test coverage badge\n\nTest Coverage Results:\n\n${coverage_output}"
         
-        # Push the changes to the main branch
+        # Push the changes to the correct branch
         git push origin master
-        
+    
       env:
         GH_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `yedextended-1.0.9/.github/workflows/python-publish.yml` & `yedextended-2.0.0a0/.github/workflows/python-publish.yml`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # For more information see: https://docs.github.com/en/actions/automating-builds-and-tests/building-and-testing-python#publishing-to-package-registries
 
 # This workflow uses actions that are not certified by GitHub.
 # They are provided by a third-party and are governed by
 # separate terms of service, privacy policy, and support
 # documentation.
 
-name: Upload Python Package
+name: PyPI release
 
 on:
   release:
     types: [published]
 
 permissions:
   contents: read
```

### Comparing `yedextended-1.0.9/.gitignore` & `yedextended-2.0.0a0/.gitignore`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.9/LICENSE` & `yedextended-2.0.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.9/PKG-INFO` & `yedextended-2.0.0a0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 Metadata-Version: 2.1
 Name: yedextended
-Version: 1.0.9
+Version: 2.0.0a0
 Summary: Python library extending yEd functionality through programmatic interface to graphs.
 Author-email: Cole St John <info@colestjohn.com>
 Project-URL: Homepage, https://github.com/cole-st-john/yedextended
 Project-URL: Issues, https://github.com/cole-st-john/yedextended/issues
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: psutil
-Requires-Dist: pygetwindow
 Requires-Dist: openpyxl
 
 
 
 
 # Extended Python Support for yEd 
+
+[![Static Badge](https://img.shields.io/badge/PyPI%20-%20yEdExtended%20-%20GREEN?logoColor=0%2C0%2C255&color=0%2C1%2C1&link=https%3A%2F%2Fpypi.org%2Fproject%2Fyedextended%2F)](https://pypi.org/project/yedextended/)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/yedextended?color=2334D058)
 [![CI](https://github.com/cole-st-john/yEdExtended/actions/workflows/ci.yml/badge.svg)](https://github.com/cole-st-john/yEdExtended/actions/workflows/ci.yml)
 ![Test Coverage](https://raw.githubusercontent.com/cole-st-john/yedextended/master/test_coverage.svg)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/yedextended?color=2334D058)
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/w/cole-st-john/yedextended)
-<!-- ![PyPI - Downloads](https://img.shields.io/pypi/dm/yedextended?labelColor=2334D058) -->
+![PyPI - Downloads](https://img.shields.io/pypi/dm/yedextended)
 
 This Python library extends the functionality of the readily available and free interactive graph editing program [yEd](http://www.yworks.com/en/products_yed_about.html), through providing a programmatic interface to graphs (of the [GraphML](http://graphml.graphdrawingraph1.org/) file format), including the following use case or functions:
 
 - [x] creating graphs
 - [x] formatting graphs
 - [x] reading graphs
 - [x] bulk data addition or management (MS excel-based)
-- [x] management of the yEd application (starting, killing, maximizing)
+- [x] management of the yEd application (starting, killing, etc.)
 - [ ] enforcing rules on graphs
 - [ ] additional layout methods
 - [ ] graph comparison tools
 
 ![yEd Graph](https://raw.githubusercontent.com/cole-st-john/yedextended/master/images/graph.gif)
 
 
@@ -76,34 +77,35 @@
 With yEdExtended you can easily create graphs, either through hardcoding, or more practically, through porting data from any data source (databases, csv, xml, etc) into a graph and graph objects (nodes, groups, edges, properties):
 
 Hardcoding Example:
 ```python
 # Instantiate graph instance
 graph1 = yed.Graph()
 
-# Add arbitrary graph detail - nodes and edges
-graph1.add_node("a")
-graph1.add_node("b")
-graph1.add_edge("a", "b")
+# Adding arbitrary graph detail - nodes
+a = graph1.add_node("a")
+b = graph1.add_node("b")
+
+# Adding edge (using node objects)
+graph1.add_edge(a, b)
 
 # Add arbitrary graph detail - group and group objects
 group1 = graph1.add_group("group 1", shape="rectangle")
-group1.add_node("c")
-group1.add_node("d")
+
+# Adding edge using node names, under owning group
 group1.add_edge("c", "d")
 ```
 
 Programmatic Example:
 ```python
 # Adding graph objects based on csv input
-import csv
-with open("examples/test.csv", encoding="utf-8-sig") as csv_file: 
-	csv_reader = csv.reader(csv_file)
-	for row in csv_reader:
-	    graph1.add_node(row)
+with open("examples\\test.csv", encoding="utf-8-sig") as csv_file:
+    csv_reader = csv.reader(csv_file)
+    for row in csv_reader:
+        graph1.add_node(row[0])
 ```
 
 ## Reading existing GraphML files
 
 yEdExtended can read GraphML files into a Python class structure, allowing for simple programmatic analysis and modification:
 
 ```python
@@ -115,51 +117,37 @@
 
 ## Using formatting
 
 yEdExtended provides for the majority of formatting one expects in yEd graphs.
 
 ```python
 # Add graph nodes and edges with some examples of non-default formatting
-graph1.add_node(
-    "foo",
-    font_family="Zapfino",
-)
+graph1.add_node("foo", font_family="Zapfino")
 
 graph1.add_node(
     "foo2",
     shape="roundrectangle",
     font_style="bolditalic",
     underlined_text="true",
 )
 
-graph1.add_edge(
-    "foo1",
-    "foo2",
-)
-graph1.add_node(
-    "abc",
-    font_size="72",
-    height="100",
-)
+graph1.add_edge("foo1", "foo2")
 
-graph1.add_node(
-    "bar",
-    label="Multi\nline\ntext",
-)
-graph1.add_node(
-    "foobar",
-    label="""Multi
+graph1.add_node("abc", font_size="72", height="100")
+
+graph1.add_node("Multi\nline\ntext")
+
+graph1.add_node("foobar").add_label("""Multi
 Line
-Text!""",
-)
+Text!""")
 
 graph1.add_edge(
     "foo",
     "foo1",
-    label="EDGE!",
+    name="EDGE!",
     width="3.0",
     color="#0000FF",
     arrowhead="white_diamond",
     arrowfoot="standard",
     line_type="dotted",
 )
 ```
@@ -245,18 +233,27 @@
 
 # Development
 
 
 Interested in contributing or co-managing further development?  Just reach out!
 
 Dev. Requirements:
+
+Install yEd from [here](https://www.yworks.com/products/yed/download#download).
+
+Ensure you have [MS Excel](https://www.microsoft.com/en/microsoft-365/excel?market=af) installed.
+
 ```console
 $ pip install pytest
 ```
 
+```console
+$ setx CI "True"
+```
+
 To run the tests:
 ```console
 $ PYTHONPATH=. pytest tests
 ```
 
 References:
```

### Comparing `yedextended-1.0.9/README.md` & `yedextended-2.0.0a0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 
 
 
 # Extended Python Support for yEd 
+
+[![Static Badge](https://img.shields.io/badge/PyPI%20-%20yEdExtended%20-%20GREEN?logoColor=0%2C0%2C255&color=0%2C1%2C1&link=https%3A%2F%2Fpypi.org%2Fproject%2Fyedextended%2F)](https://pypi.org/project/yedextended/)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/yedextended?color=2334D058)
 [![CI](https://github.com/cole-st-john/yEdExtended/actions/workflows/ci.yml/badge.svg)](https://github.com/cole-st-john/yEdExtended/actions/workflows/ci.yml)
 ![Test Coverage](https://raw.githubusercontent.com/cole-st-john/yedextended/master/test_coverage.svg)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/yedextended?color=2334D058)
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/w/cole-st-john/yedextended)
-<!-- ![PyPI - Downloads](https://img.shields.io/pypi/dm/yedextended?labelColor=2334D058) -->
+![PyPI - Downloads](https://img.shields.io/pypi/dm/yedextended)
 
 This Python library extends the functionality of the readily available and free interactive graph editing program [yEd](http://www.yworks.com/en/products_yed_about.html), through providing a programmatic interface to graphs (of the [GraphML](http://graphml.graphdrawingraph1.org/) file format), including the following use case or functions:
 
 - [x] creating graphs
 - [x] formatting graphs
 - [x] reading graphs
 - [x] bulk data addition or management (MS excel-based)
-- [x] management of the yEd application (starting, killing, maximizing)
+- [x] management of the yEd application (starting, killing, etc.)
 - [ ] enforcing rules on graphs
 - [ ] additional layout methods
 - [ ] graph comparison tools
 
 ![yEd Graph](https://raw.githubusercontent.com/cole-st-john/yedextended/master/images/graph.gif)
 
 
@@ -56,34 +58,35 @@
 With yEdExtended you can easily create graphs, either through hardcoding, or more practically, through porting data from any data source (databases, csv, xml, etc) into a graph and graph objects (nodes, groups, edges, properties):
 
 Hardcoding Example:
 ```python
 # Instantiate graph instance
 graph1 = yed.Graph()
 
-# Add arbitrary graph detail - nodes and edges
-graph1.add_node("a")
-graph1.add_node("b")
-graph1.add_edge("a", "b")
+# Adding arbitrary graph detail - nodes
+a = graph1.add_node("a")
+b = graph1.add_node("b")
+
+# Adding edge (using node objects)
+graph1.add_edge(a, b)
 
 # Add arbitrary graph detail - group and group objects
 group1 = graph1.add_group("group 1", shape="rectangle")
-group1.add_node("c")
-group1.add_node("d")
+
+# Adding edge using node names, under owning group
 group1.add_edge("c", "d")
 ```
 
 Programmatic Example:
 ```python
 # Adding graph objects based on csv input
-import csv
-with open("examples/test.csv", encoding="utf-8-sig") as csv_file: 
-	csv_reader = csv.reader(csv_file)
-	for row in csv_reader:
-	    graph1.add_node(row)
+with open("examples\\test.csv", encoding="utf-8-sig") as csv_file:
+    csv_reader = csv.reader(csv_file)
+    for row in csv_reader:
+        graph1.add_node(row[0])
 ```
 
 ## Reading existing GraphML files
 
 yEdExtended can read GraphML files into a Python class structure, allowing for simple programmatic analysis and modification:
 
 ```python
@@ -95,51 +98,37 @@
 
 ## Using formatting
 
 yEdExtended provides for the majority of formatting one expects in yEd graphs.
 
 ```python
 # Add graph nodes and edges with some examples of non-default formatting
-graph1.add_node(
-    "foo",
-    font_family="Zapfino",
-)
+graph1.add_node("foo", font_family="Zapfino")
 
 graph1.add_node(
     "foo2",
     shape="roundrectangle",
     font_style="bolditalic",
     underlined_text="true",
 )
 
-graph1.add_edge(
-    "foo1",
-    "foo2",
-)
-graph1.add_node(
-    "abc",
-    font_size="72",
-    height="100",
-)
+graph1.add_edge("foo1", "foo2")
 
-graph1.add_node(
-    "bar",
-    label="Multi\nline\ntext",
-)
-graph1.add_node(
-    "foobar",
-    label="""Multi
+graph1.add_node("abc", font_size="72", height="100")
+
+graph1.add_node("Multi\nline\ntext")
+
+graph1.add_node("foobar").add_label("""Multi
 Line
-Text!""",
-)
+Text!""")
 
 graph1.add_edge(
     "foo",
     "foo1",
-    label="EDGE!",
+    name="EDGE!",
     width="3.0",
     color="#0000FF",
     arrowhead="white_diamond",
     arrowfoot="standard",
     line_type="dotted",
 )
 ```
@@ -225,18 +214,27 @@
 
 # Development
 
 
 Interested in contributing or co-managing further development?  Just reach out!
 
 Dev. Requirements:
+
+Install yEd from [here](https://www.yworks.com/products/yed/download#download).
+
+Ensure you have [MS Excel](https://www.microsoft.com/en/microsoft-365/excel?market=af) installed.
+
 ```console
 $ pip install pytest
 ```
 
+```console
+$ setx CI "True"
+```
+
 To run the tests:
 ```console
 $ PYTHONPATH=. pytest tests
 ```
 
 References:
```

### Comparing `yedextended-1.0.9/examples/demo-basic-create-and-open.py` & `yedextended-2.0.0a0/examples/demo-basic-create-and-open.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import yedextended as yed
 
 # Instantiate graph
 graph1 = yed.Graph()
 
 # Add arbitrary graph detail - nodes and edges
-graph1.add_node("a")
-graph1.add_node("b")
-graph1.add_edge("a", "b")
+a = graph1.add_node("a")
+b = graph1.add_node("b")
+graph1.add_edge(a, b)
 
 # Add arbitrary graph detail - group and group objects
 group1 = graph1.add_group("group 1", shape="rectangle")
-group1.add_node("c")
-group1.add_node("d")
-group1.add_edge("c", "d")
+c = group1.add_node("c")
+d = group1.add_node("d")
+group1.add_edge(c, d)
 
 # subnested group
 group1_1 = group1.add_group("group1_1")
 
 # sub group elements
-group1_1.add_node("e")
-group1_1.add_node("f")
-group1_1.add_edge("e", "f")
+e = group1_1.add_node("e")
+f = group1_1.add_node("f")
+group1_1.add_edge(e, f)
 
 # Complex connections ==============
 # Standalone node to 2-layer-nested node
-graph1.add_edge("a", "e")
+graph1.add_edge(a, e)
 # Standalone node to subnested group
-graph1.add_edge("b", "group1_1")
+graph1.add_edge(b, group1_1)
 
 # Storing a graph to file and opening it
-graph_file = graph1.persist_graph("test.graphml", overwrite=True).open_with_yed()
+graph1.persist_graph("test.graphml", overwrite=True).open_with_yed()
```

### Comparing `yedextended-1.0.9/examples/demo-basic-formatting.py` & `yedextended-2.0.0a0/examples/demo-basic-formatting.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,37 +14,37 @@
     underlined_text="true",
 )
 
 graph1.add_edge("foo1", "foo2")
 
 graph1.add_node("abc", font_size="72", height="100", shape_fill="#FFFFFF")
 
-graph1.add_node("bar", label="Multi\nline\ntext")
+graph1.add_node("bar").add_label("Multi\nline\ntext")
 
 graph1.add_node(
-    "foobar",
-    label="""Multi
+    """Multi
     Line
     Text!""",
 )
 
 graph1.add_edge(
     "foo",
     "foo1",
-    label="EDGE!",
     width="3.0",
     color="#0000FF",
     arrowhead="white_diamond",
     arrowfoot="standard",
     line_type="dotted",
-)
+).add_label("EDGE!")
 
 # Demonstrate stringified graphml version of structure
 print(graph1.stringify_graph())
 
 # Several methods of writing graph to file ==============================
 with open("test_graph.graphml", "w") as fp:  # using standard python functionality
     fp.write(graph1.stringify_graph())
 
 graph1.persist_graph("example.graphml")  # using tool specific method
 
-graph1.persist_graph("pretty_example.graphml", pretty_print=True)  # using tool specific method  with pretty print
+graph1.persist_graph(
+    "pretty_example.graphml", pretty_print=True
+).open_with_yed()  # using tool specific method  with pretty print
```

### Comparing `yedextended-1.0.9/examples/demo-custom-properties-nodes-edges.py` & `yedextended-2.0.0a0/examples/demo-custom-properties-nodes-edges.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,72 +32,75 @@
 graph1.define_custom_property("edge", "Availability", "double", "100.0")
 graph1.define_custom_property("edge", "Toll Free", "boolean", "true")
 graph1.define_custom_property("edge", "Year of build", "string", "")
 
 # Create Groups
 group1 = graph1.add_group("group1", custom_properties={"Country": "Kitchen"})
 
+
 # Create Nodes
-graph1.add_node(
+pasta_city = graph1.add_node(
     "Pasta City",
     custom_properties={
         "Population": "13000",
         "Unemployment": "13.7",
         "Environmental Engagements": "true",
         "Mayor": "Genarro",
     },
 )
-graph1.add_node(
+
+
+wurst_stadt = graph1.add_node(
     "Wurst Stadt",
     custom_properties={"Population": "25100", "Unemployment": "6.2", "Mayor": "Orlowsky"},
 )
-graph1.add_node(
+gruyereville = graph1.add_node(
     "Gruyereville",
     custom_properties={
         "Population": "29650",
         "Unemployment": "11.8",
         "Environmental Engagements": "true",
         "Mayor": "Delage",
     },
 )
 
 # Create Edges
 graph1.add_edge(
-    "Pasta City",
-    "Wurst Stadt",
-    label="N666",
+    pasta_city,
+    wurst_stadt,
+    name="N666",
     arrowhead="none",
     custom_properties={
         "Year of build": "1974",
         "Distance": "356",
         "Toll Free": "false",
         "Availability": "85.7",
     },
 )
 graph1.add_edge(
-    "Pasta City",
-    "Gruyereville",
-    label="E55",
+    pasta_city,
+    gruyereville,
+    name="E55",
     arrowhead="none",
     custom_properties={
         "Year of build": "1986",
         "Distance": "1444",
         "Availability": "96.7",
     },
 )
 graph1.add_edge(
-    "Gruyereville",
-    "Wurst Stadt",
-    label="E23",
+    gruyereville,
+    wurst_stadt,
+    name="E23",
     arrowhead="none",
     custom_properties={"Year of build": "2011", "Distance": "740", "Toll Free": "false"},
 )
 
 # Write Graph
-graph1.persist_graph("demo-custom-properties-nodes-edges.graphml", pretty_print=True)
+graph1.persist_graph("demo-custom-properties-nodes-edges.graphml", pretty_print=True).open_with_yed()
 
 print(40 * "=")
 print("""
 DONE!
 
 Open the file in yEd now.
 Click on the nodes and the edges, press F6 and select the 'data' tab to view the custom properties.
```

### Comparing `yedextended-1.0.9/examples/demo-multilabels.py` & `yedextended-2.0.0a0/examples/demo-multilabels.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,40 +4,48 @@
 
 # Label class is indeed abstract:
 # label = yed.Label("test")
 
 
 graph1.add_node(
     "foo",
-    label="Center",
-    font_family="Zapfino",
     width="200",
     height="200",
     shape_fill="#FFFFFF",
     border_type="dotted",
-).add_label(
-    "Top", model_position="t", font_family="Courier New", font_style="bold"
+).add_label("Center", font_family="Zapfino").add_label(
+    "Top",
+    model_position="t",
+    font_family="Courier New",
+    font_style="bold",
 ).add_label(
     "Left",
     model_name="internal",
     model_position="l",
     font_family="Arial",
     font_style="italic",
     text_color="#FF0000",
 ).add_label(
     "Right",
     model_name="internal",
     model_position="r",
     font_family="Tahoma",
     font_style="bold",
     text_color="#00FF00",
-).add_label("Bottom", model_name="internal", model_position="b", text_color="#0000FF")
+).add_label(
+    "Bottom",
+    model_name="internal",
+    model_position="b",
+    text_color="#0000FF",
+)
 
 
-graph1.add_node("foo2", label="foo2", width="100", height="100").add_label(
+graph1.add_node("foo2", width="100", height="100").add_label(
+    "foo2",
+).add_label(
     "North-West",
     model_name="corners",
     model_position="nw",
     font_family="Courier New",
     font_style="bold",
 ).add_label(
     "North-East",
@@ -52,15 +60,20 @@
     model_position="s",
     font_family="Tahoma",
     font_style="bold",
     text_color="#00FF00",
 ).list_of_labels.pop(0)
 
 
-graph1.add_edge("foo", "foo2", width="3.0", color="#0000FF").add_label(
+graph1.add_edge(
+    "foo",
+    "foo2",
+    width="3.0",
+    color="#0000FF",
+).add_label(
     "Head",
     model_name="two_pos",
     model_position="head",
     font_family="Courier New",
     font_style="bold",
     text_color="#FF00FF",
     background_color="#FFFFFF",
@@ -76,15 +89,20 @@
     model_name="three_center",
     model_position="center",
     font_family="Courier New",
     font_style="bold",
     background_color="#FFFFFF",
 )
 
-graph1.add_edge("foo", "foo2", width="3.0", color="#0000FF").add_label(
+graph1.add_edge(
+    "foo",
+    "foo2",
+    width="3.0",
+    color="#0000FF",
+).add_label(
     "Head",
     model_name="two_pos",
     model_position="head",
     font_family="Courier New",
     font_style="bold",
     text_color="#FF00FF",
     background_color="#FFFFFF",
@@ -100,8 +118,8 @@
     model_name="three_center",
     model_position="center",
     font_family="Courier New",
     font_style="bold",
     background_color="#FFFFFF",
 )
 
-graph1.persist_graph("demo_multilabel.graphml")
+graph1.persist_graph("demo_multilabel.graphml").open_with_yed()
```

### Comparing `yedextended-1.0.9/examples/demo-uml.py` & `yedextended-2.0.0a0/examples/demo-uml.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 # import
 import yedextended as yed
 
 # instantiate graph
 graph1 = yed.Graph()
 
 # Demonstration of some UML objects =========================================
-graph1.add_node(
+car = graph1.add_node(
     "Car",
     shape_fill="#EEEEEE",
     node_type="UMLClassNode",
     UML={
         "attributes": "Model\nManufacturer\nPrice",
         "methods": "getModel()\ngetManufacturer()\ngetPrice()\nsetPrice()",
     },
 )
 
-graph1.add_node(
+icar = graph1.add_node(
     "ICar",
     shape_fill="#EEEEEE",
     node_type="UMLClassNode",
     UML={
         "stereotype": "interface",
         "attributes": "",
         "methods": "getModel()\ngetManufacturer()\ngetPrice()\nsetPrice()",
     },
 )
 
-graph1.add_node("Vehicle", shape_fill="#EEEEEE", node_type="UMLClassNode")
-graph1.add_edge("Car", "Vehicle", arrowhead="white_delta")
-graph1.add_edge("Car", "ICar", arrowhead="white_delta", line_type="dashed")
-
+vehicle = graph1.add_node("Vehicle", shape_fill="#EEEEEE", node_type="UMLClassNode")
+graph1.add_edge(car, vehicle, arrowhead="white_delta")
+graph1.add_edge(car, icar, arrowhead="white_delta", line_type="dashed")
 
 graph1.add_node("This is a note", shape_fill="#EEEEEE", node_type="UMLNoteNode")
 
 # Store Graph
-graph1.persist_graph("demo-uml.graphml")
+graph1.persist_graph("demo-uml.graphml").open_with_yed()
```

### Comparing `yedextended-1.0.9/examples/demo-url-description-groups-nodes-edges.py` & `yedextended-2.0.0a0/examples/demo-url-description-groups-nodes-edges.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,31 +39,31 @@
     url="https://www.comune.savona.it/it/",
 )
 
 # Create Edges
 italy.add_edge(
     "Turin",
     "Brescia",
-    label="E64",
+    name="E64",
     arrowhead="none",
     description="Length	246 km (153 mi)",
     url="https://en.wikipedia.org/wiki/European_route_E64",
 )
 italy.add_edge(
     "Turin",
     "Ivrea",
-    label="E612",
+    name="E612",
     arrowhead="none",
     description="Length	54 km (34 mi)",
     url="https://en.wikipedia.org/wiki/European_route_E612",
 )
 italy.add_edge(
     "Turin",
     "Savona",
-    label="E717",
+    name="E717",
     arrowhead="none",
     description="Length	141 km (88 mi)",
     url="https://en.wikipedia.org/wiki/European_route_E717",
 )
 
 # Write Graph
 graph1.persist_graph("demo-url-description-groups-nodes-edges.graphml", pretty_print=True).open_with_yed()
```

### Comparing `yedextended-1.0.9/examples/readme-3.py` & `yedextended-2.0.0a0/examples/readme-3.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,54 @@
 # import
 import yedextended as yed
 
 # Instantiate graph instance
 graph1 = yed.Graph()
 
 # Add graph nodes and edges with some examples of non-default formatting
-graph1.add_node(
+foo = graph1.add_node(
     "foo",
     font_family="Zapfino",
 )
 
-graph1.add_node(
+foo2 = graph1.add_node(
     "foo2",
     shape="roundrectangle",
     font_style="bolditalic",
     underlined_text="true",
 )
 
 graph1.add_edge(
     "foo1",
-    "foo2",
+    foo2,
 )
+
+
 graph1.add_node(
     "abc",
     font_size="72",
     height="100",
 )
 
-graph1.add_node(
-    "bar",
-    label="Multi\nline\ntext",
+graph1.add_node("bar").add_label(
+    "Multi\nline\ntext",
 )
 graph1.add_node(
     "foobar",
-    label="""Multi
+).add_label(
+    """Multi
 Line
 Text!""",
 )
 
 graph1.add_edge(
-    "foo",
-    "foo1",
-    label="EDGE!",
+    foo,
+    foo2,
+    name="EDGE!",
     width="3.0",
     color="#0000FF",
     arrowhead="white_diamond",
     arrowfoot="standard",
     line_type="dotted",
 )
+
+graph1.persist_graph().open_with_yed()
```

### Comparing `yedextended-1.0.9/examples/test.graphml` & `yedextended-2.0.0a0/examples/test.graphml`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.9/examples/yed_modified_app_created.graphml` & `yedextended-2.0.0a0/examples/yed_modified_app_created.graphml`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.9/images/demo_multilabel.png` & `yedextended-2.0.0a0/images/demo_multilabel.png`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.9/images/example-UML.png` & `yedextended-2.0.0a0/images/example-UML.png`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.9/images/example.png` & `yedextended-2.0.0a0/images/example.png`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.9/images/excel_obj_entry.gif` & `yedextended-2.0.0a0/images/excel_obj_entry.gif`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.9/images/excel_rel_entry.gif` & `yedextended-2.0.0a0/images/excel_rel_entry.gif`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.9/images/graph.gif` & `yedextended-2.0.0a0/images/graph.gif`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.9/images/graph_from_excel_obj.gif` & `yedextended-2.0.0a0/images/graph_from_excel_obj.gif`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.9/images/graph_from_excel_rel.gif` & `yedextended-2.0.0a0/images/graph_from_excel_rel.gif`

 * *Files identical despite different names*

### Comparing `yedextended-1.0.9/pyproject.toml` & `yedextended-2.0.0a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "yedextended"
 dynamic = ["version"]
 authors = [{ name = "Cole St John", email = "info@colestjohn.com" }]
 description = "Python library extending yEd functionality through programmatic interface to graphs."
 readme = "README.md"
 requires-python = ">=3.10"
-dependencies = ["psutil", "pygetwindow", "openpyxl"]
+dependencies = ["psutil", "openpyxl"]
 classifiers = [
 	"Programming Language :: Python :: 3 :: Only",
 	"Programming Language :: Python :: 3.10",
 	"Programming Language :: Python :: 3.11",
 	"Programming Language :: Python :: 3.12",
 	"License :: OSI Approved :: BSD License",
 	"Operating System :: OS Independent",
```

### Comparing `yedextended-1.0.9/src/yedextended/__init__.py` & `yedextended-2.0.0a0/src/yedextended/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,32 +4,45 @@
 * Building of yEd graph objects from scratch
 * Reading of yEd graph files
 * Management of yEd graph data in Excel (for simplified addition / management of data)
 * Opening and basic control of yEd application
 
 """
 
+from __future__ import annotations
+
+# import asyncio
+import io
 import os
 import platform
 import re
 import subprocess
 import sys
 import xml.etree.ElementTree as ET
+from random import randint
 from shutil import which
+from time import sleep
 from tkinter import messagebox as msg
-from typing import Any, List, Optional
+from typing import Any, Dict, List, Optional, Union
+from warnings import warn
 from xml.dom import minidom
 
 import openpyxl as pyxl
 import psutil
-import pygetwindow as gw
+
+# import pygetwindow as gw # potential future addition for window management
 
 # Enumerated parameters / Constants
 PROGRAM_NAME = "yEd.exe"
 
+# Testing related triggers
+testing = False
+local_testing = None
+show_guis = True
+
 LINE_TYPES = [
     "line",
     "dashed",
     "dotted",
     "dashed_dotted",
 ]
 
@@ -77,46 +90,52 @@
 
     if validValues:
         if value not in validValues:
             raise ValueError(f"{parameter_name} '{value}' is not supported. Use: '{', '.join(validValues)}'")
 
 
 class File:
-    """Object to pass around, check and act on yEd files / filepaths."""
+    """Object to check and act on yEd files / filepaths (or excel files, .xlsx,  during bulk data management)."""
 
     def __init__(self, file_name_or_path=None):
         self.DEFAULT_FILE_NAME = "temp"
         self.EXTENSION = ".graphml"
         self.dir = self.path_validate(file_name_or_path)
         self.basename = self.base_name_validate(file_name_or_path)
         self.fullpath = os.path.join(self.dir, self.basename)
         self.window_search_name = self.basename + " - yEd"
         self.file_exists = os.path.isfile(self.fullpath)
 
+    def full_path_validate(self):
+        self.file_exists = os.path.isfile(self.fullpath)
+
     def path_validate(self, temp_name_or_path=None):
         """Validate if the file was initialized with valid path - returning the same path - if not valid, return working directory as default path."""
-        path = ""
+        path = os.getcwd()
         if temp_name_or_path:
             path = os.path.dirname(temp_name_or_path)
-        return path or os.getcwd()
+            if not os.path.exists(path):
+                path = os.getcwd()
+        return os.path.realpath(path)
 
     def base_name_validate(self, temp_name_or_path=None):
-        """Validate / Build valid file name with GraphML extension"""
+        """Validate / Build valid file name with GraphML extension (also works with excel files identified with xlsx)"""
         temp_name = ""
         if temp_name_or_path:
             temp_name = os.path.basename(temp_name_or_path)
         temp_name = temp_name or f"{self.DEFAULT_FILE_NAME}"
-        if not temp_name.endswith(self.EXTENSION):
+        if not temp_name.endswith(self.EXTENSION) and not temp_name.endswith(".xlsx"):
             temp_name += self.EXTENSION
         return temp_name
 
     def open_with_yed(self, force=False):
         """Method to open GraphML file directly with yEd application (must be installed and on path)."""
-        print("opening...")
+        print("opening file with yed...")
         open_yed_file(self, force)
+        return get_yed_pid()
 
 
 class Label:
     """Generic Label Class for nodes / edges in yEd"""
 
     graphML_tagName = None
 
@@ -326,306 +345,29 @@
         """
         self.scope = scope
         self.name = name
         self.property_type = property_type
         self.default_value = default_value
         self.id = "%s_%s" % (self.scope, self.name)
 
-    def convert_to_xml(self):
+    def convert_to_xml(self) -> ET.Element:
         custom_prop_key = ET.Element("key", id=self.id)
         custom_prop_key.set("for", self.scope)
         custom_prop_key.set("attr.name", self.name)
         custom_prop_key.set("attr.type", self.property_type)
 
         return custom_prop_key
 
 
-class Group:
-    """yEd Group Object (Visual Container of Nodes / Edges / also can recursively act as Node)"""
-
-    VALID_SHAPES = [
-        "rectangle",
-        "rectangle3d",
-        "roundrectangle",
-        "diamond",
-        "ellipse",
-        "fatarrow",
-        "fatarrow2",
-        "hexagon",
-        "octagon",
-        "parallelogram",
-        "parallelogram2",
-        "star5",
-        "star6",
-        "star6",
-        "star8",
-        "trapezoid",
-        "trapezoid2",
-        "triangle",
-        "trapezoid2",
-        "triangle",
-    ]
-
-    def __init__(
-        self,
-        group_id,
-        parent_graph,
-        label=None,
-        label_alignment="center",
-        shape="rectangle",
-        closed="false",
-        font_family="Dialog",
-        underlined_text="false",
-        font_style="plain",
-        font_size="12",
-        fill="#FFCC00",
-        transparent="false",
-        border_color="#000000",
-        border_type="line",
-        border_width="1.0",
-        height=False,
-        width=False,
-        x=False,
-        y=False,
-        custom_properties=None,
-        description="",
-        url="",
-    ):
-        self.label = label
-        if label is None:
-            self.label = group_id
-
-        self.parent = None
-        self.group_id = group_id
-        self.nodes = {}
-        self.groups = {}
-        self.parent_graph = parent_graph
-        self.edges = {}
-        self.num_edges = 0
-
-        # node shape
-        checkValue("shape", shape, Group.VALID_SHAPES)
-        self.shape = shape
-
-        self.closed = closed
-
-        # label formatting options
-        self.font_family = font_family
-        self.underlined_text = underlined_text
-
-        checkValue("font_style", font_style, FONT_STYLES)
-        self.font_style = font_style
-        self.font_size = font_size
-
-        checkValue("label_alignment", label_alignment, HORIZONTAL_ALIGNMENTS)
-        self.label_alignment = label_alignment
-
-        self.fill = fill
-        self.transparent = transparent
-
-        self.geom = {}
-        if height:
-            self.geom["height"] = height
-        if width:
-            self.geom["width"] = width
-        if x:
-            self.geom["x"] = x
-        if y:
-            self.geom["y"] = y
-
-        self.border_color = border_color
-        self.border_width = border_width
-
-        checkValue("border_type", border_type, LINE_TYPES)
-        self.border_type = border_type
-
-        self.description = description
-        self.url = url
-
-        # Handle Node Custom Properties
-        for name, definition in Node.custom_properties_defs.items():
-            if custom_properties:
-                for k, v in custom_properties.items():
-                    if k not in Node.custom_properties_defs:
-                        raise RuntimeWarning("key %s not recognised" % k)
-                    if name == k:
-                        setattr(self, name, custom_properties[k])
-                        break
-                else:
-                    setattr(self, name, definition.default_value)
-            else:
-                setattr(self, name, definition.default_value)
-
-    def add_node(self, node_name, **kwargs):
-        """Adding node within Group"""
-        if node_name in self.parent_graph.existing_entities:
-            raise RuntimeWarning("Node %s already exists" % node_name)
-
-        node = Node(node_name, **kwargs)
-        node.parent = self
-        self.nodes[node_name] = node
-        self.parent_graph.existing_entities[node_name] = node
-        return node
-
-    def add_group(self, group_id, **kwargs):
-        """Adding a group within current group object (and same parent graph)."""
-        if group_id in self.parent_graph.existing_entities:
-            raise RuntimeWarning("Group %s already exists" % group_id)
-
-        group = Group(group_id, self.parent_graph, **kwargs)
-        group.parent = self
-        self.groups[group_id] = group
-        self.parent_graph.existing_entities[group_id] = group
-        return group
-
-    def add_edge(self, node1_id, node2_id, **kwargs):
-        """Adds edge - input: node names, not actual node objects"""
-        # TODO: DO EDGES NEED A PARENT FOR EASE OF OPERATIONS
-
-        node1 = self.parent_graph.existing_entities.get(node1_id) or self.add_node(node1_id)
-
-        node2 = self.parent_graph.existing_entities.get(node2_id) or self.add_node(node2_id)
-
-        # http://graphml.graphdrawing.org/primer/graphml-primer.html#Nested
-        # The edges between two nodes in a nested graph have to be declared in a graph,
-        # which is an ancestor of both nodes in the hierarchy.
-
-        if not (self.is_ancestor(node1) and self.is_ancestor(node2)):
-            raise RuntimeWarning("Group %s is not ancestor of both %s and %s" % (self.group_id, node1_id, node2_id))
-
-        self.parent_graph.num_edges += 1
-        kwargs["edge_id"] = str(self.parent_graph.num_edges)
-        edge = Edge(node1_id, node2_id, **kwargs)
-        edge.parent = self
-        self.edges[edge.edge_id] = edge
-        return edge
-
-    def remove_node(self, node_name) -> None:
-        """Remove/Delete a node from a group"""
-        if node_name not in self.nodes:
-            raise RuntimeWarning("Node %s doesn't exist" % node_name)
-        del self.nodes[node_name]
-        del self.parent_graph.existing_entities[node_name]
-
-    def remove_group(self, group_id) -> None:
-        """Removes a group from within current group object (and same parent graph)."""
-        if group_id not in self.groups:
-            raise RuntimeWarning("Group %s doesn't exist" % group_id)
-        group = self.groups[group_id]
-
-        # reroute dependents
-        for node in group.nodes.values():
-            node.parent = self  # reassign parent: node side
-            self.nodes[node.node_name] = node  # reassign parent: group side
-
-        for edge in group.edges.values():
-            edge.parent = self  # reassign parent: edge side
-            self.edges[edge.edge_id] = edge  # reassign parent: group side
-
-        for group in group.groups.values():
-            # edge.parent = self  #reassign parent: edge side
-            group.parent = self
-            self.groups[group.group_id] = group  # reassign parent: group side
-
-        # remove records
-        del self.groups[group_id]
-        del self.parent_graph.existing_entities[group_id]
-
-    def remove_edge(self, edge_id):
-        """Removing edge from group  - uses node names not node objects."""
-        if not self.edges[edge_id]:
-            raise RuntimeWarning("Edge %s does not exist under group %s" % (edge_id, self.group_id))
-
-        del self.edges[edge_id]
-        # self.num_edges -= 1
-        self.parent_graph.num_edges -= 1
-
-    def is_ancestor(self, node):
-        """Check for possible nesting conflict of this id usage"""
-        return node.parent is not None and (node.parent is self or self.is_ancestor(node.parent))
-
-    def convert_to_xml(self):
-        """Converting graph object to graphml xml object"""
-
-        node = ET.Element("node", id=self.group_id)
-        node.set("yfiles.foldertype", "group")
-        data = ET.SubElement(node, "data", key="data_node")
-
-        # node for group
-        pabn = ET.SubElement(data, "y:ProxyAutoBoundsNode")
-        r = ET.SubElement(pabn, "y:Realizers", active="0")
-        group_node = ET.SubElement(r, "y:GroupNode")
-
-        if self.geom:
-            ET.SubElement(group_node, "y:Geometry", **self.geom)
-
-        ET.SubElement(group_node, "y:Fill", color=self.fill, transparent=self.transparent)
-
-        ET.SubElement(
-            group_node,
-            "y:BorderStyle",
-            color=self.border_color,
-            type=self.border_type,
-            width=self.border_width,
-        )
-
-        label = ET.SubElement(
-            group_node,
-            "y:NodeLabel",
-            modelName="internal",
-            modelPosition="t",
-            fontFamily=self.font_family,
-            fontSize=self.font_size,
-            underlinedText=self.underlined_text,
-            fontStyle=self.font_style,
-            alignment=self.label_alignment,
-        )
-        label.text = self.label
-
-        ET.SubElement(group_node, "y:Shape", type=self.shape)
-
-        ET.SubElement(group_node, "y:State", closed=self.closed)
-
-        graph = ET.SubElement(node, "graph", edgedefault="directed", id=self.group_id)
-
-        if self.url:
-            url_node = ET.SubElement(node, "data", key="url_node")
-            url_node.text = self.url
-
-        if self.description:
-            description_node = ET.SubElement(node, "data", key="description_node")
-            description_node.text = self.description
-
-        for node_id in self.nodes:
-            n = self.nodes[node_id].convert_to_xml()
-            graph.append(n)
-
-        for group_id in self.groups:
-            n = self.groups[group_id].convert_to_xml()
-            graph.append(n)
-
-        for edge_id in self.edges:
-            e = self.edges[edge_id].convert_to_xml()
-            graph.append(e)
-
-        # Node Custom Properties
-        for name, definition in Node.custom_properties_defs.items():
-            node_custom_prop = ET.SubElement(node, "data", key=definition.id)
-            node_custom_prop.text = getattr(self, name)
-
-        return node
-        # ProxyAutoBoundsNode crap just draws bar at top of group
-
-
 class Node:
-    """yEd Node object"""
+    """yEd Node object - representing a single node in the graph"""
 
     custom_properties_defs = {}
 
-    VALID_SHAPES = [
+    VALID_NODE_SHAPES = [
         "rectangle",
         "rectangle3d",
         "roundrectangle",
         "diamond",
         "ellipse",
         "fatarrow",
         "fatarrow2",
@@ -642,16 +384,15 @@
         "triangle",
         "trapezoid2",
         "triangle",
     ]
 
     def __init__(
         self,
-        node_name,
-        label=None,
+        name: str = "",  # non-unique node name
         label_alignment="center",
         shape="rectangle",
         font_family="Dialog",
         underlined_text="false",
         font_style="plain",
         font_size="12",
         shape_fill="#FFCC00",
@@ -660,48 +401,39 @@
         border_type="line",
         border_width="1.0",
         height=False,
         width=False,
         x=False,
         y=False,
         node_type="ShapeNode",
-        UML=False,
+        UML: Union[bool, dict] = False,
         custom_properties=None,
         description="",
         url="",
     ):
-        self.list_of_labels = []  # initialize list of labels
-        if label:
-            self.add_label(
-                label,
-                alignment=label_alignment,
-                font_family=font_family,
-                underlined_text=underlined_text,
-                font_style=font_style,
-                font_size=font_size,
-            )
-        else:
-            self.add_label(
-                node_name,
-                alignment=label_alignment,
-                font_family=font_family,
-                underlined_text=underlined_text,
-                font_style=font_style,
-                font_size=font_size,
-            )
-
-        self.node_name = node_name
+        self.name: str = name
+        self.id: str = generate_temp_uuid()  # temporary unique
+        self.parent: Union[(Group, Graph, None)] = None
+
+        self.list_of_labels: list[NodeLabel] = []  # initialize list of labels
+
+        self.add_label(
+            label_text=name,
+            alignment=label_alignment,
+            font_family=font_family,
+            underlined_text=underlined_text,
+            font_style=font_style,
+            font_size=font_size,
+        )
 
         self.node_type = node_type
         self.UML = UML
 
-        self.parent = None
-
         # node shape
-        checkValue("shape", shape, Node.VALID_SHAPES)
+        checkValue("shape", shape, Node.VALID_NODE_SHAPES)
         self.shape = shape
 
         # shape fill
         self.shape_fill = shape_fill
         self.transparent = transparent
 
         # border options
@@ -735,24 +467,24 @@
                         setattr(self, name, custom_properties[k])
                         break
                 else:
                     setattr(self, name, definition.default_value)
             else:
                 setattr(self, name, definition.default_value)
 
-    def add_label(self, label_text, **kwargs):
-        """Adding node label"""
+    def add_label(self, label_text, **kwargs) -> Node:
+        """Adds node label - > returns node for continued node operations"""
         self.list_of_labels.append(NodeLabel(label_text, **kwargs))
         return self
 
-    def convert_to_xml(self):
+    def convert_to_xml(self) -> ET.Element:
         """Converting node object to xml object"""
 
-        node = ET.Element("node", id=str(self.node_name))
-        data = ET.SubElement(node, "data", key="data_node")
+        xml_node = ET.Element("node", id=str(self.id))
+        data = ET.SubElement(xml_node, "data", key="data_node")
         shape = ET.SubElement(data, "y:" + self.node_type)
 
         if self.geom:
             ET.SubElement(shape, "y:Geometry", **self.geom)
         # <y:Geometry height="30.0" width="30.0" x="475.0" y="727.0"/>
 
         ET.SubElement(shape, "y:Fill", color=self.shape_fill, transparent=self.transparent)
@@ -766,43 +498,45 @@
         )
 
         for label in self.list_of_labels:
             label.addSubElement(shape)
 
         ET.SubElement(shape, "y:Shape", type=self.shape)
 
+        # UML specific
         if self.UML:
             UML = ET.SubElement(shape, "y:UML")
 
             attributes = ET.SubElement(UML, "y:AttributeLabel", type=self.shape)
             attributes.text = self.UML["attributes"]
 
             methods = ET.SubElement(UML, "y:MethodLabel", type=self.shape)
             methods.text = self.UML["methods"]
 
             stereotype = self.UML["stereotype"] if "stereotype" in self.UML else ""
             UML.set("stereotype", stereotype)
 
+        # Special items
         if self.url:
-            url_node = ET.SubElement(node, "data", key="url_node")
+            url_node = ET.SubElement(xml_node, "data", key="url_node")
             url_node.text = self.url
 
         if self.description:
-            description_node = ET.SubElement(node, "data", key="description_node")
+            description_node = ET.SubElement(xml_node, "data", key="description_node")
             description_node.text = self.description
 
         # Node Custom Properties
         for name, definition in Node.custom_properties_defs.items():
-            node_custom_prop = ET.SubElement(node, "data", key=definition.id)
+            node_custom_prop = ET.SubElement(xml_node, "data", key=definition.id)
             node_custom_prop.text = getattr(self, name)
 
-        return node
+        return xml_node
 
     @classmethod
-    def set_custom_properties_defs(cls, custom_property):
+    def set_custom_properties_defs(cls, custom_property) -> None:
         cls.custom_properties_defs[custom_property.name] = custom_property
 
 
 class Edge:
     """yEd Edge - connecting Nodes or Groups"""
 
     custom_properties_defs = {}
@@ -828,61 +562,61 @@
         "crows_foot_one",
         "crows_foot_many",
         "crows_foot_optional",
     ]
 
     def __init__(
         self,
-        node1,
-        node2,
-        label=None,
+        node1: Node,
+        node2: Node,
+        name: str = "",
         arrowhead="standard",
         arrowfoot="none",
         color="#000000",
         line_type="line",
         width="1.0",
-        edge_id="",
         label_background_color="",
         label_border_color="",
         source_label=None,
         target_label=None,
         custom_properties=None,
         description="",
         url="",
     ):
-        self.node1 = node1
-        self.node2 = node2
-
-        self.list_of_labels = []  # initialize list of labels
+        # Primary operations
+        self.node1: Node = node1
+        self.node2: Node = node2
+        self.name: str = name
+        self.list_of_labels: list[EdgeLabel] = []  # initialize list of labels
+        self.id: str = generate_temp_uuid()  # give temp id
+        self.parent: Union[(Group, Graph, None)] = None
 
-        if label:
+        if name:
             self.add_label(
-                label,
+                name,
                 border_color=label_border_color,
                 background_color=label_background_color,
             )
 
-        if not edge_id:
-            edge_id = "%s_%s" % (node1, node2)
-
-        self.edge_id = str(edge_id)
+        # if not node1 or not node2:
+        #     id = "%s_%s" % (node1, node2)
 
         if source_label is not None:
             self.add_label(
                 source_label,
                 model_name="six_pos",
                 model_position="shead",
                 preferred_placement="source_on_edge",
                 border_color=label_border_color,
                 background_color=label_background_color,
             )
 
         if target_label is not None:
             self.add_label(
-                source_label,
+                target_label,
                 model_name="six_pos",
                 model_position="shead",
                 preferred_placement="source_on_edge",
                 border_color=label_border_color,
                 background_color=label_background_color,
             )
 
@@ -897,16 +631,14 @@
 
         self.color = color
         self.width = width
 
         self.description = description
         self.url = url
 
-        self.parent = None
-
         # Handle Edge Custom Properties
         for name, definition in Edge.custom_properties_defs.items():
             if custom_properties:
                 for k, v in custom_properties.items():
                     if k not in Edge.custom_properties_defs:
                         raise RuntimeWarning("key %s not recognised" % k)
                     if name == k:
@@ -919,18 +651,18 @@
 
     def add_label(self, label_text, **kwargs):
         """Adding edge label"""
         self.list_of_labels.append(EdgeLabel(label_text, **kwargs))
         # Enable method chaining
         return self
 
-    def convert_to_xml(self):
+    def convert_to_xml(self) -> ET.Element:
         """Converting edge object to xml object"""
 
-        edge = ET.Element("edge", id=str(self.edge_id), source=str(self.node1), target=str(self.node2))
+        edge = ET.Element("edge", id=str(self.id), source=str(self.node1.id), target=str(self.node2.id))
 
         data = ET.SubElement(edge, "data", key="data_edge")
         pl = ET.SubElement(data, "y:PolyLineEdge")
 
         ET.SubElement(pl, "y:Arrows", source=self.arrowfoot, target=self.arrowhead)
         ET.SubElement(pl, "y:LineStyle", color=self.color, type=self.line_type, width=self.width)
 
@@ -949,102 +681,901 @@
         for name, definition in Edge.custom_properties_defs.items():
             edge_custom_prop = ET.SubElement(edge, "data", key=definition.id)
             edge_custom_prop.text = getattr(self, name)
 
         return edge
 
     @classmethod
-    def set_custom_properties_defs(cls, custom_property):
+    def set_custom_properties_defs(cls, custom_property) -> None:
         cls.custom_properties_defs[custom_property.name] = custom_property
 
 
+class Group:
+    """yEd Group Object (Visual Container of Nodes / Edges / also can recursively act as Node)"""
+
+    VALID_SHAPES = [
+        "rectangle",
+        "rectangle3d",
+        "roundrectangle",
+        "diamond",
+        "ellipse",
+        "fatarrow",
+        "fatarrow2",
+        "hexagon",
+        "octagon",
+        "parallelogram",
+        "parallelogram2",
+        "star5",
+        "star6",
+        "star6",
+        "star8",
+        "trapezoid",
+        "trapezoid2",
+        "triangle",
+        "trapezoid2",
+        "triangle",
+    ]
+
+    def __init__(
+        self,
+        name: str = "",
+        top_level_graph=None,
+        label_alignment="center",
+        shape="rectangle",
+        closed="false",
+        font_family="Dialog",
+        underlined_text="false",
+        font_style="plain",
+        font_size="12",
+        fill="#FFCC00",
+        transparent="false",
+        border_color="#000000",
+        border_type="line",
+        border_width="1.0",
+        height=False,
+        width=False,
+        x=False,
+        y=False,
+        custom_properties=None,
+        description="",
+        url="",
+    ):
+        self.name = name
+        self.parent: Union[(Group, Graph, None)] = None  # set during add_group
+        self.id = generate_temp_uuid()
+
+        self.nodes: dict[str, Node] = {}
+        self.groups: dict[str, Group] = {}
+        self.edges: dict[str, Edge] = {}
+        self.combined_objects = {}
+
+        self.top_level_graph = top_level_graph
+
+        # node shape
+        checkValue("shape", shape, Group.VALID_SHAPES)
+        self.shape = shape
+
+        self.closed = closed
+
+        # label formatting options
+        self.font_family = font_family
+        self.underlined_text = underlined_text
+
+        checkValue("font_style", font_style, FONT_STYLES)
+        self.font_style = font_style
+        self.font_size = font_size
+
+        checkValue("label_alignment", label_alignment, HORIZONTAL_ALIGNMENTS)
+        self.label_alignment = label_alignment
+
+        self.fill = fill
+        self.transparent = transparent
+
+        self.geom = {}
+        if height:
+            self.geom["height"] = height
+        if width:
+            self.geom["width"] = width
+        if x:
+            self.geom["x"] = x
+        if y:
+            self.geom["y"] = y
+
+        self.border_color = border_color
+        self.border_width = border_width
+
+        checkValue("border_type", border_type, LINE_TYPES)
+        self.border_type = border_type
+
+        self.description = description
+        self.url = url
+
+        # Handle Node Custom Properties
+        for name, definition in Node.custom_properties_defs.items():
+            if custom_properties:
+                for k, v in custom_properties.items():
+                    if k not in Node.custom_properties_defs:
+                        raise RuntimeWarning("key %s not recognised" % k)
+                    if name == k:
+                        setattr(self, name, custom_properties[k])
+                        break
+                else:
+                    setattr(self, name, definition.default_value)
+            else:
+                setattr(self, name, definition.default_value)
+
+    def add_node(self, node: Union[Node, str, None] = None, **kwargs) -> Node:
+        """Adding node within Group - accepts node object (simply assigns), or node name or none (to create new node without name)."""
+        return add_node(self, node, **kwargs)
+
+    def add_group(self, group: Union[Group, str, None] = None, **kwargs) -> Group:
+        """Adding group to Group - accepts group object (simply assigns), or group name or none (to create new group without name)"""
+        return add_group(self, group, **kwargs)
+
+    def add_edge(
+        self,  # owner
+        node1: Optional[Union[(Node, Group, str)]] = None,
+        node2: Optional[Union[(Node, Group, str)]] = None,
+        **kwargs,
+    ) -> Edge:
+        """Adding edge to Group - for node1/node2 uses node / group objects or accepts names (creating new nodes under self) - or function can alternatively accept an instantiated Edge object."""
+
+        # map args into kwargs in case of excel data management ops
+        if node1:
+            kwargs["node1"] = node1
+        if node2:
+            kwargs["node2"] = node2
+
+        return add_edge(self, **kwargs)
+
+    # Removal of items ==============================
+    def remove_node(self, node: Union[Node, str]) -> None:
+        """Remove/Delete a node from group - by object or id."""
+        remove_node(self, node)
+
+    def remove_group(self, group: Union[Group, str], **kwargs) -> None:
+        """Removes a group from within current group object (and same parent graph) - by object or id."""
+        remove_group(self, group, **kwargs)
+
+    def remove_edge(self, edge: Union[Edge, str]) -> None:
+        """Removing edge from group - by object or id."""
+        remove_edge(self, edge)
+
+    def is_ancestor(self, node) -> bool:
+        """Check for possible nesting conflict of this id usage"""
+        return node.parent is not None and (node.parent is self or self.is_ancestor(node.parent))
+
+    def convert_to_xml(self) -> ET.Element:
+        """Converting graph object to graphml xml object"""
+
+        node = ET.Element("node", id=self.id)
+        node.set("yfiles.foldertype", "group")
+        data = ET.SubElement(node, "data", key="data_node")
+
+        # node for group
+        pabn = ET.SubElement(data, "y:ProxyAutoBoundsNode")
+        r = ET.SubElement(pabn, "y:Realizers", active="0")
+        group_node = ET.SubElement(r, "y:GroupNode")
+
+        if self.geom:
+            ET.SubElement(group_node, "y:Geometry", **self.geom)
+
+        ET.SubElement(group_node, "y:Fill", color=self.fill, transparent=self.transparent)
+
+        ET.SubElement(
+            group_node,
+            "y:BorderStyle",
+            color=self.border_color,
+            type=self.border_type,
+            width=self.border_width,
+        )
+
+        label = ET.SubElement(
+            group_node,
+            "y:NodeLabel",
+            modelName="internal",
+            modelPosition="t",
+            fontFamily=self.font_family,
+            fontSize=self.font_size,
+            underlinedText=self.underlined_text,
+            fontStyle=self.font_style,
+            alignment=self.label_alignment,
+        )
+        label.text = self.name
+
+        ET.SubElement(group_node, "y:Shape", type=self.shape)
+
+        ET.SubElement(group_node, "y:State", closed=self.closed)
+
+        graph = ET.SubElement(node, "graph", edgedefault="directed", id=self.id)
+
+        if self.url:
+            url_node = ET.SubElement(node, "data", key="url_node")
+            url_node.text = self.url
+
+        if self.description:
+            description_node = ET.SubElement(node, "data", key="description_node")
+            description_node.text = self.description
+
+        # Add group contained items (recursive)
+        for id in self.nodes:
+            n = self.nodes[id].convert_to_xml()
+            graph.append(n)
+
+        for id in self.groups:
+            n = self.groups[id].convert_to_xml()
+            graph.append(n)
+
+        for id in self.edges:
+            e = self.edges[id].convert_to_xml()
+            graph.append(e)
+
+        # Node Custom Properties
+        for name, definition in Node.custom_properties_defs.items():
+            node_custom_prop = ET.SubElement(node, "data", key=definition.id)
+            node_custom_prop.text = getattr(self, name)
+
+        return node
+        # ProxyAutoBoundsNode crap just draws bar at top of group
+
+
 class GraphStats:
     """Object to query and carry complete structure of current (recursive) graph objects and relationships."""
 
-    def __init__(self, graph_or_input_node):
-        self.all_nodes = dict()
-        self.all_groups = dict()
-        self.all_edges = dict()
-        self.recursive_id_extract(graph_or_input_node)
+    def __init__(self, graph: Graph):
+        self.graph = graph
+        self.gather_metadata()  # initial extraction
 
-    def recursive_id_extract(self, graph_or_input_node):
+    def recursive_id_extract(self, graph_or_input_node) -> None:
         """Gather complete structure of current (recursive) graph objects and relationships."""
         sub_nodes = graph_or_input_node.nodes.values()
         sub_groups = graph_or_input_node.groups.values()
         sub_edges = graph_or_input_node.edges.values()
 
         for node in sub_nodes:
-            id = node.node_name
-            if id:
-                self.all_nodes[id] = node
+            self.all_nodes[node.id] = node
+
+        for edge in sub_edges:
+            self.all_edges[edge.id] = edge
 
         for group in sub_groups:
-            id = group.group_id
-            if id:
-                self.all_groups[id] = group
+            self.all_groups[group.id] = group
             self.recursive_id_extract(group)
 
-        for edge in sub_edges:
-            id = edge.edge_id
-            if id:
-                self.all_edges[id] = edge
+    def gather_metadata(self):
+        """Gather metadata for all objects in the graph."""
+
+        # Establish / clear data structures
+        self.all_nodes: dict[str, Node] = {}
+        self.all_groups: dict[str, Group] = {}
+        self.all_objects: dict[str, Union[Node, Group]] = {}
+        self.all_edges: dict[str, Edge] = {}
+        self.all_graph_items: dict[str, Union[Node, Group, Edge]] = {}
+        self.id_to_name: dict[str, str] = {}
+        self.name_to_ids: dict[str, list[str]] = {}
+        self.duplicate_names: set[str] = set()
+
+        # (re)extract core graph data
+        self.recursive_id_extract(self.graph)
+
+        # Combine remaining data ========================
+        self.all_objects = {**self.all_nodes, **self.all_groups}
+        self.all_graph_items = {**self.all_objects, **self.all_edges}
+        for obj in self.all_graph_items.values():
+            self.id_to_name[obj.id] = obj.name
+            current_ids = self.name_to_ids.get(obj.name, [])
+            if current_ids:
+                self.duplicate_names.add(obj.name)
+            current_ids.append(obj.id)
+            self.name_to_ids[obj.name] = current_ids
+
+    def find_by_id(self, id) -> Union[Node, Group, Edge, None]:
+        """Find object by unique yEd id."""
+        return self.all_graph_items.get(id, None)
+
+    def find_by_name(self, name) -> List[Union[Node, Group, Edge]]:
+        """Find object by user assigned name - needs to provide for multiple (needs deduplication)."""
+        return [self.all_graph_items[id] for id in self.name_to_ids.get(name, [])]
+
+    def name_reused(self, name: str) -> bool:
+        """Find object by user assigned name - needs to provide for multiple (needs deduplication)."""
+        return name in self.duplicate_names
+
+
+class ExcelManager:
+    """Object to handle interfacing of graphs with Excel in bulk data management operations."""
+
+    def __init__(self):
+        # Template operations ==============
+        self.WB_TYPES = ["obj_and_hierarchy", "object_data", "relations"]
+        self.TEMP_EXCEL_SHEET = File("yedextended_temp.xlsx").fullpath
+        self.OBJECTS_WS_NAME = "Objects_and_Groups"
+        self.RELATIONS_WS_NAME = "Relations"
+        self.DISAMBIGUATING_SEPARATOR = "##ID:##"
+
+        # Graph operations ================
+        self.graph = Graph()
+        self.original_stats: GraphStats
+        # self.original_id_to_label: dict[str, str] = dict()
+        # self.original_id_to_obj: dict[str, Union[(Group, Edge, Node)]] = dict()
+        # self.obj_keys = list()
+        # self.obj_values = list()
+        # self.dup_objects = list()
+
+    def kill_excel(self) -> None:
+        """Providing a utility to help primarily during test"""
+        os.system('taskkill /f /im "excel.exe"')  # FIXME: Windows only
+
+    def bulk_data_op_verify(self, type) -> None:
+        """Check if the given bulk data management type is valid for Excel operations."""
+        self.type = type or self.WB_TYPES[0]  # default
+        if self.type not in self.WB_TYPES:
+            raise RuntimeWarning("Invalid Excel type. Use: %s" % ", ".join(self.WB_TYPES))
+
+    def create_excel_template(self, type) -> None:
+        """Generate excel wb per template for that wb type."""
+
+        self.bulk_data_op_verify(type)
+
+        if os.path.isfile(self.TEMP_EXCEL_SHEET):
+            os.remove(self.TEMP_EXCEL_SHEET)
+
+        # create workbook
+        excel_wb = pyxl.Workbook()
+
+        # Inserting /organizing sheets
+        excel_ws = excel_wb.active
+
+        # Create object ws
+        objects_ws = excel_wb.create_sheet(self.OBJECTS_WS_NAME, 0)
+
+        # Add header to sheet
+        objects_ws.cell(
+            row=1,
+            column=1,
+            value="FORMAT -> OBJECT_LABEL | OBJECT_ID (OPTIONAL TO SUPPORT DISAMBIGUATION) - NOTE: INDENTATION OF INFO ONE COLUMN DESIGNATES BELONGING TO OBJECT ABOVE.",
+        )
+
+        # Add relations sheet and header
+        if self.type == "relations":
+            relations_ws = excel_wb.create_sheet(self.RELATIONS_WS_NAME, 1)
+            relations_ws.cell(
+                row=1,
+                column=1,
+                value="FORMAT -> NODE1_LABEL | NODE2_LABEL | EDGE_LABEL (OPTIONAL) | EDGE_OWNER (OPTIONAL - TO ASSIGN OWNERSHIP TO SPECIFIC GROUP) - NOTE: DISAMBIGUATION SUPPORTED BY CONCATENATING LABEL WITH '##ID:##'+ID SHARED WITH OBJECT",
+            )
+
+        # Clean up
+        if excel_ws:
+            excel_wb.remove(excel_ws)  # removing default sheet
+        self.kill_excel()
+        excel_wb.save(self.TEMP_EXCEL_SHEET)
+        excel_wb.close()
+
+    def open_close_excel(*args, **kwargs):
+        """Provide wrapper for opening / saving / closing excel ops."""
+        save = kwargs.get("save", False)
+
+        def decorator(func):
+            def wrapper_func(self, *args, **kwargs):
+                in_mem_file = None
+                excel_data = kwargs.get("excel_data", None)
+                type = kwargs.get("type", None)
+                self.bulk_data_op_verify(type)
+
+                # Graph to excel
+                if save:
+                    self.create_excel_template(type)
+                    sleep(0.5)  # FIXME: Unclear if necessary
+                    with open(self.TEMP_EXCEL_SHEET, "rb") as f:
+                        in_mem_file = io.BytesIO(f.read())
+
+                # Excel to graph
+                else:
+                    # In case we are given a file path or in-memory file, for excel to graph
+                    if excel_data:
+                        if isinstance(excel_data, io.BytesIO):
+                            in_mem_file = excel_data
+                        elif isinstance(excel_data, str):
+                            with open(excel_data, "rb") as f:
+                                in_mem_file = io.BytesIO(f.read())
+                    # Primary use case - from template for graph to excel
+                    else:
+                        # It is assumed that the template is already created and filled during graph_to_excel at this point
+                        # Lets pull a version into memory
+                        with open(self.TEMP_EXCEL_SHEET, "rb") as f:
+                            in_mem_file = io.BytesIO(f.read())
+
+                # If nothing in memory at this point we have an issue
+                if not in_mem_file:
+                    raise RuntimeWarning("No excel data found to open.")
+
+                # provide fresh handles
+                self.excel_wb = pyxl.load_workbook(in_mem_file)
+                self.objects_ws = self.excel_wb[self.OBJECTS_WS_NAME]
+                if self.type == "relations":
+                    self.relations_ws = self.excel_wb[self.RELATIONS_WS_NAME]
+
+                # Perform functions operations
+                func(self, *args, **kwargs)
+
+                # Clean up
+                if save:
+                    self.excel_wb.save(self.TEMP_EXCEL_SHEET)
+                self.kill_excel()
+
+            return wrapper_func
+
+        return decorator
+
+    def disambiguate_object(self, obj: Union[Node, Group, str], direction: str = "out"):
+        """Generate Name:ID string for object - disambiguate if needed.
+        direction: [in|out] - in for excel to graph, out for graph to excel"""
+
+        if direction == "out":
+            if not obj:
+                return None
+            if obj.name in self.original_stats.duplicate_names:  # migrate to using graphstats
+                return obj.name + self.DISAMBIGUATING_SEPARATOR + obj.id  # FIXME: IN EXCEL_TO_GRAPH
+            else:
+                return obj.name
+        elif direction == "in":
+            if not obj:
+                return None, None
+
+            if self.DISAMBIGUATING_SEPARATOR in obj:
+                name = obj.split(self.DISAMBIGUATING_SEPARATOR)[0]
+                id = obj.split(self.DISAMBIGUATING_SEPARATOR)[1]
+                if not all([name, id]):
+                    warn(f"Invalid deduplication format of edge information or empty name: {name}:{id}.", SyntaxWarning)
+                    return name, id
+                # Normal situation in deduplication notation
+                else:
+                    return name, id
+            # For normal non duplicate case
+            else:
+                return obj, None  # name,id
+
+    @open_close_excel(save=True)
+    def graph_to_excel_conversion(self, type=None, graph=None) -> None:
+        """Converting graph object to excel sheet format for bulk data management operations."""
+        # lets assume there can be multiple graphs in session - so we should pass
+        if graph:
+            self.graph = graph
+
+        # Lets gather starting stats
+        self.original_stats = self.graph.gather_graph_stats()
+
+        def graph_object_extract_to_excel(self, input_node: Union[Group, Graph], indent_level):
+            """Extracting graph objects to excel."""
+            nonlocal row
+
+            sub_nodes = input_node.nodes
+            sub_groups = input_node.groups
+
+            for node in sub_nodes.values():
+                # desc = node.get(description, "")
+                # url = node.get(url, "")
+
+                # posting to excel
+                self.objects_ws.cell(row=row, column=indent_level, value=node.name)
+                self.objects_ws.cell(row=row, column=indent_level + 1, value=node.id)
+                row += 1
+
+            for group in sub_groups.values():
+                # id = group.id or ""
+                # label = getattr(group, "label", "")
+
+                # posting to excel
+                self.objects_ws.cell(row=row, column=indent_level, value=group.name)
+                self.objects_ws.cell(row=row, column=indent_level + 1, value=group.id)
+                row += 1
+
+                # Recursive extraction - adapting indent
+                graph_object_extract_to_excel(self, group, indent_level=indent_level + 1)
+
+        def relations_extract_to_excel(self, input_node: Union[Group, Graph]):
+            """Extract relations recursively - providing owner if needed"""
+            nonlocal row
+
+            # Go through edges of this "owning" object
+            sub_edges = input_node.edges
+            for edge in sub_edges.values():
+                node1name = self.disambiguate_object(edge.node1)
+                node2name = self.disambiguate_object(edge.node2)
+
+                group_name = ""
+                if isinstance(input_node, Group):
+                    group_name = self.disambiguate_object(input_node)
+
+                edge_name = self.disambiguate_object(edge)
+
+                # post to excel
+                self.relations_ws.cell(row=row, column=col, value=node1name)
+                self.relations_ws.cell(row=row, column=col + 1, value=node2name)
+                self.relations_ws.cell(row=row, column=col + 2, value=edge_name)
+                self.relations_ws.cell(row=row, column=col + 3, value=group_name)
+                row += 1
+
+            # Go to next level of relations / ownership - recursive
+            sub_groups = input_node.groups
+            for group in sub_groups.values():
+                relations_extract_to_excel(self, group)
+
+        # Perform the transformation to excel ========================
+        if self.type == "obj_and_hierarchy" or self.type == "relations":
+            row = 2
+            graph_object_extract_to_excel(self, self.graph, indent_level=1)
+
+        if self.type == "relations":
+            row = 2
+            col = 1
+            relations_extract_to_excel(self, self.graph)
+
+    @open_close_excel(save=False)
+    def excel_to_graph_conversion(self, type: Optional[str] = None, excel_data=None):
+        """Converting excel sheet data back into graph object."""
+        self.bulk_data_op_verify(type)
+
+        # Update original stats
+        self.original_stats = self.graph.gather_graph_stats()
+
+        # Begin transformation from excel to graph ========================
+        if self.type == "obj_and_hierarchy":
+            # Pull out object data
+            obj_data = list(self.objects_ws.values)
+            obj_data.pop(0)  # remove header
+
+            # identifying indents in excel (marker for groupings)
+            indent: list[int] = []
+            for row in obj_data:
+                none_i = 0
+                for val in row:
+                    if val == None:
+                        none_i += 1
+                    else:
+                        break  # per row for
+                indent.append(none_i)
+
+            # identifying groups
+            num_items = len(obj_data)
+            group_identifiers = list(map(lambda x: 1 if indent[x + 1] > indent[x] else 0, range(0, num_items - 1)))
+            group_identifiers.append(0)  # small limitation - deepest or last cannot be group - must have submembers
+
+            # sorting ownership based on indents/groups
+            owner_indexing: dict[int, Union[int, None]] = dict()
+            indent_and_group_ident = list(zip(indent, group_identifiers))
+            for i in range(0, num_items):
+                owner_indexing[i] = None
+                if i == 0:
+                    continue
+                curr_indent = indent[i]
+                for j, (indent_i, is_group) in enumerate(reversed(indent_and_group_ident[:i])):
+                    if indent_i == curr_indent - 1 and is_group == 1:
+                        owner_indexing[i] = i - (j + 1)
+                        break
+
+            # Building / Modifying objects
+            objects = list()
+            object_id_mappings: dict[str, str] = dict()
+            # all_bulk_mod_ids = set()
+            # all_curr_obj_ids = set(self.original_id_to_obj.keys())
+            for i, (starting_indent, gr_i, obj_row) in enumerate(zip(indent, group_identifiers, obj_data)):
+                # Extracting label and id
+                name = obj_row[starting_indent]
+                id = None
+                try:
+                    id = obj_row[starting_indent + 1]
+                except Exception as e:
+                    print(f"Node missing Id: {e}.")
+
+                # Checks
+                id_exists = id is not None
+                id_found = id in self.original_stats.all_objects.keys()
+
+                is_group = gr_i == 1
+                is_node = gr_i == 0
+                is_group_owned = owner_indexing[i] is not None
+                if is_group_owned:
+                    owner_index = owner_indexing[i]  # this works because the owner is always before
+                    owner_object = objects[owner_index]
+                else:
+                    owner_object = self.graph
+
+                # This is a new object - create it
+                if not id_found:
+                    # Add group
+                    if is_group:
+                        new_group = owner_object.add_group(name)
+                        objects.append(new_group)
+
+                        if id_exists:
+                            object_id_mappings[id] = new_group.id
+
+                    # Add node
+                    elif is_node:
+                        new_node = owner_object.add_node(name)
+                        objects.append(new_node)
+                        if id_exists:
+                            object_id_mappings[id] = new_node.id
+                    else:
+                        raise NotImplementedError("This state not implemented")
+
+                elif id_exists:  # TODO: NEED TO FINISH THIS
+                    # recovering previous object
+                    existing_obj = self.original_stats.all_objects[id]
+
+                    # change from node -> group
+                    if isinstance(existing_obj, Node) and is_group:
+                        # remove node
+                        existing_obj.parent.remove_node(id)
+
+                        # add group
+                        new_group = owner_object.add_group(name)
+                        objects.append(new_group)
+                        object_id_mappings[id] = new_group.id
+
+                        # TODO: ADD CONVERSION MAPPING - ID CHANGES
+
+                    # changed structuring from node <-> group
+                    # group -> node
+                    elif isinstance(existing_obj, Group) and not is_group:
+                        # remove group (without changing dependencies)
+                        existing_obj.parent.remove_group(existing_obj, heal=False)
+
+                        # add node
+                        new_node = owner_object.add_node(name)
+                        objects.append(new_node)
+                        object_id_mappings[id] = new_node.id
+
+                    elif existing_obj.name != name:
+                        existing_obj.name = name
+
+                    objects.append(existing_obj)
+
+            # Deleted objects - items previously with ids and ids are no longer there
+            # Finding difference of ids - previous ids no longer there... #FIXME: WHAT ABOUT CHANGED IDS?
+            all_updated_ids = set([obj.id for obj in [obj for obj in objects if obj] if obj.id])
+            all_orig_object_ids = set(self.original_stats.all_objects)
+            all_deleted_obj_ids = all_orig_object_ids.difference(all_updated_ids)
+            for obj_id in all_deleted_obj_ids:
+                obj: Group | Node = self.original_stats.all_objects[obj_id]
+                parent = obj.parent or self.graph
+                if isinstance(obj, Group):  # group
+                    # find all immediate dependents and connect them to owner
+                    parent.remove_group(obj_id)  # TODO: SHOULD HEALING BE REMOVED?
+
+                elif isinstance(obj, Node):  # node
+                    parent.remove_node(obj_id)
+
+        elif self.type == "relations":
+            # Access the relations sheet
+            self.relations_ws = self.excel_wb[self.RELATIONS_WS_NAME]
+            relations_data = self.relations_ws.values
+            row_length = None
+
+            # declarations
+            edge_ids_after_mod = set()
+
+            # process sheet rows
+            count: int = 0
+            for row in relations_data:
+                if count == 0:
+                    row_length = len(row)
+                    count += 1
+                    continue
+
+                # Declarations ===================================
+                # names
+                node1_name: str = ""
+                node2_name: str = ""
+                edge_name: str = ""
+                owner_name: str = ""
+
+                # ids
+                node1_id: str = ""
+                node2_id: str = ""
+                edge_id: str = ""
+                owner_id: str = ""
+
+                # found flag
+                node1_found = False
+                node2_found = False
+                edge_found = False
+                owner_found = False
+
+                # separating row values into variables (before disambiguation)
+                if row_length == 4:
+                    node1_name, node2_name, edge_name, owner_name = row
+                    edge_id = str(edge_id)
+                elif row_length == 3:
+                    node1_name, node2_name, edge_name = row
+                elif row_length == 2:
+                    node1_name, node2_name = row
+
+                # Quick check if we are working with minimally complete data
+                # At this point the name is name(+id) - assumed we can ignore empty nodes / warn
+                two_node_check = node1_name is not None and node2_name is not None
+                if not two_node_check:
+                    warn("Node names not found...skipping line of Relations.", SyntaxWarning)
+                    continue
+
+                # Disambiguate the object information based on constant separator
+                node1_name, node1_id = self.disambiguate_object(node1_name, direction="in")
+                node2_name, node2_id = self.disambiguate_object(node2_name, direction="in")
+                edge_name, edge_id = self.disambiguate_object(edge_name, direction="in")
+                owner_name, owner_id = self.disambiguate_object(owner_name, direction="in")
+
+                # Try to reidentify items ========================================
+                def find_checks(name, id):
+                    result_object = None
+                    id_found = False
+                    name_found = False
+
+                    # look for ID - in case of disambiguation
+                    if id:
+                        id_found = id in self.original_stats.all_objects.keys()
+                        if id_found:
+                            result_object = self.original_stats.all_objects[id]
+
+                    if not result_object:
+                        # Look by name
+                        if name:
+                            name_found = (
+                                name in self.original_stats.name_to_ids.keys()
+                                and not self.original_stats.name_reused(name)
+                            )
+                            if name_found:
+                                result_object = self.original_stats.all_objects[
+                                    self.original_stats.name_to_ids[name][0]
+                                ]
+
+                    return result_object, result_object is not None  # , any(id_found, name_found), id_found, name_found
+
+                # Looking for edge =================================
+                edge_object, edge_found = find_checks(edge_name, edge_id)
+
+                # Looking for node 1 ================================
+                node1_object, node1_found = find_checks(node1_name, node1_id)
+
+                # Looking for node 2 =================================
+                node2_object, node2_found = find_checks(node2_name, node2_id)
+
+                # Looking for owner =================================
+                owner_object, owner_found = find_checks(owner_name, owner_id)
+
+                # At this point - it is assumed that the user already ran objects and hierarchy and therefore objects are fixed
+                edge_nodes_found = all([node1_found, node2_found])
+                if not edge_nodes_found:
+                    warn("Object not found...skipping line of Relations.", SyntaxWarning)
+                    continue
+
+                # found edge - modify
+                if edge_found:
+                    # Update Node 1, node2, name
+                    edge_object.node1 = node1_object
+                    edge_object.node2 = node2_object
+                    edge_object.name = edge_name
+
+                    # if no owner specified - assign to graph
+                    if owner_name or owner_id:  # owner specified
+                        pass  # do nothing here
+                    else:  # no owner specified
+                        owner_object = self.graph  # specify graph as parent
+
+                    # check ownership change
+                    if edge_object.parent is not owner_object:  # if change in parent
+                        # update ownership
+                        # TODO: UPDATE EDGE OWNER
+                        if owner_object:
+                            # remove edge
+                            edge_object.parent.remove_edge(edge_object)
+                            # Add edge
+                            new_edge = owner_object.add_edge(edge_object)
+                        else:  # no  owner successfully specified
+                            # add edge
+                            new_edge = owner_object.add_edge(edge_object)
+                    # Otherwise - just passing on edge for id recording
+                    else:
+                        new_edge = edge_object
+
+                    # keep track of edges that were existing and still existing
+                    edge_ids_after_mod.add(new_edge.id)
+
+                # not found - create
+                elif not edge_found:
+                    edge_init_dict = dict()
+                    edge_init_dict["node1"] = node1_object
+                    edge_init_dict["node2"] = node2_object
+                    edge_init_dict["name"] = edge_name
+                    edge_init_dict = {key: value for (key, value) in edge_init_dict.items() if value is not None}
+                    if not owner_object:
+                        owner_object = self.graph
+                    new_edge = owner_object.add_edge(**edge_init_dict)
+                    edge_ids_after_mod.add(new_edge.id)
+
+            # Deleting edges that have been deleted
+            all_bulk_edge_ids = set(list(self.original_stats.all_edges.keys()))
+            all_deleted_edge_ids = all_bulk_edge_ids.difference(edge_ids_after_mod)
+            for del_edge_id in all_deleted_edge_ids:
+                edge_obj: Edge = self.original_stats.all_edges[del_edge_id]
+                parent = edge_obj.parent or self.graph
+                parent.remove_edge(del_edge_id)
+
+        elif self.type == "object_data":  # TODO: Implement management of deeper data - url, description, formatting
+            raise NotImplementedError("This functionality is not yet implemented.")
+
+        # Run Checks to avoid problems of manual data management
+        self.graph.run_graph_rules()
+
+    def give_user_chance_to_modify(self):
+        """Open Excel for user to modify data."""
+        # kill excel process
+        self.kill_excel()
+
+        if show_guis:
+            os.startfile(self.TEMP_EXCEL_SHEET)
+
+            user_response = msg.askokcancel(
+                title="yEd Bulk Data Management - Async", message="To process changes, save workbook and press ok."
+            )
+
+            if not user_response:
+                print("User cancelled operation.")
+                sys.exit()
+
+    def bulk_data_management(self, type=None, graph=None, excel_data=None):
+        """Process of converting to excel for manual operations, allows user to modify and then convert back to graph."""
+        self.graph_to_excel_conversion(type=type, graph=graph)
+        self.give_user_chance_to_modify()
+        self.excel_to_graph_conversion(type=type, excel_data=excel_data)
+
+        return self
 
 
 class Graph:
     """Graph structure - carries yEd graph information"""
 
-    def __init__(self, directed="directed", graph_id="G"):
-        self.nodes = {}
-        self.edges = {}
-        self.num_edges = 0
-
+    def __init__(self, directed="directed", id="G"):
         self.directed = directed
-        self.graph_id = graph_id
-        self.existing_entities = dict()
+        self.id = id
 
-        self.groups = {}
+        self.nodes: dict[str, Node] = {}
+        self.groups: dict[str, Group] = {}
+        self.edges: dict[str, Edge] = {}
+        self.combined_objects: dict[str, Union[(Node, Group)]] = {}
 
         self.custom_properties = []
 
-        self.graphml: ET.Element  # FIXME:
+        self.graphml: ET.Element
 
     # Addition of items ============================
-    def add_node(self, node_name, **kwargs):
-        """Adding defined node to graph"""
-        if node_name in self.existing_entities:
-            raise RuntimeWarning("Node %s already exists" % node_name)
-
-        node = Node(node_name, **kwargs)
-        self.nodes[node_name] = node
-        self.existing_entities[node_name] = node
-        return node
-
-    def add_edge(self, node1_id, node2_id, **kwargs):
-        """Adding edge to graph - uses node names not node objects."""
+    def add_node(self, node: Union[Node, str, None] = None, **kwargs) -> Node:
+        """Adding node within Graph - accepts node object (simply assigns), or node name or none (to create new node)."""
+        return add_node(self, node, **kwargs)
+
+    def add_group(self, group: Union[Group, str, None] = None, **kwargs) -> Group:
+        """Adding group to Graph"""
+        return add_group(self, group, **kwargs)
+
+    def add_edge(
+        self,  # owner
+        node1: Optional[Union[(Node, Group, str)]] = None,
+        node2: Optional[Union[(Node, Group, str)]] = None,
+        **kwargs,
+    ) -> Edge:
+        """Adding edge to Graph - for node1/node2 uses node / group objects or accepts names (creating new nodes under self) - or function can alternatively accept an instantiated Edge object."""
+
+        # map args into kwargs in case of excel data management ops
+        if node1:
+            kwargs["node1"] = node1
+        if node2:
+            kwargs["node2"] = node2
 
-        # Ensuring nodes are existing at time of edge creation (error avoidance) - dont need assignments
-        node1 = self.existing_entities.get(node1_id) or self.add_node(node1_id)
-        node2 = self.existing_entities.get(node2_id) or self.add_node(node2_id)
-
-        self.num_edges += 1
-        kwargs["edge_id"] = str(self.num_edges)
-        edge = Edge(node1_id, node2_id, **kwargs)
-        self.edges[edge.edge_id] = edge
-        edge.parent = self
-        return edge
-
-    def add_group(self, group_id, **kwargs):
-        """Adding group to graph"""
-        if group_id in self.existing_entities:
-            raise RuntimeWarning("Group %s already exists" % group_id)
-
-        group = Group(group_id, self, **kwargs)
-        self.groups[group_id] = group
-        self.existing_entities[group_id] = group
-        return group
+        return add_edge(self, **kwargs)
 
     def define_custom_property(self, scope, name, property_type, default_value):
         """Adding custom properties to graph (which makes them available on the contained objects in yEd)"""
         if scope not in CUSTOM_PROPERTY_SCOPES:
             raise RuntimeWarning("Scope %s not recognised" % scope)
         if property_type not in CUSTOM_PROPERTY_TYPES:
             raise RuntimeWarning("Property Type %s not recognised" % property_type)
@@ -1054,54 +1585,30 @@
         self.custom_properties.append(custom_property)
         if scope == "node":
             Node.set_custom_properties_defs(custom_property)
         elif scope == "edge":
             Edge.set_custom_properties_defs(custom_property)
 
     # Removal of items ==============================
-    def remove_node(self, node_name) -> None:
+    def remove_node(self, node: Union[Node, str]) -> None:
         """Remove/Delete a node from graph"""
-        if node_name not in self.existing_entities:
-            raise RuntimeWarning("Node %s doesn't exist" % node_name)
-        del self.nodes[node_name]
-        del self.existing_entities[node_name]
-
-    def remove_group(self, group_id):
-        """Removes a group from within current group object (and same parent graph)."""
-        if group_id not in self.existing_entities:
-            raise RuntimeWarning("Group %s doesn't exist" % group_id)
+        remove_node(self, node)
 
-        # reroute dependents
-        for node in self.nodes.values():
-            node.parent = self  # reassign parent: node side
-            self.nodes[node.node_name] = node  # reassign parent: group side
+    def remove_group(self, group: Union[Group, str], **kwargs) -> None:
+        """Removes a group from within current graph object (and same parent graph)."""
+        remove_group(self, group, **kwargs)
 
-        for edge in self.edges.values():
-            edge.parent = self  # reassign parent: edge side
-            self.edges[edge.edge_id] = edge  # reassign parent: group/graph side
+    def remove_edge(self, edge: Union[Edge, str]) -> None:
+        """Removing edge from graph - uses id."""
+        remove_edge(self, edge)
 
-        for group in self.groups.values():
-            group.parent = self
-            self.groups[group.group_id] = group  # reassign parent: group side
-
-        # eliminate records
-        del self.groups[group_id]
-        del self.existing_entities[group_id]
-
-    def remove_edge(self, edge_id):
-        """Removing edge from graph - uses node names not node objects."""
-        if not self.edges[edge_id]:
-            raise RuntimeWarning("Edge %s does not exist under graph" % (edge_id))
-        del self.edges[edge_id]
-        self.num_edges -= 1
-
-    # TODO: REMOVE / MODIFY CUSTOM PROPERTIES FUNCTIONALITY
+    # TODO: ADD FUNCTIONALITY TO REMOVE / MODIFY CUSTOM PROPERTIES
 
     # Graph functionalities ===========================
-    def construct_graphml(self):
+    def construct_graphml(self) -> None:
         """Creating template graphml xml structure and then placing all graph items into it."""
 
         # Creating XML structure in Graphml format
         # xml = ET.Element("?xml", version="1.0", encoding="UTF-8", standalone="no")
 
         graphml = ET.Element("graphml", xmlns="http://graphml.graphdrawing.org/xmlns")
         graphml.set("xmlns:java", "http://www.yworks.com/xml/yfiles-common/1.0/java")
@@ -1149,15 +1656,15 @@
             graphml.append(prop.convert_to_xml())
 
         edge_key = ET.SubElement(graphml, "key", id="data_edge")
         edge_key.set("for", "edge")
         edge_key.set("yfiles.type", "edgegraphics")
 
         # Graph node containing actual objects
-        graph = ET.SubElement(graphml, "graph", edgedefault=self.directed, id=self.graph_id)
+        graph = ET.SubElement(graphml, "graph", edgedefault=self.directed, id=self.id)
 
         # Convert python graph objects into xml structure
         for node in self.nodes.values():
             graph.append(node.convert_to_xml())
 
         for node in self.groups.values():
             graph.append(node.convert_to_xml())
@@ -1184,28 +1691,33 @@
             pretty_str = minidom.parseString(raw_str).toprettyxml()
             with open(graph_file.fullpath, "w") as f:
                 f.write(pretty_str)
         else:
             tree = ET.ElementTree(self.graphml)
             tree.write(graph_file.fullpath)  # Uses internal method to XML Etree
 
+        # recheck the file as existing or not
+        graph_file.full_path_validate()
+        print("persisting graph to file:", graph_file.fullpath)
         return graph_file
 
-    def stringify_graph(self):
+    def stringify_graph(self) -> str:
         """Returns Stringified version of graph in graphml format"""
         self.construct_graphml()
         # Py2/3 sigh.
         if sys.version_info.major < 3:
             return ET.tostring(self.graphml, encoding="UTF-8")
         else:
             return ET.tostring(self.graphml, encoding="UTF-8").decode()
 
     def from_existing_graph(self, file: str | File):
         """Parse GraphML xml of existing/stored graph file into python Graph structure."""
 
+        id_existing_to_graph_obj = dict()
+
         # Manage file input ==============================
         if isinstance(file, File):
             graph_file = file
         else:
             graph_file = File(file)
         if not graph_file.file_exists:
             raise FileNotFoundError
@@ -1232,15 +1744,15 @@
         graph_root = root.find("graph")
 
         # get major graph info
         graph_dir = graph_root.get("edgedefault")
         graph_id = graph_root.get("id")
 
         # instantiate graph object
-        new_graph = Graph(directed=graph_dir, graph_id=graph_id)
+        new_graph = Graph(directed=graph_dir, id=graph_id)
 
         # Parse graph
 
         def is_group_node(node):
             return "foldertype" in node.attrib
 
         def process_node(parent, input_node):
@@ -1250,27 +1762,27 @@
 
             for node in current_level_nodes:
                 # normal nodes
                 if not is_group_node(node):
                     node_init_dict = dict()
 
                     # <node id="n1">
-                    node_init_dict["node_name"] = node.attrib.get("id", None)
+                    existing_node_id = node.attrib.get("id", None)  # FIXME:
 
                     data_nodes = node.findall("data")
                     info_node = None
                     for data_node in data_nodes:
                         info_node = data_node.find("GenericNode") or data_node.find("ShapeNode")
                         if info_node is not None:
                             node_init_dict["node_type"] = info_node.tag
 
                             node_label = info_node.find("NodeLabel")
                             if node_label is not None:
-                                node_init_dict["label"] = node_label.text
-                                print("here")
+                                node_init_dict["name"] = node_label.text
+
                                 # TODO: PORT REST OF NODELABEL
 
                             # <Fill color="#FFCC00" transparent="false" />
                             fill = info_node.find("Fill")
                             if fill is not None:
                                 node_init_dict["shape_fill"] = fill.get("color")
                                 node_init_dict["transparent"] = fill.get("transparent")
@@ -1292,42 +1804,42 @@
                                 node_init_dict["shape"] = uml.get("AttributeLabel")
                             # TODO: THERE IS FURTHER DETAIL TO PARSE HERE under uml
                         else:
                             info = data_node.text
                             if info is not None:
                                 info = re.sub(r"<!\[CDATA\[", "", info)  # unneeded schema
                                 info = re.sub(r"\]\]>", "", info)  # unneeded schema
-                                print("info:", info)
 
                                 the_key = data_node.attrib.get("key")
 
                                 info_type = key_dict[the_key]["attr"]
                                 if info_type in ["url", "description"]:
                                     node_init_dict[info_type] = info
                     # Removing empty items
                     node_init_dict = {key: value for (key, value) in node_init_dict.items() if value is not None}
                     # create node
-                    parent.add_node(**node_init_dict)
+                    new_node = parent.add_node(**node_init_dict)
+                    id_existing_to_graph_obj[existing_node_id] = new_node
 
                 # group nodes
                 # <node id="n2" yfiles.foldertype="group">
                 elif is_group_node(node):
                     group_init_dict = dict()
 
                     # <node id="n1">
-                    group_init_dict["group_id"] = node.attrib.get("id", None)
+                    existing_group_id = node.attrib.get("id", None)
 
                     # Actual Group Data ===================================
                     data_nodes = node.findall("data")
                     for data_node in data_nodes:
                         proxy = data_node.find("ProxyAutoBoundsNode")
                         if proxy is not None:
                             realizer = proxy.find("Realizers")
 
-                            group_nodes = realizer.findall("GroupNode")  # TODO: When are there multiple?
+                            group_nodes = realizer.findall("GroupNode")
 
                             for group_node in group_nodes:
                                 geom_node = group_node.find("Geometry")
                                 if geom_node is not None:
                                     group_init_dict["height"] = geom_node.attrib.get("height", None)
                                     group_init_dict["width"] = geom_node.attrib.get("width", None)
                                     group_init_dict["x"] = geom_node.attrib.get("x", None)
@@ -1342,15 +1854,17 @@
                                 if borderstyle_node is not None:
                                     group_init_dict["border_color"] = borderstyle_node.attrib.get("color", None)
                                     group_init_dict["border_type"] = borderstyle_node.attrib.get("type", None)
                                     group_init_dict["border_width"] = borderstyle_node.attrib.get("width", None)
 
                                 nodelabel_node = group_node.find("NodeLabel")
                                 if nodelabel_node is not None:
-                                    group_init_dict["label"] = nodelabel_node.text
+                                    group_init_dict["name"] = (
+                                        nodelabel_node.text
+                                    )  # TODO: SHOULD THIS JUST BE THE FIRST ONE?  IN OTHER WORDS - IS THERE MULTIPLE THINGS TO BE CAUGHT HERE?
                                     group_init_dict["font_family"] = nodelabel_node.attrib.get("fontFamily", None)
                                     group_init_dict["font_size"] = nodelabel_node.attrib.get("fontSize", None)
                                     group_init_dict["underlined_text"] = nodelabel_node.attrib.get(
                                         "underlinedText", None
                                     )
                                     group_init_dict["font_style"] = nodelabel_node.attrib.get("fontStyle", None)
                                     group_init_dict["label_alignment"] = nodelabel_node.attrib.get("alignment", None)
@@ -1362,24 +1876,21 @@
                                 group_state_node = group_node.find("State")
                                 if group_state_node is not None:
                                     group_init_dict["closed"] = group_state_node.attrib.get("closed", None)
                                     # group_init_dict["aaa"] = group_state_node.attrib.get("closedHeight",None)
                                     # group_init_dict["aaaa"] = group_state_node.attrib.get("closedWidth",None)
                                     # group_init_dict["aaaa"] = group_state_node.attrib.get("innerGraphDisplayEnabled",None)
 
-                                # TODO: GATHER THE MULTIPLE GROUP NODES
-
                                 break
 
                         else:
                             info = data_node.text
                             if info is not None:
                                 info = re.sub(r"<!\[CDATA\[", "", info)  # unneeded schema
                                 info = re.sub(r"\]\]>", "", info)  # unneeded schema
-                                print("info:", info)
 
                                 the_key = data_node.attrib.get("key")
 
                                 info_type = key_dict[the_key]["attr"]
                                 if info_type in ["url", "description"]:
                                     group_init_dict[info_type] = info
 
@@ -1387,31 +1898,40 @@
                     sub_graph_node = node.find("graph")
 
                     # Removing empty items
                     group_init_dict = {key: value for (key, value) in group_init_dict.items() if value is not None}
 
                     # Creating new group
                     new_group = parent.add_group(**group_init_dict)
+                    id_existing_to_graph_obj[existing_group_id] = new_group
 
                     # Recursive processing
                     if sub_graph_node is not None:
                         process_node(parent=new_group, input_node=sub_graph_node)
 
                 # unknown node type
                 else:
                     raise NotImplementedError
 
             # edges then establish connections
             for edge_node in current_level_edges:
                 edge_init_dict = dict()
 
                 # <node id="n1">
-                edge_init_dict["edge_id"] = edge_node.attrib.get("id", None)
-                edge_init_dict["node1_id"] = edge_node.attrib.get("source", None)
-                edge_init_dict["node2_id"] = edge_node.attrib.get("target", None)
+                edge_id = edge_node.attrib.get("id", None)
+                node1_id = edge_node.attrib.get("source", None)
+                node2_id = edge_node.attrib.get("target", None)
+
+                try:
+                    edge_init_dict["node1"] = id_existing_to_graph_obj.get(node1_id)
+                    edge_init_dict["node2"] = id_existing_to_graph_obj.get(node2_id)
+                except Exception as e:  # TODO: MAKE MORE SPECIFIC
+                    print(f"One of nodes of existing edge {edge_id} not found: {node1_id}, {node2_id} ")
+
+                # FIXME: HOW TO MOVE FROM NODE IDS TO NODE OBJECTS - MOVE THROUGH GRAPHML FOR THE TEXT OF THAT OBJECT? - OR USE A DICTIONARY
 
                 # <data key="d5">
                 data_nodes = edge_node.findall("data")
                 for data_node in data_nodes:
                     polylineedge = data_node.find("PolyLineEdge")
 
                     if polylineedge is not None:
@@ -1441,432 +1961,64 @@
                             edge_init_dict["arrowhead"] = edgelabel_node.attrib.get("target", None)
 
                     else:
                         info = data_node.text
                         if info is not None:
                             info = re.sub(r"<!\[CDATA\[", "", info)  # unneeded schema
                             info = re.sub(r"\]\]>", "", info)  # unneeded schema
-                            print("info:", info)
 
                             the_key = data_node.attrib.get("key")
 
                             info_type = key_dict[the_key]["attr"]
                             if info_type in ["url", "description"]:
                                 edge_init_dict[info_type] = info
 
                 # bendstyle_node = polylineedge.find("BendStyle")
-                # edge_init_dict["smoothed"] = linestyle_node.attrib.get("smoothed") # FIXME
+                # edge_init_dict["smoothed"] = linestyle_node.attrib.get("smoothed") # TODO: ADD THIS
 
                 # TODO:
                 #   CUSTOM PROPERTIES
 
                 # Removing empty items
                 edge_init_dict = {key: value for (key, value) in edge_init_dict.items() if value is not None}
                 parent.add_edge(**edge_init_dict)
 
         process_node(parent=new_graph, input_node=graph_root)
 
         return new_graph
 
-    def manage_graph_data_in_excel(self, type=None):
-        """Port graph data into Excel in several formats for easy and bulk creation and management.  Then ports back into python graph structure."""
-
-        TEMP_EXCEL_SHEET = "test.xlsx"
-
-        MANAGE_TYPES = {"obj_and_hierarchy", "object_data", "relations"}
-
-        type = type or "obj_and_hierarchy"  # default
-
-        # create workbook
-        excel_wb = pyxl.Workbook()
-
-        # Inserting /organizing sheets
-        excel_ws = excel_wb.active
-
-        # Extract objects ============================================
-        original_stats = self.gather_graph_stats()
-        id_to_label = dict()
-        id_to_obj = dict()
-        OBJECTS_WS_NAME = "Objects_and_Groups"
-        objects_ws = excel_wb.create_sheet(OBJECTS_WS_NAME, 0)
-
-        # HEADER
-        objects_ws.cell(
-            row=1, column=1, value="FORMAT -> LABEL | ID (INDENTATION OF INFO MEANS BELONGING TO GROUP ABOVE.)"
-        )
-
-        row = 2
-
-        def object_extract(self, input_node, indent_level):
-            nonlocal row
-            nonlocal id_to_label
-            nonlocal id_to_obj
-
-            sub_nodes = input_node.nodes
-            sub_groups = input_node.groups
-            sub_edges = input_node.edges
-
-            for node in sub_nodes.values():
-                id = node.node_name or ""
-                labels = getattr(node, "list_of_labels")
-                # desc = node.get(description, "")
-                # url = node.get(url, "")
-                if labels:
-                    label = labels[0]._text  # ASSUMPTION: that this would make sense for most graphs
-                else:
-                    label = ""
-
-                id_to_label[id] = label
-                id_to_obj[id] = node
-
-                objects_ws.cell(row=row, column=indent_level, value=label)
-                objects_ws.cell(row=row, column=indent_level + 1, value=id)
-                row += 1
-
-            for group in sub_groups.values():
-                id = group.group_id or ""
-                label = getattr(group, "label", "")
-                objects_ws.cell(row=row, column=indent_level, value=label)
-                objects_ws.cell(row=row, column=indent_level + 1, value=id)
-                row += 1
-                print(id, label)
-
-                id_to_label[id] = label
-                id_to_obj[id] = group
-                object_extract(self, group, indent_level=indent_level + 1)
-
-        object_extract(self, self, indent_level=1)
-
-        # Extract Relations =======================================================
-        if type == "relations":
-            RELATIONS_WS_NAME = "Relations"
-            relations_ws = excel_wb.create_sheet(RELATIONS_WS_NAME, 1)
-            row = 2
-            col = 1
-            relations_ws.cell(row=1, column=1, value="FORMAT -> NODE1 | NODE2 | EDGE_LABEL | EDGE_ID ")
-            obj_keys = list(id_to_label.keys())
-            obj_values = list(id_to_label.values())
-            dup_objects = list(filter(lambda x: True if obj_values.count(x) > 1 else False, obj_values))
-
-            def relations_extract(self, input_node):
-                nonlocal row
-
-                sub_groups = input_node.groups
-                sub_edges = input_node.edges
-
-                for edge in sub_edges.values():
-                    id = edge.edge_id or ""
-                    node1 = getattr(edge, "node1")
-                    node2 = getattr(edge, "node2")
-                    labels = getattr(edge, "list_of_labels")
-                    if labels:
-                        label = labels[0]._text  # ASSUMPTION: that this would make sense for most graphs
-                    else:
-                        label = ""
-
-                    def deduplicate_obj(id):
-                        name = id_to_label[id]
-                        if name in dup_objects:
-                            return id + "##" + name
-                        else:
-                            return name
-
-                    node1name = deduplicate_obj(node1)
-                    node2name = deduplicate_obj(node2)
-
-                    group_name = ""
-                    if isinstance(input_node, Group):
-                        group_name = deduplicate_obj(input_node.group_id)
-
-                    relations_ws.cell(row=row, column=col, value=node1name)
-                    relations_ws.cell(row=row, column=col + 1, value=node2name)
-                    relations_ws.cell(row=row, column=col + 2, value=label)
-                    relations_ws.cell(row=row, column=col + 3, value=id)
-                    relations_ws.cell(row=row, column=col + 4, value=group_name)
-                    row += 1
-
-                for group in sub_groups.values():
-                    relations_extract(self, group)
-
-            relations_extract(self, self)
-
-        # potentially saving
-        excel_wb.remove(excel_ws)  # removing default sheet
-        excel_wb.save(TEMP_EXCEL_SHEET)
-        excel_wb.close()
-
-        os.startfile(TEMP_EXCEL_SHEET)
-
-        # some kind of signal?
-
-        user_response = msg.askokcancel(
-            title="yEd Bulk Data Management - Async", message="To process changes, save workbook and press ok."
-        )
-        if not user_response:
-            return
-
-        excel_wb = pyxl.load_workbook(TEMP_EXCEL_SHEET)
-
-        if type == "obj_and_hierarchy":
-            # read the data back into structure - making changes
-            # read excel for data / get some stats
-            objects_ws = excel_wb[OBJECTS_WS_NAME]
-            obj_data = list(objects_ws.values)
-            obj_data.pop(0)  # remove header
-
-            # identifying indents in excel (marker for groupings)
-            indent: list[int] = []
-            for row in obj_data:
-                none_i = 0
-                for val in row:
-                    if val == None:
-                        none_i += 1
-                    else:
-                        break  # per row for
-                indent.append(none_i)
-
-            # identifying groups
-            num_items = len(obj_data)
-            group_identifiers = list(map(lambda x: 1 if indent[x + 1] > indent[x] else 0, range(0, num_items - 1)))
-            group_identifiers.append(0)  # small limitation - deepest or last cannot be group
-
-            # identifying ownership
-            owner = dict()
-            indent_and_group_ident = list(zip(indent, group_identifiers))
-            for i in range(0, num_items):
-                owner[i] = None
-                if i == 0:
-                    continue
-                curr_indent = indent[i]
-                for j, (indent_i, is_group) in enumerate(reversed(indent_and_group_ident[:i])):
-                    if indent_i == curr_indent - 1 and is_group == 1:
-                        owner[i] = i - (j + 1)
-                        break
-
-            # of format: label|id (optional)
-
-            # identifying last used Id # TODO: NEEDS REFACTORING - ID COUNTING in yEd IS PER OWNER
-            ids = sorted(id_to_label)
-            if ids:
-                last_id = ids[-1]
-                last_id_num = re.match(r".*?(\d+)", last_id)
-                if last_id_num and last_id_num.group(1):
-                    last_id = int(last_id_num.group(1))
-            else:
-                last_id = 0
-
-            objects = list()
-            # Building / Modifying objects
-            all_bulk_mod_ids = set()
-            all_curr_obj_ids = set(id_to_obj.keys())
-            for i, (nr_indent, gr_i, obj_row) in enumerate(zip(indent, group_identifiers, obj_data)):
-                # possibilities:
-                #     completely new node / group
-                #     changed label - same node and structure
-                #     changed structuring - groups vs nodes
-                # changed structuring from node <-> group
-                #     changed owner
-                #     changed owning
-                #     there can be multiple groups at same level
-                #     negative - when in this mode - dont have ability to detect  / correct now problem relationships
-                # deleted nodes (id is no longer existing)
-
-                # Extracting label and id
-                label = obj_row[nr_indent]
-                id = None
-                try:
-                    id = obj_row[nr_indent + 1]
-                except Exception as e:
-                    print(f"Node missing Id: {e}. Id will be assigned.")
-                else:
-                    all_bulk_mod_ids.add(id)
-
-                # Checks
-                id_given = id is not None
-                id_exists = id is not None and id in id_to_label
-                is_group = gr_i == 1
-                is_node = gr_i == 0
-                is_group_owned = owner[i] is not None
-
-                # giving an id if not one assigned
-                if not id_given:
-                    if is_group:
-                        id = "g" + str(last_id + 1)
-                    if is_node:
-                        id = "n" + str(last_id + 1)
-                    last_id += 1
-
-                if is_group_owned:
-                    owner_inst = objects[owner[i]]
-
-                # This is a new object
-                if not id_exists:
-                    if is_group:
-                        if is_group_owned:
-                            objects.append(owner_inst.add_group(group_id=id, label=label))
-                        else:
-                            objects.append(self.add_group(group_id=id, label=label))
-
-                    elif is_node:
-                        if is_group_owned:
-                            objects.append(owner_inst.add_node(node_name=id, label=label))
-                        else:
-                            objects.append(self.add_node(node_name=id, label=label))
-
-                    else:
-                        raise NotImplementedError("This state not implemented")
-
-                elif id_exists:
-                    # changed name
-                    existing_obj = id_to_obj[id]
-
-                    # changed structuring from node <-> group
-
-                    # changed owner
-
-                    # changed owning
-
-                    objects.append(existing_obj)
-
-                    pass
-
-            # Deleted objects
-            all_deleted_obj_ids = all_curr_obj_ids.difference(all_bulk_mod_ids)
-            for obj_id in all_deleted_obj_ids:
-                obj: Group | Node = id_to_obj[obj_id]
-                parent = obj.parent or self
-                if isinstance(obj, Group):  # group
-                    # find all immediate dependents and connect them to owner
-                    parent.remove_group(obj_id)
-
-                elif isinstance(obj, Node):  # node
-                    parent.remove_node(obj_id)
-
-        elif type == "relations":  # TODO: Implement this
-            # Columns
-            # node1name
-            # node2name
-            # label
-            # id
-            relations_ws = excel_wb[RELATIONS_WS_NAME]
-            relations_data = relations_ws.values
-            row_length = None
-            edge_ids_after_mod = set()
-
-            count = 0
-            for row in relations_data:
-                if count == 0:
-                    row_length = len(row)
-                    count += 1
-                    continue
-                node1_name = None
-                node2_name = None
-                edge_label = None
-                edge_id = None
-
-                if row_length == 4:
-                    node1_name, node2_name, edge_label, edge_id = row
-                elif row_length == 3:
-                    node1_name, node2_name, edge_label = row
-                elif row_length == 2:
-                    node1_name, node2_name = row
-
-                edge_id = str(edge_id)
-
-                two_node_id_check = node1_name is not None and node2_name is not None
-                if not two_node_id_check:
-                    continue
-
-                id_assigned = edge_id is not None
-                label_check = edge_label is not None
-
-                id_exist = False
-                if id_assigned:
-                    id_exist = str(edge_id) in original_stats.all_edges.keys()
-
-                node1_found = node1_name in obj_values
-                node1_dedup_req = node1_name in dup_objects
-                if node1_found and not node1_dedup_req:
-                    node1_id = obj_keys[obj_values.index(node1_name)]
-                # TODO: ADD LOGIC FOR node1_found and node1_dedup_req
-
-                node2_found = node2_name in obj_values
-                node2_dedup_req = node2_name in dup_objects
-                if node2_found and not node2_dedup_req:
-                    node2_id = obj_keys[obj_values.index(node2_name)]
-                # TODO: ADD LOGIC FOR node2_found and node2_dedup_req
-
-                nodes_found = False
-                if node1_id and node2_id:
-                    nodes_found = True
-
-                # modify
-                if id_exist and nodes_found:
-                    # make changes - but only if nodes are found
-                    edge = original_stats.all_edges[edge_id]
-                    edge.node1_id = node1_id
-                    edge.node2_id = node2_id
-                    edge.label = edge_label
-
-                    # keep track of edges that were existing and still existing
-                    edge_ids_after_mod.add(edge.edge_id)
-
-                elif not nodes_found:
-                    if not node1_found:
-                        raise NameError(f"Node {node1_id} not found.")
-                    if not node2_found:
-                        raise NameError(f"Node {node2_id} not found.")
-
-                else:  # new / id not existing
-                    edge_init_dict = dict()
-                    edge_init_dict["node1_id"] = node1_id
-                    edge_init_dict["node2_id"] = node2_id
-                    edge_init_dict["label"] = edge_label
-                    edge_init_dict = {key: value for (key, value) in edge_init_dict.items() if value is not None}
-                    self.add_edge(**edge_init_dict)
-
-            # Deleting edges that have been deleted
-            all_bulk_edge_ids = set(list(original_stats.all_edges.keys()))
-            all_deleted_edge_ids = all_bulk_edge_ids.difference(edge_ids_after_mod)
-            for del_edge_id in all_deleted_edge_ids:
-                obj: Edge = original_stats.all_edges[del_edge_id]
-                parent = obj.parent or self
-                parent.remove_edge(del_edge_id)
-
-        elif type == "object_data":  # TODO: Implement management of deeper data - url, description, formatting
-            raise NotImplementedError("This functionality is not yet implemented.")
-
-        # Run Checks
-        self.run_graph_rules()
+    def manage_graph_data_in_excel(self, type: Optional[str] = None):
+        """Port graph data into Excel in several formats for easy and bulk creation and management.  Then ports back into python graph structure. Types: "obj_and_hierarchy", "object_data", "relations" """
+        return ExcelManager().bulk_data_management(graph=self, type=type)
 
     def gather_graph_stats(self) -> GraphStats:
         """Creating current Graph Stats for the current graph"""
-        return GraphStats(self)
+        return GraphStats(graph=self)
 
-    def run_graph_rules(self, correct=None):
-        """Check a few graph items that are most likely to fail following manual data management."""
+    def run_graph_rules(self, correct: Optional[str] = None) -> None:
+        """Check a few graph items that are most likely to fail following manual data management.  Correct them automatically or manually."""
         if correct is None:  #  ("auto", "manual")
             correct = "auto"
 
         stats = self.gather_graph_stats()
 
-        def stranded_edges_check(self, graph_stats, correct):
+        def stranded_edges_check(self, graph_stats: GraphStats, correct: str) -> set[Edge]:
             """Check for edges with no longer valid nodes (these will prevent yEd from opening the file).  Correct them automatically or manually."""
             stranded_edges = set()
             for edge_id, edge in graph_stats.all_edges.items():
-                node1_exist = edge.node1 in graph_stats.all_nodes.keys() or edge.node1 in graph_stats.all_groups.keys()
-                node2_exist = edge.node2 in graph_stats.all_nodes.keys() or edge.node2 in graph_stats.all_groups.keys()
-                stranded_edge = not node1_exist or not node2_exist
-                at_least_one_edge = node1_exist or node2_exist
+                node1_exist = edge.node1 in graph_stats.all_objects.values()
+                node2_exist = edge.node2 in graph_stats.all_objects.values()
+                at_least_one_edge = any([node1_exist, node2_exist])
+                stranded_edge = not all([node1_exist, node2_exist])
                 if stranded_edge:
                     stranded_edges.add(edge)
 
             if correct == "auto":
                 for edge in stranded_edges:
-                    edge.parent.remove_edge(edge.edge_id)
+                    edge.parent.remove_edge(edge.id)  # Any further postprocessing needed?
 
             elif correct == "manual":
                 # Excel - run relations and highlight edges with issues?
                 raise NotImplementedError("Manual correction of stranded edges is not yet implemented.")
 
             # offer review or update edges
             return stranded_edges
@@ -1885,20 +2037,19 @@
             message="Please install / add yEd to path.",
         )
     return yed_found_bool
 
 
 def get_yed_pid():
     """Return process id for yEd application or None if not running"""
-    pid = None
-    for process in psutil.process_iter(["name"]):
-        if process.info["name"] == PROGRAM_NAME:
-            pid = process.pid or None
-            break
-    return pid
+    yed_pid = None
+    yed_process = get_yed_process()
+    if yed_process:
+        yed_pid = yed_process.pid
+    return yed_pid
 
 
 def get_yed_process():
     """Return process object for yEd application, if there is one running."""
     process = None
     for process_iter in psutil.process_iter(["name"]):
         if process_iter.info["name"] == PROGRAM_NAME:
@@ -1908,91 +2059,287 @@
 
 
 def is_yed_open() -> bool:
     """Check whether yEd is currently open - windows, linux, os, etc."""
     return get_yed_pid() is not None
 
 
-def _maximize(file=None) -> None:
-    """Maximize/show the yEd app (for particular file) - if found. Not currently robust."""
+def start_subprocess(command):
+    try:
+        # Start the subprocess
+        process = subprocess.Popen(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+        pid = process.pid
+        # print(f"Started process with PID: {pid}")
+        return process
+    except Exception as e:
+        print(f"Unexpected error: {e}", file=sys.stderr)
+    return None
 
-    window = get_yed_graph_window_id(file)
 
-    if window:
-        window.activate()
-        window.show()
-        window.maximize()
-
-
-def get_yed_graph_window_id(file: File | None):
-    """Retrieve handle of yEd window containing file"""
-    APP_NAME = "yEd"
-    window = None
-    if not file:
-        potential_windows = [title.lower for title in gw.getAllTitles()]
-        search_name = [title for title in potential_windows if title.endswith(APP_NAME)][0]
-    else:
-        search_name = file.window_search_name
-
-    if search_name:
-        window = gw.getWindowsWithTitle(search_name)  # FIXME: gives false positive w files of same name / diff path.
-    return window[0] if window else None
+def open_yed_file(file: File, force=False):
+    """Opens yed file - also will start yed if not open. Returns process or None."""
+    if not file.file_exists:
+        return None
 
+    if force:
+        if show_guis:
+            print("Act on yEd message box...")
+            answer = msg.askokcancel(title="Force yEd App Close", message="Are you ok to force yEd closure?")
+            if not answer:
+                print("Exiting program")
+                exit()
 
-def is_yed_graph_open(file: File) -> bool:
-    """Check whether yEd is currently open with particular file - windows, linux, os, etc."""
-    window = get_yed_graph_window_id(file)
-    return window is not None
+        kill_yed()
 
+    os.startfile(file.fullpath)
 
-def open_yed_file(file: File, force=False) -> None:
-    """Opens yed file - also will start yed if not open."""
     if force:
-        answer = msg.askokcancel(title="Force yEd App Close", message="Are you ok to force yEd closure?")
-        if not answer:
-            print("Exiting program")
-            exit()
-        process = get_yed_process()
-        if process:
-            process.kill()
-    if not is_yed_graph_open(file):
-        if platform.system() == "Darwin":  # macOS
-            subprocess.call(("open", file.fullpath))
-        elif platform.system() == "Windows":  # Windows
+        sleep(4)
+        if get_yed_pid() is None:
             os.startfile(file.fullpath)
-        else:  # linux variants
-            subprocess.call(("xdg-open", file.fullpath))
 
-        _maximize(file)  # FIXME: Likely not effective
+    return get_yed_process()
+
 
+def start_yed(wait=False):
+    """Starts yEd program (if installed and on path and not already open). Returns process or None.
 
-def start_yed() -> None:
-    """Starts yEd program (if installed and on path and not already open)."""
+    Wait - if True, will wait for yEd to close before returning.
+    """
+    process = None
     if is_yed_findable():
         if not is_yed_open():
-            subprocess.run(PROGRAM_NAME)
+            if wait is False:
+                command = [
+                    PROGRAM_NAME,
+                ]
+                process = start_subprocess(command)
+
+                return process or None
+            else:
+                subprocess.run(PROGRAM_NAME)
+                return None
+
+
+def kill_yed() -> None:
+    """Ends yEd program (if installed and on path and open)."""
+    yed_process = get_yed_process()
+    if yed_process:
+        yed_process.kill()
 
 
 # Utilities =======================================
 def xml_to_simple_string(file_path) -> str:
     """Takes GraphML xml in string format and reduces complexity of the string for simpler parsing (without loss of any significant information).  Returns simplified string."""
+    graph_str = ""
     try:
         with open(file_path, "r") as graph_file:
             graph_str = graph_file.read()
 
-    except Exception as E:
-        print(f"Error: {E}")
-
+    except FileNotFoundError:
+        print(f"Error, file not found: {file_path}")
+        raise FileNotFoundError(f"Error, file not found: {file_path}")
     else:
         # Preprocessing of file for ease of parsing
         graph_str = graph_str.replace("\n", " ")  # line returns
         graph_str = graph_str.replace("\r", " ")  # line returns
         graph_str = graph_str.replace("\t", " ")  # tabs
         graph_str = re.sub("<graphml .*?>", "<graphml>", graph_str)  # unneeded schema
         graph_str = graph_str.replace("> <", "><")  # empty text
         graph_str = graph_str.replace("y:", "")  # unneeded namespace prefix
         graph_str = graph_str.replace("xml:", "")  # unneeded namespace prefix
         graph_str = graph_str.replace("yfiles.", "")  # unneeded namespace prefix
         graph_str = re.sub(" {1,}", " ", graph_str)  # reducing redundant spaces
-        # print(graph_str) # debug
 
     return graph_str
+
+
+def generate_temp_uuid() -> str:
+    """Temporary unique id for objects."""
+    return str(randint(1, 1000000))
+
+
+def assign_traceable_id(obj) -> None:
+    """Creating unique traceable id for graph objects in similar format to yEd:
+    n0, n1, ... for nodes and groups at a level
+    e0, e1, ... for edges at a level
+    n2::n2::n0 for nodes and groups at following level - full tracability
+    n2::e0 for edges at following level - full tracability (lowest level ownership where linked)
+    """
+    parent_id_prefix = ""
+    if isinstance(obj.parent, Group):
+        parent_id_prefix = obj.parent.id + "::"
+
+    if isinstance(obj, Node) or isinstance(obj, Group):
+        obj.id = (
+            parent_id_prefix + "n" + str(len(obj.parent.combined_objects))
+        )  # FIXME: HAS TO BE THE INDEX OF THIS ITEM IN THE LIST
+    elif isinstance(obj, Edge):
+        obj.id = (
+            parent_id_prefix + "e" + str(len(obj.parent.edges))
+        )  # FIXME: HAS TO BE THE INDEX OF THIS ITEM IN THE LIST
+
+
+def update_traceability(obj, owner, operation, heal=True) -> None:
+    """Updating ownership of object based on parent."""
+
+    if operation == "add":
+        # Setting parent
+        obj.parent = owner
+        if isinstance(obj.parent, Group):
+            obj.top_level_graph = obj.parent.top_level_graph
+        else:
+            obj.top_level_graph = obj.parent
+
+        assign_traceable_id(obj)
+
+        if isinstance(obj, Node):
+            obj.parent.nodes[obj.id] = obj
+            obj.parent.combined_objects[obj.id] = obj
+        elif isinstance(obj, Group):
+            obj.parent.groups[obj.id] = obj
+            obj.parent.combined_objects[obj.id] = obj
+        elif isinstance(obj, Edge):
+            obj.parent.edges[obj.id] = obj
+
+    if operation == "remove":
+        if isinstance(obj, Node):
+            del obj.parent.nodes[obj.id]
+            del obj.parent.combined_objects[obj.id]
+
+        elif isinstance(obj, Group):
+            # reroute dependents ===================
+            if heal:
+                for node in obj.nodes.values():
+                    node.parent = obj.parent  # reassign parent: node side
+                    obj.parent.nodes[node.id] = node  # reassign parent: group side
+
+                for edge in obj.edges.values():
+                    edge.parent = obj.parent  # reassign parent: edge side
+                    obj.parent.edges[edge.id] = edge  # reassign parent: group/graph side
+
+                for group in obj.groups.values():
+                    group.parent = obj.parent
+                    obj.parent.groups[group.id] = group  # reassign parent: group side
+
+            del obj.parent.groups[obj.id]
+            del obj.parent.combined_objects[obj.id]
+
+        elif isinstance(obj, Edge):
+            del obj.parent.edges[obj.id]
+
+
+# Reused graph functionality ============================
+def add_node(owner, node, **kwargs) -> Node:
+    """Adding node within Graph - accepts node object (simply assigns), or node name or none (to create new node)."""
+    if isinstance(node, Node):
+        # just update traceability - ownership
+        pass
+    if isinstance(node, str) or node is None:
+        if node:
+            kwargs["name"] = node
+        node = Node(**kwargs)
+    update_traceability(obj=node, owner=owner, operation="add")
+    return node
+
+
+def add_edge(owner: Union[(Graph, Group)], **kwargs) -> Edge:
+    """Adding edge to graph -
+    if node1/node2 names provided - creates nodes under the owner,
+    otherwise, expects node / group objects at or under this owner level.
+    Alternatively, can pass in an instantiated Edge object for ownership update."""
+
+    edge = kwargs.get("edge", None)
+
+    # If an edge is not passed in, create one
+    if not edge:
+        node1 = kwargs.get("node1", None)
+        node2 = kwargs.get("node2", None)
+
+        # Creating nodes if necessary from names - under owner
+        if isinstance(node1, str):
+            node1 = owner.add_node(node1)
+            kwargs["node1"] = node1
+
+        if isinstance(node2, str):
+            node2 = owner.add_node(node2)
+            kwargs["node2"] = node2
+
+        # If not valid object, like None, should error out
+        if not isinstance(node1, (Node, Group)):
+            raise RuntimeWarning(f"Object {node1} doesn't exist")
+
+        if not isinstance(node2, (Node, Group)):
+            raise RuntimeWarning(f"Object {node2} doesn't exist")
+
+        # http://graphml.graphdrawing.org/primer/graphml-primer.html#Nested
+        # The edges between two nodes in a nested graph have to be declared in a graph,
+        # which is an ancestor of both nodes in the hierarchy.
+
+        if isinstance(owner, Group):
+            if not (owner.is_ancestor(node1) and owner.is_ancestor(node2)):
+                raise RuntimeWarning("Group %s is not ancestor of both %s and %s" % (owner.id, node1.id, node2.id))
+
+        edge = Edge(**kwargs)
+
+    # If an edge is passed in, continue on to traceability update
+    else:
+        pass
+
+    update_traceability(obj=edge, owner=owner, operation="add")
+
+    return edge
+
+
+def add_group(owner, group, **kwargs) -> Group:
+    """Adding group to graph"""
+    if isinstance(group, Group):
+        # just needs update to traceability - ownership
+        pass
+    if isinstance(group, str) or group is None:
+        # if isinstance(owner, Group):
+        #     top_level_graph = owner.top_level_graph
+        # else:
+        #     top_level_graph = owner
+        if group:
+            kwargs["name"] = group
+        group = Group(**kwargs)
+    heal: bool = kwargs.get("heal", True)
+    update_traceability(obj=group, owner=owner, operation="add", heal=heal)
+    return group
+
+
+def remove_node(owner, node) -> None:
+    """Remove/Delete a node - accepts node or node id"""
+    if isinstance(node, Node):
+        if node not in owner.nodes.values():
+            raise RuntimeWarning(f"Node {node.id} doesn't exist")
+    if isinstance(node, str):
+        if node not in owner.nodes:
+            raise RuntimeWarning(f"Node {node} doesn't exist")
+        node = owner.nodes[node]
+    update_traceability(obj=node, owner=owner, operation="remove")
+
+
+def remove_group(owner, group) -> None:
+    """Removes a group from within current object."""
+    if isinstance(group, Group):
+        if group not in owner.groups.values():
+            raise RuntimeWarning(f"Group {group.id} doesn't exist")
+    if isinstance(group, str):
+        if group not in owner.groups:
+            raise RuntimeWarning(f"Group {group} doesn't exist")
+        group = owner.groups[group]
+
+    update_traceability(obj=group, owner=owner, operation="remove")
+
+
+def remove_edge(owner, edge) -> None:
+    """Removing edge - uses id."""
+    if isinstance(edge, Edge):
+        if edge not in owner.edges.values():
+            raise RuntimeWarning(f"Edge {edge.id} doesn't exist")
+    if isinstance(edge, str):
+        if edge not in owner.edges:
+            raise RuntimeWarning(f"Edge {edge} doesn't exist")
+        edge = owner.edges[edge]
+    update_traceability(obj=edge, owner=owner, operation="remove")
```

### Comparing `yedextended-1.0.9/src/yedextended.egg-info/PKG-INFO` & `yedextended-2.0.0a0/src/yedextended.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 Metadata-Version: 2.1
 Name: yedextended
-Version: 1.0.9
+Version: 2.0.0a0
 Summary: Python library extending yEd functionality through programmatic interface to graphs.
 Author-email: Cole St John <info@colestjohn.com>
 Project-URL: Homepage, https://github.com/cole-st-john/yedextended
 Project-URL: Issues, https://github.com/cole-st-john/yedextended/issues
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: psutil
-Requires-Dist: pygetwindow
 Requires-Dist: openpyxl
 
 
 
 
 # Extended Python Support for yEd 
+
+[![Static Badge](https://img.shields.io/badge/PyPI%20-%20yEdExtended%20-%20GREEN?logoColor=0%2C0%2C255&color=0%2C1%2C1&link=https%3A%2F%2Fpypi.org%2Fproject%2Fyedextended%2F)](https://pypi.org/project/yedextended/)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/yedextended?color=2334D058)
 [![CI](https://github.com/cole-st-john/yEdExtended/actions/workflows/ci.yml/badge.svg)](https://github.com/cole-st-john/yEdExtended/actions/workflows/ci.yml)
 ![Test Coverage](https://raw.githubusercontent.com/cole-st-john/yedextended/master/test_coverage.svg)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/yedextended?color=2334D058)
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/w/cole-st-john/yedextended)
-<!-- ![PyPI - Downloads](https://img.shields.io/pypi/dm/yedextended?labelColor=2334D058) -->
+![PyPI - Downloads](https://img.shields.io/pypi/dm/yedextended)
 
 This Python library extends the functionality of the readily available and free interactive graph editing program [yEd](http://www.yworks.com/en/products_yed_about.html), through providing a programmatic interface to graphs (of the [GraphML](http://graphml.graphdrawingraph1.org/) file format), including the following use case or functions:
 
 - [x] creating graphs
 - [x] formatting graphs
 - [x] reading graphs
 - [x] bulk data addition or management (MS excel-based)
-- [x] management of the yEd application (starting, killing, maximizing)
+- [x] management of the yEd application (starting, killing, etc.)
 - [ ] enforcing rules on graphs
 - [ ] additional layout methods
 - [ ] graph comparison tools
 
 ![yEd Graph](https://raw.githubusercontent.com/cole-st-john/yedextended/master/images/graph.gif)
 
 
@@ -76,34 +77,35 @@
 With yEdExtended you can easily create graphs, either through hardcoding, or more practically, through porting data from any data source (databases, csv, xml, etc) into a graph and graph objects (nodes, groups, edges, properties):
 
 Hardcoding Example:
 ```python
 # Instantiate graph instance
 graph1 = yed.Graph()
 
-# Add arbitrary graph detail - nodes and edges
-graph1.add_node("a")
-graph1.add_node("b")
-graph1.add_edge("a", "b")
+# Adding arbitrary graph detail - nodes
+a = graph1.add_node("a")
+b = graph1.add_node("b")
+
+# Adding edge (using node objects)
+graph1.add_edge(a, b)
 
 # Add arbitrary graph detail - group and group objects
 group1 = graph1.add_group("group 1", shape="rectangle")
-group1.add_node("c")
-group1.add_node("d")
+
+# Adding edge using node names, under owning group
 group1.add_edge("c", "d")
 ```
 
 Programmatic Example:
 ```python
 # Adding graph objects based on csv input
-import csv
-with open("examples/test.csv", encoding="utf-8-sig") as csv_file: 
-	csv_reader = csv.reader(csv_file)
-	for row in csv_reader:
-	    graph1.add_node(row)
+with open("examples\\test.csv", encoding="utf-8-sig") as csv_file:
+    csv_reader = csv.reader(csv_file)
+    for row in csv_reader:
+        graph1.add_node(row[0])
 ```
 
 ## Reading existing GraphML files
 
 yEdExtended can read GraphML files into a Python class structure, allowing for simple programmatic analysis and modification:
 
 ```python
@@ -115,51 +117,37 @@
 
 ## Using formatting
 
 yEdExtended provides for the majority of formatting one expects in yEd graphs.
 
 ```python
 # Add graph nodes and edges with some examples of non-default formatting
-graph1.add_node(
-    "foo",
-    font_family="Zapfino",
-)
+graph1.add_node("foo", font_family="Zapfino")
 
 graph1.add_node(
     "foo2",
     shape="roundrectangle",
     font_style="bolditalic",
     underlined_text="true",
 )
 
-graph1.add_edge(
-    "foo1",
-    "foo2",
-)
-graph1.add_node(
-    "abc",
-    font_size="72",
-    height="100",
-)
+graph1.add_edge("foo1", "foo2")
 
-graph1.add_node(
-    "bar",
-    label="Multi\nline\ntext",
-)
-graph1.add_node(
-    "foobar",
-    label="""Multi
+graph1.add_node("abc", font_size="72", height="100")
+
+graph1.add_node("Multi\nline\ntext")
+
+graph1.add_node("foobar").add_label("""Multi
 Line
-Text!""",
-)
+Text!""")
 
 graph1.add_edge(
     "foo",
     "foo1",
-    label="EDGE!",
+    name="EDGE!",
     width="3.0",
     color="#0000FF",
     arrowhead="white_diamond",
     arrowfoot="standard",
     line_type="dotted",
 )
 ```
@@ -245,18 +233,27 @@
 
 # Development
 
 
 Interested in contributing or co-managing further development?  Just reach out!
 
 Dev. Requirements:
+
+Install yEd from [here](https://www.yworks.com/products/yed/download#download).
+
+Ensure you have [MS Excel](https://www.microsoft.com/en/microsoft-365/excel?market=af) installed.
+
 ```console
 $ pip install pytest
 ```
 
+```console
+$ setx CI "True"
+```
+
 To run the tests:
 ```console
 $ PYTHONPATH=. pytest tests
 ```
 
 References:
```

### Comparing `yedextended-1.0.9/src/yedextended.egg-info/SOURCES.txt` & `yedextended-2.0.0a0/src/yedextended.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,44 @@
 .deepsource.toml
 .gitignore
 LICENSE
 README.md
+ci.bat
+coverage_sticker.bat
 pyproject.toml
-requirements.txt
+requirements.dev.txt
+run_tests_simple.bat
 test_coverage.svg
 .github/workflows/ci.yml
+.github/workflows/ci.yml.bak
 .github/workflows/python-publish.yml
 examples/demo-basic-create-and-open.py
 examples/demo-basic-formatting.py
 examples/demo-basic_bulk_manage1.py
 examples/demo-basic_bulk_manage2.py
 examples/demo-custom-properties-nodes-edges.py
 examples/demo-multilabels.py
 examples/demo-round-robin_read_store.py
+examples/demo-some-props.py
 examples/demo-uml.py
 examples/demo-url-description-groups-nodes-edges.py
 examples/readme-1.py
 examples/readme-2.py
 examples/readme-3.py
 examples/test.csv
 examples/test.graphml
 examples/yed_created_edges.graphml
+examples/yed_created_edges_deeper.graphml
+examples/yed_created_edges_obj.graphml
+examples/yed_created_edges_simplified.graphml
+examples/yed_created_empty_graph.graphml
 examples/yed_modified_app_created.graphml
+examples/yed_test_to_excel1.xlsx
+examples/yed_test_to_excel2.xlsx
+examples/yed_test_to_excel3.xlsx
 images/demo_multilabel.png
 images/example-UML.png
 images/example.png
 images/excel_obj_entry.gif
 images/excel_rel_entry.gif
 images/graph.gif
 images/graph_from_excel_obj.gif
```

### Comparing `yedextended-1.0.9/test_coverage.svg` & `yedextended-2.0.0a0/test_coverage.svg`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 00000150: 2233 2220 6669 6c6c 3d22 2366 6666 222f  "3" fill="#fff"/
 00000160: 3e0a 2020 2020 3c2f 6d61 736b 3e0a 2020  >.    </mask>.  
 00000170: 2020 3c67 206d 6173 6b3d 2275 726c 2823    <g mask="url(#
 00000180: 6129 223e 0a20 2020 2020 2020 203c 7061  a)">.        <pa
 00000190: 7468 2066 696c 6c3d 2223 3535 3522 2064  th fill="#555" d
 000001a0: 3d22 4d30 2030 6836 3376 3230 4830 7a22  ="M0 0h63v20H0z"
 000001b0: 2f3e 0a20 2020 2020 2020 203c 7061 7468  />.        <path
-000001c0: 2066 696c 6c3d 2223 6530 3564 3434 2220   fill="#e05d44" 
+000001c0: 2066 696c 6c3d 2223 6134 6136 3164 2220   fill="#a4a61d" 
 000001d0: 643d 224d 3633 2030 6833 3676 3230 4836  d="M63 0h36v20H6
 000001e0: 337a 222f 3e0a 2020 2020 2020 2020 3c70  3z"/>.        <p
 000001f0: 6174 6820 6669 6c6c 3d22 7572 6c28 2362  ath fill="url(#b
 00000200: 2922 2064 3d22 4d30 2030 6839 3976 3230  )" d="M0 0h99v20
 00000210: 4830 7a22 2f3e 0a20 2020 203c 2f67 3e0a  H0z"/>.    </g>.
 00000220: 2020 2020 3c67 2066 696c 6c3d 2223 6666      <g fill="#ff
 00000230: 6622 2074 6578 742d 616e 6368 6f72 3d22  f" text-anchor="
@@ -46,12 +46,12 @@
 000002d0: 6167 653c 2f74 6578 743e 0a20 2020 2020  age</text>.     
 000002e0: 2020 203c 7465 7874 2078 3d22 3331 2e35     <text x="31.5
 000002f0: 2220 793d 2231 3422 3e63 6f76 6572 6167  " y="14">coverag
 00000300: 653c 2f74 6578 743e 0a20 2020 2020 2020  e</text>.       
 00000310: 203c 7465 7874 2078 3d22 3830 2220 793d   <text x="80" y=
 00000320: 2231 3522 2066 696c 6c3d 2223 3031 3031  "15" fill="#0101
 00000330: 3031 2220 6669 6c6c 2d6f 7061 6369 7479  01" fill-opacity
-00000340: 3d22 2e33 223e 3336 253c 2f74 6578 743e  =".3">36%</text>
+00000340: 3d22 2e33 223e 3835 253c 2f74 6578 743e  =".3">85%</text>
 00000350: 0a20 2020 2020 2020 203c 7465 7874 2078  .        <text x
-00000360: 3d22 3830 2220 793d 2231 3422 3e33 3625  ="80" y="14">36%
+00000360: 3d22 3830 2220 793d 2231 3422 3e38 3525  ="80" y="14">85%
 00000370: 3c2f 7465 7874 3e0a 2020 2020 3c2f 673e  </text>.    </g>
 00000380: 0a3c 2f73 7667 3e0a                      .</svg>.
```

