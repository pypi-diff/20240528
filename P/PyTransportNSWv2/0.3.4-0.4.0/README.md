# Comparing `tmp/pytransportnswv2-0.3.4.tar.gz` & `tmp/pytransportnswv2-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytransportnswv2-0.3.4.tar", last modified: Tue May 21 05:49:41 2024, max compression
+gzip compressed data, was "pytransportnswv2-0.4.0.tar", last modified: Tue May 28 14:30:07 2024, max compression
```

## Comparing `pytransportnswv2-0.3.4.tar` & `pytransportnswv2-0.4.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:49:41.687229 pytransportnswv2-0.3.4/
--rwxr-xr-x   0 runner    (1001) docker     (127)    35149 2024-05-21 05:49:32.000000 pytransportnswv2-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-05-21 05:49:41.687229 pytransportnswv2-0.3.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:49:41.687229 pytransportnswv2-0.3.4/PyTransportNSWv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-05-21 05:49:41.000000 pytransportnswv2-0.3.4/PyTransportNSWv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-21 05:49:41.000000 pytransportnswv2-0.3.4/PyTransportNSWv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 05:49:41.000000 pytransportnswv2-0.3.4/PyTransportNSWv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-21 05:49:41.000000 pytransportnswv2-0.3.4/PyTransportNSWv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-21 05:49:41.000000 pytransportnswv2-0.3.4/PyTransportNSWv2.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     4881 2024-05-21 05:49:32.000000 pytransportnswv2-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:49:41.687229 pytransportnswv2-0.3.4/TransportNSW/
--rwxr-xr-x   0 runner    (1001) docker     (127)    13926 2024-05-21 05:49:32.000000 pytransportnswv2-0.3.4/TransportNSW/TransportNSW.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       86 2024-05-21 05:49:32.000000 pytransportnswv2-0.3.4/TransportNSW/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 05:49:41.687229 pytransportnswv2-0.3.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      823 2024-05-21 05:49:32.000000 pytransportnswv2-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:30:07.370020 pytransportnswv2-0.4.0/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    35149 2024-05-28 14:30:01.000000 pytransportnswv2-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6373 2024-05-28 14:30:07.370020 pytransportnswv2-0.4.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:30:07.370020 pytransportnswv2-0.4.0/PyTransportNSWv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6373 2024-05-28 14:30:07.000000 pytransportnswv2-0.4.0/PyTransportNSWv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-28 14:30:07.000000 pytransportnswv2-0.4.0/PyTransportNSWv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 14:30:07.000000 pytransportnswv2-0.4.0/PyTransportNSWv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-28 14:30:07.000000 pytransportnswv2-0.4.0/PyTransportNSWv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-28 14:30:07.000000 pytransportnswv2-0.4.0/PyTransportNSWv2.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5773 2024-05-28 14:30:01.000000 pytransportnswv2-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:30:07.370020 pytransportnswv2-0.4.0/TransportNSW/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18043 2024-05-28 14:30:01.000000 pytransportnswv2-0.4.0/TransportNSW/TransportNSW.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       86 2024-05-28 14:30:01.000000 pytransportnswv2-0.4.0/TransportNSW/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 14:30:07.370020 pytransportnswv2-0.4.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      823 2024-05-28 14:30:01.000000 pytransportnswv2-0.4.0/setup.py
```

### Comparing `pytransportnswv2-0.3.4/LICENSE` & `pytransportnswv2-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytransportnswv2-0.3.4/PKG-INFO` & `pytransportnswv2-0.4.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: PyTransportNSWv2
-Version: 0.3.4
-Summary: Get detailed per-trip transport information from TransportNSW
-Home-page: https://github.com/andystewart999/TransportNSW
-Author: andystewart999
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: gtfs-realtime-bindings
-Requires-Dist: requests
-
 # TransportNSW
 Python lib to access Transport NSW information.
 
 ## How to Use
 
 ### Get an API Key
 An OpenData account and API key is required to request the data. More information on how to create the free account can be found here:
@@ -29,15 +13,15 @@
 If it's available, the general occupancy level and the latitude and longitude of the selected journey's vehicle (train, bus, etc) will be returned.
 
 ### API Documentation
 The source API details can be found here: https://opendata.transport.nsw.gov.au/sites/default/files/2023-08/Trip%20Planner%20API%20manual-opendataproduction%20v3.2.pdf
 
 ### Parameters
 ```python
-.get_trip(origin_stop_id, destination_stop_id, api_key, [trip_wait_time = 0], [transport_type = 0])
+.get_trip(origin_stop_id, destination_stop_id, api_key, [journey_wait_time = 0], [transport_type = 0], [strict_transport_type = False], [raw_output = False], [journeys_to_return = 1])
 ```
 TransportNSW's trip planner can work better if you use the general location IDs (eg Central Station) rather than a specific Stop ID (eg Central Station, Platform 19) for the destination, depending on the transport type.  Forcing a specific end destination sometimes results in much more complicated trips.  Also note that the API expects (and returns) the Stop IDs as strings, although so far they all appear to be numeric.
 
 ### transport_type filters
 ```
 1: Train
 4: Light rail
@@ -45,29 +29,58 @@
 7: Coach
 9: Ferry
 11: School bus
 99: Walk
 100: Walk
 107: Cycle
 ```
+If you call the function with a `transport_type` filter and set `strict_transport_type` to `True`, only journeys whose **first** leg matches the desired filter will be considered.  Otherwise the filter includes a journey if **any** of the legs includes the desired travel type.
+
+`raw_output` simply returns the entire API response string as JSON, without making any changes to it.
 
 ### Sample Code
 
-The following example will return the next trip that starts from a bus stop in St. Ives (207537) five minutes from now, to Central Station's general stop ID (10101100):
+The following example will return the next trip that starts from Pymble Station (207310) five minutes from now, to Gordon Station (207210).  Note that specific platforms, such as Gordon Station, Platform 3 (207263) haven't been specified so any platform combination will be accepted:
 
 **Code:**
 ```python
 from TransportNSW import TransportNSW
 tnsw = TransportNSW()
 journey = tnsw.get_trip('207537', '10101100', 'YOUR_API_KEY', 5)
 print(journey)
 ```
 **Result:**
-```python
-{"due": 3, "origin_stop_id": "207537", "origin_name": "Mona Vale Rd at Shinfield Ave, St Ives", "departure_time": "2024-05-20T21:59:48Z", "destination_stop_id": "2000338", "destination_name": "Central Station, Platform 18, Sydney", "arrival_time": "2024-05-20T22:47:36Z", "origin_transport_type": "Bus", "origin_transport_name": "Sydney Buses Network", "origin_line_name": "195", "origin_line_name_short": "195", "changes": 1, "occupancy": "MANY_SEATS", "real_time_trip_id": "2096551", "latitude": -33.72665786743164, "longitude": 151.16305541992188}
+
+Unless `raw_output` is `True`, the return output always returns an array of journeys, even if `journeys_to_return` is 1.  The journey array is preceded by how many journeys were requested, and how many were actually returned that contained usable data:
+
+```json
+{
+  "journeys_to_return": 1,
+  "journeys_with_data": 1,
+  "journeys": [
+    {
+      "due": 6,
+      "origin_stop_id": "2073161",
+      "origin_name": "Pymble Station, Platform 1, Pymble",
+      "departure_time": "2024-05-28T22:40:24Z",
+      "destination_stop_id": "207261",
+      "destination_name": "Gordon Station, Platform 1, Gordon",
+      "arrival_time": "2024-05-28T22:42:30Z",
+      "origin_transport_type": "Train",
+      "origin_transport_name": "Sydney Trains Network",
+      "origin_line_name": "T1 North Shore & Western Line",
+      "origin_line_name_short": "T1",
+      "changes": 0,
+      "occupancy": "UNKNOWN",
+      "real_time_trip_id": "161E.1378.133.60.A.8.80758268",
+      "latitude": "n/a",
+      "longitude": "n/a"
+    }
+  ]
+}
 ```
 Fun fact:  TransportNSW's raw API output calls itself JSON, but it uses single quotes for strings in defiance of the JSON standards.  When using this wrapper the output is formatted such that `jq`, for example, is happy with it.
 
 * due: the time (in minutes) before the journey starts
 * origin_stop_id: the specific departure stop id
 * origin_name: the name of the departure location
 * departure_time: the departure time, in UTC
@@ -79,12 +92,11 @@
 * origin_line_name & origin_line_name_short: the full and short names of the journey
 * changes: how many transport changes are needed on the journey
 * occupancy: how full the vehicle is, if available
 * real_time_trip_id: the unique TransportNSW id for that specific journey, if available
 * latitude & longitude: The location of the vehicle, if available
 
 Please note that the origin and destination detail is just that - information about the first and last stops on the journey at the time the request was made.  We don't return any intermediate steps, transport change types etc other than the total number of changes - the assumption is that you'll know the details of your specified trip, you just want to know when the next departure is.  If you need much more detailed information then I recommend that you use the full Transport NSW trip planner website or application.
-Also note that the 'transport_type' filter, if present,  only makes sure that at least one leg of the journey includes that transport type.
 
 ## Thank you
 Thank you Dav0815 for your TransportNSW library that the vast majority of this fork is based on.  I couldn't have done it without you!
 https://github.com/Dav0815/TransportNSW
```

### Comparing `pytransportnswv2-0.3.4/PyTransportNSWv2.egg-info/PKG-INFO` & `pytransportnswv2-0.4.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTransportNSWv2
-Version: 0.3.4
+Version: 0.4.0
 Summary: Get detailed per-trip transport information from TransportNSW
 Home-page: https://github.com/andystewart999/TransportNSW
 Author: andystewart999
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -29,15 +29,15 @@
 If it's available, the general occupancy level and the latitude and longitude of the selected journey's vehicle (train, bus, etc) will be returned.
 
 ### API Documentation
 The source API details can be found here: https://opendata.transport.nsw.gov.au/sites/default/files/2023-08/Trip%20Planner%20API%20manual-opendataproduction%20v3.2.pdf
 
 ### Parameters
 ```python
-.get_trip(origin_stop_id, destination_stop_id, api_key, [trip_wait_time = 0], [transport_type = 0])
+.get_trip(origin_stop_id, destination_stop_id, api_key, [journey_wait_time = 0], [transport_type = 0], [strict_transport_type = False], [raw_output = False], [journeys_to_return = 1])
 ```
 TransportNSW's trip planner can work better if you use the general location IDs (eg Central Station) rather than a specific Stop ID (eg Central Station, Platform 19) for the destination, depending on the transport type.  Forcing a specific end destination sometimes results in much more complicated trips.  Also note that the API expects (and returns) the Stop IDs as strings, although so far they all appear to be numeric.
 
 ### transport_type filters
 ```
 1: Train
 4: Light rail
@@ -45,29 +45,58 @@
 7: Coach
 9: Ferry
 11: School bus
 99: Walk
 100: Walk
 107: Cycle
 ```
+If you call the function with a `transport_type` filter and set `strict_transport_type` to `True`, only journeys whose **first** leg matches the desired filter will be considered.  Otherwise the filter includes a journey if **any** of the legs includes the desired travel type.
+
+`raw_output` simply returns the entire API response string as JSON, without making any changes to it.
 
 ### Sample Code
 
-The following example will return the next trip that starts from a bus stop in St. Ives (207537) five minutes from now, to Central Station's general stop ID (10101100):
+The following example will return the next trip that starts from Pymble Station (207310) five minutes from now, to Gordon Station (207210).  Note that specific platforms, such as Gordon Station, Platform 3 (207263) haven't been specified so any platform combination will be accepted:
 
 **Code:**
 ```python
 from TransportNSW import TransportNSW
 tnsw = TransportNSW()
 journey = tnsw.get_trip('207537', '10101100', 'YOUR_API_KEY', 5)
 print(journey)
 ```
 **Result:**
-```python
-{"due": 3, "origin_stop_id": "207537", "origin_name": "Mona Vale Rd at Shinfield Ave, St Ives", "departure_time": "2024-05-20T21:59:48Z", "destination_stop_id": "2000338", "destination_name": "Central Station, Platform 18, Sydney", "arrival_time": "2024-05-20T22:47:36Z", "origin_transport_type": "Bus", "origin_transport_name": "Sydney Buses Network", "origin_line_name": "195", "origin_line_name_short": "195", "changes": 1, "occupancy": "MANY_SEATS", "real_time_trip_id": "2096551", "latitude": -33.72665786743164, "longitude": 151.16305541992188}
+
+Unless `raw_output` is `True`, the return output always returns an array of journeys, even if `journeys_to_return` is 1.  The journey array is preceded by how many journeys were requested, and how many were actually returned that contained usable data:
+
+```json
+{
+  "journeys_to_return": 1,
+  "journeys_with_data": 1,
+  "journeys": [
+    {
+      "due": 6,
+      "origin_stop_id": "2073161",
+      "origin_name": "Pymble Station, Platform 1, Pymble",
+      "departure_time": "2024-05-28T22:40:24Z",
+      "destination_stop_id": "207261",
+      "destination_name": "Gordon Station, Platform 1, Gordon",
+      "arrival_time": "2024-05-28T22:42:30Z",
+      "origin_transport_type": "Train",
+      "origin_transport_name": "Sydney Trains Network",
+      "origin_line_name": "T1 North Shore & Western Line",
+      "origin_line_name_short": "T1",
+      "changes": 0,
+      "occupancy": "UNKNOWN",
+      "real_time_trip_id": "161E.1378.133.60.A.8.80758268",
+      "latitude": "n/a",
+      "longitude": "n/a"
+    }
+  ]
+}
 ```
 Fun fact:  TransportNSW's raw API output calls itself JSON, but it uses single quotes for strings in defiance of the JSON standards.  When using this wrapper the output is formatted such that `jq`, for example, is happy with it.
 
 * due: the time (in minutes) before the journey starts
 * origin_stop_id: the specific departure stop id
 * origin_name: the name of the departure location
 * departure_time: the departure time, in UTC
@@ -79,12 +108,11 @@
 * origin_line_name & origin_line_name_short: the full and short names of the journey
 * changes: how many transport changes are needed on the journey
 * occupancy: how full the vehicle is, if available
 * real_time_trip_id: the unique TransportNSW id for that specific journey, if available
 * latitude & longitude: The location of the vehicle, if available
 
 Please note that the origin and destination detail is just that - information about the first and last stops on the journey at the time the request was made.  We don't return any intermediate steps, transport change types etc other than the total number of changes - the assumption is that you'll know the details of your specified trip, you just want to know when the next departure is.  If you need much more detailed information then I recommend that you use the full Transport NSW trip planner website or application.
-Also note that the 'transport_type' filter, if present,  only makes sure that at least one leg of the journey includes that transport type.
 
 ## Thank you
 Thank you Dav0815 for your TransportNSW library that the vast majority of this fork is based on.  I couldn't have done it without you!
 https://github.com/Dav0815/TransportNSW
```

### Comparing `pytransportnswv2-0.3.4/TransportNSW/TransportNSW.py` & `pytransportnswv2-0.4.0/TransportNSW/TransportNSW.py`

 * *Files 22% similar despite different names*

```diff
@@ -42,16 +42,19 @@
     # You need to register for both the Trip Planner and Realtime Vehicle Position APIs
 
     def __init__(self):
         """Initialize the data object with default values."""
         self.origin_id = None
         self.destination_id = None
         self.api_key = None
-        self.trip_wait_time = None
+        self.journey_wait_time = None
         self.transport_type = None
+        self.strict_transport_type = None
+        self.raw_output = None
+        self.journeys_to_return = None
         self.info = {
             ATTR_DUE_IN : 'n/a',
             ATTR_ORIGIN_STOP_ID : 'n/a',
             ATTR_ORIGIN_NAME : 'n/a',
             ATTR_DEPARTURE_TIME : 'n/a',
             ATTR_DESTINATION_STOP_ID : 'n/a',
             ATTR_DESTINATION_NAME : 'n/a',
@@ -63,252 +66,320 @@
             ATTR_CHANGES : 'n/a',
             ATTR_OCCUPANCY : 'n/a',
             ATTR_REAL_TIME_TRIP_ID : 'n/a',
             ATTR_LATITUDE : 'n/a',
             ATTR_LONGITUDE : 'n/a'
             }
 
-    def get_trip(self, name_origin, name_destination , api_key, trip_wait_time = 0, transport_type = 0):
+    def get_trip(self, name_origin, name_destination , api_key, journey_wait_time = 0, transport_type = 0, \
+                 strict_transport_type = False, raw_output = False, journeys_to_return = 1):
         """Get the latest data from Transport NSW."""
         fmt = '%Y-%m-%dT%H:%M:%SZ'
 
         self.name_origin = name_origin
         self.destination = name_destination
         self.api_key = api_key
-        self.trip_wait_time = trip_wait_time
+        self.journey_wait_time = journey_wait_time
         self.transport_type = transport_type
+        self.strict_transport_type = strict_transport_type
+        self.raw_output = raw_output
+        self.journeys_to_return = journeys_to_return
 
-        # This query always uses the current date and time - but add in any 'trip_wait_time' minutes
-        now_plus_wait = datetime.now() + timedelta(minutes = trip_wait_time)
+        # This query always uses the current date and time - but add in any 'journey_wait_time' minutes
+        now_plus_wait = datetime.now() + timedelta(minutes = journey_wait_time)
         itdDate = now_plus_wait.strftime('%Y%m%d')
         itdTime = now_plus_wait.strftime('%H%M')
 
-        if transport_type == 0:
-            # We only need to retrieve one trip - a transport type filter hasn't been applied
-            numberOfTrips = 1
-        else:
-            # 5 trips seems like a safe number
-            numberOfTrips = 5
+        # We don't control how many journeys are returned any more, so need to be careful of running out of valid journeys if there is a filter in place, particularly a strict filter
+        # It would be more efficient to return one journey, check if the filter is met and then retrieve the next one via a new query if not, but for now we'll only be making use of the journeys we've been given
 
         # Build the entire URL
         url = \
             'https://api.transport.nsw.gov.au/v1/tp/trip?' \
             'outputFormat=rapidJSON&coordOutputFormat=EPSG%3A4326' \
             '&depArrMacro=dep&itdDate=' + itdDate + '&itdTime=' + itdTime + \
-            '&type_origin=any&name_origin=' + name_origin + \
-            '&type_destination=any&name_destination=' + name_destination + \
-            '&calcNumberOfTrips=' + str(numberOfTrips) + \
+            '&type_origin=any&name_origin=' + self.name_origin + \
+            '&type_destination=any&name_destination=' + self.destination + \
             '&TfNSWTR=true'
+            # '&calcNumberOfTrips=' + str(journeys_to_retrieve) + \
+
 
         auth = 'apikey ' + self.api_key
         header = {'Accept': 'application/json', 'Authorization': auth}
 
         # Send the query and return an error if something goes wrong
         # Otherwise store the response
         try:
             response = requests.get(url, headers=header, timeout=10)
         except:
             logger.warning("Network or Timeout error")
-            return self.info
+            return error_return(self.info, raw_output)
 
-        # If there is no valid request (e.g. http code isn't 200)
-        # log error and return empty object
+        # If we get bad status code, log error and return with n/a or an empty string
         if response.status_code != 200:
             logger.warning("Error with the request sent; check api key")
-            return self.info
+            return error_return(self.info, raw_output)
 
         # Parse the result as a JSON object
         result = response.json()
 
         # The API will always return a valid trip, so it's just a case of grabbing what we need...
         # We're only reporting on the origin and destination, it's out of scope to discuss the specifics of the ENTIRE journey
         # This isn't a route planner, just a 'how long until the next journey I've specified' tool
         # The assumption is that the travelee will know HOW to make the defined journey, they're just asking WHEN it's happening next
         # All we potentially have to do is find the first trip that matches the transport_type filter
 
-        if transport_type == 0:
-            # Just grab the first (and only) trip
-            journey = result['journeys'][0]
-        else:
-            # Look for a trip with a matching class filter in at least one of its legs.  Could possibly be more stringent here, if ANY part of the journey fits the filter, it will be returned.
-            journey = self.find_first_journey(result['journeys'], transport_type)
-
-        if journey is None:
-            logger.warning("No journey information returned")
-            return self.info
-
-        if journey['legs'] is None:
-            logger.warning("No journey information returned")
-            return self.info
-
-        legs = journey['legs']
-        first_leg = self.find_first_leg(legs, transport_type)
-        last_leg = self.find_last_leg(legs, transport_type)
-        changes = self.find_changes(legs, transport_type)
-
-        origin = result['journeys'][0]['legs'][first_leg]['origin']
-        # probably tidy this up when we start to get occupancy data back
-        first_stop = result['journeys'][0]['legs'][first_leg]['destination']
-        destination = result['journeys'][0]['legs'][last_leg]['destination']
-        transportation = result['journeys'][0]['legs'][first_leg]['transportation']
-
-
-        # Origin info
-        origin_stop_id = origin['id']
-        origin_name = origin['name']
-        origin_departure_time = origin['departureTimeEstimated']
-
-        # How long until it leaves?
-        due = self.get_due(datetime.strptime(origin_departure_time, fmt))
-
-        # Destination info
-        destination_stop_id = destination['id']
-        destination_name = destination['name']
-        destination_arrival_time = destination['arrivalTimeEstimated']
-
-        # Origin type info - train, bus, etc
-        origin_mode_temp = transportation['product']['class']
-        origin_mode = self.get_mode(origin_mode_temp)
-        origin_mode_name = transportation['product']['name']
-
-        # RealTimeTripID info so we can try and get the current location later
-        realtimetripid = 'n/a'
-        if 'properties' in transportation:
-            if 'RealtimeTripId' in transportation['properties']:
-                realtimetripid = transportation['properties']['RealtimeTripId']
-
-        # Line info
-        origin_line_name_short = "unknown"
-        if 'disassembledName' in transportation:
-            origin_line_name_short = transportation['disassembledName']
-
-        origin_line_name = "unknown"
-        if 'number' in transportation:
-            origin_line_name = transportation['number']
-
-        # Occupancy info, if it's there
-        occupancy = 'UNKNOWN'
-        if 'properties' in first_stop:
-            if 'occupancy' in first_stop['properties']:
-                occupancy = first_stop['properties']['occupancy']
-
-        # Now might be a good time to see if we can also find the latitude and longitude
-        # Using the Realtime Vehicle Positions API
-        latitude = 'n/a'
-        longitude = 'n/a'
-
-        if realtimetripid != 'n/a':
-            # Build the URL
-            url = \
-                'https://api.transport.nsw.gov.au/v1/gtfs/vehiclepos' \
-                 + self.get_url(origin_mode)
-            auth = 'apikey ' + self.api_key
-            header = {'Authorization': auth}
+        if raw_output == True:
+            # Just return the raw output
+            return json.dumps(result)
+            exit
+
+        retrieved_journeys = len(result['journeys'])
+
+        # Loop through the results applying filters where required, and generate the appropriate JSON output including an array of in-scope trips
+        json_output=''
+        found_journeys = 0
+        no_valid_journeys = False
+
+        for current_journey in range (0, retrieved_journeys, 1):
+            if transport_type == 0:
+                # Just grab the next trip
+                journey = result['journeys'][current_journey]
+                next_journey = current_journey + 1
+            else:
+                # Look for a trip with a matching class filter in at least one of its legs.  Either ANY, or the first leg, depending on how strict we're being
+                journey, next_journey = self.find_next_journey(result['journeys'], current_journey, transport_type, strict_transport_type)
+
+            if (journey is None) or (journey['legs']) is None:
+                #We've reached the end
+                no_valid_journeys = True
+                self.info = {
+                    ATTR_DUE_IN : 'n/a',
+                    ATTR_ORIGIN_STOP_ID : 'n/a',
+                    ATTR_ORIGIN_NAME : 'n/a',
+                    ATTR_DEPARTURE_TIME : 'n/a',
+                    ATTR_DESTINATION_STOP_ID : 'n/a',
+                    ATTR_DESTINATION_NAME : 'n/a',
+                    ATTR_ARRIVAL_TIME : 'n/a',
+                    ATTR_ORIGIN_TRANSPORT_TYPE : 'n/a',
+                    ATTR_ORIGIN_TRANSPORT_NAME : 'n/a',
+                    ATTR_ORIGIN_LINE_NAME : 'n/a',
+                    ATTR_ORIGIN_LINE_NAME_SHORT : 'n/a',
+                    ATTR_CHANGES : 'n/a',
+                    ATTR_OCCUPANCY : 'n/a',
+                    ATTR_REAL_TIME_TRIP_ID : 'n/a',
+                    ATTR_LATITUDE : 'n/a',
+                    ATTR_LONGITUDE : 'n/a'
+                }
+            else:
+                legs = journey['legs']
+                first_leg = self.find_first_leg(legs, transport_type, strict_transport_type)
+                last_leg = self.find_last_leg(legs, transport_type, strict_transport_type)
+                changes = self.find_changes(legs, transport_type)
+
+                origin = first_leg['origin']
+                first_stop = first_leg['destination']
+                destination = last_leg['destination']
+                transportation = first_leg['transportation']
+
+
+                # Origin info
+                origin_stop_id = origin['id']
+                origin_name = origin['name']
+                origin_departure_time = origin['departureTimeEstimated']
+
+                # How long until it leaves?
+                due = self.get_due(datetime.strptime(origin_departure_time, fmt))
+
+                # Destination info
+                destination_stop_id = destination['id']
+                destination_name = destination['name']
+                destination_arrival_time = destination['arrivalTimeEstimated']
+
+                # Origin type info - train, bus, etc
+                origin_mode_temp = transportation['product']['class']
+                origin_mode = self.get_mode(origin_mode_temp)
+                origin_mode_name = transportation['product']['name']
+
+                # RealTimeTripID info so we can try and get the current location later
+                realtimetripid = 'n/a'
+                if 'properties' in transportation:
+                    if 'RealtimeTripId' in transportation['properties']:
+                        realtimetripid = transportation['properties']['RealtimeTripId']
+
+                # Line info
+                origin_line_name_short = "unknown"
+                if 'disassembledName' in transportation:
+                    origin_line_name_short = transportation['disassembledName']
+
+                origin_line_name = "unknown"
+                if 'number' in transportation:
+                    origin_line_name = transportation['number']
+
+                # Occupancy info, if it's there
+                occupancy = 'UNKNOWN'
+                if 'properties' in first_stop:
+                    if 'occupancy' in first_stop['properties']:
+                        occupancy = first_stop['properties']['occupancy']
+
+                # Now might be a good time to see if we can also find the latitude and longitude
+                # Using the Realtime Vehicle Positions API
+                latitude = 'n/a'
+                longitude = 'n/a'
+
+                if realtimetripid != 'n/a':
+                    # Build the URL
+                    url = \
+                        'https://api.transport.nsw.gov.au/v1/gtfs/vehiclepos' \
+                         + self.get_url(origin_mode)
+                    auth = 'apikey ' + self.api_key
+                    header = {'Authorization': auth}
+
+                    response = requests.get(url, headers=header, timeout=10)
+
+                    # Only try and process the results if we got a good return code
+                    if response.status_code == 200:
+                        # Search the feed and see if we can find the trip_id
+                        # If we do, capture the latitude and longitude
+
+                        feed = gtfs_realtime_pb2.FeedMessage()
+                        feed.ParseFromString(response.content)
+
+                        # Unfortunately we need to do some mucking about for train-based trip_ids
+                        # Define the appropriate regular expression to search for - usually just the full text
+                        bFindLocation = True
+
+                        if origin_mode == 'Train':
+                            triparray = realtimetripid.split('.')
+                            if len(triparray) == 7:
+                                trip_id_wild = triparray[0] + '.' + triparray[1] + '.' + triparray[2] + '.+.' + triparray[4] + '.' + triparray[5] + '.' + triparray[6]
+                            else:
+                                # Hmm, it's not the right length (this happens rarely) - give up
+                                bFindLocation = False
+                        else:
+                            trip_id_wild = realtimetripid
+
+                        if bFindLocation:
+                            reg = re.compile(trip_id_wild)
+
+                            for entity in feed.entity:
+                                if bool(re.match(reg, entity.vehicle.trip.trip_id)):
+                                    latitude = entity.vehicle.position.latitude
+                                    longitude = entity.vehicle.position.longitude
+                                    # We found it, so break out
+                                    break
+
+                self.info = {
+                    ATTR_DUE_IN: due,
+                    ATTR_ORIGIN_STOP_ID : origin_stop_id,
+                    ATTR_ORIGIN_NAME : origin_name,
+                    ATTR_DEPARTURE_TIME : origin_departure_time,
+                    ATTR_DESTINATION_STOP_ID : destination_stop_id,
+                    ATTR_DESTINATION_NAME : destination_name,
+                    ATTR_ARRIVAL_TIME : destination_arrival_time,
+                    ATTR_ORIGIN_TRANSPORT_TYPE : origin_mode,
+                    ATTR_ORIGIN_TRANSPORT_NAME: origin_mode_name,
+                    ATTR_ORIGIN_LINE_NAME : origin_line_name,
+                    ATTR_ORIGIN_LINE_NAME_SHORT : origin_line_name_short,
+                    ATTR_CHANGES: changes,
+                    ATTR_OCCUPANCY : occupancy,
+                    ATTR_REAL_TIME_TRIP_ID : realtimetripid,
+                    ATTR_LATITUDE : latitude,
+                    ATTR_LONGITUDE : longitude
+                    }
+
+                found_journeys = found_journeys + 1
+
+            # Add to the return array
+            if (found_journeys == journeys_to_return) or (no_valid_journeys == True):
+                json_output = json_output + json.dumps(self.info) + ']}'
+                json_output='{"journeys_to_return": ' + str(self.journeys_to_return) + ', "journeys_with_data": ' + str(found_journeys) + ', "journeys": [' + json_output
+                break
+            else:
+                json_output = json_output + json.dumps(self.info) + ', '
+                current_journey = next_journey
+
+        return json_output
+
+
+#    def find_first_journey(self, journeys, journeytype, strictness):
+#        # Find the first journey that has a leg is of the requested type
+#        journey_count = len(journeys)
+#        for journey in range (0, journey_count, 1):
+#            leg = self.find_first_leg(journeys[journey]['legs'], journeytype, strictness)
+#            if leg is not None:
+#                return journeys[journey]
+#
+#        # Hmm, we didn't find one
+#        return None
 
-            response = requests.get(url, headers=header, timeout=10)
 
-            # Only try and process the results if we got a good return code
-            if response.status_code == 200:
-                # Search the feed and see if we can find the trip_id
-                # If we do, capture the latitude and longitude
-
-                feed = gtfs_realtime_pb2.FeedMessage()
-                feed.ParseFromString(response.content)
-
-                # Unfortunately we need to do some mucking about for train-based trip_ids
-                # Define the appropriate regular expression to search for - usually just the full text
-                bFindLocation = True
-
-                if origin_mode == 'Train':
-                    triparray = realtimetripid.split('.')
-                    if len(triparray) == 7:
-                        trip_id_wild = triparray[0] + '.' + triparray[1] + '.' + triparray[2] + '.+.' + triparray[4] + '.' + triparray[5] + '.' + triparray[6]
-                    else:
-                        # Hmm, it's not the right length (this happens rarely) - give up
-                        bFindLocation = False
-                else:
-                    trip_id_wild = realtimetripid
-
-                if bFindLocation:
-                    reg = re.compile(trip_id_wild)
-
-                    for entity in feed.entity:
-                        if bool(re.match(reg, entity.vehicle.trip.trip_id)):
-                            latitude = entity.vehicle.position.latitude
-                            longitude = entity.vehicle.position.longitude
-                            # We found it, so break out
-                            break
+    def find_next_journey(self, journeys, start_journey, journeytype, strict):
+        # Find the next journey that has a leg of the requested type
+        journey_count = len(journeys)
 
-        self.info = {
-            ATTR_DUE_IN: due,
-            ATTR_ORIGIN_STOP_ID : origin_stop_id,
-            ATTR_ORIGIN_NAME : origin_name,
-            ATTR_DEPARTURE_TIME : origin_departure_time,
-            ATTR_DESTINATION_STOP_ID : destination_stop_id,
-            ATTR_DESTINATION_NAME : destination_name,
-            ATTR_ARRIVAL_TIME : destination_arrival_time,
-            ATTR_ORIGIN_TRANSPORT_TYPE : origin_mode,
-            ATTR_ORIGIN_TRANSPORT_NAME: origin_mode_name,
-            ATTR_ORIGIN_LINE_NAME : origin_line_name,
-            ATTR_ORIGIN_LINE_NAME_SHORT : origin_line_name_short,
-            ATTR_CHANGES: changes,
-            ATTR_OCCUPANCY : occupancy,
-            ATTR_REAL_TIME_TRIP_ID : realtimetripid,
-            ATTR_LATITUDE : latitude,
-            ATTR_LONGITUDE : longitude
-            }
-        return json.dumps(self.info)
+        # Some basic error checking
+        if start_journey > journey_count:
+            return None, None
 
-    def find_first_journey(self, journeys, journeytype):
-        # Find the first journey whose first leg is of the requested type
-        journey_count = len(journeys)
-        for journey in range (0, journey_count, 1):
-            leg = self.find_first_leg(journeys[journey]['legs'], journeytype)
+        for journey in range (start_journey, journey_count, 1):
+            leg = self.find_first_leg(journeys[journey]['legs'], journeytype, strict)
             if leg is not None:
-                return journeys[journey]
+                return journeys[journey], journey + 1
+            else:
+                return None, None
 
         # Hmm, we didn't find one
         return None
 
 
-    def find_first_leg(self, legs, legtype):
+    def find_first_leg(self, legs, legtype, strict):
         # Find the first leg of the requested type
         leg_count = len(legs)
         for leg in range (0, leg_count, 1):
             leg_class = legs[leg]['transportation']['product']['class']
 
-            # We've got a filter, and the leg type matches it, so return it
+            # We've got a filter, and the leg type matches it, so return that leg
             if legtype != 0 and leg_class == legtype:
-                return leg
-                
-            # We don't have a filter, and this is the first non-walk/cycle leg so return it
+                return legs[leg]
+
+            # We don't have a filter, and this is the first non-walk/cycle leg so return that leg
             if  legtype == 0 and leg_class < 99:
-                return leg
+                return legs[leg]
+
+            # Exit if we're doing strict filtering and we haven't found that type in the first leg
+            if legtype != 0 and strict == True:
+                return None
 
         # Hmm, we didn't find one
         return None
 
 
-    def find_last_leg(self, legs, legtype):
+    def find_last_leg(self, legs, legtype, strict):
         # Find the last leg of the requested type
         leg_count = len(legs)
         for leg in range (leg_count - 1, -1, -1):
             leg_class = legs[leg]['transportation']['product']['class']
 
-            # We've got a filter, and the leg type matches it, so return it
+            # We've got a filter, and the leg type matches it, so return that leg
             if legtype != 0 and leg_class == legtype:
-                return leg
-                
-            # We don't have a filter, and this is the first non-walk/cycle leg so return it
+                return legs[leg]
+
+            # We don't have a filter, and this is the first non-walk/cycle leg so return that leg
             if  legtype == 0 and leg_class < 99:
-                return leg
+                return legs[leg]
+
+            # Exit if we're doing strict filtering and we haven't found that type in the first leg
+            if legtype != 0 and strict == True:
+                return None
 
         # Hmm, we didn't find one
         return None
 
+
     def find_changes(self, legs, legtype):
         # Find out how often we have to change
         changes = 0
         leg_count = len(legs)
 
         for leg in range (0, leg_count, 1):
             leg_class = legs[leg]['transportation']['product']['class']
```

### Comparing `pytransportnswv2-0.3.4/setup.py` & `pytransportnswv2-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="PyTransportNSWv2",
-    version="0.3.4",
+    version="0.4.0",
     author="andystewart999",
     description="Get detailed per-trip transport information from TransportNSW",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/andystewart999/TransportNSW",
     packages=setuptools.find_packages(),
     install_requires=[
```

