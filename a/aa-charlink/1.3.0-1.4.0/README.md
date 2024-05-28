# Comparing `tmp/aa_charlink-1.3.0.tar.gz` & `tmp/aa_charlink-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa_charlink-1.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aa_charlink-1.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aa_charlink-1.3.0.tar` & `aa_charlink-1.4.0.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rwxr-xr-x   0        0        0    35149 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/LICENSE
--rwxr-xr-x   0        0        0     3945 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/README.md
--rwxr-xr-x   0        0        0      127 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/__init__.py
--rw-r--r--   0        0        0     3233 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/app_imports/__init__.py
--rw-r--r--   0        0        0     5216 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/app_imports/utils.py
--rwxr-xr-x   0        0        0      108 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/app_settings.py
--rwxr-xr-x   0        0        0      148 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/apps.py
--rwxr-xr-x   0        0        0      754 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/auth_hooks.py
--rwxr-xr-x   0        0        0      494 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/decorators.py
--rwxr-xr-x   0        0        0      652 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/forms.py
--rwxr-xr-x   0        0        0        0 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/imports/__init__.py
--rw-r--r--   0        0        0     2882 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/imports/afat.py
--rwxr-xr-x   0        0        0        0 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/imports/allianceauth/__init__.py
--rwxr-xr-x   0        0        0     1777 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/imports/allianceauth/corputils.py
--rw-r--r--   0        0        0     1788 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/imports/corpstats.py
--rwxr-xr-x   0        0        0     4001 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/imports/corptools.py
--rw-r--r--   0        0        0     2365 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/imports/marketmanager.py
--rwxr-xr-x   0        0        0     2058 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/imports/memberaudit.py
--rwxr-xr-x   0        0        0     1548 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/imports/miningtaxes.py
--rwxr-xr-x   0        0        0     2600 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/imports/moonmining.py
--rwxr-xr-x   0        0        0     1689 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/imports/moonstuff.py
--rwxr-xr-x   0        0        0     3962 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/imports/structures.py
--rw-r--r--   0        0        0      810 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/migrations/0001_initial.py
--rwxr-xr-x   0        0        0        0 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/migrations/__init__.py
--rwxr-xr-x   0        0        0      435 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/models.py
--rw-r--r--   0        0        0       62 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/static/charlink/css/added-icons.css
--rw-r--r--   0        0        0     4306 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/templates/charlink/app_audit.html
--rwxr-xr-x   0        0        0     4080 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/templates/charlink/audit.html
--rw-r--r--   0        0        0      746 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/templates/charlink/base.html
--rwxr-xr-x   0        0        0     6124 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/templates/charlink/charlink.html
--rw-r--r--   0        0        0      532 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/templates/charlink/dashboard_login.html
--rw-r--r--   0        0        0      903 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/templates/charlink/menu-left.html
--rw-r--r--   0        0        0      431 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/templates/charlink/menu-right.html
--rw-r--r--   0        0        0     2711 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/templates/charlink/search.html
--rw-r--r--   0        0        0     3032 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/templates/charlink/user_audit.html
--rw-r--r--   0        0        0        0 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/templatetags/__init__.py
--rw-r--r--   0        0        0      516 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/templatetags/charlink_versioned_static.py
--rw-r--r--   0        0        0      837 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/templatetags/charlinkutils.py
--rw-r--r--   0        0        0        0 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/tests/imports/__init__.py
--rw-r--r--   0        0        0     3943 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/tests/imports/test_afat.py
--rw-r--r--   0        0        0     3060 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/tests/imports/test_allianceauth_corputils.py
--rw-r--r--   0        0        0     2980 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/tests/imports/test_corpstats.py
--rw-r--r--   0        0        0     3798 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/tests/imports/test_corptools.py
--rw-r--r--   0        0        0     3197 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/tests/imports/test_marketmanager.py
--rw-r--r--   0        0        0     3213 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/tests/imports/test_memberaudit.py
--rw-r--r--   0        0        0     2272 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/tests/imports/test_miningtaxes.py
--rw-r--r--   0        0        0     3710 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/tests/imports/test_moonmining.py
--rw-r--r--   0        0        0     2440 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/tests/imports/test_moonstuff.py
--rw-r--r--   0        0        0     5986 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/tests/imports/test_structures.py
--rw-r--r--   0        0        0     8839 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/tests/test_app_imports.py
--rwxr-xr-x   0        0        0     1265 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/tests/test_auth_hooks.py
--rw-r--r--   0        0        0     1323 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/tests/test_decorators.py
--rw-r--r--   0        0        0     1261 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/tests/test_forms.py
--rw-r--r--   0        0        0     2241 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/tests/test_templatetags.py
--rw-r--r--   0        0        0     5488 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/tests/test_utils.py
--rw-r--r--   0        0        0    20489 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/tests/test_views.py
--rwxr-xr-x   0        0        0      520 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/urls.py
--rw-r--r--   0        0        0     2703 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/utils.py
--rwxr-xr-x   0        0        0     8267 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/charlink/views.py
--rwxr-xr-x   0        0        0     1519 2024-05-19 17:46:19.316582 aa_charlink-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     5404 1970-01-01 00:00:00.000000 aa_charlink-1.3.0/PKG-INFO
+-rwxr-xr-x   0        0        0    35149 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/LICENSE
+-rwxr-xr-x   0        0        0     3945 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/README.md
+-rwxr-xr-x   0        0        0      127 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/charlink/__init__.py
+-rw-r--r--   0        0        0     3233 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/charlink/app_imports/__init__.py
+-rw-r--r--   0        0        0     5216 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/charlink/app_imports/utils.py
+-rwxr-xr-x   0        0        0      108 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/charlink/app_settings.py
+-rwxr-xr-x   0        0        0      148 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/charlink/apps.py
+-rwxr-xr-x   0        0        0      754 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/charlink/auth_hooks.py
+-rwxr-xr-x   0        0        0      494 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/charlink/decorators.py
+-rwxr-xr-x   0        0        0      652 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/charlink/forms.py
+-rwxr-xr-x   0        0        0        0 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/charlink/imports/__init__.py
+-rw-r--r--   0        0        0     2882 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/charlink/imports/afat.py
+-rwxr-xr-x   0        0        0        0 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/charlink/imports/allianceauth/__init__.py
+-rwxr-xr-x   0        0        0     1777 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/charlink/imports/allianceauth/corputils.py
+-rw-r--r--   0        0        0     1788 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/charlink/imports/corpstats.py
+-rwxr-xr-x   0        0        0     4001 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/charlink/imports/corptools.py
+-rw-r--r--   0        0        0     2365 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/charlink/imports/marketmanager.py
+-rwxr-xr-x   0        0        0     2058 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/charlink/imports/memberaudit.py
+-rwxr-xr-x   0        0        0     1548 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/charlink/imports/miningtaxes.py
+-rwxr-xr-x   0        0        0     2600 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/charlink/imports/moonmining.py
+-rwxr-xr-x   0        0        0     1689 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/charlink/imports/moonstuff.py
+-rwxr-xr-x   0        0        0     3962 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/charlink/imports/structures.py
+-rw-r--r--   0        0        0      810 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/charlink/migrations/0001_initial.py
+-rwxr-xr-x   0        0        0        0 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/charlink/migrations/__init__.py
+-rwxr-xr-x   0        0        0      435 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/charlink/models.py
+-rw-r--r--   0        0        0       62 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/charlink/static/charlink/css/added-icons.css
+-rw-r--r--   0        0        0     4306 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/charlink/templates/charlink/app_audit.html
+-rwxr-xr-x   0        0        0     4080 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/charlink/templates/charlink/audit.html
+-rw-r--r--   0        0        0      746 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/charlink/templates/charlink/base.html
+-rwxr-xr-x   0        0        0     6124 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/charlink/templates/charlink/charlink.html
+-rw-r--r--   0        0        0      731 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/charlink/templates/charlink/dashboard_login.html
+-rw-r--r--   0        0        0      903 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/charlink/templates/charlink/menu-left.html
+-rw-r--r--   0        0        0      431 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/charlink/templates/charlink/menu-right.html
+-rw-r--r--   0        0        0     2711 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/charlink/templates/charlink/search.html
+-rw-r--r--   0        0        0     3032 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/charlink/templates/charlink/user_audit.html
+-rw-r--r--   0        0        0        0 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/charlink/templatetags/__init__.py
+-rw-r--r--   0        0        0      516 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/charlink/templatetags/charlink_versioned_static.py
+-rw-r--r--   0        0        0      837 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/charlink/templatetags/charlinkutils.py
+-rw-r--r--   0        0        0        0 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/charlink/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/charlink/tests/imports/__init__.py
+-rw-r--r--   0        0        0     3943 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/charlink/tests/imports/test_afat.py
+-rw-r--r--   0        0        0     3060 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/charlink/tests/imports/test_allianceauth_corputils.py
+-rw-r--r--   0        0        0     2980 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/charlink/tests/imports/test_corpstats.py
+-rw-r--r--   0        0        0     3798 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/charlink/tests/imports/test_corptools.py
+-rw-r--r--   0        0        0     3197 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/charlink/tests/imports/test_marketmanager.py
+-rw-r--r--   0        0        0     3213 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/charlink/tests/imports/test_memberaudit.py
+-rw-r--r--   0        0        0     2272 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/charlink/tests/imports/test_miningtaxes.py
+-rw-r--r--   0        0        0     3710 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/charlink/tests/imports/test_moonmining.py
+-rw-r--r--   0        0        0     2440 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/charlink/tests/imports/test_moonstuff.py
+-rw-r--r--   0        0        0     5986 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/charlink/tests/imports/test_structures.py
+-rw-r--r--   0        0        0     8839 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/charlink/tests/test_app_imports.py
+-rwxr-xr-x   0        0        0     1265 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/charlink/tests/test_auth_hooks.py
+-rw-r--r--   0        0        0     1323 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/charlink/tests/test_decorators.py
+-rw-r--r--   0        0        0     1261 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/charlink/tests/test_forms.py
+-rw-r--r--   0        0        0     2241 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/charlink/tests/test_templatetags.py
+-rw-r--r--   0        0        0     5488 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/charlink/tests/test_utils.py
+-rw-r--r--   0        0        0    20413 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/charlink/tests/test_views.py
+-rwxr-xr-x   0        0        0      520 2024-05-28 19:27:25.687322 aa_charlink-1.4.0/charlink/urls.py
+-rw-r--r--   0        0        0     2703 2024-05-28 19:27:25.691322 aa_charlink-1.4.0/charlink/utils.py
+-rwxr-xr-x   0        0        0     8267 2024-05-28 19:27:25.691322 aa_charlink-1.4.0/charlink/views.py
+-rwxr-xr-x   0        0        0     1519 2024-05-28 19:27:25.691322 aa_charlink-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     5404 1970-01-01 00:00:00.000000 aa_charlink-1.4.0/PKG-INFO
```

### Comparing `aa_charlink-1.3.0/LICENSE` & `aa_charlink-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.3.0/README.md` & `aa_charlink-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.3.0/charlink/app_imports/__init__.py` & `aa_charlink-1.4.0/charlink/app_imports/__init__.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.3.0/charlink/app_imports/utils.py` & `aa_charlink-1.4.0/charlink/app_imports/utils.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.3.0/charlink/auth_hooks.py` & `aa_charlink-1.4.0/charlink/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.3.0/charlink/forms.py` & `aa_charlink-1.4.0/charlink/forms.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.3.0/charlink/imports/afat.py` & `aa_charlink-1.4.0/charlink/imports/afat.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.3.0/charlink/imports/allianceauth/corputils.py` & `aa_charlink-1.4.0/charlink/imports/allianceauth/corputils.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.3.0/charlink/imports/corpstats.py` & `aa_charlink-1.4.0/charlink/imports/corpstats.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.3.0/charlink/imports/corptools.py` & `aa_charlink-1.4.0/charlink/imports/corptools.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.3.0/charlink/imports/marketmanager.py` & `aa_charlink-1.4.0/charlink/imports/marketmanager.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.3.0/charlink/imports/memberaudit.py` & `aa_charlink-1.4.0/charlink/imports/memberaudit.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.3.0/charlink/imports/miningtaxes.py` & `aa_charlink-1.4.0/charlink/imports/miningtaxes.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.3.0/charlink/imports/moonmining.py` & `aa_charlink-1.4.0/charlink/imports/moonmining.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.3.0/charlink/imports/moonstuff.py` & `aa_charlink-1.4.0/charlink/imports/moonstuff.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.3.0/charlink/imports/structures.py` & `aa_charlink-1.4.0/charlink/imports/structures.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.3.0/charlink/migrations/0001_initial.py` & `aa_charlink-1.4.0/charlink/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.3.0/charlink/templates/charlink/app_audit.html` & `aa_charlink-1.4.0/charlink/templates/charlink/app_audit.html`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.3.0/charlink/templates/charlink/audit.html` & `aa_charlink-1.4.0/charlink/templates/charlink/audit.html`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.3.0/charlink/templates/charlink/base.html` & `aa_charlink-1.4.0/charlink/templates/charlink/base.html`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.3.0/charlink/templates/charlink/charlink.html` & `aa_charlink-1.4.0/charlink/templates/charlink/charlink.html`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.3.0/charlink/templates/charlink/menu-left.html` & `aa_charlink-1.4.0/charlink/templates/charlink/menu-left.html`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.3.0/charlink/templates/charlink/search.html` & `aa_charlink-1.4.0/charlink/templates/charlink/search.html`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.3.0/charlink/templates/charlink/user_audit.html` & `aa_charlink-1.4.0/charlink/templates/charlink/user_audit.html`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.3.0/charlink/templatetags/charlink_versioned_static.py` & `aa_charlink-1.4.0/charlink/templatetags/charlink_versioned_static.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.3.0/charlink/templatetags/charlinkutils.py` & `aa_charlink-1.4.0/charlink/templatetags/charlinkutils.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.3.0/charlink/tests/imports/test_afat.py` & `aa_charlink-1.4.0/charlink/tests/imports/test_afat.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.3.0/charlink/tests/imports/test_allianceauth_corputils.py` & `aa_charlink-1.4.0/charlink/tests/imports/test_allianceauth_corputils.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.3.0/charlink/tests/imports/test_corpstats.py` & `aa_charlink-1.4.0/charlink/tests/imports/test_corpstats.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.3.0/charlink/tests/imports/test_corptools.py` & `aa_charlink-1.4.0/charlink/tests/imports/test_corptools.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.3.0/charlink/tests/imports/test_marketmanager.py` & `aa_charlink-1.4.0/charlink/tests/imports/test_marketmanager.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.3.0/charlink/tests/imports/test_memberaudit.py` & `aa_charlink-1.4.0/charlink/tests/imports/test_memberaudit.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.3.0/charlink/tests/imports/test_miningtaxes.py` & `aa_charlink-1.4.0/charlink/tests/imports/test_miningtaxes.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.3.0/charlink/tests/imports/test_moonmining.py` & `aa_charlink-1.4.0/charlink/tests/imports/test_moonmining.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.3.0/charlink/tests/imports/test_moonstuff.py` & `aa_charlink-1.4.0/charlink/tests/imports/test_moonstuff.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.3.0/charlink/tests/imports/test_structures.py` & `aa_charlink-1.4.0/charlink/tests/imports/test_structures.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.3.0/charlink/tests/test_app_imports.py` & `aa_charlink-1.4.0/charlink/tests/test_app_imports.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.3.0/charlink/tests/test_auth_hooks.py` & `aa_charlink-1.4.0/charlink/tests/test_auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.3.0/charlink/tests/test_decorators.py` & `aa_charlink-1.4.0/charlink/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.3.0/charlink/tests/test_forms.py` & `aa_charlink-1.4.0/charlink/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.3.0/charlink/tests/test_templatetags.py` & `aa_charlink-1.4.0/charlink/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.3.0/charlink/tests/test_utils.py` & `aa_charlink-1.4.0/charlink/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.3.0/charlink/tests/test_views.py` & `aa_charlink-1.4.0/charlink/tests/test_views.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,14 @@
                     <label class="form-check-label" for="id_charlink-testauth.testapp_import2">TestApp2</label>
                 </div>
             </div>''',
         ]
 
     def test_ok(self):
         res = dashboard_login(self.request)
-        self.assertInHTML('<h4 class="card-title mb-3">CharLink</h4>', res)
         for content in self.form_contents:
             self.assertInHTML(content, res)
 
 
 class TestDashboardPost(TestCase):
 
     @classmethod
```

### Comparing `aa_charlink-1.3.0/charlink/urls.py` & `aa_charlink-1.4.0/charlink/urls.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.3.0/charlink/utils.py` & `aa_charlink-1.4.0/charlink/utils.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.3.0/charlink/views.py` & `aa_charlink-1.4.0/charlink/views.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.3.0/pyproject.toml` & `aa_charlink-1.4.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     "allianceauth",
     "eveonline",
 	"allianceauth_charlink",
     "charlink",
 ]
 requires-python = "~=3.8"
 dependencies = [
-    "allianceauth~=4.0",
+    "allianceauth~=4.1",
     "allianceauth-app-utils~=1.14",
 ]
 
 [project.urls]
 Homepage = "https://github.com/Maestro-Zacht/aa-charlink"
 Source = "https://github.com/Maestro-Zacht/aa-charlink"
 Tracker = "https://github.com/Maestro-Zacht/aa-charlink/issues"
```

### Comparing `aa_charlink-1.3.0/PKG-INFO` & `aa_charlink-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-charlink
-Version: 1.3.0
+Version: 1.4.0
 Summary: Character Linker for Alliance Auth
 Keywords: allianceauth,eveonline,allianceauth_charlink,charlink
 Author-email: Matteo Ghia <matteo.ghia@yahoo.it>
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Dist: allianceauth~=4.0
+Requires-Dist: allianceauth~=4.1
 Requires-Dist: allianceauth-app-utils~=1.14
 Project-URL: Changelog, https://github.com/Maestro-Zacht/aa-charlink/releases
 Project-URL: Homepage, https://github.com/Maestro-Zacht/aa-charlink
 Project-URL: Source, https://github.com/Maestro-Zacht/aa-charlink
 Project-URL: Tracker, https://github.com/Maestro-Zacht/aa-charlink/issues
 
 # AllianceAuth CharLink
```

