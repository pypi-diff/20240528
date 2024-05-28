# Comparing `tmp/precli-0.5.4.tar.gz` & `tmp/precli-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "precli-0.5.4.tar", last modified: Thu May  2 17:38:56 2024, max compression
+gzip compressed data, was "precli-0.5.5.tar", last modified: Tue May 28 20:46:17 2024, max compression
```

## Comparing `precli-0.5.4.tar` & `precli-0.5.5.tar`

### file list

```diff
@@ -1,740 +1,740 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.628040 precli-0.5.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.520039 precli-0.5.4/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-02 17:38:52.000000 precli-0.5.4/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-02 17:38:52.000000 precli-0.5.4/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.520039 precli-0.5.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-02 17:38:52.000000 precli-0.5.4/.github/workflows/dependency-review.yml
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-02 17:38:52.000000 precli-0.5.4/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-02 17:38:52.000000 precli-0.5.4/.github/workflows/publish-to-test-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-02 17:38:52.000000 precli-0.5.4/.github/workflows/unit-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-02 17:38:52.000000 precli-0.5.4/.github/workflows/upload-asset.yml
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-02 17:38:52.000000 precli-0.5.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-02 17:38:52.000000 precli-0.5.4/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-02 17:38:52.000000 precli-0.5.4/.stestr.conf
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-02 17:38:56.000000 precli-0.5.4/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-05-02 17:38:52.000000 precli-0.5.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)    18499 2024-05-02 17:38:56.000000 precli-0.5.4/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-05-02 17:38:52.000000 precli-0.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-02 17:38:56.624040 precli-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-02 17:38:52.000000 precli-0.5.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-02 17:38:52.000000 precli-0.5.4/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.520039 precli-0.5.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-02 17:38:52.000000 precli-0.5.4/docs/getting-started.md
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-02 17:38:52.000000 precli-0.5.4/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.520039 precli-0.5.4/docs/man/
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-02 17:38:52.000000 precli-0.5.4/docs/man/precli.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-02 17:38:52.000000 precli-0.5.4/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.504039 precli-0.5.4/docs/rules/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.504039 precli-0.5.4/docs/rules/go/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.520039 precli-0.5.4/docs/rules/go/stdlib/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-02 17:38:52.000000 precli-0.5.4/docs/rules/go/stdlib/crypto-weak-cipher.md
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-02 17:38:52.000000 precli-0.5.4/docs/rules/go/stdlib/crypto-weak-hash.md
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-02 17:38:52.000000 precli-0.5.4/docs/rules/go/stdlib/crypto-weak-key.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.504039 precli-0.5.4/docs/rules/java/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.524039 precli-0.5.4/docs/rules/java/stdlib/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-02 17:38:52.000000 precli-0.5.4/docs/rules/java/stdlib/java-net-insecure-cookie.md
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-02 17:38:52.000000 precli-0.5.4/docs/rules/java/stdlib/java-security-weak-hash.md
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-02 17:38:52.000000 precli-0.5.4/docs/rules/java/stdlib/java-security-weak-key.md
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-02 17:38:52.000000 precli-0.5.4/docs/rules/java/stdlib/java-security-weak-random.md
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-02 17:38:52.000000 precli-0.5.4/docs/rules/java/stdlib/javax-crypto-weak-cipher.md
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-02 17:38:52.000000 precli-0.5.4/docs/rules/java/stdlib/javax-servlet-http-insecure-cookie.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.504039 precli-0.5.4/docs/rules/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.528040 precli-0.5.4/docs/rules/python/stdlib/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-02 17:38:52.000000 precli-0.5.4/docs/rules/python/stdlib/argparse-sensitive-info.md
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-02 17:38:52.000000 precli-0.5.4/docs/rules/python/stdlib/assert.md
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-02 17:38:52.000000 precli-0.5.4/docs/rules/python/stdlib/crypt-weak-hash.md
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-02 17:38:52.000000 precli-0.5.4/docs/rules/python/stdlib/ftplib-cleartext.md
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-02 17:38:52.000000 precli-0.5.4/docs/rules/python/stdlib/ftplib-unverified-context.md
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-02 17:38:52.000000 precli-0.5.4/docs/rules/python/stdlib/hashlib-improper-prng.md
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-02 17:38:52.000000 precli-0.5.4/docs/rules/python/stdlib/hashlib-weak-hash.md
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-02 17:38:52.000000 precli-0.5.4/docs/rules/python/stdlib/hmac-timing-attack.md
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-02 17:38:52.000000 precli-0.5.4/docs/rules/python/stdlib/hmac-weak-hash.md
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-02 17:38:52.000000 precli-0.5.4/docs/rules/python/stdlib/hmac-weak-key.md
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-02 17:38:52.000000 precli-0.5.4/docs/rules/python/stdlib/http-server-unrestricted-bind.md
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-02 17:38:52.000000 precli-0.5.4/docs/rules/python/stdlib/http-url-secret.md
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-02 17:38:52.000000 precli-0.5.4/docs/rules/python/stdlib/imaplib-cleartext.md
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-02 17:38:52.000000 precli-0.5.4/docs/rules/python/stdlib/imaplib-unverified-context.md
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-02 17:38:52.000000 precli-0.5.4/docs/rules/python/stdlib/json-load.md
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-02 17:38:52.000000 precli-0.5.4/docs/rules/python/stdlib/logging-insecure-listen-config.md
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-02 17:38:52.000000 precli-0.5.4/docs/rules/python/stdlib/marshal-load.md
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-02 17:38:52.000000 precli-0.5.4/docs/rules/python/stdlib/nntplib-cleartext.md
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-02 17:38:52.000000 precli-0.5.4/docs/rules/python/stdlib/nntplib-unverified-context.md
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-02 17:38:52.000000 precli-0.5.4/docs/rules/python/stdlib/pickle-load.md
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-02 17:38:52.000000 precli-0.5.4/docs/rules/python/stdlib/poplib-cleartext.md
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-02 17:38:52.000000 precli-0.5.4/docs/rules/python/stdlib/poplib-unverified-context.md
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-02 17:38:52.000000 precli-0.5.4/docs/rules/python/stdlib/re-denial-of-service.md
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-02 17:38:52.000000 precli-0.5.4/docs/rules/python/stdlib/secrets-weak-token.md
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-02 17:38:52.000000 precli-0.5.4/docs/rules/python/stdlib/shelve-open.md
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-02 17:38:52.000000 precli-0.5.4/docs/rules/python/stdlib/smtplib-cleartext.md
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-02 17:38:52.000000 precli-0.5.4/docs/rules/python/stdlib/smtplib-unverified-context.md
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-02 17:38:52.000000 precli-0.5.4/docs/rules/python/stdlib/socket-unrestricted-bind.md
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-02 17:38:52.000000 precli-0.5.4/docs/rules/python/stdlib/socketserver-unrestricted-bind.md
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-02 17:38:52.000000 precli-0.5.4/docs/rules/python/stdlib/ssl-context-weak-key.md
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-02 17:38:52.000000 precli-0.5.4/docs/rules/python/stdlib/ssl-create-unverified-context.md
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-02 17:38:52.000000 precli-0.5.4/docs/rules/python/stdlib/ssl-insecure-tls-version.md
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-02 17:38:52.000000 precli-0.5.4/docs/rules/python/stdlib/telnetlib-cleartext.md
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-02 17:38:52.000000 precli-0.5.4/docs/rules/python/stdlib/tempfile-mktemp-race-condition.md
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-02 17:38:52.000000 precli-0.5.4/docs/rules/python/stdlib/xmlrpc-server-unrestricted-bind.md
--rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-05-02 17:38:52.000000 precli-0.5.4/docs/rules.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.528040 precli-0.5.4/logo/
--rw-r--r--   0 runner    (1001) docker     (127)   179541 2024-05-02 17:38:52.000000 precli-0.5.4/logo/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-02 17:38:52.000000 precli-0.5.4/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.528040 precli-0.5.4/precli/
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-02 17:38:52.000000 precli-0.5.4/precli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-02 17:38:52.000000 precli-0.5.4/precli/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.532039 precli-0.5.4/precli/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:52.000000 precli-0.5.4/precli/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-02 17:38:52.000000 precli-0.5.4/precli/cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.536039 precli-0.5.4/precli/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:52.000000 precli-0.5.4/precli/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-05-02 17:38:52.000000 precli-0.5.4/precli/core/argument.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-02 17:38:52.000000 precli-0.5.4/precli/core/artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-05-02 17:38:52.000000 precli-0.5.4/precli/core/call.py
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-02 17:38:52.000000 precli-0.5.4/precli/core/comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-02 17:38:52.000000 precli-0.5.4/precli/core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-02 17:38:52.000000 precli-0.5.4/precli/core/fix.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-02 17:38:52.000000 precli-0.5.4/precli/core/kind.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-02 17:38:52.000000 precli-0.5.4/precli/core/level.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-02 17:38:52.000000 precli-0.5.4/precli/core/linecache.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-02 17:38:52.000000 precli-0.5.4/precli/core/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-02 17:38:52.000000 precli-0.5.4/precli/core/location.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-02 17:38:52.000000 precli-0.5.4/precli/core/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     9636 2024-05-02 17:38:52.000000 precli-0.5.4/precli/core/redos.py
--rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-05-02 17:38:52.000000 precli-0.5.4/precli/core/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-05-02 17:38:52.000000 precli-0.5.4/precli/core/run.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-02 17:38:52.000000 precli-0.5.4/precli/core/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-05-02 17:38:52.000000 precli-0.5.4/precli/core/suppression.py
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-02 17:38:52.000000 precli-0.5.4/precli/core/symtab.py
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-02 17:38:52.000000 precli-0.5.4/precli/core/tool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-02 17:38:52.000000 precli-0.5.4/precli/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.536039 precli-0.5.4/precli/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)     7447 2024-05-02 17:38:52.000000 precli-0.5.4/precli/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7664 2024-05-02 17:38:52.000000 precli-0.5.4/precli/parsers/go.py
--rw-r--r--   0 runner    (1001) docker     (127)    13970 2024-05-02 17:38:52.000000 precli-0.5.4/precli/parsers/java.py
--rw-r--r--   0 runner    (1001) docker     (127)    18725 2024-05-02 17:38:52.000000 precli-0.5.4/precli/parsers/python.py
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-02 17:38:52.000000 precli-0.5.4/precli/parsers/tokens.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.536039 precli-0.5.4/precli/renderers/
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-02 17:38:52.000000 precli-0.5.4/precli/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-05-02 17:38:52.000000 precli-0.5.4/precli/renderers/detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-02 17:38:52.000000 precli-0.5.4/precli/renderers/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-02 17:38:52.000000 precli-0.5.4/precli/renderers/markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-05-02 17:38:52.000000 precli-0.5.4/precli/renderers/plain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.536039 precli-0.5.4/precli/rules/
--rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-05-02 17:38:52.000000 precli-0.5.4/precli/rules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.536039 precli-0.5.4/precli/rules/go/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:52.000000 precli-0.5.4/precli/rules/go/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.540040 precli-0.5.4/precli/rules/go/stdlib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:52.000000 precli-0.5.4/precli/rules/go/stdlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-05-02 17:38:52.000000 precli-0.5.4/precli/rules/go/stdlib/crypto_weak_cipher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-05-02 17:38:52.000000 precli-0.5.4/precli/rules/go/stdlib/crypto_weak_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-05-02 17:38:52.000000 precli-0.5.4/precli/rules/go/stdlib/crypto_weak_key.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.540040 precli-0.5.4/precli/rules/java/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:52.000000 precli-0.5.4/precli/rules/java/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.540040 precli-0.5.4/precli/rules/java/stdlib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:52.000000 precli-0.5.4/precli/rules/java/stdlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-02 17:38:52.000000 precli-0.5.4/precli/rules/java/stdlib/java_net_insecure_cookie.py
--rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-05-02 17:38:52.000000 precli-0.5.4/precli/rules/java/stdlib/java_security_weak_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-05-02 17:38:52.000000 precli-0.5.4/precli/rules/java/stdlib/java_security_weak_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-05-02 17:38:52.000000 precli-0.5.4/precli/rules/java/stdlib/java_security_weak_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     6538 2024-05-02 17:38:52.000000 precli-0.5.4/precli/rules/java/stdlib/javax_crypto_weak_cipher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-05-02 17:38:52.000000 precli-0.5.4/precli/rules/java/stdlib/javax_servlet_http_insecure_cookie.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.540040 precli-0.5.4/precli/rules/python/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:52.000000 precli-0.5.4/precli/rules/python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.544040 precli-0.5.4/precli/rules/python/stdlib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:52.000000 precli-0.5.4/precli/rules/python/stdlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-05-02 17:38:52.000000 precli-0.5.4/precli/rules/python/stdlib/argparse_sensitive_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-05-02 17:38:52.000000 precli-0.5.4/precli/rules/python/stdlib/assert.py
--rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-05-02 17:38:52.000000 precli-0.5.4/precli/rules/python/stdlib/crypt_weak_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     5333 2024-05-02 17:38:52.000000 precli-0.5.4/precli/rules/python/stdlib/ftplib_cleartext.py
--rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-05-02 17:38:52.000000 precli-0.5.4/precli/rules/python/stdlib/ftplib_unverified_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     4834 2024-05-02 17:38:52.000000 precli-0.5.4/precli/rules/python/stdlib/hashlib_improper_prng.py
--rw-r--r--   0 runner    (1001) docker     (127)     6956 2024-05-02 17:38:52.000000 precli-0.5.4/precli/rules/python/stdlib/hashlib_weak_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-05-02 17:38:52.000000 precli-0.5.4/precli/rules/python/stdlib/hmac_timing_attack.py
--rw-r--r--   0 runner    (1001) docker     (127)     6580 2024-05-02 17:38:52.000000 precli-0.5.4/precli/rules/python/stdlib/hmac_weak_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     6813 2024-05-02 17:38:52.000000 precli-0.5.4/precli/rules/python/stdlib/hmac_weak_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-05-02 17:38:52.000000 precli-0.5.4/precli/rules/python/stdlib/http_server_unrestricted_bind.py
--rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-05-02 17:38:52.000000 precli-0.5.4/precli/rules/python/stdlib/http_url_secret.py
--rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-05-02 17:38:52.000000 precli-0.5.4/precli/rules/python/stdlib/imaplib_cleartext.py
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-05-02 17:38:52.000000 precli-0.5.4/precli/rules/python/stdlib/imaplib_unverified_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-02 17:38:52.000000 precli-0.5.4/precli/rules/python/stdlib/json_load.py
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-05-02 17:38:52.000000 precli-0.5.4/precli/rules/python/stdlib/logging_insecure_listen_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-02 17:38:52.000000 precli-0.5.4/precli/rules/python/stdlib/marshal_load.py
--rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-05-02 17:38:52.000000 precli-0.5.4/precli/rules/python/stdlib/nntplib_cleartext.py
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-05-02 17:38:52.000000 precli-0.5.4/precli/rules/python/stdlib/nntplib_unverified_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-02 17:38:52.000000 precli-0.5.4/precli/rules/python/stdlib/pickle_load.py
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-05-02 17:38:52.000000 precli-0.5.4/precli/rules/python/stdlib/poplib_cleartext.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-02 17:38:52.000000 precli-0.5.4/precli/rules/python/stdlib/poplib_unverified_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-02 17:38:52.000000 precli-0.5.4/precli/rules/python/stdlib/re_denial_of_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-05-02 17:38:52.000000 precli-0.5.4/precli/rules/python/stdlib/secrets_weak_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-05-02 17:38:52.000000 precli-0.5.4/precli/rules/python/stdlib/shelve_open.py
--rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-05-02 17:38:52.000000 precli-0.5.4/precli/rules/python/stdlib/smtplib_cleartext.py
--rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-05-02 17:38:52.000000 precli-0.5.4/precli/rules/python/stdlib/smtplib_unverified_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-02 17:38:52.000000 precli-0.5.4/precli/rules/python/stdlib/socket_unrestricted_bind.py
--rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-05-02 17:38:52.000000 precli-0.5.4/precli/rules/python/stdlib/socketserver_unrestricted_bind.py
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-05-02 17:38:52.000000 precli-0.5.4/precli/rules/python/stdlib/ssl_context_weak_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-05-02 17:38:52.000000 precli-0.5.4/precli/rules/python/stdlib/ssl_create_unverified_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     6515 2024-05-02 17:38:52.000000 precli-0.5.4/precli/rules/python/stdlib/ssl_insecure_tls_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-05-02 17:38:52.000000 precli-0.5.4/precli/rules/python/stdlib/telnetlib_cleartext.py
--rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-05-02 17:38:52.000000 precli-0.5.4/precli/rules/python/stdlib/tempfile_mktemp_race_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-05-02 17:38:52.000000 precli-0.5.4/precli/rules/python/stdlib/xmlrpc_server_unrestricted_bind.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.624040 precli-0.5.4/precli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-02 17:38:56.000000 precli-0.5.4/precli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    39386 2024-05-02 17:38:56.000000 precli-0.5.4/precli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 17:38:56.000000 precli-0.5.4/precli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-02 17:38:56.000000 precli-0.5.4/precli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 17:38:56.000000 precli-0.5.4/precli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-02 17:38:56.000000 precli-0.5.4/precli.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-02 17:38:56.000000 precli-0.5.4/precli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 17:38:56.000000 precli-0.5.4/precli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-02 17:38:52.000000 precli-0.5.4/pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-02 17:38:52.000000 precli-0.5.4/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.548040 precli-0.5.4/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)       94 2024-05-02 17:38:52.000000 precli-0.5.4/scripts/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     4389 2024-05-02 17:38:56.628040 precli-0.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-02 17:38:52.000000 precli-0.5.4/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-02 17:38:52.000000 precli-0.5.4/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.548040 precli-0.5.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:52.000000 precli-0.5.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.548040 precli-0.5.4/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.548040 precli-0.5.4/tests/unit/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.548040 precli-0.5.4/tests/unit/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/core/test_python.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.548040 precli-0.5.4/tests/unit/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.552040 precli-0.5.4/tests/unit/parsers/examples/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/parsers/examples/expression_list_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/parsers/examples/expression_list_assignment_uneven.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/parsers/examples/importlib_import_module.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/parsers/examples/suppress.go
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/parsers/examples/suppress.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/parsers/examples/suppress_lowercase_rule.go
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/parsers/examples/suppress_lowercase_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/parsers/examples/suppress_multiline.go
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/parsers/examples/suppress_multiline.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/parsers/examples/suppress_multiple_comments.go
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/parsers/examples/suppress_multiple_comments.py
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/parsers/examples/suppress_multiple_rules.go
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/parsers/examples/suppress_multiple_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/parsers/examples/suppress_preceding.go
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/parsers/examples/suppress_preceding.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/parsers/examples/suppress_spaced_rules.go
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/parsers/examples/suppress_spaced_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/parsers/examples/suppress_wrong_rule.go
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/parsers/examples/suppress_wrong_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     5514 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/parsers/test_go.py
--rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/parsers/test_python.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.552040 precli-0.5.4/tests/unit/rules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.552040 precli-0.5.4/tests/unit/rules/go/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/go/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.552040 precli-0.5.4/tests/unit/rules/go/stdlib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/go/stdlib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.552040 precli-0.5.4/tests/unit/rules/go/stdlib/crypto/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/go/stdlib/crypto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.556040 precli-0.5.4/tests/unit/rules/go/stdlib/crypto/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_cipher_aes.go
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_cipher_des.go
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_cipher_rc4.go
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_hash_md5_new.go
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_hash_md5_sum.go
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_hash_sha1_new.go
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_hash_sha1_sum.go
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_hash_sha256_new.go
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_hash_sha256_sum.go
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_dsa_1024.go
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_dsa_2048.go
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_dsa_3072.go
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_1024.go
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_2048.go
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_4096.go
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_bits_as_var.go
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/go/stdlib/crypto/test_crypto_weak_cipher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/go/stdlib/crypto/test_crypto_weak_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/go/stdlib/crypto/test_crypto_weak_key.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.556040 precli-0.5.4/tests/unit/rules/java/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/java/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.556040 precli-0.5.4/tests/unit/rules/java/stdlib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/java/stdlib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.556040 precli-0.5.4/tests/unit/rules/java/stdlib/java_net/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/java/stdlib/java_net/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.556040 precli-0.5.4/tests/unit/rules/java/stdlib/java_net/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/java/stdlib/java_net/examples/HttpCookieSecureFalse.java
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/java/stdlib/java_net/examples/HttpCookieSecureTrue.java
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/java/stdlib/java_net/test_insecure_cookie.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.556040 precli-0.5.4/tests/unit/rules/java/stdlib/java_security/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/java/stdlib/java_security/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.556040 precli-0.5.4/tests/unit/rules/java/stdlib/java_security/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/java/stdlib/java_security/examples/JavaSecuritySecureRandomSHA1PRNG.java
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/java/stdlib/java_security/examples/KeyPairGeneratorDSA.java
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/java/stdlib/java_security/examples/KeyPairGeneratorRSA.java
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/java/stdlib/java_security/examples/MessageDigestMD2.java
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/java/stdlib/java_security/examples/MessageDigestMD5.java
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/java/stdlib/java_security/examples/MessageDigestMD5Property.java
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/java/stdlib/java_security/examples/MessageDigestSHA1.java
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/java/stdlib/java_security/examples/MessageDigestSHA256.java
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/java/stdlib/java_security/examples/SecureRandomDefault.java
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/java/stdlib/java_security/examples/SecureRandomSHA1PRNG.java
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/java/stdlib/java_security/test_weak_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/java/stdlib/java_security/test_weak_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/java/stdlib/java_security/test_weak_random.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.556040 precli-0.5.4/tests/unit/rules/java/stdlib/javax_crypto/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/java/stdlib/javax_crypto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.560040 precli-0.5.4/tests/unit/rules/java/stdlib/javax_crypto/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/java/stdlib/javax_crypto/examples/Cipher3DESCBC.java
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherAESCBC.java
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherArcfour.java
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherBlowfishCBC.java
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherDESCBC.java
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherRC2.java
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherRC4.java
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherRC5.java
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/java/stdlib/javax_crypto/test_weak_cipher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.560040 precli-0.5.4/tests/unit/rules/java/stdlib/javax_servlet_http/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/java/stdlib/javax_servlet_http/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.560040 precli-0.5.4/tests/unit/rules/java/stdlib/javax_servlet_http/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/java/stdlib/javax_servlet_http/examples/CookieSecureFalse.java
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/java/stdlib/javax_servlet_http/examples/CookieSecureTrue.java
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/java/stdlib/javax_servlet_http/test_insecure_cookie.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.560040 precli-0.5.4/tests/unit/rules/python/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.560040 precli-0.5.4/tests/unit/rules/python/stdlib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.560040 precli-0.5.4/tests/unit/rules/python/stdlib/argparse/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/argparse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.560040 precli-0.5.4/tests/unit/rules/python/stdlib/argparse/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/argparse/examples/argparse_add_argument_api_key.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/argparse/examples/argparse_add_argument_default_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/argparse/examples/argparse_add_argument_password.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/argparse/examples/argparse_add_argument_password_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/argparse/examples/argparse_add_argument_password_store_true.py
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/argparse/test_argparse_sensitive_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.560040 precli-0.5.4/tests/unit/rules/python/stdlib/assert/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/assert/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.560040 precli-0.5.4/tests/unit/rules/python/stdlib/assert/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/assert/examples/assert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/assert/test_assert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.564040 precli-0.5.4/tests/unit/rules/python/stdlib/crypt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/crypt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.564040 precli-0.5.4/tests/unit/rules/python/stdlib/crypt/examples/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/crypt/examples/crypt_crypt.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/crypt/examples/crypt_crypt_method_blowfish.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/crypt/examples/crypt_crypt_method_crypt.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/crypt/examples/crypt_crypt_method_md5.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/crypt/examples/crypt_crypt_method_sha256.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/crypt/examples/crypt_crypt_method_sha512.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/crypt/examples/crypt_mksalt.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/crypt/examples/crypt_mksalt_method_blowfish.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/crypt/examples/crypt_mksalt_method_crypt.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/crypt/examples/crypt_mksalt_method_md5.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/crypt/examples/crypt_mksalt_method_sha256.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/crypt/examples/crypt_mksalt_method_sha512.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/crypt/test_crypt_weak_hash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.564040 precli-0.5.4/tests/unit/rules/python/stdlib/ftplib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ftplib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.568040 precli-0.5.4/tests/unit/rules/python/stdlib/ftplib/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ftplib/examples/ftp.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ftplib/examples/ftp_context_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ftplib/examples/ftp_login.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ftplib/examples/ftp_tls.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_context_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_login.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_login_single_statement.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_tls.py
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_tls_context_as_var.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_tls_context_none.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_tls_context_unset.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_tls_user_password.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_user_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ftplib/test_ftplib_cleartext.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ftplib/test_ftplib_unverified_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.568040 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.576040 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_blake2b.py
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_blake2s.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_improper_prng_blake2b.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_improper_prng_blake2s.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_improper_prng_pbkdf2_hmac.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_improper_prng_scrypt.py
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_md4.py
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_md5.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_md5_as_identifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_md5_importlib.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_md5_usedforsecurity_true.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_blake2b.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_blake2s.py
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_md4.py
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_md5.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_md5_sha1.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_md5_usedforsecurity_true.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_name_sha.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_ripemd160.py
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha1.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha224.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha256.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha384.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha3_224.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha3_256.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha3_384.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha3_512.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha512.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha_usedforsecurity_false.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_shake_128.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_shake_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_md4.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_md5.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_ripemd160.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha1.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha224.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha256.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha384.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha3_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha3_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha3_384.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha3_512.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_shake_128.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_shake_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_ripemd160.py
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha1.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha224.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha256.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha384.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha3_224.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha3_256.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha3_384.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha3_512.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha512.py
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha_usedforsecurity_false.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_shake_128.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_shake_256.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/test_hashlib_improper_prng.py
--rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/test_hashlib_weak_hash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.580040 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.592040 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_blake2b.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_blake2s.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_blake2b.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_blake2s.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_md4.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_md5.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_ripemd160.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha1.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha224.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha256.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha384.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha3_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha3_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha3_384.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha3_512.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha512.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_shake_128.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_shake_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_md4.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_md5.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_md5_sha1.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_ripemd160.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha1.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha224.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha256.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha384.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha3_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha3_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha3_384.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha3_512.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha512.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_shake_128.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_shake_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_weak_key_hashlib_blake2b.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_weak_key_hashlib_sha3_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_weak_key_hashlib_sm3.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_weak_key_sha224.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_weak_key_sha256.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_weak_key_sha512.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_blake2b.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_blake2s.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_blake2b.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_blake2s.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_md4.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_md5.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_ripemd160.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha1.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha224.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha256.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha384.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha3_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha3_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha3_384.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha3_512.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha512.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_shake_128.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_shake_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_md4.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_md5.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_md5_sha1.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_ripemd160.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha1.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha224.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha256.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha384.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha3_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha3_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha3_384.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha3_512.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha512.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_shake_128.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_shake_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_weak_key_blake2s.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_weak_key_hashlib_sha3_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_weak_key_hashlib_sha3_384.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_weak_key_hashlib_sha3_512.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_weak_key_sha384.py
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_weak_key_sha512_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_timing_attack.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_timing_attack_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_timing_attack_class_hexdigest.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_timing_attack_compare_digest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/test_hmac_timing_attack.py
--rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/test_hmac_weak_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/hmac/test_hmac_weak_key.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.592040 precli-0.5.4/tests/unit/rules/python/stdlib/http/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/http/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.596040 precli-0.5.4/tests/unit/rules/python/stdlib/http/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/http/examples/http_server_http_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/http/examples/http_server_threading_http_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/http/examples/http_url_secret_apikey.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/http/examples/http_url_secret_apikey_in_header.py
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/http/examples/http_url_secret_basic_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/http/examples/http_url_secret_basic_auth_as_var.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/http/examples/http_url_secret_password.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/http/examples/http_url_secret_username.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/http/test_http_server_unrestricted_bind.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/http/test_http_url_secret.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.596040 precli-0.5.4/tests/unit/rules/python/stdlib/imaplib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/imaplib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.596040 precli-0.5.4/tests/unit/rules/python/stdlib/imaplib/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_authenticate.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_context_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_login.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_login_cram_md5.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_ssl.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_ssl_context_as_var.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_ssl_context_none.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_ssl_context_unset.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_starttls.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_starttls_context_as_var.py
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_starttls_context_none.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_starttls_context_unset.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/imaplib/test_imaplib_cleartext.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/imaplib/test_imaplib_unverified_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.596040 precli-0.5.4/tests/unit/rules/python/stdlib/json/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/json/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.600040 precli-0.5.4/tests/unit/rules/python/stdlib/json/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/json/examples/json_jsondecoder_decode.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/json/examples/json_load.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/json/examples/json_loads.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/json/test_json_load.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.600040 precli-0.5.4/tests/unit/rules/python/stdlib/logging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/logging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.600040 precli-0.5.4/tests/unit/rules/python/stdlib/logging/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/logging/examples/insecure_listen_config_empty_args.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/logging/examples/insecure_listen_config_port.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/logging/examples/insecure_listen_config_port_verify_as_var.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/logging/examples/insecure_listen_config_port_verify_none.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/logging/examples/insecure_listen_config_verify_none.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/logging/examples/insecure_listen_config_verify_none_port.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/logging/examples/insecure_listen_config_verify_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/logging/test_logging_insecure_listen_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.600040 precli-0.5.4/tests/unit/rules/python/stdlib/marshal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/marshal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.600040 precli-0.5.4/tests/unit/rules/python/stdlib/marshal/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/marshal/examples/marshal_load.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/marshal/examples/marshal_loads.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/marshal/test_marshal_load.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.600040 precli-0.5.4/tests/unit/rules/python/stdlib/nntplib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/nntplib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.604040 precli-0.5.4/tests/unit/rules/python/stdlib/nntplib/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_context_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_login.py
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_ssl.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_ssl_context_as_var.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_ssl_context_none.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_ssl_context_unset.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_starttls.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_starttls_context_as_var.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_starttls_context_none.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_starttls_context_unset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/nntplib/test_nntplib_cleartext.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/nntplib/test_nntplib_unverified_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.604040 precli-0.5.4/tests/unit/rules/python/stdlib/pickle/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/pickle/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.604040 precli-0.5.4/tests/unit/rules/python/stdlib/pickle/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/pickle/examples/pickle_load.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/pickle/examples/pickle_loads.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/pickle/examples/pickle_unpickler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/pickle/test_pickle_load.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.604040 precli-0.5.4/tests/unit/rules/python/stdlib/poplib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/poplib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.608040 precli-0.5.4/tests/unit/rules/python/stdlib/poplib/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_apop.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_context_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_pass_.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_rpop.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_ssl.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_ssl_context_as_var.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_ssl_context_none.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_ssl_context_unset.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_stls.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_stls_context_as_var.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_stls_context_none.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_stls_context_unset.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/poplib/test_poplib_cleartext.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/poplib/test_poplib_unverified_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.608040 precli-0.5.4/tests/unit/rules/python/stdlib/re/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/re/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.608040 precli-0.5.4/tests/unit/rules/python/stdlib/re/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/re/examples/re_compile.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/re/examples/re_compile_good.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/re/examples/re_findall.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/re/examples/re_finditer.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/re/examples/re_fullmatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/re/examples/re_match.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/re/examples/re_search.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/re/examples/re_search_good.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/re/examples/re_split.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/re/examples/re_sub.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/re/examples/re_subn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/re/test_re_denial_of_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.608040 precli-0.5.4/tests/unit/rules/python/stdlib/secrets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/secrets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.608040 precli-0.5.4/tests/unit/rules/python/stdlib/secrets/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/secrets/examples/secrets_token_bytes.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/secrets/examples/secrets_token_bytes_default.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/secrets/examples/secrets_token_bytes_size_var.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/secrets/examples/secrets_token_hex.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/secrets/examples/secrets_token_urlsafe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/secrets/test_secrets_weak_token.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.612040 precli-0.5.4/tests/unit/rules/python/stdlib/shelve/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/shelve/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.612040 precli-0.5.4/tests/unit/rules/python/stdlib/shelve/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/shelve/examples/shelve_dbfilenameshelf.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/shelve/examples/shelve_open.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/shelve/examples/shelve_open_context_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/shelve/test_shelve_open.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.612040 precli-0.5.4/tests/unit/rules/python/stdlib/smtplib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/smtplib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.612040 precli-0.5.4/tests/unit/rules/python/stdlib/smtplib/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_context_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_login.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl_context_as_var.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl_context_none.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl_context_unset.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls_context_as_var.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls_context_none.py
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls_context_unset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/smtplib/test_smtplib_cleartext.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/smtplib/test_smtplib_unverified_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.612040 precli-0.5.4/tests/unit/rules/python/stdlib/socket/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/socket/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.612040 precli-0.5.4/tests/unit/rules/python/stdlib/socket/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/socket/examples/socket_create_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/socket/examples/socket_socket_bind.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/socket/examples/socket_socket_bind_as_var.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/socket/examples/socket_socket_bind_as_vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/socket/test_socket_unrestricted_bind.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.616040 precli-0.5.4/tests/unit/rules/python/stdlib/socketserver/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/socketserver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.616040 precli-0.5.4/tests/unit/rules/python/stdlib/socketserver/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_forking_tcp_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_forking_udp_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_tcp_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_threading_tcp_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_threading_udp_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_udp_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/socketserver/test_socketserver_unrestricted_bind.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.616040 precli-0.5.4/tests/unit/rules/python/stdlib/ssl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ssl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.624040 precli-0.5.4/tests/unit/rules/python/stdlib/ssl/examples/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ssl/examples/create_default_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ssl/examples/create_unverified_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ssl/examples/get_server_certificate_sslv2.py
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ssl/examples/get_server_certificate_sslv23.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ssl/examples/get_server_certificate_sslv3.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ssl/examples/get_server_certificate_tlsv1.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ssl/examples/get_server_certificate_tlsv11.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ssl/examples/get_server_certificate_tlsv12.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_brainpoolP256r1.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_brainpoolP384r1.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_brainpoolP384r1tls13.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_brainpoolP512r1.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_default_context.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_ffdhe2048.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_prime192v1.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_prime256v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_secp160r2.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_secp256r1.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_sect163k1.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_sect571k1.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_typed_default_param.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_typed_param.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_unverified_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_sslv2.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_sslv23.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_sslv3.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_tlsv1.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_tlsv11.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_tlsv12.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ssl/examples/wrap_socket_sslv2.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ssl/examples/wrap_socket_sslv23.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ssl/examples/wrap_socket_sslv2_server_side_true.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ssl/examples/wrap_socket_sslv3.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ssl/examples/wrap_socket_tlsv1.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ssl/examples/wrap_socket_tlsv11.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ssl/examples/wrap_socket_tlsv12.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ssl/test_ssl_context_tls_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ssl/test_ssl_context_weak_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ssl/test_ssl_create_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ssl/test_ssl_get_server_certificate_tls_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/ssl/test_ssl_wrap_socket_tls_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.624040 precli-0.5.4/tests/unit/rules/python/stdlib/telnetlib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/telnetlib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.624040 precli-0.5.4/tests/unit/rules/python/stdlib/telnetlib/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/telnetlib/examples/telnet.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/telnetlib/examples/telnetlib_telnet.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/telnetlib/examples/telnetlib_telnet_context_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/telnetlib/test_telnetlib_cleartext.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.624040 precli-0.5.4/tests/unit/rules/python/stdlib/tempfile/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/tempfile/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.624040 precli-0.5.4/tests/unit/rules/python/stdlib/tempfile/examples/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/tempfile/examples/tempfile_mktemp.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/tempfile/examples/tempfile_mktemp_args_open.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/tempfile/examples/tempfile_mktemp_args_with_open_args.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/tempfile/examples/tempfile_mktemp_open.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/tempfile/examples/tempfile_mktemp_walrus_open.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/tempfile/examples/tempfile_mktemp_with_open.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/tempfile/examples/tempfile_mktemp_with_open_multiline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/tempfile/test_tempfile_mktemp_race_condition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.624040 precli-0.5.4/tests/unit/rules/python/stdlib/xmlrpc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/xmlrpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:38:56.624040 precli-0.5.4/tests/unit/rules/python/stdlib/xmlrpc/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/xmlrpc/examples/xmlrpc_server_doc_xml_rpc_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/xmlrpc/examples/xmlrpc_server_simple_xml_rpc_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/python/stdlib/xmlrpc/test_xmlrpc_server_unrestricted_bind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-02 17:38:52.000000 precli-0.5.4/tests/unit/rules/test_case.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-02 17:38:52.000000 precli-0.5.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.779386 precli-0.5.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.667387 precli-0.5.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-28 20:46:14.000000 precli-0.5.5/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-28 20:46:14.000000 precli-0.5.5/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.667387 precli-0.5.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-28 20:46:14.000000 precli-0.5.5/.github/workflows/dependency-review.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-28 20:46:14.000000 precli-0.5.5/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-28 20:46:14.000000 precli-0.5.5/.github/workflows/publish-to-test-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-28 20:46:14.000000 precli-0.5.5/.github/workflows/unit-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-28 20:46:14.000000 precli-0.5.5/.github/workflows/upload-asset.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-28 20:46:14.000000 precli-0.5.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-28 20:46:14.000000 precli-0.5.5/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-28 20:46:17.000000 precli-0.5.5/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-05-28 20:46:14.000000 precli-0.5.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)    19910 2024-05-28 20:46:17.000000 precli-0.5.5/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-05-28 20:46:14.000000 precli-0.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-28 20:46:17.779386 precli-0.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-28 20:46:14.000000 precli-0.5.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-28 20:46:14.000000 precli-0.5.5/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.667387 precli-0.5.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-28 20:46:14.000000 precli-0.5.5/docs/getting-started.md
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-28 20:46:14.000000 precli-0.5.5/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.667387 precli-0.5.5/docs/man/
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-28 20:46:14.000000 precli-0.5.5/docs/man/precli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-28 20:46:14.000000 precli-0.5.5/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.655387 precli-0.5.5/docs/rules/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.651387 precli-0.5.5/docs/rules/go/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.667387 precli-0.5.5/docs/rules/go/stdlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/go/stdlib/crypto-weak-cipher.md
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/go/stdlib/crypto-weak-hash.md
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/go/stdlib/crypto-weak-key.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.655387 precli-0.5.5/docs/rules/java/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.671387 precli-0.5.5/docs/rules/java/stdlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/java/stdlib/java-net-insecure-cookie.md
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/java/stdlib/java-security-weak-hash.md
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/java/stdlib/java-security-weak-key.md
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/java/stdlib/java-security-weak-random.md
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/java/stdlib/javax-crypto-weak-cipher.md
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/java/stdlib/javax-servlet-http-insecure-cookie.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.655387 precli-0.5.5/docs/rules/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.675387 precli-0.5.5/docs/rules/python/stdlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/argparse-sensitive-info.md
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/assert.md
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/crypt-weak-hash.md
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/ftplib-cleartext.md
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/ftplib-unverified-context.md
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/hashlib-improper-prng.md
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/hashlib-weak-hash.md
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/hmac-timing-attack.md
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/hmac-weak-hash.md
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/hmac-weak-key.md
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/http-server-unrestricted-bind.md
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/http-url-secret.md
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/imaplib-cleartext.md
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/imaplib-unverified-context.md
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/json-load.md
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/logging-insecure-listen-config.md
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/marshal-load.md
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/nntplib-cleartext.md
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/nntplib-unverified-context.md
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/pickle-load.md
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/poplib-cleartext.md
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/poplib-unverified-context.md
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/re-denial-of-service.md
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/secrets-weak-token.md
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/shelve-open.md
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/smtplib-cleartext.md
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/smtplib-unverified-context.md
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/socket-unrestricted-bind.md
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/socketserver-unrestricted-bind.md
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/ssl-context-weak-key.md
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/ssl-create-unverified-context.md
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/ssl-insecure-tls-version.md
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/telnetlib-cleartext.md
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/tempfile-mktemp-race-condition.md
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/xmlrpc-server-unrestricted-bind.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.675387 precli-0.5.5/logo/
+-rw-r--r--   0 runner    (1001) docker     (127)   179541 2024-05-28 20:46:14.000000 precli-0.5.5/logo/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-28 20:46:14.000000 precli-0.5.5/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.675387 precli-0.5.5/precli/
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-28 20:46:14.000000 precli-0.5.5/precli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-28 20:46:14.000000 precli-0.5.5/precli/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.679386 precli-0.5.5/precli/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/precli/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11643 2024-05-28 20:46:14.000000 precli-0.5.5/precli/cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.683386 precli-0.5.5/precli/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/precli/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-28 20:46:14.000000 precli-0.5.5/precli/core/argument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-28 20:46:14.000000 precli-0.5.5/precli/core/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-28 20:46:14.000000 precli-0.5.5/precli/core/call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-28 20:46:14.000000 precli-0.5.5/precli/core/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-28 20:46:14.000000 precli-0.5.5/precli/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-28 20:46:14.000000 precli-0.5.5/precli/core/fix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-28 20:46:14.000000 precli-0.5.5/precli/core/kind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-28 20:46:14.000000 precli-0.5.5/precli/core/level.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-28 20:46:14.000000 precli-0.5.5/precli/core/linecache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-28 20:46:14.000000 precli-0.5.5/precli/core/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-28 20:46:14.000000 precli-0.5.5/precli/core/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-28 20:46:14.000000 precli-0.5.5/precli/core/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9635 2024-05-28 20:46:14.000000 precli-0.5.5/precli/core/redos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-05-28 20:46:14.000000 precli-0.5.5/precli/core/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6475 2024-05-28 20:46:14.000000 precli-0.5.5/precli/core/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-28 20:46:14.000000 precli-0.5.5/precli/core/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-28 20:46:14.000000 precli-0.5.5/precli/core/suppression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-28 20:46:14.000000 precli-0.5.5/precli/core/symtab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-28 20:46:14.000000 precli-0.5.5/precli/core/tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-28 20:46:14.000000 precli-0.5.5/precli/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.683386 precli-0.5.5/precli/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)     7123 2024-05-28 20:46:14.000000 precli-0.5.5/precli/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-05-28 20:46:14.000000 precli-0.5.5/precli/parsers/go.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13916 2024-05-28 20:46:14.000000 precli-0.5.5/precli/parsers/java.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19412 2024-05-28 20:46:14.000000 precli-0.5.5/precli/parsers/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-28 20:46:14.000000 precli-0.5.5/precli/parsers/tokens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.683386 precli-0.5.5/precli/renderers/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-28 20:46:14.000000 precli-0.5.5/precli/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5682 2024-05-28 20:46:14.000000 precli-0.5.5/precli/renderers/detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-05-28 20:46:14.000000 precli-0.5.5/precli/renderers/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-05-28 20:46:14.000000 precli-0.5.5/precli/renderers/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-28 20:46:14.000000 precli-0.5.5/precli/renderers/plain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.683386 precli-0.5.5/precli/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.683386 precli-0.5.5/precli/rules/go/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/go/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.683386 precli-0.5.5/precli/rules/go/stdlib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/go/stdlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5475 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/go/stdlib/crypto_weak_cipher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/go/stdlib/crypto_weak_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/go/stdlib/crypto_weak_key.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.683386 precli-0.5.5/precli/rules/java/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/java/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.687387 precli-0.5.5/precli/rules/java/stdlib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/java/stdlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/java/stdlib/java_net_insecure_cookie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/java/stdlib/java_security_weak_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/java/stdlib/java_security_weak_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/java/stdlib/java_security_weak_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6537 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/java/stdlib/javax_crypto_weak_cipher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/java/stdlib/javax_servlet_http_insecure_cookie.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.687387 precli-0.5.5/precli/rules/python/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.691387 precli-0.5.5/precli/rules/python/stdlib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/argparse_sensitive_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/assert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/crypt_weak_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/ftplib_cleartext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/ftplib_unverified_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4833 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/hashlib_improper_prng.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6955 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/hashlib_weak_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/hmac_timing_attack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6579 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/hmac_weak_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6812 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/hmac_weak_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/http_server_unrestricted_bind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/http_url_secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/imaplib_cleartext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/imaplib_unverified_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/json_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/logging_insecure_listen_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/marshal_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/nntplib_cleartext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/nntplib_unverified_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/pickle_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/poplib_cleartext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/poplib_unverified_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/re_denial_of_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/secrets_weak_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/shelve_open.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/smtplib_cleartext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/smtplib_unverified_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/socket_unrestricted_bind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/socketserver_unrestricted_bind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/ssl_context_weak_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/ssl_create_unverified_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6514 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/ssl_insecure_tls_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/telnetlib_cleartext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6124 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/tempfile_mktemp_race_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/xmlrpc_server_unrestricted_bind.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.779386 precli-0.5.5/precli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-28 20:46:17.000000 precli-0.5.5/precli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    39522 2024-05-28 20:46:17.000000 precli-0.5.5/precli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 20:46:17.000000 precli-0.5.5/precli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-28 20:46:17.000000 precli-0.5.5/precli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 20:46:17.000000 precli-0.5.5/precli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-28 20:46:17.000000 precli-0.5.5/precli.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-28 20:46:17.000000 precli-0.5.5/precli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-28 20:46:17.000000 precli-0.5.5/precli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-28 20:46:14.000000 precli-0.5.5/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-28 20:46:14.000000 precli-0.5.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4389 2024-05-28 20:46:17.779386 precli-0.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-28 20:46:14.000000 precli-0.5.5/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-28 20:46:14.000000 precli-0.5.5/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.691387 precli-0.5.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.691387 precli-0.5.5/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.691387 precli-0.5.5/tests/unit/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.695387 precli-0.5.5/tests/unit/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/core/test_python.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.695387 precli-0.5.5/tests/unit/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.699386 precli-0.5.5/tests/unit/parsers/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/parsers/examples/bad_coding.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/parsers/examples/expression_list_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/parsers/examples/expression_list_assignment_uneven.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/parsers/examples/importlib_import_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/parsers/examples/pep3120.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/parsers/examples/suppress.go
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/parsers/examples/suppress.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/parsers/examples/suppress_lowercase_rule.go
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/parsers/examples/suppress_lowercase_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/parsers/examples/suppress_multiline.go
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/parsers/examples/suppress_multiline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/parsers/examples/suppress_multiple_comments.go
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/parsers/examples/suppress_multiple_comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/parsers/examples/suppress_multiple_rules.go
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/parsers/examples/suppress_multiple_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/parsers/examples/suppress_preceding.go
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/parsers/examples/suppress_preceding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/parsers/examples/suppress_spaced_rules.go
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/parsers/examples/suppress_spaced_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/parsers/examples/suppress_wrong_rule.go
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/parsers/examples/suppress_wrong_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/parsers/test_go.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6012 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/parsers/test_python.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.699386 precli-0.5.5/tests/unit/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.699386 precli-0.5.5/tests/unit/rules/go/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/go/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.699386 precli-0.5.5/tests/unit/rules/go/stdlib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/go/stdlib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.699386 precli-0.5.5/tests/unit/rules/go/stdlib/crypto/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/go/stdlib/crypto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.703386 precli-0.5.5/tests/unit/rules/go/stdlib/crypto/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_cipher_aes.go
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_cipher_des.go
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_cipher_rc4.go
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_hash_md5_new.go
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_hash_md5_sum.go
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_hash_sha1_new.go
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_hash_sha1_sum.go
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_hash_sha256_new.go
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_hash_sha256_sum.go
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_dsa_1024.go
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_dsa_2048.go
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_dsa_3072.go
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_1024.go
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_2048.go
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_4096.go
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_bits_as_var.go
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/go/stdlib/crypto/test_crypto_weak_cipher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/go/stdlib/crypto/test_crypto_weak_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/go/stdlib/crypto/test_crypto_weak_key.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.703386 precli-0.5.5/tests/unit/rules/java/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.703386 precli-0.5.5/tests/unit/rules/java/stdlib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.703386 precli-0.5.5/tests/unit/rules/java/stdlib/java_net/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/java_net/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.703386 precli-0.5.5/tests/unit/rules/java/stdlib/java_net/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/java_net/examples/HttpCookieSecureFalse.java
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/java_net/examples/HttpCookieSecureTrue.java
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/java_net/test_insecure_cookie.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.703386 precli-0.5.5/tests/unit/rules/java/stdlib/java_security/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/java_security/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.707387 precli-0.5.5/tests/unit/rules/java/stdlib/java_security/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/java_security/examples/JavaSecuritySecureRandomSHA1PRNG.java
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/java_security/examples/KeyPairGeneratorDSA.java
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/java_security/examples/KeyPairGeneratorRSA.java
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/java_security/examples/MessageDigestMD2.java
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/java_security/examples/MessageDigestMD5.java
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/java_security/examples/MessageDigestMD5Property.java
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/java_security/examples/MessageDigestSHA1.java
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/java_security/examples/MessageDigestSHA256.java
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/java_security/examples/SecureRandomDefault.java
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/java_security/examples/SecureRandomSHA1PRNG.java
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/java_security/test_weak_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/java_security/test_weak_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/java_security/test_weak_random.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.707387 precli-0.5.5/tests/unit/rules/java/stdlib/javax_crypto/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/javax_crypto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.707387 precli-0.5.5/tests/unit/rules/java/stdlib/javax_crypto/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/javax_crypto/examples/Cipher3DESCBC.java
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherAESCBC.java
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherArcfour.java
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherBlowfishCBC.java
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherDESCBC.java
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherRC2.java
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherRC4.java
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherRC5.java
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/javax_crypto/test_weak_cipher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.707387 precli-0.5.5/tests/unit/rules/java/stdlib/javax_servlet_http/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/javax_servlet_http/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.707387 precli-0.5.5/tests/unit/rules/java/stdlib/javax_servlet_http/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/javax_servlet_http/examples/CookieSecureFalse.java
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/javax_servlet_http/examples/CookieSecureTrue.java
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/javax_servlet_http/test_insecure_cookie.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.707387 precli-0.5.5/tests/unit/rules/python/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.707387 precli-0.5.5/tests/unit/rules/python/stdlib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.707387 precli-0.5.5/tests/unit/rules/python/stdlib/argparse/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/argparse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.711387 precli-0.5.5/tests/unit/rules/python/stdlib/argparse/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/argparse/examples/argparse_add_argument_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/argparse/examples/argparse_add_argument_default_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/argparse/examples/argparse_add_argument_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/argparse/examples/argparse_add_argument_password_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/argparse/examples/argparse_add_argument_password_store_true.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/argparse/test_argparse_sensitive_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.711387 precli-0.5.5/tests/unit/rules/python/stdlib/assert/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/assert/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.711387 precli-0.5.5/tests/unit/rules/python/stdlib/assert/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/assert/examples/assert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/assert/test_assert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.711387 precli-0.5.5/tests/unit/rules/python/stdlib/crypt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/crypt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.711387 precli-0.5.5/tests/unit/rules/python/stdlib/crypt/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/crypt/examples/crypt_crypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/crypt/examples/crypt_crypt_method_blowfish.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/crypt/examples/crypt_crypt_method_crypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/crypt/examples/crypt_crypt_method_md5.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/crypt/examples/crypt_crypt_method_sha256.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/crypt/examples/crypt_crypt_method_sha512.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/crypt/examples/crypt_mksalt.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/crypt/examples/crypt_mksalt_method_blowfish.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/crypt/examples/crypt_mksalt_method_crypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/crypt/examples/crypt_mksalt_method_md5.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/crypt/examples/crypt_mksalt_method_sha256.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/crypt/examples/crypt_mksalt_method_sha512.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/crypt/test_crypt_weak_hash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.715386 precli-0.5.5/tests/unit/rules/python/stdlib/ftplib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ftplib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.715386 precli-0.5.5/tests/unit/rules/python/stdlib/ftplib/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ftplib/examples/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ftplib/examples/ftp_context_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ftplib/examples/ftp_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ftplib/examples/ftp_tls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_context_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_login_single_statement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_tls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_tls_context_as_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_tls_context_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_tls_context_unset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_tls_user_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_user_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ftplib/test_ftplib_cleartext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ftplib/test_ftplib_unverified_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.715386 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.727387 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_blake2b.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_blake2s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_improper_prng_blake2b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_improper_prng_blake2s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_improper_prng_pbkdf2_hmac.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_improper_prng_scrypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_md4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_md5.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_md5_as_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_md5_importlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_md5_usedforsecurity_true.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_blake2b.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_blake2s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_md4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_md5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_md5_sha1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_md5_usedforsecurity_true.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_name_sha.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_ripemd160.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha1.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha224.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha256.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha384.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha3_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha3_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha3_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha3_512.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha512.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha_usedforsecurity_false.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_shake_128.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_shake_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_md4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_md5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_ripemd160.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha3_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha3_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha3_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha3_512.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_shake_128.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_shake_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_ripemd160.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha1.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha224.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha256.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha384.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha3_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha3_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha3_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha3_512.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha512.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha_usedforsecurity_false.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_shake_128.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_shake_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/test_hashlib_improper_prng.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/test_hashlib_weak_hash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.727387 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.743386 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_blake2b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_blake2s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_blake2b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_blake2s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_md4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_md5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_ripemd160.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha3_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha3_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha3_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha3_512.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha512.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_shake_128.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_shake_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_md4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_md5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_md5_sha1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_ripemd160.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha3_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha3_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha3_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha3_512.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha512.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_shake_128.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_shake_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_weak_key_hashlib_blake2b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_weak_key_hashlib_sha3_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_weak_key_hashlib_sm3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_weak_key_sha224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_weak_key_sha256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_weak_key_sha512.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_blake2b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_blake2s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_blake2b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_blake2s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_md4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_md5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_ripemd160.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha3_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha3_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha3_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha3_512.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha512.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_shake_128.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_shake_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_md4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_md5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_md5_sha1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_ripemd160.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha3_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha3_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha3_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha3_512.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha512.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_shake_128.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_shake_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_weak_key_blake2s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_weak_key_hashlib_sha3_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_weak_key_hashlib_sha3_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_weak_key_hashlib_sha3_512.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_weak_key_sha384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_weak_key_sha512_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_timing_attack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_timing_attack_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_timing_attack_class_hexdigest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_timing_attack_compare_digest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/test_hmac_timing_attack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/test_hmac_weak_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/test_hmac_weak_key.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.747386 precli-0.5.5/tests/unit/rules/python/stdlib/http/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/http/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.747386 precli-0.5.5/tests/unit/rules/python/stdlib/http/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/http/examples/http_server_http_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/http/examples/http_server_threading_http_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/http/examples/http_url_secret_apikey.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/http/examples/http_url_secret_apikey_in_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/http/examples/http_url_secret_basic_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/http/examples/http_url_secret_basic_auth_as_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/http/examples/http_url_secret_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/http/examples/http_url_secret_username.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/http/test_http_server_unrestricted_bind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/http/test_http_url_secret.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.747386 precli-0.5.5/tests/unit/rules/python/stdlib/imaplib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/imaplib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.751387 precli-0.5.5/tests/unit/rules/python/stdlib/imaplib/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_authenticate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_context_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_login_cram_md5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_ssl_context_as_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_ssl_context_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_ssl_context_unset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_starttls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_starttls_context_as_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_starttls_context_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_starttls_context_unset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/imaplib/test_imaplib_cleartext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/imaplib/test_imaplib_unverified_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.751387 precli-0.5.5/tests/unit/rules/python/stdlib/json/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/json/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.751387 precli-0.5.5/tests/unit/rules/python/stdlib/json/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/json/examples/json_jsondecoder_decode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/json/examples/json_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/json/examples/json_loads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/json/test_json_load.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.751387 precli-0.5.5/tests/unit/rules/python/stdlib/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/logging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.751387 precli-0.5.5/tests/unit/rules/python/stdlib/logging/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/logging/examples/insecure_listen_config_empty_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/logging/examples/insecure_listen_config_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/logging/examples/insecure_listen_config_port_verify_as_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/logging/examples/insecure_listen_config_port_verify_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/logging/examples/insecure_listen_config_verify_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/logging/examples/insecure_listen_config_verify_none_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/logging/examples/insecure_listen_config_verify_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/logging/test_logging_insecure_listen_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.751387 precli-0.5.5/tests/unit/rules/python/stdlib/marshal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/marshal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.751387 precli-0.5.5/tests/unit/rules/python/stdlib/marshal/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/marshal/examples/marshal_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/marshal/examples/marshal_loads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/marshal/test_marshal_load.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.755386 precli-0.5.5/tests/unit/rules/python/stdlib/nntplib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/nntplib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.755386 precli-0.5.5/tests/unit/rules/python/stdlib/nntplib/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_context_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_ssl_context_as_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_ssl_context_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_ssl_context_unset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_starttls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_starttls_context_as_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_starttls_context_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_starttls_context_unset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/nntplib/test_nntplib_cleartext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/nntplib/test_nntplib_unverified_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.755386 precli-0.5.5/tests/unit/rules/python/stdlib/pickle/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/pickle/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.755386 precli-0.5.5/tests/unit/rules/python/stdlib/pickle/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/pickle/examples/pickle_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/pickle/examples/pickle_loads.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/pickle/examples/pickle_unpickler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/pickle/test_pickle_load.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.755386 precli-0.5.5/tests/unit/rules/python/stdlib/poplib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/poplib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.759386 precli-0.5.5/tests/unit/rules/python/stdlib/poplib/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_apop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_context_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_pass_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_rpop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_ssl_context_as_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_ssl_context_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_ssl_context_unset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_stls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_stls_context_as_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_stls_context_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_stls_context_unset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/poplib/test_poplib_cleartext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/poplib/test_poplib_unverified_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.759386 precli-0.5.5/tests/unit/rules/python/stdlib/re/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/re/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.763386 precli-0.5.5/tests/unit/rules/python/stdlib/re/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/re/examples/re_compile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/re/examples/re_compile_good.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/re/examples/re_findall.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/re/examples/re_finditer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/re/examples/re_fullmatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/re/examples/re_match.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/re/examples/re_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/re/examples/re_search_good.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/re/examples/re_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/re/examples/re_sub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/re/examples/re_subn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/re/test_re_denial_of_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.763386 precli-0.5.5/tests/unit/rules/python/stdlib/secrets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/secrets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.763386 precli-0.5.5/tests/unit/rules/python/stdlib/secrets/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/secrets/examples/secrets_token_bytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/secrets/examples/secrets_token_bytes_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/secrets/examples/secrets_token_bytes_size_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/secrets/examples/secrets_token_hex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/secrets/examples/secrets_token_hex_nbytes_unknown.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/secrets/examples/secrets_token_urlsafe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/secrets/test_secrets_weak_token.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.763386 precli-0.5.5/tests/unit/rules/python/stdlib/shelve/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/shelve/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.763386 precli-0.5.5/tests/unit/rules/python/stdlib/shelve/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/shelve/examples/shelve_dbfilenameshelf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/shelve/examples/shelve_open.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/shelve/examples/shelve_open_context_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/shelve/test_shelve_open.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.763386 precli-0.5.5/tests/unit/rules/python/stdlib/smtplib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/smtplib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.767386 precli-0.5.5/tests/unit/rules/python/stdlib/smtplib/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_context_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl_context_as_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl_context_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl_context_unset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls_context_as_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls_context_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls_context_unset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/smtplib/test_smtplib_cleartext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/smtplib/test_smtplib_unverified_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.767386 precli-0.5.5/tests/unit/rules/python/stdlib/socket/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/socket/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.767386 precli-0.5.5/tests/unit/rules/python/stdlib/socket/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/socket/examples/socket_create_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/socket/examples/socket_socket_bind.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/socket/examples/socket_socket_bind_as_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/socket/examples/socket_socket_bind_as_vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/socket/test_socket_unrestricted_bind.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.767386 precli-0.5.5/tests/unit/rules/python/stdlib/socketserver/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/socketserver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.767386 precli-0.5.5/tests/unit/rules/python/stdlib/socketserver/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_forking_tcp_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_forking_udp_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_tcp_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_threading_tcp_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_threading_udp_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_udp_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/socketserver/test_socketserver_unrestricted_bind.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.771386 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.775386 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/create_default_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/create_unverified_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/get_server_certificate_sslv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/get_server_certificate_sslv23.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/get_server_certificate_sslv3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/get_server_certificate_tlsv1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/get_server_certificate_tlsv11.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/get_server_certificate_tlsv12.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_brainpoolP256r1.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_brainpoolP384r1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_brainpoolP384r1tls13.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_brainpoolP512r1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_default_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_ffdhe2048.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_prime192v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_prime256v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_secp160r2.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_secp256r1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_sect163k1.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_sect571k1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_typed_default_param.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_typed_param.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_unverified_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_sslv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_sslv23.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_sslv3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_tlsv1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_tlsv11.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_tlsv12.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/wrap_socket_sslv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/wrap_socket_sslv23.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/wrap_socket_sslv2_server_side_true.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/wrap_socket_sslv3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/wrap_socket_tlsv1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/wrap_socket_tlsv11.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/wrap_socket_tlsv12.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/test_ssl_context_tls_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/test_ssl_context_weak_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/test_ssl_create_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/test_ssl_get_server_certificate_tls_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/test_ssl_wrap_socket_tls_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.775386 precli-0.5.5/tests/unit/rules/python/stdlib/telnetlib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/telnetlib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.779386 precli-0.5.5/tests/unit/rules/python/stdlib/telnetlib/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/telnetlib/examples/telnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/telnetlib/examples/telnetlib_telnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/telnetlib/examples/telnetlib_telnet_context_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/telnetlib/test_telnetlib_cleartext.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.779386 precli-0.5.5/tests/unit/rules/python/stdlib/tempfile/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/tempfile/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.779386 precli-0.5.5/tests/unit/rules/python/stdlib/tempfile/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/tempfile/examples/tempfile_mktemp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/tempfile/examples/tempfile_mktemp_args_open.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/tempfile/examples/tempfile_mktemp_args_with_open_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/tempfile/examples/tempfile_mktemp_open.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/tempfile/examples/tempfile_mktemp_walrus_open.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/tempfile/examples/tempfile_mktemp_with_open.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/tempfile/examples/tempfile_mktemp_with_open_multiline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/tempfile/test_tempfile_mktemp_race_condition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.779386 precli-0.5.5/tests/unit/rules/python/stdlib/xmlrpc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/xmlrpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.779386 precli-0.5.5/tests/unit/rules/python/stdlib/xmlrpc/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/xmlrpc/examples/xmlrpc_server_doc_xml_rpc_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/xmlrpc/examples/xmlrpc_server_simple_xml_rpc_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/xmlrpc/test_xmlrpc_server_unrestricted_bind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/test_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-28 20:46:14.000000 precli-0.5.5/tox.ini
```

### Comparing `precli-0.5.4/.github/workflows/dependency-review.yml` & `precli-0.5.5/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `precli-0.5.4/.github/workflows/publish-to-pypi.yml` & `precli-0.5.5/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `precli-0.5.4/.github/workflows/publish-to-test-pypi.yml` & `precli-0.5.5/.github/workflows/publish-to-test-pypi.yml`

 * *Files identical despite different names*

### Comparing `precli-0.5.4/.github/workflows/unit-test.yml` & `precli-0.5.5/.github/workflows/unit-test.yml`

 * *Files identical despite different names*

### Comparing `precli-0.5.4/.github/workflows/upload-asset.yml` & `precli-0.5.5/.github/workflows/upload-asset.yml`

 * *Files 14% similar despite different names*

```diff
@@ -37,10 +37,10 @@
       if: startsWith(github.ref, 'refs/tags/')
       with:
         files: |
           dist/*.whl
           dist/*.tar.gz
 
     - name: Attest Build Provenance
-      uses: actions/attest-build-provenance@897ed5eab6ed058a474202017ada7f40bfa52940
+      uses: actions/attest-build-provenance@173725a1209d09b31f9d30a3890cf2757ebbff0d
       with:
         subject-path: 'dist/precli-*'
```

### Comparing `precli-0.5.4/.pre-commit-config.yaml` & `precli-0.5.5/.pre-commit-config.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-exclude: ^(examples|tools|docs)
+exclude: ^(docs|tests)
 repos:
 - repo: https://github.com/pre-commit/pre-commit-hooks
   rev: v4.4.0
   hooks:
   - id: check-yaml
   - id: debug-statements
   - id: end-of-file-fixer
```

### Comparing `precli-0.5.4/CODE_OF_CONDUCT.md` & `precli-0.5.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `precli-0.5.4/ChangeLog` & `precli-0.5.5/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,42 @@
 CHANGES
 =======
 
+0.5.5
+-----
+
+* Fix for traceback in plain renderer (#494)
+* Filter the list of artifacts during discovery (#491)
+* Nit: Rearrange args to partial (#490)
+* Delay reading of file contents until parser decided (#489)
+* Redo handling of keyboard interrupts (#488)
+* Suppress FutureWarnings from tree-sitter and re modules (#487)
+* Avoid init of parsers twice (#486)
+* Support multiprocessing of file parsing (#485)
+* Bump requests from 2.32.1 to 2.32.2 (#484)
+* Refactor the invoke function in the run class (#483)
+* Nicer output using rich.console (#482)
+* Handle invalid coding for a Python file (#481)
+* Correctly handle a non unicode file without pep3120 (#479)
+* Fix unknown value for nbytes (#478)
+* Handle non-UTF-8 encoding files (#477)
+* Remove some docstring comments on return and params (#476)
+* Use f-string instead of string substitution (#475)
+* Fix typo in copyright (#469)
+* Bump requests from 2.31.0 to 2.32.1 (#467)
+* Delete .stestr.conf (#465)
+* Migrate from stestr to pytests (#464)
+* Bump actions/attest-build-provenance from 1.1.1 to 1.1.2 (#462)
+* Bump actions/attest-build-provenance from 1.1.0 to 1.1.1 (#460)
+* Add defaultConfiguration in SARIF output (#459)
+* Load metadata for any extension entry points (#458)
+* Remove the unnecessary scripts directory and contents (#457)
+* Bump actions/attest-build-provenance from 1.0.0 to 1.1.0 (#456)
+* Bump pygments from 2.17.2 to 2.18.0 (#454)
+
 0.5.4
 -----
 
 * Fix action failure to release binary (#453)
 
 0.5.3
 -----
```

### Comparing `precli-0.5.4/LICENSE` & `precli-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `precli-0.5.4/PKG-INFO` & `precli-0.5.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: precli
-Version: 0.5.4
+Version: 0.5.5
 Summary: Static analysis security tool command line
 Home-page: https://github.com/securesauce/precli
 Download-URL: https://pypi.org/project/precli/#files
 Author: Secure Sauce
 Project-URL: Release notes, https://github.com/securesauce/precli/releases
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -16,20 +16,20 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Security
 Requires-Python: >=3.12
 License-File: LICENSE
 Requires-Dist: cwe2==2.0.0
-Requires-Dist: Pygments==2.17.2
+Requires-Dist: Pygments==2.18.0
 Requires-Dist: rich==13.7.1
 Requires-Dist: tree-sitter==0.21.3
 Requires-Dist: tree-sitter-languages==1.10.2
 Requires-Dist: ignorelib==0.3.0
-Requires-Dist: requests==2.31.0
+Requires-Dist: requests==2.32.2
 Requires-Dist: sarif-om==1.0.4
 Requires-Dist: jschema-to-python==1.2.3
 Requires-Dist: outdated==0.2.2
 
 .. image:: https://raw.githubusercontent.com/securesauce/precli/main/logo/logo.png
     :alt: Precaution CLI
```

### Comparing `precli-0.5.4/README.rst` & `precli-0.5.5/README.rst`

 * *Files identical despite different names*

### Comparing `precli-0.5.4/SECURITY.md` & `precli-0.5.5/SECURITY.md`

 * *Files identical despite different names*

### Comparing `precli-0.5.4/docs/getting-started.md` & `precli-0.5.5/docs/getting-started.md`

 * *Files identical despite different names*

### Comparing `precli-0.5.4/docs/man/precli.rst` & `precli-0.5.5/docs/man/precli.rst`

 * *Files identical despite different names*

### Comparing `precli-0.5.4/docs/rules.md` & `precli-0.5.5/docs/rules.md`

 * *Files identical despite different names*

### Comparing `precli-0.5.4/logo/logo.png` & `precli-0.5.5/logo/logo.png`

 * *Files identical despite different names*

### Comparing `precli-0.5.4/precli/cli/main.py` & `precli-0.5.5/precli/cli/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 import argparse
 import logging
 import os
+import pathlib
 import sys
 import tempfile
 import zipfile
 from importlib import metadata
 from urllib.parse import urljoin
 from urllib.parse import urlparse
 
 import requests
 from ignorelib import IgnoreFilterManager
 from outdated import check_outdated
 from rich import progress
+from rich.console import Console
 
 import precli
-from precli.core import loader
 from precli.core.artifact import Artifact
 from precli.core.run import Run
 from precli.core.tool import Tool
 from precli.renderers.detailed import Detailed
 from precli.renderers.json import Json
 from precli.renderers.markdown import Markdown
 from precli.renderers.plain import Plain
@@ -124,15 +125,15 @@
             extensions += f"  {dist.name} {dist.version}\n"
     python_ver = sys.version.replace("\n", "")
     parser.add_argument(
         "--version",
         action="version",
         version=f"precli {precli.__version__}\n"
         f"{extensions}"
-        f"Copyright 2024 Secure Saurce LLC\n"
+        f"Copyright 2024 Secure Sauce LLC\n"
         f"License BUSL-1.1: Business Source License 1.1 <{BUSL_URL}>\n"
         f"  Python {python_ver}",
     )
     args = parser.parse_args()
 
     if not args.targets:
         parser.print_usage()
@@ -200,14 +201,15 @@
     prefix = root[target_len:].lstrip("/")
     urlpath = f"{owner}/{repo}/blob/{branch}"
     rel_path = "/".join([urlpath, prefix, file])
     return urljoin(GITHUB_URL, rel_path)
 
 
 def discover_files(targets: list[str], recursive: bool):
+    FILE_EXTS = (".go", ".java", ".py", ".pyw")
     artifacts = []
 
     for target in targets:
         if target.startswith(GITHUB_URL):
             owner, repo = get_owner_repo(target)
             if repo:
                 try:
@@ -241,33 +243,40 @@
 
             if recursive is True:
                 for root, _, files in gitignore_mgr.walk():
                     for file in files:
                         path = os.path.join(root, file)
                         file_path = file if os.path.isabs(path) else path
 
-                        if not preignore_mgr.is_ignored(file_path):
+                        if (
+                            not preignore_mgr.is_ignored(file_path)
+                            and pathlib.Path(path).suffix in FILE_EXTS
+                        ):
                             artifact = Artifact(path)
                             if repo:
                                 artifact.uri = file_to_url(
                                     owner, repo, branch, target, root, file
                                 )
                             artifacts.append(artifact)
             else:
                 files = os.listdir(path=target)
                 for file in files:
-                    if not (
-                        gitignore_mgr.is_ignored(file)
-                        or preignore_mgr.is_ignored(file)
+                    if (
+                        not (
+                            gitignore_mgr.is_ignored(file)
+                            or preignore_mgr.is_ignored(file)
+                        )
+                        and pathlib.Path(file).suffix in FILE_EXTS
                     ):
                         artifact = Artifact(os.path.join(target, file))
                         artifacts.append(artifact)
         else:
-            artifact = Artifact(target)
-            artifacts.append(artifact)
+            if pathlib.Path(target).suffix in FILE_EXTS:
+                artifact = Artifact(target)
+                artifacts.append(artifact)
 
     return artifacts
 
 
 def create_gist(file, renderer: str):
     match renderer:
         case "json":
@@ -319,61 +328,63 @@
     git_target = any(filter(lambda x: x.startswith(GITHUB_URL), args.targets))
 
     if (git_target or args.gist) and not args.quiet:
         check_for_update()
 
     enabled = args.enable.split(",") if args.enable else []
     disabled = args.disable.split(",") if args.disable else []
-    parsers = loader.load_parsers(enabled, disabled)
 
     # Compile a list of the targets
     artifacts = discover_files(args.targets, args.recursive)
 
-    # Flatten into a list all rules for all parsers
-    rules = [r for parser in parsers.values() for r in parser.rules.values()]
+    if args.gist is True:
+        file = tempfile.NamedTemporaryFile(mode="w+t")
+    else:
+        file = args.output if args.output else sys.stdout
+
+    console = Console(
+        file=file,
+        no_color=True if file.name != sys.stdout.name else False,
+        highlight=False,
+    )
 
     # Initialize the run
     tool = Tool(
         name="Precaution",
         download_uri=precli.__download_url__,
         full_description=precli.__summary__,
         information_uri=precli.__url__,
         organization=precli.__author__,
         short_description=precli.__summary__,
         version=precli.__version__,
-        rules=rules,
     )
-    run = Run(tool, parsers, artifacts, debug)
+    run = Run(tool, enabled, disabled, artifacts, console, debug)
 
     # Invoke the run
     run.invoke()
 
-    file = args.output
-    if args.gist is True:
-        file = tempfile.NamedTemporaryFile(mode="w+t")
-
     if args.json is True:
         renderer = "json"
-        json = Json(file=file, no_color=args.no_color)
+        json = Json(console)
         json.render(run)
     elif args.plain is True:
         renderer = "plain"
-        plain = Plain(file=file, no_color=args.no_color)
+        plain = Plain(console)
         plain.render(run)
     elif args.markdown is True:
         renderer = "markdown"
-        markdown = Markdown(file=file, no_color=args.no_color)
+        markdown = Markdown(console)
         markdown.render(run)
     else:
         renderer = "detailed"
-        detailed = Detailed(file=file, no_color=args.no_color)
+        detailed = Detailed(console)
         detailed.render(run)
 
     if file.name != sys.stdout.name:
-        print(f"Output written to file: {file.name}")
+        console.print(f"Output written to file: {file.name}")
 
     if args.gist is True:
         create_gist(file, renderer)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `precli-0.5.4/precli/core/argument.py` & `precli-0.5.5/precli/core/argument.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 from tree_sitter import Node
 
 from precli.core import utils
 from precli.parsers import tokens
 
 
 class Argument:
@@ -31,84 +31,55 @@
         if node.type in [tokens.ATTRIBUTE, tokens.SELECTOR_EXPRESSION]:
             return Argument._get_func_ident(node.named_children[1])
         if node.type in [tokens.IDENTIFIER, tokens.FIELD_IDENTIFIER]:
             return node
 
     @property
     def node(self) -> Node:
-        """
-        The node representing this argument.
-
-        :return: node for the argument
-        :rtype: Node
-        """
+        """The node representing this argument."""
         return self._node
 
     @property
     def identifier_node(self) -> Node:
         """
         The node representing just the identifier of the argument.
 
         For example, if the function is:
             a.b.c()
         The identifier node would be c
-
-        :return: identifier of the argument
-        :rtype: Node
         """
         return self._ident_node
 
     @property
     def name(self) -> str:
         """
         The name of the keyword argument.
 
         If this argument is a keyword argument, then name is the
         name component of the name-value pair.
-
-        :return: name of keyword arg
-        :rtype: str
         """
         return self._name
 
     @property
     def position(self) -> int:
         """
         The position of the argument in the arg list.
 
         If this argument is a positional, then position references
         the index in the arg list of the argument.
-
-        :return: index in arg list
-        :rtype: int
         """
         return self._position
 
     @property
     def is_str(self) -> bool:
-        """
-        True if the value is a true string.
-
-        :return: if value is a string
-        :rtype: bool
-        """
+        """True if the value is a true string."""
         return self._is_str
 
     @property
     def value(self):
-        """
-        The value of the argument.
-
-        :return: value of argument
-        :rtype: object
-        """
+        """The value of the argument."""
         return self._value
 
     @property
     def value_str(self) -> str:
-        """
-        The value as a true string.
-
-        :return: value as string
-        :rtype: str
-        """
+        """The value as a true string."""
         return self._value_str
```

### Comparing `precli-0.5.4/precli/core/artifact.py` & `precli-0.5.5/precli/core/artifact.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,86 +1,61 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 
 
 class Artifact:
     def __init__(self, file_name: str, uri: str = None):
         self._file_name = file_name
         # TODO: if uri is None, use file:///
         self._uri = uri
         self._contents = None
+        self._encoding = "utf-8"
         self._language = None
 
     @property
     def file_name(self) -> str:
-        """
-        The name of the file.
-
-        :return: file name
-        :rtype: str
-        """
+        """The name of the file."""
         return self._file_name
 
     @file_name.setter
     def file_name(self, file_name):
-        """
-        Set the file name
-
-        :param str file_name: file name
-        """
+        """Set the file name"""
         self._file_name = file_name
 
     @property
     def uri(self) -> str:
-        """
-        The URI of the artifact.
-
-        :return: URI
-        :rtype: str
-        """
+        """The URI of the artifact."""
         return self._uri
 
     @uri.setter
     def uri(self, uri):
-        """
-        Set the artifact URI.
-
-        :param str uri: URI
-        """
+        """Set the artifact URI."""
         self._uri = uri
 
     @property
-    def contents(self) -> str:
-        """
-        The contents of the artifact.
+    def encoding(self) -> str:
+        """The encoding of the file."""
+        return self._encoding
+
+    @encoding.setter
+    def encoding(self, encoding) -> str:
+        """Set the encoding of the file."""
+        self._encoding = encoding
 
-        :return: typically file contents
-        :rtype: str
-        """
+    @property
+    def contents(self) -> str:
+        """The contents of the artifact."""
         return self._contents
 
     @contents.setter
     def contents(self, contents) -> str:
-        """
-        Set the contents (for typically the file).
-
-        :param str contents: file contents
-        """
+        """Set the contents (for typically the file)."""
         self._contents = contents
 
     @property
     def language(self) -> str:
-        """
-        The programming language for this artifact.
-
-        :return: programming language name
-        :rtype: str
-        """
+        """The programming language for this artifact."""
         return self._language
 
     @language.setter
     def language(self, language) -> str:
-        """
-        Set the programming language.
-
-        :param str language: program language
-        """
+        """Set the programming language."""
         self._language = language
```

### Comparing `precli-0.5.4/precli/core/call.py` & `precli-0.5.5/precli/core/call.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 from tree_sitter import Node
 
 from precli.core.argument import Argument
 from precli.parsers import tokens
 
 
 class Call:
@@ -26,82 +26,58 @@
         self._ident_node = ident_node
         self._arg_list_node = arg_list_node
         self._args = args if args is not None else []
         self._kwargs = kwargs if kwargs is not None else {}
 
     @property
     def node(self) -> Node:
-        """
-        The node representing this call.
-
-        :return: node for the call
-        :rtype: Node
-        """
+        """The node representing this call."""
         return self._node
 
     @property
     def var_node(self) -> Node:
         """
         The node representing the variable part of a function call.
 
         For example, if the function call is:
             a.b.c()
         The function node would be a.b
-
-        :return: function for the call
-        :rtype: Node
         """
         return self._var_node
 
     @property
     def function_node(self) -> Node:
         """
         The node representing the entire function of the call.
 
         For example, if the function call is:
             a.b.c()
         The function node would be a.b.c
-
-        :return: function for the call
-        :rtype: Node
         """
         return self._func_node
 
     @property
     def identifier_node(self) -> Node:
         """
         The node representing just the identifier of the function.
 
         For example, if the function call is:
             a.b.c()
         The identifier node would be c
-
-        :return: identifier of the function
-        :rtype: Node
         """
         return self._ident_node
 
     @property
     def name(self) -> str:
-        """
-        The name of the function call.
-
-        :return: name of function
-        :rtype: str
-        """
+        """The name of the function call."""
         return self._name
 
     @property
     def name_qualified(self) -> str:
-        """
-        The fully qualified name of the function.
-
-        :return: fully qualified name of function
-        :rtype: str
-        """
+        """The fully qualified name of the function."""
         return self._name_qual
 
     @property
     def arg_list_node(self) -> Node:
         return self._arg_list_node
 
     def get_argument(
```

### Comparing `precli-0.5.4/precli/core/comparison.py` & `precli-0.5.5/precli/core/comparison.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 from tree_sitter import Node
 
 
 class Comparison:
     def __init__(
         self,
         node: Node,
@@ -16,74 +16,39 @@
         self._right_hand = right_hand
         self._left_node = node.children[0]
         self._operator_node = node.children[1]
         self._right_node = node.children[2]
 
     @property
     def node(self) -> Node:
-        """
-        The node representing this comparison.
-
-        :return: node for the comparison
-        :rtype: Node
-        """
+        """The node representing this comparison."""
         return self._node
 
     @property
     def left_node(self) -> Node:
-        """
-        The left node of the comparison.
-
-        :return: left node of comparison
-        :rtype: Node
-        """
+        """The left node of the comparison."""
         return self._left_node
 
     @property
     def operator_node(self) -> Node:
-        """
-        The operator node of this comparison.
-
-        :return: operator node of comparison
-        :rtype: Node
-        """
+        """The operator node of this comparison."""
         return self._operator_node
 
     @property
     def right_node(self) -> Node:
-        """
-        The right node of the comparison.
-
-        :return: right node of comparison
-        :rtype: Node
-        """
+        """The right node of the comparison."""
         return self._right_node
 
     @property
     def left_hand(self) -> str:
-        """
-        The left hand side of the comparison.
-
-        :return: left part of comparison
-        :rtype: str
-        """
+        """The left hand side of the comparison."""
         return self._left_hand
 
     @property
     def operator(self) -> str:
-        """
-        The operator of this comparison.
-
-        :return: operator of comparison
-        :rtype: str
-        """
+        """The operator of this comparison."""
         return self._operator
 
     @property
     def right_hand(self) -> str:
-        """
-        The right hand side of the comparison.
-
-        :return: right part of comparison
-        :rtype: str
-        """
+        """The right hand side of the comparison."""
         return self._right_hand
```

### Comparing `precli-0.5.4/precli/core/config.py` & `precli-0.5.5/precli/core/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 from precli.core.level import Level
 
 
 class Config:
     def __init__(
         self,
         enabled: bool = True,
@@ -11,43 +11,24 @@
     ):
         self._enabled = enabled
         self._level = level
         self._rank = rank
 
     @property
     def enabled(self) -> bool:
-        """
-        Whether the configuration indicates the rule is enabled.
-
-        :return: true if rule enabled
-        :rtype: bool
-        """
+        """Whether the configuration indicates the rule is enabled."""
         return self._enabled
 
     @enabled.setter
     def enabled(self, enabled):
-        """
-        Set whether the rule is enabled
-
-        :param bool enabled: True to enable
-        """
+        """Set whether the rule is enabled"""
         self._enabled = enabled
 
     @property
     def level(self) -> Level:
-        """
-        The default severity level.
-
-        :return: severity level
-        :rtype: Level
-        """
+        """The default severity level."""
         return self._level
 
     @property
     def rank(self) -> float:
-        """
-        The default rank for the rule.
-
-        :return: rank
-        :rtype: float
-        """
+        """The default rank for the rule."""
         return self._rank
```

### Comparing `precli-0.5.4/precli/core/fix.py` & `precli-0.5.5/precli/core/fix.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 Secure Saurce LLC
+# Copyright 2023 Secure Sauce LLC
 from precli.core.location import Location
 
 
 class Fix:
     def __init__(
         self,
         description: str,
@@ -11,34 +11,19 @@
     ):
         self._description = description
         self._deleted_location = deleted_location
         self._inserted_content = inserted_content
 
     @property
     def description(self) -> str:
-        """
-        Describes the proposed fix.
-
-        :return: fix description
-        :rtype: str
-        """
+        """Describes the proposed fix."""
         return self._description
 
     @property
     def deleted_location(self) -> Location:
-        """
-        Specifies the location to delete.
-
-        :return: location object indicating region to delete
-        :rtype: Location
-        """
+        """Specifies the location to delete."""
         return self._deleted_location
 
     @property
     def inserted_content(self) -> str:
-        """
-        Content to insert at location specified by deleted_location.
-
-        :return: content to insert
-        :rtype: str
-        """
+        """Content to insert at location specified by deleted_location."""
         return self._inserted_content
```

### Comparing `precli-0.5.4/precli/core/kind.py` & `precli-0.5.5/precli/core/kind.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 Secure Saurce LLC
+# Copyright 2023 Secure Sauce LLC
 import enum
 
 
 class Kind(str, enum.Enum):
     """
     The nature of the result.
```

### Comparing `precli-0.5.4/precli/core/level.py` & `precli-0.5.5/precli/core/level.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 Secure Saurce LLC
+# Copyright 2023 Secure Sauce LLC
 import enum
 
 
 class Level(str, enum.Enum):
     """
     The severity level of a result.
```

### Comparing `precli-0.5.4/precli/core/linecache.py` & `precli-0.5.5/precli/core/linecache.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 import linecache
 
 
 class LineCache:
     def __init__(self, file_name: str, file_contents: str):
         """
         Initialize the cache with the given file contents.
```

### Comparing `precli-0.5.4/precli/core/redos.py` & `precli-0.5.5/precli/core/redos.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 # Copyright 2019 Duo Security
 import collections
 import itertools
 import sys
 from re import _constants as constants
 from re import _parser as parser
```

### Comparing `precli-0.5.4/precli/core/result.py` & `precli-0.5.5/precli/core/result.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 from precli.core.artifact import Artifact
 from precli.core.fix import Fix
 from precli.core.kind import Kind
 from precli.core.level import Level
 from precli.core.linecache import LineCache
 from precli.core.location import Location
 from precli.core.suppression import Suppression
@@ -21,19 +21,20 @@
         fixes: list[Fix] = None,
         suppression: Suppression = None,
         snippet: str = None,
     ):
         self._rule_id = rule_id
         self._artifact = artifact
         self._kind = kind
-        default_config = Rule.get_by_id(self._rule_id).default_config
-        self._rank = default_config.rank
+        rule = Rule.get_by_id(self._rule_id)
+        default_config = rule.default_config if rule else None
+        self._rank = default_config.rank if default_config else -1.0
         if level:
             self._level = level
-        else:
+        elif default_config:
             self._level = default_config.level
         self._location = location
         if message:
             self._message = message
         else:
             self._message = Rule.get_by_id(self._rule_id).message
         self._fixes = fixes if fixes is not None else []
@@ -41,152 +42,107 @@
         if snippet is not None:
             self._snippet = snippet
         else:
             self._init_snippet(artifact)
 
     def _init_snippet(self, artifact: Artifact):
         if artifact is not None:
-            linecache = LineCache(
-                artifact.file_name,
-                artifact.contents.decode(),
-            )
             self._snippet = ""
-            for i in range(
-                self._location.start_line - 1, self._location.end_line + 2
-            ):
-                self._snippet += linecache.getline(i)
+            try:
+                linecache = LineCache(
+                    artifact.file_name,
+                    artifact.contents.decode(encoding=artifact.encoding),
+                )
+                for i in range(
+                    self._location.start_line - 1, self._location.end_line + 2
+                ):
+                    self._snippet += linecache.getline(i)
+            except UnicodeDecodeError:
+                pass
 
     @property
     def rule_id(self) -> str:
         """
         The ID of the rule.
 
         The IDs match ??XXX where ?? is language identifier and XXX is a
         unique number.
-
-        :return: rule ID
-        :rtype: str
         """
         return self._rule_id
 
     @property
     def artifact(self) -> Artifact:
-        """
-        Artifact, typically the file.
-
-        :return: the artifact
-        :rtype: Artifact
-        """
+        """Artifact, typically the file."""
         return self._artifact
 
     @artifact.setter
-    def artifact(self, artifact):
-        """
-        Set the file artifact.
-
-        :param Artifact artifact: file artifact
-        """
+    def artifact(self, artifact: Artifact):
+        """Set the file artifact."""
         self._artifact = artifact
         self._init_snippet(artifact)
 
     @property
     def location(self) -> Location:
         """
         The location of the issue.
 
         A location object indicates coordinates within a source file where
         the issue was found.
-
-        :return: location
-        :rtype: Location
         """
         return self._location
 
     @property
     def kind(self) -> Kind:
         """
         The nature of the result.
 
         Typically having a value of pass or fail to indicate the nature of
         the result.
-
-        :return: kind or nature of result
-        :rtype: Kind
         """
         return self._kind
 
     @property
     def level(self) -> Level:
         """
         The result severity level.
 
         If the result is being supporessed, then the level is set to NOTE.
-
-        :return: severity level
-        :rtype: Level
         """
         return self._level if self._suppression is None else Level.NOTE
 
     @property
     def message(self) -> str:
-        """
-        The result issue message.
-
-        :return: issue message
-        :rtype: str
-        """
+        """The result issue message."""
         if self._suppression is None:
             return self._message
         else:
             return "This issue is being suppressed via an inline comment."
 
     @property
     def rank(self) -> float:
         """
         The rank of the issue.
 
         The value defaults to the value from the default configuration of the
         rule.
-
-        :return: rank
-        :rtype: float
         """
         return self._rank
 
     @property
     def fixes(self) -> list[Fix]:
-        """
-        The suggested fixes for the issue.
-
-        :return: list of fixes
-        :rtype: list
-        """
+        """The suggested fixes for the issue."""
         return self._fixes if self._suppression is None else []
 
     @property
     def suppression(self) -> Suppression:
-        """
-        Possible suppressions of the result.
-
-        :return: suppression or None
-        :rtype: Suppression
-        """
+        """Possible suppressions of the result."""
         return self._suppression
 
     @suppression.setter
-    def suppression(self, suppression):
-        """
-        Set the suppression of this result
-
-        :param Suppression suppression: suppression
-        """
+    def suppression(self, suppression: Suppression):
+        """Set the suppression of this result"""
         self._suppression = suppression
 
     @property
     def snippet(self) -> str:
-        """
-        Snippet of context of the code.
-
-        :return: snippet of context
-        :rtype: str
-        """
+        """Snippet of context of the code."""
         return self._snippet
```

### Comparing `precli-0.5.4/precli/core/run.py` & `precli-0.5.5/precli/core/run.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,130 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 import datetime
 import io
 import logging
 import os
 import pathlib
 import sys
-import traceback
+from functools import partial
+from multiprocessing import Pool
 
 from pygments import lexers
-from rich import progress
+from rich.console import Console
+from rich.progress import Progress
 
+from precli.core import loader
 from precli.core.artifact import Artifact
 from precli.core.level import Level
+from precli.core.location import Location
 from precli.core.metrics import Metrics
 from precli.core.result import Result
 from precli.core.tool import Tool
+from precli.rules import Rule
 
 
 LOG = logging.getLogger(__name__)
 PROGRESS_THRESHOLD = 50
+parsers = loader.load_parsers()
+
+
+def parse_file(
+    artifact: Artifact, enabled: list[str], disabled: list[str]
+) -> list[Result]:
+    results = []
+    try:
+        if artifact.file_name == "-":
+            open_fd = os.fdopen(sys.stdin.fileno(), "rb", 0)
+            fdata = io.BytesIO(open_fd.read())
+            artifact.file_name = "<stdin>"
+            artifact.contents = fdata.read()
+            lxr = lexers.guess_lexer(artifact.contents)
+            artifact.language = lxr.aliases[0] if lxr.aliases else lxr.name
+            parser = parsers.get(artifact.language)
+        else:
+            file_extension = pathlib.Path(artifact.file_name).suffix
+            parser = next(
+                (
+                    p
+                    for p in parsers.values()
+                    if file_extension in p.file_extensions()
+                ),
+                None,
+            )
+
+        if parser:
+            LOG.debug(f"Working on file: {artifact.file_name}")
+            artifact.language = parser.lexer
+            with open(artifact.file_name, "rb") as f:
+                artifact.contents = f.read()
+            return parser.parse(artifact, enabled, disabled)
+    except OSError as e:
+        results.append(
+            Result(
+                "NO_RULE",
+                location=Location(parser.context["node"]),
+                artifact=artifact,
+                level=Level.ERROR,
+                message=e.strerror,
+            )
+        )
+    except SyntaxError as e:
+        results.append(
+            Result(
+                "NO_RULE",
+                location=Location(
+                    start_line=e.lineno,
+                    end_line=e.lineno,
+                ),
+                artifact=artifact,
+                level=Level.ERROR,
+                message="Syntax error while parsing file.",
+            )
+        )
+    except UnicodeDecodeError:
+        results.append(
+            Result(
+                "NO_RULE",
+                location=Location(parser.context["node"]),
+                artifact=artifact,
+                level=Level.ERROR,
+                message="Invalid unicode character while parsing file.",
+            )
+        )
+    except Exception as e:
+        results.append(
+            Result(
+                "NO_RULE",
+                location=Location(parser.context["node"]),
+                artifact=artifact,
+                level=Level.ERROR,
+                message=": ".join([type(e).__name__, str(e)]),
+            )
+        )
+    return results
 
 
 class Run:
     def __init__(
-        self, tool: Tool, parsers: dict, artifacts: list[Artifact], debug
+        self,
+        tool: Tool,
+        enabled: list[str],
+        disabled: list[str],
+        artifacts: list[Artifact],
+        console: Console,
+        debug,
     ):
         self._tool = tool
-        self._parsers = parsers
+        self._enabled = enabled
+        self._disabled = disabled
         self._artifacts = artifacts
+        self._console = console
         self._init_logger(debug)
         self._start_time = None
-        self._endt_time = None
+        self._end_time = None
 
     def _init_logger(self, log_level=logging.INFO):
         """Initialize the logger.
 
         :param debug: Whether to enable debug mode
         :return: An instantiated logging instance
         """
@@ -43,64 +133,62 @@
         LOG.setLevel(log_level)
         handler = logging.StreamHandler(sys.stderr)
         LOG.addHandler(handler)
         LOG.debug("logging initialized")
 
     @property
     def tool(self) -> Tool:
-        """
-        Get the tool associated with this run.
-
-        :return: tool object
-        :rtype: Tool
-        """
+        """Get the tool associated with this run."""
         return self._tool
 
+    @property
+    def rules(self) -> list[Rule]:
+        """Set of supported rules."""
+        return [r for p in parsers.values() for r in p.rules.values()]
+
     def invoke(self):
         """Invokes a run"""
         self._start_time = datetime.datetime.now(datetime.UTC)
+        results = []
+        lines = 0
 
-        # if we have problems with a file, we'll remove it from the file_list
-        # and add it to the skipped list instead
-        new_artifacts = list(self._artifacts)
-        files_skipped = []
         if (
             len(self._artifacts) > PROGRESS_THRESHOLD
             and LOG.getEffectiveLevel() <= logging.INFO
         ):
-            artifacts = progress.track(
-                self._artifacts, description="Analyzing..."
+            parse_artifact = partial(
+                parse_file, enabled=self._enabled, disabled=self._disabled
             )
-        else:
-            artifacts = self._artifacts
 
-        results = []
-        lines = 0
-        for artifact in artifacts:
-            try:
-                if artifact.file_name == "-":
-                    open_fd = os.fdopen(sys.stdin.fileno(), "rb", 0)
-                    fdata = io.BytesIO(open_fd.read())
-                    artifact.file_name = "<stdin>"
-                    artifact.contents = fdata.read()
-                else:
-                    with open(artifact.file_name, "rb") as fdata:
-                        lines += sum(1 for _ in fdata)
-                    with open(artifact.file_name, "rb") as fdata:
-                        artifact.contents = fdata.read()
-                results += self.parse_file(
-                    artifact, new_artifacts, files_skipped
+            with Progress() as progress:
+                task_id = progress.add_task(
+                    "Analyzing...", total=len(self._artifacts)
                 )
-            except OSError as e:
-                files_skipped.append((artifact.file_name, e.strerror))
-                new_artifacts.remove(artifact)
+
+                with Pool(processes=None) as pool:
+                    try:
+                        for res in pool.imap(parse_artifact, self._artifacts):
+                            results += res
+                            progress.advance(task_id)
+                    except KeyboardInterrupt:
+                        sys.exit(2)
+        else:
+            for artifact in self._artifacts:
+                if artifact.file_name != "-":
+                    with open(artifact.file_name, "rb") as f:
+                        lines += sum(1 for _ in f)
+                try:
+                    results += parse_file(
+                        artifact, self._enabled, self._disabled
+                    )
+                except KeyboardInterrupt:
+                    sys.exit(2)
 
         self._metrics = Metrics(
-            files=len(new_artifacts),
-            files_skipped=len(files_skipped),
+            files=len(self._artifacts),
             lines=lines,
             errors=sum(result.level == Level.ERROR for result in results),
             warnings=sum(result.level == Level.WARNING for result in results),
             notes=sum(result.level == Level.NOTE for result in results),
         )
         self._results = results
         self._end_time = datetime.datetime.now(datetime.UTC)
@@ -109,76 +197,16 @@
     def start_time(self):
         return self._start_time
 
     @property
     def end_time(self):
         return self._end_time
 
-    def parse_file(
-        self,
-        artifact: Artifact,
-        new_artifacts: list,
-        files_skipped: list,
-    ) -> list[Result]:
-        try:
-            if artifact.file_name == "<stdin>":
-                lxr = lexers.guess_lexer(artifact.contents)
-                artifact.language = lxr.aliases[0] if lxr.aliases else lxr.name
-                parser = self._parsers.get(artifact.language)
-            else:
-                file_extension = pathlib.Path(artifact.file_name).suffix
-                parser = next(
-                    (
-                        p
-                        for p in self._parsers.values()
-                        if file_extension in p.file_extensions()
-                    ),
-                    None,
-                )
-
-            if parser is not None:
-                LOG.debug("Working on file: %s", artifact.file_name)
-                artifact.language = parser.lexer
-                return parser.parse(artifact)
-        except KeyboardInterrupt:
-            sys.exit(2)
-        except SyntaxError as e:
-            print(
-                f"Syntax error while parsing file. ({e.filename}, "
-                f"line {e.lineno})",
-                file=sys.stderr,
-            )
-            files_skipped.append((artifact.file_name, e))
-            new_artifacts.remove(artifact)
-        except Exception as e:
-            LOG.error(
-                f"Exception occurred when executing rules against "
-                f'{artifact.file_name}. Run "precli --debug '
-                f'{artifact.file_name}" to see the full traceback.'
-            )
-            files_skipped.append(
-                (artifact.file_name, "Exception while parsing file")
-            )
-            new_artifacts.remove(artifact)
-            LOG.debug(f"  Exception string: {e}")
-            LOG.debug(f"  Exception traceback: {traceback.format_exc()}")
-        return []
-
     @property
     def results(self) -> list[Result]:
-        """
-        Get the list of results.
-
-        :return: list of results
-        :rtype: list
-        """
+        """Get the list of results."""
         return self._results
 
     @property
     def metrics(self) -> list[Result]:
-        """
-        Get the list of results.
-
-        :return: list of results
-        :rtype: list
-        """
+        """Get the list of results."""
         return self._metrics
```

### Comparing `precli-0.5.4/precli/core/suppression.py` & `precli-0.5.5/precli/core/suppression.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 Secure Saurce LLC
+# Copyright 2023 Secure Sauce LLC
 from precli.core.location import Location
 from precli.core.status import Status
 
 
 class Suppression:
     def __init__(
         self,
@@ -16,56 +16,33 @@
         self._rules = rules
         self._kind = kind
         self._status = status
         self._justification = justification
 
     @property
     def location(self) -> Location:
-        """
-        Specifies the location of the suppression.
-
-        :return: location of suppression
-        :rtype: Location
-        """
+        """Specifies the location of the suppression."""
         return self._location
 
     @property
     def rules(self) -> set[str]:
-        """
-        What rules are being suppressed.
-
-        :return: set of rule ID/names
-        :rtype: set
-        """
+        """What rules are being suppressed."""
         return self._rules
 
     @property
     def kind(self) -> str:
         """
         The kind of suppression. This can be one of two values:
             "inSource" supporessed inline in the code
             "external" suppressed in an external persistent store
-
-        :return: kind of suppression
-        :rtype: str
         """
         return self._kind
 
     @property
     def status(self) -> Status:
-        """
-        The status of the suppression.
-
-        :return: status on whether to suppress
-        :rtype: Status
-        """
+        """The status of the suppression."""
         return self._status
 
     @property
     def justification(self) -> str:
-        """
-        User-supplied string that explains why the result was suppressed.
-
-        :return: why the result was suppressed
-        :rtype: str
-        """
+        """User-supplied string that explains why the result was suppressed."""
         return self._justification
```

### Comparing `precli-0.5.4/precli/core/symtab.py` & `precli-0.5.5/precli/core/symtab.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 Secure Saurce LLC
+# Copyright 2023 Secure Sauce LLC
 from typing import Self
 
 from precli.core.call import Call
 
 
 class SymbolTable:
     def __init__(self, name, parent=None):
```

### Comparing `precli-0.5.4/precli/core/tool.py` & `precli-0.5.5/precli/core/tool.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,137 +1,72 @@
-# Copyright 2024 Secure Saurce LLC
-from precli.rules import Rule
-
-
+# Copyright 2024 Secure Sauce LLC
 class Tool:
     def __init__(
         self,
         name: str,
         download_uri: str,
         full_description: str,
         information_uri: str,
         organization: str,
         short_description: str,
         version: str,
-        rules: list[Rule],
     ):
         self._name = name
         self._download_uri = download_uri
         self._full_description = full_description
         self._information_uri = information_uri
         self._organization = organization
         self._short_description = short_description
         self._version = version
-        self._rules = rules
         self._release_date = ""
         self._extensions = []
         self._policies = []
 
     @property
     def name(self) -> str:
-        """
-        Name of the tool.
-
-        :return: tool name
-        :rtype: str
-        """
+        """Name of the tool."""
         return self._name
 
     @property
     def download_uri(self) -> str:
-        """
-        URI location to download tool.
-
-        :return: location of download
-        :rtype: str
-        """
+        """URI location to download tool."""
         return self._download_uri
 
     @property
     def full_description(self) -> str:
-        """
-        Full description of the tool.
-
-        :return: full description
-        :rtype: str
-        """
+        """Full description of the tool."""
         return self._full_description
 
     @property
     def information_uri(self) -> str:
-        """
-        Main page URL of the project
-
-        :return: information URI
-        :rtype: str
-        """
+        """Main page URL of the project"""
         return self._information_uri
 
     @property
     def organization(self) -> str:
-        """
-        Organization that produced the tool.
-
-        :return: organization name
-        :rtype: str
-        """
+        """Organization that produced the tool."""
         return self._organization
 
     @property
     def short_description(self) -> str:
-        """
-        Short description of the tool.
-
-        :return: short description
-        :rtype: str
-        """
+        """Short description of the tool."""
         return self._short_description
 
     @property
     def version(self) -> str:
-        """
-        Version of the tool.
-
-        :return: tool version
-        :rtype: str
-        """
+        """Version of the tool."""
         return self._version
 
     @property
     def release_date(self) -> str:
-        """
-        Release date of the tool.
-
-        :return: release date
-        :rtype: str
-        """
+        """Release date of the tool."""
         return self._release_date
 
     @property
     def extensions(self) -> list:
-        """
-        Extensions for the tool in use.
-
-        :return: extension list
-        :rtype: list
-        """
+        """Extensions for the tool in use."""
         return self._extensions
 
     @property
-    def rules(self) -> list[Rule]:
-        """
-        Set of supported rules.
-
-        :return: policy list
-        :rtype: list
-        """
-        return self._rules
-
-    @property
     def policies(self) -> list:
-        """
-        Set of rule configurations.
-
-        :return: policy list
-        :rtype: list
-        """
+        """Set of rule configurations."""
         return self._policies
```

### Comparing `precli-0.5.4/precli/core/utils.py` & `precli-0.5.5/precli/core/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,12 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 
 
 def is_str(value) -> bool:
-    """
-    True if the value is a tree-sitter node string.
-
-    :return: if value is a string
-    :rtype: bool
-    """
+    """True if the value is a tree-sitter node string."""
     if isinstance(value, str) and (
         value.startswith('b"""')
         or value.startswith("b'''")
         or value.startswith('b"')
         or value.startswith("b'")
         or value.startswith('"""')
         or value.startswith("'''")
@@ -22,17 +17,14 @@
     return False
 
 
 def to_str(value: str) -> str:
     """
     Converts a tree-sitter node string value to a
     true string.
-
-    :return: value as string
-    :rtype: str
     """
     if isinstance(value, str):
         value_str = value
         bytestr = False
         if value_str and value_str[0] == "b":
             value_str = value_str[1:]
             bytestr = True
```

### Comparing `precli-0.5.4/precli/parsers/__init__.py` & `precli-0.5.5/precli/parsers/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
+import warnings
 from abc import ABC
 from abc import abstractmethod
 from importlib.metadata import entry_points
 
 import tree_sitter_languages
 from tree_sitter import Node
 
@@ -20,98 +21,90 @@
 
     The parser handles most of the main functions including parsing nodes,
     processing rules based on those nodes, and compiling a list of results.
 
     Each parser is designed to operate on a specific programming language.
     """
 
-    def __init__(self, lang: str, enabled: list = None, disabled: list = None):
-        """
-        Initialize a new parser.
-
-        :param str lang: programming language name
-        :param list enabled: list of rules to enable
-        :param list disabled: list of rules to disable
-        """
+    def __init__(self, lang: str):
+        """Initialize a new parser."""
         self._lexer = lang
-        self.tree_sitter_language = tree_sitter_languages.get_language(lang)
-        self.tree_sitter_parser = tree_sitter_languages.get_parser(lang)
+
+        # Suppress the following warning from tree-sitter
+        # FutureWarning: Language(path, name) is deprecated. Use
+        # Language(ptr, name) instead.
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore", FutureWarning)
+            self.tree_sitter_language = tree_sitter_languages.get_language(
+                lang
+            )
+            self.tree_sitter_parser = tree_sitter_languages.get_parser(lang)
         self.rules = {}
         self.wildcards = {}
 
         discovered_rules = entry_points(group=f"precli.rules.{lang}")
         for rule in discovered_rules:
             self.rules[rule.name] = rule.load()(rule.name)
 
-            if enabled is not None and (
-                enabled == ["all"]
-                or self.rules[rule.name].id in enabled
-                or self.rules[rule.name].name in enabled
-            ):
-                self.rules[rule.name].default_config.enabled = True
-
-            if disabled is not None and (
-                disabled == ["all"]
-                or self.rules[rule.name].id in disabled
-                or self.rules[rule.name].name in disabled
-            ):
-                self.rules[rule.name].default_config.enabled = False
-
             if self.rules[rule.name].wildcards:
                 for k, v in self.rules[rule.name].wildcards.items():
                     if k in self.wildcards:
                         self.wildcards[k] += v
                     else:
                         self.wildcards[k] = v
 
         def child_by_type(self, type: str) -> Node:
             # Return first child with type as specified
             child = list(filter(lambda x: x.type == type, self.named_children))
             return child[0] if child else None
 
-        @property
-        def utf8_text(self) -> str:
-            return self.text.decode()
-
         setattr(Node, "child_by_type", child_by_type)
-        setattr(Node, "utf8_text", utf8_text)
 
     @property
     def lexer(self) -> str:
-        """
-        The name of the lexer
-
-        :return: lexer name
-        :rtype: str
-        """
+        """The name of the lexer"""
         return self._lexer
 
     @abstractmethod
     def file_extensions(self) -> list[str]:
-        """
-        File extension of files this parser can handle.
-        :return: file extensions such as ".py"
-        :rtype: list
-        """
+        """File extension of files this parser can handle."""
 
-    def parse(self, artifact: Artifact) -> list[Result]:
-        """
-        File extension of files this parser can handle.
+    def parse(
+        self, artifact: Artifact, enabled: list = None, disabled: list = None
+    ) -> list[Result]:
+        """File extension of files this parser can handle."""
+        for rule in self.rules.values():
+            if enabled is not None and (
+                enabled == ["all"]
+                or rule.id in enabled
+                or rule.name in enabled
+            ):
+                rule.enabled = True
 
-        :param Artifact artifact: artifact representing the file
+            if disabled is not None and (
+                disabled == ["all"]
+                or rule.id in disabled
+                or rule.name in disabled
+            ):
+                rule.enabled = False
 
-        :return: list of results
-        :rtype: list
-        """
         self.results = []
         self.context = {"artifact": artifact}
+        artifact.encoding = self.get_file_encoding(artifact.file_name)
         if artifact.contents is None:
             with open(artifact.file_name, "rb") as fdata:
                 artifact.contents = fdata.read()
         tree = self.tree_sitter_parser.parse(artifact.contents)
+
+        @property
+        def string(self) -> str:
+            return self.text.decode(encoding=artifact.encoding)
+
+        setattr(Node, "string", string)
+
         self.visit([tree.root_node])
 
         for result in self.results:
             result.artifact = artifact
 
             suppression = self.suppressions.get(result.location.start_line)
             if suppression and result.rule_id in suppression.rules:
@@ -121,26 +114,24 @@
 
     def visit(self, nodes: list[Node]):
         """
         Generic visitor of nodes.
 
         THis function will visit each node and attempt to call a more
         specific visit function if defined based on the node type.
-
-        :param list nodes: list of nodes
         """
         for node in nodes:
             # print(node)
 
             self.context["node"] = node
             visitor_fn = getattr(self, f"visit_{node.type}", self.visit)
             visitor_fn(node.children)
 
     def visit_comment(self, nodes: list[Node]):
-        comment = self.context["node"].text.decode()
+        comment = self.context["node"].string
 
         suppressed = self.SUPPRESS_COMMENT.search(comment)
         if suppressed is None:
             return
 
         matches = suppressed.groupdict()
         suppressed_rules = matches.get("rules")
@@ -203,23 +194,18 @@
 
     def analyze_node(self, node_type: str, **kwargs: dict) -> list[Result]:
         """
         Process the rules based on node_type.
 
         This function will iterate through all rules that are designed to
         handle the given node type (node_type).
-
-        :param str node_type: process nodes of this node type
-
-        :return: list of results
-        :rtype: list
         """
         fn = f"analyze_{node_type}"
         for rule in self.rules.values():
-            if hasattr(rule, fn) and rule.default_config.enabled:
+            if hasattr(rule, fn) and rule.enabled:
                 context = self.context
                 context["symtab"] = self.current_symtab
 
                 analyze_fn = getattr(rule, fn)
                 result = analyze_fn(self.context, **kwargs)
 
                 if result is not None:
```

### Comparing `precli-0.5.4/precli/parsers/go.py` & `precli-0.5.5/precli/parsers/go.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,34 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 import ast
 import re
 
 from tree_sitter import Node
 
 from precli.core.call import Call
 from precli.core.symtab import Symbol
 from precli.core.symtab import SymbolTable
 from precli.parsers import Parser
 from precli.parsers import tokens
 
 
 class Go(Parser):
-    def __init__(self, enabled: list = None, disabled: list = None):
-        super().__init__("go", enabled, disabled)
+    def __init__(self):
+        super().__init__("go")
         self.SUPPRESS_COMMENT = re.compile(
             r"// suppress:? (?P<rules>[^#]+)?#?"
         )
         self.SUPPRESSED_RULES = re.compile(r"(?:(GO\d\d\d|[a-z_]+),?)+")
 
     def file_extensions(self) -> list[str]:
         return [".go"]
 
+    def get_file_encoding(self, file_path):
+        return "utf-8"
+
     def visit_source_file(self, nodes: list[Node]):
         self.suppressions = {}
         self.current_symtab = SymbolTable("<source_file>")
         self.visit(nodes)
         self.current_symtab = self.current_symtab.parent()
 
     def visit_import_declaration(self, nodes: list[Node]):
@@ -44,24 +47,24 @@
 
     def import_spec(self, nodes: list[Node]):
         imports = {}
 
         match nodes[0].type:
             case tokens.INTERPRETED_STRING_LITERAL:
                 # import "fmt"
-                package = ast.literal_eval(nodes[0].utf8_text)
+                package = ast.literal_eval(nodes[0].string)
                 default_package = package.split("/")[-1]
                 imports[default_package] = package
 
             case tokens.PACKAGE_IDENTIFIER:
                 # import fm "fmt"
                 # Can use fm.Println instead of fmt.Println
                 if nodes[1].type == tokens.INTERPRETED_STRING_LITERAL:
-                    alias = nodes[0].utf8_text
-                    package = ast.literal_eval(nodes[1].utf8_text)
+                    alias = nodes[0].string
+                    package = ast.literal_eval(nodes[1].string)
                     imports[alias] = package
 
             case tokens.DOT:
                 # import . "fmt"
                 # Can just call Println instead of fmt.Println
                 # TODO: similar to Python wildcard imports
                 pass
@@ -73,15 +76,15 @@
                 # variables directly.
                 pass
 
         return imports
 
     def visit_function_declaration(self, nodes: list[Node]):
         func_id = self.context["node"].child_by_type(tokens.IDENTIFIER)
-        func = func_id.utf8_text
+        func = func_id.string
         self.current_symtab = SymbolTable(func, parent=self.current_symtab)
         self.visit(nodes)
         self.current_symtab = self.current_symtab.parent()
 
     def _get_var_node(self, node: Node) -> Node:
         if (
             len(node.named_children) >= 2
@@ -121,15 +124,15 @@
             arg_list_node=arg_list_node,
             args=func_call_args,
         )
 
         self.analyze_node(tokens.CALL_EXPRESSION, call=call)
 
         if call.var_node is not None:
-            symbol = self.current_symtab.get(call.var_node.utf8_text)
+            symbol = self.current_symtab.get(call.var_node.string)
             if symbol is not None and symbol.type == tokens.IDENTIFIER:
                 symbol.push_call(call)
         else:
             # TODO: why is var_node None?
             pass
 
         self.visit(nodes)
@@ -141,45 +144,45 @@
         args = []
         for child in node.named_children:
             args.append(self.resolve(child, default=child))
 
         return args
 
     def get_qual_name(self, node: Node) -> Symbol:
-        nodetext = node.utf8_text
+        nodetext = node.string
         symbol = self.current_symtab.get(nodetext)
 
         if symbol is not None:
             return symbol
         for child in node.children:
             return self.get_qual_name(child)
 
     def unchain(self, node: Node, result: list):
         """
         Unchain an attribute into its component identifiers skipping
         over argument_list of a call node and such.
         """
         if node.type == tokens.IDENTIFIER:
-            result.append(node.utf8_text)
+            result.append(node.string)
         for child in node.named_children:
             if child.type != tokens.ARGUMENT_LIST:
                 self.unchain(child, result)
 
     def resolve(self, node: Node, default=None):
         """
         Resolve the given node into its liternal value.
         """
-        nodetext = node.utf8_text
+        nodetext = node.string
         if isinstance(default, Node):
-            default = default.utf8_text
+            default = default.string
 
         try:
             match node.type:
                 case tokens.SELECTOR_EXPRESSION:
-                    nodetext = node.utf8_text
+                    nodetext = node.string
                     symbol = self.get_qual_name(node)
                     if symbol is not None:
                         value = self.join_symbol(nodetext, symbol)
                 case tokens.IDENTIFIER:
                     symbol = self.get_qual_name(node)
                     if symbol is not None:
                         value = self.join_symbol(nodetext, symbol)
```

### Comparing `precli-0.5.4/precli/parsers/java.py` & `precli-0.5.5/precli/parsers/java.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,33 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 import re
 
 from tree_sitter import Node
 
 from precli.core.call import Call
 from precli.core.symtab import Symbol
 from precli.core.symtab import SymbolTable
 from precli.parsers import Parser
 from precli.parsers import tokens
 
 
 class Java(Parser):
-    def __init__(self, enabled: list = None, disabled: list = None):
-        super().__init__("java", enabled, disabled)
+    def __init__(self):
+        super().__init__("java")
         self.SUPPRESS_COMMENT = re.compile(
             r"// suppress:? (?P<rules>[^#]+)?#?"
         )
         self.SUPPRESSED_RULES = re.compile(r"(?:(JAV\d\d\d|[a-z_]+),?)+")
 
     def file_extensions(self) -> list[str]:
         return [".java"]
 
+    def get_file_encoding(self, file_path):
+        return "utf-8"
+
     def visit_program(self, nodes: list[Node]):
         self.suppressions = {}
         self.current_symtab = SymbolTable("<program>")
         self.visit(nodes)
         self.current_symtab = self.current_symtab.parent()
 
     def visit_import_declaration(self, nodes: list[Node]):
@@ -32,71 +35,71 @@
             return
 
         if nodes[1].type != tokens.SCOPED_IDENTIFIER:
             return
 
         if len(nodes) > 3 and nodes[3].type == tokens.ASTERISK:
             # "import" scoped_identifier "." asterisk ";"
-            wc_import = nodes[1].utf8_text
+            wc_import = nodes[1].string
 
             if f"{wc_import}.*" in self.wildcards:
                 for wc in self.wildcards[f"{wc_import}.*"]:
                     full_import = ".".join(filter(None, [wc_import, wc]))
                     self.current_symtab.put(wc, tokens.IMPORT, full_import)
         else:
             # "import" scoped_identifier ";"
-            package = nodes[1].utf8_text
+            package = nodes[1].string
             symbol = package.split(".")[-1]
             self.current_symtab.put(symbol, tokens.IMPORT, package)
 
     def visit_class_declaration(self, nodes: list[Node]):
         class_id = self.context["node"].child_by_type(tokens.IDENTIFIER)
-        cls_name = class_id.utf8_text
+        cls_name = class_id.string
         self.current_symtab = SymbolTable(cls_name, parent=self.current_symtab)
         self.visit(nodes)
         self.current_symtab = self.current_symtab.parent()
 
     def visit_interface_declaration(self, nodes: list[Node]):
         if_id = self.context["node"].child_by_type(tokens.IDENTIFIER)
-        if_name = if_id.utf8_text
+        if_name = if_id.string
         self.current_symtab = SymbolTable(if_name, parent=self.current_symtab)
         self.visit(nodes)
         self.current_symtab = self.current_symtab.parent()
 
     def visit_annotation_type_declaration(self, nodes: list[Node]):
         anno_id = self.context["node"].child_by_type(tokens.IDENTIFIER)
-        ann_name = anno_id.utf8_text
+        ann_name = anno_id.string
         self.current_symtab = SymbolTable(ann_name, parent=self.current_symtab)
         self.visit(nodes)
         self.current_symtab = self.current_symtab.parent()
 
     def visit_enum_declaration(self, nodes: list[Node]):
         enum_id = self.context["node"].child_by_type(tokens.IDENTIFIER)
-        e_name = enum_id.utf8_text
+        e_name = enum_id.string
         self.current_symtab = SymbolTable(e_name, parent=self.current_symtab)
         self.visit(nodes)
         self.current_symtab = self.current_symtab.parent()
 
     def visit_constructor_declaration(self, nodes: list[Node]):
         const_id = self.context["node"].child_by_type(tokens.IDENTIFIER)
-        cst_name = const_id.utf8_text
+        cst_name = const_id.string
         self.current_symtab = SymbolTable(cst_name, parent=self.current_symtab)
         self.visit(nodes)
         self.current_symtab = self.current_symtab.parent()
 
     def visit_record_declaration(self, nodes: list[Node]):
         record_id = self.context["node"].child_by_type(tokens.IDENTIFIER)
-        rec_name = record_id.utf8_text
+        rec_name = record_id.string
         self.current_symtab = SymbolTable(rec_name, parent=self.current_symtab)
         self.visit(nodes)
         self.current_symtab = self.current_symtab.parent()
 
     def visit_method_declaration(self, nodes: list[Node]):
         method_id = self.context["node"].child_by_type(tokens.IDENTIFIER)
-        mth_name = method_id.utf8_text
+        mth_name = method_id.string
         self.current_symtab = SymbolTable(mth_name, parent=self.current_symtab)
         self.visit(nodes)
         self.current_symtab = self.current_symtab.parent()
 
     def _get_var_node(self, node: Node) -> Node:
         if (
             len(node.named_children) >= 2
@@ -153,15 +156,15 @@
             )
         ):
             left_hand = self.resolve(var_nodes[0], default=var_nodes[0])
             right_hand = self.resolve(var_nodes[1], default=var_nodes[1])
 
             # This is in case a variable is reassigned
             self.current_symtab.put(
-                var_nodes[0].utf8_text, tokens.IDENTIFIER, right_hand
+                var_nodes[0].string, tokens.IDENTIFIER, right_hand
             )
 
             # This is to help full resolution of an attribute/call.
             # This results in two entries in the symtab for this assignment.
             self.current_symtab.put(left_hand, tokens.IDENTIFIER, right_hand)
 
             if var_nodes[1].type == tokens.METHOD_INVOCATION:
@@ -196,29 +199,29 @@
     def visit_method_invocation(self, nodes: list[Node]):
         if nodes[0].type not in (tokens.FIELD_ACCESS, tokens.IDENTIFIER):
             return
 
         if nodes[1].type == "." and nodes[2].type == tokens.IDENTIFIER:
             # (field_access | identifier) "." identifier argument_list
             obj_name = self.resolve(nodes[0])
-            method = nodes[2].utf8_text
+            method = nodes[2].string
             if None in (obj_name, method):
                 return
             func_call_qual = ".".join([obj_name, method])
         else:
             # identifier argument_list
             method_name = self.resolve(nodes[0])
             if method_name is None:
                 return
             func_call_qual = method_name
 
         call = self.method_call(self.context["node"], func_call_qual)
         self.analyze_node(tokens.METHOD_INVOCATION, call=call)
 
-        symbol = self.current_symtab.get(call.var_node.utf8_text)
+        symbol = self.current_symtab.get(call.var_node.string)
         if symbol is not None and symbol.type == tokens.IDENTIFIER:
             symbol.push_call(call)
 
         self.visit(nodes)
 
     def method_call(self, node: Node, func_call_qual: str):
         if (
@@ -265,42 +268,42 @@
         args = []
         for child in node.named_children:
             args.append(self.resolve(child, default=child))
 
         return args
 
     def get_qual_name(self, node: Node) -> Symbol:
-        nodetext = node.utf8_text
+        nodetext = node.string
         symbol = self.current_symtab.get(nodetext)
 
         if symbol is not None:
             return symbol
         for child in node.children:
             return self.get_qual_name(child)
 
     def resolve(self, node: Node, default=None):
         """
         Resolve the given node into its liternal value.
         """
-        nodetext = node.utf8_text
+        nodetext = node.string
         if isinstance(default, Node):
-            default = default.utf8_text
+            default = default.string
 
         try:
             match node.type:
                 case tokens.OBJECT_CREATION_EXPRESSION:
                     # "new" (type_identifier | scoped_type_identifier)
                     # argument_list
                     if node.children[0].type == "new" and node.children[
                         1
                     ].type in (
                         tokens.TYPE_IDENTIFIER,
                         tokens.SCOPED_TYPE_IDENTIFIER,
                     ):
-                        nodetext = node.children[1].utf8_text
+                        nodetext = node.children[1].string
                         if (
                             node.children[1].type
                             == tokens.SCOPED_TYPE_IDENTIFIER
                         ):
                             symbol = Symbol(
                                 nodetext, tokens.IDENTIFIER, nodetext
                             )
@@ -311,20 +314,20 @@
                 case tokens.METHOD_INVOCATION:
                     if (
                         node.children[1].type == "."
                         and node.children[2].type == tokens.IDENTIFIER
                     ):
                         # (field_access | identifier) "." identifier
                         # argument_list
-                        part1 = node.children[0].utf8_text
-                        part2 = node.children[2].utf8_text
+                        part1 = node.children[0].string
+                        part2 = node.children[2].string
                         nodetext = ".".join([part1, part2])
                     else:
                         # identifier argument_list
-                        nodetext = node.children[0].utf8_text
+                        nodetext = node.children[0].string
                     symbol = self.get_qual_name(node.children[0])
                     if symbol is not None:
                         value = self.join_symbol(nodetext, symbol)
                 case tokens.FIELD_ACCESS:
                     symbol = Symbol(nodetext, tokens.IDENTIFIER, nodetext)
                     value = self.join_symbol(nodetext, symbol)
                 case tokens.IDENTIFIER:
```

### Comparing `precli-0.5.4/precli/parsers/python.py` & `precli-0.5.5/precli/parsers/python.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 import builtins
+import codecs
 import re
+import warnings
 from collections import namedtuple
 
 from tree_sitter import Node
 
 from precli.core.call import Call
 from precli.core.comparison import Comparison
 from precli.core.symtab import Symbol
@@ -13,22 +15,37 @@
 from precli.parsers import tokens
 
 
 Import = namedtuple("Import", "module alias")
 
 
 class Python(Parser):
-    def __init__(self, enabled: list = None, disabled: list = None):
-        super().__init__("python", enabled, disabled)
+    def __init__(self):
+        super().__init__("python")
         self.SUPPRESS_COMMENT = re.compile(r"# suppress:? (?P<rules>[^#]+)?#?")
         self.SUPPRESSED_RULES = re.compile(r"(?:(PY\d\d\d|[a-z_]+),?)+")
 
     def file_extensions(self) -> list[str]:
         return [".py", ".pyw"]
 
+    def get_file_encoding(self, file_path):
+        with open(file_path, "rb") as f:
+            first_two_lines = f.readline() + f.readline()
+
+        encoding_match = re.search(rb"coding[:=]\s*([-\w.]+)", first_two_lines)
+        if encoding_match:
+            encoding = encoding_match.group(1).decode("ascii")
+            try:
+                codecs.lookup(encoding)
+            except LookupError:
+                encoding = "utf-8"
+        else:
+            encoding = "utf-8"
+        return encoding
+
     def visit_module(self, nodes: list[Node]):
         self.suppressions = {}
         self.current_symtab = SymbolTable("<module>")
         self.visit(nodes)
         self.current_symtab = self.current_symtab.parent()
 
     def visit_import_statement(self, nodes: list[Node]):
@@ -39,22 +56,22 @@
     def visit_import_from_statement(self, nodes: list[Node]):
         imps = self.import_from_statement(nodes)
         for key, value in imps.items():
             self.current_symtab.put(key, tokens.IMPORT, value)
 
     def visit_class_definition(self, nodes: list[Node]):
         class_id = self.context["node"].child_by_type(tokens.IDENTIFIER)
-        cls_name = class_id.utf8_text
+        cls_name = class_id.string
         self.current_symtab = SymbolTable(cls_name, parent=self.current_symtab)
         self.visit(nodes)
         self.current_symtab = self.current_symtab.parent()
 
     def visit_function_definition(self, nodes: list[Node]):
         func_id = self.context["node"].child_by_type(tokens.IDENTIFIER)
-        func = func_id.utf8_text
+        func = func_id.string
         self.current_symtab = SymbolTable(func, parent=self.current_symtab)
         self.visit(nodes)
         self.current_symtab = self.current_symtab.parent()
 
     def visit_typed_default_parameter(self, nodes: list[Node]):
         self.visit_typed_parameter(nodes)
 
@@ -68,25 +85,25 @@
             tokens.STRING,
             tokens.INTEGER,
             tokens.FLOAT,
             tokens.TRUE,
             tokens.FALSE,
             tokens.NONE,
         ):
-            param_name = param_id.utf8_text
+            param_name = param_id.string
             param_type = self.resolve(
                 param_type.named_children[0],
                 default=param_type.named_children[0],
             )
             self.current_symtab.put(param_name, tokens.IDENTIFIER, param_type)
 
         self.visit(nodes)
 
     def visit_named_expression(self, nodes: list[Node]):
-        if len(nodes) > 1 and nodes[1].utf8_text == ":=":
+        if len(nodes) > 1 and nodes[1].string == ":=":
             self.visit_assignment(nodes)
         else:
             self.visit(nodes)
 
     def visit_assignment(self, nodes: list[Node]):
         # pattern_list = expression_list (i.e. HOST, PORT = "", 9999)
         if (
@@ -115,15 +132,15 @@
             tokens.NONE,
         ):
             left_hand = self.resolve(nodes[0], default=nodes[0])
             right_hand = self.resolve(nodes[2], default=nodes[2])
 
             # This is in case a variable is reassigned
             self.current_symtab.put(
-                nodes[0].utf8_text, tokens.IDENTIFIER, right_hand
+                nodes[0].string, tokens.IDENTIFIER, right_hand
             )
 
             # This is to help full resolution of an attribute/call.
             # This results in two entries in the symtab for this assignment.
             self.current_symtab.put(left_hand, tokens.IDENTIFIER, right_hand)
 
             if nodes[2].type == tokens.CALL:
@@ -198,22 +215,27 @@
         if (
             call.name_qualified == "importlib.import_module"
             and self.context["node"].parent.type == tokens.ASSIGNMENT
         ):
             module = self.importlib_import_module(call)
             if module:
                 left_hand = self.context["node"].parent.children[0]
-                identifier = left_hand.utf8_text
+                identifier = left_hand.string
                 self.current_symtab.remove(identifier)
                 self.current_symtab.put(identifier, tokens.IMPORT, module)
 
-        self.analyze_node(tokens.CALL, call=call)
+        # Suppress re module FutureWarnings. Usually a result of scanning
+        # test cases in cpython repo.
+        # For example: FutureWarning: Possible set union at position 6
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore", FutureWarning)
+            self.analyze_node(tokens.CALL, call=call)
 
         if call.var_node is not None:
-            symbol = self.current_symtab.get(call.var_node.utf8_text)
+            symbol = self.current_symtab.get(call.var_node.string)
             if symbol is not None and symbol.type == tokens.IDENTIFIER:
                 symbol.push_call(call)
         else:
             # TODO: why is var_node None?
             pass
 
         self.visit(nodes)
@@ -263,15 +285,15 @@
                     symbol.push_call(call)
 
         self.visit(nodes)
 
     def visit_comparison_operator(self, nodes: list[Node]):
         if len(nodes) > 2:
             left_hand = self.resolve(nodes[0], default=nodes[0])
-            operator = nodes[1].utf8_text
+            operator = nodes[1].string
             right_hand = self.resolve(nodes[2], default=nodes[2])
 
             comparison = Comparison(
                 self.context["node"],
                 left_hand=left_hand,
                 operator=operator,
                 right_hand=right_hand,
@@ -281,31 +303,31 @@
             )
         self.visit(nodes)
 
     def import_statement(self, nodes: list[Node]) -> dict:
         imports = {}
         for child in nodes:
             if child.type == tokens.DOTTED_NAME:
-                imports[child.utf8_text] = child.utf8_text
+                imports[child.string] = child.string
             elif child.type == tokens.ALIASED_IMPORT:
                 module = child.child_by_type(tokens.DOTTED_NAME)
                 alias = child.child_by_type(tokens.IDENTIFIER)
-                imports[alias.utf8_text] = module.utf8_text
+                imports[alias.string] = module.string
         return imports
 
     def parse_import_statement(self, nodes: list[Node]) -> list:
         imports = []
         for child in nodes:
             if child.type == tokens.DOTTED_NAME:
-                plain_import = Import(child.utf8_text, None)
+                plain_import = Import(child.string, None)
                 imports.append(plain_import)
             elif child.type == tokens.ALIASED_IMPORT:
                 module = child.child_by_type(tokens.DOTTED_NAME)
                 alias = child.child_by_type(tokens.IDENTIFIER)
-                alias_import = Import(module.utf8_text, alias.utf8_text)
+                alias_import = Import(module.string, alias.string)
                 imports.append(alias_import)
         return imports
 
     def unparse_import_statement(self, imports: list) -> str:
         modules = []
         for imp in imports:
             if imp.alias is not None:
@@ -315,15 +337,15 @@
         return f"{tokens.IMPORT} {', '.join(modules)}"
 
     def import_from_statement(self, nodes: list[Node]) -> dict:
         imports = {}
 
         module = nodes[1]
         if module.type == tokens.DOTTED_NAME:
-            from_module = module.utf8_text
+            from_module = module.string
         elif module.type == tokens.RELATIVE_IMPORT:
             # No known way to resolve the relative to absolute
             # However, shouldn't matter much since most rules
             # won't check for local modules.
             from_module = ""
 
         if nodes[2].type == tokens.IMPORT:
@@ -343,17 +365,17 @@
                     imports[key] = ".".join(filter(None, full_qual))
 
         return imports
 
     def parse_import_from_statement(self, nodes: list[Node]) -> tuple:
         module = nodes[1]
         if module.type == tokens.DOTTED_NAME:
-            package = module.utf8_text
+            package = module.string
         elif module.type == tokens.RELATIVE_IMPORT:
-            package = module.utf8_text
+            package = module.string
 
         if nodes[2].type == tokens.IMPORT:
             if nodes[3].type == tokens.WILDCARD_IMPORT:
                 modules = [Import("*", None)]
             else:
                 modules = self.parse_import_statement(nodes[3:])
             return (package, modules)
@@ -389,46 +411,46 @@
             if child.type == tokens.KEYWORD_ARGUMENT:
                 kwargs |= self.resolve(child)
             else:
                 args.append(self.resolve(child, default=child))
         return args, kwargs
 
     def get_qual_name(self, node: Node) -> Symbol:
-        nodetext = node.utf8_text
+        nodetext = node.string
         symbol = self.current_symtab.get(nodetext)
         if symbol is not None:
             return symbol
         if nodetext in dir(builtins):
             return Symbol(nodetext, tokens.IDENTIFIER, nodetext)
         for child in node.children:
             return self.get_qual_name(child)
 
     def unchain(self, node: Node, result: list):
         """
         Unchain an attribute into its component identifiers skipping
         over argument_list of a call node and such.
         """
         if node.type == tokens.IDENTIFIER:
-            result.append(node.utf8_text)
+            result.append(node.string)
         for child in node.named_children:
             if child.type != tokens.ARGUMENT_LIST:
                 self.unchain(child, result)
 
     def resolve(self, node: Node, default=None):
         """
         Resolve the given node into its liternal value.
         """
-        nodetext = node.utf8_text
+        nodetext = node.string
         if isinstance(default, Node):
-            default = default.utf8_text
+            default = default.string
 
         try:
             match node.type:
                 case tokens.CALL:
-                    nodetext = node.children[0].utf8_text
+                    nodetext = node.children[0].string
                     symbol = self.get_qual_name(node.children[0])
                     if symbol is not None:
                         value = self.join_symbol(nodetext, symbol)
                 case tokens.ATTRIBUTE:
                     result = []
                     self.unchain(node, result)
                     nodetext = ".".join(result)
@@ -436,15 +458,15 @@
                     if symbol is not None:
                         value = self.join_symbol(nodetext, symbol)
                 case tokens.IDENTIFIER:
                     symbol = self.get_qual_name(node)
                     if symbol is not None:
                         value = self.join_symbol(nodetext, symbol)
                 case tokens.KEYWORD_ARGUMENT:
-                    keyword = node.named_children[0].utf8_text
+                    keyword = node.named_children[0].string
                     kwvalue = node.named_children[1]
                     value = {keyword: self.resolve(kwvalue, default=kwvalue)}
                 case tokens.DICTIONARY:
                     # TODO: don't use ast.literal_eval
                     # value = ast.literal_eval(nodetext)
                     pass
                 case tokens.LIST:
```

### Comparing `precli-0.5.4/precli/parsers/tokens.py` & `precli-0.5.5/precli/parsers/tokens.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 IMPORT = "import"
 IMPORT_SPEC = "import_spec"
 IMPORT_SPEC_LIST = "import_spec_list"
 SCOPED_IDENTIFIER = "scoped_identifier"
 DOTTED_NAME = "dotted_name"
 DOT = "dot"
 ASTERISK = "asterisk"
```

### Comparing `precli-0.5.4/precli/renderers/detailed.py` & `precli-0.5.5/precli/renderers/detailed.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-# Copyright 2024 Secure Saurce LLC
-import sys
-
+# Copyright 2024 Secure Sauce LLC
 from rich import box
 from rich import syntax
+from rich.console import Console
 from rich.table import Table
 
 from precli.core.level import Level
 from precli.core.linecache import LineCache
 from precli.core.run import Run
 from precli.renderers import Renderer
 from precli.rules import Rule
 
 
 class Detailed(Renderer):
-    def __init__(self, file: sys.stdout, no_color: bool = False):
-        super().__init__(file=file, no_color=no_color)
+    def __init__(self, console: Console):
+        super().__init__(console)
 
     def render(self, run: Run):
         for result in run.results:
             match result.level:
                 case Level.ERROR:
                     emoji = ":no_entry-emoji:"
                     style = "red"
@@ -46,22 +45,21 @@
             self.console.print(
                 f"{emoji} {result.level.name.title()} on line "
                 f"{result.location.start_line} in {file_name}",
                 style=style,
                 markup=False,
             )
             rule = Rule.get_by_id(result.rule_id)
-            self.console.print(
-                f"{rule.id}: {rule.cwe.name}",
-                style=style,
-            )
-            self.console.print(
-                f"{result.message}",
-                style=style,
-            )
+            if rule:
+                self.console.print(f"{rule.id}: {rule.cwe.name}", style=style)
+            else:
+                self.console.print(
+                    f"{result.rule_id}: Parsing error", style=style
+                )
+            self.console.print(f"{result.message}", style=style)
 
             line_offset = result.location.start_line - 2
             code = syntax.Syntax(
                 result.snippet,
                 result.artifact.language,
                 line_numbers=True,
                 start_line=line_offset + 1,
@@ -144,18 +142,14 @@
         table.add_column(justify="left")
         table.add_column(justify="right")
         table.add_row(
             "Files analyzed",
             f"{run.metrics.files:,}",
             "Lines analyzed",
             f"{run.metrics.lines:,}",
-        )
-        table.add_row(
-            "Files skipped",
-            f"{run.metrics.files_skipped:,}",
             end_section=True,
         )
         table.add_row(
             "Errors",
             f"{run.metrics.errors:,}",
             style="red" if run.metrics.errors else "",
         )
```

### Comparing `precli-0.5.4/precli/renderers/json.py` & `precli-0.5.5/precli/renderers/json.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,31 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 import pathlib
-import sys
 import urllib.parse as urlparse
+from importlib import metadata
 
 import sarif_om
 from jschema_to_python.to_json import to_json
+from rich.console import Console
 
 from precli.core.fix import Fix
 from precli.core.result import Result
 from precli.core.run import Run
 from precli.renderers import Renderer
 from precli.rules import Rule
 
 
 SCHEMA_URI = "https://json.schemastore.org/sarif-2.1.0.json"
 SCHEMA_VER = "2.1.0"
 TS_FORMAT = "%Y-%m-%dT%H:%M:%SZ"
 
 
 class Json(Renderer):
-    def __init__(self, file: sys.stdout, no_color: bool = False):
-        super().__init__(file=file, no_color=no_color)
+    def __init__(self, console: Console):
+        super().__init__(console)
 
     def to_uri(self, file):
         path = pathlib.PurePath(file)
         if path.is_absolute():
             return path.as_uri()
         else:
             posix = path.as_posix()
@@ -56,24 +57,31 @@
             description=sarif_om.Message(text=fix.description),
         )
 
     def create_rule_if_needed(
         self, result: Result, rules: dict, rule_indices: dict
     ):
         rule = Rule.get_by_id(result.rule_id)
+        if not rule:
+            return None, -1
+
         if rule.id in rules:
             return rules[rule.id], rule_indices[rule.id]
 
         reporting_descriptor = sarif_om.ReportingDescriptor(
             id=rule.id,
             name=rule.__class__.__name__,
             help_uri=rule.help_url,
             short_description=sarif_om.MultiformatMessageString(
                 text=rule.short_description
             ),
+            default_configuration=sarif_om.ReportingConfiguration(
+                enabled=rule.default_config.enabled,
+                level=rule.default_config.level.name.lower(),
+            ),
             help=sarif_om.MultiformatMessageString(
                 text=rule.full_description, markdown=rule.full_description
             ),
             message_strings={
                 "default": sarif_om.MultiformatMessageString(text=rule.message)
             },
             properties={
@@ -102,21 +110,40 @@
             organization=run.tool.organization,
             semantic_version=run.tool.version,
             short_description=sarif_om.MultiformatMessageString(
                 text=run.tool.short_description
             ),
         )
 
+    def get_extensions(self) -> list:
+        precli_exts = []
+        for dist in metadata.distributions():
+            if dist.name.startswith("precli-"):
+                precli_exts.append(
+                    sarif_om.ToolComponent(
+                        name=dist.name,
+                        organization=dist.metadata["Author"],
+                        semantic_version=dist.version,
+                        short_description=sarif_om.MultiformatMessageString(
+                            text=dist.metadata["Summary"]
+                        ),
+                    )
+                )
+        return precli_exts
+
     def render(self, run: Run):
         log = sarif_om.SarifLog(
             schema_uri=SCHEMA_URI,
             version=SCHEMA_VER,
             runs=[
                 sarif_om.Run(
-                    tool=sarif_om.Tool(driver=self.create_tool_component(run)),
+                    tool=sarif_om.Tool(
+                        driver=self.create_tool_component(run),
+                        extensions=self.get_extensions(),
+                    ),
                     invocations=[
                         sarif_om.Invocation(
                             start_time_utc=run.start_time.strftime(TS_FORMAT),
                             end_time_utc=run.end_time.strftime(TS_FORMAT),
                             execution_successful=True,
                         )
                     ],
@@ -141,32 +168,36 @@
 
             physical_location = sarif_om.PhysicalLocation(
                 artifact_location=sarif_om.ArtifactLocation(
                     uri=self.to_uri(result.artifact.file_name)
                 )
             )
 
-            code_lines = result.snippet.splitlines(keepends=True)
-            code_line = code_lines[1] if len(code_lines) > 1 else code_lines[0]
             physical_location.region = sarif_om.Region(
                 start_line=result.location.start_line,
                 end_line=result.location.end_line,
                 start_column=result.location.start_column + 1,
                 end_column=result.location.end_column + 1,
-                snippet=sarif_om.ArtifactContent(text=code_line),
             )
 
-            physical_location.context_region = sarif_om.Region(
-                start_line=result.location.start_line - 1,
-                end_line=result.location.end_line + 1,
-                snippet=sarif_om.ArtifactContent(text=result.snippet),
-            )
+            if result.snippet:
+                lines = result.snippet.splitlines(keepends=True)
+                code_line = lines[1] if len(lines) > 1 else lines[0]
+                physical_location.region.snippet = sarif_om.ArtifactContent(
+                    text=code_line
+                )
+
+                physical_location.context_region = sarif_om.Region(
+                    start_line=result.location.start_line - 1,
+                    end_line=result.location.end_line + 1,
+                    snippet=sarif_om.ArtifactContent(text=result.snippet),
+                )
 
             sarif_result = sarif_om.Result(
-                rule_id=rule.id,
+                rule_id=result.rule_id,
                 rule_index=rule_index,
                 message=sarif_om.Message(text=result.message),
                 fixes=fixes,
                 level=result.level.name.lower(),
                 locations=[
                     sarif_om.Location(physical_location=physical_location),
                 ],
```

### Comparing `precli-0.5.4/precli/renderers/markdown.py` & `precli-0.5.5/precli/renderers/markdown.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,40 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 import logging
 import sys
 
 from rich import markdown
+from rich.console import Console
 
 from precli.core.level import Level
 from precli.core.linecache import LineCache
 from precli.core.run import Run
 from precli.renderers import Renderer
 from precli.rules import Rule
 
 
 logging.getLogger("markdown_it").setLevel(logging.INFO)
 
 
 class Markdown(Renderer):
-    def __init__(self, file: sys.stdout, no_color: bool = False):
-        super().__init__(file=file, no_color=no_color)
+    def __init__(self, console: Console):
+        super().__init__(console)
 
     def render(self, run: Run):
         output = ""
         for result in run.results:
             rule = Rule.get_by_id(result.rule_id)
 
-            linecache = LineCache(
-                result.artifact.file_name,
-                result.artifact.contents.decode(),
-            )
+            try:
+                linecache = LineCache(
+                    result.artifact.file_name,
+                    result.artifact.contents.decode(result.artifact.encoding),
+                )
+            except UnicodeDecodeError:
+                pass
 
             match result.level:
                 case Level.ERROR:
                     alert = "CAUTION"
                 case Level.WARNING:
                     alert = "WARNING"
                 case Level.NOTE:
@@ -44,29 +48,37 @@
                     )
                 else:
                     lines = f"L{result.location.start_line}"
                 file_name = f"{result.artifact.uri}#{lines}"
             else:
                 file_name = result.artifact.file_name
 
-            output += (
-                f"> [!{alert}]\n"
-                f">\n"
-                f"> [{rule.id}]({rule.help_url}): {rule.cwe.name}\n"
-                f"on line {result.location.start_line} in {file_name}\n"
-                f"> \n"
-                f"> {result.message}\n"
-            )
-
-            output += f"> ```{result.artifact.language}\n"
-            for lineno in range(
-                result.location.start_line, result.location.end_line + 1
-            ):
-                output += f"> {linecache.getline(lineno=lineno)}"
-            output += "> ```\n"
+            if rule:
+                output += (
+                    f"> [!{alert}]\n"
+                    f">\n"
+                    f"> [{rule.id}]({rule.help_url}): {rule.cwe.name}\n"
+                    f"on line {result.location.start_line} in {file_name}\n"
+                    f"> \n"
+                    f"> {result.message}\n"
+                )
+            else:
+                output += (
+                    f"> [!{alert}]\n"
+                    f">\n"
+                    f"> {result.rule_id}: Parsing error\n"
+                    f"on line {result.location.start_line} in {file_name}\n"
+                    f"> \n"
+                    f"> {result.message}\n"
+                )
+
+            if result.snippet:
+                output += f"> ```{result.artifact.language}\n"
+                output += f"{result.snippet}"
+                output += "> ```\n"
 
             if result.fixes:
                 output += f"> Suggested fix: {result.fixes[0].description}\n"
 
             for fix in result.fixes:
                 start_line = fix.deleted_location.start_line
                 start_column = fix.deleted_location.start_column
@@ -85,18 +97,17 @@
             output += "\n"
 
         output += (
             f"| Metric | Value |\n"
             f"| --- | --- |\n"
             f"| Files analyzed | {run.metrics.files:,} |\n"
             f"| Lines analyzed | {run.metrics.lines:,} |\n"
-            f"| Files skipped | {run.metrics.files_skipped:,} |\n"
             f"| Errors | {run.metrics.errors:,} |\n"
             f"| Warnings | {run.metrics.warnings:,} |\n"
             f"| Notes | {run.metrics.notes:,} |\n"
         )
 
-        if self._file.name != sys.stdout.name:
+        if self.console.file.name != sys.stdout.name:
             self.console.print(output, soft_wrap=True)
         else:
             md = markdown.Markdown(output)
             self.console.print(md, soft_wrap=True)
```

### Comparing `precli-0.5.4/precli/renderers/plain.py` & `precli-0.5.5/precli/renderers/plain.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,26 @@
-# Copyright 2024 Secure Saurce LLC
-import sys
-
+# Copyright 2024 Secure Sauce LLC
+from rich.console import Console
 from rich.padding import Padding
 
 from precli.core.level import Level
 from precli.core.run import Run
 from precli.renderers import Renderer
 from precli.rules import Rule
 
 
 class Plain(Renderer):
-    def __init__(self, file: sys.stdout, no_color: bool = False):
-        super().__init__(file=file, no_color=no_color)
+    def __init__(self, console: Console):
+        super().__init__(console)
 
     def render(self, run: Run):
         for result in run.results:
             rule = Rule.get_by_id(result.rule_id)
 
-            if self._no_color is True:
+            if self.console.no_color is True:
                 style = ""
             else:
                 match result.level:
                     case Level.ERROR:
                         style = "red"
 
                     case Level.WARNING:
@@ -31,42 +30,42 @@
                         style = "blue"
 
             if result.artifact.uri is not None:
                 file_name = result.artifact.uri
             else:
                 file_name = result.artifact.file_name
 
-            self.console.print(
-                f"{rule.id}: {rule.cwe.name}",
-            )
+            if rule:
+                self.console.print(f"{rule.id}: {rule.cwe.name}")
+            else:
+                self.console.print(f"{result.rule_id}: Parsing error")
 
             # TODO(ericwb): replace hardcoded <module> with actual scope
             self.console.print(
                 f'  File "{file_name}", line '
                 f"{result.location.start_line}, in <module>",
             )
-            code_lines = result.snippet.splitlines(keepends=True)
-            code_line = code_lines[1] if len(code_lines) > 1 else code_lines[0]
-            underline_width = (
-                result.location.end_column - result.location.start_column
-            )
-            underline = (
-                " " * result.location.start_column + "^" * underline_width
-            )
-            self.console.print(
-                Padding(code_line + underline, (0, 4)),
-            )
+            if result.snippet:
+                lines = result.snippet.splitlines(keepends=True)
+                code_line = lines[1] if len(lines) > 1 else lines[0]
+                underline_width = (
+                    result.location.end_column - result.location.start_column
+                )
+                underline = (
+                    " " * result.location.start_column + "^" * underline_width
+                )
+                self.console.print(
+                    Padding(code_line + underline, (0, 4)),
+                )
             self.console.print(
                 f"{result.level.name.title()}: ",
                 style=style,
                 end="",
             )
-            self.console.print(
-                f"{result.message}",
-            )
+            self.console.print(f"{result.message}")
             self.console.print()
         self.console.print(
             f"Found {run.metrics.errors} errors, {run.metrics.warnings} "
             f"warnings, and {run.metrics.notes} notes in "
             f"{run.metrics.files} files and {run.metrics.lines} lines of "
             f"code."
         )
```

### Comparing `precli-0.5.4/precli/rules/__init__.py` & `precli-0.5.5/precli/rules/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 from abc import ABC
 from typing import Self
 
 from cwe2.database import Database
 from cwe2.weakness import Weakness
 
 from precli.core.config import Config
@@ -41,14 +41,15 @@
         except ValueError:
             start = 0
         self._full_descr = description[start:]
         self._cwe = Rule._cwedb.get(cwe_id)
         self._message = message
         self._wildcards = wildcards
         self._config = Config() if not config else config
+        self._enabled = self._config.enabled
         self._help_url = f"https://docs.securesauce.dev/rules/{id}"
         Rule._rules[id] = self
 
     @property
     def id(self) -> str:
         """
         The ID of the rule.
@@ -58,110 +59,77 @@
         :return: rule ID
         :rtype: str
         """
         return self._id
 
     @staticmethod
     def get_by_id(id: str) -> Self:
-        """
-        Get the rule instance by the given ID.
-
-        :param str id: rule ID
-
-        :return: rule instance
-        :rtype: Rule
-        """
+        """Get the rule instance by the given ID."""
         return Rule._rules.get(id)
 
     @property
     def name(self) -> str:
         """
         Get the rule name.
 
         The rule name is an alpha string corresponding to the CWE name
         but in snake case format.
-
-        :return: rule name
-        :rtype: str
         """
         return self._name
 
     @property
     def short_description(self) -> str:
-        """
-        Short description of the rule.
-
-        :return: rule short description
-        :rtype: str
-        """
+        """Short description of the rule."""
         return self._short_descr
 
     @property
     def full_description(self) -> str:
-        """
-        Full description of the rule in markdown format.
-
-        :return: rule full description
-        :rtype: str
-        """
+        """Full description of the rule in markdown format."""
         return self._full_descr
 
     @property
     def help_url(self) -> str:
-        """
-        URL to help documentation.
-
-        :return: rule help documentation URL
-        :rtype: str
-        """
+        """URL to help documentation."""
         return self._help_url
 
     @property
     def default_config(self) -> Config:
-        """
-        Default configuration for this rule.
-
-        :return: configuration
-        :rtype: Config
-        """
+        """Default configuration for this rule."""
         return self._config
 
     @property
-    def cwe(self) -> Weakness:
-        """
-        CWE weakness object for this rule.
+    def enabled(self) -> bool:
+        """Whether the rule is enabled."""
+        return self._enabled
+
+    @enabled.setter
+    def enabled(self, enabled):
+        """Set whether the rule is enabled"""
+        self._enabled = enabled
 
-        :return: CWE weakness object
-        :rtype: Weakness
-        """
+    @property
+    def cwe(self) -> Weakness:
+        """CWE weakness object for this rule."""
         return self._cwe
 
     @property
     def message(self) -> str:
-        """
-        Concise description message of the found issue.
-
-        :return: issue message
-        :rtype: str
-        """
+        """Concise description message of the found issue."""
         return self._message
 
     @property
     def wildcards(self) -> dict[str, list[str]]:
         """
         Mapping of wildcard imports to concrete modules.
 
         This is necessary when some code has a wildcard import such as:
             from hashlib import *
 
         The * must map to concrete module names in order to fully resolve
         for rule matching.
-
-        :return: mapping of wildcard imports
-        :rtype: dict
         """
         return self._wildcards
 
     @staticmethod
     def get_fixes(
         context: dict,
         deleted_location: Location,
```

### Comparing `precli-0.5.4/precli/rules/go/stdlib/crypto_weak_cipher.py` & `precli-0.5.5/precli/rules/go/stdlib/crypto_weak_cipher.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 r"""
 # Use of a Broken or Risky Cryptographic Algorithm in `crypto` Package
 
 Using weak ciphers for cryptographic algorithms can pose significant security
 risks, and it's generally advised to avoid them in favor of stronger, more
 secure algorithms. Here's some guidance that advises against using weak
 ciphers like DES and RC4:
```

### Comparing `precli-0.5.4/precli/rules/go/stdlib/crypto_weak_hash.py` & `precli-0.5.5/precli/rules/go/stdlib/crypto_weak_hash.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 r"""
 # Reversible One Way Hash in `crypto` Package
 
 The Go `crypto` package provides a number of functions for hashing data.
 However, some of the hash algorithms supported by hashlib are insecure and
 should not be used. These insecure hash algorithms include `MD5` and
 `SHA-1`.
```

### Comparing `precli-0.5.4/precli/rules/go/stdlib/crypto_weak_key.py` & `precli-0.5.5/precli/rules/go/stdlib/crypto_weak_key.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 r"""
 # Inadequate Encryption Strength Using Weak Keys in `crypto` Package
 
 Using weak key sizes for cryptographic algorithms like RSA and DSA can
 compromise the security of your encryption and digital signatures. Here's a
 brief overview of the risks associated with weak key sizes for these
 algorithms:
```

### Comparing `precli-0.5.4/precli/rules/java/stdlib/java_net_insecure_cookie.py` & `precli-0.5.5/precli/rules/java/stdlib/java_net_insecure_cookie.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 r"""
 # Sensitive Cookie in HTTPS Session Without 'Secure' Attribute
 
 This rule identifies and flags any instance where cookies in Java web
 applications are created or set without the Secure flag. The absence of this
 flag allows the cookie to be transmitted over non-HTTPS connections, which
 poses a risk of interception by an attacker, especially through
```

### Comparing `precli-0.5.4/precli/rules/java/stdlib/java_security_weak_hash.py` & `precli-0.5.5/precli/rules/java/stdlib/java_security_weak_hash.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 r"""
 # Reversible One Way Hash in `java.security` Package
 
 The Java `MessageDigest` class provides a number of options for algorithms
 to hash data. However, some of the hash algorithms are insecure and should
 not be used. These insecure hash algorithms include `MD5` and `SHA-1`.
```

### Comparing `precli-0.5.4/precli/rules/java/stdlib/java_security_weak_key.py` & `precli-0.5.5/precli/rules/java/stdlib/java_security_weak_key.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 r"""
 # Inadequate Encryption Strength Using Weak Keys in `java.security` Package
 
 Using weak key sizes for cryptographic algorithms like RSA and DSA can
 compromise the security of your encryption and digital signatures. Here's a
 brief overview of the risks associated with weak key sizes for these
 algorithms:
```

### Comparing `precli-0.5.4/precli/rules/java/stdlib/java_security_weak_random.py` & `precli-0.5.5/precli/rules/java/stdlib/java_security_weak_random.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 r"""
 # Use of Cryptographically Weak Pseudo-Random Number Generator `SHA1PRNG`
 
 This rule identifies instances where the Java SecureRandom class is
 instantiated with the SHA1PRNG algorithm. While SHA1PRNG has been widely
 used, it is considered less secure and potentially vulnerable compared to
 newer algorithms available. The use of stronger algorithms is recommended
```

### Comparing `precli-0.5.4/precli/rules/java/stdlib/javax_crypto_weak_cipher.py` & `precli-0.5.5/precli/rules/java/stdlib/javax_crypto_weak_cipher.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 r"""
 # Use of a Broken or Risky Cryptographic Algorithm in `javax.crypto` Package
 
 Using weak ciphers for cryptographic algorithms can pose significant security
 risks, and it's generally advised to avoid them in favor of stronger, more
 secure algorithms. Here's some guidance that advises against using weak
 ciphers like 3DES, Blowfish, DES, RC2, RC4, and RC5:
```

### Comparing `precli-0.5.4/precli/rules/java/stdlib/javax_servlet_http_insecure_cookie.py` & `precli-0.5.5/precli/rules/java/stdlib/javax_servlet_http_insecure_cookie.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 r"""
 # Sensitive Cookie in HTTPS Session Without 'Secure' Attribute
 
 This rule identifies and flags any instance where cookies in Java web
 applications are created or set without the Secure flag. The absence of this
 flag allows the cookie to be transmitted over non-HTTPS connections, which
 poses a risk of interception by an attacker, especially through
```

### Comparing `precli-0.5.4/precli/rules/python/stdlib/argparse_sensitive_info.py` & `precli-0.5.5/precli/rules/python/stdlib/argparse_sensitive_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 r"""
 # Invocation of Process Using Visible Sensitive Information in `argparse`
 
 Do not read secrets directly from command line arguments. When a command
 accepts a secret like via a `--password` argument or `--api-key`, the argument
 value will leak the secret into ps output and shell history. This also
 encourages the use of insecure environment variables for secrets.
```

### Comparing `precli-0.5.4/precli/rules/python/stdlib/assert.py` & `precli-0.5.5/precli/rules/python/stdlib/assert.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 r"""
 # Improper Check Using `assert` Function
 
 Assertions are typically used during the development phase to catch logic
 errors and conditions that should never occur. However, relying on assertions
 for security checks or other critical runtime validations is not recommended
 because:
```

### Comparing `precli-0.5.4/precli/rules/python/stdlib/crypt_weak_hash.py` & `precli-0.5.5/precli/rules/python/stdlib/crypt_weak_hash.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 r"""
 # Reversible One Way Hash in `crypt` Module
 
 The Python module `crypt` provides a number of functions for password
 hashing. However, some of the hashing functions supported by `crypt` are weak
 and should not be used. These weak hashing functions include `CRYPT` and
 `MD5`.
```

### Comparing `precli-0.5.4/precli/rules/python/stdlib/ftplib_cleartext.py` & `precli-0.5.5/precli/rules/python/stdlib/ftplib_cleartext.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 r"""
 # Cleartext Transmission of Sensitive Information in the `ftplib` Module
 
 The Python module `ftplib` provides a number of functions for accessing FTP
 servers. However, the module does not provide any security features. This
 means that data transmitted over the network, including passwords, is sent
 in cleartext. This makes it possible for attackers to intercept and read
```

### Comparing `precli-0.5.4/precli/rules/python/stdlib/ftplib_unverified_context.py` & `precli-0.5.5/precli/rules/python/stdlib/ftplib_unverified_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 r"""
 # Improper Certificate Validation Using `ftplib`
 
 The Python class `ftplib.FTP_TLS` by default creates an SSL context that does
 not verify the server's certificate if the context parameter is unset or has
 a value of None. This means that an attacker can easily impersonate a
 legitimate server and fool your application into connecting to it.
```

### Comparing `precli-0.5.4/precli/rules/python/stdlib/hashlib_improper_prng.py` & `precli-0.5.5/precli/rules/python/stdlib/hashlib_improper_prng.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 r"""
 # Improper Randomness for Cryptographic `hashlib` Functions
 
 This rule detects the use of non-cryptographically secure randomness sources,
 such as Python's `random()` function, as inputs to cryptographic functions
 like `hashlib.scrypt()`. Using non-secure randomness sources can weaken the
 cryptographic strength of functions that rely on unpredictability for security.
```

### Comparing `precli-0.5.4/precli/rules/python/stdlib/hashlib_weak_hash.py` & `precli-0.5.5/precli/rules/python/stdlib/hashlib_weak_hash.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 r"""
 # Reversible One Way Hash in `hashlib` Module
 
 The Python module `hashlib` provides a number of functions for hashing data.
 However, some of the hash algorithms supported by hashlib are insecure and
 should not be used. These insecure hash algorithms include `MD4`, `MD5`,
 `RIPEMD-160` and `SHA-1`.
```

### Comparing `precli-0.5.4/precli/rules/python/stdlib/hmac_timing_attack.py` & `precli-0.5.5/precli/rules/python/stdlib/hmac_timing_attack.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 r"""
 Observable Timing Discrepancy in `hmac` Module
 
 Do not use Python's == operator to compare HMAC digests. The == operator is
 not designed to be used for cryptographic comparisons, and it can be
 vulnerable to timing attacks. Instead, use the `hmac.compare_digest()` function
 to compare HMAC digests.
```

### Comparing `precli-0.5.4/precli/rules/python/stdlib/hmac_weak_hash.py` & `precli-0.5.5/precli/rules/python/stdlib/hmac_weak_hash.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 r"""
 # Reversible One Way Hash in `hmac` Module
 
 The Python module `hmac` provides a number of functions for creating and
 verifying message authentication codes (MACs). However, some of the hash
 algorithms supported by hmac are insecure and should not be used. These
 insecure hash algorithms include `MD4`, `MD5`, `RIPEMD-160` and `SHA-1`.
```

### Comparing `precli-0.5.4/precli/rules/python/stdlib/hmac_weak_key.py` & `precli-0.5.5/precli/rules/python/stdlib/hmac_weak_key.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 r"""
 # Insufficient `hmac` Key Size
 
 This rule identifies instances where the key provided to `hmac.digest()` or
 `hmac.new()` is considered too small relative to the digest algorithm's
 digest size. Using keys that are too short can compromise the integrity and
 security of the HMAC (Hash-based Message Authentication Code), making it less
```

### Comparing `precli-0.5.4/precli/rules/python/stdlib/http_server_unrestricted_bind.py` & `precli-0.5.5/precli/rules/python/stdlib/http_server_unrestricted_bind.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 r"""
 # Binding to an Unrestricted IP Address in `http.server` Module
 
 Sockets can be bound to the IPv4 address `0.0.0.0` or IPv6 equivalent of
 `::`, which configures the socket to listen for incoming connections on all
 network interfaces. While this can be intended in environments where
 services are meant to be publicly accessible, it can also introduce significant
```

### Comparing `precli-0.5.4/precli/rules/python/stdlib/http_url_secret.py` & `precli-0.5.5/precli/rules/python/stdlib/http_url_secret.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 r"""
 # Use of HTTP Request Method With Sensitive Query Strings
 
 The inclusion of sensitive information, such as a username, password, or API
 key, directly within a URL is considered a security risk because URLs can be
 logged in various places, such as web server logs, browser history, and network
 monitoring tools, making the sensitive information vulnerable to unauthorized
```

### Comparing `precli-0.5.4/precli/rules/python/stdlib/imaplib_cleartext.py` & `precli-0.5.5/precli/rules/python/stdlib/imaplib_cleartext.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 r"""
 # Cleartext Transmission of Sensitive Information in the `imaplib` Module
 
 The Python module `imaplib` provides a number of functions for accessing
 IMAP servers. However, the default behavior of the module does not provide
 utilize secure connections. This means that data transmitted over the network,
 including passwords, is sent in cleartext. This makes it possible for attackers
```

### Comparing `precli-0.5.4/precli/rules/python/stdlib/imaplib_unverified_context.py` & `precli-0.5.5/precli/rules/python/stdlib/imaplib_unverified_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 r"""
 # Improper Certificate Validation Using `imaplib`
 
 The Python class `imaplib.IMAP4_SSL` by default creates an SSL context that
 does not verify the server's certificate if the context parameter is unset or
 has a value of None. This means that an attacker can easily impersonate a
 legitimate server and fool your application into connecting to it.
```

### Comparing `precli-0.5.4/precli/rules/python/stdlib/json_load.py` & `precli-0.5.5/precli/rules/python/stdlib/json_load.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 r"""
 # Deserialization of Untrusted Data in the `json` Module
 
 The Python `json` module provides a way to parse and generate JSON data.
 However, it is important to be aware that malicious JSON strings can be used
 to attack applications that use the json module. For example, a malicious
 JSON string could be used to cause the decoder to consume considerable CPU
```

### Comparing `precli-0.5.4/precli/rules/python/stdlib/logging_insecure_listen_config.py` & `precli-0.5.5/precli/rules/python/stdlib/logging_insecure_listen_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 r"""
 # Code Injection in Logging Config
 
 The `logging.config.listen()` function allows you to dynamically change the
 logging configuration of your application. However, if you set the verify
 argument to False, you are opening yourself up to a security vulnerability.
 This is because anyone who can connect to the listening socket can send
```

### Comparing `precli-0.5.4/precli/rules/python/stdlib/marshal_load.py` & `precli-0.5.5/precli/rules/python/stdlib/marshal_load.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 r"""
 # Deserialization of Untrusted Data in the `marshal` Module
 
 The Python `marshal` module provides a way to serialize and deserialize
 Python objects. However, it is important to be aware that malicious data
 can be used to attack applications that use the marshal module. For example,
 a malicious data could be used to cause the decoder to execute arbitrary code.
```

### Comparing `precli-0.5.4/precli/rules/python/stdlib/nntplib_cleartext.py` & `precli-0.5.5/precli/rules/python/stdlib/nntplib_cleartext.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 r"""
 # Cleartext Transmission of Sensitive Information in the `nntplib` Module
 
 The Python module `nntplib` provides a number of functions for accessing
 NNTP servers. However, the default behavior of the module does not provide
 utilize secure connections. This means that data transmitted over the network,
 including passwords, is sent in cleartext. This makes it possible for attackers
```

### Comparing `precli-0.5.4/precli/rules/python/stdlib/nntplib_unverified_context.py` & `precli-0.5.5/precli/rules/python/stdlib/nntplib_unverified_context.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 r"""
 # Improper Certificate Validation Using `nntplib`
 
 The Python class `nntplib.NNTP_SSL` by default creates an SSL context that
 does not verify the server's certificate if the context parameter is unset or
 has a value of None. This means that an attacker can easily impersonate a
 legitimate server and fool your application into connecting to it.
```

### Comparing `precli-0.5.4/precli/rules/python/stdlib/pickle_load.py` & `precli-0.5.5/precli/rules/python/stdlib/pickle_load.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 r"""
 # Deserialization of Untrusted Data in `pickle` Module
 
 The Python `pickle` module is a serialization module that can be used to
 serialize and deserialize Python objects. However, pickle is not a secure
 serialization format and should not be used to serialize sensitive data.
```

### Comparing `precli-0.5.4/precli/rules/python/stdlib/poplib_cleartext.py` & `precli-0.5.5/precli/rules/python/stdlib/poplib_cleartext.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 r"""
 # Cleartext Transmission of Sensitive Information in the `poplib` Module
 
 The Python module `poplib` provides a number of functions for accessing
 POP servers. However, the default behavior of the module does not provide
 utilize secure connections. This means that data transmitted over the network,
 including passwords, is sent in cleartext. This makes it possible for attackers
```

### Comparing `precli-0.5.4/precli/rules/python/stdlib/poplib_unverified_context.py` & `precli-0.5.5/precli/rules/python/stdlib/poplib_unverified_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 r"""
 # Improper Certificate Validation Using `poplib`
 
 The Python class `poplib.POP3_SSL` by default creates an SSL context that
 does not verify the server's certificate if the context parameter is unset or
 has a value of None. This means that an attacker can easily impersonate a
 legitimate server and fool your application into connecting to it.
```

### Comparing `precli-0.5.4/precli/rules/python/stdlib/re_denial_of_service.py` & `precli-0.5.5/precli/rules/python/stdlib/re_denial_of_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 r"""
 # Inefficient Regular Expression Complexity in `re` Module
 
 Patterns in Python's re module that are susceptible to catastrophic
 backtracking. Such patterns can lead to performance issues and may cause
 a Denial-of-Service (DoS) condition in applications by consuming an
 excessive amount of CPU time on certain inputs Vulnerability Explanation
```

### Comparing `precli-0.5.4/precli/rules/python/stdlib/secrets_weak_token.py` & `precli-0.5.5/precli/rules/python/stdlib/secrets_weak_token.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 r"""
 # Insufficient Token Length
 
 Tokens are often used as security-critical elements, such as for
 authentication, session management, or as part of cryptographic operations.
 The strength of a token is significantly influenced by its length and the
 randomness of its generation. Tokens with insufficient byte lengths lack
@@ -68,15 +68,15 @@
             "secrets.token_bytes",
             "secrets.token_hex",
             "secrets.token_urlsafe",
         ]:
             return
 
         arg = call.get_argument(position=0, name="nbytes")
-        nbytes = int(arg.value) if arg.value else 32
+        nbytes = int(arg.value) if isinstance(arg.value, int) else 32
 
         if nbytes < 32:
             fixes = Rule.get_fixes(
                 context=context,
                 deleted_location=Location(node=arg.node),
                 description="Pass None or no parameter to use the default "
                 "entropy.",
```

### Comparing `precli-0.5.4/precli/rules/python/stdlib/shelve_open.py` & `precli-0.5.5/precli/rules/python/stdlib/shelve_open.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 r"""
 # Deserialization of Untrusted Data in the `shelve` Module
 
 The Python `shelve` module provides a way to store Python objects in a file.
 It is backed by the pickle module, which is a serialization format that can
 be used to store arbitrary Python objects.
```

### Comparing `precli-0.5.4/precli/rules/python/stdlib/smtplib_cleartext.py` & `precli-0.5.5/precli/rules/python/stdlib/smtplib_cleartext.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 r"""
 # Cleartext Transmission of Sensitive Information in the `smtplib` Module
 
 The Python module `smtplib` provides a number of functions for accessing
 SMTP servers. However, the default behavior of the module does not provide
 utilize secure connections. This means that data transmitted over the network,
 including passwords, is sent in cleartext. This makes it possible for attackers
```

### Comparing `precli-0.5.4/precli/rules/python/stdlib/smtplib_unverified_context.py` & `precli-0.5.5/precli/rules/python/stdlib/smtplib_unverified_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 r"""
 # Improper Certificate Validation Using `smtplib`
 
 The Python class `smtplib.SMTP_SSL` by default creates an SSL context that
 does not verify the server's certificate if the context parameter is unset or
 has a value of None. This means that an attacker can easily impersonate a
 legitimate server and fool your application into connecting to it.
```

### Comparing `precli-0.5.4/precli/rules/python/stdlib/socket_unrestricted_bind.py` & `precli-0.5.5/precli/rules/python/stdlib/socket_unrestricted_bind.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 r"""
 # Binding to an Unrestricted IP Address in `socket` Module
 
 Sockets can be bound to the IPv4 address `0.0.0.0` or IPv6 equivalent of
 `::`, which configures the socket to listen for incoming connections on all
 network interfaces. While this can be intended in environments where
 services are meant to be publicly accessible, it can also introduce significant
```

### Comparing `precli-0.5.4/precli/rules/python/stdlib/socketserver_unrestricted_bind.py` & `precli-0.5.5/precli/rules/python/stdlib/socketserver_unrestricted_bind.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 r"""
 # Binding to an Unrestricted IP Address in `socketserver` Module
 
 Sockets can be bound to the IPv4 address `0.0.0.0` or IPv6 equivalent of
 `::`, which configures the socket to listen for incoming connections on all
 network interfaces. While this can be intended in environments where
 services are meant to be publicly accessible, it can also introduce significant
```

### Comparing `precli-0.5.4/precli/rules/python/stdlib/ssl_context_weak_key.py` & `precli-0.5.5/precli/rules/python/stdlib/ssl_context_weak_key.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 r"""
 # Inadequate Encryption Strength Using Weak Keys in SSLContext
 
 Using weak key sizes for cryptographic algorithms like Elliptic Curve can
 compromise the security of your encryption and digital signatures. Here's
 a brief overview of the risks associated with weak key sizes for this
 algorithm:
```

### Comparing `precli-0.5.4/precli/rules/python/stdlib/ssl_create_unverified_context.py` & `precli-0.5.5/precli/rules/python/stdlib/ssl_create_unverified_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 r"""
 # Improper Certificate Validation Using `ssl._create_unverified_context`
 
 The Python function `ssl._create_unverified_context()` creates a SSL context
 that does not verify the server's certificate. This means that an attacker can
 easily impersonate a legitimate server and fool your application into
 connecting to it.
```

### Comparing `precli-0.5.4/precli/rules/python/stdlib/ssl_insecure_tls_version.py` & `precli-0.5.5/precli/rules/python/stdlib/ssl_insecure_tls_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 r"""
 # Inadequate Encryption Strength Using Weak SSL Protocols
 
 The Python `ssl` modules provide a number of different protocols that can be
 used to encrypt data. However, some of these protocols are no longer
 considered secure and should not be used.
```

### Comparing `precli-0.5.4/precli/rules/python/stdlib/telnetlib_cleartext.py` & `precli-0.5.5/precli/rules/python/stdlib/telnetlib_cleartext.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 r"""
 # Cleartext Transmission of Sensitive Information in the `telnetlib` Module
 
 The Python module `telnetlib` is a low-level module that provides access to
 the telnet protocol. The telnet protocol is a cleartext protocol, which means
 that all data transmitted over the connection is visible to anyone who can
 sniff the network traffic. This includes passwords, usernames, and other
```

### Comparing `precli-0.5.4/precli/rules/python/stdlib/tempfile_mktemp_race_condition.py` & `precli-0.5.5/precli/rules/python/stdlib/tempfile_mktemp_race_condition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 r"""
 # Insecure Temporary File in the `tempfile` Module
 
 The `tempfile.mktemp` function in Python is a legacy method for creating
 temporary files with a unique name. It is important to note that this function
 is susceptible to race conditions, which can occur when multiple processes or
 threads attempt to create temporary files concurrently. These race conditions
```

### Comparing `precli-0.5.4/precli/rules/python/stdlib/xmlrpc_server_unrestricted_bind.py` & `precli-0.5.5/precli/rules/python/stdlib/xmlrpc_server_unrestricted_bind.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 r"""
 # Binding to an Unrestricted IP Address in `xmlrpc.server` Module
 
 Sockets can be bound to the IPv4 address `0.0.0.0` or IPv6 equivalent of
 `::`, which configures the socket to listen for incoming connections on all
 network interfaces. While this can be intended in environments where
 services are meant to be publicly accessible, it can also introduce significant
```

### Comparing `precli-0.5.4/precli.egg-info/PKG-INFO` & `precli-0.5.5/precli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: precli
-Version: 0.5.4
+Version: 0.5.5
 Summary: Static analysis security tool command line
 Home-page: https://github.com/securesauce/precli
 Download-URL: https://pypi.org/project/precli/#files
 Author: Secure Sauce
 Project-URL: Release notes, https://github.com/securesauce/precli/releases
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -16,20 +16,20 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Security
 Requires-Python: >=3.12
 License-File: LICENSE
 Requires-Dist: cwe2==2.0.0
-Requires-Dist: Pygments==2.17.2
+Requires-Dist: Pygments==2.18.0
 Requires-Dist: rich==13.7.1
 Requires-Dist: tree-sitter==0.21.3
 Requires-Dist: tree-sitter-languages==1.10.2
 Requires-Dist: ignorelib==0.3.0
-Requires-Dist: requests==2.31.0
+Requires-Dist: requests==2.32.2
 Requires-Dist: sarif-om==1.0.4
 Requires-Dist: jschema-to-python==1.2.3
 Requires-Dist: outdated==0.2.2
 
 .. image:: https://raw.githubusercontent.com/securesauce/precli/main/logo/logo.png
     :alt: Precaution CLI
```

### Comparing `precli-0.5.4/precli.egg-info/SOURCES.txt` & `precli-0.5.5/precli.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 .pre-commit-config.yaml
 .readthedocs.yaml
-.stestr.conf
 AUTHORS
 CODE_OF_CONDUCT.md
 ChangeLog
 LICENSE
 README.rst
 SECURITY.md
 mkdocs.yml
@@ -161,26 +160,27 @@
 precli/rules/python/stdlib/socketserver_unrestricted_bind.py
 precli/rules/python/stdlib/ssl_context_weak_key.py
 precli/rules/python/stdlib/ssl_create_unverified_context.py
 precli/rules/python/stdlib/ssl_insecure_tls_version.py
 precli/rules/python/stdlib/telnetlib_cleartext.py
 precli/rules/python/stdlib/tempfile_mktemp_race_condition.py
 precli/rules/python/stdlib/xmlrpc_server_unrestricted_bind.py
-scripts/main.py
 tests/__init__.py
 tests/unit/__init__.py
 tests/unit/cli/__init__.py
 tests/unit/core/__init__.py
 tests/unit/core/test_python.py
 tests/unit/parsers/__init__.py
 tests/unit/parsers/test_go.py
 tests/unit/parsers/test_python.py
+tests/unit/parsers/examples/bad_coding.py
 tests/unit/parsers/examples/expression_list_assignment.py
 tests/unit/parsers/examples/expression_list_assignment_uneven.py
 tests/unit/parsers/examples/importlib_import_module.py
+tests/unit/parsers/examples/pep3120.py
 tests/unit/parsers/examples/suppress.go
 tests/unit/parsers/examples/suppress.py
 tests/unit/parsers/examples/suppress_lowercase_rule.go
 tests/unit/parsers/examples/suppress_lowercase_rule.py
 tests/unit/parsers/examples/suppress_multiline.go
 tests/unit/parsers/examples/suppress_multiline.py
 tests/unit/parsers/examples/suppress_multiple_comments.go
@@ -541,14 +541,15 @@
 tests/unit/rules/python/stdlib/re/examples/re_subn.py
 tests/unit/rules/python/stdlib/secrets/__init__.py
 tests/unit/rules/python/stdlib/secrets/test_secrets_weak_token.py
 tests/unit/rules/python/stdlib/secrets/examples/secrets_token_bytes.py
 tests/unit/rules/python/stdlib/secrets/examples/secrets_token_bytes_default.py
 tests/unit/rules/python/stdlib/secrets/examples/secrets_token_bytes_size_var.py
 tests/unit/rules/python/stdlib/secrets/examples/secrets_token_hex.py
+tests/unit/rules/python/stdlib/secrets/examples/secrets_token_hex_nbytes_unknown.py
 tests/unit/rules/python/stdlib/secrets/examples/secrets_token_urlsafe.py
 tests/unit/rules/python/stdlib/shelve/__init__.py
 tests/unit/rules/python/stdlib/shelve/test_shelve_open.py
 tests/unit/rules/python/stdlib/shelve/examples/shelve_dbfilenameshelf.py
 tests/unit/rules/python/stdlib/shelve/examples/shelve_open.py
 tests/unit/rules/python/stdlib/shelve/examples/shelve_open_context_mgr.py
 tests/unit/rules/python/stdlib/smtplib/__init__.py
```

### Comparing `precli-0.5.4/precli.egg-info/entry_points.txt` & `precli-0.5.5/precli.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `precli-0.5.4/pylintrc` & `precli-0.5.5/pylintrc`

 * *Files identical despite different names*

### Comparing `precli-0.5.4/setup.cfg` & `precli-0.5.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `precli-0.5.4/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_cipher_rc4.go` & `precli-0.5.5/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_cipher_rc4.go`

 * *Files identical despite different names*

### Comparing `precli-0.5.4/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_dsa_1024.go` & `precli-0.5.5/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_dsa_1024.go`

 * *Files identical despite different names*

### Comparing `precli-0.5.4/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_dsa_2048.go` & `precli-0.5.5/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_dsa_2048.go`

 * *Files identical despite different names*

### Comparing `precli-0.5.4/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_dsa_3072.go` & `precli-0.5.5/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_dsa_3072.go`

 * *Files identical despite different names*

### Comparing `precli-0.5.4/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_1024.go` & `precli-0.5.5/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_1024.go`

 * *Files identical despite different names*

### Comparing `precli-0.5.4/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_2048.go` & `precli-0.5.5/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_2048.go`

 * *Files identical despite different names*

### Comparing `precli-0.5.4/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_4096.go` & `precli-0.5.5/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_4096.go`

 * *Files identical despite different names*

### Comparing `precli-0.5.4/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_bits_as_var.go` & `precli-0.5.5/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_bits_as_var.go`

 * *Files identical despite different names*

### Comparing `precli-0.5.4/tests/unit/rules/go/stdlib/crypto/test_crypto_weak_cipher.py` & `precli-0.5.5/tests/unit/rules/java/stdlib/java_net/test_insecure_cookie.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,48 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 import os
 
-from parameterized import parameterized
+import pytest
 
 from precli.core.level import Level
-from precli.parsers import go
+from precli.parsers import java
 from precli.rules import Rule
 from tests.unit.rules import test_case
 
 
-class CryptoWeakCipherTests(test_case.TestCase):
-    def setUp(self):
-        super().setUp()
-        self.rule_id = "GO001"
-        self.parser = go.Go()
-        self.base_path = os.path.join(
+class TestInsecureCookie(test_case.TestCase):
+    @classmethod
+    def setup_class(cls):
+        cls.rule_id = "JAV006"
+        cls.parser = java.Java()
+        cls.base_path = os.path.join(
             "tests",
             "unit",
             "rules",
-            "go",
+            "java",
             "stdlib",
-            "crypto",
+            "java_net",
             "examples",
         )
 
     def test_rule_meta(self):
         rule = Rule.get_by_id(self.rule_id)
-        self.assertEqual(self.rule_id, rule.id)
-        self.assertEqual(
-            "use_of_a_broken_or_risky_cryptographic_algorithm", rule.name
+        assert rule.id == self.rule_id
+        assert rule.name == "insecure_cookie"
+        assert (
+            rule.help_url
+            == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
-        self.assertEqual(
-            f"https://docs.securesauce.dev/rules/{self.rule_id}", rule.help_url
-        )
-        self.assertEqual(True, rule.default_config.enabled)
-        self.assertEqual(Level.ERROR, rule.default_config.level)
-        self.assertEqual(-1.0, rule.default_config.rank)
-        self.assertEqual("327", rule.cwe.cwe_id)
+        assert rule.default_config.enabled is True
+        assert rule.default_config.level == Level.WARNING
+        assert rule.default_config.rank == -1.0
+        assert rule.cwe.cwe_id == "614"
 
-    @parameterized.expand(
+    @pytest.mark.parametrize(
+        "filename",
         [
-            "crypto_weak_cipher_aes.go",
-            "crypto_weak_cipher_des.go",
-            "crypto_weak_cipher_rc4.go",
-        ]
+            "HttpCookieSecureFalse.java",
+            "HttpCookieSecureTrue.java",
+        ],
     )
     def test(self, filename):
         self.check(filename)
```

### Comparing `precli-0.5.4/tests/unit/rules/go/stdlib/crypto/test_crypto_weak_hash.py` & `precli-0.5.5/tests/unit/rules/go/stdlib/crypto/test_crypto_weak_hash.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,50 +1,52 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 import os
 
-from parameterized import parameterized
+import pytest
 
 from precli.core.level import Level
 from precli.parsers import go
 from precli.rules import Rule
 from tests.unit.rules import test_case
 
 
-class CryptoWeakHashTests(test_case.TestCase):
-    def setUp(self):
-        super().setUp()
-        self.rule_id = "GO002"
-        self.parser = go.Go()
-        self.base_path = os.path.join(
+class TestCryptoWeakHash(test_case.TestCase):
+    @classmethod
+    def setup_class(cls):
+        cls.rule_id = "GO002"
+        cls.parser = go.Go()
+        cls.base_path = os.path.join(
             "tests",
             "unit",
             "rules",
             "go",
             "stdlib",
             "crypto",
             "examples",
         )
 
     def test_rule_meta(self):
         rule = Rule.get_by_id(self.rule_id)
-        self.assertEqual(self.rule_id, rule.id)
-        self.assertEqual("reversible_one_way_hash", rule.name)
-        self.assertEqual(
-            f"https://docs.securesauce.dev/rules/{self.rule_id}", rule.help_url
+        assert rule.id == self.rule_id
+        assert rule.name == "reversible_one_way_hash"
+        assert (
+            rule.help_url
+            == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
-        self.assertEqual(True, rule.default_config.enabled)
-        self.assertEqual(Level.ERROR, rule.default_config.level)
-        self.assertEqual(-1.0, rule.default_config.rank)
-        self.assertEqual("328", rule.cwe.cwe_id)
+        assert rule.default_config.enabled is True
+        assert rule.default_config.level == Level.ERROR
+        assert rule.default_config.rank == -1.0
+        assert rule.cwe.cwe_id == "328"
 
-    @parameterized.expand(
+    @pytest.mark.parametrize(
+        "filename",
         [
             "crypto_weak_hash_md5_new.go",
             "crypto_weak_hash_md5_sum.go",
             "crypto_weak_hash_sha1_new.go",
             "crypto_weak_hash_sha1_sum.go",
             "crypto_weak_hash_sha256_new.go",
             "crypto_weak_hash_sha256_sum.go",
-        ]
+        ],
     )
     def test(self, filename):
         self.check(filename)
```

### Comparing `precli-0.5.4/tests/unit/rules/go/stdlib/crypto/test_crypto_weak_key.py` & `precli-0.5.5/tests/unit/rules/go/stdlib/crypto/test_crypto_weak_key.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,53 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 import os
 
-from parameterized import parameterized
+import pytest
 
 from precli.core.level import Level
 from precli.parsers import go
 from precli.rules import Rule
 from tests.unit.rules import test_case
 
 
-class CryptoWeakKeyTests(test_case.TestCase):
-    def setUp(self):
-        super().setUp()
-        self.rule_id = "GO003"
-        self.parser = go.Go()
-        self.base_path = os.path.join(
+class TestCryptoWeakKey(test_case.TestCase):
+    @classmethod
+    def setup_class(cls):
+        cls.rule_id = "GO003"
+        cls.parser = go.Go()
+        cls.base_path = os.path.join(
             "tests",
             "unit",
             "rules",
             "go",
             "stdlib",
             "crypto",
             "examples",
         )
 
     def test_rule_meta(self):
         rule = Rule.get_by_id(self.rule_id)
-        self.assertEqual(self.rule_id, rule.id)
-        self.assertEqual("inadequate_encryption_strength", rule.name)
-        self.assertEqual(
-            f"https://docs.securesauce.dev/rules/{self.rule_id}", rule.help_url
+        assert rule.id == self.rule_id
+        assert rule.name == "inadequate_encryption_strength"
+        assert (
+            rule.help_url
+            == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
-        self.assertEqual(True, rule.default_config.enabled)
-        self.assertEqual(Level.WARNING, rule.default_config.level)
-        self.assertEqual(-1.0, rule.default_config.rank)
-        self.assertEqual("326", rule.cwe.cwe_id)
+        assert rule.default_config.enabled is True
+        assert rule.default_config.level == Level.WARNING
+        assert rule.default_config.rank == -1.0
+        assert rule.cwe.cwe_id == "326"
 
-    @parameterized.expand(
+    @pytest.mark.parametrize(
+        "filename",
         [
             "crypto_weak_key_dsa_1024.go",
             "crypto_weak_key_dsa_2048.go",
             "crypto_weak_key_dsa_3072.go",
             "crypto_weak_key_rsa_1024.go",
             "crypto_weak_key_rsa_2048.go",
             "crypto_weak_key_rsa_4096.go",
             "crypto_weak_key_rsa_bits_as_var.go",
-        ]
+        ],
     )
     def test(self, filename):
         self.check(filename)
```

### Comparing `precli-0.5.4/tests/unit/rules/java/stdlib/java_net/test_insecure_cookie.py` & `precli-0.5.5/tests/unit/rules/python/stdlib/assert/test_assert.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,47 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 import os
 
-from parameterized import parameterized
+import pytest
 
 from precli.core.level import Level
-from precli.parsers import java
+from precli.parsers import python
 from precli.rules import Rule
 from tests.unit.rules import test_case
 
 
-class InsecureCookieTests(test_case.TestCase):
-    def setUp(self):
-        super().setUp()
-        self.rule_id = "JAV006"
-        self.parser = java.Java()
-        self.base_path = os.path.join(
+class TestAssert(test_case.TestCase):
+    @classmethod
+    def setup_class(cls):
+        cls.rule_id = "PY001"
+        cls.parser = python.Python()
+        cls.base_path = os.path.join(
             "tests",
             "unit",
             "rules",
-            "java",
+            "python",
             "stdlib",
-            "java_net",
+            "assert",
             "examples",
         )
 
     def test_rule_meta(self):
         rule = Rule.get_by_id(self.rule_id)
-        self.assertEqual(self.rule_id, rule.id)
-        self.assertEqual("insecure_cookie", rule.name)
-        self.assertEqual(
-            f"https://docs.securesauce.dev/rules/{self.rule_id}", rule.help_url
+        assert rule.id == self.rule_id
+        assert rule.name == "improper_check"
+        assert (
+            rule.help_url
+            == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
-        self.assertEqual(True, rule.default_config.enabled)
-        self.assertEqual(Level.WARNING, rule.default_config.level)
-        self.assertEqual(-1.0, rule.default_config.rank)
-        self.assertEqual("614", rule.cwe.cwe_id)
+        assert rule.default_config.enabled is True
+        assert rule.default_config.level == Level.WARNING
+        assert rule.default_config.rank == -1.0
+        assert rule.cwe.cwe_id == "703"
 
-    @parameterized.expand(
+    @pytest.mark.parametrize(
+        "filename",
         [
-            "HttpCookieSecureFalse.java",
-            "HttpCookieSecureTrue.java",
-        ]
+            "assert.py",
+        ],
     )
     def test(self, filename):
         self.check(filename)
```

### Comparing `precli-0.5.4/tests/unit/rules/java/stdlib/java_security/examples/KeyPairGeneratorDSA.java` & `precli-0.5.5/tests/unit/rules/java/stdlib/java_security/examples/KeyPairGeneratorDSA.java`

 * *Files identical despite different names*

### Comparing `precli-0.5.4/tests/unit/rules/java/stdlib/java_security/examples/KeyPairGeneratorRSA.java` & `precli-0.5.5/tests/unit/rules/java/stdlib/java_security/examples/KeyPairGeneratorRSA.java`

 * *Files identical despite different names*

### Comparing `precli-0.5.4/tests/unit/rules/java/stdlib/java_security/examples/MessageDigestMD5Property.java` & `precli-0.5.5/tests/unit/rules/java/stdlib/java_security/examples/MessageDigestMD5Property.java`

 * *Files identical despite different names*

### Comparing `precli-0.5.4/tests/unit/rules/java/stdlib/java_security/test_weak_hash.py` & `precli-0.5.5/tests/unit/rules/java/stdlib/java_security/test_weak_hash.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,49 +1,51 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 import os
 
-from parameterized import parameterized
+import pytest
 
 from precli.core.level import Level
 from precli.parsers import java
 from precli.rules import Rule
 from tests.unit.rules import test_case
 
 
-class MessageDigestWeakHashTests(test_case.TestCase):
-    def setUp(self):
-        super().setUp()
-        self.rule_id = "JAV002"
-        self.parser = java.Java()
-        self.base_path = os.path.join(
+class TestMessageDigestWeakHash(test_case.TestCase):
+    @classmethod
+    def setup_class(cls):
+        cls.rule_id = "JAV002"
+        cls.parser = java.Java()
+        cls.base_path = os.path.join(
             "tests",
             "unit",
             "rules",
             "java",
             "stdlib",
             "java_security",
             "examples",
         )
 
     def test_rule_meta(self):
         rule = Rule.get_by_id(self.rule_id)
-        self.assertEqual(self.rule_id, rule.id)
-        self.assertEqual("reversible_one_way_hash", rule.name)
-        self.assertEqual(
-            f"https://docs.securesauce.dev/rules/{self.rule_id}", rule.help_url
+        assert rule.id == self.rule_id
+        assert rule.name == "reversible_one_way_hash"
+        assert (
+            rule.help_url
+            == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
-        self.assertEqual(True, rule.default_config.enabled)
-        self.assertEqual(Level.ERROR, rule.default_config.level)
-        self.assertEqual(-1.0, rule.default_config.rank)
-        self.assertEqual("328", rule.cwe.cwe_id)
+        assert rule.default_config.enabled is True
+        assert rule.default_config.level == Level.ERROR
+        assert rule.default_config.rank == -1.0
+        assert rule.cwe.cwe_id == "328"
 
-    @parameterized.expand(
+    @pytest.mark.parametrize(
+        "filename",
         [
             "MessageDigestMD2.java",
             "MessageDigestMD5.java",
             "MessageDigestMD5Property.java",
             "MessageDigestSHA1.java",
             "MessageDigestSHA256.java",
-        ]
+        ],
     )
     def test(self, filename):
         self.check(filename)
```

### Comparing `precli-0.5.4/tests/unit/rules/java/stdlib/java_security/test_weak_key.py` & `precli-0.5.5/tests/unit/rules/python/stdlib/shelve/test_shelve_open.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,46 +1,49 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 import os
 
-from parameterized import parameterized
+import pytest
 
 from precli.core.level import Level
-from precli.parsers import java
+from precli.parsers import python
 from precli.rules import Rule
 from tests.unit.rules import test_case
 
 
-class KeyPairGeneratorWeakkeyTests(test_case.TestCase):
-    def setUp(self):
-        super().setUp()
-        self.rule_id = "JAV003"
-        self.parser = java.Java()
-        self.base_path = os.path.join(
+class TestShelveOpen(test_case.TestCase):
+    @classmethod
+    def setup_class(cls):
+        cls.rule_id = "PY015"
+        cls.parser = python.Python()
+        cls.base_path = os.path.join(
             "tests",
             "unit",
             "rules",
-            "java",
+            "python",
             "stdlib",
-            "java_security",
+            "shelve",
             "examples",
         )
 
     def test_rule_meta(self):
         rule = Rule.get_by_id(self.rule_id)
-        self.assertEqual(self.rule_id, rule.id)
-        self.assertEqual("inadequate_encryption_strength", rule.name)
-        self.assertEqual(
-            f"https://docs.securesauce.dev/rules/{self.rule_id}", rule.help_url
+        assert rule.id == self.rule_id
+        assert rule.name == "deserialization_of_untrusted_data"
+        assert (
+            rule.help_url
+            == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
-        self.assertEqual(True, rule.default_config.enabled)
-        self.assertEqual(Level.WARNING, rule.default_config.level)
-        self.assertEqual(-1.0, rule.default_config.rank)
-        self.assertEqual("326", rule.cwe.cwe_id)
+        assert rule.default_config.enabled is True
+        assert rule.default_config.level == Level.WARNING
+        assert rule.default_config.rank == -1.0
+        assert rule.cwe.cwe_id == "502"
 
-    @parameterized.expand(
+    @pytest.mark.parametrize(
+        "filename",
         [
-            "KeyPairGeneratorDSA.java",
-            "KeyPairGeneratorRSA.java",
-        ]
+            "shelve_dbfilenameshelf.py",
+            "shelve_open.py",
+            "shelve_open_context_mgr.py",
+        ],
     )
     def test(self, filename):
         self.check(filename)
```

### Comparing `precli-0.5.4/tests/unit/rules/java/stdlib/javax_crypto/examples/Cipher3DESCBC.java` & `precli-0.5.5/tests/unit/rules/java/stdlib/javax_crypto/examples/Cipher3DESCBC.java`

 * *Files identical despite different names*

### Comparing `precli-0.5.4/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherAESCBC.java` & `precli-0.5.5/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherAESCBC.java`

 * *Files identical despite different names*

### Comparing `precli-0.5.4/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherArcfour.java` & `precli-0.5.5/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherArcfour.java`

 * *Files identical despite different names*

### Comparing `precli-0.5.4/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherBlowfishCBC.java` & `precli-0.5.5/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherBlowfishCBC.java`

 * *Files identical despite different names*

### Comparing `precli-0.5.4/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherDESCBC.java` & `precli-0.5.5/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherDESCBC.java`

 * *Files identical despite different names*

### Comparing `precli-0.5.4/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherRC2.java` & `precli-0.5.5/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherRC2.java`

 * *Files identical despite different names*

### Comparing `precli-0.5.4/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherRC5.java` & `precli-0.5.5/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherRC5.java`

 * *Files identical despite different names*

### Comparing `precli-0.5.4/tests/unit/rules/java/stdlib/javax_crypto/test_weak_cipher.py` & `precli-0.5.5/tests/unit/rules/java/stdlib/java_security/test_weak_random.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,49 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 import os
 
-from parameterized import parameterized
+import pytest
 
 from precli.core.level import Level
 from precli.parsers import java
 from precli.rules import Rule
 from tests.unit.rules import test_case
 
 
-class WeakCipherTests(test_case.TestCase):
-    def setUp(self):
-        super().setUp()
-        self.rule_id = "JAV001"
-        self.parser = java.Java()
-        self.base_path = os.path.join(
+class TestSecureRandomWeakRandom(test_case.TestCase):
+    @classmethod
+    def setup_class(cls):
+        cls.rule_id = "JAV004"
+        cls.parser = java.Java()
+        cls.base_path = os.path.join(
             "tests",
             "unit",
             "rules",
             "java",
             "stdlib",
-            "javax_crypto",
+            "java_security",
             "examples",
         )
 
     def test_rule_meta(self):
         rule = Rule.get_by_id(self.rule_id)
-        self.assertEqual(self.rule_id, rule.id)
-        self.assertEqual(
-            "use_of_a_broken_or_risky_cryptographic_algorithm", rule.name
+        assert rule.id == self.rule_id
+        assert rule.name == "weak_prng"
+        assert (
+            rule.help_url
+            == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
-        self.assertEqual(
-            f"https://docs.securesauce.dev/rules/{self.rule_id}", rule.help_url
-        )
-        self.assertEqual(True, rule.default_config.enabled)
-        self.assertEqual(Level.ERROR, rule.default_config.level)
-        self.assertEqual(-1.0, rule.default_config.rank)
-        self.assertEqual("327", rule.cwe.cwe_id)
+        assert rule.default_config.enabled is True
+        assert rule.default_config.level == Level.WARNING
+        assert rule.default_config.rank == -1.0
+        assert rule.cwe.cwe_id == "338"
 
-    @parameterized.expand(
+    @pytest.mark.parametrize(
+        "filename",
         [
-            "Cipher3DESCBC.java",
-            "CipherAESCBC.java",
-            "CipherArcfour.java",
-            "CipherBlowfishCBC.java",
-            "CipherDESCBC.java",
-            "CipherRC2.java",
-            "CipherRC4.java",
-            "CipherRC5.java",
-        ]
+            "JavaSecuritySecureRandomSHA1PRNG.java",
+            "SecureRandomDefault.java",
+            "SecureRandomSHA1PRNG.java",
+        ],
     )
     def test(self, filename):
         self.check(filename)
```

### Comparing `precli-0.5.4/tests/unit/rules/python/stdlib/argparse/test_argparse_sensitive_info.py` & `precli-0.5.5/tests/unit/rules/python/stdlib/http/test_http_server_unrestricted_bind.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,49 +1,48 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 import os
 
-from parameterized import parameterized
+import pytest
 
 from precli.core.level import Level
 from precli.parsers import python
 from precli.rules import Rule
 from tests.unit.rules import test_case
 
 
-class ArgparseSensitiveInfoTests(test_case.TestCase):
-    def setUp(self):
-        super().setUp()
-        self.rule_id = "PY027"
-        self.parser = python.Python()
-        self.base_path = os.path.join(
+class TestHttpServerUnrestrictedBind(test_case.TestCase):
+    @classmethod
+    def setup_class(cls):
+        cls.rule_id = "PY031"
+        cls.parser = python.Python()
+        cls.base_path = os.path.join(
             "tests",
             "unit",
             "rules",
             "python",
             "stdlib",
-            "argparse",
+            "http",
             "examples",
         )
 
     def test_rule_meta(self):
         rule = Rule.get_by_id(self.rule_id)
-        self.assertEqual(self.rule_id, rule.id)
-        self.assertEqual("visible_sensitive_information", rule.name)
-        self.assertEqual(
-            f"https://docs.securesauce.dev/rules/{self.rule_id}", rule.help_url
+        assert rule.id == self.rule_id
+        assert rule.name == "unrestricted_bind"
+        assert (
+            rule.help_url
+            == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
-        self.assertEqual(True, rule.default_config.enabled)
-        self.assertEqual(Level.ERROR, rule.default_config.level)
-        self.assertEqual(-1.0, rule.default_config.rank)
-        self.assertEqual("214", rule.cwe.cwe_id)
+        assert rule.default_config.enabled is True
+        assert rule.default_config.level == Level.WARNING
+        assert rule.default_config.rank == -1.0
+        assert rule.cwe.cwe_id == "1327"
 
-    @parameterized.expand(
+    @pytest.mark.parametrize(
+        "filename",
         [
-            "argparse_add_argument_api_key.py",
-            "argparse_add_argument_default_action.py",
-            "argparse_add_argument_password.py",
-            "argparse_add_argument_password_file.py",
-            "argparse_add_argument_password_store_true.py",
-        ]
+            "http_server_http_server.py",
+            "http_server_threading_http_server.py",
+        ],
     )
     def test(self, filename):
         self.check(filename)
```

### Comparing `precli-0.5.4/tests/unit/rules/python/stdlib/assert/test_assert.py` & `precli-0.5.5/tests/unit/rules/python/stdlib/nntplib/test_nntplib_cleartext.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,50 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 import os
 
-from parameterized import parameterized
+import pytest
 
 from precli.core.level import Level
 from precli.parsers import python
 from precli.rules import Rule
 from tests.unit.rules import test_case
 
 
-class AssertTests(test_case.TestCase):
-    def setUp(self):
-        super().setUp()
-        self.rule_id = "PY001"
-        self.parser = python.Python()
-        self.base_path = os.path.join(
+class TestNntpCleartext(test_case.TestCase):
+    @classmethod
+    def setup_class(cls):
+        cls.rule_id = "PY012"
+        cls.parser = python.Python()
+        cls.base_path = os.path.join(
             "tests",
             "unit",
             "rules",
             "python",
             "stdlib",
-            "assert",
+            "nntplib",
             "examples",
         )
 
     def test_rule_meta(self):
         rule = Rule.get_by_id(self.rule_id)
-        self.assertEqual(self.rule_id, rule.id)
-        self.assertEqual("improper_check", rule.name)
-        self.assertEqual(
-            f"https://docs.securesauce.dev/rules/{self.rule_id}", rule.help_url
+        assert rule.id == self.rule_id
+        assert rule.name == "cleartext_transmission"
+        assert (
+            rule.help_url
+            == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
-        self.assertEqual(True, rule.default_config.enabled)
-        self.assertEqual(Level.WARNING, rule.default_config.level)
-        self.assertEqual(-1.0, rule.default_config.rank)
-        self.assertEqual("703", rule.cwe.cwe_id)
+        assert rule.default_config.enabled is True
+        assert rule.default_config.level == Level.ERROR
+        assert rule.default_config.rank == -1.0
+        assert rule.cwe.cwe_id == "319"
 
-    @parameterized.expand(
+    @pytest.mark.parametrize(
+        "filename",
         [
-            "assert.py",
-        ]
+            "nntplib_nntp_context_mgr.py",
+            "nntplib_nntp_login.py",
+            "nntplib_nntp_ssl.py",
+            "nntplib_nntp_starttls.py",
+        ],
     )
     def test(self, filename):
         self.check(filename)
```

### Comparing `precli-0.5.4/tests/unit/rules/python/stdlib/crypt/test_crypt_weak_hash.py` & `precli-0.5.5/tests/unit/rules/python/stdlib/hmac/test_hmac_weak_key.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,56 +1,58 @@
-# Copyright 2023 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 import os
 
-from parameterized import parameterized
+import pytest
 
 from precli.core.level import Level
 from precli.parsers import python
 from precli.rules import Rule
 from tests.unit.rules import test_case
 
 
-class CryptWeakHashTests(test_case.TestCase):
-    def setUp(self):
-        super().setUp()
-        self.rule_id = "PY002"
-        self.parser = python.Python()
-        self.base_path = os.path.join(
+class TestHmacWeakKey(test_case.TestCase):
+    @classmethod
+    def setup_class(cls):
+        cls.rule_id = "PY034"
+        cls.parser = python.Python()
+        cls.base_path = os.path.join(
             "tests",
             "unit",
             "rules",
             "python",
             "stdlib",
-            "crypt",
+            "hmac",
             "examples",
         )
 
     def test_rule_meta(self):
         rule = Rule.get_by_id(self.rule_id)
-        self.assertEqual(self.rule_id, rule.id)
-        self.assertEqual("reversible_one_way_hash", rule.name)
-        self.assertEqual(
-            f"https://docs.securesauce.dev/rules/{self.rule_id}", rule.help_url
+        assert rule.id == self.rule_id
+        assert rule.name == "insufficient_key_size"
+        assert (
+            rule.help_url
+            == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
-        self.assertEqual(True, rule.default_config.enabled)
-        self.assertEqual(Level.WARNING, rule.default_config.level)
-        self.assertEqual(-1.0, rule.default_config.rank)
-        self.assertEqual("328", rule.cwe.cwe_id)
+        assert rule.default_config.enabled is True
+        assert rule.default_config.level == Level.WARNING
+        assert rule.default_config.rank == -1.0
+        assert rule.cwe.cwe_id == "326"
 
-    @parameterized.expand(
+    @pytest.mark.parametrize(
+        "filename",
         [
-            "crypt_crypt.py",
-            "crypt_crypt_method_blowfish.py",
-            "crypt_crypt_method_crypt.py",
-            "crypt_crypt_method_md5.py",
-            "crypt_crypt_method_sha256.py",
-            "crypt_crypt_method_sha512.py",
-            "crypt_mksalt.py",
-            "crypt_mksalt_method_blowfish.py",
-            "crypt_mksalt_method_crypt.py",
-            "crypt_mksalt_method_md5.py",
-            "crypt_mksalt_method_sha256.py",
-            "crypt_mksalt_method_sha512.py",
-        ]
+            "hmac_digest_weak_key_hashlib_blake2b.py",
+            "hmac_digest_weak_key_hashlib_sha3_256.py",
+            "hmac_digest_weak_key_hashlib_sm3.py",
+            "hmac_digest_weak_key_sha224.py",
+            "hmac_digest_weak_key_sha256.py",
+            "hmac_digest_weak_key_sha512.py",
+            "hmac_new_weak_key_blake2s.py",
+            "hmac_new_weak_key_hashlib_sha3_224.py",
+            "hmac_new_weak_key_hashlib_sha3_384.py",
+            "hmac_new_weak_key_hashlib_sha3_512.py",
+            "hmac_new_weak_key_sha384.py",
+            "hmac_new_weak_key_sha512_256.py",
+        ],
     )
     def test(self, filename):
         self.check(filename)
```

### Comparing `precli-0.5.4/tests/unit/rules/python/stdlib/ftplib/test_ftplib_unverified_context.py` & `precli-0.5.5/tests/unit/rules/java/stdlib/javax_servlet_http/test_insecure_cookie.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,47 +1,48 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 import os
 
-from parameterized import parameterized
+import pytest
 
 from precli.core.level import Level
-from precli.parsers import python
+from precli.parsers import java
 from precli.rules import Rule
 from tests.unit.rules import test_case
 
 
-class FtplibUnverifiedContextTests(test_case.TestCase):
-    def setUp(self):
-        super().setUp()
-        self.rule_id = "PY022"
-        self.parser = python.Python()
-        self.base_path = os.path.join(
+class TestInsecureCookie(test_case.TestCase):
+    @classmethod
+    def setup_class(cls):
+        cls.rule_id = "JAV005"
+        cls.parser = java.Java()
+        cls.base_path = os.path.join(
             "tests",
             "unit",
             "rules",
-            "python",
+            "java",
             "stdlib",
-            "ftplib",
+            "javax_servlet_http",
             "examples",
         )
 
     def test_rule_meta(self):
         rule = Rule.get_by_id(self.rule_id)
-        self.assertEqual(self.rule_id, rule.id)
-        self.assertEqual("improper_certificate_validation", rule.name)
-        self.assertEqual(
-            f"https://docs.securesauce.dev/rules/{self.rule_id}", rule.help_url
+        assert rule.id == self.rule_id
+        assert rule.name == "insecure_cookie"
+        assert (
+            rule.help_url
+            == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
-        self.assertEqual(True, rule.default_config.enabled)
-        self.assertEqual(Level.WARNING, rule.default_config.level)
-        self.assertEqual(-1.0, rule.default_config.rank)
-        self.assertEqual("295", rule.cwe.cwe_id)
+        assert rule.default_config.enabled is True
+        assert rule.default_config.level == Level.WARNING
+        assert rule.default_config.rank == -1.0
+        assert rule.cwe.cwe_id == "614"
 
-    @parameterized.expand(
+    @pytest.mark.parametrize(
+        "filename",
         [
-            "ftplib_ftp_tls_context_as_var.py",
-            "ftplib_ftp_tls_context_none.py",
-            "ftplib_ftp_tls_context_unset.py",
-        ]
+            "CookieSecureFalse.java",
+            "CookieSecureTrue.java",
+        ],
     )
     def test(self, filename):
         self.check(filename)
```

### Comparing `precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/test_hashlib_improper_prng.py` & `precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/test_hashlib_improper_prng.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,48 +1,50 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 import os
 
-from parameterized import parameterized
+import pytest
 
 from precli.core.level import Level
 from precli.parsers import python
 from precli.rules import Rule
 from tests.unit.rules import test_case
 
 
-class HashlibImproperPrngTests(test_case.TestCase):
-    def setUp(self):
-        super().setUp()
-        self.rule_id = "PY035"
-        self.parser = python.Python()
-        self.base_path = os.path.join(
+class TestHashlibImproperPrng(test_case.TestCase):
+    @classmethod
+    def setup_class(cls):
+        cls.rule_id = "PY035"
+        cls.parser = python.Python()
+        cls.base_path = os.path.join(
             "tests",
             "unit",
             "rules",
             "python",
             "stdlib",
             "hashlib",
             "examples",
         )
 
     def test_rule_meta(self):
         rule = Rule.get_by_id(self.rule_id)
-        self.assertEqual(self.rule_id, rule.id)
-        self.assertEqual("improper_random", rule.name)
-        self.assertEqual(
-            f"https://docs.securesauce.dev/rules/{self.rule_id}", rule.help_url
+        assert rule.id == self.rule_id
+        assert rule.name == "improper_random"
+        assert (
+            rule.help_url
+            == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
-        self.assertEqual(True, rule.default_config.enabled)
-        self.assertEqual(Level.WARNING, rule.default_config.level)
-        self.assertEqual(-1.0, rule.default_config.rank)
-        self.assertEqual("330", rule.cwe.cwe_id)
+        assert rule.default_config.enabled is True
+        assert rule.default_config.level == Level.WARNING
+        assert rule.default_config.rank == -1.0
+        assert rule.cwe.cwe_id == "330"
 
-    @parameterized.expand(
+    @pytest.mark.parametrize(
+        "filename",
         [
             "hashlib_improper_prng_blake2b.py",
             "hashlib_improper_prng_blake2s.py",
             "hashlib_improper_prng_pbkdf2_hmac.py",
             "hashlib_improper_prng_scrypt.py",
-        ]
+        ],
     )
     def test(self, filename):
         self.check(filename)
```

### Comparing `precli-0.5.4/tests/unit/rules/python/stdlib/hashlib/test_hashlib_weak_hash.py` & `precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/test_hashlib_weak_hash.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,48 @@
-# Copyright 2023 Secure Saurce LLC
+# Copyright 2023 Secure Sauce LLC
 import os
 
-from parameterized import parameterized
+import pytest
 
 from precli.core.level import Level
 from precli.parsers import python
 from precli.rules import Rule
 from tests.unit.rules import test_case
 
 
-class HashlibWeakHashTests(test_case.TestCase):
-    def setUp(self):
-        super().setUp()
-        self.rule_id = "PY004"
-        self.parser = python.Python()
-        self.base_path = os.path.join(
+class TestHashlibWeakHash(test_case.TestCase):
+    @classmethod
+    def setup_class(cls):
+        cls.rule_id = "PY004"
+        cls.parser = python.Python()
+        cls.base_path = os.path.join(
             "tests",
             "unit",
             "rules",
             "python",
             "stdlib",
             "hashlib",
             "examples",
         )
 
     def test_rule_meta(self):
         rule = Rule.get_by_id(self.rule_id)
-        self.assertEqual(self.rule_id, rule.id)
-        self.assertEqual("reversible_one_way_hash", rule.name)
-        self.assertEqual(
-            f"https://docs.securesauce.dev/rules/{self.rule_id}", rule.help_url
+        assert rule.id == self.rule_id
+        assert rule.name == "reversible_one_way_hash"
+        assert (
+            rule.help_url
+            == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
-        self.assertEqual(True, rule.default_config.enabled)
-        self.assertEqual(Level.ERROR, rule.default_config.level)
-        self.assertEqual(-1.0, rule.default_config.rank)
-        self.assertEqual("328", rule.cwe.cwe_id)
+        assert rule.default_config.enabled is True
+        assert rule.default_config.level == Level.ERROR
+        assert rule.default_config.rank == -1.0
+        assert rule.cwe.cwe_id == "328"
 
-    @parameterized.expand(
+    @pytest.mark.parametrize(
+        "filename",
         [
             "hashlib_blake2b.py",
             "hashlib_blake2s.py",
             "hashlib_md4.py",
             "hashlib_md5.py",
             "hashlib_md5_as_identifier.py",
             "hashlib_md5_importlib.py",
@@ -90,11 +92,11 @@
             "hashlib_sha3_256.py",
             "hashlib_sha3_384.py",
             "hashlib_sha3_512.py",
             "hashlib_sha512.py",
             "hashlib_sha_usedforsecurity_false.py",
             "hashlib_shake_128.py",
             "hashlib_shake_256.py",
-        ]
+        ],
     )
     def test(self, filename):
         self.check(filename)
```

### Comparing `precli-0.5.4/tests/unit/rules/python/stdlib/hmac/test_hmac_timing_attack.py` & `precli-0.5.5/tests/unit/rules/python/stdlib/ssl/test_ssl_wrap_socket_tls_version.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,48 +1,53 @@
-# Copyright 2023 Secure Saurce LLC
+# Copyright 2023 Secure Sauce LLC
 import os
 
-from parameterized import parameterized
+import pytest
 
 from precli.core.level import Level
 from precli.parsers import python
 from precli.rules import Rule
 from tests.unit.rules import test_case
 
 
-class HmacTimingAttackTests(test_case.TestCase):
-    def setUp(self):
-        super().setUp()
-        self.rule_id = "PY005"
-        self.parser = python.Python()
-        self.base_path = os.path.join(
+class TestWrapSocket(test_case.TestCase):
+    @classmethod
+    def setup_class(cls):
+        cls.rule_id = "PY018"
+        cls.parser = python.Python()
+        cls.base_path = os.path.join(
             "tests",
             "unit",
             "rules",
             "python",
             "stdlib",
-            "hmac",
+            "ssl",
             "examples",
         )
 
     def test_rule_meta(self):
         rule = Rule.get_by_id(self.rule_id)
-        self.assertEqual(self.rule_id, rule.id)
-        self.assertEqual("observable_timing_discrepancy", rule.name)
-        self.assertEqual(
-            f"https://docs.securesauce.dev/rules/{self.rule_id}", rule.help_url
+        assert rule.id == self.rule_id
+        assert rule.name == "inadequate_encryption_strength"
+        assert (
+            rule.help_url
+            == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
-        self.assertEqual(True, rule.default_config.enabled)
-        self.assertEqual(Level.ERROR, rule.default_config.level)
-        self.assertEqual(-1.0, rule.default_config.rank)
-        self.assertEqual("208", rule.cwe.cwe_id)
+        assert rule.default_config.enabled is True
+        assert rule.default_config.level == Level.ERROR
+        assert rule.default_config.rank == -1.0
+        assert rule.cwe.cwe_id == "326"
 
-    @parameterized.expand(
+    @pytest.mark.parametrize(
+        "filename",
         [
-            "hmac_timing_attack.py",
-            "hmac_timing_attack_class.py",
-            "hmac_timing_attack_class_hexdigest.py",
-            "hmac_timing_attack_compare_digest.py",
-        ]
+            "wrap_socket_sslv2.py",
+            "wrap_socket_sslv23.py",
+            "wrap_socket_sslv2_server_side_true.py",
+            "wrap_socket_sslv3.py",
+            "wrap_socket_tlsv1.py",
+            "wrap_socket_tlsv11.py",
+            "wrap_socket_tlsv12.py",
+        ],
     )
     def test(self, filename):
         self.check(filename)
```

### Comparing `precli-0.5.4/tests/unit/rules/python/stdlib/hmac/test_hmac_weak_hash.py` & `precli-0.5.5/tests/unit/rules/python/stdlib/hmac/test_hmac_weak_hash.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,46 +1,48 @@
-# Copyright 2023 Secure Saurce LLC
+# Copyright 2023 Secure Sauce LLC
 import os
 
-from parameterized import parameterized
+import pytest
 
 from precli.core.level import Level
 from precli.parsers import python
 from precli.rules import Rule
 from tests.unit.rules import test_case
 
 
-class HmacWeakHashTests(test_case.TestCase):
-    def setUp(self):
-        super().setUp()
-        self.rule_id = "PY006"
-        self.parser = python.Python()
-        self.base_path = os.path.join(
+class TestHmacWeakHash(test_case.TestCase):
+    @classmethod
+    def setup_class(cls):
+        cls.rule_id = "PY006"
+        cls.parser = python.Python()
+        cls.base_path = os.path.join(
             "tests",
             "unit",
             "rules",
             "python",
             "stdlib",
             "hmac",
             "examples",
         )
 
     def test_rule_meta(self):
         rule = Rule.get_by_id(self.rule_id)
-        self.assertEqual(self.rule_id, rule.id)
-        self.assertEqual("reversible_one_way_hash", rule.name)
-        self.assertEqual(
-            f"https://docs.securesauce.dev/rules/{self.rule_id}", rule.help_url
+        assert rule.id == self.rule_id
+        assert rule.name == "reversible_one_way_hash"
+        assert (
+            rule.help_url
+            == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
-        self.assertEqual(True, rule.default_config.enabled)
-        self.assertEqual(Level.ERROR, rule.default_config.level)
-        self.assertEqual(-1.0, rule.default_config.rank)
-        self.assertEqual("328", rule.cwe.cwe_id)
+        assert rule.default_config.enabled is True
+        assert rule.default_config.level == Level.ERROR
+        assert rule.default_config.rank == -1.0
+        assert rule.cwe.cwe_id == "328"
 
-    @parameterized.expand(
+    @pytest.mark.parametrize(
+        "filename",
         [
             "hmac_digest_blake2b.py",
             "hmac_digest_blake2s.py",
             "hmac_digest_hashlib_blake2b.py",
             "hmac_digest_hashlib_blake2s.py",
             "hmac_digest_hashlib_md4.py",
             "hmac_digest_hashlib_md5.py",
@@ -104,11 +106,11 @@
             "hmac_new_digestmod_sha3_224.py",
             "hmac_new_digestmod_sha3_256.py",
             "hmac_new_digestmod_sha3_384.py",
             "hmac_new_digestmod_sha3_512.py",
             "hmac_new_digestmod_sha512.py",
             "hmac_new_digestmod_shake_128.py",
             "hmac_new_digestmod_shake_256.py",
-        ]
+        ],
     )
     def test(self, filename):
         self.check(filename)
```

### Comparing `precli-0.5.4/tests/unit/rules/python/stdlib/http/test_http_server_unrestricted_bind.py` & `precli-0.5.5/tests/unit/rules/python/stdlib/xmlrpc/test_xmlrpc_server_unrestricted_bind.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,48 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 import os
 
-from parameterized import parameterized
+import pytest
 
 from precli.core.level import Level
 from precli.parsers import python
 from precli.rules import Rule
 from tests.unit.rules import test_case
 
 
-class HttpServerUnrestrictedBindTests(test_case.TestCase):
-    def setUp(self):
-        super().setUp()
-        self.rule_id = "PY031"
-        self.parser = python.Python()
-        self.base_path = os.path.join(
+class TestXmlrpcServerUnrestrictedBind(test_case.TestCase):
+    @classmethod
+    def setup_class(cls):
+        cls.rule_id = "PY032"
+        cls.parser = python.Python()
+        cls.base_path = os.path.join(
             "tests",
             "unit",
             "rules",
             "python",
             "stdlib",
-            "http",
+            "xmlrpc",
             "examples",
         )
 
     def test_rule_meta(self):
         rule = Rule.get_by_id(self.rule_id)
-        self.assertEqual(self.rule_id, rule.id)
-        self.assertEqual("unrestricted_bind", rule.name)
-        self.assertEqual(
-            f"https://docs.securesauce.dev/rules/{self.rule_id}", rule.help_url
+        assert rule.id == self.rule_id
+        assert rule.name == "unrestricted_bind"
+        assert (
+            rule.help_url
+            == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
-        self.assertEqual(True, rule.default_config.enabled)
-        self.assertEqual(Level.WARNING, rule.default_config.level)
-        self.assertEqual(-1.0, rule.default_config.rank)
-        self.assertEqual("1327", rule.cwe.cwe_id)
+        assert rule.default_config.enabled is True
+        assert rule.default_config.level == Level.WARNING
+        assert rule.default_config.rank == -1.0
+        assert rule.cwe.cwe_id == "1327"
 
-    @parameterized.expand(
+    @pytest.mark.parametrize(
+        "filename",
         [
-            "http_server_http_server.py",
-            "http_server_threading_http_server.py",
-        ]
+            "xmlrpc_server_doc_xml_rpc_server.py",
+            "xmlrpc_server_simple_xml_rpc_server.py",
+        ],
     )
     def test(self, filename):
         self.check(filename)
```

### Comparing `precli-0.5.4/tests/unit/rules/python/stdlib/http/test_http_url_secret.py` & `precli-0.5.5/tests/unit/rules/python/stdlib/socket/test_socket_unrestricted_bind.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 import os
 
-from parameterized import parameterized
+import pytest
 
 from precli.core.level import Level
 from precli.parsers import python
 from precli.rules import Rule
 from tests.unit.rules import test_case
 
 
-class HttpUrlSecretTests(test_case.TestCase):
-    def setUp(self):
-        super().setUp()
-        self.rule_id = "PY007"
-        self.parser = python.Python()
-        self.base_path = os.path.join(
+class TestSocketUnrestrictedBind(test_case.TestCase):
+    @classmethod
+    def setup_class(cls):
+        cls.rule_id = "PY029"
+        cls.parser = python.Python()
+        cls.base_path = os.path.join(
             "tests",
             "unit",
             "rules",
             "python",
             "stdlib",
-            "http",
+            "socket",
             "examples",
         )
 
     def test_rule_meta(self):
         rule = Rule.get_by_id(self.rule_id)
-        self.assertEqual(self.rule_id, rule.id)
-        self.assertEqual("sensitive_query_strings", rule.name)
-        self.assertEqual(
-            f"https://docs.securesauce.dev/rules/{self.rule_id}", rule.help_url
+        assert rule.id == self.rule_id
+        assert rule.name == "unrestricted_bind"
+        assert (
+            rule.help_url
+            == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
-        self.assertEqual(True, rule.default_config.enabled)
-        self.assertEqual(Level.ERROR, rule.default_config.level)
-        self.assertEqual(-1.0, rule.default_config.rank)
-        self.assertEqual("598", rule.cwe.cwe_id)
+        assert rule.default_config.enabled is True
+        assert rule.default_config.level == Level.WARNING
+        assert rule.default_config.rank == -1.0
+        assert rule.cwe.cwe_id == "1327"
 
-    @parameterized.expand(
+    @pytest.mark.parametrize(
+        "filename",
         [
-            "http_url_secret_apikey.py",
-            "http_url_secret_apikey_in_header.py",
-            "http_url_secret_basic_auth.py",
-            "http_url_secret_basic_auth_as_var.py",
-            "http_url_secret_password.py",
-            "http_url_secret_username.py",
-        ]
+            "socket_create_server.py",
+            "socket_socket_bind.py",
+            "socket_socket_bind_as_var.py",
+            "socket_socket_bind_as_vars.py",
+        ],
     )
     def test(self, filename):
         self.check(filename)
```

### Comparing `precli-0.5.4/tests/unit/rules/python/stdlib/imaplib/test_imaplib_cleartext.py` & `precli-0.5.5/tests/unit/rules/python/stdlib/imaplib/test_imaplib_cleartext.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,53 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 import os
 
-from parameterized import parameterized
+import pytest
 
 from precli.core.level import Level
 from precli.parsers import python
 from precli.rules import Rule
 from tests.unit.rules import test_case
 
 
-class ImapCleartextTests(test_case.TestCase):
-    def setUp(self):
-        super().setUp()
-        self.rule_id = "PY008"
-        self.parser = python.Python()
-        self.base_path = os.path.join(
+class TestImapCleartext(test_case.TestCase):
+    @classmethod
+    def setup_class(cls):
+        cls.rule_id = "PY008"
+        cls.parser = python.Python()
+        cls.base_path = os.path.join(
             "tests",
             "unit",
             "rules",
             "python",
             "stdlib",
             "imaplib",
             "examples",
         )
 
     def test_rule_meta(self):
         rule = Rule.get_by_id(self.rule_id)
-        self.assertEqual(self.rule_id, rule.id)
-        self.assertEqual("cleartext_transmission", rule.name)
-        self.assertEqual(
-            f"https://docs.securesauce.dev/rules/{self.rule_id}", rule.help_url
+        assert rule.id == self.rule_id
+        assert rule.name == "cleartext_transmission"
+        assert (
+            rule.help_url
+            == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
-        self.assertEqual(True, rule.default_config.enabled)
-        self.assertEqual(Level.ERROR, rule.default_config.level)
-        self.assertEqual(-1.0, rule.default_config.rank)
-        self.assertEqual("319", rule.cwe.cwe_id)
+        assert rule.default_config.enabled is True
+        assert rule.default_config.level == Level.ERROR
+        assert rule.default_config.rank == -1.0
+        assert rule.cwe.cwe_id == "319"
 
-    @parameterized.expand(
+    @pytest.mark.parametrize(
+        "filename",
         [
             "imaplib_imap4_authenticate.py",
             "imaplib_imap4_context_mgr.py",
             "imaplib_imap4_login.py",
             "imaplib_imap4_login_cram_md5.py",
             "imaplib_imap4_ssl.py",
             "imaplib_imap4_starttls.py",
             "imaplib_imap4_stream.py",
-        ]
+        ],
     )
     def test(self, filename):
         self.check(filename)
```

### Comparing `precli-0.5.4/tests/unit/rules/python/stdlib/imaplib/test_imaplib_unverified_context.py` & `precli-0.5.5/tests/unit/rules/python/stdlib/nntplib/test_nntplib_unverified_context.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,50 +1,52 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 import os
 
-from parameterized import parameterized
+import pytest
 
 from precli.core.level import Level
 from precli.parsers import python
 from precli.rules import Rule
 from tests.unit.rules import test_case
 
 
-class ImaplibUnverifiedContextTests(test_case.TestCase):
-    def setUp(self):
-        super().setUp()
-        self.rule_id = "PY023"
-        self.parser = python.Python()
-        self.base_path = os.path.join(
+class TestNntplibUnverifiedContext(test_case.TestCase):
+    @classmethod
+    def setup_class(cls):
+        cls.rule_id = "PY024"
+        cls.parser = python.Python()
+        cls.base_path = os.path.join(
             "tests",
             "unit",
             "rules",
             "python",
             "stdlib",
-            "imaplib",
+            "nntplib",
             "examples",
         )
 
     def test_rule_meta(self):
         rule = Rule.get_by_id(self.rule_id)
-        self.assertEqual(self.rule_id, rule.id)
-        self.assertEqual("improper_certificate_validation", rule.name)
-        self.assertEqual(
-            f"https://docs.securesauce.dev/rules/{self.rule_id}", rule.help_url
+        assert rule.id == self.rule_id
+        assert rule.name == "improper_certificate_validation"
+        assert (
+            rule.help_url
+            == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
-        self.assertEqual(True, rule.default_config.enabled)
-        self.assertEqual(Level.WARNING, rule.default_config.level)
-        self.assertEqual(-1.0, rule.default_config.rank)
-        self.assertEqual("295", rule.cwe.cwe_id)
+        assert rule.default_config.enabled is True
+        assert rule.default_config.level == Level.WARNING
+        assert rule.default_config.rank == -1.0
+        assert rule.cwe.cwe_id == "295"
 
-    @parameterized.expand(
+    @pytest.mark.parametrize(
+        "filename",
         [
-            "imaplib_imap4_ssl_context_as_var.py",
-            "imaplib_imap4_ssl_context_none.py",
-            "imaplib_imap4_ssl_context_unset.py",
-            "imaplib_imap4_starttls_context_as_var.py",
-            "imaplib_imap4_starttls_context_none.py",
-            "imaplib_imap4_starttls_context_unset.py",
-        ]
+            "nntplib_nntp_ssl_context_as_var.py",
+            "nntplib_nntp_ssl_context_none.py",
+            "nntplib_nntp_ssl_context_unset.py",
+            "nntplib_nntp_starttls_context_as_var.py",
+            "nntplib_nntp_starttls_context_none.py",
+            "nntplib_nntp_starttls_context_unset.py",
+        ],
     )
     def test(self, filename):
         self.check(filename)
```

### Comparing `precli-0.5.4/tests/unit/rules/python/stdlib/json/test_json_load.py` & `precli-0.5.5/tests/unit/rules/python/stdlib/telnetlib/test_telnetlib_cleartext.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,49 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2023 Secure Sauce LLC
 import os
 
-from parameterized import parameterized
+import pytest
 
 from precli.core.level import Level
 from precli.parsers import python
 from precli.rules import Rule
 from tests.unit.rules import test_case
 
 
-class JsonLoadTests(test_case.TestCase):
-    def setUp(self):
-        super().setUp()
-        self.rule_id = "PY009"
-        self.parser = python.Python(enabled=[self.rule_id])
-        self.base_path = os.path.join(
+class TestTelnetlibCleartext(test_case.TestCase):
+    @classmethod
+    def setup_class(cls):
+        cls.rule_id = "PY020"
+        cls.parser = python.Python()
+        cls.base_path = os.path.join(
             "tests",
             "unit",
             "rules",
             "python",
             "stdlib",
-            "json",
+            "telnetlib",
             "examples",
         )
 
     def test_rule_meta(self):
         rule = Rule.get_by_id(self.rule_id)
-        self.assertEqual(self.rule_id, rule.id)
-        self.assertEqual("deserialization_of_untrusted_data", rule.name)
-        self.assertEqual(
-            f"https://docs.securesauce.dev/rules/{self.rule_id}", rule.help_url
+        assert rule.id == self.rule_id
+        assert rule.name == "cleartext_transmission"
+        assert (
+            rule.help_url
+            == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
-        self.assertEqual(True, rule.default_config.enabled)
-        self.assertEqual(Level.WARNING, rule.default_config.level)
-        self.assertEqual(-1.0, rule.default_config.rank)
-        self.assertEqual("502", rule.cwe.cwe_id)
+        assert rule.default_config.enabled is True
+        assert rule.default_config.level == Level.ERROR
+        assert rule.default_config.rank == -1.0
+        assert rule.cwe.cwe_id == "319"
 
-    @parameterized.expand(
+    @pytest.mark.parametrize(
+        "filename",
         [
-            "json_jsondecoder_decode.py",
-            "json_load.py",
-            "json_loads.py",
-        ]
+            "telnet.py",
+            "telnetlib_telnet.py",
+            "telnetlib_telnet_context_mgr.py",
+        ],
     )
     def test(self, filename):
         self.check(filename)
```

### Comparing `precli-0.5.4/tests/unit/rules/python/stdlib/logging/test_logging_insecure_listen_config.py` & `precli-0.5.5/tests/unit/rules/python/stdlib/logging/test_logging_insecure_listen_config.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,51 +1,53 @@
-# Copyright 2023 Secure Saurce LLC
+# Copyright 2023 Secure Sauce LLC
 import os
 
-from parameterized import parameterized
+import pytest
 
 from precli.core.level import Level
 from precli.parsers import python
 from precli.rules import Rule
 from tests.unit.rules import test_case
 
 
-class InsecureListenConfigTests(test_case.TestCase):
-    def setUp(self):
-        super().setUp()
-        self.rule_id = "PY010"
-        self.parser = python.Python()
-        self.base_path = os.path.join(
+class TestInsecureListenConfig(test_case.TestCase):
+    @classmethod
+    def setup_class(cls):
+        cls.rule_id = "PY010"
+        cls.parser = python.Python()
+        cls.base_path = os.path.join(
             "tests",
             "unit",
             "rules",
             "python",
             "stdlib",
             "logging",
             "examples",
         )
 
     def test_rule_meta(self):
         rule = Rule.get_by_id(self.rule_id)
-        self.assertEqual(self.rule_id, rule.id)
-        self.assertEqual("code_injection", rule.name)
-        self.assertEqual(
-            f"https://docs.securesauce.dev/rules/{self.rule_id}", rule.help_url
+        assert rule.id == self.rule_id
+        assert rule.name == "code_injection"
+        assert (
+            rule.help_url
+            == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
-        self.assertEqual(True, rule.default_config.enabled)
-        self.assertEqual(Level.WARNING, rule.default_config.level)
-        self.assertEqual(-1.0, rule.default_config.rank)
-        self.assertEqual("94", rule.cwe.cwe_id)
+        assert rule.default_config.enabled is True
+        assert rule.default_config.level == Level.WARNING
+        assert rule.default_config.rank == -1.0
+        assert rule.cwe.cwe_id == "94"
 
-    @parameterized.expand(
+    @pytest.mark.parametrize(
+        "filename",
         [
             "insecure_listen_config_empty_args.py",
             "insecure_listen_config_port.py",
             "insecure_listen_config_port_verify_as_var.py",
             "insecure_listen_config_port_verify_none.py",
             "insecure_listen_config_verify_none.py",
             "insecure_listen_config_verify_none_port.py",
             "insecure_listen_config_verify_set.py",
-        ]
+        ],
     )
     def test(self, filename):
         self.check(filename)
```

### Comparing `precli-0.5.4/tests/unit/rules/python/stdlib/marshal/test_marshal_load.py` & `precli-0.5.5/tests/unit/rules/python/stdlib/ssl/test_ssl_get_server_certificate_tls_version.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,52 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2023 Secure Sauce LLC
 import os
 
-from parameterized import parameterized
+import pytest
 
 from precli.core.level import Level
 from precli.parsers import python
 from precli.rules import Rule
 from tests.unit.rules import test_case
 
 
-class MarshalLoadTests(test_case.TestCase):
-    def setUp(self):
-        super().setUp()
-        self.rule_id = "PY011"
-        self.parser = python.Python()
-        self.base_path = os.path.join(
+class TestGetServerCertificate(test_case.TestCase):
+    @classmethod
+    def setup_class(cls):
+        cls.rule_id = "PY018"
+        cls.parser = python.Python()
+        cls.base_path = os.path.join(
             "tests",
             "unit",
             "rules",
             "python",
             "stdlib",
-            "marshal",
+            "ssl",
             "examples",
         )
 
     def test_rule_meta(self):
         rule = Rule.get_by_id(self.rule_id)
-        self.assertEqual(self.rule_id, rule.id)
-        self.assertEqual("deserialization_of_untrusted_data", rule.name)
-        self.assertEqual(
-            f"https://docs.securesauce.dev/rules/{self.rule_id}", rule.help_url
+        assert rule.id == self.rule_id
+        assert rule.name == "inadequate_encryption_strength"
+        assert (
+            rule.help_url
+            == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
-        self.assertEqual(True, rule.default_config.enabled)
-        self.assertEqual(Level.WARNING, rule.default_config.level)
-        self.assertEqual(-1.0, rule.default_config.rank)
-        self.assertEqual("502", rule.cwe.cwe_id)
+        assert rule.default_config.enabled is True
+        assert rule.default_config.level == Level.ERROR
+        assert rule.default_config.rank == -1.0
+        assert rule.cwe.cwe_id == "326"
 
-    @parameterized.expand(
+    @pytest.mark.parametrize(
+        "filename",
         [
-            "marshal_load.py",
-            "marshal_loads.py",
-        ]
+            "get_server_certificate_sslv2.py",
+            "get_server_certificate_sslv23.py",
+            "get_server_certificate_sslv3.py",
+            "get_server_certificate_tlsv1.py",
+            "get_server_certificate_tlsv11.py",
+            "get_server_certificate_tlsv12.py",
+        ],
     )
     def test(self, filename):
         self.check(filename)
```

### Comparing `precli-0.5.4/tests/unit/rules/python/stdlib/nntplib/test_nntplib_cleartext.py` & `precli-0.5.5/tests/unit/rules/python/stdlib/pickle/test_pickle_load.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,48 +1,49 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 import os
 
-from parameterized import parameterized
+import pytest
 
 from precli.core.level import Level
 from precli.parsers import python
 from precli.rules import Rule
 from tests.unit.rules import test_case
 
 
-class NntpCleartextTests(test_case.TestCase):
-    def setUp(self):
-        super().setUp()
-        self.rule_id = "PY012"
-        self.parser = python.Python()
-        self.base_path = os.path.join(
+class TestPickleLoad(test_case.TestCase):
+    @classmethod
+    def setup_class(cls):
+        cls.rule_id = "PY013"
+        cls.parser = python.Python()
+        cls.base_path = os.path.join(
             "tests",
             "unit",
             "rules",
             "python",
             "stdlib",
-            "nntplib",
+            "pickle",
             "examples",
         )
 
     def test_rule_meta(self):
         rule = Rule.get_by_id(self.rule_id)
-        self.assertEqual(self.rule_id, rule.id)
-        self.assertEqual("cleartext_transmission", rule.name)
-        self.assertEqual(
-            f"https://docs.securesauce.dev/rules/{self.rule_id}", rule.help_url
+        assert rule.id == self.rule_id
+        assert rule.name == "deserialization_of_untrusted_data"
+        assert (
+            rule.help_url
+            == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
-        self.assertEqual(True, rule.default_config.enabled)
-        self.assertEqual(Level.ERROR, rule.default_config.level)
-        self.assertEqual(-1.0, rule.default_config.rank)
-        self.assertEqual("319", rule.cwe.cwe_id)
+        assert rule.default_config.enabled is True
+        assert rule.default_config.level == Level.WARNING
+        assert rule.default_config.rank == -1.0
+        assert rule.cwe.cwe_id == "502"
 
-    @parameterized.expand(
+    @pytest.mark.parametrize(
+        "filename",
         [
-            "nntplib_nntp_context_mgr.py",
-            "nntplib_nntp_login.py",
-            "nntplib_nntp_ssl.py",
-            "nntplib_nntp_starttls.py",
-        ]
+            "pickle_load.py",
+            "pickle_loads.py",
+            "pickle_unpickler.py",
+        ],
     )
     def test(self, filename):
         self.check(filename)
```

### Comparing `precli-0.5.4/tests/unit/rules/python/stdlib/nntplib/test_nntplib_unverified_context.py` & `precli-0.5.5/tests/unit/rules/python/stdlib/smtplib/test_smtplib_unverified_context.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,52 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 import os
 
-from parameterized import parameterized
+import pytest
 
 from precli.core.level import Level
 from precli.parsers import python
 from precli.rules import Rule
 from tests.unit.rules import test_case
 
 
-class NntplibUnverifiedContextTests(test_case.TestCase):
-    def setUp(self):
-        super().setUp()
-        self.rule_id = "PY024"
-        self.parser = python.Python()
-        self.base_path = os.path.join(
+class TestSmtplibUnverifiedContext(test_case.TestCase):
+    @classmethod
+    def setup_class(cls):
+        cls.rule_id = "PY026"
+        cls.parser = python.Python()
+        cls.base_path = os.path.join(
             "tests",
             "unit",
             "rules",
             "python",
             "stdlib",
-            "nntplib",
+            "smtplib",
             "examples",
         )
 
     def test_rule_meta(self):
         rule = Rule.get_by_id(self.rule_id)
-        self.assertEqual(self.rule_id, rule.id)
-        self.assertEqual("improper_certificate_validation", rule.name)
-        self.assertEqual(
-            f"https://docs.securesauce.dev/rules/{self.rule_id}", rule.help_url
+        assert rule.id == self.rule_id
+        assert rule.name == "improper_certificate_validation"
+        assert (
+            rule.help_url
+            == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
-        self.assertEqual(True, rule.default_config.enabled)
-        self.assertEqual(Level.WARNING, rule.default_config.level)
-        self.assertEqual(-1.0, rule.default_config.rank)
-        self.assertEqual("295", rule.cwe.cwe_id)
+        assert rule.default_config.enabled is True
+        assert rule.default_config.level == Level.WARNING
+        assert rule.default_config.rank == -1.0
+        assert rule.cwe.cwe_id == "295"
 
-    @parameterized.expand(
+    @pytest.mark.parametrize(
+        "filename",
         [
-            "nntplib_nntp_ssl_context_as_var.py",
-            "nntplib_nntp_ssl_context_none.py",
-            "nntplib_nntp_ssl_context_unset.py",
-            "nntplib_nntp_starttls_context_as_var.py",
-            "nntplib_nntp_starttls_context_none.py",
-            "nntplib_nntp_starttls_context_unset.py",
-        ]
+            "smtplib_smtp_ssl_context_as_var.py",
+            "smtplib_smtp_ssl_context_none.py",
+            "smtplib_smtp_ssl_context_unset.py",
+            "smtplib_smtp_starttls_context_as_var.py",
+            "smtplib_smtp_starttls_context_none.py",
+            "smtplib_smtp_starttls_context_unset.py",
+        ],
     )
     def test(self, filename):
         self.check(filename)
```

### Comparing `precli-0.5.4/tests/unit/rules/python/stdlib/pickle/test_pickle_load.py` & `precli-0.5.5/tests/unit/rules/python/stdlib/json/test_json_load.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,49 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 import os
 
-from parameterized import parameterized
+import pytest
 
 from precli.core.level import Level
 from precli.parsers import python
 from precli.rules import Rule
 from tests.unit.rules import test_case
 
 
-class PickleLoadTests(test_case.TestCase):
-    def setUp(self):
-        super().setUp()
-        self.rule_id = "PY013"
-        self.parser = python.Python()
-        self.base_path = os.path.join(
+class TestJsonLoad(test_case.TestCase):
+    @classmethod
+    def setup_class(cls):
+        cls.rule_id = "PY009"
+        cls.parser = python.Python()
+        cls.base_path = os.path.join(
             "tests",
             "unit",
             "rules",
             "python",
             "stdlib",
-            "pickle",
+            "json",
             "examples",
         )
 
     def test_rule_meta(self):
         rule = Rule.get_by_id(self.rule_id)
-        self.assertEqual(self.rule_id, rule.id)
-        self.assertEqual("deserialization_of_untrusted_data", rule.name)
-        self.assertEqual(
-            f"https://docs.securesauce.dev/rules/{self.rule_id}", rule.help_url
+        assert rule.id == self.rule_id
+        assert rule.name == "deserialization_of_untrusted_data"
+        assert (
+            rule.help_url
+            == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
-        self.assertEqual(True, rule.default_config.enabled)
-        self.assertEqual(Level.WARNING, rule.default_config.level)
-        self.assertEqual(-1.0, rule.default_config.rank)
-        self.assertEqual("502", rule.cwe.cwe_id)
+        assert rule.default_config.enabled is False
+        assert rule.default_config.level == Level.WARNING
+        assert rule.default_config.rank == -1.0
+        assert rule.cwe.cwe_id == "502"
 
-    @parameterized.expand(
+    @pytest.mark.parametrize(
+        "filename",
         [
-            "pickle_load.py",
-            "pickle_loads.py",
-            "pickle_unpickler.py",
-        ]
+            "json_jsondecoder_decode.py",
+            "json_load.py",
+            "json_loads.py",
+        ],
     )
     def test(self, filename):
-        self.check(filename)
+        self.check(filename, enabled=[self.rule_id])
```

### Comparing `precli-0.5.4/tests/unit/rules/python/stdlib/poplib/test_poplib_cleartext.py` & `precli-0.5.5/tests/unit/rules/python/stdlib/poplib/test_poplib_cleartext.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,53 @@
-# Copyright 2023 Secure Saurce LLC
+# Copyright 2023 Secure Sauce LLC
 import os
 
-from parameterized import parameterized
+import pytest
 
 from precli.core.level import Level
 from precli.parsers import python
 from precli.rules import Rule
 from tests.unit.rules import test_case
 
 
-class PopCleartextTests(test_case.TestCase):
-    def setUp(self):
-        super().setUp()
-        self.rule_id = "PY014"
-        self.parser = python.Python()
-        self.base_path = os.path.join(
+class TestPopCleartext(test_case.TestCase):
+    @classmethod
+    def setup_class(cls):
+        cls.rule_id = "PY014"
+        cls.parser = python.Python()
+        cls.base_path = os.path.join(
             "tests",
             "unit",
             "rules",
             "python",
             "stdlib",
             "poplib",
             "examples",
         )
 
     def test_rule_meta(self):
         rule = Rule.get_by_id(self.rule_id)
-        self.assertEqual(self.rule_id, rule.id)
-        self.assertEqual("cleartext_transmission", rule.name)
-        self.assertEqual(
-            f"https://docs.securesauce.dev/rules/{self.rule_id}", rule.help_url
+        assert rule.id == self.rule_id
+        assert rule.name == "cleartext_transmission"
+        assert (
+            rule.help_url
+            == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
-        self.assertEqual(True, rule.default_config.enabled)
-        self.assertEqual(Level.ERROR, rule.default_config.level)
-        self.assertEqual(-1.0, rule.default_config.rank)
-        self.assertEqual("319", rule.cwe.cwe_id)
+        assert rule.default_config.enabled is True
+        assert rule.default_config.level == Level.ERROR
+        assert rule.default_config.rank == -1.0
+        assert rule.cwe.cwe_id == "319"
 
-    @parameterized.expand(
+    @pytest.mark.parametrize(
+        "filename",
         [
             "poplib_pop3_apop.py",
             "poplib_pop3_context_mgr.py",
             "poplib_pop3_pass_.py",
             "poplib_pop3_rpop.py",
             "poplib_pop3_ssl.py",
             "poplib_pop3_stls.py",
             "poplib_pop3_user.py",
-        ]
+        ],
     )
     def test(self, filename):
         self.check(filename)
```

### Comparing `precli-0.5.4/tests/unit/rules/python/stdlib/poplib/test_poplib_unverified_context.py` & `precli-0.5.5/tests/unit/rules/python/stdlib/argparse/test_argparse_sensitive_info.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,50 +1,51 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 import os
 
-from parameterized import parameterized
+import pytest
 
 from precli.core.level import Level
 from precli.parsers import python
 from precli.rules import Rule
 from tests.unit.rules import test_case
 
 
-class PoplibUnverifiedContextTests(test_case.TestCase):
-    def setUp(self):
-        super().setUp()
-        self.rule_id = "PY025"
-        self.parser = python.Python()
-        self.base_path = os.path.join(
+class TestArgparseSensitiveInfo(test_case.TestCase):
+    @classmethod
+    def setup_class(cls):
+        cls.rule_id = "PY027"
+        cls.parser = python.Python()
+        cls.base_path = os.path.join(
             "tests",
             "unit",
             "rules",
             "python",
             "stdlib",
-            "poplib",
+            "argparse",
             "examples",
         )
 
     def test_rule_meta(self):
         rule = Rule.get_by_id(self.rule_id)
-        self.assertEqual(self.rule_id, rule.id)
-        self.assertEqual("improper_certificate_validation", rule.name)
-        self.assertEqual(
-            f"https://docs.securesauce.dev/rules/{self.rule_id}", rule.help_url
+        assert rule.id == self.rule_id
+        assert rule.name == "visible_sensitive_information"
+        assert (
+            rule.help_url
+            == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
-        self.assertEqual(True, rule.default_config.enabled)
-        self.assertEqual(Level.WARNING, rule.default_config.level)
-        self.assertEqual(-1.0, rule.default_config.rank)
-        self.assertEqual("295", rule.cwe.cwe_id)
+        assert rule.default_config.enabled is True
+        assert rule.default_config.level == Level.ERROR
+        assert rule.default_config.rank == -1.0
+        assert rule.cwe.cwe_id == "214"
 
-    @parameterized.expand(
+    @pytest.mark.parametrize(
+        "filename",
         [
-            "poplib_pop3_ssl_context_as_var.py",
-            "poplib_pop3_ssl_context_none.py",
-            "poplib_pop3_ssl_context_unset.py",
-            "poplib_pop3_stls_context_as_var.py",
-            "poplib_pop3_stls_context_none.py",
-            "poplib_pop3_stls_context_unset.py",
-        ]
+            "argparse_add_argument_api_key.py",
+            "argparse_add_argument_default_action.py",
+            "argparse_add_argument_password.py",
+            "argparse_add_argument_password_file.py",
+            "argparse_add_argument_password_store_true.py",
+        ],
     )
     def test(self, filename):
         self.check(filename)
```

### Comparing `precli-0.5.4/tests/unit/rules/python/stdlib/re/test_re_denial_of_service.py` & `precli-0.5.5/tests/unit/rules/python/stdlib/tempfile/test_tempfile_mktemp_race_condition.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,55 +1,53 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2023 Secure Sauce LLC
 import os
 
-from parameterized import parameterized
+import pytest
 
 from precli.core.level import Level
 from precli.parsers import python
 from precli.rules import Rule
 from tests.unit.rules import test_case
 
 
-class ReDenialOfService(test_case.TestCase):
-    def setUp(self):
-        super().setUp()
-        self.rule_id = "PY033"
-        self.parser = python.Python()
-        self.base_path = os.path.join(
+class TestMktempRaceCondition(test_case.TestCase):
+    @classmethod
+    def setup_class(cls):
+        cls.rule_id = "PY021"
+        cls.parser = python.Python()
+        cls.base_path = os.path.join(
             "tests",
             "unit",
             "rules",
             "python",
             "stdlib",
-            "re",
+            "tempfile",
             "examples",
         )
 
     def test_rule_meta(self):
         rule = Rule.get_by_id(self.rule_id)
-        self.assertEqual(self.rule_id, rule.id)
-        self.assertEqual("regex_denial_of_service", rule.name)
-        self.assertEqual(
-            f"https://docs.securesauce.dev/rules/{self.rule_id}", rule.help_url
+        assert rule.id == self.rule_id
+        assert rule.name == "insecure_temporary_file"
+        assert (
+            rule.help_url
+            == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
-        self.assertEqual(True, rule.default_config.enabled)
-        self.assertEqual(Level.ERROR, rule.default_config.level)
-        self.assertEqual(-1.0, rule.default_config.rank)
-        self.assertEqual("1333", rule.cwe.cwe_id)
+        assert rule.default_config.enabled is True
+        assert rule.default_config.level == Level.WARNING
+        assert rule.default_config.rank == -1.0
+        assert rule.cwe.cwe_id == "377"
 
-    @parameterized.expand(
+    @pytest.mark.parametrize(
+        "filename",
         [
-            "re_compile.py",
-            "re_compile_good.py",
-            "re_search.py",
-            "re_search_good.py",
-            "re_match.py",
-            "re_fullmatch.py",
-            "re_split.py",
-            "re_findall.py",
-            "re_finditer.py",
-            "re_sub.py",
-            "re_subn.py",
-        ]
+            "tempfile_mktemp.py",
+            "tempfile_mktemp_args_open.py",
+            "tempfile_mktemp_args_with_open_args.py",
+            "tempfile_mktemp_open.py",
+            "tempfile_mktemp_walrus_open.py",
+            "tempfile_mktemp_with_open.py",
+            "tempfile_mktemp_with_open_multiline.py",
+        ],
     )
     def test(self, filename):
         self.check(filename)
```

### Comparing `precli-0.5.4/tests/unit/rules/python/stdlib/shelve/test_shelve_open.py` & `precli-0.5.5/tests/unit/rules/python/stdlib/http/test_http_url_secret.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,52 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 import os
 
-from parameterized import parameterized
+import pytest
 
 from precli.core.level import Level
 from precli.parsers import python
 from precli.rules import Rule
 from tests.unit.rules import test_case
 
 
-class ShelveOpenTests(test_case.TestCase):
-    def setUp(self):
-        super().setUp()
-        self.rule_id = "PY015"
-        self.parser = python.Python()
-        self.base_path = os.path.join(
+class TestHttpUrlSecret(test_case.TestCase):
+    @classmethod
+    def setup_class(cls):
+        cls.rule_id = "PY007"
+        cls.parser = python.Python()
+        cls.base_path = os.path.join(
             "tests",
             "unit",
             "rules",
             "python",
             "stdlib",
-            "shelve",
+            "http",
             "examples",
         )
 
     def test_rule_meta(self):
         rule = Rule.get_by_id(self.rule_id)
-        self.assertEqual(self.rule_id, rule.id)
-        self.assertEqual("deserialization_of_untrusted_data", rule.name)
-        self.assertEqual(
-            f"https://docs.securesauce.dev/rules/{self.rule_id}", rule.help_url
+        assert rule.id == self.rule_id
+        assert rule.name == "sensitive_query_strings"
+        assert (
+            rule.help_url
+            == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
-        self.assertEqual(True, rule.default_config.enabled)
-        self.assertEqual(Level.WARNING, rule.default_config.level)
-        self.assertEqual(-1.0, rule.default_config.rank)
-        self.assertEqual("502", rule.cwe.cwe_id)
+        assert rule.default_config.enabled is True
+        assert rule.default_config.level == Level.ERROR
+        assert rule.default_config.rank == -1.0
+        assert rule.cwe.cwe_id == "598"
 
-    @parameterized.expand(
+    @pytest.mark.parametrize(
+        "filename",
         [
-            "shelve_dbfilenameshelf.py",
-            "shelve_open.py",
-            "shelve_open_context_mgr.py",
-        ]
+            "http_url_secret_apikey.py",
+            "http_url_secret_apikey_in_header.py",
+            "http_url_secret_basic_auth.py",
+            "http_url_secret_basic_auth_as_var.py",
+            "http_url_secret_password.py",
+            "http_url_secret_username.py",
+        ],
     )
     def test(self, filename):
         self.check(filename)
```

### Comparing `precli-0.5.4/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_auth.py` & `precli-0.5.5/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_auth.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.4/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_login.py` & `precli-0.5.5/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_login.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.4/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl.py` & `precli-0.5.5/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.4/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl_context_as_var.py` & `precli-0.5.5/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl_context_as_var.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.4/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl_context_none.py` & `precli-0.5.5/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl_context_none.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.4/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl_context_unset.py` & `precli-0.5.5/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl_context_unset.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.4/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls.py` & `precli-0.5.5/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.4/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls_context_as_var.py` & `precli-0.5.5/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls_context_as_var.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.4/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls_context_none.py` & `precli-0.5.5/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls_context_none.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.4/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls_context_unset.py` & `precli-0.5.5/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls_context_unset.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.4/tests/unit/rules/python/stdlib/smtplib/test_smtplib_cleartext.py` & `precli-0.5.5/tests/unit/rules/python/stdlib/ftplib/test_ftplib_unverified_context.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 import os
 
-from parameterized import parameterized
+import pytest
 
 from precli.core.level import Level
 from precli.parsers import python
 from precli.rules import Rule
 from tests.unit.rules import test_case
 
 
-class SmtpCleartextTests(test_case.TestCase):
-    def setUp(self):
-        super().setUp()
-        self.rule_id = "PY016"
-        self.parser = python.Python()
-        self.base_path = os.path.join(
+class TestFtplibUnverifiedContext(test_case.TestCase):
+    @classmethod
+    def setup_class(cls):
+        cls.rule_id = "PY022"
+        cls.parser = python.Python()
+        cls.base_path = os.path.join(
             "tests",
             "unit",
             "rules",
             "python",
             "stdlib",
-            "smtplib",
+            "ftplib",
             "examples",
         )
 
     def test_rule_meta(self):
         rule = Rule.get_by_id(self.rule_id)
-        self.assertEqual(self.rule_id, rule.id)
-        self.assertEqual("cleartext_transmission", rule.name)
-        self.assertEqual(
-            f"https://docs.securesauce.dev/rules/{self.rule_id}", rule.help_url
+        assert rule.id == self.rule_id
+        assert rule.name == "improper_certificate_validation"
+        assert (
+            rule.help_url
+            == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
-        self.assertEqual(True, rule.default_config.enabled)
-        self.assertEqual(Level.ERROR, rule.default_config.level)
-        self.assertEqual(-1.0, rule.default_config.rank)
-        self.assertEqual("319", rule.cwe.cwe_id)
+        assert rule.default_config.enabled is True
+        assert rule.default_config.level == Level.WARNING
+        assert rule.default_config.rank == -1.0
+        assert rule.cwe.cwe_id == "295"
 
-    @parameterized.expand(
+    @pytest.mark.parametrize(
+        "filename",
         [
-            "smtplib_smtp_auth.py",
-            "smtplib_smtp_context_mgr.py",
-            "smtplib_smtp_login.py",
-            "smtplib_smtp_ssl.py",
-            "smtplib_smtp_starttls.py",
-        ]
+            "ftplib_ftp_tls_context_as_var.py",
+            "ftplib_ftp_tls_context_none.py",
+            "ftplib_ftp_tls_context_unset.py",
+        ],
     )
     def test(self, filename):
         self.check(filename)
```

### Comparing `precli-0.5.4/tests/unit/rules/python/stdlib/smtplib/test_smtplib_unverified_context.py` & `precli-0.5.5/tests/unit/rules/python/stdlib/smtplib/test_smtplib_cleartext.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,51 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 import os
 
-from parameterized import parameterized
+import pytest
 
 from precli.core.level import Level
 from precli.parsers import python
 from precli.rules import Rule
 from tests.unit.rules import test_case
 
 
-class SmtplibUnverifiedContextTests(test_case.TestCase):
-    def setUp(self):
-        super().setUp()
-        self.rule_id = "PY026"
-        self.parser = python.Python()
-        self.base_path = os.path.join(
+class TestSmtpCleartext(test_case.TestCase):
+    @classmethod
+    def setup_class(cls):
+        cls.rule_id = "PY016"
+        cls.parser = python.Python()
+        cls.base_path = os.path.join(
             "tests",
             "unit",
             "rules",
             "python",
             "stdlib",
             "smtplib",
             "examples",
         )
 
     def test_rule_meta(self):
         rule = Rule.get_by_id(self.rule_id)
-        self.assertEqual(self.rule_id, rule.id)
-        self.assertEqual("improper_certificate_validation", rule.name)
-        self.assertEqual(
-            f"https://docs.securesauce.dev/rules/{self.rule_id}", rule.help_url
+        assert rule.id == self.rule_id
+        assert rule.name == "cleartext_transmission"
+        assert (
+            rule.help_url
+            == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
-        self.assertEqual(True, rule.default_config.enabled)
-        self.assertEqual(Level.WARNING, rule.default_config.level)
-        self.assertEqual(-1.0, rule.default_config.rank)
-        self.assertEqual("295", rule.cwe.cwe_id)
+        assert rule.default_config.enabled is True
+        assert rule.default_config.level == Level.ERROR
+        assert rule.default_config.rank == -1.0
+        assert rule.cwe.cwe_id == "319"
 
-    @parameterized.expand(
+    @pytest.mark.parametrize(
+        "filename",
         [
-            "smtplib_smtp_ssl_context_as_var.py",
-            "smtplib_smtp_ssl_context_none.py",
-            "smtplib_smtp_ssl_context_unset.py",
-            "smtplib_smtp_starttls_context_as_var.py",
-            "smtplib_smtp_starttls_context_none.py",
-            "smtplib_smtp_starttls_context_unset.py",
-        ]
+            "smtplib_smtp_auth.py",
+            "smtplib_smtp_context_mgr.py",
+            "smtplib_smtp_login.py",
+            "smtplib_smtp_ssl.py",
+            "smtplib_smtp_starttls.py",
+        ],
     )
     def test(self, filename):
         self.check(filename)
```

### Comparing `precli-0.5.4/tests/unit/rules/python/stdlib/socket/test_socket_unrestricted_bind.py` & `precli-0.5.5/tests/unit/rules/python/stdlib/secrets/test_secrets_weak_token.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,48 +1,52 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 import os
 
-from parameterized import parameterized
+import pytest
 
 from precli.core.level import Level
 from precli.parsers import python
 from precli.rules import Rule
 from tests.unit.rules import test_case
 
 
-class SocketUnrestrictedBindTests(test_case.TestCase):
-    def setUp(self):
-        super().setUp()
-        self.rule_id = "PY029"
-        self.parser = python.Python()
-        self.base_path = os.path.join(
+class TestSecretsWeakToken(test_case.TestCase):
+    @classmethod
+    def setup_class(cls):
+        cls.rule_id = "PY028"
+        cls.parser = python.Python()
+        cls.base_path = os.path.join(
             "tests",
             "unit",
             "rules",
             "python",
             "stdlib",
-            "socket",
+            "secrets",
             "examples",
         )
 
     def test_rule_meta(self):
         rule = Rule.get_by_id(self.rule_id)
-        self.assertEqual(self.rule_id, rule.id)
-        self.assertEqual("unrestricted_bind", rule.name)
-        self.assertEqual(
-            f"https://docs.securesauce.dev/rules/{self.rule_id}", rule.help_url
+        assert rule.id == self.rule_id
+        assert rule.name == "insufficient_token_length"
+        assert (
+            rule.help_url
+            == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
-        self.assertEqual(True, rule.default_config.enabled)
-        self.assertEqual(Level.WARNING, rule.default_config.level)
-        self.assertEqual(-1.0, rule.default_config.rank)
-        self.assertEqual("1327", rule.cwe.cwe_id)
+        assert rule.default_config.enabled is True
+        assert rule.default_config.level == Level.WARNING
+        assert rule.default_config.rank == -1.0
+        assert rule.cwe.cwe_id == "326"
 
-    @parameterized.expand(
+    @pytest.mark.parametrize(
+        "filename",
         [
-            "socket_create_server.py",
-            "socket_socket_bind.py",
-            "socket_socket_bind_as_var.py",
-            "socket_socket_bind_as_vars.py",
-        ]
+            "secrets_token_bytes.py",
+            "secrets_token_bytes_default.py",
+            "secrets_token_bytes_size_var.py",
+            "secrets_token_hex.py",
+            "secrets_token_hex_nbytes_unknown.py",
+            "secrets_token_urlsafe.py",
+        ],
     )
     def test(self, filename):
         self.check(filename)
```

### Comparing `precli-0.5.4/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_forking_tcp_server.py` & `precli-0.5.5/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_forking_tcp_server.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.4/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_forking_udp_server.py` & `precli-0.5.5/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_forking_udp_server.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.4/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_tcp_server.py` & `precli-0.5.5/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_tcp_server.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.4/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_threading_tcp_server.py` & `precli-0.5.5/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_threading_tcp_server.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.4/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_threading_udp_server.py` & `precli-0.5.5/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_threading_udp_server.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.4/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_udp_server.py` & `precli-0.5.5/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_udp_server.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.4/tests/unit/rules/python/stdlib/ssl/test_ssl_context_tls_version.py` & `precli-0.5.5/tests/unit/rules/python/stdlib/hmac/test_hmac_timing_attack.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2023 Secure Sauce LLC
 import os
 
-from parameterized import parameterized
+import pytest
 
 from precli.core.level import Level
 from precli.parsers import python
 from precli.rules import Rule
 from tests.unit.rules import test_case
 
 
-class SslSocketTlsVersionTests(test_case.TestCase):
-    def setUp(self):
-        super().setUp()
-        self.rule_id = "PY018"
-        self.parser = python.Python()
-        self.base_path = os.path.join(
+class TestHmacTimingAttack(test_case.TestCase):
+    @classmethod
+    def setup_class(cls):
+        cls.rule_id = "PY005"
+        cls.parser = python.Python()
+        cls.base_path = os.path.join(
             "tests",
             "unit",
             "rules",
             "python",
             "stdlib",
-            "ssl",
+            "hmac",
             "examples",
         )
 
     def test_rule_meta(self):
         rule = Rule.get_by_id(self.rule_id)
-        self.assertEqual(self.rule_id, rule.id)
-        self.assertEqual("inadequate_encryption_strength", rule.name)
-        self.assertEqual(
-            f"https://docs.securesauce.dev/rules/{self.rule_id}", rule.help_url
+        assert rule.id == self.rule_id
+        assert rule.name == "observable_timing_discrepancy"
+        assert (
+            rule.help_url
+            == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
-        self.assertEqual(True, rule.default_config.enabled)
-        self.assertEqual(Level.ERROR, rule.default_config.level)
-        self.assertEqual(-1.0, rule.default_config.rank)
-        self.assertEqual("326", rule.cwe.cwe_id)
+        assert rule.default_config.enabled is True
+        assert rule.default_config.level == Level.ERROR
+        assert rule.default_config.rank == -1.0
+        assert rule.cwe.cwe_id == "208"
 
-    @parameterized.expand(
+    @pytest.mark.parametrize(
+        "filename",
         [
-            "ssl_context_sslv2.py",
-            "ssl_context_sslv23.py",
-            "ssl_context_sslv3.py",
-            "ssl_context_tlsv1.py",
-            "ssl_context_tlsv11.py",
-            "ssl_context_tlsv12.py",
-        ]
+            "hmac_timing_attack.py",
+            "hmac_timing_attack_class.py",
+            "hmac_timing_attack_class_hexdigest.py",
+            "hmac_timing_attack_compare_digest.py",
+        ],
     )
     def test(self, filename):
         self.check(filename)
```

### Comparing `precli-0.5.4/tests/unit/rules/python/stdlib/ssl/test_ssl_context_weak_key.py` & `precli-0.5.5/tests/unit/rules/python/stdlib/ssl/test_ssl_context_weak_key.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,48 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 import os
 
-from parameterized import parameterized
+import pytest
 
 from precli.core.level import Level
 from precli.parsers import python
 from precli.rules import Rule
 from tests.unit.rules import test_case
 
 
-class SslSocketWeakKeyTests(test_case.TestCase):
-    def setUp(self):
-        super().setUp()
-        self.rule_id = "PY019"
-        self.parser = python.Python()
-        self.base_path = os.path.join(
+class TestSslSocketWeakKey(test_case.TestCase):
+    @classmethod
+    def setup_class(cls):
+        cls.rule_id = "PY019"
+        cls.parser = python.Python()
+        cls.base_path = os.path.join(
             "tests",
             "unit",
             "rules",
             "python",
             "stdlib",
             "ssl",
             "examples",
         )
 
     def test_rule_meta(self):
         rule = Rule.get_by_id(self.rule_id)
-        self.assertEqual(self.rule_id, rule.id)
-        self.assertEqual("inadequate_encryption_strength", rule.name)
-        self.assertEqual(
-            f"https://docs.securesauce.dev/rules/{self.rule_id}", rule.help_url
+        assert rule.id == self.rule_id
+        assert rule.name == "inadequate_encryption_strength"
+        assert (
+            rule.help_url
+            == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
-        self.assertEqual(True, rule.default_config.enabled)
-        self.assertEqual(Level.WARNING, rule.default_config.level)
-        self.assertEqual(-1.0, rule.default_config.rank)
-        self.assertEqual("326", rule.cwe.cwe_id)
+        assert rule.default_config.enabled is True
+        assert rule.default_config.level == Level.WARNING
+        assert rule.default_config.rank == -1.0
+        assert rule.cwe.cwe_id == "326"
 
-    @parameterized.expand(
+    @pytest.mark.parametrize(
+        "filename",
         [
             "ssl_context_set_ecdh_curve_brainpoolP256r1.py",
             "ssl_context_set_ecdh_curve_brainpoolP384r1.py",
             "ssl_context_set_ecdh_curve_brainpoolP384r1tls13.py",
             "ssl_context_set_ecdh_curve_brainpoolP512r1.py",
             "ssl_context_set_ecdh_curve_default_context.py",
             "ssl_context_set_ecdh_curve_ffdhe2048.py",
@@ -49,11 +51,11 @@
             "ssl_context_set_ecdh_curve_secp160r2.py",
             "ssl_context_set_ecdh_curve_secp256r1.py",
             "ssl_context_set_ecdh_curve_sect163k1.py",
             "ssl_context_set_ecdh_curve_sect571k1.py",
             "ssl_context_set_ecdh_curve_typed_default_param.py",
             "ssl_context_set_ecdh_curve_typed_param.py",
             "ssl_context_set_ecdh_curve_unverified_context.py",
-        ]
+        ],
     )
     def test(self, filename):
         self.check(filename)
```

### Comparing `precli-0.5.4/tests/unit/rules/python/stdlib/ssl/test_ssl_create_context.py` & `precli-0.5.5/tests/unit/rules/python/stdlib/marshal/test_marshal_load.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,46 +1,48 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 import os
 
-from parameterized import parameterized
+import pytest
 
 from precli.core.level import Level
 from precli.parsers import python
 from precli.rules import Rule
 from tests.unit.rules import test_case
 
 
-class SslCreateContextTests(test_case.TestCase):
-    def setUp(self):
-        super().setUp()
-        self.rule_id = "PY017"
-        self.parser = python.Python()
-        self.base_path = os.path.join(
+class TestMarshalLoad(test_case.TestCase):
+    @classmethod
+    def setup_class(cls):
+        cls.rule_id = "PY011"
+        cls.parser = python.Python()
+        cls.base_path = os.path.join(
             "tests",
             "unit",
             "rules",
             "python",
             "stdlib",
-            "ssl",
+            "marshal",
             "examples",
         )
 
     def test_rule_meta(self):
         rule = Rule.get_by_id(self.rule_id)
-        self.assertEqual(self.rule_id, rule.id)
-        self.assertEqual("improper_certificate_validation", rule.name)
-        self.assertEqual(
-            f"https://docs.securesauce.dev/rules/{self.rule_id}", rule.help_url
+        assert rule.id == self.rule_id
+        assert rule.name == "deserialization_of_untrusted_data"
+        assert (
+            rule.help_url
+            == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
-        self.assertEqual(True, rule.default_config.enabled)
-        self.assertEqual(Level.WARNING, rule.default_config.level)
-        self.assertEqual(-1.0, rule.default_config.rank)
-        self.assertEqual("295", rule.cwe.cwe_id)
+        assert rule.default_config.enabled is True
+        assert rule.default_config.level == Level.WARNING
+        assert rule.default_config.rank == -1.0
+        assert rule.cwe.cwe_id == "502"
 
-    @parameterized.expand(
+    @pytest.mark.parametrize(
+        "filename",
         [
-            "create_default_context.py",
-            "create_unverified_context.py",
-        ]
+            "marshal_load.py",
+            "marshal_loads.py",
+        ],
     )
     def test(self, filename):
         self.check(filename)
```

### Comparing `precli-0.5.4/tests/unit/rules/python/stdlib/ssl/test_ssl_get_server_certificate_tls_version.py` & `precli-0.5.5/tests/unit/rules/java/stdlib/java_security/test_weak_key.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,50 +1,48 @@
-# Copyright 2023 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 import os
 
-from parameterized import parameterized
+import pytest
 
 from precli.core.level import Level
-from precli.parsers import python
+from precli.parsers import java
 from precli.rules import Rule
 from tests.unit.rules import test_case
 
 
-class GetServerCertificateTests(test_case.TestCase):
-    def setUp(self):
-        super().setUp()
-        self.rule_id = "PY018"
-        self.parser = python.Python()
-        self.base_path = os.path.join(
+class TestKeyPairGeneratorWeakkey(test_case.TestCase):
+    @classmethod
+    def setup_class(cls):
+        cls.rule_id = "JAV003"
+        cls.parser = java.Java()
+        cls.base_path = os.path.join(
             "tests",
             "unit",
             "rules",
-            "python",
+            "java",
             "stdlib",
-            "ssl",
+            "java_security",
             "examples",
         )
 
     def test_rule_meta(self):
         rule = Rule.get_by_id(self.rule_id)
-        self.assertEqual(self.rule_id, rule.id)
-        self.assertEqual("inadequate_encryption_strength", rule.name)
-        self.assertEqual(
-            f"https://docs.securesauce.dev/rules/{self.rule_id}", rule.help_url
+        assert rule.id == self.rule_id
+        assert rule.name == "inadequate_encryption_strength"
+        assert (
+            rule.help_url
+            == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
-        self.assertEqual(True, rule.default_config.enabled)
-        self.assertEqual(Level.ERROR, rule.default_config.level)
-        self.assertEqual(-1.0, rule.default_config.rank)
-        self.assertEqual("326", rule.cwe.cwe_id)
+        assert rule.default_config.enabled is True
+        assert rule.default_config.level == Level.WARNING
+        assert rule.default_config.rank == -1.0
+        assert rule.cwe.cwe_id == "326"
 
-    @parameterized.expand(
+    @pytest.mark.parametrize(
+        "filename",
         [
-            "get_server_certificate_sslv2.py",
-            "get_server_certificate_sslv23.py",
-            "get_server_certificate_sslv3.py",
-            "get_server_certificate_tlsv1.py",
-            "get_server_certificate_tlsv11.py",
-            "get_server_certificate_tlsv12.py",
-        ]
+            "KeyPairGeneratorDSA.java",
+            "KeyPairGeneratorRSA.java",
+        ],
     )
     def test(self, filename):
         self.check(filename)
```

### Comparing `precli-0.5.4/tests/unit/rules/python/stdlib/ssl/test_ssl_wrap_socket_tls_version.py` & `precli-0.5.5/tests/unit/rules/python/stdlib/re/test_re_denial_of_service.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,51 +1,57 @@
-# Copyright 2023 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 import os
 
-from parameterized import parameterized
+import pytest
 
 from precli.core.level import Level
 from precli.parsers import python
 from precli.rules import Rule
 from tests.unit.rules import test_case
 
 
-class WrapSocketTests(test_case.TestCase):
-    def setUp(self):
-        super().setUp()
-        self.rule_id = "PY018"
-        self.parser = python.Python()
-        self.base_path = os.path.join(
+class TestReDenialOfService(test_case.TestCase):
+    @classmethod
+    def setup_class(cls):
+        cls.rule_id = "PY033"
+        cls.parser = python.Python()
+        cls.base_path = os.path.join(
             "tests",
             "unit",
             "rules",
             "python",
             "stdlib",
-            "ssl",
+            "re",
             "examples",
         )
 
     def test_rule_meta(self):
         rule = Rule.get_by_id(self.rule_id)
-        self.assertEqual(self.rule_id, rule.id)
-        self.assertEqual("inadequate_encryption_strength", rule.name)
-        self.assertEqual(
-            f"https://docs.securesauce.dev/rules/{self.rule_id}", rule.help_url
+        assert rule.id == self.rule_id
+        assert rule.name == "regex_denial_of_service"
+        assert (
+            rule.help_url
+            == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
-        self.assertEqual(True, rule.default_config.enabled)
-        self.assertEqual(Level.ERROR, rule.default_config.level)
-        self.assertEqual(-1.0, rule.default_config.rank)
-        self.assertEqual("326", rule.cwe.cwe_id)
+        assert rule.default_config.enabled is True
+        assert rule.default_config.level == Level.ERROR
+        assert rule.default_config.rank == -1.0
+        assert rule.cwe.cwe_id == "1333"
 
-    @parameterized.expand(
+    @pytest.mark.parametrize(
+        "filename",
         [
-            "wrap_socket_sslv2.py",
-            "wrap_socket_sslv23.py",
-            "wrap_socket_sslv2_server_side_true.py",
-            "wrap_socket_sslv3.py",
-            "wrap_socket_tlsv1.py",
-            "wrap_socket_tlsv11.py",
-            "wrap_socket_tlsv12.py",
-        ]
+            "re_compile.py",
+            "re_compile_good.py",
+            "re_search.py",
+            "re_search_good.py",
+            "re_match.py",
+            "re_fullmatch.py",
+            "re_split.py",
+            "re_findall.py",
+            "re_finditer.py",
+            "re_sub.py",
+            "re_subn.py",
+        ],
     )
     def test(self, filename):
         self.check(filename)
```

### Comparing `precli-0.5.4/tests/unit/rules/python/stdlib/telnetlib/test_telnetlib_cleartext.py` & `precli-0.5.5/tests/unit/rules/python/stdlib/socketserver/test_socketserver_unrestricted_bind.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,47 +1,52 @@
-# Copyright 2023 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 import os
 
-from parameterized import parameterized
+import pytest
 
 from precli.core.level import Level
 from precli.parsers import python
 from precli.rules import Rule
 from tests.unit.rules import test_case
 
 
-class TelnetlibCleartextTests(test_case.TestCase):
-    def setUp(self):
-        super().setUp()
-        self.rule_id = "PY020"
-        self.parser = python.Python()
-        self.base_path = os.path.join(
+class TestSocketserverUnrestrictedBind(test_case.TestCase):
+    @classmethod
+    def setup_class(cls):
+        cls.rule_id = "PY030"
+        cls.parser = python.Python()
+        cls.base_path = os.path.join(
             "tests",
             "unit",
             "rules",
             "python",
             "stdlib",
-            "telnetlib",
+            "socketserver",
             "examples",
         )
 
     def test_rule_meta(self):
         rule = Rule.get_by_id(self.rule_id)
-        self.assertEqual(self.rule_id, rule.id)
-        self.assertEqual("cleartext_transmission", rule.name)
-        self.assertEqual(
-            f"https://docs.securesauce.dev/rules/{self.rule_id}", rule.help_url
+        assert rule.id == self.rule_id
+        assert rule.name == "unrestricted_bind"
+        assert (
+            rule.help_url
+            == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
-        self.assertEqual(True, rule.default_config.enabled)
-        self.assertEqual(Level.ERROR, rule.default_config.level)
-        self.assertEqual(-1.0, rule.default_config.rank)
-        self.assertEqual("319", rule.cwe.cwe_id)
+        assert rule.default_config.enabled is True
+        assert rule.default_config.level == Level.WARNING
+        assert rule.default_config.rank == -1.0
+        assert rule.cwe.cwe_id == "1327"
 
-    @parameterized.expand(
+    @pytest.mark.parametrize(
+        "filename",
         [
-            "telnet.py",
-            "telnetlib_telnet.py",
-            "telnetlib_telnet_context_mgr.py",
-        ]
+            "socketserver_tcp_server.py",
+            "socketserver_udp_server.py",
+            "socketserver_forking_tcp_server.py",
+            "socketserver_forking_udp_server.py",
+            "socketserver_threading_tcp_server.py",
+            "socketserver_threading_udp_server.py",
+        ],
     )
     def test(self, filename):
         self.check(filename)
```

### Comparing `precli-0.5.4/tox.ini` & `precli-0.5.5/tox.ini`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# Copyright 2024 Secure Saurce LLC
+# Copyright 2024 Secure Sauce LLC
 
 [tox]
 minversion = 3.2.0
 envlist = py312
 
 [testenv]
 usedevelop = True
 install_command = pip install {opts} {packages}
 setenv =
     VIRTUAL_ENV={envdir}
 deps =
        -r{toxinidir}/requirements.txt
        -r{toxinidir}/test-requirements.txt
 commands =
-    stestr run {posargs}
+    pytest {posargs}
 passenv = http_proxy, HTTP_PROXY, https_proxy, HTTPS_PROXY, no_proxy, NO_PROXY
 
 [testenv:format]
 skip_install = true
 deps =
     pre-commit
 commands =
@@ -40,7 +40,13 @@
 commands =
     mkdocs build
 
 [testenv:clean]
 skip_install = true
 deps = pyclean
 commands = pyclean {posargs:. --debris}
+
+[pytest]
+minversion = 6.0
+addopts = -v
+testpaths =
+    tests
```

