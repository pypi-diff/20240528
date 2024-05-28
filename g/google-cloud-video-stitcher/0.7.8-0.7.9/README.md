# Comparing `tmp/google-cloud-video-stitcher-0.7.8.tar.gz` & `tmp/google-cloud-video-stitcher-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-video-stitcher-0.7.8.tar", last modified: Thu Feb 22 22:44:39 2024, max compression
+gzip compressed data, was "google-cloud-video-stitcher-0.7.9.tar", last modified: Tue Mar  5 19:00:26 2024, max compression
```

## Comparing `google-cloud-video-stitcher-0.7.8.tar` & `google-cloud-video-stitcher-0.7.9.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-sr-x   0 root         (0)     1003        0 2024-02-22 22:44:39.893138 google-cloud-video-stitcher-0.7.8/
--rw-rw-r--   0 root         (0)     1003    11358 2024-02-22 22:27:49.000000 google-cloud-video-stitcher-0.7.8/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2024-02-22 22:27:49.000000 google-cloud-video-stitcher-0.7.8/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     5290 2024-02-22 22:44:39.893138 google-cloud-video-stitcher-0.7.8/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3923 2024-02-22 22:27:49.000000 google-cloud-video-stitcher-0.7.8/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2024-02-22 22:44:39.881137 google-cloud-video-stitcher-0.7.8/google/
-drwxr-sr-x   0 root         (0)     1003        0 2024-02-22 22:44:39.881137 google-cloud-video-stitcher-0.7.8/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2024-02-22 22:44:39.881137 google-cloud-video-stitcher-0.7.8/google/cloud/video/
-drwxr-sr-x   0 root         (0)     1003        0 2024-02-22 22:44:39.885137 google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher/
--rw-rw-r--   0 root         (0)     1003     4591 2024-02-22 22:27:49.000000 google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2024-02-22 22:27:49.000000 google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       88 2024-02-22 22:27:49.000000 google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-02-22 22:44:39.885137 google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher_v1/
--rw-rw-r--   0 root         (0)     1003     4140 2024-02-22 22:27:49.000000 google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     6599 2024-02-22 22:27:49.000000 google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2024-02-22 22:27:49.000000 google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       88 2024-02-22 22:27:49.000000 google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-02-22 22:44:39.885137 google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2024-02-22 22:27:49.000000 google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-02-22 22:44:39.885137 google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher_v1/services/video_stitcher_service/
--rw-rw-r--   0 root         (0)     1003      793 2024-02-22 22:27:49.000000 google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher_v1/services/video_stitcher_service/__init__.py
--rw-rw-r--   0 root         (0)     1003   139710 2024-02-22 22:27:49.000000 google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher_v1/services/video_stitcher_service/async_client.py
--rw-rw-r--   0 root         (0)     1003   163861 2024-02-22 22:27:49.000000 google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher_v1/services/video_stitcher_service/client.py
--rw-rw-r--   0 root         (0)     1003    32467 2024-02-22 22:27:49.000000 google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher_v1/services/video_stitcher_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-02-22 22:44:39.889137 google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/
--rw-rw-r--   0 root         (0)     1003     1255 2024-02-22 22:27:49.000000 google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    18187 2024-02-22 22:27:49.000000 google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    43878 2024-02-22 22:27:49.000000 google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    44754 2024-02-22 22:27:49.000000 google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   110180 2024-02-22 22:27:49.000000 google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-02-22 22:44:39.889137 google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher_v1/types/
--rw-rw-r--   0 root         (0)     1003     3774 2024-02-22 22:27:49.000000 google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     4946 2024-02-22 22:27:49.000000 google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher_v1/types/ad_tag_details.py
--rw-rw-r--   0 root         (0)     1003     4222 2024-02-22 22:27:49.000000 google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher_v1/types/cdn_keys.py
--rw-rw-r--   0 root         (0)     1003     6930 2024-02-22 22:27:49.000000 google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher_v1/types/companions.py
--rw-rw-r--   0 root         (0)     1003     5153 2024-02-22 22:27:49.000000 google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher_v1/types/events.py
--rw-rw-r--   0 root         (0)     1003     7320 2024-02-22 22:27:49.000000 google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher_v1/types/live_configs.py
--rw-rw-r--   0 root         (0)     1003    13090 2024-02-22 22:27:49.000000 google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher_v1/types/sessions.py
--rw-rw-r--   0 root         (0)     1003     2314 2024-02-22 22:27:49.000000 google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher_v1/types/slates.py
--rw-rw-r--   0 root         (0)     1003     3156 2024-02-22 22:27:49.000000 google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher_v1/types/stitch_details.py
--rw-rw-r--   0 root         (0)     1003    26457 2024-02-22 22:27:49.000000 google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher_v1/types/video_stitcher_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-02-22 22:44:39.893138 google-cloud-video-stitcher-0.7.8/google_cloud_video_stitcher.egg-info/
--rw-r--r--   0 root         (0)     1003     5290 2024-02-22 22:44:39.000000 google-cloud-video-stitcher-0.7.8/google_cloud_video_stitcher.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     2120 2024-02-22 22:44:39.000000 google-cloud-video-stitcher-0.7.8/google_cloud_video_stitcher.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2024-02-22 22:44:39.000000 google-cloud-video-stitcher-0.7.8/google_cloud_video_stitcher.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003        1 2024-02-22 22:44:39.000000 google-cloud-video-stitcher-0.7.8/google_cloud_video_stitcher.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      287 2024-02-22 22:44:39.000000 google-cloud-video-stitcher-0.7.8/google_cloud_video_stitcher.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2024-02-22 22:44:39.000000 google-cloud-video-stitcher-0.7.8/google_cloud_video_stitcher.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2024-02-22 22:44:39.893138 google-cloud-video-stitcher-0.7.8/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3053 2024-02-22 22:27:49.000000 google-cloud-video-stitcher-0.7.8/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-02-22 22:44:39.893138 google-cloud-video-stitcher-0.7.8/tests/
--rw-rw-r--   0 root         (0)     1003      600 2024-02-22 22:27:49.000000 google-cloud-video-stitcher-0.7.8/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-02-22 22:44:39.893138 google-cloud-video-stitcher-0.7.8/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2024-02-22 22:27:49.000000 google-cloud-video-stitcher-0.7.8/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-02-22 22:44:39.893138 google-cloud-video-stitcher-0.7.8/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2024-02-22 22:27:49.000000 google-cloud-video-stitcher-0.7.8/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-02-22 22:44:39.893138 google-cloud-video-stitcher-0.7.8/tests/unit/gapic/stitcher_v1/
--rw-rw-r--   0 root         (0)     1003      600 2024-02-22 22:27:49.000000 google-cloud-video-stitcher-0.7.8/tests/unit/gapic/stitcher_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   354820 2024-02-22 22:27:49.000000 google-cloud-video-stitcher-0.7.8/tests/unit/gapic/stitcher_v1/test_video_stitcher_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:00:26.470103 google-cloud-video-stitcher-0.7.9/
+-rw-rw-r--   0 root         (0)     1003    11358 2024-03-05 18:46:03.000000 google-cloud-video-stitcher-0.7.9/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2024-03-05 18:46:03.000000 google-cloud-video-stitcher-0.7.9/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     5308 2024-03-05 19:00:26.470103 google-cloud-video-stitcher-0.7.9/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3923 2024-03-05 18:46:03.000000 google-cloud-video-stitcher-0.7.9/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:00:26.458102 google-cloud-video-stitcher-0.7.9/google/
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:00:26.458102 google-cloud-video-stitcher-0.7.9/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:00:26.458102 google-cloud-video-stitcher-0.7.9/google/cloud/video/
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:00:26.462102 google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher/
+-rw-rw-r--   0 root         (0)     1003     4591 2024-03-05 18:46:03.000000 google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2024-03-05 18:46:03.000000 google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       88 2024-03-05 18:46:03.000000 google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:00:26.462102 google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher_v1/
+-rw-rw-r--   0 root         (0)     1003     4140 2024-03-05 18:46:03.000000 google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6599 2024-03-05 18:46:03.000000 google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2024-03-05 18:46:03.000000 google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       88 2024-03-05 18:46:03.000000 google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:00:26.462102 google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:03.000000 google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:00:26.462102 google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher_v1/services/video_stitcher_service/
+-rw-rw-r--   0 root         (0)     1003      793 2024-03-05 18:46:03.000000 google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher_v1/services/video_stitcher_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003   139710 2024-03-05 18:46:03.000000 google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher_v1/services/video_stitcher_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003   163861 2024-03-05 18:46:03.000000 google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher_v1/services/video_stitcher_service/client.py
+-rw-rw-r--   0 root         (0)     1003    32467 2024-03-05 18:46:03.000000 google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher_v1/services/video_stitcher_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:00:26.466102 google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1255 2024-03-05 18:46:03.000000 google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    18187 2024-03-05 18:46:03.000000 google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    43878 2024-03-05 18:46:03.000000 google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    44754 2024-03-05 18:46:03.000000 google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   110180 2024-03-05 18:46:03.000000 google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:00:26.466102 google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher_v1/types/
+-rw-rw-r--   0 root         (0)     1003     3774 2024-03-05 18:46:03.000000 google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4946 2024-03-05 18:46:03.000000 google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher_v1/types/ad_tag_details.py
+-rw-rw-r--   0 root         (0)     1003     4222 2024-03-05 18:46:03.000000 google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher_v1/types/cdn_keys.py
+-rw-rw-r--   0 root         (0)     1003     6930 2024-03-05 18:46:03.000000 google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher_v1/types/companions.py
+-rw-rw-r--   0 root         (0)     1003     5153 2024-03-05 18:46:03.000000 google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher_v1/types/events.py
+-rw-rw-r--   0 root         (0)     1003     7320 2024-03-05 18:46:03.000000 google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher_v1/types/live_configs.py
+-rw-rw-r--   0 root         (0)     1003    13090 2024-03-05 18:46:03.000000 google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher_v1/types/sessions.py
+-rw-rw-r--   0 root         (0)     1003     2314 2024-03-05 18:46:03.000000 google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher_v1/types/slates.py
+-rw-rw-r--   0 root         (0)     1003     3156 2024-03-05 18:46:03.000000 google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher_v1/types/stitch_details.py
+-rw-rw-r--   0 root         (0)     1003    26457 2024-03-05 18:46:03.000000 google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher_v1/types/video_stitcher_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:00:26.470103 google-cloud-video-stitcher-0.7.9/google_cloud_video_stitcher.egg-info/
+-rw-r--r--   0 root         (0)     1003     5308 2024-03-05 19:00:26.000000 google-cloud-video-stitcher-0.7.9/google_cloud_video_stitcher.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     2120 2024-03-05 19:00:26.000000 google-cloud-video-stitcher-0.7.9/google_cloud_video_stitcher.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-03-05 19:00:26.000000 google-cloud-video-stitcher-0.7.9/google_cloud_video_stitcher.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-03-05 19:00:26.000000 google-cloud-video-stitcher-0.7.9/google_cloud_video_stitcher.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      305 2024-03-05 19:00:26.000000 google-cloud-video-stitcher-0.7.9/google_cloud_video_stitcher.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2024-03-05 19:00:26.000000 google-cloud-video-stitcher-0.7.9/google_cloud_video_stitcher.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2024-03-05 19:00:26.470103 google-cloud-video-stitcher-0.7.9/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3197 2024-03-05 18:46:03.000000 google-cloud-video-stitcher-0.7.9/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:00:26.470103 google-cloud-video-stitcher-0.7.9/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:03.000000 google-cloud-video-stitcher-0.7.9/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:00:26.470103 google-cloud-video-stitcher-0.7.9/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:03.000000 google-cloud-video-stitcher-0.7.9/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:00:26.470103 google-cloud-video-stitcher-0.7.9/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:03.000000 google-cloud-video-stitcher-0.7.9/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:00:26.470103 google-cloud-video-stitcher-0.7.9/tests/unit/gapic/stitcher_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:03.000000 google-cloud-video-stitcher-0.7.9/tests/unit/gapic/stitcher_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   354820 2024-03-05 18:46:03.000000 google-cloud-video-stitcher-0.7.9/tests/unit/gapic/stitcher_v1/test_video_stitcher_service.py
```

### Comparing `google-cloud-video-stitcher-0.7.8/LICENSE` & `google-cloud-video-stitcher-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.8/MANIFEST.in` & `google-cloud-video-stitcher-0.7.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.8/PKG-INFO` & `google-cloud-video-stitcher-0.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-video-stitcher
-Version: 0.7.8
+Version: 0.7.9
 Summary: Google Cloud Video Stitcher API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-video-stitcher
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
 Requires-Python: >=3.7
 License-File: LICENSE
 Requires-Dist: google-api-core[grpc]!=2.0.*,!=2.1.*,!=2.10.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,<3.0.0dev,>=1.34.1
-Requires-Dist: google-auth<3.0.0dev,>=2.14.1
+Requires-Dist: google-auth!=2.24.0,!=2.25.0,<3.0.0dev,>=2.14.1
 Requires-Dist: proto-plus<2.0.0dev,>=1.22.3
 Requires-Dist: protobuf!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5,<5.0.0dev,>=3.19.5
 
 Python Client for Video Stitcher
 ================================
 
 |preview| |pypi| |versions|
```

### Comparing `google-cloud-video-stitcher-0.7.8/README.rst` & `google-cloud-video-stitcher-0.7.9/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher/__init__.py` & `google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher/gapic_version.py` & `google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.7.8"  # {x-release-please-version}
+__version__ = "0.7.9"  # {x-release-please-version}
```

### Comparing `google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher_v1/__init__.py` & `google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher_v1/gapic_metadata.json` & `google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher_v1/gapic_version.py` & `google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher_v1/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.7.8"  # {x-release-please-version}
+__version__ = "0.7.9"  # {x-release-please-version}
```

### Comparing `google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher_v1/services/__init__.py` & `google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher_v1/services/video_stitcher_service/__init__.py` & `google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher_v1/services/video_stitcher_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher_v1/services/video_stitcher_service/async_client.py` & `google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher_v1/services/video_stitcher_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher_v1/services/video_stitcher_service/client.py` & `google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher_v1/services/video_stitcher_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher_v1/services/video_stitcher_service/pagers.py` & `google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher_v1/services/video_stitcher_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/__init__.py` & `google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/base.py` & `google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/grpc.py` & `google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/grpc_asyncio.py` & `google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/rest.py` & `google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher_v1/services/video_stitcher_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher_v1/types/__init__.py` & `google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher_v1/types/ad_tag_details.py` & `google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher_v1/types/ad_tag_details.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher_v1/types/cdn_keys.py` & `google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher_v1/types/cdn_keys.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher_v1/types/companions.py` & `google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher_v1/types/companions.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher_v1/types/events.py` & `google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher_v1/types/events.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher_v1/types/live_configs.py` & `google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher_v1/types/live_configs.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher_v1/types/sessions.py` & `google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher_v1/types/sessions.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher_v1/types/slates.py` & `google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher_v1/types/slates.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher_v1/types/stitch_details.py` & `google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher_v1/types/stitch_details.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.8/google/cloud/video/stitcher_v1/types/video_stitcher_service.py` & `google-cloud-video-stitcher-0.7.9/google/cloud/video/stitcher_v1/types/video_stitcher_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.8/google_cloud_video_stitcher.egg-info/PKG-INFO` & `google-cloud-video-stitcher-0.7.9/google_cloud_video_stitcher.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-video-stitcher
-Version: 0.7.8
+Version: 0.7.9
 Summary: Google Cloud Video Stitcher API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-video-stitcher
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
 Requires-Python: >=3.7
 License-File: LICENSE
 Requires-Dist: google-api-core[grpc]!=2.0.*,!=2.1.*,!=2.10.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,<3.0.0dev,>=1.34.1
-Requires-Dist: google-auth<3.0.0dev,>=2.14.1
+Requires-Dist: google-auth!=2.24.0,!=2.25.0,<3.0.0dev,>=2.14.1
 Requires-Dist: proto-plus<2.0.0dev,>=1.22.3
 Requires-Dist: protobuf!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5,<5.0.0dev,>=3.19.5
 
 Python Client for Video Stitcher
 ================================
 
 |preview| |pypi| |versions|
```

### Comparing `google-cloud-video-stitcher-0.7.8/google_cloud_video_stitcher.egg-info/SOURCES.txt` & `google-cloud-video-stitcher-0.7.9/google_cloud_video_stitcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.8/setup.py` & `google-cloud-video-stitcher-0.7.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,17 @@
 if version[0] == "0":
     release_status = "Development Status :: 4 - Beta"
 else:
     release_status = "Development Status :: 5 - Production/Stable"
 
 dependencies = [
     "google-api-core[grpc] >= 1.34.1, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
-    "google-auth >= 2.14.1, <3.0.0dev",
+    # Exclude incompatible versions of `google-auth`
+    # See https://github.com/googleapis/google-cloud-python/issues/12364
+    "google-auth >= 2.14.1, <3.0.0dev,!=2.24.0,!=2.25.0",
     "proto-plus >= 1.22.3, <2.0.0dev",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
 ]
 url = "https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-video-stitcher"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
```

### Comparing `google-cloud-video-stitcher-0.7.8/tests/__init__.py` & `google-cloud-video-stitcher-0.7.9/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.8/tests/unit/__init__.py` & `google-cloud-video-stitcher-0.7.9/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.8/tests/unit/gapic/__init__.py` & `google-cloud-video-stitcher-0.7.9/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.8/tests/unit/gapic/stitcher_v1/__init__.py` & `google-cloud-video-stitcher-0.7.9/tests/unit/gapic/stitcher_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-video-stitcher-0.7.8/tests/unit/gapic/stitcher_v1/test_video_stitcher_service.py` & `google-cloud-video-stitcher-0.7.9/tests/unit/gapic/stitcher_v1/test_video_stitcher_service.py`

 * *Files identical despite different names*

