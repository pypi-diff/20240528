# Comparing `tmp/perspective_parquet-0.1.1.tar.gz` & `tmp/perspective_parquet-0.1.2.tar.gz`

## Comparing `perspective_parquet-0.1.1.tar` & `perspective_parquet-0.1.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/.bumpversion.cfg
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/.gitattributes
--rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/CONTRIBUTING.md
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/MANIFEST.in
--rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/Makefile
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/setup.py
--rw-r--r--   0        0        0   125754 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/test.parquet
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/binder/postBuild
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/binder/requirements.txt
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/binder/runtime.txt
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/js/.prettierrc.json
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/js/build.js
--rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/js/package.json
--rw-r--r--   0        0        0   214280 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/js/yarn.lock
--rw-r--r--   0        0        0     7489 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/js/src/js/index.js
--rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/js/src/js/psp_widget.js
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/js/src/js/utils.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/js/src/less/index.less
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/perspective_parquet/__init__.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/perspective_parquet/extension/install.json
--rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/perspective_parquet/labextension/package.json
--rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/perspective_parquet/labextension/static/169.804c1a7cf0ea9dfd1210.js
--rw-r--r--   0        0        0  8132374 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/perspective_parquet/labextension/static/28.1968cb0312a1815497cb.js
--rw-r--r--   0        0        0     7114 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/perspective_parquet/labextension/static/remoteEntry.e7c57d2259396dc4d686.js
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/perspective_parquet/labextension/static/style.js
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/perspective_parquet/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/perspective_parquet/tests/test_all.py
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/LICENSE
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/README.md
--rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    15160 2020-02-02 00:00:00.000000 perspective_parquet-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 perspective_parquet-0.1.2/.bumpversion.cfg
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 perspective_parquet-0.1.2/.gitattributes
+-rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 perspective_parquet-0.1.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 perspective_parquet-0.1.2/MANIFEST.in
+-rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 perspective_parquet-0.1.2/Makefile
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 perspective_parquet-0.1.2/setup.py
+-rw-r--r--   0        0        0   125754 2020-02-02 00:00:00.000000 perspective_parquet-0.1.2/test.parquet
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 perspective_parquet-0.1.2/binder/postBuild
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 perspective_parquet-0.1.2/binder/requirements.txt
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 perspective_parquet-0.1.2/binder/runtime.txt
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 perspective_parquet-0.1.2/js/.prettierrc.json
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 perspective_parquet-0.1.2/js/build.js
+-rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 perspective_parquet-0.1.2/js/package.json
+-rw-r--r--   0        0        0   214278 2020-02-02 00:00:00.000000 perspective_parquet-0.1.2/js/yarn.lock
+-rw-r--r--   0        0        0     7489 2020-02-02 00:00:00.000000 perspective_parquet-0.1.2/js/src/js/index.js
+-rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 perspective_parquet-0.1.2/js/src/js/psp_widget.js
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 perspective_parquet-0.1.2/js/src/js/utils.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 perspective_parquet-0.1.2/js/src/less/index.less
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 perspective_parquet-0.1.2/perspective_parquet/__init__.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 perspective_parquet-0.1.2/perspective_parquet/extension/install.json
+-rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 perspective_parquet-0.1.2/perspective_parquet/labextension/package.json
+-rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 perspective_parquet-0.1.2/perspective_parquet/labextension/static/169.804c1a7cf0ea9dfd1210.js
+-rw-r--r--   0        0        0  8132374 2020-02-02 00:00:00.000000 perspective_parquet-0.1.2/perspective_parquet/labextension/static/28.d192144fd1a9d7249be1.js
+-rw-r--r--   0        0        0     7114 2020-02-02 00:00:00.000000 perspective_parquet-0.1.2/perspective_parquet/labextension/static/remoteEntry.eea45df6b9a9af71d0e1.js
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 perspective_parquet-0.1.2/perspective_parquet/labextension/static/style.js
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 perspective_parquet-0.1.2/perspective_parquet/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 perspective_parquet-0.1.2/perspective_parquet/tests/test_all.py
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 perspective_parquet-0.1.2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 perspective_parquet-0.1.2/LICENSE
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 perspective_parquet-0.1.2/README.md
+-rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 perspective_parquet-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    15166 2020-02-02 00:00:00.000000 perspective_parquet-0.1.2/PKG-INFO
```

### Comparing `perspective_parquet-0.1.1/.bumpversion.cfg` & `perspective_parquet-0.1.2/.bumpversion.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.1
+current_version = 0.1.2
 commit = True
 tag = False
 
 [bumpversion:file:perspective_parquet/__init__.py]
 search = __version__ = "{current_version}"
 replace = __version__ = "{new_version}"
```

### Comparing `perspective_parquet-0.1.1/CONTRIBUTING.md` & `perspective_parquet-0.1.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `perspective_parquet-0.1.1/MANIFEST.in` & `perspective_parquet-0.1.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `perspective_parquet-0.1.1/Makefile` & `perspective_parquet-0.1.2/Makefile`

 * *Files identical despite different names*

### Comparing `perspective_parquet-0.1.1/test.parquet` & `perspective_parquet-0.1.2/test.parquet`

 * *Files identical despite different names*

### Comparing `perspective_parquet-0.1.1/js/build.js` & `perspective_parquet-0.1.2/js/build.js`

 * *Files identical despite different names*

### Comparing `perspective_parquet-0.1.1/js/package.json` & `perspective_parquet-0.1.2/js/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.1.2'"}*

```diff
@@ -59,9 +59,9 @@
         "clean:labextension": "rimraf ../perspective_parquet/labextension",
         "clean:lib": "rimraf lib",
         "fix": "prettier --write  \"src/js/*.js\" \"src/less/*.less\" \"*.js\" \"*.json\"",
         "lint": "prettier --check \"src/js/*.js\" \"src/less/*.less\" \"*.js\" \"*.json\"",
         "test": ":"
     },
     "style": "dist/umd/perspective-parquet.css",
-    "version": "0.1.1"
+    "version": "0.1.2"
 }
```

### Comparing `perspective_parquet-0.1.1/js/yarn.lock` & `perspective_parquet-0.1.2/js/yarn.lock`

 * *Files 1% similar despite different names*

```diff
@@ -3290,18 +3290,18 @@
 minipass@^3.0.0, minipass@^3.1.1:
   version "3.3.6"
   resolved "https://registry.yarnpkg.com/minipass/-/minipass-3.3.6.tgz#7bba384db3a1520d18c9c0e5251c3444e95dd94a"
   integrity sha512-DxiNidxSEK+tHG6zOIklvNOwm3hvCrbUrdtzY74U6HKTJxvIDfOUL5W5P2Ghd3DTkhhKPYGqeNUIh5qcM4YBfw==
   dependencies:
     yallist "^4.0.0"
 
-minipass@^4.0.0:
-  version "4.2.8"
-  resolved "https://registry.yarnpkg.com/minipass/-/minipass-4.2.8.tgz#f0010f64393ecfc1d1ccb5f582bcaf45f48e1a3a"
-  integrity sha512-fNzuVyifolSLFL4NzpF+wEF4qrgqaaKX0haXPQEdQ7NKAN+WecoKMHV09YcuL/DHxrUsYQOK3MiuDf7Ip2OXfQ==
+minipass@^5.0.0:
+  version "5.0.0"
+  resolved "https://registry.yarnpkg.com/minipass/-/minipass-5.0.0.tgz#3e9788ffb90b694a5d0ec94479a45b5d8738133d"
+  integrity sha512-3FnjYuehv9k6ovOEbyOswadCDPX1piCfhV8ncmYtHOjuPwylVWsghTLo7rabjC3Rx5xD4HDx8Wm1xnMF7S5qFQ==
 
 minizlib@^2.1.1:
   version "2.1.2"
   resolved "https://registry.yarnpkg.com/minizlib/-/minizlib-2.1.2.tgz#e90d3466ba209b932451508a11ce3d3632145931"
   integrity sha512-bAxsR8BVfj60DWXHE3u30oHzfl4G7khkSuPW+qvpd7jFRHm7dLxOjUk1EHACJ/hxLY8phGJ0YhYHZo7jil7Qdg==
   dependencies:
     minipass "^3.0.0"
@@ -3671,17 +3671,17 @@
 
 postcss-value-parser@^4.1.0:
   version "4.2.0"
   resolved "https://registry.yarnpkg.com/postcss-value-parser/-/postcss-value-parser-4.2.0.tgz#723c09920836ba6d3e5af019f92bc0971c02e514"
   integrity sha512-1NNCs6uurfkVbeXG4S8JFT9t19m45ICnif8zWLd5oPSZ50QnwMfK+H3jv408d4jw/7Bttv5axS5IiHoLaVNHeQ==
 
 postcss@^8.2.15, postcss@^8.3.11:
-  version "8.4.23"
-  resolved "https://registry.yarnpkg.com/postcss/-/postcss-8.4.23.tgz#df0aee9ac7c5e53e1075c24a3613496f9e6552ab"
-  integrity sha512-bQ3qMcpF6A/YjR55xtoTr0jGOlnPOKAIMdOWiv0EIT6HVPEaJiJB4NLljSbiHoC2RX7DN5Uvjtpbg1NPdwv1oA==
+  version "8.4.31"
+  resolved "https://registry.yarnpkg.com/postcss/-/postcss-8.4.31.tgz#92b451050a9f914da6755af352bdc0192508656d"
+  integrity sha512-PS08Iboia9mts/2ygV3eLpY5ghnUcfLV/EXTOW1E2qYxJKGGBUtNjN76FYHnMs36RmARn41bC0AZmn+rR0OVpQ==
   dependencies:
     nanoid "^3.3.6"
     picocolors "^1.0.0"
     source-map-js "^1.0.2"
 
 prettier@^2.8.8:
   version "2.8.8"
@@ -3984,27 +3984,27 @@
   integrity sha512-pvjEHOgWc9OWA/f/DE3ohBWTD6EleVLf7iFUkoSwAxttdBhB9QUebQgxER2kWueOvRJXPHNnyrvvh9eZINB8Eg==
   dependencies:
     "@types/json-schema" "^7.0.8"
     ajv "^6.12.5"
     ajv-keywords "^3.5.2"
 
 "semver@2 || 3 || 4 || 5", semver@^5.4.1, semver@^5.5.0, semver@^5.6.0:
-  version "5.7.1"
-  resolved "https://registry.yarnpkg.com/semver/-/semver-5.7.1.tgz#a954f931aeba508d307bbf069eff0c01c96116f7"
-  integrity sha512-sauaDf/PZdVgrLTNYHRtpXa1iRiKcaebiKQ1BJdpQlWH2lCvexQdX55snPFyK7QzpudqbCI0qXFfOasHdyNDGQ==
+  version "5.7.2"
+  resolved "https://registry.yarnpkg.com/semver/-/semver-5.7.2.tgz#48d55db737c3287cd4835e17fa13feace1c41ef8"
+  integrity sha512-cBznnQ9KjJqU67B52RMC65CMarK2600WFnbkcaiwWq3xy/5haFJlshgnpjovMVJ+Hff49d8GEn0b87C5pDQ10g==
 
 semver@^6.0.0:
-  version "6.3.0"
-  resolved "https://registry.yarnpkg.com/semver/-/semver-6.3.0.tgz#ee0a64c8af5e8ceea67687b133761e1becbd1d3d"
-  integrity sha512-b39TBaTSfV6yBrapU89p5fKekE2m/NwnDocOVruQFS1/veMgdzuPcnOM34M6CwxW8jH/lxEa5rBoDeUwu5HHTw==
+  version "6.3.1"
+  resolved "https://registry.yarnpkg.com/semver/-/semver-6.3.1.tgz#556d2ef8689146e46dcea4bfdd095f3434dffcb4"
+  integrity sha512-BR7VvDCVHO+q2xBEWskxS6DJE1qRnb7DxzUrogb71CWoSficBxYsiAGd+Kl0mmq/MprG9yArRkyrQxTO6XjMzA==
 
 semver@^7.3.5:
-  version "7.5.0"
-  resolved "https://registry.yarnpkg.com/semver/-/semver-7.5.0.tgz#ed8c5dc8efb6c629c88b23d41dc9bf40c1d96cd0"
-  integrity sha512-+XC0AD/R7Q2mPSRuy2Id0+CGTZ98+8f+KvwirxOKIEyid+XSx6HbC63p+O4IndTHuX5Z+JxQ0TghCkO5Cg/2HA==
+  version "7.5.4"
+  resolved "https://registry.yarnpkg.com/semver/-/semver-7.5.4.tgz#483986ec4ed38e1c6c48c34894a9182dbff68a6e"
+  integrity sha512-1bCSESV6Pv+i21Hvpxp3Dx+pSD8lIPt8uVjRrxAUt/nbswYc+tK6Y2btiULjd4+fnq15PX+nqQDC7Oft7WkwcA==
   dependencies:
     lru-cache "^6.0.0"
 
 serialize-javascript@^5.0.1:
   version "5.0.1"
   resolved "https://registry.yarnpkg.com/serialize-javascript/-/serialize-javascript-5.0.1.tgz#7886ec848049a462467a97d3d918ebb2aaf934f4"
   integrity sha512-SaaNal9imEO737H2c05Og0/8LUXG7EnsZyMa8MzkmuHoELfT6txuj0cMqRj6zfPKnmQ1yasR4PCJc8x+M4JSPA==
@@ -4227,21 +4227,21 @@
 
 tapable@^2.1.1, tapable@^2.2.0:
   version "2.2.1"
   resolved "https://registry.yarnpkg.com/tapable/-/tapable-2.2.1.tgz#1967a73ef4060a82f12ab96af86d52fdb76eeca0"
   integrity sha512-GNzQvQTOIP6RyTfE2Qxb8ZVlNmw0n88vp1szwWRimP02mnTsx3Wtn5qRdqY9w2XduFNUgvOwhNnQsjwCp+kqaQ==
 
 tar@^6.0.2, tar@^6.1.11:
-  version "6.1.13"
-  resolved "https://registry.yarnpkg.com/tar/-/tar-6.1.13.tgz#46e22529000f612180601a6fe0680e7da508847b"
-  integrity sha512-jdIBIN6LTIe2jqzay/2vtYLlBHa3JF42ot3h1dW8Q0PaAG4v8rm0cvpVePtau5C6OKXGGcgO9q2AMNSWxiLqKw==
+  version "6.2.1"
+  resolved "https://registry.yarnpkg.com/tar/-/tar-6.2.1.tgz#717549c541bc3c2af15751bea94b1dd068d4b03a"
+  integrity sha512-DZ4yORTwrbTj/7MZYq2w+/ZFdI6OZ/f9SFHR+71gIVUZhOQPHzVCLpvRnPgyaMpfWxxk/4ONva3GQSyNIKRv6A==
   dependencies:
     chownr "^2.0.0"
     fs-minipass "^2.0.0"
-    minipass "^4.0.0"
+    minipass "^5.0.0"
     minizlib "^2.1.1"
     mkdirp "^1.0.3"
     yallist "^4.0.0"
 
 terser-webpack-plugin@^4.1.0:
   version "4.2.3"
   resolved "https://registry.yarnpkg.com/terser-webpack-plugin/-/terser-webpack-plugin-4.2.3.tgz#28daef4a83bd17c1db0297070adc07fc8cfc6a9a"
```

### Comparing `perspective_parquet-0.1.1/js/src/js/index.js` & `perspective_parquet-0.1.2/js/src/js/index.js`

 * *Files identical despite different names*

### Comparing `perspective_parquet-0.1.1/js/src/js/psp_widget.js` & `perspective_parquet-0.1.2/js/src/js/psp_widget.js`

 * *Files identical despite different names*

### Comparing `perspective_parquet-0.1.1/perspective_parquet/labextension/package.json` & `perspective_parquet-0.1.2/perspective_parquet/labextension/package.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9608974358974359%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.eea45df6b9a9af71d0e1.js'}}",*

 * * "'version'": "'0.1.2'"}*

```diff
@@ -23,15 +23,15 @@
     "files": [
         "dist/**/*",
         "src/**/*"
     ],
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.e7c57d2259396dc4d686.js",
+            "load": "static/remoteEntry.eea45df6b9a9af71d0e1.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "perspective-python"
                 },
@@ -64,9 +64,9 @@
         "clean:labextension": "rimraf ../perspective_parquet/labextension",
         "clean:lib": "rimraf lib",
         "fix": "prettier --write  \"src/js/*.js\" \"src/less/*.less\" \"*.js\" \"*.json\"",
         "lint": "prettier --check \"src/js/*.js\" \"src/less/*.less\" \"*.js\" \"*.json\"",
         "test": ":"
     },
     "style": "dist/umd/perspective-parquet.css",
-    "version": "0.1.1"
+    "version": "0.1.2"
 }
```

### Comparing `perspective_parquet-0.1.1/perspective_parquet/labextension/static/169.804c1a7cf0ea9dfd1210.js` & `perspective_parquet-0.1.2/perspective_parquet/labextension/static/169.804c1a7cf0ea9dfd1210.js`

 * *Files identical despite different names*

### Comparing `perspective_parquet-0.1.1/perspective_parquet/labextension/static/28.1968cb0312a1815497cb.js` & `perspective_parquet-0.1.2/perspective_parquet/labextension/static/28.d192144fd1a9d7249be1.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -4,18 +4,18 @@
         28: (A, I, g) => {
             g.r(I), g.d(I, {
                 PerspectiveDocumentWidget: () => BI,
                 PerspectiveParquetFactory: () => QI,
                 PerspectiveRenderers: () => CI,
                 default: () => EI
             });
-            var B = g(142),
-                Q = g(687),
-                C = g(33),
-                E = g(819),
+            var B = g(46),
+                Q = g(271),
+                C = g(583),
+                E = g(413),
                 D = g(832),
                 i = Object.defineProperty,
                 G = (A, I) => {
                     for (var g in I) i(A, g, {
                         get: I[g],
                         enumerable: !0
                     })
```

### Comparing `perspective_parquet-0.1.1/perspective_parquet/labextension/static/remoteEntry.e7c57d2259396dc4d686.js` & `perspective_parquet-0.1.2/perspective_parquet/labextension/static/remoteEntry.eea45df6b9a9af71d0e1.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, u, l, s, f, p, d, c, v, h, g, b, m, y, w, S, j = {
+    var e, r, t, n, o, a, i, u, l, s, p, f, c, d, v, h, b, g, m, y, w, S, j = {
             566: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(28).then((() => () => t(28))),
                         "./extension": () => t.e(28).then((() => () => t(28))),
                         "./style": () => t.e(169).then((() => () => t(169)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
@@ -43,49 +43,49 @@
         }), r
     }, k.d = (e, r) => {
         for (var t in r) k.o(r, t) && !k.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, k.f = {}, k.e = e => Promise.all(Object.keys(k.f).reduce(((r, t) => (k.f[t](e, r), r)), [])), k.u = e => e + "." + {
-        28: "1968cb0312a1815497cb",
+        28: "d192144fd1a9d7249be1",
         169: "804c1a7cf0ea9dfd1210"
     } [e] + ".js?v=" + {
-        28: "1968cb0312a1815497cb",
+        28: "d192144fd1a9d7249be1",
         169: "804c1a7cf0ea9dfd1210"
     } [e], k.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), k.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "perspective-parquet:", k.l = (t, n, o, a) => {
         if (e[t]) e[t].push(n);
         else {
             var i, u;
             if (void 0 !== o)
                 for (var l = document.getElementsByTagName("script"), s = 0; s < l.length; s++) {
-                    var f = l[s];
-                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + o) {
-                        i = f;
+                    var p = l[s];
+                    if (p.getAttribute("src") == t || p.getAttribute("data-webpack") == r + o) {
+                        i = p;
                         break
                     }
                 }
             i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, k.nc && i.setAttribute("nonce", k.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
-            var p = (r, n) => {
-                    i.onerror = i.onload = null, clearTimeout(d);
+            var f = (r, n) => {
+                    i.onerror = i.onload = null, clearTimeout(c);
                     var o = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                d = setTimeout(p.bind(null, void 0, {
+                c = setTimeout(f.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = p.bind(null, i.onerror), i.onload = p.bind(null, i.onload), u && document.head.appendChild(i)
+            i.onerror = f.bind(null, i.onerror), i.onload = f.bind(null, i.onload), u && document.head.appendChild(i)
         }
     }, k.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -106,15 +106,15 @@
                     var o = a[e] = a[e] || {},
                         u = o[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
                         get: () => k.e(28).then((() => () => k(28))),
                         from: i,
                         eager: !1
                     })
-                })("perspective-parquet", "0.1.1"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("perspective-parquet", "0.1.2"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         k.g.importScripts && (e = k.g.location + "");
         var r = k.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -164,76 +164,76 @@
     }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 o = n < 0;
             o && (n = -n - 1);
             for (var i = 0, u = 1, l = !0;; u++, i++) {
-                var s, f, p = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (f = (typeof(s = r[i]))[0])) return !l || ("u" == p ? u > n && !o : "" == p != o);
-                if ("u" == f) {
-                    if (!l || "u" != p) return !1
+                var s, p, f = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (p = (typeof(s = r[i]))[0])) return !l || ("u" == f ? u > n && !o : "" == f != o);
+                if ("u" == p) {
+                    if (!l || "u" != f) return !1
                 } else if (l)
-                    if (p == f)
+                    if (f == p)
                         if (u <= n) {
                             if (s != e[u]) return !1
                         } else {
                             if (o ? s > e[u] : s < e[u]) return !1;
                             s != e[u] && (l = !1)
                         }
-                else if ("s" != p && "n" != p) {
+                else if ("s" != f && "n" != f) {
                     if (o || u <= n) return !1;
                     l = !1, u--
                 } else {
-                    if (u <= n || f < p != o) return !1;
+                    if (u <= n || p < f != o) return !1;
                     l = !1
-                } else "s" != p && "n" != p && (l = !1, u--)
+                } else "s" != f && "n" != f && (l = !1, u--)
             }
         }
-        var d = [],
-            c = d.pop.bind(d);
+        var c = [],
+            d = c.pop.bind(c);
         for (i = 1; i < e.length; i++) {
             var v = e[i];
-            d.push(1 == v ? c() | c() : 2 == v ? c() & c() : v ? a(v, r) : !c())
+            c.push(1 == v ? d() | d() : 2 == v ? d() & d() : v ? a(v, r) : !d())
         }
-        return !!c()
+        return !!d()
     }, i = (e, r) => {
         var t = k.S[e];
         if (!t || !k.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return (r = Object.keys(t).reduce(((e, r) => !e || n(e, r) ? r : e), 0)) && t[r]
     }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, s = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", f = (e, r, t, n) => {
+    }, s = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", p = (e, r, t, n) => {
         var o = l(e, t);
-        return a(n, o) || c(s(e, t, o, n)), h(e[t][o])
-    }, p = (e, r, t) => {
+        return a(n, o) || d(s(e, t, o, n)), h(e[t][o])
+    }, f = (e, r, t) => {
         var o = e[r];
         return (r = Object.keys(o).reduce(((e, r) => !a(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
-    }, d = (e, r, t, n) => {
+    }, c = (e, r, t, n) => {
         var a = e[t];
         return "No satisfying version (" + o(n) + ") of shared module " + t + " found in shared scope " + r + ".\nAvailable versions: " + Object.keys(a).map((e => e + " from " + a[e].from)).join(", ")
-    }, c = e => {
+    }, d = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, v = (e, r, t, n) => {
-        c(d(e, r, t, n))
-    }, h = e => (e.loaded = 1, e.get()), b = (g = e => function(r, t, n, o) {
+        d(c(e, r, t, n))
+    }, h = e => (e.loaded = 1, e.get()), g = (b = e => function(r, t, n, o) {
         var a = k.I(r);
         return a && a.then ? a.then(e.bind(e, r, k.S[r], t, n, o)) : e(r, k.S[r], t, n, o)
-    })(((e, r, t, n) => (i(e, t), h(p(r, t, n) || v(r, e, t, n) || u(r, t))))), m = g(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), y = {}, w = {
-        33: () => m("default", "@jupyterlab/apputils", [1, 3, 6, 3]),
-        142: () => m("default", "@jupyterlab/coreutils", [1, 5, 6, 3]),
-        687: () => m("default", "@jupyterlab/application", [1, 3, 6, 3]),
-        819: () => b("default", "@jupyterlab/docregistry", [1, 3, 6, 3]),
+    })(((e, r, t, n) => (i(e, t), h(f(r, t, n) || v(r, e, t, n) || u(r, t))))), m = b(((e, r, t, n) => (i(e, t), p(r, 0, t, n)))), y = {}, w = {
+        46: () => m("default", "@jupyterlab/coreutils", [1, 5, 6, 7]),
+        271: () => m("default", "@jupyterlab/application", [1, 3, 6, 7]),
+        413: () => g("default", "@jupyterlab/docregistry", [1, 3, 6, 7]),
+        583: () => m("default", "@jupyterlab/apputils", [1, 3, 6, 7]),
         832: () => m("default", "@lumino/widgets", [1, 1, 37, 2])
     }, S = {
-        28: [33, 142, 687, 819, 832]
+        28: [46, 271, 413, 583, 832]
     }, k.f.consumes = (e, r) => {
         k.o(S, e) && S[e].forEach((e => {
             if (k.o(y, e)) return r.push(y[e]);
             var t = r => {
                     y[e] = 0, k.m[e] = t => {
                         delete k.c[e], t.exports = r()
                     }
```

### Comparing `perspective_parquet-0.1.1/perspective_parquet/labextension/static/third-party-licenses.json` & `perspective_parquet-0.1.2/perspective_parquet/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `perspective_parquet-0.1.1/.gitignore` & `perspective_parquet-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `perspective_parquet-0.1.1/LICENSE` & `perspective_parquet-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `perspective_parquet-0.1.1/README.md` & `perspective_parquet-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `perspective_parquet-0.1.1/pyproject.toml` & `perspective_parquet-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     "jupyterlab>=3.5,<4",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "perspective-parquet"
 description = "Parquet viewer for perspective in JupyterLab"
-version = "0.1.1"
+version = "0.1.2"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
 authors = [
     { name = "Tim Paine", email = "t.paine154@gmail.com" },
 ]
 keywords = [
@@ -31,15 +31,15 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "License :: OSI Approved :: Apache Software License",
 ]
 dependencies = [
-    "perspective-python",
+    "perspective-python>=2,<3",
 ]
 
 [project.optional-dependencies]
 develop = [
     "black>=23",
     "check-manifest",
     "ruff",
```

### Comparing `perspective_parquet-0.1.1/PKG-INFO` & `perspective_parquet-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: perspective-parquet
-Version: 0.1.1
+Version: 0.1.2
 Summary: Parquet viewer for perspective in JupyterLab
 Project-URL: repository, https://github.com/timkpaine/perspective-parquet
 Project-URL: homepage, https://github.com/timkpaine/perspective-parquet
 Author-email: Tim Paine <t.paine154@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -215,15 +215,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
-Requires-Dist: perspective-python
+Requires-Dist: perspective-python<3,>=2
 Provides-Extra: develop
 Requires-Dist: black>=23; extra == 'develop'
 Requires-Dist: check-manifest; extra == 'develop'
 Requires-Dist: pytest; extra == 'develop'
 Requires-Dist: pytest-cov; extra == 'develop'
 Requires-Dist: ruff; extra == 'develop'
 Provides-Extra: test
```

