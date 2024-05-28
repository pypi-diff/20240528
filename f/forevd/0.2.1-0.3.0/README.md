# Comparing `tmp/forevd-0.2.1.tar.gz` & `tmp/forevd-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forevd-0.2.1.tar", max compression
+gzip compressed data, was "forevd-0.3.0.tar", max compression
```

## Comparing `forevd-0.2.1.tar` & `forevd-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11357 2024-05-02 01:22:51.177572 forevd-0.2.1/LICENSE
--rw-r--r--   0        0        0     5628 2024-05-02 01:22:51.177572 forevd-0.2.1/README.md
--rw-r--r--   0        0        0        0 2024-05-02 01:22:51.177572 forevd-0.2.1/forevd/__init__.py
--rw-r--r--   0        0        0     6590 2024-05-02 01:22:51.177572 forevd-0.2.1/forevd/__main__.py
--rw-r--r--   0        0        0     1544 2024-05-02 01:22:51.177572 forevd-0.2.1/forevd/apache/__init__.py
--rw-r--r--   0        0        0     4840 2024-05-02 01:22:51.177572 forevd-0.2.1/forevd/apache/httpd.conf
--rw-r--r--   0        0        0      216 2024-05-02 01:22:51.177572 forevd-0.2.1/forevd/app.py
--rw-r--r--   0        0        0        0 2024-05-02 01:22:51.177572 forevd-0.2.1/forevd/resources/__init__.py
--rw-r--r--   0        0        0        0 2024-05-02 01:22:51.177572 forevd-0.2.1/forevd/resources/logging/__init__.py
--rw-r--r--   0        0        0      387 2024-05-02 01:22:51.177572 forevd-0.2.1/forevd/resources/logging/cli.conf
--rw-r--r--   0        0        0      910 2024-05-02 01:22:51.177572 forevd-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     6347 1970-01-01 00:00:00.000000 forevd-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-28 15:51:59.138551 forevd-0.3.0/LICENSE
+-rw-r--r--   0        0        0     5628 2024-05-28 15:51:59.138551 forevd-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-28 15:51:59.138551 forevd-0.3.0/forevd/__init__.py
+-rw-r--r--   0        0        0     6748 2024-05-28 15:51:59.138551 forevd-0.3.0/forevd/__main__.py
+-rw-r--r--   0        0        0     1544 2024-05-28 15:51:59.138551 forevd-0.3.0/forevd/apache/__init__.py
+-rw-r--r--   0        0        0     5337 2024-05-28 15:51:59.138551 forevd-0.3.0/forevd/apache/httpd.conf
+-rw-r--r--   0        0        0      216 2024-05-28 15:51:59.138551 forevd-0.3.0/forevd/app.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:51:59.138551 forevd-0.3.0/forevd/resources/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:51:59.138551 forevd-0.3.0/forevd/resources/logging/__init__.py
+-rw-r--r--   0        0        0      387 2024-05-28 15:51:59.138551 forevd-0.3.0/forevd/resources/logging/cli.conf
+-rw-r--r--   0        0        0      910 2024-05-28 15:51:59.138551 forevd-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6347 1970-01-01 00:00:00.000000 forevd-0.3.0/PKG-INFO
```

### Comparing `forevd-0.2.1/LICENSE` & `forevd-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `forevd-0.2.1/README.md` & `forevd-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `forevd-0.2.1/forevd/__main__.py` & `forevd-0.3.0/forevd/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,15 @@
     "--http-methods",
     help="Restrict HTTP method calls for the supplied list ",
     type=cli.StrList,
 )
 @click.option(
     "--httpd-include",
     help="Add your own config from a file into the generated httpd.conf",
-    type=cli.FromJsonOrYaml(),
+    type=cli.SlurpStrOrFile(),
 )
 @click.option(
     "--ldap",
     help="Provide the LDAP config in a JSON or YAML string or file",
     type=cli.FromJsonOrYaml(),
 )
 @click.option(
@@ -195,14 +195,19 @@
     "--set-access-token/--no-set-access-token",
     "set_access_token",
     help="Set the access token",
     is_flag=True,
     default=True,
 )
 @click.option(
+    "--ssl",
+    help="Provide the SSL config in a JSON or YAML string or file",
+    type=cli.FromJsonOrYaml(),
+)
+@click.option(
     "--var-dir",
     help="The backend of this reverse proxy will front, e.g. http://localhost:8080/foo",
     type=click.Path(),
     default=_DEFAULT_VAR_DIR,
     show_default=True,
 )
 # pylint: disable=too-many-arguments,too-many-locals
@@ -223,14 +228,15 @@
     listen,
     location,
     locations,
     mtls,
     oidc,
     server_name,
     set_access_token,
+    ssl,
     var_dir,
 ):
     """forevd is a forward/reverse proxy, primarily used as a sidecar for REST or any HTTP/s apps."""
     _setup_logging(debug)
 
     if (not backend or not location) and not locations:
         raise click.UsageError("You must supply a --backend and --location or --locations")
@@ -248,14 +254,15 @@
         "debug": debug,
         "ldap": ldap,
         "locations": _nomalize_locations(
             locations, backend, location, oidc, mtls, http_methods, set_access_token
         ),
         "listen": listen,
         "oidc": oidc,
+        "ssl": ssl,
         "server_name": server_name,
     }
     _LOGGER.debug(f"config: {config}")
 
     mod = importlib.import_module(f"forevd.{backend_type}")
 
     getattr(mod, "run")(var_dir, config, do_exec, cmd)
```

### Comparing `forevd-0.2.1/forevd/apache/__init__.py` & `forevd-0.3.0/forevd/apache/__init__.py`

 * *Files identical despite different names*

### Comparing `forevd-0.2.1/forevd/apache/httpd.conf` & `forevd-0.3.0/forevd/apache/httpd.conf`

 * *Files 8% similar despite different names*

```diff
@@ -56,19 +56,29 @@
 {% raw %}
 ErrorLogFormat "[%{cu}t] [%-m:%-l] %-a %-L %M"
 LogFormat "%h %l %u [%{%Y-%m-%d %H:%M:%S}t.%{usec_frac}t] \"%r\" %>s %b \ \"%{Referer}i\" \"%{User-Agent}i\"" combined
 {% endraw %}
 
 {% if cert -%}
 SSLEngine on
-SSLCipherSuite ALL:!EXP:!eNULL:!aNULL:!MD5:-LOW:-RC4:-SSLv2:+HIGH:+MEDIUM
+{% if ssl -%}
+{% for ssl_key in ssl  -%}
+SSL{{ ssl_key }} {{ ssl[ssl_key] }}
+{% endfor %}
+{% else %}
+# Sensible defaults, per https://httpd.apache.org/docs/trunk/en/ssl/ssl_howto.html
+SSLProtocol all -SSLv3 -TLSv1 -TLSv1.1
+SSLCipherSuite ECDHE-ECDSA-AES256-GCM-SHA384:ECDHE-RSA-AES256-GCM-SHA384:ECDHE-ECDSA-CHACHA20-POLY1305:ECDHE-RSA-CHACHA20-POLY1305:ECDHE-ECDSA-AES128-GCM-SHA256:ECDHE-RSA-AES128-GCM-SHA256:ECDHE-ECDSA-AES256-SHA384:ECDHE-RSA-AES256-SHA384:ECDHE-ECDSA-AES128-SHA256:ECDHE-RSA-AES128-SHA256
+SSLHonorCipherOrder on
+SSLCompression      off
+SSLSessionTickets   off
 SSLVerifyDepth 5
-SSLProtocol all -TLSv1.3
 SSLSessionCache "shmcb:/usr/local/apache2/logs/ssl_scache(512000)"
 SSLSessionCacheTimeout 300
+{% endif -%}
 
 SSLCACertificateFile {{ ca_cert }}
 SSLCertificateFile {{ cert }}
 SSLCertificateKeyFile {{ cert_key }}
 {% endif %}
 
 {% if oidc -%}
```

### Comparing `forevd-0.2.1/pyproject.toml` & `forevd-0.3.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "forevd"
-version = "0.2.1"
+version = "0.3.0"
 description = "Forward and reverse proxy using apache or nginx"
 authors = ["Erick Bourgeois <erick@jeb.ca>"]
 license = "LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
```

### Comparing `forevd-0.2.1/PKG-INFO` & `forevd-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forevd
-Version: 0.2.1
+Version: 0.3.0
 Summary: Forward and reverse proxy using apache or nginx
 License: LICENSE
 Author: Erick Bourgeois
 Author-email: erick@jeb.ca
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

