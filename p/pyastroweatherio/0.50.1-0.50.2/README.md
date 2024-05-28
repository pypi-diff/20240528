# Comparing `tmp/pyastroweatherio-0.50.1.tar.gz` & `tmp/pyastroweatherio-0.50.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyastroweatherio-0.50.1.tar", last modified: Mon May 27 07:58:51 2024, max compression
+gzip compressed data, was "pyastroweatherio-0.50.2.tar", last modified: Tue May 28 05:27:43 2024, max compression
```

## Comparing `pyastroweatherio-0.50.1.tar` & `pyastroweatherio-0.50.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-05-27 07:58:51.190609 pyastroweatherio-0.50.1/
--rw-rw-r--   0 markus    (1000) markus    (1000)     1071 2023-04-10 18:40:11.000000 pyastroweatherio-0.50.1/LICENSE
--rw-r--r--   0 markus    (1000) markus    (1000)     1112 2024-05-27 07:58:51.190609 pyastroweatherio-0.50.1/PKG-INFO
--rw-rw-r--   0 markus    (1000) markus    (1000)     1576 2023-10-06 18:49:53.000000 pyastroweatherio-0.50.1/README.md
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-05-27 07:58:51.186609 pyastroweatherio-0.50.1/pyastroweatherio/
--rw-rw-r--   0 markus    (1000) markus    (1000)      284 2024-05-27 06:33:40.000000 pyastroweatherio-0.50.1/pyastroweatherio/__init__.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    42587 2024-05-27 06:33:53.000000 pyastroweatherio-0.50.1/pyastroweatherio/client.py
--rw-rw-r--   0 markus    (1000) markus    (1000)     6068 2024-05-25 14:57:18.000000 pyastroweatherio-0.50.1/pyastroweatherio/const.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    24883 2024-05-27 06:34:20.000000 pyastroweatherio-0.50.1/pyastroweatherio/dataclasses.py
--rw-rw-r--   0 markus    (1000) markus    (1000)      337 2024-05-25 14:57:18.000000 pyastroweatherio-0.50.1/pyastroweatherio/errors.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    47443 2024-05-27 07:50:12.000000 pyastroweatherio-0.50.1/pyastroweatherio/helper_functions.py
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-05-27 07:58:51.190609 pyastroweatherio-0.50.1/pyastroweatherio.egg-info/
--rw-r--r--   0 markus    (1000) markus    (1000)     1112 2024-05-27 07:58:51.000000 pyastroweatherio-0.50.1/pyastroweatherio.egg-info/PKG-INFO
--rw-rw-r--   0 markus    (1000) markus    (1000)      413 2024-05-27 07:58:51.000000 pyastroweatherio-0.50.1/pyastroweatherio.egg-info/SOURCES.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)        1 2024-05-27 07:58:51.000000 pyastroweatherio-0.50.1/pyastroweatherio.egg-info/dependency_links.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       25 2024-05-27 07:58:51.000000 pyastroweatherio-0.50.1/pyastroweatherio.egg-info/requires.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       17 2024-05-27 07:58:51.000000 pyastroweatherio-0.50.1/pyastroweatherio.egg-info/top_level.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       79 2024-05-27 07:58:51.190609 pyastroweatherio-0.50.1/setup.cfg
--rw-r--r--   0 markus    (1000) markus    (1000)     1397 2024-05-27 06:37:57.000000 pyastroweatherio-0.50.1/setup.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-05-28 05:27:43.419647 pyastroweatherio-0.50.2/
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1071 2023-04-10 18:40:11.000000 pyastroweatherio-0.50.2/LICENSE
+-rw-r--r--   0 markus    (1000) markus    (1000)     1112 2024-05-28 05:27:43.419647 pyastroweatherio-0.50.2/PKG-INFO
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1519 2024-05-27 17:28:04.000000 pyastroweatherio-0.50.2/README.md
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-05-28 05:27:43.403646 pyastroweatherio-0.50.2/pyastroweatherio/
+-rw-rw-r--   0 markus    (1000) markus    (1000)      284 2024-05-27 17:28:04.000000 pyastroweatherio-0.50.2/pyastroweatherio/__init__.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    42587 2024-05-27 17:28:04.000000 pyastroweatherio-0.50.2/pyastroweatherio/client.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)     6068 2024-05-27 17:28:04.000000 pyastroweatherio-0.50.2/pyastroweatherio/const.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    24611 2024-05-28 05:26:46.000000 pyastroweatherio-0.50.2/pyastroweatherio/dataclasses.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)      337 2024-05-25 14:57:18.000000 pyastroweatherio-0.50.2/pyastroweatherio/errors.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    50052 2024-05-28 05:27:01.000000 pyastroweatherio-0.50.2/pyastroweatherio/helper_functions.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-05-28 05:27:43.415646 pyastroweatherio-0.50.2/pyastroweatherio.egg-info/
+-rw-r--r--   0 markus    (1000) markus    (1000)     1112 2024-05-28 05:27:43.000000 pyastroweatherio-0.50.2/pyastroweatherio.egg-info/PKG-INFO
+-rw-rw-r--   0 markus    (1000) markus    (1000)      413 2024-05-28 05:27:43.000000 pyastroweatherio-0.50.2/pyastroweatherio.egg-info/SOURCES.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)        1 2024-05-28 05:27:43.000000 pyastroweatherio-0.50.2/pyastroweatherio.egg-info/dependency_links.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       25 2024-05-28 05:27:43.000000 pyastroweatherio-0.50.2/pyastroweatherio.egg-info/requires.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       17 2024-05-28 05:27:43.000000 pyastroweatherio-0.50.2/pyastroweatherio.egg-info/top_level.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       79 2024-05-28 05:27:43.423647 pyastroweatherio-0.50.2/setup.cfg
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1397 2024-05-28 05:27:15.000000 pyastroweatherio-0.50.2/setup.py
```

### Comparing `pyastroweatherio-0.50.1/LICENSE` & `pyastroweatherio-0.50.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.50.1/PKG-INFO` & `pyastroweatherio-0.50.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyastroweatherio
-Version: 0.50.1
+Version: 0.50.2
 Summary: Python Wrapper for 7Timer and Met.no REST API
 Home-page: https://github.com/mawinkler/pyastroweatherio
 Author: Markus Winkler
 Author-email: winkler.info@icloud.com
 License: MIT
 Keywords: AstroWeather,7Timer,Met.no,Python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyastroweatherio-0.50.1/pyastroweatherio/client.py` & `pyastroweatherio-0.50.2/pyastroweatherio/client.py`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.50.1/pyastroweatherio/const.py` & `pyastroweatherio-0.50.2/pyastroweatherio/const.py`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.50.1/pyastroweatherio/dataclasses.py` & `pyastroweatherio-0.50.2/pyastroweatherio/dataclasses.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """Defines the Data Classes used."""
 
 from datetime import datetime, timezone
 import math
 
 from pyastroweatherio.const import (
-    SEEING_MAX,
-    MAG_DEGRATION_MAX,
-    LIFTED_INDEX_VALUE,
-    LIFTED_INDEX_RANGE,
-    LIFTED_INDEX_PLAIN,
-    WIND10M_VALUE,
-    WIND10M_RANGE,
-    WIND10M_PLAIN,
-    WIND10M_DIRECTON,
-    WIND10M_MAX,
     CONDITION,
     CONDITION_PLAIN,
     DEEP_SKY_THRESHOLD,
+    LIFTED_INDEX_PLAIN,
+    LIFTED_INDEX_RANGE,
+    LIFTED_INDEX_VALUE,
+    MAG_DEGRATION_MAX,
+    SEEING_MAX,
+    WIND10M_DIRECTON,
+    WIND10M_MAX,
+    WIND10M_PLAIN,
+    WIND10M_RANGE,
+    WIND10M_VALUE,
 )
 
 
 class BaseData:
     """A representation of the base class for AstroWeather Data."""
 
     def __init__(self, data):
@@ -46,219 +46,219 @@
         self._weather = data["weather"]
         self._weather6 = data["weather6"]
         self._precipitation_amount = data["precipitation_amount"]
 
     @property
     def seventimer_init(self) -> datetime:
         """Return Forecast Anchor."""
-        
+
         if self._seventimer_init is not None:
             return self._seventimer_init.replace(microsecond=0, tzinfo=timezone.utc)
         return None
 
     @property
     def seventimer_timepoint(self) -> int:
         """Return Forecast Hour."""
-        
+
         if self._seventimer_timepoint is not None:
             return self._seventimer_timepoint
         return None
 
     @property
     def forecast_time(self) -> datetime:
         """Return Forecast Timestamp."""
-        
+
         if self._forecast_time is not None:
             return self._forecast_time.replace(microsecond=0, tzinfo=timezone.utc)
         return None
 
     @property
     def condition_percentage(self) -> int:
         """Return condition based on cloud cover, seeing and transparency."""
-        
+
         if self._condition_percentage is not None:
             return int(self._condition_percentage)
         return None
 
     @property
     def cloudcover(self) -> int:
         """Return Cloud Coverage."""
-        
+
         if self._cloudcover is not None:
             return int(self._cloudcover)
         return None
 
     @property
     def cloudcover_percentage(self) -> int:
         """Return Cloud Cover Percentage."""
-        
+
         if self._cloudcover is not None:
             return int(self._cloudcover)
         return None
 
     @property
     def cloudless_percentage(self) -> int:
         """Return Cloudless Percentage."""
-        
+
         if self._cloudcover is not None:
             return 100 - int(self._cloudcover)
         return None
 
     @property
     def cloud_area_fraction_percentage(self) -> int:
         """Return Cloud Cover Percentage."""
-        
+
         if self._cloud_area_fraction is not None:
             return int(self._cloud_area_fraction)
         return None
 
     @property
     def cloud_area_fraction_high_percentage(self) -> int:
         """Return Cloud Cover Percentage."""
-        
+
         if self._cloud_area_fraction_high is not None:
             return int(self._cloud_area_fraction_high)
         return None
 
     @property
     def cloud_area_fraction_medium_percentage(self) -> int:
         """Return Cloud Cover Percentage."""
-        
+
         if self._cloud_area_fraction_medium is not None:
             return int(self._cloud_area_fraction_medium)
         return None
 
     @property
     def cloud_area_fraction_low_percentage(self) -> int:
         """Return Cloud Cover Percentage."""
-        
+
         if self._cloud_area_fraction_low is not None:
             return int(self._cloud_area_fraction_low)
         return None
 
     @property
     def fog_area_fraction_percentage(self) -> int:
         """Return Fog Area Percentage."""
-        
+
         if self._fog_area_fraction is not None:
             return int(self._fog_area_fraction)
         return None
 
     @property
     def seeing(self) -> float:
         """Return Seeing."""
-        
+
         if self._seeing is not None:
             return round(self._seeing, 2)
         return None
 
     @property
     def seeing_percentage(self) -> int:
         """Return Seeing."""
-        
+
         if self._seeing is not None:
             return int(100 - self._seeing * 100 / SEEING_MAX)
         return None
 
     @property
     def transparency(self) -> float:
         """Return Transparency."""
-        
+
         if self._transparency is not None:
             return round(self._transparency, 2)
         return None
 
     @property
     def transparency_percentage(self) -> int:
         """Return Transparency."""
-        
+
         if self._transparency is not None:
             return int(100 - self._transparency * 100 / MAG_DEGRATION_MAX)
         return None
 
     @property
     def lifted_index(self) -> float:
         """Return Lifted Index."""
-        
+
         if self._lifted_index is not None:
             return round(self._lifted_index, 2)
         return None
 
     @property
     def rh2m(self) -> int:
         """Return 2m Relative Humidity."""
-        
+
         if self._rh2m is not None:
             return self._rh2m
         return None
 
     @property
     def wind10m_speed(self) -> float:
         """Return 10m Wind Speed."""
-        
+
         if self._wind_speed is not None:
             return self._wind_speed
         return None
 
     @property
     def calm_percentage(self) -> int:
         """Return 10m Wind Speed."""
-        
+
         if self._wind_speed is not None:
             return int(100 - self._wind_speed * (100 / WIND10M_MAX))
         return None
 
     @property
     def wind10m_direction(self) -> str:
         """Return 10m Wind Direction."""
-        
+
         if self._wind_from_direction is not None:
             direction = self._wind_from_direction
             direction += 22.5
             direction = direction % 360
             direction = int(direction / 45)  # values 0 to 7
             return WIND10M_DIRECTON[max(0, min(7, direction))]
         return None
 
     @property
     def temp2m(self) -> int:
         """Return 2m Temperature."""
-        
+
         if self._temp2m is not None:
             return self._temp2m
         return None
 
     @property
     def dewpoint2m(self) -> float:
         """Return 2m Dew Point."""
-        
+
         if self._dewpoint2m is not None:
             return round(self._dewpoint2m, 1)
         return None
 
     @property
     def weather(self) -> str:
         """Return Current Weather."""
-        
+
         if self._weather is not None:
             return self._weather.replace("_", " ").capitalize()
         return None
 
     @property
     def weather6(self) -> str:
         """Return Current Weather."""
-        
+
         if self._weather6 is not None:
             return self._weather6.replace("_", " ").capitalize()
         return None
 
     @property
     def precipitation_amount(self) -> float:
         """Return Current Weather."""
-        
+
         if self._precipitation_amount is not None:
             return self._precipitation_amount
         return None
 
 
 class LocationData(BaseData):
     """A representation of the Location AstroWeather Data."""
@@ -284,64 +284,68 @@
         self._moon_next_new_moon = data["moon_next_new_moon"]
         self._moon_next_full_moon = data["moon_next_full_moon"]
         self._moon_altitude = data["moon_altitude"]
         self._moon_azimuth = data["moon_azimuth"]
         self._night_duration_astronomical = data["night_duration_astronomical"]
         self._deep_sky_darkness_moon_rises = data["deep_sky_darkness_moon_rises"]
         self._deep_sky_darkness_moon_sets = data["deep_sky_darkness_moon_sets"]
-        self._deep_sky_darkness_moon_always_up = data["deep_sky_darkness_moon_always_up"]
-        self._deep_sky_darkness_moon_always_down = data["deep_sky_darkness_moon_always_down"]
+        self._deep_sky_darkness_moon_always_up = data[
+            "deep_sky_darkness_moon_always_up"
+        ]
+        self._deep_sky_darkness_moon_always_down = data[
+            "deep_sky_darkness_moon_always_down"
+        ]
         self._deep_sky_darkness = data["deep_sky_darkness"]
         self._deepsky_forecast = data["deepsky_forecast"]
         self._uptonight = data["uptonight"]
 
     @property
     def time_shift(self) -> int:
         """Return Forecast Timestamp."""
-        
+
         if self._time_shift is not None:
             return self._time_shift
         return None
 
     @property
     def forecast_length(self) -> int:
         """Return Forecast Length in Hours."""
-        
+
         if self._forecast_length is not None:
             return self._forecast_length
         return None
 
     @property
     def latitude(self) -> float:
         """Return Latitude."""
-        
+
         if self._latitude is not None:
             return self._latitude
         return None
 
     @property
     def longitude(self) -> float:
         """Return Longitude."""
-        
+
         if self._longitude is not None:
             return self._longitude
         return None
 
     @property
     def elevation(self) -> float:
         """Return Elevation."""
-        
+
         if self._elevation is not None:
             return self._elevation
         return None
 
     @property
     def seeing_plain(self) -> str:
         """Return Seeing."""
-        
+
         return "Deprecated. Use seeing instead."
 
     @property
     def wind10m_speed_plain(self) -> str:
         """Return wind speed plain."""
 
         if self._wind_speed is not None:
@@ -365,25 +369,25 @@
 
             return LIFTED_INDEX_PLAIN[max(0, min(7, lifted_index_value - 1))]
         return None
 
     @property
     def deep_sky_view(self) -> bool:
         """Return True if Deep Sky should be possible."""
-        
+
         if self.condition_percentage is not None:
             if self.condition_percentage >= DEEP_SKY_THRESHOLD:
                 return True
             return False
         return None
 
     @property
     def condition_plain(self) -> str:
         """Return Current View Conditions."""
-        
+
         if self.condition_percentage is not None:
             if self.condition_percentage > 80:
                 return CONDITION_PLAIN[0].capitalize()
             if self.condition_percentage > 60:
                 return CONDITION_PLAIN[1].capitalize()
             if self.condition_percentage > 40:
                 return CONDITION_PLAIN[2].capitalize()
@@ -391,287 +395,301 @@
                 return CONDITION_PLAIN[3].capitalize()
             return CONDITION_PLAIN[4].capitalize()
         return None
 
     @property
     def sun_next_rising(self) -> datetime:
         """Return Sun Next Rising Civil."""
-        
+
         if isinstance(self._sun_next_rising, datetime):
             return self._sun_next_rising
         return None
 
     @property
     def sun_next_rising_nautical(self) -> datetime:
         """Return Sun Next Rising Nautical."""
-        
+
         if isinstance(self._sun_next_rising_nautical, datetime):
             return self._sun_next_rising_nautical
         return None
 
     @property
     def sun_next_rising_astro(self) -> datetime:
         """Return Sun Next Rising Astronomical."""
-        
+
         if isinstance(self._sun_next_rising_astro, datetime):
             return self._sun_next_rising_astro
         return None
 
     @property
     def sun_next_setting(self) -> datetime:
         """Return Next Setting Civil."""
-        
+
         if isinstance(self._sun_next_setting, datetime):
             return self._sun_next_setting
         return None
 
     @property
     def sun_next_setting_nautical(self) -> datetime:
         """Return Sun Next Setting Nautical."""
-        
+
         if isinstance(self._sun_next_setting_nautical, datetime):
             return self._sun_next_setting_nautical
         return None
 
     @property
     def sun_next_setting_astro(self) -> datetime:
         """Return Sun Next Setting Astronomical."""
-        
+
         if isinstance(self._sun_next_setting_astro, datetime):
             return self._sun_next_setting_astro
         return None
 
     @property
     def sun_altitude(self) -> float:
         """Return Sun Altitude."""
-        
+
         if self._sun_altitude is not None:
             return round(self._sun_altitude, 3)
         return None
 
     @property
     def sun_azimuth(self) -> float:
         """Return sun Azimuth."""
-        
+
         if self._sun_azimuth is not None:
             return round(self._sun_azimuth, 3)
         return None
 
     @property
     def moon_next_rising(self) -> datetime:
         """Return Moon Next Rising."""
-        
+
         if isinstance(self._moon_next_rising, datetime):
             return self._moon_next_rising
         return None
 
     @property
     def moon_next_setting(self) -> datetime:
         """Return Moon Next Setting."""
-        
+
         if isinstance(self._moon_next_setting, datetime):
             return self._moon_next_setting
         return None
 
     @property
     def moon_phase(self) -> float:
         """Return Moon Phase."""
-        
+
         if self._moon_phase is not None:
             return round(self._moon_phase, 1)
         return None
 
     @property
     def moon_next_new_moon(self) -> datetime:
         """Return Moon Next New Moon."""
-        
+
         if isinstance(self._moon_next_new_moon, datetime):
             return self._moon_next_new_moon
         return None
 
     @property
     def moon_next_full_moon(self) -> datetime:
         """Return Moon Next Full Moon."""
-        
+
         if isinstance(self._moon_next_full_moon, datetime):
             return self._moon_next_full_moon
         return None
 
     @property
     def moon_altitude(self) -> float:
         """Return Moon Altitude."""
-        
+
         if self._moon_altitude is not None:
             return round(self._moon_altitude, 3)
         return None
 
     @property
     def moon_azimuth(self) -> float:
         """Return Moon Azimuth."""
-        
+
         if self._moon_azimuth is not None:
             return round(self._moon_azimuth, 3)
         return None
 
     @property
     def night_duration_astronomical(self) -> float:
         """Returns the remaining timespan of astronomical darkness."""
-        
+
         if self._night_duration_astronomical is not None:
             return self._night_duration_astronomical
         return None
 
     @property
     def deep_sky_darkness_moon_rises(self) -> bool:
         """Returns true if moon rises during astronomical night."""
-        
+
         if self._deep_sky_darkness_moon_rises is not None:
             return self._deep_sky_darkness_moon_rises
         return None
 
     @property
     def deep_sky_darkness_moon_sets(self) -> bool:
         """Returns true if moon sets during astronomical night."""
-        
+
         if self._deep_sky_darkness_moon_sets is not None:
             return self._deep_sky_darkness_moon_sets
         return None
 
     @property
     def deep_sky_darkness_moon_always_up(self) -> bool:
         """Returns true if moon is up during astronomical night."""
-        
+
         if self._deep_sky_darkness_moon_always_up is not None:
             return self._deep_sky_darkness_moon_always_up
         return None
 
     @property
     def deep_sky_darkness_moon_always_down(self) -> bool:
         """Returns true if moon is down during astronomical night."""
-        
+
         if self._deep_sky_darkness_moon_always_down is not None:
             return self._deep_sky_darkness_moon_always_down
         return None
 
     @property
     def deep_sky_darkness(self) -> float:
         """Returns the remaining timespan of deep sky darkness."""
-        
+
         if self._deep_sky_darkness is not None:
             return self._deep_sky_darkness
         return None
 
     @property
     def deepsky_forecast_today(self) -> int:
         """Return Forecas Today in Percent."""
-        
+
         if self._deepsky_forecast is not None:
             nightly_condition_sum = 0
             if len(self._deepsky_forecast) > 0:
                 for nightly_condition in self._deepsky_forecast[0].nightly_conditions:
                     nightly_condition_sum += nightly_condition
-                return int(round(nightly_condition_sum / len(self._deepsky_forecast[0].nightly_conditions)))
+                return int(
+                    round(
+                        nightly_condition_sum
+                        / len(self._deepsky_forecast[0].nightly_conditions)
+                    )
+                )
         return None
 
     @property
     def deepsky_forecast_today_dayname(self):
         """Return Forecast Todays Dayname."""
-        
+
         if self._deepsky_forecast is not None:
             if len(self._deepsky_forecast) > 0:
                 nightly_conditions = self._deepsky_forecast[0]
                 return nightly_conditions.dayname
         return None
 
     @property
     def deepsky_forecast_today_plain(self):
         """Return Forecast Today."""
-        
+
         if self._deepsky_forecast is not None:
             out = ""
             if len(self._deepsky_forecast) > 0:
                 for nightly_condition in self._deepsky_forecast[0].nightly_conditions:
-                    out += CONDITION[4 - math.floor(nightly_condition / 20)].capitalize()
+                    out += CONDITION[
+                        4 - math.floor(nightly_condition / 20)
+                    ].capitalize()
             return out
         return None
 
     @property
     def deepsky_forecast_today_desc(self):
         """Return Forecast Today Description."""
-        
+
         if self._deepsky_forecast is not None:
             if len(self._deepsky_forecast) > 0:
                 nightly_conditions = self._deepsky_forecast[0]
                 return nightly_conditions.weather.replace("_", " ").capitalize()
         return None
 
     @property
     def deepsky_forecast_tomorrow(self) -> int:
         """Return Forecas Tomorrow in Percentt."""
-        
+
         if self._deepsky_forecast is not None:
             nightly_condition_sum = 0
             if len(self._deepsky_forecast) > 1:
                 for nightly_condition in self._deepsky_forecast[1].nightly_conditions:
                     nightly_condition_sum += nightly_condition
-                return int(round(nightly_condition_sum / len(self._deepsky_forecast[1].nightly_conditions)))
+                return int(
+                    round(
+                        nightly_condition_sum
+                        / len(self._deepsky_forecast[1].nightly_conditions)
+                    )
+                )
         return None
 
     @property
     def deepsky_forecast_tomorrow_dayname(self):
         """Return Forecast Todays Dayname."""
-        
+
         if self._deepsky_forecast is not None:
             if len(self._deepsky_forecast) > 1:
                 nightly_conditions = self._deepsky_forecast[1]
                 return nightly_conditions.dayname
         return None
 
     @property
     def deepsky_forecast_tomorrow_plain(self):
         """Return Forecast Tomorrow."""
-        
+
         if self._deepsky_forecast is not None:
             out = ""
             if len(self._deepsky_forecast) > 1:
                 for nightly_condition in self._deepsky_forecast[1].nightly_conditions:
-                    out += CONDITION[4 - math.floor(nightly_condition / 20)].capitalize()
+                    out += CONDITION[
+                        4 - math.floor(nightly_condition / 20)
+                    ].capitalize()
             return out
         return None
 
     @property
     def deepsky_forecast_tomorrow_desc(self):
         """Return Forecast Tomorrow Description."""
-        
+
         if self._deepsky_forecast is not None:
             if len(self._deepsky_forecast) > 1:
                 nightly_conditions = self._deepsky_forecast[1]
                 return nightly_conditions.weather.replace("_", " ").capitalize()
         return None
 
     @property
     def deepsky_forecast(self):
         """Return Deepsky Forecast."""
-        
+
         if self._deepsky_forecast is not None:
             return self._deepsky_forecast
         return None
 
     @property
     def uptonight(self) -> int:
         """Return the number of best DSOs for tonight."""
-        
+
         if self._uptonight is not None:
             return len(self._uptonight)
         return None
 
     @property
     def uptonight_list(self) -> []:
         """Return the list of UpTonight targets."""
-        
+
         if self._uptonight is not None:
             return self._uptonight
         return None
 
 
 class ForecastData(BaseData):
     """A representation of 3-Hour Based Forecast AstroWeather Data."""
@@ -679,23 +697,23 @@
     def __init__(self, data):
         super().__init__(data)
         self._hour = data["hour"]
 
     @property
     def hour(self) -> int:
         """Return Forecast Hour of the day."""
-        
+
         if self._hour is not None:
             return self._hour
         return None
 
     @property
     def deep_sky_view(self) -> bool:
         """Return True if Deep Sky should be possible."""
-        
+
         if self.condition_percentage is not None:
             if self.condition_percentage <= DEEP_SKY_THRESHOLD:
                 return True
             return False
         return None
 
 
@@ -708,47 +726,47 @@
         self._hour = data["hour"]
         self._nightly_conditions = data["nightly_conditions"]
         self._weather = data["weather"]
 
     @property
     def seventimer_init(self) -> datetime:
         """Return Forecast Anchor."""
-        
+
         if self._seventimer_init is not None:
             return self._seventimer_init
         return None
 
     @property
     def dayname(self) -> str:
         """Return Forecast Name of the Day."""
-        
+
         if self._dayname is not None:
             return self._dayname
         return None
 
     @property
     def hour(self) -> int:
         """Return Forecast Hour."""
-        
+
         if self._hour is not None:
             return self._hour
         return None
 
     @property
     def nightly_conditions(self) -> int:
         """Return Forecast Hour."""
-        
+
         if self._nightly_conditions is not None:
             return self._nightly_conditions
         return None
 
     @property
     def weather(self) -> str:
         """Return Current Weather."""
-        
+
         if self._weather is not None:
             return self._weather.replace("_", " ").capitalize()
         return None
 
 
 class DSOUpTonight:
     """A representation of uptonight DSO."""
@@ -759,43 +777,43 @@
         self._constellation = data["constellation"]
         self._size = data["size"]
         self._foto = data["foto"]
 
     @property
     def target_name(self) -> str:
         """Return Forecast Name of the Day."""
-        
+
         if self._target_name is not None:
             return self._target_name
         return None
 
     @property
     def type(self) -> str:
         """Return Forecast Name of the Day."""
-        
+
         if self._type is not None:
             return self._type
         return None
 
     @property
     def constellation(self) -> str:
         """Return Forecast Name of the Day."""
-        
+
         if self._constellation is not None:
             return self._constellation
         return None
 
     @property
     def size(self) -> str:
         """Return Forecast Name of the Day."""
-        
+
         if self._size is not None:
             return self._size
         return None
 
     @property
     def foto(self) -> str:
         """Return Forecast Name of the Day."""
-        
+
         if self._foto is not None:
             return self._foto
         return None
```

### Comparing `pyastroweatherio-0.50.1/pyastroweatherio/helper_functions.py` & `pyastroweatherio-0.50.2/pyastroweatherio/helper_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Contains Helper functions for AstroWeather."""
 
-from datetime import UTC, datetime, timedelta, timezone
-from decimal import Decimal
+from datetime import UTC, datetime, timedelta
 import logging
 import math
 from math import degrees as deg
 from zoneinfo import ZoneInfo
 
 import ephem
 from ephem import degree
@@ -56,15 +55,17 @@
         # Dew point temperature in Celsius
         # Air pressure at sea level in hPa
         # aerosol_density in kg/m^3
 
     # #####################################################
     # Calculate lifted index
     # #####################################################
-    async def calculate_lifted_index(self, temperature, altitude, dew_point_temperature, air_pressure_at_sea_level):
+    async def calculate_lifted_index(
+        self, temperature, altitude, dew_point_temperature, air_pressure_at_sea_level
+    ):
         """Calculate atmospheric lifted index."""
         # https://en.wikipedia.org/wiki/Lifted_index
 
         if not all(
             v is not None
             for v in [
                 temperature,
@@ -80,39 +81,47 @@
 
         # Calculate saturation vapor pressure at surface temperature
         # Checked with https://www.weather.gov/epz/wxcalc_vaporpressure
         es = self._calculate_vapor_pressure(temperature)
 
         # Calculate actual vapor pressure at surface
         # Checked with https://www.weather.gov/epz/wxcalc_vaporpressure
-        e = self._calculate_vapor_pressure(dew_point_temperature)  # 6.112 * (10 ** (7.5 * (Td - Tn) / (Td - 35.85)))
+        e = self._calculate_vapor_pressure(
+            dew_point_temperature
+        )  # 6.112 * (10 ** (7.5 * (Td - Tn) / (Td - 35.85)))
 
         # Calculate mixing ratio at surface in grams per kilogram
         # Checked with https://www.weather.gov/epz/wxcalc_mixingratio
         w = self._calculate_mixing_ratio(e, air_pressure_at_sea_level)
 
         # Calculate Lifting Condensation Level
         lcl = self._calculate_lifting_condensation_level(w, air_pressure_at_sea_level)
 
         # Calculate temperature of lifted parcel at 500 mb level
-        lifted_temp_500mb = env_temp_500mb + (temperature - lcl) * 0.5  # Assumption: 500 mb is halfway through the troposphere
+        lifted_temp_500mb = (
+            env_temp_500mb + (temperature - lcl) * 0.5
+        )  # Assumption: 500 mb is halfway through the troposphere
 
         # Calculate Lifted Index
         lifted_index = env_temp_500mb - lifted_temp_500mb
 
         _LOGGER.debug(
             "Lifted Index (LI): {:.2f} °C (".format(lifted_index)
-            + "Air pressure at sea level (AP): {:.2f} mbar, ".format(air_pressure_at_sea_level)
+            + "Air pressure at sea level (AP): {:.2f} mbar, ".format(
+                air_pressure_at_sea_level
+            )
             + "Dew point(DP): {:.2f} °C, ".format(dew_point_temperature)
             + "Temperature (T): {:.2f} °C, ".format(temperature)
             + "Saturation vapor pressure at surface (ES): {:.2f} mbar, ".format(es)
             + "Actual vapor pressure at surface (E): {:.2f} mbar, ".format(e)
             + "Mixing ratio at surface (W): {:.2f} grams per kg, ".format(w)
             + "Lifting Condensation Level (LCL): {:.2f} meters, ".format(lcl)
-            + "Temperature of the lifted parcel (T Parcel): {:.2f} °C)".format(lifted_temp_500mb)
+            + "Temperature of the lifted parcel (T Parcel): {:.2f} °C)".format(
+                lifted_temp_500mb
+            )
         )
 
         return lifted_index
 
     # #####################################################
     # Calculate magniture degradation based on transparency
     # #####################################################
@@ -156,15 +165,17 @@
                 altitude,
                 dew_point_temperature,
                 air_pressure_at_sea_level,
             ]
         ):
             return None
 
-        lifted_index = await self.calculate_lifted_index(temperature, altitude, dew_point_temperature, air_pressure_at_sea_level)
+        lifted_index = await self.calculate_lifted_index(
+            temperature, altitude, dew_point_temperature, air_pressure_at_sea_level
+        )
         seeing = await self.calculate_seeing(
             temperature,
             humidity,
             dew_point_temperature,
             wind_speed,
             cloud_cover,
             altitude,
@@ -181,15 +192,17 @@
             dew_point_temperature,
             air_pressure_at_sea_level,
             lifted_index,
             seeing,
         )
 
         # Convert transparency to magnitude degradation
-        magnitude_degradation = self._transparency_to_magnitude_degradation(transparency)
+        magnitude_degradation = self._transparency_to_magnitude_degradation(
+            transparency
+        )
 
         _LOGGER.debug(
             "Magnitude Degradation: {:.2f} mag (".format(magnitude_degradation)
             + "Lifted Index (LI): {:.2f} °C, ".format(lifted_index)
             + "Seeing: {:.2f} arcsec, ".format(seeing)
             + "Estimated Atmospheric Transparency: {:.2f})".format(transparency)
         )
@@ -254,27 +267,30 @@
             ]
         ):
             return None
 
         # Constants
         C = 6.5  # 1.7
 
-        water_vapor_pressure = self._calculate_water_vapor_pressure(dew_point_temperature, humidity)
+        water_vapor_pressure = self._calculate_water_vapor_pressure(
+            dew_point_temperature, humidity
+        )
 
         # adjusted_pressure = air_pressure_at_sea_level * math.exp(-0.00012 * altitude)
-        adjusted_pressure = self._calculate_adjusted_pressure(air_pressure_at_sea_level, altitude)
+        adjusted_pressure = self._calculate_adjusted_pressure(
+            air_pressure_at_sea_level, altitude
+        )
         relative_pressure = adjusted_pressure / air_pressure_at_sea_level
 
-        # seeing_factor = (
-        #     C
-        #     * (water_vapor_pressure / 10) ** 0.25
-        #     * (wind_speed / 10) ** 0.75
-        #     * relative_pressure
-        # )
-        seeing_factor = C * (water_vapor_pressure / 10) ** 1 * relative_pressure
+        seeing_factor = (
+            C
+            * (water_vapor_pressure / 10) ** 0.25
+            * (wind_speed / 10) ** 0.75
+            * relative_pressure
+        )
         seeing = 0.98 / seeing_factor
 
         _LOGGER.debug(
             "Seeing: {:.2f} arcsec (".format(seeing)
             + "Water Vapor Pressure: {:.2f} mbar, ".format(water_vapor_pressure)
             + "Wind Speed: {:.2f} m/s, ".format(wind_speed)
             + "Relative Pressure: {:.2f} mbar, ".format(relative_pressure)
@@ -296,17 +312,17 @@
 
         lapse_rate = -0.0065  # Temperature lapse rate in K/m
         temperature_sea_level = 288.15  # Temperature at sea level in K
         gravity = 9.80665  # Acceleration due to gravity in m/s^2
         molar_mass_air = 0.02896  # Molar mass of Earth's air in kg/mol
         gas_constant = 8.31447  # Universal gas constant in J/(mol*K)
 
-        pressure_adjusted = pressure_sea_level * (1 - (lapse_rate * altitude) / temperature_sea_level) ** (
-            (gravity * molar_mass_air) / (gas_constant * lapse_rate)
-        )
+        pressure_adjusted = pressure_sea_level * (
+            1 - (lapse_rate * altitude) / temperature_sea_level
+        ) ** ((gravity * molar_mass_air) / (gas_constant * lapse_rate))
 
         return pressure_adjusted
 
     def _calculate_vapor_pressure(self, temperature):
         """
         Calculate the actual or saturation vapor pressure at the surface using the Magnus-Tetens formula.
         If the surface temperature is given, the actual vapor pressure is calculated.
@@ -409,15 +425,17 @@
         """
 
         # Constants
         A = 2440
         B = 0.00029
 
         # Calculate Lifting Condensation Level using the Clausius-Clapeyron equation
-        lcl = (A * w) / ((air_pressure_at_sea_level - w) * (1 - B * air_pressure_at_sea_level))
+        lcl = (A * w) / (
+            (air_pressure_at_sea_level - w) * (1 - B * air_pressure_at_sea_level)
+        )
 
         return lcl
 
     def _calculate_transparency(
         self,
         humidity,
         temperature,
@@ -624,145 +642,217 @@
         if self._sun_observer_astro is None:
             self._sun_observer_astro = self.get_sun_observer(ASTRONOMICAL_DUSK_DAWN)
         if self._sun is None:
             self._sun = ephem.Sun()
 
         # Rise and Setting (Civil)
         try:
-            self._sun_next_rising_civil = self._sun_observer.next_rising(ephem.Sun(), use_center=True).datetime().replace(tzinfo=UTC)
+            self._sun_next_rising_civil = (
+                self._sun_observer.next_rising(ephem.Sun(), use_center=True)
+                .datetime()
+                .replace(tzinfo=UTC)
+            )
         except (ephem.AlwaysUpError, ephem.NeverUpError):
             # Search for the next rising
             start = self._sun_observer.date.datetime()
             end = self._sun_observer.date.datetime() + timedelta(days=365)
             timestamp = start
             while timestamp < end:
                 timestamp += timedelta(minutes=1440)
                 self._sun_observer.date = timestamp
                 try:
-                    self._sun_next_rising_astro = self._sun_observer.next_rising(ephem.Sun(), use_center=True).datetime()
+                    self._sun_next_rising_astro = self._sun_observer.next_rising(
+                        ephem.Sun(), use_center=True
+                    ).datetime()
                 except (ephem.AlwaysUpError, ephem.NeverUpError):
                     continue
                 break
 
         try:
-            self._sun_next_setting_civil = self._sun_observer.next_setting(ephem.Sun(), use_center=True).datetime().replace(tzinfo=UTC)
+            self._sun_next_setting_civil = (
+                self._sun_observer.next_setting(ephem.Sun(), use_center=True)
+                .datetime()
+                .replace(tzinfo=UTC)
+            )
         except (ephem.AlwaysUpError, ephem.NeverUpError):
             # Search for the next setting
             start = self._sun_observer.date.datetime()
             end = self._sun_observer.date.datetime() + timedelta(days=365)
             timestamp = start
             while timestamp < end:
                 timestamp += timedelta(minutes=1440)
                 self._sun_observer.date = timestamp
                 try:
-                    self._sun_next_setting_astro = self._sun_observer.next_setting(ephem.Sun(), use_center=True).datetime()
+                    self._sun_next_setting_astro = self._sun_observer.next_setting(
+                        ephem.Sun(), use_center=True
+                    ).datetime()
                 except (ephem.AlwaysUpError, ephem.NeverUpError):
                     continue
                 break
 
         # Rise and Setting (Nautical)
         self._sun_observer_nautical.date = self._forecast_time
         self._sun.compute(self._sun_observer_nautical)
 
         try:
-            self._sun_next_rising_nautical = self._sun_observer_nautical.next_rising(ephem.Sun(), use_center=True).datetime().replace(tzinfo=UTC)
+            self._sun_next_rising_nautical = (
+                self._sun_observer_nautical.next_rising(ephem.Sun(), use_center=True)
+                .datetime()
+                .replace(tzinfo=UTC)
+            )
         except (ephem.AlwaysUpError, ephem.NeverUpError):
             # Search for the next astronomical rising
             start = self._sun_observer_nautical.date.datetime()
             end = self._sun_observer_nautical.date.datetime() + timedelta(days=365)
             timestamp = start
             while timestamp < end:
                 timestamp += timedelta(minutes=1440)
                 self._sun_observer_nautical.date = timestamp
                 try:
-                    self._sun_next_rising_nautical = self._sun_observer_nautical.next_rising(ephem.Sun(), use_center=True).datetime().replace(tzinfo=UTC)
+                    self._sun_next_rising_nautical = (
+                        self._sun_observer_nautical.next_rising(
+                            ephem.Sun(), use_center=True
+                        )
+                        .datetime()
+                        .replace(tzinfo=UTC)
+                    )
                 except (ephem.AlwaysUpError, ephem.NeverUpError):
                     continue
                 break
 
         try:
-            self._sun_next_setting_nautical = self._sun_observer_nautical.next_setting(ephem.Sun(), use_center=True).datetime().replace(tzinfo=UTC)
+            self._sun_next_setting_nautical = (
+                self._sun_observer_nautical.next_setting(ephem.Sun(), use_center=True)
+                .datetime()
+                .replace(tzinfo=UTC)
+            )
         except (ephem.AlwaysUpError, ephem.NeverUpError):
             # Search for the next astronomical setting
             start = self._sun_observer_nautical.date.datetime()
             end = self._sun_observer_nautical.date.datetime() + timedelta(days=365)
             timestamp = start
             while timestamp < end:
                 timestamp += timedelta(minutes=1440)
                 self._sun_observer_nautical.date = timestamp
                 try:
-                    self._sun_next_setting_nautical = self._sun_observer_nautical.next_setting(ephem.Sun(), use_center=True).datetime().replace(tzinfo=UTC)
+                    self._sun_next_setting_nautical = (
+                        self._sun_observer_nautical.next_setting(
+                            ephem.Sun(), use_center=True
+                        )
+                        .datetime()
+                        .replace(tzinfo=UTC)
+                    )
                 except (ephem.AlwaysUpError, ephem.NeverUpError):
                     continue
                 break
 
         # Rise and Setting (Astronomical)
         self._sun_observer_astro.date = self._forecast_time
         self._sun.compute(self._sun_observer_astro)
 
         try:
-            self._sun_next_rising_astro = self._sun_observer_astro.next_rising(ephem.Sun(), use_center=True).datetime().replace(tzinfo=UTC)
+            self._sun_next_rising_astro = (
+                self._sun_observer_astro.next_rising(ephem.Sun(), use_center=True)
+                .datetime()
+                .replace(tzinfo=UTC)
+            )
         except (ephem.AlwaysUpError, ephem.NeverUpError):
             # Search for the next astronomical rising
             start = self._sun_observer_astro.date.datetime()
             end = self._sun_observer_astro.date.datetime() + timedelta(days=365)
             timestamp = start
             while timestamp < end:
                 timestamp += timedelta(minutes=1440)
                 self._sun_observer_astro.date = timestamp
                 try:
-                    self._sun_next_rising_astro = self._sun_observer_astro.next_rising(ephem.Sun(), use_center=True).datetime().replace(tzinfo=UTC)
+                    self._sun_next_rising_astro = (
+                        self._sun_observer_astro.next_rising(
+                            ephem.Sun(), use_center=True
+                        )
+                        .datetime()
+                        .replace(tzinfo=UTC)
+                    )
                 except (ephem.AlwaysUpError, ephem.NeverUpError):
                     continue
                 break
 
         try:
-            self._sun_previous_rising_astro = self._sun_observer_astro.previous_rising(ephem.Sun(), use_center=True).datetime().replace(tzinfo=UTC)
+            self._sun_previous_rising_astro = (
+                self._sun_observer_astro.previous_rising(ephem.Sun(), use_center=True)
+                .datetime()
+                .replace(tzinfo=UTC)
+            )
         except (ephem.AlwaysUpError, ephem.NeverUpError):
             # Search for the previous astronomical rising
             start = self._sun_observer_astro.date.datetime()
             end = self._sun_observer_astro.date.datetime() - timedelta(days=365)
             timestamp = start
             while timestamp > end:
                 timestamp -= timedelta(minutes=1440)
                 self._sun_observer_astro.date = timestamp
                 try:
-                    self._sun_previous_rising_astro = self._sun_observer_astro.previous_rising(ephem.Sun(), use_center=True).datetime().replace(tzinfo=UTC)
+                    self._sun_previous_rising_astro = (
+                        self._sun_observer_astro.previous_rising(
+                            ephem.Sun(), use_center=True
+                        )
+                        .datetime()
+                        .replace(tzinfo=UTC)
+                    )
                 except (ephem.AlwaysUpError, ephem.NeverUpError):
                     continue
                 break
 
         try:
-            self._sun_next_setting_astro = self._sun_observer_astro.next_setting(ephem.Sun(), use_center=True).datetime().replace(tzinfo=UTC)
+            self._sun_next_setting_astro = (
+                self._sun_observer_astro.next_setting(ephem.Sun(), use_center=True)
+                .datetime()
+                .replace(tzinfo=UTC)
+            )
         except (ephem.AlwaysUpError, ephem.NeverUpError):
             # Search for the next astronomical setting
             start = self._sun_observer_astro.date.datetime()
             end = self._sun_observer_astro.date.datetime() + timedelta(days=365)
             timestamp = start
             while timestamp < end:
                 timestamp += timedelta(minutes=1440)
                 self._sun_observer_astro.date = timestamp
                 try:
-                    self._sun_next_setting_astro = self._sun_observer_astro.next_setting(ephem.Sun(), use_center=True).datetime().replace(tzinfo=UTC)
+                    self._sun_next_setting_astro = (
+                        self._sun_observer_astro.next_setting(
+                            ephem.Sun(), use_center=True
+                        )
+                        .datetime()
+                        .replace(tzinfo=UTC)
+                    )
                 except (ephem.AlwaysUpError, ephem.NeverUpError):
                     continue
                 break
 
         try:
-            self._sun_previous_setting_astro = self._sun_observer_astro.previous_setting(ephem.Sun(), use_center=True).datetime().replace(tzinfo=UTC)
+            self._sun_previous_setting_astro = (
+                self._sun_observer_astro.previous_setting(ephem.Sun(), use_center=True)
+                .datetime()
+                .replace(tzinfo=UTC)
+            )
         except (ephem.AlwaysUpError, ephem.NeverUpError):
             # Search for the previous astronomical setting
             start = self._sun_observer_astro.date.datetime()
             end = self._sun_observer_astro.date.datetime() - timedelta(days=365)
             timestamp = start
             while timestamp > end:
                 timestamp -= timedelta(minutes=1440)
                 self._sun_observer_astro.date = timestamp
                 try:
-                    self._sun_previous_setting_astro = self._sun_observer_astro.previous_setting(ephem.Sun(), use_center=True).datetime().replace(tzinfo=UTC)
+                    self._sun_previous_setting_astro = (
+                        self._sun_observer_astro.previous_setting(
+                            ephem.Sun(), use_center=True
+                        )
+                        .datetime()
+                        .replace(tzinfo=UTC)
+                    )
                 except (ephem.AlwaysUpError, ephem.NeverUpError):
                     continue
                 break
 
     def calculate_sun_altaz(self):
         """Calculates sun altitude and azimuth."""
 
@@ -789,30 +879,46 @@
             self._moon = ephem.Moon()
 
         # Rise and Setting
         self._moon_observer.date = self._forecast_time
         self._moon.compute(self._moon_observer)
 
         try:
-            self._moon_next_rising = self._moon_observer.next_rising(ephem.Moon()).datetime().replace(tzinfo=UTC)
+            self._moon_next_rising = (
+                self._moon_observer.next_rising(ephem.Moon())
+                .datetime()
+                .replace(tzinfo=UTC)
+            )
         except (ephem.AlwaysUpError, ephem.NeverUpError):
             pass
 
         try:
-            self._moon_next_setting = self._moon_observer.next_setting(ephem.Moon()).datetime().replace(tzinfo=UTC)
+            self._moon_next_setting = (
+                self._moon_observer.next_setting(ephem.Moon())
+                .datetime()
+                .replace(tzinfo=UTC)
+            )
         except (ephem.AlwaysUpError, ephem.NeverUpError):
             pass
 
         try:
-            self._moon_previous_rising = self._moon_observer.previous_rising(ephem.Moon()).datetime().replace(tzinfo=UTC)
+            self._moon_previous_rising = (
+                self._moon_observer.previous_rising(ephem.Moon())
+                .datetime()
+                .replace(tzinfo=UTC)
+            )
         except (ephem.AlwaysUpError, ephem.NeverUpError):
             pass
 
         try:
-            self._moon_previous_setting = self._moon_observer.previous_setting(ephem.Moon()).datetime().replace(tzinfo=UTC)
+            self._moon_previous_setting = (
+                self._moon_observer.previous_setting(ephem.Moon())
+                .datetime()
+                .replace(tzinfo=UTC)
+            )
         except (ephem.AlwaysUpError, ephem.NeverUpError):
             pass
 
         # self._moon_observer.date = self._forecast_time + timedelta(days=1)
         # self._moon.compute(self._moon_observer)
 
         # try:
@@ -822,18 +928,22 @@
 
         # try:
         #     self._moon_day_after_next_setting = self._moon_observer.next_setting(ephem.Moon()).datetime().replace(tzinfo=UTC)
         # except (ephem.AlwaysUpError, ephem.NeverUpError):
         #     pass
 
         # Next new Moon
-        self._moon_next_new_moon = ephem.next_new_moon(self._forecast_time).datetime().replace(tzinfo=UTC)
+        self._moon_next_new_moon = (
+            ephem.next_new_moon(self._forecast_time).datetime().replace(tzinfo=UTC)
+        )
 
         # Next full Moon
-        self._moon_next_full_moon = ephem.next_full_moon(self._forecast_time).datetime().replace(tzinfo=UTC)
+        self._moon_next_full_moon = (
+            ephem.next_full_moon(self._forecast_time).datetime().replace(tzinfo=UTC)
+        )
 
     def calculate_moon_altaz(self):
         """Calculates moon altitude and azimuth."""
 
         if self._moon_observer is None:
             self._moon_observer = self.get_moon_observer()
         if self._moon is None:
@@ -847,26 +957,36 @@
 
         # Moon Azimuth
         self._moon_azimuth = deg(float(self._moon.az))
 
     async def sun_previous_rising_astro(self) -> datetime:
         """Returns sun previous astronomical rising."""
 
-        if self._sun_previous_rising_astro is None or self._forecast_time > self._sun_previous_rising_astro:
-            _LOGGER.debug("Astronomical calculations updating sun_previous_rising_astro")
+        if (
+            self._sun_previous_rising_astro is None
+            or self._forecast_time > self._sun_previous_rising_astro
+        ):
+            _LOGGER.debug(
+                "Astronomical calculations updating sun_previous_rising_astro"
+            )
             self.calculate_sun()
 
         if self._sun_previous_rising_astro is not None:
             return self._sun_previous_rising_astro
 
     async def sun_previous_setting_astro(self) -> datetime:
         """Returns sun previous astronomical setting."""
 
-        if self._sun_previous_setting_astro is None or self._forecast_time > self._sun_previous_setting_astro:
-            _LOGGER.debug("Astronomical calculations updating sun_previous_setting_astro")
+        if (
+            self._sun_previous_setting_astro is None
+            or self._forecast_time > self._sun_previous_setting_astro
+        ):
+            _LOGGER.debug(
+                "Astronomical calculations updating sun_previous_setting_astro"
+            )
             self.calculate_sun()
 
         if self._sun_previous_setting_astro is not None:
             return self._sun_previous_setting_astro
 
     def astronomical_darkness(self) -> bool:
         """Returns true during astronomical night."""
@@ -942,35 +1062,44 @@
             return self._sun_next_rising_nautical
         if self._sun_next_rising_civil is not None:
             return self._sun_next_rising_civil
 
     async def sun_next_rising_civil(self) -> datetime:
         """Returns sun next rising."""
 
-        if self._sun_next_setting_civil is None or self._forecast_time > self._sun_next_setting_civil:
+        if (
+            self._sun_next_setting_civil is None
+            or self._forecast_time > self._sun_next_setting_civil
+        ):
             _LOGGER.debug("Astronomical calculations updating sun_next_rising_civil")
             self.calculate_sun()
 
         if self._sun_next_rising_civil is not None:
             return self._sun_next_rising_civil
 
     async def sun_next_rising_nautical(self) -> datetime:
         """Returns sun next nautical rising."""
 
-        if self._sun_next_rising_nautical is None or self._forecast_time > self._sun_next_rising_nautical:
+        if (
+            self._sun_next_rising_nautical is None
+            or self._forecast_time > self._sun_next_rising_nautical
+        ):
             _LOGGER.debug("Astronomical calculations updating sun_next_rising_nautical")
             self.calculate_sun()
 
         if self._sun_next_rising_nautical is not None:
             return self._sun_next_rising_nautical
 
     async def sun_next_rising_astro(self) -> datetime:
         """Returns sun next astronomical rising."""
 
-        if self._sun_next_rising_astro is None or self._forecast_time > self._sun_next_rising_astro:
+        if (
+            self._sun_next_rising_astro is None
+            or self._forecast_time > self._sun_next_rising_astro
+        ):
             _LOGGER.debug("Astronomical calculations updating sun_next_rising_astro")
             self.calculate_sun()
 
         if self._sun_next_rising_astro is not None:
             return self._sun_next_rising_astro
 
     async def sun_next_setting(self) -> datetime:
@@ -993,35 +1122,46 @@
             return self._sun_next_setting_nautical
         if self._sun_next_setting_civil is not None:
             return self._sun_next_setting_civil
 
     async def sun_next_setting_civil(self) -> datetime:
         """Returns sun next setting."""
 
-        if self._sun_next_setting_civil is None or self._forecast_time > self._sun_next_setting_civil:
+        if (
+            self._sun_next_setting_civil is None
+            or self._forecast_time > self._sun_next_setting_civil
+        ):
             _LOGGER.debug("Astronomical calculations updating sun_next_setting_civil")
             self.calculate_sun()
 
         if self._sun_next_setting_civil is not None:
             return self._sun_next_setting_civil
 
     async def sun_next_setting_nautical(self) -> datetime:
         """Returns sun next nautical setting."""
 
-        if self._sun_next_setting_nautical is None or self._forecast_time > self._sun_next_setting_nautical:
-            _LOGGER.debug("Astronomical calculations updating sun_next_setting_nautical")
+        if (
+            self._sun_next_setting_nautical is None
+            or self._forecast_time > self._sun_next_setting_nautical
+        ):
+            _LOGGER.debug(
+                "Astronomical calculations updating sun_next_setting_nautical"
+            )
             self.calculate_sun()
 
         if self._sun_next_setting_nautical is not None:
             return self._sun_next_setting_nautical
 
     async def sun_next_setting_astro(self) -> datetime:
         """Returns sun next astronomical setting."""
 
-        if self._sun_next_setting_astro is None or self._forecast_time > self._sun_next_setting_astro:
+        if (
+            self._sun_next_setting_astro is None
+            or self._forecast_time > self._sun_next_setting_astro
+        ):
             _LOGGER.debug("Astronomical calculations updating sun_next_setting_astro")
             self.calculate_sun()
 
         if self._sun_next_setting_astro is not None:
             return self._sun_next_setting_astro
 
     async def sun_altitude(self) -> float:
@@ -1040,25 +1180,31 @@
         if self._sun_azimuth is not None:
             return self._sun_azimuth
 
     # Return Moon information
     async def moon_next_rising(self) -> datetime:
         """Returns moon next rising."""
 
-        if self._moon_next_rising is None or self._forecast_time > self._moon_next_rising:
+        if (
+            self._moon_next_rising is None
+            or self._forecast_time > self._moon_next_rising
+        ):
             _LOGGER.debug("Astronomical calculations updating moon_next_rising")
             self.calculate_moon()
 
         if self._moon_next_rising is not None:
             return self._moon_next_rising
 
     async def moon_next_setting(self) -> datetime:
         """Returns moon next setting."""
 
-        if self._moon_next_setting is None or self._forecast_time > self._moon_next_setting:
+        if (
+            self._moon_next_setting is None
+            or self._forecast_time > self._moon_next_setting
+        ):
             _LOGGER.debug("Astronomical calculations updating moon_next_setting")
             self.calculate_moon()
 
         if self._moon_next_setting is not None:
             return self._moon_next_setting
 
     async def moon_phase(self) -> float:
@@ -1068,25 +1214,31 @@
 
         if self._moon is not None:
             return self._moon.phase
 
     async def moon_next_new_moon(self) -> float:
         """Returns the next new moon."""
 
-        if self._moon_next_new_moon is None or self._forecast_time > self._moon_next_new_moon:
+        if (
+            self._moon_next_new_moon is None
+            or self._forecast_time > self._moon_next_new_moon
+        ):
             _LOGGER.debug("Astronomical calculations updating moon_next_new_moon")
             self.calculate_moon()
 
         if self._moon_next_new_moon is not None:
             return self._moon_next_new_moon
 
     async def moon_next_full_moon(self) -> float:
         """Returns the next full moon."""
 
-        if self._moon_next_full_moon is None or self._forecast_time > self._moon_next_full_moon:
+        if (
+            self._moon_next_full_moon is None
+            or self._forecast_time > self._moon_next_full_moon
+        ):
             _LOGGER.debug("Astronomical calculations updating moon_next_full_moon")
             self.calculate_moon()
 
         if self._moon_next_full_moon is not None:
             return self._moon_next_full_moon
 
     async def moon_altitude(self) -> float:
@@ -1128,15 +1280,18 @@
 
         # Are we already in darkness?
         if self.astronomical_darkness():
             start_timestamp = self._sun_previous_setting_astro
         else:
             start_timestamp = self._sun_next_setting_astro
 
-        if self._moon_next_rising > start_timestamp and self._moon_next_rising < self._sun_next_rising_astro:
+        if (
+            self._moon_next_rising > start_timestamp
+            and self._moon_next_rising < self._sun_next_rising_astro
+        ):
             _LOGGER.debug("DSD: Moon rises during astronomical night")
             return True
         return False
 
     async def deep_sky_darkness_moon_sets(self) -> bool:
         """Returns true if moon sets during astronomical night."""
 
@@ -1150,15 +1305,18 @@
 
         # Did Moon already set in darkness?
         if self.moon_down() and self.astronomical_darkness():
             start_timestamp_moon = self._moon_previous_setting
         else:
             start_timestamp_moon = self._moon_next_setting
 
-        if start_timestamp_moon > start_timestamp and start_timestamp_moon < self._sun_next_rising_astro:
+        if (
+            start_timestamp_moon > start_timestamp
+            and start_timestamp_moon < self._sun_next_rising_astro
+        ):
             _LOGGER.debug("DSD: Moon sets during astronomical night")
             return True
         return False
 
     async def deep_sky_darkness_moon_always_up(self) -> bool:
         """Returns true if moon is up during astronomical night."""
 
@@ -1166,15 +1324,18 @@
 
         # Are we already in darkness?
         if self.astronomical_darkness():
             start_timestamp = self._sun_previous_setting_astro
         else:
             start_timestamp = self._sun_next_setting_astro
 
-        if self._moon_next_rising < start_timestamp and self._moon_next_setting > self._sun_next_rising_astro:
+        if (
+            self._moon_next_rising < start_timestamp
+            and self._moon_next_setting > self._sun_next_rising_astro
+        ):
             _LOGGER.debug("DSD: Moon is up during astronomical night")
             return True
         return False
 
     async def deep_sky_darkness_moon_always_down(self) -> bool:
         """Returns true if moon is down during astronomical night."""
 
@@ -1182,15 +1343,18 @@
 
         # Are we already in darkness?
         if self.astronomical_darkness():
             start_timestamp = self._sun_previous_setting_astro
         else:
             start_timestamp = self._sun_next_setting_astro
 
-        if self._moon_previous_setting < start_timestamp and self._moon_next_rising > self._sun_next_rising_astro:
+        if (
+            self._moon_previous_setting < start_timestamp
+            and self._moon_next_rising > self._sun_next_rising_astro
+        ):
             _LOGGER.debug("DSD: Moon is down during astronomical night")
             return True
         return False
 
     async def deep_sky_darkness(self) -> float:
         """Returns the remaining timespan of deep sky darkness."""
```

### Comparing `pyastroweatherio-0.50.1/pyastroweatherio.egg-info/PKG-INFO` & `pyastroweatherio-0.50.2/pyastroweatherio.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyastroweatherio
-Version: 0.50.1
+Version: 0.50.2
 Summary: Python Wrapper for 7Timer and Met.no REST API
 Home-page: https://github.com/mawinkler/pyastroweatherio
 Author: Markus Winkler
 Author-email: winkler.info@icloud.com
 License: MIT
 Keywords: AstroWeather,7Timer,Met.no,Python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyastroweatherio-0.50.1/setup.py` & `pyastroweatherio-0.50.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name="pyastroweatherio",
     packages=["pyastroweatherio"],
-    version="0.50.1",
+    version="0.50.2",
     license="MIT",
     description="Python Wrapper for 7Timer and Met.no REST API",
     long_description=" ".join(
         [
             "Lightweight Python 3 module to receive data via",
             "REST API from 7Timer and Met.no.",
         ],
```

