# Comparing `tmp/dwd_global_radiation-1.0.0rc8.tar.gz` & `tmp/dwd_global_radiation-1.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dwd_global_radiation-1.0.0rc8.tar", last modified: Fri May 24 18:04:17 2024, max compression
+gzip compressed data, was "dwd_global_radiation-1.1.0rc1.tar", last modified: Tue May 28 12:14:21 2024, max compression
```

## Comparing `dwd_global_radiation-1.0.0rc8.tar` & `dwd_global_radiation-1.1.0rc1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 piadmin   (1000) piadmin   (1000)        0 2024-05-24 18:04:17.900167 dwd_global_radiation-1.0.0rc8/
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)     1065 2024-05-05 09:59:58.000000 dwd_global_radiation-1.0.0rc8/LICENSE
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)    22430 2024-05-24 18:04:17.900167 dwd_global_radiation-1.0.0rc8/PKG-INFO
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)    21423 2024-05-21 10:47:19.000000 dwd_global_radiation-1.0.0rc8/README.md
-drwxr-xr-x   0 piadmin   (1000) piadmin   (1000)        0 2024-05-24 18:04:17.896167 dwd_global_radiation-1.0.0rc8/dwd_global_radiation/
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)       45 2024-05-07 07:51:24.000000 dwd_global_radiation-1.0.0rc8/dwd_global_radiation/__init__.py
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)    27565 2024-05-24 17:39:29.000000 dwd_global_radiation-1.0.0rc8/dwd_global_radiation/global_radiation.py
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)    18137 2024-05-15 21:06:36.000000 dwd_global_radiation-1.0.0rc8/dwd_global_radiation/utils.py
-drwxr-xr-x   0 piadmin   (1000) piadmin   (1000)        0 2024-05-24 18:04:17.900167 dwd_global_radiation-1.0.0rc8/dwd_global_radiation.egg-info/
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)    22430 2024-05-24 18:04:17.000000 dwd_global_radiation-1.0.0rc8/dwd_global_radiation.egg-info/PKG-INFO
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)      349 2024-05-24 18:04:17.000000 dwd_global_radiation-1.0.0rc8/dwd_global_radiation.egg-info/SOURCES.txt
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)        1 2024-05-24 18:04:17.000000 dwd_global_radiation-1.0.0rc8/dwd_global_radiation.egg-info/dependency_links.txt
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)      128 2024-05-24 18:04:17.000000 dwd_global_radiation-1.0.0rc8/dwd_global_radiation.egg-info/requires.txt
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)       21 2024-05-24 18:04:17.000000 dwd_global_radiation-1.0.0rc8/dwd_global_radiation.egg-info/top_level.txt
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)       38 2024-05-24 18:04:17.900167 dwd_global_radiation-1.0.0rc8/setup.cfg
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)     1656 2024-05-24 17:59:00.000000 dwd_global_radiation-1.0.0rc8/setup.py
+drwxr-xr-x   0 piadmin   (1000) piadmin   (1000)        0 2024-05-28 12:14:21.239580 dwd_global_radiation-1.1.0rc1/
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)     1065 2024-05-05 09:59:58.000000 dwd_global_radiation-1.1.0rc1/LICENSE
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)    22430 2024-05-28 12:14:21.239580 dwd_global_radiation-1.1.0rc1/PKG-INFO
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)    21423 2024-05-21 10:47:19.000000 dwd_global_radiation-1.1.0rc1/README.md
+drwxr-xr-x   0 piadmin   (1000) piadmin   (1000)        0 2024-05-28 12:14:21.239580 dwd_global_radiation-1.1.0rc1/dwd_global_radiation/
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)       45 2024-05-27 15:10:26.000000 dwd_global_radiation-1.1.0rc1/dwd_global_radiation/__init__.py
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)    27371 2024-05-28 11:59:54.000000 dwd_global_radiation-1.1.0rc1/dwd_global_radiation/global_radiation.py
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)     7298 2024-05-28 11:57:05.000000 dwd_global_radiation-1.1.0rc1/dwd_global_radiation/global_radiation_printer.py
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)    20227 2024-05-28 11:57:05.000000 dwd_global_radiation-1.1.0rc1/dwd_global_radiation/utils.py
+drwxr-xr-x   0 piadmin   (1000) piadmin   (1000)        0 2024-05-28 12:14:21.239580 dwd_global_radiation-1.1.0rc1/dwd_global_radiation.egg-info/
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)    22430 2024-05-28 12:14:21.000000 dwd_global_radiation-1.1.0rc1/dwd_global_radiation.egg-info/PKG-INFO
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)      398 2024-05-28 12:14:21.000000 dwd_global_radiation-1.1.0rc1/dwd_global_radiation.egg-info/SOURCES.txt
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)        1 2024-05-28 12:14:21.000000 dwd_global_radiation-1.1.0rc1/dwd_global_radiation.egg-info/dependency_links.txt
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)      128 2024-05-28 12:14:21.000000 dwd_global_radiation-1.1.0rc1/dwd_global_radiation.egg-info/requires.txt
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)       21 2024-05-28 12:14:21.000000 dwd_global_radiation-1.1.0rc1/dwd_global_radiation.egg-info/top_level.txt
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)       38 2024-05-28 12:14:21.239580 dwd_global_radiation-1.1.0rc1/setup.cfg
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)     1656 2024-05-28 11:57:22.000000 dwd_global_radiation-1.1.0rc1/setup.py
```

### Comparing `dwd_global_radiation-1.0.0rc8/LICENSE` & `dwd_global_radiation-1.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `dwd_global_radiation-1.0.0rc8/PKG-INFO` & `dwd_global_radiation-1.1.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dwd_global_radiation
-Version: 1.0.0rc8
+Version: 1.1.0rc1
 Summary: Access and analyze DWD global radiation data and forecasts
 Home-page: https://github.com/aschmere/dwd_global_radiation
 Author: Arno Schmerer
 License: MIT
 Keywords: weather meteorology radiation solar forecasting DWD data environmental data climate studies solar energy forecasting
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `dwd_global_radiation-1.0.0rc8/README.md` & `dwd_global_radiation-1.1.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `dwd_global_radiation-1.0.0rc8/dwd_global_radiation/global_radiation.py` & `dwd_global_radiation-1.1.0rc1/dwd_global_radiation/global_radiation.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,126 +17,197 @@
 - Format and print the data for easy visualization and verification.
 - Maintain data integrity and facilitate easy updates and retrieval of the most recent data
   according to specified constraints (like maximum age of data).
 
 Usage of this module is suitable for applications in environmental science, meteorology, and
 any system requiring precise global radiation data management and representation.
 """
-from dataclasses import dataclass, field
-from datetime import datetime
+
 import datetime as dtbase
-from string import Template
-import tzlocal
-from tabulate import tabulate
+import logging
+from dataclasses import dataclass, field
+from datetime import datetime, timedelta, timezone
+from typing import Any
+
 import numpy as np
+import tzlocal
 
 from . import utils
+from .global_radiation_printer import (
+    FormatConfig,
+    PrintConfig,
+    get_language_details,
+    print_forecasts,
+    print_header,
+    print_measurements,
+)
+
+# Initialize a logger for this module
+_LOGGER = logging.getLogger(__name__)
 
 MAX_AGE_HOURS_OF_GLOBAL_RAD_DATA = 3
 
+
+@dataclass
+class GlobalForecastData:
+    """
+    Holds global forecast data and its issuance time.
+
+    Attributes:
+        issuance_time (datetime): The timestamp of the last forecast data retrieval.
+        all_grid_forecasts (Any): The cached forecast data.
+    """
+
+    issuance_time: float = None
+    all_grid_forecasts: Any = None  # The actual forecast data cache∏
+
+
+@dataclass
+class GlobalMeasurementData:
+    """
+    Class to store cached global measurement data.
+
+    Attributes:
+        issuance_time (float): Timestamp of the last issuance of measurement data. Initially None.
+        latest_file_time (datetime): The latest file time from the DWD OpenData servers.
+            Initially None.
+        all_grid_measurements (list): List to store arrays of measurement data from multiple files.
+    """
+
+    issuance_time: float = None
+    latest_file_time: datetime = None  # New attribute to store the latest file time
+    all_grid_measurements: list = field(
+        default_factory=list
+    )  # List to store measurement data arrays
+
+
 @dataclass
 class Location:
     """Class for a user-provided location for measurement and forecast data"""
+
     latitude: float
     longitude: float
     name: str
     measurements: list = field(default_factory=list)
     forecasts: list = field(default_factory=list)
 
     def __repr__(self):
         measurement_count = len(self.measurements)
         forecast_count = len(self.forecasts)
         parts = [
             f"Location(name={self.name}",
             f"latitude={self.latitude}",
             f"longitude={self.longitude}",
             f"measurements={measurement_count} {'item' if measurement_count == 1 else 'items'}",
-            f"forecasts={forecast_count} {'item' if forecast_count == 1 else 'items'})"
+            f"forecasts={forecast_count} {'item' if forecast_count == 1 else 'items'})",
         ]
         return ", ".join(parts)
 
     def to_dict(self):
         """Convert Location to a dictionary."""
         return {
             "latitude": float(self.latitude),  # Explicit conversion to float
-            "longitude": float(self.longitude), # Explicit conversion to float
+            "longitude": float(self.longitude),  # Explicit conversion to float
             "name": self.name,
-            "measurements": [measurement.to_dict() for measurement in self.measurements],
-            "forecasts": [forecast.to_dict() for forecast in self.forecasts]
+            "measurements": [
+                measurement.to_dict() for measurement in self.measurements
+            ],
+            "forecasts": [forecast.to_dict() for forecast in self.forecasts],
         }
 
+
 @dataclass
 class MeasurementEntry:
     """Class for storing DWD global radiation measurement data."""
+
     timestamp: float  # assuming timestamp is a Unix time float
-    sis: float        # Solar Irradiance in W/m^2
+    sis: float  # Solar Irradiance in W/m^2
 
     def to_dict(self):
         """Convert MeasurementEntry to a dictionary."""
         return {
             "timestamp": float(self.timestamp),  # Explicit conversion to float
-            "sis": float(self.sis)               # Explicit conversion to float
+            "sis": float(self.sis),  # Explicit conversion to float
         }
 
 
 @dataclass
 class Measurement:
     """Class for hosting various quarterly hour global radiation measurement
     data from DWD servers"""
+
     grid_latitude: float
     grid_longitude: float
     distance: float
     nearest_index: int
     measurement_values: list[MeasurementEntry] = field(default_factory=list)
 
     def __repr__(self):
-        measurement_values_count=len(self.measurement_values)
+        measurement_values_count = len(self.measurement_values)
         # Round latitude and longitude to two decimal places
         lat = round(self.grid_latitude, 2) if self.grid_latitude is not None else None
         lon = round(self.grid_longitude, 2) if self.grid_longitude is not None else None
-        return (f"Measurement(grid_latitude={lat}, "
-                f"grid_longitude={lon}, "
-                f"distance={self.distance}, "
-                f"nearest_index={self.nearest_index}, "
-                f"measurement_values=Count: {measurement_values_count})")
+        return (
+            f"Measurement(grid_latitude={lat}, "
+            f"grid_longitude={lon}, "
+            f"distance={self.distance}, "
+            f"nearest_index={self.nearest_index}, "
+            f"measurement_values=Count: {measurement_values_count})"
+        )
 
     def to_dict(self):
         """Convert Measurement to a dictionary."""
         return {
             "grid_latitude": float(self.grid_latitude),  # Explicit conversion to float
-            "grid_longitude": float(self.grid_longitude), # Explicit conversion to float
-            "distance": float(self.distance),            # Explicit conversion to float
-            "nearest_index": int(self.nearest_index),    # Explicit conversion to int
-            "measurement_values": [entry.to_dict() for entry in self.measurement_values]
+            "grid_longitude": float(
+                self.grid_longitude
+            ),  # Explicit conversion to float
+            "distance": float(self.distance),  # Explicit conversion to float
+            "nearest_index": int(self.nearest_index),  # Explicit conversion to int
+            "measurement_values": [
+                entry.to_dict() for entry in self.measurement_values
+            ],
         }
 
     def add_measurement_value(self, timestamp, sis):
-        """Method for adding retrieved measurement values as SIS"""
-        self.measurement_values.append(MeasurementEntry(timestamp, sis))
+        """Method for adding retrieved measurement values as SIS."""
+        if not any(entry.timestamp == timestamp for entry in self.measurement_values):
+            self.measurement_values.append(MeasurementEntry(timestamp, sis))
+        else:
+            _LOGGER.warning(
+                "Duplicate timestamp %s found. Measurement value not added.", timestamp
+            )
 
     def get_measurement_values(self):
         """Method to retrieve all measurement values"""
         return self.measurement_values
 
+
 @dataclass
 class Forecast:
     """Class for storing Forecast data retrieved in hourly granularity from DWD servers"""
 
     issuance_time: str
     grid_latitude: float = None
     grid_longitude: float = None
     distance: float = None
     entries: list = field(default_factory=list)
-    metadata: dict = field(default_factory=
-                           lambda: {"standard_name": None, "long_name": None, "units": None})
+    metadata: dict = field(
+        default_factory=lambda: {
+            "standard_name": None,
+            "long_name": None,
+            "units": None,
+        }
+    )
 
     def __repr__(self):
         entries_count = len(self.entries)
         metadata_status = (
-            "populated" if any(value is not None for value in self.metadata.values())
+            "populated"
+            if any(value is not None for value in self.metadata.values())
             else "empty"
         )
         # Round latitude and longitude to two decimal places
         lat = round(self.grid_latitude, 2) if self.grid_latitude is not None else None
         lon = round(self.grid_longitude, 2) if self.grid_longitude is not None else None
         return (
             f"Forecast(issuance_time={self.issuance_time}, "
@@ -146,18 +217,20 @@
         )
 
     def to_dict(self):
         """Convert Forecast to a dictionary."""
         return {
             "issuance_time": float(self.issuance_time),  # Explicit conversion to float
             "grid_latitude": float(self.grid_latitude),  # Explicit conversion to float
-            "grid_longitude": float(self.grid_longitude), # Explicit conversion to float
-            "distance": float(self.distance),            # Explicit conversion to float
+            "grid_longitude": float(
+                self.grid_longitude
+            ),  # Explicit conversion to float
+            "distance": float(self.distance),  # Explicit conversion to float
             "entries": [entry.to_dict() for entry in self.entries],
-            "metadata": self.metadata
+            "metadata": self.metadata,
         }
 
     def set_metadata(self, standard_name=None, long_name=None, units=None):
         """Function for writing global radiation metadata of the DWD data file"""
         self.metadata["standard_name"] = standard_name
         self.metadata["long_name"] = long_name
         self.metadata["units"] = units
@@ -173,233 +246,90 @@
         )
 
     def add_entry(self, timestamp, sis):
         """Method to add a forecast entry from a retrieved DWD file"""
         entry = ForecastEntry(timestamp, sis)
         self.entries.append(entry)
 
+
 @dataclass
 class ForecastEntry:
     """Class for storing DWD global radiation forecast data"""
 
     timestamp: str
     sis: float
 
     def to_dict(self):
         """Convert ForecastEntry to a dictionary."""
         return {
             "timestamp": float(self.timestamp),  # Explicit conversion to float
-            "sis": float(self.sis)               # Explicit conversion to float
+            "sis": float(self.sis),  # Explicit conversion to float
         }
-
-@dataclass
-class IndentConfig:
-    """Handles indentation settings for pretty-printing data outputs."""
-    indent: str = "     "
-    sub_indent: str = "        "
-
-@dataclass
-class FormatConfig:
-    """Encapsulates formatting details such as date/time format and local timezone."""
-    dt_format: str
-    local_tz: str
-
-@dataclass
-class PrintConfig:
-    """ Class for setting configuration parameters for the global radiation print service."""
-
-    labels: dict
-    format_config: FormatConfig
-    indent_config: IndentConfig = field(default_factory=IndentConfig)
-
 @dataclass
 class GlobalRadiation:
     """This is the main class of the DWD Global Radiation Observation and Forecast Data Library
     It gets instantiated by every program using this library. It stores the whole dataclass
     hierarchy for storing the DWD forecast and measurement data. It also provides the main methods
     for retrieving the data from DWD servers via http file download."""
 
     locations: list = field(default_factory=list)
     last_measurement_fetch_date: datetime = None
     last_forecast_fetch_date: datetime = None
-    measurement_health_state: str = 'green'
-    forecast_health_state: str = 'green'
+    measurement_health_state: str = "green"
+    forecast_health_state: str = "green"
+    forecast_data: GlobalForecastData = field(default_factory=GlobalForecastData)
+    measurement_data: GlobalMeasurementData = field(
+        default_factory=GlobalMeasurementData
+    )
 
     def to_dict(self):
         """Convert GlobalRadiation to a dictionary."""
         return {
             "locations": [location.to_dict() for location in self.locations],
-            "last_measurement_fetch_date": self.last_measurement_fetch_date.isoformat(
-                ) if self.last_measurement_fetch_date else None,
-            "last_forecast_fetch_date": self.last_forecast_fetch_date.isoformat(
-                ) if self.last_forecast_fetch_date else None,
+            "last_measurement_fetch_date": (
+                self.last_measurement_fetch_date.isoformat()
+                if self.last_measurement_fetch_date
+                else None
+            ),
+            "last_forecast_fetch_date": (
+                self.last_forecast_fetch_date.isoformat()
+                if self.last_forecast_fetch_date
+                else None
+            ),
             "measurement_health_state": self.measurement_health_state,
-            "forecast_health_state": self.forecast_health_state
+            "forecast_health_state": self.forecast_health_state,
         }
 
     def get_location_by_name(self, name):
         """Returns a location by its name, if exists."""
         for location in self.locations:
             if location.name == name:
                 return location
         return None  # or raise an exception if a location is not found
 
     def print_data(self, language="English"):
         """
-        Function for printing the data of the GlobalRadiation class and its subclasses
-
-        This method provides a comprehensive print service to output all the retrieved
-        global radiation forecast and measurement data from the queried DWD datasets.
-        The default output language is English, but another supported language is German
+        Function for printing the data of the GlobalRadiation class and its subclasses.
         """
         local_tz = tzlocal.get_localzone()
-        title, labels, dt_format = self._get_language_details(language)
+        title, labels, dt_format = get_language_details(language)
         format_config = FormatConfig(dt_format=dt_format, local_tz=local_tz)
         config = PrintConfig(labels=labels, format_config=format_config)
 
-        self._print_header(title)
+        print_header(title)
         for location in self.locations:
             print(f"{config.labels['location']}: {location.name}")
             print(f"{config.indent_config.indent}{config.labels['latitude']}: {location.latitude}")
             print(
                 f"{config.indent_config.indent}{config.labels['longitude']}: {location.longitude}")
 
             if location.measurements:
-                self._print_measurements(location.measurements, config)
+                print_measurements(location.measurements, config)
             if location.forecasts:
-                self._print_forecasts(location.forecasts, config)
-
-    def _get_language_details(self, language):
-        if language == "German":
-            title = "DWD Vorhersage- und Beobachtungsdaten ausgewählter Standorte"
-            labels = {
-                "location": "Ort",
-                "latitude": "Breitengrad",
-                "longitude": "Längengrad",
-                "measurements": "Messungen",
-                "timestamp": "Zeitstempel",
-                "sis": "SIS Wert in W/m2",
-                "grid_latitude": "Rasterbreitengrad",
-                "grid_longitude": "Rasterlängengrad",
-                "distance": "Entfernung der Lokation zum nächsten Gridpunkt in km",
-                "forecasts": "Prognosen",
-                "issuance_time": "Ausgabezeit",
-                "metadata": "Metadaten",
-                "entries": "Einträge",
-            }
-            dt_format = "%d.%m.%Y %H:%M:%S"
-        else:
-            title = "DWD Forecast and Observation Data from Selected Locations"
-            labels = {
-                "location": "Location",
-                "latitude": "Latitude",
-                "longitude": "Longitude",
-                "measurements": "Measurements",
-                "timestamp": "Timestamp",
-                "sis": "SIS Value in W/m2",
-                "grid_latitude": "Grid Latitude",
-                "grid_longitude": "Grid Longitude",
-                "distance": "Distance of the location to the nearest gridpoint in km",
-                "forecasts": "Forecasts",
-                "issuance_time": "Issuance Time",
-                "metadata": "Metadata",
-                "entries": "Entries",
-            }
-            dt_format = "%Y-%m-%d %H:%M:%S"
-
-        return title, labels, dt_format
-
-    def _print_header(self, title):
-        print("=" * len(title))
-        print(title)
-        print("=" * len(title))
-
-    def _print_measurements(self, measurements, config):
-        print(f"{config.indent_config.indent}{config.labels['measurements']}:")
-        for measurement in measurements:
-            self._print_single_measurement(measurement, config)
-
-    def _print_forecasts(self, forecasts, config):
-        print(f"{config.indent_config.indent}{config.labels['forecasts']}:")
-        for forecast in forecasts:
-            self._print_single_forecast(forecast, config)
-
-    def _print_single_measurement(self, measurement, config):
-        """
-        Prints a single measurement, utilizing the PrintConfig object to access
-        necessary configuration like labels, date format, and additional indentation.
-        """
-        output = Template(
-            f"{config.indent_config.sub_indent}{config.labels['grid_latitude']}: $grid_latitude\n"
-            f"{config.indent_config.sub_indent}{config.labels['grid_longitude']}: $grid_longitude\n"
-            f"{config.indent_config.sub_indent}{config.labels['distance']}: $distance"
-        ).substitute(
-            grid_latitude=measurement.grid_latitude,
-            grid_longitude=measurement.grid_longitude,
-            distance=measurement.distance,
-        )
-        print(output)
-        if measurement.measurement_values:
-            self._print_tabulated_data(measurement.measurement_values, config)
-
-    def _print_tabulated_data(self, data_entries, config):
-        """
-        Prints data entries (either forecast entries or measurement values) in a tabulated format,
-        utilizing the PrintConfig object for formatting details such as labels, date format,
-        and additional indentation.
-        """
-        table = [
-            [
-                datetime.fromtimestamp(
-                    entry.timestamp, config.format_config.local_tz).strftime(
-                        config.format_config.dt_format),
-                entry.sis  # Now consistently using `sis` for both measurements and forecasts
-            ]
-            for entry in data_entries
-        ]
-
-        table_output = tabulate(
-            table,
-            headers=[config.labels["timestamp"], config.labels["sis"]],
-            tablefmt="grid"
-        )
-
-        table_output = "\n".join(
-            [f"{config.indent_config.sub_indent}{line}" for line in table_output.splitlines()]
-        )
-
-        print(table_output)
-
-    def _print_single_forecast(self, forecast, config):
-        """
-        Prints a single forecast, utilizing the PrintConfig object to access necessary
-        configuration like labels, date format, and additional indentation.
-        """
-        issuance_time = datetime.fromtimestamp(
-            forecast.issuance_time, config.format_config.local_tz
-        ).strftime(config.format_config.dt_format)
-
-        output = Template(
-            f"{config.indent_config.sub_indent}{config.labels['issuance_time']}: $issuance_time\n"
-            f"{config.indent_config.sub_indent}{config.labels['grid_latitude']}: $grid_latitude\n"
-            f"{config.indent_config.sub_indent}{config.labels['grid_longitude']}: $grid_longitude\n"
-            f"{config.indent_config.sub_indent}{config.labels['distance']}: $distance\n"
-            f"{config.indent_config.sub_indent}{config.labels['metadata']}: $metadata"
-        ).substitute(
-            issuance_time=issuance_time,
-            grid_latitude=forecast.grid_latitude,
-            grid_longitude=forecast.grid_longitude,
-            distance=forecast.distance,
-            metadata=forecast.metadata,
-        )
-        print(output)
-
-        if forecast.entries:
-            self._print_tabulated_data(forecast.entries, config)
-
+                print_forecasts(location.forecasts, config)
 
     def add_location(self, *, latitude=None, longitude=None, name=None):
         """
         With this method a user-provided location can be handed over to the main class.
         For all defined locations global radiation data will be retrieved and parsed.
         Checks for the uniqueness of the location name before adding to prevent duplicates.
         """
@@ -418,14 +348,15 @@
         # Check for unique location name
         if any(loc.name == name for loc in self.locations):
             raise ValueError(f"A location with the name '{name}' already exists.")
 
         # If all checks pass, create and add the new location
         location = Location(latitude, longitude, name)
         self.locations.append(location)
+
     def remove_location(self, name):
         """Removes a location by its name."""
         for i, location in enumerate(self.locations):
             if location.name == name:
                 del self.locations[i]
                 return
         raise ValueError(f"Location with name '{name}' not found")
@@ -442,15 +373,15 @@
         def calculate_candidate_points(lat, lon, lat_res=0.05, lon_res=0.05):
             lat_min = np.floor(lat / lat_res) * lat_res
             lon_min = np.floor(lon / lon_res) * lon_res
             return [
                 (lat_min, lon_min),
                 (lat_min, lon_min + lon_res),
                 (lat_min + lat_res, lon_min),
-                (lat_min + lat_res, lon_min + lon_res)
+                (lat_min + lat_res, lon_min + lon_res),
             ]
 
         def find_nearest_point(lat, lon, candidate_points):
             distances = [
                 utils.haversine(lat, lon, c_lat, c_lon)
                 for c_lat, c_lon in candidate_points
             ]
@@ -462,118 +393,188 @@
             lon_var = grid_data.variables["lon"][:]
             lat_idx = np.argmin(np.abs(lat_var - grid_lat))
             lon_idx = np.argmin(np.abs(lon_var - grid_lon))
             return lat_idx, lon_idx
 
         all_grid_global_rad_data, _ = grid_data
         candidate_points = calculate_candidate_points(latitude, longitude)
-        nearest_distance, (
-            grid_latitude, grid_longitude) = find_nearest_point(
-                latitude, longitude, candidate_points)
+        nearest_distance, (grid_latitude, grid_longitude) = find_nearest_point(
+            latitude, longitude, candidate_points
+        )
         lat_index, lon_index = get_grid_indices(
-            grid_latitude, grid_longitude, all_grid_global_rad_data)
+            grid_latitude, grid_longitude, all_grid_global_rad_data
+        )
 
         return (
             lat_index * len(all_grid_global_rad_data.variables["lon"][:]) + lon_index,
             nearest_distance,
             round(grid_latitude, 2),
-            round(grid_longitude, 2)
+            round(grid_longitude, 2),
         )
 
-
     def _get_measurement_value_from_loaded_data(
         self, all_grid_global_rad_data, nearest_index
     ):
         lat_index = nearest_index // all_grid_global_rad_data.variables["lat"].shape[0]
         lon_index = nearest_index % all_grid_global_rad_data.variables["lat"].shape[0]
         measurement_value = all_grid_global_rad_data.variables["SIS"][:][
             0, lat_index, lon_index
         ]
-        return measurement_value
+        units_string = all_grid_global_rad_data.variables["time"].units
+        time_value = all_grid_global_rad_data.variables["time"][0].data.item()
+
+        # Parse the base date from the units string and set it to UTC
+        base_date_str = units_string.split(" since ")[1]
+        base_date = datetime.strptime(base_date_str, "%Y-%m-%d %H:%M:%S")
+
+        # Ensure the base_date is in UTC
+        base_date = base_date.replace(tzinfo=timezone.utc)
+
+        # Convert the base date to a timestamp
+        base_timestamp = base_date.timestamp()
+
+        # Add the time value to the base timestamp
+        real_timestamp = base_timestamp + time_value
+
+        return real_timestamp, measurement_value
 
     def fetch_measurements(
-        self, max_hour_age_of_measurement: int = MAX_AGE_HOURS_OF_GLOBAL_RAD_DATA):
+        self, max_hour_age_of_measurement: int = MAX_AGE_HOURS_OF_GLOBAL_RAD_DATA
+    ):
         """
-        This method fetches DWD Global Radiation data from DWD OpenData servers.
+        Fetches DWD Global Radiation data from DWD OpenData servers.
 
         Parameters:
         max_hour_age_of_measurement:
-        This parameter defines the maximum age in hours, for which
-        global radiation measurement data shall be retrieved. The data provided by DWD is not actual
-        measurement data, but full-grid satellite data. Every 15min a new file is put on the DWD
-        servers. The history on the http file share goes back multiple days. As a programmer you
-        should adapt the queried history to your needs. If you want to record long term data,
-        use this method as a basis for persisting the data into an external database.
-        Use this parameter with caution, with every added hour 4 more full-grid files
-        have to be downloaded and analyzed.
-        The higher you choose this number, the longer the run time of your fetch operation will be.
-        A reasonable default is 3h set by the MAX_AGE_HOURS_OF_GLOBAL_RAD_DATA constant.
+            Defines the maximum age in hours for which global radiation measurement data
+            shall be retrieved. The data provided by DWD is not actual measurement data, but
+            full-grid satellite data. Every 15 minutes a new file is put on the DWD servers.
+            The history on the HTTP file share goes back multiple days. As a programmer,
+            you should adapt the queried history to your needs. If you want to record
+            long-term data, use this method as a basis for persisting the data into an
+            external database. Use this parameter with caution; with every added hour,
+            4 more full-grid files have to be downloaded and analyzed. The higher you choose
+            this number, the longer the run time of your fetch operation will be.
+            A reasonable default is 3h set by the MAX_AGE_HOURS_OF_GLOBAL_RAD_DATA constant.
         """
-        # Initialize measurements for all locations
-        self.reset_all_measurements()
-
-        current_date = datetime.now(dtbase.UTC)
+        current_date = datetime.now(timezone.utc)
         self.last_measurement_fetch_date = current_date
-        matching_files = utils.get_matching_dwd_globalrad_data_files(
-            current_date, max_hour_age_of_measurement)
-        # Implementing measurement health check
-        if not matching_files:
-            self.measurement_health_state = 'red'
+
+        # Check if cached data is older than 15 minutes
+        if self.measurement_data.issuance_time and (
+            (current_date.timestamp() - self.measurement_data.issuance_time)
+            < timedelta(minutes=15).total_seconds()
+        ):
+            use_cached_data = True
         else:
-            # Check if the most recent file_time is more than 1 hour behind current_date
+            matching_files = utils.get_matching_dwd_globalrad_data_files(
+                current_date, max_hour_age_of_measurement
+            )
+
+            # Implementing measurement health check
+            if not matching_files:
+                self.measurement_health_state = "red"
+                _LOGGER.warning(
+                    "No matching files found. Setting measurement health state to red."
+                )
+                return
+
             latest_file_time = max(file_time for _, file_time in matching_files)
             if (current_date - latest_file_time).total_seconds() > 3600:
-                self.measurement_health_state = 'yellow'
+                self.measurement_health_state = "yellow"
             else:
-                self.measurement_health_state = 'green'
-        for file, file_time in matching_files:
-            self.process_file(file, file_time)
+                self.measurement_health_state = "green"
+
+            # Check if the server data is newer than the cached data
+            use_cached_data = (
+                self.measurement_data.latest_file_time
+                and self.measurement_data.latest_file_time >= latest_file_time
+            )
+
+        if use_cached_data:
+            _LOGGER.info(
+                "Using cached measurement data as it is less than 15 minutes old or server data "
+                "is not newer."
+            )
+            self.process_measurements(
+                self.measurement_data.all_grid_measurements, is_cached=True
+            )
+        else:
+            self.reset_all_measurements()
+            self.measurement_data = GlobalMeasurementData()  # Reset the cache
+
+            # Process each file
+            for file, _ in matching_files:  # file_time is no longer needed
+                all_grid_global_rad_data = utils.load_sis_data(file)
+                self.measurement_data.all_grid_measurements.append(
+                    all_grid_global_rad_data
+                )
+                current_issuance_time = (
+                    utils.get_measurement_timestamp_from_netcdf_history_attrib(
+                        all_grid_global_rad_data.history
+                    )
+                )
+
+                # Update cached issuance time and latest file time if they are newer
+                if (self.measurement_data.issuance_time is None) or (
+                    current_issuance_time > self.measurement_data.issuance_time
+                ):
+                    self.measurement_data.issuance_time = current_issuance_time
+                    self.measurement_data.latest_file_time = latest_file_time
+
+                self.process_measurements([all_grid_global_rad_data], is_cached=False)
 
     def reset_all_measurements(self):
         """
         Reset the measurements for all locations.
         """
         for location in self.locations:
             location.measurements = []
 
-    def process_file(self, file, file_time):
+    def process_measurements(self, all_grid_measurements, is_cached):
         """
-        Process each data file for all locations.
+        Process measurement data for all locations.
         """
-        all_grid_global_rad_data = utils.load_sis_data(file)
-        for location in self.locations:
-            self.process_location(location, all_grid_global_rad_data, file_time)
+        for all_grid_global_rad_data in all_grid_measurements:
+            for location in self.locations:
+                if is_cached and location.measurements:
+                    continue  # Do not overwrite existing measurements with cached data
+                self.process_location(location, all_grid_global_rad_data)
 
-    def process_location(self, location, all_grid_global_rad_data, file_time):
+    def process_location(self, location, all_grid_global_rad_data):
         """
         Process each location to handle its measurement updates.
         """
         if not location.measurements:
             self.initialize_measurement_for_location(location, all_grid_global_rad_data)
-        self.update_measurement_for_location(location, all_grid_global_rad_data, file_time)
+        self.update_measurement_for_location(location, all_grid_global_rad_data)
 
     def initialize_measurement_for_location(self, location, all_grid_global_rad_data):
         """
         Initializes measurement for a location based on the nearest grid point.
         """
         latitude, longitude = location.latitude, location.longitude
         grid_data = self._get_grid_data(all_grid_global_rad_data)
-        (nearest_index, nearest_distance, grid_latitude, grid_longitude
-        )= self._get_nearest_grid_point(latitude, longitude, grid_data)
-        measurement = Measurement(grid_latitude, grid_longitude, nearest_distance, nearest_index)
+        (nearest_index, nearest_distance, grid_latitude, grid_longitude) = (
+            self._get_nearest_grid_point(latitude, longitude, grid_data)
+        )
+        measurement = Measurement(
+            grid_latitude, grid_longitude, nearest_distance, nearest_index
+        )
         location.measurements = [measurement]
 
-    def update_measurement_for_location(self, location, all_grid_global_rad_data, file_time):
+    def update_measurement_for_location(self, location, all_grid_global_rad_data):
         """
         Updates the measurement for a given location.
         """
         measurement = location.measurements[0]
-        sis_value = self._get_measurement_value_from_loaded_data(
-            all_grid_global_rad_data, measurement.nearest_index)
-        measurement.add_measurement_value(file_time.timestamp(), sis_value)
+        timestamp, sis_value = self._get_measurement_value_from_loaded_data(
+            all_grid_global_rad_data, measurement.nearest_index
+        )
+        measurement.add_measurement_value(timestamp, sis_value)
 
     def fetch_forecasts(self):
         """
         Fetches and processes global radiation forecast data for each location stored
         in the object's locations list.
 
         This function retrieves forecast data from a dataset for the current date,
@@ -584,28 +585,59 @@
         The function retrieves the forecast data using utility functions that handle
         dataset loading and
         timestamp extraction. Each forecast includes metadata such as standard names, long names,
         and units, and forecasts are only added if their timestamp is greater than
         the current timestamp.
         """
         current_date = datetime.now(dtbase.UTC)
-        self.last_forecast_fetch_date = current_date
-        all_grid_forecasts, _actualhoursbehind = utils.load_forecast_dataset(
-            current_date
-        )
-        # Check forecast data availability and timeliness
-        if utils.is_dataset_empty(all_grid_forecasts):
-            self.forecast_health_state = 'red'
-            return  # Stop processing as no data is available
-
-        # Check the timeliness of the data
-        if _actualhoursbehind > 1:
-            self.forecast_health_state = 'yellow'
+
+        # Check if we need to fetch new forecasts
+        if (
+            self.forecast_data.issuance_time
+            and (current_date.timestamp() - self.forecast_data.issuance_time)
+            < timedelta(hours=1).total_seconds()
+        ):
+            _LOGGER.info("Using cached forecast data as it is less than 1 hour old.")
+            all_grid_forecasts = self.forecast_data.all_grid_forecasts
         else:
-            self.forecast_health_state = 'green'
+            self.last_forecast_fetch_date = current_date
+            all_grid_forecasts, _actualhoursbehind = utils.load_forecast_dataset(
+                current_date
+            )
+
+            # Check forecast data availability and timeliness
+            if utils.is_dataset_empty(all_grid_forecasts):
+                self.forecast_health_state = "red"
+                _LOGGER.warning(
+                    "Forecast data is empty. Setting forecast health state to red."
+                )
+                return  # Stop processing as no data is available
+
+            # Check the timeliness of the data
+            if _actualhoursbehind > 1:
+                self.forecast_health_state = "yellow"
+                _LOGGER.warning(
+                    "Forecast data is %s hours behind. "
+                    "Setting forecast health state to yellow.",
+                    _actualhoursbehind,
+                )
+            else:
+                self.forecast_health_state = "green"
+                _LOGGER.info(
+                    "Forecast data is up to date. Setting forecast health state to green."
+                )
+
+            # Update the cached forecast data
+            global_issuance_time = (
+                utils.get_forecast_issuance_timestamp_from_netcdf_history_attrib(
+                    all_grid_forecasts.history
+                )
+            )
+            self.forecast_data.issuance_time = global_issuance_time
+            self.forecast_data.all_grid_forecasts = all_grid_forecasts
 
         for location in self.locations:
             latitude = location.latitude
             longitude = location.longitude
             selected_data = all_grid_forecasts.sel(
                 lon=longitude, lat=latitude, method="nearest"
             )
```

### Comparing `dwd_global_radiation-1.0.0rc8/dwd_global_radiation/utils.py` & `dwd_global_radiation-1.1.0rc1/dwd_global_radiation/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 """Module providing helper functions for the dwd-global-radiation main module"""
+
 from dataclasses import dataclass
 from datetime import datetime, timezone, timedelta
 import calendar
 import re
 from urllib.error import URLError
 import requests
 import numpy as np
 import xarray as xr
 from bs4 import BeautifulSoup
+
 # pylint: disable=no-name-in-module
 from netCDF4 import Dataset
+
 # pylint: enable=no-name-in-module
 import pytz
 
-MAX_HOURS_TO_GO_BACK=10
-HOURLY_MINUTE_TO_FETCH_NEW_FILE=15
-DWD_GLOBAL_RAD_DATA_BASE_URL='https://opendata.dwd.de/weather/satellite/radiation/sis/'
+MAX_HOURS_TO_GO_BACK = 10
+HOURLY_MINUTE_TO_FETCH_NEW_FILE = 15
+DWD_GLOBAL_RAD_DATA_BASE_URL = (
+    "https://opendata.dwd.de/weather/satellite/radiation/sis/"
+)
+
 
 @dataclass
 class FileParsingContext:
     """
     A context container for storing and passing data required for parsing files
     containing global radiation data from DWD (Deutscher Wetterdienst).
 
@@ -37,21 +43,23 @@
                            extracted from the file names.
 
     This context is used to encapsulate the necessary state and parameters used during the
     file processing in functions such as `process_response_content`, `parse_pre_text`, and
     `process_line`. It helps streamline the passage of multiple related parameters between
     these functions and simplifies managing their state.
     """
+
     regex_pattern: str
     regex_pattern_measurement_time: str
     current_utc_date: datetime
     max_age_hours: int
     file_links: list
     file_times: list
 
+
 def get_current_solar_radiation_forecast_url(hourstogoback, current_date):
     """
     Generates a URL to fetch the solar radiation forecast from the DWD (Deutscher Wetterdienst)
     OpenData server. The URL is constructed based on a specified `current_date` adjusted by
     a certain number of hours to go back (`hourstogoback`). This function handles edge cases
     around the beginning of months, years, and midnight hours to correctly wrap the date
     and time for the forecast URL.
@@ -70,58 +78,73 @@
     adjusts the `current_date` by subtracting the hours specified by `hourstogoback`. It handles
     special cases at the start of months and years where the date and time would otherwise roll
     over incorrectly. Adjustments are made to ensure the date and time specified in the URL
     represent a valid and existing time, particularly just before the rollover of the day, month,
     or year at midnight. The URL follows a specific pattern to match the directory and file
     structure on the DWD OpenData server.
     """
-    target_date=current_date - timedelta(hours=hourstogoback)
-    target_year=target_date.year
-    target_month=target_date.month
-    target_day=target_date.day
-    target_hour=target_date.hour
-    target_minute=target_date.minute
-
-    if (target_month == 1 and target_day == 1 and target_hour == 0 and
-        target_minute < HOURLY_MINUTE_TO_FETCH_NEW_FILE):
-        target_year= target_year - 1
-        target_month=12
-        target_day=31
-        target_hour=23
-    elif target_day == 1 and target_hour == 0 and target_minute < HOURLY_MINUTE_TO_FETCH_NEW_FILE:
-        target_month=target_month -1
-        target_hour=23
-        if target_month in [1,3,5,7,8,10,12]:
-            target_day=31
-        elif target_month in [4,6,9,11]:
-            target_day=30
+    target_date = current_date - timedelta(hours=hourstogoback)
+    target_year = target_date.year
+    target_month = target_date.month
+    target_day = target_date.day
+    target_hour = target_date.hour
+    target_minute = target_date.minute
+
+    if (
+        target_month == 1
+        and target_day == 1
+        and target_hour == 0
+        and target_minute < HOURLY_MINUTE_TO_FETCH_NEW_FILE
+    ):
+        target_year = target_year - 1
+        target_month = 12
+        target_day = 31
+        target_hour = 23
+    elif (
+        target_day == 1
+        and target_hour == 0
+        and target_minute < HOURLY_MINUTE_TO_FETCH_NEW_FILE
+    ):
+        target_month = target_month - 1
+        target_hour = 23
+        if target_month in [1, 3, 5, 7, 8, 10, 12]:
+            target_day = 31
+        elif target_month in [4, 6, 9, 11]:
+            target_day = 30
         else:
             if calendar.is_leap():
-                target_day=29
+                target_day = 29
             else:
-                target_day=28
+                target_day = 28
     elif target_hour == 0 and target_minute < HOURLY_MINUTE_TO_FETCH_NEW_FILE:
         target_day = target_day - 1
-        target_hour=23
+        target_hour = 23
     elif target_minute < HOURLY_MINUTE_TO_FETCH_NEW_FILE:
-        target_hour=target_hour - 1
+        target_hour = target_hour - 1
 
-    str_target_year=str(target_year)
-    str_target_month=f"{target_month:02d}"
-    str_target_day=f"{target_day:02d}"
-    str_target_hour=f"{target_hour:02d}"
-
-    base_url='https://opendata.dwd.de/weather/satellite/radiation/sis/SISfc'
-    url_suffix='_fc%2B18h-DE.nc#mode=bytes'
-
-    url = (base_url + str_target_year + str_target_month + str_target_day +
-           str_target_hour + url_suffix)
+    str_target_year = str(target_year)
+    str_target_month = f"{target_month:02d}"
+    str_target_day = f"{target_day:02d}"
+    str_target_hour = f"{target_hour:02d}"
+
+    base_url = "https://opendata.dwd.de/weather/satellite/radiation/sis/SISfc"
+    url_suffix = "_fc%2B18h-DE.nc#mode=bytes"
+
+    url = (
+        base_url
+        + str_target_year
+        + str_target_month
+        + str_target_day
+        + str_target_hour
+        + url_suffix
+    )
 
     return url
 
+
 def haversine(lat1, lon1, lat2, lon2):
     """
     Calculate the great-circle distance between two points on the Earth's surface given their
     latitude and longitude using the Haversine formula.
 
     Parameters:
         lat1 (float): Latitude of the first point in decimal degrees.
@@ -154,19 +177,20 @@
     lon1, lat1, lon2, lat2 = map(np.radians, [lon1, lat1, lon2, lat2])
 
     # Differenz der Koordinaten
     dlon = lon2 - lon1
     dlat = lat2 - lat1
 
     # Haversine-Formel
-    a = np.sin(dlat/2.0)**2 + np.cos(lat1) * np.cos(lat2) * np.sin(dlon/2.0)**2
+    a = np.sin(dlat / 2.0) ** 2 + np.cos(lat1) * np.cos(lat2) * np.sin(dlon / 2.0) ** 2
     c = 2 * np.arctan2(np.sqrt(a), np.sqrt(1 - a))
     distance = r * c
     return distance
 
+
 def load_forecast_dataset(current_date, max_hours_to_go_back=MAX_HOURS_TO_GO_BACK):
     """
     Attempts to load the forecast dataset for a given number of hours
     going back from the current date.
 
     Args:
         current_date (datetime): The current date and time.
@@ -194,14 +218,15 @@
         # the unavailability of the underlying cloud service and move on gracefully.
         # It's up to the class service health attributes of class GlobalRadiation to signal to
         # the end user of this library, that there is a problem with the cloud service.
         pass
 
     return None, None
 
+
 def get_forecast_issuance_timestamp_from_netcdf_history_attrib(history):
     """
     Extracts the forecast issuance timestamp from the 'history' attribute of a NetCDF file,
     which is formatted in a specific string pattern, and converts it to a UNIX timestamp.
 
     Parameters:
         history (str): The 'history' attribute string from a NetCDF file which includes
@@ -219,25 +244,68 @@
 
     Notes:
         The function assumes that the history attribute contains a date-time string formatted
         as 'YYYY-MM-DD,HH:MM'. It is designed to convert this to a datetime object in UTC and
         then to a UNIX timestamp. This timestamp can be used to reference the exact time of the
         forecast's issuance in systems that use UNIX time for scheduling or data alignment.
     """
-    pattern = r'(\d{4}-\d{2}-\d{2},\d{2}:\d{2})'
+    pattern = r"(\d{4}-\d{2}-\d{2},\d{2}:\d{2})"
     match = re.search(pattern, history)
-    dt_object = datetime.strptime(match[0], '%Y-%m-%d,%H:%M')
+    dt_object = datetime.strptime(match[0], "%Y-%m-%d,%H:%M")
     # Setzen der Zeitzone auf UTC
     dt_object_utc = dt_object.replace(tzinfo=timezone.utc)
 
     # Konvertieren des datetime-Objekts in einen Unix-Zeitstempel
     timestamp = dt_object_utc.timestamp()
 
     return timestamp
 
+
+def get_measurement_timestamp_from_netcdf_history_attrib(history):
+    """
+    Extracts the measurement timestamp from the 'history' attribute of a NetCDF file,
+    which is formatted as 'Mon May 27 16:03:17 2024', and converts it to a UNIX timestamp.
+
+    Parameters:
+        history (str): The 'history' attribute string from a NetCDF file which includes
+                       detailed information about the file's creation and processing steps.
+                       The date-time information is embedded in this string and formatted as
+                       'Mon May 27 16:03:17 2024'.
+
+    Returns:
+        float: The UNIX timestamp representing the UTC time of the measurement.
+
+    Example:
+        history = "Mon May 27 16:03:17 2024: cdo -selvar,SIS -sellonlatbox,5,16,46,57 ..."
+        timestamp = get_measurement_timestamp_from_netcdf_history_attrib(history)
+        print(timestamp)  # Outputs the UNIX timestamp for 'Mon May 27 16:03:17 2024' UTC
+
+    Notes:
+        The function assumes that the history attribute contains a date-time string formatted
+        as 'Mon May 27 16:03:17 2024'. It converts this to a datetime object in UTC and then
+        to a UNIX timestamp. This timestamp can be used to reference the exact time of the
+        measurement in systems that use UNIX time for scheduling or data alignment.
+    """
+    pattern = r"\b\w{3}\s\d{2}\s\d{2}:\d{2}:\d{2}\s\d{4}\b"
+    match = re.search(pattern, history)
+
+    if not match:
+        raise ValueError("No valid timestamp found in history attribute")
+
+    # Parse the matched string to a datetime object
+    dt_object = datetime.strptime(match.group(), "%b %d %H:%M:%S %Y")
+    # Set the timezone to UTC
+    dt_object_utc = dt_object.replace(tzinfo=timezone.utc)
+
+    # Convert the datetime object to a Unix timestamp
+    timestamp = dt_object_utc.timestamp()
+
+    return timestamp
+
+
 def get_matching_dwd_globalrad_data_files(current_utc_date=None, max_age_hours=None):
     """
     Retrieves and filters files from the DWD Global Radiation Data Base URL based on the
     provided regex pattern and the age limit defined by `max_age_hours` relative to the
     `current_utc_date`. It returns a sorted list of files that match the criteria.
 
     Parameters:
@@ -262,34 +330,37 @@
 
     Notes:
         This function assumes that the files at the specified base URL conform to specific naming
         conventions suitable for regex matching as defined in the function's parameters. It utilizes
         a context object (`FileParsingContext`) to pass state across helper functions for better
         modularity and readability.
     """
-    regex_pattern = r'^SISin\d{12}DEv3\.nc$'
-    regex_pattern_measurement_time = r'SISin(\d{4})(\d{2})(\d{2})(\d{2})(\d{2})DEv3\.nc'
+    regex_pattern = r"^SISin\d{12}DEv3\.nc$"
+    regex_pattern_measurement_time = r"SISin(\d{4})(\d{2})(\d{2})(\d{2})(\d{2})DEv3\.nc"
     response = requests.get(DWD_GLOBAL_RAD_DATA_BASE_URL, timeout=(10, 10))
     if response.status_code == 200:
         context = FileParsingContext(
             regex_pattern,
             regex_pattern_measurement_time,
             current_utc_date,
             max_age_hours,
             [],
-            []
+            [],
         )
         file_links, file_times = process_response_content(response.content, context)
         if file_links:
-            sorted_files = sorted(zip(file_links, file_times), key=lambda x: x[1], reverse=True)
+            sorted_files = sorted(
+                zip(file_links, file_times), key=lambda x: x[1], reverse=True
+            )
             return sorted_files
         return []
     print("Error:", response.status_code)
     return []
 
+
 def process_response_content(content, context):
     """
     Processes the HTML content retrieved from a URL to extract file links based on predefined
     criteria stored within a context object. This function parses the HTML, identifies `<pre>` tags,
     and extracts their contents for further processing.
 
     Parameters:
@@ -299,35 +370,37 @@
                                       for file links and their timestamps.
 
     Returns:
         tuple: Returns two lists, one of file links and the other of their respective timestamps,
                both of which meet the specified criteria within the context object.
     """
 
-    soup = BeautifulSoup(content, 'html.parser')
-    pre_tags = soup.find_all('pre')
+    soup = BeautifulSoup(content, "html.parser")
+    pre_tags = soup.find_all("pre")
     for pre_tag in pre_tags:
         pre_text = pre_tag.get_text()
         parse_pre_text(pre_text, context)
     return context.file_links, context.file_times
 
+
 def parse_pre_text(pre_text, context):
     """
     Parses text from `<pre>` tags to extract lines that are potentially valid file entries.
     Each line is processed to check against the context's regex pattern and other conditions.
 
     Parameters:
         pre_text (str): The textual content extracted from a `<pre>` tag.
         context (FileParsingContext): The context object carrying regex patterns, date-time info,
                                       and storage for valid file links and timestamps.
     """
-    lines = pre_text.strip().split('\n')
+    lines = pre_text.strip().split("\n")
     for line in lines:
         process_line(line, context)
 
+
 def process_line(line, context):
     """
     Analyzes a single line from the pre-formatted text to determine if it matches the criteria
     for a valid file link.
     If valid, extracts the date and time info, checks against the maximum age,
     and stores the link and timestamp if all conditions are met.
 
@@ -338,31 +411,34 @@
                                       valid file links and timestamps.
 
     Returns:
         None: This function directly modifies the context object based on the line's validity
               and relevancy as per the defined criteria.
     """
     parts = line.strip().split()
-    if len(parts) < 3 or parts[0].endswith('/'):
+    if len(parts) < 3 or parts[0].endswith("/"):
         return
     href = parts[0]
     if not re.match(context.regex_pattern, href):
         return
     try:
         match = re.match(context.regex_pattern_measurement_time, href)
         year, month, day, hour, minute = map(int, match.groups())
         utc_file_date = datetime(year, month, day, hour, minute, tzinfo=pytz.UTC)
-        if context.max_age_hours is not None and (context.current_utc_date - utc_file_date >
-                                                  timedelta(hours=context.max_age_hours)):
+        if context.max_age_hours is not None and (
+            context.current_utc_date - utc_file_date
+            > timedelta(hours=context.max_age_hours)
+        ):
             return
         context.file_links.append(href)
         context.file_times.append(utc_file_date)
     except (ValueError, AttributeError):
         pass  # Ignore lines that do not have a valid date/time format
 
+
 def load_sis_data(filename):
     """
     Constructs a full URL for a given filename and loads the dataset from this URL using the Dataset
     class. The URL is constructed by appending a filename to the predefined base URL and adding a
     suffix to specify the mode of access.
 
     Parameters:
@@ -381,19 +457,20 @@
 
     Notes:
         The function assumes the existence of a global constant 'DWD_GLOBAL_RAD_DATA_BASE_URL'
         which contains the base URL to which filenames and URL parameters are appended.
         The `url_suffix` is used to specify that the data should be accessed in byte mode,
         which is necessary for certain types of binary data files.
     """
-    url_suffix="#mode=bytes"
-    final_url=DWD_GLOBAL_RAD_DATA_BASE_URL + filename + url_suffix
+    url_suffix = "#mode=bytes"
+    final_url = DWD_GLOBAL_RAD_DATA_BASE_URL + filename + url_suffix
     ds = Dataset(final_url)
     return ds
 
+
 def is_dataset_empty(dataset):
     """
     Determine if the provided xarray Dataset is empty.
 
     This function checks if the dataset is None or if all dimensions within the dataset
     have a length of zero, indicating that there are no data entries present.
```

### Comparing `dwd_global_radiation-1.0.0rc8/dwd_global_radiation.egg-info/PKG-INFO` & `dwd_global_radiation-1.1.0rc1/dwd_global_radiation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dwd_global_radiation
-Version: 1.0.0rc8
+Version: 1.1.0rc1
 Summary: Access and analyze DWD global radiation data and forecasts
 Home-page: https://github.com/aschmere/dwd_global_radiation
 Author: Arno Schmerer
 License: MIT
 Keywords: weather meteorology radiation solar forecasting DWD data environmental data climate studies solar energy forecasting
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `dwd_global_radiation-1.0.0rc8/setup.py` & `dwd_global_radiation-1.1.0rc1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='dwd_global_radiation',
-    version='1.0.0rc8',
+    version='1.1.0rc1',
     packages=find_packages(),
     description='Access and analyze DWD global radiation data and forecasts',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/aschmere/dwd_global_radiation',
     author='Arno Schmerer',
     license='MIT',
```

