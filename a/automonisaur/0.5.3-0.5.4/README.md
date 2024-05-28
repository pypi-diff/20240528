# Comparing `tmp/automonisaur-0.5.3.tar.gz` & `tmp/automonisaur-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automonisaur-0.5.3.tar", last modified: Wed May 15 18:06:23 2024, max compression
+gzip compressed data, was "automonisaur-0.5.4.tar", last modified: Tue May 28 19:19:35 2024, max compression
```

## Comparing `automonisaur-0.5.3.tar` & `automonisaur-0.5.4.tar`

### file list

```diff
@@ -1,416 +1,434 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.037043 automonisaur-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-15 18:06:19.000000 automonisaur-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-05-15 18:06:23.037043 automonisaur-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4333 2024-05-15 18:06:19.000000 automonisaur-0.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:22.993042 automonisaur-0.5.3/automon/
--rwxr-xr-x   0 runner    (1001) docker     (127)       93 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/healthcheck.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:22.993042 automonisaur-0.5.3/automon/helpers/
--rwxr-xr-x   0 runner    (1001) docker     (127)      204 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1257 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/assertions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:22.993042 automonisaur-0.5.3/automon/helpers/asyncioWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/asyncioWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/asyncioWrapper/loop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:22.993042 automonisaur-0.5.3/automon/helpers/cryptography/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/cryptography/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/cryptography/hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/cryptography/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/dates.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/httpWrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/markdown.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:22.993042 automonisaur-0.5.3/automon/helpers/mathWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/mathWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/mathWrapper/file_size.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/networking.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:22.993042 automonisaur-0.5.3/automon/helpers/osWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/osWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/osWrapper/environ.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      338 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/regex.py
--rw-r--r--   0 runner    (1001) docker     (127)     4412 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/sanitation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/sleeper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:22.993042 automonisaur-0.5.3/automon/helpers/subprocessWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/subprocessWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/subprocessWrapper/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/subprocessWrapper/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:22.997042 automonisaur-0.5.3/automon/helpers/subprocessWrapper/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/subprocessWrapper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/subprocessWrapper/tests/test_run.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/subprocessWrapper/tests/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/subprocessWrapper/tests/test_sanitize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:22.997042 automonisaur-0.5.3/automon/helpers/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/tests/test_assertions.py
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/tests/test_healthcheck.py
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/tests/test_liveliness.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/tests/test_networking.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/tests/test_sanitation.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/tests/test_sleeper.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/tests/test_sleeper_async.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:22.997042 automonisaur-0.5.3/automon/helpers/threadingWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/threadingWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/threadingWrapper/initialize_threading.py
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/helpers/threadingWrapper/worker_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:22.997042 automonisaur-0.5.3/automon/integrations/
--rwxr-xr-x   0 runner    (1001) docker     (127)       27 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:22.997042 automonisaur-0.5.3/automon/integrations/beautifulsoupWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/beautifulsoupWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/beautifulsoupWrapper/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:22.997042 automonisaur-0.5.3/automon/integrations/cryptocurrency/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/cryptocurrency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/cryptocurrency/accounting.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/cryptocurrency/coinbase.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/cryptocurrency/other.py
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/cryptocurrency/robinhood.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:22.997042 automonisaur-0.5.3/automon/integrations/cryptocurrency/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/cryptocurrency/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/cryptocurrency/tests/test_crypto.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:22.997042 automonisaur-0.5.3/automon/integrations/datadogWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/datadogWrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.001042 automonisaur-0.5.3/automon/integrations/datadogWrapper/api/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/datadogWrapper/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/datadogWrapper/api/v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/datadogWrapper/api/v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/datadogWrapper/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/datadogWrapper/client_opentelemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/datadogWrapper/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/datadogWrapper/config_opentelemetry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.001042 automonisaur-0.5.3/automon/integrations/datadogWrapper/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/datadogWrapper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/datadogWrapper/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/datadogWrapper/tests/test_client_opentelemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/datadogWrapper/tests/test_config_opentelemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/datadogWrapper/tests/test_log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.001042 automonisaur-0.5.3/automon/integrations/datascience/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/datascience/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.001042 automonisaur-0.5.3/automon/integrations/datascience/pandas/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/datascience/pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/datascience/pandas/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/datascience/pandas/pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/datascience/pandas/series.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.001042 automonisaur-0.5.3/automon/integrations/datascience/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/datascience/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/datascience/tests/test_datascience.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.001042 automonisaur-0.5.3/automon/integrations/elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/elasticsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/elasticsearch/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (127)    10557 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/elasticsearch/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/elasticsearch/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/elasticsearch/jvm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/elasticsearch/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5915 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/elasticsearch/snapshots.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.001042 automonisaur-0.5.3/automon/integrations/elasticsearch/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/elasticsearch/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/elasticsearch/tests/test_elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/elasticsearch/tests/test_elasticsearch_JvmMonitor.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/elasticsearch/tests/test_elasticsearch_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/elasticsearch/tests/test_elasticsearch_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/elasticsearch/tests/test_elasticsearch_snapshot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.005042 automonisaur-0.5.3/automon/integrations/facebook/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/facebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22254 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/facebook/groups.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.005042 automonisaur-0.5.3/automon/integrations/flaskWrapper/
--rwxr-xr-x   0 runner    (1001) docker     (127)       42 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/flaskWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/flaskWrapper/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/flaskWrapper/auth_creds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/flaskWrapper/boilerplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/flaskWrapper/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.005042 automonisaur-0.5.3/automon/integrations/flaskWrapper/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/flaskWrapper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/flaskWrapper/tests/test_flask.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.005042 automonisaur-0.5.3/automon/integrations/geoip/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/geoip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.005042 automonisaur-0.5.3/automon/integrations/geoip/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/geoip/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/geoip/tests/test_geoip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.005042 automonisaur-0.5.3/automon/integrations/google/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.005042 automonisaur-0.5.3/automon/integrations/google/auth/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/auth/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/auth/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.005042 automonisaur-0.5.3/automon/integrations/google/auth/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/auth/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/auth/tests/test_config_Credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/auth/tests/test_google_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.005042 automonisaur-0.5.3/automon/integrations/google/gmail/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/gmail/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.005042 automonisaur-0.5.3/automon/integrations/google/gmail/v1/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/gmail/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/gmail/v1/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/gmail/v1/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.005042 automonisaur-0.5.3/automon/integrations/google/people/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/people/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/people/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/people/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    10867 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/people/person.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/people/results.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.009042 automonisaur-0.5.3/automon/integrations/google/people/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/people/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/people/tests/test_google_contacts.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/people/tests/test_google_contacts_neo4j.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/people/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.009042 automonisaur-0.5.3/automon/integrations/google/sheets/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/sheets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/sheets/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/sheets/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.009042 automonisaur-0.5.3/automon/integrations/google/sheets/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/sheets/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11260 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/sheets/tests/test_google_sheets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/sheets/tests/test_google_sheets_AUDIT.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/sheets/tests/test_google_sheets_clear.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.009042 automonisaur-0.5.3/automon/integrations/google/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/tests/test_google_contacts.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/google/tests/test_google_contacts_neo4j.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.009042 automonisaur-0.5.3/automon/integrations/grok/
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/grok/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.009042 automonisaur-0.5.3/automon/integrations/grok/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/grok/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/grok/tests/test_grok.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.009042 automonisaur-0.5.3/automon/integrations/instagram/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/instagram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/instagram/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8593 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/instagram/client_browser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/instagram/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7666 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/instagram/stories.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.009042 automonisaur-0.5.3/automon/integrations/instagram/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/instagram/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/instagram/tests/test_instagram.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/instagram/tests/test_instagram_browser.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/instagram/tests/test_instagram_browser_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/instagram/tests/test_instagram_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/instagram/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/instagram/xpaths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.009042 automonisaur-0.5.3/automon/integrations/ldap/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/ldap/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3523 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/ldap/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.013043 automonisaur-0.5.3/automon/integrations/mac/
--rwxr-xr-x   0 runner    (1001) docker     (127)       93 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/mac/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.013043 automonisaur-0.5.3/automon/integrations/mac/airport/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/mac/airport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6393 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/mac/airport/airport.py
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/mac/airport/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/mac/airport/ssid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.013043 automonisaur-0.5.3/automon/integrations/mac/airport/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/mac/airport/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/mac/airport/tests/test_airport.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/mac/airport/tests/test_airport_neo4j.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/mac/check.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.013043 automonisaur-0.5.3/automon/integrations/mac/macchanger/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/mac/macchanger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/mac/macchanger/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.013043 automonisaur-0.5.3/automon/integrations/mac/macchanger/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/mac/macchanger/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/mac/macchanger/tests/test_macchanger.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/mac/macchanger/tests/test_set_mac_random.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.013043 automonisaur-0.5.3/automon/integrations/minioWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/minioWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/minioWrapper/assertions.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/minioWrapper/bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)     7849 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/minioWrapper/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/minioWrapper/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/minioWrapper/object.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.013043 automonisaur-0.5.3/automon/integrations/minioWrapper/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/minioWrapper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/minioWrapper/tests/test_minio_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/minioWrapper/tests/test_minio_client_public.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/minioWrapper/tests/test_minio_client_public_clear_bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/minioWrapper/tests/test_minio_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.017042 automonisaur-0.5.3/automon/integrations/neo4jWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/neo4jWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/neo4jWrapper/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/neo4jWrapper/clientAsync.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/neo4jWrapper/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11026 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/neo4jWrapper/cypher.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/neo4jWrapper/results.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.017042 automonisaur-0.5.3/automon/integrations/neo4jWrapper/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/neo4jWrapper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/neo4jWrapper/tests/test_neo4j_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/neo4jWrapper/tests/test_neo4j_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/neo4jWrapper/tests/test_neo4j_cypher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.017042 automonisaur-0.5.3/automon/integrations/nest_asyncioWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/nest_asyncioWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/nest_asyncioWrapper/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.017042 automonisaur-0.5.3/automon/integrations/nmap/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/nmap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/nmap/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/nmap/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/nmap/output.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.017042 automonisaur-0.5.3/automon/integrations/nmap/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/nmap/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/nmap/tests/test_nmap_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/nmap/tests/test_nmap_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.017042 automonisaur-0.5.3/automon/integrations/openTelemetryWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/openTelemetryWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/openTelemetryWrapper/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/openTelemetryWrapper/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.017042 automonisaur-0.5.3/automon/integrations/openTelemetryWrapper/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/openTelemetryWrapper/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/openTelemetryWrapper/test/test_client_ready.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/openTelemetryWrapper/test/test_memory_trace_client_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/openTelemetryWrapper/test/test_memory_trace_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/openTelemetryWrapper/test/test_pop_finished_spans.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.017042 automonisaur-0.5.3/automon/integrations/openvpn/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/openvpn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6982 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/openvpn/openvpn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.017042 automonisaur-0.5.3/automon/integrations/psutilWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/psutilWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/psutilWrapper/cpu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.017042 automonisaur-0.5.3/automon/integrations/requestsWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/requestsWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6564 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/requestsWrapper/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/requestsWrapper/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/requestsWrapper/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.021043 automonisaur-0.5.3/automon/integrations/requestsWrapper/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/requestsWrapper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/requestsWrapper/tests/test_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/requestsWrapper/tests/test_rest.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/requestsWrapper/tests/test_rest_inherit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.021043 automonisaur-0.5.3/automon/integrations/scrapyWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/scrapyWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/scrapyWrapper/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.021043 automonisaur-0.5.3/automon/integrations/seleniumWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/seleniumWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/seleniumWrapper/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)    17113 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/seleniumWrapper/browser.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/seleniumWrapper/browser_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/seleniumWrapper/browser_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/seleniumWrapper/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/seleniumWrapper/config_window_size.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/seleniumWrapper/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.021043 automonisaur-0.5.3/automon/integrations/seleniumWrapper/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/seleniumWrapper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/seleniumWrapper/tests/test_browser.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/seleniumWrapper/tests/test_browser_headless.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/seleniumWrapper/tests/test_browser_useragent.py
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/seleniumWrapper/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/seleniumWrapper/tests/test_new_browser.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/seleniumWrapper/tests/test_user_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/seleniumWrapper/user_agents.py
--rw-r--r--   0 runner    (1001) docker     (127)    12308 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/seleniumWrapper/webdriver_chrome.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.021043 automonisaur-0.5.3/automon/integrations/sentryio/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/sentryio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/sentryio/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/sentryio/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.025043 automonisaur-0.5.3/automon/integrations/sentryio/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/sentryio/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/sentryio/tests/test_sentryio.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/sentryio/tests/test_sentryio_callback.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.025043 automonisaur-0.5.3/automon/integrations/shodan/
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/shodan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.025043 automonisaur-0.5.3/automon/integrations/shodan/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/shodan/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/shodan/tests/test_shodan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.025043 automonisaur-0.5.3/automon/integrations/slackWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/slackWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/slackWrapper/bots.py
--rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/slackWrapper/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5245 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/slackWrapper/clientAsync.py
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/slackWrapper/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/slackWrapper/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/slackWrapper/slack_formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)    11080 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/slackWrapper/slack_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.025043 automonisaur-0.5.3/automon/integrations/slackWrapper/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/slackWrapper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/slackWrapper/tests/test_slack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.025043 automonisaur-0.5.3/automon/integrations/snmp/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/snmp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16073 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/snmp/generate_maps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.025043 automonisaur-0.5.3/automon/integrations/splunk/
--rwxr-xr-x   0 runner    (1001) docker     (127)       66 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.025043 automonisaur-0.5.3/automon/integrations/splunk/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk/tests/test_splunk_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk/tests/test_splunk_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.029043 automonisaur-0.5.3/automon/integrations/splunk_soar/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/action_run.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/asset.py
--rw-r--r--   0 runner    (1001) docker     (127)    25563 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/container.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/datatypes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.029043 automonisaur-0.5.3/automon/integrations/splunk_soar/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.029043 automonisaur-0.5.3/automon/integrations/splunk_soar/integration/servicenow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/integration/servicenow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/integration/servicenow/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/integration/servicenow/ticket.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1731 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/phantom_unittest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/responses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.029043 automonisaur-0.5.3/automon/integrations/splunk_soar/rest/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14316 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/rest/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.033043 automonisaur-0.5.3/automon/integrations/splunk_soar/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   899665 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/tests/dino.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/tests/test_soar_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/tests/test_soar_client_create_container_attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/tests/test_soar_client_filter_vault.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/tests/test_soar_client_get_action_run.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/tests/test_soar_client_list_app_run.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/tests/test_soar_client_list_app_run_by_playbook_run.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/tests/test_soar_client_list_app_run_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/tests/test_soar_client_list_containers.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/tests/test_soar_client_list_vault.py
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/tests/test_soar_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/tests/test_soar_uat.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/tests/test_soar_uat_run_playbook.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/tests/test_soar_uat_update_playbook.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/splunk_soar/vault.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.033043 automonisaur-0.5.3/automon/integrations/swift/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/swift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17203 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/swift/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/swift/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/swift/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/swift/iterables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.033043 automonisaur-0.5.3/automon/integrations/swift/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/swift/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/swift/tests/test_swift.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.033043 automonisaur-0.5.3/automon/integrations/swimlaneWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/swimlaneWrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.033043 automonisaur-0.5.3/automon/integrations/swimlaneWrapper/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/swimlaneWrapper/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/swimlaneWrapper/api/v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7860 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/swimlaneWrapper/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/swimlaneWrapper/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.037043 automonisaur-0.5.3/automon/integrations/swimlaneWrapper/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/swimlaneWrapper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/swimlaneWrapper/tests/test_library_record_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/swimlaneWrapper/tests/test_rest_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/swimlaneWrapper/tests/test_rest_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/swimlaneWrapper/tests/test_rest_auth_token.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/swimlaneWrapper/tests/test_rest_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/swimlaneWrapper/tests/test_rest_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/swimlaneWrapper/tests/test_rest_record_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/swimlaneWrapper/tests/test_rest_record_delete_all.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/swimlaneWrapper/tests/test_rest_record_resolve_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/swimlaneWrapper/tests/test_rest_workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.037043 automonisaur-0.5.3/automon/integrations/vds/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/vds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/vds/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/vds/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.037043 automonisaur-0.5.3/automon/integrations/vds/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/vds/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/integrations/vds/tests/test_vds.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/liveliness.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.037043 automonisaur-0.5.3/automon/log/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1089 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/log/attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5568 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/log/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.037043 automonisaur-0.5.3/automon/log/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/log/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-15 18:06:19.000000 automonisaur-0.5.3/automon/log/tests/test_logger_builtin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:06:23.037043 automonisaur-0.5.3/automonisaur.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-05-15 18:06:22.000000 automonisaur-0.5.3/automonisaur.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16039 2024-05-15 18:06:22.000000 automonisaur-0.5.3/automonisaur.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 18:06:22.000000 automonisaur-0.5.3/automonisaur.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 18:06:22.000000 automonisaur-0.5.3/automonisaur.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 18:06:23.037043 automonisaur-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-15 18:06:19.000000 automonisaur-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.826220 automonisaur-0.5.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-28 19:19:32.000000 automonisaur-0.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-05-28 19:19:35.826220 automonisaur-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4333 2024-05-28 19:19:32.000000 automonisaur-0.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.782220 automonisaur-0.5.4/automon/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      105 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/healthcheck.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.782220 automonisaur-0.5.4/automon/helpers/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      204 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/helpers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1257 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/helpers/assertions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.782220 automonisaur-0.5.4/automon/helpers/asyncioWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/helpers/asyncioWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/helpers/asyncioWrapper/loop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.782220 automonisaur-0.5.4/automon/helpers/cryptography/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/helpers/cryptography/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/helpers/cryptography/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/helpers/cryptography/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/helpers/dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/helpers/httpWrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/helpers/markdown.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.786220 automonisaur-0.5.4/automon/helpers/mathWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/helpers/mathWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/helpers/mathWrapper/file_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/helpers/networking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.786220 automonisaur-0.5.4/automon/helpers/osWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/helpers/osWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/helpers/osWrapper/environ.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      338 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/helpers/regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4412 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/helpers/sanitation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/helpers/sleeper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.786220 automonisaur-0.5.4/automon/helpers/subprocessWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/helpers/subprocessWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/helpers/subprocessWrapper/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/helpers/subprocessWrapper/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.786220 automonisaur-0.5.4/automon/helpers/subprocessWrapper/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/helpers/subprocessWrapper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/helpers/subprocessWrapper/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/helpers/subprocessWrapper/tests/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/helpers/subprocessWrapper/tests/test_sanitize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/helpers/subprocessWrapper/tests/test_text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.786220 automonisaur-0.5.4/automon/helpers/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/helpers/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/helpers/tests/test_assertions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/helpers/tests/test_healthcheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/helpers/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/helpers/tests/test_liveliness.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/helpers/tests/test_networking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/helpers/tests/test_sanitation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/helpers/tests/test_sleeper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/helpers/tests/test_sleeper_async.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.786220 automonisaur-0.5.4/automon/helpers/threadingWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/helpers/threadingWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/helpers/threadingWrapper/initialize_threading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/helpers/threadingWrapper/worker_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.786220 automonisaur-0.5.4/automon/integrations/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       27 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.786220 automonisaur-0.5.4/automon/integrations/beautifulsoupWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/beautifulsoupWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/beautifulsoupWrapper/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.786220 automonisaur-0.5.4/automon/integrations/cryptocurrency/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/cryptocurrency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/cryptocurrency/accounting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/cryptocurrency/coinbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/cryptocurrency/other.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/cryptocurrency/robinhood.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.786220 automonisaur-0.5.4/automon/integrations/cryptocurrency/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/cryptocurrency/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/cryptocurrency/tests/test_crypto.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.790220 automonisaur-0.5.4/automon/integrations/datadogWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/datadogWrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.790220 automonisaur-0.5.4/automon/integrations/datadogWrapper/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/datadogWrapper/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/datadogWrapper/api/v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/datadogWrapper/api/v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/datadogWrapper/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/datadogWrapper/client_opentelemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/datadogWrapper/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/datadogWrapper/config_opentelemetry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.790220 automonisaur-0.5.4/automon/integrations/datadogWrapper/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/datadogWrapper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/datadogWrapper/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/datadogWrapper/tests/test_client_opentelemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/datadogWrapper/tests/test_config_opentelemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/datadogWrapper/tests/test_log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.790220 automonisaur-0.5.4/automon/integrations/datascience/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/datascience/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.790220 automonisaur-0.5.4/automon/integrations/datascience/pandas/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/datascience/pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/datascience/pandas/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/datascience/pandas/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/datascience/pandas/series.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.790220 automonisaur-0.5.4/automon/integrations/datascience/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/datascience/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/datascience/tests/test_datascience.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.790220 automonisaur-0.5.4/automon/integrations/elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/elasticsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/elasticsearch/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10557 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/elasticsearch/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/elasticsearch/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/elasticsearch/jvm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/elasticsearch/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5915 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/elasticsearch/snapshots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.790220 automonisaur-0.5.4/automon/integrations/elasticsearch/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/elasticsearch/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/elasticsearch/tests/test_elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/elasticsearch/tests/test_elasticsearch_JvmMonitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/elasticsearch/tests/test_elasticsearch_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/elasticsearch/tests/test_elasticsearch_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/elasticsearch/tests/test_elasticsearch_snapshot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.790220 automonisaur-0.5.4/automon/integrations/facebook/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/facebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22254 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/facebook/groups.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.794220 automonisaur-0.5.4/automon/integrations/flaskWrapper/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      106 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/flaskWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/flaskWrapper/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/flaskWrapper/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/flaskWrapper/auth_creds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/flaskWrapper/boilerplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/flaskWrapper/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/flaskWrapper/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.794220 automonisaur-0.5.4/automon/integrations/flaskWrapper/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/flaskWrapper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/flaskWrapper/tests/test_flask.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/flaskWrapper/tests/test_run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.794220 automonisaur-0.5.4/automon/integrations/geoip/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/geoip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.794220 automonisaur-0.5.4/automon/integrations/geoip/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/geoip/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/geoip/tests/test_geoip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.794220 automonisaur-0.5.4/automon/integrations/google/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/google/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.794220 automonisaur-0.5.4/automon/integrations/google/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/google/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/google/auth/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/google/auth/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.794220 automonisaur-0.5.4/automon/integrations/google/auth/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/google/auth/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/google/auth/tests/test_config_Credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/google/auth/tests/test_google_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.794220 automonisaur-0.5.4/automon/integrations/google/gmail/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/google/gmail/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.794220 automonisaur-0.5.4/automon/integrations/google/gmail/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/google/gmail/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/google/gmail/v1/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/google/gmail/v1/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.794220 automonisaur-0.5.4/automon/integrations/google/people/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/google/people/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/google/people/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7322 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/google/people/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11001 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/google/people/person.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/google/people/results.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.794220 automonisaur-0.5.4/automon/integrations/google/people/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/google/people/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/google/people/tests/test_google_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/google/people/tests/test_google_contacts_neo4j.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/google/people/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.798220 automonisaur-0.5.4/automon/integrations/google/sheets/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/google/sheets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/google/sheets/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/google/sheets/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.798220 automonisaur-0.5.4/automon/integrations/google/sheets/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/google/sheets/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11366 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/google/sheets/tests/test_google_sheets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/google/sheets/tests/test_google_sheets_AUDIT.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/google/sheets/tests/test_google_sheets_clear.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.798220 automonisaur-0.5.4/automon/integrations/google/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/google/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/google/tests/test_google_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/google/tests/test_google_contacts_neo4j.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.798220 automonisaur-0.5.4/automon/integrations/grok/
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/grok/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.798220 automonisaur-0.5.4/automon/integrations/grok/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/grok/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/grok/tests/test_grok.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.798220 automonisaur-0.5.4/automon/integrations/instagram/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/instagram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/instagram/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8593 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/instagram/client_browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/instagram/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7666 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/instagram/stories.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.798220 automonisaur-0.5.4/automon/integrations/instagram/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/instagram/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/instagram/tests/test_instagram.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/instagram/tests/test_instagram_browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/instagram/tests/test_instagram_browser_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/instagram/tests/test_instagram_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/instagram/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/instagram/xpaths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.798220 automonisaur-0.5.4/automon/integrations/ldap/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/ldap/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3523 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/ldap/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.798220 automonisaur-0.5.4/automon/integrations/mac/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       93 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/mac/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.802220 automonisaur-0.5.4/automon/integrations/mac/airport/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/mac/airport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6393 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/mac/airport/airport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/mac/airport/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/mac/airport/ssid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.802220 automonisaur-0.5.4/automon/integrations/mac/airport/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/mac/airport/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/mac/airport/tests/test_airport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/mac/airport/tests/test_airport_neo4j.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/mac/check.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.802220 automonisaur-0.5.4/automon/integrations/mac/macchanger/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/mac/macchanger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/mac/macchanger/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.802220 automonisaur-0.5.4/automon/integrations/mac/macchanger/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/mac/macchanger/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/mac/macchanger/tests/test_macchanger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/mac/macchanger/tests/test_set_mac_random.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.802220 automonisaur-0.5.4/automon/integrations/mac/wdutil/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/mac/wdutil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/mac/wdutil/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/mac/wdutil/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/mac/wdutil/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.802220 automonisaur-0.5.4/automon/integrations/mac/wdutil/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/mac/wdutil/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/mac/wdutil/tests/test_client_ready.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/mac/wdutil/tests/test_client_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/mac/wdutil/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/mac/wdutil/tests/test_wdutil.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.802220 automonisaur-0.5.4/automon/integrations/minioWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/minioWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/minioWrapper/assertions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/minioWrapper/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7849 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/minioWrapper/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/minioWrapper/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/minioWrapper/object.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.806220 automonisaur-0.5.4/automon/integrations/minioWrapper/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/minioWrapper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/minioWrapper/tests/test_minio_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/minioWrapper/tests/test_minio_client_public.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/minioWrapper/tests/test_minio_client_public_clear_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/minioWrapper/tests/test_minio_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.806220 automonisaur-0.5.4/automon/integrations/neo4jWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/neo4jWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6389 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/neo4jWrapper/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/neo4jWrapper/clientAsync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/neo4jWrapper/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11026 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/neo4jWrapper/cypher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/neo4jWrapper/results.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.806220 automonisaur-0.5.4/automon/integrations/neo4jWrapper/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/neo4jWrapper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/neo4jWrapper/tests/test_neo4j_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/neo4jWrapper/tests/test_neo4j_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/neo4jWrapper/tests/test_neo4j_cypher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.806220 automonisaur-0.5.4/automon/integrations/nest_asyncioWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/nest_asyncioWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/nest_asyncioWrapper/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.806220 automonisaur-0.5.4/automon/integrations/nmap/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/nmap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/nmap/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/nmap/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/nmap/output.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.806220 automonisaur-0.5.4/automon/integrations/nmap/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/nmap/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/nmap/tests/test_nmap_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/nmap/tests/test_nmap_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.806220 automonisaur-0.5.4/automon/integrations/openTelemetryWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/openTelemetryWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/openTelemetryWrapper/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/openTelemetryWrapper/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.810220 automonisaur-0.5.4/automon/integrations/openTelemetryWrapper/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/openTelemetryWrapper/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/openTelemetryWrapper/test/test_client_ready.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/openTelemetryWrapper/test/test_memory_trace_client_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/openTelemetryWrapper/test/test_memory_trace_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/openTelemetryWrapper/test/test_pop_finished_spans.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.810220 automonisaur-0.5.4/automon/integrations/openvpn/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/openvpn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6982 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/openvpn/openvpn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.810220 automonisaur-0.5.4/automon/integrations/psutilWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/psutilWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/psutilWrapper/cpu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.810220 automonisaur-0.5.4/automon/integrations/requestsWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/requestsWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6564 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/requestsWrapper/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/requestsWrapper/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/requestsWrapper/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.810220 automonisaur-0.5.4/automon/integrations/requestsWrapper/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/requestsWrapper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/requestsWrapper/tests/test_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/requestsWrapper/tests/test_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/requestsWrapper/tests/test_rest_inherit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.810220 automonisaur-0.5.4/automon/integrations/scrapyWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/scrapyWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/scrapyWrapper/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.810220 automonisaur-0.5.4/automon/integrations/seleniumWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/seleniumWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/seleniumWrapper/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19858 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/seleniumWrapper/browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/seleniumWrapper/browser_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/seleniumWrapper/browser_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/seleniumWrapper/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/seleniumWrapper/config_window_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/seleniumWrapper/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.814220 automonisaur-0.5.4/automon/integrations/seleniumWrapper/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/seleniumWrapper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/seleniumWrapper/tests/test_browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/seleniumWrapper/tests/test_browser_cookies_autosave.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/seleniumWrapper/tests/test_browser_headless.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/seleniumWrapper/tests/test_browser_useragent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/seleniumWrapper/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/seleniumWrapper/tests/test_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/seleniumWrapper/tests/test_new_browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/seleniumWrapper/tests/test_user_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/seleniumWrapper/user_agents.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12452 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/seleniumWrapper/webdriver_chrome.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.814220 automonisaur-0.5.4/automon/integrations/sentryio/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/sentryio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/sentryio/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/sentryio/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.814220 automonisaur-0.5.4/automon/integrations/sentryio/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/sentryio/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/sentryio/tests/test_sentryio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/sentryio/tests/test_sentryio_callback.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.814220 automonisaur-0.5.4/automon/integrations/shodan/
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/shodan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.814220 automonisaur-0.5.4/automon/integrations/shodan/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/shodan/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/shodan/tests/test_shodan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.814220 automonisaur-0.5.4/automon/integrations/slackWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/slackWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/slackWrapper/bots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/slackWrapper/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5245 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/slackWrapper/clientAsync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/slackWrapper/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/slackWrapper/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/slackWrapper/slack_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11080 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/slackWrapper/slack_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.814220 automonisaur-0.5.4/automon/integrations/slackWrapper/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/slackWrapper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/slackWrapper/tests/test_slack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.814220 automonisaur-0.5.4/automon/integrations/snmp/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/snmp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16073 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/snmp/generate_maps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.814220 automonisaur-0.5.4/automon/integrations/splunk/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       66 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/splunk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/splunk/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/splunk/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/splunk/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.818220 automonisaur-0.5.4/automon/integrations/splunk/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/splunk/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/splunk/tests/test_splunk_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/splunk/tests/test_splunk_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.818220 automonisaur-0.5.4/automon/integrations/splunk_soar/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/splunk_soar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/splunk_soar/action_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/splunk_soar/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/splunk_soar/asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25543 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/splunk_soar/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/splunk_soar/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/splunk_soar/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/splunk_soar/datatypes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.818220 automonisaur-0.5.4/automon/integrations/splunk_soar/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/splunk_soar/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.818220 automonisaur-0.5.4/automon/integrations/splunk_soar/integration/servicenow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/splunk_soar/integration/servicenow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/splunk_soar/integration/servicenow/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/splunk_soar/integration/servicenow/ticket.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1731 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/splunk_soar/phantom_unittest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/splunk_soar/responses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.818220 automonisaur-0.5.4/automon/integrations/splunk_soar/rest/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/splunk_soar/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14316 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/splunk_soar/rest/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/splunk_soar/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.822220 automonisaur-0.5.4/automon/integrations/splunk_soar/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/splunk_soar/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   899665 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/splunk_soar/tests/dino.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/splunk_soar/tests/test_soar_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/splunk_soar/tests/test_soar_client_create_container_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/splunk_soar/tests/test_soar_client_filter_vault.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/splunk_soar/tests/test_soar_client_get_action_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/splunk_soar/tests/test_soar_client_list_app_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/splunk_soar/tests/test_soar_client_list_app_run_by_playbook_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/splunk_soar/tests/test_soar_client_list_app_run_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/splunk_soar/tests/test_soar_client_list_containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/splunk_soar/tests/test_soar_client_list_vault.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/splunk_soar/tests/test_soar_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/splunk_soar/tests/test_soar_uat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/splunk_soar/tests/test_soar_uat_run_playbook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/splunk_soar/tests/test_soar_uat_update_playbook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/splunk_soar/vault.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.822220 automonisaur-0.5.4/automon/integrations/swift/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/swift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17203 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/swift/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/swift/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/swift/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/swift/iterables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.822220 automonisaur-0.5.4/automon/integrations/swift/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/swift/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/swift/tests/test_swift.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.822220 automonisaur-0.5.4/automon/integrations/swimlaneWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/swimlaneWrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.822220 automonisaur-0.5.4/automon/integrations/swimlaneWrapper/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/swimlaneWrapper/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/swimlaneWrapper/api/v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7860 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/swimlaneWrapper/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/swimlaneWrapper/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.826220 automonisaur-0.5.4/automon/integrations/swimlaneWrapper/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/swimlaneWrapper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/swimlaneWrapper/tests/test_library_record_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/swimlaneWrapper/tests/test_rest_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/swimlaneWrapper/tests/test_rest_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/swimlaneWrapper/tests/test_rest_auth_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/swimlaneWrapper/tests/test_rest_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/swimlaneWrapper/tests/test_rest_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/swimlaneWrapper/tests/test_rest_record_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/swimlaneWrapper/tests/test_rest_record_delete_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/swimlaneWrapper/tests/test_rest_record_resolve_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/swimlaneWrapper/tests/test_rest_workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.826220 automonisaur-0.5.4/automon/integrations/vds/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/vds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/vds/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/vds/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.826220 automonisaur-0.5.4/automon/integrations/vds/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/vds/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/integrations/vds/tests/test_vds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/liveliness.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.826220 automonisaur-0.5.4/automon/log/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1120 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/log/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5689 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/log/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.826220 automonisaur-0.5.4/automon/log/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/log/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/log/tests/test_log_secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-28 19:19:32.000000 automonisaur-0.5.4/automon/log/tests/test_logger_builtin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:19:35.826220 automonisaur-0.5.4/automonisaur.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-05-28 19:19:35.000000 automonisaur-0.5.4/automonisaur.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16844 2024-05-28 19:19:35.000000 automonisaur-0.5.4/automonisaur.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 19:19:35.000000 automonisaur-0.5.4/automonisaur.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-28 19:19:35.000000 automonisaur-0.5.4/automonisaur.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 19:19:35.826220 automonisaur-0.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-28 19:19:32.000000 automonisaur-0.5.4/setup.py
```

### Comparing `automonisaur-0.5.3/LICENSE` & `automonisaur-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/PKG-INFO` & `automonisaur-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automonisaur
-Version: 0.5.3
+Version: 0.5.4
 Summary: Core libraries for automonisaur
 Home-page: https://github.com/TheShellLand/automonisaur
 Author: naisanza
 Author-email: naisanza@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -59,15 +59,15 @@
 | Data Scraping   | beautifulsoup<br/>facebook groups<br/>instagram<br/>scrapy  |
 | Databases       | elasticsearch<br/>neo4j<br/>splunk                          |
 | Data Store      | minio<br/>swift                                             |
 | Devices         | snmp                                                        |
 | Google Cloud    | google auth api<br/>google people api<br/>google sheets api |
 | Helpers         | os<br/>subprocess<br/>threading<br/>socket<br/>datetime     |
 | Logging         | sentryio                                                    |
-| MacOS           | airport<br/>macchanger                                      |
+| MacOS           | airport<br/>macchanger<br/>wdutil                           |
 | Python          | logging<br/>requests                                        |
 | SOAR            | swimlane<br/>splunk soar                                    |
 | Recon           | nmap                                                        |
 | Test Automation | selenium                                                    |
 
 #### Requires
```

### Comparing `automonisaur-0.5.3/README.md` & `automonisaur-0.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 | Data Scraping   | beautifulsoup<br/>facebook groups<br/>instagram<br/>scrapy  |
 | Databases       | elasticsearch<br/>neo4j<br/>splunk                          |
 | Data Store      | minio<br/>swift                                             |
 | Devices         | snmp                                                        |
 | Google Cloud    | google auth api<br/>google people api<br/>google sheets api |
 | Helpers         | os<br/>subprocess<br/>threading<br/>socket<br/>datetime     |
 | Logging         | sentryio                                                    |
-| MacOS           | airport<br/>macchanger                                      |
+| MacOS           | airport<br/>macchanger<br/>wdutil                           |
 | Python          | logging<br/>requests                                        |
 | SOAR            | swimlane<br/>splunk soar                                    |
 | Recon           | nmap                                                        |
 | Test Automation | selenium                                                    |
 
 #### Requires
```

### Comparing `automonisaur-0.5.3/automon/helpers/assertions.py` & `automonisaur-0.5.4/automon/helpers/assertions.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/helpers/markdown.py` & `automonisaur-0.5.4/automon/helpers/markdown.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/helpers/networking.py` & `automonisaur-0.5.4/automon/helpers/networking.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/helpers/osWrapper/environ.py` & `automonisaur-0.5.4/automon/helpers/osWrapper/environ.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/helpers/sanitation.py` & `automonisaur-0.5.4/automon/helpers/sanitation.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/helpers/sleeper.py` & `automonisaur-0.5.4/automon/helpers/sleeper.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/helpers/subprocessWrapper/run.py` & `automonisaur-0.5.4/automon/helpers/subprocessWrapper/run.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,23 +56,29 @@
         logger.debug(command)
         if command:
             self.command = command
             return True
         return False
 
     @property
-    def stdout(self):
+    def stdout(self) -> bytes:
+        if type(self._stdout) is str:
+            return str(self._stdout).encode()
+
         return self._stdout
 
     @property
     def stdout_lines(self):
         return self.stdout.decode().splitlines()
 
     @property
-    def stderr(self):
+    def stderr(self) -> bytes:
+        if type(self._stderr) is str:
+            return str(self._stderr).encode()
+
         return self._stderr
 
     @property
     def stderr_lines(self):
         return self.stderr.decode().splitlines()
 
     def which(self, program: str, *args, **kwargs) -> bool:
```

### Comparing `automonisaur-0.5.3/automon/helpers/subprocessWrapper/tests/test_runner.py` & `automonisaur-0.5.4/automon/helpers/subprocessWrapper/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/helpers/tests/test_assertions.py` & `automonisaur-0.5.4/automon/helpers/tests/test_assertions.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/helpers/tests/test_networking.py` & `automonisaur-0.5.4/automon/helpers/tests/test_networking.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/helpers/tests/test_sanitation.py` & `automonisaur-0.5.4/automon/helpers/tests/test_sanitation.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/helpers/tests/test_sleeper.py` & `automonisaur-0.5.4/automon/helpers/tests/test_sleeper.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/helpers/threadingWrapper/initialize_threading.py` & `automonisaur-0.5.4/automon/helpers/threadingWrapper/initialize_threading.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/helpers/threadingWrapper/worker_thread.py` & `automonisaur-0.5.4/automon/helpers/threadingWrapper/worker_thread.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/beautifulsoupWrapper/client.py` & `automonisaur-0.5.4/automon/integrations/beautifulsoupWrapper/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/cryptocurrency/accounting.py` & `automonisaur-0.5.4/automon/integrations/cryptocurrency/accounting.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/cryptocurrency/coinbase.py` & `automonisaur-0.5.4/automon/integrations/cryptocurrency/coinbase.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/cryptocurrency/other.py` & `automonisaur-0.5.4/automon/integrations/cryptocurrency/other.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/cryptocurrency/robinhood.py` & `automonisaur-0.5.4/automon/integrations/cryptocurrency/robinhood.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/cryptocurrency/tests/test_crypto.py` & `automonisaur-0.5.4/automon/integrations/cryptocurrency/tests/test_crypto.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/datadogWrapper/client.py` & `automonisaur-0.5.4/automon/integrations/datadogWrapper/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from automon.integrations.requestsWrapper import RequestsClient
-from automon.log import logging
+from automon import log
 
 from .config import DatadogConfigRest
 from .api import V1, V2
 
-logger = logging.getLogger(__name__)
-logger.setLevel(logging.DEBUG)
+logger = log.logging.getLogger(__name__)
+logger.setLevel(log.logging.DEBUG)
 
 
 class DatadogClientRest(object):
 
     def __init__(self, host: str = None, api_key: str = None):
         self.config = DatadogConfigRest(host=host, api_key=api_key)
         self.requests = RequestsClient()
```

### Comparing `automonisaur-0.5.3/automon/integrations/datadogWrapper/client_opentelemetry.py` & `automonisaur-0.5.4/automon/integrations/datadogWrapper/client_opentelemetry.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from automon.log import logging
+from automon import log
 
 from .config_opentelemetry import DatadogOpenTelemetryConfig
 
-logger = logging.getLogger(__name__)
-logger.setLevel(logging.DEBUG)
+logger = log.logging.getLogger(__name__)
+logger.setLevel(log.logging.DEBUG)
 
 
 class DatadogOpenTelemetryClient(object):
 
     def __init__(self, host: str = None, api_key: str = None, app_key: str = None):
         self.config = DatadogOpenTelemetryConfig(host=host, api_key=api_key, app_key=app_key)
```

### Comparing `automonisaur-0.5.3/automon/integrations/datadogWrapper/config.py` & `automonisaur-0.5.4/automon/integrations/datadogWrapper/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from automon import environ
-from automon.log import logging
+from automon import log
 
-logger = logging.getLogger(__name__)
-logger.setLevel(logging.DEBUG)
+logger = log.logging.getLogger(__name__)
+logger.setLevel(log.logging.DEBUG)
 
 
 class DatadogConfigRest(object):
     api_key: str
 
     def __init__(self, host: str = 'https://api.datadoghq.com', api_key: str = None, app_key: str = None):
         self.host = host or environ('DD_SITE')
```

### Comparing `automonisaur-0.5.3/automon/integrations/datadogWrapper/config_opentelemetry.py` & `automonisaur-0.5.4/automon/integrations/datadogWrapper/config_opentelemetry.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 import opentelemetry
 from opentelemetry.trace import set_tracer_provider
 
 from automon import environ
-from automon.log import logging
+from automon import log
 
-logger = logging.getLogger(__name__)
-logger.setLevel(logging.DEBUG)
+logger = log.logging.getLogger(__name__)
+logger.setLevel(log.logging.DEBUG)
 
 
 class DatadogOpenTelemetryConfig(object):
 
     def __init__(self, host: str = 'https://api.datadoghq.com', api_key: str = None, app_key: str = None):
         self.host = host or environ('DD_SITE')
         self.api_key = api_key or environ('DD_API_KEY')
```

### Comparing `automonisaur-0.5.3/automon/integrations/datadogWrapper/tests/test_log.py` & `automonisaur-0.5.4/automon/integrations/datadogWrapper/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/datascience/pandas/pandas.py` & `automonisaur-0.5.4/automon/integrations/datascience/pandas/pandas.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/datascience/tests/test_datascience.py` & `automonisaur-0.5.4/automon/integrations/datascience/tests/test_datascience.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/elasticsearch/cleanup.py` & `automonisaur-0.5.4/automon/integrations/elasticsearch/cleanup.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/elasticsearch/client.py` & `automonisaur-0.5.4/automon/integrations/elasticsearch/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/elasticsearch/config.py` & `automonisaur-0.5.4/automon/integrations/elasticsearch/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import os
-import logging
 
 from automon import log
 from automon.helpers.sanitation import Sanitation as S
 
 logger = log.logging.getLogger(__name__)
 logger.setLevel(log.DEBUG)
 
-logging.getLogger('elasticsearch').setLevel(logging.ERROR)
-logging.getLogger('urllib3.connectionpool').setLevel(logging.ERROR)
+log.logging.getLogger('elasticsearch').setLevel(log.logging.ERROR)
+log.logging.getLogger('urllib3.connectionpool').setLevel(log.logging.ERROR)
 
 
 class ElasticsearchConfig:
 
     def __init__(self, host: str = None,
                  cloud_id: str = None,
                  user: str = '',
```

### Comparing `automonisaur-0.5.3/automon/integrations/elasticsearch/jvm.py` & `automonisaur-0.5.4/automon/integrations/elasticsearch/jvm.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/elasticsearch/metrics.py` & `automonisaur-0.5.4/automon/integrations/elasticsearch/metrics.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/elasticsearch/snapshots.py` & `automonisaur-0.5.4/automon/integrations/elasticsearch/snapshots.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/elasticsearch/tests/test_elasticsearch.py` & `automonisaur-0.5.4/automon/integrations/elasticsearch/tests/test_elasticsearch.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/elasticsearch/tests/test_elasticsearch_JvmMonitor.py` & `automonisaur-0.5.4/automon/integrations/elasticsearch/tests/test_elasticsearch_JvmMonitor.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/elasticsearch/tests/test_elasticsearch_snapshot.py` & `automonisaur-0.5.4/automon/integrations/elasticsearch/tests/test_elasticsearch_snapshot.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/facebook/groups.py` & `automonisaur-0.5.4/automon/integrations/facebook/groups.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/flaskWrapper/auth.py` & `automonisaur-0.5.4/automon/integrations/flaskWrapper/auth.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/flaskWrapper/boilerplate.py` & `automonisaur-0.5.4/automon/integrations/flaskWrapper/boilerplate.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/flaskWrapper/tests/test_flask.py` & `automonisaur-0.5.4/automon/integrations/flaskWrapper/tests/test_flask.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/google/auth/client.py` & `automonisaur-0.5.4/automon/integrations/google/auth/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/google/auth/config.py` & `automonisaur-0.5.4/automon/integrations/google/auth/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/google/gmail/v1/client.py` & `automonisaur-0.5.4/automon/integrations/google/gmail/v1/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/google/gmail/v1/config.py` & `automonisaur-0.5.4/automon/integrations/google/gmail/v1/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/google/people/client.py` & `automonisaur-0.5.4/automon/integrations/google/people/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/google/people/config.py` & `automonisaur-0.5.4/automon/integrations/google/people/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,28 +188,28 @@
                     token_uri=self.token_uri,
                     auth_provider_x509_cert_url=self.auth_provider_x509_cert_url,
                     client_secret=self.client_secret,
                     redirect_uris=self.redirect_uris
                 )
             }
 
-        logger.warning(f'Missing client_type')
-        return False
+        logger.error(f'Missing client_type')
+        return {}
 
     def from_authorized_user_file(self, file: str) -> Credentials:
         """Load token.json"""
         return self.Credentials.from_authorized_user_file(file, self.scopes)
 
     def isReady(self):
         if self.client_type:
             return True
         if self.oauth_dict():
             return True
 
-        logger.warning(f'config is not ready')
+        logger.error(f'config is not ready')
         return False
 
     def load_oauth(self, oauth: dict) -> Credentials:
         if 'installed' in oauth.keys():
             oauth = oauth['installed']
             self._client_type = 'installed'
             return self.update(oauth)
```

### Comparing `automonisaur-0.5.3/automon/integrations/google/people/person.py` & `automonisaur-0.5.4/automon/integrations/google/people/person.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 from automon import log
 
 logger = log.logging.getLogger(__name__)
 logger.setLevel(log.DEBUG)
 
 
 class AgeRange(Enum):
-    """Please use person.ageRanges instead"""
-    logger.warning(DeprecationWarning)
+    logger.warning(DeprecationWarning(f'Depreciated AgeRange, please use person.ageRanges instead'))
 
     AGE_RANGE_UNSPECIFIED = 'AGE_RANGE_UNSPECIFIED'
     LESS_THAN_EIGHTEEN = 'LESS_THAN_EIGHTEEN'
     EIGHTEEN_TO_TWENTY = 'EIGHTEEN_TO_TWENTY'
     TWENTY_ONE_OR_OLDER = 'TWENTY_ONE_OR_OLDER'
 
 
@@ -390,35 +389,35 @@
     }
     person: str
     type: str
     formattedType: str
 
 
 class RelationshipInterest(object):
-    logger.warning(DeprecationWarning)
+    logger.warning(DeprecationWarning('Depreciated RelationshipInterest'))
 
     metadata: {
         FieldMetadata
     }
     value: str
     formattedValue: str
 
 
 class RelationshipStatus(object):
-    logger.warning(DeprecationWarning)
+    logger.warning(DeprecationWarning('Depreciated RelationshipStatus'))
 
     metadata: {
         FieldMetadata
     }
     value: str
     formattedValue: str
 
 
 class Residence(object):
-    logger.warning(DeprecationWarning)
+    logger.warning(DeprecationWarning('Depreciated Residence'))
 
     metadata: {
         FieldMetadata
     }
     value: str
     current: bool
 
@@ -436,15 +435,15 @@
     metadata: {
         FieldMetadata
     }
     value: str
 
 
 class Tagline(object):
-    logger.warning(DeprecationWarning)
+    logger.warning(DeprecationWarning('Depreciated Tagline'))
 
     metadata: {
         FieldMetadata
     }
     value: str
```

### Comparing `automonisaur-0.5.3/automon/integrations/google/people/results.py` & `automonisaur-0.5.4/automon/integrations/google/people/results.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/google/people/urls.py` & `automonisaur-0.5.4/automon/integrations/google/people/urls.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/google/sheets/client.py` & `automonisaur-0.5.4/automon/integrations/google/sheets/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/google/sheets/config.py` & `automonisaur-0.5.4/automon/integrations/google/sheets/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/google/sheets/tests/test_google_sheets.py` & `automonisaur-0.5.4/automon/integrations/google/sheets/tests/test_google_sheets.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 import profile
 import asyncio
-import logging
 import datetime
 import tracemalloc
 
 import pandas as pd
 import numpy as np
 
-from automon.log import logger
+from automon import log
 from automon.helpers.sleeper import Sleeper
 from automon.integrations.facebook import FacebookGroups
 from automon.integrations.google.sheets import GoogleSheetsClient
 
-logging.getLogger('google_auth_httplib2').setLevel(logging.ERROR)
-logging.getLogger('googleapiclient.discovery').setLevel(logging.ERROR)
-logging.getLogger('googleapiclient.discovery_cache').setLevel(logging.ERROR)
-logging.getLogger('urllib3.connectionpool').setLevel(logging.ERROR)
-logging.getLogger('selenium.webdriver.common.service').setLevel(logging.ERROR)
-logging.getLogger('selenium.webdriver.remote.remote_connection').setLevel(logging.ERROR)
-logging.getLogger('selenium.webdriver.common.selenium_manager').setLevel(logging.ERROR)
-
-logging.getLogger('automon.integrations.seleniumWrapper.browser').setLevel(logging.CRITICAL)
-logging.getLogger('automon.integrations.seleniumWrapper.webdriver_chrome').setLevel(logging.INFO)
-logging.getLogger('automon.integrations.google.sheets.client').setLevel(logging.INFO)
-logging.getLogger('automon.integrations.facebook.groups').setLevel(logging.DEBUG)
-logging.getLogger('automon.integrations.requestsWrapper.client').setLevel(logging.INFO)
-logging.getLogger('automon.helpers.sleeper').setLevel(logging.INFO)
+log.logging.getLogger('google_auth_httplib2').setLevel(log.logging.ERROR)
+log.logging.getLogger('googleapiclient.discovery').setLevel(log.logging.ERROR)
+log.logging.getLogger('googleapiclient.discovery_cache').setLevel(log.logging.ERROR)
+log.logging.getLogger('urllib3.connectionpool').setLevel(log.logging.ERROR)
+log.logging.getLogger('selenium.webdriver.common.service').setLevel(log.logging.ERROR)
+log.logging.getLogger('selenium.webdriver.remote.remote_connection').setLevel(log.logging.ERROR)
+log.logging.getLogger('selenium.webdriver.common.selenium_manager').setLevel(log.logging.ERROR)
+
+log.logging.getLogger('automon.integrations.seleniumWrapper.browser').setLevel(log.logging.CRITICAL)
+log.logging.getLogger('automon.integrations.seleniumWrapper.webdriver_chrome').setLevel(log.logging.INFO)
+log.logging.getLogger('automon.integrations.google.sheets.client').setLevel(log.logging.INFO)
+log.logging.getLogger('automon.integrations.facebook.groups').setLevel(log.logging.DEBUG)
+log.logging.getLogger('automon.integrations.requestsWrapper.client').setLevel(log.logging.INFO)
+log.logging.getLogger('automon.helpers.sleeper').setLevel(log.logging.INFO)
 
 tracemalloc.start()
 
-log = logger.logging.getLogger(__name__)
-log.setLevel(logger.DEBUG)
+logger = log.logging.getLogger(__name__)
+logger.setLevel(log.DEBUG)
 
 SHEET_NAME = 'Automated Count DO NOT EDIT'
 SHEET_NAME_INGEST = 'URLS TO INGEST'
 
 sheets_client = GoogleSheetsClient(
     worksheet=SHEET_NAME,
 )
@@ -56,15 +55,15 @@
     await facebook_group_client.set_url(url=url)
 
     try:
         result = await facebook_group_client.get_about(rate_limiting=False)
         dict = await facebook_group_client.to_dict()
         await facebook_group_client.quit()
     except Exception as e:
-        log.error(f'{e}')
+        logger.error(f'{e}')
 
     return dict
 
 
 async def url_cleaner(url: str):
     if not url:
         return
@@ -188,15 +187,15 @@
     )
 
     update = await sheets_client.update(
         range=f'{SHEET_NAME}!A{sheet_index_df}:Z',
         values=[x for x in df.values.tolist()]
     )
 
-    log.info(f'{sheet_index_df}: {[x for x in df.values.tolist()]}')
+    logger.info(f'{sheet_index_df}: {[x for x in df.values.tolist()]}')
 
     return df
 
 
 async def memory_profiler():
     snapshot = tracemalloc.take_snapshot()
     top_stats = snapshot.statistics("lineno")
@@ -212,15 +211,15 @@
     df_memory_profile['size_MB'] = df_memory_profile['size_KB'].apply(
         lambda KB: round(KB / 1024)
     )
     cols = df_memory_profile.columns.tolist()
     cols.sort()
     df_memory_profile = df_memory_profile.loc[:, cols]
 
-    log.debug(
+    logger.debug(
         f"total memory used: {df_memory_profile['size_MB'].sum()} MB; "
         f'most memory used: '
         f'{df_memory_profile.iloc[0].to_dict()}'
     )
 
     return df_memory_profile
 
@@ -278,15 +277,15 @@
         duplicate_index, duplicate_row = duplicate
 
         # clear row in sheet
         data_range = f'{SHEET_NAME}!{duplicate_index}:{duplicate_index}'
         result = await sheets_client.clear(range=data_range)
         # max 60/min
         Sleeper.seconds(f'WriteRequestsPerMinutePerUser', seconds=1)
-        log.info(result)
+        logger.info(result)
         df = df.drop(duplicate_index)
 
     # ingest urls from SHEET_NAME_INGEST
     await sheets_client.get_values(
         range=f'{SHEET_NAME_INGEST}!A:Z'
     )
     ingest_sheet_values = sheets_client.values
@@ -310,22 +309,22 @@
             values = [[x for x in df.loc[index_add_url].values.tolist()]]
 
             update = await sheets_client.update(
                 range=f'{SHEET_NAME}!A{index_add_url}:Z',
                 values=values
             )
 
-            log.info(
+            logger.info(
                 f'{index_add_url}: {values}'
             )
 
         # clear url from ingest sheet
         data_range = f'{SHEET_NAME_INGEST}!{ingest_index}:{ingest_index}'
         clear = await sheets_client.clear(range=data_range)
-        log.info(f'{clear}')
+        logger.info(f'{clear}')
 
     return df
 
 
 async def main():
     df = await expensive_state_keeping()
 
@@ -340,18 +339,18 @@
         last_updated = f'{todays_date.year}-{todays_date.month}'
         if df_batch['last_updated'].iloc[0] == last_updated:
             # log.debug(f'skipping {data_index}, {data_row.to_dict()}')
             # df = expensive_state_keeping()
             continue
 
         try:
-            log.info(f'complete {round(data_index / len(df) * 100)}% {data_index}/{len(df)}')
+            logger.info(f'complete {round(data_index / len(df) * 100)}% {data_index}/{len(df)}')
             batch_result = await batch_processing(sheet_index=data_index, df=df_batch)
         except Exception as error:
-            log.error(f'{error}')
+            logger.error(f'{error}')
         df_memory = await memory_profiler()
 
 
 if __name__ == '__main__':
     # loop = asyncio.get_event_loop()
     # loop.run_until_complete(main())
     asyncio.run(main())
```

### Comparing `automonisaur-0.5.3/automon/integrations/google/sheets/tests/test_google_sheets_AUDIT.py` & `automonisaur-0.5.4/automon/integrations/google/sheets/tests/test_google_sheets_AUDIT.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/google/sheets/tests/test_google_sheets_clear.py` & `automonisaur-0.5.4/automon/integrations/google/sheets/tests/test_google_sheets_clear.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/grok/__init__.py` & `automonisaur-0.5.4/automon/integrations/grok/__init__.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/instagram/client.py` & `automonisaur-0.5.4/automon/integrations/instagram/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/instagram/client_browser.py` & `automonisaur-0.5.4/automon/integrations/instagram/client_browser.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/instagram/config.py` & `automonisaur-0.5.4/automon/integrations/instagram/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,23 +17,22 @@
             login=self.login,
             password="*" * len(self.password) if self.password else ''
         ))
 
     @property
     def login(self):
         if not self._login:
-            logger.error(f'INSTAGRAM_LOGIN')
+            logger.error(f'missing INSTAGRAM_LOGIN')
         return self._login
 
     @property
     def password(self):
         if not self._password:
-            logger.error(f'INSTAGRAM_PASSWORD')
+            logger.error(f'missing INSTAGRAM_PASSWORD')
         return self._password
 
     @property
     def is_configured(self):
         if self.login and self.password:
-            logger.info(f'{True}')
             return True
-        logger.error(f'{False}')
+        logger.error(f'not configured')
         return False
```

### Comparing `automonisaur-0.5.3/automon/integrations/instagram/stories.py` & `automonisaur-0.5.4/automon/integrations/instagram/stories.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/instagram/tests/test_instagram_browser.py` & `automonisaur-0.5.4/automon/integrations/instagram/tests/test_instagram_browser.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/instagram/tests/test_instagram_browser_auth.py` & `automonisaur-0.5.4/automon/integrations/instagram/tests/test_instagram_browser_auth.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/instagram/xpaths.py` & `automonisaur-0.5.4/automon/integrations/instagram/xpaths.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/ldap/client.py` & `automonisaur-0.5.4/automon/integrations/ldap/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/mac/airport/airport.py` & `automonisaur-0.5.4/automon/integrations/mac/airport/airport.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/mac/airport/scan.py` & `automonisaur-0.5.4/automon/integrations/mac/airport/scan.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/mac/airport/ssid.py` & `automonisaur-0.5.4/automon/integrations/mac/airport/ssid.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/mac/airport/tests/test_airport.py` & `automonisaur-0.5.4/automon/integrations/mac/airport/tests/test_airport.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/mac/airport/tests/test_airport_neo4j.py` & `automonisaur-0.5.4/automon/integrations/mac/airport/tests/test_airport_neo4j.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/mac/macchanger/client.py` & `automonisaur-0.5.4/automon/integrations/mac/macchanger/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/mac/macchanger/tests/test_macchanger.py` & `automonisaur-0.5.4/automon/integrations/mac/macchanger/tests/test_macchanger.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/minioWrapper/client.py` & `automonisaur-0.5.4/automon/integrations/minioWrapper/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/minioWrapper/config.py` & `automonisaur-0.5.4/automon/integrations/minioWrapper/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/minioWrapper/object.py` & `automonisaur-0.5.4/automon/integrations/minioWrapper/object.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/minioWrapper/tests/test_minio_client.py` & `automonisaur-0.5.4/automon/integrations/minioWrapper/tests/test_minio_client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/minioWrapper/tests/test_minio_client_public.py` & `automonisaur-0.5.4/automon/integrations/minioWrapper/tests/test_minio_client_public.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/minioWrapper/tests/test_minio_client_public_clear_bucket.py` & `automonisaur-0.5.4/automon/integrations/minioWrapper/tests/test_minio_client_public_clear_bucket.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/neo4jWrapper/client.py` & `automonisaur-0.5.4/automon/integrations/neo4jWrapper/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import neo4j
-import logging
 
 from neo4j import GraphDatabase
 from queue import Queue
 
 from automon import log
 from automon.integrations.neo4jWrapper.cypher import Cypher
 
 from .config import Neo4jConfig
 from .results import Results
 
-log.logging.getLogger('neo4j').setLevel(logging.ERROR)
+log.logging.getLogger('neo4j').setLevel(log.logging.ERROR)
 logger = log.logging.getLogger(__name__)
 logger.setLevel(log.DEBUG)
 
 
 class Neo4jClient:
 
     def __init__(self,
```

### Comparing `automonisaur-0.5.3/automon/integrations/neo4jWrapper/clientAsync.py` & `automonisaur-0.5.4/automon/integrations/neo4jWrapper/clientAsync.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/neo4jWrapper/config.py` & `automonisaur-0.5.4/automon/integrations/neo4jWrapper/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/neo4jWrapper/cypher.py` & `automonisaur-0.5.4/automon/integrations/neo4jWrapper/cypher.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/neo4jWrapper/results.py` & `automonisaur-0.5.4/automon/integrations/neo4jWrapper/results.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/neo4jWrapper/tests/test_neo4j_client.py` & `automonisaur-0.5.4/automon/integrations/neo4jWrapper/tests/test_neo4j_client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/neo4jWrapper/tests/test_neo4j_config.py` & `automonisaur-0.5.4/automon/integrations/neo4jWrapper/tests/test_neo4j_config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/neo4jWrapper/tests/test_neo4j_cypher.py` & `automonisaur-0.5.4/automon/integrations/neo4jWrapper/tests/test_neo4j_cypher.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/nest_asyncioWrapper/client.py` & `automonisaur-0.5.4/automon/integrations/nest_asyncioWrapper/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import asyncio
-import logging
 import nest_asyncio
 
 from automon import log
 
 logger = log.logging.getLogger(__name__)
 logger.setLevel(log.ERROR)
```

### Comparing `automonisaur-0.5.3/automon/integrations/nmap/client.py` & `automonisaur-0.5.4/automon/integrations/nmap/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/nmap/config.py` & `automonisaur-0.5.4/automon/integrations/nmap/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/nmap/output.py` & `automonisaur-0.5.4/automon/integrations/nmap/output.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/nmap/tests/test_nmap_client.py` & `automonisaur-0.5.4/automon/integrations/nmap/tests/test_nmap_client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/openTelemetryWrapper/client.py` & `automonisaur-0.5.4/automon/integrations/openTelemetryWrapper/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import json
 import opentelemetry
 
 from opentelemetry.util import types
 from opentelemetry.trace import Status, StatusCode
 
-from automon.log import logging
+from automon import log
 
 from .config import OpenTelemetryConfig
 
-logger = logging.getLogger(__name__)
-logger.setLevel(logging.DEBUG)
+logger = log.logging.getLogger(__name__)
+logger.setLevel(log.logging.DEBUG)
 
 
 class OpenTelemetryClient(object):
 
     def __init__(self):
         self.config = OpenTelemetryConfig()
```

### Comparing `automonisaur-0.5.3/automon/integrations/openTelemetryWrapper/config.py` & `automonisaur-0.5.4/automon/integrations/openTelemetryWrapper/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import asyncio
 import opentelemetry
 
 from opentelemetry.sdk.trace import TracerProvider
 from opentelemetry.sdk.trace.export import SimpleSpanProcessor
 from opentelemetry.sdk.trace.export.in_memory_span_exporter import InMemorySpanExporter
 
-from automon.log import logging
+from automon import log
 
-logger = logging.getLogger(__name__)
-logger.setLevel(logging.DEBUG)
+logger = log.logging.getLogger(__name__)
+logger.setLevel(log.logging.DEBUG)
 
 
 class OpenTelemetryConfig(object):
     def __init__(self):
         self.opentelemetry = opentelemetry
         self.provider = TracerProvider()
         self.memory_processor = InMemorySpanExporter()
```

### Comparing `automonisaur-0.5.3/automon/integrations/openvpn/openvpn.py` & `automonisaur-0.5.4/automon/integrations/openvpn/openvpn.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/requestsWrapper/client.py` & `automonisaur-0.5.4/automon/integrations/requestsWrapper/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/requestsWrapper/rest.py` & `automonisaur-0.5.4/automon/integrations/requestsWrapper/rest.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/requestsWrapper/tests/test_requests.py` & `automonisaur-0.5.4/automon/integrations/requestsWrapper/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/seleniumWrapper/actions.py` & `automonisaur-0.5.4/automon/integrations/seleniumWrapper/actions.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/seleniumWrapper/browser.py` & `automonisaur-0.5.4/automon/integrations/seleniumWrapper/browser.py`

 * *Files 20% similar despite different names*

```diff
@@ -30,14 +30,17 @@
     webdriver: selenium.webdriver
     status: int
 
     def __init__(self, config: SeleniumConfig = None):
         """A selenium wrapper"""
 
         self._config = config or SeleniumConfig()
+        self._selenium = selenium
+
+        self.logs = {}
 
     def __repr__(self):
         try:
             return str(dict(
                 webdriver=self.webdriver.name or None,
                 window_size=self.window_size,
             ))
@@ -51,16 +54,18 @@
         """Set of supported locator strategies"""
         return selenium.webdriver.common.by.By()
 
     @property
     def config(self):
         return self._config
 
-    async def cookie_file_to_dict(self, file: str = 'cookies.txt'):
-        logger.debug(f'{file}')
+    async def cookie_file_to_dict(self, file: str = 'cookies.txt') -> list:
+        logger.debug(dict(
+            cookie_file_to_dict=file
+        ))
         with open(file, 'r') as file:
             return json.loads(file.read())
 
     @property
     def _current_url(self):
         try:
             self.webdriver.current_url
@@ -68,27 +73,61 @@
         except Exception as error:
             return
 
     @property
     def webdriver(self):
         return self.config.webdriver
 
-    @property
-    def get_log(self) -> list:
-        """Gets the log for a given log type"""
-        logs = []
+    async def get_log(self, log_type: str) -> list:
+        """Get logs for log type"""
+        return self.webdriver.get_log(log_type)
+
+    async def get_logs(self) -> dict:
+        """Get all logs
+
+        you can only run this once
+        afterwards the logs are cleared from the webdriver
+        """
         for log_type in self.webdriver.log_types:
-            logs.append(
+            self.logs.update(
                 {
                     log_type: self.webdriver.get_log(log_type)
                 }
             )
+        return self.logs
 
+    async def get_log_browser(self) -> list:
+        """Get browser logs"""
+        logs = await self.get_log('browser')
         return logs
 
+    async def get_log_driver(self) -> list:
+        """Get driver logs"""
+        logs = await self.get_log('driver')
+        return logs
+
+    async def get_log_performance(self) -> list:
+        """Get performance logs"""
+        logs = await self.get_log('performance')
+        return logs
+
+    async def check_page_load_finished(self) -> bool:
+        """Checks for `frameStoppedLoading` string in performance logs"""
+        logs = await self.get_log_performance()
+
+        check = []
+        for log_dict in logs:
+            if 'frameStoppedLoading' in log_dict.get('message'):
+                check.append(log_dict)
+
+        if check:
+            return True
+
+        return False
+
     @property
     def keys(self):
         """Set of special keys codes"""
         return selenium.webdriver.common.keys.Keys
 
     async def refresh(self):
         self.webdriver.refresh()
@@ -104,15 +143,17 @@
             return self.webdriver.execute_script("return navigator.userAgent")
         except:
             return None
 
     @property
     def current_url(self):
         if self.webdriver:
-            logger.debug(self._current_url)
+            logger.debug(dict(
+                current_url=self._current_url
+            ))
             if self._current_url == 'data:,':
                 return ''
             return self._current_url
 
         logger.info(None)
         return ''
 
@@ -120,15 +161,15 @@
     def window_size(self):
         return self.config.webdriver_wrapper.window_size
 
     def _screenshot_name(self, prefix=None):
         """Generate a unique filename"""
 
         title = self.webdriver.title
-        url = self._current_url
+        url = self.current_url
         hostname = urlparse(url).hostname
 
         hostname_ = Sanitation.ascii_numeric_only(hostname)
         title_ = Sanitation.ascii_numeric_only(title)
         timestamp = Dates.filename_timestamp()
 
         if prefix:
@@ -172,18 +213,26 @@
         except Exception as error:
             raise Exception(error)
 
     async def add_cookie(self, cookie_dict: dict) -> bool:
         result = self.webdriver.add_cookie(cookie_dict=cookie_dict)
 
         if result is None:
-            logger.debug(f'{cookie_dict}')
+            logger.debug(dict(
+                domain=cookie_dict.get('domain'),
+                path=cookie_dict.get('path'),
+                secure=cookie_dict.get('secure'),
+                expiry=cookie_dict.get('expiry'),
+                name=cookie_dict.get('name'),
+            ))
             return True
 
-        logger.error(f'{cookie_dict}')
+        logger.error(dict(
+            add_cookie=cookie_dict
+        ))
         return False
 
     async def add_cookie_from_file(self, file: str) -> bool:
         """add cookies from file"""
         if os.path.exists(file):
             await self.add_cookies_from_list(
                 await self.cookie_file_to_dict(file=file)
@@ -193,78 +242,91 @@
         logger.error(f'{file}')
         return False
 
     async def add_cookies_from_list(self, cookies_list: list) -> bool:
         for cookie in cookies_list:
             await self.add_cookie(cookie_dict=cookie)
 
-        logger.debug(f'{True}')
+        logger.debug(dict(
+            add_cookies_from_list=len(cookies_list)
+        ))
         return True
 
     async def add_cookie_from_current_url(self):
         logger.info(f'{self.url}')
         return self.add_cookie_from_url(self.url)
 
     async def add_cookie_from_url(self, url: str) -> bool:
         """add cookies from matching hostname"""
         cookie_file = await self._url_filename(url=url)
 
         if os.path.exists(cookie_file):
             logger.info(f'{cookie_file}')
-            return self.add_cookie_from_file(file=cookie_file)
+            return await self.add_cookie_from_file(file=cookie_file)
 
         logger.error(f'{cookie_file}')
 
     async def add_cookie_from_base64(self, base64_str: str) -> bool:
         if base64_str:
             await self.add_cookies_from_list(
                 json.loads(base64.b64decode(base64_str))
             )
             logger.debug(f'{True}')
             return True
 
         logger.error(f'{base64_str}')
         return False
 
+    async def autosave_cookies(self) -> bool:
+        if self.current_url:
+            await self.save_cookies_for_current_url()
+            return await self.load_cookies_for_current_url()
+
     async def delete_all_cookies(self) -> None:
         result = self.webdriver.delete_all_cookies()
         logger.info(f'{True}')
         return result
 
     async def _url_filename(self, url: str):
         parsed = await self.urlparse(url)
         hostname = parsed.hostname
         cookie_file = f'cookies-{hostname}.txt'
-        logger.info(f'{cookie_file}')
+        logger.debug(dict(
+            _url_filename=cookie_file
+        ))
         return cookie_file
 
     async def get_cookie(self, name: str) -> dict:
         result = self.webdriver.get_cookie(name=name)
         logger.info(f'{result}')
         return result
 
     async def get_cookies(self) -> [dict]:
-        result = self.webdriver.get_cookies()
-        logger.debug(f'{True}')
-        return result
+        cookies = self.webdriver.get_cookies()
+        logger.debug(dict(
+            get_cookies=len(cookies)
+        ))
+        return cookies
 
     async def get_cookies_base64(self) -> base64:
-        result = self.get_cookies()
+        cookies = await self.get_cookies()
         logger.debug(f'{True}')
         return base64.b64encode(
-            json.dumps(result).encode()
+            json.dumps(cookies).encode()
         ).decode()
 
     async def get_cookies_json(self) -> json.dumps:
-        cookies = self.get_cookies()
-        logger.debug(f'{True}')
+        cookies = await self.get_cookies()
+        logger.debug(dict(
+            get_cookies_json=len(cookies)
+        ))
         return json.dumps(cookies)
 
     async def get_cookies_summary(self):
-        result = self.get_cookies()
+        result = await self.get_cookies()
         summary = {}
         if result:
             for cookie in result:
                 cookie = dict(cookie)
                 domain = cookie.get('domain')
                 name = cookie.get('name')
                 expiry = cookie.get('expiry')
@@ -290,16 +352,19 @@
             message = error_parsed[0]
             session = error_parsed[1]
             stacktrace = error_parsed[2:]
             stacktrace = ' '.join(stacktrace)
 
             return message, session, stacktrace
 
-        except Exception as error:
-            logger.error(error)
+        except Exception as e:
+            logger.error(dict(
+                exception=e,
+                error=error,
+            ))
 
         return error, None, None
 
     async def find_element(
             self,
             value: str,
             by: By.ID = By.ID,
@@ -334,19 +399,23 @@
         try:
             if self.webdriver.get(url, **kwargs) is None:
                 logger.info(str(dict(
                     url=url,
                     current_url=self.current_url,
                     kwargs=kwargs
                 )))
+
+            if self.config.cookies_autosave:
+                await self.autosave_cookies()
+
             return True
         except Exception as error:
-            logger.error(str(dict(
+            logger.error(dict(
                 error=error,
-            )))
+            ))
 
         return False
 
     async def get_page(self, *args, **kwargs):
         """alias to get"""
         return self.get(*args, **kwargs)
 
@@ -356,15 +425,15 @@
 
     async def get_page_source_beautifulsoup(
             self,
             markdup: str = None,
             features: str = 'lxml') -> BeautifulSoup:
         """read page source with beautifulsoup"""
         if not markdup:
-            markdup = self.get_page_source()
+            markdup = await self.get_page_source()
         return BeautifulSoup(
             markup=markdup,
             features=features)
 
     async def get_random_user_agent(
             self,
             filter: list or str = None,
@@ -404,17 +473,31 @@
         """browser is running"""
         if self.webdriver:
             logger.info(f'{True}')
             return True
         logger.error(f'{False}')
         return False
 
+    async def load_cookies_for_current_url(self) -> bool:
+        filename = await self._url_filename(url=self.url)
+        logger.info(dict(
+            load_cookies_for_current_url=filename,
+            url=self.url,
+        ))
+        return await self.add_cookie_from_file(file=filename)
+
+    @property
+    def page_source(self):
+        return self.webdriver.page_source
+
     async def urlparse(self, url: str):
         parsed = urlparse(url=url)
-        logger.debug(f'{parsed}')
+        logger.debug(dict(
+            urlparse=parsed
+        ))
         return parsed
 
     async def quit(self) -> bool:
         """gracefully quit browser"""
         try:
             self.webdriver.close()
             self.webdriver.quit()
@@ -428,34 +511,45 @@
             )))
             return False
         return True
 
     async def run(self):
         """run browser"""
         try:
-            await self.config.run()
-        except:
+            return await self.config.run()
+        except Exception as error:
+            logger.error(dict(
+                error=error
+            ))
             return False
 
-    async def save_cookies_for_current_url(self):
-        filename = self._url_filename(url=self.url)
-        logger.info(f'{filename}')
+    async def save_cookies_for_current_url(self) -> bool:
+        filename = await self._url_filename(url=self.url)
+        logger.info(dict(
+            save_cookies_for_current_url=filename,
+            url=self.url,
+        ))
         return await self.save_cookies_to_file(file=filename)
 
-    async def save_cookies_to_file(self, file: str):
+    async def save_cookies_to_file(self, file: str) -> bool:
         with open(file, 'w') as cookies:
             cookies.write(
                 await self.get_cookies_json()
             )
 
         if os.path.exists(file):
-            logger.info(f'{os.path.abspath(file)} ({os.stat(file).st_size} B)')
+            logger.info(dict(
+                save_cookies_to_file=os.path.abspath(file),
+                bytes=os.stat(file).st_size
+            ))
             return True
 
-        logger.error(f'{file}')
+        logger.error(dict(
+            file=file
+        ))
         return False
 
     async def save_screenshot(
             self,
             filename: str = None,
             prefix: str = None,
             folder: str = None,
```

### Comparing `automonisaur-0.5.3/automon/integrations/seleniumWrapper/browser_types.py` & `automonisaur-0.5.4/automon/integrations/seleniumWrapper/browser_types.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/seleniumWrapper/config.py` & `automonisaur-0.5.4/automon/integrations/seleniumWrapper/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 
 class SeleniumConfig(object):
     def __init__(self):
         self._webdriver = None
         self.webdriver_wrapper = None
 
+        self.cookies_autosave: bool = environ('SELENIUM_COOKIES_AUTOSAVE', False)
         self._cookies_base64 = environ('SELENIUM_COOKIES_BASE64')
         self._cookies_file = environ('SELENIUM_COOKIES_FILE')
 
     @property
     def webdriver(self):
         try:
             return self.webdriver_wrapper.webdriver
```

### Comparing `automonisaur-0.5.3/automon/integrations/seleniumWrapper/config_window_size.py` & `automonisaur-0.5.4/automon/integrations/seleniumWrapper/config_window_size.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/seleniumWrapper/tests/test_browser.py` & `automonisaur-0.5.4/automon/integrations/seleniumWrapper/tests/test_browser.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import unittest
 import asyncio
 
 from automon.integrations.seleniumWrapper import SeleniumBrowser, ChromeWrapper
 
 browser = SeleniumBrowser()
 browser.config.webdriver_wrapper = ChromeWrapper()
-browser.config.webdriver_wrapper.enable_defaults()
-browser.config.webdriver_wrapper.enable_headless()
+browser.config.webdriver_wrapper.enable_defaults().enable_headless()
 
 
 class SeleniumClientTest(unittest.TestCase):
     if asyncio.run(browser.run()):
 
         def test_fake_page(self):
-            self.assertFalse(browser.get('http://555.555.555.555'))
+            self.assertFalse(asyncio.run(browser.get('http://555.555.555.555')))
 
         def test_real_page(self):
             if asyncio.run(browser.get('http://1.1.1.1')):
                 self.assertTrue(True)
 
         def test_screenshot_png(self):
             if asyncio.run(browser.get('http://google.com')):
@@ -28,11 +27,13 @@
                 self.assertTrue(asyncio.run(browser.get_screenshot_as_base64()))
 
         def test_screenshot_file(self):
             if asyncio.run(browser.get('http://bing.com')):
                 self.assertTrue(asyncio.run(browser.save_screenshot()))
                 self.assertTrue(asyncio.run(browser.save_screenshot(folder='./')))
 
+    asyncio.run(browser.quit())
+
 
 if __name__ == '__main__':
     unittest.main()
     browser.quit()
```

### Comparing `automonisaur-0.5.3/automon/integrations/seleniumWrapper/tests/test_browser_headless.py` & `automonisaur-0.5.4/automon/integrations/seleniumWrapper/tests/test_browser_headless.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 import unittest
 import asyncio
 
 from automon.integrations.seleniumWrapper import SeleniumBrowser, ChromeWrapper
 
 browser = SeleniumBrowser()
 browser.config.webdriver_wrapper = ChromeWrapper()
-browser.config.webdriver_wrapper.enable_defaults()
-browser.config.webdriver_wrapper.enable_headless()
+browser.config.webdriver_wrapper.enable_defaults().enable_headless()
 
 
 class SeleniumClientTest(unittest.TestCase):
     if asyncio.run(browser.run()):
 
         def test(self):
 
-            asyncio.run(browser.set_window_size(device_type='web-large'))
+            if asyncio.run(browser.get('http://1.1.1.1')):
 
-            if asyncio.run(browser.get('http://bing.com')):
-                self.assertTrue(asyncio.run(browser.save_screenshot()))
-                self.assertTrue(asyncio.run(browser.save_screenshot()))
-                self.assertTrue(asyncio.run(browser.save_screenshot(folder='./')))
+                if asyncio.run(browser.check_page_load_finished()):
+                    self.assertTrue(asyncio.run(browser.save_screenshot()))
+                    self.assertTrue(asyncio.run(browser.save_screenshot(folder='./')))
 
             asyncio.run(browser.quit())
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `automonisaur-0.5.3/automon/integrations/seleniumWrapper/tests/test_browser_useragent.py` & `automonisaur-0.5.4/automon/integrations/seleniumWrapper/tests/test_browser_useragent.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import unittest
 import asyncio
 
 from automon.integrations.seleniumWrapper import SeleniumBrowser, ChromeWrapper
 
 browser = SeleniumBrowser()
 browser.config.webdriver_wrapper = ChromeWrapper()
-browser.config.webdriver_wrapper.enable_defaults()
-browser.config.webdriver_wrapper.enable_headless()
+browser.config.webdriver_wrapper.enable_defaults().enable_headless()
 
 agent = 'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:112.0) Gecko/20100101 Firefox/112.0'
 
 browser.config.webdriver_wrapper.set_user_agent(agent)
 
 
 class SeleniumClientTest(unittest.TestCase):
```

### Comparing `automonisaur-0.5.3/automon/integrations/seleniumWrapper/tests/test_user_agent.py` & `automonisaur-0.5.4/automon/integrations/seleniumWrapper/tests/test_user_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
         test = SeleniumUserAgentBuilder()
         self.assertTrue(test.filter_agent('applewebkit'))
         self.assertTrue(test.filter_agent('AppleWebKit', case_sensitive=True))
 
         self.assertFalse(test.filter_agent('xxxxx'))
         self.assertFalse(test.filter_agent('xxxxx', case_sensitive=True))
 
-
     def test_random(self):
         test = SeleniumUserAgentBuilder()
         self.assertTrue(test.get_random_agent('applewebkit'))
         self.assertTrue(test.get_random_agent('AppleWebKit', case_sensitive=True))
 
         self.assertFalse(test.get_random_agent('xxxxx'))
         self.assertFalse(test.get_random_agent('xxxxx', case_sensitive=True))
```

### Comparing `automonisaur-0.5.3/automon/integrations/seleniumWrapper/user_agents.py` & `automonisaur-0.5.4/automon/integrations/seleniumWrapper/user_agents.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/seleniumWrapper/webdriver_chrome.py` & `automonisaur-0.5.4/automon/integrations/seleniumWrapper/webdriver_chrome.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,14 @@
         self._chrome_options = selenium.webdriver.ChromeOptions()
         self._chromedriver_path = environ_list('SELENIUM_CHROMEDRIVER_PATH')
         self._ChromeService = None
         self._window_size = set_window_size()
 
         self.update_paths(self.chromedriver_path)
 
-        if not self.chromedriver_path:
-            logger.error('missing SELENIUM_CHROMEDRIVER_PATH')
-
     def __repr__(self):
         if self._webdriver:
             return str(dict(
                 name=self.webdriver.name,
                 window_size=self.window_size,
                 browserVersion=self.browserVersion,
                 chromedriverVersion=self.chromedriverVersion,
@@ -55,14 +52,16 @@
 
     @property
     def chromedriver_path(self):
         for path in self._chromedriver_path:
             if os.path.exists(path):
                 return path
 
+        logger.error('missing SELENIUM_CHROMEDRIVER_PATH')
+
     @property
     def chromedriverVersion(self):
         if self.webdriver:
             return self.webdriver.capabilities.get('chrome').get('chromedriverVersion')
 
     @property
     def ChromeService(self):
@@ -128,14 +127,15 @@
 
     def enable_bigshm(self):
         logger.warning('Big shm not yet implemented')
         return self
 
     def enable_defaults(self):
         self.enable_maximized()
+        self.enable_logging()
         return self
 
     def enable_fullscreen(self):
         self.chrome_options.add_argument("--start-fullscreen")
         logger.debug(str(dict(
             add_argument=f'--start-fullscreen'
         )))
@@ -144,14 +144,21 @@
     def enable_headless(self):
         self.chrome_options.add_argument('headless')
         logger.debug(str(dict(
             add_argument='headless'
         )))
         return self
 
+    def enable_logging(self):
+        self.chrome_options.set_capability('goog:loggingPrefs', {'performance': 'ALL'})
+        logger.debug(dict(
+            set_capability=('goog:loggingPrefs', {'performance': 'ALL'})
+        ))
+        return self
+
     def enable_notifications(self):
         """Pass the argument 1 to allow and 2 to block
 
         """
         self.chrome_options.add_experimental_option(
             "prefs", {"profile.default_content_setting_values.notifications": 1}
         )
@@ -300,15 +307,15 @@
         """
         logger.warning('Default shm size is 64m, which will cause chrome driver to crash.')
 
         self.enable_defaults()
         self.disable_sandbox()
         return self
 
-    async def run(self) -> selenium.webdriver.Chrome:
+    async def run(self) -> bool:
         try:
             if self.chromedriver_path:
                 self._ChromeService = selenium.webdriver.ChromeService(
                     executable_path=self.chromedriver_path
                 )
                 logger.debug(str(dict(
                     ChromeService=self.ChromeService
@@ -316,20 +323,20 @@
 
                 self._webdriver = selenium.webdriver.Chrome(
                     service=self.ChromeService,
                     options=self.chrome_options
                 )
                 logger.info(f'{self}')
 
-                return self.webdriver
+                return True
 
             self._webdriver = selenium.webdriver.Chrome(options=self.chrome_options)
             logger.info(f'{self}')
 
-            return self.webdriver
+            return True
         except Exception as error:
             logger.error(f'{error}')
             raise Exception(error)
 
     async def set_chromedriver(self, chromedriver_path: str):
         logger.debug(f'{chromedriver_path}')
         self._chromedriver_path.append(chromedriver_path)
@@ -396,17 +403,15 @@
                 logger.debug(str(dict(
                     SELENIUM_CHROMEDRIVER_PATH=path,
                     PATH=os.environ['PATH']
                 )))
 
                 return True
 
-        logger.error(dict(
-            chromedriver_path=path
-        ))
+        return False
 
     async def quit(self):
         """quit
 
         """
         result = self.webdriver.quit()
         logger.info(f'{result}')
```

### Comparing `automonisaur-0.5.3/automon/integrations/sentryio/client.py` & `automonisaur-0.5.4/automon/integrations/sentryio/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/sentryio/config.py` & `automonisaur-0.5.4/automon/integrations/sentryio/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/sentryio/tests/test_sentryio.py` & `automonisaur-0.5.4/automon/integrations/sentryio/tests/test_sentryio.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/sentryio/tests/test_sentryio_callback.py` & `automonisaur-0.5.4/automon/integrations/sentryio/tests/test_sentryio_callback.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/shodan/__init__.py` & `automonisaur-0.5.4/automon/integrations/shodan/__init__.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/slackWrapper/bots.py` & `automonisaur-0.5.4/automon/integrations/slackWrapper/bots.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/slackWrapper/client.py` & `automonisaur-0.5.4/automon/integrations/slackWrapper/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/slackWrapper/clientAsync.py` & `automonisaur-0.5.4/automon/integrations/slackWrapper/clientAsync.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/slackWrapper/config.py` & `automonisaur-0.5.4/automon/integrations/slackWrapper/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/slackWrapper/error.py` & `automonisaur-0.5.4/automon/integrations/slackWrapper/error.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/slackWrapper/slack_formatting.py` & `automonisaur-0.5.4/automon/integrations/slackWrapper/slack_formatting.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/slackWrapper/slack_logger.py` & `automonisaur-0.5.4/automon/integrations/slackWrapper/slack_logger.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/slackWrapper/tests/test_slack.py` & `automonisaur-0.5.4/automon/integrations/slackWrapper/tests/test_slack.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/snmp/generate_maps.py` & `automonisaur-0.5.4/automon/integrations/snmp/generate_maps.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/splunk/client.py` & `automonisaur-0.5.4/automon/integrations/splunk/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/splunk/config.py` & `automonisaur-0.5.4/automon/integrations/splunk/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/splunk/helpers.py` & `automonisaur-0.5.4/automon/integrations/splunk/helpers.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/splunk/tests/test_splunk_client.py` & `automonisaur-0.5.4/automon/integrations/splunk/tests/test_splunk_client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/splunk/tests/test_splunk_config.py` & `automonisaur-0.5.4/automon/integrations/splunk/tests/test_splunk_config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/splunk_soar/client.py` & `automonisaur-0.5.4/automon/integrations/splunk_soar/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -320,16 +320,15 @@
         if self.config.is_ready:
             if self._get(Urls.container(page_size=1)):
                 logger.info(f'client connected '
                             f'{self.config.host} '
                             f'[{self.client.response.status_code}] ')
                 return True
 
-        else:
-            logger.warning(f'client not connected')
+        logger.error(f'client not connected')
         return False
 
     @_is_connected
     def filter_vault(self, filter: str, page_size: int = None, **kwargs) -> [Vault]:
         """Filter for matching vault files"""
         matches = []
```

### Comparing `automonisaur-0.5.3/automon/integrations/splunk_soar/config.py` & `automonisaur-0.5.4/automon/integrations/splunk_soar/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,19 +16,16 @@
         self.user = user or environ('SPLUNK_SOAR_USER')
         self.password = password or environ('SPLUNK_SOAR_PASSWORD')
         self.auth = (self.user, self.password)
         self.auth_token = auth_token or environ('SPLUNK_SOAR_AUTH_TOKEN')
 
         self.headers = {'ph-auth-token': self.auth_token}
 
-        if not self.host:
-            logger.warning(f'missing SPLUNK_SOAR_HOST')
-
     def __repr__(self):
         return f'{self.__dict__}'
 
     @property
     def is_ready(self) -> bool:
         if self.host:
             return True
-        logger.warning(f'bad config')
+        logger.error(f'missing SPLUNK_SOAR_HOST')
         return False
```

### Comparing `automonisaur-0.5.3/automon/integrations/splunk_soar/datatypes.py` & `automonisaur-0.5.4/automon/integrations/splunk_soar/datatypes.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/splunk_soar/integration/servicenow/ticket.py` & `automonisaur-0.5.4/automon/integrations/splunk_soar/integration/servicenow/ticket.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/splunk_soar/phantom_unittest.py` & `automonisaur-0.5.4/automon/integrations/splunk_soar/phantom_unittest.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/splunk_soar/responses.py` & `automonisaur-0.5.4/automon/integrations/splunk_soar/responses.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/splunk_soar/rest/urls.py` & `automonisaur-0.5.4/automon/integrations/splunk_soar/rest/urls.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/splunk_soar/rules.py` & `automonisaur-0.5.4/automon/integrations/splunk_soar/rules.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-import logging
+from automon import log
 
 from .phantom_unittest import import_playbook, container, results, artifact
 
 timestamp = '%(asctime)s'
 levelname = '%(levelname)s'
 modname = '%(name)s'
 message = '%(message)s'
 log_format = f'{timestamp}\t{levelname}\t({modname})\t{message}'
 
-logging.basicConfig(level=logging.DEBUG, format=log_format)
-log = logging.getLogger(__name__)
-log.setLevel(logging.DEBUG)
+log.logging.basicConfig(level=log.logging.DEBUG, format=log_format)
+logger = log.logging.getLogger(__name__)
+logger.setLevel(log.logging.DEBUG)
 
 
 def playbook(playbook_to_import: str, container: dict = container(),
              name: str = '', callback: object = None):
     """Mock function"""
-    log = logging.getLogger(f'{__name__}.{playbook.__name__}')
+    logger = log.logging.getLogger(f'{__name__}.{playbook.__name__}')
 
     # logger.info(f'playbook_to_import: str, container: dict = {}, name: str, callback: object')
 
     logger.debug(f'playbook_to_import: {playbook_to_import}')
     logger.debug(f'container: {container}')
     logger.debug(f'name: {name}')
     logger.debug(f'callback: {callback}')
 
     return import_playbook(playbook_to_import)
 
 
 def get_run_data(key: str, **kwargs):
     """Mock function"""
-    log = logging.getLogger(f'{__name__}.{get_run_data.__name__}')
+    logger = log.logging.getLogger(f'{__name__}.{get_run_data.__name__}')
 
     # logger.info(f'key: {key}')
     logger.debug(f'key: {key}')
 
     return key
 
 
 def condition(container: dict = container(), conditions: list = [], name: str = ''):
     """Mock function"""
-    log = logging.getLogger(f'{__name__}.{condition.__name__}')
+    logger = log.logging.getLogger(f'{__name__}.{condition.__name__}')
 
     logger.debug(f'{help(condition)}')
 
     logger.debug(f'container: {container}')
     logger.debug(f'conditions: {conditions}')
     logger.debug(f'name: {name}')
 
     return container, conditions, name
 
 
 def format(container: dict = container(), template: str = '', parameters: list = [str],
            name: str = ''):
     """Mock function"""
-    log = logging.getLogger(f'{__name__}.{format.__name__}')
+    logger = log.logging.getLogger(f'{__name__}.{format.__name__}')
 
     logger.debug('container: dict = {}, template: str = '', parameters: list = [], name: str = ''')
 
     parameters_orig = parameters
 
     parameters = [
         [x.split(':')] for x in parameters
@@ -70,37 +70,37 @@
     logger.debug(f'name: {name}')
 
     return container, template, parameters, name
 
 
 def get_format_data(name: str, **kwargs):
     """Mock function"""
-    log = logging.getLogger(f'{__name__}.{get_format_data.__name__}')
+    logger = log.logging.getLogger(f'{__name__}.{get_format_data.__name__}')
 
     logger.debug(f'name: {name}')
 
     return name
 
 
 def collect2(container: dict = container(), datapath: list = [], action_results: object = None):
     """Mock function"""
-    log = logging.getLogger(f'{__name__}.{collect2.__name__}')
+    logger = log.logging.getLogger(f'{__name__}.{collect2.__name__}')
 
     logger.info('container: dict = {}, datapath: list = [], action_results: object = None')
 
     logger.debug(f'container: {container}')
     logger.debug(f'datapath: {datapath}')
     logger.debug(f'action_results: {action_results}')
 
     return [[artifact(), artifact()]]
 
 
 def act(action: str, parameters: str, assets: list, callback: object, name: str, parent_action: str = ''):
     """Mock function"""
-    log = logging.getLogger(f'{__name__}.{act.__name__}')
+    logger = log.logging.getLogger(f'{__name__}.{act.__name__}')
 
     # logger.info(f'action: str, parameters: str, assets: list, callback: object, name: str')
 
     logger.debug(f'action: {action}')
     logger.debug(f'parameters: {parameters}')
     logger.debug(f'assets: {assets}')
     logger.debug(f'callback: {callback}')
@@ -108,15 +108,15 @@
     logger.debug(f'parent_action: {parent_action}')
 
     return action, parameters, assets, callback, name, parent_action
 
 
 def save_run_data(key: str, value: str, auto: bool):
     """Mock function"""
-    log = logging.getLogger(f'{__name__}.{save_run_data.__name__}')
+    logger = log.logging.getLogger(f'{__name__}.{save_run_data.__name__}')
 
     logger.debug(f'key: {key}')
     logger.debug(f'value: {value}')
     logger.debug(f'auto: {auto}')
 
     return key, value, auto
```

### Comparing `automonisaur-0.5.3/automon/integrations/splunk_soar/tests/dino.py` & `automonisaur-0.5.4/automon/integrations/splunk_soar/tests/dino.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/splunk_soar/tests/test_soar_client.py` & `automonisaur-0.5.4/automon/integrations/splunk_soar/tests/test_soar_client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/splunk_soar/tests/test_soar_client_create_container_attachment.py` & `automonisaur-0.5.4/automon/integrations/splunk_soar/tests/test_soar_client_create_container_attachment.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/splunk_soar/tests/test_soar_client_list_containers.py` & `automonisaur-0.5.4/automon/integrations/splunk_soar/tests/test_soar_client_list_containers.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/splunk_soar/tests/test_soar_uat.py` & `automonisaur-0.5.4/automon/integrations/splunk_soar/tests/test_soar_uat.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/splunk_soar/tests/test_soar_uat_run_playbook.py` & `automonisaur-0.5.4/automon/integrations/splunk_soar/tests/test_soar_uat_run_playbook.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/splunk_soar/tests/test_soar_uat_update_playbook.py` & `automonisaur-0.5.4/automon/integrations/splunk_soar/tests/test_soar_uat_update_playbook.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/splunk_soar/vault.py` & `automonisaur-0.5.4/automon/integrations/splunk_soar/vault.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/swift/client.py` & `automonisaur-0.5.4/automon/integrations/swift/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/swift/config.py` & `automonisaur-0.5.4/automon/integrations/swift/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,52 +1,68 @@
 import os
 
 from automon import log
+from automon import environ
 
 logger = log.logging.getLogger(__name__)
 logger.setLevel(log.DEBUG)
 
 
 class SwiftConfig:
-    OPENSTACK_USERNAME = os.getenv('OPENSTACK_USERNAME') or ''
-    OPENSTACK_PASSWORD = os.getenv('OPENSTACK_PASSWORD') or ''
-    OPENSTACK_AUTH_URL = os.getenv('OPENSTACK_AUTH_URL') or ''
-    OPENSTACK_PROJECT_ID = os.getenv('OPENSTACK_PROJECT_ID') or ''
-    OPENSTACK_PROJECT_NAME = os.getenv('OPENSTACK_PROJECT_NAME') or ''
-    OPENSTACK_USER_DOMAIN_NAME = os.getenv('OPENSTACK_USER_DOMAIN_NAME') or ''
-    OPENSTACK_PROJECT_DOMAIN_ID = os.getenv('OPENSTACK_PROJECT_DOMAIN_ID') or ''
-    OPENSTACK_REGION_NAME = os.getenv('OPENSTACK_REGION_NAME') or 'RegionOne'
-    OPENSTACK_INTERFACE = os.getenv('OPENSTACK_INTERFACE') or 'public'
-    OPENSTACK_IDENTITY_API_VERSION = os.getenv('OPENSTACK_IDENTITY_API_VERSION') or '3'
-    SWIFTCLIENT_INSECURE = os.getenv('SWIFTCLIENT_INSECURE') or 'True'
+    OPENSTACK_USERNAME = environ('OPENSTACK_USERNAME', '')
+    OPENSTACK_PASSWORD = environ('OPENSTACK_PASSWORD', '')
+    OPENSTACK_AUTH_URL = environ('OPENSTACK_AUTH_URL', '')
+    OPENSTACK_PROJECT_ID = environ('OPENSTACK_PROJECT_ID', '')
+    OPENSTACK_PROJECT_NAME = environ('OPENSTACK_PROJECT_NAME', '')
+    OPENSTACK_USER_DOMAIN_NAME = environ('OPENSTACK_USER_DOMAIN_NAME', '')
+    OPENSTACK_PROJECT_DOMAIN_ID = environ('OPENSTACK_PROJECT_DOMAIN_ID', '')
+    OPENSTACK_REGION_NAME = environ('OPENSTACK_REGION_NAME', 'RegionOne')
+    OPENSTACK_INTERFACE = environ('OPENSTACK_INTERFACE', 'public')
+    OPENSTACK_IDENTITY_API_VERSION = environ('OPENSTACK_IDENTITY_API_VERSION', 3)
+    SWIFTCLIENT_INSECURE = environ('SWIFTCLIENT_INSECURE', True)
 
     def __init__(self):
+        pass
 
+    def is_ready(self):
         if not self.OPENSTACK_USERNAME:
-            logger.warning(f'missing OPENSTACK_USERNAME')
+            logger.error(f'missing OPENSTACK_USERNAME')
+            return False
         if not self.OPENSTACK_PASSWORD:
-            logger.warning(f'missing OPENSTACK_PASSWORD')
+            logger.error(f'missing OPENSTACK_PASSWORD')
+            return False
         if not self.OPENSTACK_AUTH_URL:
-            logger.warning(f'missing OPENSTACK_AUTH_URL')
+            logger.error(f'missing OPENSTACK_AUTH_URL')
+            return False
         if not self.OPENSTACK_PROJECT_ID:
-            logger.warning(f'missing OPENSTACK_PROJECT_ID')
+            logger.error(f'missing OPENSTACK_PROJECT_ID')
+            return False
         if not self.OPENSTACK_PROJECT_NAME:
-            logger.warning(f'missing OPENSTACK_PROJECT_NAME')
+            logger.error(f'missing OPENSTACK_PROJECT_NAME')
+            return False
         if not self.OPENSTACK_USER_DOMAIN_NAME:
-            logger.warning(f'missing OPENSTACK_USER_DOMAIN_NAME')
+            logger.error(f'missing OPENSTACK_USER_DOMAIN_NAME')
+            return False
         if not self.OPENSTACK_PROJECT_DOMAIN_ID:
-            logger.warning(f'missing OPENSTACK_PROJECT_DOMAIN_ID')
+            logger.error(f'missing OPENSTACK_PROJECT_DOMAIN_ID')
+            return False
         if not self.OPENSTACK_REGION_NAME:
-            logger.warning(f'missing OPENSTACK_REGION_NAME')
+            logger.error(f'missing OPENSTACK_REGION_NAME')
+            return False
         if not self.OPENSTACK_INTERFACE:
-            logger.warning(f'missing OPENSTACK_INTERFACE')
+            logger.error(f'missing OPENSTACK_INTERFACE')
+            return False
         if not self.OPENSTACK_IDENTITY_API_VERSION:
-            logger.warning(f'missing OPENSTACK_IDENTITY_API_VERSION')
+            logger.error(f'missing OPENSTACK_IDENTITY_API_VERSION')
+            return False
         if not self.SWIFTCLIENT_INSECURE:
-            logger.warning(f'missing SWIFTCLIENT_INSECURE')
+            logger.error(f'missing SWIFTCLIENT_INSECURE')
+            return False
+
+        return True
 
     def __eq__(self, other):
         if not isinstance(other, SwiftConfig):
             logger.warning(f'Not implemented')
             return NotImplemented
 
         return self.OPENSTACK_USERNAME == other.OPENSTACK_USERNAME and \
```

### Comparing `automonisaur-0.5.3/automon/integrations/swift/error.py` & `automonisaur-0.5.4/automon/integrations/swift/error.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/swift/iterables.py` & `automonisaur-0.5.4/automon/integrations/swift/iterables.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/swift/tests/test_swift.py` & `automonisaur-0.5.4/automon/integrations/swift/tests/test_swift.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/swimlaneWrapper/api/v2.py` & `automonisaur-0.5.4/automon/integrations/swimlaneWrapper/api/v2.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/swimlaneWrapper/client.py` & `automonisaur-0.5.4/automon/integrations/swimlaneWrapper/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/swimlaneWrapper/config.py` & `automonisaur-0.5.4/automon/integrations/swimlaneWrapper/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/swimlaneWrapper/tests/test_library_record_create.py` & `automonisaur-0.5.4/automon/integrations/swimlaneWrapper/tests/test_library_record_create.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/swimlaneWrapper/tests/test_rest_app.py` & `automonisaur-0.5.4/automon/integrations/swimlaneWrapper/tests/test_rest_app.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/swimlaneWrapper/tests/test_rest_auth.py` & `automonisaur-0.5.4/automon/integrations/swimlaneWrapper/tests/test_rest_auth.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/swimlaneWrapper/tests/test_rest_auth_token.py` & `automonisaur-0.5.4/automon/integrations/swimlaneWrapper/tests/test_rest_auth_token.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/swimlaneWrapper/tests/test_rest_logging.py` & `automonisaur-0.5.4/automon/integrations/swimlaneWrapper/tests/test_rest_logging.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/swimlaneWrapper/tests/test_rest_record.py` & `automonisaur-0.5.4/automon/integrations/swimlaneWrapper/tests/test_rest_record.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/swimlaneWrapper/tests/test_rest_record_create.py` & `automonisaur-0.5.4/automon/integrations/swimlaneWrapper/tests/test_rest_record_create.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/swimlaneWrapper/tests/test_rest_record_delete_all.py` & `automonisaur-0.5.4/automon/integrations/swimlaneWrapper/tests/test_rest_record_delete_all.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/swimlaneWrapper/tests/test_rest_record_resolve_fields.py` & `automonisaur-0.5.4/automon/integrations/swimlaneWrapper/tests/test_rest_record_resolve_fields.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/vds/client.py` & `automonisaur-0.5.4/automon/integrations/vds/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/integrations/vds/config.py` & `automonisaur-0.5.4/automon/integrations/vds/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/log/__init__.py` & `automonisaur-0.5.4/automon/log/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from automon.helpers.osWrapper import environ
 
 from .attributes import LogRecordAttribute
 from .logger import Logging, LogStream, TEST, DEBUG, INFO, WARN, ERROR, CRITICAL, NOTSET
 from .logger import logging
+from .logger import log_secret
 
 log_format = f'{LogRecordAttribute(timestamp=True).levelname().name_and_lineno().funcName().message()}'
 log_format_opentelemetry = environ('OTEL_PYTHON_LOG_FORMAT') or '\t'.join(
     [
         f'%(asctime)s',
         f'%(levelname)s',
         f'[%(name)s]',
```

### Comparing `automonisaur-0.5.3/automon/log/attributes.py` & `automonisaur-0.5.4/automon/log/attributes.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automon/log/logger.py` & `automonisaur-0.5.4/automon/log/logger.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import hashlib
 import traceback
 
 from automon.helpers import Dates
 from automon.helpers.markdown import Chat, Format
 
 from .attributes import LogRecordAttribute
 
@@ -14,14 +15,18 @@
 CRITICAL = logging.CRITICAL
 NOTSET = logging.NOTSET
 
 logger = logging.getLogger(__name__)
 logger.setLevel(CRITICAL)
 
 
+def log_secret(secret: str) -> str:
+    return len(hashlib.md5(str(secret).encode()).hexdigest()) * '*'
+
+
 class Callback(object):
 
     def __init__(self, callbacks: list):
         """Log to callbacks
         """
 
         self.callbacks = callbacks
```

### Comparing `automonisaur-0.5.3/automon/log/tests/test_logger_builtin.py` & `automonisaur-0.5.4/automon/log/tests/test_logger_builtin.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.5.3/automonisaur.egg-info/PKG-INFO` & `automonisaur-0.5.4/automonisaur.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automonisaur
-Version: 0.5.3
+Version: 0.5.4
 Summary: Core libraries for automonisaur
 Home-page: https://github.com/TheShellLand/automonisaur
 Author: naisanza
 Author-email: naisanza@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -59,15 +59,15 @@
 | Data Scraping   | beautifulsoup<br/>facebook groups<br/>instagram<br/>scrapy  |
 | Databases       | elasticsearch<br/>neo4j<br/>splunk                          |
 | Data Store      | minio<br/>swift                                             |
 | Devices         | snmp                                                        |
 | Google Cloud    | google auth api<br/>google people api<br/>google sheets api |
 | Helpers         | os<br/>subprocess<br/>threading<br/>socket<br/>datetime     |
 | Logging         | sentryio                                                    |
-| MacOS           | airport<br/>macchanger                                      |
+| MacOS           | airport<br/>macchanger<br/>wdutil                           |
 | Python          | logging<br/>requests                                        |
 | SOAR            | swimlane<br/>splunk soar                                    |
 | Recon           | nmap                                                        |
 | Test Automation | selenium                                                    |
 
 #### Requires
```

### Comparing `automonisaur-0.5.3/automonisaur.egg-info/SOURCES.txt` & `automonisaur-0.5.4/automonisaur.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 automon/helpers/subprocessWrapper/__init__.py
 automon/helpers/subprocessWrapper/exceptions.py
 automon/helpers/subprocessWrapper/run.py
 automon/helpers/subprocessWrapper/tests/__init__.py
 automon/helpers/subprocessWrapper/tests/test_run.py
 automon/helpers/subprocessWrapper/tests/test_runner.py
 automon/helpers/subprocessWrapper/tests/test_sanitize.py
+automon/helpers/subprocessWrapper/tests/test_text.py
 automon/helpers/tests/__init__.py
 automon/helpers/tests/test_assertions.py
 automon/helpers/tests/test_healthcheck.py
 automon/helpers/tests/test_helpers.py
 automon/helpers/tests/test_liveliness.py
 automon/helpers/tests/test_networking.py
 automon/helpers/tests/test_sanitation.py
@@ -83,20 +84,23 @@
 automon/integrations/elasticsearch/tests/test_elasticsearch_JvmMonitor.py
 automon/integrations/elasticsearch/tests/test_elasticsearch_client.py
 automon/integrations/elasticsearch/tests/test_elasticsearch_common.py
 automon/integrations/elasticsearch/tests/test_elasticsearch_snapshot.py
 automon/integrations/facebook/__init__.py
 automon/integrations/facebook/groups.py
 automon/integrations/flaskWrapper/__init__.py
+automon/integrations/flaskWrapper/app.py
 automon/integrations/flaskWrapper/auth.py
 automon/integrations/flaskWrapper/auth_creds.py
 automon/integrations/flaskWrapper/boilerplate.py
+automon/integrations/flaskWrapper/client.py
 automon/integrations/flaskWrapper/config.py
 automon/integrations/flaskWrapper/tests/__init__.py
 automon/integrations/flaskWrapper/tests/test_flask.py
+automon/integrations/flaskWrapper/tests/test_run.py
 automon/integrations/geoip/__init__.py
 automon/integrations/geoip/tests/__init__.py
 automon/integrations/geoip/tests/test_geoip.py
 automon/integrations/google/__init__.py
 automon/integrations/google/auth/__init__.py
 automon/integrations/google/auth/client.py
 automon/integrations/google/auth/config.py
@@ -153,14 +157,23 @@
 automon/integrations/mac/airport/tests/test_airport.py
 automon/integrations/mac/airport/tests/test_airport_neo4j.py
 automon/integrations/mac/macchanger/__init__.py
 automon/integrations/mac/macchanger/client.py
 automon/integrations/mac/macchanger/tests/__init__.py
 automon/integrations/mac/macchanger/tests/test_macchanger.py
 automon/integrations/mac/macchanger/tests/test_set_mac_random.py
+automon/integrations/mac/wdutil/__init__.py
+automon/integrations/mac/wdutil/client.py
+automon/integrations/mac/wdutil/config.py
+automon/integrations/mac/wdutil/exceptions.py
+automon/integrations/mac/wdutil/tests/__init__.py
+automon/integrations/mac/wdutil/tests/test_client_ready.py
+automon/integrations/mac/wdutil/tests/test_client_run.py
+automon/integrations/mac/wdutil/tests/test_config.py
+automon/integrations/mac/wdutil/tests/test_wdutil.py
 automon/integrations/minioWrapper/__init__.py
 automon/integrations/minioWrapper/assertions.py
 automon/integrations/minioWrapper/bucket.py
 automon/integrations/minioWrapper/client.py
 automon/integrations/minioWrapper/config.py
 automon/integrations/minioWrapper/object.py
 automon/integrations/minioWrapper/tests/__init__.py
@@ -217,17 +230,19 @@
 automon/integrations/seleniumWrapper/config.py
 automon/integrations/seleniumWrapper/config_window_size.py
 automon/integrations/seleniumWrapper/exceptions.py
 automon/integrations/seleniumWrapper/user_agents.py
 automon/integrations/seleniumWrapper/webdriver_chrome.py
 automon/integrations/seleniumWrapper/tests/__init__.py
 automon/integrations/seleniumWrapper/tests/test_browser.py
+automon/integrations/seleniumWrapper/tests/test_browser_cookies_autosave.py
 automon/integrations/seleniumWrapper/tests/test_browser_headless.py
 automon/integrations/seleniumWrapper/tests/test_browser_useragent.py
 automon/integrations/seleniumWrapper/tests/test_config.py
+automon/integrations/seleniumWrapper/tests/test_logs.py
 automon/integrations/seleniumWrapper/tests/test_new_browser.py
 automon/integrations/seleniumWrapper/tests/test_user_agent.py
 automon/integrations/sentryio/__init__.py
 automon/integrations/sentryio/client.py
 automon/integrations/sentryio/config.py
 automon/integrations/sentryio/tests/__init__.py
 automon/integrations/sentryio/tests/test_sentryio.py
@@ -315,12 +330,13 @@
 automon/integrations/vds/config.py
 automon/integrations/vds/tests/__init__.py
 automon/integrations/vds/tests/test_vds.py
 automon/log/__init__.py
 automon/log/attributes.py
 automon/log/logger.py
 automon/log/tests/__init__.py
+automon/log/tests/test_log_secret.py
 automon/log/tests/test_logger_builtin.py
 automonisaur.egg-info/PKG-INFO
 automonisaur.egg-info/SOURCES.txt
 automonisaur.egg-info/dependency_links.txt
 automonisaur.egg-info/top_level.txt
```

### Comparing `automonisaur-0.5.3/setup.py` & `automonisaur-0.5.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="automonisaur",
-    version="0.5.3",
+    version="0.5.4",
     author="naisanza",
     author_email="naisanza@gmail.com",
     description="Core libraries for automonisaur",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TheShellLand/automonisaur",
     packages=setuptools.find_packages(),
```

