# Comparing `tmp/swh.journal-1.5.0.tar.gz` & `tmp/swh_journal-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swh.journal-1.5.0.tar", last modified: Mon Dec  4 16:30:44 2023, max compression
+gzip compressed data, was "swh_journal-1.5.1.tar", last modified: Tue May 28 10:55:23 2024, max compression
```

## Comparing `swh.journal-1.5.0.tar` & `swh_journal-1.5.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-12-04 16:30:44.919709 swh.journal-1.5.0/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      355 2023-12-04 16:30:38.000000 swh.journal-1.5.0/.copier-answers.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      140 2023-12-04 16:30:38.000000 swh.journal-1.5.0/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) jenkins    (120)      356 2023-12-04 16:30:38.000000 swh.journal-1.5.0/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)      943 2023-12-04 16:30:38.000000 swh.journal-1.5.0/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      112 2023-12-04 16:30:38.000000 swh.journal-1.5.0/AUTHORS
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3397 2023-12-04 16:30:38.000000 swh.journal-1.5.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) jenkins    (120)       15 2023-12-04 16:30:38.000000 swh.journal-1.5.0/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) jenkins    (120)    35147 2023-12-04 16:30:38.000000 swh.journal-1.5.0/LICENSE
--rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2023-12-04 16:30:38.000000 swh.journal-1.5.0/Makefile
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1904 2023-12-04 16:30:44.919709 swh.journal-1.5.0/PKG-INFO
--rw-r--r--   0 jenkins    (115) jenkins    (120)      339 2023-12-04 16:30:38.000000 swh.journal-1.5.0/README.rst
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-12-04 16:30:44.911709 swh.journal-1.5.0/docs/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2023-12-04 16:30:38.000000 swh.journal-1.5.0/docs/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2023-12-04 16:30:38.000000 swh.journal-1.5.0/docs/Makefile
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-12-04 16:30:44.911709 swh.journal-1.5.0/docs/_static/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2023-12-04 16:30:38.000000 swh.journal-1.5.0/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-12-04 16:30:44.911709 swh.journal-1.5.0/docs/_templates/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2023-12-04 16:30:38.000000 swh.journal-1.5.0/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) jenkins    (120)       43 2023-12-04 16:30:38.000000 swh.journal-1.5.0/docs/conf.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      901 2023-12-04 16:30:38.000000 swh.journal-1.5.0/docs/example-journal-client.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      233 2023-12-04 16:30:38.000000 swh.journal-1.5.0/docs/index.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3204 2023-12-04 16:30:38.000000 swh.journal-1.5.0/docs/journal-clients.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)      596 2023-12-04 16:30:38.000000 swh.journal-1.5.0/mypy.ini
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1734 2023-12-04 16:30:38.000000 swh.journal-1.5.0/pyproject.toml
--rw-r--r--   0 jenkins    (115) jenkins    (120)       97 2023-12-04 16:30:38.000000 swh.journal-1.5.0/pytest.ini
--rw-r--r--   0 jenkins    (115) jenkins    (120)       36 2023-12-04 16:30:38.000000 swh.journal-1.5.0/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)       48 2023-12-04 16:30:38.000000 swh.journal-1.5.0/requirements-test.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      405 2023-12-04 16:30:38.000000 swh.journal-1.5.0/requirements.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      120 2023-12-04 16:30:44.919709 swh.journal-1.5.0/setup.cfg
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-12-04 16:30:44.903709 swh.journal-1.5.0/swh/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-12-04 16:30:44.915709 swh.journal-1.5.0/swh/journal/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      326 2023-12-04 16:30:38.000000 swh.journal-1.5.0/swh/journal/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    18418 2023-12-04 16:30:38.000000 swh.journal-1.5.0/swh/journal/client.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2023-12-04 16:30:38.000000 swh.journal-1.5.0/swh/journal/py.typed
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7957 2023-12-04 16:30:38.000000 swh.journal-1.5.0/swh/journal/pytest_plugin.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3624 2023-12-04 16:30:38.000000 swh.journal-1.5.0/swh/journal/serializers.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-12-04 16:30:44.915709 swh.journal-1.5.0/swh/journal/tests/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2023-12-04 16:30:38.000000 swh.journal-1.5.0/swh/journal/tests/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      521 2023-12-04 16:30:38.000000 swh.journal-1.5.0/swh/journal/tests/journal_data.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      465 2023-12-04 16:30:38.000000 swh.journal-1.5.0/swh/journal/tests/log4j.properties
--rw-r--r--   0 jenkins    (115) jenkins    (120)    19253 2023-12-04 16:30:38.000000 swh.journal-1.5.0/swh/journal/tests/test_client.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1807 2023-12-04 16:30:38.000000 swh.journal-1.5.0/swh/journal/tests/test_inmemory.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     9123 2023-12-04 16:30:38.000000 swh.journal-1.5.0/swh/journal/tests/test_kafka_writer.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2183 2023-12-04 16:30:38.000000 swh.journal-1.5.0/swh/journal/tests/test_pytest_plugin.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3181 2023-12-04 16:30:38.000000 swh.journal-1.5.0/swh/journal/tests/test_serializers.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2465 2023-12-04 16:30:38.000000 swh.journal-1.5.0/swh/journal/tests/test_stream.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-12-04 16:30:44.915709 swh.journal-1.5.0/swh/journal/writer/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2110 2023-12-04 16:30:38.000000 swh.journal-1.5.0/swh/journal/writer/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1921 2023-12-04 16:30:38.000000 swh.journal-1.5.0/swh/journal/writer/inmemory.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1156 2023-12-04 16:30:38.000000 swh.journal-1.5.0/swh/journal/writer/interface.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    11213 2023-12-04 16:30:38.000000 swh.journal-1.5.0/swh/journal/writer/kafka.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1491 2023-12-04 16:30:38.000000 swh.journal-1.5.0/swh/journal/writer/stream.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2023-12-04 16:30:44.915709 swh.journal-1.5.0/swh.journal.egg-info/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1904 2023-12-04 16:30:44.000000 swh.journal-1.5.0/swh.journal.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1230 2023-12-04 16:30:44.000000 swh.journal-1.5.0/swh.journal.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        1 2023-12-04 16:30:44.000000 swh.journal-1.5.0/swh.journal.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)       58 2023-12-04 16:30:44.000000 swh.journal-1.5.0/swh.journal.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      233 2023-12-04 16:30:44.000000 swh.journal-1.5.0/swh.journal.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        4 2023-12-04 16:30:44.000000 swh.journal-1.5.0/swh.journal.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1337 2023-12-04 16:30:38.000000 swh.journal-1.5.0/tox.ini
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-28 10:55:23.693455 swh_journal-1.5.1/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      355 2024-05-28 10:55:17.000000 swh_journal-1.5.1/.copier-answers.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      158 2024-05-28 10:55:17.000000 swh_journal-1.5.1/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      356 2024-05-28 10:55:17.000000 swh_journal-1.5.1/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1385 2024-05-28 10:55:17.000000 swh_journal-1.5.1/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      112 2024-05-28 10:55:17.000000 swh_journal-1.5.1/AUTHORS
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3397 2024-05-28 10:55:17.000000 swh_journal-1.5.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       15 2024-05-28 10:55:17.000000 swh_journal-1.5.1/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    35147 2024-05-28 10:55:17.000000 swh_journal-1.5.1/LICENSE
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2024-05-28 10:55:17.000000 swh_journal-1.5.1/Makefile
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1909 2024-05-28 10:55:23.693455 swh_journal-1.5.1/PKG-INFO
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      339 2024-05-28 10:55:17.000000 swh_journal-1.5.1/README.rst
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-28 10:55:23.681455 swh_journal-1.5.1/docs/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-05-28 10:55:17.000000 swh_journal-1.5.1/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-05-28 10:55:17.000000 swh_journal-1.5.1/docs/Makefile
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-28 10:55:23.681455 swh_journal-1.5.1/docs/_static/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-28 10:55:17.000000 swh_journal-1.5.1/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-28 10:55:23.681455 swh_journal-1.5.1/docs/_templates/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-28 10:55:17.000000 swh_journal-1.5.1/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       43 2024-05-28 10:55:17.000000 swh_journal-1.5.1/docs/conf.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      899 2024-05-28 10:55:17.000000 swh_journal-1.5.1/docs/example-journal-client.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      233 2024-05-28 10:55:17.000000 swh_journal-1.5.1/docs/index.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3204 2024-05-28 10:55:17.000000 swh_journal-1.5.1/docs/journal-clients.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      596 2024-05-28 10:55:17.000000 swh_journal-1.5.1/mypy.ini
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1734 2024-05-28 10:55:17.000000 swh_journal-1.5.1/pyproject.toml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       96 2024-05-28 10:55:17.000000 swh_journal-1.5.1/pytest.ini
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       36 2024-05-28 10:55:17.000000 swh_journal-1.5.1/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       55 2024-05-28 10:55:17.000000 swh_journal-1.5.1/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      405 2024-05-28 10:55:17.000000 swh_journal-1.5.1/requirements.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      120 2024-05-28 10:55:23.697455 swh_journal-1.5.1/setup.cfg
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-28 10:55:23.673455 swh_journal-1.5.1/swh/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-28 10:55:23.685454 swh_journal-1.5.1/swh/journal/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      326 2024-05-28 10:55:17.000000 swh_journal-1.5.1/swh/journal/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    18698 2024-05-28 10:55:17.000000 swh_journal-1.5.1/swh/journal/client.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2024-05-28 10:55:17.000000 swh_journal-1.5.1/swh/journal/py.typed
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8140 2024-05-28 10:55:17.000000 swh_journal-1.5.1/swh/journal/pytest_plugin.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3624 2024-05-28 10:55:17.000000 swh_journal-1.5.1/swh/journal/serializers.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-28 10:55:23.689455 swh_journal-1.5.1/swh/journal/tests/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-28 10:55:17.000000 swh_journal-1.5.1/swh/journal/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      521 2024-05-28 10:55:17.000000 swh_journal-1.5.1/swh/journal/tests/journal_data.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      465 2024-05-28 10:55:17.000000 swh_journal-1.5.1/swh/journal/tests/log4j.properties
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    19252 2024-05-28 10:55:17.000000 swh_journal-1.5.1/swh/journal/tests/test_client.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1517 2024-05-28 10:55:17.000000 swh_journal-1.5.1/swh/journal/tests/test_inmemory.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8731 2024-05-28 10:55:17.000000 swh_journal-1.5.1/swh/journal/tests/test_kafka_writer.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2183 2024-05-28 10:55:17.000000 swh_journal-1.5.1/swh/journal/tests/test_pytest_plugin.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3181 2024-05-28 10:55:17.000000 swh_journal-1.5.1/swh/journal/tests/test_serializers.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2465 2024-05-28 10:55:17.000000 swh_journal-1.5.1/swh/journal/tests/test_stream.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-28 10:55:23.689455 swh_journal-1.5.1/swh/journal/writer/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2109 2024-05-28 10:55:17.000000 swh_journal-1.5.1/swh/journal/writer/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1921 2024-05-28 10:55:17.000000 swh_journal-1.5.1/swh/journal/writer/inmemory.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1156 2024-05-28 10:55:17.000000 swh_journal-1.5.1/swh/journal/writer/interface.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    11213 2024-05-28 10:55:17.000000 swh_journal-1.5.1/swh/journal/writer/kafka.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1491 2024-05-28 10:55:17.000000 swh_journal-1.5.1/swh/journal/writer/stream.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-28 10:55:23.689455 swh_journal-1.5.1/swh.journal.egg-info/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1909 2024-05-28 10:55:23.000000 swh_journal-1.5.1/swh.journal.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1230 2024-05-28 10:55:23.000000 swh_journal-1.5.1/swh.journal.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        1 2024-05-28 10:55:23.000000 swh_journal-1.5.1/swh.journal.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       58 2024-05-28 10:55:23.000000 swh_journal-1.5.1/swh.journal.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      238 2024-05-28 10:55:23.000000 swh_journal-1.5.1/swh.journal.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        4 2024-05-28 10:55:23.000000 swh_journal-1.5.1/swh.journal.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1067 2024-05-28 10:55:17.000000 swh_journal-1.5.1/tox.ini
```

### Comparing `swh.journal-1.5.0/CODE_OF_CONDUCT.md` & `swh_journal-1.5.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh.journal-1.5.0/LICENSE` & `swh_journal-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `swh.journal-1.5.0/PKG-INFO` & `swh_journal-1.5.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.journal
-Version: 1.5.0
+Version: 1.5.1
 Summary: Software Heritage Journal utilities
 Author-email: Software Heritage developers <swh-devel@inria.fr>
 Project-URL: Homepage, https://gitlab.softwareheritage.org/swh/devel/swh-journal
 Project-URL: Bug Reports, https://gitlab.softwareheritage.org/swh/devel/swh-journal/-/issues
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Documentation, https://docs.softwareheritage.org/devel/swh-journal/
 Project-URL: Source, https://gitlab.softwareheritage.org/swh/devel/swh-journal.git
@@ -24,15 +24,15 @@
 Requires-Dist: swh.model>=0.12.0
 Provides-Extra: testing
 Requires-Dist: confluent-kafka!=2.1.0; extra == "testing"
 Requires-Dist: msgpack!=1.0.1,>=1.0.0; extra == "testing"
 Requires-Dist: tenacity; extra == "testing"
 Requires-Dist: swh.core>=1.1; extra == "testing"
 Requires-Dist: swh.model>=0.12.0; extra == "testing"
-Requires-Dist: pytest; extra == "testing"
+Requires-Dist: pytest>=8.1; extra == "testing"
 Requires-Dist: pytest-mock; extra == "testing"
 Requires-Dist: hypothesis; extra == "testing"
 Requires-Dist: swh.core[testing]; extra == "testing"
 
 swh-journal
 ===========
```

### Comparing `swh.journal-1.5.0/docs/example-journal-client.py` & `swh_journal-1.5.1/docs/example-journal-client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pprint
 
 
 def process_objects(all_objects):
     """Worker function handling incoming objects"""
-    for (object_type, objects) in all_objects.items():
+    for object_type, objects in all_objects.items():
         for object_ in objects:
             print(f"New {object_type} object:")
             pprint.pprint(object_)
             print()
 
 
 def main():
```

### Comparing `swh.journal-1.5.0/docs/journal-clients.rst` & `swh_journal-1.5.1/docs/journal-clients.rst`

 * *Files identical despite different names*

### Comparing `swh.journal-1.5.0/mypy.ini` & `swh_journal-1.5.1/mypy.ini`

 * *Files identical despite different names*

### Comparing `swh.journal-1.5.0/pyproject.toml` & `swh_journal-1.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `swh.journal-1.5.0/swh/journal/client.py` & `swh_journal-1.5.1/swh/journal/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from collections import defaultdict
 import enum
 from importlib import import_module
 from itertools import cycle
 import logging
 import os
+import time
 from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union
 import warnings
 
 from confluent_kafka import (
     OFFSET_BEGINNING,
     Consumer,
     KafkaError,
@@ -369,27 +370,29 @@
                 for i in cycle(reversed(range(10))):
                     messages = self.consumer.consume(
                         timeout=timeout, num_messages=batch_size
                     )
                     if messages:
                         break
 
-                    # do check for an EOF condition iff we already consumed
+                    # do check for an EOF condition if we already consumed
                     # messages, otherwise we could detect an EOF condition
                     # before messages had a chance to reach us (e.g. in tests)
                     if total_objects_processed > 0 and i == 0:
+                        assignment = self.get_assignment()
+
                         if self.on_eof == EofBehavior.STOP:
                             at_eof = all(
                                 (tp.topic, tp.partition) in self.eof_reached
-                                for tp in self.consumer.assignment()
+                                for tp in assignment
                             )
                             if at_eof:
                                 break
                         elif self.on_eof == EofBehavior.RESTART:
-                            for tp in self.consumer.assignment():
+                            for tp in assignment:
                                 if (tp.topic, tp.partition) in self.eof_reached:
                                     self.eof_reached.remove((tp.topic, tp.partition))
                                     self.statsd.increment("partition_restart_total")
                                     new_tp = TopicPartition(
                                         tp.topic,
                                         tp.partition,
                                         OFFSET_BEGINNING,
@@ -441,23 +444,31 @@
                 objects[object_type].append(deserialized_object)
 
         if objects:
             worker_fn(dict(objects))
         self.consumer.commit()
 
         if self.on_eof in (EofBehavior.STOP, EofBehavior.RESTART):
+            assignment = self.get_assignment()
+
             at_eof = all(
-                (tp.topic, tp.partition) in self.eof_reached
-                for tp in self.consumer.assignment()
+                (tp.topic, tp.partition) in self.eof_reached for tp in assignment
             )
         elif self.on_eof == EofBehavior.CONTINUE:
             at_eof = False
         else:
             assert False, f"Unexpected on_eof behavior: {self.on_eof}"
 
         return nb_processed, at_eof
 
     def deserialize_message(self, message, object_type=None):
         return self.value_deserializer(object_type, message.value())
 
     def close(self):
         self.consumer.close()
+
+    def get_assignment(self):
+        while not (assignment := self.consumer.assignment()):
+            logger.info("No partition assigned, waiting for a new assignment")
+            time.sleep(1)
+
+        return assignment
```

### Comparing `swh.journal-1.5.0/swh/journal/pytest_plugin.py` & `swh_journal-1.5.1/swh/journal/pytest_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 import attr
 from confluent_kafka import Consumer, KafkaException, Producer
 from confluent_kafka.admin import AdminClient
 import pytest
 
 from swh.journal.serializers import kafka_to_key, kafka_to_value, pprint_key
+from swh.model.model import Content
 from swh.model.tests.swh_model_data import TEST_OBJECTS
 
 
 def ensure_lists(value: Any) -> Any:
     """
     >>> ensure_lists(["foo", 42])
     ['foo', 42]
@@ -98,15 +99,19 @@
 
         (received_keys, received_values) = zip(*consumed_messages[object_type])
 
         if object_type in ("content", "skipped_content"):
             for value in received_values:
                 value.pop("ctime", None)
         if object_type == "content":
-            known_objects = [attr.evolve(o, data=None) for o in known_objects]
+            contents = []
+            for o in known_objects:
+                assert isinstance(o, Content)  # to keep mypy happy
+                contents.append(attr.evolve(o, data=None))
+            known_objects = contents
 
         for key in known_keys:
             assert key in received_keys, (
                 f"expected {object_type} key {pprint_key(key)} "
                 "absent from consumed messages"
             )
```

### Comparing `swh.journal-1.5.0/swh/journal/serializers.py` & `swh_journal-1.5.1/swh/journal/serializers.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.5.0/swh/journal/tests/journal_data.py` & `swh_journal-1.5.1/swh/journal/tests/journal_data.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.5.0/swh/journal/tests/test_client.py` & `swh_journal-1.5.1/swh/journal/tests/test_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -611,15 +611,14 @@
     assert revisions[0] not in processed_revisions
     assert all(rev in processed_revisions for rev in revisions[1:])
 
 
 def test_client_create_topics(
     kafka_prefix: str, kafka_consumer_group: str, kafka_server_base: str, mocker
 ):
-
     # the Mock broker does not support the CreateTopic admin API, so we
     # mock the call to AdminClient.create_topics
     mock_admin = mocker.patch("swh.journal.client.AdminClient")
     mock_topic_future = mocker.Mock()
     mock_topic_future.result.return_value = None
     mock_admin.create_topics.return_value = {
         kafka_prefix + ".revision": mock_topic_future
```

### Comparing `swh.journal-1.5.0/swh/journal/tests/test_inmemory.py` & `swh_journal-1.5.1/swh/journal/tests/test_inmemory.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 # Copyright (C) 2019-2022 The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
-import pytest
-
 from swh.journal.writer import model_object_dict_sanitizer
 from swh.journal.writer.inmemory import InMemoryJournalWriter
-from swh.model.model import BaseModel
 from swh.model.tests.swh_model_data import TEST_OBJECTS
 
 
 def test_write_additions_anonymized():
     writer = InMemoryJournalWriter(
         value_sanitizer=model_object_dict_sanitizer, anonymize=True
     )
@@ -40,14 +37,7 @@
         writer.write_additions(object_type, objects)
 
         for object in objects:
             expected.add((object_type, object))
 
     assert not set(writer.privileged_objects)
     assert expected == set(writer.objects)
-
-
-def test_write_addition_errors_without_unique_key():
-    writer = InMemoryJournalWriter(value_sanitizer=model_object_dict_sanitizer)
-
-    with pytest.raises(NotImplementedError):
-        writer.write_addition("BaseModel", BaseModel())
```

### Comparing `swh.journal-1.5.0/swh/journal/tests/test_kafka_writer.py` & `swh_journal-1.5.1/swh/journal/tests/test_kafka_writer.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from confluent_kafka import Consumer, Producer
 import pytest
 
 from swh.journal.pytest_plugin import assert_all_objects_consumed, consume_messages
 from swh.journal.writer import model_object_dict_sanitizer
 from swh.journal.writer.kafka import KafkaDeliveryError, KafkaJournalWriter
-from swh.model.model import BaseModel, Directory, Release, Revision
+from swh.model.model import Directory, Release, Revision
 from swh.model.tests.swh_model_data import TEST_OBJECTS
 
 
 def test_kafka_writer(
     kafka_prefix: str,
     kafka_server: str,
     consumer: Consumer,
@@ -139,15 +139,14 @@
     assert len(exc.value.delivery_failures) == 1
     delivery_failure = exc.value.delivery_failures[0]
     assert delivery_failure.key == empty_dir.id
     assert delivery_failure.code == "SWH_MOCK_ERROR"
 
 
 def test_write_delivery_timeout(kafka_prefix: str, kafka_server: str):
-
     produced = []
 
     class MockProducer(Producer):
         """A kafka producer which pretends to produce messages, but never sends any
         delivery acknowledgements"""
 
         def produce(self, **kwargs):
@@ -232,26 +231,14 @@
 
     empty_dir = Directory(entries=())
 
     with pytest.raises(KafkaDeliveryError):
         writer.write_addition("directory", empty_dir)
 
 
-def test_write_addition_errors_without_unique_key(kafka_prefix: str, kafka_server: str):
-    writer = KafkaJournalWriter(
-        brokers=[kafka_server],
-        client_id="kafka_writer",
-        prefix=kafka_prefix,
-        value_sanitizer=model_object_dict_sanitizer,
-    )
-
-    with pytest.raises(NotImplementedError):
-        writer.write_addition("BaseModel", BaseModel())
-
-
 def test_kafka_writer_delete(
     kafka_prefix: str, kafka_server: str, consumer: Consumer
 ) -> None:
     # This test is a bit sad: we are using the Mock broker and it does not
     # support configuring Kafka topics. Therefore we cannot enable compaction.
     # So the only thing we can test is that a tombstone has been pushed.
     writer = KafkaJournalWriter(
```

### Comparing `swh.journal-1.5.0/swh/journal/tests/test_pytest_plugin.py` & `swh_journal-1.5.1/swh/journal/tests/test_pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.5.0/swh/journal/tests/test_serializers.py` & `swh_journal-1.5.1/swh/journal/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.5.0/swh/journal/tests/test_stream.py` & `swh_journal-1.5.1/swh/journal/tests/test_stream.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.5.0/swh/journal/writer/__init__.py` & `swh_journal-1.5.1/swh/journal/writer/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     object_dict = object_dict.copy()
     if object_type == "content":
         object_dict.pop("data", None)
     return object_dict
 
 
 def get_journal_writer(cls, **kwargs) -> JournalWriterInterface:
-
     if "args" in kwargs:
         warnings.warn(
             'Explicit "args" key is deprecated, use keys directly instead.',
             DeprecationWarning,
         )
         kwargs = kwargs["args"]
```

### Comparing `swh.journal-1.5.0/swh/journal/writer/inmemory.py` & `swh_journal-1.5.1/swh/journal/writer/inmemory.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.5.0/swh/journal/writer/interface.py` & `swh_journal-1.5.1/swh/journal/writer/interface.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.5.0/swh/journal/writer/kafka.py` & `swh_journal-1.5.1/swh/journal/writer/kafka.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.5.0/swh/journal/writer/stream.py` & `swh_journal-1.5.1/swh/journal/writer/stream.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.5.0/swh.journal.egg-info/PKG-INFO` & `swh_journal-1.5.1/swh.journal.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.journal
-Version: 1.5.0
+Version: 1.5.1
 Summary: Software Heritage Journal utilities
 Author-email: Software Heritage developers <swh-devel@inria.fr>
 Project-URL: Homepage, https://gitlab.softwareheritage.org/swh/devel/swh-journal
 Project-URL: Bug Reports, https://gitlab.softwareheritage.org/swh/devel/swh-journal/-/issues
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Documentation, https://docs.softwareheritage.org/devel/swh-journal/
 Project-URL: Source, https://gitlab.softwareheritage.org/swh/devel/swh-journal.git
@@ -24,15 +24,15 @@
 Requires-Dist: swh.model>=0.12.0
 Provides-Extra: testing
 Requires-Dist: confluent-kafka!=2.1.0; extra == "testing"
 Requires-Dist: msgpack!=1.0.1,>=1.0.0; extra == "testing"
 Requires-Dist: tenacity; extra == "testing"
 Requires-Dist: swh.core>=1.1; extra == "testing"
 Requires-Dist: swh.model>=0.12.0; extra == "testing"
-Requires-Dist: pytest; extra == "testing"
+Requires-Dist: pytest>=8.1; extra == "testing"
 Requires-Dist: pytest-mock; extra == "testing"
 Requires-Dist: hypothesis; extra == "testing"
 Requires-Dist: swh.core[testing]; extra == "testing"
 
 swh-journal
 ===========
```

### Comparing `swh.journal-1.5.0/swh.journal.egg-info/SOURCES.txt` & `swh_journal-1.5.1/swh.journal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

