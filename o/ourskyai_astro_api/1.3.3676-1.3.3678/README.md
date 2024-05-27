# Comparing `tmp/ourskyai_astro_api-1.3.3676.tar.gz` & `tmp/ourskyai_astro_api-1.3.3678.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ourskyai_astro_api-1.3.3676.tar", max compression
+gzip compressed data, was "ourskyai_astro_api-1.3.3678.tar", max compression
```

## Comparing `ourskyai_astro_api-1.3.3676.tar` & `ourskyai_astro_api-1.3.3678.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0    11541 2024-05-25 16:56:26.175171 ourskyai_astro_api-1.3.3676/README.md
--rw-r--r--   0        0        0     6292 2024-05-25 16:56:29.438963 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/__init__.py
--rw-r--r--   0        0        0      106 2024-05-25 16:56:29.470961 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/api/__init__.py
--rw-r--r--   0        0        0   260295 2024-05-25 16:56:29.546956 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/api/default_api.py
--rw-r--r--   0        0        0    30352 2024-05-25 16:56:29.590953 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/api_client.py
--rw-r--r--   0        0        0      852 2024-05-25 16:56:29.634950 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/api_response.py
--rw-r--r--   0        0        0    14687 2024-05-25 16:56:29.678948 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/configuration.py
--rw-r--r--   0        0        0     5433 2024-05-25 16:56:29.730944 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/exceptions.py
--rw-r--r--   0        0        0     5651 2024-05-25 16:56:29.798940 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/__init__.py
--rw-r--r--   0        0        0      819 2024-05-25 16:56:29.842937 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/asset_file_type.py
--rw-r--r--   0        0        0      931 2024-05-25 16:56:29.886934 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/asset_type.py
--rw-r--r--   0        0        0      809 2024-05-25 16:56:29.942931 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/calibration_master_type.py
--rw-r--r--   0        0        0     2092 2024-05-25 16:56:29.994927 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/daily_weather_city.py
--rw-r--r--   0        0        0     4308 2024-05-25 16:56:30.038925 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/daily_weather_forecast_item.py
--rw-r--r--   0        0        0     2527 2024-05-25 16:56:30.066923 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/daily_weather_forecast_item_temp.py
--rw-r--r--   0        0        0     2551 2024-05-25 16:56:30.114920 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/daily_weather_forecast_item_weather_inner.py
--rw-r--r--   0        0        0     2947 2024-05-25 16:56:30.146918 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/daily_weather_forecast_list_response.py
--rw-r--r--   0        0        0     1904 2024-05-25 16:56:30.202914 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/empty_success.py
--rw-r--r--   0        0        0     1186 2024-05-25 16:56:30.242911 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/filter_type.py
--rw-r--r--   0        0        0     1930 2024-05-25 16:56:30.282909 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/fits_header.py
--rw-r--r--   0        0        0     2155 2024-05-25 16:56:30.322906 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/location.py
--rw-r--r--   0        0        0      747 2024-05-25 16:56:30.374903 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/mount_type.py
--rw-r--r--   0        0        0      887 2024-05-25 16:56:30.426900 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/node_state.py
--rw-r--r--   0        0        0      827 2024-05-25 16:56:30.470897 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/optical_tube_type.py
--rw-r--r--   0        0        0      751 2024-05-25 16:56:30.506895 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/shutter_type.py
--rw-r--r--   0        0        0     1892 2024-05-25 16:56:30.562891 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/successful_create.py
--rw-r--r--   0        0        0      768 2024-05-25 16:56:30.610888 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/tracking_type.py
--rw-r--r--   0        0        0     3258 2024-05-25 16:56:30.658885 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_astro_project.py
--rw-r--r--   0        0        0     3969 2024-05-25 16:56:30.722881 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_astro_project_asset.py
--rw-r--r--   0        0        0     2569 2024-05-25 16:56:30.754879 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_astro_project_asset_metadata.py
--rw-r--r--   0        0        0     2399 2024-05-25 16:56:30.802876 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_astro_project_asset_metadata_color_combination.py
--rw-r--r--   0        0        0     2381 2024-05-25 16:56:30.854873 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_astro_target.py
--rw-r--r--   0        0        0     3640 2024-05-25 16:56:30.902869 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_calibration_master.py
--rw-r--r--   0        0        0     4908 2024-05-25 16:56:30.950866 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_camera.py
--rw-r--r--   0        0        0     2421 2024-05-25 16:56:31.002863 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_create_astro_project_image_set_request.py
--rw-r--r--   0        0        0     2668 2024-05-25 16:56:31.046860 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_create_astro_project_request.py
--rw-r--r--   0        0        0     2121 2024-05-25 16:56:31.086858 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_create_astro_project_response.py
--rw-r--r--   0        0        0     3777 2024-05-25 16:56:31.126855 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_create_calibration_master_request.py
--rw-r--r--   0        0        0     2147 2024-05-25 16:56:31.178852 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_create_calibration_master_response.py
--rw-r--r--   0        0        0     7059 2024-05-25 16:56:31.226849 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_create_camera_request.py
--rw-r--r--   0        0        0     2044 2024-05-25 16:56:31.262847 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_create_image_set_image_request.py
--rw-r--r--   0        0        0     2115 2024-05-25 16:56:31.306844 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_create_image_set_image_response.py
--rw-r--r--   0        0        0     2683 2024-05-25 16:56:31.350841 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_create_image_set_request.py
--rw-r--r--   0        0        0     2296 2024-05-25 16:56:31.426836 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_create_mount_request.py
--rw-r--r--   0        0        0     3146 2024-05-25 16:56:31.502831 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_create_node_request.py
--rw-r--r--   0        0        0     2447 2024-05-25 16:56:31.550828 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_create_optical_tube_request.py
--rw-r--r--   0        0        0     2441 2024-05-25 16:56:31.594825 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_elevation_mask_point.py
--rw-r--r--   0        0        0     3289 2024-05-25 16:56:31.626823 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_gain_curve.py
--rw-r--r--   0        0        0     2051 2024-05-25 16:56:31.670821 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_gain_curve_point.py
--rw-r--r--   0        0        0     2096 2024-05-25 16:56:31.710818 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_get_astro_platform_credit_balance_response.py
--rw-r--r--   0        0        0     2364 2024-05-25 16:56:31.758815 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_get_nodes.py
--rw-r--r--   0        0        0     7066 2024-05-25 16:56:31.802812 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_get_or_create_camera_request.py
--rw-r--r--   0        0        0     2324 2024-05-25 16:56:31.850809 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_get_or_create_mount_request.py
--rw-r--r--   0        0        0     2513 2024-05-25 16:56:31.902806 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_get_or_create_optical_tube_request.py
--rw-r--r--   0        0        0     3436 2024-05-25 16:56:31.946803 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_image_set.py
--rw-r--r--   0        0        0     5797 2024-05-25 16:56:31.994800 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_image_set_image.py
--rw-r--r--   0        0        0      795 2024-05-25 16:56:32.054796 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_job_kind.py
--rw-r--r--   0        0        0     2632 2024-05-25 16:56:32.098793 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_job_log.py
--rw-r--r--   0        0        0      803 2024-05-25 16:56:32.170789 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_job_status.py
--rw-r--r--   0        0        0     1914 2024-05-25 16:56:32.242784 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_mount.py
--rw-r--r--   0        0        0     4458 2024-05-25 16:56:32.282781 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_node.py
--rw-r--r--   0        0        0     2564 2024-05-25 16:56:32.334778 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_node_with_location.py
--rw-r--r--   0        0        0     2239 2024-05-25 16:56:32.378775 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_optical_tube.py
--rw-r--r--   0        0        0     3057 2024-05-25 16:56:32.442771 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_platform_credit.py
--rw-r--r--   0        0        0      870 2024-05-25 16:56:32.490768 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_platform_credit_source.py
--rw-r--r--   0        0        0      800 2024-05-25 16:56:32.538765 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_platform_credit_type.py
--rw-r--r--   0        0        0      776 2024-05-25 16:56:32.590762 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_platform_credit_unit.py
--rw-r--r--   0        0        0     2045 2024-05-25 16:56:32.634759 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_put_stack_astro_project_request.py
--rw-r--r--   0        0        0     2051 2024-05-25 16:56:32.698755 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_read_noise_point.py
--rw-r--r--   0        0        0     2050 2024-05-25 16:56:32.730753 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_setup_action.py
--rw-r--r--   0        0        0     2940 2024-05-25 16:56:32.802748 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_slew_timing.py
--rw-r--r--   0        0        0     2240 2024-05-25 16:56:32.842746 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_slew_timing_interval.py
--rw-r--r--   0        0        0     4605 2024-05-25 16:56:32.894742 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_update_node_request.py
--rw-r--r--   0        0        0     2522 2024-05-25 16:56:32.950739 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_video_mode_framerate_property.py
--rw-r--r--   0        0        0        0 2024-05-25 16:56:32.982737 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/py.typed
--rw-r--r--   0        0        0    12935 2024-05-25 16:56:33.030734 ourskyai_astro_api-1.3.3676/ourskyai_astro_api/rest.py
--rw-r--r--   0        0        0      739 2024-05-25 16:56:33.066732 ourskyai_astro_api-1.3.3676/pyproject.toml
--rw-r--r--   0        0        0    12509 1970-01-01 00:00:00.000000 ourskyai_astro_api-1.3.3676/PKG-INFO
+-rw-r--r--   0        0        0    11541 2024-05-27 23:24:31.142924 ourskyai_astro_api-1.3.3678/README.md
+-rw-r--r--   0        0        0     6292 2024-05-27 23:24:34.594965 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/__init__.py
+-rw-r--r--   0        0        0      106 2024-05-27 23:24:34.622965 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/api/__init__.py
+-rw-r--r--   0        0        0   260295 2024-05-27 23:24:34.698966 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/api/default_api.py
+-rw-r--r--   0        0        0    30352 2024-05-27 23:24:34.742967 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/api_client.py
+-rw-r--r--   0        0        0      852 2024-05-27 23:24:34.798968 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/api_response.py
+-rw-r--r--   0        0        0    14687 2024-05-27 23:24:34.858968 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/configuration.py
+-rw-r--r--   0        0        0     5433 2024-05-27 23:24:34.906969 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/exceptions.py
+-rw-r--r--   0        0        0     5651 2024-05-27 23:24:34.954970 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/__init__.py
+-rw-r--r--   0        0        0      819 2024-05-27 23:24:35.010970 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/asset_file_type.py
+-rw-r--r--   0        0        0      931 2024-05-27 23:24:35.042971 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/asset_type.py
+-rw-r--r--   0        0        0      809 2024-05-27 23:24:35.094971 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/calibration_master_type.py
+-rw-r--r--   0        0        0     2092 2024-05-27 23:24:35.150972 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/daily_weather_city.py
+-rw-r--r--   0        0        0     4308 2024-05-27 23:24:35.242973 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/daily_weather_forecast_item.py
+-rw-r--r--   0        0        0     2527 2024-05-27 23:24:35.286974 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/daily_weather_forecast_item_temp.py
+-rw-r--r--   0        0        0     2551 2024-05-27 23:24:35.334974 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/daily_weather_forecast_item_weather_inner.py
+-rw-r--r--   0        0        0     2947 2024-05-27 23:24:35.378975 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/daily_weather_forecast_list_response.py
+-rw-r--r--   0        0        0     1904 2024-05-27 23:24:35.422975 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/empty_success.py
+-rw-r--r--   0        0        0     1186 2024-05-27 23:24:35.478976 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/filter_type.py
+-rw-r--r--   0        0        0     1930 2024-05-27 23:24:35.526976 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/fits_header.py
+-rw-r--r--   0        0        0     2155 2024-05-27 23:24:35.574977 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/location.py
+-rw-r--r--   0        0        0      747 2024-05-27 23:24:35.642978 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/mount_type.py
+-rw-r--r--   0        0        0      887 2024-05-27 23:24:35.686978 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/node_state.py
+-rw-r--r--   0        0        0      827 2024-05-27 23:24:35.754979 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/optical_tube_type.py
+-rw-r--r--   0        0        0      751 2024-05-27 23:24:35.802980 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/shutter_type.py
+-rw-r--r--   0        0        0     1892 2024-05-27 23:24:35.846980 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/successful_create.py
+-rw-r--r--   0        0        0      768 2024-05-27 23:24:35.934981 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/tracking_type.py
+-rw-r--r--   0        0        0     3258 2024-05-27 23:24:35.986982 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_astro_project.py
+-rw-r--r--   0        0        0     3969 2024-05-27 23:24:36.034983 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_astro_project_asset.py
+-rw-r--r--   0        0        0     2569 2024-05-27 23:24:36.082983 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_astro_project_asset_metadata.py
+-rw-r--r--   0        0        0     2399 2024-05-27 23:24:36.142984 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_astro_project_asset_metadata_color_combination.py
+-rw-r--r--   0        0        0     2381 2024-05-27 23:24:36.194984 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_astro_target.py
+-rw-r--r--   0        0        0     3640 2024-05-27 23:24:36.238985 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_calibration_master.py
+-rw-r--r--   0        0        0     4908 2024-05-27 23:24:36.290985 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_camera.py
+-rw-r--r--   0        0        0     2421 2024-05-27 23:24:36.338986 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_create_astro_project_image_set_request.py
+-rw-r--r--   0        0        0     2668 2024-05-27 23:24:36.402987 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_create_astro_project_request.py
+-rw-r--r--   0        0        0     2121 2024-05-27 23:24:36.446987 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_create_astro_project_response.py
+-rw-r--r--   0        0        0     3777 2024-05-27 23:24:36.486988 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_create_calibration_master_request.py
+-rw-r--r--   0        0        0     2147 2024-05-27 23:24:36.546989 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_create_calibration_master_response.py
+-rw-r--r--   0        0        0     7059 2024-05-27 23:24:36.598989 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_create_camera_request.py
+-rw-r--r--   0        0        0     2044 2024-05-27 23:24:36.638990 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_create_image_set_image_request.py
+-rw-r--r--   0        0        0     2115 2024-05-27 23:24:36.682990 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_create_image_set_image_response.py
+-rw-r--r--   0        0        0     2683 2024-05-27 23:24:36.746991 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_create_image_set_request.py
+-rw-r--r--   0        0        0     2296 2024-05-27 23:24:36.794992 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_create_mount_request.py
+-rw-r--r--   0        0        0     3146 2024-05-27 23:24:36.846992 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_create_node_request.py
+-rw-r--r--   0        0        0     2447 2024-05-27 23:24:36.894993 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_create_optical_tube_request.py
+-rw-r--r--   0        0        0     2441 2024-05-27 23:24:36.938993 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_elevation_mask_point.py
+-rw-r--r--   0        0        0     3289 2024-05-27 23:24:37.014994 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_gain_curve.py
+-rw-r--r--   0        0        0     2051 2024-05-27 23:24:37.054995 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_gain_curve_point.py
+-rw-r--r--   0        0        0     2096 2024-05-27 23:24:37.106995 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_get_astro_platform_credit_balance_response.py
+-rw-r--r--   0        0        0     2364 2024-05-27 23:24:37.142996 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_get_nodes.py
+-rw-r--r--   0        0        0     7066 2024-05-27 23:24:37.194996 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_get_or_create_camera_request.py
+-rw-r--r--   0        0        0     2324 2024-05-27 23:24:37.238997 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_get_or_create_mount_request.py
+-rw-r--r--   0        0        0     2513 2024-05-27 23:24:37.282997 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_get_or_create_optical_tube_request.py
+-rw-r--r--   0        0        0     3436 2024-05-27 23:24:37.326998 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_image_set.py
+-rw-r--r--   0        0        0     5797 2024-05-27 23:24:37.374998 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_image_set_image.py
+-rw-r--r--   0        0        0      795 2024-05-27 23:24:37.418999 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_job_kind.py
+-rw-r--r--   0        0        0     2632 2024-05-27 23:24:37.455000 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_job_log.py
+-rw-r--r--   0        0        0      803 2024-05-27 23:24:37.531000 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_job_status.py
+-rw-r--r--   0        0        0     1914 2024-05-27 23:24:37.575001 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_mount.py
+-rw-r--r--   0        0        0     4458 2024-05-27 23:24:37.667002 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_node.py
+-rw-r--r--   0        0        0     2564 2024-05-27 23:24:37.719003 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_node_with_location.py
+-rw-r--r--   0        0        0     2239 2024-05-27 23:24:37.779003 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_optical_tube.py
+-rw-r--r--   0        0        0     3057 2024-05-27 23:24:37.843004 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_platform_credit.py
+-rw-r--r--   0        0        0      870 2024-05-27 23:24:37.879005 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_platform_credit_source.py
+-rw-r--r--   0        0        0      800 2024-05-27 23:24:37.923005 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_platform_credit_type.py
+-rw-r--r--   0        0        0      776 2024-05-27 23:24:37.967006 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_platform_credit_unit.py
+-rw-r--r--   0        0        0     2045 2024-05-27 23:24:38.023006 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_put_stack_astro_project_request.py
+-rw-r--r--   0        0        0     2051 2024-05-27 23:24:38.067007 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_read_noise_point.py
+-rw-r--r--   0        0        0     2050 2024-05-27 23:24:38.111007 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_setup_action.py
+-rw-r--r--   0        0        0     2940 2024-05-27 23:24:38.159008 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_slew_timing.py
+-rw-r--r--   0        0        0     2240 2024-05-27 23:24:38.211009 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_slew_timing_interval.py
+-rw-r--r--   0        0        0     4605 2024-05-27 23:24:38.267009 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_update_node_request.py
+-rw-r--r--   0        0        0     2522 2024-05-27 23:24:38.323010 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_video_mode_framerate_property.py
+-rw-r--r--   0        0        0        0 2024-05-27 23:24:38.379011 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/py.typed
+-rw-r--r--   0        0        0    12935 2024-05-27 23:24:38.415011 ourskyai_astro_api-1.3.3678/ourskyai_astro_api/rest.py
+-rw-r--r--   0        0        0      739 2024-05-27 23:24:38.479012 ourskyai_astro_api-1.3.3678/pyproject.toml
+-rw-r--r--   0        0        0    12509 1970-01-01 00:00:00.000000 ourskyai_astro_api-1.3.3678/PKG-INFO
```

### Comparing `ourskyai_astro_api-1.3.3676/README.md` & `ourskyai_astro_api-1.3.3678/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ourskyai-astro-api
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

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/__init__.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 # flake8: noqa
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "1.3.3676"
+__version__ = "1.3.3678"
 
 # import apis into sdk package
 from ourskyai_astro_api.api.default_api import DefaultApi
 
 # import ApiClient
 from ourskyai_astro_api.api_response import ApiResponse
 from ourskyai_astro_api.api_client import ApiClient
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/api/default_api.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/api/default_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import re  # noqa: F401
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/api_client.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
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

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/api_response.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/api_response.py`

 * *Files identical despite different names*

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/configuration.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
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

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/exceptions.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 class OpenApiException(Exception):
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/__init__.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 # import models into model package
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/asset_file_type.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/asset_file_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/asset_type.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/asset_type.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/calibration_master_type.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/calibration_master_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/daily_weather_city.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/daily_weather_city.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/daily_weather_forecast_item.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/daily_weather_forecast_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/daily_weather_forecast_item_temp.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/daily_weather_forecast_item_temp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/daily_weather_forecast_item_weather_inner.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/daily_weather_forecast_item_weather_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/daily_weather_forecast_list_response.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/daily_weather_forecast_list_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/empty_success.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/empty_success.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/filter_type.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/filter_type.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/fits_header.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/fits_header.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/location.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/location.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/mount_type.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/mount_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/node_state.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/node_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/optical_tube_type.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/optical_tube_type.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/shutter_type.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/shutter_type.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/successful_create.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/successful_create.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/tracking_type.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/tracking_type.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_astro_project.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_astro_project.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_astro_project_asset.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_astro_project_asset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_astro_project_asset_metadata.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_astro_project_asset_metadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_astro_project_asset_metadata_color_combination.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_astro_project_asset_metadata_color_combination.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_astro_target.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_astro_target.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_calibration_master.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_calibration_master.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_camera.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_camera.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_create_astro_project_image_set_request.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_create_astro_project_image_set_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_create_astro_project_request.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_create_astro_project_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_create_astro_project_response.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_create_astro_project_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_create_calibration_master_request.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_create_calibration_master_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_create_calibration_master_response.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_create_calibration_master_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_create_camera_request.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_create_camera_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_create_image_set_image_request.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_create_image_set_image_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_create_image_set_image_response.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_create_image_set_image_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_create_image_set_request.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_create_image_set_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_create_mount_request.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_create_mount_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_create_node_request.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_create_node_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_create_optical_tube_request.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_create_optical_tube_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_elevation_mask_point.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_elevation_mask_point.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_gain_curve.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_gain_curve.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_gain_curve_point.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_gain_curve_point.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_get_astro_platform_credit_balance_response.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_get_astro_platform_credit_balance_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_get_nodes.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_get_nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_get_or_create_camera_request.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_get_or_create_camera_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_get_or_create_mount_request.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_get_or_create_mount_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_get_or_create_optical_tube_request.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_get_or_create_optical_tube_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_image_set.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_image_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_image_set_image.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_image_set_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_job_kind.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_job_kind.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_job_log.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_job_log.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_job_status.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_job_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_mount.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_mount.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_node.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_node_with_location.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_node_with_location.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_optical_tube.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_optical_tube.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_platform_credit.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_platform_credit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_platform_credit_source.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_platform_credit_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_platform_credit_type.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_platform_credit_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_platform_credit_unit.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_platform_credit_unit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_put_stack_astro_project_request.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_put_stack_astro_project_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_read_noise_point.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_read_noise_point.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_setup_action.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_setup_action.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_slew_timing.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_slew_timing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_slew_timing_interval.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_slew_timing_interval.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_update_node_request.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_update_node_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/models/v1_video_mode_framerate_property.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/models/v1_video_mode_framerate_property.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3676/ourskyai_astro_api/rest.py` & `ourskyai_astro_api-1.3.3678/ourskyai_astro_api/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3676
+    The version of the OpenAPI document: 1.3.3678
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
```

### Comparing `ourskyai_astro_api-1.3.3676/pyproject.toml` & `ourskyai_astro_api-1.3.3678/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ourskyai_astro_api"
-version = "1.3.3676"
+version = "1.3.3678"
 description = "OurSky Astro"
 authors = ["OpenAPI Generator Community <team@openapitools.org>"]
 license = "NoLicense"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "OurSky Astro"]
 include = ["ourskyai_astro_api/py.typed"]
```

### Comparing `ourskyai_astro_api-1.3.3676/PKG-INFO` & `ourskyai_astro_api-1.3.3678/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ourskyai_astro_api
-Version: 1.3.3676
+Version: 1.3.3678
 Summary: OurSky Astro
 Home-page: https://github.com/GIT_USER_ID/GIT_REPO_ID
 License: NoLicense
 Keywords: OpenAPI,OpenAPI-Generator,OurSky Astro
 Author: OpenAPI Generator Community
 Author-email: team@openapitools.org
 Requires-Python: >=3.7,<4.0
@@ -24,16 +24,16 @@
 Description-Content-Type: text/markdown
 
 # ourskyai-astro-api
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

