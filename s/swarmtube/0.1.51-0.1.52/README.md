# Comparing `tmp/swarmtube-0.1.51-py2.py3-none-any.whl.zip` & `tmp/swarmtube-0.1.52-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 50655 bytes, number of entries: 48
--rw-rw-r--  2.0 unx     1683 b- defN 24-May-28 06:14 swarmtube/__init__.py
+Zip file size: 50676 bytes, number of entries: 48
+-rw-rw-r--  2.0 unx     1683 b- defN 24-May-28 09:43 swarmtube/__init__.py
 -rw-rw-r--  2.0 unx      665 b- defN 24-May-04 08:01 swarmtube/definitions.py
 -rw-rw-r--  2.0 unx     6691 b- defN 24-May-02 16:20 swarmtube/swarmtube.py
 -rw-rw-r--  2.0 unx     1780 b- defN 24-May-02 16:20 swarmtube/cli/__init__.py
 -rw-rw-r--  2.0 unx     3834 b- defN 24-May-02 16:20 swarmtube/cli/config.py
 -rw-rw-r--  2.0 unx     2279 b- defN 24-May-02 16:20 swarmtube/cli/inventory.py
 -rw-rw-r--  2.0 unx     1577 b- defN 24-May-02 16:20 swarmtube/cli/main.py
 -rw-rw-r--  2.0 unx     1800 b- defN 24-May-02 16:20 swarmtube/cli/publish.py
@@ -31,20 +31,20 @@
 -rw-rw-r--  2.0 unx     1887 b- defN 24-May-02 16:20 swarmtube/models/config.py
 -rw-rw-r--  2.0 unx       34 b- defN 24-May-02 16:20 swarmtube/models/enums.py
 -rw-rw-r--  2.0 unx     1886 b- defN 24-May-02 16:20 swarmtube/models/inventory.py
 -rw-rw-r--  2.0 unx     1675 b- defN 24-May-02 16:20 swarmtube/models/script.py
 -rw-rw-r--  2.0 unx     1907 b- defN 24-May-02 16:20 swarmtube/models/swarmtube.py
 -rw-rw-r--  2.0 unx     1649 b- defN 24-May-02 16:20 swarmtube/models/task.py
 -rw-rw-r--  2.0 unx        0 b- defN 24-May-19 06:38 swarmtube/particles/__init__.py
--rw-rw-r--  2.0 unx    10269 b- defN 24-May-27 21:15 swarmtube/particles/fiware.py
+-rw-rw-r--  2.0 unx    10352 b- defN 24-May-28 09:19 swarmtube/particles/fiware.py
 -rw-rw-r--  2.0 unx      555 b- defN 24-May-02 16:20 swarmtube/ports/__init__.py
 -rw-rw-r--  2.0 unx     1389 b- defN 24-May-02 16:20 swarmtube/ports/preferences.py
 -rw-rw-r--  2.0 unx      182 b- defN 24-May-02 16:20 swarmtube/storage/__init__.py
 -rw-rw-r--  2.0 unx     1330 b- defN 24-May-02 16:20 swarmtube/storage/surreal.py
--rw-rw-r--  2.0 unx      168 b- defN 24-May-28 06:21 swarmtube-0.1.51.dist-info/AUTHORS.rst
--rw-rw-r--  2.0 unx     1075 b- defN 24-May-28 06:21 swarmtube-0.1.51.dist-info/LICENSE
--rw-rw-r--  2.0 unx     2201 b- defN 24-May-28 06:21 swarmtube-0.1.51.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 24-May-28 06:21 swarmtube-0.1.51.dist-info/WHEEL
--rw-rw-r--  2.0 unx       49 b- defN 24-May-28 06:21 swarmtube-0.1.51.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       10 b- defN 24-May-28 06:21 swarmtube-0.1.51.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     3986 b- defN 24-May-28 06:21 swarmtube-0.1.51.dist-info/RECORD
-48 files, 137559 bytes uncompressed, 44337 bytes compressed:  67.8%
+-rw-rw-r--  2.0 unx      168 b- defN 24-May-28 09:45 swarmtube-0.1.52.dist-info/AUTHORS.rst
+-rw-rw-r--  2.0 unx     1075 b- defN 24-May-28 09:45 swarmtube-0.1.52.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     2201 b- defN 24-May-28 09:45 swarmtube-0.1.52.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 24-May-28 09:45 swarmtube-0.1.52.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       49 b- defN 24-May-28 09:45 swarmtube-0.1.52.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       10 b- defN 24-May-28 09:45 swarmtube-0.1.52.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     3986 b- defN 24-May-28 09:45 swarmtube-0.1.52.dist-info/RECORD
+48 files, 137642 bytes uncompressed, 44358 bytes compressed:  67.8%
```

## zipnote {}

```diff
@@ -117,29 +117,29 @@
 
 Filename: swarmtube/storage/__init__.py
 Comment: 
 
 Filename: swarmtube/storage/surreal.py
 Comment: 
 
-Filename: swarmtube-0.1.51.dist-info/AUTHORS.rst
+Filename: swarmtube-0.1.52.dist-info/AUTHORS.rst
 Comment: 
 
-Filename: swarmtube-0.1.51.dist-info/LICENSE
+Filename: swarmtube-0.1.52.dist-info/LICENSE
 Comment: 
 
-Filename: swarmtube-0.1.51.dist-info/METADATA
+Filename: swarmtube-0.1.52.dist-info/METADATA
 Comment: 
 
-Filename: swarmtube-0.1.51.dist-info/WHEEL
+Filename: swarmtube-0.1.52.dist-info/WHEEL
 Comment: 
 
-Filename: swarmtube-0.1.51.dist-info/entry_points.txt
+Filename: swarmtube-0.1.52.dist-info/entry_points.txt
 Comment: 
 
-Filename: swarmtube-0.1.51.dist-info/top_level.txt
+Filename: swarmtube-0.1.52.dist-info/top_level.txt
 Comment: 
 
-Filename: swarmtube-0.1.51.dist-info/RECORD
+Filename: swarmtube-0.1.52.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## swarmtube/__init__.py

```diff
@@ -29,8 +29,8 @@
 11. [ ] define test cases (tests/*.py) and get main
 12. [ ] implement automatic test cases
 
 """
 
 __author__ = """Asterio Gonzalez"""
 __email__ = "asterio.gonzalez@gmail.com"
-__version__ = "0.1.51"
+__version__ = "0.1.52"
```

## swarmtube/particles/fiware.py

```diff
@@ -188,14 +188,15 @@
 
         """
         for tries in range(1, 15):
             try:
                 async with aiohttp.ClientSession() as session:
                     # log.info(f"{self.app_url}{path}: {query_data}")
                     async with session.post(
+                        # TODO: fiware-servicepath is based on data item + headers
                         self.target_url, data=data, headers=self.HEADERS
                     ) as response:
                         if response.status < 300:
                             # result = await response.json()
                             # meta = result["meta"]
                             # stream = result["result"]
```

## Comparing `swarmtube-0.1.51.dist-info/LICENSE` & `swarmtube-0.1.52.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `swarmtube-0.1.51.dist-info/METADATA` & `swarmtube-0.1.52.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarmtube
-Version: 0.1.51
+Version: 0.1.52
 Summary: Swarm Workflow based on Tubes
 Home-page: https://github.com/asterio.gonzalez/swarmtube
 Author: Asterio Gonzalez
 Author-email: asterio.gonzalez@gmail.com
 License: MIT license
 Keywords: swarmtube
 Classifier: Development Status :: 2 - Pre-Alpha
```

## Comparing `swarmtube-0.1.51.dist-info/RECORD` & `swarmtube-0.1.52.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-swarmtube/__init__.py,sha256=l7BLsLZwoe2z6JXDi2Doy7pSP9PuD5ZtArI1eSiLxqA,1683
+swarmtube/__init__.py,sha256=1xldowtB9iIKwJz9ywB9l3LEFAUsZQuL7yILkaW07YM,1683
 swarmtube/definitions.py,sha256=aU08kgwbLPmUwZKdMYAAWNSNl5ZBIk70pkkx0VjKzlI,665
 swarmtube/swarmtube.py,sha256=uktSYYLbcB6wLd3SH6n_7MsZULi4xXl3tljJ1sCj7Js,6691
 swarmtube/cli/__init__.py,sha256=vn0EccAVZb4LjRugK__sLjr4OHBrPV8tK-ScyYSoQpc,1780
 swarmtube/cli/config.py,sha256=3oW1q326XFGlLABSZLqT-NSu3j27rhkAyXqcypBUO7Q,3834
 swarmtube/cli/inventory.py,sha256=Vnjc4uKeOspYyX5-GOvFx04F96lbzLTtla0ba33j2zY,2279
 swarmtube/cli/main.py,sha256=D7OxrEy-fy7N85CwdWOH81We37MTk2PgBrtuU_ClR28,1577
 swarmtube/cli/publish.py,sha256=JhZWxYagMQrIRgFtlaTE9XJ8saXFkhMqnFIPFAeIxwo,1800
@@ -30,19 +30,19 @@
 swarmtube/models/config.py,sha256=cMhlQzCgo0N9qBMRQEPbBj1UxAC_OZc_PNLeNSoGV2M,1887
 swarmtube/models/enums.py,sha256=QxW9YtWOVokO3gXjELfE52paN_ZUNnXhs1HBtTpvZFE,34
 swarmtube/models/inventory.py,sha256=-18lewwVXVrRlq7CfALqKiNjVdwSoKCdRX-KtN2_uD0,1886
 swarmtube/models/script.py,sha256=pwCxOht-OXeysa8c0D9M6OyUdSDe7UaHiCVxSdOVU0M,1675
 swarmtube/models/swarmtube.py,sha256=dACX0MkqchNveuuoxGyYzKvIL6zTKKBYeSmxp_41OKc,1907
 swarmtube/models/task.py,sha256=ygyl1Fd8MI_x8S4KSFo50o3_YaE5n7F9kx4390T-ItU,1649
 swarmtube/particles/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-swarmtube/particles/fiware.py,sha256=gilNK-9Im4WJ6LNYplUJfsiO1lPeuy-LVhsn7pyfW1Y,10269
+swarmtube/particles/fiware.py,sha256=EoTk5jGWAP-ovLDFNu5CUyoCfD1maQGaxltucbbp87c,10352
 swarmtube/ports/__init__.py,sha256=DUg8Upo_F0Y8LxfTqh1Q8IYSChmGSp1ZlZqwI-NXdag,555
 swarmtube/ports/preferences.py,sha256=RrSG1IrHu0_eiFVr9-LhFckPHDj7RcEVQTTDhJKO_uk,1389
 swarmtube/storage/__init__.py,sha256=CSNhFbyDpDg_fxHHw9x2GcOdx8qXZTw50_cKxKgtJ4g,182
 swarmtube/storage/surreal.py,sha256=QTEikrYghbv8nyKjc02aJRBcvBlppCNKmxjI4Qned-8,1330
-swarmtube-0.1.51.dist-info/AUTHORS.rst,sha256=3ZPoqg8Aav8DSYKd0fwcwn4_5HwSiMLart0E5Un00-U,168
-swarmtube-0.1.51.dist-info/LICENSE,sha256=JqzQ9S4hVjQBOM8SiUG9-qhokt1oKfE2qJMRNa3t410,1075
-swarmtube-0.1.51.dist-info/METADATA,sha256=C-UZRUGMJ-A_4Nkbb5nzq5h_IDt22BTThxL7iYwFE08,2201
-swarmtube-0.1.51.dist-info/WHEEL,sha256=DZajD4pwLWue70CAfc7YaxT1wLUciNBvN_TTcvXpltE,110
-swarmtube-0.1.51.dist-info/entry_points.txt,sha256=X-CwHgWDulWyiPxEbHmHwg9mE7FxpaCOHctheYiJgeM,49
-swarmtube-0.1.51.dist-info/top_level.txt,sha256=jJMGZgOJVEYy1TfxYBXsNV5EzL59YaT1xSDO5Fe4Pr8,10
-swarmtube-0.1.51.dist-info/RECORD,,
+swarmtube-0.1.52.dist-info/AUTHORS.rst,sha256=3ZPoqg8Aav8DSYKd0fwcwn4_5HwSiMLart0E5Un00-U,168
+swarmtube-0.1.52.dist-info/LICENSE,sha256=JqzQ9S4hVjQBOM8SiUG9-qhokt1oKfE2qJMRNa3t410,1075
+swarmtube-0.1.52.dist-info/METADATA,sha256=HitnAbYZjUNhpGwELXVduGs6nR0NTPECfCmQdJ3ICXE,2201
+swarmtube-0.1.52.dist-info/WHEEL,sha256=DZajD4pwLWue70CAfc7YaxT1wLUciNBvN_TTcvXpltE,110
+swarmtube-0.1.52.dist-info/entry_points.txt,sha256=X-CwHgWDulWyiPxEbHmHwg9mE7FxpaCOHctheYiJgeM,49
+swarmtube-0.1.52.dist-info/top_level.txt,sha256=jJMGZgOJVEYy1TfxYBXsNV5EzL59YaT1xSDO5Fe4Pr8,10
+swarmtube-0.1.52.dist-info/RECORD,,
```

