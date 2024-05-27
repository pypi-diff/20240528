# Comparing `tmp/ourskyai_platform_api-1.3.3676.tar.gz` & `tmp/ourskyai_platform_api-1.3.3678.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ourskyai_platform_api-1.3.3676.tar", max compression
+gzip compressed data, was "ourskyai_platform_api-1.3.3678.tar", max compression
```

## Comparing `ourskyai_platform_api-1.3.3676.tar` & `ourskyai_platform_api-1.3.3678.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0     9968 2024-05-25 16:56:26.235167 ourskyai_platform_api-1.3.3676/README.md
--rw-r--r--   0        0        0     6552 2024-05-25 16:56:29.766942 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/__init__.py
--rw-r--r--   0        0        0      109 2024-05-25 16:56:29.794940 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/api/__init__.py
--rw-r--r--   0        0        0   206365 2024-05-25 16:56:29.862936 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/api/default_api.py
--rw-r--r--   0        0        0    30373 2024-05-25 16:56:29.906933 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/api_client.py
--rw-r--r--   0        0        0      852 2024-05-25 16:56:29.954930 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/api_response.py
--rw-r--r--   0        0        0    14693 2024-05-25 16:56:30.002927 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/configuration.py
--rw-r--r--   0        0        0     5436 2024-05-25 16:56:30.042924 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/exceptions.py
--rw-r--r--   0        0        0     5881 2024-05-25 16:56:30.078922 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/__init__.py
--rw-r--r--   0        0        0      745 2024-05-25 16:56:30.126919 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/camera_mode.py
--rw-r--r--   0        0        0     1907 2024-05-25 16:56:30.178916 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/empty_success.py
--rw-r--r--   0        0        0     1189 2024-05-25 16:56:30.242911 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/filter_type.py
--rw-r--r--   0        0        0     1933 2024-05-25 16:56:30.286909 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/fits_header.py
--rw-r--r--   0        0        0     2158 2024-05-25 16:56:30.342905 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/location.py
--rw-r--r--   0        0        0      777 2024-05-25 16:56:30.390902 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/metric_type.py
--rw-r--r--   0        0        0      750 2024-05-25 16:56:30.434899 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/mount_type.py
--rw-r--r--   0        0        0      890 2024-05-25 16:56:30.486896 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/node_state.py
--rw-r--r--   0        0        0      830 2024-05-25 16:56:30.518894 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/optical_tube_type.py
--rw-r--r--   0        0        0     2407 2024-05-25 16:56:30.602888 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/plate_solve_parameters.py
--rw-r--r--   0        0        0      754 2024-05-25 16:56:30.662885 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/shutter_type.py
--rw-r--r--   0        0        0     1895 2024-05-25 16:56:30.710882 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/successful_create.py
--rw-r--r--   0        0        0      771 2024-05-25 16:56:30.738880 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/tracking_type.py
--rw-r--r--   0        0        0     2622 2024-05-25 16:56:30.786877 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_auto_focus_instruction.py
--rw-r--r--   0        0        0     2366 2024-05-25 16:56:30.838873 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_auto_focus_instruction_coordinates_inner.py
--rw-r--r--   0        0        0     4920 2024-05-25 16:56:30.886870 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_camera.py
--rw-r--r--   0        0        0     2115 2024-05-25 16:56:30.930868 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_client_token.py
--rw-r--r--   0        0        0     2047 2024-05-25 16:56:30.978865 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_complete_observation_request.py
--rw-r--r--   0        0        0     2047 2024-05-25 16:56:31.038861 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_create_image_set_image_request.py
--rw-r--r--   0        0        0     2118 2024-05-25 16:56:31.090857 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_create_image_set_image_response.py
--rw-r--r--   0        0        0     2692 2024-05-25 16:56:31.142854 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_create_image_set_request.py
--rw-r--r--   0        0        0     2302 2024-05-25 16:56:31.186851 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_create_mount_request.py
--rw-r--r--   0        0        0     2071 2024-05-25 16:56:31.230848 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_create_node_controller_artifact_request.py
--rw-r--r--   0        0        0     2710 2024-05-25 16:56:31.282845 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_create_node_diagnostic.py
--rw-r--r--   0        0        0     2715 2024-05-25 16:56:31.330842 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_create_node_diagnostics_request.py
--rw-r--r--   0        0        0     3152 2024-05-25 16:56:31.378839 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_create_node_request.py
--rw-r--r--   0        0        0     2453 2024-05-25 16:56:31.442835 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_create_optical_tube_request.py
--rw-r--r--   0        0        0     2124 2024-05-25 16:56:31.478833 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_diagnostic_instruction.py
--rw-r--r--   0        0        0     2444 2024-05-25 16:56:31.518830 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_elevation_mask_point.py
--rw-r--r--   0        0        0      719 2024-05-25 16:56:31.578826 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_file_type.py
--rw-r--r--   0        0        0     3298 2024-05-25 16:56:31.622824 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_gain_curve.py
--rw-r--r--   0        0        0     2054 2024-05-25 16:56:31.666821 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_gain_curve_point.py
--rw-r--r--   0        0        0     2570 2024-05-25 16:56:31.706818 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_get_instruction_request.py
--rw-r--r--   0        0        0     2370 2024-05-25 16:56:31.738816 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_get_nodes.py
--rw-r--r--   0        0        0     7081 2024-05-25 16:56:31.782813 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_get_or_create_camera_request.py
--rw-r--r--   0        0        0     2330 2024-05-25 16:56:31.818811 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_get_or_create_mount_request.py
--rw-r--r--   0        0        0     2519 2024-05-25 16:56:31.866808 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_get_or_create_optical_tube_request.py
--rw-r--r--   0        0        0     2675 2024-05-25 16:56:31.914805 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_get_plate_solve_catalog_diff_request.py
--rw-r--r--   0        0        0     3985 2024-05-25 16:56:31.962802 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_ground_station_participant.py
--rw-r--r--   0        0        0     3445 2024-05-25 16:56:32.022798 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_image_set.py
--rw-r--r--   0        0        0     5803 2024-05-25 16:56:32.066795 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_image_set_image.py
--rw-r--r--   0        0        0     3763 2024-05-25 16:56:32.102793 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_instruction.py
--rw-r--r--   0        0        0     2400 2024-05-25 16:56:32.150790 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_metric.py
--rw-r--r--   0        0        0     1917 2024-05-25 16:56:32.194787 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_mount.py
--rw-r--r--   0        0        0     4470 2024-05-25 16:56:32.258783 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_node.py
--rw-r--r--   0        0        0      850 2024-05-25 16:56:32.314779 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_node_component_type.py
--rw-r--r--   0        0        0     1963 2024-05-25 16:56:32.362776 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_node_controller_artifact.py
--rw-r--r--   0        0        0     1669 2024-05-25 16:56:32.422773 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_node_diagnostic_type.py
--rw-r--r--   0        0        0     2573 2024-05-25 16:56:32.470770 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_node_with_location.py
--rw-r--r--   0        0        0     5537 2024-05-25 16:56:32.518766 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_observation_instruction.py
--rw-r--r--   0        0        0     2242 2024-05-25 16:56:32.570763 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_optical_tube.py
--rw-r--r--   0        0        0     2135 2024-05-25 16:56:32.602761 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_plate_solve_catalog_file.py
--rw-r--r--   0        0        0     2648 2024-05-25 16:56:32.690755 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_plate_solve_catalog_file_download.py
--rw-r--r--   0        0        0     2054 2024-05-25 16:56:32.742752 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_read_noise_point.py
--rw-r--r--   0        0        0     2401 2024-05-25 16:56:32.794749 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_release.py
--rw-r--r--   0        0        0     2053 2024-05-25 16:56:32.842746 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_setup_action.py
--rw-r--r--   0        0        0     2946 2024-05-25 16:56:32.894742 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_slew_timing.py
--rw-r--r--   0        0        0     2243 2024-05-25 16:56:32.950739 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_slew_timing_interval.py
--rw-r--r--   0        0        0     3601 2024-05-25 16:56:32.994736 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_update_node_components_request.py
--rw-r--r--   0        0        0     6269 2024-05-25 16:56:33.054732 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_update_node_components_request_camera.py
--rw-r--r--   0        0        0     2402 2024-05-25 16:56:33.134727 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_update_node_components_request_mount.py
--rw-r--r--   0        0        0     2591 2024-05-25 16:56:33.190724 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_update_node_components_request_optical_tube.py
--rw-r--r--   0        0        0     4620 2024-05-25 16:56:33.226721 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_update_node_request.py
--rw-r--r--   0        0        0     2525 2024-05-25 16:56:33.266719 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_video_mode_framerate_property.py
--rw-r--r--   0        0        0     2224 2024-05-25 16:56:33.314716 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v2_complete_observation_request.py
--rw-r--r--   0        0        0        0 2024-05-25 16:56:33.350713 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/py.typed
--rw-r--r--   0        0        0    12941 2024-05-25 16:56:33.406710 ourskyai_platform_api-1.3.3676/ourskyai_platform_api/rest.py
--rw-r--r--   0        0        0      751 2024-05-25 16:56:33.458706 ourskyai_platform_api-1.3.3676/pyproject.toml
--rw-r--r--   0        0        0    10945 1970-01-01 00:00:00.000000 ourskyai_platform_api-1.3.3676/PKG-INFO
+-rw-r--r--   0        0        0     9968 2024-05-27 23:24:31.150924 ourskyai_platform_api-1.3.3678/README.md
+-rw-r--r--   0        0        0     6552 2024-05-27 23:24:34.446963 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/__init__.py
+-rw-r--r--   0        0        0      109 2024-05-27 23:24:34.478964 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/api/__init__.py
+-rw-r--r--   0        0        0   206365 2024-05-27 23:24:34.558965 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/api/default_api.py
+-rw-r--r--   0        0        0    30373 2024-05-27 23:24:34.598965 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/api_client.py
+-rw-r--r--   0        0        0      852 2024-05-27 23:24:34.650966 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/api_response.py
+-rw-r--r--   0        0        0    14693 2024-05-27 23:24:34.694966 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/configuration.py
+-rw-r--r--   0        0        0     5436 2024-05-27 23:24:34.738967 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/exceptions.py
+-rw-r--r--   0        0        0     5881 2024-05-27 23:24:34.778967 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/__init__.py
+-rw-r--r--   0        0        0      745 2024-05-27 23:24:34.814968 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/camera_mode.py
+-rw-r--r--   0        0        0     1907 2024-05-27 23:24:34.858968 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/empty_success.py
+-rw-r--r--   0        0        0     1189 2024-05-27 23:24:34.906969 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/filter_type.py
+-rw-r--r--   0        0        0     1933 2024-05-27 23:24:34.986970 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/fits_header.py
+-rw-r--r--   0        0        0     2158 2024-05-27 23:24:35.030970 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/location.py
+-rw-r--r--   0        0        0      777 2024-05-27 23:24:35.070971 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/metric_type.py
+-rw-r--r--   0        0        0      750 2024-05-27 23:24:35.110971 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/mount_type.py
+-rw-r--r--   0        0        0      890 2024-05-27 23:24:35.198972 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/node_state.py
+-rw-r--r--   0        0        0      830 2024-05-27 23:24:35.238973 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/optical_tube_type.py
+-rw-r--r--   0        0        0     2407 2024-05-27 23:24:35.298974 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/plate_solve_parameters.py
+-rw-r--r--   0        0        0      754 2024-05-27 23:24:35.346974 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/shutter_type.py
+-rw-r--r--   0        0        0     1895 2024-05-27 23:24:35.402975 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/successful_create.py
+-rw-r--r--   0        0        0      771 2024-05-27 23:24:35.454975 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/tracking_type.py
+-rw-r--r--   0        0        0     2622 2024-05-27 23:24:35.502976 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_auto_focus_instruction.py
+-rw-r--r--   0        0        0     2366 2024-05-27 23:24:35.550977 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_auto_focus_instruction_coordinates_inner.py
+-rw-r--r--   0        0        0     4920 2024-05-27 23:24:35.602977 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_camera.py
+-rw-r--r--   0        0        0     2115 2024-05-27 23:24:35.650978 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_client_token.py
+-rw-r--r--   0        0        0     2047 2024-05-27 23:24:35.706978 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_complete_observation_request.py
+-rw-r--r--   0        0        0     2047 2024-05-27 23:24:35.766979 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_create_image_set_image_request.py
+-rw-r--r--   0        0        0     2118 2024-05-27 23:24:35.846980 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_create_image_set_image_response.py
+-rw-r--r--   0        0        0     2692 2024-05-27 23:24:35.902981 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_create_image_set_request.py
+-rw-r--r--   0        0        0     2302 2024-05-27 23:24:35.946981 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_create_mount_request.py
+-rw-r--r--   0        0        0     2071 2024-05-27 23:24:36.002982 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_create_node_controller_artifact_request.py
+-rw-r--r--   0        0        0     2710 2024-05-27 23:24:36.046983 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_create_node_diagnostic.py
+-rw-r--r--   0        0        0     2715 2024-05-27 23:24:36.090983 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_create_node_diagnostics_request.py
+-rw-r--r--   0        0        0     3152 2024-05-27 23:24:36.146984 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_create_node_request.py
+-rw-r--r--   0        0        0     2453 2024-05-27 23:24:36.198984 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_create_optical_tube_request.py
+-rw-r--r--   0        0        0     2124 2024-05-27 23:24:36.254985 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_diagnostic_instruction.py
+-rw-r--r--   0        0        0     2444 2024-05-27 23:24:36.378986 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_elevation_mask_point.py
+-rw-r--r--   0        0        0      719 2024-05-27 23:24:36.430987 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_file_type.py
+-rw-r--r--   0        0        0     3298 2024-05-27 23:24:36.474988 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_gain_curve.py
+-rw-r--r--   0        0        0     2054 2024-05-27 23:24:36.550989 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_gain_curve_point.py
+-rw-r--r--   0        0        0     2570 2024-05-27 23:24:36.602989 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_get_instruction_request.py
+-rw-r--r--   0        0        0     2370 2024-05-27 23:24:36.646990 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_get_nodes.py
+-rw-r--r--   0        0        0     7081 2024-05-27 23:24:36.694990 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_get_or_create_camera_request.py
+-rw-r--r--   0        0        0     2330 2024-05-27 23:24:36.746991 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_get_or_create_mount_request.py
+-rw-r--r--   0        0        0     2519 2024-05-27 23:24:36.806992 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_get_or_create_optical_tube_request.py
+-rw-r--r--   0        0        0     2675 2024-05-27 23:24:36.846992 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_get_plate_solve_catalog_diff_request.py
+-rw-r--r--   0        0        0     3985 2024-05-27 23:24:36.894993 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_ground_station_participant.py
+-rw-r--r--   0        0        0     3445 2024-05-27 23:24:36.942993 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_image_set.py
+-rw-r--r--   0        0        0     5803 2024-05-27 23:24:36.986994 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_image_set_image.py
+-rw-r--r--   0        0        0     3763 2024-05-27 23:24:37.034994 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_instruction.py
+-rw-r--r--   0        0        0     2400 2024-05-27 23:24:37.078995 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_metric.py
+-rw-r--r--   0        0        0     1917 2024-05-27 23:24:37.122995 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_mount.py
+-rw-r--r--   0        0        0     4470 2024-05-27 23:24:37.170996 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_node.py
+-rw-r--r--   0        0        0      850 2024-05-27 23:24:37.210996 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_node_component_type.py
+-rw-r--r--   0        0        0     1963 2024-05-27 23:24:37.254997 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_node_controller_artifact.py
+-rw-r--r--   0        0        0     1669 2024-05-27 23:24:37.290998 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_node_diagnostic_type.py
+-rw-r--r--   0        0        0     2573 2024-05-27 23:24:37.354998 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_node_with_location.py
+-rw-r--r--   0        0        0     5537 2024-05-27 23:24:37.398999 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_observation_instruction.py
+-rw-r--r--   0        0        0     2242 2024-05-27 23:24:37.475000 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_optical_tube.py
+-rw-r--r--   0        0        0     2135 2024-05-27 23:24:37.539000 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_plate_solve_catalog_file.py
+-rw-r--r--   0        0        0     2648 2024-05-27 23:24:37.583001 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_plate_solve_catalog_file_download.py
+-rw-r--r--   0        0        0     2054 2024-05-27 23:24:37.647002 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_read_noise_point.py
+-rw-r--r--   0        0        0     2401 2024-05-27 23:24:37.695002 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_release.py
+-rw-r--r--   0        0        0     2053 2024-05-27 23:24:37.759003 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_setup_action.py
+-rw-r--r--   0        0        0     2946 2024-05-27 23:24:37.803004 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_slew_timing.py
+-rw-r--r--   0        0        0     2243 2024-05-27 23:24:37.855004 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_slew_timing_interval.py
+-rw-r--r--   0        0        0     3601 2024-05-27 23:24:37.899005 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_update_node_components_request.py
+-rw-r--r--   0        0        0     6269 2024-05-27 23:24:37.967006 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_update_node_components_request_camera.py
+-rw-r--r--   0        0        0     2402 2024-05-27 23:24:38.011006 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_update_node_components_request_mount.py
+-rw-r--r--   0        0        0     2591 2024-05-27 23:24:38.055007 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_update_node_components_request_optical_tube.py
+-rw-r--r--   0        0        0     4620 2024-05-27 23:24:38.099007 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_update_node_request.py
+-rw-r--r--   0        0        0     2525 2024-05-27 23:24:38.151008 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_video_mode_framerate_property.py
+-rw-r--r--   0        0        0     2224 2024-05-27 23:24:38.179008 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v2_complete_observation_request.py
+-rw-r--r--   0        0        0        0 2024-05-27 23:24:38.207008 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/py.typed
+-rw-r--r--   0        0        0    12941 2024-05-27 23:24:38.271009 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/rest.py
+-rw-r--r--   0        0        0      751 2024-05-27 23:24:38.315010 ourskyai_platform_api-1.3.3678/pyproject.toml
+-rw-r--r--   0        0        0    10945 1970-01-01 00:00:00.000000 ourskyai_platform_api-1.3.3678/PKG-INFO
```

### Comparing `ourskyai_platform_api-1.3.3676/README.md` & `ourskyai_platform_api-1.3.3678/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ourskyai-platform-api
 No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.3.3676
-- Package version: 1.3.3676
+- API version: 1.3.3678
+- Package version: 1.3.3678
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation & Usage
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/__init__.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 # flake8: noqa
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "1.3.3676"
+__version__ = "1.3.3678"
 
 # import apis into sdk package
 from ourskyai_platform_api.api.default_api import DefaultApi
 
 # import ApiClient
 from ourskyai_platform_api.api_response import ApiResponse
 from ourskyai_platform_api.api_client import ApiClient
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/api/default_api.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/api/default_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import re  # noqa: F401
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/api_client.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import atexit
@@ -72,15 +72,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.3.3676/python'
+        self.user_agent = 'OpenAPI-Generator/1.3.3678/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/api_response.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/api_response.py`

 * *Files identical despite different names*

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/configuration.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import copy
@@ -371,16 +371,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.3.3676\n"\
-               "SDK Package Version: 1.3.3676".\
+               "Version of the API: 1.3.3678\n"\
+               "SDK Package Version: 1.3.3678".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/exceptions.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 class OpenApiException(Exception):
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/__init__.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 # import models into model package
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/camera_mode.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/camera_mode.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/empty_success.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/empty_success.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/filter_type.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/filter_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/fits_header.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/fits_header.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/location.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/location.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/metric_type.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/metric_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/mount_type.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/mount_type.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/node_state.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/node_state.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/optical_tube_type.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/optical_tube_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/plate_solve_parameters.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/plate_solve_parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/shutter_type.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/shutter_type.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/successful_create.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/successful_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/tracking_type.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/tracking_type.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_auto_focus_instruction.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_auto_focus_instruction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_auto_focus_instruction_coordinates_inner.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_auto_focus_instruction_coordinates_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_camera.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_camera.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_client_token.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_client_token.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_complete_observation_request.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_complete_observation_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_create_image_set_image_request.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_create_image_set_image_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_create_image_set_image_response.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_create_image_set_image_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_create_image_set_request.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_create_image_set_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_create_mount_request.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_create_mount_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_create_node_controller_artifact_request.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_create_node_controller_artifact_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_create_node_diagnostic.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_create_node_diagnostic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_create_node_diagnostics_request.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_create_node_diagnostics_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_create_node_request.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_create_node_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_create_optical_tube_request.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_create_optical_tube_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_diagnostic_instruction.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_diagnostic_instruction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_elevation_mask_point.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_elevation_mask_point.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_file_type.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_file_type.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_gain_curve.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_gain_curve.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_gain_curve_point.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_gain_curve_point.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_get_instruction_request.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_get_instruction_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_get_nodes.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_get_nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_get_or_create_camera_request.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_get_or_create_camera_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_get_or_create_mount_request.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_get_or_create_mount_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_get_or_create_optical_tube_request.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_get_or_create_optical_tube_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_get_plate_solve_catalog_diff_request.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_get_plate_solve_catalog_diff_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_ground_station_participant.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_ground_station_participant.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_image_set.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_image_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_image_set_image.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_image_set_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_instruction.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_instruction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_metric.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_metric.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_mount.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_mount.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_node.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_node_component_type.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_node_component_type.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_node_controller_artifact.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_node_controller_artifact.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_node_diagnostic_type.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_node_diagnostic_type.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_node_with_location.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_node_with_location.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_observation_instruction.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_observation_instruction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_optical_tube.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_optical_tube.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_plate_solve_catalog_file.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_plate_solve_catalog_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_plate_solve_catalog_file_download.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_plate_solve_catalog_file_download.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_read_noise_point.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_read_noise_point.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_release.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_release.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_setup_action.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_setup_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_slew_timing.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_slew_timing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_slew_timing_interval.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_slew_timing_interval.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_update_node_components_request.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_update_node_components_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_update_node_components_request_camera.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_update_node_components_request_camera.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_update_node_components_request_mount.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_update_node_components_request_mount.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_update_node_components_request_optical_tube.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_update_node_components_request_optical_tube.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_update_node_request.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_update_node_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v1_video_mode_framerate_property.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_video_mode_framerate_property.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/models/v2_complete_observation_request.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v2_complete_observation_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3676/ourskyai_platform_api/rest.py` & `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
```

### Comparing `ourskyai_platform_api-1.3.3676/pyproject.toml` & `ourskyai_platform_api-1.3.3678/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ourskyai_platform_api"
-version = "1.3.3676"
+version = "1.3.3678"
 description = "OurSky Platform"
 authors = ["OpenAPI Generator Community <team@openapitools.org>"]
 license = "NoLicense"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "OurSky Platform"]
 include = ["ourskyai_platform_api/py.typed"]
```

### Comparing `ourskyai_platform_api-1.3.3676/PKG-INFO` & `ourskyai_platform_api-1.3.3678/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ourskyai_platform_api
-Version: 1.3.3676
+Version: 1.3.3678
 Summary: OurSky Platform
 Home-page: https://github.com/GIT_USER_ID/GIT_REPO_ID
 License: NoLicense
 Keywords: OpenAPI,OpenAPI-Generator,OurSky Platform
 Author: OpenAPI Generator Community
 Author-email: team@openapitools.org
 Requires-Python: >=3.7,<4.0
@@ -24,16 +24,16 @@
 Description-Content-Type: text/markdown
 
 # ourskyai-platform-api
 No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.3.3676
-- Package version: 1.3.3676
+- API version: 1.3.3678
+- Package version: 1.3.3678
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation & Usage
```

