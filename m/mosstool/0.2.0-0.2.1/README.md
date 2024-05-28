# Comparing `tmp/mosstool-0.2.0.tar.gz` & `tmp/mosstool-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosstool-0.2.0.tar", max compression
+gzip compressed data, was "mosstool-0.2.1.tar", max compression
```

## Comparing `mosstool-0.2.0.tar` & `mosstool-0.2.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0      106 2024-05-27 09:17:14.447507 mosstool-0.2.0/README.md
--rw-r--r--   0        0        0      268 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/__init__.py
--rw-r--r--   0        0        0    16340 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/_map_util/add_aoi_pop.py
--rw-r--r--   0        0        0    70559 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/_map_util/aoi_matcher.py
--rw-r--r--   0        0        0    16237 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/_map_util/aoiutils.py
--rw-r--r--   0        0        0     2956 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/_map_util/const.py
--rw-r--r--   0        0        0    11404 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/_map_util/convert_aoi.py
--rw-r--r--   0        0        0    16609 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/_map_util/format_checker.py
--rw-r--r--   0        0        0    21033 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/_map_util/gen_traffic_light.py
--rw-r--r--   0        0        0     2045 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/_map_util/map_aois_matchers.py
--rw-r--r--   0        0        0     1155 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/_map_util/osm_const.py
--rw-r--r--   0        0        0        0 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/_util/__init__.py
--rw-r--r--   0        0        0      444 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/_util/angle.py
--rw-r--r--   0        0        0     3626 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/_util/bezier.py
--rw-r--r--   0        0        0    12436 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/_util/line.py
--rw-r--r--   0        0        0      100 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/builder/__init__.py
--rw-r--r--   0        0        0   206163 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/builder/builder.py
--rw-r--r--   0        0        0      185 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/osm/__init__.py
--rw-r--r--   0        0        0     7162 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/osm/_motif.py
--rw-r--r--   0        0        0     2643 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/osm/_wayutil.py
--rw-r--r--   0        0        0    14567 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/osm/building.py
--rw-r--r--   0        0        0    28323 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/osm/roadnet.py
--rw-r--r--   0        0        0      373 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/public_transport/__init__.py
--rw-r--r--   0        0        0    12458 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/public_transport/get_bus.py
--rw-r--r--   0        0        0    12224 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/public_transport/get_subway.py
--rw-r--r--   0        0        0    21211 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/public_transport/get_transitland.py
--rw-r--r--   0        0        0    16145 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/public_transport/public_transport_post.py
--rw-r--r--   0        0        0       92 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/sumo/__init__.py
--rw-r--r--   0        0        0    37747 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/sumo/map.py
--rw-r--r--   0        0        0       79 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/vis/__init__.py
--rw-r--r--   0        0        0     9999 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/vis/map.py
--rw-r--r--   0        0        0       36 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/trip/__init__.py
--rw-r--r--   0        0        0      758 2024-05-27 09:17:15.107514 mosstool-0.2.0/mosstool/trip/generator/AIGC.py
--rw-r--r--   0        0        0      347 2024-05-27 09:17:15.107514 mosstool-0.2.0/mosstool/trip/generator/__init__.py
--rw-r--r--   0        0        0      621 2024-05-27 09:17:15.107514 mosstool-0.2.0/mosstool/trip/generator/_util/const.py
--rw-r--r--   0        0        0      406 2024-05-27 09:17:15.107514 mosstool-0.2.0/mosstool/trip/generator/_util/utils.py
--rw-r--r--   0        0        0    18572 2024-05-27 09:17:15.107514 mosstool-0.2.0/mosstool/trip/generator/generate_from_od.py
--rw-r--r--   0        0        0     3774 2024-05-27 09:17:15.107514 mosstool-0.2.0/mosstool/trip/generator/gravity.py
--rw-r--r--   0        0        0     5190 2024-05-27 09:17:15.107514 mosstool-0.2.0/mosstool/trip/generator/random.py
--rw-r--r--   0        0        0      702 2024-05-27 09:17:15.107514 mosstool-0.2.0/mosstool/trip/generator/template.py
--rw-r--r--   0        0        0      119 2024-05-27 09:17:15.107514 mosstool-0.2.0/mosstool/trip/route/__init__.py
--rw-r--r--   0        0        0     2105 2024-05-27 09:17:15.107514 mosstool-0.2.0/mosstool/trip/route/client.py
--rw-r--r--   0        0        0     3398 2024-05-27 09:17:15.107514 mosstool-0.2.0/mosstool/trip/route/preroute.py
--rw-r--r--   0        0        0      100 2024-05-27 09:17:15.107514 mosstool-0.2.0/mosstool/trip/sumo/__init__.py
--rw-r--r--   0        0        0    37589 2024-05-27 09:17:15.107514 mosstool-0.2.0/mosstool/trip/sumo/route.py
--rw-r--r--   0        0        0       78 2024-05-27 09:17:15.107514 mosstool-0.2.0/mosstool/trip/vis/__init__.py
--rw-r--r--   0        0        0     8307 2024-05-27 09:17:15.107514 mosstool-0.2.0/mosstool/trip/vis/trip.py
--rw-r--r--   0        0        0      783 2024-05-27 09:17:15.107514 mosstool-0.2.0/mosstool/type/__init__.py
--rw-r--r--   0        0        0       22 2024-05-27 09:17:15.107514 mosstool-0.2.0/mosstool/util/__init__.py
--rw-r--r--   0        0        0      481 2024-05-27 09:17:15.107514 mosstool-0.2.0/mosstool/util/color.py
--rw-r--r--   0        0        0     4519 2024-05-27 09:17:15.107514 mosstool-0.2.0/mosstool/util/format_converter.py
--rw-r--r--   0        0        0    14922 2024-05-27 09:17:15.107514 mosstool-0.2.0/mosstool/util/geo_match_pop.py
--rw-r--r--   0        0        0     2039 2024-05-27 09:17:15.107514 mosstool-0.2.0/mosstool/util/map_merger.py
--rw-r--r--   0        0        0     6538 2024-05-27 09:17:15.107514 mosstool-0.2.0/mosstool/util/map_splitter.py
--rw-r--r--   0        0        0        0 2024-05-27 09:17:15.107514 mosstool-0.2.0/mosstool/util/test/__init__.py
--rw-r--r--   0        0        0      194 2024-05-27 09:17:15.107514 mosstool-0.2.0/mosstool/util/test/test_color.py
--rw-r--r--   0        0        0     1150 2024-05-27 09:17:15.107514 mosstool-0.2.0/mosstool/util/test/test_format_conveter.py
--rw-r--r--   0        0        0      853 2024-05-27 09:17:15.107514 mosstool-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1503 1970-01-01 00:00:00.000000 mosstool-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      106 2024-05-28 11:11:04.791999 mosstool-0.2.1/README.md
+-rw-r--r--   0        0        0      268 2024-05-28 11:11:05.448002 mosstool-0.2.1/mosstool/map/__init__.py
+-rw-r--r--   0        0        0    16340 2024-05-28 11:11:05.448002 mosstool-0.2.1/mosstool/map/_map_util/add_aoi_pop.py
+-rw-r--r--   0        0        0    70559 2024-05-28 11:11:05.448002 mosstool-0.2.1/mosstool/map/_map_util/aoi_matcher.py
+-rw-r--r--   0        0        0    16237 2024-05-28 11:11:05.448002 mosstool-0.2.1/mosstool/map/_map_util/aoiutils.py
+-rw-r--r--   0        0        0     2956 2024-05-28 11:11:05.448002 mosstool-0.2.1/mosstool/map/_map_util/const.py
+-rw-r--r--   0        0        0    11404 2024-05-28 11:11:05.448002 mosstool-0.2.1/mosstool/map/_map_util/convert_aoi.py
+-rw-r--r--   0        0        0    16609 2024-05-28 11:11:05.448002 mosstool-0.2.1/mosstool/map/_map_util/format_checker.py
+-rw-r--r--   0        0        0    21033 2024-05-28 11:11:05.448002 mosstool-0.2.1/mosstool/map/_map_util/gen_traffic_light.py
+-rw-r--r--   0        0        0     2045 2024-05-28 11:11:05.448002 mosstool-0.2.1/mosstool/map/_map_util/map_aois_matchers.py
+-rw-r--r--   0        0        0     1155 2024-05-28 11:11:05.448002 mosstool-0.2.1/mosstool/map/_map_util/osm_const.py
+-rw-r--r--   0        0        0        0 2024-05-28 11:11:05.448002 mosstool-0.2.1/mosstool/map/_util/__init__.py
+-rw-r--r--   0        0        0      444 2024-05-28 11:11:05.448002 mosstool-0.2.1/mosstool/map/_util/angle.py
+-rw-r--r--   0        0        0     3626 2024-05-28 11:11:05.448002 mosstool-0.2.1/mosstool/map/_util/bezier.py
+-rw-r--r--   0        0        0    12436 2024-05-28 11:11:05.448002 mosstool-0.2.1/mosstool/map/_util/line.py
+-rw-r--r--   0        0        0      100 2024-05-28 11:11:05.448002 mosstool-0.2.1/mosstool/map/builder/__init__.py
+-rw-r--r--   0        0        0   206163 2024-05-28 11:11:05.448002 mosstool-0.2.1/mosstool/map/builder/builder.py
+-rw-r--r--   0        0        0      185 2024-05-28 11:11:05.448002 mosstool-0.2.1/mosstool/map/osm/__init__.py
+-rw-r--r--   0        0        0     7162 2024-05-28 11:11:05.448002 mosstool-0.2.1/mosstool/map/osm/_motif.py
+-rw-r--r--   0        0        0     2643 2024-05-28 11:11:05.448002 mosstool-0.2.1/mosstool/map/osm/_wayutil.py
+-rw-r--r--   0        0        0    14567 2024-05-28 11:11:05.448002 mosstool-0.2.1/mosstool/map/osm/building.py
+-rw-r--r--   0        0        0    28323 2024-05-28 11:11:05.448002 mosstool-0.2.1/mosstool/map/osm/roadnet.py
+-rw-r--r--   0        0        0      373 2024-05-28 11:11:05.448002 mosstool-0.2.1/mosstool/map/public_transport/__init__.py
+-rw-r--r--   0        0        0    12458 2024-05-28 11:11:05.448002 mosstool-0.2.1/mosstool/map/public_transport/get_bus.py
+-rw-r--r--   0        0        0    12224 2024-05-28 11:11:05.448002 mosstool-0.2.1/mosstool/map/public_transport/get_subway.py
+-rw-r--r--   0        0        0    21211 2024-05-28 11:11:05.448002 mosstool-0.2.1/mosstool/map/public_transport/get_transitland.py
+-rw-r--r--   0        0        0    16145 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/map/public_transport/public_transport_post.py
+-rw-r--r--   0        0        0       92 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/map/sumo/__init__.py
+-rw-r--r--   0        0        0    37747 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/map/sumo/map.py
+-rw-r--r--   0        0        0       79 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/map/vis/__init__.py
+-rw-r--r--   0        0        0     9999 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/map/vis/map.py
+-rw-r--r--   0        0        0       36 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/trip/__init__.py
+-rw-r--r--   0        0        0      758 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/trip/generator/AIGC.py
+-rw-r--r--   0        0        0      347 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/trip/generator/__init__.py
+-rw-r--r--   0        0        0      688 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/trip/generator/_util/const.py
+-rw-r--r--   0        0        0      406 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/trip/generator/_util/utils.py
+-rw-r--r--   0        0        0    19820 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/trip/generator/generate_from_od.py
+-rw-r--r--   0        0        0     3774 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/trip/generator/gravity.py
+-rw-r--r--   0        0        0     5190 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/trip/generator/random.py
+-rw-r--r--   0        0        0      702 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/trip/generator/template.py
+-rw-r--r--   0        0        0      119 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/trip/route/__init__.py
+-rw-r--r--   0        0        0     2105 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/trip/route/client.py
+-rw-r--r--   0        0        0     3398 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/trip/route/preroute.py
+-rw-r--r--   0        0        0      100 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/trip/sumo/__init__.py
+-rw-r--r--   0        0        0    37589 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/trip/sumo/route.py
+-rw-r--r--   0        0        0       78 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/trip/vis/__init__.py
+-rw-r--r--   0        0        0     8307 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/trip/vis/trip.py
+-rw-r--r--   0        0        0      783 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/type/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/util/__init__.py
+-rw-r--r--   0        0        0      481 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/util/color.py
+-rw-r--r--   0        0        0     4519 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/util/format_converter.py
+-rw-r--r--   0        0        0    14922 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/util/geo_match_pop.py
+-rw-r--r--   0        0        0     2039 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/util/map_merger.py
+-rw-r--r--   0        0        0     6538 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/util/map_splitter.py
+-rw-r--r--   0        0        0        0 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/util/test/__init__.py
+-rw-r--r--   0        0        0      194 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/util/test/test_color.py
+-rw-r--r--   0        0        0     1150 2024-05-28 11:11:05.452002 mosstool-0.2.1/mosstool/util/test/test_format_conveter.py
+-rw-r--r--   0        0        0      853 2024-05-28 11:11:05.452002 mosstool-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1503 1970-01-01 00:00:00.000000 mosstool-0.2.1/PKG-INFO
```

### Comparing `mosstool-0.2.0/mosstool/map/_map_util/add_aoi_pop.py` & `mosstool-0.2.1/mosstool/map/_map_util/add_aoi_pop.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.0/mosstool/map/_map_util/aoi_matcher.py` & `mosstool-0.2.1/mosstool/map/_map_util/aoi_matcher.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.0/mosstool/map/_map_util/aoiutils.py` & `mosstool-0.2.1/mosstool/map/_map_util/aoiutils.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.0/mosstool/map/_map_util/const.py` & `mosstool-0.2.1/mosstool/map/_map_util/const.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.0/mosstool/map/_map_util/convert_aoi.py` & `mosstool-0.2.1/mosstool/map/_map_util/convert_aoi.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.0/mosstool/map/_map_util/format_checker.py` & `mosstool-0.2.1/mosstool/map/_map_util/format_checker.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.0/mosstool/map/_map_util/gen_traffic_light.py` & `mosstool-0.2.1/mosstool/map/_map_util/gen_traffic_light.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.0/mosstool/map/_map_util/map_aois_matchers.py` & `mosstool-0.2.1/mosstool/map/_map_util/map_aois_matchers.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.0/mosstool/map/_map_util/osm_const.py` & `mosstool-0.2.1/mosstool/map/_map_util/osm_const.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.0/mosstool/map/_util/bezier.py` & `mosstool-0.2.1/mosstool/map/_util/bezier.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.0/mosstool/map/_util/line.py` & `mosstool-0.2.1/mosstool/map/_util/line.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.0/mosstool/map/builder/builder.py` & `mosstool-0.2.1/mosstool/map/builder/builder.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.0/mosstool/map/osm/_motif.py` & `mosstool-0.2.1/mosstool/map/osm/_motif.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.0/mosstool/map/osm/_wayutil.py` & `mosstool-0.2.1/mosstool/map/osm/_wayutil.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.0/mosstool/map/osm/building.py` & `mosstool-0.2.1/mosstool/map/osm/building.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.0/mosstool/map/osm/roadnet.py` & `mosstool-0.2.1/mosstool/map/osm/roadnet.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.0/mosstool/map/public_transport/get_bus.py` & `mosstool-0.2.1/mosstool/map/public_transport/get_bus.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.0/mosstool/map/public_transport/get_subway.py` & `mosstool-0.2.1/mosstool/map/public_transport/get_subway.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.0/mosstool/map/public_transport/get_transitland.py` & `mosstool-0.2.1/mosstool/map/public_transport/get_transitland.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.0/mosstool/map/public_transport/public_transport_post.py` & `mosstool-0.2.1/mosstool/map/public_transport/public_transport_post.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.0/mosstool/map/sumo/map.py` & `mosstool-0.2.1/mosstool/map/sumo/map.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.0/mosstool/map/vis/map.py` & `mosstool-0.2.1/mosstool/map/vis/map.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.0/mosstool/trip/generator/AIGC.py` & `mosstool-0.2.1/mosstool/trip/generator/AIGC.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.0/mosstool/trip/generator/_util/const.py` & `mosstool-0.2.1/mosstool/trip/generator/_util/const.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,7 +22,14 @@
     "HWHWH+": 1.43,
 }
 BUS = tripv2.TRIP_MODE_BUS_WALK
 CAR = tripv2.TRIP_MODE_DRIVE_ONLY
 BIKE = tripv2.TRIP_MODE_BIKE_WALK
 WALK = tripv2.TRIP_MODE_WALK_ONLY
 LANE_TYPE_DRIVING = mapv2.LANE_TYPE_DRIVING
+ALL_TRIP_MODES = [
+    BUS,
+    BUS,
+    CAR,
+    CAR,
+    WALK,
+]
```

### Comparing `mosstool-0.2.0/mosstool/trip/generator/generate_from_od.py` & `mosstool-0.2.1/mosstool/trip/generator/generate_from_od.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,14 +29,64 @@
         for p_geo in geo.geoms:
             all_coords.extend(list(p_geo.exterior.coords))
         return all_coords
     else:
         return list(geo.coords)
 
 
+# determine trip mode
+def _get_mode(p1, p2):
+    (x1, y1), (x2, y2) = p1, p2
+    dis = ((x2 - x1) ** 2 + (y2 - y1) ** 2) ** 0.5
+    if dis > DIS_CAR:
+        return CAR
+    elif dis > DIS_BIKE:
+        return BIKE
+    else:
+        return WALK
+
+
+def _get_mode_with_distribution(p1, p2):
+    (x1, y1), (x2, y2) = p1, p2
+    distance = ((x2 - x1) ** 2 + (y2 - y1) ** 2) ** 0.5
+    subway_expense = 10
+    bus_expense = 5
+    driving_duration = distance / (30 / 3.6)
+    subway_duration = distance / (35 / 3.6) + 10 * 60
+    bus_duration = distance / (15 / 3.6) + 10 * 60
+    bicycle_duration = distance / (10 / 3.6)
+    parking_fee = 20  # 停车费
+    age = 0.384  # 18到35岁人口占比
+    income = 0.395  # 低收入人群占比
+    if bus_expense > 0:
+        V_bus = -0.0516 * bus_duration / 60 - 0.4810 * bus_expense
+    else:
+        V_bus = -np.inf
+    if subway_expense > 0:
+        V_subway = -0.0512 * subway_duration / 60 - 0.0833 * subway_expense
+    else:
+        V_subway = -np.inf
+    V_fuel = (
+        -0.0705 * driving_duration / 60
+        + 0.5680 * age
+        - 0.8233 * income
+        - 0.0941 * parking_fee
+    )
+    V_elec = -0.0339 * driving_duration / 60 - 0.1735 * parking_fee
+    if distance > 15000:
+        V_bicycle = -np.inf
+    else:
+        V_bicycle = -0.1185 * bicycle_duration / 60
+    V = np.array([V_bus, V_subway, V_fuel, V_elec, V_bicycle])
+    V = np.exp(V)
+    V = V / sum(V)
+    choice_index = np.random.choice(len(V), p=V)
+    return ALL_TRIP_MODES[choice_index]
+
+
 def _match_aoi_unit(projector, aoi):
     global shapes
     x, y = projector(aoi["geo"][0][0], aoi["geo"][0][1])
     p = geometry.Point((x, y))
     for id, j in enumerate(shapes):
         if j.contains(p):
             return (aoi["id"], id)
@@ -164,33 +214,21 @@
                 min(int(time[i - 1] / OD_TIME_INTERVAL), LEN_OD_TIMES - 1),
             ]  # hour to int index
             p = p / sum(p)
             other_region = rng.choice(n_region, p=p)
             a = choose_aoi_from_region(other_region)
             aoi_list.append(a)
             now_region = other_region
-
-    # determine trip mode
-    def get_mode(p1, p2):
-        (x1, y1), (x2, y2) = p1, p2
-        dis = ((x2 - x1) ** 2 + (y2 - y1) ** 2) ** 0.5
-        if dis > DIS_CAR:
-            return CAR
-        elif dis > DIS_BIKE:
-            return BIKE
-        else:
-            return WALK
-
     trip_mode = []
     for i in range(len(aoi_list) - 1):
         lon1, lat1 = aoi_map[aoi_list[i]]["geo"][0][:2]
         lon2, lat2 = aoi_map[aoi_list[i + 1]]["geo"][0][:2]
         p1 = projector(longitude=lon1, latitude=lat1)
         p2 = projector(longitude=lon2, latitude=lat2)
-        trip_mode.append(get_mode(p1, p2))
+        trip_mode.append(_get_mode_with_distribution(p1, p2))
 
     # determine activity
     activity = []
     for i in range(len(aoi_list) - 1):
         activity.append(aoi_map[aoi_list[i + 1]]["external"]["catg"])
 
     assert len(aoi_list) == len(time) + 1
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mosstool-0.2.0/mosstool/trip/generator/gravity.py` & `mosstool-0.2.1/mosstool/trip/generator/gravity.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.0/mosstool/trip/generator/random.py` & `mosstool-0.2.1/mosstool/trip/generator/random.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.0/mosstool/trip/generator/template.py` & `mosstool-0.2.1/mosstool/trip/generator/template.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.0/mosstool/trip/route/client.py` & `mosstool-0.2.1/mosstool/trip/route/client.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.0/mosstool/trip/route/preroute.py` & `mosstool-0.2.1/mosstool/trip/route/preroute.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.0/mosstool/trip/sumo/route.py` & `mosstool-0.2.1/mosstool/trip/sumo/route.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.0/mosstool/trip/vis/trip.py` & `mosstool-0.2.1/mosstool/trip/vis/trip.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.0/mosstool/type/__init__.py` & `mosstool-0.2.1/mosstool/type/__init__.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.0/mosstool/util/format_converter.py` & `mosstool-0.2.1/mosstool/util/format_converter.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.0/mosstool/util/geo_match_pop.py` & `mosstool-0.2.1/mosstool/util/geo_match_pop.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.0/mosstool/util/map_merger.py` & `mosstool-0.2.1/mosstool/util/map_merger.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.0/mosstool/util/map_splitter.py` & `mosstool-0.2.1/mosstool/util/map_splitter.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.0/mosstool/util/test/test_format_conveter.py` & `mosstool-0.2.1/mosstool/util/test/test_format_conveter.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.0/pyproject.toml` & `mosstool-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mosstool"
-version = "0.2.0"
+version = "0.2.1"
 description = "MObility Simulation System toolbox "
 authors = ["Jun Zhang <zhangjun990222@qq.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `mosstool-0.2.0/PKG-INFO` & `mosstool-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosstool
-Version: 0.2.0
+Version: 0.2.1
 Summary: MObility Simulation System toolbox 
 License: MIT
 Author: Jun Zhang
 Author-email: zhangjun990222@qq.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

