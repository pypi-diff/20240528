# Comparing `tmp/obs_img_utils-1.3.0.tar.gz` & `tmp/obs_img_utils-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obs_img_utils-1.3.0.tar", last modified: Wed May  8 15:34:33 2024, max compression
+gzip compressed data, was "obs_img_utils-1.4.0.tar", last modified: Tue May 28 20:34:31 2024, max compression
```

## Comparing `obs_img_utils-1.3.0.tar` & `obs_img_utils-1.4.0.tar`

### file list

```diff
@@ -1,41 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:34:33.575693 obs_img_utils-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-05-08 15:34:25.000000 obs_img_utils-1.3.0/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-08 15:34:25.000000 obs_img_utils-1.3.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    32402 2024-05-08 15:34:25.000000 obs_img_utils-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-08 15:34:25.000000 obs_img_utils-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-08 15:34:33.575693 obs_img_utils-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-08 15:34:25.000000 obs_img_utils-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:34:33.571694 obs_img_utils-1.3.0/obs_img_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-08 15:34:25.000000 obs_img_utils-1.3.0/obs_img_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21144 2024-05-08 15:34:25.000000 obs_img_utils-1.3.0/obs_img_utils/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10741 2024-05-08 15:34:25.000000 obs_img_utils-1.3.0/obs_img_utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-05-08 15:34:25.000000 obs_img_utils-1.3.0/obs_img_utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13318 2024-05-08 15:34:25.000000 obs_img_utils-1.3.0/obs_img_utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5958 2024-05-08 15:34:25.000000 obs_img_utils-1.3.0/obs_img_utils/web_content.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:34:33.575693 obs_img_utils-1.3.0/obs_img_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-08 15:34:33.000000 obs_img_utils-1.3.0/obs_img_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-08 15:34:33.000000 obs_img_utils-1.3.0/obs_img_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:34:33.000000 obs_img_utils-1.3.0/obs_img_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-08 15:34:33.000000 obs_img_utils-1.3.0/obs_img_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:34:33.000000 obs_img_utils-1.3.0/obs_img_utils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-08 15:34:33.000000 obs_img_utils-1.3.0/obs_img_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-08 15:34:33.000000 obs_img_utils-1.3.0/obs_img_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:34:33.571694 obs_img_utils-1.3.0/package/
--rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-05-08 15:34:25.000000 obs_img_utils-1.3.0/package/python3-obs-img-utils.spec
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-08 15:34:25.000000 obs_img_utils-1.3.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-08 15:34:25.000000 obs_img_utils-1.3.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-08 15:34:25.000000 obs_img_utils-1.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-08 15:34:33.575693 obs_img_utils-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-05-08 15:34:25.000000 obs_img_utils-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:34:33.571694 obs_img_utils-1.3.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:34:33.575693 obs_img_utils-1.3.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-05-08 15:34:25.000000 obs_img_utils-1.3.0/tests/data/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-08 15:34:25.000000 obs_img_utils-1.3.0/tests/data/index.json
--rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-05-08 15:34:25.000000 obs_img_utils-1.3.0/tests/data/index_name_picker.html
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-08 15:34:25.000000 obs_img_utils-1.3.0/tests/data/index_new.html
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-08 15:34:25.000000 obs_img_utils-1.3.0/tests/data/openSUSE-Leap-15.0-Azure.x86_64-1.0.0-Build1.133.packages
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-08 15:34:25.000000 obs_img_utils-1.3.0/tests/data/report
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-05-08 15:34:25.000000 obs_img_utils-1.3.0/tests/test_obs_img_utils_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     9723 2024-05-08 15:34:25.000000 obs_img_utils-1.3.0/tests/test_obs_img_utils_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-05-08 15:34:25.000000 obs_img_utils-1.3.0/tests/test_obs_img_utils_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-05-08 15:34:25.000000 obs_img_utils-1.3.0/tests/test_web_content.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:34:31.944084 obs_img_utils-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-05-28 20:34:21.000000 obs_img_utils-1.4.0/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-28 20:34:21.000000 obs_img_utils-1.4.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    32402 2024-05-28 20:34:21.000000 obs_img_utils-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-28 20:34:21.000000 obs_img_utils-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-05-28 20:34:31.940084 obs_img_utils-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-28 20:34:21.000000 obs_img_utils-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:34:31.936084 obs_img_utils-1.4.0/obs_img_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-28 20:34:21.000000 obs_img_utils-1.4.0/obs_img_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21144 2024-05-28 20:34:21.000000 obs_img_utils-1.4.0/obs_img_utils/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10741 2024-05-28 20:34:21.000000 obs_img_utils-1.4.0/obs_img_utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-05-28 20:34:21.000000 obs_img_utils-1.4.0/obs_img_utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13318 2024-05-28 20:34:21.000000 obs_img_utils-1.4.0/obs_img_utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5958 2024-05-28 20:34:21.000000 obs_img_utils-1.4.0/obs_img_utils/web_content.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:34:31.940084 obs_img_utils-1.4.0/obs_img_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-05-28 20:34:31.000000 obs_img_utils-1.4.0/obs_img_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-28 20:34:31.000000 obs_img_utils-1.4.0/obs_img_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 20:34:31.000000 obs_img_utils-1.4.0/obs_img_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-28 20:34:31.000000 obs_img_utils-1.4.0/obs_img_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 20:34:31.000000 obs_img_utils-1.4.0/obs_img_utils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-28 20:34:31.000000 obs_img_utils-1.4.0/obs_img_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-28 20:34:31.000000 obs_img_utils-1.4.0/obs_img_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-28 20:34:21.000000 obs_img_utils-1.4.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-28 20:34:21.000000 obs_img_utils-1.4.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-28 20:34:21.000000 obs_img_utils-1.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 20:34:31.944084 obs_img_utils-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-28 20:34:21.000000 obs_img_utils-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:34:31.940084 obs_img_utils-1.4.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:34:31.940084 obs_img_utils-1.4.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-05-28 20:34:21.000000 obs_img_utils-1.4.0/tests/data/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-28 20:34:21.000000 obs_img_utils-1.4.0/tests/data/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-05-28 20:34:21.000000 obs_img_utils-1.4.0/tests/data/index_name_picker.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-28 20:34:21.000000 obs_img_utils-1.4.0/tests/data/index_new.html
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-28 20:34:21.000000 obs_img_utils-1.4.0/tests/data/openSUSE-Leap-15.0-Azure.x86_64-1.0.0-Build1.133.packages
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-28 20:34:21.000000 obs_img_utils-1.4.0/tests/data/report
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-05-28 20:34:21.000000 obs_img_utils-1.4.0/tests/test_obs_img_utils_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9723 2024-05-28 20:34:21.000000 obs_img_utils-1.4.0/tests/test_obs_img_utils_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-05-28 20:34:21.000000 obs_img_utils-1.4.0/tests/test_obs_img_utils_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-05-28 20:34:21.000000 obs_img_utils-1.4.0/tests/test_web_content.py
```

### Comparing `obs_img_utils-1.3.0/CHANGES.md` & `obs_img_utils-1.4.0/CHANGES.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+v1.4.0 (2024-05-28)
+===================
+
+- Update python version support and CI testing
+- Update spec for pyton 3.11 build
+
 v1.3.0 (2024-05-08)
 ===================
 
 - Do not raise if image metadata not found unless conditions are provided
 - Cleanup tests and rename setup method
 - Update readthedocs config file
```

### Comparing `obs_img_utils-1.3.0/CONTRIBUTING.md` & `obs_img_utils-1.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `obs_img_utils-1.3.0/LICENSE` & `obs_img_utils-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `obs_img_utils-1.3.0/PKG-INFO` & `obs_img_utils-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: obs-img-utils
-Version: 1.3.0
+Version: 1.4.0
 Summary: Package provides utils for images in Open Build Service.
 Home-page: https://github.com/SUSE-Enceladus/obs-img-utils
 Author: SUSE
 Author-email: public-cloud-dev@susecloud.net
 License: GPLv3+
 Keywords: obs-img-utils obs_img_utils
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Requires-Python: >=3.5
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: lxml
 Requires-Dist: pyyaml
 Requires-Dist: xmltodict
 Provides-Extra: dev
```

### Comparing `obs_img_utils-1.3.0/README.md` & `obs_img_utils-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `obs_img_utils-1.3.0/obs_img_utils/__init__.py` & `obs_img_utils-1.4.0/obs_img_utils/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 __author__ = """SUSE"""
 __email__ = 'public-cloud-dev@susecloud.net'
-__version__ = '1.3.0'
+__version__ = '1.4.0'
```

### Comparing `obs_img_utils-1.3.0/obs_img_utils/api.py` & `obs_img_utils-1.4.0/obs_img_utils/api.py`

 * *Files identical despite different names*

### Comparing `obs_img_utils-1.3.0/obs_img_utils/cli.py` & `obs_img_utils-1.4.0/obs_img_utils/cli.py`

 * *Files identical despite different names*

### Comparing `obs_img_utils-1.3.0/obs_img_utils/exceptions.py` & `obs_img_utils-1.4.0/obs_img_utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `obs_img_utils-1.3.0/obs_img_utils/utils.py` & `obs_img_utils-1.4.0/obs_img_utils/utils.py`

 * *Files identical despite different names*

### Comparing `obs_img_utils-1.3.0/obs_img_utils/web_content.py` & `obs_img_utils-1.4.0/obs_img_utils/web_content.py`

 * *Files identical despite different names*

### Comparing `obs_img_utils-1.3.0/obs_img_utils.egg-info/PKG-INFO` & `obs_img_utils-1.4.0/obs_img_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: obs-img-utils
-Version: 1.3.0
+Version: 1.4.0
 Summary: Package provides utils for images in Open Build Service.
 Home-page: https://github.com/SUSE-Enceladus/obs-img-utils
 Author: SUSE
 Author-email: public-cloud-dev@susecloud.net
 License: GPLv3+
 Keywords: obs-img-utils obs_img_utils
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Requires-Python: >=3.5
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: lxml
 Requires-Dist: pyyaml
 Requires-Dist: xmltodict
 Provides-Extra: dev
```

### Comparing `obs_img_utils-1.3.0/obs_img_utils.egg-info/SOURCES.txt` & `obs_img_utils-1.4.0/obs_img_utils.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 obs_img_utils.egg-info/PKG-INFO
 obs_img_utils.egg-info/SOURCES.txt
 obs_img_utils.egg-info/dependency_links.txt
 obs_img_utils.egg-info/entry_points.txt
 obs_img_utils.egg-info/not-zip-safe
 obs_img_utils.egg-info/requires.txt
 obs_img_utils.egg-info/top_level.txt
-package/python3-obs-img-utils.spec
 tests/test_obs_img_utils_api.py
 tests/test_obs_img_utils_cli.py
 tests/test_obs_img_utils_utils.py
 tests/test_web_content.py
 tests/data/index.html
 tests/data/index.json
 tests/data/index_name_picker.html
```

### Comparing `obs_img_utils-1.3.0/setup.py` & `obs_img_utils-1.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 with open('requirements-dev.txt') as req_file:
     dev_requirements = test_requirements + req_file.read().splitlines()[2:]
 
 
 setup(
     name='obs-img-utils',
-    version='1.3.0',
+    version='1.4.0',
     description="Package provides utils for images in Open Build Service.",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="SUSE",
     author_email='public-cloud-dev@susecloud.net',
     url='https://github.com/SUSE-Enceladus/obs-img-utils',
     packages=find_packages(),
@@ -51,15 +51,15 @@
     },
     entry_points={
         'console_scripts': [
             'obs-img-utils=obs_img_utils.cli:main'
         ]
     },
     include_package_data=True,
-    python_requires='>=3.5',
+    python_requires='>=3.8',
     install_requires=requirements,
     extras_require={
         'dev': dev_requirements,
         'test': test_requirements
     },
     license='GPLv3+',
     zip_safe=False,
@@ -69,12 +69,13 @@
         'Environment :: Console',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: '
         'GNU General Public License v3 or later (GPLv3+)',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
 )
```

### Comparing `obs_img_utils-1.3.0/tests/data/index.html` & `obs_img_utils-1.4.0/tests/data/index.html`

 * *Files identical despite different names*

### Comparing `obs_img_utils-1.3.0/tests/data/index_name_picker.html` & `obs_img_utils-1.4.0/tests/data/index_name_picker.html`

 * *Files identical despite different names*

### Comparing `obs_img_utils-1.3.0/tests/data/index_new.html` & `obs_img_utils-1.4.0/tests/data/index_new.html`

 * *Files identical despite different names*

### Comparing `obs_img_utils-1.3.0/tests/test_obs_img_utils_api.py` & `obs_img_utils-1.4.0/tests/test_obs_img_utils_api.py`

 * *Files identical despite different names*

### Comparing `obs_img_utils-1.3.0/tests/test_obs_img_utils_cli.py` & `obs_img_utils-1.4.0/tests/test_obs_img_utils_cli.py`

 * *Files identical despite different names*

### Comparing `obs_img_utils-1.3.0/tests/test_obs_img_utils_utils.py` & `obs_img_utils-1.4.0/tests/test_obs_img_utils_utils.py`

 * *Files identical despite different names*

### Comparing `obs_img_utils-1.3.0/tests/test_web_content.py` & `obs_img_utils-1.4.0/tests/test_web_content.py`

 * *Files identical despite different names*

