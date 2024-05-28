# Comparing `tmp/python_cmethods-2.2.4.tar.gz` & `tmp/python_cmethods-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_cmethods-2.2.4.tar", last modified: Mon May 20 08:48:08 2024, max compression
+gzip compressed data, was "python_cmethods-2.2.5.tar", last modified: Tue May 28 03:53:55 2024, max compression
```

## Comparing `python_cmethods-2.2.4.tar` & `python_cmethods-2.2.5.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:48:08.209335 python_cmethods-2.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:48:08.201335 python_cmethods-2.2.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:48:08.201335 python_cmethods-2.2.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/.github/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/.github/dependabot.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:48:08.201335 python_cmethods-2.2.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/.github/workflows/_build.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/.github/workflows/_build_doc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/.github/workflows/_codecov.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/.github/workflows/_codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/.github/workflows/_pre_commit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/.github/workflows/_pypi_publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/.github/workflows/_pypi_test_publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/.github/workflows/_test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/.github/workflows/cicd.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/.github/workflows/dependabot_auto_approve.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/.github/workflows/scorecard.yml
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13733 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    32891 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    54246 2024-05-20 08:48:08.209335 python_cmethods-2.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14083 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:48:08.205335 python_cmethods-2.2.4/cmethods/
--rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/cmethods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-20 08:48:08.000000 python_cmethods-2.2.4/cmethods/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6683 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/cmethods/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     8989 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/cmethods/distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     4688 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/cmethods/scaling.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/cmethods/static.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/cmethods/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     7360 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/cmethods/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7502 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:48:08.205335 python_cmethods-2.2.4/python_cmethods.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    54246 2024-05-20 08:48:08.000000 python_cmethods-2.2.4/python_cmethods.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-20 08:48:08.000000 python_cmethods-2.2.4/python_cmethods.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 08:48:08.000000 python_cmethods-2.2.4/python_cmethods.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-20 08:48:08.000000 python_cmethods-2.2.4/python_cmethods.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-20 08:48:08.000000 python_cmethods-2.2.4/python_cmethods.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-20 08:48:08.000000 python_cmethods-2.2.4/python_cmethods.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 08:48:08.209335 python_cmethods-2.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-20 08:48:01.000000 python_cmethods-2.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 03:53:55.133173 python_cmethods-2.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-28 03:53:48.000000 python_cmethods-2.2.5/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 03:53:55.125172 python_cmethods-2.2.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 03:53:55.125172 python_cmethods-2.2.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-28 03:53:48.000000 python_cmethods-2.2.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-28 03:53:48.000000 python_cmethods-2.2.5/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-28 03:53:48.000000 python_cmethods-2.2.5/.github/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-28 03:53:48.000000 python_cmethods-2.2.5/.github/dependabot.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 03:53:55.129172 python_cmethods-2.2.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-05-28 03:53:48.000000 python_cmethods-2.2.5/.github/workflows/_build.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-28 03:53:48.000000 python_cmethods-2.2.5/.github/workflows/_build_doc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-28 03:53:48.000000 python_cmethods-2.2.5/.github/workflows/_codecov.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-05-28 03:53:48.000000 python_cmethods-2.2.5/.github/workflows/_codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-28 03:53:48.000000 python_cmethods-2.2.5/.github/workflows/_pre_commit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-28 03:53:48.000000 python_cmethods-2.2.5/.github/workflows/_pypi_publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-28 03:53:48.000000 python_cmethods-2.2.5/.github/workflows/_pypi_test_publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-28 03:53:48.000000 python_cmethods-2.2.5/.github/workflows/_test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-28 03:53:48.000000 python_cmethods-2.2.5/.github/workflows/cicd.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-28 03:53:48.000000 python_cmethods-2.2.5/.github/workflows/dependabot_auto_approve.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-28 03:53:48.000000 python_cmethods-2.2.5/.github/workflows/scorecard.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-28 03:53:48.000000 python_cmethods-2.2.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-05-28 03:53:48.000000 python_cmethods-2.2.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-28 03:53:48.000000 python_cmethods-2.2.5/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13733 2024-05-28 03:53:48.000000 python_cmethods-2.2.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    32891 2024-05-28 03:53:48.000000 python_cmethods-2.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-28 03:53:48.000000 python_cmethods-2.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-28 03:53:48.000000 python_cmethods-2.2.5/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    54239 2024-05-28 03:53:55.133173 python_cmethods-2.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14055 2024-05-28 03:53:48.000000 python_cmethods-2.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-28 03:53:48.000000 python_cmethods-2.2.5/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 03:53:55.129172 python_cmethods-2.2.5/cmethods/
+-rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-05-28 03:53:48.000000 python_cmethods-2.2.5/cmethods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-28 03:53:54.000000 python_cmethods-2.2.5/cmethods/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6683 2024-05-28 03:53:48.000000 python_cmethods-2.2.5/cmethods/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8898 2024-05-28 03:53:48.000000 python_cmethods-2.2.5/cmethods/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4688 2024-05-28 03:53:48.000000 python_cmethods-2.2.5/cmethods/scaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-28 03:53:48.000000 python_cmethods-2.2.5/cmethods/static.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-28 03:53:48.000000 python_cmethods-2.2.5/cmethods/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7360 2024-05-28 03:53:48.000000 python_cmethods-2.2.5/cmethods/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7548 2024-05-28 03:53:48.000000 python_cmethods-2.2.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 03:53:55.129172 python_cmethods-2.2.5/python_cmethods.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    54239 2024-05-28 03:53:55.000000 python_cmethods-2.2.5/python_cmethods.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-28 03:53:55.000000 python_cmethods-2.2.5/python_cmethods.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 03:53:55.000000 python_cmethods-2.2.5/python_cmethods.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-28 03:53:55.000000 python_cmethods-2.2.5/python_cmethods.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-28 03:53:55.000000 python_cmethods-2.2.5/python_cmethods.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-28 03:53:55.000000 python_cmethods-2.2.5/python_cmethods.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 03:53:55.133173 python_cmethods-2.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-28 03:53:48.000000 python_cmethods-2.2.5/setup.py
```

### Comparing `python_cmethods-2.2.4/.gitattributes` & `python_cmethods-2.2.5/.gitattributes`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.4/.github/ISSUE_TEMPLATE/bug_report.md` & `python_cmethods-2.2.5/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.4/.github/ISSUE_TEMPLATE/feature_request.md` & `python_cmethods-2.2.5/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.4/.github/codecov.yml` & `python_cmethods-2.2.5/.github/codecov.yml`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.4/.github/workflows/_build.yaml` & `python_cmethods-2.2.5/.github/workflows/_build.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 permissions: read-all
 
 jobs:
   Build:
     runs-on: ${{ inputs.os }}
     steps:
       - name: Checkout repository
-        uses: actions/checkout@44c2b7a8a4ea60a981eaca3cf939b5f4305c123b # v4.1.5
+        uses: actions/checkout@a5ac7e51b41094c92402da3b24376905380afc29 # v4.1.6
         with:
           fetch-depth: 0 # IMPORTANT: otherwise the current tag does not get fetched and the build version gets worse
 
       - name: Set up Python ${{ inputs.python-version }}
         uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d # v5.1.0
         with:
           python-version: ${{ inputs.python-version }}
```

### Comparing `python_cmethods-2.2.4/.github/workflows/_build_doc.yaml` & `python_cmethods-2.2.5/.github/workflows/_build_doc.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 permissions: read-all
 
 jobs:
   Build:
     runs-on: ${{ inputs.os }}
     steps:
       - name: Checkout repository
-        uses: actions/checkout@44c2b7a8a4ea60a981eaca3cf939b5f4305c123b # v4.1.5
+        uses: actions/checkout@a5ac7e51b41094c92402da3b24376905380afc29 # v4.1.6
 
       - name: Set up Python ${{ inputs.python-version }}
         uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d # v5.1.0
         with:
           python-version: ${{ inputs.python-version }}
 
       - name: Install dependencies
```

### Comparing `python_cmethods-2.2.4/.github/workflows/_codecov.yaml` & `python_cmethods-2.2.5/.github/workflows/_codecov.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     runs-on: ${{ inputs.os }}
     env:
       OS: ${{ inputs.os }}
       PYTHON: ${{ inputs.python-version }}
 
     steps:
       - name: Checkout repository
-        uses: actions/checkout@44c2b7a8a4ea60a981eaca3cf939b5f4305c123b # v4.1.5
+        uses: actions/checkout@a5ac7e51b41094c92402da3b24376905380afc29 # v4.1.6
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d # v5.1.0
         with:
           python-version: ${{ inputs.python-version }}
 
       - name: Install dependencies
@@ -47,15 +47,15 @@
       - name: Install package
         run: python -m pip install ".[dev,test]"
 
       - name: Generate coverage report
         run: pytest --cov --cov-report=xml
 
       - name: Upload coverage to Codecov
-        uses: codecov/codecov-action@5ecb98a3c6b747ed38dc09f787459979aebb39be #v4.3.1
+        uses: codecov/codecov-action@125fc84a9a348dbcf27191600683ec096ec9021c #v4.4.1
         with:
           token: ${{ secrets.CODECOV_TOKEN }}
           files: coverage.xml
           env_vars: OS,PYTHON
           fail_ci_if_error: true
           flags: unittests
           name: codecov-umbrella
```

### Comparing `python_cmethods-2.2.4/.github/workflows/_codeql.yaml` & `python_cmethods-2.2.5/.github/workflows/_codeql.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     #   matrix:
     #     language: ["python"]
     # CodeQL supports [ 'cpp', 'csharp', 'go', 'java', 'javascript', 'python', 'ruby' ]
     # Learn more about CodeQL language support at https://aka.ms/codeql-docs/language-support
 
     steps:
       - name: Checkout repository
-        uses: actions/checkout@44c2b7a8a4ea60a981eaca3cf939b5f4305c123b # v4.1.5
+        uses: actions/checkout@a5ac7e51b41094c92402da3b24376905380afc29 # v4.1.6
 
       # Initializes the CodeQL tools for scanning.
       - name: Initialize CodeQL
         uses: github/codeql-action/init@v3
         with:
           languages: python
           # If you wish to specify custom queries, you can do so here or in a config file.
```

### Comparing `python_cmethods-2.2.4/.github/workflows/_pypi_publish.yaml` & `python_cmethods-2.2.5/.github/workflows/_pypi_publish.yaml`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.4/.github/workflows/_pypi_test_publish.yaml` & `python_cmethods-2.2.5/.github/workflows/_pypi_test_publish.yaml`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.4/.github/workflows/cicd.yaml` & `python_cmethods-2.2.5/.github/workflows/cicd.yaml`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.4/.github/workflows/dependabot_auto_approve.yaml` & `python_cmethods-2.2.5/.github/workflows/dependabot_auto_approve.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 jobs:
   dependabot:
     runs-on: ubuntu-latest
     if: ${{ github.actor == 'dependabot[bot]' }}
     steps:
       - name: Dependabot metadata
         id: dependabot-metadata
-        uses: dependabot/fetch-metadata@v1.1.1
+        uses: dependabot/fetch-metadata@v2.1.0
         with:
           github-token: "${{ secrets.GITHUB_TOKEN }}"
       - name: Approve a PR
         if: ${{ steps.dependabot-metadata.outputs.update-type != 'version-update:semver-major' }}
         run: gh pr review --approve "$PR_URL"
         env:
           PR_URL: ${{ github.event.pull_request.html_url }}
```

### Comparing `python_cmethods-2.2.4/.github/workflows/scorecard.yml` & `python_cmethods-2.2.5/.github/workflows/scorecard.yml`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
       id-token: write
       # Uncomment the permissions below if installing in a private repository.
       # contents: read
       # actions: read
 
     steps:
       - name: "Checkout code"
-        uses: actions/checkout@44c2b7a8a4ea60a981eaca3cf939b5f4305c123b # v4.1.5
+        uses: actions/checkout@a5ac7e51b41094c92402da3b24376905380afc29 # v4.1.6
         with:
           persist-credentials: false
 
       - name: "Run analysis"
         uses: ossf/scorecard-action@dc50aa9510b46c811795eb24b2f1ba02a914e534 # v2.3.3
         with:
           results_file: results.sarif
```

### Comparing `python_cmethods-2.2.4/.gitignore` & `python_cmethods-2.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.4/.pre-commit-config.yaml` & `python_cmethods-2.2.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.4/CHANGELOG.md` & `python_cmethods-2.2.5/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.4/LICENSE` & `python_cmethods-2.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.4/Makefile` & `python_cmethods-2.2.5/Makefile`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.4/PKG-INFO` & `python_cmethods-2.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-cmethods
-Version: 2.2.4
+Version: 2.2.5
 Summary: A collection of bias correction techniques written in Python - for climate sciences.
 Author-email: Benjamin Thomas Schwertfeger <contact@b-schwertfeger.de>
 Maintainer-email: Benjamin Thomas Schwertfeger <contact@b-schwertfeger.de>
 License: GNU GENERAL PUBLIC LICENSE
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -656,14 +656,15 @@
 Classifier: Operating System :: Unix
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: xarray>=2022.11.0
 Requires-Dist: netCDF4>=1.6.1
 Requires-Dist: numpy
+Requires-Dist: click
 Requires-Dist: cloup
 Provides-Extra: jupyter
 Requires-Dist: venv-kernel; extra == "jupyter"
 Provides-Extra: dev
 Requires-Dist: setuptools_scm; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: sphinx; extra == "dev"
@@ -831,16 +832,16 @@
 > pre-installed using Homebrew (`brew install hdf5 netcdf`).
 
 ```bash
 python3 -m pip install python-cmethods
 ```
 
 The package is also available via conda-forge. See
-[conda-forge/python_cmethods-feedstock](https://github.com/conda-forge/python_cmethods-feedstock/tree/main) for more
-information.
+[conda-forge/python_cmethods](https://anaconda.org/conda-forge/python_cmethods)
+for more information.
 
 <a name="examples"></a>
 
 ## 4. CLI Usage
 
 The python-cmethods package provides a command-line interface for applying
 various bias correction methods out of the box.
```

### Comparing `python_cmethods-2.2.4/README.md` & `python_cmethods-2.2.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -145,16 +145,16 @@
 > pre-installed using Homebrew (`brew install hdf5 netcdf`).
 
 ```bash
 python3 -m pip install python-cmethods
 ```
 
 The package is also available via conda-forge. See
-[conda-forge/python_cmethods-feedstock](https://github.com/conda-forge/python_cmethods-feedstock/tree/main) for more
-information.
+[conda-forge/python_cmethods](https://anaconda.org/conda-forge/python_cmethods)
+for more information.
 
 <a name="examples"></a>
 
 ## 4. CLI Usage
 
 The python-cmethods package provides a command-line interface for applying
 various bias correction methods out of the box.
```

### Comparing `python_cmethods-2.2.4/SECURITY.md` & `python_cmethods-2.2.5/SECURITY.md`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.4/cmethods/__init__.py` & `python_cmethods-2.2.5/cmethods/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,49 +25,65 @@
 _{m} = long-term monthly interval
 """
 
 from __future__ import annotations
 
 import logging
 import sys
+from typing import TYPE_CHECKING, Any
+
+if TYPE_CHECKING:
+    from cloup import Context
 
 import cloup
 import xarray as xr
-from cloup import (
-    HelpFormatter,
-    HelpTheme,
-    Path,
-    Style,
-    command,
-    option,
-    option_group,
-    version_option,
-)
+from click import echo
+from cloup import HelpFormatter, HelpTheme, Path, Style, command, option, option_group
 from cloup.constraints import Equal, If, require_all
 
 from cmethods.core import adjust
 
 __all__ = ["adjust"]
 
 
+def print_version(
+    ctx: Context,
+    param: Any,  # noqa: ARG001
+    value: Any,
+) -> None:
+    """Prints the version of the package"""
+    if not value or ctx.resilient_parsing:
+        return
+    from importlib.metadata import version
+
+    echo(version("python-cmethods"))
+    ctx.exit()
+
+
 @command(
     context_settings={
         "auto_envvar_prefix": "CMETHODS",
         "help_option_names": ["-h", "--help"],
     },
     formatter_settings=HelpFormatter.settings(
         theme=HelpTheme(
             invoked_command=Style(fg="bright_yellow"),
             heading=Style(fg="bright_white", bold=True),
             constraint=Style(fg="magenta"),
             col1=Style(fg="bright_yellow"),
         ),
     ),
 )
-@version_option(message="%version%")
+@option(
+    "--version",
+    is_flag=True,
+    callback=print_version,
+    expose_value=False,
+    is_eager=True,
+)
 @option(
     "--obs",
     "--observations",
     required=True,
     type=Path(exists=True),
     help="Reference data set (control period)",
 )
```

### Comparing `python_cmethods-2.2.4/cmethods/core.py` & `python_cmethods-2.2.5/cmethods/core.py`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.4/cmethods/distribution.py` & `python_cmethods-2.2.5/cmethods/distribution.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,20 +140,16 @@
 
         m_simh = np.array(m_simh)
         m_simp = np.array(m_simp)
         m_simh_mean = np.nanmean(m_simh)
         m_simp_mean = np.nanmean(m_simp)
 
         if kind in ADDITIVE:
-            epsilon = np.interp(
-                m_simp - m_simp_mean + m_simh_mean,
-                xbins,
-                cdf_simh,
-            )  # Eq. 1
-            X = get_inverse_of_cdf(cdf_obs, epsilon, xbins) + m_simp_mean - m_simh_mean  # Eq. 1
+            epsilon = np.interp(m_simp - m_simp_mean, xbins, cdf_simh)  # Eq. 1
+            X = get_inverse_of_cdf(cdf_obs, epsilon, xbins) + m_simp_mean  # Eq. 1
 
         else:  # kind in cls.MULTIPLICATIVE:
             epsilon = np.interp(  # Eq. 2
                 ensure_dividable(
                     (m_simh_mean * m_simp),
                     m_simp_mean,
                     max_scaling_factor=max_scaling_factor,
```

### Comparing `python_cmethods-2.2.4/cmethods/scaling.py` & `python_cmethods-2.2.5/cmethods/scaling.py`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.4/cmethods/static.py` & `python_cmethods-2.2.5/cmethods/static.py`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.4/cmethods/utils.py` & `python_cmethods-2.2.5/cmethods/utils.py`

 * *Files identical despite different names*

### Comparing `python_cmethods-2.2.4/pyproject.toml` & `python_cmethods-2.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,21 @@
 maintainers = [
   { name = "Benjamin Thomas Schwertfeger", email = "contact@b-schwertfeger.de" },
 ]
 description = "A collection of bias correction techniques written in Python - for climate sciences."
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.8"
-dependencies = ["xarray>=2022.11.0", "netCDF4>=1.6.1", "numpy", "cloup"]
+dependencies = [
+  "xarray>=2022.11.0",
+  "netCDF4>=1.6.1",
+  "numpy",
+  "click",
+  "cloup",
+]
 keywords = [
   "climate-science",
   "bias",
   "bias-correction",
   "bias-adjustment",
   "climate-reanalysis",
   "reanalysis",
@@ -64,14 +70,15 @@
 [tool.pytest]
 junit_family = "xunit2"
 testpaths = ["tests"]
 
 [tool.pytest.ini_options]
 cache_dir = ".cache/pytest"
 markers = ["wip: Used to run a specific test by hand."]
+addopts = "--maxfail=1"
 
 [tool.coverage.run]
 source = ["cmethods"]
 omit = ["*tests*"]
 concurrency = ["multiprocessing"]
 
 [tool.coverage.report]
```

### Comparing `python_cmethods-2.2.4/python_cmethods.egg-info/PKG-INFO` & `python_cmethods-2.2.5/python_cmethods.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-cmethods
-Version: 2.2.4
+Version: 2.2.5
 Summary: A collection of bias correction techniques written in Python - for climate sciences.
 Author-email: Benjamin Thomas Schwertfeger <contact@b-schwertfeger.de>
 Maintainer-email: Benjamin Thomas Schwertfeger <contact@b-schwertfeger.de>
 License: GNU GENERAL PUBLIC LICENSE
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -656,14 +656,15 @@
 Classifier: Operating System :: Unix
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: xarray>=2022.11.0
 Requires-Dist: netCDF4>=1.6.1
 Requires-Dist: numpy
+Requires-Dist: click
 Requires-Dist: cloup
 Provides-Extra: jupyter
 Requires-Dist: venv-kernel; extra == "jupyter"
 Provides-Extra: dev
 Requires-Dist: setuptools_scm; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: sphinx; extra == "dev"
@@ -831,16 +832,16 @@
 > pre-installed using Homebrew (`brew install hdf5 netcdf`).
 
 ```bash
 python3 -m pip install python-cmethods
 ```
 
 The package is also available via conda-forge. See
-[conda-forge/python_cmethods-feedstock](https://github.com/conda-forge/python_cmethods-feedstock/tree/main) for more
-information.
+[conda-forge/python_cmethods](https://anaconda.org/conda-forge/python_cmethods)
+for more information.
 
 <a name="examples"></a>
 
 ## 4. CLI Usage
 
 The python-cmethods package provides a command-line interface for applying
 various bias correction methods out of the box.
```

### Comparing `python_cmethods-2.2.4/python_cmethods.egg-info/SOURCES.txt` & `python_cmethods-2.2.5/python_cmethods.egg-info/SOURCES.txt`

 * *Files identical despite different names*

