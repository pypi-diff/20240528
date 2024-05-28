# Comparing `tmp/nebari_plugin_self_registration-0.0.8.tar.gz` & `tmp/nebari_plugin_self_registration-0.0.9.tar.gz`

## Comparing `nebari_plugin_self_registration-0.0.8.tar` & `nebari_plugin_self_registration-0.0.9.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/.github/workflows/publish-docker-image.yaml
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/.github/workflows/publish-pypi.yaml
--rw-r--r--   0        0        0   203481 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/images/account-confirm.png
--rw-r--r--   0        0        0   143215 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/images/account-register.png
--rw-r--r--   0        0        0    97043 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/images/nebari-splash.png
--rw-r--r--   0        0        0   215778 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/images/verify-email.png
--rw-r--r--   0        0        0    16370 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/images/welcome-nebari.png
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/self-registration/.dockerignore
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/self-registration/Dockerfile
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/self-registration/Dockerfile.local
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/self-registration/config.sample.yaml
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/self-registration/requirements.txt
--rwxr-xr-x   0        0        0      262 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/self-registration/run.sh
--rw-r--r--   0        0        0     3922 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/self-registration/app/job.py
--rw-r--r--   0        0        0     7526 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/self-registration/app/main.py
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/self-registration/app/theme.py
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/self-registration/app/static/favicon.ico
--rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/self-registration/app/static/logo.svg
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/self-registration/app/templates/base.html
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/self-registration/app/templates/index.html
--rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/self-registration/app/templates/styles.css
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/self-registration/app/templates/success.html
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/__about__.py
--rw-r--r--   0        0        0     7454 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/__init__.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/main.tf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/outputs.tf
--rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/variables.tf
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/versions.tf
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/keycloak/main.tf
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/keycloak/outputs.tf
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/keycloak/variables.tf
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/keycloak/versions.tf
--rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/self-registration/main.tf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/self-registration/outputs.tf
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/self-registration/variables.tf
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/.helmignore
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/Chart.yaml
--rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/values.yaml
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/NOTES.txt
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/_helpers.tpl
--rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/deployment.yaml
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/hpa.yaml
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/ingress.yaml
--rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/job.yaml
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/secret.yaml
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/service.yaml
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/serviceaccount.yaml
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/traefik.yaml
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/tests/test-connection.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/tests/unit/__init__.py
--rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/tests/unit/test_plugin.py
--rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/LICENSE
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/README.md
--rw-r--r--   0        0        0     3523 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.9/.github/workflows/publish-docker-image.yaml
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.9/.github/workflows/publish-pypi.yaml
+-rw-r--r--   0        0        0   203481 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.9/images/account-confirm.png
+-rw-r--r--   0        0        0   143215 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.9/images/account-register.png
+-rw-r--r--   0        0        0    97043 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.9/images/nebari-splash.png
+-rw-r--r--   0        0        0   215778 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.9/images/verify-email.png
+-rw-r--r--   0        0        0    16370 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.9/images/welcome-nebari.png
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.9/self-registration/.dockerignore
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.9/self-registration/Dockerfile
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.9/self-registration/Dockerfile.local
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.9/self-registration/config.sample.yaml
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.9/self-registration/requirements.txt
+-rwxr-xr-x   0        0        0      262 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.9/self-registration/run.sh
+-rw-r--r--   0        0        0     3922 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.9/self-registration/app/job.py
+-rw-r--r--   0        0        0     7526 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.9/self-registration/app/main.py
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.9/self-registration/app/theme.py
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.9/self-registration/app/static/favicon.ico
+-rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.9/self-registration/app/static/logo.svg
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.9/self-registration/app/templates/base.html
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.9/self-registration/app/templates/index.html
+-rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.9/self-registration/app/templates/styles.css
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.9/self-registration/app/templates/success.html
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.9/src/nebari_plugin_self_registration/__about__.py
+-rw-r--r--   0        0        0     7505 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.9/src/nebari_plugin_self_registration/__init__.py
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.9/src/nebari_plugin_self_registration/terraform/main.tf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.9/src/nebari_plugin_self_registration/terraform/outputs.tf
+-rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.9/src/nebari_plugin_self_registration/terraform/variables.tf
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.9/src/nebari_plugin_self_registration/terraform/versions.tf
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.9/src/nebari_plugin_self_registration/terraform/modules/keycloak/main.tf
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.9/src/nebari_plugin_self_registration/terraform/modules/keycloak/outputs.tf
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.9/src/nebari_plugin_self_registration/terraform/modules/keycloak/variables.tf
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.9/src/nebari_plugin_self_registration/terraform/modules/keycloak/versions.tf
+-rw-r--r--   0        0        0     2879 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.9/src/nebari_plugin_self_registration/terraform/modules/self-registration/main.tf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.9/src/nebari_plugin_self_registration/terraform/modules/self-registration/outputs.tf
+-rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.9/src/nebari_plugin_self_registration/terraform/modules/self-registration/variables.tf
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.9/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/.helmignore
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.9/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/Chart.yaml
+-rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.9/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/values.yaml
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.9/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/NOTES.txt
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.9/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/_helpers.tpl
+-rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.9/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/deployment.yaml
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.9/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/hpa.yaml
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.9/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/ingress.yaml
+-rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.9/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/job.yaml
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.9/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/secret.yaml
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.9/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/service.yaml
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.9/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/serviceaccount.yaml
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.9/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/traefik.yaml
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.9/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/tests/test-connection.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.9/src/nebari_plugin_self_registration/tests/unit/__init__.py
+-rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.9/src/nebari_plugin_self_registration/tests/unit/test_plugin.py
+-rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.9/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.9/README.md
+-rw-r--r--   0        0        0     3523 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 nebari_plugin_self_registration-0.0.9/PKG-INFO
```

### Comparing `nebari_plugin_self_registration-0.0.8/.github/workflows/publish-docker-image.yaml` & `nebari_plugin_self_registration-0.0.9/.github/workflows/publish-docker-image.yaml`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.8/.github/workflows/publish-pypi.yaml` & `nebari_plugin_self_registration-0.0.9/.github/workflows/publish-pypi.yaml`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.8/images/account-confirm.png` & `nebari_plugin_self_registration-0.0.9/images/account-confirm.png`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.8/images/account-register.png` & `nebari_plugin_self_registration-0.0.9/images/account-register.png`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.8/images/nebari-splash.png` & `nebari_plugin_self_registration-0.0.9/images/nebari-splash.png`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.8/images/verify-email.png` & `nebari_plugin_self_registration-0.0.9/images/verify-email.png`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.8/images/welcome-nebari.png` & `nebari_plugin_self_registration-0.0.9/images/welcome-nebari.png`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.8/self-registration/app/job.py` & `nebari_plugin_self_registration-0.0.9/self-registration/app/job.py`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.8/self-registration/app/main.py` & `nebari_plugin_self_registration-0.0.9/self-registration/app/main.py`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.8/self-registration/app/theme.py` & `nebari_plugin_self_registration-0.0.9/self-registration/app/theme.py`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.8/self-registration/app/static/favicon.ico` & `nebari_plugin_self_registration-0.0.9/self-registration/app/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.8/self-registration/app/static/logo.svg` & `nebari_plugin_self_registration-0.0.9/self-registration/app/static/logo.svg`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.8/self-registration/app/templates/base.html` & `nebari_plugin_self_registration-0.0.9/self-registration/app/templates/base.html`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.8/self-registration/app/templates/index.html` & `nebari_plugin_self_registration-0.0.9/self-registration/app/templates/index.html`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.8/self-registration/app/templates/styles.css` & `nebari_plugin_self_registration-0.0.9/self-registration/app/templates/styles.css`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.8/self-registration/app/templates/success.html` & `nebari_plugin_self_registration-0.0.9/self-registration/app/templates/success.html`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/__init__.py` & `nebari_plugin_self_registration-0.0.9/src/nebari_plugin_self_registration/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
 
 class SelfRegistrationAffinitySelectorConfig(Base):
     default: str
     app: Optional[str] = ""
     job: Optional[str] = ""
 
-
 class SelfRegistrationAffinityConfig(Base):
     enabled: Optional[bool] = True
     selector: Union[SelfRegistrationAffinitySelectorConfig, str] = "general"
 
 
 class SelfRegistrationConfig(Base):
     name: Optional[str] = "self-registration"
@@ -164,14 +163,15 @@
                     self.config.self_registration.affinity.selector.__dict__
                     if isinstance(
                         self.config.self_registration.affinity.selector, SelfRegistrationAffinitySelectorConfig
                     )
                     else self.config.self_registration.affinity.selector
                 ),
             },
+            "cloud_provider": self.config.provider,
             "theme": self.config.theme.jupyterhub.dict(),
         }
 
     def get_keycloak_config(self, stage_outputs: Dict[str, Dict[str, Any]]):
         directory = "stages/05-kubernetes-keycloak"
 
         return {
```

### Comparing `nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/main.tf` & `nebari_plugin_self_registration-0.0.9/src/nebari_plugin_self_registration/terraform/main.tf`

 * *Files 16% similar despite different names*

```diff
@@ -24,9 +24,10 @@
   registration_message      = var.registration_message
   namespace                 = var.namespace
   keycloak_base_url         = var.external_url
   keycloak_config           = module.keycloak.config
   overrides                 = var.overrides
   realm_id                  = var.realm_id
   affinity                  = var.affinity
+  cloud_provider            = var.cloud_provider
   theme                     = var.theme
 }
```

### Comparing `nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/variables.tf` & `nebari_plugin_self_registration-0.0.9/src/nebari_plugin_self_registration/terraform/variables.tf`

 * *Files 2% similar despite different names*

```diff
@@ -93,12 +93,21 @@
 
   validation {
     condition     = can(tostring(var.affinity.selector)) || (can(var.affinity.selector.default) && length(try(var.affinity.selector.default, "")) > 0)
     error_message = "\"affinity.selector\" argument must be a string or object { default, app, job }"
   }
 }
 
+
+# GENERAL SETTINGS
+# -----------------
+variable "cloud_provider" {
+  description = "Cloud provider where Nebari is deployed to"
+  type        = string
+}
+
 variable "theme" {
   description = "Theme configured in theme.jupyterhub"
   type        = map(any)
   default     = {}
+
 }
```

### Comparing `nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/keycloak/main.tf` & `nebari_plugin_self_registration-0.0.9/src/nebari_plugin_self_registration/terraform/modules/keycloak/main.tf`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/self-registration/main.tf` & `nebari_plugin_self_registration-0.0.9/src/nebari_plugin_self_registration/terraform/modules/self-registration/main.tf`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,19 @@
         job  = var.affinity.selector
       },
     )
     } : {
     enabled  = false
     selector = null
   }
+
+  affinity_selector_key = {
+    aws = "eks.amazonaws.com/nodegroup"
+    gcp = "cloud.google.com/gke-nodepool"
+  }
 }
 
 resource "kubernetes_namespace" "this" {
   count = var.create_namespace ? 1 : 0
 
   metadata {
     name = var.namespace
@@ -38,15 +43,15 @@
       affinity = local.affinity.enabled ? {
         nodeAffinity = {
           requiredDuringSchedulingIgnoredDuringExecution = {
             nodeSelectorTerms = [
               {
                 matchExpressions = [
                   {
-                    key      = "eks.amazonaws.com/nodegroup"
+                    key      = local.affinity_selector_key[var.cloud_provider]
                     operator = "In"
                     values   = [local.affinity.selector.app]
                   }
                 ]
               }
             ]
           }
@@ -56,15 +61,15 @@
         affinity = local.affinity.enabled ? {
           nodeAffinity = {
             requiredDuringSchedulingIgnoredDuringExecution = {
               nodeSelectorTerms = [
                 {
                   matchExpressions = [
                     {
-                      key      = "eks.amazonaws.com/nodegroup"
+                      key      = local.affinity_selector_key[var.cloud_provider]
                       operator = "In"
                       values   = [local.affinity.selector.job]
                     }
                   ]
                 }
               ]
             }
```

### Comparing `nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/self-registration/variables.tf` & `nebari_plugin_self_registration-0.0.9/src/nebari_plugin_self_registration/terraform/modules/self-registration/variables.tf`

 * *Files 3% similar despite different names*

```diff
@@ -80,12 +80,17 @@
 
   validation {
     condition     = can(tostring(var.affinity.selector)) || (can(var.affinity.selector.default) && length(try(var.affinity.selector.default, "")) > 0)
     error_message = "\"affinity.selector\" argument must be a string or object { default, app, job }"
   }
 }
 
+
+variable "cloud_provider" {
+  type = string
+}
+
 variable "theme" {
   description = "Theme configured in theme.jupyterhub"
   type        = map(any)
   default     = {}
-}
+}
```

### Comparing `nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/Chart.yaml` & `nebari_plugin_self_registration-0.0.9/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/Chart.yaml`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/values.yaml` & `nebari_plugin_self_registration-0.0.9/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/values.yaml`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/NOTES.txt` & `nebari_plugin_self_registration-0.0.9/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/NOTES.txt`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/_helpers.tpl` & `nebari_plugin_self_registration-0.0.9/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/deployment.yaml` & `nebari_plugin_self_registration-0.0.9/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/deployment.yaml`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/hpa.yaml` & `nebari_plugin_self_registration-0.0.9/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/hpa.yaml`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/ingress.yaml` & `nebari_plugin_self_registration-0.0.9/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/ingress.yaml`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/job.yaml` & `nebari_plugin_self_registration-0.0.9/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/job.yaml`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/traefik.yaml` & `nebari_plugin_self_registration-0.0.9/src/nebari_plugin_self_registration/terraform/modules/self-registration/chart/templates/traefik.yaml`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.8/src/nebari_plugin_self_registration/tests/unit/test_plugin.py` & `nebari_plugin_self_registration-0.0.9/src/nebari_plugin_self_registration/tests/unit/test_plugin.py`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.8/.gitignore` & `nebari_plugin_self_registration-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.8/LICENSE` & `nebari_plugin_self_registration-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.8/README.md` & `nebari_plugin_self_registration-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.8/pyproject.toml` & `nebari_plugin_self_registration-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nebari_plugin_self_registration-0.0.8/PKG-INFO` & `nebari_plugin_self_registration-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nebari-plugin-self-registration
-Version: 0.0.8
+Version: 0.0.9
 Summary: MetroStar - Self-Registration Plugin for Nebari Platform
 Project-URL: Documentation, https://github.com/MetroStar/nebari-self-registration#readme
 Project-URL: Issues, https://github.com/MetroStar/nebari-self-registration/issues
 Project-URL: Source, https://github.com/MetroStar/nebari-self-registration
 Author-email: Ken Foster <kfoster@metrostar.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
```

