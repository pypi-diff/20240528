# Comparing `tmp/wideo-0.5.0.tar.gz` & `tmp/wideo-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wideo-0.5.0.tar", max compression
+gzip compressed data, was "wideo-0.6.0.tar", max compression
```

## Comparing `wideo-0.5.0.tar` & `wideo-0.6.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0      674 2024-01-31 15:27:01.410416 wideo-0.5.0/README.md
--rw-r--r--   0        0        0      469 2024-01-31 15:27:01.418417 wideo-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1584 2024-01-31 15:27:01.418417 wideo-0.5.0/src/wideo/__init__.py
--rw-r--r--   0        0        0      767 2024-01-31 15:27:01.418417 wideo-0.5.0/src/wideo/admin_urls.py
--rw-r--r--   0        0        0      174 2024-01-31 15:27:01.418417 wideo-0.5.0/src/wideo/apps.py
--rw-r--r--   0        0        0      470 2024-01-31 15:27:01.418417 wideo-0.5.0/src/wideo/blocks.py
--rw-r--r--   0        0        0     2696 2024-01-31 15:27:01.418417 wideo-0.5.0/src/wideo/codecs.py
--rw-r--r--   0        0        0       92 2024-01-31 15:27:01.418417 wideo-0.5.0/src/wideo/exceptions.py
--rw-r--r--   0        0        0     7726 2024-01-31 15:27:01.418417 wideo-0.5.0/src/wideo/ffmpeg.py
--rw-r--r--   0        0        0      329 2024-01-31 15:27:01.418417 wideo-0.5.0/src/wideo/fields.py
--rw-r--r--   0        0        0      334 2024-01-31 15:27:01.418417 wideo-0.5.0/src/wideo/forms.py
--rw-r--r--   0        0        0        0 2024-01-31 15:27:01.418417 wideo-0.5.0/src/wideo/management/__init__.py
--rw-r--r--   0        0        0        0 2024-01-31 15:27:01.418417 wideo-0.5.0/src/wideo/management/commands/__init__.py
--rw-r--r--   0        0        0      321 2024-01-31 15:27:01.418417 wideo-0.5.0/src/wideo/management/commands/delete_orphan_uploaded_videos.py
--rw-r--r--   0        0        0      552 2024-01-31 15:27:01.418417 wideo-0.5.0/src/wideo/management/commands/encode_videos.py
--rw-r--r--   0        0        0     9737 2024-01-31 15:27:01.418417 wideo-0.5.0/src/wideo/migrations/0001_initial.py
--rw-r--r--   0        0        0      676 2024-01-31 15:27:01.418417 wideo-0.5.0/src/wideo/migrations/0002_lock.py
--rw-r--r--   0        0        0     2955 2024-01-31 15:27:01.418417 wideo-0.5.0/src/wideo/migrations/0003_uploadedvideochunk.py
--rw-r--r--   0        0        0      666 2024-01-31 15:27:01.418417 wideo-0.5.0/src/wideo/migrations/0004_alter_video_upload.py
--rw-r--r--   0        0        0      696 2024-01-31 15:27:01.418417 wideo-0.5.0/src/wideo/migrations/0005_alter_video_upload.py
--rw-r--r--   0        0        0        0 2024-01-31 15:27:01.418417 wideo-0.5.0/src/wideo/migrations/__init__.py
--rw-r--r--   0        0        0     6482 2024-01-31 15:27:01.418417 wideo-0.5.0/src/wideo/models.py
--rw-r--r--   0        0        0      777 2024-01-31 15:27:01.418417 wideo-0.5.0/src/wideo/permissions.py
--rw-r--r--   0        0        0     1544 2024-01-31 15:27:01.418417 wideo-0.5.0/src/wideo/signals.py
--rw-r--r--   0        0        0     1301 2024-01-31 15:27:01.418417 wideo-0.5.0/src/wideo/storage.py
--rw-r--r--   0        0        0      655 2024-01-31 15:27:01.418417 wideo-0.5.0/src/wideo/tasks.py
--rw-r--r--   0        0        0      222 2024-01-31 15:27:01.418417 wideo-0.5.0/src/wideo/templates/wideo/blocks/video.html
--rw-r--r--   0        0        0     4210 2024-01-31 15:27:01.418417 wideo-0.5.0/src/wideo/templates/wideo/forms/file.html
--rw-r--r--   0        0        0      190 2024-01-31 15:27:01.418417 wideo-0.5.0/src/wideo/templates/wideo/forms/file_edit.html
--rw-r--r--   0        0        0      179 2024-01-31 15:27:01.418417 wideo-0.5.0/src/wideo/templates/wideo/icons/video.svg
--rw-r--r--   0        0        0      457 2024-01-31 15:27:01.418417 wideo-0.5.0/src/wideo/templates/wideo/preview/plyr_styles.html
--rw-r--r--   0        0        0     1757 2024-01-31 15:27:01.418417 wideo-0.5.0/src/wideo/templates/wideo/preview/video_source.html
--rw-r--r--   0        0        0      124 2024-01-31 15:27:01.418417 wideo-0.5.0/src/wideo/templates/wideo/video.html
--rw-r--r--   0        0        0     3303 2024-01-31 15:27:01.418417 wideo-0.5.0/src/wideo/templates/wideo/videos/add.html
--rw-r--r--   0        0        0     1621 2024-01-31 15:27:01.418417 wideo-0.5.0/src/wideo/templates/wideo/videos/confirm_delete.html
--rw-r--r--   0        0        0     2690 2024-01-31 15:27:01.418417 wideo-0.5.0/src/wideo/templates/wideo/videos/edit.html
--rw-r--r--   0        0        0     4455 2024-01-31 15:27:01.418417 wideo-0.5.0/src/wideo/templates/wideo/videos/index.html
--rw-r--r--   0        0        0     2586 2024-01-31 15:27:01.418417 wideo-0.5.0/src/wideo/templates/wideo/videos/results.html
--rw-r--r--   0        0        0        0 2024-01-31 15:27:01.418417 wideo-0.5.0/src/wideo/templates/wideo/videos/results_video.html
--rw-r--r--   0        0        0        0 2024-01-31 15:27:01.418417 wideo-0.5.0/src/wideo/templatetags/__init__.py
--rw-r--r--   0        0        0      231 2024-01-31 15:27:01.418417 wideo-0.5.0/src/wideo/templatetags/settings.py
--rw-r--r--   0        0        0    14570 2024-01-31 15:27:01.418417 wideo-0.5.0/src/wideo/views.py
--rw-r--r--   0        0        0      612 2024-01-31 15:27:01.418417 wideo-0.5.0/src/wideo/wagtail_hooks.py
--rw-r--r--   0        0        0      126 2024-01-31 15:27:01.418417 wideo-0.5.0/src/wideo/widgets.py
--rw-r--r--   0        0        0     1228 1970-01-01 00:00:00.000000 wideo-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      674 2024-05-28 12:34:51.374830 wideo-0.6.0/README.md
+-rw-r--r--   0        0        0      468 2024-05-28 12:34:51.382830 wideo-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1584 2024-05-28 12:34:51.382830 wideo-0.6.0/src/wideo/__init__.py
+-rw-r--r--   0        0        0      767 2024-05-28 12:34:51.382830 wideo-0.6.0/src/wideo/admin_urls.py
+-rw-r--r--   0        0        0      174 2024-05-28 12:34:51.382830 wideo-0.6.0/src/wideo/apps.py
+-rw-r--r--   0        0        0      470 2024-05-28 12:34:51.382830 wideo-0.6.0/src/wideo/blocks.py
+-rw-r--r--   0        0        0     2696 2024-05-28 12:34:51.382830 wideo-0.6.0/src/wideo/codecs.py
+-rw-r--r--   0        0        0       92 2024-05-28 12:34:51.382830 wideo-0.6.0/src/wideo/exceptions.py
+-rw-r--r--   0        0        0     7726 2024-05-28 12:34:51.382830 wideo-0.6.0/src/wideo/ffmpeg.py
+-rw-r--r--   0        0        0      329 2024-05-28 12:34:51.382830 wideo-0.6.0/src/wideo/fields.py
+-rw-r--r--   0        0        0      334 2024-05-28 12:34:51.382830 wideo-0.6.0/src/wideo/forms.py
+-rw-r--r--   0        0        0        0 2024-05-28 12:34:51.382830 wideo-0.6.0/src/wideo/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 12:34:51.382830 wideo-0.6.0/src/wideo/management/commands/__init__.py
+-rw-r--r--   0        0        0      321 2024-05-28 12:34:51.382830 wideo-0.6.0/src/wideo/management/commands/delete_orphan_uploaded_videos.py
+-rw-r--r--   0        0        0      552 2024-05-28 12:34:51.382830 wideo-0.6.0/src/wideo/management/commands/encode_videos.py
+-rw-r--r--   0        0        0     9737 2024-05-28 12:34:51.382830 wideo-0.6.0/src/wideo/migrations/0001_initial.py
+-rw-r--r--   0        0        0      676 2024-05-28 12:34:51.382830 wideo-0.6.0/src/wideo/migrations/0002_lock.py
+-rw-r--r--   0        0        0     2955 2024-05-28 12:34:51.382830 wideo-0.6.0/src/wideo/migrations/0003_uploadedvideochunk.py
+-rw-r--r--   0        0        0      666 2024-05-28 12:34:51.382830 wideo-0.6.0/src/wideo/migrations/0004_alter_video_upload.py
+-rw-r--r--   0        0        0      696 2024-05-28 12:34:51.382830 wideo-0.6.0/src/wideo/migrations/0005_alter_video_upload.py
+-rw-r--r--   0        0        0        0 2024-05-28 12:34:51.382830 wideo-0.6.0/src/wideo/migrations/__init__.py
+-rw-r--r--   0        0        0     6482 2024-05-28 12:34:51.382830 wideo-0.6.0/src/wideo/models.py
+-rw-r--r--   0        0        0      777 2024-05-28 12:34:51.382830 wideo-0.6.0/src/wideo/permissions.py
+-rw-r--r--   0        0        0     1544 2024-05-28 12:34:51.382830 wideo-0.6.0/src/wideo/signals.py
+-rw-r--r--   0        0        0     1301 2024-05-28 12:34:51.382830 wideo-0.6.0/src/wideo/storage.py
+-rw-r--r--   0        0        0      655 2024-05-28 12:34:51.382830 wideo-0.6.0/src/wideo/tasks.py
+-rw-r--r--   0        0        0      222 2024-05-28 12:34:51.382830 wideo-0.6.0/src/wideo/templates/wideo/blocks/video.html
+-rw-r--r--   0        0        0     4210 2024-05-28 12:34:51.382830 wideo-0.6.0/src/wideo/templates/wideo/forms/file.html
+-rw-r--r--   0        0        0      190 2024-05-28 12:34:51.382830 wideo-0.6.0/src/wideo/templates/wideo/forms/file_edit.html
+-rw-r--r--   0        0        0      179 2024-05-28 12:34:51.382830 wideo-0.6.0/src/wideo/templates/wideo/icons/video.svg
+-rw-r--r--   0        0        0      457 2024-05-28 12:34:51.382830 wideo-0.6.0/src/wideo/templates/wideo/preview/plyr_styles.html
+-rw-r--r--   0        0        0     1757 2024-05-28 12:34:51.382830 wideo-0.6.0/src/wideo/templates/wideo/preview/video_source.html
+-rw-r--r--   0        0        0      124 2024-05-28 12:34:51.382830 wideo-0.6.0/src/wideo/templates/wideo/video.html
+-rw-r--r--   0        0        0     3303 2024-05-28 12:34:51.382830 wideo-0.6.0/src/wideo/templates/wideo/videos/add.html
+-rw-r--r--   0        0        0     1621 2024-05-28 12:34:51.382830 wideo-0.6.0/src/wideo/templates/wideo/videos/confirm_delete.html
+-rw-r--r--   0        0        0     2690 2024-05-28 12:34:51.382830 wideo-0.6.0/src/wideo/templates/wideo/videos/edit.html
+-rw-r--r--   0        0        0     4455 2024-05-28 12:34:51.382830 wideo-0.6.0/src/wideo/templates/wideo/videos/index.html
+-rw-r--r--   0        0        0     2586 2024-05-28 12:34:51.382830 wideo-0.6.0/src/wideo/templates/wideo/videos/results.html
+-rw-r--r--   0        0        0        0 2024-05-28 12:34:51.382830 wideo-0.6.0/src/wideo/templates/wideo/videos/results_video.html
+-rw-r--r--   0        0        0        0 2024-05-28 12:34:51.382830 wideo-0.6.0/src/wideo/templatetags/__init__.py
+-rw-r--r--   0        0        0      231 2024-05-28 12:34:51.382830 wideo-0.6.0/src/wideo/templatetags/settings.py
+-rw-r--r--   0        0        0    14570 2024-05-28 12:34:51.382830 wideo-0.6.0/src/wideo/views.py
+-rw-r--r--   0        0        0      612 2024-05-28 12:34:51.382830 wideo-0.6.0/src/wideo/wagtail_hooks.py
+-rw-r--r--   0        0        0      126 2024-05-28 12:34:51.382830 wideo-0.6.0/src/wideo/widgets.py
+-rw-r--r--   0        0        0     1162 1970-01-01 00:00:00.000000 wideo-0.6.0/PKG-INFO
```

### Comparing `wideo-0.5.0/README.md` & `wideo-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `wideo-0.5.0/src/wideo/__init__.py` & `wideo-0.6.0/src/wideo/__init__.py`

 * *Files identical despite different names*

### Comparing `wideo-0.5.0/src/wideo/admin_urls.py` & `wideo-0.6.0/src/wideo/admin_urls.py`

 * *Files identical despite different names*

### Comparing `wideo-0.5.0/src/wideo/codecs.py` & `wideo-0.6.0/src/wideo/codecs.py`

 * *Files identical despite different names*

### Comparing `wideo-0.5.0/src/wideo/ffmpeg.py` & `wideo-0.6.0/src/wideo/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `wideo-0.5.0/src/wideo/management/commands/encode_videos.py` & `wideo-0.6.0/src/wideo/management/commands/encode_videos.py`

 * *Files identical despite different names*

### Comparing `wideo-0.5.0/src/wideo/migrations/0001_initial.py` & `wideo-0.6.0/src/wideo/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wideo-0.5.0/src/wideo/migrations/0002_lock.py` & `wideo-0.6.0/src/wideo/migrations/0002_lock.py`

 * *Files identical despite different names*

### Comparing `wideo-0.5.0/src/wideo/migrations/0003_uploadedvideochunk.py` & `wideo-0.6.0/src/wideo/migrations/0003_uploadedvideochunk.py`

 * *Files identical despite different names*

### Comparing `wideo-0.5.0/src/wideo/migrations/0004_alter_video_upload.py` & `wideo-0.6.0/src/wideo/migrations/0004_alter_video_upload.py`

 * *Files identical despite different names*

### Comparing `wideo-0.5.0/src/wideo/migrations/0005_alter_video_upload.py` & `wideo-0.6.0/src/wideo/migrations/0005_alter_video_upload.py`

 * *Files identical despite different names*

### Comparing `wideo-0.5.0/src/wideo/models.py` & `wideo-0.6.0/src/wideo/models.py`

 * *Files identical despite different names*

### Comparing `wideo-0.5.0/src/wideo/permissions.py` & `wideo-0.6.0/src/wideo/permissions.py`

 * *Files identical despite different names*

### Comparing `wideo-0.5.0/src/wideo/signals.py` & `wideo-0.6.0/src/wideo/signals.py`

 * *Files identical despite different names*

### Comparing `wideo-0.5.0/src/wideo/storage.py` & `wideo-0.6.0/src/wideo/storage.py`

 * *Files identical despite different names*

### Comparing `wideo-0.5.0/src/wideo/tasks.py` & `wideo-0.6.0/src/wideo/tasks.py`

 * *Files identical despite different names*

### Comparing `wideo-0.5.0/src/wideo/templates/wideo/forms/file.html` & `wideo-0.6.0/src/wideo/templates/wideo/forms/file.html`

 * *Files identical despite different names*

### Comparing `wideo-0.5.0/src/wideo/templates/wideo/preview/video_source.html` & `wideo-0.6.0/src/wideo/templates/wideo/preview/video_source.html`

 * *Files identical despite different names*

### Comparing `wideo-0.5.0/src/wideo/templates/wideo/videos/add.html` & `wideo-0.6.0/src/wideo/templates/wideo/videos/add.html`

 * *Files identical despite different names*

### Comparing `wideo-0.5.0/src/wideo/templates/wideo/videos/confirm_delete.html` & `wideo-0.6.0/src/wideo/templates/wideo/videos/confirm_delete.html`

 * *Files identical despite different names*

### Comparing `wideo-0.5.0/src/wideo/templates/wideo/videos/edit.html` & `wideo-0.6.0/src/wideo/templates/wideo/videos/edit.html`

 * *Files identical despite different names*

### Comparing `wideo-0.5.0/src/wideo/templates/wideo/videos/index.html` & `wideo-0.6.0/src/wideo/templates/wideo/videos/index.html`

 * *Files identical despite different names*

### Comparing `wideo-0.5.0/src/wideo/templates/wideo/videos/results.html` & `wideo-0.6.0/src/wideo/templates/wideo/videos/results.html`

 * *Files identical despite different names*

### Comparing `wideo-0.5.0/src/wideo/views.py` & `wideo-0.6.0/src/wideo/views.py`

 * *Files identical despite different names*

### Comparing `wideo-0.5.0/src/wideo/wagtail_hooks.py` & `wideo-0.6.0/src/wideo/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `wideo-0.5.0/PKG-INFO` & `wideo-0.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: wideo
-Version: 0.5.0
+Version: 0.6.0
 Summary: Add video goodness to your Wagtail website
 License: WTFPL
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: celery (>=5.2,<5.3)
+Requires-Dist: celery (==5.*)
 Requires-Dist: python-magic (>=0.4.27,<0.5.0)
-Requires-Dist: wagtail (>=4.1,<4.2)
+Requires-Dist: wagtail (==5.*)
 Description-Content-Type: text/markdown
 
 # Model W &mdash; Wideo
 
 This package enables easy video uploading and encoding in Wagtail.
 
 Basic usage:
```

