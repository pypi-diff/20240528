# Comparing `tmp/django_cool_urls-0.0.1.tar.gz` & `tmp/django_cool_urls-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_cool_urls-0.0.1.tar", max compression
+gzip compressed data, was "django_cool_urls-0.1.0.tar", max compression
```

## Comparing `django_cool_urls-0.0.1.tar` & `django_cool_urls-0.1.0.tar`

### file list

```diff
@@ -1,38 +1,44 @@
--rw-r--r--   0        0        0    35137 2024-05-20 17:39:21.436774 django_cool_urls-0.0.1/LICENSE
--rw-r--r--   0        0        0     1866 2024-05-20 20:17:13.328061 django_cool_urls-0.0.1/README.md
--rw-r--r--   0        0        0        0 2024-05-10 16:27:22.150287 django_cool_urls-0.0.1/cool_urls/__init__.py
--rw-r--r--   0        0        0     1301 2024-05-22 22:21:31.653847 django_cool_urls-0.0.1/cool_urls/admin.py
--rw-r--r--   0        0        0      390 2024-05-22 22:12:24.929492 django_cool_urls-0.0.1/cool_urls/apps.py
--rw-r--r--   0        0        0      205 2024-05-18 20:31:13.504062 django_cool_urls-0.0.1/cool_urls/coolers/__init__.py
--rw-r--r--   0        0        0     2509 2024-05-19 13:38:55.987287 django_cool_urls-0.0.1/cool_urls/coolers/base.py
--rw-r--r--   0        0        0       94 2024-05-10 16:27:22.210288 django_cool_urls-0.0.1/cool_urls/coolers/exceptions.py
--rw-r--r--   0        0        0     1846 2024-05-19 22:26:48.473493 django_cool_urls-0.0.1/cool_urls/coolers/files.py
--rw-r--r--   0        0        0     4048 2024-05-19 13:28:07.276568 django_cool_urls-0.0.1/cool_urls/coolers/pages.py
--rw-r--r--   0        0        0     8106 2024-05-21 22:27:06.135403 django_cool_urls-0.0.1/cool_urls/coolers/videos.py
--rw-r--r--   0        0        0      698 2024-05-14 21:47:23.096123 django_cool_urls-0.0.1/cool_urls/logging.py
--rw-r--r--   0        0        0     1033 2024-05-14 22:14:29.447255 django_cool_urls-0.0.1/cool_urls/management/commands/check_cool_urls.py
--rw-r--r--   0        0        0     1091 2024-05-19 20:51:50.141237 django_cool_urls-0.0.1/cool_urls/management/commands/cool_url.py
--rw-r--r--   0        0        0      398 2024-05-20 17:37:34.605478 django_cool_urls-0.0.1/cool_urls/management/commands/cool_urls.py
--rw-r--r--   0        0        0     3898 2024-05-18 21:19:44.946565 django_cool_urls-0.0.1/cool_urls/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-05-10 16:27:22.153621 django_cool_urls-0.0.1/cool_urls/migrations/__init__.py
--rw-r--r--   0        0        0     5610 2024-05-21 20:34:20.308550 django_cool_urls-0.0.1/cool_urls/models.py
--rw-r--r--   0        0        0      434 2024-05-13 20:35:59.913282 django_cool_urls-0.0.1/cool_urls/receivers.py
--rw-r--r--   0        0        0      131 2024-05-14 19:53:53.742788 django_cool_urls-0.0.1/cool_urls/signals.py
--rw-r--r--   0        0        0        0 2024-05-10 16:27:22.193621 django_cool_urls-0.0.1/cool_urls/templatetags/__init__.py
--rw-r--r--   0        0        0      712 2024-05-14 20:33:12.080088 django_cool_urls-0.0.1/cool_urls/templatetags/cool_urls.py
--rw-r--r--   0        0        0        0 2024-05-14 19:53:53.742788 django_cool_urls-0.0.1/cool_urls/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-05-14 19:53:53.742788 django_cool_urls-0.0.1/cool_urls/tests/coolers/__init__.py
--rw-r--r--   0        0        0     3134 2024-05-19 13:34:07.072132 django_cool_urls-0.0.1/cool_urls/tests/coolers/test_base.py
--rw-r--r--   0        0        0     2353 2024-05-18 21:19:44.916566 django_cool_urls-0.0.1/cool_urls/tests/coolers/test_files.py
--rw-r--r--   0        0        0     6140 2024-05-19 13:33:59.482028 django_cool_urls-0.0.1/cool_urls/tests/coolers/test_pages.py
--rw-r--r--   0        0        0     8067 2024-05-21 21:18:50.977491 django_cool_urls-0.0.1/cool_urls/tests/coolers/test_videos.py
--rw-r--r--   0        0        0        0 2024-05-14 22:14:51.797637 django_cool_urls-0.0.1/cool_urls/tests/management/__init__.py
--rw-r--r--   0        0        0        0 2024-05-14 22:14:58.677751 django_cool_urls-0.0.1/cool_urls/tests/management/commands/__init__.py
--rw-r--r--   0        0        0     2639 2024-05-18 21:19:44.909899 django_cool_urls-0.0.1/cool_urls/tests/management/commands/test_check_cool_urls.py
--rw-r--r--   0        0        0     1547 2024-05-18 21:19:44.866565 django_cool_urls-0.0.1/cool_urls/tests/management/commands/test_cool_url.py
--rw-r--r--   0        0        0      770 2024-05-22 22:24:36.311281 django_cool_urls-0.0.1/cool_urls/tests/test_admin.py
--rw-r--r--   0        0        0     4822 2024-05-18 21:19:44.893232 django_cool_urls-0.0.1/cool_urls/tests/test_models.py
--rw-r--r--   0        0        0      364 2024-05-18 21:19:44.959899 django_cool_urls-0.0.1/cool_urls/tests/test_receivers.py
--rw-r--r--   0        0        0     1972 2024-05-18 21:19:44.986566 django_cool_urls-0.0.1/cool_urls/tests/test_templatetags.py
--rw-r--r--   0        0        0     1576 2024-05-19 22:34:51.825658 django_cool_urls-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2567 1970-01-01 00:00:00.000000 django_cool_urls-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35137 2024-05-20 17:39:21.436774 django_cool_urls-0.1.0/LICENSE
+-rw-r--r--   0        0        0     2049 2024-05-24 22:30:43.308370 django_cool_urls-0.1.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-10 16:27:22.150287 django_cool_urls-0.1.0/cool_urls/__init__.py
+-rw-r--r--   0        0        0     1301 2024-05-22 22:21:31.653847 django_cool_urls-0.1.0/cool_urls/admin.py
+-rw-r--r--   0        0        0      390 2024-05-22 22:12:24.929492 django_cool_urls-0.1.0/cool_urls/apps.py
+-rw-r--r--   0        0        0      205 2024-05-18 20:31:13.504062 django_cool_urls-0.1.0/cool_urls/coolers/__init__.py
+-rw-r--r--   0        0        0     2509 2024-05-19 13:38:55.987287 django_cool_urls-0.1.0/cool_urls/coolers/base.py
+-rw-r--r--   0        0        0       94 2024-05-10 16:27:22.210288 django_cool_urls-0.1.0/cool_urls/coolers/exceptions.py
+-rw-r--r--   0        0        0     1846 2024-05-19 22:26:48.473493 django_cool_urls-0.1.0/cool_urls/coolers/files.py
+-rw-r--r--   0        0        0     4162 2024-05-27 22:50:53.337388 django_cool_urls-0.1.0/cool_urls/coolers/pages.py
+-rw-r--r--   0        0        0     6633 2024-05-27 22:50:53.337388 django_cool_urls-0.1.0/cool_urls/coolers/videos.py
+-rw-r--r--   0        0        0      698 2024-05-14 21:47:23.096123 django_cool_urls-0.1.0/cool_urls/logging.py
+-rw-r--r--   0        0        0     1033 2024-05-14 22:14:29.447255 django_cool_urls-0.1.0/cool_urls/management/commands/check_cool_urls.py
+-rw-r--r--   0        0        0     1091 2024-05-19 20:51:50.141237 django_cool_urls-0.1.0/cool_urls/management/commands/cool_url.py
+-rw-r--r--   0        0        0      398 2024-05-20 17:37:34.605478 django_cool_urls-0.1.0/cool_urls/management/commands/cool_urls.py
+-rw-r--r--   0        0        0      699 2024-05-27 22:50:53.337388 django_cool_urls-0.1.0/cool_urls/management/commands/scratch.py
+-rw-r--r--   0        0        0     5274 2024-05-24 22:20:53.158262 django_cool_urls-0.1.0/cool_urls/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-05-10 16:27:22.153621 django_cool_urls-0.1.0/cool_urls/migrations/__init__.py
+-rw-r--r--   0        0        0     5610 2024-05-24 22:15:48.614829 django_cool_urls-0.1.0/cool_urls/models.py
+-rw-r--r--   0        0        0      434 2024-05-13 20:35:59.913282 django_cool_urls-0.1.0/cool_urls/receivers.py
+-rw-r--r--   0        0        0      131 2024-05-14 19:53:53.742788 django_cool_urls-0.1.0/cool_urls/signals.py
+-rw-r--r--   0        0        0      387 2024-05-27 22:50:53.337388 django_cool_urls-0.1.0/cool_urls/templates/cool_urls/videos/local.html
+-rw-r--r--   0        0        0       64 2024-05-27 22:50:53.337388 django_cool_urls-0.1.0/cool_urls/templates/cool_urls/videos/remote/default.html
+-rw-r--r--   0        0        0      256 2024-05-27 22:50:53.337388 django_cool_urls-0.1.0/cool_urls/templates/cool_urls/videos/remote/vimeo.html
+-rw-r--r--   0        0        0      330 2024-05-27 22:50:53.337388 django_cool_urls-0.1.0/cool_urls/templates/cool_urls/videos/remote/youtube.html
+-rw-r--r--   0        0        0        0 2024-05-10 16:27:22.193621 django_cool_urls-0.1.0/cool_urls/templatetags/__init__.py
+-rw-r--r--   0        0        0     1705 2024-05-24 23:19:59.585191 django_cool_urls-0.1.0/cool_urls/templatetags/cool_urls.py
+-rw-r--r--   0        0        0        0 2024-05-14 19:53:53.742788 django_cool_urls-0.1.0/cool_urls/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 19:53:53.742788 django_cool_urls-0.1.0/cool_urls/tests/coolers/__init__.py
+-rw-r--r--   0        0        0     3134 2024-05-19 13:34:07.072132 django_cool_urls-0.1.0/cool_urls/tests/coolers/test_base.py
+-rw-r--r--   0        0        0     2353 2024-05-18 21:19:44.916566 django_cool_urls-0.1.0/cool_urls/tests/coolers/test_files.py
+-rw-r--r--   0        0        0     6140 2024-05-19 13:33:59.482028 django_cool_urls-0.1.0/cool_urls/tests/coolers/test_pages.py
+-rw-r--r--   0        0        0     8145 2024-05-27 22:50:53.337388 django_cool_urls-0.1.0/cool_urls/tests/coolers/test_videos.py
+-rw-r--r--   0        0        0        0 2024-05-14 22:14:51.797637 django_cool_urls-0.1.0/cool_urls/tests/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 22:14:58.677751 django_cool_urls-0.1.0/cool_urls/tests/management/commands/__init__.py
+-rw-r--r--   0        0        0     2639 2024-05-18 21:19:44.909899 django_cool_urls-0.1.0/cool_urls/tests/management/commands/test_check_cool_urls.py
+-rw-r--r--   0        0        0     1547 2024-05-18 21:19:44.866565 django_cool_urls-0.1.0/cool_urls/tests/management/commands/test_cool_url.py
+-rw-r--r--   0        0        0      770 2024-05-22 22:24:36.311281 django_cool_urls-0.1.0/cool_urls/tests/test_admin.py
+-rw-r--r--   0        0        0     5817 2024-05-28 01:35:48.025093 django_cool_urls-0.1.0/cool_urls/tests/test_functional.py
+-rw-r--r--   0        0        0     4822 2024-05-18 21:19:44.893232 django_cool_urls-0.1.0/cool_urls/tests/test_models.py
+-rw-r--r--   0        0        0      364 2024-05-18 21:19:44.959899 django_cool_urls-0.1.0/cool_urls/tests/test_receivers.py
+-rw-r--r--   0        0        0     3110 2024-05-24 23:13:59.126859 django_cool_urls-0.1.0/cool_urls/tests/test_templatetags.py
+-rw-r--r--   0        0        0     1576 2024-05-28 02:28:26.578013 django_cool_urls-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2750 1970-01-01 00:00:00.000000 django_cool_urls-0.1.0/PKG-INFO
```

### Comparing `django_cool_urls-0.0.1/LICENSE` & `django_cool_urls-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_cool_urls-0.0.1/cool_urls/admin.py` & `django_cool_urls-0.1.0/cool_urls/admin.py`

 * *Files identical despite different names*

### Comparing `django_cool_urls-0.0.1/cool_urls/coolers/base.py` & `django_cool_urls-0.1.0/cool_urls/coolers/base.py`

 * *Files identical despite different names*

### Comparing `django_cool_urls-0.0.1/cool_urls/coolers/files.py` & `django_cool_urls-0.1.0/cool_urls/coolers/files.py`

 * *Files identical despite different names*

### Comparing `django_cool_urls-0.0.1/cool_urls/coolers/pages.py` & `django_cool_urls-0.1.0/cool_urls/coolers/pages.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,19 @@
     def can_handle(cls, cool_url: CoolUrl) -> bool:
         return True
 
     def cool(self) -> None:
         self.prepare_fetch()
 
         if self._target_path.exists():
-            self.logger.warning("Page has already been cooled.  Exiting.")
+            self.logger.warning(
+                "Page has already been cooled at %s.  Exiting.",
+                self._target_path,
+            )
+            self.cool_url.mark_as_ready()
             return
 
         if not self._monolith:
             raise CoolingError(
                 "Cannot find monolith.  Please install it and make sure it's "
                 "in your ${PATH} to continue."
             )
```

### Comparing `django_cool_urls-0.0.1/cool_urls/logging.py` & `django_cool_urls-0.1.0/cool_urls/logging.py`

 * *Files identical despite different names*

### Comparing `django_cool_urls-0.0.1/cool_urls/management/commands/check_cool_urls.py` & `django_cool_urls-0.1.0/cool_urls/management/commands/check_cool_urls.py`

 * *Files identical despite different names*

### Comparing `django_cool_urls-0.0.1/cool_urls/management/commands/cool_url.py` & `django_cool_urls-0.1.0/cool_urls/management/commands/cool_url.py`

 * *Files identical despite different names*

### Comparing `django_cool_urls-0.0.1/cool_urls/models.py` & `django_cool_urls-0.1.0/cool_urls/models.py`

 * *Files identical despite different names*

### Comparing `django_cool_urls-0.0.1/cool_urls/tests/coolers/test_base.py` & `django_cool_urls-0.1.0/cool_urls/tests/coolers/test_base.py`

 * *Files identical despite different names*

### Comparing `django_cool_urls-0.0.1/cool_urls/tests/coolers/test_files.py` & `django_cool_urls-0.1.0/cool_urls/tests/coolers/test_files.py`

 * *Files identical despite different names*

### Comparing `django_cool_urls-0.0.1/cool_urls/tests/coolers/test_pages.py` & `django_cool_urls-0.1.0/cool_urls/tests/coolers/test_pages.py`

 * *Files identical despite different names*

### Comparing `django_cool_urls-0.0.1/cool_urls/tests/coolers/test_videos.py` & `django_cool_urls-0.1.0/cool_urls/tests/coolers/test_videos.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from ...models import CoolUrl
 
 
 class VideoCoolerTestCase(TestCase):
     def test_remote_markup(self):
         cu = CoolUrl.objects.create(url="https://youtube.com/watch?v=test")
         self.assertEqual(
-            VideoCooler(cu).remote_markup,
+            VideoCooler(cu).remote_markup.strip(),
             '<p>Waiting on download of <a href="https://youtube.com/watch?v=test">https://youtube.com/watch?v=test</a></p>',  # NOQA: E501
         )
 
     def test_local_markup(self):
         url = "https://youtube.com/watch?v=test"
         hsh = "d3569d4e77d39b5c28e6111206653718"
         cu = CoolUrl.objects.create(url=url)
@@ -153,14 +153,15 @@
                             "key": "FFmpegConcat",
                             "only_multi_video": True,
                             "when": "playlist",
                         }
                     ],
                     "retries": 10,
                     "writethumbnail": True,
+                    "quiet": True,
                     "outtmpl": str(d / hsh / "video.%(ext)s"),
                 },
             )
             self.assertEqual(
                 m.call_args_list[1][0][0],
                 {
                     "color": {"stderr": "no_color", "stdout": "no_color"},
@@ -172,14 +173,15 @@
                             "key": "FFmpegConcat",
                             "only_multi_video": True,
                             "when": "playlist",
                         }
                     ],
                     "retries": 10,
                     "writethumbnail": True,
+                    "quiet": True,
                     "outtmpl": str(d / hsh / "video.%(ext)s"),
                 },
             )
 
             cu.refresh_from_db()
             self.assertTrue(cu.is_ready)
             self.assertFalse(cu.is_processing)
```

### Comparing `django_cool_urls-0.0.1/cool_urls/tests/management/commands/test_check_cool_urls.py` & `django_cool_urls-0.1.0/cool_urls/tests/management/commands/test_check_cool_urls.py`

 * *Files identical despite different names*

### Comparing `django_cool_urls-0.0.1/cool_urls/tests/management/commands/test_cool_url.py` & `django_cool_urls-0.1.0/cool_urls/tests/management/commands/test_cool_url.py`

 * *Files identical despite different names*

### Comparing `django_cool_urls-0.0.1/cool_urls/tests/test_admin.py` & `django_cool_urls-0.1.0/cool_urls/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `django_cool_urls-0.0.1/cool_urls/tests/test_models.py` & `django_cool_urls-0.1.0/cool_urls/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django_cool_urls-0.0.1/cool_urls/tests/test_templatetags.py` & `django_cool_urls-0.1.0/cool_urls/tests/test_templatetags.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,68 @@
-from unittest.mock import patch
 
-from django.test import TestCase
+from django.test import TestCase, override_settings
 
 from ..models import CoolUrl
 from ..templatetags.cool_urls import cool_embed, cool_url
 
 
+def fake_policy(url: str, is_embedded: bool) -> bool:
+    return "test" in url
+
+
 class CoolEmbedTestCase(TestCase):
     def test_without_policy(self):
         url = "https://youtube.com/watch?v=test"
         cool_embed(url)
         self.assertEqual(CoolUrl.objects.count(), 1)
         cu = CoolUrl.objects.get(url=url)
         self.assertEqual(cu.url, url)
         self.assertFalse(cu.show_local)
         self.assertTrue(cu.is_embedded)
 
-    @patch("cool_urls.templatetags.cool_urls.POLICY", "LOCAL")
+    @override_settings(COOL_URLS_POLICY="LOCAL")
+    def test_with_local_policy(self):
+        url = "https://youtube.com/watch?v=test"
+        cool_embed(url)
+        self.assertEqual(CoolUrl.objects.count(), 1)
+        cu = CoolUrl.objects.get(url=url)
+        self.assertEqual(cu.url, url)
+        self.assertTrue(cu.show_local)
+        self.assertTrue(cu.is_embedded)
+
+    @override_settings(COOL_URLS_POLICY="REMOTE")
     def test_with_policy(self):
         url = "https://youtube.com/watch?v=test"
         cool_embed(url)
         self.assertEqual(CoolUrl.objects.count(), 1)
         cu = CoolUrl.objects.get(url=url)
         self.assertEqual(cu.url, url)
+        self.assertFalse(cu.show_local)
+        self.assertTrue(cu.is_embedded)
+
+    @override_settings(
+        COOL_URLS_POLICY="cool_urls.tests.test_templatetags.fake_policy"
+    )
+    def test_with_callable_policy(self):
+        url1 = "https://youtube.com/watch?v=test"
+        cool_embed(url1)
+        self.assertEqual(CoolUrl.objects.count(), 1)
+        cu = CoolUrl.objects.get(url=url1)
+        self.assertEqual(cu.url, url1)
         self.assertTrue(cu.show_local)
         self.assertTrue(cu.is_embedded)
 
+        url2 = "https://youtube.com/watch?v=no"
+        cool_embed(url2)
+        self.assertEqual(CoolUrl.objects.count(), 2)
+        cu = CoolUrl.objects.get(url=url2)
+        self.assertEqual(cu.url, url2)
+        self.assertFalse(cu.show_local)
+        self.assertTrue(cu.is_embedded)
+
     def test_multiple_invocations(self):
         url = "https://youtube.com/watch?v=test"
         cool_embed(url)
         cool_embed(url)
         self.assertEqual(CoolUrl.objects.count(), 1)
 
 
@@ -39,15 +72,15 @@
         cool_url(url)
         self.assertEqual(CoolUrl.objects.count(), 1)
         cu = CoolUrl.objects.get(url=url)
         self.assertEqual(cu.url, url)
         self.assertFalse(cu.show_local)
         self.assertFalse(cu.is_embedded)
 
-    @patch("cool_urls.templatetags.cool_urls.POLICY", "LOCAL")
+    @override_settings(COOL_URLS_POLICY="LOCAL")
     def test_with_policy(self):
         url = "https://example.com/"
         cool_url(url)
         self.assertEqual(CoolUrl.objects.count(), 1)
         cu = CoolUrl.objects.get(url=url)
         self.assertEqual(cu.url, url)
         self.assertTrue(cu.show_local)
```

### Comparing `django_cool_urls-0.0.1/pyproject.toml` & `django_cool_urls-0.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-cool-urls"
-version = "0.0.1"
+version = "0.1.0"
 description = "Freeze outgoing links in time so that your site never 404s on external pages"
 authors = ["Daniel Quinn <code@danielquinn.org>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 packages = [
     { include = "cool_urls" }
 ]
```

### Comparing `django_cool_urls-0.0.1/PKG-INFO` & `django_cool_urls-0.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-cool-urls
-Version: 0.0.1
+Version: 0.1.0
 Summary: Freeze outgoing links in time so that your site never 404s on external pages
 License: AGPL-3.0-or-later
 Author: Daniel Quinn
 Author-email: code@danielquinn.org
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: embed
 Requires-Dist: Django (>=3.2)
 Requires-Dist: httpx (>=0.27.0,<0.28.0)
 Requires-Dist: yt-dlp (>=2024.4.9,<2025.0.0) ; extra == "embed"
 Description-Content-Type: text/markdown
 
-![logo.png](docs/logo.png)
+![logo.png](https://gitlab.com/danielquinn/django-cool-urls/-/raw/master/docs/logo.png)
 
 # Django Cool URLs
 
 Tim Berners-Lee is credited with saying that "cool URLs don't change", but
 sadly that's just not the case.  Cool URLs are changing all the time because
 the people who run those sites are moving stuff around or just deleting
 whole pages and domains.
@@ -46,18 +46,19 @@
 ```html
 <a href="{% cool_url 'https://something-awesome.ca/' %}">Nifty!</a>
 ```
 
 If that page ever 404s, your site will switch to showing the locally cached
 version.  Think of it like your own private [archive.org](https://archive.org/).
 
-Currently, this project supports caching *most* pages (see the [Caveats](caveats.md) page)
+Currently, this project supports caching *most* pages (see the [Caveats](https://danielquinn.gitlab.io/django-cool-urls/caveats/) page)
 as well as embedded video from YouTube, Vimeo, and Instagram.
 
 
 * [Official documentation](https://danielquinn.gitlab.io/django-cool-urls/)
     * [Installation](https://danielquinn.gitlab.io/django-cool-urls/installation/)
     * [Configuration](https://danielquinn.gitlab.io/django-cool-urls/configuration/)
     * [How to use it](https://danielquinn.gitlab.io/django-cool-urls/how-to-use-it/)
     * [Caveats & troubleshooting](https://danielquinn.gitlab.io/django-cool-urls/caveats/)
     * [Development](https://danielquinn.gitlab.io/django-cool-urls/development/)
+    * [Changelog](https://danielquinn.gitlab.io/django-cool-urls/changelog/)
```

#### html2text {}

```diff
@@ -1,32 +1,34 @@
-Metadata-Version: 2.1 Name: django-cool-urls Version: 0.0.1 Summary: Freeze
+Metadata-Version: 2.1 Name: django-cool-urls Version: 0.1.0 Summary: Freeze
 outgoing links in time so that your site never 404s on external pages License:
 AGPL-3.0-or-later Author: Daniel Quinn Author-email: code@danielquinn.org
 Requires-Python: >=3.11,<4.0 Classifier: License :: OSI Approved :: GNU Affero
 General Public License v3 or later (AGPLv3+) Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Provides-Extra: embed Requires-Dist:
 Django (>=3.2) Requires-Dist: httpx (>=0.27.0,<0.28.0) Requires-Dist: yt-dlp
 (>=2024.4.9,<2025.0.0) ; extra == "embed" Description-Content-Type: text/
-markdown ![logo.png](docs/logo.png) # Django Cool URLs Tim Berners-Lee is
-credited with saying that "cool URLs don't change", but sadly that's just not
-the case. Cool URLs are changing all the time because the people who run those
-sites are moving stuff around or just deleting whole pages and domains. If you
-have a long-running site full of links like a blog however, this means that
-over time your site can be pointing to a lot of dead links, which is bad for
-your SEO. It's also annoying when you're looking over a post from 10 years ago
-that says something like "[this](.) is some really nice work" and that link
-404s. With `django-cool-urls`, you can link to whatever you like and the state
-of that page is captured from the moment you linked to it. If the page ever
-disappears from the web, you can automatically switch over to the local copy.
-All you need to do is switch from doing this: ```html _N_i_f_t_y_! ``` to this:
-```html _N_i_f_t_y_! ``` If that page ever 404s, your site will switch to showing the
-locally cached version. Think of it like your own private [archive.org](https:/
-/archive.org/). Currently, this project supports caching *most* pages (see the
-[Caveats](caveats.md) page) as well as embedded video from YouTube, Vimeo, and
-Instagram. * [Official documentation](https://danielquinn.gitlab.io/django-
-cool-urls/) * [Installation](https://danielquinn.gitlab.io/django-cool-urls/
-installation/) * [Configuration](https://danielquinn.gitlab.io/django-cool-
-urls/configuration/) * [How to use it](https://danielquinn.gitlab.io/django-
-cool-urls/how-to-use-it/) * [Caveats & troubleshooting](https://
-danielquinn.gitlab.io/django-cool-urls/caveats/) * [Development](https://
-danielquinn.gitlab.io/django-cool-urls/development/)
+markdown ![logo.png](https://gitlab.com/danielquinn/django-cool-urls/-/raw/
+master/docs/logo.png) # Django Cool URLs Tim Berners-Lee is credited with
+saying that "cool URLs don't change", but sadly that's just not the case. Cool
+URLs are changing all the time because the people who run those sites are
+moving stuff around or just deleting whole pages and domains. If you have a
+long-running site full of links like a blog however, this means that over time
+your site can be pointing to a lot of dead links, which is bad for your SEO.
+It's also annoying when you're looking over a post from 10 years ago that says
+something like "[this](.) is some really nice work" and that link 404s. With
+`django-cool-urls`, you can link to whatever you like and the state of that
+page is captured from the moment you linked to it. If the page ever disappears
+from the web, you can automatically switch over to the local copy. All you need
+to do is switch from doing this: ```html _N_i_f_t_y_! ``` to this: ```html _N_i_f_t_y_! ```
+If that page ever 404s, your site will switch to showing the locally cached
+version. Think of it like your own private [archive.org](https://archive.org/).
+Currently, this project supports caching *most* pages (see the [Caveats](https:
+//danielquinn.gitlab.io/django-cool-urls/caveats/) page) as well as embedded
+video from YouTube, Vimeo, and Instagram. * [Official documentation](https://
+danielquinn.gitlab.io/django-cool-urls/) * [Installation](https://
+danielquinn.gitlab.io/django-cool-urls/installation/) * [Configuration](https:/
+/danielquinn.gitlab.io/django-cool-urls/configuration/) * [How to use it]
+(https://danielquinn.gitlab.io/django-cool-urls/how-to-use-it/) * [Caveats &
+troubleshooting](https://danielquinn.gitlab.io/django-cool-urls/caveats/) *
+[Development](https://danielquinn.gitlab.io/django-cool-urls/development/) *
+[Changelog](https://danielquinn.gitlab.io/django-cool-urls/changelog/)
```

