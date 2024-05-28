# Comparing `tmp/swh_core-3.1.0.tar.gz` & `tmp/swh_core-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swh_core-3.1.0.tar", last modified: Tue May  7 13:49:24 2024, max compression
+gzip compressed data, was "swh_core-3.2.0.tar", last modified: Tue May 28 12:13:45 2024, max compression
```

## Comparing `swh_core-3.1.0.tar` & `swh_core-3.2.0.tar`

### file list

```diff
@@ -1,168 +1,167 @@
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.157636 swh_core-3.1.0/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      342 2024-05-07 13:49:17.000000 swh_core-3.1.0/.copier-answers.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      158 2024-05-07 13:49:17.000000 swh_core-3.1.0/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) jenkins    (120)      356 2024-05-07 13:49:17.000000 swh_core-3.1.0/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1410 2024-05-07 13:49:17.000000 swh_core-3.1.0/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      112 2024-05-07 13:49:17.000000 swh_core-3.1.0/AUTHORS
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3397 2024-05-07 13:49:17.000000 swh_core-3.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) jenkins    (120)       31 2024-05-07 13:49:17.000000 swh_core-3.1.0/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) jenkins    (120)    35147 2024-05-07 13:49:17.000000 swh_core-3.1.0/LICENSE
--rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2024-05-07 13:49:17.000000 swh_core-3.1.0/Makefile
--rw-r--r--   0 jenkins    (115) jenkins    (120)       95 2024-05-07 13:49:17.000000 swh_core-3.1.0/Makefile.local
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3541 2024-05-07 13:49:24.157636 swh_core-3.1.0/PKG-INFO
--rw-r--r--   0 jenkins    (115) jenkins    (120)      293 2024-05-07 13:49:17.000000 swh_core-3.1.0/README.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)      712 2024-05-07 13:49:17.000000 swh_core-3.1.0/conftest.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.117637 swh_core-3.1.0/docs/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-05-07 13:49:17.000000 swh_core-3.1.0/docs/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-05-07 13:49:17.000000 swh_core-3.1.0/docs/Makefile
--rw-r--r--   0 jenkins    (115) jenkins    (120)      293 2024-05-07 13:49:17.000000 swh_core-3.1.0/docs/README.rst
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.117637 swh_core-3.1.0/docs/_static/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:17.000000 swh_core-3.1.0/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.117637 swh_core-3.1.0/docs/_templates/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:17.000000 swh_core-3.1.0/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) jenkins    (120)      383 2024-05-07 13:49:17.000000 swh_core-3.1.0/docs/cli.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)       43 2024-05-07 13:49:17.000000 swh_core-3.1.0/docs/conf.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6486 2024-05-07 13:49:17.000000 swh_core-3.1.0/docs/db.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)      273 2024-05-07 13:49:17.000000 swh_core-3.1.0/docs/index.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)      982 2024-05-07 13:49:17.000000 swh_core-3.1.0/mypy.ini
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2117 2024-05-07 13:49:17.000000 swh_core-3.1.0/pyproject.toml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      156 2024-05-07 13:49:17.000000 swh_core-3.1.0/pytest.ini
--rw-r--r--   0 jenkins    (115) jenkins    (120)       58 2024-05-07 13:49:17.000000 swh_core-3.1.0/requirements-db.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      147 2024-05-07 13:49:17.000000 swh_core-3.1.0/requirements-http.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)       15 2024-05-07 13:49:17.000000 swh_core-3.1.0/requirements-logging.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:17.000000 swh_core-3.1.0/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      159 2024-05-07 13:49:17.000000 swh_core-3.1.0/requirements-test.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)       71 2024-05-07 13:49:17.000000 swh_core-3.1.0/requirements.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      170 2024-05-07 13:49:24.157636 swh_core-3.1.0/setup.cfg
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.117637 swh_core-3.1.0/swh/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      143 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/__main__.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.121636 swh_core-3.1.0/swh/core/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/__init__.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.125636 swh_core-3.1.0/swh/core/api/
--rw-r--r--   0 jenkins    (115) jenkins    (120)    21775 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/api/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6379 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/api/asynchronous.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2073 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/api/classes.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1192 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/api/gunicorn_config.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5812 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/api/negotiation.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    10114 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/api/serializers.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.125636 swh_core-3.1.0/swh/core/api/tests/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/api/tests/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/api/tests/conftest.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4292 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/api/tests/server_testing.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7863 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/api/tests/test_async.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2755 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/api/tests/test_classes.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5404 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/api/tests/test_gunicorn.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      862 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/api/tests/test_init.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6944 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/api/tests/test_rpc_client.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5170 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/api/tests/test_rpc_client_server.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7968 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/api/tests/test_rpc_server.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4871 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/api/tests/test_rpc_server_asynchronous.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8925 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/api/tests/test_serializers.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)       63 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/api_async.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.129636 swh_core-3.1.0/swh/core/cli/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5496 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/cli/__init__.py
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)    14013 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/cli/db.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2044 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/collections.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     9207 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/config.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.129636 swh_core-3.1.0/swh/core/db/
--rw-r--r--   0 jenkins    (115) jenkins    (120)    10619 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/db/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4888 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/db/common.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    24051 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/db/db_utils.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.129636 swh_core-3.1.0/swh/core/db/sql/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      664 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/db/sql/35-dbversion.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      683 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/db/sql/36-dbmodule.sql
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.129636 swh_core-3.1.0/swh/core/db/tests/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/db/tests/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2554 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/db/tests/conftest.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.105637 swh_core-3.1.0/swh/core/db/tests/data/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.105637 swh_core-3.1.0/swh/core/db/tests/data/cli/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.133636 swh_core-3.1.0/swh/core/db/tests/data/cli/sql/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       41 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/db/tests/data/cli/sql/0-superuser-init.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      790 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/db/tests/data/cli/sql/15-flavor.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      137 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/db/tests/data/cli/sql/30-schema.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      156 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/db/tests/data/cli/sql/40-funcs.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      126 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/db/tests/data/cli/sql/50-data.sql
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.133636 swh_core-3.1.0/swh/core/db/tests/data/cli/sql/upgrades/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      199 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/db/tests/data/cli/sql/upgrades/001.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)       82 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/db/tests/data/cli/sql/upgrades/002.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)       82 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/db/tests/data/cli/sql/upgrades/003.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)       82 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/db/tests/data/cli/sql/upgrades/004.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      306 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/db/tests/data/cli/sql/upgrades/005-bis.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)       82 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/db/tests/data/cli/sql/upgrades/005.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      196 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/db/tests/data/cli/sql/upgrades/006.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)    15397 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/db/tests/test_cli.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    13826 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/db/tests/test_db.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     9400 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/db/tests/test_db_utils.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.133636 swh_core-3.1.0/swh/core/github/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/github/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6612 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/github/pytest_plugin.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.137636 swh_core-3.1.0/swh/core/github/tests/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/github/tests/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    14265 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/github/tests/test_github_utils.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1440 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/github/tests/test_pytest_plugin.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    11211 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/github/utils.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4331 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/logger.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2583 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/logging.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/py.typed
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12994 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/pytest_plugin.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3271 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/retry.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3603 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/sentry.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    16759 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/statsd.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8364 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tarball.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.137636 swh_core-3.1.0/swh/core/tests/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       98 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.141636 swh_core-3.1.0/swh/core/tests/data/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.145636 swh_core-3.1.0/swh/core/tests/data/archives/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2028 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/data/archives/ca-certificates-20210603-1-any.pkg.tar.zst
--rw-r--r--   0 jenkins    (115) jenkins    (120)  1087901 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/data/archives/groff-1.02.tar.Z
--rw-r--r--   0 jenkins    (115) jenkins    (120)      550 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/data/archives/hello.jar
--rw-r--r--   0 jenkins    (115) jenkins    (120)    10240 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/data/archives/hello.tar
--rw-r--r--   0 jenkins    (115) jenkins    (120)      199 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/data/archives/hello.tar.bz2
--rw-r--r--   0 jenkins    (115) jenkins    (120)      181 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/data/archives/hello.tar.gz
--rw-r--r--   0 jenkins    (115) jenkins    (120)      190 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/data/archives/hello.tar.lz
--rw-r--r--   0 jenkins    (115) jenkins    (120)    10240 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/data/archives/hello.tar.x
--rw-r--r--   0 jenkins    (115) jenkins    (120)      199 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/data/archives/hello.tbz
--rw-r--r--   0 jenkins    (115) jenkins    (120)      199 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/data/archives/hello.tbz2
--rw-r--r--   0 jenkins    (115) jenkins    (120)      551 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/data/archives/hello.war
--rw-r--r--   0 jenkins    (115) jenkins    (120)      162 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/data/archives/hello.zip
--rw-r--r--   0 jenkins    (115) jenkins    (120)   845917 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/data/archives/msk316src.zip
--rw-r--r--   0 jenkins    (115) jenkins    (120)    45185 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/data/archives/tokei-12.1.2.crate
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.145636 swh_core-3.1.0/swh/core/tests/data/http_example.com/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       12 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/data/http_example.com/something.json
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.145636 swh_core-3.1.0/swh/core/tests/data/https_example.com/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       23 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/data/https_example.com/file.json
--rw-r--r--   0 jenkins    (115) jenkins    (120)       28 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/data/https_example.com/file.json,name=doe,firstname=jane
--rw-r--r--   0 jenkins    (115) jenkins    (120)       25 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/data/https_example.com/file.json_visit1
--rw-r--r--   0 jenkins    (115) jenkins    (120)        9 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/data/https_example.com/other.json
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.145636 swh_core-3.1.0/swh/core/tests/data/https_forge.s.o/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       12 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/data/https_forge.s.o/api_diffusion,attachments[uris]=1
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.145636 swh_core-3.1.0/swh/core/tests/data/https_www.reference.com/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       17 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/data/https_www.reference.com/web,q=What+Is+an+Example+of+a+URL?,qo=contentPageRelatedSearch,o=600605,l=dir,sga=1
--rw-r--r--   0 jenkins    (115) jenkins    (120)      642 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/data/logging-config.yaml
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.149636 swh_core-3.1.0/swh/core/tests/fixture/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/fixture/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      401 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/fixture/conftest.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.109637 swh_core-3.1.0/swh/core/tests/fixture/data/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.149636 swh_core-3.1.0/swh/core/tests/fixture/data/https_example.com/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       25 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/fixture/data/https_example.com/file.json
--rw-r--r--   0 jenkins    (115) jenkins    (120)      797 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/fixture/test_pytest_plugin.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    11911 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/test_cli.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2439 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/test_collections.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    10147 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/test_config.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3738 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/test_logger.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2826 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/test_logging.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4018 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/test_pytest_plugin.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2580 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/test_retry.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4879 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/test_sentry.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    18746 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/test_statsd.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     9873 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/test_tarball.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5422 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/test_utils.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5788 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/utils.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.149636 swh_core-3.1.0/swh.core.egg-info/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3541 2024-05-07 13:49:24.000000 swh_core-3.1.0/swh.core.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4363 2024-05-07 13:49:24.000000 swh_core-3.1.0/swh.core.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        1 2024-05-07 13:49:24.000000 swh_core-3.1.0/swh.core.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      148 2024-05-07 13:49:24.000000 swh_core-3.1.0/swh.core.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      661 2024-05-07 13:49:24.000000 swh_core-3.1.0/swh.core.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        4 2024-05-07 13:49:24.000000 swh_core-3.1.0/swh.core.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1550 2024-05-07 13:49:17.000000 swh_core-3.1.0/tox.ini
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-28 12:13:45.389148 swh_core-3.2.0/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      342 2024-05-28 12:13:39.000000 swh_core-3.2.0/.copier-answers.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      158 2024-05-28 12:13:39.000000 swh_core-3.2.0/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      356 2024-05-28 12:13:39.000000 swh_core-3.2.0/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1410 2024-05-28 12:13:39.000000 swh_core-3.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      112 2024-05-28 12:13:39.000000 swh_core-3.2.0/AUTHORS
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3397 2024-05-28 12:13:39.000000 swh_core-3.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       31 2024-05-28 12:13:39.000000 swh_core-3.2.0/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    35147 2024-05-28 12:13:39.000000 swh_core-3.2.0/LICENSE
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2024-05-28 12:13:39.000000 swh_core-3.2.0/Makefile
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       95 2024-05-28 12:13:39.000000 swh_core-3.2.0/Makefile.local
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3541 2024-05-28 12:13:45.389148 swh_core-3.2.0/PKG-INFO
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      293 2024-05-28 12:13:39.000000 swh_core-3.2.0/README.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      712 2024-05-28 12:13:39.000000 swh_core-3.2.0/conftest.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-28 12:13:45.353148 swh_core-3.2.0/docs/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-05-28 12:13:39.000000 swh_core-3.2.0/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-05-28 12:13:39.000000 swh_core-3.2.0/docs/Makefile
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      293 2024-05-28 12:13:39.000000 swh_core-3.2.0/docs/README.rst
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-28 12:13:45.353148 swh_core-3.2.0/docs/_static/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-28 12:13:39.000000 swh_core-3.2.0/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-28 12:13:45.353148 swh_core-3.2.0/docs/_templates/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-28 12:13:39.000000 swh_core-3.2.0/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      383 2024-05-28 12:13:39.000000 swh_core-3.2.0/docs/cli.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       43 2024-05-28 12:13:39.000000 swh_core-3.2.0/docs/conf.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6486 2024-05-28 12:13:39.000000 swh_core-3.2.0/docs/db.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      273 2024-05-28 12:13:39.000000 swh_core-3.2.0/docs/index.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      928 2024-05-28 12:13:39.000000 swh_core-3.2.0/mypy.ini
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2117 2024-05-28 12:13:39.000000 swh_core-3.2.0/pyproject.toml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      156 2024-05-28 12:13:39.000000 swh_core-3.2.0/pytest.ini
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       58 2024-05-28 12:13:39.000000 swh_core-3.2.0/requirements-db.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      147 2024-05-28 12:13:39.000000 swh_core-3.2.0/requirements-http.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       15 2024-05-28 12:13:39.000000 swh_core-3.2.0/requirements-logging.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-28 12:13:39.000000 swh_core-3.2.0/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      159 2024-05-28 12:13:39.000000 swh_core-3.2.0/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       71 2024-05-28 12:13:39.000000 swh_core-3.2.0/requirements.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      170 2024-05-28 12:13:45.393148 swh_core-3.2.0/setup.cfg
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-28 12:13:45.353148 swh_core-3.2.0/swh/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      143 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/__main__.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-28 12:13:45.357148 swh_core-3.2.0/swh/core/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/__init__.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-28 12:13:45.361148 swh_core-3.2.0/swh/core/api/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    21775 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/api/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6379 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/api/asynchronous.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2073 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/api/classes.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1192 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/api/gunicorn_config.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5812 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/api/negotiation.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    10114 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/api/serializers.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-28 12:13:45.361148 swh_core-3.2.0/swh/core/api/tests/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/api/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4292 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/api/tests/server_testing.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7863 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/api/tests/test_async.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2755 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/api/tests/test_classes.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5408 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/api/tests/test_gunicorn.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      862 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/api/tests/test_init.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6944 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/api/tests/test_rpc_client.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5170 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/api/tests/test_rpc_client_server.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7791 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/api/tests/test_rpc_server.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4871 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/api/tests/test_rpc_server_asynchronous.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8925 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/api/tests/test_serializers.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       63 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/api_async.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-28 12:13:45.365148 swh_core-3.2.0/swh/core/cli/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5506 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/cli/__init__.py
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)    14226 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/cli/db.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2044 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/collections.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     9229 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/config.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-28 12:13:45.365148 swh_core-3.2.0/swh/core/db/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    10619 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/db/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4888 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/db/common.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    24051 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/db/db_utils.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-28 12:13:45.365148 swh_core-3.2.0/swh/core/db/sql/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      664 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/db/sql/35-dbversion.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      683 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/db/sql/36-dbmodule.sql
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-28 12:13:45.365148 swh_core-3.2.0/swh/core/db/tests/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/db/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2554 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/db/tests/conftest.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-28 12:13:45.341148 swh_core-3.2.0/swh/core/db/tests/data/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-28 12:13:45.341148 swh_core-3.2.0/swh/core/db/tests/data/cli/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-28 12:13:45.369148 swh_core-3.2.0/swh/core/db/tests/data/cli/sql/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       41 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/db/tests/data/cli/sql/0-superuser-init.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      790 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/db/tests/data/cli/sql/15-flavor.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      137 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/db/tests/data/cli/sql/30-schema.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      156 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/db/tests/data/cli/sql/40-funcs.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      126 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/db/tests/data/cli/sql/50-data.sql
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-28 12:13:45.369148 swh_core-3.2.0/swh/core/db/tests/data/cli/sql/upgrades/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      199 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/db/tests/data/cli/sql/upgrades/001.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       82 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/db/tests/data/cli/sql/upgrades/002.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       82 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/db/tests/data/cli/sql/upgrades/003.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       82 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/db/tests/data/cli/sql/upgrades/004.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      306 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/db/tests/data/cli/sql/upgrades/005-bis.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       82 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/db/tests/data/cli/sql/upgrades/005.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      196 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/db/tests/data/cli/sql/upgrades/006.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    15397 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/db/tests/test_cli.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    13826 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/db/tests/test_db.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     9400 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/db/tests/test_db_utils.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-28 12:13:45.369148 swh_core-3.2.0/swh/core/github/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/github/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6612 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/github/pytest_plugin.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-28 12:13:45.373148 swh_core-3.2.0/swh/core/github/tests/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/github/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    14265 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/github/tests/test_github_utils.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1440 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/github/tests/test_pytest_plugin.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    11211 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/github/utils.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4331 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/logger.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2583 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/logging.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/py.typed
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12994 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/pytest_plugin.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3271 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/retry.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3607 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/sentry.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    16759 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/statsd.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8364 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/tarball.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-28 12:13:45.373148 swh_core-3.2.0/swh/core/tests/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       98 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-28 12:13:45.373148 swh_core-3.2.0/swh/core/tests/data/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-28 12:13:45.381148 swh_core-3.2.0/swh/core/tests/data/archives/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2028 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/tests/data/archives/ca-certificates-20210603-1-any.pkg.tar.zst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)  1087901 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/tests/data/archives/groff-1.02.tar.Z
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      550 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/tests/data/archives/hello.jar
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    10240 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/tests/data/archives/hello.tar
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      199 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/tests/data/archives/hello.tar.bz2
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      181 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/tests/data/archives/hello.tar.gz
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      190 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/tests/data/archives/hello.tar.lz
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    10240 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/tests/data/archives/hello.tar.x
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      199 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/tests/data/archives/hello.tbz
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      199 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/tests/data/archives/hello.tbz2
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      551 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/tests/data/archives/hello.war
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      162 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/tests/data/archives/hello.zip
+-rw-r--r--   0 jenkins    (115) jenkins    (120)   845917 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/tests/data/archives/msk316src.zip
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    45185 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/tests/data/archives/tokei-12.1.2.crate
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-28 12:13:45.381148 swh_core-3.2.0/swh/core/tests/data/http_example.com/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       12 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/tests/data/http_example.com/something.json
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-28 12:13:45.381148 swh_core-3.2.0/swh/core/tests/data/https_example.com/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       23 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/tests/data/https_example.com/file.json
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       28 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/tests/data/https_example.com/file.json,name=doe,firstname=jane
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       25 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/tests/data/https_example.com/file.json_visit1
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        9 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/tests/data/https_example.com/other.json
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-28 12:13:45.381148 swh_core-3.2.0/swh/core/tests/data/https_forge.s.o/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       12 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/tests/data/https_forge.s.o/api_diffusion,attachments[uris]=1
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-28 12:13:45.381148 swh_core-3.2.0/swh/core/tests/data/https_www.reference.com/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       17 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/tests/data/https_www.reference.com/web,q=What+Is+an+Example+of+a+URL?,qo=contentPageRelatedSearch,o=600605,l=dir,sga=1
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      642 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/tests/data/logging-config.yaml
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-28 12:13:45.381148 swh_core-3.2.0/swh/core/tests/fixture/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/tests/fixture/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      401 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/tests/fixture/conftest.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-28 12:13:45.345148 swh_core-3.2.0/swh/core/tests/fixture/data/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-28 12:13:45.385148 swh_core-3.2.0/swh/core/tests/fixture/data/https_example.com/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       25 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/tests/fixture/data/https_example.com/file.json
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      797 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/tests/fixture/test_pytest_plugin.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    11916 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/tests/test_cli.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2439 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/tests/test_collections.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     9783 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/tests/test_config.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3738 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/tests/test_logger.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2826 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/tests/test_logging.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4018 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/tests/test_pytest_plugin.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2580 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/tests/test_retry.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4879 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/tests/test_sentry.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    18779 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/tests/test_statsd.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     9873 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/tests/test_tarball.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5422 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/tests/test_utils.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5788 2024-05-28 12:13:39.000000 swh_core-3.2.0/swh/core/utils.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-28 12:13:45.385148 swh_core-3.2.0/swh.core.egg-info/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3541 2024-05-28 12:13:45.000000 swh_core-3.2.0/swh.core.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4332 2024-05-28 12:13:45.000000 swh_core-3.2.0/swh.core.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        1 2024-05-28 12:13:45.000000 swh_core-3.2.0/swh.core.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      148 2024-05-28 12:13:45.000000 swh_core-3.2.0/swh.core.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      661 2024-05-28 12:13:45.000000 swh_core-3.2.0/swh.core.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        4 2024-05-28 12:13:45.000000 swh_core-3.2.0/swh.core.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1550 2024-05-28 12:13:39.000000 swh_core-3.2.0/tox.ini
```

### Comparing `swh_core-3.1.0/.pre-commit-config.yaml` & `swh_core-3.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/CODE_OF_CONDUCT.md` & `swh_core-3.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/LICENSE` & `swh_core-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/PKG-INFO` & `swh_core-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.core
-Version: 3.1.0
+Version: 3.2.0
 Summary: Software Heritage core utilities
 Author-email: Software Heritage developers <swh-devel@inria.fr>
 Project-URL: Homepage, https://gitlab.softwareheritage.org/swh/devel/swh-core
 Project-URL: Bug Reports, https://gitlab.softwareheritage.org/swh/devel/swh-core/-/issues
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Documentation, https://docs.softwareheritage.org/devel/swh-core/
 Project-URL: Source, https://gitlab.softwareheritage.org/swh/devel/swh-core.git
```

### Comparing `swh_core-3.1.0/conftest.py` & `swh_core-3.2.0/conftest.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/docs/db.rst` & `swh_core-3.2.0/docs/db.rst`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/mypy.ini` & `swh_core-3.2.0/mypy.ini`

 * *Files 7% similar despite different names*

```diff
@@ -30,17 +30,14 @@
 
 [mypy-magic.*]
 ignore_missing_imports = True
 
 [mypy-msgpack.*]
 ignore_missing_imports = True
 
-[mypy-pkg_resources.*]
-ignore_missing_imports = True
-
 [mypy-pytest_postgresql.*]
 ignore_missing_imports = True
 
 [mypy-requests_mock.*]
 ignore_missing_imports = True
 
 [mypy-systemd.*]
```

### Comparing `swh_core-3.1.0/pyproject.toml` & `swh_core-3.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/swh/core/api/__init__.py` & `swh_core-3.2.0/swh/core/api/__init__.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/swh/core/api/asynchronous.py` & `swh_core-3.2.0/swh/core/api/asynchronous.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/swh/core/api/classes.py` & `swh_core-3.2.0/swh/core/api/classes.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/swh/core/api/gunicorn_config.py` & `swh_core-3.2.0/swh/core/api/gunicorn_config.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/swh/core/api/negotiation.py` & `swh_core-3.2.0/swh/core/api/negotiation.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/swh/core/api/serializers.py` & `swh_core-3.2.0/swh/core/api/serializers.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/swh/core/api/tests/server_testing.py` & `swh_core-3.2.0/swh/core/api/tests/server_testing.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/swh/core/api/tests/test_async.py` & `swh_core-3.2.0/swh/core/api/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/swh/core/api/tests/test_classes.py` & `swh_core-3.2.0/swh/core/api/tests/test_classes.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/swh/core/api/tests/test_gunicorn.py` & `swh_core-3.2.0/swh/core/api/tests/test_gunicorn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # Copyright (C) 2019-2024  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
+from importlib.metadata import distribution
 import os
 
-import pkg_resources
-
 import swh.core.api.gunicorn_config as gunicorn_config
 
 
 def test_post_fork_default(mocker):
     flask_integration = object()  # unique object to check for equality
     logging_integration = object()  # unique object to check for equality
     mocker.patch(
@@ -76,15 +75,15 @@
             "SWH_SENTRY_ENVIRONMENT": "tests",
             "SWH_MAIN_PACKAGE": "swh.core",
         },
     )
 
     gunicorn_config.post_fork(None, None)
 
-    version = pkg_resources.get_distribution("swh.core").version
+    version = distribution("swh.core").version
 
     sentry_sdk_init.assert_called_once_with(
         dsn="test_dsn",
         integrations=[flask_integration, logging_integration],
         debug=False,
         release="swh.core@" + version,
         environment="tests",
```

### Comparing `swh_core-3.1.0/swh/core/api/tests/test_init.py` & `swh_core-3.2.0/swh/core/api/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/swh/core/api/tests/test_rpc_client.py` & `swh_core-3.2.0/swh/core/api/tests/test_rpc_client.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/swh/core/api/tests/test_rpc_client_server.py` & `swh_core-3.2.0/swh/core/api/tests/test_rpc_client_server.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/swh/core/api/tests/test_rpc_server.py` & `swh_core-3.2.0/swh/core/api/tests/test_rpc_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -151,22 +151,17 @@
         ],
         data=msgpack.dumps({"data": "toto"}),
     )
 
     assert res.status_code == 500
     assert res.mimetype == "application/x-msgpack", res.data
     data = msgpack.loads(res.data)
-    assert (
-        data.items()
-        >= {
-            "type": "ValueError",
-            "module": "builtins",
-            "args": ["this is an unexpected exception"],
-        }.items()
-    ), data
+    assert data["type"] == "ValueError"
+    assert data["module"] == "builtins"
+    assert data["args"] == ["this is an unexpected exception"]
 
 
 def test_rpc_server_custom_exception(flask_app_client):
     res = flask_app_client.post(
         url_for("custom_crashy"),
         headers=[
             ("Content-Type", "application/x-msgpack"),
@@ -174,22 +169,20 @@
         ],
         data=msgpack.dumps({"data": "toto"}),
     )
 
     assert res.status_code == 503
     assert res.mimetype == "application/x-msgpack", res.data
     data = msgpack.loads(res.data)
-    assert (
-        data.items()
-        >= {
-            "type": "MyCustomException",
-            "module": "swh.core.api.tests.test_rpc_server",
-            "args": ["try again later!"],
-        }.items()
-    ), data
+    assert data["type"] == "MyCustomException"
+    assert data["module"] in (
+        "swh.core.api.tests.test_rpc_server",
+        "core.api.tests.test_rpc_server",
+    )
+    assert data["args"] == ["try again later!"]
 
 
 def test_rpc_server_psycopg2_adminshutdown(flask_app_client):
     pytest.importorskip("psycopg2")
 
     res = flask_app_client.post(
         url_for("adminshutdown_crash"),
@@ -199,22 +192,17 @@
         ],
         data=msgpack.dumps({"data": "toto"}),
     )
 
     assert res.status_code == 503
     assert res.mimetype == "application/x-msgpack", res.data
     data = msgpack.loads(res.data)
-    assert (
-        data.items()
-        >= {
-            "type": "AdminShutdown",
-            "module": "psycopg2.errors",
-            "args": ["cluster is shutting down"],
-        }.items()
-    ), data
+    assert data["type"] == "AdminShutdown"
+    assert data["module"] == "psycopg2.errors"
+    assert data["args"] == ["cluster is shutting down"]
 
 
 def test_rpc_server_psycopg2_querycancelled(flask_app_client):
     pytest.importorskip("psycopg2")
 
     res = flask_app_client.post(
         url_for("querycancelled_crash"),
@@ -224,22 +212,17 @@
         ],
         data=msgpack.dumps({"data": "toto"}),
     )
 
     assert res.status_code == 500
     assert res.mimetype == "application/x-msgpack", res.data
     data = msgpack.loads(res.data)
-    assert (
-        data.items()
-        >= {
-            "type": "QueryCanceled",
-            "module": "psycopg2.errors",
-            "args": ["too big!"],
-        }.items()
-    ), data
+    assert data["type"] == "QueryCanceled"
+    assert data["module"] == "psycopg2.errors"
+    assert data["args"] == ["too big!"]
 
 
 def test_rpc_server_extra_serializers(flask_app_client):
     res = flask_app_client.post(
         url_for("serializer_test"),
         headers=[
             ("Content-Type", "application/x-msgpack"),
```

### Comparing `swh_core-3.1.0/swh/core/api/tests/test_rpc_server_asynchronous.py` & `swh_core-3.2.0/swh/core/api/tests/test_rpc_server_asynchronous.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/swh/core/api/tests/test_serializers.py` & `swh_core-3.2.0/swh/core/api/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/swh/core/cli/__init__.py` & `swh_core-3.2.0/swh/core/cli/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Copyright (C) 2019-2023  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
+from importlib.metadata import entry_points
 import logging
 import warnings
 
 import click
-import pkg_resources
 
 CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
 
 logger = logging.getLogger(__name__)
 
 
 class SWHHelpFormatter(click.HelpFormatter):
@@ -151,15 +151,15 @@
 
 
 def main():
     # Even though swh() sets up logging, we need an earlier basic logging setup
     # for the next few logging statements
     logging.basicConfig()
     # load plugins that define cli sub commands
-    for entry_point in pkg_resources.iter_entry_points("swh.cli.subcommands"):
+    for entry_point in entry_points(group="swh.cli.subcommands"):
         try:
             cmd = entry_point.load()
             if isinstance(cmd, click.BaseCommand):
                 # for BW compat, auto add click commands
                 warnings.warn(
                     f"{entry_point.name}: automagic addition of click commands "
                     f"to the main swh group is deprecated",
```

### Comparing `swh_core-3.1.0/swh/core/cli/db.py` & `swh_core-3.2.0/swh/core/cli/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,20 +168,21 @@
     from swh.core.db.db_utils import (
         get_database_info,
         import_swhmodule,
         populate_database_for_package,
         swh_set_db_version,
     )
 
-    cfg = None
     if dbname is None:
         # use the db cnx from the config file; the expected config entry is the
         # given module name
         cfg = ctx.obj["config"].get(module, {})
         dbname = get_dburl_from_config(cfg)
+    else:
+        cfg = {"cls": "postgresql", "db": dbname}
 
     if not dbname:
         raise click.BadParameter(
             "Missing the postgresql connection configuration. Either fix your "
             "configuration file or use the --dbname option."
         )
 
@@ -195,16 +196,14 @@
             "ERROR: the database version has been populated by sql init scripts. "
             "This is now deprecated and should not happen any more"
         )
     else:
         # db version has not been populated by sql init scripts (new style),
         # let's do it; instantiate the data source to retrieve the current
         # (expected) db version
-        if cfg is None:
-            cfg = {"cls": "postgresql", "db": dbname}
         datastore_factory = getattr(import_swhmodule(module), "get_datastore", None)
         if datastore_factory:
             datastore = datastore_factory(**cfg)
             if not hasattr(datastore, "current_version"):
                 logger.warning(
                     "Datastore %s does not declare the " "'current_version' attribute",
                     datastore,
@@ -320,14 +319,22 @@
         for version, tstamp, desc in versions:
             click.echo(f"{version} [{tstamp}] {desc}")
 
 
 @db.command(name="upgrade", context_settings=CONTEXT_SETTINGS)
 @click.argument("module", required=True)
 @click.option(
+    "--dbname",
+    "--db-name",
+    "-d",
+    help="Database name or connection URI.",
+    default=None,
+    show_default=False,
+)
+@click.option(
     "--to-version",
     type=int,
     help="Upgrade up to version VERSION",
     metavar="VERSION",
     default=None,
 )
 @click.option(
@@ -335,15 +342,15 @@
     help="Do not ask questions (use default answer to all questions)",
     default=True,
 )
 @click.option(
     "--module-config-key", help="Module configuration key to lookup.", default=None
 )
 @click.pass_context
-def db_upgrade(ctx, module, to_version, interactive, module_config_key):
+def db_upgrade(ctx, module, dbname, to_version, interactive, module_config_key):
     """Upgrade the database for given module (to a given version if specified).
 
     Examples::
 
         \b
         swh db upgrade storage
         swh db upgrade scheduler --to-version=10
@@ -356,16 +363,19 @@
         swh_db_upgrade,
         swh_set_db_module,
     )
 
     # use the db cnx from the config file; the expected config entry is either the given
     # module_config_key or defaulting to the module name (if module_config_key is not
     # provided)
-    cfg = ctx.obj["config"].get(module_config_key or module, {})
-    dbname = get_dburl_from_config(cfg)
+    if dbname is None:
+        cfg = ctx.obj["config"].get(module_config_key or module, {})
+        dbname = get_dburl_from_config(cfg)
+    else:
+        cfg = {"cls": "postgresql", "db": dbname}
 
     if not dbname:
         raise click.BadParameter(
             "Missing the postgresql connection configuration. Either fix your "
             "configuration file or use the --dbname option."
         )
```

### Comparing `swh_core-3.1.0/swh/core/collections.py` & `swh_core-3.2.0/swh/core/collections.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/swh/core/config.py` & `swh_core-3.2.0/swh/core/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         PermissionError if the file cannot be read.
     """
 
     try:
         os.stat(filepath)
     except PermissionError:
         raise
-    except FileNotFoundError:
+    except (FileNotFoundError, NotADirectoryError):
         return False
     else:
         if os.access(filepath, os.R_OK):
             return True
         else:
             raise PermissionError("Permission denied: {filepath!r}")
```

### Comparing `swh_core-3.1.0/swh/core/db/__init__.py` & `swh_core-3.2.0/swh/core/db/__init__.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/swh/core/db/common.py` & `swh_core-3.2.0/swh/core/db/common.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/swh/core/db/db_utils.py` & `swh_core-3.2.0/swh/core/db/db_utils.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/swh/core/db/sql/35-dbversion.sql` & `swh_core-3.2.0/swh/core/db/sql/35-dbversion.sql`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/swh/core/db/sql/36-dbmodule.sql` & `swh_core-3.2.0/swh/core/db/sql/36-dbmodule.sql`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/swh/core/db/tests/conftest.py` & `swh_core-3.2.0/swh/core/db/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/swh/core/db/tests/data/cli/sql/15-flavor.sql` & `swh_core-3.2.0/swh/core/db/tests/data/cli/sql/15-flavor.sql`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/swh/core/db/tests/test_cli.py` & `swh_core-3.2.0/swh/core/db/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/swh/core/db/tests/test_db.py` & `swh_core-3.2.0/swh/core/db/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/swh/core/db/tests/test_db_utils.py` & `swh_core-3.2.0/swh/core/db/tests/test_db_utils.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/swh/core/github/pytest_plugin.py` & `swh_core-3.2.0/swh/core/github/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/swh/core/github/tests/test_github_utils.py` & `swh_core-3.2.0/swh/core/github/tests/test_github_utils.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/swh/core/github/tests/test_pytest_plugin.py` & `swh_core-3.2.0/swh/core/github/tests/test_pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/swh/core/github/utils.py` & `swh_core-3.2.0/swh/core/github/utils.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/swh/core/logger.py` & `swh_core-3.2.0/swh/core/logger.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/swh/core/logging.py` & `swh_core-3.2.0/swh/core/logging.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/swh/core/pytest_plugin.py` & `swh_core-3.2.0/swh/core/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/swh/core/retry.py` & `swh_core-3.2.0/swh/core/retry.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/swh/core/sentry.py` & `swh_core-3.2.0/swh/core/sentry.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 # Copyright (C) 2019-2024  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
+from importlib.metadata import distribution
 import logging
 import os
 from typing import Dict, List, Optional
 
-import pkg_resources
-
 logger = logging.getLogger(__name__)
 
 
 def get_sentry_release(main_package: Optional[str] = None):
     main_package = os.environ.get("SWH_MAIN_PACKAGE", main_package)
     if main_package:
-        version = pkg_resources.get_distribution(main_package).version
+        version = distribution(main_package).version
         return f"{main_package}@{version}"
     else:
         return None
 
 
 def override_with_bool_envvar(envvar: str, default: bool) -> bool:
     """Override the `default` with the environment variable `envvar` parsed as a boolean"""
```

### Comparing `swh_core-3.1.0/swh/core/statsd.py` & `swh_core-3.2.0/swh/core/statsd.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/swh/core/tarball.py` & `swh_core-3.2.0/swh/core/tarball.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/swh/core/tests/data/archives/ca-certificates-20210603-1-any.pkg.tar.zst` & `swh_core-3.2.0/swh/core/tests/data/archives/ca-certificates-20210603-1-any.pkg.tar.zst`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/swh/core/tests/data/archives/groff-1.02.tar.Z` & `swh_core-3.2.0/swh/core/tests/data/archives/groff-1.02.tar.Z`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/swh/core/tests/data/archives/hello.jar` & `swh_core-3.2.0/swh/core/tests/data/archives/hello.jar`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/swh/core/tests/data/archives/hello.tar` & `swh_core-3.2.0/swh/core/tests/data/archives/hello.tar`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/swh/core/tests/data/archives/hello.tar.x` & `swh_core-3.2.0/swh/core/tests/data/archives/hello.tar.x`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/swh/core/tests/data/archives/hello.war` & `swh_core-3.2.0/swh/core/tests/data/archives/hello.war`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/swh/core/tests/data/archives/msk316src.zip` & `swh_core-3.2.0/swh/core/tests/data/archives/msk316src.zip`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/swh/core/tests/data/archives/tokei-12.1.2.crate` & `swh_core-3.2.0/swh/core/tests/data/archives/tokei-12.1.2.crate`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/swh/core/tests/data/logging-config.yaml` & `swh_core-3.2.0/swh/core/tests/data/logging-config.yaml`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/swh/core/tests/fixture/test_pytest_plugin.py` & `swh_core-3.2.0/swh/core/tests/fixture/test_pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/swh/core/tests/test_cli.py` & `swh_core-3.2.0/swh/core/tests/test_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Copyright (C) 2019-2024  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
+from importlib.metadata import distribution
 import logging
 import textwrap
 from typing import List
 
 import click
 from click.testing import CliRunner
-import pkg_resources
 import pytest
 import yaml
 
 help_msg_snippets = (
     (
         "Usage",
         (
@@ -234,15 +234,15 @@
         "SWH_SENTRY_DSN": "test_dsn",
         "SWH_MAIN_PACKAGE": "swh.core",
         "SWH_SENTRY_ENVIRONMENT": "tests",
     }
     result = runner.invoke(swhmain, ["test"], env=env, auto_envvar_prefix="SWH")
     assert result.exit_code == 0
 
-    version = pkg_resources.get_distribution("swh.core").version
+    version = distribution("swh.core").version
 
     assert result.output.strip() == """Hello SWH!"""
     sentry_sdk_init.assert_called_once_with(
         dsn="test_dsn",
         debug=False,
         integrations=[],
         release="swh.core@" + version,
```

### Comparing `swh_core-3.1.0/swh/core/tests/test_collections.py` & `swh_core-3.2.0/swh/core/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/swh/core/tests/test_config.py` & `swh_core-3.2.0/swh/core/tests/test_config.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,32 +3,19 @@
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 import os
 from pathlib import Path
 import shutil
 
-import pkg_resources.extern.packaging.version
 import pytest
 import yaml
 
 from swh.core import config
 
-pytest_v = pkg_resources.get_distribution("pytest").parsed_version
-if pytest_v < pkg_resources.extern.packaging.version.parse("3.9"):
-
-    @pytest.fixture
-    def tmp_path():
-        import pathlib
-        import tempfile
-
-        with tempfile.TemporaryDirectory() as tmpdir:
-            yield pathlib.Path(tmpdir)
-
-
 default_conf = {
     "a": ("int", 2),
     "b": ("string", "default-string"),
     "c": ("bool", True),
     "d": ("int", 10),
     "e": ("int", None),
     "f": ("bool", None),
```

### Comparing `swh_core-3.1.0/swh/core/tests/test_logger.py` & `swh_core-3.2.0/swh/core/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/swh/core/tests/test_logging.py` & `swh_core-3.2.0/swh/core/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/swh/core/tests/test_pytest_plugin.py` & `swh_core-3.2.0/swh/core/tests/test_pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/swh/core/tests/test_retry.py` & `swh_core-3.2.0/swh/core/tests/test_retry.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/swh/core/tests/test_sentry.py` & `swh_core-3.2.0/swh/core/tests/test_sentry.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/swh/core/tests/test_statsd.py` & `swh_core-3.2.0/swh/core/tests/test_statsd.py`

 * *Files 0% similar despite different names*

```diff
@@ -247,15 +247,15 @@
     assert result, (1, 2, 1 == 3)
 
     packet = statsd.socket.recv()
     name_value, type_ = packet.split("|")
     name, value = name_value.split(":")
 
     assert type_ == "ms"
-    assert name == "swh.core.tests.test_statsd.func"
+    assert name in ("swh.core.tests.test_statsd.func", "core.tests.test_statsd.func")
     assert_almost_equal(500, float(value), 100)
 
 
 def test_timed_coroutine(statsd):
     """
     Measure the distribution of a coroutine function's run time.
     """
```

### Comparing `swh_core-3.1.0/swh/core/tests/test_tarball.py` & `swh_core-3.2.0/swh/core/tests/test_tarball.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/swh/core/tests/test_utils.py` & `swh_core-3.2.0/swh/core/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/swh/core/utils.py` & `swh_core-3.2.0/swh/core/utils.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/swh.core.egg-info/PKG-INFO` & `swh_core-3.2.0/swh.core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.core
-Version: 3.1.0
+Version: 3.2.0
 Summary: Software Heritage core utilities
 Author-email: Software Heritage developers <swh-devel@inria.fr>
 Project-URL: Homepage, https://gitlab.softwareheritage.org/swh/devel/swh-core
 Project-URL: Bug Reports, https://gitlab.softwareheritage.org/swh/devel/swh-core/-/issues
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Documentation, https://docs.softwareheritage.org/devel/swh-core/
 Project-URL: Source, https://gitlab.softwareheritage.org/swh/devel/swh-core.git
```

### Comparing `swh_core-3.1.0/swh.core.egg-info/SOURCES.txt` & `swh_core-3.2.0/swh.core.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,14 @@
 swh/core/api/__init__.py
 swh/core/api/asynchronous.py
 swh/core/api/classes.py
 swh/core/api/gunicorn_config.py
 swh/core/api/negotiation.py
 swh/core/api/serializers.py
 swh/core/api/tests/__init__.py
-swh/core/api/tests/conftest.py
 swh/core/api/tests/server_testing.py
 swh/core/api/tests/test_async.py
 swh/core/api/tests/test_classes.py
 swh/core/api/tests/test_gunicorn.py
 swh/core/api/tests/test_init.py
 swh/core/api/tests/test_rpc_client.py
 swh/core/api/tests/test_rpc_client_server.py
```

### Comparing `swh_core-3.1.0/swh.core.egg-info/requires.txt` & `swh_core-3.2.0/swh.core.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `swh_core-3.1.0/tox.ini` & `swh_core-3.2.0/tox.ini`

 * *Files identical despite different names*

