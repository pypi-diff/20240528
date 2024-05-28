# Comparing `tmp/audire-1.0.1b1.tar.gz` & `tmp/audire-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audire-1.0.1b1.tar", last modified: Mon May 20 13:37:09 2024, max compression
+gzip compressed data, was "audire-1.1.0.tar", last modified: Tue May 28 09:09:16 2024, max compression
```

## Comparing `audire-1.0.1b1.tar` & `audire-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:37:09.512989 audire-1.0.1b1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:37:09.512989 audire-1.0.1b1/Audire.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-20 13:37:09.000000 audire-1.0.1b1/Audire.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-20 13:37:09.000000 audire-1.0.1b1/Audire.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 13:37:09.000000 audire-1.0.1b1/Audire.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-20 13:37:09.000000 audire-1.0.1b1/Audire.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 13:37:09.000000 audire-1.0.1b1/Audire.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-20 13:37:05.000000 audire-1.0.1b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-20 13:37:09.512989 audire-1.0.1b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-20 13:37:05.000000 audire-1.0.1b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:37:09.512989 audire-1.0.1b1/audire/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-20 13:37:05.000000 audire-1.0.1b1/audire/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-05-20 13:37:05.000000 audire-1.0.1b1/audire/dotdict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-05-20 13:37:05.000000 audire-1.0.1b1/audire/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:37:09.512989 audire-1.0.1b1/audire/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-20 13:37:05.000000 audire-1.0.1b1/audire/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-20 13:37:05.000000 audire-1.0.1b1/audire/helpers/soundcloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-05-20 13:37:05.000000 audire-1.0.1b1/audire/helpers/youtube.py
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-20 13:37:05.000000 audire-1.0.1b1/audire/main.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 13:37:09.512989 audire-1.0.1b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-20 13:37:05.000000 audire-1.0.1b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:09:16.403142 audire-1.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:09:16.403142 audire-1.1.0/Audire.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-28 09:09:16.000000 audire-1.1.0/Audire.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-28 09:09:16.000000 audire-1.1.0/Audire.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 09:09:16.000000 audire-1.1.0/Audire.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-28 09:09:16.000000 audire-1.1.0/Audire.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-28 09:09:16.000000 audire-1.1.0/Audire.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-28 09:09:12.000000 audire-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-28 09:09:16.403142 audire-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-28 09:09:12.000000 audire-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:09:16.403142 audire-1.1.0/audire/
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-28 09:09:12.000000 audire-1.1.0/audire/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-05-28 09:09:12.000000 audire-1.1.0/audire/dotdict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-28 09:09:12.000000 audire-1.1.0/audire/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:09:16.403142 audire-1.1.0/audire/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-28 09:09:12.000000 audire-1.1.0/audire/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-28 09:09:12.000000 audire-1.1.0/audire/helpers/saavn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-28 09:09:12.000000 audire-1.1.0/audire/helpers/soundcloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-05-28 09:09:12.000000 audire-1.1.0/audire/helpers/spotify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-28 09:09:12.000000 audire-1.1.0/audire/helpers/youtube.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-05-28 09:09:12.000000 audire-1.1.0/audire/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 09:09:16.403142 audire-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-28 09:09:12.000000 audire-1.1.0/setup.py
```

### Comparing `audire-1.0.1b1/Audire.egg-info/PKG-INFO` & `audire-1.1.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,15 @@
-Metadata-Version: 2.1
-Name: Audire
-Version: 1.0.1b1
-Summary: A Package to search and get download links for songs from various platforms asynchronously.
-Home-page: https://github.com/LinuxGuy312/Audire
-Author: Eren
-Author-email: linuxguy312@segfault.net
-License: MIT
-Keywords: songs,song,music,youtube,ytm,Audire,audire
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: ~=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: aiohttp
-Requires-Dist: bs4
-
 # Audire
 
 A Package to search and get download links for songs from various platforms asynchronously.
 
-[![Python](http://forthebadge.com/images/badges/made-with-python.svg)](https://python.org/)
+![Python](https://img.shields.io/badge/made_with-python-blue?style=for-the-badge&logoColor=blue&labelColor=lightblue&link=https%3A%2F%2Fwww.python.org)
+![PyPI - Version](https://img.shields.io/pypi/v/Audire?style=for-the-badge&label=Audire&link=https%3A%2F%2Fpypi.org%2Fproject%2FAudire)
+
 
----
-> [!NOTE]
-> "Audire" is a Latin verb meaning "to hear" or "to listen." It's the root of many English words related to sound and listening, like "audit" and "auditory."
 
 
 ## Installation
 
 ```sh
 $ pip install audire
 ```
@@ -80,7 +56,18 @@
 However, you can take help from the well written docstrings this way:
 
 ```py
 from audire import Audire
 
 print(help(Audire().search))
 ```
+
+## License
+This project is licensed under the MIT License. See the [MIT](https://opensource.org/license/mit) file for details.
+
+## Contributing
+If you wish to contribute to this project, please [fork](https://github.com/LinuxGuy312/Audire/fork) and [create a pull request](https://github.com/LinuxGuy312/Audire/compare) or [submit an issue](https://github.com/LinuxGuy312/Audire/issues/new).
+
+## Contact
+For any Questions or concerns, please contact me at:
+- Telegram : [@WH0907](https://t.me/WH0907)
+- Email : linuxguy312@segfault.net
```

### Comparing `audire-1.0.1b1/LICENSE` & `audire-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `audire-1.0.1b1/audire/__init__.py` & `audire-1.1.0/audire/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 from .main import *
 
-__version__ = "1.0.1b1"
+__version__ = "1.1.0"
```

### Comparing `audire-1.0.1b1/audire/dotdict.py` & `audire-1.1.0/audire/dotdict.py`

 * *Files identical despite different names*

### Comparing `audire-1.0.1b1/audire/errors.py` & `audire-1.1.0/audire/errors.py`

 * *Files 13% similar despite different names*

```diff
@@ -52,7 +52,15 @@
 
 class NoResultsFoundError(BaseError):
     """
     Exception raised when no results are found for a given query.
     """
 
     message = "No Results Found for the given query"
+
+
+class NoDownloadsFoundError(BaseError):
+    """
+    Exception raised when no download results are found for the given URL.
+    """
+
+    message = "No Download Results Found for the given URL"
```

### Comparing `audire-1.0.1b1/audire/helpers/__init__.py` & `audire-1.1.0/audire/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `audire-1.0.1b1/audire/helpers/soundcloud.py` & `audire-1.1.0/audire/helpers/soundcloud.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,10 +46,10 @@
 
     async with aiohttp.request(
         "POST", url=api, json=payload, headers=headers
     ) as response:
         response = await response.json()
         dlurl = response.get("url")
         if not url:
-            raise errors.NoResultsFoundError
+            raise errors.NoDownloadsFoundError
         data = {"download_url": dlurl}
         return dotdict.DotDict(data)
```

### Comparing `audire-1.0.1b1/audire/helpers/youtube.py` & `audire-1.1.0/audire/helpers/youtube.py`

 * *Files 9% similar despite different names*

```diff
@@ -76,10 +76,10 @@
 
     async with aiohttp.request(
         "POST", url=api, json=payload, headers=headers
     ) as response:
         response = await response.json()
         dlurl = response.get("url")
         if not url:
-            raise errors.NoResultsFoundError
+            raise errors.NoDownloadsFoundError
         data = {"download_url": dlurl}
         return dotdict.DotDict(data)
```

### Comparing `audire-1.0.1b1/audire/main.py` & `audire-1.1.0/audire/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,32 +19,36 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 from audire import dotdict, errors
 from audire.helpers import (
-    youtube,
+    saavn,
     soundcloud,
+    spotify,
+    youtube,
 )
 
 
 class Audire:
     """
     Audire class search and get download links for music across various platforms.
 
     Attributes:
         platforms (list): List of supported Platforms.
     """
 
     def __init__(self):
         self.platforms = [
+            "saavn",  # JioSaavn
+            "soundcloud",  # SoundCloud
+            "spotify",  # Spotify
             "yt",  # YouTube
             "ytm",  # YouTube Music
-            "soundcloud",
         ]
 
     async def search(
         self, query: str, platform: str = "ytm", limit: int = 10
     ) -> dotdict.DotDict:
         """
         Audire Search Function.
@@ -65,14 +69,20 @@
 
         if platform == "ytm":
             return await youtube.search(query, True, limit)
 
         if platform == "soundcloud":
             return None
 
+        if platform == "saavn":
+            return await saavn.search(query, limit)
+
+        if platform == "spotify":
+            return await spotify.search(query, limit)
+
     async def get_download(self, url: str, platform: str) -> dotdict.DotDict:
         """
         Returns An Object.
 
         Parameters:
             url (str): URL of song.
             platform (str): Platform of download.
@@ -85,7 +95,13 @@
             raise errors.PlatformNotSupportedError
 
         if platform in ("yt", "ytm"):
             return await youtube.get_download(url)
 
         if platform == "soundcloud":
             return await soundcloud.get_download(url)
+
+        if platform == "saavn":
+            return await saavn.get_download(url)
+
+        if platform == "spotify":
+            return await spotify.get_download(url)
```

### Comparing `audire-1.0.1b1/setup.py` & `audire-1.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,12 +31,12 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
-        "Development Status :: 4 - Beta",
+        "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: MIT License",
     ],
     python_requires="~=3.7",
 )
```

