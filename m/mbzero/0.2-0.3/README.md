# Comparing `tmp/mbzero-0.2.tar.gz` & `tmp/mbzero-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbzero-0.2.tar", last modified: Wed Apr 10 13:53:32 2024, max compression
+gzip compressed data, was "mbzero-0.3.tar", last modified: Tue May 28 13:29:56 2024, max compression
```

## Comparing `mbzero-0.2.tar` & `mbzero-0.3.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 louis     (1337) louis     (1337)        0 2024-04-10 13:53:32.622236 mbzero-0.2/
--rw-r--r--   0 louis     (1337) louis     (1337)     1269 2024-04-09 18:56:12.000000 mbzero-0.2/LICENSE
--rw-r--r--   0 louis     (1337) louis     (1337)     2894 2024-04-10 13:53:32.622236 mbzero-0.2/PKG-INFO
--rw-r--r--   0 louis     (1337) louis     (1337)     1976 2024-04-08 21:03:02.000000 mbzero-0.2/README.md
-drwxr-xr-x   0 louis     (1337) louis     (1337)        0 2024-04-10 13:53:32.622236 mbzero-0.2/mbzero/
--rw-r--r--   0 louis     (1337) louis     (1337)      309 2024-04-09 21:26:05.000000 mbzero-0.2/mbzero/__init__.py
--rw-r--r--   0 louis     (1337) louis     (1337)     1987 2024-04-10 13:23:13.000000 mbzero-0.2/mbzero/caarequest.py
--rw-r--r--   0 louis     (1337) louis     (1337)     7640 2024-04-10 13:23:54.000000 mbzero-0.2/mbzero/mbzauth.py
--rw-r--r--   0 louis     (1337) louis     (1337)      745 2024-04-09 19:00:53.000000 mbzero-0.2/mbzero/mbzerror.py
--rw-r--r--   0 louis     (1337) louis     (1337)    10024 2024-04-09 19:48:38.000000 mbzero-0.2/mbzero/mbzrequest.py
--rw-r--r--   0 louis     (1337) louis     (1337)     2484 2024-04-09 19:00:38.000000 mbzero-0.2/mbzero/oauth2_session_revoke.py
-drwxr-xr-x   0 louis     (1337) louis     (1337)        0 2024-04-10 13:53:32.622236 mbzero-0.2/mbzero.egg-info/
--rw-r--r--   0 louis     (1337) louis     (1337)     2894 2024-04-10 13:53:32.000000 mbzero-0.2/mbzero.egg-info/PKG-INFO
--rw-r--r--   0 louis     (1337) louis     (1337)      424 2024-04-10 13:53:32.000000 mbzero-0.2/mbzero.egg-info/SOURCES.txt
--rw-r--r--   0 louis     (1337) louis     (1337)        1 2024-04-10 13:53:32.000000 mbzero-0.2/mbzero.egg-info/dependency_links.txt
--rw-r--r--   0 louis     (1337) louis     (1337)      138 2024-04-10 13:53:32.000000 mbzero-0.2/mbzero.egg-info/requires.txt
--rw-r--r--   0 louis     (1337) louis     (1337)        7 2024-04-10 13:53:32.000000 mbzero-0.2/mbzero.egg-info/top_level.txt
--rw-r--r--   0 louis     (1337) louis     (1337)      861 2024-04-10 13:49:32.000000 mbzero-0.2/pyproject.toml
--rw-r--r--   0 louis     (1337) louis     (1337)       38 2024-04-10 13:53:32.622236 mbzero-0.2/setup.cfg
-drwxr-xr-x   0 louis     (1337) louis     (1337)        0 2024-04-10 13:53:32.622236 mbzero-0.2/tests/
--rw-r--r--   0 louis     (1337) louis     (1337)     6213 2024-04-09 19:01:37.000000 mbzero-0.2/tests/test_auth.py
--rw-r--r--   0 louis     (1337) louis     (1337)     3328 2024-04-10 13:25:44.000000 mbzero-0.2/tests/test_caa.py
--rw-r--r--   0 louis     (1337) louis     (1337)     2873 2024-04-09 19:02:22.000000 mbzero-0.2/tests/test_oauthrequests.py
--rw-r--r--   0 louis     (1337) louis     (1337)    15042 2024-04-09 19:01:56.000000 mbzero-0.2/tests/test_requests.py
--rw-r--r--   0 louis     (1337) louis     (1337)     8364 2024-04-10 13:26:29.000000 mbzero-0.2/tests/test_submission.py
+drwxr-xr-x   0 louis     (1337) louis     (1337)        0 2024-05-28 13:29:56.755446 mbzero-0.3/
+-rw-r--r--   0 louis     (1337) louis     (1337)     1269 2024-04-09 18:56:12.000000 mbzero-0.3/LICENSE
+-rw-r--r--   0 louis     (1337) louis     (1337)     2894 2024-05-28 13:29:56.755446 mbzero-0.3/PKG-INFO
+-rw-r--r--   0 louis     (1337) louis     (1337)     1976 2024-04-08 21:03:02.000000 mbzero-0.3/README.md
+drwxr-xr-x   0 louis     (1337) louis     (1337)        0 2024-05-28 13:29:56.755446 mbzero-0.3/mbzero/
+-rw-r--r--   0 louis     (1337) louis     (1337)      309 2024-05-19 20:48:05.000000 mbzero-0.3/mbzero/__init__.py
+-rw-r--r--   0 louis     (1337) louis     (1337)     1987 2024-04-10 13:23:13.000000 mbzero-0.3/mbzero/caarequest.py
+-rw-r--r--   0 louis     (1337) louis     (1337)     7314 2024-05-27 21:31:19.000000 mbzero-0.3/mbzero/mbzauth.py
+-rw-r--r--   0 louis     (1337) louis     (1337)      741 2024-05-27 21:31:19.000000 mbzero-0.3/mbzero/mbzerror.py
+-rw-r--r--   0 louis     (1337) louis     (1337)    10147 2024-05-27 21:31:19.000000 mbzero-0.3/mbzero/mbzrequest.py
+-rw-r--r--   0 louis     (1337) louis     (1337)     2484 2024-05-27 20:58:35.000000 mbzero-0.3/mbzero/oauth2_session_revoke.py
+drwxr-xr-x   0 louis     (1337) louis     (1337)        0 2024-05-28 13:29:56.755446 mbzero-0.3/mbzero.egg-info/
+-rw-r--r--   0 louis     (1337) louis     (1337)     2894 2024-05-28 13:29:56.000000 mbzero-0.3/mbzero.egg-info/PKG-INFO
+-rw-r--r--   0 louis     (1337) louis     (1337)      445 2024-05-28 13:29:56.000000 mbzero-0.3/mbzero.egg-info/SOURCES.txt
+-rw-r--r--   0 louis     (1337) louis     (1337)        1 2024-05-28 13:29:56.000000 mbzero-0.3/mbzero.egg-info/dependency_links.txt
+-rw-r--r--   0 louis     (1337) louis     (1337)      138 2024-05-28 13:29:56.000000 mbzero-0.3/mbzero.egg-info/requires.txt
+-rw-r--r--   0 louis     (1337) louis     (1337)        7 2024-05-28 13:29:56.000000 mbzero-0.3/mbzero.egg-info/top_level.txt
+-rw-r--r--   0 louis     (1337) louis     (1337)      861 2024-05-28 13:28:17.000000 mbzero-0.3/pyproject.toml
+-rw-r--r--   0 louis     (1337) louis     (1337)       38 2024-05-28 13:29:56.755446 mbzero-0.3/setup.cfg
+drwxr-xr-x   0 louis     (1337) louis     (1337)        0 2024-05-28 13:29:56.755446 mbzero-0.3/tests/
+-rw-r--r--   0 louis     (1337) louis     (1337)     9226 2024-05-27 21:31:19.000000 mbzero-0.3/tests/test_auth.py
+-rw-r--r--   0 louis     (1337) louis     (1337)     3610 2024-05-27 21:31:19.000000 mbzero-0.3/tests/test_caa.py
+-rw-r--r--   0 louis     (1337) louis     (1337)     1596 2024-05-27 21:28:03.000000 mbzero-0.3/tests/test_errors.py
+-rw-r--r--   0 louis     (1337) louis     (1337)     2806 2024-05-27 21:31:19.000000 mbzero-0.3/tests/test_oauthrequests.py
+-rw-r--r--   0 louis     (1337) louis     (1337)    16641 2024-05-27 21:31:19.000000 mbzero-0.3/tests/test_requests.py
+-rw-r--r--   0 louis     (1337) louis     (1337)     9292 2024-05-27 21:31:19.000000 mbzero-0.3/tests/test_submission.py
```

### Comparing `mbzero-0.2/LICENSE` & `mbzero-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mbzero-0.2/PKG-INFO` & `mbzero-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbzero
-Version: 0.2
+Version: 0.3
 Summary: Python bindings for the MusicBrainz and the Cover Art Archive webservices
 Author-email: Louis Rannou <louson@gresille.org>
 Project-URL: Homepage, https://gitlab.com/Louson-public/personal/python-mbzero
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
```

### Comparing `mbzero-0.2/README.md` & `mbzero-0.3/README.md`

 * *Files identical despite different names*

### Comparing `mbzero-0.2/mbzero/caarequest.py` & `mbzero-0.3/mbzero/caarequest.py`

 * *Files identical despite different names*

### Comparing `mbzero-0.2/mbzero/mbzauth.py` & `mbzero-0.3/mbzero/mbzauth.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,38 +26,33 @@
         :param oauth2_url: optional OAuth2 endpoint"""
         self.name = None
         self.password = None
         self.oauth2_url = oauth2_url or MUSICBRAINZ_OAUTH2
         self.oauth2_client_id = None
         self.oauth2_client_secret = None
         self.oauth2_session = None
-        self.oauth2_token = None
-        self.oauth2_refresh_token = None
 
     def has_auth(self):
         """Returns true if name/passwd credentials have been set"""
         return (self.name is not None) and (self.password is not None)
 
     def has_oauth2(self):
         """Returns true if OAuth2 has been set"""
-        return self.oauth2_token is not None
+        return (self.oauth2_session is not None
+                and self.oauth2_session.authorized)
 
     def auth_set(self, name, passwd):
         """Username/password authentication"""
         self.name = name
         self.password = passwd
 
     def auth(self):
         """Get username/password"""
         return (self.name, self.password)
 
-    def oauth2(self):
-        """Get the OAuth2 session"""
-        return self.oauth2_session
-
     def oauth2_set_url(self, url):
         """Change the default OAuth2 endpoint"""
         self.oauth2_url = url
 
     def oauth2_new(self, token, refresh_token=None,
                    client_id=None, client_secret=None,
                    redirect_uri=MUSICBRAINZ_OAUTH2_URI, scope=[]):
@@ -66,22 +61,28 @@
         :param token: access token to use for authentication
         :param refresh_token: refresh token to use for refreshing
         :param client_id: optional client application ID
         :param client_secret: optional client application secret
         :param redirect_uri: optional redirect URI (defaults to the redirect
                              URI defined in the Musicbrainz documentation)
         :param scope: optional Musicbrainz scope"""
+        oauth2_token = {
+            "access_token": token,
+            "token_type": "bearer"
+        }
+        if refresh_token is not None:
+            oauth2_token["refresh_token"] = refresh_token
+
         try:
             self.oauth2_session = OAuth2Session(client_id,
+                                                scope=scope,
                                                 redirect_uri=redirect_uri,
-                                                scope=scope)
+                                                token=oauth2_token)
             self.oauth2_client_id = client_id
             self.oauth2_client_secret = client_secret
-            self.oauth2_token = token
-            self.oauth2_refresh_token = refresh_token
         except Exception as e:
             raise MbzOauth2Error(e)
 
     def oauth2_init(self, client_id, url=None,
                     redirect_uri=MUSICBRAINZ_OAUTH2_URI, scope=[]):
         """Initialize the creation of tokens
 
@@ -116,56 +117,50 @@
             url = self.oauth2_url + OAUTH2_PATH_TOKEN
 
         try:
             token = self.oauth2_session.fetch_token(
                 url, code=response_code,
                 client_secret=client_secret)
             self.oauth2_client_secret = client_secret
-            self.oauth2_token = token["access_token"]
-            self.oauth2_refresh_token = token["refresh_token"]
             return token
         except Exception as e:
             raise MbzOauth2Error(e)
 
     def oauth2_refresh(self, refresh_token=None,
                        url=None):
         """Refresh an access token.
 
         :param refresh_token: optional refresh token used to refresh the
                               access token
         :param url: optional token endpoint (defaults to musicbrainz)
         :return: the new access token"""
-        if not self.oauth2_refresh_token and not refresh_token:
-            raise MbzOauth2Error("No refresh token known")
-        elif not refresh_token:
-            refresh_token = self.oauth2_refresh_token
-
         if url is None:
             url = self.oauth2_url + OAUTH2_PATH_TOKEN
 
         try:
             token = self.oauth2_session.refresh_token(
                 url, refresh_token=refresh_token,
                 client_id=self.oauth2_client_id,
                 client_secret=self.oauth2_client_secret)
-            self.oauth2_token = token["access_token"]
             return token
         except Exception as e:
             raise MbzOauth2Error(e)
 
     def oauth2_revoke(self, token=None, url=None):
         """Revoke a token pair
 
-        :param token: optional token used to refresh the access token
+        :param token: optional token used to refresh the access token.
+                      If not provided, the current session's access_token
+                      is revoked.
         :param url: optional revocation endpoint (defaults to musicbrainz)
         """
-        if not self.oauth2_token and not token:
-            raise MbzOauth2Error("No refresh token known")
-        elif not token:
-            token = self.oauth2_token
+        if self.oauth2_session is None:
+            raise MbzOauth2Error("OAuth2 session not initialiazed")
+        if token is None:
+            token = self.oauth2_session.access_token
 
         if url is None:
             url = self.oauth2_url + OAUTH2_PATH_REVOKE
 
         try:
             revoke_token(self.oauth2_session,
                          url, token,
@@ -183,23 +178,19 @@
         :param headers: Optional request headers
         :param url: Optional API endpoint (defaults is to
                     musicbrainz.org OAuth2 endpoint)
         :return: the result of the request"""
         if url is None:
             url = self.oauth2_url
 
-        headers["Authorization"] = "Bearer %s" % self.oauth2_token
-
         return self.oauth2_session.get(
             url + request, params=payload,
             headers=headers)
 
     def _oauth2_post(self, request, payload={}, headers={},
                      data=None, url=None):
         if url is None:
             url = self.oauth2_url
 
-        headers["Authorization"] = "Bearer %s" % self.oauth2_token
-
         return self.oauth2_session.post(
             url + request, data=data, params=payload,
             headers=headers)
```

### Comparing `mbzero-0.2/mbzero/mbzerror.py` & `mbzero-0.3/mbzero/mbzerror.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,14 @@
         self.cause = cause
 
     def __str__(self):
         if self.message:
             msg = "%s, " % self.message
         else:
             msg = ""
-            msg += "caused by: %s" % str(self.cause)
+        msg += "caused by: %s" % str(self.cause)
         return msg
 
 
 class MbzOauth2Error(MbzWebServiceError):
     """OAuth2 failure"""
     pass
```

### Comparing `mbzero-0.2/mbzero/mbzrequest.py` & `mbzero-0.3/mbzero/mbzrequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,16 +116,19 @@
             _headers = headers.copy()
         if "User-Agent" not in _headers:
             _headers["User-Agent"] = self.user_agent
 
         if data_type == "xml":
             _headers["Content-Type"] = "application/xml; charset=utf-8"
         else:
-            raise Exception("Musicbrainz does not support %s content"
-                            % data_type)
+            raise MbzSubmissionError("Musicbrainz does not support %s content"
+                                     % data_type)
+
+        if credentials is None:
+            raise MbzSubmissionError("Submission requires credentials")
 
         if opts is not None:
             if "url" in opts:
                 url = opts.get("url", "")
             if "extra_headers" in opts:
                 _headers.update(opts.get("extra_headers"))
             if "extra_payload" in opts:
```

### Comparing `mbzero-0.2/mbzero/oauth2_session_revoke.py` & `mbzero-0.3/mbzero/oauth2_session_revoke.py`

 * *Files identical despite different names*

### Comparing `mbzero-0.2/mbzero.egg-info/PKG-INFO` & `mbzero-0.3/mbzero.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbzero
-Version: 0.2
+Version: 0.3
 Summary: Python bindings for the MusicBrainz and the Cover Art Archive webservices
 Author-email: Louis Rannou <louson@gresille.org>
 Project-URL: Homepage, https://gitlab.com/Louson-public/personal/python-mbzero
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
```

### Comparing `mbzero-0.2/pyproject.toml` & `mbzero-0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires  = [
     "setuptools", "requests", "requests_oauthlib"
 ]
 
 [project]
 name = "mbzero"
-version = "0.2"
+version = "0.3"
 description = "Python bindings for the MusicBrainz and the Cover Art Archive webservices"
 readme = "README.md"
 authors = [
     {name = "Louis Rannou", email = "louson@gresille.org"},
 ]
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `mbzero-0.2/tests/test_auth.py` & `mbzero-0.3/tests/test_auth.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 
 import unittest
 from unittest.mock import patch
 
 from mbzero import mbzauth as mba
 
 
+def _raise_exception(*args, **kwargs):
+    raise Exception("mock")
+
+
 class AuthTest(unittest.TestCase):
     def testAuth(self):
         cred = mba.MbzCredentials()
         self.assertFalse(cred.has_auth())
         cred.auth_set("name", "pass")
         self.assertTrue(cred.has_auth())
         self.assertEqual(cred.auth(), ("name", "pass"))
@@ -65,36 +69,63 @@
     def testInitURLSetOther(self, mock_auth):
         mock_auth.return_value = ["auth_url", 1]
         self.cred.oauth2_init(self.client_id, url="somewhere")
         mock_auth.assert_called_once_with(
             "somewhere"
         )
 
+    @patch('requests_oauthlib.OAuth2Session.__init__', _raise_exception)
+    def testInitFails(self):
+        t = False
+        try:
+            self.cred.oauth2_init(self.client_id)
+        except mba.MbzOauth2Error:
+            t = True
+        self.assertTrue(t)
+
+    @patch('requests_oauthlib.OAuth2Session.__init__', _raise_exception)
+    def testNewFails(self):
+        t = False
+        try:
+            self.cred.oauth2_new(None)
+        except mba.MbzOauth2Error:
+            t = True
+        self.assertTrue(t)
+
 
 class Oauth2Process(unittest.TestCase):
     def setUp(self):
         self.client_id = "clientID"
         self.client_secret = "clientSecret"
         self.token = "token"
         self.refresh = "refresh"
         self.cred = mba.MbzCredentials()
         self.cred.oauth2_new(self.token, self.refresh,
                              client_id=self.client_id,
                              client_secret=self.client_secret)
-        self.headers = {"Authorization": "Bearer %s" % self.token}
+        self.headers = {}
 
     @patch('requests_oauthlib.OAuth2Session.fetch_token')
     def testConfirm(self, mock_fetch):
         mock_fetch.return_value = {"access_token": self.token,
                                    "refresh_token": self.refresh}
         self.cred.oauth2_confirm("code", self.client_secret)
         mock_fetch.assert_called_once_with(
             mba.MUSICBRAINZ_OAUTH2 + mba.OAUTH2_PATH_TOKEN,
             code="code", client_secret=self.client_secret)
 
+    @patch('requests_oauthlib.OAuth2Session.fetch_token', _raise_exception)
+    def testConfirmFail(self):
+        t = False
+        try:
+            self.cred.oauth2_confirm("code", self.client_secret)
+        except mba.MbzOauth2Error:
+            t = True
+        self.assertTrue(t)
+
     @patch('requests_oauthlib.OAuth2Session.fetch_token')
     def testConfirmAPIOther(self, mock_fetch):
         mock_fetch.return_value = {"access_token": self.token,
                                    "refresh_token": self.refresh}
         self.cred.oauth2_confirm("code", self.client_secret,
                                  url="somewhere")
         mock_fetch.assert_called_once_with(
@@ -117,14 +148,23 @@
         self.cred.oauth2_refresh(self.refresh,
                                  url="somewhere")
         mock_refresh.assert_called_once_with(
             "somewhere",
             refresh_token=self.refresh,
             client_id=self.client_id, client_secret=self.client_secret)
 
+    @patch('requests_oauthlib.OAuth2Session.refresh_token', _raise_exception)
+    def testRefreshFail(self):
+        t = False
+        try:
+            self.cred.oauth2_refresh(self.refresh)
+        except mba.MbzOauth2Error:
+            t = True
+        self.assertTrue(t)
+
     @patch('requests_oauthlib.OAuth2Session.get')
     def testGet(self, mock_get):
         self.cred._oauth2_get("/request")
         mock_get.assert_called_once_with(
             mba.MUSICBRAINZ_OAUTH2 + "/request",
             params={}, headers=self.headers)
 
@@ -153,7 +193,52 @@
     def testGetWithHeaders(self, mock_get):
         headers = {"hd": "test"}
         self.cred._oauth2_get("/request", headers=headers)
         headers.update(self.headers)
         mock_get.assert_called_once_with(
             mba.MUSICBRAINZ_OAUTH2 + "/request",
             params={}, headers=headers)
+
+    @patch('requests_oauthlib.OAuth2Session.post')
+    def testPost(self, mock_post):
+        self.cred._oauth2_post("/request")
+        mock_post.assert_called_once_with(
+            mba.MUSICBRAINZ_OAUTH2 + "/request",
+            params={}, headers=self.headers, data=None)
+
+    @patch('requests_oauthlib.OAuth2Session.post')
+    def testPostAPIOther(self, mock_post):
+        self.cred._oauth2_post("/request", url="somewhere")
+        mock_post.assert_called_once_with(
+            "somewhere/request",
+            params={}, headers=self.headers, data=None)
+
+    @patch('requests_oauthlib.OAuth2Session.post')
+    def testPostAPIEmpty(self, mock_post):
+        self.cred._oauth2_post("/request", url="")
+        mock_post.assert_called_once_with(
+            "/request",
+            params={}, headers=self.headers, data=None)
+
+    @patch('requests_oauthlib.OAuth2Session.post')
+    def testPostWithPayload(self, mock_post):
+        self.cred._oauth2_post("/request", payload={"pl": "test"})
+        mock_post.assert_called_once_with(
+            mba.MUSICBRAINZ_OAUTH2 + "/request",
+            params={"pl": "test"}, headers=self.headers, data=None)
+
+    @patch('requests_oauthlib.OAuth2Session.post')
+    def testPostWithHeaders(self, mock_post):
+        headers = {"hd": "test"}
+        self.cred._oauth2_post("/request", headers=headers, data=None)
+        headers.update(self.headers, data=None)
+        mock_post.assert_called_once_with(
+            mba.MUSICBRAINZ_OAUTH2 + "/request",
+            params={}, headers=headers, data=None)
+
+    @patch('requests_oauthlib.OAuth2Session.post')
+    def testPostWithData(self, mock_post):
+        data = "this is data"
+        self.cred._oauth2_post("/request", headers=self.headers, data=data)
+        mock_post.assert_called_once_with(
+            mba.MUSICBRAINZ_OAUTH2 + "/request",
+            params={}, headers=self.headers, data=data)
```

### Comparing `mbzero-0.2/tests/test_caa.py` & `mbzero-0.3/tests/test_caa.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,19 @@
 from mbzero import caarequest as caa
 
 
 CAA_API = caa.CAA_API
 OTHER_API = "https://example.com"
 
 
+def _raise_exception(*args, **kwargs):
+    from requests import exceptions as rexc
+    raise rexc.RequestException
+
+
 @patch('requests.head')
 @patch('requests.get')
 class CaaTest(unittest.TestCase):
     def setUp(self):
         self.user_agent = "test_user_agent"
         self.headers = {"User-Agent": self.user_agent}
         self.payload = {"fmt": "json"}
@@ -67,20 +72,29 @@
                        "artist", "0383dadf-2a4e-4d10-a46a-e9e041da8eb3",
                        "front"
                        ).send()
         mock_get.assert_called_once_with(
             CAA_API + "/artist/0383dadf-2a4e-4d10-a46a-e9e041da8eb3/front",
             self.payload, headers=self.headers)
 
-    def testCaaHead(self, _, mock_head):
-        caa.CaaRequest(self.user_agent,
-                       "artist", "0383dadf-2a4e-4d10-a46a-e9e041da8eb3"
-                       ).send(head=True)
-        mock_head.assert_called_once_with(
-            CAA_API + "/artist/0383dadf-2a4e-4d10-a46a-e9e041da8eb3")
-
     def testCaaHeadAPIOther(self, _, mock_head):
         caa.CaaRequest(self.user_agent, "artist",
                        "0383dadf-2a4e-4d10-a46a-e9e041da8eb3"
                        ).send(head=True, opts={"url": OTHER_API})
         mock_head.assert_called_once_with(
             OTHER_API + "/artist/0383dadf-2a4e-4d10-a46a-e9e041da8eb3")
+
+
+class CaaTestException(unittest.TestCase):
+    def setUp(self):
+        self.user_agent = "test_user_agent"
+
+    @patch('requests.head', _raise_exception)
+    def testCaaHeadException(self):
+        t = False
+        try:
+            caa.CaaRequest(self.user_agent,
+                           "artist", "0383dadf-2a4e-4d10-a46a-e9e041da8eb3"
+                           ).send(head=True)
+        except caa.MbzRequestError:
+            t = True
+        self.assertTrue(t)
```

### Comparing `mbzero-0.2/tests/test_oauthrequests.py` & `mbzero-0.3/tests/test_oauthrequests.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,15 @@
         self.token = "token"
         self.refresh = "refresh"
         self.cred = mba.MbzCredentials()
         self.cred.oauth2_new(self.token, self.refresh,
                              client_id=self.client_id,
                              client_secret=self.client_secret)
         self.user_agent = "test_user_agent"
-        self.headers = {"User-Agent": self.user_agent,
-                        "Authorization": "Bearer %s" % self.token}
+        self.headers = {"User-Agent": self.user_agent}
         self.payload = {"fmt": "json"}
 
     @patch('requests_oauthlib.OAuth2Session.get')
     def testSend(self, mock_get):
         mock_get.return_value = RequestResultOK()
         mbr.MbzRequest(self.user_agent
                        ).get("/request",
```

### Comparing `mbzero-0.2/tests/test_requests.py` & `mbzero-0.3/tests/test_requests.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,20 +2,26 @@
 #
 #  SPDX-License-Identifier: BSD-2
 
 import unittest
 from unittest.mock import patch
 
 from mbzero import mbzrequest as mbr
+from mbzero import mbzauth as mba
 
 
 MUSICBRAINZ_API = mbr.MUSICBRAINZ_API
 OTHER_API = "https://example.com"
 
 
+def _raise_request_exception(*args, **kwargs):
+    from requests import exceptions
+    raise exceptions.RequestException("mock")
+
+
 @patch('requests.get')
 class RequestTest(unittest.TestCase):
     def setUp(self):
         self.user_agent = "test_user_agent"
         self.headers = {"User-Agent": self.user_agent}
         self.payload = {"fmt": "json"}
 
@@ -77,14 +83,25 @@
                              )
         req.set_url("")
         req.get("/request",
                 payload=self.payload, headers=self.headers)
         mock_get.assert_called_once_with(
             "/request", self.payload, headers=self.headers)
 
+    @patch('requests.auth.HTTPDigestAuth', return_value="auth")
+    def testSendCredentials(self, _, mock_get):
+        creds = mba.MbzCredentials()
+        creds.auth_set("name", "pass")
+        mbr.MbzRequest(self.user_agent
+                       ).get("/request", creds,
+                             payload=self.payload, headers=self.headers)
+        mock_get.assert_called_once_with(
+            MUSICBRAINZ_API + "/request", self.payload, headers=self.headers,
+            auth="auth")
+
 
 @patch('requests.get')
 class LookupTest(unittest.TestCase):
     def setUp(self):
         self.user_agent = "test_user_agent"
         self.headers = {"User-Agent": self.user_agent}
         self.payload = {"fmt": "json"}
@@ -346,7 +363,36 @@
 
     def testSearchFmtNone(self, mock_get):
         mbr.MbzRequestSearch(self.user_agent, "release", "QUERY"
                              ).send(opts={"fmt": None})
         mock_get.assert_called_once_with(
             MUSICBRAINZ_API + "/release?query=QUERY",
             self.payload, headers=self.headers)
+
+
+@patch('requests.get', _raise_request_exception)
+@patch('requests.post', _raise_request_exception)
+class RequestsExceptionTest(unittest.TestCase):
+    def setUp(self):
+        self.user_agent = "test_user_agent"
+        self.headers = {"User-Agent": self.user_agent}
+        self.payload = {"fmt": "json"}
+
+    def testSendException(self):
+        t = False
+        try:
+            mbr.MbzRequest(self.user_agent
+                           ).get("/request",
+                                 payload=self.payload, headers=self.headers)
+        except mbr.MbzRequestError:
+            t = True
+        self.assertTrue(t)
+
+    def testPostException(self):
+        t = False
+        try:
+            mbr.MbzSubmission(self.user_agent,
+                              "entity", self.payload, "xml"
+                              ).send(mba.MbzCredentials())
+        except mbr.MbzSubmissionError:
+            t = True
+        self.assertTrue(t)
```

### Comparing `mbzero-0.2/tests/test_submission.py` & `mbzero-0.3/tests/test_submission.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,16 +15,15 @@
 
 
 @patch('requests_oauthlib.OAuth2Session.post')
 class SubmissionTest(unittest.TestCase):
     def setUp(self):
         self.user_agent = "test_user_agent"
         self.client = "test_client"
-        self.headers = {"User-Agent": self.user_agent,
-                        "Authorization": "Bearer token"}
+        self.headers = {"User-Agent": self.user_agent}
         self.payload = {"fmt": "json"}
         self.data = "data"
         self.data_type = "xml"
         self.cred = mba.MbzCredentials()
         self.cred.oauth2_new("token", "refresh",
                              "client_id", "client_secret")
 
@@ -188,7 +187,32 @@
         try:
             mbr.MbzSubmission(self.user_agent, "request",
                               data="data", data_type="WRONG").send(
                                   credentials=self.cred)
         except Exception:
             pass
         mock_post.assert_not_called()
+
+    @patch('requests.auth.HTTPDigestAuth', return_value="auth")
+    @patch('requests.post')
+    def testSubmissionCredentials(self, mock_post, *_):
+        mbr.MbzSubmission(self.user_agent, "request",
+                          data="data", data_type="xml").send(
+                              mba.MbzCredentials())
+        headers = self.headers
+        headers["Content-Type"] = "application/xml; charset=utf-8"
+        payload = self.payload
+        payload["client"] = self.user_agent
+        mock_post.assert_called_once_with(
+            MUSICBRAINZ_API + "/request",
+            data=self.data,
+            params=self.payload, headers=self.headers, auth="auth")
+
+    def testSubmissionCredentialsNone(self, _):
+        t = False
+        try:
+            mbr.MbzSubmission(self.user_agent,
+                              "entity", self.payload, "xml",
+                              ).send()
+        except mbr.MbzSubmissionError:
+            t = True
+        self.assertTrue(t)
```

