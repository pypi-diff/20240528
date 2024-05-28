# Comparing `tmp/aliyun-img-utils-2.1.0.tar.gz` & `tmp/aliyun_img_utils-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aliyun-img-utils-2.1.0.tar", last modified: Wed May 25 21:29:21 2022, max compression
+gzip compressed data, was "aliyun_img_utils-2.2.0.tar", last modified: Tue May 28 19:13:35 2024, max compression
```

## Comparing `aliyun-img-utils-2.1.0.tar` & `aliyun_img_utils-2.2.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 21:29:21.513535 aliyun-img-utils-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1962 2022-05-25 21:29:10.000000 aliyun-img-utils-2.1.0/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (121)     2502 2022-05-25 21:29:10.000000 aliyun-img-utils-2.1.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)    32403 2022-05-25 21:29:10.000000 aliyun-img-utils-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      420 2022-05-25 21:29:10.000000 aliyun-img-utils-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    11439 2022-05-25 21:29:21.513535 aliyun-img-utils-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    10424 2022-05-25 21:29:10.000000 aliyun-img-utils-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 21:29:21.509535 aliyun-img-utils-2.1.0/aliyun_img_utils/
--rw-r--r--   0 runner    (1001) docker     (121)      999 2022-05-25 21:29:10.000000 aliyun-img-utils-2.1.0/aliyun_img_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18669 2022-05-25 21:29:10.000000 aliyun-img-utils-2.1.0/aliyun_img_utils/aliyun_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     1323 2022-05-25 21:29:10.000000 aliyun-img-utils-2.1.0/aliyun_img_utils/aliyun_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    25525 2022-05-25 21:29:10.000000 aliyun-img-utils-2.1.0/aliyun_img_utils/aliyun_image.py
--rw-r--r--   0 runner    (1001) docker     (121)     9231 2022-05-25 21:29:10.000000 aliyun-img-utils-2.1.0/aliyun_img_utils/aliyun_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 21:29:21.513535 aliyun-img-utils-2.1.0/aliyun_img_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    11439 2022-05-25 21:29:21.000000 aliyun-img-utils-2.1.0/aliyun_img_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      689 2022-05-25 21:29:21.000000 aliyun-img-utils-2.1.0/aliyun_img_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-25 21:29:21.000000 aliyun-img-utils-2.1.0/aliyun_img_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-05-25 21:29:21.000000 aliyun-img-utils-2.1.0/aliyun_img_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-25 21:29:21.000000 aliyun-img-utils-2.1.0/aliyun_img_utils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-05-25 21:29:21.000000 aliyun-img-utils-2.1.0/aliyun_img_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-05-25 21:29:21.000000 aliyun-img-utils-2.1.0/aliyun_img_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-05-25 21:29:10.000000 aliyun-img-utils-2.1.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-05-25 21:29:10.000000 aliyun-img-utils-2.1.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-05-25 21:29:10.000000 aliyun-img-utils-2.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-05-25 21:29:21.513535 aliyun-img-utils-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2784 2022-05-25 21:29:10.000000 aliyun-img-utils-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 21:29:21.513535 aliyun-img-utils-2.1.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 21:29:21.513535 aliyun-img-utils-2.1.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-05-25 21:29:10.000000 aliyun-img-utils-2.1.0/tests/data/blob.vhd
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-05-25 21:29:10.000000 aliyun-img-utils-2.1.0/tests/data/default.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    14670 2022-05-25 21:29:10.000000 aliyun-img-utils-2.1.0/tests/test_aliyun_image.py
--rw-r--r--   0 runner    (1001) docker     (121)     5991 2022-05-25 21:29:10.000000 aliyun-img-utils-2.1.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     2735 2022-05-25 21:29:10.000000 aliyun-img-utils-2.1.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:13:35.271118 aliyun_img_utils-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-28 19:13:22.000000 aliyun_img_utils-2.2.0/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-28 19:13:22.000000 aliyun_img_utils-2.2.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    32403 2024-05-28 19:13:22.000000 aliyun_img_utils-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-28 19:13:22.000000 aliyun_img_utils-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-05-28 19:13:35.271118 aliyun_img_utils-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10424 2024-05-28 19:13:22.000000 aliyun_img_utils-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:13:35.267118 aliyun_img_utils-2.2.0/aliyun_img_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-28 19:13:22.000000 aliyun_img_utils-2.2.0/aliyun_img_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19588 2024-05-28 19:13:22.000000 aliyun_img_utils-2.2.0/aliyun_img_utils/aliyun_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-28 19:13:22.000000 aliyun_img_utils-2.2.0/aliyun_img_utils/aliyun_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25990 2024-05-28 19:13:22.000000 aliyun_img_utils-2.2.0/aliyun_img_utils/aliyun_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-05-28 19:13:22.000000 aliyun_img_utils-2.2.0/aliyun_img_utils/aliyun_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:13:35.271118 aliyun_img_utils-2.2.0/aliyun_img_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-05-28 19:13:35.000000 aliyun_img_utils-2.2.0/aliyun_img_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-28 19:13:35.000000 aliyun_img_utils-2.2.0/aliyun_img_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 19:13:35.000000 aliyun_img_utils-2.2.0/aliyun_img_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-28 19:13:35.000000 aliyun_img_utils-2.2.0/aliyun_img_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 19:13:35.000000 aliyun_img_utils-2.2.0/aliyun_img_utils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-28 19:13:35.000000 aliyun_img_utils-2.2.0/aliyun_img_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-28 19:13:35.000000 aliyun_img_utils-2.2.0/aliyun_img_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-28 19:13:22.000000 aliyun_img_utils-2.2.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-28 19:13:22.000000 aliyun_img_utils-2.2.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-28 19:13:22.000000 aliyun_img_utils-2.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-28 19:13:35.271118 aliyun_img_utils-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-05-28 19:13:22.000000 aliyun_img_utils-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:13:35.271118 aliyun_img_utils-2.2.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 19:13:35.271118 aliyun_img_utils-2.2.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-28 19:13:22.000000 aliyun_img_utils-2.2.0/tests/data/blob.vhd
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-28 19:13:22.000000 aliyun_img_utils-2.2.0/tests/data/default.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    15178 2024-05-28 19:13:22.000000 aliyun_img_utils-2.2.0/tests/test_aliyun_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6475 2024-05-28 19:13:22.000000 aliyun_img_utils-2.2.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-28 19:13:22.000000 aliyun_img_utils-2.2.0/tests/test_utils.py
```

### Comparing `aliyun-img-utils-2.1.0/CHANGES.md` & `aliyun_img_utils-2.2.0/CHANGES.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v2.2.0 (2024-05-28)
+===================
+
+- Increase the timeout for wait on image method
+- Remove superfluous delete blob option
+- Add endpoint for retrieving image share permission
+- Update python versions for ci testing
+- Migrate spec file to build for python 3.11
+
 v2.1.0 (2022-05-25)
 ===================
 
 - Consistant error handling in class methods
 - Sanitize all HttpErrors
 
 v2.0.0 (2022-02-09)
```

### Comparing `aliyun-img-utils-2.1.0/CONTRIBUTING.md` & `aliyun_img_utils-2.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `aliyun-img-utils-2.1.0/LICENSE` & `aliyun_img_utils-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-img-utils-2.1.0/PKG-INFO` & `aliyun_img_utils-2.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,7 @@
-Metadata-Version: 2.1
-Name: aliyun-img-utils
-Version: 2.1.0
-Summary: Package that provides utilities for handling images in Aliyun Cloud.
-Home-page: https://github.com/SUSE-Enceladus/aliyun-img-utils
-Author: SUSE
-Author-email: public-cloud-dev@susecloud.net
-License: GPLv3+
-Keywords: aliyun-img-utils aliyun_img_utils
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: System :: Software Distribution
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: test
-License-File: LICENSE
-
 # Overview
 
 **aliyun-img-utils** provides a command line utility and API for publishing
 images in the Aliyun Cloud. This includes helper functions for uploading
 image blobs, creating compute images and replicating/publishing/deprecating/
 images across all available regions.
 
@@ -412,9 +385,7 @@
 # License
 
 Copyright (c) 2021 SUSE LLC.
 
 Distributed under the terms of GPL-3.0+ license, see
 [LICENSE](https://github.com/SUSE-Enceladus/aliyun-img-utils/blob/master/LICENSE)
 for details.
-
-
```

### Comparing `aliyun-img-utils-2.1.0/README.md` & `aliyun_img_utils-2.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,48 @@
+Metadata-Version: 2.1
+Name: aliyun-img-utils
+Version: 2.2.0
+Summary: Package that provides utilities for handling images in Aliyun Cloud.
+Home-page: https://github.com/SUSE-Enceladus/aliyun-img-utils
+Author: SUSE
+Author-email: public-cloud-dev@susecloud.net
+License: GPLv3+
+Keywords: aliyun-img-utils aliyun_img_utils
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: System :: Software Distribution
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: click
+Requires-Dist: oss2
+Requires-Dist: PyYAML
+Requires-Dist: aliyun-python-sdk-core
+Requires-Dist: aliyun-python-sdk-ecs
+Requires-Dist: python-dateutil
+Provides-Extra: dev
+Requires-Dist: coverage; extra == "dev"
+Requires-Dist: flake8; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: bumpversion; extra == "dev"
+Requires-Dist: pip>=7.0.0; extra == "dev"
+Provides-Extra: test
+Requires-Dist: coverage; extra == "test"
+Requires-Dist: flake8; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
+
 # Overview
 
 **aliyun-img-utils** provides a command line utility and API for publishing
 images in the Aliyun Cloud. This includes helper functions for uploading
 image blobs, creating compute images and replicating/publishing/deprecating/
 images across all available regions.
```

### Comparing `aliyun-img-utils-2.1.0/aliyun_img_utils/__init__.py` & `aliyun_img_utils-2.2.0/aliyun_img_utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,8 +18,8 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 __author__ = """SUSE"""
 __email__ = 'public-cloud-dev@susecloud.net'
-__version__ = '2.1.0'
+__version__ = '2.2.0'
```

### Comparing `aliyun-img-utils-2.1.0/aliyun_img_utils/aliyun_cli.py` & `aliyun_img_utils-2.2.0/aliyun_img_utils/aliyun_cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -340,34 +340,29 @@
 @click.option(
     '--image-name',
     type=click.STRING,
     help='Name of the image to be deleted.',
     required=True
 )
 @click.option(
-    '--delete-blob',
-    is_flag=True,
-    help='Also delete the image blob from storage bucket.'
-)
-@click.option(
     '--force',
     is_flag=True,
     help='Forcibly deletes the custom image, regardless of '
          'whether the image is being used by other instances.'
 )
 @click.option(
     '--regions',
     help='A comma separated list of region ids for '
          'deleting the provided image. If no regions '
          'are provided the image will be deleted in all '
          'available regions.'
 )
 @add_options(shared_options)
 @click.pass_context
-def delete(context, image_name, delete_blob, force, regions, **kwargs):
+def delete(context, image_name, force, regions, **kwargs):
     """Delete a compute image and optionally the backing qcow2 blob."""
     process_shared_options(context.obj, kwargs)
     config_data = get_config(context.obj)
     logger = get_logger(config_data.log_level)
 
     with handle_errors(config_data.log_level, config_data.no_color):
         aliyun_image = AliyunImage(
@@ -376,15 +371,14 @@
             config_data.region,
             config_data.bucket_name,
             log_level=config_data.log_level,
             log_callback=logger
         )
 
         keyword_args = {
-            'delete_blob': delete_blob,
             'force': force
         }
 
         if regions:
             regions = regions.split(',')
             keyword_args['regions'] = regions
 
@@ -687,16 +681,57 @@
 
     echo_style(
         json.dumps(image_data, indent=2),
         config_data.no_color
     )
 
 
+@click.command()
+@click.option(
+    '--image-name',
+    type=click.STRING,
+    help='Name of the image to get share permission.',
+    required=True
+)
+@add_options(shared_options)
+@click.pass_context
+def share_permission(context, image_name, **kwargs):
+    """
+    Describe compute image share permission in the current region.
+    """
+    process_shared_options(context.obj, kwargs)
+    config_data = get_config(context.obj)
+    logger = get_logger(config_data.log_level)
+
+    with handle_errors(config_data.log_level, config_data.no_color):
+        aliyun_image = AliyunImage(
+            config_data.access_key,
+            config_data.access_secret,
+            config_data.region,
+            config_data.bucket_name,
+            log_level=config_data.log_level,
+            log_callback=logger
+        )
+
+        keyword_args = {}
+
+        response = aliyun_image.describe_share_permission(
+            image_name,
+            **keyword_args
+        )
+
+    echo_style(
+        json.dumps(response, indent=2),
+        config_data.no_color
+    )
+
+
 image.add_command(activate)
 image.add_command(create)
 image.add_command(delete)
 image.add_command(deprecate)
 image.add_command(publish)
 image.add_command(replicate)
 image.add_command(upload)
 image.add_command(info)
+image.add_command(share_permission)
 main.add_command(image)
```

### Comparing `aliyun-img-utils-2.1.0/aliyun_img_utils/aliyun_exceptions.py` & `aliyun_img_utils-2.2.0/aliyun_img_utils/aliyun_exceptions.py`

 * *Files identical despite different names*

### Comparing `aliyun-img-utils-2.1.0/aliyun_img_utils/aliyun_image.py` & `aliyun_img_utils-2.2.0/aliyun_img_utils/aliyun_image.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,17 @@
 )
 from aliyunsdkecs.request.v20140526.DescribeRegionsRequest import (
     DescribeRegionsRequest
 )
 from aliyunsdkecs.request.v20140526.CopyImageRequest import (
     CopyImageRequest
 )
+from aliyunsdkecs.request.v20140526.DescribeImageSharePermissionRequest import (  # noqa
+    DescribeImageSharePermissionRequest
+)
 from aliyunsdkecs.request.v20140526.ModifyImageSharePermissionRequest import (
     ModifyImageSharePermissionRequest
 )
 from aliyunsdkecs.request.v20140526.ModifyImageAttributeRequest import (
     ModifyImageAttributeRequest
 )
 from aliyunsdkecs.request.v20140526.TagResourcesRequest import (
@@ -228,21 +231,19 @@
         self.wait_on_blob(blob_name)
 
         return blob_name
 
     def delete_compute_image(
         self,
         image_name,
-        delete_blob=False,
         force=False
     ):
         """
-        Delete compute image in current region.
-
-        If delete_blob is True delete the backing storage blob.
+        Delete compute image in current region. This automatically deletes
+        the backing storage object.
         """
         try:
             image = self.get_compute_image(image_name=image_name)
         except AliyunImageException:
             return False
 
         request = DeleteImageRequest()
@@ -259,31 +260,19 @@
             raise AliyunImageException(
                 f'Unable to delete image: {error}.'
             )
 
         self.wait_on_compute_image_delete(image['ImageId'])
         self.log.info(f'{image["ImageId"]} deleted in {self.region}')
 
-        if delete_blob:
-            oss_object = None
-            try:
-                device = image['DiskDeviceMappings']['DiskDeviceMapping'][0]
-                oss_object = device['ImportOSSObject']
-            except (IndexError, KeyError):
-                pass
-
-            if oss_object:
-                self.delete_storage_blob(oss_object)
-
         return True
 
     def delete_compute_image_in_regions(
         self,
         image_name,
-        delete_blob=False,
         force=False,
         regions=None
     ):
         """
         Delete the compute image based on image name in all regions.
 
         If a region list is not provided use all available regions.
@@ -293,15 +282,14 @@
 
         for region in regions:
             self.region = region
 
             try:
                 self.delete_compute_image(
                     image_name,
-                    delete_blob=delete_blob,
                     force=force
                 )
             except Exception as error:
                 self.log.error(
                     f'Failed to delete {image_name} in {self.region}: '
                     f'{error}.'
                 )
@@ -382,15 +370,15 @@
             else:
                 time.sleep(10)
 
         raise AliyunImageException(
             'Image not deleted within 5 minutes.'
         )
 
-    def wait_on_compute_image(self, image_id, timeout=1500):
+    def wait_on_compute_image(self, image_id, timeout=3600):
         """
         Wait for the compute image to show up in region.
 
         If it doesn't show up in 30 mintues raise exception.
         """
         start = time.time()
         end = start + timeout
@@ -418,27 +406,28 @@
                 )
             else:
                 raise AliyunImageException(
                     f'Image in an unknown state: {status}'
                 )
 
         raise AliyunImageException(
-            'Image not available within 30 minutes.'
+            f'Image not available within {timeout} seconds.'
         )
 
     def create_compute_image(
         self,
         image_name,
         image_description,
         blob_name,
         platform,
         os_type='linux',
         arch='x86_64',
         disk_image_size=20,
-        force_replace_image=False
+        force_replace_image=False,
+        timeout=3600
     ):
         """
         Create compute image in current region from storage blob.
 
         If image exists and force replace is True delete the existing
         image before re-creating.
         """
@@ -468,15 +457,15 @@
             )
         except Exception as error:
             raise AliyunImageCreateException(
                 f'Unable to create image: {error}.'
             )
 
         # Image creation is async so wait until image shows up
-        self.wait_on_compute_image(response['ImageId'])
+        self.wait_on_compute_image(response['ImageId'], timeout=timeout)
 
         return response['ImageId']
 
     def copy_compute_image(self, source_image_name, destination_region):
         """
         Copy compute image to specified region.
         """
@@ -526,14 +515,36 @@
                     f'Failed to copy {source_image_name} '
                     f'to {region}: {error}'
                 )
                 images[region] = None
 
         return images
 
+    def describe_share_permission(self, source_image_name):
+        """
+        Describe the images share permissions in current region.
+        """
+        image = self.get_compute_image(image_name=source_image_name)
+
+        request = DescribeImageSharePermissionRequest()
+        request.set_accept_format('json')
+        request.set_ImageId(image['ImageId'])
+
+        try:
+            with handle_http_errors():
+                response = json.loads(
+                    self.compute_client.do_action_with_exception(request)
+                )
+        except Exception as error:
+            raise AliyunImageException(
+                f'Unable to describe share permission for image: {error}.'
+            )
+
+        return response
+
     def publish_image(self, source_image_name, launch_permission):
         """
         Publish compute image in current region.
         """
         image = self.get_compute_image(image_name=source_image_name)
 
         request = ModifyImageSharePermissionRequest()
```

### Comparing `aliyun-img-utils-2.1.0/aliyun_img_utils/aliyun_utils.py` & `aliyun_img_utils-2.2.0/aliyun_img_utils/aliyun_utils.py`

 * *Files identical despite different names*

### Comparing `aliyun-img-utils-2.1.0/aliyun_img_utils.egg-info/PKG-INFO` & `aliyun_img_utils-2.2.0/aliyun_img_utils.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,47 @@
 Metadata-Version: 2.1
 Name: aliyun-img-utils
-Version: 2.1.0
+Version: 2.2.0
 Summary: Package that provides utilities for handling images in Aliyun Cloud.
 Home-page: https://github.com/SUSE-Enceladus/aliyun-img-utils
 Author: SUSE
 Author-email: public-cloud-dev@susecloud.net
 License: GPLv3+
 Keywords: aliyun-img-utils aliyun_img_utils
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: System :: Software Distribution
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.5
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: click
+Requires-Dist: oss2
+Requires-Dist: PyYAML
+Requires-Dist: aliyun-python-sdk-core
+Requires-Dist: aliyun-python-sdk-ecs
+Requires-Dist: python-dateutil
 Provides-Extra: dev
+Requires-Dist: coverage; extra == "dev"
+Requires-Dist: flake8; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: bumpversion; extra == "dev"
+Requires-Dist: pip>=7.0.0; extra == "dev"
 Provides-Extra: test
-License-File: LICENSE
+Requires-Dist: coverage; extra == "test"
+Requires-Dist: flake8; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
 
 # Overview
 
 **aliyun-img-utils** provides a command line utility and API for publishing
 images in the Aliyun Cloud. This includes helper functions for uploading
 image blobs, creating compute images and replicating/publishing/deprecating/
 images across all available regions.
@@ -412,9 +426,7 @@
 # License
 
 Copyright (c) 2021 SUSE LLC.
 
 Distributed under the terms of GPL-3.0+ license, see
 [LICENSE](https://github.com/SUSE-Enceladus/aliyun-img-utils/blob/master/LICENSE)
 for details.
-
-
```

### Comparing `aliyun-img-utils-2.1.0/aliyun_img_utils.egg-info/SOURCES.txt` & `aliyun_img_utils-2.2.0/aliyun_img_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aliyun-img-utils-2.1.0/setup.py` & `aliyun_img_utils-2.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 with open('requirements-dev.txt') as req_file:
     dev_requirements = test_requirements + req_file.read().splitlines()[2:]
 
 
 setup(
     name='aliyun-img-utils',
-    version='2.1.0',
+    version='2.2.0',
     description='Package that provides utilities for '
                 'handling images in Aliyun Cloud.',
     long_description=readme,
     long_description_content_type='text/markdown',
     author='SUSE',
     author_email='public-cloud-dev@susecloud.net',
     url='https://github.com/SUSE-Enceladus/aliyun-img-utils',
@@ -52,15 +52,15 @@
     },
     entry_points={
         'console_scripts': [
             'aliyun-img-utils=aliyun_img_utils.aliyun_cli:main'
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
@@ -70,13 +70,14 @@
         'Environment :: Console',
         'Intended Audience :: Developers',
         'Topic :: System :: Software Distribution',
         'License :: OSI Approved :: '
         'GNU General Public License v3 or later (GPLv3+)',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
     ],
 )
```

### Comparing `aliyun-img-utils-2.1.0/tests/test_aliyun_image.py` & `aliyun_img_utils-2.2.0/tests/test_aliyun_image.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     AliyunImageUploadException
 )
 
 
 class TestAliyunImage(object):
     """Test Aliyun Image class."""
 
-    def setup(self):
+    def setup_method(self):
         self.image = AliyunImage(
             '12345',
             '54321',
             'cn-beijing',
             bucket_name='test-bucket'
         )
 
@@ -163,17 +163,16 @@
             self.image.upload_image_tarball(
                 'tests/data/blob.qcow2',
                 page_size=8 * 8 * 1024,
                 progress_callback=callback,
                 force_replace_image=True
             )
 
-    @patch.object(AliyunImage, 'delete_storage_blob')
     @patch.object(AliyunImage, 'get_compute_image')
-    def test_delete_compute_image(self, mock_get_image, mock_delete_tarball):
+    def test_delete_compute_image(self, mock_get_image):
         image = {
             'ImageId': 'm-123',
             'DiskDeviceMappings': {
                 'DiskDeviceMapping': [{'ImportOSSObject': 'test-blob'}]
             }
         }
         mock_get_image.side_effect = [
@@ -183,22 +182,20 @@
         ]
 
         client = Mock()
         self.image._compute_client = client
 
         assert self.image.delete_compute_image(
             'test-image',
-            delete_blob=True,
             force=True
         )
 
         # Image not exists
         assert self.image.delete_compute_image(
             'test-image',
-            delete_blob=True
         ) is False
 
     @patch.object(AliyunImage, 'delete_compute_image')
     @patch.object(AliyunImage, 'get_regions')
     def test_delete_compute_image_in_regions(
         self,
         mock_get_regions,
@@ -441,7 +438,24 @@
             self.image.wait_on_compute_image('m-123')
 
         image = {'ImageId': 'm-123', 'Status': 'Available'}
         mock_get_image.return_value = image
 
         # Available state
         self.image.wait_on_compute_image('m-123')
+
+    @patch.object(AliyunImage, 'get_compute_image')
+    def test_get_share_permission(self, mock_get_image):
+        image = {'ImageId': 'm-123', 'Status': 'Available'}
+        mock_get_image.return_value = image
+
+        client = Mock()
+        self.image._compute_client = client
+
+        client.do_action_with_exception.return_value = (
+            '{"share_groups": [], "accounts": {"account": []}}'
+        )
+        self.image.describe_share_permission('m-123')
+
+        client.do_action_with_exception.side_effect = Exception
+        with raises(AliyunImageException):
+            self.image.describe_share_permission('m-123')
```

### Comparing `aliyun-img-utils-2.1.0/tests/test_cli.py` & `aliyun_img_utils-2.2.0/tests/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,7 +181,24 @@
         '--regions', 'cn-beijing,cn-shanghai'
     ]
 
     runner = CliRunner()
     result = runner.invoke(main, args)
     assert result.exit_code == 0
     assert 'Image activated' in result.output
+
+
+@patch('aliyun_img_utils.aliyun_cli.AliyunImage')
+def test_cli_share_permission(mock_img_class):
+    image_class = MagicMock()
+    image_class.describe_share_permission.return_value = (
+        '{"share_groups": [], "accounts": {"account": []}}'
+    )
+    mock_img_class.return_value = image_class
+
+    args = [
+        'image', 'share-permission', '--image-name', 'test-image'
+    ]
+
+    runner = CliRunner()
+    result = runner.invoke(main, args)
+    assert result.exit_code == 0
```

### Comparing `aliyun-img-utils-2.1.0/tests/test_utils.py` & `aliyun_img_utils-2.2.0/tests/test_utils.py`

 * *Files identical despite different names*

