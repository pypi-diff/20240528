# Comparing `tmp/spacestudio-orbit-propagation-1.1.3.tar.gz` & `tmp/spacestudio-orbit-propagation-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacestudio-orbit-propagation-1.1.3.tar", last modified: Tue May 28 12:26:25 2024, max compression
+gzip compressed data, was "spacestudio-orbit-propagation-1.1.4.tar", last modified: Tue May 28 12:40:25 2024, max compression
```

## Comparing `spacestudio-orbit-propagation-1.1.3.tar` & `spacestudio-orbit-propagation-1.1.4.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 12:26:25.879807 spacestudio-orbit-propagation-1.1.3/
--rw-r--r--   0 root         (0) root         (0)      993 2024-05-28 12:26:25.879807 spacestudio-orbit-propagation-1.1.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5635 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/README.md
--rw-r--r--   0 root         (0) root         (0)     2030 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       69 2024-05-28 12:26:25.879807 spacestudio-orbit-propagation-1.1.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2120 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 12:26:25.871808 spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/
--rw-r--r--   0 root         (0) root         (0)     4541 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 12:26:25.871808 spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/api/
--rw-r--r--   0 root         (0) root         (0)      117 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12344 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/api/default_api.py
--rw-r--r--   0 root         (0) root         (0)    26714 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/api_client.py
--rw-r--r--   0 root         (0) root         (0)      652 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/api_response.py
--rw-r--r--   0 root         (0) root         (0)    15088 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/configuration.py
--rw-r--r--   0 root         (0) root         (0)     6254 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 12:26:25.875807 spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/
--rw-r--r--   0 root         (0) root         (0)     3793 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5435 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/advanced_orbit_parameters.py
--rw-r--r--   0 root         (0) root         (0)     3130 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/axis.py
--rw-r--r--   0 root         (0) root         (0)     2973 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/body_solar_array.py
--rw-r--r--   0 root         (0) root         (0)     4412 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/box_spacecraft_geometry.py
--rw-r--r--   0 root         (0) root         (0)     3125 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/circular_altitude_orbit_parameters.py
--rw-r--r--   0 root         (0) root         (0)     3291 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/circular_ground_track_repeated_orbit_parameters.py
--rw-r--r--   0 root         (0) root         (0)     3669 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/deployable_fixed_solar_array.py
--rw-r--r--   0 root         (0) root         (0)     3651 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/deployable_rotating_solar_array.py
--rw-r--r--   0 root         (0) root         (0)     3532 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/drag_perturbation.py
--rw-r--r--   0 root         (0) root         (0)     3237 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/earth_potential_perturbation.py
--rw-r--r--   0 root         (0) root         (0)     3347 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/elliptical_ground_track_repeated_eccentricity_orbit_parameters.py
--rw-r--r--   0 root         (0) root         (0)     3474 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/elliptical_perigee_alt_apogee_alt_orbit_parameters.py
--rw-r--r--   0 root         (0) root         (0)     3251 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/elliptical_perigee_alt_eccentricity_orbit_parameters.py
--rw-r--r--   0 root         (0) root         (0)     2934 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/elliptical_sma_eccentricity_orbit_parameters.py
--rw-r--r--   0 root         (0) root         (0)     1046 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/ephemeris_type.py
--rw-r--r--   0 root         (0) root         (0)     4273 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/orbit.py
--rw-r--r--   0 root         (0) root         (0)     7925 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/orbit_parameters.py
--rw-r--r--   0 root         (0) root         (0)     3663 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/orbit_propagation_request.py
--rw-r--r--   0 root         (0) root         (0)     6660 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/orbit_propagation_request_inputs.py
--rw-r--r--   0 root         (0) root         (0)     3720 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/orbit_propagation_request_outputs.py
--rw-r--r--   0 root         (0) root         (0)     5375 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/orbit_propagation_result.py
--rw-r--r--   0 root         (0) root         (0)     2974 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/orbit_propagation_result_field_indexes_inner.py
--rw-r--r--   0 root         (0) root         (0)     5505 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/perturbation.py
--rw-r--r--   0 root         (0) root         (0)     2958 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/platform.py
--rw-r--r--   0 root         (0) root         (0)     5236 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/solar_array.py
--rw-r--r--   0 root         (0) root         (0)     1131 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/solar_array_face.py
--rw-r--r--   0 root         (0) root         (0)     4848 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/spacecraft_geometry.py
--rw-r--r--   0 root         (0) root         (0)     3419 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/spacecraft_geometry_dimension.py
--rw-r--r--   0 root         (0) root         (0)     3228 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/spherical_spacecraft_geometry.py
--rw-r--r--   0 root         (0) root         (0)     3304 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/srp_perturbation.py
--rw-r--r--   0 root         (0) root         (0)     2818 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/third_body_perturbation.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/py.typed
--rw-r--r--   0 root         (0) root         (0)     9705 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 12:26:25.879807 spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation.egg-info/
--rw-r--r--   0 root         (0) root         (0)      993 2024-05-28 12:26:25.000000 spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4115 2024-05-28 12:26:25.000000 spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 12:26:25.000000 spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       76 2024-05-28 12:26:25.000000 spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2024-05-28 12:26:25.000000 spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 12:26:25.879807 spacestudio-orbit-propagation-1.1.3/test/
--rw-r--r--   0 root         (0) root         (0)     2059 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/test/test_advanced_orbit_parameters.py
--rw-r--r--   0 root         (0) root         (0)     1609 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/test/test_axis.py
--rw-r--r--   0 root         (0) root         (0)     1728 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/test/test_body_solar_array.py
--rw-r--r--   0 root         (0) root         (0)     2228 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/test/test_box_spacecraft_geometry.py
--rw-r--r--   0 root         (0) root         (0)     1889 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/test/test_circular_altitude_orbit_parameters.py
--rw-r--r--   0 root         (0) root         (0)     2061 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/test/test_circular_ground_track_repeated_orbit_parameters.py
--rw-r--r--   0 root         (0) root         (0)     1105 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/test/test_default_api.py
--rw-r--r--   0 root         (0) root         (0)     1997 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/test/test_deployable_fixed_solar_array.py
--rw-r--r--   0 root         (0) root         (0)     2030 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/test/test_deployable_rotating_solar_array.py
--rw-r--r--   0 root         (0) root         (0)     1872 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/test/test_drag_perturbation.py
--rw-r--r--   0 root         (0) root         (0)     1881 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/test/test_earth_potential_perturbation.py
--rw-r--r--   0 root         (0) root         (0)     2230 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/test/test_elliptical_ground_track_repeated_eccentricity_orbit_parameters.py
--rw-r--r--   0 root         (0) root         (0)     2097 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/test/test_elliptical_perigee_alt_apogee_alt_orbit_parameters.py
--rw-r--r--   0 root         (0) root         (0)     2091 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/test/test_elliptical_perigee_alt_eccentricity_orbit_parameters.py
--rw-r--r--   0 root         (0) root         (0)     1965 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/test/test_elliptical_sma_eccentricity_orbit_parameters.py
--rw-r--r--   0 root         (0) root         (0)     1001 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/test/test_ephemeris_type.py
--rw-r--r--   0 root         (0) root         (0)     2215 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/test/test_orbit.py
--rw-r--r--   0 root         (0) root         (0)     1716 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/test/test_orbit_parameters.py
--rw-r--r--   0 root         (0) root         (0)     3805 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/test/test_orbit_propagation_request.py
--rw-r--r--   0 root         (0) root         (0)     3271 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/test/test_orbit_propagation_request_inputs.py
--rw-r--r--   0 root         (0) root         (0)     2057 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/test/test_orbit_propagation_request_outputs.py
--rw-r--r--   0 root         (0) root         (0)     2519 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/test/test_orbit_propagation_result.py
--rw-r--r--   0 root         (0) root         (0)     2007 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/test/test_orbit_propagation_result_field_indexes_inner.py
--rw-r--r--   0 root         (0) root         (0)     1655 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/test/test_perturbation.py
--rw-r--r--   0 root         (0) root         (0)     1606 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/test/test_platform.py
--rw-r--r--   0 root         (0) root         (0)     1632 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/test/test_solar_array.py
--rw-r--r--   0 root         (0) root         (0)     1009 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/test/test_solar_array_face.py
--rw-r--r--   0 root         (0) root         (0)     1733 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/test/test_spacecraft_geometry.py
--rw-r--r--   0 root         (0) root         (0)     1887 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/test/test_spacecraft_geometry_dimension.py
--rw-r--r--   0 root         (0) root         (0)     1855 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/test/test_spherical_spacecraft_geometry.py
--rw-r--r--   0 root         (0) root         (0)     1853 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/test/test_srp_perturbation.py
--rw-r--r--   0 root         (0) root         (0)     1735 2024-05-28 12:26:18.000000 spacestudio-orbit-propagation-1.1.3/test/test_third_body_perturbation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 12:40:25.242436 spacestudio-orbit-propagation-1.1.4/
+-rw-r--r--   0 root         (0) root         (0)     1082 2024-05-28 12:40:25.242436 spacestudio-orbit-propagation-1.1.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6010 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/README.md
+-rw-r--r--   0 root         (0) root         (0)     2030 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       69 2024-05-28 12:40:25.242436 spacestudio-orbit-propagation-1.1.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2274 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 12:40:25.238436 spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/
+-rw-r--r--   0 root         (0) root         (0)     4606 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 12:40:25.238436 spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/api/
+-rw-r--r--   0 root         (0) root         (0)      117 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13015 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/api/default_api.py
+-rw-r--r--   0 root         (0) root         (0)    26779 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/api_client.py
+-rw-r--r--   0 root         (0) root         (0)      652 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/api_response.py
+-rw-r--r--   0 root         (0) root         (0)    15153 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     6319 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 12:40:25.238436 spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/
+-rw-r--r--   0 root         (0) root         (0)     3858 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5500 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/advanced_orbit_parameters.py
+-rw-r--r--   0 root         (0) root         (0)     3195 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/axis.py
+-rw-r--r--   0 root         (0) root         (0)     3038 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/body_solar_array.py
+-rw-r--r--   0 root         (0) root         (0)     4477 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/box_spacecraft_geometry.py
+-rw-r--r--   0 root         (0) root         (0)     3190 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/circular_altitude_orbit_parameters.py
+-rw-r--r--   0 root         (0) root         (0)     3356 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/circular_ground_track_repeated_orbit_parameters.py
+-rw-r--r--   0 root         (0) root         (0)     3734 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/deployable_fixed_solar_array.py
+-rw-r--r--   0 root         (0) root         (0)     3716 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/deployable_rotating_solar_array.py
+-rw-r--r--   0 root         (0) root         (0)     3597 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/drag_perturbation.py
+-rw-r--r--   0 root         (0) root         (0)     3302 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/earth_potential_perturbation.py
+-rw-r--r--   0 root         (0) root         (0)     3412 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/elliptical_ground_track_repeated_eccentricity_orbit_parameters.py
+-rw-r--r--   0 root         (0) root         (0)     3539 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/elliptical_perigee_alt_apogee_alt_orbit_parameters.py
+-rw-r--r--   0 root         (0) root         (0)     3316 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/elliptical_perigee_alt_eccentricity_orbit_parameters.py
+-rw-r--r--   0 root         (0) root         (0)     2999 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/elliptical_sma_eccentricity_orbit_parameters.py
+-rw-r--r--   0 root         (0) root         (0)     1111 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/ephemeris_type.py
+-rw-r--r--   0 root         (0) root         (0)     4338 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/orbit.py
+-rw-r--r--   0 root         (0) root         (0)     7990 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/orbit_parameters.py
+-rw-r--r--   0 root         (0) root         (0)     3728 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/orbit_propagation_request.py
+-rw-r--r--   0 root         (0) root         (0)     6736 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/orbit_propagation_request_inputs.py
+-rw-r--r--   0 root         (0) root         (0)     3822 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/orbit_propagation_request_outputs.py
+-rw-r--r--   0 root         (0) root         (0)     5440 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/orbit_propagation_result.py
+-rw-r--r--   0 root         (0) root         (0)     3039 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/orbit_propagation_result_field_indexes_inner.py
+-rw-r--r--   0 root         (0) root         (0)     5570 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/perturbation.py
+-rw-r--r--   0 root         (0) root         (0)     3023 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/platform.py
+-rw-r--r--   0 root         (0) root         (0)     5301 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/solar_array.py
+-rw-r--r--   0 root         (0) root         (0)     1196 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/solar_array_face.py
+-rw-r--r--   0 root         (0) root         (0)     4959 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/spacecraft_geometry.py
+-rw-r--r--   0 root         (0) root         (0)     3484 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/spacecraft_geometry_dimension.py
+-rw-r--r--   0 root         (0) root         (0)     3293 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/spherical_spacecraft_geometry.py
+-rw-r--r--   0 root         (0) root         (0)     3369 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/srp_perturbation.py
+-rw-r--r--   0 root         (0) root         (0)     2883 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/third_body_perturbation.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/py.typed
+-rw-r--r--   0 root         (0) root         (0)     9770 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 12:40:25.242436 spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1082 2024-05-28 12:40:25.000000 spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4115 2024-05-28 12:40:25.000000 spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 12:40:25.000000 spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       76 2024-05-28 12:40:25.000000 spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2024-05-28 12:40:25.000000 spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 12:40:25.242436 spacestudio-orbit-propagation-1.1.4/test/
+-rw-r--r--   0 root         (0) root         (0)     2124 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/test/test_advanced_orbit_parameters.py
+-rw-r--r--   0 root         (0) root         (0)     1674 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/test/test_axis.py
+-rw-r--r--   0 root         (0) root         (0)     1793 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/test/test_body_solar_array.py
+-rw-r--r--   0 root         (0) root         (0)     2293 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/test/test_box_spacecraft_geometry.py
+-rw-r--r--   0 root         (0) root         (0)     1954 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/test/test_circular_altitude_orbit_parameters.py
+-rw-r--r--   0 root         (0) root         (0)     2126 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/test/test_circular_ground_track_repeated_orbit_parameters.py
+-rw-r--r--   0 root         (0) root         (0)     1158 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/test/test_default_api.py
+-rw-r--r--   0 root         (0) root         (0)     2062 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/test/test_deployable_fixed_solar_array.py
+-rw-r--r--   0 root         (0) root         (0)     2095 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/test/test_deployable_rotating_solar_array.py
+-rw-r--r--   0 root         (0) root         (0)     1937 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/test/test_drag_perturbation.py
+-rw-r--r--   0 root         (0) root         (0)     1946 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/test/test_earth_potential_perturbation.py
+-rw-r--r--   0 root         (0) root         (0)     2295 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/test/test_elliptical_ground_track_repeated_eccentricity_orbit_parameters.py
+-rw-r--r--   0 root         (0) root         (0)     2162 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/test/test_elliptical_perigee_alt_apogee_alt_orbit_parameters.py
+-rw-r--r--   0 root         (0) root         (0)     2156 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/test/test_elliptical_perigee_alt_eccentricity_orbit_parameters.py
+-rw-r--r--   0 root         (0) root         (0)     2030 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/test/test_elliptical_sma_eccentricity_orbit_parameters.py
+-rw-r--r--   0 root         (0) root         (0)     1066 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/test/test_ephemeris_type.py
+-rw-r--r--   0 root         (0) root         (0)     2280 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/test/test_orbit.py
+-rw-r--r--   0 root         (0) root         (0)     1781 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/test/test_orbit_parameters.py
+-rw-r--r--   0 root         (0) root         (0)     3870 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/test/test_orbit_propagation_request.py
+-rw-r--r--   0 root         (0) root         (0)     3336 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/test/test_orbit_propagation_request_inputs.py
+-rw-r--r--   0 root         (0) root         (0)     2122 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/test/test_orbit_propagation_request_outputs.py
+-rw-r--r--   0 root         (0) root         (0)     2584 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/test/test_orbit_propagation_result.py
+-rw-r--r--   0 root         (0) root         (0)     2072 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/test/test_orbit_propagation_result_field_indexes_inner.py
+-rw-r--r--   0 root         (0) root         (0)     1720 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/test/test_perturbation.py
+-rw-r--r--   0 root         (0) root         (0)     1671 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/test/test_platform.py
+-rw-r--r--   0 root         (0) root         (0)     1697 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/test/test_solar_array.py
+-rw-r--r--   0 root         (0) root         (0)     1074 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/test/test_solar_array_face.py
+-rw-r--r--   0 root         (0) root         (0)     1798 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/test/test_spacecraft_geometry.py
+-rw-r--r--   0 root         (0) root         (0)     1952 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/test/test_spacecraft_geometry_dimension.py
+-rw-r--r--   0 root         (0) root         (0)     1920 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/test/test_spherical_spacecraft_geometry.py
+-rw-r--r--   0 root         (0) root         (0)     1918 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/test/test_srp_perturbation.py
+-rw-r--r--   0 root         (0) root         (0)     1800 2024-05-28 12:40:18.000000 spacestudio-orbit-propagation-1.1.4/test/test_third_body_perturbation.py
```

### Comparing `spacestudio-orbit-propagation-1.1.3/PKG-INFO` & `spacestudio-orbit-propagation-1.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: spacestudio-orbit-propagation
-Version: 1.1.3
+Version: 1.1.4
 Summary: Spacestudio Orbit Propagation API
 Home-page: 
 Author: OpenAPI Generator community
 Author-email: team@openapitools.org
 License: Exotrail
 Keywords: OpenAPI,OpenAPI-Generator,Spacestudio Orbit Propagation API
 Description-Content-Type: text/markdown
 Requires-Dist: urllib3<2.1.0,>=1.25.3
 Requires-Dist: python-dateutil
 Requires-Dist: pydantic>=2
 Requires-Dist: typing-extensions>=4.7.1
 
-    &lt;b&gt;CHANGELOG&lt;/b&gt; &lt;ul&gt;   &lt;li&gt;&lt;b&gt;1.1.3&lt;/b&gt; - 2024-05-28 - Improve API documentation&lt;/li&gt;   &lt;li&gt;&lt;b&gt;1.1.2&lt;/b&gt; - 2024-05-28 - Improve API documentation&lt;/li&gt;   &lt;li&gt;&lt;b&gt;1.1.1&lt;/b&gt; - 2024-05-28 - Delete &lt;i&gt;NONE&lt;/i&gt; solar array type&lt;/li&gt;   &lt;li&gt;&lt;b&gt;1.1.0&lt;/b&gt; - 2024-05-28 - Add perturbations and refactor API&lt;/li&gt;   &lt;li&gt;&lt;b&gt;1.0.0&lt;/b&gt; - 2024-05-27 - Initial version&lt;/li&gt; &lt;/ul&gt; 
+    &lt;b&gt;CHANGELOG&lt;/b&gt; &lt;ul&gt;   &lt;li&gt;&lt;b&gt;1.1.4&lt;/b&gt; - 2024-05-28 - Improve API documentation&lt;/li&gt;   &lt;li&gt;&lt;b&gt;1.1.3&lt;/b&gt; - 2024-05-28 - Improve API documentation&lt;/li&gt;   &lt;li&gt;&lt;b&gt;1.1.2&lt;/b&gt; - 2024-05-28 - Improve API documentation&lt;/li&gt;   &lt;li&gt;&lt;b&gt;1.1.1&lt;/b&gt; - 2024-05-28 - Delete &lt;i&gt;NONE&lt;/i&gt; solar array type&lt;/li&gt;   &lt;li&gt;&lt;b&gt;1.1.0&lt;/b&gt; - 2024-05-28 - Add perturbations and refactor API&lt;/li&gt;   &lt;li&gt;&lt;b&gt;1.0.0&lt;/b&gt; - 2024-05-27 - Initial version&lt;/li&gt; &lt;/ul&gt;
```

### Comparing `spacestudio-orbit-propagation-1.1.3/README.md` & `spacestudio-orbit-propagation-1.1.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # spacestudio-orbit-propagation
 <b>CHANGELOG</b>
 <ul>
+  <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>
   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>
   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>
   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>
   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>
   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li>
 </ul>
 
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.1.3
-- Package version: 1.1.3
+- API version: 1.1.4
+- Package version: 1.1.4
 - Generator version: 7.7.0-SNAPSHOT
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
@@ -80,33 +81,33 @@
 )
 
 
 # Enter a context with an instance of the API client
 with spacestudio_orbit_propagation.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = spacestudio_orbit_propagation.DefaultApi(api_client)
-    orbit_propagation_request = spacestudio_orbit_propagation.OrbitPropagationRequest() # OrbitPropagationRequest |  (optional)
+    orbit_propagation_request = {"inputs":{"duration":864000,"propagationType":"NUMERICAL","targetDateDefinitionType":"DURATION","initialOrbit":{"sso":false,"inclination":0.5,"sma":"61.1.4","eccentricity":0,"parameters":{"parametersType":"CIRCULAR_ALTITUDE","altitude":"61.1.4"}},"platform":{"mass":112}},"outputs":{"ephemerides":["KEPLERIAN"],"ephemeridesStep":3600,"meanEphemerides":true,"osculatingEphemerides":false}} # OrbitPropagationRequest |  (optional)
 
     try:
-        # Triggers an orbit propagation computation
+        # Orbit propagation computation
         api_response = api_instance.compute_orbit_propagation(orbit_propagation_request=orbit_propagation_request)
         print("The response of DefaultApi->compute_orbit_propagation:\n")
         pprint(api_response)
     except ApiException as e:
         print("Exception when calling DefaultApi->compute_orbit_propagation: %s\n" % e)
 
 ```
 
 ## Documentation for API Endpoints
 
 All URIs are relative to *http://localhost*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
-*DefaultApi* | [**compute_orbit_propagation**](docs/DefaultApi.md#compute_orbit_propagation) | **POST** / | Triggers an orbit propagation computation
+*DefaultApi* | [**compute_orbit_propagation**](docs/DefaultApi.md#compute_orbit_propagation) | **POST** / | Orbit propagation computation
 
 
 ## Documentation For Models
 
  - [AdvancedOrbitParameters](docs/AdvancedOrbitParameters.md)
  - [Axis](docs/Axis.md)
  - [BodySolarArray](docs/BodySolarArray.md)
```

### Comparing `spacestudio-orbit-propagation-1.1.3/pyproject.toml` & `spacestudio-orbit-propagation-1.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spacestudio_orbit_propagation"
-version = "1.1.3"
+version = "1.1.4"
 description = "Spacestudio Orbit Propagation API"
 authors = ["OpenAPI Generator Community <team@openapitools.org>"]
 license = "Exotrail"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "Spacestudio Orbit Propagation API"]
 include = ["spacestudio_orbit_propagation/py.typed"]
```

### Comparing `spacestudio-orbit-propagation-1.1.3/setup.py` & `spacestudio-orbit-propagation-1.1.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from setuptools import setup, find_packages  # noqa: H301
@@ -17,15 +17,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "spacestudio-orbit-propagation"
-VERSION = "1.1.3"
+VERSION = "1.1.4"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3, < 2.1.0",
     "python-dateutil",
     "pydantic >= 2",
     "typing-extensions >= 4.7.1",
 ]
@@ -40,11 +40,11 @@
     keywords=["OpenAPI", "OpenAPI-Generator", "Spacestudio Orbit Propagation API"],
     install_requires=REQUIRES,
     packages=find_packages(exclude=["test", "tests"]),
     include_package_data=True,
     license="Exotrail",
     long_description_content_type='text/markdown',
     long_description="""\
-    &lt;b&gt;CHANGELOG&lt;/b&gt; &lt;ul&gt;   &lt;li&gt;&lt;b&gt;1.1.3&lt;/b&gt; - 2024-05-28 - Improve API documentation&lt;/li&gt;   &lt;li&gt;&lt;b&gt;1.1.2&lt;/b&gt; - 2024-05-28 - Improve API documentation&lt;/li&gt;   &lt;li&gt;&lt;b&gt;1.1.1&lt;/b&gt; - 2024-05-28 - Delete &lt;i&gt;NONE&lt;/i&gt; solar array type&lt;/li&gt;   &lt;li&gt;&lt;b&gt;1.1.0&lt;/b&gt; - 2024-05-28 - Add perturbations and refactor API&lt;/li&gt;   &lt;li&gt;&lt;b&gt;1.0.0&lt;/b&gt; - 2024-05-27 - Initial version&lt;/li&gt; &lt;/ul&gt; 
+    &lt;b&gt;CHANGELOG&lt;/b&gt; &lt;ul&gt;   &lt;li&gt;&lt;b&gt;1.1.4&lt;/b&gt; - 2024-05-28 - Improve API documentation&lt;/li&gt;   &lt;li&gt;&lt;b&gt;1.1.3&lt;/b&gt; - 2024-05-28 - Improve API documentation&lt;/li&gt;   &lt;li&gt;&lt;b&gt;1.1.2&lt;/b&gt; - 2024-05-28 - Improve API documentation&lt;/li&gt;   &lt;li&gt;&lt;b&gt;1.1.1&lt;/b&gt; - 2024-05-28 - Delete &lt;i&gt;NONE&lt;/i&gt; solar array type&lt;/li&gt;   &lt;li&gt;&lt;b&gt;1.1.0&lt;/b&gt; - 2024-05-28 - Add perturbations and refactor API&lt;/li&gt;   &lt;li&gt;&lt;b&gt;1.0.0&lt;/b&gt; - 2024-05-27 - Initial version&lt;/li&gt; &lt;/ul&gt; 
     """,  # noqa: E501
     package_data={"spacestudio_orbit_propagation": ["py.typed"]},
 )
```

### Comparing `spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/__init__.py` & `spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # coding: utf-8
 
 # flake8: noqa
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "1.1.3"
+__version__ = "1.1.4"
 
 # import apis into sdk package
 from spacestudio_orbit_propagation.api.default_api import DefaultApi
 
 # import ApiClient
 from spacestudio_orbit_propagation.api_response import ApiResponse
 from spacestudio_orbit_propagation.api_client import ApiClient
```

### Comparing `spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/api/default_api.py` & `spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/api/default_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
@@ -51,17 +51,17 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> OrbitPropagationResult:
-        """Triggers an orbit propagation computation
+        """Orbit propagation computation
 
-        Triggers an orbit propagation computation
+        Extrapolate an orbit using a numerical or semi-analytical propagator under the effects of perturbations. The semi analytical propagator can be used to efficiently study the evolution of the mean orbital elements  over very long duration (several years).  
 
         :param orbit_propagation_request:
         :type orbit_propagation_request: OrbitPropagationRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -119,17 +119,17 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[OrbitPropagationResult]:
-        """Triggers an orbit propagation computation
+        """Orbit propagation computation
 
-        Triggers an orbit propagation computation
+        Extrapolate an orbit using a numerical or semi-analytical propagator under the effects of perturbations. The semi analytical propagator can be used to efficiently study the evolution of the mean orbital elements  over very long duration (several years).  
 
         :param orbit_propagation_request:
         :type orbit_propagation_request: OrbitPropagationRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -187,17 +187,17 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Triggers an orbit propagation computation
+        """Orbit propagation computation
 
-        Triggers an orbit propagation computation
+        Extrapolate an orbit using a numerical or semi-analytical propagator under the effects of perturbations. The semi analytical propagator can be used to efficiently study the evolution of the mean orbital elements  over very long duration (several years).  
 
         :param orbit_propagation_request:
         :type orbit_propagation_request: OrbitPropagationRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
```

### Comparing `spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/api_client.py` & `spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import datetime
@@ -84,15 +84,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.1.3/python'
+        self.user_agent = 'OpenAPI-Generator/1.1.4/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         pass
```

### Comparing `spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/api_response.py` & `spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/api_response.py`

 * *Files identical despite different names*

### Comparing `spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/configuration.py` & `spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import copy
@@ -373,16 +373,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.1.3\n"\
-               "SDK Package Version: 1.1.3".\
+               "Version of the API: 1.1.4\n"\
+               "SDK Package Version: 1.1.4".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/exceptions.py` & `spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 from typing import Any, Optional
 from typing_extensions import Self
```

### Comparing `spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/__init__.py` & `spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 # flake8: noqa
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 # import models into model package
```

### Comparing `spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/advanced_orbit_parameters.py` & `spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/advanced_orbit_parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/axis.py` & `spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/axis.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/body_solar_array.py` & `spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/body_solar_array.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/box_spacecraft_geometry.py` & `spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/box_spacecraft_geometry.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/circular_altitude_orbit_parameters.py` & `spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/circular_altitude_orbit_parameters.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/circular_ground_track_repeated_orbit_parameters.py` & `spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/circular_ground_track_repeated_orbit_parameters.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/deployable_fixed_solar_array.py` & `spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/deployable_fixed_solar_array.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/deployable_rotating_solar_array.py` & `spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/deployable_rotating_solar_array.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/drag_perturbation.py` & `spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/drag_perturbation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/earth_potential_perturbation.py` & `spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/earth_potential_perturbation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/elliptical_ground_track_repeated_eccentricity_orbit_parameters.py` & `spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/elliptical_ground_track_repeated_eccentricity_orbit_parameters.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/elliptical_perigee_alt_apogee_alt_orbit_parameters.py` & `spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/elliptical_perigee_alt_apogee_alt_orbit_parameters.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/elliptical_perigee_alt_eccentricity_orbit_parameters.py` & `spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/elliptical_perigee_alt_eccentricity_orbit_parameters.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/elliptical_sma_eccentricity_orbit_parameters.py` & `spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/elliptical_sma_eccentricity_orbit_parameters.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/ephemeris_type.py` & `spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/solar_array_face.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import json
 from enum import Enum
 from typing_extensions import Self
 
 
-class EphemerisType(str, Enum):
+class SolarArrayFace(str, Enum):
     """
-    EphemerisType
+    SolarArrayFace
     """
 
     """
     allowed enum values
     """
-    CARTESIAN = 'CARTESIAN'
-    KEPLERIAN = 'KEPLERIAN'
+    PLUS_X = 'PLUS_X'
+    MINUS_X = 'MINUS_X'
+    PLUS_Y = 'PLUS_Y'
+    MINUS_Y = 'MINUS_Y'
+    PLUS_Z = 'PLUS_Z'
+    MINUS_Z = 'MINUS_Z'
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of EphemerisType from a JSON string"""
+        """Create an instance of SolarArrayFace from a JSON string"""
         return cls(json.loads(json_str))
```

### Comparing `spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/orbit.py` & `spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/orbit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/orbit_parameters.py` & `spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/orbit_parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/orbit_propagation_request.py` & `spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/orbit_propagation_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/orbit_propagation_request_inputs.py` & `spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/orbit_propagation_request_inputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
@@ -25,15 +25,15 @@
 from spacestudio_orbit_propagation.models.platform import Platform
 from spacestudio_orbit_propagation.models.spacecraft_geometry import SpacecraftGeometry
 from typing import Optional, Set
 from typing_extensions import Self
 
 class OrbitPropagationRequestInputs(BaseModel):
     """
-    OrbitPropagationRequestInputs
+    The orbit propagation computation inputs
     """ # noqa: E501
     target_date_definition_type: Optional[StrictStr] = Field(default=None, description="The type of target date to use (either DURATION or TARGET_DATE)", alias="targetDateDefinitionType")
     duration: Optional[StrictInt] = Field(default=None, description="The duration of the orbit extrapolation in seconds (if DURATION target date definition type is used)")
     target_date: Optional[datetime] = Field(default=None, description="The target date/time (if TARGET_DATE target date definition type is used)", alias="targetDate")
     propagation_type: Optional[StrictStr] = Field(default=None, description="The type of propagation to use for the computation", alias="propagationType")
     platform: Optional[Platform] = None
     spacecraft_geometry: Optional[SpacecraftGeometry] = Field(default=None, alias="spacecraftGeometry")
```

### Comparing `spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/orbit_propagation_request_outputs.py` & `spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/orbit_propagation_request_outputs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
@@ -21,15 +21,15 @@
 from typing import Any, ClassVar, Dict, List, Optional
 from spacestudio_orbit_propagation.models.ephemeris_type import EphemerisType
 from typing import Optional, Set
 from typing_extensions import Self
 
 class OrbitPropagationRequestOutputs(BaseModel):
     """
-    OrbitPropagationRequestOutputs
+    Configuration of the expected orbit propagation computation outputs
     """ # noqa: E501
     ephemerides: Optional[List[EphemerisType]] = None
     ephemerides_step: Optional[StrictInt] = Field(default=None, description="The step of the ephemerides, in seconds", alias="ephemeridesStep")
     mean_ephemerides: Optional[StrictBool] = Field(default=None, description="Indicates whether the mean ephemerides should be computed", alias="meanEphemerides")
     osculating_ephemerides: Optional[StrictBool] = Field(default=None, description="Indicates whether the osculating ephemerides should be computed", alias="osculatingEphemerides")
     __properties: ClassVar[List[str]] = ["ephemerides", "ephemeridesStep", "meanEphemerides", "osculatingEphemerides"]
```

### Comparing `spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/orbit_propagation_result.py` & `spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/orbit_propagation_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/orbit_propagation_result_field_indexes_inner.py` & `spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/orbit_propagation_result_field_indexes_inner.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/perturbation.py` & `spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/perturbation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/platform.py` & `spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/platform.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/solar_array.py` & `spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/solar_array.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/solar_array_face.py` & `spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/ephemeris_type.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,37 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import json
 from enum import Enum
 from typing_extensions import Self
 
 
-class SolarArrayFace(str, Enum):
+class EphemerisType(str, Enum):
     """
-    SolarArrayFace
+    EphemerisType
     """
 
     """
     allowed enum values
     """
-    PLUS_X = 'PLUS_X'
-    MINUS_X = 'MINUS_X'
-    PLUS_Y = 'PLUS_Y'
-    MINUS_Y = 'MINUS_Y'
-    PLUS_Z = 'PLUS_Z'
-    MINUS_Z = 'MINUS_Z'
+    CARTESIAN = 'CARTESIAN'
+    KEPLERIAN = 'KEPLERIAN'
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of SolarArrayFace from a JSON string"""
+        """Create an instance of EphemerisType from a JSON string"""
         return cls(json.loads(json_str))
```

### Comparing `spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/spacecraft_geometry.py` & `spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/spacecraft_geometry.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
@@ -26,15 +26,15 @@
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     from spacestudio_orbit_propagation.models.box_spacecraft_geometry import BoxSpacecraftGeometry
     from spacestudio_orbit_propagation.models.spherical_spacecraft_geometry import SphericalSpacecraftGeometry
 
 class SpacecraftGeometry(BaseModel):
     """
-    SpacecraftGeometry
+    If drag perturbation is request, the geometry of the spacecraft.
     """ # noqa: E501
     type: Optional[StrictStr] = Field(default=None, description="The type of spacecraft geometry")
     __properties: ClassVar[List[str]] = ["type"]
 
     @field_validator('type')
     def type_validate_enum(cls, value):
         """Validates the enum"""
```

### Comparing `spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/spacecraft_geometry_dimension.py` & `spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/spacecraft_geometry_dimension.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/spherical_spacecraft_geometry.py` & `spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/spherical_spacecraft_geometry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/srp_perturbation.py` & `spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/srp_perturbation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/models/third_body_perturbation.py` & `spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/models/third_body_perturbation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation/rest.py` & `spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
```

### Comparing `spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation.egg-info/PKG-INFO` & `spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: spacestudio-orbit-propagation
-Version: 1.1.3
+Version: 1.1.4
 Summary: Spacestudio Orbit Propagation API
 Home-page: 
 Author: OpenAPI Generator community
 Author-email: team@openapitools.org
 License: Exotrail
 Keywords: OpenAPI,OpenAPI-Generator,Spacestudio Orbit Propagation API
 Description-Content-Type: text/markdown
 Requires-Dist: urllib3<2.1.0,>=1.25.3
 Requires-Dist: python-dateutil
 Requires-Dist: pydantic>=2
 Requires-Dist: typing-extensions>=4.7.1
 
-    &lt;b&gt;CHANGELOG&lt;/b&gt; &lt;ul&gt;   &lt;li&gt;&lt;b&gt;1.1.3&lt;/b&gt; - 2024-05-28 - Improve API documentation&lt;/li&gt;   &lt;li&gt;&lt;b&gt;1.1.2&lt;/b&gt; - 2024-05-28 - Improve API documentation&lt;/li&gt;   &lt;li&gt;&lt;b&gt;1.1.1&lt;/b&gt; - 2024-05-28 - Delete &lt;i&gt;NONE&lt;/i&gt; solar array type&lt;/li&gt;   &lt;li&gt;&lt;b&gt;1.1.0&lt;/b&gt; - 2024-05-28 - Add perturbations and refactor API&lt;/li&gt;   &lt;li&gt;&lt;b&gt;1.0.0&lt;/b&gt; - 2024-05-27 - Initial version&lt;/li&gt; &lt;/ul&gt; 
+    &lt;b&gt;CHANGELOG&lt;/b&gt; &lt;ul&gt;   &lt;li&gt;&lt;b&gt;1.1.4&lt;/b&gt; - 2024-05-28 - Improve API documentation&lt;/li&gt;   &lt;li&gt;&lt;b&gt;1.1.3&lt;/b&gt; - 2024-05-28 - Improve API documentation&lt;/li&gt;   &lt;li&gt;&lt;b&gt;1.1.2&lt;/b&gt; - 2024-05-28 - Improve API documentation&lt;/li&gt;   &lt;li&gt;&lt;b&gt;1.1.1&lt;/b&gt; - 2024-05-28 - Delete &lt;i&gt;NONE&lt;/i&gt; solar array type&lt;/li&gt;   &lt;li&gt;&lt;b&gt;1.1.0&lt;/b&gt; - 2024-05-28 - Add perturbations and refactor API&lt;/li&gt;   &lt;li&gt;&lt;b&gt;1.0.0&lt;/b&gt; - 2024-05-27 - Initial version&lt;/li&gt; &lt;/ul&gt;
```

### Comparing `spacestudio-orbit-propagation-1.1.3/spacestudio_orbit_propagation.egg-info/SOURCES.txt` & `spacestudio-orbit-propagation-1.1.4/spacestudio_orbit_propagation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spacestudio-orbit-propagation-1.1.3/test/test_advanced_orbit_parameters.py` & `spacestudio-orbit-propagation-1.1.4/test/test_advanced_orbit_parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
```

### Comparing `spacestudio-orbit-propagation-1.1.3/test/test_axis.py` & `spacestudio-orbit-propagation-1.1.4/test/test_axis.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
```

### Comparing `spacestudio-orbit-propagation-1.1.3/test/test_body_solar_array.py` & `spacestudio-orbit-propagation-1.1.4/test/test_body_solar_array.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
```

### Comparing `spacestudio-orbit-propagation-1.1.3/test/test_box_spacecraft_geometry.py` & `spacestudio-orbit-propagation-1.1.4/test/test_box_spacecraft_geometry.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
```

### Comparing `spacestudio-orbit-propagation-1.1.3/test/test_circular_altitude_orbit_parameters.py` & `spacestudio-orbit-propagation-1.1.4/test/test_circular_altitude_orbit_parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
```

### Comparing `spacestudio-orbit-propagation-1.1.3/test/test_circular_ground_track_repeated_orbit_parameters.py` & `spacestudio-orbit-propagation-1.1.4/test/test_circular_ground_track_repeated_orbit_parameters.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
```

### Comparing `spacestudio-orbit-propagation-1.1.3/test/test_default_api.py` & `spacestudio-orbit-propagation-1.1.4/test/test_default_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
@@ -25,14 +25,14 @@
 
     def tearDown(self) -> None:
         pass
 
     def test_compute_orbit_propagation(self) -> None:
         """Test case for compute_orbit_propagation
 
-        Triggers an orbit propagation computation
+        Orbit propagation computation
         """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `spacestudio-orbit-propagation-1.1.3/test/test_deployable_fixed_solar_array.py` & `spacestudio-orbit-propagation-1.1.4/test/test_deployable_fixed_solar_array.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
```

### Comparing `spacestudio-orbit-propagation-1.1.3/test/test_deployable_rotating_solar_array.py` & `spacestudio-orbit-propagation-1.1.4/test/test_deployable_rotating_solar_array.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
```

### Comparing `spacestudio-orbit-propagation-1.1.3/test/test_drag_perturbation.py` & `spacestudio-orbit-propagation-1.1.4/test/test_drag_perturbation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
```

### Comparing `spacestudio-orbit-propagation-1.1.3/test/test_earth_potential_perturbation.py` & `spacestudio-orbit-propagation-1.1.4/test/test_earth_potential_perturbation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
```

### Comparing `spacestudio-orbit-propagation-1.1.3/test/test_elliptical_ground_track_repeated_eccentricity_orbit_parameters.py` & `spacestudio-orbit-propagation-1.1.4/test/test_elliptical_ground_track_repeated_eccentricity_orbit_parameters.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
```

### Comparing `spacestudio-orbit-propagation-1.1.3/test/test_elliptical_perigee_alt_apogee_alt_orbit_parameters.py` & `spacestudio-orbit-propagation-1.1.4/test/test_elliptical_perigee_alt_apogee_alt_orbit_parameters.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
```

### Comparing `spacestudio-orbit-propagation-1.1.3/test/test_elliptical_perigee_alt_eccentricity_orbit_parameters.py` & `spacestudio-orbit-propagation-1.1.4/test/test_elliptical_perigee_alt_eccentricity_orbit_parameters.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
```

### Comparing `spacestudio-orbit-propagation-1.1.3/test/test_elliptical_sma_eccentricity_orbit_parameters.py` & `spacestudio-orbit-propagation-1.1.4/test/test_elliptical_sma_eccentricity_orbit_parameters.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
```

### Comparing `spacestudio-orbit-propagation-1.1.3/test/test_ephemeris_type.py` & `spacestudio-orbit-propagation-1.1.4/test/test_ephemeris_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
```

### Comparing `spacestudio-orbit-propagation-1.1.3/test/test_orbit.py` & `spacestudio-orbit-propagation-1.1.4/test/test_orbit.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
```

### Comparing `spacestudio-orbit-propagation-1.1.3/test/test_orbit_parameters.py` & `spacestudio-orbit-propagation-1.1.4/test/test_orbit_parameters.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
```

### Comparing `spacestudio-orbit-propagation-1.1.3/test/test_orbit_propagation_request.py` & `spacestudio-orbit-propagation-1.1.4/test/test_orbit_propagation_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
```

### Comparing `spacestudio-orbit-propagation-1.1.3/test/test_orbit_propagation_request_inputs.py` & `spacestudio-orbit-propagation-1.1.4/test/test_orbit_propagation_request_inputs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
```

### Comparing `spacestudio-orbit-propagation-1.1.3/test/test_orbit_propagation_request_outputs.py` & `spacestudio-orbit-propagation-1.1.4/test/test_orbit_propagation_request_outputs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
```

### Comparing `spacestudio-orbit-propagation-1.1.3/test/test_orbit_propagation_result.py` & `spacestudio-orbit-propagation-1.1.4/test/test_orbit_propagation_result.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
```

### Comparing `spacestudio-orbit-propagation-1.1.3/test/test_orbit_propagation_result_field_indexes_inner.py` & `spacestudio-orbit-propagation-1.1.4/test/test_orbit_propagation_result_field_indexes_inner.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
```

### Comparing `spacestudio-orbit-propagation-1.1.3/test/test_perturbation.py` & `spacestudio-orbit-propagation-1.1.4/test/test_perturbation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
```

### Comparing `spacestudio-orbit-propagation-1.1.3/test/test_platform.py` & `spacestudio-orbit-propagation-1.1.4/test/test_platform.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
```

### Comparing `spacestudio-orbit-propagation-1.1.3/test/test_solar_array.py` & `spacestudio-orbit-propagation-1.1.4/test/test_solar_array.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
```

### Comparing `spacestudio-orbit-propagation-1.1.3/test/test_solar_array_face.py` & `spacestudio-orbit-propagation-1.1.4/test/test_solar_array_face.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
```

### Comparing `spacestudio-orbit-propagation-1.1.3/test/test_spacecraft_geometry.py` & `spacestudio-orbit-propagation-1.1.4/test/test_spacecraft_geometry.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
```

### Comparing `spacestudio-orbit-propagation-1.1.3/test/test_spacecraft_geometry_dimension.py` & `spacestudio-orbit-propagation-1.1.4/test/test_spacecraft_geometry_dimension.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
```

### Comparing `spacestudio-orbit-propagation-1.1.3/test/test_spherical_spacecraft_geometry.py` & `spacestudio-orbit-propagation-1.1.4/test/test_spherical_spacecraft_geometry.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
```

### Comparing `spacestudio-orbit-propagation-1.1.3/test/test_srp_perturbation.py` & `spacestudio-orbit-propagation-1.1.4/test/test_srp_perturbation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
```

### Comparing `spacestudio-orbit-propagation-1.1.3/test/test_third_body_perturbation.py` & `spacestudio-orbit-propagation-1.1.4/test/test_third_body_perturbation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Spacestudio Orbit Propagation API
 
-    <b>CHANGELOG</b> <ul>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
+    <b>CHANGELOG</b> <ul>   <li><b>1.1.4</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.3</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.2</b> - 2024-05-28 - Improve API documentation</li>   <li><b>1.1.1</b> - 2024-05-28 - Delete <i>NONE</i> solar array type</li>   <li><b>1.1.0</b> - 2024-05-28 - Add perturbations and refactor API</li>   <li><b>1.0.0</b> - 2024-05-27 - Initial version</li> </ul> 
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.1.4
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
```

