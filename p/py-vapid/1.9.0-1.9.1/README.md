# Comparing `tmp/py-vapid-1.9.0.tar.gz` & `tmp/py_vapid-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-vapid-1.9.0.tar", last modified: Mon Dec  5 23:50:11 2022, max compression
+gzip compressed data, was "py_vapid-1.9.1.tar", last modified: Tue May 28 02:55:53 2024, max compression
```

## Comparing `py-vapid-1.9.0.tar` & `py_vapid-1.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 jrconlin  (1000) jrconlin  (1000)        0 2022-12-05 23:50:11.147311 py-vapid-1.9.0/
--rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)    16725 2020-06-08 16:07:17.000000 py-vapid-1.9.0/LICENSE
--rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)       91 2017-04-18 16:58:22.000000 py-vapid-1.9.0/MANIFEST.in
--rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)     4390 2022-12-05 23:50:11.147311 py-vapid-1.9.0/PKG-INFO
--rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)     3749 2022-09-23 15:55:47.000000 py-vapid-1.9.0/README.md
--rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)     3926 2022-12-05 23:49:33.000000 py-vapid-1.9.0/README.rst
-drwxrwxr-x   0 jrconlin  (1000) jrconlin  (1000)        0 2022-12-05 23:50:11.147311 py-vapid-1.9.0/py_vapid/
--rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)    11747 2022-09-23 15:56:38.000000 py-vapid-1.9.0/py_vapid/__init__.py
--rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)     2547 2020-06-08 16:07:17.000000 py-vapid-1.9.0/py_vapid/jwt.py
--rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)     4548 2022-09-23 15:56:38.000000 py-vapid-1.9.0/py_vapid/main.py
-drwxrwxr-x   0 jrconlin  (1000) jrconlin  (1000)        0 2022-12-05 23:50:11.147311 py-vapid-1.9.0/py_vapid/tests/
--rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)    10407 2022-09-23 15:55:47.000000 py-vapid-1.9.0/py_vapid/tests/test_vapid.py
--rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)      921 2020-06-08 16:07:17.000000 py-vapid-1.9.0/py_vapid/utils.py
-drwxrwxr-x   0 jrconlin  (1000) jrconlin  (1000)        0 2022-12-05 23:50:11.147311 py-vapid-1.9.0/py_vapid.egg-info/
--rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)     4390 2022-12-05 23:50:11.000000 py-vapid-1.9.0/py_vapid.egg-info/PKG-INFO
--rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)      424 2022-12-05 23:50:11.000000 py-vapid-1.9.0/py_vapid.egg-info/SOURCES.txt
--rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)        1 2022-12-05 23:50:11.000000 py-vapid-1.9.0/py_vapid.egg-info/dependency_links.txt
--rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)       64 2022-12-05 23:50:11.000000 py-vapid-1.9.0/py_vapid.egg-info/entry_points.txt
--rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)        1 2021-04-05 16:52:08.000000 py-vapid-1.9.0/py_vapid.egg-info/not-zip-safe
--rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)       18 2022-12-05 23:50:11.000000 py-vapid-1.9.0/py_vapid.egg-info/requires.txt
--rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)        9 2022-12-05 23:50:11.000000 py-vapid-1.9.0/py_vapid.egg-info/top_level.txt
--rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)       18 2020-06-08 16:07:17.000000 py-vapid-1.9.0/requirements.txt
--rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)      103 2022-12-05 23:50:11.147311 py-vapid-1.9.0/setup.cfg
--rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)     1693 2022-09-23 15:58:16.000000 py-vapid-1.9.0/setup.py
--rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)       55 2021-03-12 17:42:33.000000 py-vapid-1.9.0/test-requirements.txt
+drwxrwxr-x   0 jrconlin  (1000) jrconlin  (1000)        0 2024-05-28 02:55:53.904291 py_vapid-1.9.1/
+-rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)    16725 2020-06-08 16:07:17.000000 py_vapid-1.9.1/LICENSE
+-rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)       91 2017-04-18 16:58:22.000000 py_vapid-1.9.1/MANIFEST.in
+-rw-r--r--   0 jrconlin  (1000) jrconlin  (1000)     4403 2024-05-28 02:55:53.904291 py_vapid-1.9.1/PKG-INFO
+-rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)     4138 2022-12-05 23:57:58.000000 py_vapid-1.9.1/README.md
+-rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)     3926 2022-12-05 23:57:58.000000 py_vapid-1.9.1/README.rst
+drwxrwxr-x   0 jrconlin  (1000) jrconlin  (1000)        0 2024-05-28 02:55:53.901291 py_vapid-1.9.1/py_vapid/
+-rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)    12833 2024-05-28 01:57:36.000000 py_vapid-1.9.1/py_vapid/__init__.py
+-rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)     2547 2020-06-08 16:07:17.000000 py_vapid-1.9.1/py_vapid/jwt.py
+-rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)     4548 2022-12-05 23:52:53.000000 py_vapid-1.9.1/py_vapid/main.py
+drwxrwxr-x   0 jrconlin  (1000) jrconlin  (1000)        0 2024-05-28 02:55:53.903292 py_vapid-1.9.1/py_vapid/tests/
+-rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)    10403 2022-12-05 23:57:58.000000 py_vapid-1.9.1/py_vapid/tests/test_vapid.py
+-rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)      921 2020-06-08 16:07:17.000000 py_vapid-1.9.1/py_vapid/utils.py
+drwxrwxr-x   0 jrconlin  (1000) jrconlin  (1000)        0 2024-05-28 02:55:53.903292 py_vapid-1.9.1/py_vapid.egg-info/
+-rw-r--r--   0 jrconlin  (1000) jrconlin  (1000)     4403 2024-05-28 02:55:53.000000 py_vapid-1.9.1/py_vapid.egg-info/PKG-INFO
+-rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)      424 2024-05-28 02:55:53.000000 py_vapid-1.9.1/py_vapid.egg-info/SOURCES.txt
+-rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)        1 2024-05-28 02:55:53.000000 py_vapid-1.9.1/py_vapid.egg-info/dependency_links.txt
+-rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)       45 2024-05-28 02:55:53.000000 py_vapid-1.9.1/py_vapid.egg-info/entry_points.txt
+-rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)        1 2021-04-05 16:52:08.000000 py_vapid-1.9.1/py_vapid.egg-info/not-zip-safe
+-rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)       18 2024-05-28 02:55:53.000000 py_vapid-1.9.1/py_vapid.egg-info/requires.txt
+-rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)        9 2024-05-28 02:55:53.000000 py_vapid-1.9.1/py_vapid.egg-info/top_level.txt
+-rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)       18 2020-06-08 16:07:17.000000 py_vapid-1.9.1/requirements.txt
+-rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)      103 2024-05-28 02:55:53.905291 py_vapid-1.9.1/setup.cfg
+-rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)     1693 2024-05-28 02:45:33.000000 py_vapid-1.9.1/setup.py
+-rw-rw-r--   0 jrconlin  (1000) jrconlin  (1000)       55 2021-03-12 17:42:33.000000 py_vapid-1.9.1/test-requirements.txt
```

### Comparing `py-vapid-1.9.0/LICENSE` & `py_vapid-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py-vapid-1.9.0/PKG-INFO` & `py_vapid-1.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: py-vapid
-Version: 1.9.0
+Version: 1.9.1
 Summary: Simple VAPID header generation library
 Home-page: https://github.com/mozilla-services/vapid
 Author: JR Conlin
 Author-email: src+vapid@jrconlin.com
 License: MPL2
 Keywords: vapid push webpush
-Platform: UNKNOWN
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: cryptography>=2.5
 
 |PyPI version py_vapid|
 
 Easy VAPID generation
 =====================
 
 This minimal library contains the minimal set of functions you need to
@@ -117,9 +117,7 @@
 
 I’m terrible about updating the Changelog. Please see the
 ```git log`` <https://github.com/web-push-libs/vapid/pulls?q=is%3Apr+is%3Aclosed>`__
 history for details.
 
 .. |PyPI version py_vapid| image:: https://badge.fury.io/py/py-vapid.svg
    :target: https://pypi.org/project/py-vapid/
-
-
```

### Comparing `py-vapid-1.9.0/README.md` & `py_vapid-1.9.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,35 @@
+# Easy VAPID generation
+
 [![PyPI version py_vapid](https://badge.fury.io/py/py-vapid.svg)](https://pypi.org/project/py-vapid/)
 
-# Easy VAPID generation
+This library is available on [pypi as py-vapid](https://pypi.python.org/pypi/py-vapid).
+Source is available on [github](https://github.com/mozilla-services/vapid).
+Please note: This library was designated as a `Critical Project` by PyPi, it is currently
+maintained by [a single person](https://xkcd.com/2347/). I still accept PRs and Issues, but
+make of that what you will.
 
 This minimal library contains the minimal set of functions you need to
 generate a VAPID key set and get the headers you'll need to sign a
 WebPush subscription update.
 
 VAPID is a voluntary standard for WebPush subscription providers
 (sites that send WebPush updates to remote customers) to self-identify
 to Push Servers (the servers that convey the push notifications).
 
 The VAPID "claims" are a set of JSON keys and values. There are two
 required fields, one semi-optional and several optional additional
 fields.
 
 At a minimum a VAPID claim set should look like:
-```
+
+```json
 {"sub":"mailto:YourEmail@YourSite.com","aud":"https://PushServer","exp":"ExpirationTimestamp"}
 ```
+
 A few notes:
 
 ***sub*** is the email address you wish to have on record for this
 request, prefixed with "`mailto:`". If things go wrong, this is the
 email that will be used to contact you (for instance). This can be a
 general delivery address like "`mailto:push_operations@example.com`" or a
 specific address like "`mailto:bob@example.com`".
@@ -52,19 +60,21 @@
 app, `bin/vapid`.
 
 ## App Installation
 
 You'll need `python virtualenv` Run that in the current directory.
 
 Then run
-```
+
+```python
 bin/pip install -r requirements.txt
 
 bin/python setup.py install
 ```
+
 ## App Usage
 
 Run by itself, `bin/vapid` will check and optionally create the
 public_key.pem and private_key.pem files.
 
 `bin/vapid --gen` can be used to generate a new set of public and
 private key PEM files. These will overwrite the contents of
```

### Comparing `py-vapid-1.9.0/README.rst` & `py_vapid-1.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `py-vapid-1.9.0/py_vapid/__init__.py` & `py_vapid-1.9.1/py_vapid/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -312,14 +312,25 @@
 
     https://tools.ietf.org/html/rfc8292
 
     """
     _schema = "vapid"
 
     def sign(self, claims, crypto_key=None):
+        """Generate an authorization token
+
+        :param claims: JSON object containing the JWT claims to use.
+        :type claims: dict
+        :param crypto_key: Optional existing crypto_key header content. The
+            vapid public key will be appended to this data.
+        :type crypto_key: str
+        :returns: a hash containing the header fields to use in
+            the subscription update.
+        :rtype: dict
+        """
         sig = sign(self._base_sign(claims), self.private_key)
         pkey = self.public_key.public_bytes(
                 serialization.Encoding.X962,
                 serialization.PublicFormat.UncompressedPoint
             )
         return{
             "Authorization": "{schema} t={t},k={k}".format(
@@ -327,14 +338,21 @@
                 t=sig,
                 k=b64urlencode(pkey)
             )
         }
 
     @classmethod
     def verify(cls, auth):
+        """Ensure that the token is correctly formatted and valid
+
+        :param auth: An Authorization header
+        :type auth: str
+        :rtype: bool
+
+        """
         pref_tok = auth.rsplit(' ', 1)
         assert pref_tok[0].lower() == cls._schema, (
                 "Incorrect schema specified")
         parts = {}
         for tok in pref_tok[1].split(','):
             kv = tok.split('=', 1)
             parts[kv[0]] = kv[1]
@@ -345,15 +363,29 @@
         kp = cls().from_raw_public(parts['k'].encode())
         tokens = parts['t'].rsplit('.', 1)
         return kp.verify_token(
             validation_token=tokens[0].encode(),
             verification_token=tokens[1]
         )
 
+
 def _check_sub(sub):
-    pattern =(
-        r"^(mailto:.+@((localhost|[%\w-]+(\.[%\w-]+)+|([0-9a-f]{1,4}):+([0-9a-f]{1,4})?)))|https:\/\/(localhost|[\w-]+\.[\w\.-]+|([0-9a-f]{1,4}:+)+([0-9a-f]{1,4})?)$"
+    """ Check to see if the `sub` is a properly formatted `mailto:`
+
+    a `mailto:` should be a SMTP mail address. Mind you, since I run
+    YouFailAtEmail.com, you have every right to yell about how terrible
+    this check is. I really should be doing a proper component parse
+    and valiate each component individually per RFC5341, instead I do
+    the unholy regex you see below.
+
+    :param sub: Candidate JWT `sub`
+    :type sub: str
+    :rtype: bool
+
+    """
+    pattern = (
+        r"^(mailto:.+@((localhost|[%\w-]+(\.[%\w-]+)+|([0-9a-f]{1,4}):+([0-9a-f]{1,4})?)))|https:\/\/(localhost|[\w-]+\.[\w\.-]+|([0-9a-f]{1,4}:+)+([0-9a-f]{1,4})?)$" # noqa
         )
     return re.match(pattern, sub, re.IGNORECASE) is not None
 
 
 Vapid = Vapid02
```

### Comparing `py-vapid-1.9.0/py_vapid/jwt.py` & `py_vapid-1.9.1/py_vapid/jwt.py`

 * *Files identical despite different names*

### Comparing `py-vapid-1.9.0/py_vapid/main.py` & `py_vapid-1.9.1/py_vapid/main.py`

 * *Files identical despite different names*

### Comparing `py-vapid-1.9.0/py_vapid/tests/test_vapid.py` & `py_vapid-1.9.1/py_vapid/tests/test_vapid.py`

 * *Files 4% similar despite different names*

```diff
@@ -142,16 +142,16 @@
                 serialization.PublicFormat.UncompressedPoint
             )
         ).decode('utf8').replace('+', '-').replace('/', '_').strip()
         items = decode(result['Authorization'].split(' ')[1], pkey)
         for k in claims:
             assert items[k] == claims[k]
         result = v.sign(claims)
-        assert result['Crypto-Key'] == ('p256ecdsa=' +
-            TEST_KEY_PUBLIC_RAW.decode('utf8'))
+        assert result['Crypto-Key'] == (
+            'p256ecdsa=' + TEST_KEY_PUBLIC_RAW.decode('utf8'))
         # Verify using the same function as Integration
         # this should ensure that the r,s sign values are correctly formed
         assert Vapid01.verify(
             key=result['Crypto-Key'].split('=')[1],
             auth=result['Authorization']
         )
 
@@ -206,15 +206,15 @@
         key = ("BDd3_hVL9fZi9Ybo2UUzA284WG5FZR30_95YeZJsiApwXKpNcF1rRPF3foI"
                "iBHXRdJI2Qhumhf6_LFTeZaNndIo")
         auth = ("WebPush eyJ0eXAiOiJKV1QiLCJhbGciOiJFUzI1NiJ9.eyJhdWQiOiJod"
                 "HRwczovL3VwZGF0ZXMucHVzaC5zZXJ2aWNlcy5tb3ppbGxhLmNvbSIsImV"
                 "4cCI6MTQ5NDY3MTQ3MCwic3ViIjoibWFpbHRvOnNpbXBsZS1wdXNoLWRlb"
                 "W9AZ2F1bnRmYWNlLmNvLnVrIn0.LqPi86T-HJ71TXHAYFptZEHD7Wlfjcc"
                 "4u5jYZ17WpqOlqDcW-5Wtx3x1OgYX19alhJ9oLumlS2VzEvNioZ_BAD")
-        assert Vapid01.verify(key=key, auth=auth) == False
+        assert not Vapid01.verify(key=key, auth=auth)
 
     def test_bad_sign(self):
         v = Vapid01.from_file("/tmp/private")
         self.assertRaises(VapidException,
                           v.sign,
                           {})
         self.assertRaises(VapidException,
```

### Comparing `py-vapid-1.9.0/py_vapid/utils.py` & `py_vapid-1.9.1/py_vapid/utils.py`

 * *Files identical despite different names*

### Comparing `py-vapid-1.9.0/py_vapid.egg-info/PKG-INFO` & `py_vapid-1.9.1/py_vapid.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: py-vapid
-Version: 1.9.0
+Version: 1.9.1
 Summary: Simple VAPID header generation library
 Home-page: https://github.com/mozilla-services/vapid
 Author: JR Conlin
 Author-email: src+vapid@jrconlin.com
 License: MPL2
 Keywords: vapid push webpush
-Platform: UNKNOWN
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: cryptography>=2.5
 
 |PyPI version py_vapid|
 
 Easy VAPID generation
 =====================
 
 This minimal library contains the minimal set of functions you need to
@@ -117,9 +117,7 @@
 
 I’m terrible about updating the Changelog. Please see the
 ```git log`` <https://github.com/web-push-libs/vapid/pulls?q=is%3Apr+is%3Aclosed>`__
 history for details.
 
 .. |PyPI version py_vapid| image:: https://badge.fury.io/py/py-vapid.svg
    :target: https://pypi.org/project/py-vapid/
-
-
```

### Comparing `py-vapid-1.9.0/setup.py` & `py_vapid-1.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import io
 import os
 
 from setuptools import setup, find_packages
 
-__version__ = "1.9.0"
+__version__ = "1.9.1"
 
 
 def read_from(file):
     reply = []
     with io.open(os.path.join(here, file), encoding='utf8') as f:
         for l in f:
             l = l.strip()
```

