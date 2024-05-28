# Comparing `tmp/scrnaseq-0.0.1.tar.gz` & `tmp/scrnaseq-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrnaseq-0.0.1.tar", last modified: Mon May 20 03:14:47 2024, max compression
+gzip compressed data, was "scrnaseq-0.1.0.tar", last modified: Tue May 28 03:01:06 2024, max compression
```

## Comparing `scrnaseq-0.0.1.tar` & `scrnaseq-0.1.0.tar`

### file list

```diff
@@ -1,44 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 03:14:47.070940 scrnaseq-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-20 03:13:44.000000 scrnaseq-0.0.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 03:14:47.058940 scrnaseq-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 03:14:47.062940 scrnaseq-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-20 03:13:44.000000 scrnaseq-0.0.1/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-20 03:13:44.000000 scrnaseq-0.0.1/.github/workflows/pypi-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-20 03:13:44.000000 scrnaseq-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-20 03:13:44.000000 scrnaseq-0.0.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-20 03:13:44.000000 scrnaseq-0.0.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-20 03:13:44.000000 scrnaseq-0.0.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    13490 2024-05-20 03:13:44.000000 scrnaseq-0.0.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-20 03:13:44.000000 scrnaseq-0.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-05-20 03:14:47.070940 scrnaseq-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-20 03:13:44.000000 scrnaseq-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 03:14:47.066940 scrnaseq-0.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-20 03:13:44.000000 scrnaseq-0.0.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 03:14:47.066940 scrnaseq-0.0.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-20 03:13:44.000000 scrnaseq-0.0.1/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-20 03:13:44.000000 scrnaseq-0.0.1/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-20 03:13:44.000000 scrnaseq-0.0.1/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)    10039 2024-05-20 03:13:44.000000 scrnaseq-0.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-20 03:13:44.000000 scrnaseq-0.0.1/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-20 03:13:44.000000 scrnaseq-0.0.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-20 03:13:44.000000 scrnaseq-0.0.1/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-20 03:13:44.000000 scrnaseq-0.0.1/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-20 03:13:44.000000 scrnaseq-0.0.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-20 03:13:44.000000 scrnaseq-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-20 03:14:47.070940 scrnaseq-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-20 03:13:44.000000 scrnaseq-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 03:14:47.062940 scrnaseq-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 03:14:47.066940 scrnaseq-0.0.1/src/scrnaseq/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-20 03:13:44.000000 scrnaseq-0.0.1/src/scrnaseq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-05-20 03:13:44.000000 scrnaseq-0.0.1/src/scrnaseq/fetch_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 03:14:47.066940 scrnaseq-0.0.1/src/scrnaseq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-05-20 03:14:47.000000 scrnaseq-0.0.1/src/scrnaseq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-20 03:14:47.000000 scrnaseq-0.0.1/src/scrnaseq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 03:14:47.000000 scrnaseq-0.0.1/src/scrnaseq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 03:14:46.000000 scrnaseq-0.0.1/src/scrnaseq.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-20 03:14:47.000000 scrnaseq-0.0.1/src/scrnaseq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-20 03:14:47.000000 scrnaseq-0.0.1/src/scrnaseq.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 03:14:47.066940 scrnaseq-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-20 03:13:44.000000 scrnaseq-0.0.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-20 03:13:44.000000 scrnaseq-0.0.1/tests/test_fetch_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-05-20 03:13:44.000000 scrnaseq-0.0.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 03:01:06.758494 scrnaseq-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-28 02:55:53.000000 scrnaseq-0.1.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 03:01:06.746493 scrnaseq-0.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 03:01:06.750493 scrnaseq-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-05-28 02:55:53.000000 scrnaseq-0.1.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-28 02:55:53.000000 scrnaseq-0.1.0/.github/workflows/pypi-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-28 02:55:53.000000 scrnaseq-0.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-28 02:55:53.000000 scrnaseq-0.1.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-28 02:55:53.000000 scrnaseq-0.1.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-28 02:55:53.000000 scrnaseq-0.1.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13490 2024-05-28 02:55:53.000000 scrnaseq-0.1.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-28 02:55:53.000000 scrnaseq-0.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10434 2024-05-28 03:01:06.758494 scrnaseq-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9309 2024-05-28 02:55:53.000000 scrnaseq-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 03:01:06.750493 scrnaseq-0.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-28 02:55:53.000000 scrnaseq-0.1.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 03:01:06.750493 scrnaseq-0.1.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-28 02:55:53.000000 scrnaseq-0.1.0/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-28 02:55:53.000000 scrnaseq-0.1.0/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-28 02:55:53.000000 scrnaseq-0.1.0/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10838 2024-05-28 02:55:53.000000 scrnaseq-0.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-28 02:55:53.000000 scrnaseq-0.1.0/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-28 02:55:53.000000 scrnaseq-0.1.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-28 02:55:53.000000 scrnaseq-0.1.0/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-28 02:55:53.000000 scrnaseq-0.1.0/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-28 02:55:53.000000 scrnaseq-0.1.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-28 02:55:53.000000 scrnaseq-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-28 03:01:06.758494 scrnaseq-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-28 02:55:53.000000 scrnaseq-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 03:01:06.746493 scrnaseq-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 03:01:06.754494 scrnaseq-0.1.0/src/scrnaseq/
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-28 02:55:53.000000 scrnaseq-0.1.0/src/scrnaseq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-05-28 02:55:53.000000 scrnaseq-0.1.0/src/scrnaseq/fetch_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6075 2024-05-28 02:55:53.000000 scrnaseq-0.1.0/src/scrnaseq/list_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-28 02:55:53.000000 scrnaseq-0.1.0/src/scrnaseq/list_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-05-28 02:55:53.000000 scrnaseq-0.1.0/src/scrnaseq/polish_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-05-28 02:55:53.000000 scrnaseq-0.1.0/src/scrnaseq/save_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-05-28 02:55:53.000000 scrnaseq-0.1.0/src/scrnaseq/search_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-05-28 02:55:53.000000 scrnaseq-0.1.0/src/scrnaseq/upload_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-05-28 02:55:53.000000 scrnaseq-0.1.0/src/scrnaseq/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 03:01:06.754494 scrnaseq-0.1.0/src/scrnaseq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10434 2024-05-28 03:01:06.000000 scrnaseq-0.1.0/src/scrnaseq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-28 03:01:06.000000 scrnaseq-0.1.0/src/scrnaseq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 03:01:06.000000 scrnaseq-0.1.0/src/scrnaseq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 03:01:06.000000 scrnaseq-0.1.0/src/scrnaseq.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-28 03:01:06.000000 scrnaseq-0.1.0/src/scrnaseq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-28 03:01:06.000000 scrnaseq-0.1.0/src/scrnaseq.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 03:01:06.754494 scrnaseq-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-28 02:55:53.000000 scrnaseq-0.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-28 02:55:53.000000 scrnaseq-0.1.0/tests/test_fetch_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-28 02:55:53.000000 scrnaseq-0.1.0/tests/test_list_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-28 02:55:53.000000 scrnaseq-0.1.0/tests/test_list_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5786 2024-05-28 02:55:53.000000 scrnaseq-0.1.0/tests/test_polish_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-28 02:55:53.000000 scrnaseq-0.1.0/tests/test_save_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-28 02:55:53.000000 scrnaseq-0.1.0/tests/test_search_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-05-28 02:55:53.000000 scrnaseq-0.1.0/tests/test_upload_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-05-28 02:55:53.000000 scrnaseq-0.1.0/tox.ini
```

### Comparing `scrnaseq-0.0.1/.coveragerc` & `scrnaseq-0.1.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `scrnaseq-0.0.1/.github/workflows/pypi-publish.yml` & `scrnaseq-0.1.0/.github/workflows/pypi-publish.yml`

 * *Files 23% similar despite different names*

```diff
@@ -5,47 +5,76 @@
 
 on:
   push:
     tags: "*"
 
 jobs:
   build:
-
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v2
-    - name: Set up Python 3.9
-      uses: actions/setup-python@v2
-      with:
-        python-version: 3.9
-    - name: Install dependencies
-      run: |
-        python -m pip install --upgrade pip
-        pip install flake8 pytest tox
-    # - name: Lint with flake8
-    #   run: |
-    #     # stop the build if there are Python syntax errors or undefined names
-    #     flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
-    #     # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
-    #     # flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
-    - name: Test with tox
-      run: |
-        tox
-    - name: Build docs
-      run: |
-        tox -e docs
-    - run: touch ./docs/_build/html/.nojekyll
-    - name: GH Pages Deployment
-      uses: JamesIves/github-pages-deploy-action@4.1.3
-      with:
-        branch: gh-pages # The branch the action should deploy to.
-        folder: ./docs/_build/html
-        clean: true # Automatically remove deleted files from the deploy branch
-    - name: Build Project and Publish
-      run: |
-        python -m tox -e clean,build
-    - name: Publish package
-      uses: pypa/gh-action-pypi-publish@27b31702a0e7fc50959f5ad993c78deac1bdfc29
-      with:
-        user: __token__
-        password: ${{ secrets.PYPI_PASSWORD }}
+      - uses: actions/checkout@v2
+
+      - name: Set up Python 3.9
+        uses: actions/setup-python@v2
+        with:
+          python-version: 3.9
+
+      # build SQLite from source, because I need 3.35<=
+      - name: Download SQLite3
+        run: |
+          wget https://www.sqlite.org/2024/sqlite-autoconf-3450300.tar.gz
+          tar -xvf sqlite-autoconf-3450300.tar.gz
+
+      - name: Install SQLite3
+        run: |
+          ./configure
+          make
+          sudo make install
+          export PATH="/usr/local/lib:$PATH"
+        working-directory: sqlite-autoconf-3450300
+
+      - name: Install dependencies
+        run: |
+          python -m pip install --upgrade pip
+          pip install flake8 pytest tox
+        env:
+          LD_LIBRARY_PATH: /usr/local/lib
+      # - name: Lint with flake8
+      #   run: |
+      #     # stop the build if there are Python syntax errors or undefined names
+      #     flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
+      #     # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
+      #     # flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
+
+      - name: Test with tox
+        run: |
+          tox
+        env:
+          LD_LIBRARY_PATH: /usr/local/lib
+
+      - name: Build docs
+        run: |
+          tox -e docs
+        env:
+          LD_LIBRARY_PATH: /usr/local/lib
+
+      - run: touch ./docs/_build/html/.nojekyll
+
+      - name: GH Pages Deployment
+        uses: JamesIves/github-pages-deploy-action@4.1.3
+        with:
+          branch: gh-pages # The branch the action should deploy to.
+          folder: ./docs/_build/html
+          clean: true # Automatically remove deleted files from the deploy branch
+
+      - name: Build Project and Publish
+        run: |
+          python -m tox -e clean,build
+        env:
+          LD_LIBRARY_PATH: /usr/local/lib
+
+      - name: Publish package
+        uses: pypa/gh-action-pypi-publish@27b31702a0e7fc50959f5ad993c78deac1bdfc29
+        with:
+          user: __token__
+          password: ${{ secrets.PYPI_PASSWORD }}
```

### Comparing `scrnaseq-0.0.1/.gitignore` & `scrnaseq-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `scrnaseq-0.0.1/.readthedocs.yml` & `scrnaseq-0.1.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `scrnaseq-0.0.1/CONTRIBUTING.md` & `scrnaseq-0.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `scrnaseq-0.0.1/LICENSE.txt` & `scrnaseq-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scrnaseq-0.0.1/docs/Makefile` & `scrnaseq-0.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `scrnaseq-0.0.1/docs/conf.py` & `scrnaseq-0.1.0/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -167,15 +167,15 @@
 todo_emit_warnings = True
 
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
-html_theme = "alabaster"
+html_theme = "furo"
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 html_theme_options = {
     "sidebar_width": "300px",
     "page_width": "1200px"
@@ -245,14 +245,24 @@
 
 # This is the file name suffix for HTML files (e.g. ".xhtml").
 # html_file_suffix = None
 
 # Output file base name for HTML help builder.
 htmlhelp_basename = "scrnaseq-doc"
 
+autodoc_default_options = {
+    # 'members': 'var1, var2',
+    # 'member-order': 'bysource',
+    "special-members": True,
+    "undoc-members": True,
+    "exclude-members": "__weakref__, __dict__, __str__, __module__",
+}
+
+autosummary_generate = True
+autosummary_imported_members = True
 
 # -- Options for LaTeX output ------------------------------------------------
 
 latex_elements = {
     # The paper size ("letterpaper" or "a4paper").
     # "papersize": "letterpaper",
     # The font size ("10pt", "11pt" or "12pt").
@@ -295,10 +305,17 @@
     "matplotlib": ("https://matplotlib.org", None),
     "numpy": ("https://numpy.org/doc/stable", None),
     "sklearn": ("https://scikit-learn.org/stable", None),
     "pandas": ("https://pandas.pydata.org/pandas-docs/stable", None),
     "scipy": ("https://docs.scipy.org/doc/scipy/reference", None),
     "setuptools": ("https://setuptools.pypa.io/en/stable/", None),
     "pyscaffold": ("https://pyscaffold.org/en/stable", None),
+    "biocframe": ("https://biocpy.github.io/BiocFrame", None),
+    "genomicranges": ("https://biocpy.github.io/GenomicRanges", None),
+    "singlecellexperiment": ("https://biocpy.github.io/SingleCellExperiment", None),
+    "summarizedexperiment": ("https://biocpy.github.io/SummarizedExperiment", None),
+    "gypsum_client": ("https://artifactdb.github.io/gypsum-py", None),
+    "delayedarray": ("https://biocpy.github.io/DelayedArray", None),
+    "dolomite_base": ("https://artifactdb.github.io/dolomite-base", None),
 }
 
 print(f"loading configurations for {project} {version} ...", file=sys.stderr)
```

### Comparing `scrnaseq-0.0.1/setup.cfg` & `scrnaseq-0.1.0/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -21,30 +21,35 @@
 include_package_data = True
 package_dir = 
 	=src
 install_requires = 
 	importlib-metadata; python_version<"3.8"
 	dolomite_base
 	dolomite_matrix
-	dolomite_sce
-	gypsum_client>=0.1.1
-	delayedarray
+	dolomite_sce>=0.1.2
+	gypsum_client>=0.1.3
+	delayedarray>=0.5.1
 	summarizedexperiment
 	singlecellexperiment
+	pandas
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [options.extras_require]
+optional = 
+	anndata
 testing = 
 	setuptools
 	pytest
 	pytest-cov
+	scipy
+	anndata
 
 [options.entry_points]
 
 [tool:pytest]
 addopts = 
 	--cov scrnaseq --cov-report term-missing
 	--verbose
```

### Comparing `scrnaseq-0.0.1/setup.py` & `scrnaseq-0.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `scrnaseq-0.0.1/src/scrnaseq.egg-info/SOURCES.txt` & `scrnaseq-0.1.0/src/scrnaseq.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -20,15 +20,28 @@
 docs/index.md
 docs/license.md
 docs/readme.md
 docs/requirements.txt
 docs/_static/.gitignore
 src/scrnaseq/__init__.py
 src/scrnaseq/fetch_dataset.py
+src/scrnaseq/list_datasets.py
+src/scrnaseq/list_versions.py
+src/scrnaseq/polish_dataset.py
+src/scrnaseq/save_dataset.py
+src/scrnaseq/search_datasets.py
+src/scrnaseq/upload_dataset.py
+src/scrnaseq/utils.py
 src/scrnaseq.egg-info/PKG-INFO
 src/scrnaseq.egg-info/SOURCES.txt
 src/scrnaseq.egg-info/dependency_links.txt
 src/scrnaseq.egg-info/not-zip-safe
 src/scrnaseq.egg-info/requires.txt
 src/scrnaseq.egg-info/top_level.txt
 tests/conftest.py
-tests/test_fetch_dataset.py
+tests/test_fetch_dataset.py
+tests/test_list_dataset.py
+tests/test_list_version.py
+tests/test_polish_dataset.py
+tests/test_save_dataset.py
+tests/test_search_datasets.py
+tests/test_upload_dataset.py
```

### Comparing `scrnaseq-0.0.1/tox.ini` & `scrnaseq-0.1.0/tox.ini`

 * *Files identical despite different names*

