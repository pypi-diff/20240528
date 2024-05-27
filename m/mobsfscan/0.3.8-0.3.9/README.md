# Comparing `tmp/mobsfscan-0.3.8.tar.gz` & `tmp/mobsfscan-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mobsfscan-0.3.8.tar", last modified: Fri Mar 22 23:50:53 2024, max compression
+gzip compressed data, was "mobsfscan-0.3.9.tar", last modified: Mon May 27 22:28:30 2024, max compression
```

## Comparing `mobsfscan-0.3.8.tar` & `mobsfscan-0.3.9.tar`

### file list

```diff
@@ -1,89 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 23:50:53.035246 mobsfscan-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    25978 2024-03-22 23:50:53.035246 mobsfscan-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    25164 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 23:50:53.027246 mobsfscan-0.3.8/mobsfscan/
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 23:50:53.027246 mobsfscan-0.3.8/mobsfscan/formatters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/formatters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/formatters/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/formatters/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     6041 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/formatters/sarif.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/formatters/sonarqube.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    14166 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)    13460 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/manifest_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     8675 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/mobsfscan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 23:50:53.023246 mobsfscan-0.3.8/mobsfscan/rules/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 23:50:53.023246 mobsfscan-0.3.8/mobsfscan/rules/patterns/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 23:50:53.023246 mobsfscan-0.3.8/mobsfscan/rules/patterns/android/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 23:50:53.027246 mobsfscan-0.3.8/mobsfscan/rules/patterns/android/kotlin/
--rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/rules/patterns/android/kotlin/best_practices.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    12404 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/rules/patterns/android/kotlin/kotlin_rules.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 23:50:53.023246 mobsfscan-0.3.8/mobsfscan/rules/patterns/ios/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 23:50:53.027246 mobsfscan-0.3.8/mobsfscan/rules/patterns/ios/objectivec/
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/rules/patterns/ios/objectivec/best_practices.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/rules/patterns/ios/objectivec/objective_c_rules.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 23:50:53.027246 mobsfscan-0.3.8/mobsfscan/rules/patterns/ios/swift/
--rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/rules/patterns/ios/swift/best_practices.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8719 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/rules/patterns/ios/swift/swift_rules.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 23:50:53.023246 mobsfscan-0.3.8/mobsfscan/rules/semgrep/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 23:50:53.031246 mobsfscan-0.3.8/mobsfscan/rules/semgrep/android/
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/rules/semgrep/android/hidden_ui.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/rules/semgrep/android/logging.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/rules/semgrep/android/secrets.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/rules/semgrep/android/word_readable_writable.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 23:50:53.031246 mobsfscan-0.3.8/mobsfscan/rules/semgrep/best_practices/
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/rules/semgrep/best_practices/android_safetynetapi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/rules/semgrep/best_practices/flag_secure.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/rules/semgrep/best_practices/root_detection.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/rules/semgrep/best_practices/tapjacking.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/rules/semgrep/best_practices/tls_certificate_transparency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/rules/semgrep/best_practices/tls_pinning.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 23:50:53.031246 mobsfscan-0.3.8/mobsfscan/rules/semgrep/crypto/
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/rules/semgrep/crypto/aes_ecb.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/rules/semgrep/crypto/aes_encryption_keys.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/rules/semgrep/crypto/cbc_padding_oracle.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/rules/semgrep/crypto/cbc_static_iv.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/rules/semgrep/crypto/insecure_random.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/rules/semgrep/crypto/insecure_ssl_v3.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/rules/semgrep/crypto/rsa_no_oeap.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/rules/semgrep/crypto/sha1_hash.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/rules/semgrep/crypto/weak_ciphers.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/rules/semgrep/crypto/weak_hashes.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/rules/semgrep/crypto/weak_iv.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/rules/semgrep/crypto/weak_key_size.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 23:50:53.035246 mobsfscan-0.3.8/mobsfscan/rules/semgrep/deserialization/
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/rules/semgrep/deserialization/jackson_deserialization.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/rules/semgrep/deserialization/object_deserialization.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 23:50:53.035246 mobsfscan-0.3.8/mobsfscan/rules/semgrep/injection/
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/rules/semgrep/injection/command_injection.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/rules/semgrep/injection/command_injection_formated.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/rules/semgrep/injection/sqlite_injection.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 23:50:53.035246 mobsfscan-0.3.8/mobsfscan/rules/semgrep/network/
--rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/rules/semgrep/network/accept_self_signed.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/rules/semgrep/network/default_http_client_tls.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 23:50:53.035246 mobsfscan-0.3.8/mobsfscan/rules/semgrep/webview/
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/rules/semgrep/webview/webview_debugging.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/rules/semgrep/webview/webview_external_storage.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/rules/semgrep/webview/webview_file_access.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/rules/semgrep/webview/webview_ignore_ssl_errors.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/rules/semgrep/webview/webview_javascript_interface.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 23:50:53.035246 mobsfscan-0.3.8/mobsfscan/rules/semgrep/xxe/
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/rules/semgrep/xxe/xmldecoder_xxe.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/rules/semgrep/xxe/xmlfactory_external_entities_enabled.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/rules/semgrep/xxe/xmlfactory_xxe.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/mobsfscan/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 23:50:53.035246 mobsfscan-0.3.8/mobsfscan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    25978 2024-03-22 23:50:52.000000 mobsfscan-0.3.8/mobsfscan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-03-22 23:50:52.000000 mobsfscan-0.3.8/mobsfscan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 23:50:52.000000 mobsfscan-0.3.8/mobsfscan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-22 23:50:52.000000 mobsfscan-0.3.8/mobsfscan.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-22 23:50:52.000000 mobsfscan-0.3.8/mobsfscan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-22 23:50:52.000000 mobsfscan-0.3.8/mobsfscan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 23:50:53.035246 mobsfscan-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-03-22 23:50:44.000000 mobsfscan-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:28:30.220006 mobsfscan-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    25978 2024-05-27 22:28:30.220006 mobsfscan-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    25164 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:28:30.212006 mobsfscan-0.3.9/mobsfscan/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:28:30.212006 mobsfscan-0.3.9/mobsfscan/formatters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/formatters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/formatters/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/formatters/json_fmt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6041 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/formatters/sarif.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/formatters/sonarqube.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14260 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13460 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/manifest_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8675 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/mobsfscan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:28:30.208006 mobsfscan-0.3.9/mobsfscan/rules/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:28:30.208006 mobsfscan-0.3.9/mobsfscan/rules/patterns/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:28:30.208006 mobsfscan-0.3.9/mobsfscan/rules/patterns/android/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:28:30.212006 mobsfscan-0.3.9/mobsfscan/rules/patterns/android/kotlin/
+-rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/rules/patterns/android/kotlin/best_practices.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13046 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/rules/patterns/android/kotlin/kotlin_rules.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:28:30.208006 mobsfscan-0.3.9/mobsfscan/rules/patterns/ios/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:28:30.212006 mobsfscan-0.3.9/mobsfscan/rules/patterns/ios/objectivec/
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/rules/patterns/ios/objectivec/best_practices.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/rules/patterns/ios/objectivec/objective_c_rules.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:28:30.212006 mobsfscan-0.3.9/mobsfscan/rules/patterns/ios/swift/
+-rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/rules/patterns/ios/swift/best_practices.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8719 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/rules/patterns/ios/swift/swift_rules.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:28:30.208006 mobsfscan-0.3.9/mobsfscan/rules/semgrep/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:28:30.216006 mobsfscan-0.3.9/mobsfscan/rules/semgrep/android/
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/rules/semgrep/android/hidden_ui.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/rules/semgrep/android/logging.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/rules/semgrep/android/secrets.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/rules/semgrep/android/word_readable_writable.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:28:30.216006 mobsfscan-0.3.9/mobsfscan/rules/semgrep/best_practices/
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/rules/semgrep/best_practices/android_safetynetapi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/rules/semgrep/best_practices/flag_secure.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/rules/semgrep/best_practices/root_detection.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/rules/semgrep/best_practices/tapjacking.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/rules/semgrep/best_practices/tls_certificate_transparency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/rules/semgrep/best_practices/tls_pinning.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:28:30.216006 mobsfscan-0.3.9/mobsfscan/rules/semgrep/crypto/
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/rules/semgrep/crypto/aes_ecb.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/rules/semgrep/crypto/aes_encryption_keys.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/rules/semgrep/crypto/cbc_padding_oracle.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/rules/semgrep/crypto/cbc_static_iv.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/rules/semgrep/crypto/insecure_random.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/rules/semgrep/crypto/insecure_ssl_v3.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/rules/semgrep/crypto/rsa_no_oeap.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/rules/semgrep/crypto/sha1_hash.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/rules/semgrep/crypto/weak_ciphers.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/rules/semgrep/crypto/weak_hashes.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/rules/semgrep/crypto/weak_iv.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/rules/semgrep/crypto/weak_key_size.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:28:30.216006 mobsfscan-0.3.9/mobsfscan/rules/semgrep/deserialization/
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/rules/semgrep/deserialization/jackson_deserialization.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/rules/semgrep/deserialization/object_deserialization.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:28:30.220006 mobsfscan-0.3.9/mobsfscan/rules/semgrep/injection/
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/rules/semgrep/injection/command_injection.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/rules/semgrep/injection/command_injection_formated.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/rules/semgrep/injection/sqlite_injection.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:28:30.220006 mobsfscan-0.3.9/mobsfscan/rules/semgrep/network/
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/rules/semgrep/network/accept_self_signed.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/rules/semgrep/network/default_http_client_tls.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:28:30.220006 mobsfscan-0.3.9/mobsfscan/rules/semgrep/webview/
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/rules/semgrep/webview/webview_allow_file_from_url.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/rules/semgrep/webview/webview_debugging.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/rules/semgrep/webview/webview_external_storage.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/rules/semgrep/webview/webview_file_access.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/rules/semgrep/webview/webview_ignore_ssl_errors.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/rules/semgrep/webview/webview_javascript_interface.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:28:30.220006 mobsfscan-0.3.9/mobsfscan/rules/semgrep/xxe/
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/rules/semgrep/xxe/xmldecoder_xxe.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/rules/semgrep/xxe/xmlfactory_external_entities_enabled.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/rules/semgrep/xxe/xmlfactory_xxe.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/mobsfscan/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 22:28:30.220006 mobsfscan-0.3.9/mobsfscan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    25978 2024-05-27 22:28:30.000000 mobsfscan-0.3.9/mobsfscan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-05-27 22:28:30.000000 mobsfscan-0.3.9/mobsfscan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 22:28:30.000000 mobsfscan-0.3.9/mobsfscan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-27 22:28:30.000000 mobsfscan-0.3.9/mobsfscan.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-27 22:28:30.000000 mobsfscan-0.3.9/mobsfscan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-27 22:28:30.000000 mobsfscan-0.3.9/mobsfscan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 22:28:30.220006 mobsfscan-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-05-27 22:28:22.000000 mobsfscan-0.3.9/setup.py
```

### Comparing `mobsfscan-0.3.8/LICENSE` & `mobsfscan-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mobsfscan-0.3.8/PKG-INFO` & `mobsfscan-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mobsfscan
-Version: 0.3.8
+Version: 0.3.9
 Summary: mobsfscan is a static analysis tool that can find insecure code patterns in your Android and iOS source code. Supports Java, Kotlin, Swift, and Objective C Code.
 Home-page: https://github.com/MobSF/mobsfscan
 Author: Ajin Abraham
 Author-email: ajin25@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

### Comparing `mobsfscan-0.3.8/README.md` & `mobsfscan-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `mobsfscan-0.3.8/mobsfscan/__main__.py` & `mobsfscan-0.3.9/mobsfscan/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import argparse
 import sys
 
 from mobsfscan import __version__
 from mobsfscan.mobsfscan import MobSFScan
 from mobsfscan.formatters import (
     cli,
-    json,
+    json_fmt,
     sarif,
     sonarqube,
 )
 
 
 def handle_exit(results, exit_warn, no_fail):
     """Handle Exit."""
@@ -83,15 +83,15 @@
         ).scan()
         if args.sonarqube:
             sonarqube.sonarqube_output(
                 args.output,
                 scan_results,
                 __version__)
         elif args.json:
-            json.json_output(
+            json_fmt.json_output(
                 args.output,
                 scan_results,
                 __version__)
         elif args.sarif:
             sarif.sarif_output(
                 args.output,
                 scan_results,
```

### Comparing `mobsfscan-0.3.8/mobsfscan/formatters/cli.py` & `mobsfscan-0.3.9/mobsfscan/formatters/cli.py`

 * *Files identical despite different names*

### Comparing `mobsfscan-0.3.8/mobsfscan/formatters/sarif.py` & `mobsfscan-0.3.9/mobsfscan/formatters/sarif.py`

 * *Files identical despite different names*

### Comparing `mobsfscan-0.3.8/mobsfscan/formatters/sonarqube.py` & `mobsfscan-0.3.9/mobsfscan/formatters/sonarqube.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf_8 -*-
 """Sonarqube output format."""
 
-from mobsfscan.formatters.json import json_output
+from mobsfscan.formatters.json_fmt import json_output
 
 
 def get_sonarqube_issue(mobsfscan_issue):
     sonarqube_severity_mapping = {
         'ERROR': 'CRITICAL',
         'WARNING': 'MAJOR',
         'INFO': 'INFO',
```

### Comparing `mobsfscan-0.3.8/mobsfscan/logger.py` & `mobsfscan-0.3.9/mobsfscan/logger.py`

 * *Files identical despite different names*

### Comparing `mobsfscan-0.3.8/mobsfscan/manifest.py` & `mobsfscan-0.3.9/mobsfscan/manifest.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,19 @@
     '29': '10',
     '30': '11',
     '31': '12',
     '32': '12L',
     '33': '13',
     '34': '14',
     '35': '15',
+    '36': '16',
+    '37': '17',  # Guess work
+    '38': '18',
+    '39': '19',
+    '40': '20',
 }
 
 
 def scan_manifest(xml_paths, validate_func):
     """Scan android manifest xml."""
     results = []
     p = None
```

### Comparing `mobsfscan-0.3.8/mobsfscan/manifest_metadata.py` & `mobsfscan-0.3.9/mobsfscan/manifest_metadata.py`

 * *Files identical despite different names*

### Comparing `mobsfscan-0.3.8/mobsfscan/mobsfscan.py` & `mobsfscan-0.3.9/mobsfscan/mobsfscan.py`

 * *Files identical despite different names*

### Comparing `mobsfscan-0.3.8/mobsfscan/rules/patterns/android/kotlin/best_practices.yaml` & `mobsfscan-0.3.9/mobsfscan/rules/patterns/android/kotlin/best_practices.yaml`

 * *Files identical despite different names*

### Comparing `mobsfscan-0.3.8/mobsfscan/rules/patterns/android/kotlin/kotlin_rules.yaml` & `mobsfscan-0.3.9/mobsfscan/rules/patterns/android/kotlin/kotlin_rules.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -76,14 +76,31 @@
   severity: WARNING
   input_case: exact
   metadata:
     cwe: cwe-749
     owasp-mobile: m1
     masvs: platform-7
     reference: https://github.com/MobSF/owasp-mstg/blob/master/Document/0x05h-Testing-Platform-Interaction.md#testing-javascript-execution-in-webviews-mstg-platform-5
+- id: android_kotlin_webview_allow_file_from_url
+  message: >-
+    Ensure that user controlled URLs never reaches the Webview. Enabling file access
+    from URLs in WebView can leak sensitive information from the file system.
+  type: RegexAndOr
+  pattern:
+    - setJavaScriptEnabled\(true\)
+    - - \.setAllowFileAccessFromFileURLs\(true\)
+      - \.setAllowUniversalAccessFromFileURLs\(true\)
+  severity: warning
+  input_case: exact
+  metadata:
+    cvss: 6.1
+    cwe: cwe-200
+    owasp-mobile: m1
+    masvs: platform-7
+    ref: https://github.com/MobSF/owasp-mstg/blob/master/Document/0x05h-Testing-Platform-Interaction.md#static-analysis-6
 - id: android_kotlin_webview_debug
   message: Remote WebView debugging is enabled.
   type: RegexAnd
   pattern:
     - \.setWebContentsDebuggingEnabled\(true\)
     - WebView
   severity: ERROR
```

### Comparing `mobsfscan-0.3.8/mobsfscan/rules/patterns/ios/objectivec/best_practices.yaml` & `mobsfscan-0.3.9/mobsfscan/rules/patterns/ios/objectivec/best_practices.yaml`

 * *Files identical despite different names*

### Comparing `mobsfscan-0.3.8/mobsfscan/rules/patterns/ios/objectivec/objective_c_rules.yaml` & `mobsfscan-0.3.9/mobsfscan/rules/patterns/ios/objectivec/objective_c_rules.yaml`

 * *Files identical despite different names*

### Comparing `mobsfscan-0.3.8/mobsfscan/rules/patterns/ios/swift/best_practices.yaml` & `mobsfscan-0.3.9/mobsfscan/rules/patterns/ios/swift/best_practices.yaml`

 * *Files identical despite different names*

### Comparing `mobsfscan-0.3.8/mobsfscan/rules/patterns/ios/swift/swift_rules.yaml` & `mobsfscan-0.3.9/mobsfscan/rules/patterns/ios/swift/swift_rules.yaml`

 * *Files identical despite different names*

### Comparing `mobsfscan-0.3.8/mobsfscan/rules/semgrep/android/hidden_ui.yaml` & `mobsfscan-0.3.9/mobsfscan/rules/semgrep/android/hidden_ui.yaml`

 * *Files identical despite different names*

### Comparing `mobsfscan-0.3.8/mobsfscan/rules/semgrep/android/logging.yaml` & `mobsfscan-0.3.9/mobsfscan/rules/semgrep/android/logging.yaml`

 * *Files identical despite different names*

### Comparing `mobsfscan-0.3.8/mobsfscan/rules/semgrep/android/secrets.yaml` & `mobsfscan-0.3.9/mobsfscan/rules/semgrep/android/secrets.yaml`

 * *Files identical despite different names*

### Comparing `mobsfscan-0.3.8/mobsfscan/rules/semgrep/android/word_readable_writable.yaml` & `mobsfscan-0.3.9/mobsfscan/rules/semgrep/android/word_readable_writable.yaml`

 * *Files identical despite different names*

### Comparing `mobsfscan-0.3.8/mobsfscan/rules/semgrep/best_practices/android_safetynetapi.yaml` & `mobsfscan-0.3.9/mobsfscan/rules/semgrep/best_practices/android_safetynetapi.yaml`

 * *Files identical despite different names*

### Comparing `mobsfscan-0.3.8/mobsfscan/rules/semgrep/best_practices/flag_secure.yaml` & `mobsfscan-0.3.9/mobsfscan/rules/semgrep/best_practices/flag_secure.yaml`

 * *Files identical despite different names*

### Comparing `mobsfscan-0.3.8/mobsfscan/rules/semgrep/best_practices/root_detection.yaml` & `mobsfscan-0.3.9/mobsfscan/rules/semgrep/best_practices/root_detection.yaml`

 * *Files identical despite different names*

### Comparing `mobsfscan-0.3.8/mobsfscan/rules/semgrep/best_practices/tapjacking.yaml` & `mobsfscan-0.3.9/mobsfscan/rules/semgrep/best_practices/tapjacking.yaml`

 * *Files identical despite different names*

### Comparing `mobsfscan-0.3.8/mobsfscan/rules/semgrep/best_practices/tls_certificate_transparency.yaml` & `mobsfscan-0.3.9/mobsfscan/rules/semgrep/best_practices/tls_certificate_transparency.yaml`

 * *Files identical despite different names*

### Comparing `mobsfscan-0.3.8/mobsfscan/rules/semgrep/best_practices/tls_pinning.yaml` & `mobsfscan-0.3.9/mobsfscan/rules/semgrep/best_practices/tls_pinning.yaml`

 * *Files identical despite different names*

### Comparing `mobsfscan-0.3.8/mobsfscan/rules/semgrep/crypto/aes_ecb.yaml` & `mobsfscan-0.3.9/mobsfscan/rules/semgrep/crypto/aes_ecb.yaml`

 * *Files identical despite different names*

### Comparing `mobsfscan-0.3.8/mobsfscan/rules/semgrep/crypto/aes_encryption_keys.yaml` & `mobsfscan-0.3.9/mobsfscan/rules/semgrep/crypto/aes_encryption_keys.yaml`

 * *Files identical despite different names*

### Comparing `mobsfscan-0.3.8/mobsfscan/rules/semgrep/crypto/cbc_padding_oracle.yaml` & `mobsfscan-0.3.9/mobsfscan/rules/semgrep/crypto/cbc_padding_oracle.yaml`

 * *Files identical despite different names*

### Comparing `mobsfscan-0.3.8/mobsfscan/rules/semgrep/crypto/cbc_static_iv.yaml` & `mobsfscan-0.3.9/mobsfscan/rules/semgrep/crypto/cbc_static_iv.yaml`

 * *Files identical despite different names*

### Comparing `mobsfscan-0.3.8/mobsfscan/rules/semgrep/crypto/insecure_random.yaml` & `mobsfscan-0.3.9/mobsfscan/rules/semgrep/crypto/insecure_random.yaml`

 * *Files identical despite different names*

### Comparing `mobsfscan-0.3.8/mobsfscan/rules/semgrep/crypto/insecure_ssl_v3.yaml` & `mobsfscan-0.3.9/mobsfscan/rules/semgrep/crypto/insecure_ssl_v3.yaml`

 * *Files identical despite different names*

### Comparing `mobsfscan-0.3.8/mobsfscan/rules/semgrep/crypto/rsa_no_oeap.yaml` & `mobsfscan-0.3.9/mobsfscan/rules/semgrep/crypto/rsa_no_oeap.yaml`

 * *Files identical despite different names*

### Comparing `mobsfscan-0.3.8/mobsfscan/rules/semgrep/crypto/sha1_hash.yaml` & `mobsfscan-0.3.9/mobsfscan/rules/semgrep/crypto/sha1_hash.yaml`

 * *Files identical despite different names*

### Comparing `mobsfscan-0.3.8/mobsfscan/rules/semgrep/crypto/weak_ciphers.yaml` & `mobsfscan-0.3.9/mobsfscan/rules/semgrep/crypto/weak_ciphers.yaml`

 * *Files identical despite different names*

### Comparing `mobsfscan-0.3.8/mobsfscan/rules/semgrep/crypto/weak_hashes.yaml` & `mobsfscan-0.3.9/mobsfscan/rules/semgrep/crypto/weak_hashes.yaml`

 * *Files identical despite different names*

### Comparing `mobsfscan-0.3.8/mobsfscan/rules/semgrep/crypto/weak_iv.yaml` & `mobsfscan-0.3.9/mobsfscan/rules/semgrep/crypto/weak_iv.yaml`

 * *Files identical despite different names*

### Comparing `mobsfscan-0.3.8/mobsfscan/rules/semgrep/crypto/weak_key_size.yaml` & `mobsfscan-0.3.9/mobsfscan/rules/semgrep/crypto/weak_key_size.yaml`

 * *Files identical despite different names*

### Comparing `mobsfscan-0.3.8/mobsfscan/rules/semgrep/deserialization/jackson_deserialization.yaml` & `mobsfscan-0.3.9/mobsfscan/rules/semgrep/deserialization/jackson_deserialization.yaml`

 * *Files identical despite different names*

### Comparing `mobsfscan-0.3.8/mobsfscan/rules/semgrep/deserialization/object_deserialization.yaml` & `mobsfscan-0.3.9/mobsfscan/rules/semgrep/deserialization/object_deserialization.yaml`

 * *Files identical despite different names*

### Comparing `mobsfscan-0.3.8/mobsfscan/rules/semgrep/injection/command_injection.yaml` & `mobsfscan-0.3.9/mobsfscan/rules/semgrep/injection/command_injection.yaml`

 * *Files identical despite different names*

### Comparing `mobsfscan-0.3.8/mobsfscan/rules/semgrep/injection/command_injection_formated.yaml` & `mobsfscan-0.3.9/mobsfscan/rules/semgrep/injection/command_injection_formated.yaml`

 * *Files identical despite different names*

### Comparing `mobsfscan-0.3.8/mobsfscan/rules/semgrep/injection/sqlite_injection.yaml` & `mobsfscan-0.3.9/mobsfscan/rules/semgrep/injection/sqlite_injection.yaml`

 * *Files identical despite different names*

### Comparing `mobsfscan-0.3.8/mobsfscan/rules/semgrep/network/accept_self_signed.yaml` & `mobsfscan-0.3.9/mobsfscan/rules/semgrep/network/accept_self_signed.yaml`

 * *Files identical despite different names*

### Comparing `mobsfscan-0.3.8/mobsfscan/rules/semgrep/network/default_http_client_tls.yaml` & `mobsfscan-0.3.9/mobsfscan/rules/semgrep/network/default_http_client_tls.yaml`

 * *Files identical despite different names*

### Comparing `mobsfscan-0.3.8/mobsfscan/rules/semgrep/webview/webview_debugging.yaml` & `mobsfscan-0.3.9/mobsfscan/rules/semgrep/webview/webview_debugging.yaml`

 * *Files identical despite different names*

### Comparing `mobsfscan-0.3.8/mobsfscan/rules/semgrep/webview/webview_external_storage.yaml` & `mobsfscan-0.3.9/mobsfscan/rules/semgrep/webview/webview_external_storage.yaml`

 * *Files identical despite different names*

### Comparing `mobsfscan-0.3.8/mobsfscan/rules/semgrep/webview/webview_file_access.yaml` & `mobsfscan-0.3.9/mobsfscan/rules/semgrep/webview/webview_file_access.yaml`

 * *Files identical despite different names*

### Comparing `mobsfscan-0.3.8/mobsfscan/rules/semgrep/webview/webview_ignore_ssl_errors.yaml` & `mobsfscan-0.3.9/mobsfscan/rules/semgrep/webview/webview_ignore_ssl_errors.yaml`

 * *Files identical despite different names*

### Comparing `mobsfscan-0.3.8/mobsfscan/rules/semgrep/webview/webview_javascript_interface.yaml` & `mobsfscan-0.3.9/mobsfscan/rules/semgrep/webview/webview_javascript_interface.yaml`

 * *Files identical despite different names*

### Comparing `mobsfscan-0.3.8/mobsfscan/rules/semgrep/xxe/xmldecoder_xxe.yaml` & `mobsfscan-0.3.9/mobsfscan/rules/semgrep/xxe/xmldecoder_xxe.yaml`

 * *Files identical despite different names*

### Comparing `mobsfscan-0.3.8/mobsfscan/rules/semgrep/xxe/xmlfactory_external_entities_enabled.yaml` & `mobsfscan-0.3.9/mobsfscan/rules/semgrep/xxe/xmlfactory_external_entities_enabled.yaml`

 * *Files identical despite different names*

### Comparing `mobsfscan-0.3.8/mobsfscan/rules/semgrep/xxe/xmlfactory_xxe.yaml` & `mobsfscan-0.3.9/mobsfscan/rules/semgrep/xxe/xmlfactory_xxe.yaml`

 * *Files identical despite different names*

### Comparing `mobsfscan-0.3.8/mobsfscan/settings.py` & `mobsfscan-0.3.9/mobsfscan/settings.py`

 * *Files identical despite different names*

### Comparing `mobsfscan-0.3.8/mobsfscan/utils.py` & `mobsfscan-0.3.9/mobsfscan/utils.py`

 * *Files identical despite different names*

### Comparing `mobsfscan-0.3.8/mobsfscan.egg-info/PKG-INFO` & `mobsfscan-0.3.9/mobsfscan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mobsfscan
-Version: 0.3.8
+Version: 0.3.9
 Summary: mobsfscan is a static analysis tool that can find insecure code patterns in your Android and iOS source code. Supports Java, Kotlin, Swift, and Objective C Code.
 Home-page: https://github.com/MobSF/mobsfscan
 Author: Ajin Abraham
 Author-email: ajin25@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

### Comparing `mobsfscan-0.3.8/mobsfscan.egg-info/SOURCES.txt` & `mobsfscan-0.3.9/mobsfscan.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 mobsfscan.egg-info/SOURCES.txt
 mobsfscan.egg-info/dependency_links.txt
 mobsfscan.egg-info/entry_points.txt
 mobsfscan.egg-info/requires.txt
 mobsfscan.egg-info/top_level.txt
 mobsfscan/formatters/__init__.py
 mobsfscan/formatters/cli.py
-mobsfscan/formatters/json.py
+mobsfscan/formatters/json_fmt.py
 mobsfscan/formatters/sarif.py
 mobsfscan/formatters/sonarqube.py
 mobsfscan/rules/patterns/android/kotlin/best_practices.yaml
 mobsfscan/rules/patterns/android/kotlin/kotlin_rules.yaml
 mobsfscan/rules/patterns/ios/objectivec/best_practices.yaml
 mobsfscan/rules/patterns/ios/objectivec/objective_c_rules.yaml
 mobsfscan/rules/patterns/ios/swift/best_practices.yaml
@@ -53,14 +53,15 @@
 mobsfscan/rules/semgrep/deserialization/jackson_deserialization.yaml
 mobsfscan/rules/semgrep/deserialization/object_deserialization.yaml
 mobsfscan/rules/semgrep/injection/command_injection.yaml
 mobsfscan/rules/semgrep/injection/command_injection_formated.yaml
 mobsfscan/rules/semgrep/injection/sqlite_injection.yaml
 mobsfscan/rules/semgrep/network/accept_self_signed.yaml
 mobsfscan/rules/semgrep/network/default_http_client_tls.yaml
+mobsfscan/rules/semgrep/webview/webview_allow_file_from_url.yaml
 mobsfscan/rules/semgrep/webview/webview_debugging.yaml
 mobsfscan/rules/semgrep/webview/webview_external_storage.yaml
 mobsfscan/rules/semgrep/webview/webview_file_access.yaml
 mobsfscan/rules/semgrep/webview/webview_ignore_ssl_errors.yaml
 mobsfscan/rules/semgrep/webview/webview_javascript_interface.yaml
 mobsfscan/rules/semgrep/xxe/xmldecoder_xxe.yaml
 mobsfscan/rules/semgrep/xxe/xmlfactory_external_entities_enabled.yaml
```

### Comparing `mobsfscan-0.3.8/setup.py` & `mobsfscan-0.3.9/setup.py`

 * *Files identical despite different names*

