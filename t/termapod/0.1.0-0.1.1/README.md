# Comparing `tmp/termapod-0.1.0.tar.gz` & `tmp/termapod-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "termapod-0.1.0.tar", last modified: Sat Apr 27 20:52:53 2024, max compression
+gzip compressed data, was "termapod-0.1.1.tar", last modified: Tue May 28 17:51:37 2024, max compression
```

## Comparing `termapod-0.1.0.tar` & `termapod-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-04-27 20:52:53.748682 termapod-0.1.0/
--rw-rw-r--   0 schrock   (1000) schrock   (1000)     3090 2024-04-26 23:09:55.000000 termapod-0.1.0/.gitignore
--rw-r--r--   0 schrock   (1000) schrock   (1000)       28 2024-04-23 19:00:47.000000 termapod-0.1.0/.nvimrc
--rw-rw-r--   0 schrock   (1000) schrock   (1000)     1071 2024-04-23 00:39:20.000000 termapod-0.1.0/LICENSE
--rw-r--r--   0 schrock   (1000) schrock   (1000)     1909 2024-04-27 20:52:53.748682 termapod-0.1.0/PKG-INFO
--rw-rw-r--   0 schrock   (1000) schrock   (1000)     1092 2024-04-27 20:10:27.000000 termapod-0.1.0/README.md
--rw-r--r--   0 schrock   (1000) schrock   (1000)     1110 2024-04-27 20:01:20.000000 termapod-0.1.0/pyproject.toml
--rw-r--r--   0 schrock   (1000) schrock   (1000)       89 2024-04-23 19:54:18.000000 termapod-0.1.0/pyrightconfig.json
--rw-r--r--   0 schrock   (1000) schrock   (1000)      101 2024-04-23 18:52:28.000000 termapod-0.1.0/requirements.txt
--rw-rw-r--   0 schrock   (1000) schrock   (1000)       38 2024-04-27 20:52:53.748682 termapod-0.1.0/setup.cfg
--rw-r--r--   0 schrock   (1000) schrock   (1000)       38 2024-04-24 21:50:09.000000 termapod-0.1.0/setup.py
-drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-04-27 20:52:53.744682 termapod-0.1.0/src/
-drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-04-27 20:52:53.748682 termapod-0.1.0/src/termapod/
--rw-r--r--   0 schrock   (1000) schrock   (1000)      217 2024-04-26 23:08:49.000000 termapod-0.1.0/src/termapod/__init__.py
--rw-rw-r--   0 schrock   (1000) schrock   (1000)      411 2024-04-27 20:52:53.000000 termapod-0.1.0/src/termapod/_version.py
--rw-rw-r--   0 schrock   (1000) schrock   (1000)     3366 2024-04-27 20:17:15.000000 termapod-0.1.0/src/termapod/termapod.py
-drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-04-27 20:52:53.748682 termapod-0.1.0/src/termapod.egg-info/
--rw-r--r--   0 schrock   (1000) schrock   (1000)     1909 2024-04-27 20:52:53.000000 termapod-0.1.0/src/termapod.egg-info/PKG-INFO
--rw-rw-r--   0 schrock   (1000) schrock   (1000)      389 2024-04-27 20:52:53.000000 termapod-0.1.0/src/termapod.egg-info/SOURCES.txt
--rw-rw-r--   0 schrock   (1000) schrock   (1000)        1 2024-04-27 20:52:53.000000 termapod-0.1.0/src/termapod.egg-info/dependency_links.txt
--rw-rw-r--   0 schrock   (1000) schrock   (1000)       52 2024-04-27 20:52:53.000000 termapod-0.1.0/src/termapod.egg-info/entry_points.txt
--rw-rw-r--   0 schrock   (1000) schrock   (1000)       32 2024-04-27 20:52:53.000000 termapod-0.1.0/src/termapod.egg-info/requires.txt
--rw-rw-r--   0 schrock   (1000) schrock   (1000)        9 2024-04-27 20:52:53.000000 termapod-0.1.0/src/termapod.egg-info/top_level.txt
+drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-05-28 17:51:37.945762 termapod-0.1.1/
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)     3090 2024-04-26 23:09:55.000000 termapod-0.1.1/.gitignore
+-rw-r--r--   0 schrock   (1000) schrock   (1000)       28 2024-04-23 19:00:47.000000 termapod-0.1.1/.nvimrc
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)     1071 2024-04-23 00:39:20.000000 termapod-0.1.1/LICENSE
+-rw-r--r--   0 schrock   (1000) schrock   (1000)     1909 2024-05-28 17:51:37.945762 termapod-0.1.1/PKG-INFO
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)     1092 2024-04-27 20:10:27.000000 termapod-0.1.1/README.md
+-rw-r--r--   0 schrock   (1000) schrock   (1000)     1110 2024-04-27 20:01:20.000000 termapod-0.1.1/pyproject.toml
+-rw-r--r--   0 schrock   (1000) schrock   (1000)       89 2024-04-23 19:54:18.000000 termapod-0.1.1/pyrightconfig.json
+-rw-r--r--   0 schrock   (1000) schrock   (1000)      101 2024-04-23 18:52:28.000000 termapod-0.1.1/requirements.txt
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)       38 2024-05-28 17:51:37.945762 termapod-0.1.1/setup.cfg
+-rw-r--r--   0 schrock   (1000) schrock   (1000)       38 2024-04-24 21:50:09.000000 termapod-0.1.1/setup.py
+drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-05-28 17:51:37.941762 termapod-0.1.1/src/
+drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-05-28 17:51:37.945762 termapod-0.1.1/src/termapod/
+-rw-r--r--   0 schrock   (1000) schrock   (1000)      217 2024-04-26 23:08:49.000000 termapod-0.1.1/src/termapod/__init__.py
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)      411 2024-05-28 17:51:37.000000 termapod-0.1.1/src/termapod/_version.py
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)     3678 2024-05-28 17:47:36.000000 termapod-0.1.1/src/termapod/termapod.py
+drwxrwxr-x   0 schrock   (1000) schrock   (1000)        0 2024-05-28 17:51:37.945762 termapod-0.1.1/src/termapod.egg-info/
+-rw-r--r--   0 schrock   (1000) schrock   (1000)     1909 2024-05-28 17:51:37.000000 termapod-0.1.1/src/termapod.egg-info/PKG-INFO
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)      389 2024-05-28 17:51:37.000000 termapod-0.1.1/src/termapod.egg-info/SOURCES.txt
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)        1 2024-05-28 17:51:37.000000 termapod-0.1.1/src/termapod.egg-info/dependency_links.txt
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)       52 2024-05-28 17:51:37.000000 termapod-0.1.1/src/termapod.egg-info/entry_points.txt
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)       32 2024-05-28 17:51:37.000000 termapod-0.1.1/src/termapod.egg-info/requires.txt
+-rw-rw-r--   0 schrock   (1000) schrock   (1000)        9 2024-05-28 17:51:37.000000 termapod-0.1.1/src/termapod.egg-info/top_level.txt
```

### Comparing `termapod-0.1.0/.gitignore` & `termapod-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `termapod-0.1.0/LICENSE` & `termapod-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `termapod-0.1.0/PKG-INFO` & `termapod-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: termapod
-Version: 0.1.0
+Version: 0.1.1
 Summary: An ASCII block / ANSI color renderer for NASA's Astonomy Pic of the Day. For like no reason.
 Author-email: Trevor Schrock <spacemeat@gmail.com>
 Maintainer-email: Trevor Schrock <spacemeat@gmail.com>
 License: MIT License
 Project-URL: Repository, https://github.com/spacemeat/termapod
 Keywords: astronomy,NASA,ASCII,ANSI
 Classifier: Development Status :: 4 - Beta
```

### Comparing `termapod-0.1.0/README.md` & `termapod-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `termapod-0.1.0/pyproject.toml` & `termapod-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `termapod-0.1.0/src/termapod/termapod.py` & `termapod-0.1.1/src/termapod/termapod.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,27 +9,30 @@
 import sys
 
 from PIL import Image
 import requests
 
 from . import __version__
 
+class ApodScrapingError(Exception):
+    pass
+
 cache_dir = Path.home() / '.config/termapod'
 
 def get_image_cache_path() -> Path:
     ''' Gets the cached image's local path.'''
     today = date.today()
     image_cache_path = cache_dir / ('image-' + today.strftime('%Y-%m-%d') + '.jpg')
     return image_cache_path
 
 def is_cached() -> bool:
     ''' Returns if today's image has been cached.'''
     return get_image_cache_path().exists()
 
-def get_image_and_caption() -> tuple[Image, str]:
+def get_image_and_caption() -> tuple[Image.Image | None, str]:
     ''' Returns the APOD image either from cache or the web.'''
     if is_cached() and '--no-cache' not in sys.argv:
         im = Image.open(get_image_cache_path())
         with open(cache_dir / 'caption.txt', 'rt', encoding='utf-8') as f:
             caption = f.read()
         return (im, caption)
 
@@ -39,18 +42,22 @@
     text = resp.text
     m = re.search(r'<IMG SRC=(.*)>', text)
     pat = '<IMG SRC=\"(.*?)\".*>'
     m = re.search(pat, text, re.S)
     img_url = ''
     if m is not None:
         img_url = base_url + m[1]
+    else:
+        raise ApodScrapingError("URL scraping failed to turn up an image source. Maybe it's a "
+            "video today?")
 
     pat = r'<b>(.*?)</b>'
     m = re.search(pat, text, re.S)
     caption = ''
+    print (f'URL: {m}')
     if m is not None:
         caption = m[1].strip()
 
     im = Image.open(requests.get(img_url, stream=True).raw)
 
     if '--no-save-cache' not in sys.argv:
         # delete previous APODs
@@ -62,22 +69,22 @@
         with open(cache_dir / 'caption.txt', 'wt', encoding='utf-8') as f:
             f.write(caption)
 
         im.save(get_image_cache_path(), 'JPEG')
 
     return (im, caption)
 
-def resize_image(txy: terminal_size, im: Image) -> None:
+def resize_image(txy: terminal_size, im: Image.Image) -> None:
     ''' Resize the image (in place) to the available terminal elements, keeping
     the aspect ratio.'''
     cols, rows = txy
     size = cols, rows * 2 - 3
     im.thumbnail(size, Image.Resampling.LANCZOS)
 
-def convert_to_ansi(txy: terminal_size, im: Image, caption: str) -> str:
+def convert_to_ansi(txy: terminal_size, im: Image.Image, caption: str) -> str:
     ''' Returns an ANSI-colored ASCII block made from the image and caption.'''
     s = ''
     def fg(rgb):
         return f'\033[38;2;{rgb[0]};{rgb[1]};{rgb[2]}m'
     def bg(rgb):
         return f'\033[48;2;{rgb[0]};{rgb[1]};{rgb[2]}m'
 
@@ -98,15 +105,19 @@
 def main():
     ''' Meign.'''
     if len(sys.argv) > 1 and sys.argv[1] in ['-v', '--version']:
         print (f'termapod version {__version__}')
         return
 
     txy = shutil.get_terminal_size()
-    im, caption = get_image_and_caption()
-    if im:
-        resize_image(txy, im)
-        s = convert_to_ansi(txy, im, caption)
-        print (s)
+    try:
+        im, caption = get_image_and_caption()
+        if im:
+            resize_image(txy, im)
+            s = convert_to_ansi(txy, im, caption)
+            print (s)
+
+    except ApodScrapingError as e:
+        print (e)
 
 if __name__ == "__main__":
     main()
```

### Comparing `termapod-0.1.0/src/termapod.egg-info/PKG-INFO` & `termapod-0.1.1/src/termapod.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: termapod
-Version: 0.1.0
+Version: 0.1.1
 Summary: An ASCII block / ANSI color renderer for NASA's Astonomy Pic of the Day. For like no reason.
 Author-email: Trevor Schrock <spacemeat@gmail.com>
 Maintainer-email: Trevor Schrock <spacemeat@gmail.com>
 License: MIT License
 Project-URL: Repository, https://github.com/spacemeat/termapod
 Keywords: astronomy,NASA,ASCII,ANSI
 Classifier: Development Status :: 4 - Beta
```

